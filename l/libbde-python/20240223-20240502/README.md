# Comparing `tmp/libbde-python-20240223.tar.gz` & `tmp/libbde-python-20240502.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libbde-python-20240223.tar", last modified: Fri Feb 23 03:42:00 2024, max compression
+gzip compressed data, was "libbde-python-20240502.tar", last modified: Thu May  2 04:50:32 2024, max compression
```

## Comparing `libbde-python-20240223.tar` & `libbde-python-20240502.tar`

### file list

```diff
@@ -1,926 +1,926 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/bdetools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37141 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/mount_dokan.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2979 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/mount_file_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1775 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/bdetools_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26427 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/mount_fuse.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4012 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/bdetools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4005 2024-02-23 02:48:27.000000 libbde-20240223/bdetools/info_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5411 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/mount_dokan.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/bdetools_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1458 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/bdetools_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/bdetools_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1306 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/bdetools_input.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18932 2024-02-23 02:48:27.000000 libbde-20240223/bdetools/mount_file_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/bdetools_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1498 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/bdetools_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11853 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/byte_size_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2471 2023-12-03 08:57:23.000000 libbde-20240223/bdetools/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1421 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/bdetools_output.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5701 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/bdetools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21702 2024-02-23 02:48:27.000000 libbde-20240223/bdetools/mount_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44113 2024-02-23 02:48:27.000000 libbde-20240223/bdetools/info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3611 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/mount_file_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/bdetools_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/bdetools_libbde.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/bdetools_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8762 2024-02-23 02:48:27.000000 libbde-20240223/bdetools/bdeinfo.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1207 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/bdetools_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4132 2024-02-23 02:48:27.000000 libbde-20240223/bdetools/mount_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6306 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/bdetools_input.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1765 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/bdetools_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34112 2024-02-23 02:48:27.000000 libbde-20240223/bdetools/mount_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1477 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/bdetools_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1437 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/bdetools_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1403 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/bdetools_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35440 2024-02-23 03:03:50.000000 libbde-20240223/bdetools/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1737 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/bdetools_signal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4527 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/bdetools_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1988 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/byte_size_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18120 2024-02-23 02:48:27.000000 libbde-20240223/bdetools/bdemount.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2759 2024-02-23 02:47:19.000000 libbde-20240223/bdetools/mount_fuse.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-02-23 02:47:17.000000 libbde-20240223/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-02-23 03:03:50.000000 libbde-20240223/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 02:47:17.000000 libbde-20240223/NEWS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-02-23 03:03:51.000000 libbde-20240223/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/pybde/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2076 2024-02-23 02:47:19.000000 libbde-20240223/pybde/pybde_key_protector.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4698 2024-02-23 02:48:27.000000 libbde-20240223/pybde/pybde_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8840 2024-02-23 02:47:19.000000 libbde-20240223/pybde/pybde_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2027 2024-02-23 02:47:19.000000 libbde-20240223/pybde/pybde_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-02-23 02:47:19.000000 libbde-20240223/pybde/pybde_libbde.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4042 2024-02-23 02:47:19.000000 libbde-20240223/pybde/pybde_file_object_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1842 2024-02-23 02:47:19.000000 libbde-20240223/pybde/pybde.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1526 2024-02-23 02:47:19.000000 libbde-20240223/pybde/pybde_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2842 2024-02-23 02:47:19.000000 libbde-20240223/pybde/pybde_guid.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9506 2024-02-23 02:47:19.000000 libbde-20240223/pybde/pybde_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7138 2024-02-23 02:47:19.000000 libbde-20240223/pybde/pybde_encryption_methods.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-02-23 02:47:19.000000 libbde-20240223/pybde/pybde_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1374 2023-12-03 08:57:20.000000 libbde-20240223/pybde/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1519 2024-02-23 02:47:19.000000 libbde-20240223/pybde/pybde_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1352 2024-02-23 02:47:19.000000 libbde-20240223/pybde/pybde_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66046 2024-02-23 02:48:27.000000 libbde-20240223/pybde/pybde_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8869 2024-02-23 02:47:19.000000 libbde-20240223/pybde/pybde_key_protector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16024 2024-02-23 02:48:27.000000 libbde-20240223/pybde/pybde.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7137 2024-02-23 02:47:19.000000 libbde-20240223/pybde/pybde_key_protection_types.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16577 2024-02-23 02:47:19.000000 libbde-20240223/pybde/pybde_datetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-02-23 02:47:19.000000 libbde-20240223/pybde/pybde_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33702 2024-02-23 02:47:19.000000 libbde-20240223/pybde/pybde_file_object_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2024-02-23 02:47:19.000000 libbde-20240223/pybde/pybde_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2483 2024-02-23 02:47:19.000000 libbde-20240223/pybde/pybde_key_protectors.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1384 2024-02-23 02:47:19.000000 libbde-20240223/pybde/pybde_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9493 2024-02-23 02:47:19.000000 libbde-20240223/pybde/pybde_key_protectors.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49155 2024-02-23 03:03:51.000000 libbde-20240223/pybde/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1698 2024-02-23 02:47:19.000000 libbde-20240223/pybde/pybde_encryption_methods.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1726 2024-02-23 02:47:19.000000 libbde-20240223/pybde/pybde_key_protection_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1804 2024-02-23 02:47:19.000000 libbde-20240223/pybde/pybde_datetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1165 2024-02-23 02:47:19.000000 libbde-20240223/pybde/pybde_guid.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:58.000000 libbde-20240223/libcaes/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-23 03:03:23.000000 libbde-20240223/libcaes/libcaes_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2885 2024-02-23 03:03:23.000000 libbde-20240223/libcaes/libcaes_tweaked_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4464 2024-02-23 03:03:23.000000 libbde-20240223/libcaes/libcaes_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-23 03:03:23.000000 libbde-20240223/libcaes/libcaes_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82616 2024-02-23 03:03:23.000000 libbde-20240223/libcaes/libcaes_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1743 2024-02-23 03:03:23.000000 libbde-20240223/libcaes/libcaes_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-02-23 03:03:23.000000 libbde-20240223/libcaes/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-23 03:03:23.000000 libbde-20240223/libcaes/libcaes_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1608 2024-02-23 03:03:23.000000 libbde-20240223/libcaes/libcaes_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-23 03:03:23.000000 libbde-20240223/libcaes/libcaes_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-02-23 03:03:23.000000 libbde-20240223/libcaes/libcaes_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-23 03:03:23.000000 libbde-20240223/libcaes/libcaes_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-02-23 03:03:23.000000 libbde-20240223/libcaes/libcaes_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30517 2024-02-23 03:03:50.000000 libbde-20240223/libcaes/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33103 2024-02-23 03:03:23.000000 libbde-20240223/libcaes/libcaes_tweaked_context.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:58.000000 libbde-20240223/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-23 03:03:36.000000 libbde-20240223/libfguid/libfguid_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-02-23 03:03:36.000000 libbde-20240223/libfguid/libfguid_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-02-23 03:03:36.000000 libbde-20240223/libfguid/libfguid_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-23 03:03:36.000000 libbde-20240223/libfguid/libfguid_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      681 2024-02-23 03:03:36.000000 libbde-20240223/libfguid/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-23 03:03:36.000000 libbde-20240223/libfguid/libfguid_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-23 03:03:36.000000 libbde-20240223/libfguid/libfguid_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-02-23 03:03:36.000000 libbde-20240223/libfguid/libfguid_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-02-23 03:03:36.000000 libbde-20240223/libfguid/libfguid_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-02-23 03:03:36.000000 libbde-20240223/libfguid/libfguid_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-02-23 03:03:36.000000 libbde-20240223/libfguid/libfguid_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30259 2024-02-23 03:03:50.000000 libbde-20240223/libfguid/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-23 03:03:36.000000 libbde-20240223/libfguid/libfguid_error.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:57.000000 libbde-20240223/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2023-12-03 08:57:23.000000 libbde-20240223/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18233 2023-12-03 08:57:23.000000 libbde-20240223/m4/libfdatetime.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 08:57:23.000000 libbde-20240223/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2023-12-03 08:57:23.000000 libbde-20240223/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 08:57:24.000000 libbde-20240223/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 08:57:24.000000 libbde-20240223/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31269 2023-12-03 08:57:23.000000 libbde-20240223/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 08:57:24.000000 libbde-20240223/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 08:57:24.000000 libbde-20240223/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2023-12-03 08:57:23.000000 libbde-20240223/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-12-03 08:57:23.000000 libbde-20240223/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2023-12-03 08:57:23.000000 libbde-20240223/m4/libcsplit.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 08:57:23.000000 libbde-20240223/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-12-03 08:57:23.000000 libbde-20240223/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-02-23 03:03:45.000000 libbde-20240223/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-02-23 03:03:45.000000 libbde-20240223/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 08:57:24.000000 libbde-20240223/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5232 2023-12-03 08:57:23.000000 libbde-20240223/m4/libfuse.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-02-23 03:03:45.000000 libbde-20240223/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 08:57:24.000000 libbde-20240223/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 08:57:23.000000 libbde-20240223/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-12-03 08:57:23.000000 libbde-20240223/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2023-12-03 08:57:23.000000 libbde-20240223/m4/libfguid.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2023-12-03 08:57:23.000000 libbde-20240223/m4/libbfio.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8319 2023-12-03 08:57:23.000000 libbde-20240223/m4/libhmac.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 08:57:24.000000 libbde-20240223/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-02-23 03:03:45.000000 libbde-20240223/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 08:57:24.000000 libbde-20240223/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 08:57:24.000000 libbde-20240223/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-02-23 03:03:45.000000 libbde-20240223/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 08:57:24.000000 libbde-20240223/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 08:57:23.000000 libbde-20240223/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27481 2023-12-03 08:57:23.000000 libbde-20240223/m4/libcrypto.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19791 2023-12-03 08:57:23.000000 libbde-20240223/m4/libfvalue.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 08:57:23.000000 libbde-20240223/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7325 2023-12-03 08:57:23.000000 libbde-20240223/m4/libfcache.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-12-03 08:57:23.000000 libbde-20240223/m4/pthread.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6269 2023-12-03 08:57:23.000000 libbde-20240223/m4/libcaes.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3509 2024-02-23 02:47:17.000000 libbde-20240223/libbde.spec.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:57.000000 libbde-20240223/include/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16052 2024-02-23 03:04:01.000000 libbde-20240223/include/libbde.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      444 2024-02-23 02:47:17.000000 libbde-20240223/include/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:57.000000 libbde-20240223/include/libbde/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2596 2024-02-23 02:47:18.000000 libbde-20240223/include/libbde/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2594 2024-02-23 03:04:01.000000 libbde-20240223/include/libbde/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4967 2024-02-23 02:47:18.000000 libbde-20240223/include/libbde/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4836 2024-02-23 03:04:01.000000 libbde-20240223/include/libbde/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-02-23 02:47:18.000000 libbde-20240223/include/libbde/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6622 2024-02-23 02:47:18.000000 libbde-20240223/include/libbde/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-23 02:47:18.000000 libbde-20240223/include/libbde/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-02-23 03:04:01.000000 libbde-20240223/include/libbde/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5078 2024-02-23 02:47:18.000000 libbde-20240223/include/libbde/codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28767 2024-02-23 03:03:50.000000 libbde-20240223/include/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16052 2024-02-23 02:47:18.000000 libbde-20240223/include/libbde.h.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:58.000000 libbde-20240223/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-02-23 02:47:18.000000 libbde-20240223/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-02-23 02:47:18.000000 libbde-20240223/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-02-23 02:47:18.000000 libbde-20240223/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-02-23 02:47:18.000000 libbde-20240223/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-02-23 02:47:18.000000 libbde-20240223/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-02-23 02:47:18.000000 libbde-20240223/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-02-23 02:47:18.000000 libbde-20240223/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-02-23 02:47:17.000000 libbde-20240223/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-02-23 02:47:18.000000 libbde-20240223/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7372 2024-02-23 03:04:01.000000 libbde-20240223/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19398 2024-02-23 03:03:50.000000 libbde-20240223/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20504 2024-02-23 03:04:01.000000 libbde-20240223/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-02-23 02:47:18.000000 libbde-20240223/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-02-23 02:47:18.000000 libbde-20240223/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-02-23 02:47:18.000000 libbde-20240223/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25812 2024-02-23 03:03:50.000000 libbde-20240223/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:58.000000 libbde-20240223/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-02-23 03:03:28.000000 libbde-20240223/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-02-23 03:03:28.000000 libbde-20240223/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2024-02-23 03:03:28.000000 libbde-20240223/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-02-23 03:03:28.000000 libbde-20240223/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-23 03:03:28.000000 libbde-20240223/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-02-23 03:03:28.000000 libbde-20240223/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-02-23 03:03:28.000000 libbde-20240223/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-02-23 03:03:28.000000 libbde-20240223/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-02-23 03:03:28.000000 libbde-20240223/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-02-23 03:03:28.000000 libbde-20240223/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30815 2024-02-23 03:03:50.000000 libbde-20240223/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-23 03:03:28.000000 libbde-20240223/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-02-23 03:03:28.000000 libbde-20240223/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-02-23 03:03:28.000000 libbde-20240223/libclocale/libclocale_codepage.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:58.000000 libbde-20240223/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-02-23 03:03:34.000000 libbde-20240223/libfcache/libfcache_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-02-23 03:03:34.000000 libbde-20240223/libfcache/libfcache_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-02-23 03:03:34.000000 libbde-20240223/libfcache/libfcache_cache_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-23 03:03:34.000000 libbde-20240223/libfcache/libfcache_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-02-23 03:03:34.000000 libbde-20240223/libfcache/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-23 03:03:34.000000 libbde-20240223/libfcache/libfcache_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-23 03:03:34.000000 libbde-20240223/libfcache/libfcache_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-02-23 03:03:34.000000 libbde-20240223/libfcache/libfcache_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-02-23 03:03:34.000000 libbde-20240223/libfcache/libfcache_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-23 03:03:34.000000 libbde-20240223/libfcache/libfcache_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-23 03:03:34.000000 libbde-20240223/libfcache/libfcache_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-02-23 03:03:34.000000 libbde-20240223/libfcache/libfcache_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-23 03:03:34.000000 libbde-20240223/libfcache/libfcache_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-02-23 03:03:34.000000 libbde-20240223/libfcache/libfcache_cache_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31288 2024-02-23 03:03:50.000000 libbde-20240223/libfcache/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-02-23 03:03:34.000000 libbde-20240223/libfcache/libfcache_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-02-23 03:03:34.000000 libbde-20240223/libfcache/libfcache_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-02-23 03:03:34.000000 libbde-20240223/libfcache/libfcache_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2390 2023-12-04 16:58:09.000000 libbde-20240223/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:58.000000 libbde-20240223/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_file_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_file_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_file_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_file_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_file_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_file_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_memory_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_file_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_file_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_memory_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_memory_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34274 2024-02-23 03:03:50.000000 libbde-20240223/libbfio/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_memory_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-02-23 03:03:22.000000 libbde-20240223/libbfio/libbfio_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 08:56:43.000000 libbde-20240223/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-02-23 03:03:50.000000 libbde-20240223/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:57.000000 libbde-20240223/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-02-23 02:47:17.000000 libbde-20240223/dpkg/libbde.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-02-23 02:47:17.000000 libbde-20240223/dpkg/libbde-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1022 2024-02-23 02:47:19.000000 libbde-20240223/dpkg/copyright
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:57.000000 libbde-20240223/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-02-23 02:47:17.000000 libbde-20240223/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2087 2024-02-23 02:47:17.000000 libbde-20240223/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-02-23 02:47:17.000000 libbde-20240223/dpkg/libbde-tools.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      753 2024-02-23 02:47:17.000000 libbde-20240223/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      119 2024-02-23 02:47:17.000000 libbde-20240223/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      138 2024-02-23 03:04:01.000000 libbde-20240223/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-02-23 02:47:17.000000 libbde-20240223/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-02-23 02:47:17.000000 libbde-20240223/dpkg/libbde-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      476 2024-02-23 03:04:01.000000 libbde-20240223/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-02-23 02:47:17.000000 libbde-20240223/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  2123694 2024-02-23 03:03:49.000000 libbde-20240223/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-02-23 03:03:50.000000 libbde-20240223/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-02-23 03:03:50.000000 libbde-20240223/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/bde_test_sector_data/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6199 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/bde_test_sector_data/bde_test_sector_data.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/bde_test_key_protector/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5961 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/bde_test_key_protector/bde_test_key_protector.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/bde_test_key/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5931 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/bde_test_key/bde_test_key.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/pybde/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/pybde/pybde.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/libcaes/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4777 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/libcaes/libcaes.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/libfguid/libfguid.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/bdemount/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7688 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/bdemount/bdemount.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/bde_test_stretch_key/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5955 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/bde_test_stretch_key/bde_test_stretch_key.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/bde_test_sector_data_vector/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6220 2024-02-23 02:48:06.000000 libbde-20240223/msvscpp/bde_test_sector_data_vector/bde_test_sector_data_vector.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/libclocale/libclocale.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/bde_test_tools_output/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5885 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/bde_test_tools_output/bde_test_tools_output.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/bde_test_tools_signal/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5885 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/bde_test_tools_signal/bde_test_tools_signal.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/libfcache/libfcache.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2007 2024-02-23 02:48:06.000000 libbde-20240223/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/libbfio/libbfio.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/bde_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5783 2024-02-23 02:48:06.000000 libbde-20240223/msvscpp/bde_test_notify/bde_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/bde_test_volume/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6587 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/bde_test_volume/bde_test_volume.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/bde_test_aes_ccm_encrypted_key/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5985 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/bde_test_aes_ccm_encrypted_key/bde_test_aes_ccm_encrypted_key.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/libbde/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11175 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/libbde/libbde.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/bde_test_external_key/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5958 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/bde_test_external_key/bde_test_external_key.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/bde_test_volume_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6205 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/bde_test_volume_header/bde_test_volume_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/bde_test_volume_master_key/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5973 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/bde_test_volume_master_key/bde_test_volume_master_key.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41767 2024-02-23 02:48:06.000000 libbde-20240223/msvscpp/libbde.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/bde_test_password_keep/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5961 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/bde_test_password_keep/bde_test_password_keep.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/bde_test_encryption_context/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5976 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/bde_test_encryption_context/bde_test_encryption_context.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/bdeinfo/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6970 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/bdeinfo/bdeinfo.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/bde_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6590 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/bde_test_support/bde_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/bde_test_metadata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5946 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/bde_test_metadata/bde_test_metadata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/bde_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5697 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/bde_test_error/bde_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/libcpath/libcpath.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/bde_test_io_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5949 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/bde_test_io_handle/bde_test_io_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/bde_test_metadata_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6211 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/bde_test_metadata_header/bde_test_metadata_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/libhmac/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6182 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/libhmac/libhmac.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/bde_test_metadata_block_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6229 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/bde_test_metadata_block_header/bde_test_metadata_block_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/libcsplit/libcsplit.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/bde_test_metadata_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5964 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/bde_test_metadata_entry/bde_test_metadata_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24787 2024-02-23 03:03:50.000000 libbde-20240223/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8010 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/libfvalue/libfvalue.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-02-23 02:47:42.000000 libbde-20240223/msvscpp/libfdatetime/libfdatetime.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/bde_test_password/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5788 2024-02-23 02:48:06.000000 libbde-20240223/msvscpp/bde_test_password/bde_test_password.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/msvscpp/bde_test_tools_info_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6378 2024-02-23 02:48:06.000000 libbde-20240223/msvscpp/bde_test_tools_info_handle/bde_test_tools_info_handle.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       90 2024-02-23 02:47:18.000000 libbde-20240223/AUTHORS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:58.000000 libbde-20240223/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-23 03:03:27.000000 libbde-20240223/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-02-23 03:03:27.000000 libbde-20240223/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-23 03:03:27.000000 libbde-20240223/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-02-23 03:03:27.000000 libbde-20240223/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-02-23 03:03:27.000000 libbde-20240223/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-02-23 03:03:27.000000 libbde-20240223/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      942 2024-02-23 03:03:27.000000 libbde-20240223/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-02-23 03:03:27.000000 libbde-20240223/libcfile/libcfile_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-23 03:03:27.000000 libbde-20240223/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-02-23 03:03:27.000000 libbde-20240223/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-23 03:03:27.000000 libbde-20240223/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-02-23 03:03:27.000000 libbde-20240223/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-23 03:03:27.000000 libbde-20240223/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-23 03:03:27.000000 libbde-20240223/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-02-23 03:03:27.000000 libbde-20240223/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-23 03:03:27.000000 libbde-20240223/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-02-23 03:03:27.000000 libbde-20240223/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31579 2024-02-23 03:03:50.000000 libbde-20240223/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-23 03:03:27.000000 libbde-20240223/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-23 03:03:27.000000 libbde-20240223/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-02-23 03:03:27.000000 libbde-20240223/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-02-23 03:03:27.000000 libbde-20240223/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1133 2024-02-23 02:48:06.000000 libbde-20240223/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      803 2024-02-23 02:47:17.000000 libbde-20240223/libbde.pc.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/libbde/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2335 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_sector_data_vector.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2132 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10458 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_metadata_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2730 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11284 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_external_key.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16347 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_ntfs_volume_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_metadata_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1753 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_password_keep.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2639 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_volume_master_key.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10148 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2017 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_key_protector.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10062 2024-02-23 02:47:19.000000 libbde-20240223/libbde/bde_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9594 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11433 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_metadata_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1914 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_external_key.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8965 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_sector_data_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_password_keep.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1791 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_stretch_key.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_aes_ccm_encrypted_key.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1542 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11182 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_recovery.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4346 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2980 2023-12-03 08:57:22.000000 libbde-20240223/libbde/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5837 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_metadata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6251 2024-02-23 02:47:19.000000 libbde-20240223/libbde/bde_metadata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   112107 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1761 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_diffuser.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1410 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_libhmac.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11864 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_password.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1084 2024-02-23 03:04:01.000000 libbde-20240223/libbde/libbde.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2096 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_metadata_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1996 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1785 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_libfvalue.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7215 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1890 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_sector_data.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7119 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_stretch_key.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1780 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_ntfs_volume_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1086 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11324 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_metadata_block_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1720 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1823 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2648 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_encryption_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18061 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_diffuser.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12427 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_sector_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4344 2024-02-23 03:04:01.000000 libbde-20240223/libbde/libbde_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73873 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_metadata.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2646 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_metadata_block_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_key.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18249 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_volume_master_key.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2301 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_password.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1562 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_recovery.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1584 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1892 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_aes_ccm_encrypted_key.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25487 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_volume_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1911 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39546 2024-02-23 03:03:50.000000 libbde-20240223/libbde/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2298 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_volume_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2934 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24702 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_encryption_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9860 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2571 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5810 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_key_protector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_libcaes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1611 2024-02-23 02:47:19.000000 libbde-20240223/libbde/libbde_key.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-02-23 03:03:50.000000 libbde-20240223/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:58.000000 libbde-20240223/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1127 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33263 2024-02-23 03:03:50.000000 libbde-20240223/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-23 03:03:24.000000 libbde-20240223/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-02-23 02:47:17.000000 libbde-20240223/pyproject.toml
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2417 2024-02-23 03:04:01.000000 libbde-20240223/libbde.spec
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      477 2024-02-23 02:47:17.000000 libbde-20240223/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-02-23 03:03:50.000000 libbde-20240223/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-02-23 02:47:17.000000 libbde-20240223/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1685 2024-02-23 02:48:35.000000 libbde-20240223/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 08:56:43.000000 libbde-20240223/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:58.000000 libbde-20240223/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-02-23 03:03:33.000000 libbde-20240223/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-02-23 03:03:33.000000 libbde-20240223/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-02-23 03:03:33.000000 libbde-20240223/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-02-23 03:03:33.000000 libbde-20240223/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-02-23 03:03:33.000000 libbde-20240223/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-02-23 03:03:33.000000 libbde-20240223/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-23 03:03:33.000000 libbde-20240223/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-02-23 03:03:33.000000 libbde-20240223/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-02-23 03:03:33.000000 libbde-20240223/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-02-23 03:03:33.000000 libbde-20240223/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-02-23 03:03:33.000000 libbde-20240223/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-02-23 03:03:33.000000 libbde-20240223/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-02-23 03:03:33.000000 libbde-20240223/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-02-23 03:03:33.000000 libbde-20240223/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-02-23 03:03:33.000000 libbde-20240223/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-02-23 03:03:33.000000 libbde-20240223/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-02-23 03:03:33.000000 libbde-20240223/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-02-23 03:03:33.000000 libbde-20240223/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-02-23 03:03:33.000000 libbde-20240223/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-02-23 03:03:33.000000 libbde-20240223/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-23 03:03:33.000000 libbde-20240223/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-02-23 03:03:33.000000 libbde-20240223/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-02-23 03:03:33.000000 libbde-20240223/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-02-23 03:03:33.000000 libbde-20240223/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-02-23 03:03:33.000000 libbde-20240223/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-02-23 03:03:33.000000 libbde-20240223/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-02-23 03:03:33.000000 libbde-20240223/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33669 2024-02-23 03:03:50.000000 libbde-20240223/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-02-23 03:03:33.000000 libbde-20240223/libcthreads/libcthreads_queue.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-02-23 03:03:51.000000 libbde-20240223/test-driver
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:58.000000 libbde-20240223/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-02-23 03:03:30.000000 libbde-20240223/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-23 03:03:30.000000 libbde-20240223/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-02-23 03:03:30.000000 libbde-20240223/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      842 2024-02-23 03:03:30.000000 libbde-20240223/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-02-23 03:03:30.000000 libbde-20240223/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-02-23 03:03:30.000000 libbde-20240223/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-02-23 03:03:30.000000 libbde-20240223/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-02-23 03:03:30.000000 libbde-20240223/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-02-23 03:03:30.000000 libbde-20240223/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-02-23 03:03:30.000000 libbde-20240223/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-23 03:03:30.000000 libbde-20240223/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-02-23 03:03:30.000000 libbde-20240223/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30857 2024-02-23 03:03:50.000000 libbde-20240223/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-23 03:03:30.000000 libbde-20240223/libcpath/libcpath_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-02-23 03:03:30.000000 libbde-20240223/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-02-23 03:03:30.000000 libbde-20240223/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-02-23 03:03:30.000000 libbde-20240223/libcpath/libcpath_path.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2066 2023-12-03 08:56:43.000000 libbde-20240223/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      178 2023-12-03 08:57:23.000000 libbde-20240223/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7219 2024-02-23 02:48:55.000000 libbde-20240223/manuals/libbde.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2327 2024-02-23 02:47:19.000000 libbde-20240223/manuals/bdeinfo.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27802 2024-02-23 03:03:50.000000 libbde-20240223/manuals/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1958 2024-02-23 02:47:19.000000 libbde-20240223/manuals/bdemount.1
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15109 2024-02-23 02:48:06.000000 libbde-20240223/tests/bde_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6877 2024-02-23 02:48:06.000000 libbde-20240223/tests/bde_test_encryption_context.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3357 2024-02-23 02:47:19.000000 libbde-20240223/tests/test_bdeinfo.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5971 2024-02-23 02:48:06.000000 libbde-20240223/tests/bde_test_stretch_key.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6027 2024-02-23 02:48:06.000000 libbde-20240223/tests/bde_test_external_key.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4106 2024-02-23 02:48:27.000000 libbde-20240223/tests/test_tools.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-02-23 02:47:19.000000 libbde-20240223/tests/bde_test_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4606 2024-02-23 02:47:19.000000 libbde-20240223/tests/bde_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6204 2024-02-23 02:48:06.000000 libbde-20240223/tests/bde_test_metadata_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-02-23 02:47:19.000000 libbde-20240223/tests/bde_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3332 2024-02-23 02:48:27.000000 libbde-20240223/tests/pybde_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2803 2024-02-23 02:48:06.000000 libbde-20240223/tests/bde_test_key_protector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10023 2024-02-23 02:48:06.000000 libbde-20240223/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-02-23 02:47:19.000000 libbde-20240223/tests/bde_test_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16025 2024-02-23 02:48:06.000000 libbde-20240223/tests/bde_test_volume_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8504 2024-02-23 02:47:19.000000 libbde-20240223/tests/bde_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16764 2024-02-23 02:48:06.000000 libbde-20240223/tests/bde_test_sector_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20211 2024-02-23 02:48:06.000000 libbde-20240223/tests/bde_test_metadata.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-02-23 02:47:19.000000 libbde-20240223/tests/bde_test_getopt.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-02-23 02:47:19.000000 libbde-20240223/tests/test_manpage.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4116 2024-02-23 02:47:19.000000 libbde-20240223/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16382 2024-02-23 02:48:06.000000 libbde-20240223/tests/bde_test_metadata_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8053 2024-02-23 02:48:06.000000 libbde-20240223/tests/bde_test_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6885 2024-02-23 02:48:06.000000 libbde-20240223/tests/bde_test_sector_data_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1977 2024-02-23 02:47:19.000000 libbde-20240223/tests/bde_test_functions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-02-23 02:47:19.000000 libbde-20240223/tests/bde_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-02-23 02:47:19.000000 libbde-20240223/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16197 2024-02-23 02:48:06.000000 libbde-20240223/tests/bde_test_metadata_block_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4077 2024-02-23 02:47:19.000000 libbde-20240223/tests/bde_test_tools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5724 2024-02-23 02:48:06.000000 libbde-20240223/tests/bde_test_key.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15698 2024-02-23 02:47:19.000000 libbde-20240223/tests/bde_test_functions.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-23 02:47:19.000000 libbde-20240223/tests/bde_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4229 2024-02-23 02:47:19.000000 libbde-20240223/tests/bde_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11319 2024-02-23 02:48:06.000000 libbde-20240223/tests/bde_test_volume_master_key.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5618 2024-02-23 02:47:19.000000 libbde-20240223/tests/bde_test_tools_info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81609 2024-02-23 02:48:06.000000 libbde-20240223/tests/bde_test_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7158 2024-02-23 02:47:19.000000 libbde-20240223/tests/bde_test_password.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-02-23 02:47:19.000000 libbde-20240223/tests/bde_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-02-23 02:47:19.000000 libbde-20240223/tests/bde_test_libbde.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74258 2024-02-23 03:03:51.000000 libbde-20240223/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2403 2024-02-23 02:47:19.000000 libbde-20240223/tests/bde_test_tools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6541 2024-02-23 02:48:06.000000 libbde-20240223/tests/bde_test_aes_ccm_encrypted_key.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-02-23 02:47:19.000000 libbde-20240223/tests/bde_test_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25495 2024-02-23 02:48:27.000000 libbde-20240223/tests/pybde_test_volume.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3059 2024-02-23 02:47:19.000000 libbde-20240223/tests/bde_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4527 2024-02-23 02:47:19.000000 libbde-20240223/tests/bde_test_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6031 2024-02-23 02:47:19.000000 libbde-20240223/tests/bde_test_password_keep.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4347 2024-02-23 02:48:27.000000 libbde-20240223/tests/test_library.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2210 2024-02-23 02:47:19.000000 libbde-20240223/ossfuzz/volume_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      962 2024-02-23 02:47:19.000000 libbde-20240223/ossfuzz/ossfuzz_libbde.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      898 2023-12-03 08:56:44.000000 libbde-20240223/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-02-23 02:47:19.000000 libbde-20240223/ossfuzz/ossfuzz_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33055 2024-02-23 03:03:50.000000 libbde-20240223/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-02-23 03:03:45.000000 libbde-20240223/ltmain.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:58.000000 libbde-20240223/libhmac/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47989 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_sha1_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_sha224.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50026 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_sha512_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14448 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_md5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2079 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_md5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1942 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9362 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14650 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_sha512.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45648 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_sha256_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_sha224.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1623 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2060 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_sha1.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3443 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_sha256_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1121 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45605 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_sha224_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_md5_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_sha256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3368 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_sha1_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33389 2024-02-23 03:03:50.000000 libbde-20240223/libhmac/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_sha256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3461 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_sha224_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3444 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_sha512_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_sha512.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14514 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_sha1.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40596 2024-02-23 03:03:39.000000 libbde-20240223/libhmac/libhmac_md5_context.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:58.000000 libbde-20240223/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-02-23 03:03:31.000000 libbde-20240223/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-02-23 03:03:31.000000 libbde-20240223/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-02-23 03:03:31.000000 libbde-20240223/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-02-23 03:03:31.000000 libbde-20240223/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-23 03:03:31.000000 libbde-20240223/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      884 2024-02-23 03:03:31.000000 libbde-20240223/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-23 03:03:31.000000 libbde-20240223/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-02-23 03:03:31.000000 libbde-20240223/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-23 03:03:31.000000 libbde-20240223/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-02-23 03:03:31.000000 libbde-20240223/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-23 03:03:31.000000 libbde-20240223/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-02-23 03:03:31.000000 libbde-20240223/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-23 03:03:31.000000 libbde-20240223/libcsplit/libcsplit_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-23 03:03:31.000000 libbde-20240223/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-23 03:03:31.000000 libbde-20240223/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-02-23 03:03:31.000000 libbde-20240223/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31637 2024-02-23 03:03:50.000000 libbde-20240223/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-02-23 03:03:31.000000 libbde-20240223/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-02-23 03:03:31.000000 libbde-20240223/libcsplit/libcsplit_narrow_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:59.000000 libbde-20240223/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 08:57:24.000000 libbde-20240223/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 08:57:24.000000 libbde-20240223/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 08:57:24.000000 libbde-20240223/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 08:57:24.000000 libbde-20240223/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 08:57:24.000000 libbde-20240223/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 08:57:24.000000 libbde-20240223/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 08:57:24.000000 libbde-20240223/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 08:57:24.000000 libbde-20240223/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 08:57:24.000000 libbde-20240223/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2024-02-23 03:04:01.000000 libbde-20240223/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 08:57:24.000000 libbde-20240223/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 08:57:24.000000 libbde-20240223/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:58.000000 libbde-20240223/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4197 2024-02-23 03:03:41.000000 libbde-20240223/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    54381 2024-02-23 03:03:50.000000 libbde-20240223/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-02-23 03:03:41.000000 libbde-20240223/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41934 2024-02-23 03:03:50.000000 libbde-20240223/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:58.000000 libbde-20240223/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_split_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3075 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_split_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1684 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_value_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_split_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_value_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_binary_data.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_value_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_split_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_floating_point.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_binary_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_value_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36094 2024-02-23 03:03:50.000000 libbde-20240223/libfvalue/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84529 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_floating_point.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-02-23 03:03:37.000000 libbde-20240223/libfvalue/libfvalue_libuna.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:58.000000 libbde-20240223/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-02-23 03:03:29.000000 libbde-20240223/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-02-23 03:03:29.000000 libbde-20240223/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-02-23 03:03:29.000000 libbde-20240223/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-02-23 03:03:29.000000 libbde-20240223/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-02-23 03:03:29.000000 libbde-20240223/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-02-23 03:03:29.000000 libbde-20240223/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-02-23 03:03:29.000000 libbde-20240223/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-02-23 03:03:29.000000 libbde-20240223/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-02-23 03:03:29.000000 libbde-20240223/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-02-23 03:03:29.000000 libbde-20240223/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-02-23 03:03:29.000000 libbde-20240223/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30691 2024-02-23 03:03:50.000000 libbde-20240223/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-02-23 03:03:29.000000 libbde-20240223/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-02-23 03:03:29.000000 libbde-20240223/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:58.000000 libbde-20240223/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-02-23 03:03:25.000000 libbde-20240223/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-02-23 03:03:25.000000 libbde-20240223/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-02-23 03:03:25.000000 libbde-20240223/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-02-23 03:03:25.000000 libbde-20240223/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-02-23 03:03:25.000000 libbde-20240223/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-02-23 03:03:25.000000 libbde-20240223/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-02-23 03:03:25.000000 libbde-20240223/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-02-23 03:03:25.000000 libbde-20240223/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-02-23 03:03:25.000000 libbde-20240223/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-02-23 03:03:25.000000 libbde-20240223/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-02-23 03:03:25.000000 libbde-20240223/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30204 2024-02-23 03:03:50.000000 libbde-20240223/libcerror/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-02-23 03:41:58.000000 libbde-20240223/libfdatetime/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-02-23 03:03:35.000000 libbde-20240223/libfdatetime/libfdatetime_floatingtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-02-23 03:03:35.000000 libbde-20240223/libfdatetime/libfdatetime_nsf_timedate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-02-23 03:03:35.000000 libbde-20240223/libfdatetime/libfdatetime_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-02-23 03:03:35.000000 libbde-20240223/libfdatetime/libfdatetime_floatingtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-02-23 03:03:35.000000 libbde-20240223/libfdatetime/libfdatetime_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-02-23 03:03:35.000000 libbde-20240223/libfdatetime/libfdatetime_hfs_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-02-23 03:03:35.000000 libbde-20240223/libfdatetime/libfdatetime_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-02-23 03:03:35.000000 libbde-20240223/libfdatetime/libfdatetime_hfs_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1148 2024-02-23 03:03:35.000000 libbde-20240223/libfdatetime/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-02-23 03:03:35.000000 libbde-20240223/libfdatetime/libfdatetime_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-02-23 03:03:35.000000 libbde-20240223/libfdatetime/libfdatetime_systemtime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-02-23 03:03:35.000000 libbde-20240223/libfdatetime/libfdatetime_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-02-23 03:03:35.000000 libbde-20240223/libfdatetime/libfdatetime_posix_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-02-23 03:03:35.000000 libbde-20240223/libfdatetime/libfdatetime_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-02-23 03:03:35.000000 libbde-20240223/libfdatetime/libfdatetime_fat_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-02-23 03:03:35.000000 libbde-20240223/libfdatetime/libfdatetime_systemtime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-02-23 03:03:35.000000 libbde-20240223/libfdatetime/libfdatetime_nsf_timedate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-02-23 03:03:35.000000 libbde-20240223/libfdatetime/libfdatetime_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-02-23 03:03:35.000000 libbde-20240223/libfdatetime/libfdatetime_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-02-23 03:03:35.000000 libbde-20240223/libfdatetime/libfdatetime_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-02-23 03:03:35.000000 libbde-20240223/libfdatetime/libfdatetime_posix_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-02-23 03:03:35.000000 libbde-20240223/libfdatetime/libfdatetime_date_time_values.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-02-23 03:03:35.000000 libbde-20240223/libfdatetime/libfdatetime_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-02-23 03:03:35.000000 libbde-20240223/libfdatetime/libfdatetime_date_time_values.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-02-23 03:03:35.000000 libbde-20240223/libfdatetime/libfdatetime_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33430 2024-02-23 03:03:50.000000 libbde-20240223/libfdatetime/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-02-23 03:03:35.000000 libbde-20240223/libfdatetime/libfdatetime_fat_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56913 2024-02-23 03:03:47.000000 libbde-20240223/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8402 2024-02-23 02:47:17.000000 libbde-20240223/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      408 2024-02-23 03:42:00.293579 libbde-20240223/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/bdetools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37141 2024-05-02 03:56:48.000000 libbde-20240502/bdetools/mount_dokan.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2979 2024-05-02 03:56:48.000000 libbde-20240502/bdetools/mount_file_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1775 2024-05-02 03:56:48.000000 libbde-20240502/bdetools/bdetools_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27263 2024-05-02 03:56:48.000000 libbde-20240502/bdetools/mount_fuse.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4012 2024-05-02 03:56:48.000000 libbde-20240502/bdetools/bdetools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4005 2024-05-02 03:58:00.000000 libbde-20240502/bdetools/info_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5411 2024-05-02 03:56:48.000000 libbde-20240502/bdetools/mount_dokan.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-02 03:56:48.000000 libbde-20240502/bdetools/bdetools_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1458 2024-05-02 03:56:48.000000 libbde-20240502/bdetools/bdetools_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-05-02 03:56:48.000000 libbde-20240502/bdetools/bdetools_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1306 2024-05-02 03:56:48.000000 libbde-20240502/bdetools/bdetools_input.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18932 2024-05-02 03:58:00.000000 libbde-20240502/bdetools/mount_file_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-05-02 03:56:48.000000 libbde-20240502/bdetools/bdetools_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1498 2024-05-02 03:56:48.000000 libbde-20240502/bdetools/bdetools_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11853 2024-05-02 03:56:48.000000 libbde-20240502/bdetools/byte_size_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2467 2024-05-02 04:03:49.000000 libbde-20240502/bdetools/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1421 2024-05-02 03:56:48.000000 libbde-20240502/bdetools/bdetools_output.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5701 2024-05-02 03:56:48.000000 libbde-20240502/bdetools/bdetools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21702 2024-05-02 03:58:00.000000 libbde-20240502/bdetools/mount_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44113 2024-05-02 03:58:00.000000 libbde-20240502/bdetools/info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3611 2024-05-02 03:56:48.000000 libbde-20240502/bdetools/mount_file_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-05-02 03:56:48.000000 libbde-20240502/bdetools/bdetools_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-05-02 03:56:48.000000 libbde-20240502/bdetools/bdetools_libbde.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2024-05-02 03:56:48.000000 libbde-20240502/bdetools/bdetools_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8762 2024-05-02 03:58:00.000000 libbde-20240502/bdetools/bdeinfo.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1207 2024-05-02 03:56:48.000000 libbde-20240502/bdetools/bdetools_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4132 2024-05-02 03:58:00.000000 libbde-20240502/bdetools/mount_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6306 2024-05-02 03:56:48.000000 libbde-20240502/bdetools/bdetools_input.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1765 2024-05-02 03:56:48.000000 libbde-20240502/bdetools/bdetools_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34130 2024-05-02 03:58:00.000000 libbde-20240502/bdetools/mount_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1477 2024-05-02 03:56:48.000000 libbde-20240502/bdetools/bdetools_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1437 2024-05-02 03:56:48.000000 libbde-20240502/bdetools/bdetools_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1403 2024-05-02 03:56:48.000000 libbde-20240502/bdetools/bdetools_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36001 2024-05-02 04:28:19.000000 libbde-20240502/bdetools/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1737 2024-05-02 03:56:48.000000 libbde-20240502/bdetools/bdetools_signal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4527 2024-05-02 03:56:48.000000 libbde-20240502/bdetools/bdetools_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1988 2024-05-02 03:56:48.000000 libbde-20240502/bdetools/byte_size_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19419 2024-05-02 03:58:00.000000 libbde-20240502/bdetools/bdemount.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3550 2024-05-02 03:58:00.000000 libbde-20240502/bdetools/mount_fuse.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-05-02 03:56:45.000000 libbde-20240502/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-05-02 04:28:19.000000 libbde-20240502/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 03:56:45.000000 libbde-20240502/NEWS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-05-02 04:28:20.000000 libbde-20240502/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/pybde/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2076 2024-05-02 03:56:48.000000 libbde-20240502/pybde/pybde_key_protector.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4698 2024-05-02 03:58:00.000000 libbde-20240502/pybde/pybde_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8840 2024-05-02 03:56:48.000000 libbde-20240502/pybde/pybde_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2027 2024-05-02 03:56:48.000000 libbde-20240502/pybde/pybde_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-05-02 03:56:48.000000 libbde-20240502/pybde/pybde_libbde.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4042 2024-05-02 03:56:48.000000 libbde-20240502/pybde/pybde_file_object_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1842 2024-05-02 03:56:48.000000 libbde-20240502/pybde/pybde.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1526 2024-05-02 03:56:48.000000 libbde-20240502/pybde/pybde_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2842 2024-05-02 03:56:48.000000 libbde-20240502/pybde/pybde_guid.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9506 2024-05-02 03:56:48.000000 libbde-20240502/pybde/pybde_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7138 2024-05-02 03:56:48.000000 libbde-20240502/pybde/pybde_encryption_methods.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-05-02 03:56:48.000000 libbde-20240502/pybde/pybde_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1370 2024-05-02 04:03:59.000000 libbde-20240502/pybde/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1519 2024-05-02 03:56:48.000000 libbde-20240502/pybde/pybde_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1352 2024-05-02 03:56:48.000000 libbde-20240502/pybde/pybde_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66022 2024-05-02 03:58:00.000000 libbde-20240502/pybde/pybde_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8869 2024-05-02 03:56:48.000000 libbde-20240502/pybde/pybde_key_protector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16024 2024-05-02 03:58:00.000000 libbde-20240502/pybde/pybde.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7137 2024-05-02 03:56:48.000000 libbde-20240502/pybde/pybde_key_protection_types.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16577 2024-05-02 03:56:48.000000 libbde-20240502/pybde/pybde_datetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-05-02 03:56:48.000000 libbde-20240502/pybde/pybde_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33702 2024-05-02 03:56:48.000000 libbde-20240502/pybde/pybde_file_object_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1429 2024-05-02 03:56:48.000000 libbde-20240502/pybde/pybde_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2483 2024-05-02 03:56:48.000000 libbde-20240502/pybde/pybde_key_protectors.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1384 2024-05-02 03:56:48.000000 libbde-20240502/pybde/pybde_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9493 2024-05-02 03:56:48.000000 libbde-20240502/pybde/pybde_key_protectors.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49792 2024-05-02 04:28:20.000000 libbde-20240502/pybde/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1698 2024-05-02 03:56:48.000000 libbde-20240502/pybde/pybde_encryption_methods.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1726 2024-05-02 03:56:48.000000 libbde-20240502/pybde/pybde_key_protection_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1804 2024-05-02 03:56:48.000000 libbde-20240502/pybde/pybde_datetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1165 2024-05-02 03:56:48.000000 libbde-20240502/pybde/pybde_guid.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/libcaes/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-02 04:27:48.000000 libbde-20240502/libcaes/libcaes_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2885 2024-05-02 04:27:48.000000 libbde-20240502/libcaes/libcaes_tweaked_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4464 2024-05-02 04:27:48.000000 libbde-20240502/libcaes/libcaes_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-02 04:27:48.000000 libbde-20240502/libcaes/libcaes_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82616 2024-05-02 04:27:48.000000 libbde-20240502/libcaes/libcaes_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1743 2024-05-02 04:27:48.000000 libbde-20240502/libcaes/libcaes_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      734 2024-05-02 04:27:48.000000 libbde-20240502/libcaes/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-02 04:27:48.000000 libbde-20240502/libcaes/libcaes_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1608 2024-05-02 04:27:48.000000 libbde-20240502/libcaes/libcaes_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-02 04:27:48.000000 libbde-20240502/libcaes/libcaes_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-05-02 04:27:48.000000 libbde-20240502/libcaes/libcaes_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-02 04:27:48.000000 libbde-20240502/libcaes/libcaes_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-05-02 04:27:48.000000 libbde-20240502/libcaes/libcaes_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30814 2024-05-02 04:28:20.000000 libbde-20240502/libcaes/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33103 2024-05-02 04:27:48.000000 libbde-20240502/libcaes/libcaes_tweaked_context.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:30.000000 libbde-20240502/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-02 04:28:01.000000 libbde-20240502/libfguid/libfguid_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-05-02 04:28:01.000000 libbde-20240502/libfguid/libfguid_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-05-02 04:28:01.000000 libbde-20240502/libfguid/libfguid_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-02 04:28:01.000000 libbde-20240502/libfguid/libfguid_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      677 2024-05-02 04:28:01.000000 libbde-20240502/libfguid/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-02 04:28:01.000000 libbde-20240502/libfguid/libfguid_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-02 04:28:01.000000 libbde-20240502/libfguid/libfguid_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-05-02 04:28:01.000000 libbde-20240502/libfguid/libfguid_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-05-02 04:28:01.000000 libbde-20240502/libfguid/libfguid_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-05-02 04:28:01.000000 libbde-20240502/libfguid/libfguid_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-05-02 04:28:01.000000 libbde-20240502/libfguid/libfguid_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30465 2024-05-02 04:28:20.000000 libbde-20240502/libfguid/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-02 04:28:01.000000 libbde-20240502/libfguid/libfguid_error.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:29.000000 libbde-20240502/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11734 2024-05-02 03:56:49.000000 libbde-20240502/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18489 2024-05-02 03:56:49.000000 libbde-20240502/m4/libfdatetime.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 08:57:23.000000 libbde-20240502/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9615 2024-05-02 03:56:49.000000 libbde-20240502/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 08:57:24.000000 libbde-20240502/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 08:57:24.000000 libbde-20240502/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-05-02 03:56:49.000000 libbde-20240502/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 08:57:24.000000 libbde-20240502/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 08:57:24.000000 libbde-20240502/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-05-02 03:56:49.000000 libbde-20240502/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-05-02 03:56:49.000000 libbde-20240502/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7625 2024-05-02 03:56:49.000000 libbde-20240502/m4/libcsplit.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-04-11 16:55:50.000000 libbde-20240502/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-05-02 03:56:49.000000 libbde-20240502/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-05-02 04:28:13.000000 libbde-20240502/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-05-02 04:28:13.000000 libbde-20240502/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 08:57:24.000000 libbde-20240502/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7058 2024-04-13 08:15:03.000000 libbde-20240502/m4/libfuse.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-05-02 04:28:12.000000 libbde-20240502/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 08:57:24.000000 libbde-20240502/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-05-02 03:56:49.000000 libbde-20240502/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-05-02 03:56:49.000000 libbde-20240502/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5876 2024-05-02 03:56:49.000000 libbde-20240502/m4/libfguid.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11923 2024-05-02 03:56:49.000000 libbde-20240502/m4/libbfio.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8550 2024-05-02 03:56:49.000000 libbde-20240502/m4/libhmac.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 08:57:24.000000 libbde-20240502/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-05-02 04:28:13.000000 libbde-20240502/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 08:57:24.000000 libbde-20240502/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 08:57:24.000000 libbde-20240502/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-05-02 04:28:13.000000 libbde-20240502/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 08:57:24.000000 libbde-20240502/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-05-02 03:56:49.000000 libbde-20240502/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27647 2024-04-11 16:55:50.000000 libbde-20240502/m4/libcrypto.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20032 2024-05-02 03:56:49.000000 libbde-20240502/m4/libfvalue.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 08:57:23.000000 libbde-20240502/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7566 2024-05-02 03:56:49.000000 libbde-20240502/m4/libfcache.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-04-11 16:55:50.000000 libbde-20240502/m4/pthread.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6500 2024-05-02 03:56:49.000000 libbde-20240502/m4/libcaes.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3509 2024-05-02 03:56:45.000000 libbde-20240502/libbde.spec.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:29.000000 libbde-20240502/include/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16052 2024-05-02 04:28:34.000000 libbde-20240502/include/libbde.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      395 2024-05-02 04:02:20.000000 libbde-20240502/include/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:29.000000 libbde-20240502/include/libbde/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2596 2024-05-02 03:56:47.000000 libbde-20240502/include/libbde/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2594 2024-05-02 04:28:34.000000 libbde-20240502/include/libbde/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4967 2024-05-02 03:56:47.000000 libbde-20240502/include/libbde/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4836 2024-05-02 04:28:34.000000 libbde-20240502/include/libbde/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-05-02 03:56:47.000000 libbde-20240502/include/libbde/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6622 2024-05-02 03:56:47.000000 libbde-20240502/include/libbde/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-02 03:56:47.000000 libbde-20240502/include/libbde/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-05-02 04:28:34.000000 libbde-20240502/include/libbde/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5078 2024-05-02 03:56:47.000000 libbde-20240502/include/libbde/codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28803 2024-05-02 04:28:19.000000 libbde-20240502/include/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16052 2024-05-02 03:56:47.000000 libbde-20240502/include/libbde.h.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:29.000000 libbde-20240502/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-05-02 03:56:47.000000 libbde-20240502/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-05-02 03:56:47.000000 libbde-20240502/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-05-02 03:56:47.000000 libbde-20240502/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-05-02 03:56:47.000000 libbde-20240502/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-02 03:56:47.000000 libbde-20240502/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-05-02 03:56:47.000000 libbde-20240502/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-05-02 03:56:47.000000 libbde-20240502/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-05-02 04:02:20.000000 libbde-20240502/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-05-02 03:56:47.000000 libbde-20240502/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7372 2024-05-02 04:28:34.000000 libbde-20240502/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19481 2024-05-02 04:28:19.000000 libbde-20240502/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20593 2024-05-02 04:28:34.000000 libbde-20240502/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-05-02 03:56:47.000000 libbde-20240502/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-05-02 03:56:47.000000 libbde-20240502/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-05-02 03:56:47.000000 libbde-20240502/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25875 2024-05-02 04:28:19.000000 libbde-20240502/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:30.000000 libbde-20240502/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-05-02 04:27:53.000000 libbde-20240502/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-05-02 04:27:53.000000 libbde-20240502/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-05-02 04:27:53.000000 libbde-20240502/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-05-02 04:27:53.000000 libbde-20240502/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-02 04:27:53.000000 libbde-20240502/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-02 04:27:53.000000 libbde-20240502/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-05-02 04:27:53.000000 libbde-20240502/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-05-02 04:27:53.000000 libbde-20240502/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-05-02 04:27:53.000000 libbde-20240502/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-05-02 04:27:53.000000 libbde-20240502/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31073 2024-05-02 04:28:20.000000 libbde-20240502/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-02 04:27:53.000000 libbde-20240502/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-05-02 04:27:53.000000 libbde-20240502/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-05-02 04:27:53.000000 libbde-20240502/libclocale/libclocale_codepage.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:30.000000 libbde-20240502/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-02 04:27:59.000000 libbde-20240502/libfcache/libfcache_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-05-02 04:27:59.000000 libbde-20240502/libfcache/libfcache_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-05-02 04:27:59.000000 libbde-20240502/libfcache/libfcache_cache_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-02 04:27:59.000000 libbde-20240502/libfcache/libfcache_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      876 2024-05-02 04:27:59.000000 libbde-20240502/libfcache/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-02 04:27:59.000000 libbde-20240502/libfcache/libfcache_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-02 04:27:59.000000 libbde-20240502/libfcache/libfcache_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-05-02 04:27:59.000000 libbde-20240502/libfcache/libfcache_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-05-02 04:27:59.000000 libbde-20240502/libfcache/libfcache_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-02 04:27:59.000000 libbde-20240502/libfcache/libfcache_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-02 04:27:59.000000 libbde-20240502/libfcache/libfcache_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-05-02 04:27:59.000000 libbde-20240502/libfcache/libfcache_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-02 04:27:59.000000 libbde-20240502/libfcache/libfcache_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-05-02 04:27:59.000000 libbde-20240502/libfcache/libfcache_cache_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31582 2024-05-02 04:28:20.000000 libbde-20240502/libfcache/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-02 04:27:59.000000 libbde-20240502/libfcache/libfcache_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-05-02 04:27:59.000000 libbde-20240502/libfcache/libfcache_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-05-02 04:27:59.000000 libbde-20240502/libfcache/libfcache_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2198 2024-05-02 04:04:48.000000 libbde-20240502/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:30.000000 libbde-20240502/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_file_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_file_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_file_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_file_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_file_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_file_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_memory_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_file_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_file_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_memory_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_memory_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34925 2024-05-02 04:28:19.000000 libbde-20240502/libbfio/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_memory_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-05-02 04:27:46.000000 libbde-20240502/libbfio/libbfio_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 08:56:43.000000 libbde-20240502/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-05-02 04:28:19.000000 libbde-20240502/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:29.000000 libbde-20240502/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-05-02 03:56:45.000000 libbde-20240502/dpkg/libbde.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-05-02 03:56:45.000000 libbde-20240502/dpkg/libbde-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1022 2024-05-02 03:56:49.000000 libbde-20240502/dpkg/copyright
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:29.000000 libbde-20240502/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-05-02 03:56:45.000000 libbde-20240502/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2087 2024-05-02 03:56:45.000000 libbde-20240502/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-05-02 03:56:45.000000 libbde-20240502/dpkg/libbde-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      753 2024-05-02 03:56:45.000000 libbde-20240502/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      119 2024-05-02 03:56:45.000000 libbde-20240502/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      138 2024-05-02 04:28:34.000000 libbde-20240502/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-05-02 03:56:45.000000 libbde-20240502/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-05-02 03:56:45.000000 libbde-20240502/dpkg/libbde-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      476 2024-05-02 04:28:34.000000 libbde-20240502/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-05-02 03:56:45.000000 libbde-20240502/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  2131317 2024-05-02 04:28:17.000000 libbde-20240502/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-05-02 04:28:19.000000 libbde-20240502/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-05-02 04:28:19.000000 libbde-20240502/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/bde_test_sector_data/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6199 2024-05-02 03:57:11.000000 libbde-20240502/msvscpp/bde_test_sector_data/bde_test_sector_data.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/bde_test_key_protector/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5961 2024-05-02 03:57:11.000000 libbde-20240502/msvscpp/bde_test_key_protector/bde_test_key_protector.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/bde_test_key/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5931 2024-05-02 03:57:11.000000 libbde-20240502/msvscpp/bde_test_key/bde_test_key.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/pybde/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-05-02 03:57:11.000000 libbde-20240502/msvscpp/pybde/pybde.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/libcaes/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4777 2024-05-02 03:57:11.000000 libbde-20240502/msvscpp/libcaes/libcaes.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-05-02 03:57:11.000000 libbde-20240502/msvscpp/libfguid/libfguid.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/bdemount/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7688 2024-05-02 03:57:11.000000 libbde-20240502/msvscpp/bdemount/bdemount.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/bde_test_stretch_key/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5955 2024-05-02 03:57:11.000000 libbde-20240502/msvscpp/bde_test_stretch_key/bde_test_stretch_key.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/bde_test_sector_data_vector/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6220 2024-05-02 03:57:30.000000 libbde-20240502/msvscpp/bde_test_sector_data_vector/bde_test_sector_data_vector.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-05-02 03:57:11.000000 libbde-20240502/msvscpp/libclocale/libclocale.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/bde_test_tools_output/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5885 2024-05-02 03:57:12.000000 libbde-20240502/msvscpp/bde_test_tools_output/bde_test_tools_output.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/bde_test_tools_signal/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5885 2024-05-02 03:57:12.000000 libbde-20240502/msvscpp/bde_test_tools_signal/bde_test_tools_signal.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-05-02 03:57:11.000000 libbde-20240502/msvscpp/libfcache/libfcache.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1978 2024-05-02 04:03:32.000000 libbde-20240502/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-05-02 03:57:11.000000 libbde-20240502/msvscpp/libbfio/libbfio.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/bde_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5783 2024-05-02 03:57:30.000000 libbde-20240502/msvscpp/bde_test_notify/bde_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/bde_test_volume/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6587 2024-05-02 03:57:12.000000 libbde-20240502/msvscpp/bde_test_volume/bde_test_volume.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/bde_test_aes_ccm_encrypted_key/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5985 2024-05-02 03:57:11.000000 libbde-20240502/msvscpp/bde_test_aes_ccm_encrypted_key/bde_test_aes_ccm_encrypted_key.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-05-02 03:57:11.000000 libbde-20240502/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/libbde/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11175 2024-05-02 03:57:11.000000 libbde-20240502/msvscpp/libbde/libbde.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/bde_test_external_key/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5958 2024-05-02 03:57:11.000000 libbde-20240502/msvscpp/bde_test_external_key/bde_test_external_key.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-05-02 03:57:11.000000 libbde-20240502/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/bde_test_volume_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6205 2024-05-02 03:57:12.000000 libbde-20240502/msvscpp/bde_test_volume_header/bde_test_volume_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/bde_test_volume_master_key/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5973 2024-05-02 03:57:12.000000 libbde-20240502/msvscpp/bde_test_volume_master_key/bde_test_volume_master_key.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41767 2024-05-02 03:57:30.000000 libbde-20240502/msvscpp/libbde.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/bde_test_password_keep/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5961 2024-05-02 03:57:11.000000 libbde-20240502/msvscpp/bde_test_password_keep/bde_test_password_keep.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/bde_test_encryption_context/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5976 2024-05-02 03:57:11.000000 libbde-20240502/msvscpp/bde_test_encryption_context/bde_test_encryption_context.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/bdeinfo/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6970 2024-05-02 03:57:11.000000 libbde-20240502/msvscpp/bdeinfo/bdeinfo.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-05-02 03:57:11.000000 libbde-20240502/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/bde_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6590 2024-05-02 03:57:12.000000 libbde-20240502/msvscpp/bde_test_support/bde_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/bde_test_metadata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5946 2024-05-02 03:57:11.000000 libbde-20240502/msvscpp/bde_test_metadata/bde_test_metadata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/bde_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5697 2024-05-02 03:57:11.000000 libbde-20240502/msvscpp/bde_test_error/bde_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-05-02 03:57:11.000000 libbde-20240502/msvscpp/libcpath/libcpath.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/bde_test_io_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5949 2024-05-02 03:57:11.000000 libbde-20240502/msvscpp/bde_test_io_handle/bde_test_io_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/bde_test_metadata_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6211 2024-05-02 03:57:11.000000 libbde-20240502/msvscpp/bde_test_metadata_header/bde_test_metadata_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/libhmac/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6182 2024-05-02 03:57:12.000000 libbde-20240502/msvscpp/libhmac/libhmac.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/bde_test_metadata_block_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6229 2024-05-02 03:57:11.000000 libbde-20240502/msvscpp/bde_test_metadata_block_header/bde_test_metadata_block_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-05-02 03:57:12.000000 libbde-20240502/msvscpp/libcsplit/libcsplit.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/bde_test_metadata_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5964 2024-05-02 03:57:11.000000 libbde-20240502/msvscpp/bde_test_metadata_entry/bde_test_metadata_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-05-02 03:57:12.000000 libbde-20240502/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24843 2024-05-02 04:28:20.000000 libbde-20240502/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8010 2024-05-02 03:57:12.000000 libbde-20240502/msvscpp/libfvalue/libfvalue.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-05-02 03:57:12.000000 libbde-20240502/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-05-02 03:57:12.000000 libbde-20240502/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6069 2024-05-02 03:57:12.000000 libbde-20240502/msvscpp/libfdatetime/libfdatetime.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/bde_test_password/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5788 2024-05-02 03:57:30.000000 libbde-20240502/msvscpp/bde_test_password/bde_test_password.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/msvscpp/bde_test_tools_info_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6378 2024-05-02 03:57:30.000000 libbde-20240502/msvscpp/bde_test_tools_info_handle/bde_test_tools_info_handle.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       90 2024-05-02 03:56:46.000000 libbde-20240502/AUTHORS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:30.000000 libbde-20240502/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-02 04:27:52.000000 libbde-20240502/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-05-02 04:27:52.000000 libbde-20240502/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-02 04:27:52.000000 libbde-20240502/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-02 04:27:52.000000 libbde-20240502/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-05-02 04:27:52.000000 libbde-20240502/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-05-02 04:27:52.000000 libbde-20240502/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      938 2024-05-02 04:27:52.000000 libbde-20240502/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-02 04:27:52.000000 libbde-20240502/libcfile/libcfile_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-02 04:27:52.000000 libbde-20240502/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-05-02 04:27:52.000000 libbde-20240502/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-02 04:27:52.000000 libbde-20240502/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-02 04:27:52.000000 libbde-20240502/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-02 04:27:52.000000 libbde-20240502/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-02 04:27:52.000000 libbde-20240502/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-05-02 04:27:52.000000 libbde-20240502/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-02 04:27:52.000000 libbde-20240502/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-05-02 04:27:52.000000 libbde-20240502/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31906 2024-05-02 04:28:20.000000 libbde-20240502/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-02 04:27:52.000000 libbde-20240502/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-02 04:27:52.000000 libbde-20240502/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-05-02 04:27:52.000000 libbde-20240502/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-05-02 04:27:52.000000 libbde-20240502/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1133 2024-05-02 03:58:00.000000 libbde-20240502/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      803 2024-05-02 03:56:45.000000 libbde-20240502/libbde.pc.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/libbde/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2335 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_sector_data_vector.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2132 2024-05-02 03:56:47.000000 libbde-20240502/libbde/libbde_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10458 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_metadata_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2730 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11284 2024-05-02 03:56:47.000000 libbde-20240502/libbde/libbde_external_key.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16347 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_ntfs_volume_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1730 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_metadata_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1753 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_password_keep.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2639 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_volume_master_key.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10148 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2017 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_key_protector.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10062 2024-05-02 03:56:47.000000 libbde-20240502/libbde/bde_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9594 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11433 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_metadata_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1914 2024-05-02 03:56:47.000000 libbde-20240502/libbde/libbde_external_key.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8965 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_sector_data_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_password_keep.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1791 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_stretch_key.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-05-02 03:56:47.000000 libbde-20240502/libbde/libbde_aes_ccm_encrypted_key.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1542 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11182 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_recovery.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4346 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-05-02 04:04:13.000000 libbde-20240502/libbde/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5837 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_metadata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6251 2024-05-02 03:56:47.000000 libbde-20240502/libbde/bde_metadata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   112107 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1761 2024-05-02 03:56:47.000000 libbde-20240502/libbde/libbde_diffuser.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1410 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_libhmac.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11864 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_password.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1084 2024-05-02 04:28:34.000000 libbde-20240502/libbde/libbde.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1697 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2096 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_metadata_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1996 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1785 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_libfvalue.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7215 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1890 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_sector_data.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7119 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_stretch_key.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1780 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_ntfs_volume_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1086 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-05-02 03:56:47.000000 libbde-20240502/libbde/libbde_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11324 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_metadata_block_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1720 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1823 2024-05-02 03:56:47.000000 libbde-20240502/libbde/libbde.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2648 2024-05-02 03:56:47.000000 libbde-20240502/libbde/libbde_encryption_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18061 2024-05-02 03:56:47.000000 libbde-20240502/libbde/libbde_diffuser.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12427 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_sector_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4344 2024-05-02 04:28:34.000000 libbde-20240502/libbde/libbde_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73873 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_metadata.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2646 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_metadata_block_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_key.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18249 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_volume_master_key.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2301 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_password.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1562 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_recovery.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1584 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1892 2024-05-02 03:56:47.000000 libbde-20240502/libbde/libbde_aes_ccm_encrypted_key.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25487 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_volume_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1911 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40737 2024-05-02 04:28:19.000000 libbde-20240502/libbde/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2298 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_volume_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2934 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24702 2024-05-02 03:56:47.000000 libbde-20240502/libbde/libbde_encryption_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9860 2024-05-02 03:56:47.000000 libbde-20240502/libbde/libbde_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2571 2024-05-02 03:56:47.000000 libbde-20240502/libbde/libbde_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5810 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_key_protector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-05-02 03:56:47.000000 libbde-20240502/libbde/libbde_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_libcaes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-05-02 03:56:47.000000 libbde-20240502/libbde/libbde_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1611 2024-05-02 03:56:48.000000 libbde-20240502/libbde/libbde_key.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-05-02 04:28:19.000000 libbde-20240502/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:30.000000 libbde-20240502/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33819 2024-05-02 04:28:20.000000 libbde-20240502/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-02 04:27:49.000000 libbde-20240502/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-05-02 03:56:45.000000 libbde-20240502/pyproject.toml
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2419 2024-05-02 04:28:34.000000 libbde-20240502/libbde.spec
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      477 2024-05-02 03:56:45.000000 libbde-20240502/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-05-02 04:28:19.000000 libbde-20240502/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-05-02 03:56:45.000000 libbde-20240502/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1685 2024-05-02 03:58:00.000000 libbde-20240502/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 08:56:43.000000 libbde-20240502/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:29.000000 libbde-20240502/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-05-02 04:27:58.000000 libbde-20240502/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-05-02 04:27:58.000000 libbde-20240502/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-05-02 04:27:58.000000 libbde-20240502/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-05-02 04:27:58.000000 libbde-20240502/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-05-02 04:27:58.000000 libbde-20240502/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-05-02 04:27:58.000000 libbde-20240502/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-02 04:27:58.000000 libbde-20240502/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-05-02 04:27:58.000000 libbde-20240502/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-05-02 04:27:58.000000 libbde-20240502/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-05-02 04:27:58.000000 libbde-20240502/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-05-02 04:27:58.000000 libbde-20240502/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-05-02 04:27:58.000000 libbde-20240502/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-05-02 04:27:58.000000 libbde-20240502/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-05-02 04:27:58.000000 libbde-20240502/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-05-02 04:27:58.000000 libbde-20240502/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-05-02 04:27:58.000000 libbde-20240502/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-05-02 04:27:58.000000 libbde-20240502/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-05-02 04:27:58.000000 libbde-20240502/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-05-02 04:27:58.000000 libbde-20240502/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-05-02 04:27:58.000000 libbde-20240502/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-02 04:27:58.000000 libbde-20240502/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-05-02 04:27:58.000000 libbde-20240502/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-05-02 04:27:58.000000 libbde-20240502/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-05-02 04:27:58.000000 libbde-20240502/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-05-02 04:27:58.000000 libbde-20240502/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-05-02 04:27:58.000000 libbde-20240502/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-05-02 04:27:58.000000 libbde-20240502/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34258 2024-05-02 04:28:20.000000 libbde-20240502/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-05-02 04:27:58.000000 libbde-20240502/libcthreads/libcthreads_queue.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-05-02 04:28:20.000000 libbde-20240502/test-driver
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:30.000000 libbde-20240502/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-05-02 04:27:55.000000 libbde-20240502/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-02 04:27:55.000000 libbde-20240502/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-05-02 04:27:55.000000 libbde-20240502/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2024-05-02 04:27:55.000000 libbde-20240502/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-02 04:27:55.000000 libbde-20240502/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-02 04:27:55.000000 libbde-20240502/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-02 04:27:55.000000 libbde-20240502/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-05-02 04:27:55.000000 libbde-20240502/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-05-02 04:27:55.000000 libbde-20240502/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-02 04:27:55.000000 libbde-20240502/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-02 04:27:55.000000 libbde-20240502/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-02 04:27:55.000000 libbde-20240502/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31104 2024-05-02 04:28:20.000000 libbde-20240502/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-02 04:27:55.000000 libbde-20240502/libcpath/libcpath_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-02 04:27:55.000000 libbde-20240502/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-05-02 04:27:55.000000 libbde-20240502/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-05-02 04:27:55.000000 libbde-20240502/libcpath/libcpath_path.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2066 2023-12-03 08:56:43.000000 libbde-20240502/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      149 2024-05-02 04:03:22.000000 libbde-20240502/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7218 2024-05-02 03:56:49.000000 libbde-20240502/manuals/libbde.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2327 2024-05-02 03:56:49.000000 libbde-20240502/manuals/bdeinfo.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27858 2024-05-02 04:28:20.000000 libbde-20240502/manuals/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1958 2024-05-02 03:56:49.000000 libbde-20240502/manuals/bdemount.1
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15109 2024-05-02 03:57:30.000000 libbde-20240502/tests/bde_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6877 2024-05-02 03:57:30.000000 libbde-20240502/tests/bde_test_encryption_context.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3326 2024-05-02 03:56:49.000000 libbde-20240502/tests/test_bdeinfo.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5971 2024-05-02 03:57:30.000000 libbde-20240502/tests/bde_test_stretch_key.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6027 2024-05-02 03:57:30.000000 libbde-20240502/tests/bde_test_external_key.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4075 2024-05-02 04:01:13.000000 libbde-20240502/tests/test_tools.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2024-05-02 03:56:49.000000 libbde-20240502/tests/bde_test_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4606 2024-05-02 03:56:49.000000 libbde-20240502/tests/bde_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6204 2024-05-02 03:57:30.000000 libbde-20240502/tests/bde_test_metadata_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-02 03:56:49.000000 libbde-20240502/tests/bde_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3332 2024-05-02 03:58:00.000000 libbde-20240502/tests/pybde_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2803 2024-05-02 03:57:30.000000 libbde-20240502/tests/bde_test_key_protector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10040 2024-05-02 04:03:06.000000 libbde-20240502/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-02 03:56:49.000000 libbde-20240502/tests/bde_test_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16025 2024-05-02 03:57:30.000000 libbde-20240502/tests/bde_test_volume_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8504 2024-05-02 03:56:49.000000 libbde-20240502/tests/bde_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16764 2024-05-02 03:57:30.000000 libbde-20240502/tests/bde_test_sector_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20211 2024-05-02 03:57:30.000000 libbde-20240502/tests/bde_test_metadata.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1803 2024-05-02 03:56:49.000000 libbde-20240502/tests/bde_test_getopt.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-02 03:56:49.000000 libbde-20240502/tests/test_manpage.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4447 2024-05-02 03:56:49.000000 libbde-20240502/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16382 2024-05-02 03:57:30.000000 libbde-20240502/tests/bde_test_metadata_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8053 2024-05-02 03:57:30.000000 libbde-20240502/tests/bde_test_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6885 2024-05-02 03:57:30.000000 libbde-20240502/tests/bde_test_sector_data_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1977 2024-05-02 03:56:49.000000 libbde-20240502/tests/bde_test_functions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1527 2024-05-02 03:56:49.000000 libbde-20240502/tests/bde_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-05-02 03:56:49.000000 libbde-20240502/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16197 2024-05-02 03:57:30.000000 libbde-20240502/tests/bde_test_metadata_block_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4077 2024-05-02 03:56:49.000000 libbde-20240502/tests/bde_test_tools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5724 2024-05-02 03:57:30.000000 libbde-20240502/tests/bde_test_key.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15698 2024-05-02 03:56:49.000000 libbde-20240502/tests/bde_test_functions.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-02 03:56:49.000000 libbde-20240502/tests/bde_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4229 2024-05-02 03:56:49.000000 libbde-20240502/tests/bde_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11319 2024-05-02 03:57:30.000000 libbde-20240502/tests/bde_test_volume_master_key.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5618 2024-05-02 03:56:49.000000 libbde-20240502/tests/bde_test_tools_info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81609 2024-05-02 03:57:30.000000 libbde-20240502/tests/bde_test_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7158 2024-05-02 03:56:49.000000 libbde-20240502/tests/bde_test_password.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-05-02 03:56:49.000000 libbde-20240502/tests/bde_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-05-02 03:56:49.000000 libbde-20240502/tests/bde_test_libbde.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    75804 2024-05-02 04:28:20.000000 libbde-20240502/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2403 2024-05-02 03:56:49.000000 libbde-20240502/tests/bde_test_tools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6541 2024-05-02 03:57:30.000000 libbde-20240502/tests/bde_test_aes_ccm_encrypted_key.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-02 03:56:49.000000 libbde-20240502/tests/bde_test_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25495 2024-05-02 03:58:00.000000 libbde-20240502/tests/pybde_test_volume.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3059 2024-05-02 03:56:49.000000 libbde-20240502/tests/bde_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4527 2024-05-02 03:56:49.000000 libbde-20240502/tests/bde_test_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6031 2024-05-02 03:56:49.000000 libbde-20240502/tests/bde_test_password_keep.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4316 2024-05-02 04:00:46.000000 libbde-20240502/tests/test_library.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2210 2024-05-02 03:56:48.000000 libbde-20240502/ossfuzz/volume_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      962 2024-05-02 03:56:48.000000 libbde-20240502/ossfuzz/ossfuzz_libbde.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      894 2024-05-02 04:02:33.000000 libbde-20240502/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-05-02 03:56:48.000000 libbde-20240502/ossfuzz/ossfuzz_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33174 2024-05-02 04:28:20.000000 libbde-20240502/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-05-02 04:28:12.000000 libbde-20240502/ltmain.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:30.000000 libbde-20240502/libhmac/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47989 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_sha1_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_sha224.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50026 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_sha512_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14448 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_md5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2079 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_md5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1942 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9362 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14650 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_sha512.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45648 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_sha256_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_sha224.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1623 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2060 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_sha1.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3443 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_sha256_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1117 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45605 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_sha224_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_md5_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_sha256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3368 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_sha1_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33969 2024-05-02 04:28:20.000000 libbde-20240502/libhmac/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_sha256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3461 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_sha224_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3444 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_sha512_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_sha512.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14514 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_sha1.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40596 2024-05-02 04:28:04.000000 libbde-20240502/libhmac/libhmac_md5_context.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:30.000000 libbde-20240502/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-05-02 04:27:56.000000 libbde-20240502/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-05-02 04:27:56.000000 libbde-20240502/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-05-02 04:27:56.000000 libbde-20240502/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-05-02 04:27:56.000000 libbde-20240502/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-02 04:27:56.000000 libbde-20240502/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-05-02 04:27:56.000000 libbde-20240502/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-02 04:27:56.000000 libbde-20240502/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-05-02 04:27:56.000000 libbde-20240502/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-02 04:27:56.000000 libbde-20240502/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-05-02 04:27:56.000000 libbde-20240502/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-02 04:27:56.000000 libbde-20240502/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-05-02 04:27:56.000000 libbde-20240502/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-02 04:27:56.000000 libbde-20240502/libcsplit/libcsplit_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-02 04:27:56.000000 libbde-20240502/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-02 04:27:56.000000 libbde-20240502/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-05-02 04:27:56.000000 libbde-20240502/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32001 2024-05-02 04:28:20.000000 libbde-20240502/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-05-02 04:27:56.000000 libbde-20240502/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-05-02 04:27:56.000000 libbde-20240502/libcsplit/libcsplit_narrow_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:31.000000 libbde-20240502/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 08:57:24.000000 libbde-20240502/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 08:57:24.000000 libbde-20240502/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 08:57:24.000000 libbde-20240502/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 08:57:24.000000 libbde-20240502/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 08:57:24.000000 libbde-20240502/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 08:57:24.000000 libbde-20240502/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 08:57:24.000000 libbde-20240502/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 08:57:24.000000 libbde-20240502/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 08:57:24.000000 libbde-20240502/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2024-05-02 04:28:34.000000 libbde-20240502/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 08:57:24.000000 libbde-20240502/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 08:57:24.000000 libbde-20240502/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:30.000000 libbde-20240502/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-05-02 04:28:07.000000 libbde-20240502/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57585 2024-05-02 04:28:20.000000 libbde-20240502/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-05-02 04:28:07.000000 libbde-20240502/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41872 2024-05-02 04:28:19.000000 libbde-20240502/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:30.000000 libbde-20240502/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_split_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3075 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_split_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_value_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_split_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_value_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_binary_data.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_value_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_split_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_floating_point.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_binary_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_value_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36894 2024-05-02 04:28:20.000000 libbde-20240502/libfvalue/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84529 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_floating_point.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-05-02 04:28:03.000000 libbde-20240502/libfvalue/libfvalue_libuna.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:30.000000 libbde-20240502/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-02 04:27:54.000000 libbde-20240502/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-02 04:27:54.000000 libbde-20240502/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-05-02 04:27:54.000000 libbde-20240502/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-05-02 04:27:54.000000 libbde-20240502/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-05-02 04:27:54.000000 libbde-20240502/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-02 04:27:54.000000 libbde-20240502/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-05-02 04:27:54.000000 libbde-20240502/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-05-02 04:27:54.000000 libbde-20240502/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-05-02 04:27:54.000000 libbde-20240502/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-05-02 04:27:54.000000 libbde-20240502/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-05-02 04:27:54.000000 libbde-20240502/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30942 2024-05-02 04:28:20.000000 libbde-20240502/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-02 04:27:54.000000 libbde-20240502/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-05-02 04:27:54.000000 libbde-20240502/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:29.000000 libbde-20240502/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-05-02 04:27:50.000000 libbde-20240502/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-05-02 04:27:50.000000 libbde-20240502/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-02 04:27:50.000000 libbde-20240502/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-05-02 04:27:50.000000 libbde-20240502/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-05-02 04:27:50.000000 libbde-20240502/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-02 04:27:50.000000 libbde-20240502/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-05-02 04:27:50.000000 libbde-20240502/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-05-02 04:27:50.000000 libbde-20240502/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-05-02 04:27:50.000000 libbde-20240502/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-02 04:27:50.000000 libbde-20240502/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-02 04:27:50.000000 libbde-20240502/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30409 2024-05-02 04:28:20.000000 libbde-20240502/libcerror/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:30.000000 libbde-20240502/libfdatetime/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5406 2024-05-02 04:28:00.000000 libbde-20240502/libfdatetime/libfdatetime_floatingtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34352 2024-05-02 04:28:00.000000 libbde-20240502/libfdatetime/libfdatetime_nsf_timedate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1887 2024-05-02 04:28:00.000000 libbde-20240502/libfdatetime/libfdatetime_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33399 2024-05-02 04:28:00.000000 libbde-20240502/libfdatetime/libfdatetime_floatingtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1220 2024-05-02 04:28:00.000000 libbde-20240502/libfdatetime/libfdatetime_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5010 2024-05-02 04:28:00.000000 libbde-20240502/libfdatetime/libfdatetime_hfs_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4182 2024-05-02 04:28:00.000000 libbde-20240502/libfdatetime/libfdatetime_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31774 2024-05-02 04:28:00.000000 libbde-20240502/libfdatetime/libfdatetime_hfs_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1144 2024-05-02 04:28:00.000000 libbde-20240502/libfdatetime/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35109 2024-05-02 04:28:00.000000 libbde-20240502/libfdatetime/libfdatetime_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4993 2024-05-02 04:28:00.000000 libbde-20240502/libfdatetime/libfdatetime_systemtime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-02 04:28:00.000000 libbde-20240502/libfdatetime/libfdatetime_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50166 2024-05-02 04:28:00.000000 libbde-20240502/libfdatetime/libfdatetime_posix_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1440 2024-05-02 04:28:00.000000 libbde-20240502/libfdatetime/libfdatetime_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5342 2024-05-02 04:28:00.000000 libbde-20240502/libfdatetime/libfdatetime_fat_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41822 2024-05-02 04:28:00.000000 libbde-20240502/libfdatetime/libfdatetime_systemtime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5761 2024-05-02 04:28:00.000000 libbde-20240502/libfdatetime/libfdatetime_nsf_timedate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1450 2024-05-02 04:28:00.000000 libbde-20240502/libfdatetime/libfdatetime_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1154 2024-05-02 04:28:00.000000 libbde-20240502/libfdatetime/libfdatetime_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2966 2024-05-02 04:28:00.000000 libbde-20240502/libfdatetime/libfdatetime_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5771 2024-05-02 04:28:00.000000 libbde-20240502/libfdatetime/libfdatetime_posix_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3131 2024-05-02 04:28:00.000000 libbde-20240502/libfdatetime/libfdatetime_date_time_values.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5340 2024-05-02 04:28:00.000000 libbde-20240502/libfdatetime/libfdatetime_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53085 2024-05-02 04:28:00.000000 libbde-20240502/libfdatetime/libfdatetime_date_time_values.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-05-02 04:28:00.000000 libbde-20240502/libfdatetime/libfdatetime_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33993 2024-05-02 04:28:20.000000 libbde-20240502/libfdatetime/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31754 2024-05-02 04:28:00.000000 libbde-20240502/libfdatetime/libfdatetime_fat_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56913 2024-05-02 04:28:16.000000 libbde-20240502/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8402 2024-05-02 03:56:45.000000 libbde-20240502/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      408 2024-05-02 04:50:32.495825 libbde-20240502/PKG-INFO
```

### Comparing `libbde-20240223/bdetools/mount_dokan.c` & `libbde-20240502/bdetools/mount_dokan.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/mount_file_system.h` & `libbde-20240502/bdetools/mount_file_system.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/bdetools_libuna.h` & `libbde-20240502/bdetools/bdetools_libuna.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/mount_fuse.c` & `libbde-20240502/bdetools/mount_fuse.c`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 #include "bdetools_libcnotify.h"
 #include "bdetools_unused.h"
 #include "mount_fuse.h"
 #include "mount_handle.h"
 
 extern mount_handle_t *bdemount_mount_handle;
 
-#if defined( HAVE_LIBFUSE ) || defined( HAVE_LIBOSXFUSE )
+#if defined( HAVE_LIBFUSE ) || defined( HAVE_LIBFUSE3 ) || defined( HAVE_LIBOSXFUSE )
 
 #if ( SIZEOF_OFF_T != 8 ) && ( SIZEOF_OFF_T != 4 )
 #error Size of off_t not supported
 #endif
 
 /* Sets the values in a stat info structure
  * The time values are a signed 64-bit POSIX date and time value in number of nanoseconds
@@ -251,19 +251,28 @@
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
 		 "%s: unable to set stat info.",
 		 function );
 
 		return( -1 );
 	}
+#if defined( HAVE_LIBFUSE3 )
+	if( filler(
+	     buffer,
+	     name,
+	     stat_info,
+	     0,
+	     0 ) == 1 )
+#else
 	if( filler(
 	     buffer,
 	     name,
 	     stat_info,
 	     0 ) == 1 )
+#endif
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_SET_FAILED,
 		 "%s: unable to set directory entry.",
 		 function );
@@ -651,34 +660,48 @@
 	}
 	return( result );
 }
 
 /* Reads a directory
  * Returns 0 if successful or a negative errno value otherwise
  */
+#if defined( HAVE_LIBFUSE3 )
+int mount_fuse_readdir(
+     const char *path,
+     void *buffer,
+     fuse_fill_dir_t filler,
+     off_t offset BDETOOLS_ATTRIBUTE_UNUSED,
+     struct fuse_file_info *file_info BDETOOLS_ATTRIBUTE_UNUSED,
+     enum fuse_readdir_flags flags BDETOOLS_ATTRIBUTE_UNUSED )
+#else
 int mount_fuse_readdir(
      const char *path,
      void *buffer,
      fuse_fill_dir_t filler,
      off_t offset BDETOOLS_ATTRIBUTE_UNUSED,
      struct fuse_file_info *file_info BDETOOLS_ATTRIBUTE_UNUSED )
+#endif
 {
 	struct stat *stat_info                = NULL;
 	libcerror_error_t *error              = NULL;
 	mount_file_entry_t *parent_file_entry = NULL;
 	mount_file_entry_t *sub_file_entry    = NULL;
 	static char *function                 = "mount_fuse_readdir";
 	char *name                            = NULL;
 	size_t name_size                      = 0;
 	int number_of_sub_file_entries        = 0;
 	int result                            = 0;
 	int sub_file_entry_index              = 0;
 
 	BDETOOLS_UNREFERENCED_PARAMETER( offset )
 
+#if defined( HAVE_LIBFUSE3 )
+	BDETOOLS_UNREFERENCED_PARAMETER( flags )
+#endif
+
 #if defined( HAVE_DEBUG_OUTPUT )
 	if( libcnotify_verbose != 0 )
 	{
 		libcnotify_printf(
 		 "%s: %s\n",
 		 function,
 		 path );
@@ -1040,28 +1063,39 @@
 	}
 	return( result );
 }
 
 /* Retrieves the file stat info
  * Returns 0 if successful or a negative errno value otherwise
  */
+#if defined( HAVE_LIBFUSE3 )
+int mount_fuse_getattr(
+     const char *path,
+     struct stat *stat_info,
+     struct fuse_file_info *file_info BDETOOLS_ATTRIBUTE_UNUSED )
+#else
 int mount_fuse_getattr(
      const char *path,
      struct stat *stat_info )
+#endif
 {
 	libcerror_error_t *error       = NULL;
 	mount_file_entry_t *file_entry = NULL;
 	static char *function          = "mount_fuse_getattr";
 	size64_t file_size             = 0;
 	uint64_t access_time           = 0;
 	uint64_t inode_change_time     = 0;
 	uint64_t modification_time     = 0;
 	uint16_t file_mode             = 0;
 	int result                     = 0;
 
+#if defined( HAVE_LIBFUSE3 )
+	BDETOOLS_UNREFERENCED_PARAMETER( file_info )
+#endif
+
 #if defined( HAVE_DEBUG_OUTPUT )
 	if( libcnotify_verbose != 0 )
 	{
 		libcnotify_printf(
 		 "%s: %s\n",
 		 function,
 		 path );
@@ -1310,9 +1344,9 @@
 		 error );
 		libcerror_error_free(
 		 &error );
 	}
 	return;
 }
 
-#endif /* defined( HAVE_LIBFUSE ) || defined( HAVE_LIBOSXFUSE ) */
+#endif /* defined( HAVE_LIBFUSE ) || defined( HAVE_LIBFUSE3 ) || defined( HAVE_LIBOSXFUSE ) */
```

### Comparing `libbde-20240223/bdetools/bdetools_output.c` & `libbde-20240502/bdetools/bdetools_output.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/info_handle.h` & `libbde-20240502/bdetools/info_handle.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/mount_dokan.h` & `libbde-20240502/bdetools/mount_dokan.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/bdetools_libcdata.h` & `libbde-20240502/bdetools/bdetools_libcdata.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/bdetools_libcsplit.h` & `libbde-20240502/bdetools/bdetools_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/bdetools_libcnotify.h` & `libbde-20240502/bdetools/bdetools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/bdetools_input.h` & `libbde-20240502/bdetools/bdetools_input.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/mount_file_system.c` & `libbde-20240502/bdetools/mount_file_system.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/bdetools_getopt.h` & `libbde-20240502/bdetools/bdetools_getopt.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/bdetools_libclocale.h` & `libbde-20240502/bdetools/bdetools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/byte_size_string.c` & `libbde-20240502/bdetools/byte_size_string.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/Makefile.am` & `libbde-20240502/bdetools/Makefile.am`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -88,19 +88,17 @@
 	@LIBCDATA_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	../libbde/libbde.la \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on bdeinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(bdeinfo_SOURCES)
 	@echo "Running splint on bdemount ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(bdemount_SOURCES)
```

### Comparing `libbde-20240223/bdetools/bdetools_output.h` & `libbde-20240502/bdetools/bdetools_output.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/bdetools_signal.c` & `libbde-20240502/bdetools/bdetools_signal.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/mount_file_entry.c` & `libbde-20240502/bdetools/mount_file_entry.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/info_handle.c` & `libbde-20240502/bdetools/info_handle.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/mount_file_entry.h` & `libbde-20240502/bdetools/mount_file_entry.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/bdetools_unused.h` & `libbde-20240502/bdetools/bdetools_unused.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/bdetools_libbde.h` & `libbde-20240502/bdetools/bdetools_libbde.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/bdetools_libbfio.h` & `libbde-20240502/bdetools/bdetools_libbfio.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/bdeinfo.c` & `libbde-20240502/bdetools/bdeinfo.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/bdetools_i18n.h` & `libbde-20240502/bdetools/bdetools_i18n.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/mount_handle.h` & `libbde-20240502/bdetools/mount_handle.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/bdetools_input.c` & `libbde-20240502/bdetools/bdetools_input.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/bdetools_libfdatetime.h` & `libbde-20240502/bdetools/bdetools_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/mount_handle.c` & `libbde-20240502/bdetools/mount_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1169,15 +1169,15 @@
 	{
 		fprintf(
 		 stdout,
 		 "Volume is locked and a password is needed to unlock it.\n\n" );
 
 		if( bdetools_prompt_for_password(
 		     stdout,
-		     "Password",
+		     _SYSTEM_STRING( "Password" ),
 		     password,
 		     64,
 		     error ) != 1 )
 		{
 			fprintf(
 			 stderr,
 			 "Unable to retrieve password.\n" );
```

### Comparing `libbde-20240223/bdetools/bdetools_libcerror.h` & `libbde-20240502/bdetools/bdetools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/bdetools_libfguid.h` & `libbde-20240502/bdetools/bdetools_libfguid.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/bdetools_libcpath.h` & `libbde-20240502/bdetools/bdetools_libcpath.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/Makefile.in` & `libbde-20240502/bdetools/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -477,14 +477,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -547,16 +549,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -635,15 +637,16 @@
 	@LIBCDATA_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	../libbde/libbde.la \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -901,23 +904,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/bdeinfo.Po
+	-rm -f ./$(DEPDIR)/bdemount.Po
+	-rm -f ./$(DEPDIR)/bdetools_getopt.Po
+	-rm -f ./$(DEPDIR)/bdetools_input.Po
+	-rm -f ./$(DEPDIR)/bdetools_output.Po
+	-rm -f ./$(DEPDIR)/bdetools_signal.Po
+	-rm -f ./$(DEPDIR)/byte_size_string.Po
+	-rm -f ./$(DEPDIR)/info_handle.Po
+	-rm -f ./$(DEPDIR)/mount_dokan.Po
+	-rm -f ./$(DEPDIR)/mount_file_entry.Po
+	-rm -f ./$(DEPDIR)/mount_file_system.Po
+	-rm -f ./$(DEPDIR)/mount_fuse.Po
+	-rm -f ./$(DEPDIR)/mount_handle.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1013,17 +1031,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on bdeinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(bdeinfo_SOURCES)
 	@echo "Running splint on bdemount ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(bdemount_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libbde-20240223/bdetools/bdetools_signal.h` & `libbde-20240502/bdetools/bdetools_signal.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/bdetools_getopt.c` & `libbde-20240502/bdetools/bdetools_getopt.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/byte_size_string.h` & `libbde-20240502/bdetools/byte_size_string.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/bdetools/bdemount.c` & `libbde-20240502/bdetools/bdemount.c`

 * *Files 2% similar despite different names*

```diff
@@ -153,19 +153,27 @@
 	char *program                                = "bdemount";
 	system_integer_t option                      = 0;
 	size_t path_prefix_size                      = 0;
 	int result                                   = 0;
 	int unattended_mode                          = 0;
 	int verbose                                  = 0;
 
-#if defined( HAVE_LIBFUSE ) || defined( HAVE_LIBOSXFUSE )
+#if defined( HAVE_LIBFUSE ) || defined( HAVE_LIBFUSE3 ) || defined( HAVE_LIBOSXFUSE )
 	struct fuse_operations bdemount_fuse_operations;
 
+#if defined( HAVE_LIBFUSE3 )
+	/* Need to set this to 1 even if there no arguments, otherwise this causes
+	 * fuse: empty argv passed to fuse_session_new()
+	 */
+	char *fuse_argv[ 2 ]                         = { program, NULL };
+	struct fuse_args bdemount_fuse_arguments     = FUSE_ARGS_INIT(1, fuse_argv);
+#else
 	struct fuse_args bdemount_fuse_arguments     = FUSE_ARGS_INIT(0, NULL);
 	struct fuse_chan *bdemount_fuse_channel      = NULL;
+#endif
 	struct fuse *bdemount_fuse_handle            = NULL;
 
 #elif defined( HAVE_LIBDOKAN )
 	DOKAN_OPERATIONS bdemount_dokan_operations;
 	DOKAN_OPTIONS bdemount_dokan_options;
 #endif
 
@@ -423,15 +431,15 @@
 	{
 		fprintf(
 		 stderr,
 		 "Unable to unlock source volume\n" );
 
 		goto on_error;
 	}
-#if defined( HAVE_LIBFUSE ) || defined( HAVE_LIBOSXFUSE )
+#if defined( HAVE_LIBFUSE ) || defined( HAVE_LIBFUSE3 ) || defined( HAVE_LIBOSXFUSE )
 	if( option_extended_options != NULL )
 	{
 		/* This argument is required but ignored
 		 */
 		if( fuse_opt_add_arg(
 		     &bdemount_fuse_arguments,
 		     "" ) != 0 )
@@ -479,14 +487,42 @@
 	bdemount_fuse_operations.release    = &mount_fuse_release;
 	bdemount_fuse_operations.opendir    = &mount_fuse_opendir;
 	bdemount_fuse_operations.readdir    = &mount_fuse_readdir;
 	bdemount_fuse_operations.releasedir = &mount_fuse_releasedir;
 	bdemount_fuse_operations.getattr    = &mount_fuse_getattr;
 	bdemount_fuse_operations.destroy    = &mount_fuse_destroy;
 
+#if defined( HAVE_LIBFUSE3 )
+	bdemount_fuse_handle = fuse_new(
+	                        &bdemount_fuse_arguments,
+	                        &bdemount_fuse_operations,
+	                        sizeof( struct fuse_operations ),
+	                        bdemount_mount_handle );
+
+	if( bdemount_fuse_handle == NULL )
+	{
+		fprintf(
+		 stderr,
+		 "Unable to create fuse handle.\n" );
+
+		goto on_error;
+	}
+	result = fuse_mount(
+	          bdemount_fuse_handle,
+	          mount_point );
+
+	if( result != 0 )
+	{
+		fprintf(
+		 stderr,
+		 "Unable to fuse mount file system.\n" );
+
+		goto on_error;
+	}
+#else
 	bdemount_fuse_channel = fuse_mount(
 	                         mount_point,
 	                         &bdemount_fuse_arguments );
 
 	if( bdemount_fuse_channel == NULL )
 	{
 		fprintf(
@@ -506,14 +542,16 @@
 	{
 		fprintf(
 		 stderr,
 		 "Unable to create fuse handle.\n" );
 
 		goto on_error;
 	}
+#endif /* defined( HAVE_LIBFUSE3 ) */
+
 	if( verbose == 0 )
 	{
 		if( fuse_daemonize(
 		     0 ) != 0 )
 		{
 			fprintf(
 			 stderr,
@@ -560,18 +598,22 @@
 	{
 		fprintf(
 		 stderr,
 		 "Unable to clear dokan options.\n" );
 
 		goto on_error;
 	}
-	bdemount_dokan_options.Version     = DOKAN_VERSION;
-	bdemount_dokan_options.ThreadCount = 0;
-	bdemount_dokan_options.MountPoint  = mount_point;
+	bdemount_dokan_options.Version    = DOKAN_VERSION;
+	bdemount_dokan_options.MountPoint = mount_point;
 
+#if DOKAN_MINIMUM_COMPATIBLE_VERSION >= 200
+	bdemount_dokan_options.SingleThread = TRUE;
+#else
+	bdemount_dokan_options.ThreadCount  = 0;
+#endif
 	if( verbose != 0 )
 	{
 		bdemount_dokan_options.Options |= DOKAN_OPTION_STDERR;
 #if defined( HAVE_DEBUG_OUTPUT )
 		bdemount_dokan_options.Options |= DOKAN_OPTION_DEBUG;
 #endif
 	}
@@ -633,18 +675,24 @@
 	bdemount_dokan_operations.GetVolumeInformation = &mount_dokan_GetVolumeInformation;
 	bdemount_dokan_operations.Unmounted            = NULL;
 	bdemount_dokan_operations.FindStreams          = NULL;
 	bdemount_dokan_operations.Mounted              = NULL;
 
 #endif /* ( DOKAN_VERSION >= 600 ) && ( DOKAN_VERSION < 800 ) */
 
+#if DOKAN_MINIMUM_COMPATIBLE_VERSION >= 200
+	DokanInit();
+#endif
 	result = DokanMain(
 	          &bdemount_dokan_options,
 	          &bdemount_dokan_operations );
 
+#if DOKAN_MINIMUM_COMPATIBLE_VERSION >= 200
+	DokanShutdown();
+#endif
 	switch( result )
 	{
 		case DOKAN_SUCCESS:
 			break;
 
 		case DOKAN_ERROR:
 			fprintf(
@@ -694,25 +742,25 @@
 #else
 	fprintf(
 	 stderr,
 	 "No sub system to mount BDE format.\n" );
 
 	return( EXIT_FAILURE );
 
-#endif /* defined( HAVE_LIBFUSE ) || defined( HAVE_LIBOSXFUSE ) */
+#endif /* defined( HAVE_LIBFUSE ) || defined( HAVE_LIBFUSE3 ) || defined( HAVE_LIBOSXFUSE ) */
 
 on_error:
 	if( error != NULL )
 	{
 		libcnotify_print_error_backtrace(
 		 error );
 		libcerror_error_free(
 		 &error );
 	}
-#if defined( HAVE_LIBFUSE ) || defined( HAVE_LIBOSXFUSE )
+#if defined( HAVE_LIBFUSE ) || defined( HAVE_LIBFUSE3 ) || defined( HAVE_LIBOSXFUSE )
 	if( bdemount_fuse_handle != NULL )
 	{
 		fuse_destroy(
 		 bdemount_fuse_handle );
 	}
 	fuse_opt_free_args(
 	 &bdemount_fuse_arguments );
```

### Comparing `libbde-20240223/bdetools/mount_fuse.h` & `libbde-20240502/bdetools/mount_fuse.h`

 * *Files 15% similar despite different names*

```diff
@@ -21,36 +21,46 @@
 
 #if !defined( _MOUNT_FUSE_H )
 #define _MOUNT_FUSE_H
 
 #include <common.h>
 #include <types.h>
 
-#if defined( HAVE_LIBFUSE ) || defined( HAVE_LIBOSXFUSE )
+#if defined( HAVE_LIBFUSE ) || defined( HAVE_LIBFUSE3 ) || defined( HAVE_LIBOSXFUSE )
+
+#if !defined( FUSE_USE_VERSION ) && !defined( CYGFUSE )
+
+/* Ensure FUSE_USE_VERSION is defined before including fuse.h
+ */
+#if defined( HAVE_LIBFUSE3 )
+#define FUSE_USE_VERSION	30
+#else
 #define FUSE_USE_VERSION	26
+#endif
 
-#if defined( HAVE_LIBFUSE )
-#include <fuse.h>
+#endif /* !defined( FUSE_USE_VERSION ) && !defined( CYGFUSE ) */
 
+#if defined( HAVE_LIBFUSE ) || defined( HAVE_LIBFUSE3 )
+#include <fuse.h>
 #elif defined( HAVE_LIBOSXFUSE )
 #include <osxfuse/fuse.h>
 #endif
 
-#endif /* defined( HAVE_LIBFUSE ) || defined( HAVE_LIBOSXFUSE ) */
+#endif /* defined( HAVE_LIBFUSE ) || defined( HAVE_LIBFUSE3 ) || defined( HAVE_LIBOSXFUSE ) */
 
 #include "bdetools_libbde.h"
 #include "bdetools_libcerror.h"
 #include "mount_file_entry.h"
 #include "mount_handle.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-#if defined( HAVE_LIBFUSE ) || defined( HAVE_LIBOSXFUSE )
+#if defined( HAVE_LIBFUSE ) || defined( HAVE_LIBFUSE3 ) || defined( HAVE_LIBOSXFUSE )
 
 int mount_fuse_set_stat_info(
      struct stat *stat_info,
      size64_t size,
      uint16_t file_mode,
      int64_t access_time,
      int64_t inode_change_time,
@@ -80,33 +90,50 @@
      const char *path,
      struct fuse_file_info *file_info );
 
 int mount_fuse_opendir(
      const char *path,
      struct fuse_file_info *file_info );
 
+#if defined( HAVE_LIBFUSE3 )
+int mount_fuse_readdir(
+     const char *path,
+     void *buffer,
+     fuse_fill_dir_t filler,
+     off_t offset,
+     struct fuse_file_info *file_info,
+     enum fuse_readdir_flags flags );
+#else
 int mount_fuse_readdir(
      const char *path,
      void *buffer,
      fuse_fill_dir_t filler,
      off_t offset,
      struct fuse_file_info *file_info );
+#endif
 
 int mount_fuse_releasedir(
      const char *path,
      struct fuse_file_info *file_info );
 
+#if defined( HAVE_LIBFUSE3 )
+int mount_fuse_getattr(
+     const char *path,
+     struct stat *stat_info,
+     struct fuse_file_info *file_info );
+#else
 int mount_fuse_getattr(
      const char *path,
      struct stat *stat_info );
+#endif
 
 void mount_fuse_destroy(
       void *private_data );
 
-#endif /* defined( HAVE_LIBFUSE ) || defined( HAVE_LIBOSXFUSE ) */
+#endif /* defined( HAVE_LIBFUSE ) || defined( HAVE_LIBFUSE3 ) || defined( HAVE_LIBOSXFUSE ) */
 
 #if defined( __cplusplus )
 }
 #endif
 
 #endif /* !defined( _MOUNT_FUSE_H ) */
```

### Comparing `libbde-20240223/COPYING` & `libbde-20240502/COPYING`

 * *Files identical despite different names*

### Comparing `libbde-20240223/install-sh` & `libbde-20240502/install-sh`

 * *Files identical despite different names*

### Comparing `libbde-20240223/depcomp` & `libbde-20240502/depcomp`

 * *Files identical despite different names*

### Comparing `libbde-20240223/pybde/pybde_key_protector.h` & `libbde-20240502/pybde/pybde_key_protector.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/pybde/pybde_volume.h` & `libbde-20240502/pybde/pybde_volume.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/pybde/pybde_integer.c` & `libbde-20240502/pybde/pybde_integer.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/pybde/pybde_python.h` & `libbde-20240502/pybde/pybde_python.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/pybde/pybde_libbde.h` & `libbde-20240502/pybde/pybde_libbde.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/pybde/pybde_file_object_io_handle.h` & `libbde-20240502/pybde/pybde_file_object_io_handle.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/pybde/pybde.h` & `libbde-20240502/pybde/pybde.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/pybde/pybde_integer.h` & `libbde-20240502/pybde/pybde_integer.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/pybde/pybde_guid.c` & `libbde-20240502/pybde/pybde_guid.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/pybde/pybde_error.c` & `libbde-20240502/pybde/pybde_error.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/pybde/pybde_encryption_methods.c` & `libbde-20240502/pybde/pybde_encryption_methods.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/pybde/pybde_libclocale.h` & `libbde-20240502/pybde/pybde_libclocale.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/pybde/Makefile.am` & `libbde-20240502/pybde/Makefile.am`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_PYTHON
 AM_CFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -48,13 +48,11 @@
 	@LIBFGUID_LIBADD@
 
 pybde_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pybde_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libbde-20240223/pybde/pybde_libbfio.h` & `libbde-20240502/pybde/pybde_libbfio.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/pybde/pybde_libfguid.h` & `libbde-20240502/pybde/pybde_libfguid.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/pybde/pybde_volume.c` & `libbde-20240502/pybde/pybde_volume.c`

 * *Files 0% similar despite different names*

```diff
@@ -96,22 +96,22 @@
 	  "unlock() -> Boolean\n"
 	  "\n"
 	  "Unlocks the volume." },
 
 	{ "read_buffer",
 	  (PyCFunction) pybde_volume_read_buffer,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read_buffer(size) -> Binary string\n"
+	  "read_buffer(size) -> Bytes\n"
 	  "\n"
 	  "Reads a buffer of unencrypted data." },
 
 	{ "read_buffer_at_offset",
 	  (PyCFunction) pybde_volume_read_buffer_at_offset,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read_buffer_at_offset(size, offset) -> Binary string\n"
+	  "read_buffer_at_offset(size, offset) -> Bytes\n"
 	  "\n"
 	  "Reads a buffer of unencrypted data at a specific offset." },
 
 	{ "seek_offset",
 	  (PyCFunction) pybde_volume_seek_offset,
 	  METH_VARARGS | METH_KEYWORDS,
 	  "seek_offset(offset, whence) -> None\n"
@@ -124,15 +124,15 @@
 	  "get_offset() -> Integer\n"
 	  "\n"
 	  "Retrieves the current offset within the unencrypted data." },
 
 	{ "read",
 	  (PyCFunction) pybde_volume_read_buffer,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read(size) -> Binary string\n"
+	  "read(size) -> Bytes\n"
 	  "\n"
 	  "Reads a buffer of unencrypted data." },
 
 	{ "seek",
 	  (PyCFunction) pybde_volume_seek_offset,
 	  METH_VARARGS | METH_KEYWORDS,
 	  "seek(offset, whence) -> None\n"
```

### Comparing `libbde-20240223/pybde/pybde_key_protector.c` & `libbde-20240502/pybde/pybde_key_protector.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/pybde/pybde.c` & `libbde-20240502/pybde/pybde.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/pybde/pybde_key_protection_types.c` & `libbde-20240502/pybde/pybde_key_protection_types.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/pybde/pybde_datetime.c` & `libbde-20240502/pybde/pybde_datetime.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/pybde/pybde_error.h` & `libbde-20240502/pybde/pybde_error.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/pybde/pybde_file_object_io_handle.c` & `libbde-20240502/pybde/pybde_file_object_io_handle.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/pybde/pybde_libcerror.h` & `libbde-20240502/pybde/pybde_libcerror.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/pybde/pybde_key_protectors.h` & `libbde-20240502/pybde/pybde_key_protectors.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/pybde/pybde_unused.h` & `libbde-20240502/pybde/pybde_unused.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/pybde/pybde_key_protectors.c` & `libbde-20240502/pybde/pybde_key_protectors.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/pybde/Makefile.in` & `libbde-20240502/pybde/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -522,14 +522,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -592,16 +594,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_PYTHON_TRUE@AM_CFLAGS = \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/include \
-@HAVE_PYTHON_TRUE@	-I$(top_srcdir)/common \
+@HAVE_PYTHON_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_PYTHON_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_PYTHON_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -640,15 +642,16 @@
 @HAVE_PYTHON_TRUE@	@LIBCFILE_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBBFIO_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBFGUID_LIBADD@
 
 @HAVE_PYTHON_TRUE@pybde_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pybde_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -962,24 +965,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-pyexecLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/pybde_la-pybde.Plo
+	-rm -f ./$(DEPDIR)/pybde_la-pybde_datetime.Plo
+	-rm -f ./$(DEPDIR)/pybde_la-pybde_encryption_methods.Plo
+	-rm -f ./$(DEPDIR)/pybde_la-pybde_error.Plo
+	-rm -f ./$(DEPDIR)/pybde_la-pybde_file_object_io_handle.Plo
+	-rm -f ./$(DEPDIR)/pybde_la-pybde_guid.Plo
+	-rm -f ./$(DEPDIR)/pybde_la-pybde_integer.Plo
+	-rm -f ./$(DEPDIR)/pybde_la-pybde_key_protection_types.Plo
+	-rm -f ./$(DEPDIR)/pybde_la-pybde_key_protector.Plo
+	-rm -f ./$(DEPDIR)/pybde_la-pybde_key_protectors.Plo
+	-rm -f ./$(DEPDIR)/pybde_la-pybde_volume.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1074,13 +1090,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-pyexecLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libbde-20240223/pybde/pybde_encryption_methods.h` & `libbde-20240502/pybde/pybde_encryption_methods.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/pybde/pybde_key_protection_types.h` & `libbde-20240502/pybde/pybde_key_protection_types.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/pybde/pybde_datetime.h` & `libbde-20240502/pybde/pybde_datetime.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/pybde/pybde_guid.h` & `libbde-20240502/pybde/pybde_guid.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcaes/libcaes_unused.h` & `libbde-20240502/libcaes/libcaes_unused.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcaes/libcaes_tweaked_context.h` & `libbde-20240502/libcaes/libcaes_tweaked_context.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcaes/libcaes_context.h` & `libbde-20240502/libcaes/libcaes_context.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcaes/libcaes_error.c` & `libbde-20240502/libcaes/libcaes_error.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcaes/libcaes_context.c` & `libbde-20240502/libcaes/libcaes_context.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcaes/libcaes_definitions.h` & `libbde-20240502/libcaes/libcaes_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 #if !defined( HAVE_LOCAL_LIBCAES )
 #include <libcaes/definitions.h>
 
 /* The definitions in <libcaes/definitions.h> are copied here
  * for local use of libcaes
  */
 #else
-#define LIBCAES_VERSION				20240114
+#define LIBCAES_VERSION				20240413
 
 /* The libcaes version string
  */
-#define LIBCAES_VERSION_STRING			"20240114"
+#define LIBCAES_VERSION_STRING			"20240413"
 
 /* The crypt modes
  */
 enum LIBCAES_CRYPT_MODES
 {
 	LIBCAES_CRYPT_MODE_DECRYPT		= 0,
 	LIBCAES_CRYPT_MODE_ENCRYPT		= 1
```

### Comparing `libbde-20240223/libcaes/Makefile.am` & `libbde-20240502/libcaes/Makefile.am`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 if HAVE_LOCAL_LIBCAES
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
-	@LIBCERROR_CPPFLAGS@ 
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
+	@LIBCERROR_CPPFLAGS@ \
+	@LIBCRYPTO_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcaes.la
 
 libcaes_la_SOURCES = \
 	libcaes_context.c libcaes_context.h \
 	libcaes_definitions.h \
 	libcaes_extern.h \
@@ -14,19 +15,17 @@
 	libcaes_libcerror.h \
 	libcaes_support.c libcaes_support.h \
 	libcaes_tweaked_context.c libcaes_tweaked_context.h \
 	libcaes_types.h \
 	libcaes_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcaes ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcaes_la_SOURCES)
```

### Comparing `libbde-20240223/libcaes/libcaes_error.h` & `libbde-20240502/libcaes/libcaes_error.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcaes/libcaes_types.h` & `libbde-20240502/libcaes/libcaes_types.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcaes/libcaes_extern.h` & `libbde-20240502/libcaes/libcaes_extern.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcaes/libcaes_support.h` & `libbde-20240502/libcaes/libcaes_support.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcaes/libcaes_libcerror.h` & `libbde-20240502/libcaes/libcaes_libcerror.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcaes/libcaes_support.c` & `libbde-20240502/libcaes/libcaes_support.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcaes/Makefile.in` & `libbde-20240502/libcaes/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -469,14 +469,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -539,31 +541,33 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCAES_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCAES_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCAES_TRUE@	-I$(top_srcdir)/common \
-@HAVE_LOCAL_LIBCAES_TRUE@	@LIBCERROR_CPPFLAGS@ 
+@HAVE_LOCAL_LIBCAES_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCAES_TRUE@	-I../common -I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCAES_TRUE@	@LIBCERROR_CPPFLAGS@ \
+@HAVE_LOCAL_LIBCAES_TRUE@	@LIBCRYPTO_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCAES_TRUE@noinst_LTLIBRARIES = libcaes.la
 @HAVE_LOCAL_LIBCAES_TRUE@libcaes_la_SOURCES = \
 @HAVE_LOCAL_LIBCAES_TRUE@	libcaes_context.c libcaes_context.h \
 @HAVE_LOCAL_LIBCAES_TRUE@	libcaes_definitions.h \
 @HAVE_LOCAL_LIBCAES_TRUE@	libcaes_extern.h \
 @HAVE_LOCAL_LIBCAES_TRUE@	libcaes_error.c libcaes_error.h \
 @HAVE_LOCAL_LIBCAES_TRUE@	libcaes_libcerror.h \
 @HAVE_LOCAL_LIBCAES_TRUE@	libcaes_support.c libcaes_support.h \
 @HAVE_LOCAL_LIBCAES_TRUE@	libcaes_tweaked_context.c libcaes_tweaked_context.h \
 @HAVE_LOCAL_LIBCAES_TRUE@	libcaes_types.h \
 @HAVE_LOCAL_LIBCAES_TRUE@	libcaes_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -766,24 +770,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcaes_context.Plo
+	-rm -f ./$(DEPDIR)/libcaes_error.Plo
+	-rm -f ./$(DEPDIR)/libcaes_support.Plo
+	-rm -f ./$(DEPDIR)/libcaes_tweaked_context.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -870,17 +880,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcaes ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcaes_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libbde-20240223/libcaes/libcaes_tweaked_context.c` & `libbde-20240502/libcaes/libcaes_tweaked_context.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfguid/libfguid_error.c` & `libbde-20240502/libfguid/libfguid_error.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfguid/libfguid_support.h` & `libbde-20240502/libfguid/libfguid_support.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfguid/libfguid_identifier.h` & `libbde-20240502/libfguid/libfguid_identifier.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfguid/libfguid_libcerror.h` & `libbde-20240502/libfguid/libfguid_libcerror.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfguid/Makefile.am` & `libbde-20240502/libfguid/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFGUID
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfguid.la
 
 libfguid_la_SOURCES = \
 	libfguid_definitions.h \
 	libfguid_extern.h \
@@ -13,19 +13,17 @@
 	libfguid_libcerror.h \
 	libfguid_identifier.c libfguid_identifier.h \
 	libfguid_support.c libfguid_support.h \
 	libfguid_types.h \
 	libfguid_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfguid ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfguid_la_SOURCES)
```

### Comparing `libbde-20240223/libfguid/libfguid_unused.h` & `libbde-20240502/libfguid/libfguid_unused.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfguid/libfguid_extern.h` & `libbde-20240502/libfguid/libfguid_extern.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfguid/libfguid_types.h` & `libbde-20240502/libfguid/libfguid_types.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfguid/libfguid_identifier.c` & `libbde-20240502/libfguid/libfguid_identifier.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfguid/libfguid_support.c` & `libbde-20240502/libfguid/libfguid_support.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfguid/libfguid_definitions.h` & `libbde-20240502/libfguid/libfguid_definitions.h`

 * *Files 6% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfguid/definitions.h> are copied here
  * for local use of libfguid
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFGUID_VERSION					20240116
+#define LIBFGUID_VERSION					20240415
 
 /* The version string
  */
-#define LIBFGUID_VERSION_STRING					"20240116"
+#define LIBFGUID_VERSION_STRING					"20240415"
 
 /* The byte order definitions
  */
 #define LIBFGUID_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define LIBFGUID_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The GUID identifier version definitions
```

### Comparing `libbde-20240223/libfguid/Makefile.in` & `libbde-20240502/libfguid/Makefile.in`

 * *Files 0% similar despite different names*

```diff
@@ -469,14 +469,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -539,30 +541,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFGUID_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFGUID_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFGUID_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFGUID_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFGUID_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFGUID_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFGUID_TRUE@noinst_LTLIBRARIES = libfguid.la
 @HAVE_LOCAL_LIBFGUID_TRUE@libfguid_la_SOURCES = \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_definitions.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_extern.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_error.c libfguid_error.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_libcerror.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_identifier.c libfguid_identifier.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_support.c libfguid_support.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_types.h \
 @HAVE_LOCAL_LIBFGUID_TRUE@	libfguid_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -764,24 +767,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfguid_error.Plo
+	-rm -f ./$(DEPDIR)/libfguid_identifier.Plo
+	-rm -f ./$(DEPDIR)/libfguid_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -867,17 +875,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfguid ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfguid_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libbde-20240223/libfguid/libfguid_error.h` & `libbde-20240502/libfguid/libfguid_error.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/m4/libcfile.m4` & `libbde-20240502/m4/libcfile.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcfile required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcfile is available
 dnl ac_libcfile_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCFILE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno],
     [ac_cv_libcfile=no],
     [ac_cv_libcfile=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcfile which returns "yes" and --with-libcfile= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect],
+      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcfile"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcfile],
           [1])
@@ -199,16 +201,17 @@
             libcfile_file_remove_wide,
             [ac_cv_libcfile_dummy=yes],
             [ac_cv_libcfile=no])
           ])
 
         ac_cv_libcfile_LIBADD="-lcfile"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes],
+      [test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcfile in directory: $ac_cv_with_libcfile],
         [1])
       ])
     ])
 
   AS_IF(
@@ -354,15 +357,15 @@
   AS_IF(
     [test "x$ac_cv_func_unlink" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: unlink],
       [1])
     ])
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
   ])
 
 dnl Function to detect how to enable libcfile
 AC_DEFUN([AX_LIBCFILE_CHECK_ENABLE],
```

### Comparing `libbde-20240223/m4/libfdatetime.m4` & `libbde-20240502/m4/libfdatetime.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfdatetime required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libfdatetime is available
 dnl ac_libfdatetime_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFDATETIME_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdatetime" = xno],
     [ac_cv_libfdatetime=no],
     [ac_cv_libfdatetime=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfdatetime which returns "yes" and --with-libfdatetime= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect],
+      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfdatetime"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfdatetime}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdatetime}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfdatetime],
           [1])
@@ -455,16 +457,17 @@
           fdatetime,
           libfdatetime_systemetime_copy_to_utf32_string_with_index,
           [ac_cv_libfdatetime_dummy=yes],
           [ac_cv_libfdatetime=no])
 
         ac_cv_libfdatetime_LIBADD="-lfdatetime"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_libfdatetime" != xyes],
+      [test "x$ac_cv_libfdatetime" != xyes && test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfdatetime in directory: $ac_cv_with_libfdatetime],
         [1])
       ])
     ])
 
   AS_IF(
@@ -486,15 +489,15 @@
     ])
   ])
 
 dnl Function to detect if libfdatetime dependencies are available
 AC_DEFUN([AX_LIBFDATETIME_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime";
+  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime -I\$(top_srcdir)/libfdatetime";
   ac_cv_libfdatetime_LIBADD="../libfdatetime/libfdatetime.la";
 
   ac_cv_libfdatetime=local
   ])
 
 dnl Function to detect how to enable libfdatetime
 AC_DEFUN([AX_LIBFDATETIME_CHECK_ENABLE],
```

### Comparing `libbde-20240223/m4/tests.m4` & `libbde-20240502/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libbde-20240223/m4/libcpath.m4` & `libbde-20240502/m4/libcpath.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcpath required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcpath is available
 dnl ac_libcpath_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCPATH_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno],
     [ac_cv_libcpath=no],
     [ac_cv_libcpath=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcpath which returns "yes" and --with-libcpath= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect],
+      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcpath"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcpath],
           [1])
@@ -148,16 +150,17 @@
             libcpath_path_make_directory_wide,
             [ac_cv_libcpath_dummy=yes],
             [ac_cv_libcpath=no])
           ])
 
         ac_cv_libcpath_LIBADD="-lcpath"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes],
+      [test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcpath in directory: $ac_cv_with_libcpath],
         [1])
       ])
     ])
 
   AS_IF(
@@ -269,15 +272,15 @@
     [AC_MSG_FAILURE(
       [Missing functions: getcwd],
       [1])
     ])
 
   AX_LIBCPATH_CHECK_FUNC_MKDIR
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
   ])
 
 dnl Function to detect how to enable libcpath
 AC_DEFUN([AX_LIBCPATH_CHECK_ENABLE],
```

### Comparing `libbde-20240223/m4/lib-prefix.m4` & `libbde-20240502/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libbde-20240223/m4/progtest.m4` & `libbde-20240502/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libbde-20240223/m4/libuna.m4` & `libbde-20240502/m4/libuna.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libuna or required headers and functions
 dnl
-dnl Version: 20230702
+dnl Version: 20240413
 
 dnl Function to detect if a specific libuna definition is available.
 AC_DEFUN([AX_LIBUNA_CHECK_DEFINITION],
   [AC_CACHE_CHECK(
     [if `$1' is defined],
     [$2],
     [AC_LANG_PUSH(C)
@@ -23,16 +23,18 @@
 dnl ac_libuna_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBUNA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno],
     [ac_cv_libuna=no],
     [ac_cv_libuna=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libuna which returns "yes" and --with-libuna= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect],
+      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libuna"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libuna],
           [1])
@@ -938,16 +940,17 @@
           [ac_cv_libuna_defines_compare_greater])
         AS_IF(
           [test "x$ac_cv_libuna_defines_utf16_stream_allow_unpaired_surrogate" != xyes],
           [ac_cv_libuna=no])
 
         ac_cv_libuna_LIBADD="-luna"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes],
+      [test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libuna in directory: $ac_cv_with_libuna],
         [1])
       ])
     ])
 
   AS_IF(
@@ -969,15 +972,15 @@
     ])
   ])
 
 dnl Function to detect if libuna dependencies are available
 AC_DEFUN([AX_LIBUNA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
   ])
 
 dnl Function to detect how to enable libuna
 AC_DEFUN([AX_LIBUNA_CHECK_ENABLE],
```

### Comparing `libbde-20240223/m4/gettext.m4` & `libbde-20240502/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libbde-20240223/m4/lib-ld.m4` & `libbde-20240502/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libbde-20240223/m4/libclocale.m4` & `libbde-20240502/m4/libclocale.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libclocale required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libclocale is available
 dnl ac_libclocale_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCLOCALE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno],
     [ac_cv_libclocale=no],
     [ac_cv_libclocale=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libclocale which returns "yes" and --with-libclocale= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect],
+      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libclocale"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libclocale],
           [1])
@@ -122,16 +124,17 @@
           clocale,
           libclocale_initialize,
           [ac_cv_libclocale_dummy=yes],
           [ac_cv_libclocale=no])
 
         ac_cv_libclocale_LIBADD="-lclocale"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes],
+      [test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libclocale in directory: $ac_cv_with_libclocale],
         [1])
       ])
     ])
 
   AS_IF(
@@ -216,15 +219,15 @@
     [AC_MSG_FAILURE(
       [Missing function: setlocale],
       [1])
     ])
 
   AX_LIBCLOCALE_CHECK_FUNC_LANGINFO_CODESET
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
   ])
 
 dnl Function to detect how to enable libclocale
 AC_DEFUN([AX_LIBCLOCALE_CHECK_ENABLE],
```

### Comparing `libbde-20240223/m4/libcdata.m4` & `libbde-20240502/m4/libcdata.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcdata required headers and functions
 dnl
-dnl Version: 20230108
+dnl Version: 20240413
 
 dnl Function to detect if libcdata is available
 dnl ac_libcdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno],
     [ac_cv_libcdata=no],
     [ac_cv_libcdata=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcdata which returns "yes" and --with-libcdata= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect],
+      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcdata"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcdata],
           [1])
@@ -493,16 +495,17 @@
           cdata,
           libcdata_tree_node_get_leaf_node_list,
           [ac_cv_libcdata_dummy=yes],
           [ac_cv_libcdata=no])
 
         ac_cv_libcdata_LIBADD="-lcdata"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes],
+      [test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcdata in directory: $ac_cv_with_libcdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -524,15 +527,15 @@
     ])
   ])
 
 dnl Function to detect if libcdata dependencies are available
 AC_DEFUN([AX_LIBCDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
   ])
 
 dnl Function to detect how to enable libcdata
 AC_DEFUN([AX_LIBCDATA_CHECK_ENABLE],
```

### Comparing `libbde-20240223/m4/libcsplit.m4` & `libbde-20240502/m4/libcsplit.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcsplit required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcsplit is available
 dnl ac_libcsplit_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno],
     [ac_cv_libcsplit=no],
     [ac_cv_libcsplit=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcsplit which returns "yes" and --with-libcsplit= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect],
+      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcsplit"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcsplit],
           [1])
@@ -143,16 +145,17 @@
             libcsplit_wide_split_string_set_segment_by_index,
             [ac_cv_libcsplit_dummy=yes],
             [ac_cv_libcsplit=no])
           ])
 
         ac_cv_libcsplit_LIBADD="-lcsplit"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes],
+      [test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcsplit in directory: $ac_cv_with_libcsplit],
         [1])
       ])
     ])
 
   AS_IF(
@@ -174,15 +177,15 @@
     ])
   ])
 
 dnl Function to detect if libcsplit dependencies are available
 AC_DEFUN([AX_LIBCSPLIT_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
   ])
 
 dnl Function to detect how to enable libcsplit
 AC_DEFUN([AX_LIBCSPLIT_CHECK_ENABLE],
```

### Comparing `libbde-20240223/m4/common.m4` & `libbde-20240502/m4/common.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for common headers and functions
 dnl
-dnl Version: 20181117
+dnl Version: 20240308
 
 dnl Function to test if a certain feature was disabled
 AC_DEFUN([AX_COMMON_ARG_DISABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
@@ -22,15 +22,15 @@
 dnl Function to test if a certain feature was enabled
 AC_DEFUN([AX_COMMON_ARG_ENABLE],
 [
   AC_ARG_ENABLE(
     [$1],
     [AS_HELP_STRING(
       [--enable-$1],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_enable_$2=$enableval],
     [ac_cv_enable_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to enable $3],
       [ac_cv_enable_$2],
       [ac_cv_enable_$2=$4])dnl
@@ -39,15 +39,15 @@
 dnl Function to test if the location of a certain feature was provided
 AC_DEFUN([AX_COMMON_ARG_WITH],
 [
   AC_ARG_WITH(
     [$1],
     [AS_HELP_STRING(
       [--with-$1[[=$5]]],
-      [$3 [default=$4]])],
+      [$3 @<:@default=$4@:>@])],
     [ac_cv_with_$2=$withval],
     [ac_cv_with_$2=$4])dnl
 
     AC_CACHE_CHECK(
       [whether to use $3],
       [ac_cv_with_$2],
       [ac_cv_with_$2=$4])dnl
```

### Comparing `libbde-20240223/m4/libcthreads.m4` & `libbde-20240502/m4/libcthreads.m4`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcthreads required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcthreads is available
 dnl ac_libcthreads_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCTHREADS_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno],
     [ac_cv_libcthreads=no],
     [ac_cv_libcthreads=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcthreads which returns "yes" and --with-libcthreads= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect],
+      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcthreads"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcthreads],
           [1])
@@ -244,15 +246,15 @@
           [ac_cv_libcthreads_dummy=yes],
           [ac_cv_libcthreads=no])
 
         ac_cv_libcthreads_LIBADD="-lcthreads"])
       ])
 
     AS_IF(
-      [test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes],
+      [test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcthreads in directory: $ac_cv_with_libcthreads],
         [1])
       ])
     ])
 
   AS_IF(
@@ -286,15 +288,15 @@
     [dnl Check for enabling pthread support
     AX_PTHREAD_CHECK_ENABLE
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread],
     [ac_cv_libcthreads_multi_threading="winapi"])
 
   AS_IF(
     [test "x$ac_cv_libcthreads_multi_threading" != xno],
-    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+    [ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local],
     [ac_cv_libcthreads=no])
   ])
 
 dnl Function to detect how to enable libcthreads
```

### Comparing `libbde-20240223/m4/ltversion.m4` & `libbde-20240502/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libbde-20240223/m4/ltsugar.m4` & `libbde-20240502/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libbde-20240223/m4/host-cpu-c-abi.m4` & `libbde-20240502/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libbde-20240223/m4/libfuse.m4` & `libbde-20240502/m4/libfuse.m4`

 * *Files 13% similar despite different names*

```diff
@@ -1,62 +1,90 @@
 dnl Checks for libfuse required headers and functions
 dnl
-dnl Version: 20220118
+dnl Version: 20240413
 
 dnl Function to detect if libfuse is available
 dnl ac_libfuse_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFUSE_CHECK_LIB],
-  [dnl Check if parameters were provided
-  AS_IF(
-    [test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_with_libfuse" != xauto-detect],
-    [AS_IF(
-      [test -d "$ac_cv_with_libfuse"],
-      [CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
-      LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"],
-      [AC_MSG_WARN([no such directory: $ac_cv_with_libfuse])
-      ])
-    ])
-
-  AS_IF(
-    [test "x$ac_cv_with_libfuse" = xno],
+  [AS_IF(
+    [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfuse" = xno],
     [ac_cv_libfuse=no],
-    [dnl Check for a pkg-config file
+    [dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfuse which returns "yes" and --with-libfuse= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"],
-      [PKG_CHECK_MODULES(
-        [fuse],
-        [fuse >= 2.6],
-        [ac_cv_libfuse=libfuse],
-        [ac_cv_libfuse=no])
+      [test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes],
+      [AS_IF(
+        [test -d "$ac_cv_with_libfuse"],
+        [CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"],
+        [AC_MSG_FAILURE(
+          [no such directory: $ac_cv_with_libfuse],
+          [1])
+        ])],
+      [dnl Check for a pkg-config file
+      AS_IF(
+        [test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"],
+        [PKG_CHECK_MODULES(
+          [fuse3],
+          [fuse3 >= 3.0],
+          [ac_cv_libfuse=libfuse3],
+          [ac_cv_libfuse=no])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xno],
+          [PKG_CHECK_MODULES(
+            [fuse],
+            [fuse >= 2.6],
+            [ac_cv_libfuse=libfuse],
+            [ac_cv_libfuse=no])
+          ])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse3],
+          [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse3_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse3_LIBS"])
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse],
+          [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"])
+        ])
       ])
 
+    backup_CPPFLAGS="$CPPFLAGS"
+
+    dnl Check for libfuse and libfuse3
     AS_IF(
-      [test "x$ac_cv_libfuse" = xlibfuse],
-      [ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS"
-      ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"],
+      [test "x$ac_cv_libfuse" != xlibfuse && test "x$ac_cv_libfuse" != xlibfuse3],
       [dnl Check for headers
-      AC_CHECK_HEADERS(
-        [fuse.h],
-        [ac_cv_header_fuse_h=yes],
-        [ac_cv_header_fuse_h=no])
 
-      dnl libfuse sometimes requires -D_FILE_OFFSET_BITS=64 to be set
-      dnl macFuse requires -DFUSE_USE_VERSION=26 to be set
+      CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=30"
+      AC_CHECK_HEADERS([fuse.h])
+
       AS_IF(
-        [test "x$ac_cv_header_fuse_h" = xno],
-        [AS_UNSET([ac_cv_header_fuse_h])
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64 -DFUSE_USE_VERSION=26"
+        [test "x$ac_cv_header_fuse_h" = xyes],
+        [ac_cv_libfuse=libfuse3],
+        [CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
         AC_CHECK_HEADERS([fuse.h])
-      ])
+
+        AS_IF(
+          [test "x$ac_cv_header_fuse_h" = xyes],
+          [ac_cv_libfuse=libfuse])
+        ])
 
       AS_IF(
         [test "x$ac_cv_header_fuse_h" = xno],
         [ac_cv_libfuse=no],
         [dnl Check for the individual functions
-        ac_cv_libfuse=libfuse
+        AC_CHECK_LIB(
+          fuse,
+          fuse_invalidate,
+          [ac_cv_libfuse=libfuse],
+          [ac_cv_libfuse=libfuse3])
 
         AC_CHECK_LIB(
           fuse,
           fuse_daemonize,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
@@ -71,32 +99,30 @@
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
           fuse,
           fuse_new,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
 
-        ac_cv_libfuse_LIBADD="-lfuse";
+        dnl libfuse and libfuse3 require -D_FILE_OFFSET_BITS=64 to be set
+        ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
+        AS_IF(
+          [test "x$ac_cv_libfuse" = xlibfuse3],
+          [ac_cv_libfuse_LIBADD="-lfuse3"],
+          [ac_cv_libfuse_LIBADD="-lfuse"])
         ])
       ])
 
     dnl Check for libosxfuse
     AS_IF(
       [test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno],
-      [CPPFLAGS="$CPPFLAGS -DFUSE_USE_VERSION=26"
+      [CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
       AC_CHECK_HEADERS([osxfuse/fuse.h])
 
-      dnl libosxfuse sometimes requires -D_FILE_OFFSET_BITS=64 to be set
-      AS_IF(
-        [test "x$ac_cv_header_osxfuse_fuse_h" = xno],
-        [AS_UNSET([ac_cv_header_osxfuse_fuse_h])
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64"
-        AC_CHECK_HEADERS([osxfuse/fuse.h])
-      ])
-
       AS_IF(
         [test "x$ac_cv_header_osxfuse_fuse_h" = xno],
         [ac_cv_libfuse=no],
         [dnl Check for the individual functions
         ac_cv_libfuse=libosxfuse
 
         AC_CHECK_LIB(
@@ -116,27 +142,46 @@
           [ac_cv_libfuse=no])
         AC_CHECK_LIB(
           osxfuse,
           fuse_new,
           [ac_cv_libfuse_dummy=yes],
           [ac_cv_libfuse=no])
 
+        dnl libosxfuse requires -D_FILE_OFFSET_BITS=64 to be set
+        ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
         ac_cv_libfuse_LIBADD="-losxfuse";
         ])
       ])
+
+    AS_IF(
+      [test "x$ac_cv_libfuse" != xyes && test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported libfuse in directory: $ac_cv_with_libfuse],
+        [1])
+      ])
+
+    CPPFLAGS="$backup_CPPFLAGS"
     ])
 
   AS_IF(
     [test "x$ac_cv_libfuse" = xlibfuse],
     [AC_DEFINE(
       [HAVE_LIBFUSE],
       [1],
       [Define to 1 if you have the 'fuse' library (-lfuse).])
     ])
   AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_DEFINE(
+      [HAVE_LIBFUSE3],
+      [1],
+      [Define to 1 if you have the 'fuse3' library (-lfuse3).])
+    ])
+  AS_IF(
     [test "x$ac_cv_libfuse" = xlibosxfuse],
     [AC_DEFINE(
       [HAVE_LIBOSXFUSE],
       [1],
       [Define to 1 if you have the 'osxfuse' library (-losxfuse).])
     ])
 
@@ -179,14 +224,20 @@
   AS_IF(
     [test "x$ac_cv_libfuse" = xlibfuse],
     [AC_SUBST(
       [ax_libfuse_pc_libs_private],
       [-lfuse])
     ])
   AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_SUBST(
+      [ax_libfuse_pc_libs_private],
+      [-lfuse3])
+    ])
+  AS_IF(
     [test "x$ac_cv_libfuse" = xlibosxfuse],
     [AC_SUBST(
       [ax_libfuse_pc_libs_private],
       [-losxfuse])
     ])
 
   AS_IF(
@@ -194,9 +245,18 @@
     [AC_SUBST(
       [ax_libfuse_spec_requires],
       [fuse-libs])
     AC_SUBST(
       [ax_libfuse_spec_build_requires],
       [fuse-devel])
     ])
+  AS_IF(
+    [test "x$ac_cv_libfuse" = xlibfuse3],
+    [AC_SUBST(
+      [ax_libfuse_spec_requires],
+      [fuse3-libs])
+    AC_SUBST(
+      [ax_libfuse_spec_build_requires],
+      [fuse3-devel])
+    ])
   ])
```

### Comparing `libbde-20240223/m4/libtool.m4` & `libbde-20240502/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libbde-20240223/m4/po.m4` & `libbde-20240502/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libbde-20240223/m4/libcerror.m4` & `libbde-20240502/m4/libcerror.m4`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcerror required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcerror is available
 dnl ac_libcerror_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCERROR_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno],
     [ac_cv_libcerror=no],
     [ac_cv_libcerror=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcerror which returns "yes" and --with-libcerror= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect],
+      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcerror"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcerror],
           [1])
@@ -95,16 +97,17 @@
           cerror,
           libcerror_system_set_error,
           [ac_cv_libcerror_dummy=yes],
           [ac_cv_libcerror=no])
 
         ac_cv_libcerror_LIBADD="-lcerror"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes],
+      [test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcerror in directory: $ac_cv_with_libcerror],
         [1])
       ])
     ])
 
   AS_IF(
@@ -162,15 +165,15 @@
       [test "x$ac_cv_func_strerror" != xyes],
       [AC_MSG_FAILURE(
         [Missing functions: strerror_r and strerror],
         [1])
       ])
     ])
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
   ])
 
 dnl Function to detect how to enable libcerror
 AC_DEFUN([AX_LIBCERROR_CHECK_ENABLE],
```

### Comparing `libbde-20240223/m4/libcnotify.m4` & `libbde-20240502/m4/libcnotify.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcnotify required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libcnotify is available
 dnl ac_libcnotify_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno],
     [ac_cv_libcnotify=no],
     [ac_cv_libcnotify=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcnotify which returns "yes" and --with-libcnotify= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect],
+      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcnotify"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcnotify],
           [1])
@@ -92,16 +94,17 @@
           cnotify,
           libcnotify_verbose_set,
           [ac_cv_libcnotify_dummy=yes],
           [ac_cv_libcnotify=no])
 
         ac_cv_libcnotify_LIBADD="-lcnotify"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes],
+      [test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcnotify in directory: $ac_cv_with_libcnotify],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
       [Missing headers: stdarg.h and varargs.h],
       [1])
     ])
 
   dnl Headers included in libcnotify/libcnotify_stream.c
   AC_CHECK_HEADERS([errno.h])
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
   ])
 
 dnl Function to detect how to enable libcnotify
 AC_DEFUN([AX_LIBCNOTIFY_CHECK_ENABLE],
```

### Comparing `libbde-20240223/m4/libfguid.m4` & `libbde-20240502/m4/libfguid.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfguid required headers and functions
 dnl
-dnl Version: 20190308
+dnl Version: 20240413
 
 dnl Function to detect if libfguid is available
 dnl ac_libfguid_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFGUID_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfguid" = xno],
     [ac_cv_libfguid=no],
     [ac_cv_libfguid=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfguid which returns "yes" and --with-libfguid= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect],
+      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfguid"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfguid}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfguid}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfguid],
           [1])
@@ -103,16 +105,17 @@
           fguid,
           libfguid_identifier_copy_to_utf32_string_with_index,
           [ac_cv_libfguid_dummy=yes],
           [ac_cv_libfguid=no])
 
         ac_cv_libfguid_LIBADD="-lfguid"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_libfguid" != xyes],
+      [test "x$ac_cv_libfguid" != xyes && test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfguid in directory: $ac_cv_with_libfguid],
         [1])
       ])
     ])
 
   AS_IF(
@@ -134,15 +137,15 @@
     ])
   ])
 
 dnl Function to detect if libfguid dependencies are available
 AC_DEFUN([AX_LIBFGUID_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
   ])
 
 
 dnl Function to detect how to enable libfguid
```

### Comparing `libbde-20240223/m4/libbfio.m4` & `libbde-20240502/m4/libbfio.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libbfio required headers and functions
 dnl
-dnl Version: 20201125
+dnl Version: 20240413
 
 dnl Function to detect if libbfio is available
 dnl ac_libbfio_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBBFIO_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno],
     [ac_cv_libbfio=no],
     [ac_cv_libbfio=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libbfio which returns "yes" and --with-libbfio= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect],
+      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libbfio"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libbfio],
           [1])
@@ -316,16 +318,17 @@
             libbfio_file_pool_open_wide,
             [ac_cv_libbfio_dummy=yes],
             [ac_cv_libbfio=no])
           ])
 
         ac_cv_libbfio_LIBADD="-lbfio"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes],
+      [test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libbfio in directory: $ac_cv_with_libbfio],
         [1])
       ])
     ])
 
   AS_IF(
@@ -347,15 +350,15 @@
     ])
   ])
 
 dnl Function to detect if libbfio dependencies are available
 AC_DEFUN([AX_LIBBFIO_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
   ])
 
 dnl Function to detect how to enable libbfio
 AC_DEFUN([AX_LIBBFIO_CHECK_ENABLE],
```

### Comparing `libbde-20240223/m4/libhmac.m4` & `libbde-20240502/m4/libhmac.m4`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libhmac required headers and functions
 dnl
-dnl Version: 20200104
+dnl Version: 20240413
 
 dnl Function to detect if libhmac is available
 dnl ac_libhmac_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBHMAC_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libhmac" = xno],
     [ac_cv_libhmac=no],
     [ac_cv_libhmac=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libhmac which returns "yes" and --with-libhmac= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect],
+      [test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect && test "x$ac_cv_with_libhmac" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libhmac"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libhmac}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libhmac}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libhmac],
           [1])
@@ -161,16 +163,17 @@
           hmac,
           libhmac_sha512_free,
           [ac_cv_libhmac_dummy=yes],
           [ac_cv_libhmac=no])
 
         ac_cv_libhmac_LIBADD="-lhmac"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect && test "x$ac_cv_libhmac" != xyes],
+      [test "x$ac_cv_libhmac" != xyes && test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect && test "x$ac_cv_with_libhmac" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libhmac in directory: $ac_cv_with_libhmac],
         [1])
       ])
     ])
 
   AS_IF(
@@ -240,15 +243,15 @@
     [ac_cv_libhmac_sha256=$ac_cv_libcrypto_sha256])
 
   AS_IF(
     [test "x$ac_cv_libcrypto" = xno || test "x$ac_cv_libcrypto_sha512" = xno],
     [ac_cv_libhmac_sha512=local],
     [ac_cv_libhmac_sha512=$ac_cv_libcrypto_sha512])
 
-  ac_cv_libhmac_CPPFLAGS="-I../libhmac";
+  ac_cv_libhmac_CPPFLAGS="-I../libhmac -I\$(top_srcdir)/libhmac";
   ac_cv_libhmac_LIBADD="../libhmac/libhmac.la";
 
   ac_cv_libhmac=local
   ])
 
 dnl Function to detect how to enable libhmac
 AC_DEFUN([AX_LIBHMAC_CHECK_ENABLE],
```

### Comparing `libbde-20240223/m4/intlmacosx.m4` & `libbde-20240502/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libbde-20240223/m4/lt~obsolete.m4` & `libbde-20240502/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libbde-20240223/m4/lib-link.m4` & `libbde-20240502/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libbde-20240223/m4/iconv.m4` & `libbde-20240502/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libbde-20240223/m4/ltoptions.m4` & `libbde-20240502/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libbde-20240223/m4/nls.m4` & `libbde-20240502/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libbde-20240223/m4/python.m4` & `libbde-20240502/m4/python.m4`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Functions for Python bindings
 dnl
-dnl Version: 20231119
+dnl Version: 20240418
 
 dnl Function to check if the python binary is available
 dnl "python${PYTHON_VERSION} python python# python#.#"
 AC_DEFUN([AX_PROG_PYTHON],
   [AS_IF(
     [test "x${PYTHON_VERSION}" != x],
     [ax_python_progs="python${PYTHON_VERSION}"],
@@ -72,18 +72,20 @@
     PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     AC_MSG_CHECKING(
       [for Python libraries])
     AC_MSG_RESULT(
       [$PYTHON_LDFLAGS])
 
-    dnl For CygWin add the -no-undefined linker flag
+    dnl For CygWin and MinGW add the -no-undefined linker flag
     AS_CASE(
-      [$host_os],
-      [cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [$build],
+      [*-*-cygwin*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-mingw*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
+      [*-*-msys*],[PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined"],
       [*],[])
 
     dnl Check for the existence of Python.h
     BACKUP_CPPFLAGS="${CPPFLAGS}"
     CPPFLAGS="${CPPFLAGS} ${PYTHON_INCLUDES}"
 
     AC_CHECK_HEADERS(
```

### Comparing `libbde-20240223/m4/libcrypto.m4` & `libbde-20240502/m4/libcrypto.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dnl Checks for libcrypto required headers and functions
 dnl
-dnl Version: 20231007
+dnl Version: 20240308
 
 dnl Function to detect whether openssl/evp.h can be used in combination with zlib.h
 AC_DEFUN([AX_LIBCRYPTO_CHECK_OPENSSL_EVP_ZLIB_COMPATIBILE],
   [AC_CACHE_CHECK(
     [if openssl/evp.h can be used in combination with zlib.h],
     [ac_cv_openssl_evp_zlib_compatible],
     [AC_LANG_PUSH(C)
@@ -619,16 +619,18 @@
 
 dnl Function to detect if libcrypto (openssl) dependencies are available
 AC_DEFUN([AX_LIBCRYPTO_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_openssl" = xno],
     [ac_cv_libcrypto=no],
     [dnl Check if the directory provided as parameter exists
+    dnl For both --with-openssl which returns "yes" and --with-openssl= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect],
+      [test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect && test "x$ac_cv_with_openssl" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_openssl"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_openssl}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_openssl}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_openssl],
           [1])
```

### Comparing `libbde-20240223/m4/libfvalue.m4` & `libbde-20240502/m4/libfvalue.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfvalue required headers and functions
 dnl
-dnl Version: 20200711
+dnl Version: 20240413
 
 dnl Function to detect if libfvalue is available
 dnl ac_libfvalue_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFVALUE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfvalue" = xno],
     [ac_cv_libfvalue=no],
     [ac_cv_libfvalue=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfvalue which returns "yes" and --with-libfvalue= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect],
+      [test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfvalue"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfvalue}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfvalue}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfvalue],
           [1])
@@ -585,16 +587,17 @@
           fvalue,
           libfvalue_value_type_set_data_strings_array,
           [ac_cv_libfvalue_dummy=yes],
           [ac_cv_libfvalue=no])
 
         ac_cv_libfvalue_LIBADD="-lfvalue"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_libfvalue" != xyes],
+      [test "x$ac_cv_libfvalue" != xyes && test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfvalue in directory: $ac_cv_with_libfvalue],
         [1])
       ])
     ])
 
   AS_IF(
@@ -616,15 +619,15 @@
     ])
   ])
 
 dnl Function to detect if libfvalue dependencies are available
 AC_DEFUN([AX_LIBFVALUE_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue";
+  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue -I\$(top_srcdir)/libfvalue";
   ac_cv_libfvalue_LIBADD="../libfvalue/libfvalue.la";
 
   ac_cv_libfvalue=local
   ])
 
 dnl Function to detect how to enable libfvalue
 AC_DEFUN([AX_LIBFVALUE_CHECK_ENABLE],
```

### Comparing `libbde-20240223/m4/types.m4` & `libbde-20240502/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libbde-20240223/m4/libfcache.m4` & `libbde-20240502/m4/libfcache.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libfcache required headers and functions
 dnl
-dnl Version: 20230115
+dnl Version: 20240413
 
 dnl Function to detect if libfcache is available
 dnl ac_libfcache_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFCACHE_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfcache" = xno],
     [ac_cv_libfcache=no],
     [ac_cv_libfcache=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfcache which returns "yes" and --with-libfcache= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect],
+      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfcache"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfcache}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfcache}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfcache],
           [1])
@@ -147,16 +149,17 @@
           fcache,
           libfcache_date_time_get_timestamp,
           [ac_cv_libfcache_dummy=yes],
           [ac_cv_libfcache=no])
 
         ac_cv_libfcache_LIBADD="-lfcache"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_libfcache" != xyes],
+      [test "x$ac_cv_libfcache" != xyes && test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfcache in directory: $ac_cv_with_libfcache],
         [1])
       ])
     ])
 
   AS_IF(
@@ -192,15 +195,15 @@
   AS_IF(
     [test "x$ac_cv_func_time" != xyes],
     [AC_MSG_FAILURE(
       [Missing function: time],
       [1])
     ])
 
-  ac_cv_libfcache_CPPFLAGS="-I../libfcache";
+  ac_cv_libfcache_CPPFLAGS="-I../libfcache -I\$(top_srcdir)/libfcache";
   ac_cv_libfcache_LIBADD="../libfcache/libfcache.la";
 
   ac_cv_libfcache=local
   ])
 
 dnl Function to detect how to enable libfcache
 AC_DEFUN([AX_LIBFCACHE_CHECK_ENABLE],
```

### Comparing `libbde-20240223/m4/pthread.m4` & `libbde-20240502/m4/pthread.m4`

 * *Files 18% similar despite different names*

```diff
@@ -1,183 +1,196 @@
 dnl Functions for pthread
 dnl
-dnl Version: 20130509
+dnl Version: 20240308
 
 dnl Function to detect if pthread is available
 AC_DEFUN([AX_PTHREAD_CHECK_LIB],
- [dnl Check if parameters were provided
- AS_IF(
-  [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect],
   [AS_IF(
-   [test -d "$ac_cv_with_pthread"],
-   [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
-   [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
-   ])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_with_pthread" = xno],
-  [ac_cv_pthread=no],
-  [dnl Check for headers
-  AC_CHECK_HEADERS([pthread.h])
+    [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno],
+    [ac_cv_pthread=no],
+    [ac_cv_pthread=check
+    dnl Check if parameters were provided
+    dnl For both --with-pthread which returns "yes" and --with-pthread= which returns ""
+    dnl treat them as auto-detection.
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AS_IF(
+        [test -d "$ac_cv_with_pthread"],
+        [CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"],
+        [AC_MSG_WARN([no such directory: $ac_cv_with_pthread])
+        ])
+      ])
+    ])
+
+    AS_IF(
+      [test "x$ac_cv_pthread" = xcheck],
+      [dnl Check for headers
+      AC_CHECK_HEADERS([pthread.h])
+
+      AS_IF(
+        [test "x$ac_cv_header_pthread_h" = xno],
+        [ac_cv_pthread=no],
+        [dnl Check for the individual functions
+        ac_cv_pthread=pthread
+
+        dnl Thread functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_create,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_exit,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_join,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Condition functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_broadcast,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_signal,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_cond_wait,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Mutex functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_lock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_trylock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_mutex_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        dnl Read/Write lock functions
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_init,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_destroy,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_rdlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_wrlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+        AC_CHECK_LIB(
+          pthread,
+          pthread_rwlock_unlock,
+          [ac_pthread_dummy=yes],
+          [ac_cv_pthread=no])
+
+        ac_cv_pthread_LIBADD="-lpthread";
+      ])
+
+    AS_IF(
+      [test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported pthread in directory: $ac_cv_with_pthread],
+        [1])
+      ])
+    ])
 
   AS_IF(
-   [test "x$ac_cv_header_pthread_h" = xno],
-   [ac_cv_pthread=no],
-   [dnl Check for the individual functions
-   ac_cv_pthread=pthread
-
-   dnl Thread functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_create,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_exit,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_join,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Condition functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_broadcast,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_signal,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_cond_wait,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Mutex functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_lock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_trylock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_mutex_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   dnl Read/Write lock functions
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_init,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_destroy,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_rdlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_wrlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-   AC_CHECK_LIB(
-    pthread,
-    pthread_rwlock_unlock,
-    [ac_pthread_dummy=yes],
-    [ac_cv_pthread=no])
-
-   ac_cv_pthread_LIBADD="-lpthread";
-   ])
-  ])
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_DEFINE(
+      [HAVE_PTHREAD],
+      [1],
+      [Define to 1 if you have the 'pthread' library (-lpthread).])
+    ])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_DEFINE(
-   [HAVE_PTHREAD],
-   [1],
-   [Define to 1 if you have the 'pthread' library (-lpthread).])
-  ])
-
- AS_IF(
-  [test "x$ac_cv_pthread" != xno],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [1]) ],
-  [AC_SUBST(
-   [HAVE_PTHREAD],
-   [0])
+  AS_IF(
+    [test "x$ac_cv_pthread" != xno],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [1]) ],
+    [AC_SUBST(
+      [HAVE_PTHREAD],
+      [0])
+    ])
   ])
- ])
 
 dnl Function to detect how to enable pthread
 AC_DEFUN([AX_PTHREAD_CHECK_ENABLE],
- [AX_COMMON_ARG_WITH(
-  [pthread],
-  [pthread],
-  [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
-  [auto-detect],
-  [DIR])
-
- dnl Check for a shared library version
- AX_PTHREAD_CHECK_LIB
-
- AS_IF(
-  [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
-  [AC_SUBST(
-   [PTHREAD_CPPFLAGS],
-   [$ac_cv_pthread_CPPFLAGS])
-  ])
- AS_IF(
-  [test "x$ac_cv_pthread_LIBADD" != "x"],
-  [AC_SUBST(
-   [PTHREAD_LIBADD],
-   [$ac_cv_pthread_LIBADD])
-  ])
+  [AX_COMMON_ARG_WITH(
+    [pthread],
+    [pthread],
+    [search for pthread in includedir and libdir or in the specified DIR, or no if not to use pthread],
+    [auto-detect],
+    [DIR])
 
- AS_IF(
-  [test "x$ac_cv_pthread" = xpthread],
-  [AC_SUBST(
-   [ax_pthread_pc_libs_private],
-   [-lpthread])
+  dnl Check for a shared library version
+  AX_PTHREAD_CHECK_LIB
+
+  AS_IF(
+    [test "x$ac_cv_pthread_CPPFLAGS" != "x"],
+    [AC_SUBST(
+      [PTHREAD_CPPFLAGS],
+      [$ac_cv_pthread_CPPFLAGS])
+    ])
+  AS_IF(
+    [test "x$ac_cv_pthread_LIBADD" != "x"],
+    [AC_SUBST(
+      [PTHREAD_LIBADD],
+      [$ac_cv_pthread_LIBADD])
+    ])
+
+  AS_IF(
+    [test "x$ac_cv_pthread" = xpthread],
+    [AC_SUBST(
+      [ax_pthread_pc_libs_private],
+      [-lpthread])
+    ])
   ])
- ])
```

### Comparing `libbde-20240223/m4/libcaes.m4` & `libbde-20240502/m4/libcaes.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Checks for libcaes required headers and functions
 dnl
-dnl Version: 20220529
+dnl Version: 20240413
 
 dnl Function to detect if libcaes is available
 dnl ac_libcaes_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBCAES_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcaes" = xno],
     [ac_cv_libcaes=no],
     [ac_cv_libcaes=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libcaes which returns "yes" and --with-libcaes= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libcaes" != x && test "x$ac_cv_with_libcaes" != xauto-detect],
+      [test "x$ac_cv_with_libcaes" != x && test "x$ac_cv_with_libcaes" != xauto-detect && test "x$ac_cv_with_libcaes" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libcaes"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libcaes}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcaes}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libcaes],
           [1])
@@ -107,16 +109,17 @@
           caes,
           libcaes_crypt_xts,
           [ac_cv_libcaes_dummy=yes],
           [ac_cv_libcaes=no])
 
         ac_cv_libcaes_LIBADD="-lcaes"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libcaes" != x && test "x$ac_cv_with_libcaes" != xauto-detect && test "x$ac_cv_libcaes" != xyes],
+      [test "x$ac_cv_libcaes" != xyes && test "x$ac_cv_with_libcaes" != x && test "x$ac_cv_with_libcaes" != xauto-detect && test "x$ac_cv_with_libcaes" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libcaes in directory: $ac_cv_with_libcaes],
         [1])
       ])
     ])
 
   AS_IF(
@@ -165,15 +168,15 @@
     [ac_cv_libcaes_aes_ecb=$ac_cv_libcrypto_aes_ecb])
 
   AS_IF(
     [test "x$ac_cv_libcrypto" = xno || test "x$ac_cv_libcrypto_aes_xts" = xno],
     [ac_cv_libcaes_aes_xts=local],
     [ac_cv_libcaes_aes_xts=$ac_cv_libcrypto_aes_xts])
 
-  ac_cv_libcaes_CPPFLAGS="-I../libcaes";
+  ac_cv_libcaes_CPPFLAGS="-I../libcaes -I\$(top_srcdir)/libcaes";
   ac_cv_libcaes_LIBADD="../libcaes/libcaes.la";
 
   ac_cv_libcaes=local
   ])
 
 dnl Function to detect how to enable libcaes
 AC_DEFUN([AX_LIBCAES_CHECK_ENABLE],
```

### Comparing `libbde-20240223/libbde.spec.in` & `libbde-20240502/libbde.spec.in`

 * *Files identical despite different names*

### Comparing `libbde-20240223/include/libbde.h` & `libbde-20240502/include/libbde.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/include/libbde/definitions.h.in` & `libbde-20240502/include/libbde/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libbde-20240223/include/libbde/definitions.h` & `libbde-20240502/include/libbde/definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBBDE_DEFINITIONS_H )
 #define _LIBBDE_DEFINITIONS_H
 
 #include <libbde/types.h>
 
-#define LIBBDE_VERSION					20240223
+#define LIBBDE_VERSION					20240502
 
 /* The version string
  */
-#define LIBBDE_VERSION_STRING				"20240223"
+#define LIBBDE_VERSION_STRING				"20240502"
 
 /* The file access
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBBDE_ACCESS_FLAGS
```

### Comparing `libbde-20240223/include/libbde/types.h.in` & `libbde-20240502/include/libbde/types.h.in`

 * *Files identical despite different names*

### Comparing `libbde-20240223/include/libbde/types.h` & `libbde-20240502/include/libbde/types.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/include/libbde/features.h.in` & `libbde-20240502/include/libbde/features.h.in`

 * *Files identical despite different names*

### Comparing `libbde-20240223/include/libbde/error.h` & `libbde-20240502/include/libbde/error.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/include/libbde/extern.h` & `libbde-20240502/include/libbde/extern.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/include/libbde/features.h` & `libbde-20240502/include/libbde/features.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/include/libbde/codepage.h` & `libbde-20240502/include/libbde/codepage.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/include/Makefile.in` & `libbde-20240502/include/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -459,14 +459,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -545,15 +547,20 @@
 
 EXTRA_DIST = \
 	libbde.h.in \
 	libbde/definitions.h.in \
 	libbde/features.h.in \
 	libbde/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libbde.h \
+	libbde/definitions.h \
+	libbde/features.h \
+	libbde/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -750,23 +757,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -848,17 +857,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libbde.h
-	-rm -f libbde/definitions.h
-	-rm -f libbde/features.h
-	-rm -f libbde/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libbde-20240223/include/libbde.h.in` & `libbde-20240502/include/libbde.h.in`

 * *Files identical despite different names*

### Comparing `libbde-20240223/common/config_borlandc.h` & `libbde-20240502/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/common/file_stream.h` & `libbde-20240502/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/common/memory.h` & `libbde-20240502/common/memory.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/common/byte_stream.h` & `libbde-20240502/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/common/common.h` & `libbde-20240502/common/common.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/common/config_winapi.h` & `libbde-20240502/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/common/system_string.h` & `libbde-20240502/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/common/types.h.in` & `libbde-20240502/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libbde-20240223/common/types.h` & `libbde-20240502/common/types.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/common/config.h.in` & `libbde-20240502/common/config.h.in`

 * *Files 1% similar despite different names*

```diff
@@ -269,14 +269,17 @@
 
 /* Define to 1 if you have the <libfguid.h> header file. */
 #undef HAVE_LIBFGUID_H
 
 /* Define to 1 if you have the 'fuse' library (-lfuse). */
 #undef HAVE_LIBFUSE
 
+/* Define to 1 if you have the 'fuse3' library (-lfuse3). */
+#undef HAVE_LIBFUSE3
+
 /* Define to 1 if you have the `fvalue' library (-lfvalue). */
 #undef HAVE_LIBFVALUE
 
 /* Define to 1 if you have the <libfvalue.h> header file. */
 #undef HAVE_LIBFVALUE_H
 
 /* Define to 1 if you have the `hmac' library (-lhmac). */
```

### Comparing `libbde-20240223/common/config.h` & `libbde-20240502/common/config.h`

 * *Files 1% similar despite different names*

```diff
@@ -268,15 +268,18 @@
 /* Define to 1 if you have the `fguid' library (-lfguid). */
 /* #undef HAVE_LIBFGUID */
 
 /* Define to 1 if you have the <libfguid.h> header file. */
 /* #undef HAVE_LIBFGUID_H */
 
 /* Define to 1 if you have the 'fuse' library (-lfuse). */
-#define HAVE_LIBFUSE 1
+/* #undef HAVE_LIBFUSE */
+
+/* Define to 1 if you have the 'fuse3' library (-lfuse3). */
+#define HAVE_LIBFUSE3 1
 
 /* Define to 1 if you have the `fvalue' library (-lfvalue). */
 /* #undef HAVE_LIBFVALUE */
 
 /* Define to 1 if you have the <libfvalue.h> header file. */
 /* #undef HAVE_LIBFVALUE_H */
 
@@ -640,24 +643,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libbde"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libbde 20240223"
+#define PACKAGE_STRING "libbde 20240502"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libbde"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240223"
+#define PACKAGE_VERSION "20240502"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -678,15 +681,15 @@
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Define to 1 if your <sys/time.h> declares `struct tm'. */
 /* #undef TM_IN_SYS_TIME */
 
 /* Version number of package */
-#define VERSION "20240223"
+#define VERSION "20240502"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libbde-20240223/common/wide_string.h` & `libbde-20240502/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/common/narrow_string.h` & `libbde-20240502/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/common/config_msc.h` & `libbde-20240502/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/common/Makefile.in` & `libbde-20240502/common/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -429,14 +429,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -498,15 +500,17 @@
 sharedstatedir = @sharedstatedir@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
-AM_CPPFLAGS = -I$(top_srcdir)/include
+AM_CPPFLAGS = \
+	-I../include -I$(top_srcdir)/include
+
 EXTRA_DIST = \
 	byte_stream.h \
 	common.h \
 	config.h \
 	config_borlandc.h \
 	config_msc.h \
 	config_winapi.h \
@@ -514,15 +518,18 @@
 	memory.h \
 	narrow_string.h \
 	system_string.h \
 	types.h \
 	types.h.in \
 	wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	config.h \
+	types.h \
+	Makefile \
 	Makefile.in
 
 all: config.h
 	$(MAKE) $(AM_MAKEFLAGS) all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -690,23 +697,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-hdr distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -786,15 +795,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f config.h
-	-rm -f types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libbde-20240223/libclocale/libclocale_wide_string.c` & `libbde-20240502/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libclocale/libclocale_support.h` & `libbde-20240502/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libclocale/Makefile.am` & `libbde-20240502/libclocale/Makefile.am`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 if HAVE_LOCAL_LIBCLOCALE
 AM_CPPFLAGS = \
 	-DLOCALEDIR=\"$(datadir)/locale\" \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libclocale.la
 
 libclocale_la_SOURCES = \
 	libclocale_codepage.c libclocale_codepage.h \
 	libclocale_definitions.h \
@@ -14,19 +14,17 @@
 	libclocale_libcerror.h \
 	libclocale_locale.c libclocale_locale.h \
 	libclocale_support.c libclocale_support.h \
 	libclocale_unused.h \
 	libclocale_wide_string.c libclocale_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
```

### Comparing `libbde-20240223/libclocale/libclocale_definitions.h` & `libbde-20240502/libclocale/libclocale_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 #include <libclocale/definitions.h>
 
 /* The definitions in <libclocale/definitions.h> are copied here
  * for local use of libclocale
  */
 #else
 
-#define LIBCLOCALE_VERSION					20240107
+#define LIBCLOCALE_VERSION					20240414
 
 /* The libclocale version string
  */
-#define LIBCLOCALE_VERSION_STRING				"20240107"
+#define LIBCLOCALE_VERSION_STRING				"20240414"
 
 /* The codepage feature flag definitions
  */
 enum LIBCLOCALE_CODEPAGES_FEATURE_FLAGS
 {
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_ISO_8859		= 0x00000001UL,
 	LIBCLOCALE_CODEPAGE_FEATURE_FLAG_HAVE_KOI8		= 0x00000002UL,
```

### Comparing `libbde-20240223/libclocale/libclocale_unused.h` & `libbde-20240502/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libclocale/libclocale_libcerror.h` & `libbde-20240502/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libclocale/libclocale_locale.h` & `libbde-20240502/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libclocale/libclocale_support.c` & `libbde-20240502/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libclocale/libclocale_codepage.c` & `libbde-20240502/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libclocale/libclocale_locale.c` & `libbde-20240502/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libclocale/Makefile.in` & `libbde-20240502/libclocale/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -473,14 +473,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -544,30 +546,31 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCLOCALE_TRUE@AM_CPPFLAGS = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	-DLOCALEDIR=\"$(datadir)/locale\" \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCLOCALE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCLOCALE_TRUE@noinst_LTLIBRARIES = libclocale.la
 @HAVE_LOCAL_LIBCLOCALE_TRUE@libclocale_la_SOURCES = \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_codepage.c libclocale_codepage.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_definitions.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_extern.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_libcerror.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_locale.c libclocale_locale.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_support.c libclocale_support.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_unused.h \
 @HAVE_LOCAL_LIBCLOCALE_TRUE@	libclocale_wide_string.c libclocale_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -770,24 +773,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libclocale_codepage.Plo
+	-rm -f ./$(DEPDIR)/libclocale_locale.Plo
+	-rm -f ./$(DEPDIR)/libclocale_support.Plo
+	-rm -f ./$(DEPDIR)/libclocale_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -874,17 +883,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libclocale ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libclocale_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libbde-20240223/libclocale/libclocale_extern.h` & `libbde-20240502/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libclocale/libclocale_wide_string.h` & `libbde-20240502/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libclocale/libclocale_codepage.h` & `libbde-20240502/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfcache/libfcache_libcdata.h` & `libbde-20240502/libfcache/libfcache_libcdata.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfcache/libfcache_types.h` & `libbde-20240502/libfcache/libfcache_types.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfcache/libfcache_cache_value.c` & `libbde-20240502/libfcache/libfcache_cache_value.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfcache/libfcache_unused.h` & `libbde-20240502/libfcache/libfcache_unused.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfcache/Makefile.am` & `libbde-20240502/libfcache/Makefile.am`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFCACHE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfcache.la
 
@@ -19,19 +19,17 @@
 	libfcache_libcdata.h \
 	libfcache_libcerror.h \
 	libfcache_support.c libfcache_support.h \
 	libfcache_types.h \
 	libfcache_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfcache ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcache_la_SOURCES)
```

### Comparing `libbde-20240223/libfcache/libfcache_support.h` & `libbde-20240502/libfcache/libfcache_support.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfcache/libfcache_error.h` & `libbde-20240502/libfcache/libfcache_error.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfcache/libfcache_support.c` & `libbde-20240502/libfcache/libfcache_support.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfcache/libfcache_cache.h` & `libbde-20240502/libfcache/libfcache_cache.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfcache/libfcache_error.c` & `libbde-20240502/libfcache/libfcache_error.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfcache/libfcache_libcerror.h` & `libbde-20240502/libfcache/libfcache_libcerror.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfcache/libfcache_date_time.c` & `libbde-20240502/libfcache/libfcache_date_time.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfcache/libfcache_extern.h` & `libbde-20240502/libfcache/libfcache_extern.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfcache/libfcache_cache_value.h` & `libbde-20240502/libfcache/libfcache_cache_value.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfcache/Makefile.in` & `libbde-20240502/libfcache/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -476,14 +476,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -546,16 +548,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFCACHE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFCACHE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFCACHE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFCACHE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFCACHE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFCACHE_TRUE@noinst_LTLIBRARIES = libfcache.la
 @HAVE_LOCAL_LIBFCACHE_TRUE@libfcache_la_SOURCES = \
@@ -567,15 +569,16 @@
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_extern.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_libcdata.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_libcerror.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_support.c libfcache_support.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_types.h \
 @HAVE_LOCAL_LIBFCACHE_TRUE@	libfcache_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -779,24 +782,31 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfcache_cache.Plo
+	-rm -f ./$(DEPDIR)/libfcache_cache_value.Plo
+	-rm -f ./$(DEPDIR)/libfcache_date_time.Plo
+	-rm -f ./$(DEPDIR)/libfcache_error.Plo
+	-rm -f ./$(DEPDIR)/libfcache_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -884,17 +894,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfcache ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfcache_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libbde-20240223/libfcache/libfcache_date_time.h` & `libbde-20240502/libfcache/libfcache_date_time.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfcache/libfcache_definitions.h` & `libbde-20240502/libfcache/libfcache_definitions.h`

 * *Files 6% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBFCACHE )
 #include <libfcache/definitions.h>
 
 /* The definitions in <libfcache/definitions.h> are copied here
  * for local use of libfcache
  */
 #else
-#define LIBFCACHE_VERSION					20240112
+#define LIBFCACHE_VERSION					20240414
 
 /* The libfcache version string
  */
-#define LIBFCACHE_VERSION_STRING				"20240112"
+#define LIBFCACHE_VERSION_STRING				"20240414"
 
 /* The cache value flags definitions
  */
 enum LIBFCACHE_CACHE_VALUE_FLAGS
 {
 	/* The cache value is not managed by the library
 	 */
```

### Comparing `libbde-20240223/libfcache/libfcache_cache.c` & `libbde-20240502/libfcache/libfcache_cache.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/Makefile.am` & `libbde-20240502/Makefile.am`

 * *Files 22% similar despite different names*

```diff
@@ -61,16 +61,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libbde.pc \
+	libbde.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 
 pkgconfig_DATA = \
 	libbde.pc
 
 libtool: @LIBTOOL_DEPS@
@@ -95,19 +102,7 @@
 	(cd $(srcdir)/libfguid && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfvalue && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libhmac && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libcaes && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libbde && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libbde.pc
-	-rm -f libbde.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
```

### Comparing `libbde-20240223/libbfio/libbfio_file_range.h` & `libbde-20240502/libbfio/libbfio_file_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_file_range_io_handle.c` & `libbde-20240502/libbfio/libbfio_file_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_support.c` & `libbde-20240502/libbfio/libbfio_support.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_libcpath.h` & `libbde-20240502/libbfio/libbfio_libcpath.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcpath header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_error.h` & `libbde-20240502/libbfio/libbfio_error.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_libclocale.h` & `libbde-20240502/libbfio/libbfio_libclocale.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libclocale header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_error.c` & `libbde-20240502/libbfio/libbfio_error.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_libuna.h` & `libbde-20240502/libbfio/libbfio_libuna.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libuna header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_file_io_handle.h` & `libbde-20240502/libbfio/libbfio_file_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_file_pool.h` & `libbde-20240502/libbfio/libbfio_file_pool.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_file_range.c` & `libbde-20240502/libbfio/libbfio_file_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_types.h` & `libbde-20240502/libbfio/libbfio_types.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_unused.h` & `libbde-20240502/libbfio/libbfio_unused.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_libcdata.h` & `libbde-20240502/libbfio/libbfio_libcdata.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcdata header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_file.h` & `libbde-20240502/libbfio/libbfio_file.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/Makefile.am` & `libbde-20240502/libbfio/Makefile.am`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBBFIO
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
@@ -38,17 +38,17 @@
 	libbfio_pool.c libbfio_pool.h \
 	libbfio_support.c libbfio_support.h \
 	libbfio_system_string.c libbfio_system_string.h \
 	libbfio_types.h \
 	libbfio_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
```

### Comparing `libbde-20240223/libbfio/libbfio_libcfile.h` & `libbde-20240502/libbfio/libbfio_libcfile.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcfile header
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_definitions.h` & `libbde-20240502/libbfio/libbfio_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBBFIO )
 #include <libbfio/definitions.h>
 
 /* The definitions in <libbfio/definitions.h> are copied here
  * for local use of libbfio
  */
 #else
-#define LIBBFIO_VERSION					20221025
+#define LIBBFIO_VERSION					20240414
 
 /* The libbfio version string
  */
-#define LIBBFIO_VERSION_STRING				"20221025"
+#define LIBBFIO_VERSION_STRING				"20240414"
 
 /* The library flags definitions
  */
 enum LIBBFIO_FLAGS
 {
 	/* The IO handle is not managed by the library
 	 */
```

### Comparing `libbde-20240223/libbfio/libbfio_codepage.h` & `libbde-20240502/libbfio/libbfio_codepage.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Codepage functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_file_io_handle.c` & `libbde-20240502/libbfio/libbfio_file_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_support.h` & `libbde-20240502/libbfio/libbfio_support.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_memory_range.h` & `libbde-20240502/libbfio/libbfio_memory_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_file_pool.c` & `libbde-20240502/libbfio/libbfio_file_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_file_range_io_handle.h` & `libbde-20240502/libbfio/libbfio_file_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_libcthreads.h` & `libbde-20240502/libbfio/libbfio_libcthreads.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcthreads header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_system_string.h` & `libbde-20240502/libbfio/libbfio_system_string.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_memory_range_io_handle.c` & `libbde-20240502/libbfio/libbfio_memory_range_io_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_handle.c` & `libbde-20240502/libbfio/libbfio_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_file.c` & `libbde-20240502/libbfio/libbfio_file.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * File functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_handle.h` & `libbde-20240502/libbfio/libbfio_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_memory_range.c` & `libbde-20240502/libbfio/libbfio_memory_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_pool.c` & `libbde-20240502/libbfio/libbfio_pool.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_libcerror.h` & `libbde-20240502/libbfio/libbfio_libcerror.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/Makefile.in` & `libbde-20240502/libbfio/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -494,14 +494,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -564,16 +566,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBBFIO_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBBFIO_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBBFIO_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBBFIO_TRUE@	@LIBCFILE_CPPFLAGS@ \
@@ -604,15 +606,16 @@
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_memory_range_io_handle.c libbfio_memory_range_io_handle.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_pool.c libbfio_pool.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_support.c libbfio_support.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_system_string.c libbfio_system_string.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_types.h \
 @HAVE_LOCAL_LIBBFIO_TRUE@	libbfio_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -823,24 +826,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libbfio_error.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_file_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range.Plo
+	-rm -f ./$(DEPDIR)/libbfio_memory_range_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbfio_pool.Plo
+	-rm -f ./$(DEPDIR)/libbfio_support.Plo
+	-rm -f ./$(DEPDIR)/libbfio_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -909,14 +926,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -927,23 +946,22 @@
 	install-data install-data-am install-dvi install-dvi-am \
 	install-exec install-exec-am install-html install-html-am \
 	install-info install-info-am install-man install-pdf \
 	install-pdf-am install-ps install-ps-am install-strip \
 	installcheck installcheck-am installdirs maintainer-clean \
 	maintainer-clean-generic mostlyclean mostlyclean-compile \
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
-	sources-am sources-local splint splint-am splint-local tags \
-	tags-am uninstall uninstall-am
+	sources-am sources-local splint-am splint-local tags tags-am \
+	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libbfio ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbfio_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libbde-20240223/libbfio/libbfio_system_string.c` & `libbde-20240502/libbfio/libbfio_system_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * System string functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_memory_range_io_handle.h` & `libbde-20240502/libbfio/libbfio_memory_range_io_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Memory range IO handle functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_extern.h` & `libbde-20240502/libbfio/libbfio_extern.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/libbfio/libbfio_pool.h` & `libbde-20240502/libbfio/libbfio_pool.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal pool functions
  *
- * Copyright (C) 2009-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2009-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libbde-20240223/config.guess` & `libbde-20240502/config.guess`

 * *Files identical despite different names*

### Comparing `libbde-20240223/dpkg/copyright` & `libbde-20240502/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libbde-20240223/dpkg/control` & `libbde-20240502/dpkg/control`

 * *Files identical despite different names*

### Comparing `libbde-20240223/dpkg/rules` & `libbde-20240502/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libbde-20240223/COPYING.LESSER` & `libbde-20240502/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libbde-20240223/configure` & `libbde-20240502/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libbde 20240223.
+# Generated by GNU Autoconf 2.71 for libbde 20240502.
 #
 # Report bugs to <joachim.metz@gmail.com>.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
@@ -617,16 +617,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='libbde'
 PACKAGE_TARNAME='libbde'
-PACKAGE_VERSION='20240223'
-PACKAGE_STRING='libbde 20240223'
+PACKAGE_VERSION='20240502'
+PACKAGE_STRING='libbde 20240502'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libbde.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -678,14 +678,16 @@
 ax_libfuse_spec_requires
 ax_libfuse_pc_libs_private
 LIBFUSE_LIBADD
 LIBFUSE_CPPFLAGS
 HAVE_LIBFUSE
 fuse_LIBS
 fuse_CFLAGS
+fuse3_LIBS
+fuse3_CFLAGS
 HAVE_PYTHON_TESTS_FALSE
 HAVE_PYTHON_TESTS_TRUE
 HAVE_PYTHON_FALSE
 HAVE_PYTHON_TRUE
 PYTHON_PACKAGE_DIR
 PYTHON_LIBRARY_DIR
 pyexecdir
@@ -1143,14 +1145,16 @@
 libfvalue_LIBS
 libhmac_CFLAGS
 libhmac_LIBS
 openssl_CFLAGS
 openssl_LIBS
 libcaes_CFLAGS
 libcaes_LIBS
+fuse3_CFLAGS
+fuse3_LIBS
 fuse_CFLAGS
 fuse_LIBS'
 
 
 # Initialize some variables set by options.
 ac_init_help=
 ac_init_version=false
@@ -1693,15 +1697,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libbde 20240223 to adapt to many kinds of systems.
+\`configure' configures libbde 20240502 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1764,15 +1768,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libbde 20240223:";;
+     short | recursive ) echo "Configuration of libbde 20240502:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1970,14 +1974,17 @@
               C compiler flags for openssl, overriding pkg-config
   openssl_LIBS
               linker flags for openssl, overriding pkg-config
   libcaes_CFLAGS
               C compiler flags for libcaes, overriding pkg-config
   libcaes_LIBS
               linker flags for libcaes, overriding pkg-config
+  fuse3_CFLAGS
+              C compiler flags for fuse3, overriding pkg-config
+  fuse3_LIBS  linker flags for fuse3, overriding pkg-config
   fuse_CFLAGS C compiler flags for fuse, overriding pkg-config
   fuse_LIBS   linker flags for fuse, overriding pkg-config
 
 Use these variables to override the choices made by `configure' or to help
 it to find libraries and programs with nonstandard names/locations.
 
 Report bugs to <joachim.metz@gmail.com>.
@@ -2040,15 +2047,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libbde configure 20240223
+libbde configure 20240502
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2761,15 +2768,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libbde $as_me 20240223, which was
+It was created by libbde $as_me 20240502, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4250,15 +4257,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libbde'
- VERSION='20240223'
+ VERSION='20240502'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -23845,15 +23852,15 @@
 printf "%s\n" "$ac_cv_with_libcerror" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcerror" = xno
 then :
   ac_cv_libcerror=no
 else $as_nop
   ac_cv_libcerror=check
-        if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect
+                if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   if test -d "$ac_cv_with_libcerror"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcerror}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcerror}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -24344,15 +24351,16 @@
 fi
 
 
         ac_cv_libcerror_LIBADD="-lcerror"
 fi
 
 fi
-    if test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_libcerror" != xyes
+
+    if test "x$ac_cv_libcerror" != xyes && test "x$ac_cv_with_libcerror" != x && test "x$ac_cv_with_libcerror" != xauto-detect && test "x$ac_cv_with_libcerror" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcerror in directory: $ac_cv_with_libcerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -24494,15 +24502,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -24596,15 +24604,15 @@
     ac_cv_libcthreads_multi_threading="no"
 else $as_nop
       if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcthreads" = xno
 then :
   ac_cv_libcthreads=no
 else $as_nop
   ac_cv_libcthreads=check
-        if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect
+                if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   if test -d "$ac_cv_with_libcthreads"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcthreads}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcthreads}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -26236,15 +26244,15 @@
 
 
         ac_cv_libcthreads_LIBADD="-lcthreads"
 fi
 
 fi
 
-    if test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_libcthreads" != xyes
+    if test "x$ac_cv_libcthreads" != xyes && test "x$ac_cv_with_libcthreads" != x && test "x$ac_cv_with_libcthreads" != xauto-detect && test "x$ac_cv_with_libcthreads" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcthreads in directory: $ac_cv_with_libcthreads
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -26298,47 +26306,52 @@
   printf %s "(cached) " >&6
 else $as_nop
   ac_cv_with_pthread=auto-detect
 fi
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_pthread" >&5
 printf "%s\n" "$ac_cv_with_pthread" >&6; }
 
-   if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xno && test "x$ac_cv_with_pthread" != xauto-detect
+    if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_pthread" = xno
+then :
+  ac_cv_pthread=no
+else $as_nop
+  ac_cv_pthread=check
+                if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
 then :
   if test -d "$ac_cv_with_pthread"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_pthread}/include"
-   LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_pthread}/lib"
 else $as_nop
   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_pthread" >&5
 printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_pthread" >&2;}
 
 fi
 
 fi
 
- if test "x$ac_cv_with_pthread" = xno
+fi
+
+    if test "x$ac_cv_pthread" = xcheck
 then :
-  ac_cv_pthread=no
-else $as_nop
-    ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
+        ac_fn_c_check_header_compile "$LINENO" "pthread.h" "ac_cv_header_pthread_h" "$ac_includes_default"
 if test "x$ac_cv_header_pthread_h" = xyes
 then :
   printf "%s\n" "#define HAVE_PTHREAD_H 1" >>confdefs.h
 
 fi
 
 
-  if test "x$ac_cv_header_pthread_h" = xno
+      if test "x$ac_cv_header_pthread_h" = xno
 then :
   ac_cv_pthread=no
 else $as_nop
-     ac_cv_pthread=pthread
+          ac_cv_pthread=pthread
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_create in -lpthread" >&5
 printf %s "checking for pthread_create in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_create+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26372,15 +26385,15 @@
 if test "x$ac_cv_lib_pthread_pthread_create" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_exit in -lpthread" >&5
 printf %s "checking for pthread_exit in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_exit+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26414,15 +26427,15 @@
 if test "x$ac_cv_lib_pthread_pthread_exit" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_join in -lpthread" >&5
 printf %s "checking for pthread_join in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_join+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26457,15 +26470,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_init in -lpthread" >&5
 printf %s "checking for pthread_cond_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26499,15 +26512,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_destroy in -lpthread" >&5
 printf %s "checking for pthread_cond_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26541,15 +26554,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_broadcast in -lpthread" >&5
 printf %s "checking for pthread_cond_broadcast in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_broadcast+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26583,15 +26596,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_broadcast" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_signal in -lpthread" >&5
 printf %s "checking for pthread_cond_signal in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_signal+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26625,15 +26638,15 @@
 if test "x$ac_cv_lib_pthread_pthread_cond_signal" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_cond_wait in -lpthread" >&5
 printf %s "checking for pthread_cond_wait in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_cond_wait+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26668,15 +26681,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_init in -lpthread" >&5
 printf %s "checking for pthread_mutex_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26710,15 +26723,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_destroy in -lpthread" >&5
 printf %s "checking for pthread_mutex_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26752,15 +26765,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_lock in -lpthread" >&5
 printf %s "checking for pthread_mutex_lock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_lock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26794,15 +26807,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_lock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_trylock in -lpthread" >&5
 printf %s "checking for pthread_mutex_trylock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_trylock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26836,15 +26849,15 @@
 if test "x$ac_cv_lib_pthread_pthread_mutex_trylock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_mutex_unlock in -lpthread" >&5
 printf %s "checking for pthread_mutex_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_mutex_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26879,15 +26892,15 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-      { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
+                { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_init in -lpthread" >&5
 printf %s "checking for pthread_rwlock_init in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_init+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26921,15 +26934,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_init" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_destroy in -lpthread" >&5
 printf %s "checking for pthread_rwlock_destroy in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_destroy+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -26963,15 +26976,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_destroy" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_rdlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_rdlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_rdlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -27005,15 +27018,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_rdlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_wrlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_wrlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_wrlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -27047,15 +27060,15 @@
 if test "x$ac_cv_lib_pthread_pthread_rwlock_wrlock" = xyes
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
-   { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for pthread_rwlock_unlock in -lpthread" >&5
 printf %s "checking for pthread_rwlock_unlock in -lpthread... " >&6; }
 if test ${ac_cv_lib_pthread_pthread_rwlock_unlock+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
   ac_check_lib_save_LIBS=$LIBS
 LIBS="-lpthread  $LIBS"
@@ -27090,67 +27103,76 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-   ac_cv_pthread_LIBADD="-lpthread";
+        ac_cv_pthread_LIBADD="-lpthread";
+
+fi
+
+    if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported pthread in directory: $ac_cv_with_pthread
+See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
 
 printf "%s\n" "#define HAVE_PTHREAD 1" >>confdefs.h
 
 
 fi
 
- if test "x$ac_cv_pthread" != xno
+  if test "x$ac_cv_pthread" != xno
 then :
   HAVE_PTHREAD=1
 
 else $as_nop
   HAVE_PTHREAD=0
 
 
 fi
 
 
- if test "x$ac_cv_pthread_CPPFLAGS" != "x"
+  if test "x$ac_cv_pthread_CPPFLAGS" != "x"
 then :
   PTHREAD_CPPFLAGS=$ac_cv_pthread_CPPFLAGS
 
 
 fi
- if test "x$ac_cv_pthread_LIBADD" != "x"
+  if test "x$ac_cv_pthread_LIBADD" != "x"
 then :
   PTHREAD_LIBADD=$ac_cv_pthread_LIBADD
 
 
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+  if test "x$ac_cv_pthread" = xpthread
 then :
   ax_pthread_pc_libs_private=-lpthread
 
 
 fi
 
       ac_cv_libcthreads_multi_threading=$ac_cv_pthread
 else $as_nop
   ac_cv_libcthreads_multi_threading="winapi"
 fi
 
   if test "x$ac_cv_libcthreads_multi_threading" != xno
 then :
-  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads";
+  ac_cv_libcthreads_CPPFLAGS="-I../libcthreads -I\$(top_srcdir)/libcthreads";
     ac_cv_libcthreads_LIBADD="../libcthreads/libcthreads.la";
 
     ac_cv_libcthreads=local
 else $as_nop
   ac_cv_libcthreads=no
 fi
 
@@ -27238,15 +27260,15 @@
 printf "%s\n" "$ac_cv_with_libcdata" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcdata" = xno
 then :
   ac_cv_libcdata=no
 else $as_nop
   ac_cv_libcdata=check
-        if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect
+                if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   if test -d "$ac_cv_with_libcdata"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcdata}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -31017,15 +31039,16 @@
 fi
 
 
         ac_cv_libcdata_LIBADD="-lcdata"
 fi
 
 fi
-    if test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_libcdata" != xyes
+
+    if test "x$ac_cv_libcdata" != xyes && test "x$ac_cv_with_libcdata" != x && test "x$ac_cv_with_libcdata" != xauto-detect && test "x$ac_cv_with_libcdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcdata in directory: $ac_cv_with_libcdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -31050,15 +31073,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcdata" != xyes
 then :
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDATA 1" >>confdefs.h
@@ -31128,15 +31151,15 @@
 printf "%s\n" "$ac_cv_with_libclocale" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libclocale" = xno
 then :
   ac_cv_libclocale=no
 else $as_nop
   ac_cv_libclocale=check
-        if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect
+                if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   if test -d "$ac_cv_with_libclocale"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libclocale}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libclocale}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -31683,15 +31706,16 @@
 fi
 
 
         ac_cv_libclocale_LIBADD="-lclocale"
 fi
 
 fi
-    if test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_libclocale" != xyes
+
+    if test "x$ac_cv_libclocale" != xyes && test "x$ac_cv_with_libclocale" != x && test "x$ac_cv_with_libclocale" != xauto-detect && test "x$ac_cv_with_libclocale" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libclocale in directory: $ac_cv_with_libclocale
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -31847,15 +31871,15 @@
 
 printf "%s\n" "#define HAVE_LANGINFO_CODESET 1" >>confdefs.h
 
 
 fi
 
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCLOCALE 1" >>confdefs.h
@@ -31925,15 +31949,15 @@
 printf "%s\n" "$ac_cv_with_libcnotify" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcnotify" = xno
 then :
   ac_cv_libcnotify=no
 else $as_nop
   ac_cv_libcnotify=check
-        if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect
+                if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   if test -d "$ac_cv_with_libcnotify"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcnotify}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcnotify}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -32383,15 +32407,16 @@
 fi
 
 
         ac_cv_libcnotify_LIBADD="-lcnotify"
 fi
 
 fi
-    if test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_libcnotify" != xyes
+
+    if test "x$ac_with_libcnotify" != xyes && test "x$ac_cv_with_libcnotify" != x && test "x$ac_cv_with_libcnotify" != xauto-detect && test "x$ac_cv_with_libcnotify" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcnotify in directory: $ac_cv_with_libcnotify
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -32446,15 +32471,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -32524,15 +32549,15 @@
 printf "%s\n" "$ac_cv_with_libcsplit" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcsplit" = xno
 then :
   ac_cv_libcsplit=no
 else $as_nop
   ac_cv_libcsplit=check
-        if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect
+                if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   if test -d "$ac_cv_with_libcsplit"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcsplit}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcsplit}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -33247,15 +33272,16 @@
 
 fi
 
         ac_cv_libcsplit_LIBADD="-lcsplit"
 fi
 
 fi
-    if test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_libcsplit" != xyes
+
+    if test "x$ac_cv_libcsplit" != xyes && test "x$ac_cv_with_libcsplit" != x && test "x$ac_cv_with_libcsplit" != xauto-detect && test "x$ac_cv_with_libcsplit" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcsplit in directory: $ac_cv_with_libcsplit
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -33280,15 +33306,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcsplit" != xyes
 then :
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCSPLIT 1" >>confdefs.h
@@ -33358,15 +33384,15 @@
 printf "%s\n" "$ac_cv_with_libuna" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libuna" = xno
 then :
   ac_cv_libuna=no
 else $as_nop
   ac_cv_libuna=check
-        if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect
+                if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   if test -d "$ac_cv_with_libuna"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libuna}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libuna}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -40568,15 +40594,16 @@
   ac_cv_libuna=no
 fi
 
         ac_cv_libuna_LIBADD="-luna"
 fi
 
 fi
-    if test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_libuna" != xyes
+
+    if test "x$ac_cv_libuna" != xyes && test "x$ac_cv_with_libuna" != x && test "x$ac_cv_with_libuna" != xauto-detect && test "x$ac_cv_with_libuna" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libuna in directory: $ac_cv_with_libuna
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -40601,15 +40628,15 @@
 
 fi
 
 
     if test "x$ac_cv_libuna" != xyes
 then :
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBUNA 1" >>confdefs.h
@@ -40679,15 +40706,15 @@
 printf "%s\n" "$ac_cv_with_libcfile" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcfile" = xno
 then :
   ac_cv_libcfile=no
 else $as_nop
   ac_cv_libcfile=check
-        if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect
+                if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   if test -d "$ac_cv_with_libcfile"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcfile}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcfile}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -41868,15 +41895,16 @@
 
 fi
 
         ac_cv_libcfile_LIBADD="-lcfile"
 fi
 
 fi
-    if test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_libcfile" != xyes
+
+    if test "x$ac_cv_libcfile" != xyes && test "x$ac_cv_with_libcfile" != x && test "x$ac_cv_with_libcfile" != xauto-detect && test "x$ac_cv_with_libcfile" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcfile in directory: $ac_cv_with_libcfile
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -42190,15 +42218,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: unlink
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libcfile_CPPFLAGS="-I../libcfile";
+  ac_cv_libcfile_CPPFLAGS="-I../libcfile -I\$(top_srcdir)/libcfile";
   ac_cv_libcfile_LIBADD="../libcfile/libcfile.la";
 
   ac_cv_libcfile=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCFILE 1" >>confdefs.h
@@ -42268,15 +42296,15 @@
 printf "%s\n" "$ac_cv_with_libcpath" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcpath" = xno
 then :
   ac_cv_libcpath=no
 else $as_nop
   ac_cv_libcpath=check
-        if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect
+                if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   if test -d "$ac_cv_with_libcpath"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcpath}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcpath}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -43073,15 +43101,16 @@
 
 fi
 
         ac_cv_libcpath_LIBADD="-lcpath"
 fi
 
 fi
-    if test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_libcpath" != xyes
+
+    if test "x$ac_cv_libcpath" != xyes && test "x$ac_cv_with_libcpath" != x && test "x$ac_cv_with_libcpath" != xauto-detect && test "x$ac_cv_with_libcpath" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcpath in directory: $ac_cv_with_libcpath
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -43271,15 +43300,15 @@
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: mkdir
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCPATH 1" >>confdefs.h
@@ -43349,15 +43378,15 @@
 printf "%s\n" "$ac_cv_with_libbfio" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libbfio" = xno
 then :
   ac_cv_libbfio=no
 else $as_nop
   ac_cv_libbfio=check
-        if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect
+                if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   if test -d "$ac_cv_with_libbfio"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libbfio}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libbfio}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -45467,15 +45496,16 @@
 
 fi
 
         ac_cv_libbfio_LIBADD="-lbfio"
 fi
 
 fi
-    if test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_libbfio" != xyes
+
+    if test "x$ac_cv_libbfio" != xyes && test "x$ac_cv_with_libbfio" != x && test "x$ac_cv_with_libbfio" != xauto-detect && test "x$ac_cv_with_libbfio" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libbfio in directory: $ac_cv_with_libbfio
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -45500,15 +45530,15 @@
 
 fi
 
 
     if test "x$ac_cv_libbfio" != xyes
 then :
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBBFIO 1" >>confdefs.h
@@ -45578,15 +45608,15 @@
 printf "%s\n" "$ac_cv_with_libfcache" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfcache" = xno
 then :
   ac_cv_libfcache=no
 else $as_nop
   ac_cv_libfcache=check
-        if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect
+                if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes
 then :
   if test -d "$ac_cv_with_libfcache"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfcache}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfcache}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -46498,15 +46528,16 @@
 fi
 
 
         ac_cv_libfcache_LIBADD="-lfcache"
 fi
 
 fi
-    if test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_libfcache" != xyes
+
+    if test "x$ac_cv_libfcache" != xyes && test "x$ac_cv_with_libfcache" != x && test "x$ac_cv_with_libfcache" != xauto-detect && test "x$ac_cv_with_libfcache" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfcache in directory: $ac_cv_with_libfcache
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -46599,15 +46630,15 @@
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: time
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
-  ac_cv_libfcache_CPPFLAGS="-I../libfcache";
+  ac_cv_libfcache_CPPFLAGS="-I../libfcache -I\$(top_srcdir)/libfcache";
   ac_cv_libfcache_LIBADD="../libfcache/libfcache.la";
 
   ac_cv_libfcache=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFCACHE 1" >>confdefs.h
@@ -46677,15 +46708,15 @@
 printf "%s\n" "$ac_cv_with_libfdatetime" >&6; }
 
   if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdatetime" = xno
 then :
   ac_cv_libfdatetime=no
 else $as_nop
   ac_cv_libfdatetime=check
-        if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect
+                if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes
 then :
   if test -d "$ac_cv_with_libfdatetime"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfdatetime}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdatetime}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -50121,15 +50152,16 @@
 fi
 
 
         ac_cv_libfdatetime_LIBADD="-lfdatetime"
 fi
 
 fi
-    if test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_libfdatetime" != xyes
+
+    if test "x$ac_cv_libfdatetime" != xyes && test "x$ac_cv_with_libfdatetime" != x && test "x$ac_cv_with_libfdatetime" != xauto-detect && test "x$ac_cv_with_libfdatetime" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfdatetime in directory: $ac_cv_with_libfdatetime
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -50154,15 +50186,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdatetime" != xyes
 then :
 
-  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime";
+  ac_cv_libfdatetime_CPPFLAGS="-I../libfdatetime -I\$(top_srcdir)/libfdatetime";
   ac_cv_libfdatetime_LIBADD="../libfdatetime/libfdatetime.la";
 
   ac_cv_libfdatetime=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATETIME 1" >>confdefs.h
@@ -50232,15 +50264,15 @@
 printf "%s\n" "$ac_cv_with_libfguid" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfguid" = xno
 then :
   ac_cv_libfguid=no
 else $as_nop
   ac_cv_libfguid=check
-        if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect
+                if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes
 then :
   if test -d "$ac_cv_with_libfguid"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfguid}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfguid}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -50814,15 +50846,16 @@
 fi
 
 
         ac_cv_libfguid_LIBADD="-lfguid"
 fi
 
 fi
-    if test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_libfguid" != xyes
+
+    if test "x$ac_cv_libfguid" != xyes && test "x$ac_cv_with_libfguid" != x && test "x$ac_cv_with_libfguid" != xauto-detect && test "x$ac_cv_with_libfguid" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfguid in directory: $ac_cv_with_libfguid
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -50847,15 +50880,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfguid" != xyes
 then :
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFGUID 1" >>confdefs.h
@@ -50925,15 +50958,15 @@
 printf "%s\n" "$ac_cv_with_libfvalue" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfvalue" = xno
 then :
   ac_cv_libfvalue=no
 else $as_nop
   ac_cv_libfvalue=check
-        if test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect
+                if test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes
 then :
   if test -d "$ac_cv_with_libfvalue"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfvalue}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfvalue}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -55239,15 +55272,16 @@
 fi
 
 
         ac_cv_libfvalue_LIBADD="-lfvalue"
 fi
 
 fi
-    if test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_libfvalue" != xyes
+
+    if test "x$ac_cv_libfvalue" != xyes && test "x$ac_cv_with_libfvalue" != x && test "x$ac_cv_with_libfvalue" != xauto-detect && test "x$ac_cv_with_libfvalue" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfvalue in directory: $ac_cv_with_libfvalue
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -55272,15 +55306,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfvalue" != xyes
 then :
 
-  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue";
+  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue -I\$(top_srcdir)/libfvalue";
   ac_cv_libfvalue_LIBADD="../libfvalue/libfvalue.la";
 
   ac_cv_libfvalue=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFVALUE 1" >>confdefs.h
@@ -55350,15 +55384,15 @@
 printf "%s\n" "$ac_cv_with_libhmac" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libhmac" = xno
 then :
   ac_cv_libhmac=no
 else $as_nop
   ac_cv_libhmac=check
-        if test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect
+                if test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect && test "x$ac_cv_with_libhmac" != xyes
 then :
   if test -d "$ac_cv_with_libhmac"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libhmac}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libhmac}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -56356,15 +56390,16 @@
 fi
 
 
         ac_cv_libhmac_LIBADD="-lhmac"
 fi
 
 fi
-    if test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect && test "x$ac_cv_libhmac" != xyes
+
+    if test "x$ac_cv_libhmac" != xyes && test "x$ac_cv_with_libhmac" != x && test "x$ac_cv_with_libhmac" != xauto-detect && test "x$ac_cv_with_libhmac" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libhmac in directory: $ac_cv_with_libhmac
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -56470,15 +56505,15 @@
 
   if test "x$ac_cv_enable_static_executables" != xyes
 then :
       if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_openssl" = xno
 then :
   ac_cv_libcrypto=no
 else $as_nop
-      if test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect
+              if test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect && test "x$ac_cv_with_openssl" != xyes
 then :
   if test -d "$ac_cv_with_openssl"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_openssl}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_openssl}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -60656,15 +60691,15 @@
   if test "x$ac_cv_libcrypto" = xno || test "x$ac_cv_libcrypto_sha512" = xno
 then :
   ac_cv_libhmac_sha512=local
 else $as_nop
   ac_cv_libhmac_sha512=$ac_cv_libcrypto_sha512
 fi
 
-  ac_cv_libhmac_CPPFLAGS="-I../libhmac";
+  ac_cv_libhmac_CPPFLAGS="-I../libhmac -I\$(top_srcdir)/libhmac";
   ac_cv_libhmac_LIBADD="../libhmac/libhmac.la";
 
   ac_cv_libhmac=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBHMAC 1" >>confdefs.h
@@ -60734,15 +60769,15 @@
 printf "%s\n" "$ac_cv_with_libcaes" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libcaes" = xno
 then :
   ac_cv_libcaes=no
 else $as_nop
   ac_cv_libcaes=check
-        if test "x$ac_cv_with_libcaes" != x && test "x$ac_cv_with_libcaes" != xauto-detect
+                if test "x$ac_cv_with_libcaes" != x && test "x$ac_cv_with_libcaes" != xauto-detect && test "x$ac_cv_with_libcaes" != xyes
 then :
   if test -d "$ac_cv_with_libcaes"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libcaes}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libcaes}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -61318,15 +61353,16 @@
 fi
 
 
         ac_cv_libcaes_LIBADD="-lcaes"
 fi
 
 fi
-    if test "x$ac_cv_with_libcaes" != x && test "x$ac_cv_with_libcaes" != xauto-detect && test "x$ac_cv_libcaes" != xyes
+
+    if test "x$ac_cv_libcaes" != xyes && test "x$ac_cv_with_libcaes" != x && test "x$ac_cv_with_libcaes" != xauto-detect && test "x$ac_cv_with_libcaes" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libcaes in directory: $ac_cv_with_libcaes
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -61424,15 +61460,15 @@
 
   if test "x$ac_cv_enable_static_executables" != xyes
 then :
       if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_openssl" = xno
 then :
   ac_cv_libcrypto=no
 else $as_nop
-      if test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect
+              if test "x$ac_cv_with_openssl" != x && test "x$ac_cv_with_openssl" != xauto-detect && test "x$ac_cv_with_openssl" != xyes
 then :
   if test -d "$ac_cv_with_openssl"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_openssl}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_openssl}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -64259,15 +64295,15 @@
   if test "x$ac_cv_libcrypto" = xno || test "x$ac_cv_libcrypto_aes_xts" = xno
 then :
   ac_cv_libcaes_aes_xts=local
 else $as_nop
   ac_cv_libcaes_aes_xts=$ac_cv_libcrypto_aes_xts
 fi
 
-  ac_cv_libcaes_CPPFLAGS="-I../libcaes";
+  ac_cv_libcaes_CPPFLAGS="-I../libcaes -I\$(top_srcdir)/libcaes";
   ac_cv_libcaes_LIBADD="../libcaes/libcaes.la";
 
   ac_cv_libcaes=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCAES 1" >>confdefs.h
@@ -64578,16 +64614,20 @@
         PYTHON_LDFLAGS=`${PYTHON_CONFIG} --ldflags 2>/dev/null`;
 
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for Python libraries" >&5
 printf %s "checking for Python libraries... " >&6; }
     { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $PYTHON_LDFLAGS" >&5
 printf "%s\n" "$PYTHON_LDFLAGS" >&6; }
 
-        case $host_os in #(
-  cygwin*) :
+        case $build in #(
+  *-*-cygwin*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-mingw*) :
+    PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
+  *-*-msys*) :
     PYTHON_LDFLAGS="${PYTHON_LDFLAGS} -no-undefined" ;; #(
   *) :
      ;; #(
   *) :
      ;;
 esac
 
@@ -64745,33 +64785,107 @@
   printf %s "(cached) " >&6
 else $as_nop
   ac_cv_with_libfuse=auto-detect
 fi
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_with_libfuse" >&5
 printf "%s\n" "$ac_cv_with_libfuse" >&6; }
 
-      if test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_with_libfuse" != xauto-detect
+    if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfuse" = xno
+then :
+  ac_cv_libfuse=no
+else $as_nop
+              if test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes
 then :
   if test -d "$ac_cv_with_libfuse"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfuse}/include"
-      LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"
+        LDFLAGS="$LDFLAGS -L${ac_cv_with_libfuse}/lib"
 else $as_nop
-  { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_libfuse" >&5
-printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_libfuse" >&2;}
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "no such directory: $ac_cv_with_libfuse
+See \`config.log' for more details" "$LINENO" 5; }
 
 fi
+else $as_nop
+        if test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"
+then :
 
+pkg_failed=no
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse3 >= 3.0" >&5
+printf %s "checking for fuse3 >= 3.0... " >&6; }
+
+if test -n "$fuse3_CFLAGS"; then
+    pkg_cv_fuse3_CFLAGS="$fuse3_CFLAGS"
+ elif test -n "$PKG_CONFIG"; then
+    if test -n "$PKG_CONFIG" && \
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"fuse3 >= 3.0\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "fuse3 >= 3.0") 2>&5
+  ac_status=$?
+  printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
+  test $ac_status = 0; }; then
+  pkg_cv_fuse3_CFLAGS=`$PKG_CONFIG --cflags "fuse3 >= 3.0" 2>/dev/null`
+		      test "x$?" != "x0" && pkg_failed=yes
+else
+  pkg_failed=yes
+fi
+ else
+    pkg_failed=untried
+fi
+if test -n "$fuse3_LIBS"; then
+    pkg_cv_fuse3_LIBS="$fuse3_LIBS"
+ elif test -n "$PKG_CONFIG"; then
+    if test -n "$PKG_CONFIG" && \
+    { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$PKG_CONFIG --exists --print-errors \"fuse3 >= 3.0\""; } >&5
+  ($PKG_CONFIG --exists --print-errors "fuse3 >= 3.0") 2>&5
+  ac_status=$?
+  printf "%s\n" "$as_me:${as_lineno-$LINENO}: \$? = $ac_status" >&5
+  test $ac_status = 0; }; then
+  pkg_cv_fuse3_LIBS=`$PKG_CONFIG --libs "fuse3 >= 3.0" 2>/dev/null`
+		      test "x$?" != "x0" && pkg_failed=yes
+else
+  pkg_failed=yes
+fi
+ else
+    pkg_failed=untried
 fi
 
-  if test "x$ac_cv_with_libfuse" = xno
-then :
-  ac_cv_libfuse=no
-else $as_nop
-      if test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"
+
+
+if test $pkg_failed = yes; then
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: no" >&5
+printf "%s\n" "no" >&6; }
+
+if $PKG_CONFIG --atleast-pkgconfig-version 0.20; then
+        _pkg_short_errors_supported=yes
+else
+        _pkg_short_errors_supported=no
+fi
+        if test $_pkg_short_errors_supported = yes; then
+                fuse3_PKG_ERRORS=`$PKG_CONFIG --short-errors --print-errors --cflags --libs "fuse3 >= 3.0" 2>&1`
+        else
+                fuse3_PKG_ERRORS=`$PKG_CONFIG --print-errors --cflags --libs "fuse3 >= 3.0" 2>&1`
+        fi
+        # Put the nasty error message in config.log where it belongs
+        echo "$fuse3_PKG_ERRORS" >&5
+
+        ac_cv_libfuse=no
+elif test $pkg_failed = untried; then
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: no" >&5
+printf "%s\n" "no" >&6; }
+        ac_cv_libfuse=no
+else
+        fuse3_CFLAGS=$pkg_cv_fuse3_CFLAGS
+        fuse3_LIBS=$pkg_cv_fuse3_LIBS
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: yes" >&5
+printf "%s\n" "yes" >&6; }
+        ac_cv_libfuse=libfuse3
+fi
+
+        if test "x$ac_cv_libfuse" = xno
 then :
 
 pkg_failed=no
 { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse >= 2.6" >&5
 printf %s "checking for fuse >= 2.6... " >&6; }
 
 if test -n "$fuse_CFLAGS"; then
@@ -64839,51 +64953,110 @@
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: yes" >&5
 printf "%s\n" "yes" >&6; }
         ac_cv_libfuse=libfuse
 fi
 
 fi
 
-    if test "x$ac_cv_libfuse" = xlibfuse
+        if test "x$ac_cv_libfuse" = xlibfuse3
 then :
-  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS"
-      ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"
-else $as_nop
-               for ac_header in fuse.h
-do :
-  ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
+  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse3_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse3_LIBS"
+fi
+
+        if test "x$ac_cv_libfuse" = xlibfuse
+then :
+  ac_cv_libfuse_CPPFLAGS="$pkg_cv_fuse_CFLAGS -D_FILE_OFFSET_BITS=64"
+          ac_cv_libfuse_LIBADD="$pkg_cv_fuse_LIBS"
+fi
+
+fi
+
+fi
+
+    backup_CPPFLAGS="$CPPFLAGS"
+
+        if test "x$ac_cv_libfuse" != xlibfuse && test "x$ac_cv_libfuse" != xlibfuse3
+then :
+
+      CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=30"
+      ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_FUSE_H 1" >>confdefs.h
- ac_cv_header_fuse_h=yes
-else $as_nop
-  ac_cv_header_fuse_h=no
+
 fi
 
-done
 
-                  if test "x$ac_cv_header_fuse_h" = xno
+      if test "x$ac_cv_header_fuse_h" = xyes
 then :
-  { ac_cv_header_fuse_h=; unset ac_cv_header_fuse_h;}
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64 -DFUSE_USE_VERSION=26"
+  ac_cv_libfuse=libfuse3
+else $as_nop
+  CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
         ac_fn_c_check_header_compile "$LINENO" "fuse.h" "ac_cv_header_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_FUSE_H 1" >>confdefs.h
 
 fi
 
 
+        if test "x$ac_cv_header_fuse_h" = xyes
+then :
+  ac_cv_libfuse=libfuse
+fi
+
 fi
 
       if test "x$ac_cv_header_fuse_h" = xno
 then :
   ac_cv_libfuse=no
 else $as_nop
-          ac_cv_libfuse=libfuse
+          { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_invalidate in -lfuse" >&5
+printf %s "checking for fuse_invalidate in -lfuse... " >&6; }
+if test ${ac_cv_lib_fuse_fuse_invalidate+y}
+then :
+  printf %s "(cached) " >&6
+else $as_nop
+  ac_check_lib_save_LIBS=$LIBS
+LIBS="-lfuse  $LIBS"
+cat confdefs.h - <<_ACEOF >conftest.$ac_ext
+/* end confdefs.h.  */
+
+/* Override any GCC internal prototype to avoid an error.
+   Use char because int might match the return type of a GCC
+   builtin and then its argument prototype would still apply.  */
+char fuse_invalidate ();
+int
+main (void)
+{
+return fuse_invalidate ();
+  ;
+  return 0;
+}
+_ACEOF
+if ac_fn_c_try_link "$LINENO"
+then :
+  ac_cv_lib_fuse_fuse_invalidate=yes
+else $as_nop
+  ac_cv_lib_fuse_fuse_invalidate=no
+fi
+rm -f core conftest.err conftest.$ac_objext conftest.beam \
+    conftest$ac_exeext conftest.$ac_ext
+LIBS=$ac_check_lib_save_LIBS
+fi
+{ printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: $ac_cv_lib_fuse_fuse_invalidate" >&5
+printf "%s\n" "$ac_cv_lib_fuse_fuse_invalidate" >&6; }
+if test "x$ac_cv_lib_fuse_fuse_invalidate" = xyes
+then :
+  ac_cv_libfuse=libfuse
+else $as_nop
+  ac_cv_libfuse=libfuse3
+fi
+
 
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_daemonize in -lfuse" >&5
 printf %s "checking for fuse_daemonize in -lfuse... " >&6; }
 if test ${ac_cv_lib_fuse_fuse_daemonize+y}
 then :
   printf %s "(cached) " >&6
 else $as_nop
@@ -65046,45 +65219,38 @@
 then :
   ac_cv_libfuse_dummy=yes
 else $as_nop
   ac_cv_libfuse=no
 fi
 
 
-        ac_cv_libfuse_LIBADD="-lfuse";
+                ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
 
+        if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ac_cv_libfuse_LIBADD="-lfuse3"
+else $as_nop
+  ac_cv_libfuse_LIBADD="-lfuse"
 fi
 
 fi
 
-        if test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno
-then :
-  CPPFLAGS="$CPPFLAGS -DFUSE_USE_VERSION=26"
-      ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
-if test "x$ac_cv_header_osxfuse_fuse_h" = xyes
-then :
-  printf "%s\n" "#define HAVE_OSXFUSE_FUSE_H 1" >>confdefs.h
-
 fi
 
-
-            if test "x$ac_cv_header_osxfuse_fuse_h" = xno
+        if test "x$ac_cv_with_libfuse" != xno && test "x$ac_cv_header_fuse_h" = xno
 then :
-  { ac_cv_header_osxfuse_fuse_h=; unset ac_cv_header_osxfuse_fuse_h;}
-        CPPFLAGS="$CPPFLAGS -D_FILE_OFFSET_BITS=64"
-        ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
+  CPPFLAGS="$backup_CPPFLAGS -DFUSE_USE_VERSION=26"
+      ac_fn_c_check_header_compile "$LINENO" "osxfuse/fuse.h" "ac_cv_header_osxfuse_fuse_h" "$ac_includes_default"
 if test "x$ac_cv_header_osxfuse_fuse_h" = xyes
 then :
   printf "%s\n" "#define HAVE_OSXFUSE_FUSE_H 1" >>confdefs.h
 
 fi
 
 
-fi
-
       if test "x$ac_cv_header_osxfuse_fuse_h" = xno
 then :
   ac_cv_libfuse=no
 else $as_nop
           ac_cv_libfuse=libosxfuse
 
         { printf "%s\n" "$as_me:${as_lineno-$LINENO}: checking for fuse_daemonize in -losxfuse" >&5
@@ -65252,29 +65418,49 @@
 then :
   ac_cv_libfuse_dummy=yes
 else $as_nop
   ac_cv_libfuse=no
 fi
 
 
+                ac_cv_libfuse_CPPFLAGS="-D_FILE_OFFSET_BITS=64"
+
         ac_cv_libfuse_LIBADD="-losxfuse";
 
 fi
 
 fi
 
+    if test "x$ac_cv_libfuse" != xyes && test "x$ac_cv_with_libfuse" != x && test "x$ac_cv_with_libfuse" != xauto-detect && test "x$ac_cv_with_libfuse" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported libfuse in directory: $ac_cv_with_libfuse
+See \`config.log' for more details" "$LINENO" 5; }
+
+fi
+
+    CPPFLAGS="$backup_CPPFLAGS"
+
 fi
 
   if test "x$ac_cv_libfuse" = xlibfuse
 then :
 
 printf "%s\n" "#define HAVE_LIBFUSE 1" >>confdefs.h
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+
+printf "%s\n" "#define HAVE_LIBFUSE3 1" >>confdefs.h
+
+
+fi
   if test "x$ac_cv_libfuse" = xlibosxfuse
 then :
 
 printf "%s\n" "#define HAVE_LIBOSXFUSE 1" >>confdefs.h
 
 
 fi
@@ -65305,14 +65491,20 @@
 
   if test "x$ac_cv_libfuse" = xlibfuse
 then :
   ax_libfuse_pc_libs_private=-lfuse
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ax_libfuse_pc_libs_private=-lfuse3
+
+
+fi
   if test "x$ac_cv_libfuse" = xlibosxfuse
 then :
   ax_libfuse_pc_libs_private=-losxfuse
 
 
 fi
 
@@ -65320,14 +65512,22 @@
 then :
   ax_libfuse_spec_requires=fuse-libs
 
     ax_libfuse_spec_build_requires=fuse-devel
 
 
 fi
+  if test "x$ac_cv_libfuse" = xlibfuse3
+then :
+  ax_libfuse_spec_requires=fuse3-libs
+
+    ax_libfuse_spec_build_requires=fuse3-devel
+
+
+fi
 
 
 ac_fn_c_check_header_compile "$LINENO" "signal.h" "ac_cv_header_signal_h" "$ac_includes_default"
 if test "x$ac_cv_header_signal_h" = xyes
 then :
   printf "%s\n" "#define HAVE_SIGNAL_H 1" >>confdefs.h
 
@@ -66291,15 +66491,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libbde $as_me 20240223, which was
+This file was extended by libbde $as_me 20240502, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -66359,15 +66559,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libbde config.status 20240223
+libbde config.status 20240502
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libbde-20240223/compile` & `libbde-20240502/compile`

 * *Files identical despite different names*

### Comparing `libbde-20240223/missing` & `libbde-20240502/missing`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/bde_test_sector_data/bde_test_sector_data.vcproj` & `libbde-20240502/msvscpp/bde_test_sector_data/bde_test_sector_data.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/bde_test_key_protector/bde_test_key_protector.vcproj` & `libbde-20240502/msvscpp/bde_test_key_protector/bde_test_key_protector.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/bde_test_key/bde_test_key.vcproj` & `libbde-20240502/msvscpp/bde_test_key/bde_test_key.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/pybde/pybde.vcproj` & `libbde-20240502/msvscpp/pybde/pybde.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/libcaes/libcaes.vcproj` & `libbde-20240502/msvscpp/libcaes/libcaes.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/libfguid/libfguid.vcproj` & `libbde-20240502/msvscpp/libfguid/libfguid.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/bdemount/bdemount.vcproj` & `libbde-20240502/msvscpp/bdemount/bdemount.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/bde_test_stretch_key/bde_test_stretch_key.vcproj` & `libbde-20240502/msvscpp/bde_test_stretch_key/bde_test_stretch_key.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/bde_test_sector_data_vector/bde_test_sector_data_vector.vcproj` & `libbde-20240502/msvscpp/bde_test_sector_data_vector/bde_test_sector_data_vector.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/libclocale/libclocale.vcproj` & `libbde-20240502/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/bde_test_tools_output/bde_test_tools_output.vcproj` & `libbde-20240502/msvscpp/bde_test_tools_output/bde_test_tools_output.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/bde_test_tools_signal/bde_test_tools_signal.vcproj` & `libbde-20240502/msvscpp/bde_test_tools_signal/bde_test_tools_signal.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/libfcache/libfcache.vcproj` & `libbde-20240502/msvscpp/libfcache/libfcache.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/Makefile.am` & `libbde-20240502/msvscpp/Makefile.am`

 * *Files 2% similar despite different names*

```diff
@@ -44,13 +44,11 @@
 	libuna/libuna.vcproj \
 	pybde/pybde.vcproj \
 	libbde.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libbde-20240223/msvscpp/libbfio/libbfio.vcproj` & `libbde-20240502/msvscpp/libbfio/libbfio.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/bde_test_notify/bde_test_notify.vcproj` & `libbde-20240502/msvscpp/bde_test_notify/bde_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/bde_test_volume/bde_test_volume.vcproj` & `libbde-20240502/msvscpp/bde_test_volume/bde_test_volume.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/bde_test_aes_ccm_encrypted_key/bde_test_aes_ccm_encrypted_key.vcproj` & `libbde-20240502/msvscpp/bde_test_aes_ccm_encrypted_key/bde_test_aes_ccm_encrypted_key.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/libcfile/libcfile.vcproj` & `libbde-20240502/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/libbde/libbde.vcproj` & `libbde-20240502/msvscpp/libbde/libbde.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/bde_test_external_key/bde_test_external_key.vcproj` & `libbde-20240502/msvscpp/bde_test_external_key/bde_test_external_key.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/libcdata/libcdata.vcproj` & `libbde-20240502/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/bde_test_volume_header/bde_test_volume_header.vcproj` & `libbde-20240502/msvscpp/bde_test_volume_header/bde_test_volume_header.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/bde_test_volume_master_key/bde_test_volume_master_key.vcproj` & `libbde-20240502/msvscpp/bde_test_volume_master_key/bde_test_volume_master_key.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/libbde.sln` & `libbde-20240502/msvscpp/libbde.sln`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/bde_test_password_keep/bde_test_password_keep.vcproj` & `libbde-20240502/msvscpp/bde_test_password_keep/bde_test_password_keep.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/bde_test_encryption_context/bde_test_encryption_context.vcproj` & `libbde-20240502/msvscpp/bde_test_encryption_context/bde_test_encryption_context.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/bdeinfo/bdeinfo.vcproj` & `libbde-20240502/msvscpp/bdeinfo/bdeinfo.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/libcthreads/libcthreads.vcproj` & `libbde-20240502/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/bde_test_support/bde_test_support.vcproj` & `libbde-20240502/msvscpp/bde_test_support/bde_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/bde_test_metadata/bde_test_metadata.vcproj` & `libbde-20240502/msvscpp/bde_test_metadata/bde_test_metadata.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/bde_test_error/bde_test_error.vcproj` & `libbde-20240502/msvscpp/bde_test_error/bde_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/libcpath/libcpath.vcproj` & `libbde-20240502/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/bde_test_io_handle/bde_test_io_handle.vcproj` & `libbde-20240502/msvscpp/bde_test_io_handle/bde_test_io_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/bde_test_metadata_header/bde_test_metadata_header.vcproj` & `libbde-20240502/msvscpp/bde_test_metadata_header/bde_test_metadata_header.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/libhmac/libhmac.vcproj` & `libbde-20240502/msvscpp/libhmac/libhmac.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/bde_test_metadata_block_header/bde_test_metadata_block_header.vcproj` & `libbde-20240502/msvscpp/bde_test_metadata_block_header/bde_test_metadata_block_header.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/libcsplit/libcsplit.vcproj` & `libbde-20240502/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/bde_test_metadata_entry/bde_test_metadata_entry.vcproj` & `libbde-20240502/msvscpp/bde_test_metadata_entry/bde_test_metadata_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/libuna/libuna.vcproj` & `libbde-20240502/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/Makefile.in` & `libbde-20240502/msvscpp/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -411,14 +411,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -530,15 +532,16 @@
 	libuna/libuna.vcproj \
 	pybde/pybde.vcproj \
 	libbde.sln
 
 EXTRA_DIST = \
 	$(MSVSCPP_FILES)
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -642,23 +645,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -737,13 +742,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libbde-20240223/msvscpp/libfvalue/libfvalue.vcproj` & `libbde-20240502/msvscpp/libfvalue/libfvalue.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/libcnotify/libcnotify.vcproj` & `libbde-20240502/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/libcerror/libcerror.vcproj` & `libbde-20240502/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/libfdatetime/libfdatetime.vcproj` & `libbde-20240502/msvscpp/libfdatetime/libfdatetime.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/bde_test_password/bde_test_password.vcproj` & `libbde-20240502/msvscpp/bde_test_password/bde_test_password.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/msvscpp/bde_test_tools_info_handle/bde_test_tools_info_handle.vcproj` & `libbde-20240502/msvscpp/bde_test_tools_info_handle/bde_test_tools_info_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcfile/libcfile_extern.h` & `libbde-20240502/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcfile/libcfile_support.h` & `libbde-20240502/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcfile/libcfile_unused.h` & `libbde-20240502/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcfile/libcfile_notify.h` & `libbde-20240502/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcfile/libcfile_support.c` & `libbde-20240502/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcfile/libcfile_types.h` & `libbde-20240502/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcfile/Makefile.am` & `libbde-20240502/libcfile/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCFILE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcfile.la
 
@@ -22,19 +22,17 @@
 	libcfile_support.c libcfile_support.h \
 	libcfile_system_string.c libcfile_system_string.h \
 	libcfile_types.h \
 	libcfile_unused.h \
 	libcfile_winapi.c libcfile_winapi.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
```

### Comparing `libbde-20240223/libcfile/libcfile_notify.c` & `libbde-20240502/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcfile/libcfile_system_string.h` & `libbde-20240502/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcfile/libcfile_file.h` & `libbde-20240502/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcfile/libcfile_libcnotify.h` & `libbde-20240502/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcfile/libcfile_system_string.c` & `libbde-20240502/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcfile/libcfile_error.h` & `libbde-20240502/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcfile/libcfile_libcerror.h` & `libbde-20240502/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcfile/libcfile_file.c` & `libbde-20240502/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcfile/libcfile_libclocale.h` & `libbde-20240502/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcfile/libcfile_winapi.h` & `libbde-20240502/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcfile/Makefile.in` & `libbde-20240502/libcfile/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -476,14 +476,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -546,16 +548,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCFILE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCFILE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCFILE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCFILE_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCFILE_TRUE@noinst_LTLIBRARIES = libcfile.la
 @HAVE_LOCAL_LIBCFILE_TRUE@libcfile_la_SOURCES = \
@@ -570,15 +572,16 @@
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_notify.c libcfile_notify.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_support.c libcfile_support.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_system_string.c libcfile_system_string.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_types.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_unused.h \
 @HAVE_LOCAL_LIBCFILE_TRUE@	libcfile_winapi.c libcfile_winapi.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -783,24 +786,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcfile_error.Plo
+	-rm -f ./$(DEPDIR)/libcfile_file.Plo
+	-rm -f ./$(DEPDIR)/libcfile_notify.Plo
+	-rm -f ./$(DEPDIR)/libcfile_support.Plo
+	-rm -f ./$(DEPDIR)/libcfile_system_string.Plo
+	-rm -f ./$(DEPDIR)/libcfile_winapi.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -889,17 +900,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcfile ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcfile_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libbde-20240223/libcfile/libcfile_error.c` & `libbde-20240502/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcfile/libcfile_libuna.h` & `libbde-20240502/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcfile/libcfile_winapi.c` & `libbde-20240502/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcfile/libcfile_definitions.h` & `libbde-20240502/libcfile/libcfile_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcfile/definitions.h>
 
 /* The definitions in <libcfile/definitions.h> are copied here
  * for local use of libcfile
  */
 #else
 
-#define LIBCFILE_VERSION				20240106
+#define LIBCFILE_VERSION				20240414
 
 /* The libcfile version string
  */
-#define LIBCFILE_VERSION_STRING				"20240106"
+#define LIBCFILE_VERSION_STRING				"20240414"
 
 /* The file access flags
  * bit 1	set to 1 for read access
  * bit 2	set to 1 for write access
  * bit 3	set to 1 to truncate an existing file on write
  * bit 4-8	not used
  */
```

### Comparing `libbde-20240223/README` & `libbde-20240502/README`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde.pc.in` & `libbde-20240502/libbde.pc.in`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_sector_data_vector.h` & `libbde-20240502/libbde/libbde_sector_data_vector.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_libfcache.h` & `libbde-20240502/libbde/libbde_libfcache.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_debug.h` & `libbde-20240502/libbde/libbde_debug.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_metadata_header.c` & `libbde-20240502/libbde/libbde_metadata_header.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_notify.c` & `libbde-20240502/libbde/libbde_notify.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_external_key.c` & `libbde-20240502/libbde/libbde_external_key.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_ntfs_volume_header.c` & `libbde-20240502/libbde/libbde_ntfs_volume_header.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_libuna.h` & `libbde-20240502/libbde/libbde_libuna.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_metadata_entry.h` & `libbde-20240502/libbde/libbde_metadata_entry.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_password_keep.h` & `libbde-20240502/libbde/libbde_password_keep.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_volume_master_key.h` & `libbde-20240502/libbde/libbde_volume_master_key.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_libcnotify.h` & `libbde-20240502/libbde/libbde_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_support.c` & `libbde-20240502/libbde/libbde_support.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_key_protector.h` & `libbde-20240502/libbde/libbde_key_protector.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/bde_volume.h` & `libbde-20240502/libbde/bde_volume.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_volume.h` & `libbde-20240502/libbde/libbde_volume.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_metadata_entry.c` & `libbde-20240502/libbde/libbde_metadata_entry.c`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -465,18 +465,18 @@
 		libcnotify_printf(
 		 "\n" );
 	}
 #endif /* defined( HAVE_DEBUG_OUTPUT ) */
 
 	return( 1 );
 
-on_error:
 #if defined( HAVE_DEBUG_OUTPUT )
+on_error:
 	if( value_string != NULL )
 	{
 		memory_free(
 		 value_string );
 	}
-#endif
 	return( -1 );
+#endif
 }
```

### Comparing `libbde-20240223/libbde/libbde_external_key.h` & `libbde-20240502/libbde/libbde_external_key.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_sector_data_vector.c` & `libbde-20240502/libbde/libbde_sector_data_vector.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_password_keep.c` & `libbde-20240502/libbde/libbde_password_keep.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_stretch_key.h` & `libbde-20240502/libbde/libbde_stretch_key.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_libclocale.h` & `libbde-20240502/libbde/libbde_libclocale.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_aes_ccm_encrypted_key.c` & `libbde-20240502/libbde/libbde_aes_ccm_encrypted_key.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_libcdata.h` & `libbde-20240502/libbde/libbde_libcdata.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_notify.h` & `libbde-20240502/libbde/libbde_notify.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_recovery.c` & `libbde-20240502/libbde/libbde_recovery.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_definitions.h.in` & `libbde-20240502/libbde/libbde_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/Makefile.am` & `libbde-20240502/libbde/Makefile.am`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -94,21 +94,19 @@
 libbde_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libbde_definitions.h.in \
 	libbde.rc \
 	libbde.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libbde_definitions.h \
+	libbde.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libbde_definitions.h
-	-rm -f libbde.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libbde ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbde_la_SOURCES)
```

### Comparing `libbde-20240223/libbde/libbde_metadata.h` & `libbde-20240502/libbde/libbde_metadata.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/bde_metadata.h` & `libbde-20240502/libbde/bde_metadata.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_libfguid.h` & `libbde-20240502/libbde/libbde_libfguid.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_volume.c` & `libbde-20240502/libbde/libbde_volume.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_diffuser.h` & `libbde-20240502/libbde/libbde_diffuser.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_libhmac.h` & `libbde-20240502/libbde/libbde_libhmac.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_password.c` & `libbde-20240502/libbde/libbde_password.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde.rc` & `libbde-20240502/libbde/libbde.rc`

 * *Files 2% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the BitLocker Drive Encryption (BDE) format\0"
-      VALUE "FileVersion",		"20240223" "\0"
+      VALUE "FileVersion",		"20240502" "\0"
       VALUE "InternalName",		"libbde.dll\0"
       VALUE "LegalCopyright",		"(C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libbde.dll\0"
       VALUE "ProductName",		"libbde\0"
-      VALUE "ProductVersion",		"20240223" "\0"
+      VALUE "ProductVersion",		"20240502" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libbde/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libbde-20240223/libbde/libbde_libbfio.h` & `libbde-20240502/libbde/libbde_libbfio.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_metadata_header.h` & `libbde-20240502/libbde/libbde_metadata_header.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_support.h` & `libbde-20240502/libbde/libbde_support.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_libfvalue.h` & `libbde-20240502/libbde/libbde_libfvalue.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_io_handle.c` & `libbde-20240502/libbde/libbde_io_handle.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_sector_data.h` & `libbde-20240502/libbde/libbde_sector_data.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_stretch_key.c` & `libbde-20240502/libbde/libbde_stretch_key.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_ntfs_volume_header.h` & `libbde-20240502/libbde/libbde_ntfs_volume_header.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde.rc.in` & `libbde-20240502/libbde/libbde.rc.in`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_extern.h` & `libbde-20240502/libbde/libbde_extern.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_metadata_block_header.c` & `libbde-20240502/libbde/libbde_metadata_block_header.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_libfdatetime.h` & `libbde-20240502/libbde/libbde_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde.c` & `libbde-20240502/libbde/libbde.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_encryption_context.h` & `libbde-20240502/libbde/libbde_encryption_context.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_diffuser.c` & `libbde-20240502/libbde/libbde_diffuser.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_sector_data.c` & `libbde-20240502/libbde/libbde_sector_data.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_definitions.h` & `libbde-20240502/libbde/libbde_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 #if !defined( HAVE_LOCAL_LIBBDE )
 #include <libbde/definitions.h>
 
 /* The definitions in <libbde/definitions.h> are copied here
  * for local use of libbde
  */
 #else
-#define LIBBDE_VERSION					20240223
+#define LIBBDE_VERSION					20240502
 
 /* The version string
  */
-#define LIBBDE_VERSION_STRING				"20240223"
+#define LIBBDE_VERSION_STRING				"20240502"
 
 /* The file access
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBBDE_ACCESS_FLAGS
```

### Comparing `libbde-20240223/libbde/libbde_metadata.c` & `libbde-20240502/libbde/libbde_metadata.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_metadata_block_header.h` & `libbde-20240502/libbde/libbde_metadata_block_header.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_key.c` & `libbde-20240502/libbde/libbde_key.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_volume_master_key.c` & `libbde-20240502/libbde/libbde_volume_master_key.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_password.h` & `libbde-20240502/libbde/libbde_password.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_recovery.h` & `libbde-20240502/libbde/libbde_recovery.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_types.h` & `libbde-20240502/libbde/libbde_types.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_libcerror.h` & `libbde-20240502/libbde/libbde_libcerror.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_aes_ccm_encrypted_key.h` & `libbde-20240502/libbde/libbde_aes_ccm_encrypted_key.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_volume_header.c` & `libbde-20240502/libbde/libbde_volume_header.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_libcthreads.h` & `libbde-20240502/libbde/libbde_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/Makefile.in` & `libbde-20240502/libbde/Makefile.in`

 * *Files 5% similar despite different names*

```diff
@@ -524,14 +524,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -594,16 +596,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -691,15 +693,18 @@
 
 libbde_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libbde_definitions.h.in \
 	libbde.rc \
 	libbde.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libbde_definitions.h \
+	libbde.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -955,24 +960,52 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libLTLIBRARIES clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libbde.Plo
+	-rm -f ./$(DEPDIR)/libbde_aes_ccm_encrypted_key.Plo
+	-rm -f ./$(DEPDIR)/libbde_debug.Plo
+	-rm -f ./$(DEPDIR)/libbde_diffuser.Plo
+	-rm -f ./$(DEPDIR)/libbde_encryption_context.Plo
+	-rm -f ./$(DEPDIR)/libbde_error.Plo
+	-rm -f ./$(DEPDIR)/libbde_external_key.Plo
+	-rm -f ./$(DEPDIR)/libbde_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libbde_key.Plo
+	-rm -f ./$(DEPDIR)/libbde_key_protector.Plo
+	-rm -f ./$(DEPDIR)/libbde_metadata.Plo
+	-rm -f ./$(DEPDIR)/libbde_metadata_block_header.Plo
+	-rm -f ./$(DEPDIR)/libbde_metadata_entry.Plo
+	-rm -f ./$(DEPDIR)/libbde_metadata_header.Plo
+	-rm -f ./$(DEPDIR)/libbde_notify.Plo
+	-rm -f ./$(DEPDIR)/libbde_ntfs_volume_header.Plo
+	-rm -f ./$(DEPDIR)/libbde_password.Plo
+	-rm -f ./$(DEPDIR)/libbde_password_keep.Plo
+	-rm -f ./$(DEPDIR)/libbde_recovery.Plo
+	-rm -f ./$(DEPDIR)/libbde_sector_data.Plo
+	-rm -f ./$(DEPDIR)/libbde_sector_data_vector.Plo
+	-rm -f ./$(DEPDIR)/libbde_stretch_key.Plo
+	-rm -f ./$(DEPDIR)/libbde_support.Plo
+	-rm -f ./$(DEPDIR)/libbde_volume.Plo
+	-rm -f ./$(DEPDIR)/libbde_volume_header.Plo
+	-rm -f ./$(DEPDIR)/libbde_volume_master_key.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1081,19 +1114,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libbde_definitions.h
-	-rm -f libbde.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libbde ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libbde_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libbde-20240223/libbde/libbde_volume_header.h` & `libbde-20240502/libbde/libbde_volume_header.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_io_handle.h` & `libbde-20240502/libbde/libbde_io_handle.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_encryption_context.c` & `libbde-20240502/libbde/libbde_encryption_context.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_unused.h` & `libbde-20240502/libbde/libbde_unused.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_debug.c` & `libbde-20240502/libbde/libbde_debug.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_codepage.h` & `libbde-20240502/libbde/libbde_codepage.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_key_protector.c` & `libbde-20240502/libbde/libbde_key_protector.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_error.h` & `libbde-20240502/libbde/libbde_error.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_libcaes.h` & `libbde-20240502/libbde/libbde_libcaes.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_error.c` & `libbde-20240502/libbde/libbde_error.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde/libbde_key.h` & `libbde-20240502/libbde/libbde_key.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/INSTALL` & `libbde-20240502/INSTALL`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcdata/libcdata_list_element.h` & `libbde-20240502/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcdata/libcdata_array.h` & `libbde-20240502/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcdata/libcdata_definitions.h` & `libbde-20240502/libcdata/libcdata_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcdata/definitions.h>
 
 /* The definitions in <libcdata/definitions.h> are copied here
  * for local use of libcdata
  */
 #else
 
-#define LIBCDATA_VERSION				20240103
+#define LIBCDATA_VERSION				20240414
 
 /* The libcdata version string
  */
-#define LIBCDATA_VERSION_STRING				"20240103"
+#define LIBCDATA_VERSION_STRING				"20240414"
 
 /* The comparison function definitions
  */
 enum LIBCDATA_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libbde-20240223/libcdata/libcdata_libcerror.h` & `libbde-20240502/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcdata/libcdata_unused.h` & `libbde-20240502/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcdata/libcdata_btree.h` & `libbde-20240502/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcdata/libcdata_btree.c` & `libbde-20240502/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcdata/libcdata_support.c` & `libbde-20240502/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcdata/libcdata_list.c` & `libbde-20240502/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcdata/libcdata_extern.h` & `libbde-20240502/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcdata/libcdata_list.h` & `libbde-20240502/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcdata/libcdata_btree_values_list.h` & `libbde-20240502/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcdata/Makefile.am` & `libbde-20240502/libcdata/Makefile.am`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcdata.la
 
 libcdata_la_SOURCES = \
@@ -24,19 +24,17 @@
 	libcdata_range_list_value.c libcdata_range_list_value.h \
 	libcdata_support.c libcdata_support.h \
 	libcdata_tree_node.c libcdata_tree_node.h \
 	libcdata_types.h \
 	libcdata_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
```

### Comparing `libbde-20240223/libcdata/libcdata_btree_node.h` & `libbde-20240502/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcdata/libcdata_range_list_value.h` & `libbde-20240502/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcdata/libcdata_range_list.h` & `libbde-20240502/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcdata/libcdata_range_list.c` & `libbde-20240502/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcdata/libcdata_array.c` & `libbde-20240502/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcdata/libcdata_list_element.c` & `libbde-20240502/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcdata/libcdata_libcthreads.h` & `libbde-20240502/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcdata/libcdata_tree_node.h` & `libbde-20240502/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcdata/libcdata_error.h` & `libbde-20240502/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcdata/libcdata_types.h` & `libbde-20240502/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcdata/libcdata_btree_node.c` & `libbde-20240502/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcdata/libcdata_tree_node.c` & `libbde-20240502/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcdata/libcdata_support.h` & `libbde-20240502/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcdata/Makefile.in` & `libbde-20240502/libcdata/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -490,14 +490,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -560,16 +562,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCDATA_TRUE@noinst_LTLIBRARIES = libcdata.la
 @HAVE_LOCAL_LIBCDATA_TRUE@libcdata_la_SOURCES = \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_array.c libcdata_array.h \
@@ -586,15 +588,16 @@
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list.c libcdata_range_list.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_range_list_value.c libcdata_range_list_value.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_support.c libcdata_support.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_tree_node.c libcdata_tree_node.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_types.h \
 @HAVE_LOCAL_LIBCDATA_TRUE@	libcdata_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -804,24 +807,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcdata_array.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_node.Plo
+	-rm -f ./$(DEPDIR)/libcdata_btree_values_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_error.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libcdata_range_list_value.Plo
+	-rm -f ./$(DEPDIR)/libcdata_support.Plo
+	-rm -f ./$(DEPDIR)/libcdata_tree_node.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -915,17 +931,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libbde-20240223/libcdata/libcdata_range_list_value.c` & `libbde-20240502/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcdata/libcdata_btree_values_list.c` & `libbde-20240502/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcdata/libcdata_error.c` & `libbde-20240502/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libbde.spec` & `libbde-20240502/libbde.spec`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libbde
-Version: 20240223
+Version: 20240502
 Release: 1
 Summary: Library to access the BitLocker Drive Encryption (BDE) format
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libbde
 Requires:         openssl        
@@ -36,16 +36,16 @@
 
 %description -n libbde-python3
 Python 3 bindings for libbde
 
 %package -n libbde-tools
 Summary: Several tools for reading BitLocker Drive Encryption volumes
 Group: Applications/System
-Requires: libbde = %{version}-%{release} fuse-libs
-BuildRequires: fuse-devel
+Requires: libbde = %{version}-%{release} fuse3-libs
+BuildRequires: fuse3-devel
 
 %description -n libbde-tools
 Several tools for reading BitLocker Drive Encryption volumes
 
 %prep
 %setup -q
 
@@ -91,10 +91,10 @@
 %files -n libbde-tools
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Fri Feb 23 2024 Joachim Metz <joachim.metz@gmail.com> 20240223-1
+* Thu May  2 2024 Joachim Metz <joachim.metz@gmail.com> 20240502-1
 - Auto-generated
```

### Comparing `libbde-20240223/config.sub` & `libbde-20240502/config.sub`

 * *Files identical despite different names*

### Comparing `libbde-20240223/setup.py` & `libbde-20240502/setup.py`

 * *Files identical despite different names*

### Comparing `libbde-20240223/acinclude.m4` & `libbde-20240502/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libbde-20240223/config.rpath` & `libbde-20240502/config.rpath`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcthreads/libcthreads_thread.h` & `libbde-20240502/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcthreads/libcthreads_read_write_lock.h` & `libbde-20240502/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcthreads/libcthreads_thread.c` & `libbde-20240502/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcthreads/libcthreads_thread_pool.h` & `libbde-20240502/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcthreads/libcthreads_support.h` & `libbde-20240502/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcthreads/libcthreads_lock.h` & `libbde-20240502/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcthreads/libcthreads_unused.h` & `libbde-20240502/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcthreads/libcthreads_lock.c` & `libbde-20240502/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcthreads/libcthreads_condition.h` & `libbde-20240502/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcthreads/libcthreads_repeating_thread.h` & `libbde-20240502/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcthreads/Makefile.am` & `libbde-20240502/libcthreads/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCTHREADS
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcthreads.la
 
 libcthreads_la_SOURCES = \
 	libcthreads_condition.c libcthreads_condition.h \
@@ -22,19 +22,17 @@
 	libcthreads_thread.c libcthreads_thread.h \
 	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 	libcthreads_types.h \
 	libcthreads_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
```

### Comparing `libbde-20240223/libcthreads/libcthreads_support.c` & `libbde-20240502/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcthreads/libcthreads_mutex.c` & `libbde-20240502/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcthreads/libcthreads_queue.c` & `libbde-20240502/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcthreads/libcthreads_mutex.h` & `libbde-20240502/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcthreads/libcthreads_types.h` & `libbde-20240502/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcthreads/libcthreads_thread_attributes.h` & `libbde-20240502/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcthreads/libcthreads_condition.c` & `libbde-20240502/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcthreads/libcthreads_error.c` & `libbde-20240502/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcthreads/libcthreads_read_write_lock.c` & `libbde-20240502/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcthreads/libcthreads_libcerror.h` & `libbde-20240502/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcthreads/libcthreads_definitions.h` & `libbde-20240502/libcthreads/libcthreads_definitions.h`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcthreads/definitions.h>
 
 /* The definitions in <libcthreads/definitions.h> are copied here
  * for local use of libcthreads
  */
 #else
 
-#define LIBCTHREADS_VERSION				20240102
+#define LIBCTHREADS_VERSION				20240413
 
 /* The libcthreads version string
  */
-#define LIBCTHREADS_VERSION_STRING			"20240102"
+#define LIBCTHREADS_VERSION_STRING			"20240413"
 
 /* The comparison function definitions
  */
 enum LIBCTHREADS_COMPARE_DEFINITIONS
 {
 	/* The first value is less than the second value
 	 */
```

### Comparing `libbde-20240223/libcthreads/libcthreads_thread_pool.c` & `libbde-20240502/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcthreads/libcthreads_error.h` & `libbde-20240502/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcthreads/libcthreads_thread_attributes.c` & `libbde-20240502/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcthreads/libcthreads_extern.h` & `libbde-20240502/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcthreads/libcthreads_repeating_thread.c` & `libbde-20240502/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcthreads/Makefile.in` & `libbde-20240502/libcthreads/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -494,14 +494,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -564,16 +566,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCTHREADS_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCTHREADS_TRUE@noinst_LTLIBRARIES = libcthreads.la
 @HAVE_LOCAL_LIBCTHREADS_TRUE@libcthreads_la_SOURCES = \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_condition.c libcthreads_condition.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_definitions.h \
@@ -588,15 +590,16 @@
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_support.c libcthreads_support.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread.c libcthreads_thread.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_attributes.c libcthreads_thread_attributes.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_thread_pool.c libcthreads_thread_pool.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_types.h \
 @HAVE_LOCAL_LIBCTHREADS_TRUE@	libcthreads_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -806,24 +809,37 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcthreads_condition.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_error.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_mutex.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_queue.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_read_write_lock.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_repeating_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_support.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_attributes.Plo
+	-rm -f ./$(DEPDIR)/libcthreads_thread_pool.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -917,17 +933,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcthreads ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcthreads_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libbde-20240223/libcthreads/libcthreads_queue.h` & `libbde-20240502/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/test-driver` & `libbde-20240502/test-driver`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcpath/libcpath_support.c` & `libbde-20240502/libcpath/libcpath_support.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcpath/libcpath_libcerror.h` & `libbde-20240502/libcpath/libcpath_libcerror.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcpath/libcpath_definitions.h` & `libbde-20240502/libcpath/libcpath_definitions.h`

 * *Files 4% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcpath/definitions.h>
 
 /* The definitions in <libcpath/definitions.h> are copied here
  * for local use of libcpath
  */
 #else
 
-#define LIBCPATH_VERSION			20240109
+#define LIBCPATH_VERSION			20240414
 
 /* The libcpath version string
  */
-#define LIBCPATH_VERSION_STRING			"20240109"
+#define LIBCPATH_VERSION_STRING			"20240414"
 
 #if defined( WINAPI )
 #define LIBCPATH_SEPARATOR			'\\'
 
 #else
 #define LIBCPATH_SEPARATOR			'/'
```

### Comparing `libbde-20240223/libcpath/Makefile.am` & `libbde-20240502/libcpath/Makefile.am`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCPATH
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcpath.la
 
@@ -19,19 +19,17 @@
 	libcpath_libcsplit.h \
 	libcpath_libuna.h \
 	libcpath_support.c libcpath_support.h \
 	libcpath_system_string.c libcpath_system_string.h \
 	libcpath_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
```

### Comparing `libbde-20240223/libcpath/libcpath_error.c` & `libbde-20240502/libcpath/libcpath_error.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcpath/libcpath_extern.h` & `libbde-20240502/libcpath/libcpath_extern.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcpath/libcpath_system_string.h` & `libbde-20240502/libcpath/libcpath_system_string.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcpath/libcpath_support.h` & `libbde-20240502/libcpath/libcpath_support.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcpath/libcpath_libcsplit.h` & `libbde-20240502/libcpath/libcpath_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcpath/libcpath_system_string.c` & `libbde-20240502/libcpath/libcpath_system_string.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcpath/libcpath_libclocale.h` & `libbde-20240502/libcpath/libcpath_libclocale.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcpath/libcpath_error.h` & `libbde-20240502/libcpath/libcpath_error.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcpath/Makefile.in` & `libbde-20240502/libcpath/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -470,14 +470,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -540,16 +542,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCPATH_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCPATH_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCPATH_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBCSPLIT_CPPFLAGS@ \
 @HAVE_LOCAL_LIBCPATH_TRUE@	@LIBUNA_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCPATH_TRUE@noinst_LTLIBRARIES = libcpath.la
 @HAVE_LOCAL_LIBCPATH_TRUE@libcpath_la_SOURCES = \
@@ -561,15 +563,16 @@
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libclocale.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libcsplit.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_libuna.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_support.c libcpath_support.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_system_string.c libcpath_system_string.h \
 @HAVE_LOCAL_LIBCPATH_TRUE@	libcpath_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -772,24 +775,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcpath_error.Plo
+	-rm -f ./$(DEPDIR)/libcpath_path.Plo
+	-rm -f ./$(DEPDIR)/libcpath_support.Plo
+	-rm -f ./$(DEPDIR)/libcpath_system_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -876,17 +885,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcpath ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcpath_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libbde-20240223/libcpath/libcpath_libuna.h` & `libbde-20240502/libcpath/libcpath_libuna.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcpath/libcpath_unused.h` & `libbde-20240502/libcpath/libcpath_unused.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcpath/libcpath_path.c` & `libbde-20240502/libcpath/libcpath_path.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcpath/libcpath_path.h` & `libbde-20240502/libcpath/libcpath_path.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/ChangeLog` & `libbde-20240502/ChangeLog`

 * *Files identical despite different names*

### Comparing `libbde-20240223/manuals/libbde.3` & `libbde-20240502/manuals/libbde.3`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-.Dd June 18, 2022
+.Dd May  2, 2024
 .Dt libbde 3
 .Os libbde
 .Sh NAME
 .Nm libbde.h
 .Nd Library to access the BitLocker Drive Encryption (BDE) format
 .Sh SYNOPSIS
 .In libbde.h
@@ -100,20 +100,20 @@
 .Fn libbde_volume_set_utf16_password "libbde_volume_t *volume" "const uint16_t *utf16_string" "size_t utf16_string_length" "libbde_error_t **error"
 .Ft int
 .Fn libbde_volume_set_utf8_recovery_password "libbde_volume_t *volume" "const uint8_t *utf8_string" "size_t utf8_string_length" "libbde_error_t **error"
 .Ft int
 .Fn libbde_volume_set_utf16_recovery_password "libbde_volume_t *volume" "const uint16_t *utf16_string" "size_t utf16_string_length" "libbde_error_t **error"
 .Ft int
 .Fn libbde_volume_read_startup_key "libbde_volume_t *volume" "const char *filename" "libbde_error_t **error"
+.Ft int
+.Fn libbde_volume_read_startup_key_wide "libbde_volume_t *volume" "const wchar_t *filename" "libbde_error_t **error"
 .Pp
 Available when compiled with wide character string support:
 .Ft int
 .Fn libbde_volume_open_wide "libbde_volume_t *volume" "const wchar_t *filename" "int access_flags" "libbde_error_t **error"
-.Ft int
-.Fn libbde_volume_read_startup_key_wide "libbde_volume_t *volume" "const wchar_t *filename" "libbde_error_t **error"
 .Pp
 Available when compiled with libbfio support:
 .Ft int
 .Fn libbde_volume_open_file_io_handle "libbde_volume_t *volume" "libbfio_handle_t *file_io_handle" "int access_flags" "libbde_error_t **error"
 .Ft int
 .Fn libbde_volume_read_startup_key_file_io_handle "libbde_volume_t *volume" "libbfio_handle_t *file_io_handle" "libbde_error_t **error"
 .Pp
```

### Comparing `libbde-20240223/manuals/bdeinfo.1` & `libbde-20240502/manuals/bdeinfo.1`

 * *Files identical despite different names*

### Comparing `libbde-20240223/manuals/Makefile.in` & `libbde-20240502/manuals/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -443,14 +443,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -522,15 +524,16 @@
 	libbde.3
 
 EXTRA_DIST = \
 	bdeinfo.1 \
 	bdemount.1 \
 	libbde.3
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -723,23 +726,25 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic
 
 dvi: dvi-am
 
 dvi-am:
 
 html: html-am
@@ -821,13 +826,10 @@
 	mostlyclean-libtool pdf pdf-am ps ps-am sources-am \
 	sources-local splint-am splint-local tags-am uninstall \
 	uninstall-am uninstall-man uninstall-man1 uninstall-man3
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libbde-20240223/manuals/bdemount.1` & `libbde-20240502/manuals/bdemount.1`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_support.c` & `libbde-20240502/tests/bde_test_support.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_encryption_context.c` & `libbde-20240502/tests/bde_test_encryption_context.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/test_bdeinfo.sh` & `libbde-20240502/tests/test_bdeinfo.sh`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Info tool testing script
 #
-# Version: 20231005
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 PROFILES=("bdeinfo");
 OPTIONS_PER_PROFILE=("");
@@ -28,20 +28,17 @@
 if ! test -x "${TEST_EXECUTABLE}";
 then
 	echo "Missing test executable: ${TEST_EXECUTABLE}";
 
 	exit ${EXIT_FAILURE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libbde-20240223/tests/bde_test_stretch_key.c` & `libbde-20240502/tests/bde_test_stretch_key.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_external_key.c` & `libbde-20240502/tests/bde_test_external_key.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/test_tools.sh` & `libbde-20240502/tests/test_tools.sh`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests tools functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 TOOLS_TESTS="info_handle output signal";
 TOOLS_TESTS_WITH_INPUT="";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_TOOLS_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libbde-20240223/tests/bde_test_libbfio.h` & `libbde-20240502/tests/bde_test_libbfio.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_memory.c` & `libbde-20240502/tests/bde_test_memory.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_metadata_entry.c` & `libbde-20240502/tests/bde_test_metadata_entry.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_libcerror.h` & `libbde-20240502/tests/bde_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/pybde_test_support.py` & `libbde-20240502/tests/pybde_test_support.py`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_key_protector.c` & `libbde-20240502/tests/bde_test_key_protector.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/Makefile.am` & `libbde-20240502/tests/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AUTOMAKE_OPTIONS = subdir-objects
 
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -441,13 +441,12 @@
 	bde_test_unused.h \
 	bde_test_volume_master_key.c
 
 bde_test_volume_master_key_LDADD = \
 	../libbde/libbde.la \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
-
-distclean: clean
-	-rm -f Makefile
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
```

### Comparing `libbde-20240223/tests/bde_test_libclocale.h` & `libbde-20240502/tests/bde_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_volume_header.c` & `libbde-20240502/tests/bde_test_volume_header.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_macros.h` & `libbde-20240502/tests/bde_test_macros.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_sector_data.c` & `libbde-20240502/tests/bde_test_sector_data.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_metadata.c` & `libbde-20240502/tests/bde_test_metadata.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_getopt.h` & `libbde-20240502/tests/bde_test_getopt.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/test_python_module.sh` & `libbde-20240502/tests/test_python_module.sh`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 #!/usr/bin/env bash
 # Tests Python module functions and types.
 #
-# Version: 20240120
+# Version: 20240417
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_NO_TESTS_RAN=5;
 EXIT_IGNORE=77;
 
 TEST_FUNCTIONS="support";
 TEST_FUNCTIONS_WITH_INPUT="volume";
 OPTION_SETS=("password" "recovery_password" "startup_key");
 
 TEST_TOOL_DIRECTORY=".";
 INPUT_GLOB="*";
 
+LIBRARY_NAME="libbde";
+PYTHON_MODULE="pybde";
+
 test_python_function()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pybde_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_SCRIPT}";
 	local RESULT=$?;
 
 	return ${RESULT};
 }
 
 test_python_function_with_input()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pybde_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	if ! test -d "input";
 	then
 		echo "Test input directory not found.";
 
 		return ${EXIT_IGNORE};
 	fi
@@ -46,15 +49,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "pybde");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "${PYTHON_MODULE}");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -121,30 +124,35 @@
 }
 
 if test -n "${SKIP_PYTHON_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
 
 source ${TEST_RUNNER};
 
+PLATFORM=`uname -s | sed 's/-.*$//'`;
+
+if test "${PLATFORM}" = "MINGW64_NT" || test "${PLATFORM}" = "MSYS_NT";
+then
+	cp ../${LIBRARY_NAME}/.libs/*.dll ../${PYTHON_MODULE}/.libs/;
+	cp ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.dll ../${PYTHON_MODULE}/.libs/${PYTHON_MODULE}.pyd;
+fi
+
 RESULT=${EXIT_IGNORE};
 
 for TEST_FUNCTION in ${TEST_FUNCTIONS};
 do
 	test_python_function "${TEST_FUNCTION}";
 	RESULT=$?;
```

### Comparing `libbde-20240223/tests/bde_test_metadata_header.c` & `libbde-20240502/tests/bde_test_metadata_header.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_io_handle.c` & `libbde-20240502/tests/bde_test_io_handle.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_sector_data_vector.c` & `libbde-20240502/tests/bde_test_sector_data_vector.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_functions.h` & `libbde-20240502/tests/bde_test_functions.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_unused.h` & `libbde-20240502/tests/bde_test_unused.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/test_runner.sh` & `libbde-20240502/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_metadata_block_header.c` & `libbde-20240502/tests/bde_test_metadata_block_header.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_tools_signal.c` & `libbde-20240502/tests/bde_test_tools_signal.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_key.c` & `libbde-20240502/tests/bde_test_key.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_functions.c` & `libbde-20240502/tests/bde_test_functions.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_libcnotify.h` & `libbde-20240502/tests/bde_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_notify.c` & `libbde-20240502/tests/bde_test_notify.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_volume_master_key.c` & `libbde-20240502/tests/bde_test_volume_master_key.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_tools_info_handle.c` & `libbde-20240502/tests/bde_test_tools_info_handle.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_volume.c` & `libbde-20240502/tests/bde_test_volume.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_password.c` & `libbde-20240502/tests/bde_test_password.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_memory.h` & `libbde-20240502/tests/bde_test_memory.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_libbde.h` & `libbde-20240502/tests/bde_test_libbde.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/Makefile.in` & `libbde-20240502/tests/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -851,14 +851,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -922,16 +924,16 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 AUTOMAKE_OPTIONS = subdir-objects
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBCSPLIT_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
@@ -1338,16 +1340,18 @@
 	bde_test_unused.h \
 	bde_test_volume_master_key.c
 
 bde_test_volume_master_key_LDADD = \
 	../libbde/libbde.la \
 	@LIBCERROR_LIBADD@
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	Makefile \
+	Makefile.in \
+	notify_stream.log
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .log .o .obj .test .test$(EXEEXT) .trs
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -1879,24 +1883,58 @@
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
 	-rm -f ../bdetools/$(DEPDIR)/$(am__dirstamp)
 	-rm -f ../bdetools/$(am__dirstamp)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ../bdetools/$(DEPDIR)/bdetools_input.Po
+	-rm -f ../bdetools/$(DEPDIR)/bdetools_output.Po
+	-rm -f ../bdetools/$(DEPDIR)/bdetools_signal.Po
+	-rm -f ../bdetools/$(DEPDIR)/byte_size_string.Po
+	-rm -f ../bdetools/$(DEPDIR)/info_handle.Po
+	-rm -f ./$(DEPDIR)/bde_test_aes_ccm_encrypted_key.Po
+	-rm -f ./$(DEPDIR)/bde_test_encryption_context.Po
+	-rm -f ./$(DEPDIR)/bde_test_error.Po
+	-rm -f ./$(DEPDIR)/bde_test_external_key.Po
+	-rm -f ./$(DEPDIR)/bde_test_functions.Po
+	-rm -f ./$(DEPDIR)/bde_test_getopt.Po
+	-rm -f ./$(DEPDIR)/bde_test_io_handle.Po
+	-rm -f ./$(DEPDIR)/bde_test_key.Po
+	-rm -f ./$(DEPDIR)/bde_test_key_protector.Po
+	-rm -f ./$(DEPDIR)/bde_test_memory.Po
+	-rm -f ./$(DEPDIR)/bde_test_metadata.Po
+	-rm -f ./$(DEPDIR)/bde_test_metadata_block_header.Po
+	-rm -f ./$(DEPDIR)/bde_test_metadata_entry.Po
+	-rm -f ./$(DEPDIR)/bde_test_metadata_header.Po
+	-rm -f ./$(DEPDIR)/bde_test_notify.Po
+	-rm -f ./$(DEPDIR)/bde_test_password.Po
+	-rm -f ./$(DEPDIR)/bde_test_password_keep.Po
+	-rm -f ./$(DEPDIR)/bde_test_sector_data.Po
+	-rm -f ./$(DEPDIR)/bde_test_sector_data_vector.Po
+	-rm -f ./$(DEPDIR)/bde_test_stretch_key.Po
+	-rm -f ./$(DEPDIR)/bde_test_support.Po
+	-rm -f ./$(DEPDIR)/bde_test_tools_info_handle.Po
+	-rm -f ./$(DEPDIR)/bde_test_tools_output.Po
+	-rm -f ./$(DEPDIR)/bde_test_tools_signal.Po
+	-rm -f ./$(DEPDIR)/bde_test_volume.Po
+	-rm -f ./$(DEPDIR)/bde_test_volume_header.Po
+	-rm -f ./$(DEPDIR)/bde_test_volume_master_key.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -2011,13 +2049,10 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	recheck sources-am sources-local splint-am splint-local tags \
 	tags-am uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libbde-20240223/tests/bde_test_tools_output.c` & `libbde-20240502/tests/bde_test_tools_output.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_aes_ccm_encrypted_key.c` & `libbde-20240502/tests/bde_test_aes_ccm_encrypted_key.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_libuna.h` & `libbde-20240502/tests/bde_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/pybde_test_volume.py` & `libbde-20240502/tests/pybde_test_volume.py`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_error.c` & `libbde-20240502/tests/bde_test_error.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_getopt.c` & `libbde-20240502/tests/bde_test_getopt.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/bde_test_password_keep.c` & `libbde-20240502/tests/bde_test_password_keep.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/tests/test_library.sh` & `libbde-20240502/tests/test_library.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env bash
 # Tests library functions and types.
 #
-# Version: 20231007
+# Version: 20240413
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
 EXIT_IGNORE=77;
 
 LIBRARY_TESTS="aes_ccm_encrypted_key encryption_context error external_key io_handle key key_protector metadata metadata_block_header metadata_entry metadata_header notify password password_keep sector_data sector_data_vector stretch_key volume_header volume_master_key";
 LIBRARY_TESTS_WITH_INPUT="support volume";
@@ -137,20 +137,17 @@
 }
 
 if test -n "${SKIP_LIBRARY_TESTS}";
 then
 	exit ${EXIT_IGNORE};
 fi
 
-TEST_RUNNER="tests/test_runner.sh";
+TEST_DIRECTORY=`dirname $0`;
 
-if ! test -f "${TEST_RUNNER}";
-then
-	TEST_RUNNER="./test_runner.sh";
-fi
+TEST_RUNNER="${TEST_DIRECTORY}/test_runner.sh";
 
 if ! test -f "${TEST_RUNNER}";
 then
 	echo "Missing test runner: ${TEST_RUNNER}";
 
 	exit ${EXIT_FAILURE};
 fi
```

### Comparing `libbde-20240223/ossfuzz/volume_fuzzer.cc` & `libbde-20240502/ossfuzz/volume_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libbde-20240223/ossfuzz/ossfuzz_libbde.h` & `libbde-20240502/ossfuzz/ossfuzz_libbde.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/ossfuzz/Makefile.am` & `libbde-20240502/ossfuzz/Makefile.am`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LIB_FUZZING_ENGINE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCLOCALE_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBCFILE_CPPFLAGS@ \
 	@LIBCPATH_CPPFLAGS@ \
@@ -29,17 +29,15 @@
 	../libbde/libbde.la \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCERROR_LIBADD@ \
 	@LIBINTL@
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on volume_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(volume_fuzzer_SOURCES)
```

### Comparing `libbde-20240223/ossfuzz/ossfuzz_libbfio.h` & `libbde-20240502/ossfuzz/ossfuzz_libbfio.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/ossfuzz/Makefile.in` & `libbde-20240502/ossfuzz/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -483,14 +483,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -553,16 +555,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@AM_CPPFLAGS = \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LIB_FUZZING_ENGINE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCFILE_CPPFLAGS@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCPATH_CPPFLAGS@ \
@@ -582,15 +584,16 @@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libbde/libbde.la \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCNOTIFY_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCLOCALE_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCERROR_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBINTL@
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .cc .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -832,23 +835,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-binPROGRAMS clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/volume_fuzzer.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -932,17 +938,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on volume_fuzzer ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(volume_fuzzer_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libbde-20240223/ltmain.sh` & `libbde-20240502/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/libhmac_sha1_context.c` & `libbde-20240502/libhmac/libhmac_sha1_context.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/libhmac_sha224.h` & `libbde-20240502/libhmac/libhmac_sha224.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/libhmac_sha512_context.c` & `libbde-20240502/libhmac/libhmac_sha512_context.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/libhmac_extern.h` & `libbde-20240502/libhmac/libhmac_extern.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/libhmac_md5.c` & `libbde-20240502/libhmac/libhmac_md5.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/libhmac_md5.h` & `libbde-20240502/libhmac/libhmac_md5.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/libhmac_error.h` & `libbde-20240502/libhmac/libhmac_error.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/libhmac_types.h` & `libbde-20240502/libhmac/libhmac_types.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/libhmac_byte_stream.h` & `libbde-20240502/libhmac/libhmac_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/libhmac_sha512.c` & `libbde-20240502/libhmac/libhmac_sha512.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/libhmac_sha256_context.c` & `libbde-20240502/libhmac/libhmac_sha256_context.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/libhmac_sha224.c` & `libbde-20240502/libhmac/libhmac_sha224.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/libhmac_definitions.h` & `libbde-20240502/libhmac/libhmac_definitions.h`

 * *Files 8% similar despite different names*

```diff
@@ -30,19 +30,19 @@
 #if !defined( HAVE_LOCAL_LIBHMAC )
 #include <libhmac/definitions.h>
 
 /* The definitions in <libhmac/definitions.h> are copied here
  * for local use of libhmac
  */
 #else
-#define LIBHMAC_VERSION			20240129
+#define LIBHMAC_VERSION			20240417
 
 /* The libhmac version string
  */
-#define LIBHMAC_VERSION_STRING		"20240129"
+#define LIBHMAC_VERSION_STRING		"20240417"
 
 /* The digest hash sizes
  */
 #define LIBHMAC_MD5_HASH_SIZE		16
 #define LIBHMAC_SHA1_HASH_SIZE		20
 #define LIBHMAC_SHA224_HASH_SIZE	28
 #define LIBHMAC_SHA256_HASH_SIZE	32
```

### Comparing `libbde-20240223/libhmac/libhmac_unused.h` & `libbde-20240502/libhmac/libhmac_unused.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/libhmac_sha1.h` & `libbde-20240502/libhmac/libhmac_sha1.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/libhmac_sha256_context.h` & `libbde-20240502/libhmac/libhmac_sha256_context.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/Makefile.am` & `libbde-20240502/libhmac/Makefile.am`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBHMAC
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCRYPTO_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libhmac.la
 
 libhmac_la_SOURCES = \
@@ -25,19 +25,17 @@
 	libhmac_sha512.c libhmac_sha512.h \
 	libhmac_sha512_context.c libhmac_sha512_context.h \
 	libhmac_support.c libhmac_support.h \
 	libhmac_types.h \
 	libhmac_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libhmac ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libhmac_la_SOURCES)
```

### Comparing `libbde-20240223/libhmac/libhmac_sha224_context.c` & `libbde-20240502/libhmac/libhmac_sha224_context.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/libhmac_md5_context.h` & `libbde-20240502/libhmac/libhmac_md5_context.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/libhmac_sha256.c` & `libbde-20240502/libhmac/libhmac_sha256.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/libhmac_sha1_context.h` & `libbde-20240502/libhmac/libhmac_sha1_context.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/libhmac_libcerror.h` & `libbde-20240502/libhmac/libhmac_libcerror.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/libhmac_error.c` & `libbde-20240502/libhmac/libhmac_error.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/libhmac_support.h` & `libbde-20240502/libhmac/libhmac_support.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/Makefile.in` & `libbde-20240502/libhmac/Makefile.in`

 * *Files 7% similar despite different names*

```diff
@@ -493,14 +493,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -563,16 +565,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBHMAC_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBHMAC_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBHMAC_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBHMAC_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBHMAC_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBHMAC_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBHMAC_TRUE@	@LIBCRYPTO_CPPFLAGS@ \
 @HAVE_LOCAL_LIBHMAC_TRUE@	@PTHREAD_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBHMAC_TRUE@noinst_LTLIBRARIES = libhmac.la
 @HAVE_LOCAL_LIBHMAC_TRUE@libhmac_la_SOURCES = \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_byte_stream.h \
@@ -590,15 +592,16 @@
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_sha256_context.c libhmac_sha256_context.h \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_sha512.c libhmac_sha512.h \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_sha512_context.c libhmac_sha512_context.h \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_support.c libhmac_support.h \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_types.h \
 @HAVE_LOCAL_LIBHMAC_TRUE@	libhmac_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -809,24 +812,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libhmac_error.Plo
+	-rm -f ./$(DEPDIR)/libhmac_md5.Plo
+	-rm -f ./$(DEPDIR)/libhmac_md5_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha1.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha1_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha224.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha224_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha256.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha256_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha512.Plo
+	-rm -f ./$(DEPDIR)/libhmac_sha512_context.Plo
+	-rm -f ./$(DEPDIR)/libhmac_support.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -921,17 +938,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libhmac ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libhmac_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libbde-20240223/libhmac/libhmac_sha256.h` & `libbde-20240502/libhmac/libhmac_sha256.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/libhmac_sha224_context.h` & `libbde-20240502/libhmac/libhmac_sha224_context.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/libhmac_sha512_context.h` & `libbde-20240502/libhmac/libhmac_sha512_context.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/libhmac_sha512.h` & `libbde-20240502/libhmac/libhmac_sha512.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/libhmac_support.c` & `libbde-20240502/libhmac/libhmac_support.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/libhmac_sha1.c` & `libbde-20240502/libhmac/libhmac_sha1.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libhmac/libhmac_md5_context.c` & `libbde-20240502/libhmac/libhmac_md5_context.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcsplit/libcsplit_narrow_string.c` & `libbde-20240502/libcsplit/libcsplit_narrow_string.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcsplit/libcsplit_definitions.h` & `libbde-20240502/libcsplit/libcsplit_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 #include <libcsplit/definitions.h>
 
 /* The definitions in <libcsplit/definitions.h> are copied here
  * for local use of libcsplit
  */
 #else
 
-#define LIBCSPLIT_VERSION			20240110
+#define LIBCSPLIT_VERSION			20240414
 
 /* The libcsplit version string
  */
-#define LIBCSPLIT_VERSION_STRING		"20240110"
+#define LIBCSPLIT_VERSION_STRING		"20240414"
 
 #endif /* !defined( HAVE_LOCAL_LIBCSPLIT ) */
 
 #endif
```

### Comparing `libbde-20240223/libcsplit/libcsplit_types.h` & `libbde-20240502/libcsplit/libcsplit_types.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcsplit/libcsplit_wide_split_string.c` & `libbde-20240502/libcsplit/libcsplit_wide_split_string.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcsplit/libcsplit_support.h` & `libbde-20240502/libcsplit/libcsplit_support.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcsplit/Makefile.am` & `libbde-20240502/libcsplit/Makefile.am`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCSPLIT
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcsplit.la
 
 libcsplit_la_SOURCES = \
 	libcsplit_definitions.h \
 	libcsplit_error.c libcsplit_error.h \
@@ -16,19 +16,17 @@
 	libcsplit_support.c libcsplit_support.h \
 	libcsplit_types.h \
 	libcsplit_unused.h \
 	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 	libcsplit_wide_string.c libcsplit_wide_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
```

### Comparing `libbde-20240223/libcsplit/libcsplit_libcerror.h` & `libbde-20240502/libcsplit/libcsplit_libcerror.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcsplit/libcsplit_wide_string.c` & `libbde-20240502/libcsplit/libcsplit_wide_string.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcsplit/libcsplit_unused.h` & `libbde-20240502/libcsplit/libcsplit_unused.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcsplit/libcsplit_wide_split_string.h` & `libbde-20240502/libcsplit/libcsplit_wide_split_string.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcsplit/libcsplit_error.c` & `libbde-20240502/libcsplit/libcsplit_error.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcsplit/libcsplit_narrow_split_string.c` & `libbde-20240502/libcsplit/libcsplit_narrow_split_string.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcsplit/libcsplit_extern.h` & `libbde-20240502/libcsplit/libcsplit_extern.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcsplit/libcsplit_error.h` & `libbde-20240502/libcsplit/libcsplit_error.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcsplit/libcsplit_support.c` & `libbde-20240502/libcsplit/libcsplit_support.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcsplit/libcsplit_wide_string.h` & `libbde-20240502/libcsplit/libcsplit_wide_string.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcsplit/Makefile.in` & `libbde-20240502/libcsplit/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -480,14 +480,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -550,16 +552,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCSPLIT_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCSPLIT_TRUE@noinst_LTLIBRARIES = libcsplit.la
 @HAVE_LOCAL_LIBCSPLIT_TRUE@libcsplit_la_SOURCES = \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_definitions.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_error.c libcsplit_error.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_extern.h \
@@ -568,15 +570,16 @@
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_libcerror.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_support.c libcsplit_support.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_types.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_unused.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_split_string.c libcsplit_wide_split_string.h \
 @HAVE_LOCAL_LIBCSPLIT_TRUE@	libcsplit_wide_string.c libcsplit_wide_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -781,24 +784,32 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcsplit_error.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_narrow_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_support.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_split_string.Plo
+	-rm -f ./$(DEPDIR)/libcsplit_wide_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -887,17 +898,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcsplit ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcsplit_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libbde-20240223/libcsplit/libcsplit_narrow_split_string.h` & `libbde-20240502/libcsplit/libcsplit_narrow_split_string.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcsplit/libcsplit_narrow_string.h` & `libbde-20240502/libcsplit/libcsplit_narrow_string.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/po/remove-potcdate.sin` & `libbde-20240502/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libbde-20240223/po/Makefile.in.in` & `libbde-20240502/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libbde-20240223/po/en@quot.header` & `libbde-20240502/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libbde-20240223/po/en@boldquot.header` & `libbde-20240502/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libbde-20240223/po/insert-header.sin` & `libbde-20240502/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libbde-20240223/po/Makevars` & `libbde-20240502/po/Makevars`

 * *Files identical despite different names*

### Comparing `libbde-20240223/po/Makevars.in` & `libbde-20240502/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libbde-20240223/po/Rules-quot` & `libbde-20240502/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_windows_1251.c` & `libbde-20240502/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_utf16_string.c` & `libbde-20240502/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_base16_stream.c` & `libbde-20240502/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_utf8_stream.h` & `libbde-20240502/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_iso_8859_2.h` & `libbde-20240502/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_windows_932.c` & `libbde-20240502/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_dingbats.h` & `libbde-20240502/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_utf8_string.c` & `libbde-20240502/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_base64_stream.c` & `libbde-20240502/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_error.h` & `libbde-20240502/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_turkish.h` & `libbde-20240502/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_unicode_character.c` & `libbde-20240502/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_gaelic.c` & `libbde-20240502/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_arabic.h` & `libbde-20240502/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_thai.c` & `libbde-20240502/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_windows_874.h` & `libbde-20240502/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_iso_8859_15.h` & `libbde-20240502/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_utf8_string.h` & `libbde-20240502/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_iso_8859_16.c` & `libbde-20240502/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_windows_1255.c` & `libbde-20240502/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_utf7_stream.c` & `libbde-20240502/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_byte_stream.h` & `libbde-20240502/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_koi8_u.c` & `libbde-20240502/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_unused.h` & `libbde-20240502/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_iso_8859_6.c` & `libbde-20240502/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_iso_8859_14.c` & `libbde-20240502/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_base64_stream.h` & `libbde-20240502/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_error.c` & `libbde-20240502/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_centraleurroman.h` & `libbde-20240502/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_romanian.c` & `libbde-20240502/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_iso_8859_6.h` & `libbde-20240502/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_iso_8859_9.c` & `libbde-20240502/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_russian.h` & `libbde-20240502/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_dingbats.c` & `libbde-20240502/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_iso_8859_15.c` & `libbde-20240502/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_windows_936.c` & `libbde-20240502/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_croatian.h` & `libbde-20240502/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_scsu.h` & `libbde-20240502/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/Makefile.am` & `libbde-20240502/libuna/Makefile.am`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBUNA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libuna.la
 
 libuna_la_SOURCES = \
 	libuna_base16_stream.c libuna_base16_stream.h \
 	libuna_base32_stream.c libuna_base32_stream.h \
@@ -73,19 +73,17 @@
 	libuna_utf32_stream.c libuna_utf32_stream.h \
 	libuna_utf32_string.c libuna_utf32_string.h \
 	libuna_utf7_stream.c libuna_utf7_stream.h \
 	libuna_utf8_stream.c libuna_utf8_stream.h \
 	libuna_utf8_string.c libuna_utf8_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
```

### Comparing `libbde-20240223/libuna/libuna_utf32_stream.c` & `libbde-20240502/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_windows_936.h` & `libbde-20240502/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_iso_8859_10.c` & `libbde-20240502/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_roman.c` & `libbde-20240502/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_utf7_stream.h` & `libbde-20240502/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_iso_8859_3.h` & `libbde-20240502/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_thai.h` & `libbde-20240502/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_farsi.h` & `libbde-20240502/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_ukrainian.c` & `libbde-20240502/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_inuit.c` & `libbde-20240502/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_windows_932.h` & `libbde-20240502/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_windows_874.c` & `libbde-20240502/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_iso_8859_5.c` & `libbde-20240502/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_iso_8859_10.h` & `libbde-20240502/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_definitions.h` & `libbde-20240502/libuna/libuna_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 
 /* The definitions in <libuna/definitions.h> are copied here
  * for local use of libuna
  */
 #else
 #include <byte_stream.h>
 
-#define LIBUNA_VERSION						20240130
+#define LIBUNA_VERSION						20240414
 
 /* The libuna version string
  */
-#define LIBUNA_VERSION_STRING					"20240130"
+#define LIBUNA_VERSION_STRING					"20240414"
 
 /* The endian definitions
  */
 #define	LIBUNA_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define	LIBUNA_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The codepage definitions
```

### Comparing `libbde-20240223/libuna/libuna_url_stream.h` & `libbde-20240502/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_icelandic.h` & `libbde-20240502/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_koi8_u.h` & `libbde-20240502/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_utf16_stream.c` & `libbde-20240502/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_windows_1253.c` & `libbde-20240502/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_iso_8859_4.h` & `libbde-20240502/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_greek.c` & `libbde-20240502/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_libcerror.h` & `libbde-20240502/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_centraleurroman.c` & `libbde-20240502/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_windows_1254.c` & `libbde-20240502/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_iso_8859_13.h` & `libbde-20240502/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_iso_8859_7.h` & `libbde-20240502/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_windows_1255.h` & `libbde-20240502/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_unicode_character.h` & `libbde-20240502/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_iso_8859_8.h` & `libbde-20240502/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_iso_8859_13.c` & `libbde-20240502/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_windows_949.h` & `libbde-20240502/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_cyrillic.c` & `libbde-20240502/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_celtic.c` & `libbde-20240502/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_support.h` & `libbde-20240502/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_iso_8859_4.c` & `libbde-20240502/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_windows_949.c` & `libbde-20240502/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_utf16_stream.h` & `libbde-20240502/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_symbol.c` & `libbde-20240502/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_roman.h` & `libbde-20240502/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_windows_1257.c` & `libbde-20240502/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_windows_1254.h` & `libbde-20240502/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_windows_950.c` & `libbde-20240502/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_extern.h` & `libbde-20240502/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_windows_1256.c` & `libbde-20240502/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_types.h` & `libbde-20240502/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_base32_stream.h` & `libbde-20240502/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_windows_1253.h` & `libbde-20240502/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_iso_8859_16.h` & `libbde-20240502/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_utf8_stream.c` & `libbde-20240502/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_windows_1250.h` & `libbde-20240502/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_iso_8859_2.c` & `libbde-20240502/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_support.c` & `libbde-20240502/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_koi8_r.c` & `libbde-20240502/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_iso_8859_5.h` & `libbde-20240502/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_utf16_string.h` & `libbde-20240502/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_utf32_string.c` & `libbde-20240502/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_icelandic.c` & `libbde-20240502/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_windows_1256.h` & `libbde-20240502/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_utf32_string.h` & `libbde-20240502/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_romanian.h` & `libbde-20240502/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_iso_8859_8.c` & `libbde-20240502/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_koi8_r.h` & `libbde-20240502/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_cyrillic.h` & `libbde-20240502/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_arabic.c` & `libbde-20240502/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_croatian.c` & `libbde-20240502/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_iso_8859_9.h` & `libbde-20240502/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_greek.h` & `libbde-20240502/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_windows_1258.h` & `libbde-20240502/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_iso_8859_7.c` & `libbde-20240502/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/Makefile.in` & `libbde-20240502/libuna/Makefile.in`

 * *Files 8% similar despite different names*

```diff
@@ -648,14 +648,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -718,16 +720,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBUNA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBUNA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBUNA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBUNA_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBUNA_TRUE@noinst_LTLIBRARIES = libuna.la
 @HAVE_LOCAL_LIBUNA_TRUE@libuna_la_SOURCES = \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base16_stream.c libuna_base16_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base32_stream.c libuna_base32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_base64_stream.c libuna_base64_stream.h \
@@ -793,15 +795,16 @@
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf16_string.c libuna_utf16_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_stream.c libuna_utf32_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf32_string.c libuna_utf32_string.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf7_stream.c libuna_utf7_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_stream.c libuna_utf8_stream.h \
 @HAVE_LOCAL_LIBUNA_TRUE@	libuna_utf8_string.c libuna_utf8_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -1063,24 +1066,89 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libuna_base16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_base64_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_byte_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_10.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_13.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_14.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_15.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_16.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_2.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_3.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_4.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_5.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_6.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_7.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_8.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_iso_8859_9.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_r.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_koi8_u.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_arabic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_celtic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_centraleurroman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_croatian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_cyrillic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_dingbats.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_farsi.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_gaelic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_greek.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_icelandic.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_inuit.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_roman.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_romanian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_russian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_symbol.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_thai.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_turkish.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_mac_ukrainian.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1250.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1251.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1252.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1253.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1254.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1255.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1256.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1257.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_1258.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_874.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_932.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_936.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_949.Plo
+	-rm -f ./$(DEPDIR)/libuna_codepage_windows_950.Plo
+	-rm -f ./$(DEPDIR)/libuna_error.Plo
+	-rm -f ./$(DEPDIR)/libuna_scsu.Plo
+	-rm -f ./$(DEPDIR)/libuna_support.Plo
+	-rm -f ./$(DEPDIR)/libuna_unicode_character.Plo
+	-rm -f ./$(DEPDIR)/libuna_url_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf32_string.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf7_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_stream.Plo
+	-rm -f ./$(DEPDIR)/libuna_utf8_string.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1226,17 +1294,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libbde-20240223/libuna/libuna_codepage_iso_8859_3.c` & `libbde-20240502/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_windows_1250.c` & `libbde-20240502/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_scsu.c` & `libbde-20240502/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_windows_1252.c` & `libbde-20240502/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_turkish.c` & `libbde-20240502/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_ukrainian.h` & `libbde-20240502/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_russian.c` & `libbde-20240502/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_windows_1258.c` & `libbde-20240502/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_celtic.h` & `libbde-20240502/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_byte_stream.c` & `libbde-20240502/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_gaelic.h` & `libbde-20240502/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_utf32_stream.h` & `libbde-20240502/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_symbol.h` & `libbde-20240502/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_windows_1257.h` & `libbde-20240502/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_inuit.h` & `libbde-20240502/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_mac_farsi.c` & `libbde-20240502/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_windows_950.h` & `libbde-20240502/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_url_stream.c` & `libbde-20240502/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_windows_1251.h` & `libbde-20240502/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_windows_1252.h` & `libbde-20240502/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_codepage_iso_8859_14.h` & `libbde-20240502/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_base16_stream.h` & `libbde-20240502/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libuna/libuna_base32_stream.c` & `libbde-20240502/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/Makefile.in` & `libbde-20240502/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -530,14 +530,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -665,16 +667,23 @@
 EXTRA_DIST = \
 	$(DPKG_FILES) \
 	$(GETTEXT_FILES) \
 	$(PKGCONFIG_FILES) \
 	$(SETUP_PY_FILES) \
 	$(SPEC_FILES)
 
-MAINTAINERCLEANFILES = \
-	Makefile.in
+DISTCLEANFILES = \
+	config.status \
+	config.cache \
+	config.log \
+	libbde.pc \
+	libbde.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libbde.pc
 
 all: all-recursive
 
@@ -1091,23 +1100,26 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-recursive
 
 clean-am: clean-generic clean-libtool mostlyclean-am
 
+distclean: distclean-recursive
+	-rm -f $(am__CONFIG_DISTCLEAN_FILES)
+	-rm -f Makefile
 distclean-am: clean-am distclean-generic distclean-libtool \
 	distclean-tags
 
 dvi: dvi-recursive
 
 dvi-am:
 
@@ -1220,22 +1232,10 @@
 	(cd $(srcdir)/libfguid && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfvalue && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libhmac && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libcaes && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libbde && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libbde.pc
-	-rm -f libbde.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libbde-20240223/libfvalue/libfvalue_filetime.c` & `libbde-20240502/libfvalue/libfvalue_filetime.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_utf16_string.c` & `libbde-20240502/libfvalue/libfvalue_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_libfwnt.h` & `libbde-20240502/libfvalue/libfvalue_libfwnt.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_value.c` & `libbde-20240502/libfvalue/libfvalue_value.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_value.h` & `libbde-20240502/libfvalue/libfvalue_value.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_definitions.h` & `libbde-20240502/libfvalue/libfvalue_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfvalue/definitions.h> are copied here
  * for local use of libfvalue
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFVALUE_VERSION						20240124
+#define LIBFVALUE_VERSION						20240415
 
 /* The libfvalue version string
  */
-#define LIBFVALUE_VERSION_STRING					"20240124"
+#define LIBFVALUE_VERSION_STRING					"20240415"
 
 /* The endian definitions
  */
 #define LIBFVALUE_ENDIAN_BIG						_BYTE_STREAM_ENDIAN_BIG
 #define LIBFVALUE_ENDIAN_LITTLE						_BYTE_STREAM_ENDIAN_LITTLE
 #define LIBFVALUE_ENDIAN_NATIVE						(uint8_t) 'n'
```

### Comparing `libbde-20240223/libfvalue/libfvalue_codepage.h` & `libbde-20240502/libfvalue/libfvalue_codepage.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_split_utf16_string.c` & `libbde-20240502/libfvalue/libfvalue_split_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_error.c` & `libbde-20240502/libfvalue/libfvalue_error.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_utf8_string.c` & `libbde-20240502/libfvalue/libfvalue_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_unused.h` & `libbde-20240502/libfvalue/libfvalue_unused.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_split_utf16_string.h` & `libbde-20240502/libfvalue/libfvalue_split_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_filetime.h` & `libbde-20240502/libfvalue/libfvalue_filetime.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_support.c` & `libbde-20240502/libfvalue/libfvalue_support.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_extern.h` & `libbde-20240502/libfvalue/libfvalue_extern.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/Makefile.am` & `libbde-20240502/libfvalue/Makefile.am`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFVALUE
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBFDATETIME_CPPFLAGS@ \
 	@LIBFGUID_CPPFLAGS@ \
@@ -40,19 +40,17 @@
 	libfvalue_value_type.c libfvalue_value_type.h \
 	libfvalue_support.c libfvalue_support.h \
 	libfvalue_unused.h \
 	libfvalue_utf8_string.c libfvalue_utf8_string.h \
 	libfvalue_utf16_string.c libfvalue_utf16_string.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfvalue ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfvalue_la_SOURCES)
```

### Comparing `libbde-20240223/libfvalue/libfvalue_value_type.h` & `libbde-20240502/libfvalue/libfvalue_value_type.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_libcerror.h` & `libbde-20240502/libfvalue/libfvalue_libcerror.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_split_utf8_string.c` & `libbde-20240502/libfvalue/libfvalue_split_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_data_handle.h` & `libbde-20240502/libfvalue/libfvalue_data_handle.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_libcnotify.h` & `libbde-20240502/libfvalue/libfvalue_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_data_handle.c` & `libbde-20240502/libfvalue/libfvalue_data_handle.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_integer.c` & `libbde-20240502/libfvalue/libfvalue_integer.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_value_type.c` & `libbde-20240502/libfvalue/libfvalue_value_type.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_integer.h` & `libbde-20240502/libfvalue/libfvalue_integer.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_binary_data.h` & `libbde-20240502/libfvalue/libfvalue_binary_data.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_value_entry.h` & `libbde-20240502/libfvalue/libfvalue_value_entry.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_utf16_string.h` & `libbde-20240502/libfvalue/libfvalue_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_error.h` & `libbde-20240502/libfvalue/libfvalue_error.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_table.h` & `libbde-20240502/libfvalue/libfvalue_table.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_libfguid.h` & `libbde-20240502/libfvalue/libfvalue_libfguid.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_split_utf8_string.h` & `libbde-20240502/libfvalue/libfvalue_split_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_floating_point.h` & `libbde-20240502/libfvalue/libfvalue_floating_point.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_libfdatetime.h` & `libbde-20240502/libfvalue/libfvalue_libfdatetime.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_string.h` & `libbde-20240502/libfvalue/libfvalue_string.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_binary_data.c` & `libbde-20240502/libfvalue/libfvalue_binary_data.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_value_entry.c` & `libbde-20240502/libfvalue/libfvalue_value_entry.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_libcdata.h` & `libbde-20240502/libfvalue/libfvalue_libcdata.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_support.h` & `libbde-20240502/libfvalue/libfvalue_support.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_table.c` & `libbde-20240502/libfvalue/libfvalue_table.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/Makefile.in` & `libbde-20240502/libfvalue/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -511,14 +511,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -581,16 +583,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFVALUE_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFVALUE_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFVALUE_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFVALUE_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFVALUE_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBFDATETIME_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBFGUID_CPPFLAGS@ \
@@ -623,15 +625,16 @@
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_value_entry.c libfvalue_value_entry.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_value_type.c libfvalue_value_type.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_support.c libfvalue_support.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_unused.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_utf8_string.c libfvalue_utf8_string.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_utf16_string.c libfvalue_utf16_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -846,24 +849,42 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfvalue_binary_data.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_data_handle.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_error.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_filetime.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_floating_point.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_integer.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_split_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_split_utf8_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_support.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_table.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_utf16_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_utf8_string.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value_entry.Plo
+	-rm -f ./$(DEPDIR)/libfvalue_value_type.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -962,17 +983,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfvalue ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfvalue_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libbde-20240223/libfvalue/libfvalue_utf8_string.h` & `libbde-20240502/libfvalue/libfvalue_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_floating_point.c` & `libbde-20240502/libfvalue/libfvalue_floating_point.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_types.h` & `libbde-20240502/libfvalue/libfvalue_types.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_string.c` & `libbde-20240502/libfvalue/libfvalue_string.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfvalue/libfvalue_libuna.h` & `libbde-20240502/libfvalue/libfvalue_libuna.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcnotify/libcnotify_definitions.h` & `libbde-20240502/libcnotify/libcnotify_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcnotify/definitions.h>
 
 /* The definitions in <libcnotify/definitions.h> are copied here
  * for local use of libcnotify
  */
 #else
 
-#define LIBCNOTIFY_VERSION				20240108
+#define LIBCNOTIFY_VERSION				20240414
 
 /* The libcnotify version string
  */
-#define LIBCNOTIFY_VERSION_STRING			"20240108"
+#define LIBCNOTIFY_VERSION_STRING			"20240414"
 
 /* The print data flags
  */
 enum LIBCNOTIFY_NOTIFY_PRINT_DATA_FLAGS
 {
 	LIBCNOTIFY_PRINT_DATA_FLAG_GROUP_DATA		= 0x01,
 };
```

### Comparing `libbde-20240223/libcnotify/libcnotify_extern.h` & `libbde-20240502/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcnotify/libcnotify_support.c` & `libbde-20240502/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcnotify/libcnotify_stream.h` & `libbde-20240502/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcnotify/Makefile.am` & `libbde-20240502/libcnotify/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBCNOTIFY
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libcnotify.la
 
 libcnotify_la_SOURCES = \
 	libcnotify_definitions.h \
 	libcnotify_extern.h \
@@ -13,19 +13,17 @@
 	libcnotify_print.c libcnotify_print.h \
 	libcnotify_stream.c libcnotify_stream.h \
 	libcnotify_support.c libcnotify_support.h \
 	libcnotify_unused.h \
 	libcnotify_verbose.c libcnotify_verbose.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
```

### Comparing `libbde-20240223/libcnotify/libcnotify_unused.h` & `libbde-20240502/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcnotify/libcnotify_verbose.h` & `libbde-20240502/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcnotify/libcnotify_print.h` & `libbde-20240502/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcnotify/libcnotify_stream.c` & `libbde-20240502/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcnotify/libcnotify_support.h` & `libbde-20240502/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcnotify/libcnotify_verbose.c` & `libbde-20240502/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcnotify/Makefile.in` & `libbde-20240502/libcnotify/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -472,14 +472,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -542,30 +544,31 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCNOTIFY_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@noinst_LTLIBRARIES = libcnotify.la
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@libcnotify_la_SOURCES = \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_definitions.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_extern.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_libcerror.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_print.c libcnotify_print.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_stream.c libcnotify_stream.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_support.c libcnotify_support.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_unused.h \
 @HAVE_LOCAL_LIBCNOTIFY_TRUE@	libcnotify_verbose.c libcnotify_verbose.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -768,24 +771,30 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcnotify_print.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_stream.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_support.Plo
+	-rm -f ./$(DEPDIR)/libcnotify_verbose.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -872,17 +881,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcnotify ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcnotify_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libbde-20240223/libcnotify/libcnotify_libcerror.h` & `libbde-20240502/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcnotify/libcnotify_print.c` & `libbde-20240502/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcerror/libcerror_system.c` & `libbde-20240502/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcerror/libcerror_error.c` & `libbde-20240502/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcerror/libcerror_extern.h` & `libbde-20240502/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcerror/Makefile.am` & `libbde-20240502/libcerror/Makefile.am`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 if HAVE_LOCAL_LIBCERROR
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common 
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common 
 
 noinst_LTLIBRARIES = libcerror.la
 
 libcerror_la_SOURCES = \
 	libcerror_definitions.h \
 	libcerror_extern.h \
 	libcerror_error.c libcerror_error.h \
 	libcerror_support.c libcerror_support.h \
 	libcerror_system.c libcerror_system.h \
 	libcerror_types.h \
 	libcerror_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
```

### Comparing `libbde-20240223/libcerror/libcerror_types.h` & `libbde-20240502/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcerror/libcerror_support.h` & `libbde-20240502/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcerror/libcerror_error.h` & `libbde-20240502/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcerror/libcerror_system.h` & `libbde-20240502/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcerror/libcerror_definitions.h` & `libbde-20240502/libcerror/libcerror_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,19 @@
 #include <libcerror/definitions.h>
 
 /* The definitions in <libcerror/definitions.h> are copied here
  * for local use of libcerror
  */
 #else
 
-#define LIBCERROR_VERSION				20240101
+#define LIBCERROR_VERSION				20240413
 
 /* The libcerror version string
  */
-#define LIBCERROR_VERSION_STRING			"20240101"
+#define LIBCERROR_VERSION_STRING			"20240413"
 
 /* The error domains
  */
 enum LIBCERROR_ERROR_DOMAINS
 {
 	LIBCERROR_ERROR_DOMAIN_ARGUMENTS		= (int) 'a',
 	LIBCERROR_ERROR_DOMAIN_CONVERSION		= (int) 'c',
```

### Comparing `libbde-20240223/libcerror/libcerror_support.c` & `libbde-20240502/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcerror/libcerror_unused.h` & `libbde-20240502/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libcerror/Makefile.in` & `libbde-20240502/libcerror/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -469,14 +469,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -539,28 +541,29 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBCERROR_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBCERROR_TRUE@	-I$(top_srcdir)/common 
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBCERROR_TRUE@	-I../common -I$(top_srcdir)/common 
 
 @HAVE_LOCAL_LIBCERROR_TRUE@noinst_LTLIBRARIES = libcerror.la
 @HAVE_LOCAL_LIBCERROR_TRUE@libcerror_la_SOURCES = \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_definitions.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_extern.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_error.c libcerror_error.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_support.c libcerror_support.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_system.c libcerror_system.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_types.h \
 @HAVE_LOCAL_LIBCERROR_TRUE@	libcerror_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -762,24 +765,29 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libcerror_error.Plo
+	-rm -f ./$(DEPDIR)/libcerror_support.Plo
+	-rm -f ./$(DEPDIR)/libcerror_system.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -865,17 +873,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libcerror ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libcerror_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libbde-20240223/libfdatetime/libfdatetime_floatingtime.h` & `libbde-20240502/libfdatetime/libfdatetime_floatingtime.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfdatetime/libfdatetime_nsf_timedate.c` & `libbde-20240502/libfdatetime/libfdatetime_nsf_timedate.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfdatetime/libfdatetime_error.h` & `libbde-20240502/libfdatetime/libfdatetime_error.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfdatetime/libfdatetime_floatingtime.c` & `libbde-20240502/libfdatetime/libfdatetime_floatingtime.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfdatetime/libfdatetime_support.h` & `libbde-20240502/libfdatetime/libfdatetime_support.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfdatetime/libfdatetime_hfs_time.h` & `libbde-20240502/libfdatetime/libfdatetime_hfs_time.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfdatetime/libfdatetime_definitions.h` & `libbde-20240502/libfdatetime/libfdatetime_definitions.h`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfdatetime/definitions.h> are copied here
  * for local use of libfdatetime
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFDATETIME_VERSION					20240115
+#define LIBFDATETIME_VERSION					20240415
 
 /* The version string
  */
-#define LIBFDATETIME_VERSION_STRING				"20240115"
+#define LIBFDATETIME_VERSION_STRING				"20240415"
 
 /* The byte order definitions
  */
 #define LIBFDATETIME_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define LIBFDATETIME_ENDIAN_LITTLE				_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The string format definition flags
```

### Comparing `libbde-20240223/libfdatetime/libfdatetime_hfs_time.c` & `libbde-20240502/libfdatetime/libfdatetime_hfs_time.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfdatetime/Makefile.am` & `libbde-20240502/libfdatetime/Makefile.am`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFDATETIME
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ 
 
 noinst_LTLIBRARIES = libfdatetime.la
 
 libfdatetime_la_SOURCES = \
 	libfdatetime_date_time_values.c libfdatetime_date_time_values.h \
 	libfdatetime_definitions.h \
@@ -20,19 +20,17 @@
 	libfdatetime_posix_time.c libfdatetime_posix_time.h \
 	libfdatetime_support.c libfdatetime_support.h \
 	libfdatetime_systemtime.c libfdatetime_systemtime.h \
 	libfdatetime_types.h \
 	libfdatetime_unused.h
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdatetime ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdatetime_la_SOURCES)
```

### Comparing `libbde-20240223/libfdatetime/libfdatetime_filetime.c` & `libbde-20240502/libfdatetime/libfdatetime_filetime.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfdatetime/libfdatetime_systemtime.h` & `libbde-20240502/libfdatetime/libfdatetime_systemtime.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfdatetime/libfdatetime_extern.h` & `libbde-20240502/libfdatetime/libfdatetime_extern.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfdatetime/libfdatetime_posix_time.c` & `libbde-20240502/libfdatetime/libfdatetime_posix_time.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfdatetime/libfdatetime_unused.h` & `libbde-20240502/libfdatetime/libfdatetime_unused.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfdatetime/libfdatetime_fat_date_time.h` & `libbde-20240502/libfdatetime/libfdatetime_fat_date_time.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfdatetime/libfdatetime_systemtime.c` & `libbde-20240502/libfdatetime/libfdatetime_systemtime.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfdatetime/libfdatetime_nsf_timedate.h` & `libbde-20240502/libfdatetime/libfdatetime_nsf_timedate.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfdatetime/libfdatetime_libcerror.h` & `libbde-20240502/libfdatetime/libfdatetime_libcerror.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfdatetime/libfdatetime_support.c` & `libbde-20240502/libfdatetime/libfdatetime_support.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfdatetime/libfdatetime_error.c` & `libbde-20240502/libfdatetime/libfdatetime_error.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfdatetime/libfdatetime_posix_time.h` & `libbde-20240502/libfdatetime/libfdatetime_posix_time.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfdatetime/libfdatetime_date_time_values.h` & `libbde-20240502/libfdatetime/libfdatetime_date_time_values.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfdatetime/libfdatetime_filetime.h` & `libbde-20240502/libfdatetime/libfdatetime_filetime.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfdatetime/libfdatetime_date_time_values.c` & `libbde-20240502/libfdatetime/libfdatetime_date_time_values.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfdatetime/libfdatetime_types.h` & `libbde-20240502/libfdatetime/libfdatetime_types.h`

 * *Files identical despite different names*

### Comparing `libbde-20240223/libfdatetime/Makefile.in` & `libbde-20240502/libfdatetime/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -491,14 +491,16 @@
 build_vendor = @build_vendor@
 builddir = @builddir@
 datadir = @datadir@
 datarootdir = @datarootdir@
 docdir = @docdir@
 dvidir = @dvidir@
 exec_prefix = @exec_prefix@
+fuse3_CFLAGS = @fuse3_CFLAGS@
+fuse3_LIBS = @fuse3_LIBS@
 fuse_CFLAGS = @fuse_CFLAGS@
 fuse_LIBS = @fuse_LIBS@
 host = @host@
 host_alias = @host_alias@
 host_cpu = @host_cpu@
 host_os = @host_os@
 host_vendor = @host_vendor@
@@ -561,16 +563,16 @@
 srcdir = @srcdir@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 @HAVE_LOCAL_LIBFDATETIME_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFDATETIME_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	@LIBCERROR_CPPFLAGS@ 
 
 @HAVE_LOCAL_LIBFDATETIME_TRUE@noinst_LTLIBRARIES = libfdatetime.la
 @HAVE_LOCAL_LIBFDATETIME_TRUE@libfdatetime_la_SOURCES = \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_date_time_values.c libfdatetime_date_time_values.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_definitions.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_extern.h \
@@ -583,15 +585,16 @@
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_nsf_timedate.c libfdatetime_nsf_timedate.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_posix_time.c libfdatetime_posix_time.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_support.c libfdatetime_support.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_systemtime.c libfdatetime_systemtime.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_types.h \
 @HAVE_LOCAL_LIBFDATETIME_TRUE@	libfdatetime_unused.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -800,24 +803,36 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfdatetime_date_time_values.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_error.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_fat_date_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_filetime.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_floatingtime.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_hfs_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_nsf_timedate.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_posix_time.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_support.Plo
+	-rm -f ./$(DEPDIR)/libfdatetime_systemtime.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -910,17 +925,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfdatetime ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdatetime_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libbde-20240223/libfdatetime/libfdatetime_fat_date_time.c` & `libbde-20240502/libfdatetime/libfdatetime_fat_date_time.c`

 * *Files identical despite different names*

### Comparing `libbde-20240223/aclocal.m4` & `libbde-20240502/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libbde-20240223/configure.ac` & `libbde-20240502/configure.ac`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libbde],
- [20240223],
+ [20240502],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libbde.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

