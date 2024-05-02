# Comparing `tmp/libfvde-python-20240113.tar.gz` & `tmp/libfvde-python-20240502.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libfvde-python-20240113.tar", last modified: Sat Jan 13 10:25:41 2024, max compression
+gzip compressed data, was "libfvde-python-20240502.tar", last modified: Thu May  2 05:49:20 2024, max compression
```

## Comparing `libfvde-python-20240113.tar` & `libfvde-python-20240502.tar`

### file list

```diff
@@ -1,998 +1,998 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:34.000000 libfvde-20240113/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_area.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_mapped_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3999 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1256 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_area.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_mapped_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_segments_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_segments_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34939 2024-01-13 09:42:44.000000 libfvde-20240113/libfdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-01-13 09:42:23.000000 libfvde-20240113/libfdata/libfdata_vector.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-01-13 09:19:22.000000 libfvde-20240113/COPYING
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-01-13 09:42:44.000000 libfvde-20240113/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 09:19:22.000000 libfvde-20240113/NEWS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-01-13 09:42:45.000000 libfvde-20240113/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:34.000000 libfvde-20240113/libfplist/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1401 2024-01-13 09:42:25.000000 libfvde-20240113/libfplist/libfplist_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-01-13 09:42:25.000000 libfvde-20240113/libfplist/libfplist_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5928 2024-01-13 09:42:25.000000 libfvde-20240113/libfplist/libfplist_xml_attribute.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1635 2024-01-13 09:42:25.000000 libfvde-20240113/libfplist/libfplist_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6651 2024-01-13 09:42:25.000000 libfvde-20240113/libfplist/libfplist_xml_scanner.l
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-01-13 09:42:25.000000 libfvde-20240113/libfplist/libfplist_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)  8431465 2024-01-13 09:43:38.000000 libfvde-20240113/libfplist/libfplist_xml_scanner.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56503 2024-01-13 09:43:38.000000 libfvde-20240113/libfplist/libfplist_xml_parser.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1516 2024-01-13 09:42:25.000000 libfvde-20240113/libfplist/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-01-13 09:42:25.000000 libfvde-20240113/libfplist/libfplist_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-01-13 09:42:25.000000 libfvde-20240113/libfplist/libfplist_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1788 2024-01-13 09:42:25.000000 libfvde-20240113/libfplist/libfplist_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1711 2024-01-13 09:42:25.000000 libfvde-20240113/libfplist/libfplist_xml_attribute.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-01-13 09:42:25.000000 libfvde-20240113/libfplist/libfplist_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-01-13 09:42:25.000000 libfvde-20240113/libfplist/libfplist_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1460 2024-01-13 09:42:25.000000 libfvde-20240113/libfplist/libfplist_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-01-13 09:42:25.000000 libfvde-20240113/libfplist/libfplist_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-01-13 09:42:25.000000 libfvde-20240113/libfplist/libfplist_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12481 2024-01-13 09:42:25.000000 libfvde-20240113/libfplist/libfplist_xml_parser.y
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4066 2024-01-13 09:43:38.000000 libfvde-20240113/libfplist/libfplist_xml_parser.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15149 2024-01-13 09:42:25.000000 libfvde-20240113/libfplist/libfplist_property_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3419 2024-01-13 09:42:25.000000 libfvde-20240113/libfplist/libfplist_property.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34608 2024-01-13 09:42:25.000000 libfvde-20240113/libfplist/libfplist_property.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15574 2024-01-13 09:42:25.000000 libfvde-20240113/libfplist/libfplist_xml_tag.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2497 2024-01-13 09:42:25.000000 libfvde-20240113/libfplist/libfplist_property_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-01-13 09:42:25.000000 libfvde-20240113/libfplist/libfplist_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1794 2024-01-13 09:42:25.000000 libfvde-20240113/libfplist/libfplist_libfvalue.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35780 2024-01-13 09:42:45.000000 libfvde-20240113/libfplist/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2894 2024-01-13 09:42:25.000000 libfvde-20240113/libfplist/libfplist_xml_tag.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:34.000000 libfvde-20240113/libcaes/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-01-13 09:42:11.000000 libfvde-20240113/libcaes/libcaes_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2885 2024-01-13 09:42:11.000000 libfvde-20240113/libcaes/libcaes_tweaked_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4464 2024-01-13 09:42:11.000000 libfvde-20240113/libcaes/libcaes_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-01-13 09:42:11.000000 libfvde-20240113/libcaes/libcaes_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82616 2024-01-13 09:42:11.000000 libfvde-20240113/libcaes/libcaes_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1743 2024-01-13 09:42:11.000000 libfvde-20240113/libcaes/libcaes_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-01-13 09:42:11.000000 libfvde-20240113/libcaes/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-01-13 09:42:11.000000 libfvde-20240113/libcaes/libcaes_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1608 2024-01-13 09:42:11.000000 libfvde-20240113/libcaes/libcaes_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-01-13 09:42:11.000000 libfvde-20240113/libcaes/libcaes_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-01-13 09:42:11.000000 libfvde-20240113/libcaes/libcaes_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-01-13 09:42:11.000000 libfvde-20240113/libcaes/libcaes_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-01-13 09:42:11.000000 libfvde-20240113/libcaes/libcaes_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31459 2024-01-13 09:42:44.000000 libfvde-20240113/libcaes/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33103 2024-01-13 09:42:11.000000 libfvde-20240113/libcaes/libcaes_tweaked_context.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/pyfvde/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-01-13 09:19:25.000000 libfvde-20240113/pyfvde/pyfvde_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22664 2024-01-13 09:21:20.000000 libfvde-20240113/pyfvde/pyfvde_volume_group.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2024-01-13 09:19:25.000000 libfvde-20240113/pyfvde/pyfvde_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16593 2024-01-13 09:19:25.000000 libfvde-20240113/pyfvde/pyfvde_datetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32405 2024-01-13 09:21:20.000000 libfvde-20240113/pyfvde/pyfvde_logical_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2527 2024-01-13 09:19:25.000000 libfvde-20240113/pyfvde/pyfvde_logical_volumes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8858 2024-01-13 09:19:25.000000 libfvde-20240113/pyfvde/pyfvde_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3713 2024-01-13 09:21:20.000000 libfvde-20240113/pyfvde/pyfvde_logical_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4960 2024-01-13 09:19:25.000000 libfvde-20240113/pyfvde/pyfvde_file_objects_io_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16283 2024-01-13 09:21:20.000000 libfvde-20240113/pyfvde/pyfvde.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1535 2024-01-13 09:19:25.000000 libfvde-20240113/pyfvde/pyfvde_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1512 2023-12-03 09:08:56.000000 libfvde-20240113/pyfvde/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-01-13 09:19:25.000000 libfvde-20240113/pyfvde/pyfvde_libfvde.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-01-13 09:19:25.000000 libfvde-20240113/pyfvde/pyfvde_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4160 2024-01-13 09:21:20.000000 libfvde-20240113/pyfvde/pyfvde_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2030 2024-01-13 09:19:25.000000 libfvde-20240113/pyfvde/pyfvde_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-01-13 09:19:25.000000 libfvde-20240113/pyfvde/pyfvde_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-01-13 09:21:20.000000 libfvde-20240113/pyfvde/pyfvde_guid.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33791 2024-01-13 09:19:25.000000 libfvde-20240113/pyfvde/pyfvde_file_object_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    63679 2024-01-13 09:21:20.000000 libfvde-20240113/pyfvde/pyfvde_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1815 2024-01-13 09:19:25.000000 libfvde-20240113/pyfvde/pyfvde_datetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2310 2024-01-13 09:19:25.000000 libfvde-20240113/pyfvde/pyfvde_physical_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10741 2024-01-13 09:21:20.000000 libfvde-20240113/pyfvde/pyfvde_physical_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3290 2024-01-13 09:21:20.000000 libfvde-20240113/pyfvde/pyfvde_volume_group.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-01-13 09:19:25.000000 libfvde-20240113/pyfvde/pyfvde_guid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2548 2024-01-13 09:19:25.000000 libfvde-20240113/pyfvde/pyfvde_physical_volumes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4080 2024-01-13 09:19:25.000000 libfvde-20240113/pyfvde/pyfvde_file_object_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9597 2024-01-13 09:19:25.000000 libfvde-20240113/pyfvde/pyfvde_logical_volumes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9659 2024-01-13 09:19:25.000000 libfvde-20240113/pyfvde/pyfvde_physical_volumes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-01-13 09:19:25.000000 libfvde-20240113/pyfvde/pyfvde_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    53752 2024-01-13 09:42:45.000000 libfvde-20240113/pyfvde/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1855 2024-01-13 09:19:25.000000 libfvde-20240113/pyfvde/pyfvde.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-01-13 09:19:25.000000 libfvde-20240113/pyfvde/pyfvde_file_objects_io_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-01-13 09:19:25.000000 libfvde-20240113/pyfvde/pyfvde_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-01-13 09:19:25.000000 libfvde-20240113/pyfvde/pyfvde_error.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:34.000000 libfvde-20240113/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-01-13 09:42:24.000000 libfvde-20240113/libfguid/libfguid_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-01-13 09:42:24.000000 libfvde-20240113/libfguid/libfguid_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-01-13 09:42:24.000000 libfvde-20240113/libfguid/libfguid_identifier.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-01-13 09:42:24.000000 libfvde-20240113/libfguid/libfguid_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      646 2024-01-13 09:42:24.000000 libfvde-20240113/libfguid/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-01-13 09:42:24.000000 libfvde-20240113/libfguid/libfguid_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-01-13 09:42:24.000000 libfvde-20240113/libfguid/libfguid_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-01-13 09:42:24.000000 libfvde-20240113/libfguid/libfguid_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-01-13 09:42:24.000000 libfvde-20240113/libfguid/libfguid_identifier.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-01-13 09:42:24.000000 libfvde-20240113/libfguid/libfguid_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-01-13 09:42:24.000000 libfvde-20240113/libfguid/libfguid_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31154 2024-01-13 09:42:44.000000 libfvde-20240113/libfguid/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-01-13 09:42:24.000000 libfvde-20240113/libfguid/libfguid_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3650 2024-01-13 09:19:22.000000 libfvde-20240113/libfvde.spec.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/libfvde/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1132 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde.rc.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8260 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_sector_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_checksum.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1614 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1611 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2180 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4353 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_encryption_context_plist.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14533 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_password.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8407 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_logical_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7980 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_bit_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26590 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_volume_group.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1514 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_libfplist.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81729 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_logical_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1327 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_compression.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1900 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2214 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/fvde_metadata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2246 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_metadata_block.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1512 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_libcaes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3324 2023-12-03 09:08:39.000000 libfvde-20240113/libfvde/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2707 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_physical_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2847 2024-01-13 09:43:00.000000 libfvde-20240113/libfvde/libfvde_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2086 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1928 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_physical_volume_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1525 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1480 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_libhmac.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2811 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   168049 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_encrypted_metadata.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1943 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_sector_data.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1573 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_keyring.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1647 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17109 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_encryption_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_volume_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3213 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_checksum.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5033 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_physical_volume_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44991 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_encryption_context_plist.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4771 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_logical_volume_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1130 2024-01-13 09:43:00.000000 libfvde-20240113/libfvde/libfvde.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1805 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_password.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1987 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7458 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_volume_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4093 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12433 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_metadata_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48684 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_deflate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10777 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9512 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_encrypted_metadata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1802 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3696 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/fvde_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1507 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1445 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4107 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_metadata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2020 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_segment_descriptor.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2683 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2146 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_huffman_tree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2484 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_encryption_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41300 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_metadata.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3526 2024-01-13 09:21:50.000000 libfvde-20240113/libfvde/libfvde_deflate.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2333 2024-01-13 09:21:50.000000 libfvde-20240113/libfvde/libfvde_bit_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1464 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1857 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_libfvalue.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1841 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4374 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_volume_group.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9373 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19712 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_logical_volume_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2965 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1769 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12569 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_huffman_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1469 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4975 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41493 2024-01-13 09:42:45.000000 libfvde-20240113/libfvde/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3194 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_keyring.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3202 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_volume_header.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122689 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22452 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_volume_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4578 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_segment_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11293 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_physical_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1842 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5703 2024-01-13 09:19:25.000000 libfvde-20240113/libfvde/libfvde_compression.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:33.000000 libfvde-20240113/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2023-12-03 09:08:37.000000 libfvde-20240113/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:08:37.000000 libfvde-20240113/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2023-12-03 09:08:37.000000 libfvde-20240113/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:08:37.000000 libfvde-20240113/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:08:37.000000 libfvde-20240113/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31269 2023-12-03 09:08:36.000000 libfvde-20240113/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:08:37.000000 libfvde-20240113/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:08:37.000000 libfvde-20240113/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2023-12-03 09:08:37.000000 libfvde-20240113/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-12-03 09:08:37.000000 libfvde-20240113/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2023-12-03 09:08:37.000000 libfvde-20240113/m4/libcsplit.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-12-03 09:08:37.000000 libfvde-20240113/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-12-03 09:08:37.000000 libfvde-20240113/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-01-13 09:42:37.000000 libfvde-20240113/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-01-13 09:42:37.000000 libfvde-20240113/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15545 2023-12-03 09:08:37.000000 libfvde-20240113/m4/libfdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:08:37.000000 libfvde-20240113/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5232 2023-12-03 09:08:37.000000 libfvde-20240113/m4/libfuse.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-01-13 09:42:37.000000 libfvde-20240113/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:08:37.000000 libfvde-20240113/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-12-03 09:08:37.000000 libfvde-20240113/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-12-03 09:08:37.000000 libfvde-20240113/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5640 2023-12-03 09:08:37.000000 libfvde-20240113/m4/libfguid.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2023-12-03 09:08:37.000000 libfvde-20240113/m4/libbfio.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8319 2023-12-03 09:08:37.000000 libfvde-20240113/m4/libhmac.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:08:37.000000 libfvde-20240113/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-01-13 09:42:37.000000 libfvde-20240113/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:08:37.000000 libfvde-20240113/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:08:37.000000 libfvde-20240113/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-01-13 09:42:37.000000 libfvde-20240113/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:08:36.000000 libfvde-20240113/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6323 2023-12-03 09:08:37.000000 libfvde-20240113/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27481 2023-12-03 09:08:37.000000 libfvde-20240113/m4/libcrypto.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19791 2023-12-03 09:08:37.000000 libfvde-20240113/m4/libfvalue.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:08:37.000000 libfvde-20240113/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7325 2023-12-03 09:08:37.000000 libfvde-20240113/m4/libfcache.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-12-03 09:08:37.000000 libfvde-20240113/m4/pthread.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6201 2023-12-03 09:08:36.000000 libfvde-20240113/m4/libfplist.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7383 2023-12-03 09:08:37.000000 libfvde-20240113/m4/zlib.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6269 2023-12-03 09:08:37.000000 libfvde-20240113/m4/libcaes.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:33.000000 libfvde-20240113/include/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30542 2024-01-13 09:19:24.000000 libfvde-20240113/include/libfvde.h.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:33.000000 libfvde-20240113/include/libfvde/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1905 2024-01-13 09:19:24.000000 libfvde-20240113/include/libfvde/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1903 2024-01-13 09:43:00.000000 libfvde-20240113/include/libfvde/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5185 2024-01-13 09:19:24.000000 libfvde-20240113/include/libfvde/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5054 2024-01-13 09:43:00.000000 libfvde-20240113/include/libfvde/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1608 2024-01-13 09:19:24.000000 libfvde-20240113/include/libfvde/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2024-01-13 09:19:24.000000 libfvde-20240113/include/libfvde/error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1481 2024-01-13 09:19:24.000000 libfvde-20240113/include/libfvde/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2024-01-13 09:43:00.000000 libfvde-20240113/include/libfvde/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5264 2024-01-13 09:19:24.000000 libfvde-20240113/include/libfvde/codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      459 2024-01-13 09:19:22.000000 libfvde-20240113/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30542 2024-01-13 09:42:59.000000 libfvde-20240113/include/libfvde.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29728 2024-01-13 09:42:44.000000 libfvde-20240113/include/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:33.000000 libfvde-20240113/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-01-13 09:19:24.000000 libfvde-20240113/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-01-13 09:19:24.000000 libfvde-20240113/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-01-13 09:19:24.000000 libfvde-20240113/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-01-13 09:19:24.000000 libfvde-20240113/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-01-13 09:19:24.000000 libfvde-20240113/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-01-13 09:19:24.000000 libfvde-20240113/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-01-13 09:19:24.000000 libfvde-20240113/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      366 2024-01-13 09:19:22.000000 libfvde-20240113/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-01-13 09:19:24.000000 libfvde-20240113/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7373 2024-01-13 09:43:00.000000 libfvde-20240113/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20052 2024-01-13 09:42:43.000000 libfvde-20240113/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21198 2024-01-13 09:43:00.000000 libfvde-20240113/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-01-13 09:19:24.000000 libfvde-20240113/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-01-13 09:19:24.000000 libfvde-20240113/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-01-13 09:19:24.000000 libfvde-20240113/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26754 2024-01-13 09:42:44.000000 libfvde-20240113/common/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:33.000000 libfvde-20240113/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-01-13 09:42:16.000000 libfvde-20240113/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-01-13 09:42:16.000000 libfvde-20240113/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      779 2024-01-13 09:42:16.000000 libfvde-20240113/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-01-13 09:42:16.000000 libfvde-20240113/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-01-13 09:42:16.000000 libfvde-20240113/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-01-13 09:42:16.000000 libfvde-20240113/libclocale/libclocale_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-01-13 09:42:16.000000 libfvde-20240113/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-01-13 09:42:16.000000 libfvde-20240113/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-01-13 09:42:16.000000 libfvde-20240113/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-01-13 09:42:16.000000 libfvde-20240113/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31757 2024-01-13 09:42:44.000000 libfvde-20240113/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-01-13 09:42:16.000000 libfvde-20240113/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-01-13 09:42:16.000000 libfvde-20240113/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-01-13 09:42:16.000000 libfvde-20240113/libclocale/libclocale_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2464 2024-01-13 09:43:00.000000 libfvde-20240113/libfvde.spec
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:34.000000 libfvde-20240113/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-01-13 09:42:22.000000 libfvde-20240113/libfcache/libfcache_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-01-13 09:42:22.000000 libfvde-20240113/libfcache/libfcache_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-01-13 09:42:22.000000 libfvde-20240113/libfcache/libfcache_cache_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-01-13 09:42:22.000000 libfvde-20240113/libfcache/libfcache_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-01-13 09:42:22.000000 libfvde-20240113/libfcache/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-01-13 09:42:22.000000 libfvde-20240113/libfcache/libfcache_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-01-13 09:42:22.000000 libfvde-20240113/libfcache/libfcache_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-01-13 09:42:22.000000 libfvde-20240113/libfcache/libfcache_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-01-13 09:42:22.000000 libfvde-20240113/libfcache/libfcache_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-01-13 09:42:22.000000 libfvde-20240113/libfcache/libfcache_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-01-13 09:42:22.000000 libfvde-20240113/libfcache/libfcache_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-01-13 09:42:22.000000 libfvde-20240113/libfcache/libfcache_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-01-13 09:42:22.000000 libfvde-20240113/libfcache/libfcache_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-01-13 09:42:22.000000 libfvde-20240113/libfcache/libfcache_cache_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32230 2024-01-13 09:42:44.000000 libfvde-20240113/libfcache/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-01-13 09:42:22.000000 libfvde-20240113/libfcache/libfcache_date_time.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-01-13 09:42:22.000000 libfvde-20240113/libfcache/libfcache_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-01-13 09:42:22.000000 libfvde-20240113/libfcache/libfcache_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2462 2023-12-03 09:08:36.000000 libfvde-20240113/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:34.000000 libfvde-20240113/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_file_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_file_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_file_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_file_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_file_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_file_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_memory_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_file_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_file_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_memory_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_memory_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35216 2024-01-13 09:42:44.000000 libfvde-20240113/libbfio/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_memory_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-01-13 09:42:09.000000 libfvde-20240113/libbfio/libbfio_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:08:35.000000 libfvde-20240113/ABOUT-NLS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-01-13 09:42:44.000000 libfvde-20240113/config.guess
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:33.000000 libfvde-20240113/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-01-13 09:19:22.000000 libfvde-20240113/dpkg/libfvde-dev.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1024 2024-01-13 09:19:26.000000 libfvde-20240113/dpkg/copyright
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:33.000000 libfvde-20240113/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-01-13 09:19:22.000000 libfvde-20240113/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2136 2024-01-13 09:19:22.000000 libfvde-20240113/dpkg/control
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-01-13 09:19:22.000000 libfvde-20240113/dpkg/libfvde.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      761 2024-01-13 09:19:22.000000 libfvde-20240113/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      120 2024-01-13 09:19:22.000000 libfvde-20240113/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      139 2024-01-13 09:43:00.000000 libfvde-20240113/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-01-13 09:19:22.000000 libfvde-20240113/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-01-13 09:19:22.000000 libfvde-20240113/dpkg/libfvde-python3.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-01-13 09:19:22.000000 libfvde-20240113/dpkg/libfvde-tools.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      483 2024-01-13 09:43:00.000000 libfvde-20240113/setup.cfg
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-01-13 09:19:22.000000 libfvde-20240113/COPYING.LESSER
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  2150165 2024-01-13 09:42:42.000000 libfvde-20240113/configure
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-01-13 09:42:44.000000 libfvde-20240113/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-01-13 09:42:44.000000 libfvde-20240113/missing
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/libfdata/libfdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvde_test_encrypted_metadata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6174 2024-01-13 09:20:29.000000 libfvde-20240113/msvscpp/fvde_test_encrypted_metadata/fvde_test_encrypted_metadata.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44126 2024-01-13 09:20:29.000000 libfvde-20240113/msvscpp/libfvde.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvde_test_segment_descriptor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6092 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/fvde_test_segment_descriptor/fvde_test_segment_descriptor.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvde_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6714 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/fvde_test_support/fvde_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/zlib/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6068 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/zlib/zlib.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/libfplist/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6237 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/libfplist/libfplist.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvde_test_compression/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6071 2024-01-13 09:20:29.000000 libfvde-20240113/msvscpp/fvde_test_compression/fvde_test_compression.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/libcaes/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4777 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/libcaes/libcaes.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/pyfvde/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7522 2024-01-13 09:20:29.000000 libfvde-20240113/msvscpp/pyfvde/pyfvde.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/libfguid/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/libfguid/libfguid.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/libfvde/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11896 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/libfvde/libfvde.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvde_test_logical_volume/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6080 2024-01-13 09:20:29.000000 libfvde-20240113/msvscpp/fvde_test_logical_volume/fvde_test_logical_volume.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/libclocale/libclocale.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvde_test_tools_signal/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6001 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/fvde_test_tools_signal/fvde_test_tools_signal.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/libfcache/libfcache.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2348 2024-01-13 09:20:29.000000 libfvde-20240113/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/libbfio/libbfio.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvde_test_keyring/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6059 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/fvde_test_keyring/fvde_test_keyring.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvde_test_encryption_context/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6092 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/fvde_test_encryption_context/fvde_test_encryption_context.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvdewipekey/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6535 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/fvdewipekey/fvdewipekey.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvde_test_deflate/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5983 2024-01-13 09:20:29.000000 libfvde-20240113/msvscpp/fvde_test_deflate/fvde_test_deflate.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvde_test_physical_volume_descriptor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6116 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/fvde_test_physical_volume_descriptor/fvde_test_physical_volume_descriptor.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvde_test_logical_volume_descriptor/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6113 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/fvde_test_logical_volume_descriptor/fvde_test_logical_volume_descriptor.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvdeinfo/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7198 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/fvdeinfo/fvdeinfo.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvde_test_volume_data_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6092 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/fvde_test_volume_data_handle/fvde_test_volume_data_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvde_test_volume_header/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6324 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/fvde_test_volume_header/fvde_test_volume_header.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvde_test_metadata_block/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6080 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/fvde_test_metadata_block/fvde_test_metadata_block.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvde_test_io_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6065 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/fvde_test_io_handle/fvde_test_io_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvde_test_encryption_context_plist/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6110 2024-01-13 09:20:29.000000 libfvde-20240113/msvscpp/fvde_test_encryption_context_plist/fvde_test_encryption_context_plist.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/libcpath/libcpath.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvde_test_sector_data/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6071 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/fvde_test_sector_data/fvde_test_sector_data.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvde_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5810 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/fvde_test_error/fvde_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvde_test_checksum/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5902 2024-01-13 09:20:29.000000 libfvde-20240113/msvscpp/fvde_test_checksum/fvde_test_checksum.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvde_test_metadata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6062 2024-01-13 09:20:29.000000 libfvde-20240113/msvscpp/fvde_test_metadata/fvde_test_metadata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/libhmac/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5312 2024-01-13 09:20:29.000000 libfvde-20240113/msvscpp/libhmac/libhmac.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvde_test_physical_volume/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6083 2024-01-13 09:20:29.000000 libfvde-20240113/msvscpp/fvde_test_physical_volume/fvde_test_physical_volume.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvde_test_bit_stream/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6068 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/fvde_test_bit_stream/fvde_test_bit_stream.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/libcsplit/libcsplit.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvde_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5896 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/fvde_test_notify/fvde_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26070 2024-01-13 09:42:45.000000 libfvde-20240113/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7924 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/libfvalue/libfvalue.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvde_test_huffman_tree/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6074 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/fvde_test_huffman_tree/fvde_test_huffman_tree.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvde_test_volume/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6711 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/fvde_test_volume/fvde_test_volume.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvde_test_tools_output/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6001 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/fvde_test_tools_output/fvde_test_tools_output.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvde_test_volume_group/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6074 2024-01-13 09:20:29.000000 libfvde-20240113/msvscpp/fvde_test_volume_group/fvde_test_volume_group.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/msvscpp/fvdemount/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7925 2024-01-13 09:19:55.000000 libfvde-20240113/msvscpp/fvdemount/fvdemount.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      280 2024-01-13 09:21:31.000000 libfvde-20240113/AUTHORS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:34.000000 libfvde-20240113/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-01-13 09:42:14.000000 libfvde-20240113/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-01-13 09:42:14.000000 libfvde-20240113/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-01-13 09:42:14.000000 libfvde-20240113/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-01-13 09:42:14.000000 libfvde-20240113/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-01-13 09:42:14.000000 libfvde-20240113/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-01-13 09:42:14.000000 libfvde-20240113/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      942 2024-01-13 09:42:14.000000 libfvde-20240113/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-01-13 09:42:14.000000 libfvde-20240113/libcfile/libcfile_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-01-13 09:42:14.000000 libfvde-20240113/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-01-13 09:42:14.000000 libfvde-20240113/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-01-13 09:42:14.000000 libfvde-20240113/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-01-13 09:42:14.000000 libfvde-20240113/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-01-13 09:42:14.000000 libfvde-20240113/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-01-13 09:42:14.000000 libfvde-20240113/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-01-13 09:42:14.000000 libfvde-20240113/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-01-13 09:42:14.000000 libfvde-20240113/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-01-13 09:42:14.000000 libfvde-20240113/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32521 2024-01-13 09:42:44.000000 libfvde-20240113/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-01-13 09:42:14.000000 libfvde-20240113/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-01-13 09:42:14.000000 libfvde-20240113/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-01-13 09:42:14.000000 libfvde-20240113/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-01-13 09:42:14.000000 libfvde-20240113/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1981 2024-01-13 09:21:31.000000 libfvde-20240113/README
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-01-13 09:42:44.000000 libfvde-20240113/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/fvdetools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37242 2024-01-13 09:19:26.000000 libfvde-20240113/fvdetools/mount_dokan.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-01-13 09:19:25.000000 libfvde-20240113/fvdetools/fvdetools_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3051 2024-01-13 09:21:31.000000 libfvde-20240113/fvdetools/mount_file_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26512 2024-01-13 09:19:26.000000 libfvde-20240113/fvdetools/mount_fuse.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-01-13 09:21:31.000000 libfvde-20240113/fvdetools/info_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5483 2024-01-13 09:19:26.000000 libfvde-20240113/fvdetools/mount_dokan.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1312 2024-01-13 09:19:25.000000 libfvde-20240113/fvdetools/fvdetools_input.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1460 2024-01-13 09:19:25.000000 libfvde-20240113/fvdetools/fvdetools_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1570 2024-01-13 09:19:25.000000 libfvde-20240113/fvdetools/fvdetools_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1847 2024-01-13 09:19:25.000000 libfvde-20240113/fvdetools/fvdetools_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17296 2024-01-13 09:21:31.000000 libfvde-20240113/fvdetools/mount_file_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5795 2024-01-13 09:19:25.000000 libfvde-20240113/fvdetools/fvdetools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4003 2024-01-13 09:19:25.000000 libfvde-20240113/fvdetools/fvdetools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11856 2024-01-13 09:19:25.000000 libfvde-20240113/fvdetools/byte_size_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1475 2024-01-13 09:19:25.000000 libfvde-20240113/fvdetools/fvdetools_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1509 2024-01-13 09:19:25.000000 libfvde-20240113/fvdetools/fvdetools_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3414 2023-12-03 09:08:39.000000 libfvde-20240113/fvdetools/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1814 2024-01-13 09:19:25.000000 libfvde-20240113/fvdetools/fvdetools_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1549 2024-01-13 09:19:25.000000 libfvde-20240113/fvdetools/fvdetools_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1605 2024-01-13 09:19:26.000000 libfvde-20240113/fvdetools/fvdetools_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21090 2024-01-13 09:21:31.000000 libfvde-20240113/fvdetools/mount_file_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47235 2024-01-13 09:21:31.000000 libfvde-20240113/fvdetools/info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3661 2024-01-13 09:21:31.000000 libfvde-20240113/fvdetools/mount_file_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9020 2024-01-13 09:21:31.000000 libfvde-20240113/fvdetools/fvdeinfo.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1877 2024-01-13 09:19:25.000000 libfvde-20240113/fvdetools/fvdetools_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13497 2024-01-13 09:19:26.000000 libfvde-20240113/fvdetools/wipekey_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4249 2024-01-13 09:21:31.000000 libfvde-20240113/fvdetools/mount_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2491 2024-01-13 09:19:26.000000 libfvde-20240113/fvdetools/wipekey_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4600 2024-01-13 09:19:25.000000 libfvde-20240113/fvdetools/fvdetools_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1620 2024-01-13 09:19:25.000000 libfvde-20240113/fvdetools/fvdetools_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18374 2024-01-13 09:21:31.000000 libfvde-20240113/fvdetools/fvdemount.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33896 2024-01-13 09:21:31.000000 libfvde-20240113/fvdetools/mount_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6311 2024-01-13 09:19:25.000000 libfvde-20240113/fvdetools/fvdetools_input.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-01-13 09:19:26.000000 libfvde-20240113/fvdetools/fvdetools_signal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6998 2024-01-13 09:19:26.000000 libfvde-20240113/fvdetools/fvdewipekey.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1042 2024-01-13 09:19:25.000000 libfvde-20240113/fvdetools/fvdetools_libfvde.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38245 2024-01-13 09:42:44.000000 libfvde-20240113/fvdetools/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1989 2024-01-13 09:19:25.000000 libfvde-20240113/fvdetools/byte_size_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1279 2024-01-13 09:19:25.000000 libfvde-20240113/fvdetools/fvdetools_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-01-13 09:19:25.000000 libfvde-20240113/fvdetools/fvdetools_output.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-01-13 09:19:26.000000 libfvde-20240113/fvdetools/mount_fuse.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:33.000000 libfvde-20240113/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/libcdata_btree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1127 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34205 2024-01-13 09:42:44.000000 libfvde-20240113/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-01-13 09:42:12.000000 libfvde-20240113/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-01-13 09:19:22.000000 libfvde-20240113/pyproject.toml
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6860 2024-01-13 09:42:45.000000 libfvde-20240113/ylwrap
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      484 2024-01-13 09:19:22.000000 libfvde-20240113/setup.cfg.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-01-13 09:42:44.000000 libfvde-20240113/config.sub
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-01-13 09:19:22.000000 libfvde-20240113/setup.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-01-13 09:21:31.000000 libfvde-20240113/acinclude.m4
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:08:35.000000 libfvde-20240113/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:33.000000 libfvde-20240113/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-01-13 09:42:21.000000 libfvde-20240113/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-01-13 09:42:21.000000 libfvde-20240113/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-01-13 09:42:21.000000 libfvde-20240113/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-01-13 09:42:21.000000 libfvde-20240113/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-01-13 09:42:21.000000 libfvde-20240113/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-01-13 09:42:21.000000 libfvde-20240113/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-01-13 09:42:21.000000 libfvde-20240113/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-01-13 09:42:21.000000 libfvde-20240113/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-01-13 09:42:21.000000 libfvde-20240113/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-01-13 09:42:21.000000 libfvde-20240113/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1171 2024-01-13 09:42:21.000000 libfvde-20240113/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-01-13 09:42:21.000000 libfvde-20240113/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-01-13 09:42:21.000000 libfvde-20240113/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-01-13 09:42:21.000000 libfvde-20240113/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-01-13 09:42:21.000000 libfvde-20240113/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-01-13 09:42:21.000000 libfvde-20240113/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-01-13 09:42:21.000000 libfvde-20240113/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-01-13 09:42:21.000000 libfvde-20240113/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-01-13 09:42:21.000000 libfvde-20240113/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-01-13 09:42:21.000000 libfvde-20240113/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-01-13 09:42:21.000000 libfvde-20240113/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-01-13 09:42:21.000000 libfvde-20240113/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-01-13 09:42:21.000000 libfvde-20240113/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-01-13 09:42:21.000000 libfvde-20240113/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-01-13 09:42:21.000000 libfvde-20240113/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-01-13 09:42:21.000000 libfvde-20240113/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-01-13 09:42:21.000000 libfvde-20240113/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34611 2024-01-13 09:42:44.000000 libfvde-20240113/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-01-13 09:42:21.000000 libfvde-20240113/libcthreads/libcthreads_queue.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-01-13 09:42:45.000000 libfvde-20240113/test-driver
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:34.000000 libfvde-20240113/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-01-13 09:42:18.000000 libfvde-20240113/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-01-13 09:42:18.000000 libfvde-20240113/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-01-13 09:42:18.000000 libfvde-20240113/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      842 2024-01-13 09:42:18.000000 libfvde-20240113/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-01-13 09:42:18.000000 libfvde-20240113/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-01-13 09:42:18.000000 libfvde-20240113/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-01-13 09:42:18.000000 libfvde-20240113/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-01-13 09:42:18.000000 libfvde-20240113/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-01-13 09:42:18.000000 libfvde-20240113/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-01-13 09:42:18.000000 libfvde-20240113/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-01-13 09:42:18.000000 libfvde-20240113/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-01-13 09:42:18.000000 libfvde-20240113/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31799 2024-01-13 09:42:44.000000 libfvde-20240113/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-01-13 09:42:18.000000 libfvde-20240113/libcpath/libcpath_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-01-13 09:42:18.000000 libfvde-20240113/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-01-13 09:42:18.000000 libfvde-20240113/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-01-13 09:42:18.000000 libfvde-20240113/libcpath/libcpath_path.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5202 2023-12-03 09:08:35.000000 libfvde-20240113/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10728 2024-01-13 09:21:20.000000 libfvde-20240113/manuals/libfvde.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      184 2023-12-03 09:08:39.000000 libfvde-20240113/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2263 2024-01-13 09:19:26.000000 libfvde-20240113/manuals/fvdeinfo.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1847 2024-01-13 09:19:26.000000 libfvde-20240113/manuals/fvdemount.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28750 2024-01-13 09:42:45.000000 libfvde-20240113/manuals/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/tests/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6782 2024-01-13 09:20:46.000000 libfvde-20240113/tests/fvde_test_sector_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)  6375570 2024-01-13 09:20:46.000000 libfvde-20240113/tests/fvde_test_encryption_context_plist.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8087 2024-01-13 09:20:46.000000 libfvde-20240113/tests/fvde_test_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5799 2024-01-13 09:19:26.000000 libfvde-20240113/tests/fvde_test_keyring.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15192 2024-01-13 09:19:26.000000 libfvde-20240113/tests/fvde_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8539 2024-01-13 09:19:26.000000 libfvde-20240113/tests/fvde_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4231 2024-01-13 09:19:26.000000 libfvde-20240113/tests/fvde_test_checksum.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-01-13 09:19:26.000000 libfvde-20240113/tests/fvde_test_libfvde.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17533 2024-01-13 09:20:46.000000 libfvde-20240113/tests/fvde_test_logical_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-01-13 09:19:26.000000 libfvde-20240113/tests/fvde_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-01-13 09:19:26.000000 libfvde-20240113/tests/fvde_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1620 2024-01-13 09:22:56.000000 libfvde-20240113/tests/fvde_test_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20944 2024-01-13 09:22:01.000000 libfvde-20240113/tests/pyfvde_test_logical_volume.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12703 2024-01-13 09:20:46.000000 libfvde-20240113/tests/fvde_test_metadata.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4092 2024-01-13 09:24:45.000000 libfvde-20240113/tests/test_tools.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5531 2024-01-13 09:19:26.000000 libfvde-20240113/tests/fvde_test_compression.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1987 2024-01-13 09:19:26.000000 libfvde-20240113/tests/fvde_test_functions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21372 2024-01-13 09:22:01.000000 libfvde-20240113/tests/pyfvde_test_volume.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4531 2024-01-13 09:19:26.000000 libfvde-20240113/tests/fvde_test_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6904 2024-01-13 09:20:46.000000 libfvde-20240113/tests/fvde_test_logical_volume_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10223 2024-01-13 09:20:46.000000 libfvde-20240113/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15712 2024-01-13 09:19:26.000000 libfvde-20240113/tests/fvde_test_functions.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6385 2024-01-13 09:20:46.000000 libfvde-20240113/tests/fvde_test_segment_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1706 2024-01-13 09:19:26.000000 libfvde-20240113/tests/fvde_test_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-01-13 09:19:26.000000 libfvde-20240113/tests/fvde_test_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4653 2024-01-13 09:19:26.000000 libfvde-20240113/tests/fvde_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11058 2024-01-13 09:22:01.000000 libfvde-20240113/tests/pyfvde_test_volume_group.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   127481 2024-01-13 09:20:46.000000 libfvde-20240113/tests/fvde_test_encrypted_metadata.c
--rwxr--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-01-13 09:19:26.000000 libfvde-20240113/tests/test_manpage.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3904 2024-01-13 09:24:14.000000 libfvde-20240113/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13622 2024-01-13 09:20:46.000000 libfvde-20240113/tests/fvde_test_bit_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2024-01-13 09:19:26.000000 libfvde-20240113/tests/fvde_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100206 2024-01-13 09:19:26.000000 libfvde-20240113/tests/fvde_test_deflate.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7726 2024-01-13 09:20:46.000000 libfvde-20240113/tests/fvde_test_volume_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2425 2024-01-13 09:20:46.000000 libfvde-20240113/tests/fvde_test_tools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8968 2024-01-13 09:20:46.000000 libfvde-20240113/tests/fvde_test_physical_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8565 2024-01-13 09:22:01.000000 libfvde-20240113/tests/pyfvde_test_physical_volume.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-01-13 09:19:26.000000 libfvde-20240113/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8109 2024-01-13 09:20:46.000000 libfvde-20240113/tests/fvde_test_metadata_block.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1691 2024-01-13 09:19:26.000000 libfvde-20240113/tests/fvde_test_memory.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3354 2024-01-13 09:19:26.000000 libfvde-20240113/tests/test_fvdeinfo.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2024-01-13 09:19:26.000000 libfvde-20240113/tests/fvde_test_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6960 2024-01-13 09:20:46.000000 libfvde-20240113/tests/fvde_test_physical_volume_descriptor.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3144 2024-01-13 09:22:01.000000 libfvde-20240113/tests/pyfvde_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30660 2024-01-13 09:20:46.000000 libfvde-20240113/tests/fvde_test_huffman_tree.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4276 2024-01-13 09:19:26.000000 libfvde-20240113/tests/fvde_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24384 2024-01-13 09:20:46.000000 libfvde-20240113/tests/fvde_test_volume_header.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4123 2024-01-13 09:20:46.000000 libfvde-20240113/tests/fvde_test_tools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    77514 2024-01-13 09:42:45.000000 libfvde-20240113/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-01-13 09:19:26.000000 libfvde-20240113/tests/fvde_test_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57129 2024-01-13 09:20:46.000000 libfvde-20240113/tests/fvde_test_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8921 2024-01-13 09:20:46.000000 libfvde-20240113/tests/fvde_test_volume_group.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-01-13 09:19:26.000000 libfvde-20240113/tests/fvde_test_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7263 2024-01-13 09:20:46.000000 libfvde-20240113/tests/fvde_test_encryption_context.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4422 2024-01-13 09:24:14.000000 libfvde-20240113/tests/test_library.sh
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3510 2024-01-13 09:19:25.000000 libfvde-20240113/ossfuzz/volume_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      901 2023-12-03 09:08:36.000000 libfvde-20240113/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-01-13 09:19:25.000000 libfvde-20240113/ossfuzz/ossfuzz_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34003 2024-01-13 09:42:45.000000 libfvde-20240113/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2024-01-13 09:19:25.000000 libfvde-20240113/ossfuzz/ossfuzz_libfvde.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-01-13 09:42:37.000000 libfvde-20240113/ltmain.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      859 2024-01-13 09:19:22.000000 libfvde-20240113/libfvde.pc.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:34.000000 libfvde-20240113/libhmac/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47989 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_sha1_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_sha224.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50026 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_sha512_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14448 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_md5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2079 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_md5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1942 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9362 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14650 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_sha512.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45648 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_sha256_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_sha224.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1623 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2060 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_sha1.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3443 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_sha256_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1121 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45605 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_sha224_context.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_md5_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_sha256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3368 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_sha1_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34331 2024-01-13 09:42:45.000000 libfvde-20240113/libhmac/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_sha256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3461 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_sha224_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3444 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_sha512_context.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_sha512.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14514 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_sha1.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40596 2024-01-13 09:42:28.000000 libfvde-20240113/libhmac/libhmac_md5_context.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:33.000000 libfvde-20240113/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-01-13 09:42:19.000000 libfvde-20240113/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-01-13 09:42:19.000000 libfvde-20240113/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-01-13 09:42:19.000000 libfvde-20240113/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-01-13 09:42:19.000000 libfvde-20240113/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-01-13 09:42:19.000000 libfvde-20240113/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      884 2024-01-13 09:42:19.000000 libfvde-20240113/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-01-13 09:42:19.000000 libfvde-20240113/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-01-13 09:42:19.000000 libfvde-20240113/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-01-13 09:42:19.000000 libfvde-20240113/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-01-13 09:42:19.000000 libfvde-20240113/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-01-13 09:42:19.000000 libfvde-20240113/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-01-13 09:42:19.000000 libfvde-20240113/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-01-13 09:42:19.000000 libfvde-20240113/libcsplit/libcsplit_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-01-13 09:42:19.000000 libfvde-20240113/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-01-13 09:42:19.000000 libfvde-20240113/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-01-13 09:42:19.000000 libfvde-20240113/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32579 2024-01-13 09:42:44.000000 libfvde-20240113/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-01-13 09:42:19.000000 libfvde-20240113/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-01-13 09:42:19.000000 libfvde-20240113/libcsplit/libcsplit_narrow_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:35.000000 libfvde-20240113/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:08:36.000000 libfvde-20240113/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:08:36.000000 libfvde-20240113/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:08:36.000000 libfvde-20240113/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:08:36.000000 libfvde-20240113/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:08:36.000000 libfvde-20240113/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:08:36.000000 libfvde-20240113/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:08:36.000000 libfvde-20240113/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:08:36.000000 libfvde-20240113/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:08:36.000000 libfvde-20240113/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-01-13 09:42:59.000000 libfvde-20240113/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:08:36.000000 libfvde-20240113/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:08:36.000000 libfvde-20240113/po/Rules-quot
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:33.000000 libfvde-20240113/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4162 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55276 2024-01-13 09:42:45.000000 libfvde-20240113/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-01-13 09:42:31.000000 libfvde-20240113/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42975 2024-01-13 09:42:44.000000 libfvde-20240113/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:34.000000 libfvde-20240113/libfvalue/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_filetime.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6310 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_libfwnt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_split_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6272 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2876 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_split_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_filetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_value_type.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_split_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_data_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_data_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_value_type.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_binary_data.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_value_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_table.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_libfguid.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2843 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_split_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_floating_point.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_libfdatetime.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_binary_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_value_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_table.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36935 2024-01-13 09:42:45.000000 libfvde-20240113/libfvalue/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84540 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_floating_point.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-01-13 09:42:27.000000 libfvde-20240113/libfvalue/libfvalue_libuna.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:33.000000 libfvde-20240113/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-01-13 09:42:17.000000 libfvde-20240113/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-01-13 09:42:17.000000 libfvde-20240113/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-01-13 09:42:17.000000 libfvde-20240113/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-01-13 09:42:17.000000 libfvde-20240113/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      728 2024-01-13 09:42:17.000000 libfvde-20240113/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-01-13 09:42:17.000000 libfvde-20240113/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-01-13 09:42:17.000000 libfvde-20240113/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-01-13 09:42:17.000000 libfvde-20240113/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-01-13 09:42:17.000000 libfvde-20240113/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-01-13 09:42:17.000000 libfvde-20240113/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-01-13 09:42:17.000000 libfvde-20240113/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31633 2024-01-13 09:42:44.000000 libfvde-20240113/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-01-13 09:42:17.000000 libfvde-20240113/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-01-13 09:42:17.000000 libfvde-20240113/libcnotify/libcnotify_print.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-01-13 10:25:33.000000 libfvde-20240113/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-01-13 09:42:13.000000 libfvde-20240113/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-01-13 09:42:13.000000 libfvde-20240113/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-01-13 09:42:13.000000 libfvde-20240113/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      640 2024-01-13 09:42:13.000000 libfvde-20240113/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-01-13 09:42:13.000000 libfvde-20240113/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-01-13 09:42:13.000000 libfvde-20240113/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-01-13 09:42:13.000000 libfvde-20240113/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-01-13 09:42:13.000000 libfvde-20240113/libcerror/libcerror_system.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-01-13 09:42:13.000000 libfvde-20240113/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-01-13 09:42:13.000000 libfvde-20240113/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-01-13 09:42:13.000000 libfvde-20240113/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31146 2024-01-13 09:42:44.000000 libfvde-20240113/libcerror/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56964 2024-01-13 09:42:40.000000 libfvde-20240113/aclocal.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8807 2024-01-13 09:19:22.000000 libfvde-20240113/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      415 2024-01-13 10:25:41.856414 libfvde-20240113/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:13.000000 libfvde-20240502/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_area.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_mapped_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4017 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1287 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_area.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_mapped_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_segments_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_segments_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35606 2024-05-02 05:25:46.000000 libfvde-20240502/libfdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2024-05-02 05:25:22.000000 libfvde-20240502/libfdata/libfdata_vector.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2024-05-02 04:50:54.000000 libfvde-20240502/COPYING
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2024-05-02 05:25:45.000000 libfvde-20240502/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 04:50:54.000000 libfvde-20240502/NEWS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2024-05-02 05:25:46.000000 libfvde-20240502/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:13.000000 libfvde-20240502/libfplist/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1401 2024-05-02 05:25:26.000000 libfvde-20240502/libfplist/libfplist_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-05-02 05:25:26.000000 libfvde-20240502/libfplist/libfplist_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5928 2024-05-02 05:25:26.000000 libfvde-20240502/libfplist/libfplist_xml_attribute.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1635 2024-05-02 05:25:26.000000 libfvde-20240502/libfplist/libfplist_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6651 2024-05-02 05:25:26.000000 libfvde-20240502/libfplist/libfplist_xml_scanner.l
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-05-02 05:25:26.000000 libfvde-20240502/libfplist/libfplist_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)  8431465 2024-05-02 05:26:43.000000 libfvde-20240502/libfplist/libfplist_xml_scanner.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56503 2024-05-02 05:26:43.000000 libfvde-20240502/libfplist/libfplist_xml_parser.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1492 2024-05-02 05:25:26.000000 libfvde-20240502/libfplist/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-02 05:25:26.000000 libfvde-20240502/libfplist/libfplist_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-02 05:25:26.000000 libfvde-20240502/libfplist/libfplist_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1788 2024-05-02 05:25:26.000000 libfvde-20240502/libfplist/libfplist_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1711 2024-05-02 05:25:26.000000 libfvde-20240502/libfplist/libfplist_xml_attribute.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-02 05:25:26.000000 libfvde-20240502/libfplist/libfplist_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-02 05:25:26.000000 libfvde-20240502/libfplist/libfplist_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1460 2024-05-02 05:25:26.000000 libfvde-20240502/libfplist/libfplist_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-02 05:25:26.000000 libfvde-20240502/libfplist/libfplist_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-05-02 05:25:26.000000 libfvde-20240502/libfplist/libfplist_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12481 2024-05-02 05:25:26.000000 libfvde-20240502/libfplist/libfplist_xml_parser.y
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4066 2024-05-02 05:26:43.000000 libfvde-20240502/libfplist/libfplist_xml_parser.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15149 2024-05-02 05:25:26.000000 libfvde-20240502/libfplist/libfplist_property_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3419 2024-05-02 05:25:26.000000 libfvde-20240502/libfplist/libfplist_property.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34608 2024-05-02 05:25:26.000000 libfvde-20240502/libfplist/libfplist_property.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15574 2024-05-02 05:25:26.000000 libfvde-20240502/libfplist/libfplist_xml_tag.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2497 2024-05-02 05:25:26.000000 libfvde-20240502/libfplist/libfplist_property_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-02 05:25:26.000000 libfvde-20240502/libfplist/libfplist_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1794 2024-05-02 05:25:26.000000 libfvde-20240502/libfplist/libfplist_libfvalue.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    36196 2024-05-02 05:25:46.000000 libfvde-20240502/libfplist/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2894 2024-05-02 05:25:26.000000 libfvde-20240502/libfplist/libfplist_xml_tag.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:13.000000 libfvde-20240502/libcaes/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-02 05:24:56.000000 libfvde-20240502/libcaes/libcaes_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2885 2024-05-02 05:24:56.000000 libfvde-20240502/libcaes/libcaes_tweaked_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4464 2024-05-02 05:24:56.000000 libfvde-20240502/libcaes/libcaes_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-02 05:24:56.000000 libfvde-20240502/libcaes/libcaes_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82616 2024-05-02 05:24:56.000000 libfvde-20240502/libcaes/libcaes_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1743 2024-05-02 05:24:56.000000 libfvde-20240502/libcaes/libcaes_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      734 2024-05-02 05:24:56.000000 libfvde-20240502/libcaes/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-02 05:24:56.000000 libfvde-20240502/libcaes/libcaes_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1608 2024-05-02 05:24:56.000000 libfvde-20240502/libcaes/libcaes_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-02 05:24:56.000000 libfvde-20240502/libcaes/libcaes_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-05-02 05:24:56.000000 libfvde-20240502/libcaes/libcaes_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-02 05:24:56.000000 libfvde-20240502/libcaes/libcaes_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-05-02 05:24:56.000000 libfvde-20240502/libcaes/libcaes_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31756 2024-05-02 05:25:45.000000 libfvde-20240502/libcaes/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33103 2024-05-02 05:24:56.000000 libfvde-20240502/libcaes/libcaes_tweaked_context.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:13.000000 libfvde-20240502/pyfvde/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1453 2024-05-02 04:50:59.000000 libfvde-20240502/pyfvde/pyfvde_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22664 2024-05-02 04:52:02.000000 libfvde-20240502/pyfvde/pyfvde_volume_group.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1355 2024-05-02 04:50:59.000000 libfvde-20240502/pyfvde/pyfvde_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16593 2024-05-02 04:50:59.000000 libfvde-20240502/pyfvde/pyfvde_datetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32378 2024-05-02 04:52:02.000000 libfvde-20240502/pyfvde/pyfvde_logical_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2527 2024-05-02 04:50:59.000000 libfvde-20240502/pyfvde/pyfvde_logical_volumes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8858 2024-05-02 04:50:59.000000 libfvde-20240502/pyfvde/pyfvde_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3713 2024-05-02 04:52:02.000000 libfvde-20240502/pyfvde/pyfvde_logical_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4960 2024-05-02 04:50:59.000000 libfvde-20240502/pyfvde/pyfvde_file_objects_io_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16283 2024-05-02 04:52:02.000000 libfvde-20240502/pyfvde/pyfvde.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1535 2024-05-02 04:50:59.000000 libfvde-20240502/pyfvde/pyfvde_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1508 2024-05-02 04:53:38.000000 libfvde-20240502/pyfvde/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      965 2024-05-02 04:50:59.000000 libfvde-20240502/pyfvde/pyfvde_libfvde.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1531 2024-05-02 04:50:59.000000 libfvde-20240502/pyfvde/pyfvde_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4160 2024-05-02 04:52:02.000000 libfvde-20240502/pyfvde/pyfvde_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2030 2024-05-02 04:50:59.000000 libfvde-20240502/pyfvde/pyfvde_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-02 04:50:59.000000 libfvde-20240502/pyfvde/pyfvde_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-05-02 04:52:02.000000 libfvde-20240502/pyfvde/pyfvde_guid.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33791 2024-05-02 04:50:59.000000 libfvde-20240502/pyfvde/pyfvde_file_object_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    63652 2024-05-02 04:52:02.000000 libfvde-20240502/pyfvde/pyfvde_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1815 2024-05-02 04:50:59.000000 libfvde-20240502/pyfvde/pyfvde_datetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2310 2024-05-02 04:50:59.000000 libfvde-20240502/pyfvde/pyfvde_physical_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10741 2024-05-02 04:52:02.000000 libfvde-20240502/pyfvde/pyfvde_physical_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3290 2024-05-02 04:52:02.000000 libfvde-20240502/pyfvde/pyfvde_volume_group.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-05-02 04:50:59.000000 libfvde-20240502/pyfvde/pyfvde_guid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2548 2024-05-02 04:50:59.000000 libfvde-20240502/pyfvde/pyfvde_physical_volumes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4080 2024-05-02 04:50:59.000000 libfvde-20240502/pyfvde/pyfvde_file_object_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9597 2024-05-02 04:50:59.000000 libfvde-20240502/pyfvde/pyfvde_logical_volumes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9659 2024-05-02 04:50:59.000000 libfvde-20240502/pyfvde/pyfvde_physical_volumes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-05-02 04:50:59.000000 libfvde-20240502/pyfvde/pyfvde_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    54522 2024-05-02 05:25:46.000000 libfvde-20240502/pyfvde/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1855 2024-05-02 04:50:59.000000 libfvde-20240502/pyfvde/pyfvde.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-05-02 04:50:59.000000 libfvde-20240502/pyfvde/pyfvde_file_objects_io_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-05-02 04:50:59.000000 libfvde-20240502/pyfvde/pyfvde_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-05-02 04:50:59.000000 libfvde-20240502/pyfvde/pyfvde_error.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:13.000000 libfvde-20240502/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-02 05:25:24.000000 libfvde-20240502/libfguid/libfguid_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1192 2024-05-02 05:25:24.000000 libfvde-20240502/libfguid/libfguid_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5688 2024-05-02 05:25:24.000000 libfvde-20240502/libfguid/libfguid_identifier.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-02 05:25:24.000000 libfvde-20240502/libfguid/libfguid_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      677 2024-05-02 05:25:24.000000 libfvde-20240502/libfguid/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-02 05:25:24.000000 libfvde-20240502/libfguid/libfguid_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-02 05:25:24.000000 libfvde-20240502/libfguid/libfguid_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1515 2024-05-02 05:25:24.000000 libfvde-20240502/libfguid/libfguid_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    67571 2024-05-02 05:25:24.000000 libfvde-20240502/libfguid/libfguid_identifier.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1134 2024-05-02 05:25:24.000000 libfvde-20240502/libfguid/libfguid_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2341 2024-05-02 05:25:24.000000 libfvde-20240502/libfguid/libfguid_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31407 2024-05-02 05:25:46.000000 libfvde-20240502/libfguid/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-02 05:25:24.000000 libfvde-20240502/libfguid/libfguid_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3650 2024-05-02 04:50:54.000000 libfvde-20240502/libfvde.spec.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:13.000000 libfvde-20240502/libfvde/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1132 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde.rc.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8260 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_sector_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_checksum.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1614 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1611 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2180 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4353 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_encryption_context_plist.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14533 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_password.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8407 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_logical_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7980 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_bit_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26590 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_volume_group.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1514 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_libfplist.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81729 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_logical_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1327 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_compression.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1900 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2214 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/fvde_metadata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2246 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_metadata_block.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1512 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_libcaes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3310 2024-05-02 04:54:04.000000 libfvde-20240502/libfvde/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2707 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_physical_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2847 2024-05-02 05:26:02.000000 libfvde-20240502/libfvde/libfvde_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2086 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1928 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_physical_volume_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1525 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1480 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_libhmac.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2811 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   168049 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_encrypted_metadata.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1943 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_sector_data.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1573 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_keyring.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1647 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17109 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_encryption_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2468 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_volume_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3213 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_checksum.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5033 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_physical_volume_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44991 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_encryption_context_plist.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4771 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_logical_volume_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1130 2024-05-02 05:26:02.000000 libfvde-20240502/libfvde/libfvde.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1805 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_password.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1987 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7458 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_volume_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4093 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12433 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_metadata_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    48684 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_deflate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10777 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9512 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_encrypted_metadata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1802 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3696 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/fvde_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1507 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1445 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4107 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_metadata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2020 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_segment_descriptor.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2683 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2146 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_huffman_tree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2484 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_encryption_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41300 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_metadata.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3526 2024-05-02 04:52:16.000000 libfvde-20240502/libfvde/libfvde_deflate.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2333 2024-05-02 04:52:16.000000 libfvde-20240502/libfvde/libfvde_bit_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1464 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1857 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_libfvalue.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1841 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4374 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_volume_group.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9373 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19712 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_logical_volume_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2965 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1769 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12569 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_huffman_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1469 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4975 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42823 2024-05-02 05:25:46.000000 libfvde-20240502/libfvde/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3194 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_keyring.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3202 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_volume_header.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122689 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22452 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_volume_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4578 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_segment_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11293 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_physical_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1842 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5703 2024-05-02 04:50:58.000000 libfvde-20240502/libfvde/libfvde_compression.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:12.000000 libfvde-20240502/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11734 2024-05-02 04:51:00.000000 libfvde-20240502/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-12-03 09:08:37.000000 libfvde-20240502/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9615 2024-05-02 04:51:00.000000 libfvde-20240502/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-12-03 09:08:37.000000 libfvde-20240502/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-12-03 09:08:37.000000 libfvde-20240502/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31495 2024-05-02 04:51:00.000000 libfvde-20240502/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-12-03 09:08:37.000000 libfvde-20240502/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-12-03 09:08:37.000000 libfvde-20240502/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8476 2024-05-02 04:51:00.000000 libfvde-20240502/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17383 2024-05-02 04:51:00.000000 libfvde-20240502/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7625 2024-05-02 04:51:00.000000 libfvde-20240502/m4/libcsplit.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14127 2024-05-02 04:51:00.000000 libfvde-20240502/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11362 2024-05-02 04:51:00.000000 libfvde-20240502/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2024-05-02 05:25:38.000000 libfvde-20240502/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2024-05-02 05:25:38.000000 libfvde-20240502/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15781 2024-05-02 04:51:00.000000 libfvde-20240502/m4/libfdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-12-03 09:08:37.000000 libfvde-20240502/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7058 2024-05-02 04:51:00.000000 libfvde-20240502/m4/libfuse.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2024-05-02 05:25:38.000000 libfvde-20240502/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-12-03 09:08:37.000000 libfvde-20240502/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6501 2024-05-02 04:51:00.000000 libfvde-20240502/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5886 2024-05-02 04:51:00.000000 libfvde-20240502/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5876 2024-05-02 04:51:00.000000 libfvde-20240502/m4/libfguid.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11923 2024-05-02 04:51:00.000000 libfvde-20240502/m4/libbfio.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8550 2024-05-02 04:51:00.000000 libfvde-20240502/m4/libhmac.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-12-03 09:08:37.000000 libfvde-20240502/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2024-05-02 05:25:38.000000 libfvde-20240502/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-12-03 09:08:37.000000 libfvde-20240502/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-12-03 09:08:37.000000 libfvde-20240502/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2024-05-02 05:25:38.000000 libfvde-20240502/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-12-03 09:08:36.000000 libfvde-20240502/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6476 2024-05-02 04:51:00.000000 libfvde-20240502/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27647 2024-05-02 04:51:00.000000 libfvde-20240502/m4/libcrypto.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20032 2024-05-02 04:51:00.000000 libfvde-20240502/m4/libfvalue.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-12-03 09:08:37.000000 libfvde-20240502/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7566 2024-05-02 04:51:00.000000 libfvde-20240502/m4/libfcache.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5093 2024-05-02 04:51:00.000000 libfvde-20240502/m4/pthread.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6709 2024-05-02 04:51:00.000000 libfvde-20240502/m4/libfplist.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7819 2024-05-02 04:51:00.000000 libfvde-20240502/m4/zlib.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6500 2024-05-02 04:51:00.000000 libfvde-20240502/m4/libcaes.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:12.000000 libfvde-20240502/include/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30542 2024-05-02 04:50:57.000000 libfvde-20240502/include/libfvde.h.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:12.000000 libfvde-20240502/include/libfvde/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1905 2024-05-02 04:50:57.000000 libfvde-20240502/include/libfvde/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1903 2024-05-02 05:26:01.000000 libfvde-20240502/include/libfvde/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5185 2024-05-02 04:50:57.000000 libfvde-20240502/include/libfvde/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5054 2024-05-02 05:26:02.000000 libfvde-20240502/include/libfvde/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1608 2024-05-02 04:50:57.000000 libfvde-20240502/include/libfvde/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2024-05-02 04:50:57.000000 libfvde-20240502/include/libfvde/error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1481 2024-05-02 04:50:57.000000 libfvde-20240502/include/libfvde/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2024-05-02 05:26:02.000000 libfvde-20240502/include/libfvde/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5264 2024-05-02 04:50:57.000000 libfvde-20240502/include/libfvde/codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      410 2024-05-02 04:52:32.000000 libfvde-20240502/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30542 2024-05-02 05:26:01.000000 libfvde-20240502/include/libfvde.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29764 2024-05-02 05:25:45.000000 libfvde-20240502/include/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:12.000000 libfvde-20240502/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      957 2024-05-02 04:50:57.000000 libfvde-20240502/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2024-05-02 04:50:57.000000 libfvde-20240502/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2024-05-02 04:50:57.000000 libfvde-20240502/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2024-05-02 04:50:57.000000 libfvde-20240502/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-02 04:50:57.000000 libfvde-20240502/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2024-05-02 04:50:57.000000 libfvde-20240502/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2024-05-02 04:50:57.000000 libfvde-20240502/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      343 2024-05-02 04:52:32.000000 libfvde-20240502/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2024-05-02 04:50:57.000000 libfvde-20240502/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7373 2024-05-02 05:26:02.000000 libfvde-20240502/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20135 2024-05-02 05:25:45.000000 libfvde-20240502/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21287 2024-05-02 05:26:02.000000 libfvde-20240502/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2024-05-02 04:50:57.000000 libfvde-20240502/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2024-05-02 04:50:57.000000 libfvde-20240502/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2024-05-02 04:50:57.000000 libfvde-20240502/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26817 2024-05-02 05:25:45.000000 libfvde-20240502/common/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:12.000000 libfvde-20240502/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2024-05-02 05:25:05.000000 libfvde-20240502/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2024-05-02 05:25:05.000000 libfvde-20240502/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      775 2024-05-02 05:25:05.000000 libfvde-20240502/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2024-05-02 05:25:05.000000 libfvde-20240502/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-02 05:25:05.000000 libfvde-20240502/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-02 05:25:05.000000 libfvde-20240502/libclocale/libclocale_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2024-05-02 05:25:05.000000 libfvde-20240502/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3142 2024-05-02 05:25:05.000000 libfvde-20240502/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2024-05-02 05:25:05.000000 libfvde-20240502/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2024-05-02 05:25:05.000000 libfvde-20240502/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32015 2024-05-02 05:25:46.000000 libfvde-20240502/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-02 05:25:05.000000 libfvde-20240502/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2024-05-02 05:25:05.000000 libfvde-20240502/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2024-05-02 05:25:05.000000 libfvde-20240502/libclocale/libclocale_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2466 2024-05-02 05:26:02.000000 libfvde-20240502/libfvde.spec
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:13.000000 libfvde-20240502/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-02 05:25:20.000000 libfvde-20240502/libfcache/libfcache_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2024-05-02 05:25:20.000000 libfvde-20240502/libfcache/libfcache_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2024-05-02 05:25:20.000000 libfvde-20240502/libfcache/libfcache_cache_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-02 05:25:20.000000 libfvde-20240502/libfcache/libfcache_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      876 2024-05-02 05:25:20.000000 libfvde-20240502/libfcache/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-02 05:25:20.000000 libfvde-20240502/libfcache/libfcache_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-02 05:25:20.000000 libfvde-20240502/libfcache/libfcache_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2024-05-02 05:25:20.000000 libfvde-20240502/libfcache/libfcache_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2024-05-02 05:25:20.000000 libfvde-20240502/libfcache/libfcache_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-02 05:25:20.000000 libfvde-20240502/libfcache/libfcache_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-02 05:25:20.000000 libfvde-20240502/libfcache/libfcache_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2024-05-02 05:25:20.000000 libfvde-20240502/libfcache/libfcache_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-02 05:25:20.000000 libfvde-20240502/libfcache/libfcache_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2024-05-02 05:25:20.000000 libfvde-20240502/libfcache/libfcache_cache_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32524 2024-05-02 05:25:46.000000 libfvde-20240502/libfcache/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2024-05-02 05:25:20.000000 libfvde-20240502/libfcache/libfcache_date_time.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2024-05-02 05:25:20.000000 libfvde-20240502/libfcache/libfcache_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2024-05-02 05:25:20.000000 libfvde-20240502/libfcache/libfcache_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2270 2024-05-02 04:54:44.000000 libfvde-20240502/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:13.000000 libfvde-20240502/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_file_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_file_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_file_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_file_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_file_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_file_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_memory_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_file_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_file_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_memory_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_memory_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35867 2024-05-02 05:25:45.000000 libfvde-20240502/libbfio/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_memory_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2024-05-02 05:24:54.000000 libfvde-20240502/libbfio/libbfio_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-12-03 09:08:35.000000 libfvde-20240502/ABOUT-NLS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49939 2024-05-02 05:25:45.000000 libfvde-20240502/config.guess
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:12.000000 libfvde-20240502/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2024-05-02 04:50:54.000000 libfvde-20240502/dpkg/libfvde-dev.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1024 2024-05-02 04:51:00.000000 libfvde-20240502/dpkg/copyright
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:12.000000 libfvde-20240502/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2024-05-02 04:50:54.000000 libfvde-20240502/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2136 2024-05-02 04:50:54.000000 libfvde-20240502/dpkg/control
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2024-05-02 04:50:54.000000 libfvde-20240502/dpkg/libfvde.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      761 2024-05-02 04:50:54.000000 libfvde-20240502/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      120 2024-05-02 04:50:54.000000 libfvde-20240502/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      139 2024-05-02 05:26:02.000000 libfvde-20240502/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2024-05-02 04:50:54.000000 libfvde-20240502/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       18 2024-05-02 04:50:54.000000 libfvde-20240502/dpkg/libfvde-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       27 2024-05-02 04:50:54.000000 libfvde-20240502/dpkg/libfvde-tools.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      483 2024-05-02 05:26:02.000000 libfvde-20240502/setup.cfg
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2024-05-02 04:50:54.000000 libfvde-20240502/COPYING.LESSER
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  2158758 2024-05-02 05:25:43.000000 libfvde-20240502/configure
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2024-05-02 05:25:45.000000 libfvde-20240502/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2024-05-02 05:25:45.000000 libfvde-20240502/missing
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/libfdata/libfdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvde_test_encrypted_metadata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6174 2024-05-02 04:51:47.000000 libfvde-20240502/msvscpp/fvde_test_encrypted_metadata/fvde_test_encrypted_metadata.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    44126 2024-05-02 04:51:47.000000 libfvde-20240502/msvscpp/libfvde.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvde_test_segment_descriptor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6092 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/fvde_test_segment_descriptor/fvde_test_segment_descriptor.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvde_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6714 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/fvde_test_support/fvde_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/zlib/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6068 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/zlib/zlib.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/libfplist/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6237 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/libfplist/libfplist.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvde_test_compression/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6071 2024-05-02 04:51:47.000000 libfvde-20240502/msvscpp/fvde_test_compression/fvde_test_compression.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/libcaes/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4777 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/libcaes/libcaes.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/pyfvde/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7522 2024-05-02 04:51:47.000000 libfvde-20240502/msvscpp/pyfvde/pyfvde.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/libfguid/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4631 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/libfguid/libfguid.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/libfvde/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11896 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/libfvde/libfvde.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvde_test_logical_volume/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6080 2024-05-02 04:51:47.000000 libfvde-20240502/msvscpp/fvde_test_logical_volume/fvde_test_logical_volume.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/libclocale/libclocale.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvde_test_tools_signal/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6001 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/fvde_test_tools_signal/fvde_test_tools_signal.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/libfcache/libfcache.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2319 2024-05-02 04:53:51.000000 libfvde-20240502/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/libbfio/libbfio.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvde_test_keyring/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6059 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/fvde_test_keyring/fvde_test_keyring.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvde_test_encryption_context/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6092 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/fvde_test_encryption_context/fvde_test_encryption_context.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvdewipekey/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6535 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/fvdewipekey/fvdewipekey.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvde_test_deflate/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5983 2024-05-02 04:51:47.000000 libfvde-20240502/msvscpp/fvde_test_deflate/fvde_test_deflate.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvde_test_physical_volume_descriptor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6116 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/fvde_test_physical_volume_descriptor/fvde_test_physical_volume_descriptor.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvde_test_logical_volume_descriptor/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6113 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/fvde_test_logical_volume_descriptor/fvde_test_logical_volume_descriptor.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvdeinfo/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7198 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/fvdeinfo/fvdeinfo.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvde_test_volume_data_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6092 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/fvde_test_volume_data_handle/fvde_test_volume_data_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvde_test_volume_header/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6324 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/fvde_test_volume_header/fvde_test_volume_header.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvde_test_metadata_block/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6080 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/fvde_test_metadata_block/fvde_test_metadata_block.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvde_test_io_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6065 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/fvde_test_io_handle/fvde_test_io_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvde_test_encryption_context_plist/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6110 2024-05-02 04:51:47.000000 libfvde-20240502/msvscpp/fvde_test_encryption_context_plist/fvde_test_encryption_context_plist.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/libcpath/libcpath.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvde_test_sector_data/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6071 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/fvde_test_sector_data/fvde_test_sector_data.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvde_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5810 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/fvde_test_error/fvde_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvde_test_checksum/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5902 2024-05-02 04:51:47.000000 libfvde-20240502/msvscpp/fvde_test_checksum/fvde_test_checksum.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvde_test_metadata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6062 2024-05-02 04:51:47.000000 libfvde-20240502/msvscpp/fvde_test_metadata/fvde_test_metadata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/libhmac/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5312 2024-05-02 04:51:47.000000 libfvde-20240502/msvscpp/libhmac/libhmac.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvde_test_physical_volume/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6083 2024-05-02 04:51:47.000000 libfvde-20240502/msvscpp/fvde_test_physical_volume/fvde_test_physical_volume.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvde_test_bit_stream/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6068 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/fvde_test_bit_stream/fvde_test_bit_stream.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/libcsplit/libcsplit.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvde_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5896 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/fvde_test_notify/fvde_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26126 2024-05-02 05:25:46.000000 libfvde-20240502/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7924 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/libfvalue/libfvalue.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvde_test_huffman_tree/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6074 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/fvde_test_huffman_tree/fvde_test_huffman_tree.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvde_test_volume/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6711 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/fvde_test_volume/fvde_test_volume.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvde_test_tools_output/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6001 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/fvde_test_tools_output/fvde_test_tools_output.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvde_test_volume_group/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6074 2024-05-02 04:51:47.000000 libfvde-20240502/msvscpp/fvde_test_volume_group/fvde_test_volume_group.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/msvscpp/fvdemount/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7925 2024-05-02 04:51:23.000000 libfvde-20240502/msvscpp/fvdemount/fvdemount.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      280 2024-05-02 04:52:16.000000 libfvde-20240502/AUTHORS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:12.000000 libfvde-20240502/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-02 05:25:03.000000 libfvde-20240502/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2024-05-02 05:25:03.000000 libfvde-20240502/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-02 05:25:03.000000 libfvde-20240502/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2024-05-02 05:25:03.000000 libfvde-20240502/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2024-05-02 05:25:03.000000 libfvde-20240502/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-05-02 05:25:03.000000 libfvde-20240502/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      938 2024-05-02 05:25:03.000000 libfvde-20240502/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2024-05-02 05:25:03.000000 libfvde-20240502/libcfile/libcfile_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-02 05:25:03.000000 libfvde-20240502/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2024-05-02 05:25:03.000000 libfvde-20240502/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-02 05:25:03.000000 libfvde-20240502/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-02 05:25:03.000000 libfvde-20240502/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-02 05:25:03.000000 libfvde-20240502/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-02 05:25:03.000000 libfvde-20240502/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2024-05-02 05:25:03.000000 libfvde-20240502/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-02 05:25:03.000000 libfvde-20240502/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2024-05-02 05:25:03.000000 libfvde-20240502/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32848 2024-05-02 05:25:46.000000 libfvde-20240502/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-02 05:25:03.000000 libfvde-20240502/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-02 05:25:03.000000 libfvde-20240502/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2024-05-02 05:25:03.000000 libfvde-20240502/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2024-05-02 05:25:03.000000 libfvde-20240502/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1981 2024-05-02 04:52:02.000000 libfvde-20240502/README
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2024-05-02 05:25:45.000000 libfvde-20240502/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:13.000000 libfvde-20240502/fvdetools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37242 2024-05-02 04:50:59.000000 libfvde-20240502/fvdetools/mount_dokan.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-05-02 04:50:59.000000 libfvde-20240502/fvdetools/fvdetools_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3051 2024-05-02 04:52:02.000000 libfvde-20240502/fvdetools/mount_file_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26512 2024-05-02 04:52:02.000000 libfvde-20240502/fvdetools/mount_fuse.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-05-02 04:52:02.000000 libfvde-20240502/fvdetools/info_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5483 2024-05-02 04:50:59.000000 libfvde-20240502/fvdetools/mount_dokan.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1312 2024-05-02 04:50:59.000000 libfvde-20240502/fvdetools/fvdetools_input.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1460 2024-05-02 04:50:59.000000 libfvde-20240502/fvdetools/fvdetools_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1570 2024-05-02 04:50:59.000000 libfvde-20240502/fvdetools/fvdetools_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1847 2024-05-02 04:50:59.000000 libfvde-20240502/fvdetools/fvdetools_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17296 2024-05-02 04:52:02.000000 libfvde-20240502/fvdetools/mount_file_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5795 2024-05-02 04:50:59.000000 libfvde-20240502/fvdetools/fvdetools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4003 2024-05-02 04:50:59.000000 libfvde-20240502/fvdetools/fvdetools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11856 2024-05-02 04:50:59.000000 libfvde-20240502/fvdetools/byte_size_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1475 2024-05-02 04:50:59.000000 libfvde-20240502/fvdetools/fvdetools_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1509 2024-05-02 04:50:59.000000 libfvde-20240502/fvdetools/fvdetools_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3410 2024-05-02 04:53:31.000000 libfvde-20240502/fvdetools/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1814 2024-05-02 04:50:59.000000 libfvde-20240502/fvdetools/fvdetools_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1549 2024-05-02 04:50:59.000000 libfvde-20240502/fvdetools/fvdetools_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1605 2024-05-02 04:50:59.000000 libfvde-20240502/fvdetools/fvdetools_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21090 2024-05-02 04:52:02.000000 libfvde-20240502/fvdetools/mount_file_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47235 2024-05-02 04:52:02.000000 libfvde-20240502/fvdetools/info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3661 2024-05-02 04:52:02.000000 libfvde-20240502/fvdetools/mount_file_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9020 2024-05-02 04:52:02.000000 libfvde-20240502/fvdetools/fvdeinfo.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1877 2024-05-02 04:50:59.000000 libfvde-20240502/fvdetools/fvdetools_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13497 2024-05-02 04:50:59.000000 libfvde-20240502/fvdetools/wipekey_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4249 2024-05-02 04:52:02.000000 libfvde-20240502/fvdetools/mount_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2491 2024-05-02 04:50:59.000000 libfvde-20240502/fvdetools/wipekey_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4600 2024-05-02 04:50:59.000000 libfvde-20240502/fvdetools/fvdetools_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1620 2024-05-02 04:50:59.000000 libfvde-20240502/fvdetools/fvdetools_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18374 2024-05-02 04:52:02.000000 libfvde-20240502/fvdetools/fvdemount.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33896 2024-05-02 04:52:02.000000 libfvde-20240502/fvdetools/mount_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6311 2024-05-02 04:50:59.000000 libfvde-20240502/fvdetools/fvdetools_input.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-02 04:50:59.000000 libfvde-20240502/fvdetools/fvdetools_signal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6998 2024-05-02 04:50:59.000000 libfvde-20240502/fvdetools/fvdewipekey.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1042 2024-05-02 04:50:59.000000 libfvde-20240502/fvdetools/fvdetools_libfvde.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    38885 2024-05-02 05:25:45.000000 libfvde-20240502/fvdetools/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1989 2024-05-02 04:50:59.000000 libfvde-20240502/fvdetools/byte_size_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1279 2024-05-02 04:50:59.000000 libfvde-20240502/fvdetools/fvdetools_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2024-05-02 04:50:59.000000 libfvde-20240502/fvdetools/fvdetools_output.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-05-02 04:52:02.000000 libfvde-20240502/fvdetools/mount_fuse.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:12.000000 libfvde-20240502/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/libcdata_btree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1123 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34761 2024-05-02 05:25:45.000000 libfvde-20240502/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-02 05:24:58.000000 libfvde-20240502/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       91 2024-05-02 04:50:54.000000 libfvde-20240502/pyproject.toml
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6860 2024-05-02 05:25:46.000000 libfvde-20240502/ylwrap
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      484 2024-05-02 04:50:54.000000 libfvde-20240502/setup.cfg.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35796 2024-05-02 05:25:45.000000 libfvde-20240502/config.sub
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     9278 2024-05-02 04:50:54.000000 libfvde-20240502/setup.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2024-05-02 04:52:02.000000 libfvde-20240502/acinclude.m4
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-12-03 09:08:35.000000 libfvde-20240502/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:12.000000 libfvde-20240502/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2024-05-02 05:25:17.000000 libfvde-20240502/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2024-05-02 05:25:17.000000 libfvde-20240502/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2024-05-02 05:25:17.000000 libfvde-20240502/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2024-05-02 05:25:17.000000 libfvde-20240502/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2024-05-02 05:25:17.000000 libfvde-20240502/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2024-05-02 05:25:17.000000 libfvde-20240502/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-02 05:25:17.000000 libfvde-20240502/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2024-05-02 05:25:17.000000 libfvde-20240502/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-05-02 05:25:17.000000 libfvde-20240502/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2024-05-02 05:25:17.000000 libfvde-20240502/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1167 2024-05-02 05:25:17.000000 libfvde-20240502/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2024-05-02 05:25:17.000000 libfvde-20240502/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2024-05-02 05:25:17.000000 libfvde-20240502/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2024-05-02 05:25:17.000000 libfvde-20240502/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2024-05-02 05:25:17.000000 libfvde-20240502/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2024-05-02 05:25:17.000000 libfvde-20240502/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2024-05-02 05:25:17.000000 libfvde-20240502/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2024-05-02 05:25:17.000000 libfvde-20240502/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2024-05-02 05:25:17.000000 libfvde-20240502/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2024-05-02 05:25:17.000000 libfvde-20240502/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-02 05:25:17.000000 libfvde-20240502/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2024-05-02 05:25:17.000000 libfvde-20240502/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2024-05-02 05:25:17.000000 libfvde-20240502/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2024-05-02 05:25:17.000000 libfvde-20240502/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2024-05-02 05:25:17.000000 libfvde-20240502/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2024-05-02 05:25:17.000000 libfvde-20240502/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2024-05-02 05:25:17.000000 libfvde-20240502/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35200 2024-05-02 05:25:46.000000 libfvde-20240502/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-05-02 05:25:17.000000 libfvde-20240502/libcthreads/libcthreads_queue.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2024-05-02 05:25:46.000000 libfvde-20240502/test-driver
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:12.000000 libfvde-20240502/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2024-05-02 05:25:11.000000 libfvde-20240502/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2024-05-02 05:25:11.000000 libfvde-20240502/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2024-05-02 05:25:11.000000 libfvde-20240502/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      838 2024-05-02 05:25:11.000000 libfvde-20240502/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2024-05-02 05:25:11.000000 libfvde-20240502/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2024-05-02 05:25:11.000000 libfvde-20240502/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2024-05-02 05:25:11.000000 libfvde-20240502/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2024-05-02 05:25:11.000000 libfvde-20240502/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-05-02 05:25:11.000000 libfvde-20240502/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2024-05-02 05:25:11.000000 libfvde-20240502/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-02 05:25:11.000000 libfvde-20240502/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2024-05-02 05:25:11.000000 libfvde-20240502/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32046 2024-05-02 05:25:46.000000 libfvde-20240502/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2024-05-02 05:25:11.000000 libfvde-20240502/libcpath/libcpath_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2024-05-02 05:25:11.000000 libfvde-20240502/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2024-05-02 05:25:11.000000 libfvde-20240502/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2024-05-02 05:25:11.000000 libfvde-20240502/libcpath/libcpath_path.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5202 2023-12-03 09:08:35.000000 libfvde-20240502/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10728 2024-05-02 05:00:38.000000 libfvde-20240502/manuals/libfvde.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      155 2024-05-02 04:53:15.000000 libfvde-20240502/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2263 2024-05-02 04:51:00.000000 libfvde-20240502/manuals/fvdeinfo.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1847 2024-05-02 04:51:00.000000 libfvde-20240502/manuals/fvdemount.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28806 2024-05-02 05:25:46.000000 libfvde-20240502/manuals/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/tests/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6782 2024-05-02 04:51:48.000000 libfvde-20240502/tests/fvde_test_sector_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)  6375570 2024-05-02 04:51:47.000000 libfvde-20240502/tests/fvde_test_encryption_context_plist.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8087 2024-05-02 04:51:47.000000 libfvde-20240502/tests/fvde_test_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5799 2024-05-02 04:51:00.000000 libfvde-20240502/tests/fvde_test_keyring.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15192 2024-05-02 04:51:00.000000 libfvde-20240502/tests/fvde_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8539 2024-05-02 04:51:00.000000 libfvde-20240502/tests/fvde_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4231 2024-05-02 04:51:00.000000 libfvde-20240502/tests/fvde_test_checksum.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      973 2024-05-02 04:51:00.000000 libfvde-20240502/tests/fvde_test_libfvde.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17533 2024-05-02 04:51:47.000000 libfvde-20240502/tests/fvde_test_logical_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2024-05-02 04:51:00.000000 libfvde-20240502/tests/fvde_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2024-05-02 04:51:00.000000 libfvde-20240502/tests/fvde_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1620 2024-05-02 04:52:23.000000 libfvde-20240502/tests/fvde_test_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20944 2024-05-02 04:52:02.000000 libfvde-20240502/tests/pyfvde_test_logical_volume.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12703 2024-05-02 04:51:47.000000 libfvde-20240502/tests/fvde_test_metadata.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4061 2024-05-02 04:59:13.000000 libfvde-20240502/tests/test_tools.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5531 2024-05-02 04:51:00.000000 libfvde-20240502/tests/fvde_test_compression.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1987 2024-05-02 04:51:00.000000 libfvde-20240502/tests/fvde_test_functions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21372 2024-05-02 04:52:02.000000 libfvde-20240502/tests/pyfvde_test_volume.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4531 2024-05-02 04:51:00.000000 libfvde-20240502/tests/fvde_test_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6904 2024-05-02 04:51:47.000000 libfvde-20240502/tests/fvde_test_logical_volume_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10240 2024-05-02 04:53:06.000000 libfvde-20240502/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15712 2024-05-02 04:51:00.000000 libfvde-20240502/tests/fvde_test_functions.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6385 2024-05-02 04:51:48.000000 libfvde-20240502/tests/fvde_test_segment_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1706 2024-05-02 04:51:00.000000 libfvde-20240502/tests/fvde_test_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2024-05-02 04:51:00.000000 libfvde-20240502/tests/fvde_test_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4653 2024-05-02 04:51:00.000000 libfvde-20240502/tests/fvde_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11058 2024-05-02 04:52:02.000000 libfvde-20240502/tests/pyfvde_test_volume_group.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   127481 2024-05-02 04:51:47.000000 libfvde-20240502/tests/fvde_test_encrypted_metadata.c
+-rwxr--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-02 04:50:59.000000 libfvde-20240502/tests/test_manpage.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4488 2024-05-02 04:58:48.000000 libfvde-20240502/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13622 2024-05-02 04:51:47.000000 libfvde-20240502/tests/fvde_test_bit_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3099 2024-05-02 04:51:00.000000 libfvde-20240502/tests/fvde_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100206 2024-05-02 04:51:00.000000 libfvde-20240502/tests/fvde_test_deflate.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7726 2024-05-02 04:51:48.000000 libfvde-20240502/tests/fvde_test_volume_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2425 2024-05-02 04:51:48.000000 libfvde-20240502/tests/fvde_test_tools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8968 2024-05-02 04:51:47.000000 libfvde-20240502/tests/fvde_test_physical_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8565 2024-05-02 04:52:02.000000 libfvde-20240502/tests/pyfvde_test_physical_volume.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33607 2024-05-02 04:51:00.000000 libfvde-20240502/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8109 2024-05-02 04:51:47.000000 libfvde-20240502/tests/fvde_test_metadata_block.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1691 2024-05-02 04:51:00.000000 libfvde-20240502/tests/fvde_test_memory.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3323 2024-05-02 04:50:59.000000 libfvde-20240502/tests/test_fvdeinfo.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2024-05-02 04:51:00.000000 libfvde-20240502/tests/fvde_test_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6960 2024-05-02 04:51:48.000000 libfvde-20240502/tests/fvde_test_physical_volume_descriptor.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3144 2024-05-02 04:52:02.000000 libfvde-20240502/tests/pyfvde_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30660 2024-05-02 04:51:47.000000 libfvde-20240502/tests/fvde_test_huffman_tree.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4276 2024-05-02 04:51:00.000000 libfvde-20240502/tests/fvde_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24384 2024-05-02 04:51:48.000000 libfvde-20240502/tests/fvde_test_volume_header.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4123 2024-05-02 04:51:48.000000 libfvde-20240502/tests/fvde_test_tools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    79106 2024-05-02 05:25:46.000000 libfvde-20240502/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-02 04:51:00.000000 libfvde-20240502/tests/fvde_test_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57129 2024-05-02 04:51:48.000000 libfvde-20240502/tests/fvde_test_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8921 2024-05-02 04:51:48.000000 libfvde-20240502/tests/fvde_test_volume_group.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-05-02 04:51:00.000000 libfvde-20240502/tests/fvde_test_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7263 2024-05-02 04:51:47.000000 libfvde-20240502/tests/fvde_test_encryption_context.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4391 2024-05-02 04:58:17.000000 libfvde-20240502/tests/test_library.sh
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3510 2024-05-02 04:50:58.000000 libfvde-20240502/ossfuzz/volume_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      897 2024-05-02 04:52:43.000000 libfvde-20240502/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-05-02 04:50:58.000000 libfvde-20240502/ossfuzz/ossfuzz_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34122 2024-05-02 05:25:46.000000 libfvde-20240502/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      967 2024-05-02 04:50:58.000000 libfvde-20240502/ossfuzz/ossfuzz_libfvde.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2024-05-02 05:25:38.000000 libfvde-20240502/ltmain.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      859 2024-05-02 04:50:54.000000 libfvde-20240502/libfvde.pc.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:13.000000 libfvde-20240502/libhmac/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    47989 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_sha1_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_sha224.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    50026 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_sha512_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14448 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_md5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2079 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_md5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1942 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9362 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14650 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_sha512.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45648 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_sha256_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_sha224.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1623 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2060 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_sha1.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3443 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_sha256_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1117 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    45605 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_sha224_context.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_md5_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14649 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_sha256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3368 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_sha1_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1185 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34911 2024-05-02 05:25:46.000000 libfvde-20240502/libhmac/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_sha256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3461 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_sha224_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3444 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_sha512_context.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2089 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_sha512.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1109 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14514 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_sha1.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40596 2024-05-02 05:25:29.000000 libfvde-20240502/libhmac/libhmac_md5_context.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:12.000000 libfvde-20240502/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2024-05-02 05:25:14.000000 libfvde-20240502/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2024-05-02 05:25:14.000000 libfvde-20240502/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2024-05-02 05:25:14.000000 libfvde-20240502/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2024-05-02 05:25:14.000000 libfvde-20240502/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-02 05:25:14.000000 libfvde-20240502/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      880 2024-05-02 05:25:14.000000 libfvde-20240502/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-02 05:25:14.000000 libfvde-20240502/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2024-05-02 05:25:14.000000 libfvde-20240502/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-02 05:25:14.000000 libfvde-20240502/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2024-05-02 05:25:14.000000 libfvde-20240502/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-02 05:25:14.000000 libfvde-20240502/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2024-05-02 05:25:14.000000 libfvde-20240502/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-02 05:25:14.000000 libfvde-20240502/libcsplit/libcsplit_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-02 05:25:14.000000 libfvde-20240502/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-02 05:25:14.000000 libfvde-20240502/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2024-05-02 05:25:14.000000 libfvde-20240502/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32943 2024-05-02 05:25:46.000000 libfvde-20240502/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2024-05-02 05:25:14.000000 libfvde-20240502/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2024-05-02 05:25:14.000000 libfvde-20240502/libcsplit/libcsplit_narrow_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:14.000000 libfvde-20240502/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-12-03 09:08:36.000000 libfvde-20240502/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-12-03 09:08:36.000000 libfvde-20240502/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-12-03 09:08:36.000000 libfvde-20240502/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-12-03 09:08:36.000000 libfvde-20240502/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-12-03 09:08:36.000000 libfvde-20240502/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-12-03 09:08:36.000000 libfvde-20240502/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-12-03 09:08:36.000000 libfvde-20240502/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-12-03 09:08:36.000000 libfvde-20240502/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-12-03 09:08:36.000000 libfvde-20240502/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1853 2024-05-02 05:26:01.000000 libfvde-20240502/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1852 2023-12-03 09:08:36.000000 libfvde-20240502/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-12-03 09:08:36.000000 libfvde-20240502/po/Rules-quot
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:12.000000 libfvde-20240502/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98308 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101450 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   156918 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4193 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20049 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16705 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19850 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8000 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    94606 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    58527 2024-05-02 05:25:46.000000 libfvde-20240502/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2024-05-02 05:25:32.000000 libfvde-20240502/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    42913 2024-05-02 05:25:45.000000 libfvde-20240502/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:13.000000 libfvde-20240502/libfvalue/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2913 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_filetime.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6390 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_libfwnt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   125143 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    20255 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10693 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3267 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14234 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_split_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3075 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_split_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1629 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_filetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1139 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1653 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2831 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_value_type.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13854 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_split_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5127 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_data_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1379 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40414 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_data_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    70736 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39827 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_value_type.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7448 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3264 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_binary_data.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1665 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_value_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1427 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3515 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_table.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1495 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_libfguid.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_split_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7626 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_floating_point.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_libfdatetime.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4451 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39905 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_binary_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4662 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_value_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1199 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32203 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_table.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37782 2024-05-02 05:25:46.000000 libfvde-20240502/libfvalue/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1417 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    84529 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_floating_point.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1964 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    73330 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2024-05-02 05:25:28.000000 libfvde-20240502/libfvalue/libfvalue_libuna.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:12.000000 libfvde-20240502/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2024-05-02 05:25:08.000000 libfvde-20240502/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2024-05-02 05:25:08.000000 libfvde-20240502/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2024-05-02 05:25:08.000000 libfvde-20240502/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2024-05-02 05:25:08.000000 libfvde-20240502/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      724 2024-05-02 05:25:08.000000 libfvde-20240502/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2024-05-02 05:25:08.000000 libfvde-20240502/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2024-05-02 05:25:08.000000 libfvde-20240502/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2024-05-02 05:25:08.000000 libfvde-20240502/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2024-05-02 05:25:08.000000 libfvde-20240502/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2024-05-02 05:25:08.000000 libfvde-20240502/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2024-05-02 05:25:08.000000 libfvde-20240502/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31884 2024-05-02 05:25:46.000000 libfvde-20240502/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2024-05-02 05:25:08.000000 libfvde-20240502/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2024-05-02 05:25:08.000000 libfvde-20240502/libcnotify/libcnotify_print.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2024-05-02 05:49:12.000000 libfvde-20240502/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2024-05-02 05:25:00.000000 libfvde-20240502/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2024-05-02 05:25:00.000000 libfvde-20240502/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2024-05-02 05:25:00.000000 libfvde-20240502/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      636 2024-05-02 05:25:00.000000 libfvde-20240502/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2024-05-02 05:25:00.000000 libfvde-20240502/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2024-05-02 05:25:00.000000 libfvde-20240502/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2024-05-02 05:25:00.000000 libfvde-20240502/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2024-05-02 05:25:00.000000 libfvde-20240502/libcerror/libcerror_system.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2024-05-02 05:25:00.000000 libfvde-20240502/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2024-05-02 05:25:00.000000 libfvde-20240502/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2024-05-02 05:25:00.000000 libfvde-20240502/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31351 2024-05-02 05:25:45.000000 libfvde-20240502/libcerror/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    56964 2024-05-02 05:25:41.000000 libfvde-20240502/aclocal.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8807 2024-05-02 04:50:54.000000 libfvde-20240502/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      415 2024-05-02 05:49:20.260634 libfvde-20240502/PKG-INFO
```

### Comparing `libfvde-20240113/libfdata/libfdata_error.h` & `libfvde-20240502/libfdata/libfdata_error.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_area.c` & `libfvde-20240502/libfdata/libfdata_area.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The area functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_stream.h` & `libfvde-20240502/libfdata/libfdata_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The stream functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_cache.h` & `libfvde-20240502/libfdata/libfdata_cache.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Cache functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_range_list.c` & `libfvde-20240502/libfdata/libfdata_range_list.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The range list functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_mapped_range.c` & `libfvde-20240502/libfdata/libfdata_mapped_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The (data) mapped range functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_libcerror.h` & `libfvde-20240502/libfdata/libfdata_libcerror.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_definitions.h` & `libfvde-20240502/libfdata/libfdata_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBFDATA )
 #include <libfdata/definitions.h>
 
 /* The definitions in <libfdata/definitions.h> are copied here
  * for local use of libfdata
  */
 #else
-#define LIBFDATA_VERSION						20230319
+#define LIBFDATA_VERSION						20240415
 
 /* The libfdata version string
  */
-#define LIBFDATA_VERSION_STRING						"20230319"
+#define LIBFDATA_VERSION_STRING						"20240415"
 
 /* The library flag definitions
  */
 enum LIBFDATA_FLAGS
 {
 	/* The data is not managed by the library
 	 */
```

### Comparing `libfvde-20240113/libfdata/libfdata_list.c` & `libfvde-20240502/libfdata/libfdata_list.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The list functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_libcdata.h` & `libfvde-20240502/libfdata/libfdata_libcdata.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcdata header wrapper
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_list.h` & `libfvde-20240502/libfdata/libfdata_list.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The list functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_list_element.h` & `libfvde-20240502/libfdata/libfdata_list_element.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The list element functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -93,14 +93,15 @@
 int libfdata_list_element_get_timestamp(
      libfdata_list_element_t *element,
      int64_t *timestamp,
      libcerror_error_t **error );
 
 /* Data range functions
  */
+LIBFDATA_EXTERN \
 int libfdata_list_element_get_data_range(
      libfdata_list_element_t *element,
      int *file_index,
      off64_t *offset,
      size64_t *size,
      uint32_t *flags,
      libcerror_error_t **error );
```

### Comparing `libfvde-20240113/libfdata/Makefile.am` & `libfvde-20240502/libfdata/Makefile.am`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 if HAVE_LOCAL_LIBFDATA
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCTHREADS_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBFCACHE_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
 
@@ -31,17 +31,17 @@
 	libfdata_stream.c libfdata_stream.h \
 	libfdata_support.c libfdata_support.h \
 	libfdata_types.h \
 	libfdata_unused.h \
 	libfdata_vector.c libfdata_vector.h
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
 	@echo "Running splint on libfdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdata_la_SOURCES)
```

### Comparing `libfvde-20240113/libfdata/libfdata_libcnotify.h` & `libfvde-20240502/libfdata/libfdata_libcnotify.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcnotify header wrapper
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_extern.h` & `libfvde-20240502/libfdata/libfdata_extern.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_notify.c` & `libfvde-20240502/libfdata/libfdata_notify.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Notification functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_cache.c` & `libfvde-20240502/libfdata/libfdata_cache.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Cache functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_stream.c` & `libfvde-20240502/libfdata/libfdata_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The stream functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_unused.h` & `libfvde-20240502/libfdata/libfdata_unused.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_range.h` & `libfvde-20240502/libfdata/libfdata_range.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The range functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_area.h` & `libfvde-20240502/libfdata/libfdata_area.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The area functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_error.c` & `libfvde-20240502/libfdata/libfdata_error.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_support.h` & `libfvde-20240502/libfdata/libfdata_support.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_range.c` & `libfvde-20240502/libfdata/libfdata_range.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The range functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_mapped_range.h` & `libfvde-20240502/libfdata/libfdata_mapped_range.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The (data) mapped range functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_support.c` & `libfvde-20240502/libfplist/libfplist_support.c`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2016-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -20,22 +20,22 @@
  */
 
 #include <common.h>
 #include <types.h>
 
 #include <stdio.h>
 
-#include "libfdata_definitions.h"
-#include "libfdata_support.h"
+#include "libfplist_definitions.h"
+#include "libfplist_support.h"
 
-#if !defined( HAVE_LOCAL_LIBFDATA )
+#if !defined( HAVE_LOCAL_LIBFPLIST )
 
 /* Returns the library version as a string
  */
-const char *libfdata_get_version(
+const char *libfplist_get_version(
              void )
 {
-	return( (const char *) LIBFDATA_VERSION_STRING );
+	return( (const char *) LIBFPLIST_VERSION_STRING );
 }
 
-#endif /* !defined( HAVE_LOCAL_LIBFDATA ) */
+#endif
```

### Comparing `libfvde-20240113/libfdata/libfdata_list_element.c` & `libfvde-20240502/libfdata/libfdata_list_element.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The list element functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_segments_array.c` & `libfvde-20240502/libfdata/libfdata_segments_array.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The segments array functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_types.h` & `libfvde-20240502/libfdata/libfdata_types.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_notify.h` & `libfvde-20240502/libfdata/libfdata_notify.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Notification functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_range_list.h` & `libfvde-20240502/libfdata/libfdata_range_list.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The range list functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_segments_array.h` & `libfvde-20240502/libfdata/libfdata_segments_array.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The segments array functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/Makefile.in` & `libfvde-20240502/libfdata/Makefile.in`

 * *Files 5% similar despite different names*

```diff
@@ -514,14 +514,16 @@
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
@@ -588,16 +590,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 @HAVE_LOCAL_LIBFDATA_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFDATA_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFDATA_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFDATA_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFDATA_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCTHREADS_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@LIBFCACHE_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFDATA_TRUE@	@PTHREAD_CPPFLAGS@ 
 
@@ -621,15 +623,16 @@
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_segments_array.c libfdata_segments_array.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_stream.c libfdata_stream.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_support.c libfdata_support.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_types.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_unused.h \
 @HAVE_LOCAL_LIBFDATA_TRUE@	libfdata_vector.c libfdata_vector.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -841,24 +844,39 @@
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
+		-rm -f ./$(DEPDIR)/libfdata_area.Plo
+	-rm -f ./$(DEPDIR)/libfdata_cache.Plo
+	-rm -f ./$(DEPDIR)/libfdata_error.Plo
+	-rm -f ./$(DEPDIR)/libfdata_list.Plo
+	-rm -f ./$(DEPDIR)/libfdata_list_element.Plo
+	-rm -f ./$(DEPDIR)/libfdata_mapped_range.Plo
+	-rm -f ./$(DEPDIR)/libfdata_notify.Plo
+	-rm -f ./$(DEPDIR)/libfdata_range.Plo
+	-rm -f ./$(DEPDIR)/libfdata_range_list.Plo
+	-rm -f ./$(DEPDIR)/libfdata_segments_array.Plo
+	-rm -f ./$(DEPDIR)/libfdata_stream.Plo
+	-rm -f ./$(DEPDIR)/libfdata_support.Plo
+	-rm -f ./$(DEPDIR)/libfdata_vector.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -928,14 +946,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -946,23 +966,22 @@
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
 	@echo "Running splint on libfdata ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfdata_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfvde-20240113/libfdata/libfdata_vector.c` & `libfvde-20240502/libfdata/libfdata_vector.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The vector functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_libfcache.h` & `libfvde-20240502/libfdata/libfdata_libfcache.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libfcache header wrapper
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfdata/libfdata_vector.h` & `libfvde-20240502/libfdata/libfdata_vector.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The vector functions
  *
- * Copyright (C) 2010-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/COPYING` & `libfvde-20240502/COPYING`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/install-sh` & `libfvde-20240502/install-sh`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/depcomp` & `libfvde-20240502/depcomp`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfplist/libfplist_libfguid.h` & `libfvde-20240502/libfplist/libfplist_libfguid.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libfguid header wrapper
  *
- * Copyright (C) 2016-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2016-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfplist/libfplist_libuna.h` & `libfvde-20240502/libfplist/libfplist_libuna.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libuna header wrapper
  *
- * Copyright (C) 2016-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2016-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfplist/libfplist_xml_attribute.c` & `libfvde-20240502/libfplist/libfplist_xml_attribute.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * XML attribute functions
  *
- * Copyright (C) 2016-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2016-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfplist/libfplist_types.h` & `libfvde-20240502/libfplist/libfplist_types.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2016-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2016-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfplist/libfplist_xml_scanner.l` & `libfvde-20240502/libfplist/libfplist_xml_scanner.l`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 %option noinput nounput noyylineno nounistd
 %option noyyalloc noyyrealloc noyyfree
 
 %{
 /*
  * XML scanner functions
  *
- * Copyright (C) 2016-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2016-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfplist/libfplist_support.h` & `libfvde-20240502/libfplist/libfplist_support.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2016-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2016-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfplist/libfplist_xml_scanner.c` & `libfvde-20240502/libfplist/libfplist_xml_scanner.c`

 * *Files 0% similar despite different names*

```diff
@@ -157967,15 +157967,15 @@
 #line 1 "libfplist_xml_scanner.l"
 #define YY_NO_INPUT 1
 #define YY_NO_UNISTD_H 1
 #line 7 "libfplist_xml_scanner.l"
 /*
  * XML scanner functions
  *
- * Copyright (C) 2016-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2016-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfplist/libfplist_xml_parser.c` & `libfvde-20240502/libfplist/libfplist_xml_parser.c`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 #define yychar          libfplist_xml_scanner_char
 
 /* First part of user prologue.  */
 
 /*
  * XML parser functions
  *
- * Copyright (C) 2016-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2016-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfplist/Makefile.am` & `libfvde-20240502/libfplist/Makefile.am`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 AM_LFLAGS = -Cf
 AM_YFLAGS = -d -v -l -p libfplist_xml_scanner_
 
 if HAVE_LOCAL_LIBFPLIST
 AM_CPPFLAGS = \
-	-I$(top_srcdir)/include \
-	-I$(top_srcdir)/common \
+	-I../include -I$(top_srcdir)/include \
+	-I../common -I$(top_srcdir)/common \
 	@LIBCERROR_CPPFLAGS@ \
 	@LIBCDATA_CPPFLAGS@ \
 	@LIBCNOTIFY_CPPFLAGS@ \
 	@LIBUNA_CPPFLAGS@ \
 	@LIBFGUID_CPPFLAGS@ \
 	@LIBFVALUE_CPPFLAGS@ 
 
@@ -40,23 +40,21 @@
 	libfplist_xml_tag.c libfplist_xml_tag.h
 endif
 
 EXTRA_DIST = \
 	libfplist_xml_parser.c libfplist_xml_parser.h \
 	libfplist_xml_scanner.c
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfplist_xml_parser.c \
+	libfplist_xml_parser.h \
+	libfplist_xml_parser.output \
+	libfplist_xml_scanner.c \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libfplist_xml_parser.c
-	-rm -f libfplist_xml_parser.h
-	-rm -f libfplist_xml_parser.output
-	-rm -f libfplist_xml_scanner.c
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfplist ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfplist_la_SOURCES)
```

### Comparing `libfvde-20240113/libfplist/libfplist_unused.h` & `libfvde-20240502/libfplist/libfplist_unused.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2016-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2016-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfplist/libfplist_error.h` & `libfvde-20240502/libfplist/libfplist_error.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2016-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2016-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfplist/libfplist_definitions.h` & `libfvde-20240502/libfplist/libfplist_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2016-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2016-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfplist/definitions.h> are copied here
  * for local use of libfplist
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFPLIST_VERSION			20231023
+#define LIBFPLIST_VERSION			20240415
 
 /* The version string
  */
-#define LIBFPLIST_VERSION_STRING		"20231023"
+#define LIBFPLIST_VERSION_STRING		"20240415"
 
 enum LIBFPLIST_VALUE_TYPES
 {
 	LIBFPLIST_VALUE_TYPE_UNKNOWN		= 0,
 	LIBFPLIST_VALUE_TYPE_ARRAY		= 1,
 	LIBFPLIST_VALUE_TYPE_BINARY_DATA	= 2,
 	LIBFPLIST_VALUE_TYPE_BOOLEAN		= 3,
```

### Comparing `libfvde-20240113/libfplist/libfplist_xml_attribute.h` & `libfvde-20240502/libfplist/libfplist_xml_attribute.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * XML attribute functions
  *
- * Copyright (C) 2016-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2016-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfplist/libfplist_libcdata.h` & `libfvde-20240502/libfplist/libfplist_libcdata.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcdata header wrapper
  *
- * Copyright (C) 2016-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2016-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfplist/libfplist_error.c` & `libfvde-20240502/libfplist/libfplist_error.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2016-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2016-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfplist/libfplist_libcnotify.h` & `libfvde-20240502/libfplist/libfplist_libcnotify.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcnotify header
  *
- * Copyright (C) 2016-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2016-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfplist/libfplist_libcerror.h` & `libfvde-20240502/libcaes/libcaes_libcerror.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2016-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBFPLIST_LIBCERROR_H )
-#define _LIBFPLIST_LIBCERROR_H
+#if !defined( _LIBCAES_LIBCERROR_H )
+#define _LIBCAES_LIBCERROR_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCERROR for local use of libcerror
  */
 #if defined( HAVE_LOCAL_LIBCERROR )
 
@@ -42,9 +42,9 @@
 #define LIBCERROR_DLL_IMPORT
 #endif
 
 #include <libcerror.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCERROR ) */
 
-#endif /* !defined( _LIBFPLIST_LIBCERROR_H ) */
+#endif /* !defined( _LIBCAES_LIBCERROR_H ) */
```

### Comparing `libfvde-20240113/libfplist/libfplist_support.c` & `libfvde-20240502/libfguid/libfguid_support.c`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2016-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -20,22 +20,22 @@
  */
 
 #include <common.h>
 #include <types.h>
 
 #include <stdio.h>
 
-#include "libfplist_definitions.h"
-#include "libfplist_support.h"
+#include "libfguid_definitions.h"
+#include "libfguid_support.h"
 
-#if !defined( HAVE_LOCAL_LIBFPLIST )
+#if !defined( HAVE_LOCAL_LIBFGUID )
 
 /* Returns the library version as a string
  */
-const char *libfplist_get_version(
+const char *libfguid_get_version(
              void )
 {
-	return( (const char *) LIBFPLIST_VERSION_STRING );
+	return( (const char *) LIBFGUID_VERSION_STRING );
 }
 
 #endif
```

### Comparing `libfvde-20240113/libfplist/libfplist_xml_parser.y` & `libfvde-20240502/libfplist/libfplist_xml_parser.y`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 %{
 /*
  * XML parser functions
  *
- * Copyright (C) 2016-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2016-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfplist/libfplist_xml_parser.h` & `libfvde-20240502/libfplist/libfplist_xml_parser.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfplist/libfplist_property_list.c` & `libfvde-20240502/libfplist/libfplist_property_list.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Property list functions
  *
- * Copyright (C) 2016-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2016-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfplist/libfplist_property.h` & `libfvde-20240502/libfplist/libfplist_property.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Property functions
  *
- * Copyright (C) 2016-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2016-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfplist/libfplist_property.c` & `libfvde-20240502/libfplist/libfplist_property.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Property functions
  *
- * Copyright (C) 2016-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2016-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfplist/libfplist_xml_tag.c` & `libfvde-20240502/libfplist/libfplist_xml_tag.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * XML tag functions
  *
- * Copyright (C) 2016-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2016-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfplist/libfplist_property_list.h` & `libfvde-20240502/libfplist/libfplist_property_list.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Property list functions
  *
- * Copyright (C) 2016-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2016-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfplist/libfplist_extern.h` & `libfvde-20240502/libfplist/libfplist_extern.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2016-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2016-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfplist/libfplist_libfvalue.h` & `libfvde-20240502/libfplist/libfplist_libfvalue.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libfvalue header wrapper
  *
- * Copyright (C) 2016-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2016-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfplist/Makefile.in` & `libfvde-20240502/libfplist/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -526,14 +526,16 @@
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
@@ -602,16 +604,16 @@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
 AM_LFLAGS = -Cf
 AM_YFLAGS = -d -v -l -p libfplist_xml_scanner_
 @HAVE_LOCAL_LIBFPLIST_TRUE@AM_CPPFLAGS = \
-@HAVE_LOCAL_LIBFPLIST_TRUE@	-I$(top_srcdir)/include \
-@HAVE_LOCAL_LIBFPLIST_TRUE@	-I$(top_srcdir)/common \
+@HAVE_LOCAL_LIBFPLIST_TRUE@	-I../include -I$(top_srcdir)/include \
+@HAVE_LOCAL_LIBFPLIST_TRUE@	-I../common -I$(top_srcdir)/common \
 @HAVE_LOCAL_LIBFPLIST_TRUE@	@LIBCERROR_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFPLIST_TRUE@	@LIBCDATA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFPLIST_TRUE@	@LIBCNOTIFY_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFPLIST_TRUE@	@LIBUNA_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFPLIST_TRUE@	@LIBFGUID_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFPLIST_TRUE@	@LIBFVALUE_CPPFLAGS@ 
 
@@ -641,15 +643,20 @@
 @HAVE_LOCAL_LIBFPLIST_TRUE@	libfplist_xml_scanner.l \
 @HAVE_LOCAL_LIBFPLIST_TRUE@	libfplist_xml_tag.c libfplist_xml_tag.h
 
 EXTRA_DIST = \
 	libfplist_xml_parser.c libfplist_xml_parser.h \
 	libfplist_xml_scanner.c
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfplist_xml_parser.c \
+	libfplist_xml_parser.h \
+	libfplist_xml_parser.output \
+	libfplist_xml_scanner.c \
+	Makefile \
 	Makefile.in
 
 all: $(BUILT_SOURCES)
 	$(MAKE) $(AM_MAKEFLAGS) all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .l .lo .o .obj .y
@@ -869,28 +876,38 @@
 mostlyclean-generic:
 
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
 	-rm -f libfplist_xml_parser.c
 	-rm -f libfplist_xml_parser.h
 	-rm -f libfplist_xml_scanner.c
 	-test -z "$(BUILT_SOURCES)" || rm -f $(BUILT_SOURCES)
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-generic clean-libtool clean-noinstLTLIBRARIES \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ./$(DEPDIR)/libfplist_error.Plo
+	-rm -f ./$(DEPDIR)/libfplist_property.Plo
+	-rm -f ./$(DEPDIR)/libfplist_property_list.Plo
+	-rm -f ./$(DEPDIR)/libfplist_support.Plo
+	-rm -f ./$(DEPDIR)/libfplist_xml_attribute.Plo
+	-rm -f ./$(DEPDIR)/libfplist_xml_parser.Plo
+	-rm -f ./$(DEPDIR)/libfplist_xml_scanner.Plo
+	-rm -f ./$(DEPDIR)/libfplist_xml_tag.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -981,21 +998,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libfplist_xml_parser.c
-	-rm -f libfplist_xml_parser.h
-	-rm -f libfplist_xml_parser.output
-	-rm -f libfplist_xml_scanner.c
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfplist ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfplist_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfvde-20240113/libfplist/libfplist_xml_tag.h` & `libfvde-20240502/libfplist/libfplist_xml_tag.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * XML tag functions
  *
- * Copyright (C) 2016-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2016-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libcaes/libcaes_unused.h` & `libfvde-20240502/libcaes/libcaes_unused.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libcaes/libcaes_tweaked_context.h` & `libfvde-20240502/libcaes/libcaes_tweaked_context.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * AES tweaked de/encryption context functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libcaes/libcaes_context.h` & `libfvde-20240502/libcaes/libcaes_context.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * AES de/encryption context functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libcaes/libcaes_error.c` & `libfvde-20240502/libcaes/libcaes_error.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libcaes/libcaes_context.c` & `libfvde-20240502/libcaes/libcaes_context.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * AES de/encryption context functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libcaes/libcaes_definitions.h` & `libfvde-20240502/libcaes/libcaes_definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -30,19 +30,19 @@
 #if !defined( HAVE_LOCAL_LIBCAES )
 #include <libcaes/definitions.h>
 
 /* The definitions in <libcaes/definitions.h> are copied here
  * for local use of libcaes
  */
 #else
-#define LIBCAES_VERSION				20231120
+#define LIBCAES_VERSION				20240413
 
 /* The libcaes version string
  */
-#define LIBCAES_VERSION_STRING			"20231120"
+#define LIBCAES_VERSION_STRING			"20240413"
 
 /* The crypt modes
  */
 enum LIBCAES_CRYPT_MODES
 {
 	LIBCAES_CRYPT_MODE_DECRYPT		= 0,
 	LIBCAES_CRYPT_MODE_ENCRYPT		= 1
```

### Comparing `libfvde-20240113/libcaes/Makefile.am` & `libfvde-20240502/libcaes/Makefile.am`

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

### Comparing `libfvde-20240113/libcaes/libcaes_error.h` & `libfvde-20240502/libcaes/libcaes_error.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libcaes/libcaes_types.h` & `libfvde-20240502/libcaes/libcaes_types.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libcaes/libcaes_extern.h` & `libfvde-20240502/libcaes/libcaes_extern.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libcaes/libcaes_support.h` & `libfvde-20240502/libcaes/libcaes_support.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libcaes/libcaes_libcerror.h` & `libfvde-20240502/libcdata/libcdata_libcerror.h`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2006-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBCAES_LIBCERROR_H )
-#define _LIBCAES_LIBCERROR_H
+#if !defined( _LIBCDATA_LIBCERROR_H )
+#define _LIBCDATA_LIBCERROR_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCERROR for local use of libcerror
  */
 #if defined( HAVE_LOCAL_LIBCERROR )
 
@@ -42,9 +42,9 @@
 #define LIBCERROR_DLL_IMPORT
 #endif
 
 #include <libcerror.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCERROR ) */
 
-#endif /* !defined( _LIBCAES_LIBCERROR_H ) */
+#endif /* !defined( _LIBCDATA_LIBCERROR_H ) */
```

### Comparing `libfvde-20240113/libcaes/libcaes_support.c` & `libfvde-20240502/libcaes/libcaes_support.c`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libcaes/Makefile.in` & `libfvde-20240502/libcaes/Makefile.in`

 * *Files 1% similar despite different names*

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
@@ -564,31 +566,33 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -791,24 +795,30 @@
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
 
@@ -895,17 +905,14 @@
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

### Comparing `libfvde-20240113/libcaes/libcaes_tweaked_context.c` & `libfvde-20240502/libcaes/libcaes_tweaked_context.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * AES encryption functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/pyfvde/pyfvde_libclocale.h` & `libfvde-20240502/pyfvde/pyfvde_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/pyfvde_volume_group.c` & `libfvde-20240502/pyfvde/pyfvde_volume_group.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/pyfvde_libfguid.h` & `libfvde-20240502/pyfvde/pyfvde_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/pyfvde_datetime.c` & `libfvde-20240502/pyfvde/pyfvde_datetime.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/pyfvde_logical_volume.c` & `libfvde-20240502/pyfvde/pyfvde_logical_volume.c`

 * *Files 1% similar despite different names*

```diff
@@ -44,22 +44,22 @@
 	  "unlock() -> Boolean\n"
 	  "\n"
 	  "Unlocks the logical volume." },
 
 	{ "read_buffer",
 	  (PyCFunction) pyfvde_logical_volume_read_buffer,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read_buffer(size) -> Binary string\n"
+	  "read_buffer(size)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data." },
 
 	{ "read_buffer_at_offset",
 	  (PyCFunction) pyfvde_logical_volume_read_buffer_at_offset,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read_buffer_at_offset(size, offset) -> Binary string\n"
+	  "read_buffer_at_offset(size, offset)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data at a specific offset." },
 
 	{ "seek_offset",
 	  (PyCFunction) pyfvde_logical_volume_seek_offset,
 	  METH_VARARGS | METH_KEYWORDS,
 	  "seek_offset(offset, whence) -> None\n"
@@ -72,15 +72,15 @@
 	  "get_offset() -> Integer\n"
 	  "\n"
 	  "Retrieves the current offset of the data." },
 
 	{ "read",
 	  (PyCFunction) pyfvde_logical_volume_read_buffer,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read(size) -> Binary string\n"
+	  "read(size)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of data." },
 
 	{ "seek",
 	  (PyCFunction) pyfvde_logical_volume_seek_offset,
 	  METH_VARARGS | METH_KEYWORDS,
 	  "seek(offset, whence) -> None\n"
```

### Comparing `libfvde-20240113/pyfvde/pyfvde_logical_volumes.h` & `libfvde-20240502/pyfvde/pyfvde_logical_volumes.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/pyfvde_integer.c` & `libfvde-20240502/pyfvde/pyfvde_integer.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/pyfvde_logical_volume.h` & `libfvde-20240502/pyfvde/pyfvde_logical_volume.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/pyfvde_file_objects_io_pool.c` & `libfvde-20240502/pyfvde/pyfvde_file_objects_io_pool.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/pyfvde.c` & `libfvde-20240502/pyfvde/pyfvde.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/pyfvde_integer.h` & `libfvde-20240502/pyfvde/pyfvde_integer.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/Makefile.am` & `libfvde-20240502/pyfvde/Makefile.am`

 * *Files 9% similar despite different names*

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
@@ -50,13 +50,11 @@
 	@LIBFGUID_LIBADD@
 
 pyfvde_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 pyfvde_la_LDFLAGS  = -module -avoid-version $(PYTHON_LDFLAGS)
 
 endif
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f Makefile
-
```

### Comparing `libfvde-20240113/pyfvde/pyfvde_libfvde.h` & `libfvde-20240502/pyfvde/pyfvde_libfvde.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/pyfvde_error.h` & `libfvde-20240502/pyfvde/pyfvde_error.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/pyfvde_volume.h` & `libfvde-20240502/pyfvde/pyfvde_volume.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/pyfvde_python.h` & `libfvde-20240502/pyfvde/pyfvde_python.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/pyfvde_libcerror.h` & `libfvde-20240502/pyfvde/pyfvde_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/pyfvde_guid.c` & `libfvde-20240502/pyfvde/pyfvde_guid.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/pyfvde_file_object_io_handle.c` & `libfvde-20240502/pyfvde/pyfvde_file_object_io_handle.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/pyfvde_volume.c` & `libfvde-20240502/pyfvde/pyfvde_volume.c`

 * *Files 0% similar despite different names*

```diff
@@ -119,22 +119,22 @@
 	  "unlock() -> Boolean\n"
 	  "\n"
 	  "Unlocks the volume." },
 
 	{ "read_buffer",
 	  (PyCFunction) pyfvde_volume_read_buffer,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read_buffer(size) -> Binary string\n"
+	  "read_buffer(size)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of volume data." },
 
 	{ "read_buffer_at_offset",
 	  (PyCFunction) pyfvde_volume_read_buffer_at_offset,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read_buffer_at_offset(size, offset) -> Binary string\n"
+	  "read_buffer_at_offset(size, offset)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of volume data at a specific offset." },
 
 	{ "seek_offset",
 	  (PyCFunction) pyfvde_volume_seek_offset,
 	  METH_VARARGS | METH_KEYWORDS,
 	  "seek_offset(offset, whence) -> None\n"
@@ -149,15 +149,15 @@
 	  "Retrieved the current offset within the volume data." },
 
 	/* Some Pythonesque aliases */
 
 	{ "read",
 	  (PyCFunction) pyfvde_volume_read_buffer,
 	  METH_VARARGS | METH_KEYWORDS,
-	  "read(size) -> Binary string\n"
+	  "read(size)-> Bytes\n"
 	  "\n"
 	  "Reads a buffer of volume data." },
 
 	{ "seek",
 	  (PyCFunction) pyfvde_volume_seek_offset,
 	  METH_VARARGS | METH_KEYWORDS,
 	  "seek(offset, whence) -> None\n"
```

### Comparing `libfvde-20240113/pyfvde/pyfvde_datetime.h` & `libfvde-20240502/pyfvde/pyfvde_datetime.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/pyfvde_physical_volume.h` & `libfvde-20240502/pyfvde/pyfvde_physical_volume.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/pyfvde_physical_volume.c` & `libfvde-20240502/pyfvde/pyfvde_physical_volume.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/pyfvde_volume_group.h` & `libfvde-20240502/pyfvde/pyfvde_volume_group.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/pyfvde_guid.h` & `libfvde-20240502/pyfvde/pyfvde_guid.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/pyfvde_physical_volumes.h` & `libfvde-20240502/pyfvde/pyfvde_physical_volumes.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/pyfvde_file_object_io_handle.h` & `libfvde-20240502/pyfvde/pyfvde_file_object_io_handle.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/pyfvde_logical_volumes.c` & `libfvde-20240502/pyfvde/pyfvde_logical_volumes.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/pyfvde_physical_volumes.c` & `libfvde-20240502/pyfvde/pyfvde_physical_volumes.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/pyfvde_unused.h` & `libfvde-20240502/pyfvde/pyfvde_unused.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/Makefile.in` & `libfvde-20240502/pyfvde/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -549,14 +549,16 @@
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
@@ -623,16 +625,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -673,15 +675,16 @@
 @HAVE_PYTHON_TRUE@	@LIBCFILE_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBCPATH_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBBFIO_LIBADD@ \
 @HAVE_PYTHON_TRUE@	@LIBFGUID_LIBADD@
 
 @HAVE_PYTHON_TRUE@pyfvde_la_CPPFLAGS = $(PYTHON_CPPFLAGS)
 @HAVE_PYTHON_TRUE@pyfvde_la_LDFLAGS = -module -avoid-version $(PYTHON_LDFLAGS)
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -1011,24 +1014,39 @@
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
+		-rm -f ./$(DEPDIR)/pyfvde_la-pyfvde.Plo
+	-rm -f ./$(DEPDIR)/pyfvde_la-pyfvde_datetime.Plo
+	-rm -f ./$(DEPDIR)/pyfvde_la-pyfvde_error.Plo
+	-rm -f ./$(DEPDIR)/pyfvde_la-pyfvde_file_object_io_handle.Plo
+	-rm -f ./$(DEPDIR)/pyfvde_la-pyfvde_file_objects_io_pool.Plo
+	-rm -f ./$(DEPDIR)/pyfvde_la-pyfvde_guid.Plo
+	-rm -f ./$(DEPDIR)/pyfvde_la-pyfvde_integer.Plo
+	-rm -f ./$(DEPDIR)/pyfvde_la-pyfvde_logical_volume.Plo
+	-rm -f ./$(DEPDIR)/pyfvde_la-pyfvde_logical_volumes.Plo
+	-rm -f ./$(DEPDIR)/pyfvde_la-pyfvde_physical_volume.Plo
+	-rm -f ./$(DEPDIR)/pyfvde_la-pyfvde_physical_volumes.Plo
+	-rm -f ./$(DEPDIR)/pyfvde_la-pyfvde_volume.Plo
+	-rm -f ./$(DEPDIR)/pyfvde_la-pyfvde_volume_group.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1125,13 +1143,10 @@
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

### Comparing `libfvde-20240113/pyfvde/pyfvde.h` & `libfvde-20240502/pyfvde/pyfvde.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/pyfvde_file_objects_io_pool.h` & `libfvde-20240502/pyfvde/pyfvde_file_objects_io_pool.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/pyfvde_libbfio.h` & `libfvde-20240502/pyfvde/pyfvde_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/pyfvde/pyfvde_error.c` & `libfvde-20240502/pyfvde/pyfvde_error.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfguid/libfguid_error.c` & `libfvde-20240502/libfguid/libfguid_error.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfguid/libfguid_support.h` & `libfvde-20240502/libfguid/libfguid_support.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfguid/libfguid_identifier.h` & `libfvde-20240502/libfguid/libfguid_identifier.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Global (or Universal) Unique Identifier (GUID/UUID) functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfguid/libfguid_libcerror.h` & `libfvde-20240502/libfguid/libfguid_libcerror.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfguid/Makefile.am` & `libfvde-20240502/libfguid/Makefile.am`

 * *Files 16% similar despite different names*

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
@@ -13,17 +13,17 @@
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
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libfguid ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfguid_la_SOURCES)
```

### Comparing `libfvde-20240113/libfguid/libfguid_unused.h` & `libfvde-20240502/libfguid/libfguid_unused.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfguid/libfguid_extern.h` & `libfvde-20240502/libfguid/libfguid_extern.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfguid/libfguid_types.h` & `libfvde-20240502/libfguid/libfguid_types.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfguid/libfguid_identifier.c` & `libfvde-20240502/libfguid/libfguid_identifier.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * GUID functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfguid/libfguid_support.c` & `libfvde-20240502/libfvalue/libfvalue_support.c`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -20,22 +20,22 @@
  */
 
 #include <common.h>
 #include <types.h>
 
 #include <stdio.h>
 
-#include "libfguid_definitions.h"
-#include "libfguid_support.h"
+#include "libfvalue_definitions.h"
+#include "libfvalue_support.h"
 
-#if !defined( HAVE_LOCAL_LIBFGUID )
+#if !defined( HAVE_LOCAL_LIBFVALUE )
 
 /* Returns the library version as a string
  */
-const char *libfguid_get_version(
+const char *libfvalue_get_version(
              void )
 {
-	return( (const char *) LIBFGUID_VERSION_STRING );
+	return( (const char *) LIBFVALUE_VERSION_STRING );
 }
 
 #endif
```

### Comparing `libfvde-20240113/libfguid/libfguid_definitions.h` & `libfvde-20240502/libfguid/libfguid_definitions.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfguid/definitions.h> are copied here
  * for local use of libfguid
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFGUID_VERSION					20220113
+#define LIBFGUID_VERSION					20240415
 
 /* The version string
  */
-#define LIBFGUID_VERSION_STRING					"20220113"
+#define LIBFGUID_VERSION_STRING					"20240415"
 
 /* The byte order definitions
  */
 #define LIBFGUID_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define LIBFGUID_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The GUID identifier version definitions
```

### Comparing `libfvde-20240113/libfguid/Makefile.in` & `libfvde-20240502/libfguid/Makefile.in`

 * *Files 1% similar despite different names*

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
@@ -564,30 +566,31 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -789,24 +792,29 @@
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
 
@@ -866,14 +874,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -884,23 +894,22 @@
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
 	@echo "Running splint on libfguid ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfguid_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfvde-20240113/libfguid/libfguid_error.h` & `libfvde-20240502/libfguid/libfguid_error.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvde.spec.in` & `libfvde-20240502/libfvde.spec.in`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde.rc.in` & `libfvde-20240502/libfvde/libfvde.rc.in`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_sector_data.c` & `libfvde-20240502/libfvde/libfvde_sector_data.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_checksum.h` & `libfvde-20240502/libfvde/libfvde_checksum.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_libcdata.h` & `libfvde-20240502/libfvde/libfvde_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_libfdata.h` & `libfvde-20240502/libfvde/libfvde_libfdata.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_types.h` & `libfvde-20240502/libfvde/libfvde_types.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_encryption_context_plist.h` & `libfvde-20240502/libfvde/libfvde_encryption_context_plist.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_password.c` & `libfvde-20240502/libfvde/libfvde_password.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_logical_volume.h` & `libfvde-20240502/libfvde/libfvde_logical_volume.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_bit_stream.c` & `libfvde-20240502/libfvde/libfvde_bit_stream.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_volume_group.c` & `libfvde-20240502/libfvde/libfvde_volume_group.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_libfplist.h` & `libfvde-20240502/libfvde/libfvde_libfplist.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_logical_volume.c` & `libfvde-20240502/libfvde/libfvde_logical_volume.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_compression.h` & `libfvde-20240502/libfvde/libfvde_compression.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde.c` & `libfvde-20240502/libfvde/libfvde.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/fvde_metadata.h` & `libfvde-20240502/libfvde/fvde_metadata.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_metadata_block.h` & `libfvde-20240502/libfvde/libfvde_metadata_block.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_libcaes.h` & `libfvde-20240502/libfvde/libfvde_libcaes.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/Makefile.am` & `libfvde-20240502/libfvde/Makefile.am`

 * *Files 9% similar despite different names*

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
@@ -102,21 +102,19 @@
 libfvde_la_LDFLAGS = -no-undefined -version-info 1:0:0
 
 EXTRA_DIST = \
 	libfvde_definitions.h.in \
 	libfvde.rc \
 	libfvde.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfvde_definitions.h \
+	libfvde.rc \
+	Makefile \
 	Makefile.in
 
-distclean: clean
-	-rm -f libfvde_definitions.h
-	-rm -f libfvde.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfvde ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfvde_la_SOURCES)
```

### Comparing `libfvde-20240113/libfvde/libfvde_physical_volume.h` & `libfvde-20240502/libfvde/libfvde_physical_volume.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_definitions.h` & `libfvde-20240502/libfvde/libfvde_definitions.h.in`

 * *Files 2% similar despite different names*

```diff
@@ -34,19 +34,19 @@
 #if !defined( HAVE_LOCAL_LIBFVDE )
 #include <libfvde/definitions.h>
 
 /* The definitions in <libfvde/definitions.h> are copied here
  * for local use of libfvde
  */
 #else
-#define LIBFVDE_VERSION					20240113
+#define LIBFVDE_VERSION					@VERSION@
 
 /* The version string
  */
-#define LIBFVDE_VERSION_STRING				"20240113"
+#define LIBFVDE_VERSION_STRING				"@VERSION@"
 
 /* The file access
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBFVDE_ACCESS_FLAGS
```

### Comparing `libfvde-20240113/libfvde/libfvde_support.h` & `libfvde-20240502/libfvde/libfvde_support.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_physical_volume_descriptor.h` & `libfvde-20240502/libfvde/libfvde_physical_volume_descriptor.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_libclocale.h` & `libfvde-20240502/libfvde/libfvde_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_libhmac.h` & `libfvde-20240502/libfvde/libfvde_libhmac.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_notify.c` & `libfvde-20240502/libfvde/libfvde_notify.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_encrypted_metadata.c` & `libfvde-20240502/libfvde/libfvde_encrypted_metadata.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_definitions.h.in` & `libfvde-20240502/libfvde/libfvde_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -34,19 +34,19 @@
 #if !defined( HAVE_LOCAL_LIBFVDE )
 #include <libfvde/definitions.h>
 
 /* The definitions in <libfvde/definitions.h> are copied here
  * for local use of libfvde
  */
 #else
-#define LIBFVDE_VERSION					@VERSION@
+#define LIBFVDE_VERSION					20240502
 
 /* The version string
  */
-#define LIBFVDE_VERSION_STRING				"@VERSION@"
+#define LIBFVDE_VERSION_STRING				"20240502"
 
 /* The file access
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBFVDE_ACCESS_FLAGS
```

### Comparing `libfvde-20240113/libfvde/libfvde_sector_data.h` & `libfvde-20240502/libfvde/libfvde_sector_data.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_keyring.h` & `libfvde-20240502/libfvde/libfvde_keyring.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_notify.h` & `libfvde-20240502/libfvde/libfvde_notify.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_encryption_context.c` & `libfvde-20240502/libfvde/libfvde_encryption_context.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_volume_data_handle.h` & `libfvde-20240502/libfvde/libfvde_volume_data_handle.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_checksum.c` & `libfvde-20240502/libfvde/libfvde_checksum.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_physical_volume_descriptor.c` & `libfvde-20240502/libfvde/libfvde_physical_volume_descriptor.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_encryption_context_plist.c` & `libfvde-20240502/libfvde/libfvde_encryption_context_plist.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_logical_volume_descriptor.h` & `libfvde-20240502/libfvde/libfvde_logical_volume_descriptor.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde.rc` & `libfvde-20240502/libfvde/libfvde.rc`

 * *Files 10% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the FileVault Drive Encryption (FVDE) format\0"
-      VALUE "FileVersion",		"20240113" "\0"
+      VALUE "FileVersion",		"20240502" "\0"
       VALUE "InternalName",		"libfvde.dll\0"
       VALUE "LegalCopyright",		"(C) 2011-2024, Omar Choudary <choudary.omar@gmail.com>, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libfvde.dll\0"
       VALUE "ProductName",		"libfvde\0"
-      VALUE "ProductVersion",		"20240113" "\0"
+      VALUE "ProductVersion",		"20240502" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libfvde/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libfvde-20240113/libfvde/libfvde_password.h` & `libfvde-20240502/libfvde/libfvde_password.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_libcthreads.h` & `libfvde-20240502/libfvde/libfvde_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_volume_data_handle.c` & `libfvde-20240502/libfvde/libfvde_volume_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_io_handle.c` & `libfvde-20240502/libfvde/libfvde_io_handle.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_metadata_block.c` & `libfvde-20240502/libfvde/libfvde_metadata_block.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_deflate.c` & `libfvde-20240502/libfvde/libfvde_deflate.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_volume.h` & `libfvde-20240502/libfvde/libfvde_volume.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_encrypted_metadata.h` & `libfvde-20240502/libfvde/libfvde_encrypted_metadata.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_libcnotify.h` & `libfvde-20240502/libfvde/libfvde_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_libuna.h` & `libfvde-20240502/libfvde/libfvde_libuna.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/fvde_volume.h` & `libfvde-20240502/libfvde/fvde_volume.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_libcerror.h` & `libfvde-20240502/libfvde/libfvde_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_libfcache.h` & `libfvde-20240502/libfvde/libfvde_libfcache.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_extern.h` & `libfvde-20240502/libfvde/libfvde_extern.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_metadata.h` & `libfvde-20240502/libfvde/libfvde_metadata.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_segment_descriptor.h` & `libfvde-20240502/libfvde/libfvde_segment_descriptor.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_codepage.h` & `libfvde-20240502/libfvde/libfvde_codepage.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_debug.h` & `libfvde-20240502/libfvde/libfvde_debug.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_huffman_tree.h` & `libfvde-20240502/libfvde/libfvde_huffman_tree.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_encryption_context.h` & `libfvde-20240502/libfvde/libfvde_encryption_context.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_metadata.c` & `libfvde-20240502/libfvde/libfvde_metadata.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_deflate.h` & `libfvde-20240502/libfvde/libfvde_deflate.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_bit_stream.h` & `libfvde-20240502/libfvde/libfvde_bit_stream.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_libfguid.h` & `libfvde-20240502/libfvde/libfvde_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_libfvalue.h` & `libfvde-20240502/libfvde/libfvde_libfvalue.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_error.h` & `libfvde-20240502/libfvde/libfvde_error.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_volume_group.h` & `libfvde-20240502/libfvde/libfvde_volume_group.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_support.c` & `libfvde-20240502/libfvde/libfvde_support.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_logical_volume_descriptor.c` & `libfvde-20240502/libfvde/libfvde_logical_volume_descriptor.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_error.c` & `libfvde-20240502/libfvde/libfvde_error.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_libbfio.h` & `libfvde-20240502/libfvde/libfvde_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_huffman_tree.c` & `libfvde-20240502/libfvde/libfvde_huffman_tree.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_unused.h` & `libfvde-20240502/libfvde/libfvde_unused.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_debug.c` & `libfvde-20240502/libfvde/libfvde_debug.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/Makefile.in` & `libfvde-20240502/libfvde/Makefile.in`

 * *Files 6% similar despite different names*

```diff
@@ -550,14 +550,16 @@
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
@@ -624,16 +626,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -729,15 +731,18 @@
 
 libfvde_la_LDFLAGS = -no-undefined -version-info 1:0:0
 EXTRA_DIST = \
 	libfvde_definitions.h.in \
 	libfvde.rc \
 	libfvde.rc.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfvde_definitions.h \
+	libfvde.rc \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -995,24 +1000,54 @@
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
+		-rm -f ./$(DEPDIR)/libfvde.Plo
+	-rm -f ./$(DEPDIR)/libfvde_bit_stream.Plo
+	-rm -f ./$(DEPDIR)/libfvde_checksum.Plo
+	-rm -f ./$(DEPDIR)/libfvde_compression.Plo
+	-rm -f ./$(DEPDIR)/libfvde_debug.Plo
+	-rm -f ./$(DEPDIR)/libfvde_deflate.Plo
+	-rm -f ./$(DEPDIR)/libfvde_encrypted_metadata.Plo
+	-rm -f ./$(DEPDIR)/libfvde_encryption_context.Plo
+	-rm -f ./$(DEPDIR)/libfvde_encryption_context_plist.Plo
+	-rm -f ./$(DEPDIR)/libfvde_error.Plo
+	-rm -f ./$(DEPDIR)/libfvde_huffman_tree.Plo
+	-rm -f ./$(DEPDIR)/libfvde_io_handle.Plo
+	-rm -f ./$(DEPDIR)/libfvde_keyring.Plo
+	-rm -f ./$(DEPDIR)/libfvde_logical_volume.Plo
+	-rm -f ./$(DEPDIR)/libfvde_logical_volume_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libfvde_metadata.Plo
+	-rm -f ./$(DEPDIR)/libfvde_metadata_block.Plo
+	-rm -f ./$(DEPDIR)/libfvde_notify.Plo
+	-rm -f ./$(DEPDIR)/libfvde_password.Plo
+	-rm -f ./$(DEPDIR)/libfvde_physical_volume.Plo
+	-rm -f ./$(DEPDIR)/libfvde_physical_volume_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libfvde_sector_data.Plo
+	-rm -f ./$(DEPDIR)/libfvde_segment_descriptor.Plo
+	-rm -f ./$(DEPDIR)/libfvde_support.Plo
+	-rm -f ./$(DEPDIR)/libfvde_volume.Plo
+	-rm -f ./$(DEPDIR)/libfvde_volume_data_handle.Plo
+	-rm -f ./$(DEPDIR)/libfvde_volume_group.Plo
+	-rm -f ./$(DEPDIR)/libfvde_volume_header.Plo
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1123,19 +1158,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-libLTLIBRARIES
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libfvde_definitions.h
-	-rm -f libfvde.rc
-	-rm -f Makefile
-
 sources-local: $(BUILT_SOURCES)
 
 splint-local:
 	@echo "Running splint on libfvde ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfvde_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
```

### Comparing `libfvde-20240113/libfvde/libfvde_keyring.c` & `libfvde-20240502/libfvde/libfvde_keyring.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_volume_header.h` & `libfvde-20240502/libfvde/libfvde_volume_header.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_volume.c` & `libfvde-20240502/libfvde/libfvde_volume.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_volume_header.c` & `libfvde-20240502/libfvde/libfvde_volume_header.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_segment_descriptor.c` & `libfvde-20240502/libfvde/libfvde_segment_descriptor.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_physical_volume.c` & `libfvde-20240502/libfvde/libfvde_physical_volume.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_io_handle.h` & `libfvde-20240502/libfvde/libfvde_io_handle.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde/libfvde_compression.c` & `libfvde-20240502/libfvde/libfvde_compression.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/m4/libcfile.m4` & `libfvde-20240502/m4/libcfile.m4`

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

### Comparing `libfvde-20240113/m4/tests.m4` & `libfvde-20240502/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/m4/libcpath.m4` & `libfvde-20240502/m4/libcpath.m4`

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

### Comparing `libfvde-20240113/m4/lib-prefix.m4` & `libfvde-20240502/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/m4/progtest.m4` & `libfvde-20240502/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/m4/libuna.m4` & `libfvde-20240502/m4/libuna.m4`

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

### Comparing `libfvde-20240113/m4/gettext.m4` & `libfvde-20240502/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/m4/lib-ld.m4` & `libfvde-20240502/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/m4/libclocale.m4` & `libfvde-20240502/m4/libclocale.m4`

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

### Comparing `libfvde-20240113/m4/libcdata.m4` & `libfvde-20240502/m4/libcdata.m4`

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

### Comparing `libfvde-20240113/m4/libcsplit.m4` & `libfvde-20240502/m4/libcsplit.m4`

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

### Comparing `libfvde-20240113/m4/common.m4` & `libfvde-20240502/m4/common.m4`

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

### Comparing `libfvde-20240113/m4/libcthreads.m4` & `libfvde-20240502/m4/libcthreads.m4`

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

### Comparing `libfvde-20240113/m4/ltversion.m4` & `libfvde-20240502/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/m4/ltsugar.m4` & `libfvde-20240502/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/m4/libfdata.m4` & `libfvde-20240502/m4/libfdata.m4`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Functions for libfdata
 dnl
-dnl Version: 20230318
+dnl Version: 20240413
 
 dnl Function to detect if libfdata is available
 dnl ac_libfdata_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFDATA_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdata" = xno],
     [ac_cv_libfdata=no],
     [ac_cv_libfdata=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfdata which returns "yes" and --with-libfdata= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect],
+      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfdata"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdata}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfdata],
           [1])
@@ -450,16 +452,17 @@
         dnl TODO: add functions
 
         dnl Vector list functions
         dnl TODO: add functions
 
         ac_cv_libfdata_LIBADD="-lfdata"])
       ])
+
     AS_IF(
-      [test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_libfdata" != xyes],
+      [test "x$ac_cv_libfdata" != xyes && test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes],
       [AC_MSG_FAILURE(
         [unable to find supported libfdata in directory: $ac_cv_with_libfdata],
         [1])
       ])
     ])
 
   AS_IF(
@@ -481,15 +484,15 @@
     ])
   ])
 
 dnl Function to detect if libfdata dependencies are available
 AC_DEFUN([AX_LIBFDATA_CHECK_LOCAL],
   [dnl No additional checks.
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
   ])
 
 dnl Function to detect how to enable libfdata
 AC_DEFUN([AX_LIBFDATA_CHECK_ENABLE],
```

### Comparing `libfvde-20240113/m4/host-cpu-c-abi.m4` & `libfvde-20240502/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/m4/libfuse.m4` & `libfvde-20240502/m4/libfuse.m4`

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

### Comparing `libfvde-20240113/m4/libtool.m4` & `libfvde-20240502/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/m4/po.m4` & `libfvde-20240502/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/m4/libcerror.m4` & `libfvde-20240502/m4/libcerror.m4`

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

### Comparing `libfvde-20240113/m4/libcnotify.m4` & `libfvde-20240502/m4/libcnotify.m4`

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

### Comparing `libfvde-20240113/m4/libfguid.m4` & `libfvde-20240502/m4/libfguid.m4`

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

### Comparing `libfvde-20240113/m4/libbfio.m4` & `libfvde-20240502/m4/libbfio.m4`

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

### Comparing `libfvde-20240113/m4/libhmac.m4` & `libfvde-20240502/m4/libhmac.m4`

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

### Comparing `libfvde-20240113/m4/intlmacosx.m4` & `libfvde-20240502/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/m4/lt~obsolete.m4` & `libfvde-20240502/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/m4/lib-link.m4` & `libfvde-20240502/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/m4/iconv.m4` & `libfvde-20240502/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/m4/ltoptions.m4` & `libfvde-20240502/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/m4/nls.m4` & `libfvde-20240502/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/m4/python.m4` & `libfvde-20240502/m4/python.m4`

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

### Comparing `libfvde-20240113/m4/libcrypto.m4` & `libfvde-20240502/m4/libcrypto.m4`

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

### Comparing `libfvde-20240113/m4/libfvalue.m4` & `libfvde-20240502/m4/libfvalue.m4`

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

### Comparing `libfvde-20240113/m4/types.m4` & `libfvde-20240502/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/m4/libfcache.m4` & `libfvde-20240502/m4/libfcache.m4`

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

### Comparing `libfvde-20240113/m4/pthread.m4` & `libfvde-20240502/m4/pthread.m4`

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

### Comparing `libfvde-20240113/m4/libfplist.m4` & `libfvde-20240502/m4/libfplist.m4`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 dnl Functions for libfplist
 dnl
-dnl Version: 20230218
+dnl Version: 20240413
 
 dnl Function to detect if libfplist is available
 dnl ac_libfplist_dummy is used to prevent AC_CHECK_LIB adding unnecessary -l<library> arguments
 AC_DEFUN([AX_LIBFPLIST_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfplist" = xno],
     [ac_cv_libfplist=no],
     [ac_cv_libfplist=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-libfplist which returns "yes" and --with-libfplist= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_libfplist" != x && test "x$ac_cv_with_libfplist" != xauto-detect],
+      [test "x$ac_cv_with_libfplist" != x && test "x$ac_cv_with_libfplist" != xauto-detect && test "x$ac_cv_with_libfplist" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_libfplist"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_libfplist}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfplist}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_libfplist],
           [1])
@@ -135,14 +137,21 @@
           libfplist_property_get_sub_property_by_utf8_name,
           [ac_cv_libfplist_dummy=yes],
           [ac_cv_libfplist=no])
 
         ac_cv_libfplist_LIBADD="-lfplist"
         ])
       ])
+
+    AS_IF(
+      [test "x$ac_cv_libfplist" != xyes && test "x$ac_cv_with_libfplist" != x && test "x$ac_cv_with_libfplist" != xauto-detect && test "x$ac_cv_with_libfplist" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported libfplist in directory: $ac_cv_with_libfplist],
+        [1])
+      ])
     ])
 
   AS_IF(
     [test "x$ac_cv_libfplist" = xyes],
     [AC_DEFINE(
       [HAVE_LIBFPLIST],
       [1],
@@ -161,15 +170,15 @@
   ])
 
 dnl Function to detect if libfplist dependencies are available
 AC_DEFUN([AX_LIBFPLIST_CHECK_LOCAL],
   [AC_PROG_LEX(noyywrap)
   AC_PROG_YACC
 
-  ac_cv_libfplist_CPPFLAGS="-I../libfplist";
+  ac_cv_libfplist_CPPFLAGS="-I../libfplist -I\$(top_srcdir)/libfplist";
   ac_cv_libfplist_LIBADD="../libfplist/libfplist.la";
 
   ac_cv_libfplist=local
   ])
 
 dnl Function to detect how to enable libfplist
 AC_DEFUN([AX_LIBFPLIST_CHECK_ENABLE],
```

### Comparing `libfvde-20240113/m4/zlib.m4` & `libfvde-20240502/m4/zlib.m4`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 dnl Checks for zlib required headers and functions
 dnl
-dnl Version: 20201230
+dnl Version: 20240314
 
 dnl Function to detect if zlib is available
 AC_DEFUN([AX_ZLIB_CHECK_LIB],
   [AS_IF(
     [test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_zlib" = xno],
     [ac_cv_zlib=no],
     [ac_cv_zlib=check
     dnl Check if the directory provided as parameter exists
+    dnl For both --with-zlib which returns "yes" and --with-zlib= which returns ""
+    dnl treat them as auto-detection.
     AS_IF(
-      [test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect],
+      [test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect && test "x$ac_cv_with_zlib" != xyes],
       [AS_IF(
         [test -d "$ac_cv_with_zlib"],
         [CFLAGS="$CFLAGS -I${ac_cv_with_zlib}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_zlib}/lib"],
         [AC_MSG_FAILURE(
           [no such directory: $ac_cv_with_zlib],
           [1])
@@ -58,14 +60,21 @@
             [Missing function: zlibVersion in library: zlib.],
             [1])
           ])
 
         ac_cv_zlib_LIBADD="-lz";
         ])
       ])
+
+    AS_IF(
+      [test "x$ac_cv_zlib" != xyes && test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect && test "x$ac_cv_with_zlib" != xyes],
+      [AC_MSG_FAILURE(
+        [unable to find supported zlib in directory: $ac_cv_with_zlib],
+        [1])
+      ])
     ])
 
   AS_IF(
     [test "x$ac_cv_zlib" = xzlib],
     [AC_DEFINE(
       [HAVE_ZLIB],
       [1],
```

### Comparing `libfvde-20240113/m4/libcaes.m4` & `libfvde-20240502/m4/libcaes.m4`

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

### Comparing `libfvde-20240113/include/libfvde.h.in` & `libfvde-20240502/include/libfvde.h.in`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/include/libfvde/definitions.h.in` & `libfvde-20240502/include/libfvde/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/include/libfvde/definitions.h` & `libfvde-20240502/include/libfvde/definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -21,19 +21,19 @@
  */
 
 #if !defined( _LIBFVDE_DEFINITIONS_H )
 #define _LIBFVDE_DEFINITIONS_H
 
 #include <libfvde/types.h>
 
-#define LIBFVDE_VERSION				20240113
+#define LIBFVDE_VERSION				20240502
 
 /* The version string
  */
-#define LIBFVDE_VERSION_STRING			"20240113"
+#define LIBFVDE_VERSION_STRING			"20240502"
 
 /* The file access
  * bit 1        set to 1 for read access
  * bit 2        set to 1 for write access
  * bit 3-8      not used
  */
 enum LIBFVDE_ACCESS_FLAGS
```

### Comparing `libfvde-20240113/include/libfvde/types.h.in` & `libfvde-20240502/include/libfvde/types.h.in`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/include/libfvde/types.h` & `libfvde-20240502/include/libfvde/types.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/include/libfvde/features.h.in` & `libfvde-20240502/include/libfvde/features.h.in`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/include/libfvde/error.h` & `libfvde-20240502/include/libfvde/error.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/include/libfvde/extern.h` & `libfvde-20240502/include/libfvde/extern.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/include/libfvde/features.h` & `libfvde-20240502/include/libfvde/features.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/include/libfvde/codepage.h` & `libfvde-20240502/include/libfvde/codepage.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/include/libfvde.h` & `libfvde-20240502/include/libfvde.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/include/Makefile.in` & `libfvde-20240502/include/Makefile.in`

 * *Files 1% similar despite different names*

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
@@ -570,15 +572,20 @@
 
 EXTRA_DIST = \
 	libfvde.h.in \
 	libfvde/definitions.h.in \
 	libfvde/features.h.in \
 	libfvde/types.h.in
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	libfvde.h \
+	libfvde/definitions.h \
+	libfvde/features.h \
+	libfvde/types.h \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -775,23 +782,25 @@
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
@@ -873,17 +882,10 @@
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-includeHEADERS \
 	uninstall-pkgincludeHEADERS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f libfvde.h
-	-rm -f libfvde/definitions.h
-	-rm -f libfvde/features.h
-	-rm -f libfvde/types.h
-	-rm -f Makefile
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfvde-20240113/common/config_borlandc.h` & `libfvde-20240502/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/common/file_stream.h` & `libfvde-20240502/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/common/memory.h` & `libfvde-20240502/common/memory.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/common/byte_stream.h` & `libfvde-20240502/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/common/common.h` & `libfvde-20240502/common/common.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/common/config_winapi.h` & `libfvde-20240502/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/common/system_string.h` & `libfvde-20240502/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/common/types.h.in` & `libfvde-20240502/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/common/types.h` & `libfvde-20240502/common/types.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/common/config.h.in` & `libfvde-20240502/common/config.h.in`

 * *Files 1% similar despite different names*

```diff
@@ -275,14 +275,17 @@
 
 /* Define to 1 if you have the <libfplist.h> header file. */
 #undef HAVE_LIBFPLIST_H
 
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

### Comparing `libfvde-20240113/common/config.h` & `libfvde-20240502/common/config.h`

 * *Files 1% similar despite different names*

```diff
@@ -274,15 +274,18 @@
 /* Define to 1 if you have the `fplist' library (-lfplist). */
 /* #undef HAVE_LIBFPLIST */
 
 /* Define to 1 if you have the <libfplist.h> header file. */
 /* #undef HAVE_LIBFPLIST_H */
 
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
 
@@ -661,24 +664,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libfvde"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libfvde 20240113"
+#define PACKAGE_STRING "libfvde 20240502"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libfvde"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20240113"
+#define PACKAGE_VERSION "20240502"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -699,15 +702,15 @@
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Define to 1 if your <sys/time.h> declares `struct tm'. */
 /* #undef TM_IN_SYS_TIME */
 
 /* Version number of package */
-#define VERSION "20240113"
+#define VERSION "20240502"
 
 /* Define to 1 if `lex' declares `yytext' as a `char *' by default, not a
    `char[]'. */
 #define YYTEXT_POINTER 1
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
```

### Comparing `libfvde-20240113/common/wide_string.h` & `libfvde-20240502/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/common/narrow_string.h` & `libfvde-20240502/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/common/config_msc.h` & `libfvde-20240502/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/common/Makefile.in` & `libfvde-20240502/common/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -450,14 +450,16 @@
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
@@ -523,15 +525,17 @@
 sysconfdir = @sysconfdir@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -539,15 +543,18 @@
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
@@ -715,23 +722,25 @@
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
@@ -811,15 +820,10 @@
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

### Comparing `libfvde-20240113/libclocale/libclocale_wide_string.c` & `libfvde-20240502/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libclocale/libclocale_support.h` & `libfvde-20240502/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libclocale/Makefile.am` & `libfvde-20240502/libclocale/Makefile.am`

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

### Comparing `libfvde-20240113/libclocale/libclocale_definitions.h` & `libfvde-20240502/libclocale/libclocale_definitions.h`

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

### Comparing `libfvde-20240113/libclocale/libclocale_unused.h` & `libfvde-20240502/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libclocale/libclocale_libcerror.h` & `libfvde-20240502/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libclocale/libclocale_locale.h` & `libfvde-20240502/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libclocale/libclocale_support.c` & `libfvde-20240502/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libclocale/libclocale_codepage.c` & `libfvde-20240502/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libclocale/libclocale_locale.c` & `libfvde-20240502/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libclocale/Makefile.in` & `libfvde-20240502/libclocale/Makefile.in`

 * *Files 3% similar despite different names*

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
@@ -569,30 +571,31 @@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -795,24 +798,30 @@
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
 
@@ -899,17 +908,14 @@
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

### Comparing `libfvde-20240113/libclocale/libclocale_extern.h` & `libfvde-20240502/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libclocale/libclocale_wide_string.h` & `libfvde-20240502/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libclocale/libclocale_codepage.h` & `libfvde-20240502/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde.spec` & `libfvde-20240502/libfvde.spec`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libfvde
-Version: 20240113
+Version: 20240502
 Release: 1
 Summary: Library to access the FileVault Drive Encryption (FVDE) format
 Group: System Environment/Libraries
 License: LGPL-3.0-or-later
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libfvde
 Requires:         openssl          zlib
@@ -36,16 +36,16 @@
 
 %description -n libfvde-python3
 Python 3 bindings for libfvde
 
 %package -n libfvde-tools
 Summary: Several tools for reading FileVault Drive Encryption volumes
 Group: Applications/System
-Requires: libfvde = %{version}-%{release} fuse-libs
-BuildRequires: fuse-devel
+Requires: libfvde = %{version}-%{release} fuse3-libs
+BuildRequires: fuse3-devel
 
 %description -n libfvde-tools
 Several tools for reading FileVault Drive Encryption volumes
 
 %prep
 %setup -q
 
@@ -91,10 +91,10 @@
 %files -n libfvde-tools
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Sat Jan 13 2024 Joachim Metz <joachim.metz@gmail.com> 20240113-1
+* Thu May  2 2024 Joachim Metz <joachim.metz@gmail.com> 20240502-1
 - Auto-generated
```

### Comparing `libfvde-20240113/libfcache/libfcache_libcdata.h` & `libfvde-20240502/libfcache/libfcache_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfcache/libfcache_types.h` & `libfvde-20240502/libfcache/libfcache_types.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfcache/libfcache_cache_value.c` & `libfvde-20240502/libfcache/libfcache_cache_value.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfcache/libfcache_unused.h` & `libfvde-20240502/libfcache/libfcache_unused.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfcache/Makefile.am` & `libfvde-20240502/libfcache/Makefile.am`

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

### Comparing `libfvde-20240113/libfcache/libfcache_support.h` & `libfvde-20240502/libfcache/libfcache_support.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfcache/libfcache_error.h` & `libfvde-20240502/libfcache/libfcache_error.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfcache/libfcache_support.c` & `libfvde-20240502/libfcache/libfcache_support.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfcache/libfcache_cache.h` & `libfvde-20240502/libfcache/libfcache_cache.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfcache/libfcache_error.c` & `libfvde-20240502/libfcache/libfcache_error.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfcache/libfcache_libcerror.h` & `libfvde-20240502/libfcache/libfcache_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfcache/libfcache_date_time.c` & `libfvde-20240502/libfcache/libfcache_date_time.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfcache/libfcache_extern.h` & `libfvde-20240502/libfcache/libfcache_extern.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfcache/libfcache_cache_value.h` & `libfvde-20240502/libfcache/libfcache_cache_value.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfcache/Makefile.in` & `libfvde-20240502/libfcache/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -497,14 +497,16 @@
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
@@ -571,16 +573,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -592,15 +594,16 @@
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
@@ -804,24 +807,31 @@
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
 
@@ -909,17 +919,14 @@
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

### Comparing `libfvde-20240113/libfcache/libfcache_date_time.h` & `libfvde-20240502/libfcache/libfcache_date_time.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfcache/libfcache_definitions.h` & `libfvde-20240502/libfcache/libfcache_definitions.h`

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

### Comparing `libfvde-20240113/libfcache/libfcache_cache.c` & `libfvde-20240502/libfcache/libfcache_cache.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/Makefile.am` & `libfvde-20240502/Makefile.am`

 * *Files 19% similar despite different names*

```diff
@@ -62,16 +62,23 @@
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
+	libfvde.pc \
+	libfvde.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 
 pkgconfig_DATA = \
 	libfvde.pc
 
 libtool: @LIBTOOL_DEPS@
@@ -97,19 +104,7 @@
 	(cd $(srcdir)/libfvalue && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfplist && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libhmac && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libcaes && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfvde && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libfvde.pc
-	-rm -f libfvde.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
```

### Comparing `libfvde-20240113/libbfio/libbfio_file_range.h` & `libfvde-20240502/libbfio/libbfio_file_range.h`

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

### Comparing `libfvde-20240113/libbfio/libbfio_file_range_io_handle.c` & `libfvde-20240502/libbfio/libbfio_file_range_io_handle.c`

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

### Comparing `libfvde-20240113/libbfio/libbfio_support.c` & `libfvde-20240502/libbfio/libbfio_support.c`

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

### Comparing `libfvde-20240113/libbfio/libbfio_libcpath.h` & `libfvde-20240502/libbfio/libbfio_libcpath.h`

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

### Comparing `libfvde-20240113/libbfio/libbfio_error.h` & `libfvde-20240502/libbfio/libbfio_error.h`

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

### Comparing `libfvde-20240113/libbfio/libbfio_libclocale.h` & `libfvde-20240502/libbfio/libbfio_libclocale.h`

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

### Comparing `libfvde-20240113/libbfio/libbfio_error.c` & `libfvde-20240502/libbfio/libbfio_error.c`

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

### Comparing `libfvde-20240113/libbfio/libbfio_libuna.h` & `libfvde-20240502/libbfio/libbfio_libuna.h`

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

### Comparing `libfvde-20240113/libbfio/libbfio_file_io_handle.h` & `libfvde-20240502/libbfio/libbfio_file_io_handle.h`

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

### Comparing `libfvde-20240113/libbfio/libbfio_file_pool.h` & `libfvde-20240502/libbfio/libbfio_file_pool.h`

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

### Comparing `libfvde-20240113/libbfio/libbfio_file_range.c` & `libfvde-20240502/libbfio/libbfio_file_range.c`

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

### Comparing `libfvde-20240113/libbfio/libbfio_types.h` & `libfvde-20240502/libbfio/libbfio_types.h`

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

### Comparing `libfvde-20240113/libbfio/libbfio_unused.h` & `libfvde-20240502/libbfio/libbfio_unused.h`

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

### Comparing `libfvde-20240113/libbfio/libbfio_libcdata.h` & `libfvde-20240502/libbfio/libbfio_libcdata.h`

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

### Comparing `libfvde-20240113/libbfio/libbfio_file.h` & `libfvde-20240502/libbfio/libbfio_file.h`

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

### Comparing `libfvde-20240113/libbfio/Makefile.am` & `libfvde-20240502/libbfio/Makefile.am`

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

### Comparing `libfvde-20240113/libbfio/libbfio_libcfile.h` & `libfvde-20240502/libbfio/libbfio_libcfile.h`

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

### Comparing `libfvde-20240113/libbfio/libbfio_definitions.h` & `libfvde-20240502/libbfio/libbfio_definitions.h`

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

### Comparing `libfvde-20240113/libbfio/libbfio_codepage.h` & `libfvde-20240502/libbfio/libbfio_codepage.h`

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

### Comparing `libfvde-20240113/libbfio/libbfio_file_io_handle.c` & `libfvde-20240502/libbfio/libbfio_file_io_handle.c`

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

### Comparing `libfvde-20240113/libbfio/libbfio_support.h` & `libfvde-20240502/libbfio/libbfio_support.h`

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

### Comparing `libfvde-20240113/libbfio/libbfio_memory_range.h` & `libfvde-20240502/libbfio/libbfio_memory_range.h`

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

### Comparing `libfvde-20240113/libbfio/libbfio_file_pool.c` & `libfvde-20240502/libbfio/libbfio_file_pool.c`

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

### Comparing `libfvde-20240113/libbfio/libbfio_file_range_io_handle.h` & `libfvde-20240502/libbfio/libbfio_file_range_io_handle.h`

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

### Comparing `libfvde-20240113/libbfio/libbfio_libcthreads.h` & `libfvde-20240502/libbfio/libbfio_libcthreads.h`

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

### Comparing `libfvde-20240113/libbfio/libbfio_system_string.h` & `libfvde-20240502/libbfio/libbfio_system_string.h`

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

### Comparing `libfvde-20240113/libbfio/libbfio_memory_range_io_handle.c` & `libfvde-20240502/libbfio/libbfio_memory_range_io_handle.c`

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

### Comparing `libfvde-20240113/libbfio/libbfio_handle.c` & `libfvde-20240502/libbfio/libbfio_handle.c`

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

### Comparing `libfvde-20240113/libbfio/libbfio_file.c` & `libfvde-20240502/libbfio/libbfio_file.c`

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

### Comparing `libfvde-20240113/libbfio/libbfio_handle.h` & `libfvde-20240502/libbfio/libbfio_handle.h`

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

### Comparing `libfvde-20240113/libbfio/libbfio_memory_range.c` & `libfvde-20240502/libbfio/libbfio_memory_range.c`

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

### Comparing `libfvde-20240113/libbfio/libbfio_pool.c` & `libfvde-20240502/libbfio/libbfio_pool.c`

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

### Comparing `libfvde-20240113/libbfio/libbfio_libcerror.h` & `libfvde-20240502/libbfio/libbfio_libcerror.h`

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

### Comparing `libfvde-20240113/libbfio/Makefile.in` & `libfvde-20240502/libbfio/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -515,14 +515,16 @@
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
@@ -589,16 +591,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -629,15 +631,16 @@
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
@@ -848,24 +851,38 @@
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
 
@@ -934,14 +951,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -952,23 +971,22 @@
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

### Comparing `libfvde-20240113/libbfio/libbfio_system_string.c` & `libfvde-20240502/libbfio/libbfio_system_string.c`

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

### Comparing `libfvde-20240113/libbfio/libbfio_memory_range_io_handle.h` & `libfvde-20240502/libbfio/libbfio_memory_range_io_handle.h`

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

### Comparing `libfvde-20240113/libbfio/libbfio_extern.h` & `libfvde-20240502/libbfio/libbfio_extern.h`

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

### Comparing `libfvde-20240113/libbfio/libbfio_pool.h` & `libfvde-20240502/libbfio/libbfio_pool.h`

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

### Comparing `libfvde-20240113/config.guess` & `libfvde-20240502/config.guess`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/dpkg/copyright` & `libfvde-20240502/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/dpkg/control` & `libfvde-20240502/dpkg/control`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/dpkg/rules` & `libfvde-20240502/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/COPYING.LESSER` & `libfvde-20240502/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/configure` & `libfvde-20240502/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libfvde 20240113.
+# Generated by GNU Autoconf 2.71 for libfvde 20240502.
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
 PACKAGE_NAME='libfvde'
 PACKAGE_TARNAME='libfvde'
-PACKAGE_VERSION='20240113'
-PACKAGE_STRING='libfvde 20240113'
+PACKAGE_VERSION='20240502'
+PACKAGE_STRING='libfvde 20240502'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libfvde.h.in"
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
@@ -1177,14 +1179,16 @@
 zlib_LIBS
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
@@ -1727,15 +1731,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libfvde 20240113 to adapt to many kinds of systems.
+\`configure' configures libfvde 20240502 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1798,15 +1802,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libfvde 20240113:";;
+     short | recursive ) echo "Configuration of libfvde 20240502:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -2021,14 +2025,17 @@
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
@@ -2091,15 +2098,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libfvde configure 20240113
+libfvde configure 20240502
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2812,15 +2819,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libfvde $as_me 20240113, which was
+It was created by libfvde $as_me 20240502, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4301,15 +4308,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libfvde'
- VERSION='20240113'
+ VERSION='20240502'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -23896,15 +23903,15 @@
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
@@ -24395,15 +24402,16 @@
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
@@ -24545,15 +24553,15 @@
 as_fn_error 1 "Missing functions: strerror_r and strerror
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 fi
 
-  ac_cv_libcerror_CPPFLAGS="-I../libcerror";
+  ac_cv_libcerror_CPPFLAGS="-I../libcerror -I\$(top_srcdir)/libcerror";
   ac_cv_libcerror_LIBADD="../libcerror/libcerror.la";
 
   ac_cv_libcerror=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCERROR 1" >>confdefs.h
@@ -24647,15 +24655,15 @@
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
@@ -26287,15 +26295,15 @@
 
 
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
@@ -26349,47 +26357,52 @@
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
@@ -26423,15 +26436,15 @@
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
@@ -26465,15 +26478,15 @@
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
@@ -26508,15 +26521,15 @@
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
@@ -26550,15 +26563,15 @@
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
@@ -26592,15 +26605,15 @@
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
@@ -26634,15 +26647,15 @@
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
@@ -26676,15 +26689,15 @@
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
@@ -26719,15 +26732,15 @@
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
@@ -26761,15 +26774,15 @@
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
@@ -26803,15 +26816,15 @@
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
@@ -26845,15 +26858,15 @@
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
@@ -26887,15 +26900,15 @@
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
@@ -26930,15 +26943,15 @@
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
@@ -26972,15 +26985,15 @@
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
@@ -27014,15 +27027,15 @@
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
@@ -27056,15 +27069,15 @@
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
@@ -27098,15 +27111,15 @@
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
@@ -27141,67 +27154,76 @@
 then :
   ac_pthread_dummy=yes
 else $as_nop
   ac_cv_pthread=no
 fi
 
 
-   ac_cv_pthread_LIBADD="-lpthread";
+        ac_cv_pthread_LIBADD="-lpthread";
 
 fi
 
+    if test "x$ac_cv_with_pthread" != x && test "x$ac_cv_with_pthread" != xauto-detect && test "x$ac_cv_with_pthread" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported pthread in directory: $ac_cv_with_pthread
+See \`config.log' for more details" "$LINENO" 5; }
+
 fi
 
- if test "x$ac_cv_pthread" = xpthread
+fi
+
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
 
@@ -27289,15 +27311,15 @@
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
@@ -31068,15 +31090,16 @@
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
@@ -31101,15 +31124,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcdata" != xyes
 then :
 
-  ac_cv_libcdata_CPPFLAGS="-I../libcdata";
+  ac_cv_libcdata_CPPFLAGS="-I../libcdata -I\$(top_srcdir)/libcdata";
   ac_cv_libcdata_LIBADD="../libcdata/libcdata.la";
 
   ac_cv_libcdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCDATA 1" >>confdefs.h
@@ -31179,15 +31202,15 @@
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
@@ -31734,15 +31757,16 @@
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
@@ -31898,15 +31922,15 @@
 
 printf "%s\n" "#define HAVE_LANGINFO_CODESET 1" >>confdefs.h
 
 
 fi
 
 
-  ac_cv_libclocale_CPPFLAGS="-I../libclocale";
+  ac_cv_libclocale_CPPFLAGS="-I../libclocale -I\$(top_srcdir)/libclocale";
   ac_cv_libclocale_LIBADD="../libclocale/libclocale.la";
 
   ac_cv_libclocale=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCLOCALE 1" >>confdefs.h
@@ -31976,15 +32000,15 @@
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
@@ -32434,15 +32458,16 @@
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
@@ -32497,15 +32522,15 @@
 if test "x$ac_cv_header_errno_h" = xyes
 then :
   printf "%s\n" "#define HAVE_ERRNO_H 1" >>confdefs.h
 
 fi
 
 
-  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify";
+  ac_cv_libcnotify_CPPFLAGS="-I../libcnotify -I\$(top_srcdir)/libcnotify";
   ac_cv_libcnotify_LIBADD="../libcnotify/libcnotify.la";
 
   ac_cv_libcnotify=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCNOTIFY 1" >>confdefs.h
@@ -32575,15 +32600,15 @@
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
@@ -33298,15 +33323,16 @@
 
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
@@ -33331,15 +33357,15 @@
 
 fi
 
 
     if test "x$ac_cv_libcsplit" != xyes
 then :
 
-  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit";
+  ac_cv_libcsplit_CPPFLAGS="-I../libcsplit -I\$(top_srcdir)/libcsplit";
   ac_cv_libcsplit_LIBADD="../libcsplit/libcsplit.la";
 
   ac_cv_libcsplit=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCSPLIT 1" >>confdefs.h
@@ -33409,15 +33435,15 @@
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
@@ -40619,15 +40645,16 @@
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
@@ -40652,15 +40679,15 @@
 
 fi
 
 
     if test "x$ac_cv_libuna" != xyes
 then :
 
-  ac_cv_libuna_CPPFLAGS="-I../libuna";
+  ac_cv_libuna_CPPFLAGS="-I../libuna -I\$(top_srcdir)/libuna";
   ac_cv_libuna_LIBADD="../libuna/libuna.la";
 
   ac_cv_libuna=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBUNA 1" >>confdefs.h
@@ -40730,15 +40757,15 @@
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
@@ -41919,15 +41946,16 @@
 
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
@@ -42241,15 +42269,15 @@
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
@@ -42319,15 +42347,15 @@
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
@@ -43124,15 +43152,16 @@
 
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
@@ -43322,15 +43351,15 @@
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "Missing function: mkdir
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
 
 
-  ac_cv_libcpath_CPPFLAGS="-I../libcpath";
+  ac_cv_libcpath_CPPFLAGS="-I../libcpath -I\$(top_srcdir)/libcpath";
   ac_cv_libcpath_LIBADD="../libcpath/libcpath.la";
 
   ac_cv_libcpath=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBCPATH 1" >>confdefs.h
@@ -43400,15 +43429,15 @@
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
@@ -45518,15 +45547,16 @@
 
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
@@ -45551,15 +45581,15 @@
 
 fi
 
 
     if test "x$ac_cv_libbfio" != xyes
 then :
 
-  ac_cv_libbfio_CPPFLAGS="-I../libbfio";
+  ac_cv_libbfio_CPPFLAGS="-I../libbfio -I\$(top_srcdir)/libbfio";
   ac_cv_libbfio_LIBADD="../libbfio/libbfio.la";
 
   ac_cv_libbfio=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBBFIO 1" >>confdefs.h
@@ -45629,15 +45659,15 @@
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
@@ -46549,15 +46579,16 @@
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
@@ -46650,15 +46681,15 @@
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
@@ -46728,15 +46759,15 @@
 printf "%s\n" "$ac_cv_with_libfdata" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfdata" = xno
 then :
   ac_cv_libfdata=no
 else $as_nop
   ac_cv_libfdata=check
-        if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect
+                if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes
 then :
   if test -d "$ac_cv_with_libfdata"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfdata}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfdata}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -50016,15 +50047,16 @@
 
 
 
         ac_cv_libfdata_LIBADD="-lfdata"
 fi
 
 fi
-    if test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_libfdata" != xyes
+
+    if test "x$ac_cv_libfdata" != xyes && test "x$ac_cv_with_libfdata" != x && test "x$ac_cv_with_libfdata" != xauto-detect && test "x$ac_cv_with_libfdata" != xyes
 then :
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
 printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
 as_fn_error 1 "unable to find supported libfdata in directory: $ac_cv_with_libfdata
 See \`config.log' for more details" "$LINENO" 5; }
 
 fi
@@ -50049,15 +50081,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfdata" != xyes
 then :
 
-  ac_cv_libfdata_CPPFLAGS="-I../libfdata";
+  ac_cv_libfdata_CPPFLAGS="-I../libfdata -I\$(top_srcdir)/libfdata";
   ac_cv_libfdata_LIBADD="../libfdata/libfdata.la";
 
   ac_cv_libfdata=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFDATA 1" >>confdefs.h
@@ -50127,15 +50159,15 @@
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
@@ -50709,15 +50741,16 @@
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
@@ -50742,15 +50775,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfguid" != xyes
 then :
 
-  ac_cv_libfguid_CPPFLAGS="-I../libfguid";
+  ac_cv_libfguid_CPPFLAGS="-I../libfguid -I\$(top_srcdir)/libfguid";
   ac_cv_libfguid_LIBADD="../libfguid/libfguid.la";
 
   ac_cv_libfguid=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFGUID 1" >>confdefs.h
@@ -50820,15 +50853,15 @@
 printf "%s\n" "$ac_cv_with_libfplist" >&6; }
 
   if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_libfplist" = xno
 then :
   ac_cv_libfplist=no
 else $as_nop
   ac_cv_libfplist=check
-        if test "x$ac_cv_with_libfplist" != x && test "x$ac_cv_with_libfplist" != xauto-detect
+                if test "x$ac_cv_with_libfplist" != x && test "x$ac_cv_with_libfplist" != xauto-detect && test "x$ac_cv_with_libfplist" != xyes
 then :
   if test -d "$ac_cv_with_libfplist"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_libfplist}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_libfplist}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -51619,14 +51652,23 @@
 
         ac_cv_libfplist_LIBADD="-lfplist"
 
 fi
 
 fi
 
+    if test "x$ac_cv_libfplist" != xyes && test "x$ac_cv_with_libfplist" != x && test "x$ac_cv_with_libfplist" != xauto-detect && test "x$ac_cv_with_libfplist" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported libfplist in directory: $ac_cv_with_libfplist
+See \`config.log' for more details" "$LINENO" 5; }
+
+fi
+
 fi
 
   if test "x$ac_cv_libfplist" = xyes
 then :
 
 printf "%s\n" "#define HAVE_LIBFPLIST 1" >>confdefs.h
 
@@ -51909,15 +51951,15 @@
 
 
   test -n "$YACC" && break
 done
 test -n "$YACC" || YACC="yacc"
 
 
-  ac_cv_libfplist_CPPFLAGS="-I../libfplist";
+  ac_cv_libfplist_CPPFLAGS="-I../libfplist -I\$(top_srcdir)/libfplist";
   ac_cv_libfplist_LIBADD="../libfplist/libfplist.la";
 
   ac_cv_libfplist=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFPLIST 1" >>confdefs.h
@@ -51987,15 +52029,15 @@
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
@@ -56301,15 +56343,16 @@
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
@@ -56334,15 +56377,15 @@
 
 fi
 
 
     if test "x$ac_cv_libfvalue" != xyes
 then :
 
-  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue";
+  ac_cv_libfvalue_CPPFLAGS="-I../libfvalue -I\$(top_srcdir)/libfvalue";
   ac_cv_libfvalue_LIBADD="../libfvalue/libfvalue.la";
 
   ac_cv_libfvalue=local
 
 
 
 printf "%s\n" "#define HAVE_LOCAL_LIBFVALUE 1" >>confdefs.h
@@ -56412,15 +56455,15 @@
 printf "%s\n" "$ac_cv_with_zlib" >&6; }
 
     if test "x$ac_cv_enable_shared_libs" = xno || test "x$ac_cv_with_zlib" = xno
 then :
   ac_cv_zlib=no
 else $as_nop
   ac_cv_zlib=check
-        if test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect
+                if test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect && test "x$ac_cv_with_zlib" != xyes
 then :
   if test -d "$ac_cv_with_zlib"
 then :
   CFLAGS="$CFLAGS -I${ac_cv_with_zlib}/include"
         LDFLAGS="$LDFLAGS -L${ac_cv_with_zlib}/lib"
 else $as_nop
   { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
@@ -56587,14 +56630,23 @@
 
         ac_cv_zlib_LIBADD="-lz";
 
 fi
 
 fi
 
+    if test "x$ac_cv_zlib" != xyes && test "x$ac_cv_with_zlib" != x && test "x$ac_cv_with_zlib" != xauto-detect && test "x$ac_cv_with_zlib" != xyes
+then :
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "unable to find supported zlib in directory: $ac_cv_with_zlib
+See \`config.log' for more details" "$LINENO" 5; }
+
+fi
+
 fi
 
   if test "x$ac_cv_zlib" = xzlib
 then :
 
 printf "%s\n" "#define HAVE_ZLIB 1" >>confdefs.h
 
@@ -56725,15 +56777,15 @@
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
@@ -57731,15 +57783,16 @@
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
@@ -57845,15 +57898,15 @@
 
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
@@ -62031,15 +62084,15 @@
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
@@ -62109,15 +62162,15 @@
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
@@ -62693,15 +62746,16 @@
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
@@ -62799,15 +62853,15 @@
 
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
@@ -65634,15 +65688,15 @@
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
@@ -65953,16 +66007,20 @@
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
 
@@ -66120,33 +66178,107 @@
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
+else $as_nop
+  { { printf "%s\n" "$as_me:${as_lineno-$LINENO}: error: in \`$ac_pwd':" >&5
+printf "%s\n" "$as_me: error: in \`$ac_pwd':" >&2;}
+as_fn_error 1 "no such directory: $ac_cv_with_libfuse
+See \`config.log' for more details" "$LINENO" 5; }
+
+fi
 else $as_nop
-  { printf "%s\n" "$as_me:${as_lineno-$LINENO}: WARNING: no such directory: $ac_cv_with_libfuse" >&5
-printf "%s\n" "$as_me: WARNING: no such directory: $ac_cv_with_libfuse" >&2;}
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
 fi
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
+fi
+
+
+
+if test $pkg_failed = yes; then
+        { printf "%s\n" "$as_me:${as_lineno-$LINENO}: result: no" >&5
+printf "%s\n" "no" >&6; }
 
+if $PKG_CONFIG --atleast-pkgconfig-version 0.20; then
+        _pkg_short_errors_supported=yes
+else
+        _pkg_short_errors_supported=no
 fi
+        if test $_pkg_short_errors_supported = yes; then
+                fuse3_PKG_ERRORS=`$PKG_CONFIG --short-errors --print-errors --cflags --libs "fuse3 >= 3.0" 2>&1`
+        else
+                fuse3_PKG_ERRORS=`$PKG_CONFIG --print-errors --cflags --libs "fuse3 >= 3.0" 2>&1`
+        fi
+        # Put the nasty error message in config.log where it belongs
+        echo "$fuse3_PKG_ERRORS" >&5
 
-  if test "x$ac_cv_with_libfuse" = xno
-then :
-  ac_cv_libfuse=no
-else $as_nop
-      if test "x$cross_compiling" != "xyes" && test "x$PKGCONFIG" != "x"
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
@@ -66214,51 +66346,110 @@
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
@@ -66421,45 +66612,38 @@
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
@@ -66627,29 +66811,49 @@
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
@@ -66680,14 +66884,20 @@
 
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
 
@@ -66695,14 +66905,22 @@
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
 
@@ -67672,15 +67890,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libfvde $as_me 20240113, which was
+This file was extended by libfvde $as_me 20240502, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -67740,15 +67958,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libfvde config.status 20240113
+libfvde config.status 20240502
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libfvde-20240113/compile` & `libfvde-20240502/compile`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/missing` & `libfvde-20240502/missing`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/libfdata/libfdata.vcproj` & `libfvde-20240502/msvscpp/libfdata/libfdata.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvde_test_encrypted_metadata/fvde_test_encrypted_metadata.vcproj` & `libfvde-20240502/msvscpp/fvde_test_encrypted_metadata/fvde_test_encrypted_metadata.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/libfvde.sln` & `libfvde-20240502/msvscpp/libfvde.sln`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvde_test_segment_descriptor/fvde_test_segment_descriptor.vcproj` & `libfvde-20240502/msvscpp/fvde_test_segment_descriptor/fvde_test_segment_descriptor.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvde_test_support/fvde_test_support.vcproj` & `libfvde-20240502/msvscpp/fvde_test_support/fvde_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/zlib/zlib.vcproj` & `libfvde-20240502/msvscpp/zlib/zlib.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/libfplist/libfplist.vcproj` & `libfvde-20240502/msvscpp/libfplist/libfplist.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvde_test_compression/fvde_test_compression.vcproj` & `libfvde-20240502/msvscpp/fvde_test_compression/fvde_test_compression.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/libcaes/libcaes.vcproj` & `libfvde-20240502/msvscpp/libcaes/libcaes.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/pyfvde/pyfvde.vcproj` & `libfvde-20240502/msvscpp/pyfvde/pyfvde.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/libfguid/libfguid.vcproj` & `libfvde-20240502/msvscpp/libfguid/libfguid.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/libfvde/libfvde.vcproj` & `libfvde-20240502/msvscpp/libfvde/libfvde.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvde_test_logical_volume/fvde_test_logical_volume.vcproj` & `libfvde-20240502/msvscpp/fvde_test_logical_volume/fvde_test_logical_volume.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/libclocale/libclocale.vcproj` & `libfvde-20240502/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvde_test_tools_signal/fvde_test_tools_signal.vcproj` & `libfvde-20240502/msvscpp/fvde_test_tools_signal/fvde_test_tools_signal.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/libfcache/libfcache.vcproj` & `libfvde-20240502/msvscpp/libfcache/libfcache.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/Makefile.am` & `libfvde-20240502/msvscpp/Makefile.am`

 * *Files 5% similar despite different names*

```diff
@@ -50,13 +50,11 @@
 	pyfvde/pyfvde.vcproj \
 	zlib/zlib.vcproj \
 	libfvde.sln
 
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

### Comparing `libfvde-20240113/msvscpp/libbfio/libbfio.vcproj` & `libfvde-20240502/msvscpp/libbfio/libbfio.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvde_test_keyring/fvde_test_keyring.vcproj` & `libfvde-20240502/msvscpp/fvde_test_keyring/fvde_test_keyring.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvde_test_encryption_context/fvde_test_encryption_context.vcproj` & `libfvde-20240502/msvscpp/fvde_test_encryption_context/fvde_test_encryption_context.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvdewipekey/fvdewipekey.vcproj` & `libfvde-20240502/msvscpp/fvdewipekey/fvdewipekey.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvde_test_deflate/fvde_test_deflate.vcproj` & `libfvde-20240502/msvscpp/fvde_test_deflate/fvde_test_deflate.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/libcfile/libcfile.vcproj` & `libfvde-20240502/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvde_test_physical_volume_descriptor/fvde_test_physical_volume_descriptor.vcproj` & `libfvde-20240502/msvscpp/fvde_test_physical_volume_descriptor/fvde_test_physical_volume_descriptor.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/libcdata/libcdata.vcproj` & `libfvde-20240502/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvde_test_logical_volume_descriptor/fvde_test_logical_volume_descriptor.vcproj` & `libfvde-20240502/msvscpp/fvde_test_logical_volume_descriptor/fvde_test_logical_volume_descriptor.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvdeinfo/fvdeinfo.vcproj` & `libfvde-20240502/msvscpp/fvdeinfo/fvdeinfo.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvde_test_volume_data_handle/fvde_test_volume_data_handle.vcproj` & `libfvde-20240502/msvscpp/fvde_test_volume_data_handle/fvde_test_volume_data_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvde_test_volume_header/fvde_test_volume_header.vcproj` & `libfvde-20240502/msvscpp/fvde_test_volume_header/fvde_test_volume_header.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvde_test_metadata_block/fvde_test_metadata_block.vcproj` & `libfvde-20240502/msvscpp/fvde_test_metadata_block/fvde_test_metadata_block.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvde_test_io_handle/fvde_test_io_handle.vcproj` & `libfvde-20240502/msvscpp/fvde_test_io_handle/fvde_test_io_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/libcthreads/libcthreads.vcproj` & `libfvde-20240502/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvde_test_encryption_context_plist/fvde_test_encryption_context_plist.vcproj` & `libfvde-20240502/msvscpp/fvde_test_encryption_context_plist/fvde_test_encryption_context_plist.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/libcpath/libcpath.vcproj` & `libfvde-20240502/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvde_test_sector_data/fvde_test_sector_data.vcproj` & `libfvde-20240502/msvscpp/fvde_test_sector_data/fvde_test_sector_data.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvde_test_error/fvde_test_error.vcproj` & `libfvde-20240502/msvscpp/fvde_test_error/fvde_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvde_test_checksum/fvde_test_checksum.vcproj` & `libfvde-20240502/msvscpp/fvde_test_checksum/fvde_test_checksum.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvde_test_metadata/fvde_test_metadata.vcproj` & `libfvde-20240502/msvscpp/fvde_test_metadata/fvde_test_metadata.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/libhmac/libhmac.vcproj` & `libfvde-20240502/msvscpp/libhmac/libhmac.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvde_test_physical_volume/fvde_test_physical_volume.vcproj` & `libfvde-20240502/msvscpp/fvde_test_physical_volume/fvde_test_physical_volume.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvde_test_bit_stream/fvde_test_bit_stream.vcproj` & `libfvde-20240502/msvscpp/fvde_test_bit_stream/fvde_test_bit_stream.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/libcsplit/libcsplit.vcproj` & `libfvde-20240502/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvde_test_notify/fvde_test_notify.vcproj` & `libfvde-20240502/msvscpp/fvde_test_notify/fvde_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/libuna/libuna.vcproj` & `libfvde-20240502/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/Makefile.in` & `libfvde-20240502/msvscpp/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -432,14 +432,16 @@
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
@@ -561,15 +563,16 @@
 	pyfvde/pyfvde.vcproj \
 	zlib/zlib.vcproj \
 	libfvde.sln
 
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
@@ -673,23 +676,25 @@
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
@@ -768,13 +773,10 @@
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

### Comparing `libfvde-20240113/msvscpp/libfvalue/libfvalue.vcproj` & `libfvde-20240502/msvscpp/libfvalue/libfvalue.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvde_test_huffman_tree/fvde_test_huffman_tree.vcproj` & `libfvde-20240502/msvscpp/fvde_test_huffman_tree/fvde_test_huffman_tree.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvde_test_volume/fvde_test_volume.vcproj` & `libfvde-20240502/msvscpp/fvde_test_volume/fvde_test_volume.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvde_test_tools_output/fvde_test_tools_output.vcproj` & `libfvde-20240502/msvscpp/fvde_test_tools_output/fvde_test_tools_output.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvde_test_volume_group/fvde_test_volume_group.vcproj` & `libfvde-20240502/msvscpp/fvde_test_volume_group/fvde_test_volume_group.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/libcnotify/libcnotify.vcproj` & `libfvde-20240502/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/libcerror/libcerror.vcproj` & `libfvde-20240502/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/msvscpp/fvdemount/fvdemount.vcproj` & `libfvde-20240502/msvscpp/fvdemount/fvdemount.vcproj`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcfile/libcfile_extern.h` & `libfvde-20240502/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcfile/libcfile_support.h` & `libfvde-20240502/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcfile/libcfile_unused.h` & `libfvde-20240502/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcfile/libcfile_notify.h` & `libfvde-20240502/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcfile/libcfile_support.c` & `libfvde-20240502/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcfile/libcfile_types.h` & `libfvde-20240502/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcfile/Makefile.am` & `libfvde-20240502/libcfile/Makefile.am`

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

### Comparing `libfvde-20240113/libcfile/libcfile_notify.c` & `libfvde-20240502/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcfile/libcfile_system_string.h` & `libfvde-20240502/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcfile/libcfile_file.h` & `libfvde-20240502/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcfile/libcfile_libcnotify.h` & `libfvde-20240502/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcfile/libcfile_system_string.c` & `libfvde-20240502/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcfile/libcfile_error.h` & `libfvde-20240502/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcfile/libcfile_libcerror.h` & `libfvde-20240502/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcfile/libcfile_file.c` & `libfvde-20240502/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcfile/libcfile_libclocale.h` & `libfvde-20240502/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcfile/libcfile_winapi.h` & `libfvde-20240502/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcfile/Makefile.in` & `libfvde-20240502/libcfile/Makefile.in`

 * *Files 3% similar despite different names*

```diff
@@ -497,14 +497,16 @@
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
@@ -571,16 +573,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -595,15 +597,16 @@
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
@@ -808,24 +811,32 @@
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
 
@@ -914,17 +925,14 @@
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

### Comparing `libfvde-20240113/libcfile/libcfile_error.c` & `libfvde-20240502/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcfile/libcfile_libuna.h` & `libfvde-20240502/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcfile/libcfile_winapi.c` & `libfvde-20240502/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcfile/libcfile_definitions.h` & `libfvde-20240502/libcfile/libcfile_definitions.h`

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

### Comparing `libfvde-20240113/README` & `libfvde-20240502/README`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/INSTALL` & `libfvde-20240502/INSTALL`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/mount_dokan.c` & `libfvde-20240502/fvdetools/mount_dokan.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/fvdetools_libcnotify.h` & `libfvde-20240502/fvdetools/fvdetools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/mount_file_system.h` & `libfvde-20240502/fvdetools/mount_file_system.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/mount_fuse.c` & `libfvde-20240502/fvdetools/mount_fuse.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/info_handle.h` & `libfvde-20240502/fvdetools/info_handle.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/mount_dokan.h` & `libfvde-20240502/fvdetools/mount_dokan.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/fvdetools_input.h` & `libfvde-20240502/fvdetools/fvdetools_input.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/fvdetools_libcsplit.h` & `libfvde-20240502/fvdetools/fvdetools_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/fvdetools_libclocale.h` & `libfvde-20240502/fvdetools/fvdetools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/fvdetools_libuna.h` & `libfvde-20240502/fvdetools/fvdetools_libuna.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/mount_file_system.c` & `libfvde-20240502/fvdetools/mount_file_system.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/fvdetools_signal.c` & `libfvde-20240502/fvdetools/fvdetools_signal.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/fvdetools_output.c` & `libfvde-20240502/fvdetools/fvdetools_output.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/byte_size_string.c` & `libfvde-20240502/fvdetools/byte_size_string.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/fvdetools_libcpath.h` & `libfvde-20240502/fvdetools/fvdetools_libcpath.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/fvdetools_libfguid.h` & `libfvde-20240502/fvdetools/fvdetools_libfguid.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/Makefile.am` & `libfvde-20240502/fvdetools/Makefile.am`

 * *Files 2% similar despite different names*

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
@@ -122,20 +122,18 @@
 	@LIBCDATA_LIBADD@ \
 	../libfvde/libfvde.la \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
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
 	@echo "Running splint on fvdeinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(fvdeinfo_SOURCES)
 	@echo "Running splint on fvdemount ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(fvdemount_SOURCES)
 	@echo "Running splint on fvdewipekey ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(fvdewipekey_SOURCES)
```

### Comparing `libfvde-20240113/fvdetools/fvdetools_libbfio.h` & `libfvde-20240502/fvdetools/fvdetools_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/fvdetools_libcerror.h` & `libfvde-20240502/fvdetools/fvdetools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/fvdetools_unused.h` & `libfvde-20240502/fvdetools/fvdetools_unused.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/mount_file_entry.c` & `libfvde-20240502/fvdetools/mount_file_entry.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/info_handle.c` & `libfvde-20240502/fvdetools/info_handle.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/mount_file_entry.h` & `libfvde-20240502/fvdetools/mount_file_entry.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/fvdeinfo.c` & `libfvde-20240502/fvdetools/fvdeinfo.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/fvdetools_getopt.h` & `libfvde-20240502/fvdetools/fvdetools_getopt.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/wipekey_handle.c` & `libfvde-20240502/fvdetools/wipekey_handle.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/mount_handle.h` & `libfvde-20240502/fvdetools/mount_handle.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/wipekey_handle.h` & `libfvde-20240502/fvdetools/wipekey_handle.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/fvdetools_getopt.c` & `libfvde-20240502/fvdetools/fvdetools_getopt.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/fvdetools_libcdata.h` & `libfvde-20240502/fvdetools/fvdetools_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/fvdemount.c` & `libfvde-20240502/fvdetools/fvdemount.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/mount_handle.c` & `libfvde-20240502/fvdetools/mount_handle.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/fvdetools_input.c` & `libfvde-20240502/fvdetools/fvdetools_input.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/fvdetools_signal.h` & `libfvde-20240502/fvdetools/fvdetools_signal.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/fvdewipekey.c` & `libfvde-20240502/fvdetools/fvdewipekey.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/fvdetools_libfvde.h` & `libfvde-20240502/fvdetools/fvdetools_libfvde.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/Makefile.in` & `libfvde-20240502/fvdetools/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -508,14 +508,16 @@
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
@@ -582,16 +584,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -703,15 +705,16 @@
 	@LIBCDATA_LIBADD@ \
 	../libfvde/libfvde.la \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
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
@@ -975,23 +978,40 @@
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
+		-rm -f ./$(DEPDIR)/byte_size_string.Po
+	-rm -f ./$(DEPDIR)/fvdeinfo.Po
+	-rm -f ./$(DEPDIR)/fvdemount.Po
+	-rm -f ./$(DEPDIR)/fvdetools_getopt.Po
+	-rm -f ./$(DEPDIR)/fvdetools_input.Po
+	-rm -f ./$(DEPDIR)/fvdetools_output.Po
+	-rm -f ./$(DEPDIR)/fvdetools_signal.Po
+	-rm -f ./$(DEPDIR)/fvdewipekey.Po
+	-rm -f ./$(DEPDIR)/info_handle.Po
+	-rm -f ./$(DEPDIR)/mount_dokan.Po
+	-rm -f ./$(DEPDIR)/mount_file_entry.Po
+	-rm -f ./$(DEPDIR)/mount_file_system.Po
+	-rm -f ./$(DEPDIR)/mount_fuse.Po
+	-rm -f ./$(DEPDIR)/mount_handle.Po
+	-rm -f ./$(DEPDIR)/wipekey_handle.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -1089,17 +1109,14 @@
 	mostlyclean-generic mostlyclean-libtool pdf pdf-am ps ps-am \
 	sources-am sources-local splint-am splint-local tags tags-am \
 	uninstall uninstall-am uninstall-binPROGRAMS
 
 .PRECIOUS: Makefile
 
 
-distclean: clean
-	-rm -f Makefile
-
 splint-local:
 	@echo "Running splint on fvdeinfo ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(fvdeinfo_SOURCES)
 	@echo "Running splint on fvdemount ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(fvdemount_SOURCES)
 	@echo "Running splint on fvdewipekey ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(fvdewipekey_SOURCES)
```

### Comparing `libfvde-20240113/fvdetools/byte_size_string.h` & `libfvde-20240502/fvdetools/byte_size_string.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/fvdetools_i18n.h` & `libfvde-20240502/fvdetools/fvdetools_i18n.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/fvdetools_output.h` & `libfvde-20240502/fvdetools/fvdetools_output.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/fvdetools/mount_fuse.h` & `libfvde-20240502/fvdetools/mount_fuse.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcdata/libcdata_list_element.h` & `libfvde-20240502/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcdata/libcdata_array.h` & `libfvde-20240502/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcdata/libcdata_definitions.h` & `libfvde-20240502/libcdata/libcdata_definitions.h`

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

### Comparing `libfvde-20240113/libcdata/libcdata_libcerror.h` & `libfvde-20240502/libcpath/libcpath_libcerror.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2006-2024, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBCDATA_LIBCERROR_H )
-#define _LIBCDATA_LIBCERROR_H
+#if !defined( _LIBCPATH_LIBCERROR_H )
+#define _LIBCPATH_LIBCERROR_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCERROR for local use of libcerror
  */
 #if defined( HAVE_LOCAL_LIBCERROR )
 
@@ -42,9 +42,9 @@
 #define LIBCERROR_DLL_IMPORT
 #endif
 
 #include <libcerror.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCERROR ) */
 
-#endif /* !defined( _LIBCDATA_LIBCERROR_H ) */
+#endif /* !defined( _LIBCPATH_LIBCERROR_H ) */
```

### Comparing `libfvde-20240113/libcdata/libcdata_unused.h` & `libfvde-20240502/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcdata/libcdata_btree.h` & `libfvde-20240502/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcdata/libcdata_btree.c` & `libfvde-20240502/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcdata/libcdata_support.c` & `libfvde-20240502/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcdata/libcdata_list.c` & `libfvde-20240502/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcdata/libcdata_extern.h` & `libfvde-20240502/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcdata/libcdata_list.h` & `libfvde-20240502/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcdata/libcdata_btree_values_list.h` & `libfvde-20240502/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcdata/Makefile.am` & `libfvde-20240502/libcdata/Makefile.am`

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

### Comparing `libfvde-20240113/libcdata/libcdata_btree_node.h` & `libfvde-20240502/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcdata/libcdata_range_list_value.h` & `libfvde-20240502/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcdata/libcdata_range_list.h` & `libfvde-20240502/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcdata/libcdata_range_list.c` & `libfvde-20240502/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcdata/libcdata_array.c` & `libfvde-20240502/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcdata/libcdata_list_element.c` & `libfvde-20240502/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcdata/libcdata_libcthreads.h` & `libfvde-20240502/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcdata/libcdata_tree_node.h` & `libfvde-20240502/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcdata/libcdata_error.h` & `libfvde-20240502/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcdata/libcdata_types.h` & `libfvde-20240502/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcdata/libcdata_btree_node.c` & `libfvde-20240502/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcdata/libcdata_tree_node.c` & `libfvde-20240502/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcdata/libcdata_support.h` & `libfvde-20240502/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcdata/Makefile.in` & `libfvde-20240502/libcdata/Makefile.in`

 * *Files 3% similar despite different names*

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
@@ -585,16 +587,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -611,15 +613,16 @@
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
@@ -829,24 +832,37 @@
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
 
@@ -940,17 +956,14 @@
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

### Comparing `libfvde-20240113/libcdata/libcdata_range_list_value.c` & `libfvde-20240502/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcdata/libcdata_btree_values_list.c` & `libfvde-20240502/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcdata/libcdata_error.c` & `libfvde-20240502/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/ylwrap` & `libfvde-20240502/ylwrap`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/config.sub` & `libfvde-20240502/config.sub`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/setup.py` & `libfvde-20240502/setup.py`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/acinclude.m4` & `libfvde-20240502/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/config.rpath` & `libfvde-20240502/config.rpath`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcthreads/libcthreads_thread.h` & `libfvde-20240502/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcthreads/libcthreads_read_write_lock.h` & `libfvde-20240502/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcthreads/libcthreads_thread.c` & `libfvde-20240502/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcthreads/libcthreads_thread_pool.h` & `libfvde-20240502/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcthreads/libcthreads_support.h` & `libfvde-20240502/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcthreads/libcthreads_lock.h` & `libfvde-20240502/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcthreads/libcthreads_unused.h` & `libfvde-20240502/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcthreads/libcthreads_lock.c` & `libfvde-20240502/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcthreads/libcthreads_condition.h` & `libfvde-20240502/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcthreads/libcthreads_repeating_thread.h` & `libfvde-20240502/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcthreads/Makefile.am` & `libfvde-20240502/libcthreads/Makefile.am`

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

### Comparing `libfvde-20240113/libcthreads/libcthreads_support.c` & `libfvde-20240502/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcthreads/libcthreads_mutex.c` & `libfvde-20240502/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcthreads/libcthreads_queue.c` & `libfvde-20240502/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcthreads/libcthreads_mutex.h` & `libfvde-20240502/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcthreads/libcthreads_types.h` & `libfvde-20240502/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcthreads/libcthreads_thread_attributes.h` & `libfvde-20240502/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcthreads/libcthreads_condition.c` & `libfvde-20240502/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcthreads/libcthreads_error.c` & `libfvde-20240502/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcthreads/libcthreads_read_write_lock.c` & `libfvde-20240502/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcthreads/libcthreads_libcerror.h` & `libfvde-20240502/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcthreads/libcthreads_definitions.h` & `libfvde-20240502/libcthreads/libcthreads_definitions.h`

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

### Comparing `libfvde-20240113/libcthreads/libcthreads_thread_pool.c` & `libfvde-20240502/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcthreads/libcthreads_error.h` & `libfvde-20240502/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcthreads/libcthreads_thread_attributes.c` & `libfvde-20240502/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcthreads/libcthreads_extern.h` & `libfvde-20240502/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcthreads/libcthreads_repeating_thread.c` & `libfvde-20240502/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcthreads/Makefile.in` & `libfvde-20240502/libcthreads/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -515,14 +515,16 @@
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
@@ -589,16 +591,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -613,15 +615,16 @@
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
@@ -831,24 +834,37 @@
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
 
@@ -942,17 +958,14 @@
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

### Comparing `libfvde-20240113/libcthreads/libcthreads_queue.h` & `libfvde-20240502/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/test-driver` & `libfvde-20240502/test-driver`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcpath/libcpath_support.c` & `libfvde-20240502/libcpath/libcpath_support.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcpath/libcpath_libcerror.h` & `libfvde-20240502/libcsplit/libcsplit_libcerror.h`

 * *Files 3% similar despite different names*

```diff
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBCPATH_LIBCERROR_H )
-#define _LIBCPATH_LIBCERROR_H
+#if !defined( _LIBCSPLIT_LIBCERROR_H )
+#define _LIBCSPLIT_LIBCERROR_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCERROR for local use of libcerror
  */
 #if defined( HAVE_LOCAL_LIBCERROR )
 
@@ -42,9 +42,9 @@
 #define LIBCERROR_DLL_IMPORT
 #endif
 
 #include <libcerror.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCERROR ) */
 
-#endif /* !defined( _LIBCPATH_LIBCERROR_H ) */
+#endif /* !defined( _LIBCSPLIT_LIBCERROR_H ) */
```

### Comparing `libfvde-20240113/libcpath/libcpath_definitions.h` & `libfvde-20240502/libcpath/libcpath_definitions.h`

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

### Comparing `libfvde-20240113/libcpath/Makefile.am` & `libfvde-20240502/libcpath/Makefile.am`

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

### Comparing `libfvde-20240113/libcpath/libcpath_error.c` & `libfvde-20240502/libcpath/libcpath_error.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcpath/libcpath_extern.h` & `libfvde-20240502/libcpath/libcpath_extern.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcpath/libcpath_system_string.h` & `libfvde-20240502/libcpath/libcpath_system_string.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcpath/libcpath_support.h` & `libfvde-20240502/libcpath/libcpath_support.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcpath/libcpath_libcsplit.h` & `libfvde-20240502/libcpath/libcpath_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcpath/libcpath_system_string.c` & `libfvde-20240502/libcpath/libcpath_system_string.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcpath/libcpath_libclocale.h` & `libfvde-20240502/libcpath/libcpath_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcpath/libcpath_error.h` & `libfvde-20240502/libcpath/libcpath_error.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcpath/Makefile.in` & `libfvde-20240502/libcpath/Makefile.in`

 * *Files 2% similar despite different names*

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
@@ -565,16 +567,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -586,15 +588,16 @@
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
@@ -797,24 +800,30 @@
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
 
@@ -901,17 +910,14 @@
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

### Comparing `libfvde-20240113/libcpath/libcpath_libuna.h` & `libfvde-20240502/libcpath/libcpath_libuna.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcpath/libcpath_unused.h` & `libfvde-20240502/libcpath/libcpath_unused.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcpath/libcpath_path.c` & `libfvde-20240502/libcpath/libcpath_path.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcpath/libcpath_path.h` & `libfvde-20240502/libcpath/libcpath_path.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/ChangeLog` & `libfvde-20240502/ChangeLog`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/manuals/libfvde.3` & `libfvde-20240502/manuals/libfvde.3`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/manuals/fvdeinfo.1` & `libfvde-20240502/manuals/fvdeinfo.1`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/manuals/fvdemount.1` & `libfvde-20240502/manuals/fvdemount.1`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/manuals/Makefile.in` & `libfvde-20240502/manuals/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -464,14 +464,16 @@
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
@@ -547,15 +549,16 @@
 	libfvde.3
 
 EXTRA_DIST = \
 	fvdeinfo.1 \
 	fvdemount.1 \
 	libfvde.3
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
 	@for dep in $?; do \
@@ -748,23 +751,25 @@
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
@@ -846,13 +851,10 @@
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

### Comparing `libfvde-20240113/tests/fvde_test_sector_data.c` & `libfvde-20240502/tests/fvde_test_sector_data.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_encryption_context_plist.c` & `libfvde-20240502/tests/fvde_test_encryption_context_plist.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_io_handle.c` & `libfvde-20240502/tests/fvde_test_io_handle.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_keyring.c` & `libfvde-20240502/tests/fvde_test_keyring.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_support.c` & `libfvde-20240502/tests/fvde_test_support.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_macros.h` & `libfvde-20240502/tests/fvde_test_macros.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_checksum.c` & `libfvde-20240502/tests/fvde_test_checksum.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_libfvde.h` & `libfvde-20240502/tests/fvde_test_libfvde.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_logical_volume.c` & `libfvde-20240502/tests/fvde_test_logical_volume.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_libcnotify.h` & `libfvde-20240502/tests/fvde_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_unused.h` & `libfvde-20240502/tests/fvde_test_unused.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_libcdata.h` & `libfvde-20240502/tests/fvde_test_libcdata.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/pyfvde_test_logical_volume.py` & `libfvde-20240502/tests/pyfvde_test_logical_volume.py`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_metadata.c` & `libfvde-20240502/tests/fvde_test_metadata.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/test_tools.sh` & `libfvde-20240502/tests/test_tools.sh`

 * *Files 2% similar despite different names*

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
 
 TOOLS_TESTS="output signal";
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

### Comparing `libfvde-20240113/tests/fvde_test_compression.c` & `libfvde-20240502/tests/fvde_test_compression.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_functions.h` & `libfvde-20240502/tests/fvde_test_functions.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/pyfvde_test_volume.py` & `libfvde-20240502/tests/pyfvde_test_volume.py`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_getopt.c` & `libfvde-20240502/tests/fvde_test_getopt.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_logical_volume_descriptor.c` & `libfvde-20240502/tests/fvde_test_logical_volume_descriptor.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/Makefile.am` & `libfvde-20240502/tests/Makefile.am`

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
@@ -437,13 +437,12 @@
 	@LIBCSPLIT_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libfvde/libfvde.la \
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

### Comparing `libfvde-20240113/tests/fvde_test_functions.c` & `libfvde-20240502/tests/fvde_test_functions.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_segment_descriptor.c` & `libfvde-20240502/tests/fvde_test_segment_descriptor.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_libbfio.h` & `libfvde-20240502/tests/fvde_test_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_libclocale.h` & `libfvde-20240502/tests/fvde_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_memory.c` & `libfvde-20240502/tests/fvde_test_memory.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/pyfvde_test_volume_group.py` & `libfvde-20240502/tests/pyfvde_test_volume_group.py`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_encrypted_metadata.c` & `libfvde-20240502/tests/fvde_test_encrypted_metadata.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/test_python_module.sh` & `libfvde-20240502/tests/test_python_module.sh`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 #!/usr/bin/env bash
 # Tests Python module functions and types.
 #
-# Version: 20231005
+# Version: 20240417
 
 EXIT_SUCCESS=0;
 EXIT_FAILURE=1;
+EXIT_NO_TESTS_RAN=5;
 EXIT_IGNORE=77;
 
 TEST_FUNCTIONS="support";
 TEST_FUNCTIONS_WITH_INPUT="logical_volume physical_volume volume volume_group";
 OPTION_SETS=("offset" "password" "recovery_password");
 
 TEST_TOOL_DIRECTORY=".";
 INPUT_GLOB="*";
 
+LIBRARY_NAME="libfvde";
+PYTHON_MODULE="pyfvde";
+
 test_python_function()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyfvde_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	run_test_with_arguments "${TEST_DESCRIPTION}" "${TEST_SCRIPT}";
 	local RESULT=$?;
 
 	return ${RESULT};
 }
 
 test_python_function_with_input()
 {
 	local TEST_FUNCTION=$1;
 
 	local TEST_DESCRIPTION="Testing Python-bindings functions: ${TEST_FUNCTION}";
-	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/pyfvde_test_${TEST_FUNCTION}.py";
+	local TEST_SCRIPT="${TEST_TOOL_DIRECTORY}/${PYTHON_MODULE}_test_${TEST_FUNCTION}.py";
 
 	if ! test -d "input";
 	then
 		echo "Test input directory not found.";
 
 		return ${EXIT_IGNORE};
 	fi
@@ -45,15 +49,15 @@
 	if test ${RESULT} -eq ${EXIT_SUCCESS};
 	then
 		echo "No files or directories found in the test input directory";
 
 		return ${EXIT_IGNORE};
 	fi
 
-	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "pyfvde");
+	local TEST_PROFILE_DIRECTORY=$(get_test_profile_directory "input" "${PYTHON_MODULE}");
 
 	local IGNORE_LIST=$(read_ignore_list "${TEST_PROFILE_DIRECTORY}");
 
 	RESULT=${EXIT_SUCCESS};
 
 	for TEST_SET_INPUT_DIRECTORY in input/*;
 	do
@@ -120,38 +124,47 @@
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
 
-	if test ${RESULT} -ne ${EXIT_SUCCESS};
+	if test ${RESULT} -eq ${EXIT_NO_TESTS_RAN};
+	then
+		RESULT=${EXIT_IGNORE};
+	fi
+	if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
 	then
 		break;
 	fi
 done
 
 if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
 then
@@ -164,16 +177,19 @@
 	then
 		test_python_function_with_input "${TEST_FUNCTION}";
 		RESULT=$?;
 	else
 		test_python_function "${TEST_FUNCTION}";
 		RESULT=$?;
 	fi
-
-	if test ${RESULT} -ne ${EXIT_SUCCESS};
+	if test ${RESULT} -eq ${EXIT_NO_TESTS_RAN};
+	then
+		RESULT=${EXIT_IGNORE};
+	fi
+	if test ${RESULT} -ne ${EXIT_SUCCESS} && test ${RESULT} -ne ${EXIT_IGNORE};
 	then
 		break;
 	fi
 done
 
 exit ${RESULT};
```

### Comparing `libfvde-20240113/tests/fvde_test_bit_stream.c` & `libfvde-20240502/tests/fvde_test_bit_stream.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_error.c` & `libfvde-20240502/tests/fvde_test_error.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_deflate.c` & `libfvde-20240502/tests/fvde_test_deflate.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_volume_data_handle.c` & `libfvde-20240502/tests/fvde_test_volume_data_handle.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_tools_output.c` & `libfvde-20240502/tests/fvde_test_tools_output.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_physical_volume.c` & `libfvde-20240502/tests/fvde_test_physical_volume.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/pyfvde_test_physical_volume.py` & `libfvde-20240502/tests/pyfvde_test_physical_volume.py`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/test_runner.sh` & `libfvde-20240502/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_metadata_block.c` & `libfvde-20240502/tests/fvde_test_metadata_block.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_memory.h` & `libfvde-20240502/tests/fvde_test_memory.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/test_fvdeinfo.sh` & `libfvde-20240502/tests/test_fvdeinfo.sh`

 * *Files 4% similar despite different names*

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
 
 PROFILES=("fvdeinfo");
 OPTIONS_PER_PROFILE=("-u");
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

### Comparing `libfvde-20240113/tests/fvde_test_getopt.h` & `libfvde-20240502/tests/fvde_test_getopt.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_physical_volume_descriptor.c` & `libfvde-20240502/tests/fvde_test_physical_volume_descriptor.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/pyfvde_test_support.py` & `libfvde-20240502/tests/pyfvde_test_support.py`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_huffman_tree.c` & `libfvde-20240502/tests/fvde_test_huffman_tree.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_notify.c` & `libfvde-20240502/tests/fvde_test_notify.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_volume_header.c` & `libfvde-20240502/tests/fvde_test_volume_header.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_tools_signal.c` & `libfvde-20240502/tests/fvde_test_tools_signal.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/Makefile.in` & `libfvde-20240502/tests/Makefile.in`

 * *Files 4% similar despite different names*

```diff
@@ -902,14 +902,16 @@
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
@@ -977,16 +979,16 @@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -1386,16 +1388,18 @@
 	@LIBCSPLIT_LIBADD@ \
 	@LIBCNOTIFY_LIBADD@ \
 	@LIBCLOCALE_LIBADD@ \
 	@LIBCDATA_LIBADD@ \
 	../libfvde/libfvde.la \
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
@@ -1933,24 +1937,58 @@
 clean-generic:
 
 distclean-generic:
 	-test -z "$(CONFIG_CLEAN_FILES)" || rm -f $(CONFIG_CLEAN_FILES)
 	-test . = "$(srcdir)" || test -z "$(CONFIG_CLEAN_VPATH_FILES)" || rm -f $(CONFIG_CLEAN_VPATH_FILES)
 	-rm -f ../fvdetools/$(DEPDIR)/$(am__dirstamp)
 	-rm -f ../fvdetools/$(am__dirstamp)
+	-test -z "$(DISTCLEANFILES)" || rm -f $(DISTCLEANFILES)
 
 maintainer-clean-generic:
 	@echo "This command is intended for maintainers to use"
 	@echo "it deletes files that may require special tools to rebuild."
-	-test -z "$(MAINTAINERCLEANFILES)" || rm -f $(MAINTAINERCLEANFILES)
 clean: clean-am
 
 clean-am: clean-checkPROGRAMS clean-generic clean-libtool \
 	mostlyclean-am
 
+distclean: distclean-am
+		-rm -f ../fvdetools/$(DEPDIR)/fvdetools_output.Po
+	-rm -f ../fvdetools/$(DEPDIR)/fvdetools_signal.Po
+	-rm -f ./$(DEPDIR)/fvde_test_bit_stream.Po
+	-rm -f ./$(DEPDIR)/fvde_test_checksum.Po
+	-rm -f ./$(DEPDIR)/fvde_test_compression.Po
+	-rm -f ./$(DEPDIR)/fvde_test_deflate.Po
+	-rm -f ./$(DEPDIR)/fvde_test_encrypted_metadata.Po
+	-rm -f ./$(DEPDIR)/fvde_test_encryption_context.Po
+	-rm -f ./$(DEPDIR)/fvde_test_encryption_context_plist.Po
+	-rm -f ./$(DEPDIR)/fvde_test_error.Po
+	-rm -f ./$(DEPDIR)/fvde_test_functions.Po
+	-rm -f ./$(DEPDIR)/fvde_test_getopt.Po
+	-rm -f ./$(DEPDIR)/fvde_test_huffman_tree.Po
+	-rm -f ./$(DEPDIR)/fvde_test_io_handle.Po
+	-rm -f ./$(DEPDIR)/fvde_test_keyring.Po
+	-rm -f ./$(DEPDIR)/fvde_test_logical_volume.Po
+	-rm -f ./$(DEPDIR)/fvde_test_logical_volume_descriptor.Po
+	-rm -f ./$(DEPDIR)/fvde_test_memory.Po
+	-rm -f ./$(DEPDIR)/fvde_test_metadata.Po
+	-rm -f ./$(DEPDIR)/fvde_test_metadata_block.Po
+	-rm -f ./$(DEPDIR)/fvde_test_notify.Po
+	-rm -f ./$(DEPDIR)/fvde_test_physical_volume.Po
+	-rm -f ./$(DEPDIR)/fvde_test_physical_volume_descriptor.Po
+	-rm -f ./$(DEPDIR)/fvde_test_sector_data.Po
+	-rm -f ./$(DEPDIR)/fvde_test_segment_descriptor.Po
+	-rm -f ./$(DEPDIR)/fvde_test_support.Po
+	-rm -f ./$(DEPDIR)/fvde_test_tools_output.Po
+	-rm -f ./$(DEPDIR)/fvde_test_tools_signal.Po
+	-rm -f ./$(DEPDIR)/fvde_test_volume.Po
+	-rm -f ./$(DEPDIR)/fvde_test_volume_data_handle.Po
+	-rm -f ./$(DEPDIR)/fvde_test_volume_group.Po
+	-rm -f ./$(DEPDIR)/fvde_test_volume_header.Po
+	-rm -f Makefile
 distclean-am: clean-am distclean-compile distclean-generic \
 	distclean-tags
 
 dvi: dvi-am
 
 dvi-am:
 
@@ -2065,13 +2103,10 @@
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

### Comparing `libfvde-20240113/tests/fvde_test_libcerror.h` & `libfvde-20240502/tests/fvde_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_volume.c` & `libfvde-20240502/tests/fvde_test_volume.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_volume_group.c` & `libfvde-20240502/tests/fvde_test_volume_group.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_libuna.h` & `libfvde-20240502/tests/fvde_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/fvde_test_encryption_context.c` & `libfvde-20240502/tests/fvde_test_encryption_context.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/tests/test_library.sh` & `libfvde-20240502/tests/test_library.sh`

 * *Files 6% similar despite different names*

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
 
 LIBRARY_TESTS="bit_stream checksum compression deflate encrypted_metadata encryption_context encryption_context_plist error huffman_tree io_handle keyring logical_volume logical_volume_descriptor metadata metadata_block notify physical_volume physical_volume_descriptor sector_data segment_descriptor volume_data_handle volume_group volume_header";
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

### Comparing `libfvde-20240113/ossfuzz/volume_fuzzer.cc` & `libfvde-20240502/ossfuzz/volume_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/ossfuzz/Makefile.am` & `libfvde-20240502/ossfuzz/Makefile.am`

 * *Files 9% similar despite different names*

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
 	../libfvde/libfvde.la \
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

### Comparing `libfvde-20240113/ossfuzz/ossfuzz_libbfio.h` & `libfvde-20240502/ossfuzz/ossfuzz_libbfio.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/ossfuzz/Makefile.in` & `libfvde-20240502/ossfuzz/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -504,14 +504,16 @@
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
@@ -578,16 +580,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -607,15 +609,16 @@
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	@LIBCDATA_LIBADD@ \
 @HAVE_LIB_FUZZING_ENGINE_TRUE@	../libfvde/libfvde.la \
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
@@ -857,23 +860,26 @@
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
 
@@ -957,17 +963,14 @@
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

### Comparing `libfvde-20240113/ossfuzz/ossfuzz_libfvde.h` & `libfvde-20240502/ossfuzz/ossfuzz_libfvde.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/ltmain.sh` & `libfvde-20240502/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libfvde.pc.in` & `libfvde-20240502/libfvde.pc.in`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libhmac/libhmac_sha1_context.c` & `libfvde-20240502/libhmac/libhmac_sha1_context.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA1 context functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libhmac/libhmac_sha224.h` & `libfvde-20240502/libhmac/libhmac_sha224.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-224 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libhmac/libhmac_sha512_context.c` & `libfvde-20240502/libhmac/libhmac_sha512_context.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-512 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libhmac/libhmac_extern.h` & `libfvde-20240502/libhmac/libhmac_extern.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libhmac/libhmac_md5.c` & `libfvde-20240502/libhmac/libhmac_md5.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MD5 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libhmac/libhmac_md5.h` & `libfvde-20240502/libhmac/libhmac_md5.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MD5 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libhmac/libhmac_error.h` & `libfvde-20240502/libhmac/libhmac_error.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libhmac/libhmac_types.h` & `libfvde-20240502/libhmac/libhmac_types.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libhmac/libhmac_byte_stream.h` & `libfvde-20240502/libhmac/libhmac_byte_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Byte stream functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libhmac/libhmac_sha512.c` & `libfvde-20240502/libhmac/libhmac_sha512.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-512 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libhmac/libhmac_sha256_context.c` & `libfvde-20240502/libhmac/libhmac_sha256_context.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-256 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libhmac/libhmac_sha224.c` & `libfvde-20240502/libhmac/libhmac_sha224.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-224 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libhmac/libhmac_definitions.h` & `libfvde-20240502/libhmac/libhmac_definitions.h`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -30,19 +30,19 @@
 #if !defined( HAVE_LOCAL_LIBHMAC )
 #include <libhmac/definitions.h>
 
 /* The definitions in <libhmac/definitions.h> are copied here
  * for local use of libhmac
  */
 #else
-#define LIBHMAC_VERSION			20231127
+#define LIBHMAC_VERSION			20240417
 
 /* The libhmac version string
  */
-#define LIBHMAC_VERSION_STRING		"20231127"
+#define LIBHMAC_VERSION_STRING		"20240417"
 
 /* The digest hash sizes
  */
 #define LIBHMAC_MD5_HASH_SIZE		16
 #define LIBHMAC_SHA1_HASH_SIZE		20
 #define LIBHMAC_SHA224_HASH_SIZE	28
 #define LIBHMAC_SHA256_HASH_SIZE	32
```

### Comparing `libfvde-20240113/libhmac/libhmac_unused.h` & `libfvde-20240502/libhmac/libhmac_unused.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libhmac/libhmac_sha1.h` & `libfvde-20240502/libhmac/libhmac_sha1.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA1 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libhmac/libhmac_sha256_context.h` & `libfvde-20240502/libhmac/libhmac_sha256_context.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-256 context functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libhmac/Makefile.am` & `libfvde-20240502/libhmac/Makefile.am`

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

### Comparing `libfvde-20240113/libhmac/libhmac_sha224_context.c` & `libfvde-20240502/libhmac/libhmac_sha224_context.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-224 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libhmac/libhmac_md5_context.h` & `libfvde-20240502/libhmac/libhmac_md5_context.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MD5 context functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libhmac/libhmac_sha256.c` & `libfvde-20240502/libhmac/libhmac_sha256.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-256 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libhmac/libhmac_sha1_context.h` & `libfvde-20240502/libhmac/libhmac_sha1_context.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA1 context functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libhmac/libhmac_libcerror.h` & `libfvde-20240502/libfvalue/libfvalue_libcerror.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBHMAC_LIBCERROR_H )
-#define _LIBHMAC_LIBCERROR_H
+#if !defined( _LIBFVALUE_LIBCERROR_H )
+#define _LIBFVALUE_LIBCERROR_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCERROR for local use of libcerror
  */
 #if defined( HAVE_LOCAL_LIBCERROR )
 
@@ -42,9 +42,9 @@
 #define LIBCERROR_DLL_IMPORT
 #endif
 
 #include <libcerror.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCERROR ) */
 
-#endif /* !defined( _LIBHMAC_LIBCERROR_H ) */
+#endif /* !defined( _LIBFVALUE_LIBCERROR_H ) */
```

### Comparing `libfvde-20240113/libhmac/libhmac_error.c` & `libfvde-20240502/libhmac/libhmac_error.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libhmac/libhmac_support.h` & `libfvde-20240502/libhmac/libhmac_support.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libhmac/Makefile.in` & `libfvde-20240502/libhmac/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -514,14 +514,16 @@
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
@@ -588,16 +590,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -615,15 +617,16 @@
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
@@ -834,24 +837,38 @@
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
 
@@ -946,17 +963,14 @@
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

### Comparing `libfvde-20240113/libhmac/libhmac_sha256.h` & `libfvde-20240502/libhmac/libhmac_sha256.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-256 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libhmac/libhmac_sha224_context.h` & `libfvde-20240502/libhmac/libhmac_sha224_context.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-224 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libhmac/libhmac_sha512_context.h` & `libfvde-20240502/libhmac/libhmac_sha512_context.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-512 context functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libhmac/libhmac_sha512.h` & `libfvde-20240502/libhmac/libhmac_sha512.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA-512 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libhmac/libhmac_support.c` & `libfvde-20240502/libuna/libuna_support.c`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -18,22 +18,22 @@
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include <common.h>
 #include <types.h>
 
-#include "libhmac_definitions.h"
-#include "libhmac_support.h"
+#include "libuna_definitions.h"
+#include "libuna_support.h"
 
-#if !defined( HAVE_LOCAL_LIBHMAC )
+#if !defined( HAVE_LOCAL_LIBUNA )
 
 /* Returns the library version as a string
  */
-const char *libhmac_get_version(
+const char *libuna_get_version(
              void )
 {
-	return( (const char *) LIBHMAC_VERSION_STRING );
+	return( (const char *) LIBUNA_VERSION_STRING );
 }
 
-#endif
+#endif /* !defined( HAVE_LOCAL_LIBUNA ) */
```

### Comparing `libfvde-20240113/libhmac/libhmac_sha1.c` & `libfvde-20240502/libhmac/libhmac_sha1.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * SHA1 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libhmac/libhmac_md5_context.c` & `libfvde-20240502/libhmac/libhmac_md5_context.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MD5 functions
  *
- * Copyright (C) 2011-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libcsplit/libcsplit_narrow_string.c` & `libfvde-20240502/libcsplit/libcsplit_narrow_string.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcsplit/libcsplit_definitions.h` & `libfvde-20240502/libcsplit/libcsplit_definitions.h`

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

### Comparing `libfvde-20240113/libcsplit/libcsplit_types.h` & `libfvde-20240502/libcsplit/libcsplit_types.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcsplit/libcsplit_wide_split_string.c` & `libfvde-20240502/libcsplit/libcsplit_wide_split_string.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcsplit/libcsplit_support.h` & `libfvde-20240502/libcsplit/libcsplit_support.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcsplit/Makefile.am` & `libfvde-20240502/libcsplit/Makefile.am`

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

### Comparing `libfvde-20240113/libcsplit/libcsplit_libcerror.h` & `libfvde-20240502/libuna/libuna_libcerror.h`

 * *Files 4% similar despite different names*

```diff
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBCSPLIT_LIBCERROR_H )
-#define _LIBCSPLIT_LIBCERROR_H
+#if !defined( _LIBUNA_LIBCERROR_H )
+#define _LIBUNA_LIBCERROR_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCERROR for local use of libcerror
  */
 #if defined( HAVE_LOCAL_LIBCERROR )
 
@@ -42,9 +42,9 @@
 #define LIBCERROR_DLL_IMPORT
 #endif
 
 #include <libcerror.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCERROR ) */
 
-#endif /* !defined( _LIBCSPLIT_LIBCERROR_H ) */
+#endif /* !defined( _LIBUNA_LIBCERROR_H ) */
```

### Comparing `libfvde-20240113/libcsplit/libcsplit_wide_string.c` & `libfvde-20240502/libcsplit/libcsplit_wide_string.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcsplit/libcsplit_unused.h` & `libfvde-20240502/libcsplit/libcsplit_unused.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcsplit/libcsplit_wide_split_string.h` & `libfvde-20240502/libcsplit/libcsplit_wide_split_string.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcsplit/libcsplit_error.c` & `libfvde-20240502/libcsplit/libcsplit_error.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcsplit/libcsplit_narrow_split_string.c` & `libfvde-20240502/libcsplit/libcsplit_narrow_split_string.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcsplit/libcsplit_extern.h` & `libfvde-20240502/libcsplit/libcsplit_extern.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcsplit/libcsplit_error.h` & `libfvde-20240502/libcsplit/libcsplit_error.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcsplit/libcsplit_support.c` & `libfvde-20240502/libcsplit/libcsplit_support.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcsplit/libcsplit_wide_string.h` & `libfvde-20240502/libcsplit/libcsplit_wide_string.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcsplit/Makefile.in` & `libfvde-20240502/libcsplit/Makefile.in`

 * *Files 2% similar despite different names*

```diff
@@ -501,14 +501,16 @@
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
@@ -575,16 +577,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -593,15 +595,16 @@
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
@@ -806,24 +809,32 @@
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
 
@@ -912,17 +923,14 @@
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

### Comparing `libfvde-20240113/libcsplit/libcsplit_narrow_split_string.h` & `libfvde-20240502/libcsplit/libcsplit_narrow_split_string.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcsplit/libcsplit_narrow_string.h` & `libfvde-20240502/libcsplit/libcsplit_narrow_string.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/po/remove-potcdate.sin` & `libfvde-20240502/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/po/Makefile.in.in` & `libfvde-20240502/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/po/en@quot.header` & `libfvde-20240502/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/po/en@boldquot.header` & `libfvde-20240502/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/po/insert-header.sin` & `libfvde-20240502/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/po/Makevars` & `libfvde-20240502/po/Makevars`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/po/Makevars.in` & `libfvde-20240502/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/po/Rules-quot` & `libfvde-20240502/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libuna/libuna_codepage_windows_1251.c` & `libfvde-20240502/libuna/libuna_codepage_windows_1251.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1251 codepage (Cyrillic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_utf16_string.c` & `libfvde-20240502/libuna/libuna_utf16_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_base16_stream.c` & `libfvde-20240502/libuna/libuna_base16_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base16 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_utf8_stream.h` & `libfvde-20240502/libuna/libuna_utf8_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_iso_8859_2.h` & `libfvde-20240502/libuna/libuna_codepage_iso_8859_2.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-2 codepage (Central European) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_windows_932.c` & `libfvde-20240502/libuna/libuna_codepage_windows_932.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 932 codepage (Japanese Shift-JIS) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_dingbats.h` & `libfvde-20240502/libuna/libuna_codepage_mac_dingbats.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacDingbats codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_utf8_string.c` & `libfvde-20240502/libuna/libuna_utf8_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_base64_stream.c` & `libfvde-20240502/libuna/libuna_base64_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base64 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_error.h` & `libfvde-20240502/libuna/libuna_error.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_turkish.h` & `libfvde-20240502/libuna/libuna_codepage_mac_turkish.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacTurkish codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_unicode_character.c` & `libfvde-20240502/libuna/libuna_unicode_character.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Unicode character functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_gaelic.c` & `libfvde-20240502/libuna/libuna_codepage_mac_gaelic.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacGaelic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_arabic.h` & `libfvde-20240502/libuna/libuna_codepage_mac_arabic.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacArabic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_thai.c` & `libfvde-20240502/libuna/libuna_codepage_mac_thai.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacThai codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_windows_874.h` & `libfvde-20240502/libuna/libuna_codepage_windows_874.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 874 codepage (Thai) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_iso_8859_15.h` & `libfvde-20240502/libuna/libuna_codepage_iso_8859_9.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-15 codepage (Latin 9) functions
+ * ISO 8859-9 codepage (Turkish) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,31 +15,31 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_15_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_15_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_9_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_9_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_15_byte_stream_to_unicode_base_0xa0[ 32 ];
+const uint16_t libuna_codepage_iso_8859_9_byte_stream_to_unicode_base_0xd0[ 48 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_15_unicode_to_byte_stream_base_0x00a0[ 32 ];
+const uint8_t libuna_codepage_iso_8859_9_unicode_to_byte_stream_base_0x00d0[ 48 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_15_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_9_H ) */
```

### Comparing `libfvde-20240113/libuna/libuna_utf8_string.h` & `libfvde-20240502/libuna/libuna_utf8_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_iso_8859_16.c` & `libfvde-20240502/libuna/libuna_codepage_iso_8859_16.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-16 codepage (Latin 10) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_windows_1255.c` & `libfvde-20240502/libuna/libuna_codepage_windows_1255.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1255 codepage (Hebrew) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_utf7_stream.c` & `libfvde-20240502/libuna/libuna_utf7_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-7 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_byte_stream.h` & `libfvde-20240502/libuna/libuna_byte_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Byte stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_koi8_u.c` & `libfvde-20240502/libuna/libuna_codepage_koi8_u.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * KOI8-U codepage (Ukrainian Cyrillic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_unused.h` & `libfvde-20240502/libuna/libuna_unused.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_iso_8859_6.c` & `libfvde-20240502/libuna/libuna_codepage_iso_8859_6.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-6 codepage (Arabic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_iso_8859_14.c` & `libfvde-20240502/libuna/libuna_codepage_iso_8859_14.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-14 codepage (Celtic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_base64_stream.h` & `libfvde-20240502/libuna/libuna_base64_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base64 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_error.c` & `libfvde-20240502/libuna/libuna_error.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_centraleurroman.h` & `libfvde-20240502/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCentralEurRoman codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_romanian.c` & `libfvde-20240502/libuna/libuna_codepage_mac_romanian.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRomanian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_iso_8859_6.h` & `libfvde-20240502/libuna/libuna_codepage_iso_8859_6.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-6 codepage (Arabic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_iso_8859_9.c` & `libfvde-20240502/libuna/libuna_codepage_iso_8859_9.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-9 codepage (Turkish) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_russian.h` & `libfvde-20240502/libuna/libuna_codepage_mac_russian.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRussian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_dingbats.c` & `libfvde-20240502/libuna/libuna_codepage_mac_dingbats.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacDingbats codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_iso_8859_15.c` & `libfvde-20240502/libuna/libuna_codepage_iso_8859_15.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-15 codepage (Latin 9) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_windows_936.c` & `libfvde-20240502/libuna/libuna_codepage_windows_936.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 936 codepage (Chinese Simplified) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_croatian.h` & `libfvde-20240502/libuna/libuna_codepage_mac_croatian.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCroatian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_scsu.h` & `libfvde-20240502/libuna/libuna_scsu.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Standard Compression Scheme for Unicode (SCSU) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/Makefile.am` & `libfvde-20240502/libuna/Makefile.am`

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
@@ -73,17 +73,17 @@
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
-	/bin/rm -f Makefile
+sources-local: $(BUILT_SOURCES)
 
-splint:
+splint-local:
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
```

### Comparing `libfvde-20240113/libuna/libuna_utf32_stream.c` & `libfvde-20240502/libuna/libuna_utf32_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-32 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_windows_936.h` & `libfvde-20240502/libuna/libuna_codepage_windows_936.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 936 codepage (Chinese Simplified) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_iso_8859_10.c` & `libfvde-20240502/libuna/libuna_codepage_iso_8859_10.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-10 codepage (Nordic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_roman.c` & `libfvde-20240502/libuna/libuna_codepage_mac_roman.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRoman codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_utf7_stream.h` & `libfvde-20240502/libuna/libuna_utf7_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-7 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_iso_8859_3.h` & `libfvde-20240502/libuna/libuna_codepage_iso_8859_3.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-3 codepage (Latin 3) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_thai.h` & `libfvde-20240502/libuna/libuna_codepage_mac_thai.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacThai codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_farsi.h` & `libfvde-20240502/libuna/libuna_codepage_mac_farsi.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacFarsi codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_ukrainian.c` & `libfvde-20240502/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacUkrainian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_inuit.c` & `libfvde-20240502/libuna/libuna_codepage_mac_inuit.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacInuit codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_windows_932.h` & `libfvde-20240502/libuna/libuna_codepage_windows_932.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 932 codepage (Japanese Shift-JIS) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_windows_874.c` & `libfvde-20240502/libuna/libuna_codepage_windows_874.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 874 codepage (Thai) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_iso_8859_5.c` & `libfvde-20240502/libuna/libuna_codepage_iso_8859_5.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-5 codepage (Cyrillic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_iso_8859_10.h` & `libfvde-20240502/libuna/libuna_codepage_iso_8859_10.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-10 codepage (Nordic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_definitions.h` & `libfvde-20240502/libuna/libuna_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -31,19 +31,19 @@
 
 /* The definitions in <libuna/definitions.h> are copied here
  * for local use of libuna
  */
 #else
 #include <byte_stream.h>
 
-#define LIBUNA_VERSION						20230710
+#define LIBUNA_VERSION						20240414
 
 /* The libuna version string
  */
-#define LIBUNA_VERSION_STRING					"20230710"
+#define LIBUNA_VERSION_STRING					"20240414"
 
 /* The endian definitions
  */
 #define	LIBUNA_ENDIAN_BIG					_BYTE_STREAM_ENDIAN_BIG
 #define	LIBUNA_ENDIAN_LITTLE					_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The codepage definitions
```

### Comparing `libfvde-20240113/libuna/libuna_url_stream.h` & `libfvde-20240502/libuna/libuna_url_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Percent or URL encoded stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_icelandic.h` & `libfvde-20240502/libuna/libuna_codepage_mac_icelandic.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacIcelandic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_koi8_u.h` & `libfvde-20240502/libuna/libuna_codepage_koi8_u.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * KOI8-U codepage (Ukrainian Cyrillic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_utf16_stream.c` & `libfvde-20240502/libuna/libuna_utf16_stream.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_windows_1253.c` & `libfvde-20240502/libuna/libuna_codepage_windows_1253.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1253 codepage (Greek) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_iso_8859_4.h` & `libfvde-20240502/libuna/libuna_codepage_iso_8859_4.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-4 codepage (Baltic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_greek.c` & `libfvde-20240502/libuna/libuna_codepage_mac_greek.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacGreek codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_libcerror.h` & `libfvde-20240502/libhmac/libhmac_libcerror.h`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2011-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_LIBCERROR_H )
-#define _LIBUNA_LIBCERROR_H
+#if !defined( _LIBHMAC_LIBCERROR_H )
+#define _LIBHMAC_LIBCERROR_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCERROR for local use of libcerror
  */
 #if defined( HAVE_LOCAL_LIBCERROR )
 
@@ -42,9 +42,9 @@
 #define LIBCERROR_DLL_IMPORT
 #endif
 
 #include <libcerror.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCERROR ) */
 
-#endif /* !defined( _LIBUNA_LIBCERROR_H ) */
+#endif /* !defined( _LIBHMAC_LIBCERROR_H ) */
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_centraleurroman.c` & `libfvde-20240502/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCentralEurRoman codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_windows_1254.c` & `libfvde-20240502/libuna/libuna_codepage_windows_1254.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1254 codepage (Turkish) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_iso_8859_13.h` & `libfvde-20240502/libuna/libuna_codepage_iso_8859_13.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-13 codepage (Baltic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_iso_8859_7.h` & `libfvde-20240502/libuna/libuna_codepage_iso_8859_7.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-7 codepage (Greek) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_windows_1255.h` & `libfvde-20240502/libuna/libuna_codepage_windows_1251.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Windows 1255 codepage (Hebrew) functions
+ * Windows 1251 codepage (Cyrillic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1255_H )
-#define _LIBUNA_CODEPAGE_WINDOWS_1255_H
+#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1251_H )
+#define _LIBUNA_CODEPAGE_WINDOWS_1251_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_windows_1255_copy_from_byte_stream(
+int libuna_codepage_windows_1251_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_windows_1255_copy_to_byte_stream(
+int libuna_codepage_windows_1251_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1255_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1251_H ) */
```

### Comparing `libfvde-20240113/libuna/libuna_unicode_character.h` & `libfvde-20240502/libuna/libuna_unicode_character.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Unicode character functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_iso_8859_8.h` & `libfvde-20240502/libuna/libuna_codepage_iso_8859_8.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-8 codepage (Hebrew) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_iso_8859_13.c` & `libfvde-20240502/libuna/libuna_codepage_iso_8859_13.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-13 codepage (Baltic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_windows_949.h` & `libfvde-20240502/libuna/libuna_codepage_windows_949.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 949 codepage (Korean) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_cyrillic.c` & `libfvde-20240502/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCyrillic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_celtic.c` & `libfvde-20240502/libuna/libuna_codepage_mac_celtic.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCeltic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_support.h` & `libfvde-20240502/libuna/libuna_support.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_iso_8859_4.c` & `libfvde-20240502/libuna/libuna_codepage_iso_8859_4.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-4 codepage (Baltic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_windows_949.c` & `libfvde-20240502/libuna/libuna_codepage_windows_949.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 949 codepage (Korean) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_utf16_stream.h` & `libfvde-20240502/libuna/libuna_utf16_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_symbol.c` & `libfvde-20240502/libuna/libuna_codepage_mac_symbol.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacSymbol codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_roman.h` & `libfvde-20240502/libuna/libuna_codepage_mac_roman.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRoman codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_windows_1257.c` & `libfvde-20240502/libuna/libuna_codepage_windows_1257.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1257 codepage (Baltic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_windows_1254.h` & `libfvde-20240502/libuna/libuna_codepage_windows_1254.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1254 codepage (Turkish) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_windows_950.c` & `libfvde-20240502/libuna/libuna_codepage_windows_950.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 950 codepage (Traditional Chinese) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_extern.h` & `libfvde-20240502/libuna/libuna_extern.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_windows_1256.c` & `libfvde-20240502/libuna/libuna_codepage_windows_1256.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1256 codepage (Arabic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_types.h` & `libfvde-20240502/libuna/libuna_types.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_base32_stream.h` & `libfvde-20240502/libuna/libuna_base32_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base32 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_windows_1253.h` & `libfvde-20240502/libuna/libuna_codepage_windows_1253.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1253 codepage (Greek) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_iso_8859_16.h` & `libfvde-20240502/libuna/libuna_codepage_iso_8859_16.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-16 codepage (Latin 10) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_utf8_stream.c` & `libfvde-20240502/libuna/libuna_utf8_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_windows_1250.h` & `libfvde-20240502/libuna/libuna_codepage_windows_1250.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1250 codepage (Central European) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_iso_8859_2.c` & `libfvde-20240502/libuna/libuna_codepage_iso_8859_2.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-2 codepage (Central European) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_support.c` & `libfvde-20240502/libcerror/libcerror_support.c`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -18,22 +18,22 @@
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include <common.h>
 #include <types.h>
 
-#include "libuna_definitions.h"
-#include "libuna_support.h"
+#include "libcerror_definitions.h"
+#include "libcerror_support.h"
 
-#if !defined( HAVE_LOCAL_LIBUNA )
+#if !defined( HAVE_LOCAL_LIBCERROR )
 
 /* Returns the library version as a string
  */
-const char *libuna_get_version(
+const char *libcerror_get_version(
              void )
 {
-	return( (const char *) LIBUNA_VERSION_STRING );
+	return( (const char *) LIBCERROR_VERSION_STRING );
 }
 
-#endif /* !defined( HAVE_LOCAL_LIBUNA ) */
+#endif /* !defined( HAVE_LOCAL_LIBCERROR ) */
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_koi8_r.c` & `libfvde-20240502/libuna/libuna_codepage_koi8_r.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * KOI8-R codepage (Russian Cyrillic) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_iso_8859_5.h` & `libfvde-20240502/libuna/libuna_codepage_iso_8859_15.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-5 codepage (Cyrillic) functions
+ * ISO 8859-15 codepage (Latin 9) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,31 +15,31 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_5_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_5_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_15_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_15_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_5_byte_stream_to_unicode_base_0xa0[ 96 ];
+const uint16_t libuna_codepage_iso_8859_15_byte_stream_to_unicode_base_0xa0[ 32 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_5_unicode_to_byte_stream_base_0x0400[ 96 ];
+const uint8_t libuna_codepage_iso_8859_15_unicode_to_byte_stream_base_0x00a0[ 32 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_5_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_15_H ) */
```

### Comparing `libfvde-20240113/libuna/libuna_utf16_string.h` & `libfvde-20240502/libuna/libuna_utf16_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_utf32_string.c` & `libfvde-20240502/libuna/libuna_utf32_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-32 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_icelandic.c` & `libfvde-20240502/libuna/libuna_codepage_mac_icelandic.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacIcelandic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_windows_1256.h` & `libfvde-20240502/libuna/libuna_codepage_windows_1256.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1256 codepage (Arabic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_utf32_string.h` & `libfvde-20240502/libuna/libuna_utf32_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-32 string functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_romanian.h` & `libfvde-20240502/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * MacRomanian codepage functions
+ * MacCyrillic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_MAC_ROMANIAN_H )
-#define _LIBUNA_CODEPAGE_MAC_ROMANIAN_H
+#if !defined( _LIBUNA_CODEPAGE_MAC_CYRILLIC_H )
+#define _LIBUNA_CODEPAGE_MAC_CYRILLIC_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_mac_romanian_copy_from_byte_stream(
+int libuna_codepage_mac_cyrillic_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_mac_romanian_copy_to_byte_stream(
+int libuna_codepage_mac_cyrillic_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_MAC_ROMANIAN_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_MAC_CYRILLIC_H ) */
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_iso_8859_8.c` & `libfvde-20240502/libuna/libuna_codepage_iso_8859_8.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-8 codepage (Hebrew) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_koi8_r.h` & `libfvde-20240502/libuna/libuna_codepage_koi8_r.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * KOI8-R codepage (Russian Cyrillic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_cyrillic.h` & `libfvde-20240502/libuna/libuna_codepage_mac_gaelic.h`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * MacCyrillic codepage functions
+ * MacGaelic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_MAC_CYRILLIC_H )
-#define _LIBUNA_CODEPAGE_MAC_CYRILLIC_H
+#if !defined( _LIBUNA_CODEPAGE_MAC_GAELIC_H )
+#define _LIBUNA_CODEPAGE_MAC_GAELIC_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_mac_cyrillic_copy_from_byte_stream(
+int libuna_codepage_mac_gaelic_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_mac_cyrillic_copy_to_byte_stream(
+int libuna_codepage_mac_gaelic_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_MAC_CYRILLIC_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_MAC_GAELIC_H ) */
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_arabic.c` & `libfvde-20240502/libuna/libuna_codepage_mac_arabic.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacArabic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_croatian.c` & `libfvde-20240502/libuna/libuna_codepage_mac_croatian.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCroatian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_iso_8859_9.h` & `libfvde-20240502/libuna/libuna_codepage_iso_8859_5.h`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * ISO 8859-9 codepage (Turkish) functions
+ * ISO 8859-5 codepage (Cyrillic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,31 +15,31 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_ISO_8859_9_H )
-#define _LIBUNA_CODEPAGE_ISO_8859_9_H
+#if !defined( _LIBUNA_CODEPAGE_ISO_8859_5_H )
+#define _LIBUNA_CODEPAGE_ISO_8859_5_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_extern.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 LIBUNA_EXTERN_VARIABLE \
-const uint16_t libuna_codepage_iso_8859_9_byte_stream_to_unicode_base_0xd0[ 48 ];
+const uint16_t libuna_codepage_iso_8859_5_byte_stream_to_unicode_base_0xa0[ 96 ];
 
 LIBUNA_EXTERN_VARIABLE \
-const uint8_t libuna_codepage_iso_8859_9_unicode_to_byte_stream_base_0x00d0[ 48 ];
+const uint8_t libuna_codepage_iso_8859_5_unicode_to_byte_stream_base_0x0400[ 96 ];
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_9_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_ISO_8859_5_H ) */
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_greek.h` & `libfvde-20240502/libuna/libuna_codepage_mac_greek.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacGreek codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_windows_1258.h` & `libfvde-20240502/libuna/libuna_codepage_windows_1258.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1258 codepage (Vietnamese) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_iso_8859_7.c` & `libfvde-20240502/libuna/libuna_codepage_iso_8859_7.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-7 codepage (Greek) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/Makefile.in` & `libfvde-20240502/libuna/Makefile.in`

 * *Files 14% similar despite different names*

```diff
@@ -669,14 +669,16 @@
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
@@ -743,16 +745,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -818,15 +820,16 @@
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
@@ -1088,24 +1091,89 @@
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
 
@@ -1225,14 +1293,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -1243,23 +1313,22 @@
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
 	@echo "Running splint on libuna ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libuna_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_iso_8859_3.c` & `libfvde-20240502/libuna/libuna_codepage_iso_8859_3.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-3 codepage (Latin 3) function
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_windows_1250.c` & `libfvde-20240502/libuna/libuna_codepage_windows_1250.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1250 codepage (Central European) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_scsu.c` & `libfvde-20240502/libuna/libuna_scsu.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Standard Compression Scheme for Unicode (SCSU) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_windows_1252.c` & `libfvde-20240502/libuna/libuna_codepage_windows_1252.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1252 codepage (Western European/Latin 1) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_turkish.c` & `libfvde-20240502/libuna/libuna_codepage_mac_turkish.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacTurkish codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_ukrainian.h` & `libfvde-20240502/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacUkrainian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_russian.c` & `libfvde-20240502/libuna/libuna_codepage_mac_russian.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacRussian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_windows_1258.c` & `libfvde-20240502/libuna/libuna_codepage_windows_1258.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1258 codepage (Vietnamese) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_celtic.h` & `libfvde-20240502/libuna/libuna_codepage_mac_celtic.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacCeltic codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_byte_stream.c` & `libfvde-20240502/libuna/libuna_byte_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Byte stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_gaelic.h` & `libfvde-20240502/libuna/libuna_codepage_windows_1257.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * MacGaelic codepage functions
+ * Windows 1257 codepage (Baltic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_MAC_GAELIC_H )
-#define _LIBUNA_CODEPAGE_MAC_GAELIC_H
+#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1257_H )
+#define _LIBUNA_CODEPAGE_WINDOWS_1257_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_mac_gaelic_copy_from_byte_stream(
+int libuna_codepage_windows_1257_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_mac_gaelic_copy_to_byte_stream(
+int libuna_codepage_windows_1257_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_MAC_GAELIC_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1257_H ) */
```

### Comparing `libfvde-20240113/libuna/libuna_utf32_stream.h` & `libfvde-20240502/libuna/libuna_utf32_stream.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-32 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_symbol.h` & `libfvde-20240502/libuna/libuna_codepage_mac_symbol.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacSymbol codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_windows_1257.h` & `libfvde-20240502/libuna/libuna_codepage_mac_inuit.h`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Windows 1257 codepage (Baltic) functions
+ * MacInuit codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1257_H )
-#define _LIBUNA_CODEPAGE_WINDOWS_1257_H
+#if !defined( _LIBUNA_CODEPAGE_MAC_INUIT_H )
+#define _LIBUNA_CODEPAGE_MAC_INUIT_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_windows_1257_copy_from_byte_stream(
+int libuna_codepage_mac_inuit_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_windows_1257_copy_to_byte_stream(
+int libuna_codepage_mac_inuit_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1257_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_MAC_INUIT_H ) */
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_inuit.h` & `libfvde-20240502/libuna/libuna_codepage_mac_romanian.h`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * MacInuit codepage functions
+ * MacRomanian codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_MAC_INUIT_H )
-#define _LIBUNA_CODEPAGE_MAC_INUIT_H
+#if !defined( _LIBUNA_CODEPAGE_MAC_ROMANIAN_H )
+#define _LIBUNA_CODEPAGE_MAC_ROMANIAN_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_mac_inuit_copy_from_byte_stream(
+int libuna_codepage_mac_romanian_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_mac_inuit_copy_to_byte_stream(
+int libuna_codepage_mac_romanian_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_MAC_INUIT_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_MAC_ROMANIAN_H ) */
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_mac_farsi.c` & `libfvde-20240502/libuna/libuna_codepage_mac_farsi.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * MacFarsi codepage functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_windows_950.h` & `libfvde-20240502/libuna/libuna_codepage_windows_950.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 950 codepage (Traditional Chinese) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_url_stream.c` & `libfvde-20240502/libuna/libuna_url_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Percent or URL encoded stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_windows_1251.h` & `libfvde-20240502/libuna/libuna_codepage_windows_1255.h`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
- * Windows 1251 codepage (Cyrillic) functions
+ * Windows 1255 codepage (Hebrew) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,40 +15,40 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1251_H )
-#define _LIBUNA_CODEPAGE_WINDOWS_1251_H
+#if !defined( _LIBUNA_CODEPAGE_WINDOWS_1255_H )
+#define _LIBUNA_CODEPAGE_WINDOWS_1255_H
 
 #include <common.h>
 #include <types.h>
 
 #include "libuna_libcerror.h"
 #include "libuna_types.h"
 
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
-int libuna_codepage_windows_1251_copy_from_byte_stream(
+int libuna_codepage_windows_1255_copy_from_byte_stream(
      libuna_unicode_character_t *unicode_character,
      const uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
-int libuna_codepage_windows_1251_copy_to_byte_stream(
+int libuna_codepage_windows_1255_copy_to_byte_stream(
      libuna_unicode_character_t unicode_character,
      uint8_t *byte_stream,
      size_t byte_stream_size,
      size_t *byte_stream_index,
      libcerror_error_t **error );
 
 #if defined( __cplusplus )
 }
 #endif
 
-#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1251_H ) */
+#endif /* !defined( _LIBUNA_CODEPAGE_WINDOWS_1255_H ) */
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_windows_1252.h` & `libfvde-20240502/libuna/libuna_codepage_windows_1252.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Windows 1252 codepage (Western European/Latin 1) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_codepage_iso_8859_14.h` & `libfvde-20240502/libuna/libuna_codepage_iso_8859_14.h`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * ISO 8859-14 codepage (Celtic) functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_base16_stream.h` & `libfvde-20240502/libuna/libuna_base16_stream.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base16 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libuna/libuna_base32_stream.c` & `libfvde-20240502/libuna/libuna_base32_stream.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Base32 stream functions
  *
- * Copyright (C) 2008-2023, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/Makefile.in` & `libfvde-20240502/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -551,14 +551,16 @@
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
@@ -691,16 +693,23 @@
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
+	libfvde.pc \
+	libfvde.spec \
+	Makefile \
+	Makefile.in \
+	po/Makevars
 
 pkgconfigdir = $(libdir)/pkgconfig
 pkgconfig_DATA = \
 	libfvde.pc
 
 all: all-recursive
 
@@ -1117,23 +1126,26 @@
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
 
@@ -1247,22 +1259,10 @@
 	(cd $(srcdir)/libfvalue && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfplist && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libhmac && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libcaes && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/libfvde && $(MAKE) $(AM_MAKEFLAGS))
 	(cd $(srcdir)/po && $(MAKE) $(AM_MAKEFLAGS))
 
-distclean: clean
-	-rm -f Makefile
-	-rm -f config.status
-	-rm -f config.cache
-	-rm -f config.log
-	-rm -f libfvde.pc
-	-rm -f libfvde.spec
-	@for dir in ${subdirs}; do \
-		(cd $$dir && $(MAKE) distclean) \
-		|| case "$(MFLAGS)" in *k*) fail=yes;; *) exit 1;; esac; \
-	done && test -z "$$fail"
-
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_filetime.c` & `libfvde-20240502/libfvalue/libfvalue_filetime.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Filetime functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_utf16_string.c` & `libfvde-20240502/libfvalue/libfvalue_utf16_string.c`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 string value functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -32,22 +32,22 @@
 int libfvalue_utf16_string_split(
      const uint16_t *utf16_string,
      size_t utf16_string_size,
      uint16_t delimiter,
      libfvalue_split_utf16_string_t **split_string,
      libcerror_error_t **error )
 {
-	uint16_t *segment_start = NULL;
-	uint16_t *segment_end   = NULL;
-	uint16_t *string_end    = NULL;
-	static char *function   = "libfvalue_utf16_string_split";
-	size_t string_size      = 0;
-	ssize_t segment_length  = 0;
-	int number_of_segments  = 0;
-	int segment_index       = 0;
+	uint16_t *segment_end      = NULL;
+	uint16_t *segment_start    = NULL;
+	const uint16_t *string_end = NULL;
+	static char *function      = "libfvalue_utf16_string_split";
+	size_t string_size         = 0;
+	ssize_t segment_length     = 0;
+	int number_of_segments     = 0;
+	int segment_index          = 0;
 
 	if( utf16_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -92,18 +92,22 @@
 	/* An empty string has no segments
 	 */
 	if( ( utf16_string_size == 0 )
 	 || ( utf16_string[ 0 ] == 0 ) )
 	{
 		return( 1 );
 	}
+	if( utf16_string[ utf16_string_size - 1 ] == 0 )
+	{
+		utf16_string_size--;
+	}
 	/* Determine the number of segments
 	 */
 	segment_start = (uint16_t *) utf16_string;
-	string_end    = (uint16_t *) &( utf16_string[ utf16_string_size - 1 ] );
+	string_end    = utf16_string + utf16_string_size;
 
 	do
 	{
 		segment_end = segment_start;
 
 		while( segment_end <= string_end )
 		{
@@ -142,15 +146,15 @@
 	while( segment_end != NULL );
 
 	number_of_segments = segment_index;
 
 	if( libfvalue_split_utf16_string_initialize(
 	     split_string,
 	     utf16_string,
-	     utf16_string_size,
+	     utf16_string_size + 1,
 	     number_of_segments,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_INITIALIZE_FAILED,
@@ -212,15 +216,15 @@
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
 		 "%s: invalid string size value out of bounds.",
 		 function );
 
 		goto on_error;
 	}
-	string_end = &( segment_start[ string_size - 1 ] );
+	string_end = segment_start + utf16_string_size;
 
 	for( segment_index = 0;
 	     segment_index < number_of_segments;
 	     segment_index++ )
 	{
 		segment_end = segment_start;
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_libfwnt.h` & `libfvde-20240502/libfvalue/libfvalue_libfwnt.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libfwnt header wrapper
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_value.c` & `libfvde-20240502/libfvalue/libfvalue_value.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Value functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_value.h` & `libfvde-20240502/libfvalue/libfvalue_value.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Value functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_definitions.h` & `libfvde-20240502/libfvalue/libfvalue_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal definitions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -32,19 +32,19 @@
 
 /* The definitions in <libfvalue/definitions.h> are copied here
  * for local use of libfvalue
  */
 #else
 #include <byte_stream.h>
 
-#define LIBFVALUE_VERSION						20220120
+#define LIBFVALUE_VERSION						20240415
 
 /* The libfvalue version string
  */
-#define LIBFVALUE_VERSION_STRING					"20220120"
+#define LIBFVALUE_VERSION_STRING					"20240415"
 
 /* The endian definitions
  */
 #define LIBFVALUE_ENDIAN_BIG						_BYTE_STREAM_ENDIAN_BIG
 #define LIBFVALUE_ENDIAN_LITTLE						_BYTE_STREAM_ENDIAN_LITTLE
 #define LIBFVALUE_ENDIAN_NATIVE						(uint8_t) 'n'
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_codepage.h` & `libfvde-20240502/libfvalue/libfvalue_codepage.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Codepage functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_split_utf16_string.c` & `libfvde-20240502/libfvalue/libfvalue_split_utf16_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Split UTF-16 string functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_error.c` & `libfvde-20240502/libfvalue/libfvalue_error.c`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_utf8_string.c` & `libfvde-20240502/libfvalue/libfvalue_utf8_string.c`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 string value functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -32,22 +32,22 @@
 int libfvalue_utf8_string_split(
      const uint8_t *utf8_string,
      size_t utf8_string_size,
      uint8_t delimiter,
      libfvalue_split_utf8_string_t **split_string,
      libcerror_error_t **error )
 {
-	uint8_t *segment_start = NULL;
-	uint8_t *segment_end   = NULL;
-	uint8_t *string_end    = NULL;
-	static char *function  = "libfvalue_utf8_string_split";
-	size_t string_size     = 0;
-	ssize_t segment_length = 0;
-	int number_of_segments = 0;
-	int segment_index      = 0;
+	uint8_t *segment_end      = NULL;
+	uint8_t *segment_start    = NULL;
+	const uint8_t *string_end = NULL;
+	static char *function     = "libfvalue_utf8_string_split";
+	size_t string_size        = 0;
+	ssize_t segment_length    = 0;
+	int number_of_segments    = 0;
+	int segment_index         = 0;
 
 	if( utf8_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_ARGUMENTS,
 		 LIBCERROR_ARGUMENT_ERROR_INVALID_VALUE,
@@ -92,18 +92,22 @@
 	/* An empty string has no segments
 	 */
 	if( ( utf8_string_size == 0 )
 	 || ( utf8_string[ 0 ] == 0 ) )
 	{
 		return( 1 );
 	}
+	if( utf8_string[ utf8_string_size - 1 ] == 0 )
+	{
+		utf8_string_size--;
+	}
 	/* Determine the number of segments
 	 */
 	segment_start = (uint8_t *) utf8_string;
-	string_end    = (uint8_t *) &( utf8_string[ utf8_string_size - 1 ] );
+	string_end    = utf8_string + utf8_string_size;
 
 	do
 	{
 		segment_end = segment_start;
 
 		while( segment_end <= string_end )
 		{
@@ -142,15 +146,15 @@
 	while( segment_end != NULL );
 
 	number_of_segments = segment_index;
 
 	if( libfvalue_split_utf8_string_initialize(
 	     split_string,
 	     utf8_string,
-	     utf8_string_size,
+	     utf8_string_size + 1,
 	     number_of_segments,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_INITIALIZE_FAILED,
@@ -212,15 +216,15 @@
 		 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 		 LIBCERROR_RUNTIME_ERROR_VALUE_OUT_OF_BOUNDS,
 		 "%s: invalid string size value out of bounds.",
 		 function );
 
 		goto on_error;
 	}
-	string_end = &( segment_start[ string_size - 1 ] );
+	string_end = segment_start + utf8_string_size;
 
 	for( segment_index = 0;
 	     segment_index < number_of_segments;
 	     segment_index++ )
 	{
 		segment_end = segment_start;
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_unused.h` & `libfvde-20240502/libfvalue/libfvalue_unused.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Definitions to silence compiler warnings about unused function attributes/parameters.
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_split_utf16_string.h` & `libfvde-20240502/libfvalue/libfvalue_split_utf16_string.h`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Split UTF-16 string functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -25,14 +25,21 @@
 #include <common.h>
 #include <types.h>
 
 #include "libfvalue_extern.h"
 #include "libfvalue_libcerror.h"
 #include "libfvalue_types.h"
 
+#if defined( __CYGWIN__ ) || defined( __MINGW32__ )
+
+/* This inclusion is needed otherwise some linkers mess up exporting the UTF-16 string functions.
+ */
+#include "libfvalue_utf16_string.h"
+#endif
+
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 typedef struct libfvalue_internal_split_utf16_string libfvalue_internal_split_utf16_string_t;
 
 struct libfvalue_internal_split_utf16_string
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_filetime.h` & `libfvde-20240502/libfvalue/libfvalue_filetime.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Filetime functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_support.c` & `libfvde-20240502/libcnotify/libcnotify_support.c`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -18,24 +18,22 @@
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include <common.h>
 #include <types.h>
 
-#include <stdio.h>
+#include "libcnotify_definitions.h"
+#include "libcnotify_support.h"
 
-#include "libfvalue_definitions.h"
-#include "libfvalue_support.h"
-
-#if !defined( HAVE_LOCAL_LIBFVALUE )
+#if !defined( HAVE_LOCAL_LIBCNOTIFY )
 
 /* Returns the library version as a string
  */
-const char *libfvalue_get_version(
+const char *libcnotify_get_version(
              void )
 {
-	return( (const char *) LIBFVALUE_VERSION_STRING );
+	return( (const char *) LIBCNOTIFY_VERSION_STRING );
 }
 
-#endif
+#endif /* !defined( HAVE_LOCAL_LIBCNOTIFY ) */
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_extern.h` & `libfvde-20240502/libfvalue/libfvalue_extern.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal extern definition
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/Makefile.am` & `libfvde-20240502/libfvalue/Makefile.am`

 * *Files 4% similar despite different names*

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
 	@LIBFGUID_CPPFLAGS@ \
 	@PTHREAD_CPPFLAGS@ 
@@ -25,31 +25,31 @@
 	libfvalue_libcdata.h \
 	libfvalue_libcerror.h \
 	libfvalue_libcnotify.h \
 	libfvalue_libfdatetime.h \
 	libfvalue_libfguid.h \
 	libfvalue_libfwnt.h \
 	libfvalue_libuna.h \
-	libfvalue_split_utf16_string.c libfvalue_split_utf16_string.h \
 	libfvalue_split_utf8_string.c libfvalue_split_utf8_string.h \
+	libfvalue_split_utf16_string.c libfvalue_split_utf16_string.h \
 	libfvalue_string.c libfvalue_string.h \
 	libfvalue_types.h \
 	libfvalue_table.c libfvalue_table.h \
 	libfvalue_value.c libfvalue_value.h \
 	libfvalue_value_entry.c libfvalue_value_entry.h \
 	libfvalue_value_type.c libfvalue_value_type.h \
 	libfvalue_support.c libfvalue_support.h \
 	libfvalue_unused.h \
-	libfvalue_utf16_string.c libfvalue_utf16_string.h \
-	libfvalue_utf8_string.c libfvalue_utf8_string.h
+	libfvalue_utf8_string.c libfvalue_utf8_string.h \
+	libfvalue_utf16_string.c libfvalue_utf16_string.h
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
 	@echo "Running splint on libfvalue ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfvalue_la_SOURCES)
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_value_type.h` & `libfvde-20240502/libfvalue/libfvalue_value_type.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Value type functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_libcerror.h` & `libfvde-20240502/libfplist/libfplist_libcerror.h`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcerror header wrapper
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2016-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -15,16 +15,16 @@
  * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
  * GNU General Public License for more details.
  *
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
-#if !defined( _LIBFVALUE_LIBCERROR_H )
-#define _LIBFVALUE_LIBCERROR_H
+#if !defined( _LIBFPLIST_LIBCERROR_H )
+#define _LIBFPLIST_LIBCERROR_H
 
 #include <common.h>
 
 /* Define HAVE_LOCAL_LIBCERROR for local use of libcerror
  */
 #if defined( HAVE_LOCAL_LIBCERROR )
 
@@ -42,9 +42,9 @@
 #define LIBCERROR_DLL_IMPORT
 #endif
 
 #include <libcerror.h>
 
 #endif /* defined( HAVE_LOCAL_LIBCERROR ) */
 
-#endif /* !defined( _LIBFVALUE_LIBCERROR_H ) */
+#endif /* !defined( _LIBFPLIST_LIBCERROR_H ) */
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_split_utf8_string.c` & `libfvde-20240502/libfvalue/libfvalue_split_utf8_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Split UTF-8 string functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_data_handle.h` & `libfvde-20240502/libfvalue/libfvalue_data_handle.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Data handle functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_libcnotify.h` & `libfvde-20240502/libfvalue/libfvalue_libcnotify.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal libcnotify header
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_data_handle.c` & `libfvde-20240502/libfvalue/libfvalue_data_handle.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Data handle functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_integer.c` & `libfvde-20240502/libfvalue/libfvalue_integer.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Integer value functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -1888,16 +1888,16 @@
 	static char *function          = "libfvalue_utf16_string_with_index_copy_to_integer";
 	size_t maximum_string_index    = 0;
 	size_t safe_utf16_string_index = 0;
 	uint64_t divider               = 0;
 	uint64_t value_64bit           = 0;
 	uint32_t string_format_type    = 0;
 	uint32_t supported_flags       = 0;
+	uint16_t character_value       = 0;
 	uint8_t byte_value             = 0;
-	uint8_t character_value        = 0;
 	int8_t bit_shift               = 0;
 	int8_t sign                    = 1;
 
 	if( utf16_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
@@ -2551,18 +2551,18 @@
      libcerror_error_t **error )
 {
 	static char *function          = "libfvalue_utf32_string_with_index_copy_to_integer";
 	size_t maximum_string_index    = 0;
 	size_t safe_utf32_string_index = 0;
 	uint64_t divider               = 0;
 	uint64_t value_64bit           = 0;
+	uint32_t character_value       = 0;
 	uint32_t string_format_type    = 0;
 	uint32_t supported_flags       = 0;
 	uint8_t byte_value             = 0;
-	uint8_t character_value        = 0;
 	int8_t bit_shift               = 0;
 	int8_t sign                    = 1;
 
 	if( utf32_string == NULL )
 	{
 		libcerror_error_set(
 		 error,
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_value_type.c` & `libfvde-20240502/libfvalue/libfvalue_value_type.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Value functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_integer.h` & `libfvde-20240502/libfvalue/libfvalue_integer.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Integer value functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_binary_data.h` & `libfvde-20240502/libfvalue/libfvalue_binary_data.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Binary data value functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_value_entry.h` & `libfvde-20240502/libfvalue/libfvalue_value_entry.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Value entry functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_utf16_string.h` & `libfvde-20240502/libfvalue/libfvalue_utf16_string.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-16 string value functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_error.h` & `libfvde-20240502/libfvalue/libfvalue_error.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Error functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_table.h` & `libfvde-20240502/libfvalue/libfvalue_table.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Values table functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_libfguid.h` & `libfvde-20240502/libfvalue/libfvalue_libfguid.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libfguid header wrapper
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_split_utf8_string.h` & `libfvde-20240502/libfvalue/libfvalue_split_utf8_string.h`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Split UTF-8 string functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -25,14 +25,21 @@
 #include <common.h>
 #include <types.h>
 
 #include "libfvalue_extern.h"
 #include "libfvalue_libcerror.h"
 #include "libfvalue_types.h"
 
+#if defined( __CYGWIN__ ) || defined( __MINGW32__ )
+
+/* This inclusion is needed otherwise some linkers mess up exporting the UTF-8 string functions.
+ */
+#include "libfvalue_utf8_string.h"
+#endif
+
 #if defined( __cplusplus )
 extern "C" {
 #endif
 
 typedef struct libfvalue_internal_split_utf8_string libfvalue_internal_split_utf8_string_t;
 
 struct libfvalue_internal_split_utf8_string
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_floating_point.h` & `libfvde-20240502/libfvalue/libfvalue_floating_point.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Floating point value (IEEE 754) functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_libfdatetime.h` & `libfvde-20240502/libfvalue/libfvalue_libfdatetime.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libfdatetime header wrapper
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_string.h` & `libfvde-20240502/libfvalue/libfvalue_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * String value functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_binary_data.c` & `libfvde-20240502/libfvalue/libfvalue_binary_data.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Binary data value functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_value_entry.c` & `libfvde-20240502/libfvalue/libfvalue_value_entry.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Value entry functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_libcdata.h` & `libfvde-20240502/libfvalue/libfvalue_libcdata.h`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libcdata header wrapper
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_support.h` & `libfvde-20240502/libfvalue/libfvalue_support.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_table.c` & `libfvde-20240502/libfvalue/libfvalue_table.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Values table functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/Makefile.in` & `libfvde-20240502/libfvalue/Makefile.in`

 * *Files 7% similar despite different names*

```diff
@@ -127,41 +127,41 @@
 	libfvalue_definitions.h libfvalue_error.c libfvalue_error.h \
 	libfvalue_extern.h libfvalue_filetime.c libfvalue_filetime.h \
 	libfvalue_floating_point.c libfvalue_floating_point.h \
 	libfvalue_integer.c libfvalue_integer.h libfvalue_libcdata.h \
 	libfvalue_libcerror.h libfvalue_libcnotify.h \
 	libfvalue_libfdatetime.h libfvalue_libfguid.h \
 	libfvalue_libfwnt.h libfvalue_libuna.h \
-	libfvalue_split_utf16_string.c libfvalue_split_utf16_string.h \
 	libfvalue_split_utf8_string.c libfvalue_split_utf8_string.h \
+	libfvalue_split_utf16_string.c libfvalue_split_utf16_string.h \
 	libfvalue_string.c libfvalue_string.h libfvalue_types.h \
 	libfvalue_table.c libfvalue_table.h libfvalue_value.c \
 	libfvalue_value.h libfvalue_value_entry.c \
 	libfvalue_value_entry.h libfvalue_value_type.c \
 	libfvalue_value_type.h libfvalue_support.c libfvalue_support.h \
-	libfvalue_unused.h libfvalue_utf16_string.c \
-	libfvalue_utf16_string.h libfvalue_utf8_string.c \
-	libfvalue_utf8_string.h
+	libfvalue_unused.h libfvalue_utf8_string.c \
+	libfvalue_utf8_string.h libfvalue_utf16_string.c \
+	libfvalue_utf16_string.h
 @HAVE_LOCAL_LIBFVALUE_TRUE@am_libfvalue_la_OBJECTS =  \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_binary_data.lo \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_data_handle.lo \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_error.lo \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_filetime.lo \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_floating_point.lo \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_integer.lo \
-@HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_split_utf16_string.lo \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_split_utf8_string.lo \
+@HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_split_utf16_string.lo \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_string.lo \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_table.lo \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_value.lo \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_value_entry.lo \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_value_type.lo \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_support.lo \
-@HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_utf16_string.lo \
-@HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_utf8_string.lo
+@HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_utf8_string.lo \
+@HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_utf16_string.lo
 libfvalue_la_OBJECTS = $(am_libfvalue_la_OBJECTS)
 AM_V_lt = $(am__v_lt_@AM_V@)
 am__v_lt_ = $(am__v_lt_@AM_DEFAULT_V@)
 am__v_lt_0 = --silent
 am__v_lt_1 = 
 @HAVE_LOCAL_LIBFVALUE_TRUE@am_libfvalue_la_rpath =
 AM_V_P = $(am__v_P_@AM_V@)
@@ -532,14 +532,16 @@
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
@@ -606,16 +608,16 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@LIBFGUID_CPPFLAGS@ \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	@PTHREAD_CPPFLAGS@ 
@@ -634,28 +636,29 @@
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_libcdata.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_libcerror.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_libcnotify.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_libfdatetime.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_libfguid.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_libfwnt.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_libuna.h \
-@HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_split_utf16_string.c libfvalue_split_utf16_string.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_split_utf8_string.c libfvalue_split_utf8_string.h \
+@HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_split_utf16_string.c libfvalue_split_utf16_string.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_string.c libfvalue_string.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_types.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_table.c libfvalue_table.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_value.c libfvalue_value.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_value_entry.c libfvalue_value_entry.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_value_type.c libfvalue_value_type.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_support.c libfvalue_support.h \
 @HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_unused.h \
-@HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_utf16_string.c libfvalue_utf16_string.h \
-@HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_utf8_string.c libfvalue_utf8_string.h
+@HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_utf8_string.c libfvalue_utf8_string.h \
+@HAVE_LOCAL_LIBFVALUE_TRUE@	libfvalue_utf16_string.c libfvalue_utf16_string.h
 
-MAINTAINERCLEANFILES = \
+DISTCLEANFILES = \
+	Makefile \
 	Makefile.in
 
 all: all-am
 
 .SUFFIXES:
 .SUFFIXES: .c .lo .o .obj
 $(srcdir)/Makefile.in:  $(srcdir)/Makefile.am  $(am__configure_deps)
@@ -870,24 +873,42 @@
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
 
@@ -960,14 +981,16 @@
 
 ps-am:
 
 sources: sources-am
 
 sources-am: sources-local
 
+splint: splint-am
+
 splint-am: splint-local
 
 uninstall-am:
 
 .MAKE: install-am install-strip
 
 .PHONY: CTAGS GTAGS TAGS all all-am am--depfiles check check-am clean \
@@ -978,23 +1001,22 @@
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
 	@echo "Running splint on libfvalue ..."
 	-splint -preproc -redef $(DEFS) $(DEFAULT_INCLUDES) $(INCLUDES) $(AM_CPPFLAGS) $(libfvalue_la_SOURCES)
 
 # Tell versions [3.59,3.63) of GNU make to not export all variables.
 # Otherwise a system limit (for SysV at least) may be exceeded.
 .NOEXPORT:
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_utf8_string.h` & `libfvde-20240502/libfvalue/libfvalue_utf8_string.h`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * UTF-8 string value functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_floating_point.c` & `libfvde-20240502/libfvalue/libfvalue_floating_point.c`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Floating point value (IEEE 754) functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -1976,20 +1976,20 @@
 		 "%s: unsupported string format type.",
 		 function );
 
 		return( -1 );
 	}
 	if( string_format_type == LIBFVALUE_FLOATING_POINT_FORMAT_TYPE_HEXADECIMAL )
 	{
-		number_of_characters = (uint16_t) ( floating_point_value_size >> 2 ) + 3;
+		number_of_characters = (uint8_t) ( floating_point_value_size >> 2 ) + 3;
 	}
 	else
 	{
-		bit_shift = (uint16_t) ( floating_point_value_size - 1 );
-		is_signed = (uint16_t) ( floating_point_value >> bit_shift );
+		bit_shift = (int8_t) ( floating_point_value_size - 1 );
+		is_signed = (uint8_t) ( floating_point_value >> bit_shift );
 
 		if( is_signed != 0 )
 		{
 			floating_point_value &= ~( (uint64_t) 1 << bit_shift );
 		}
 		switch( floating_point_value_size )
 		{
@@ -2114,15 +2114,15 @@
 		return( -1 );
 	}
 	if( string_format_type == LIBFVALUE_FLOATING_POINT_FORMAT_TYPE_HEXADECIMAL )
 	{
 		utf16_string[ safe_utf16_string_index++ ] = (uint16_t) '0';
 		utf16_string[ safe_utf16_string_index++ ] = (uint16_t) 'x';
 
-		bit_shift = (uint16_t) ( floating_point_value_size - 4 );
+		bit_shift = (int8_t) ( floating_point_value_size - 4 );
 
 		do
 		{
 			byte_value = (uint16_t) ( ( floating_point_value >> bit_shift ) & 0x0f );
 
 			if( byte_value <= 9 )
 			{
@@ -2286,16 +2286,16 @@
 	size_t fraction_index          = 0;
 	size_t maximum_string_index    = 0;
 	size_t safe_utf16_string_index = 0;
 	uint64_t divider               = 0;
 	uint64_t value_64bit           = 0;
 	uint32_t string_format_type    = 0;
 	uint32_t supported_flags       = 0;
+	uint16_t character_value       = 0;
 	uint8_t byte_value             = 0;
-	uint8_t character_value        = 0;
 	int8_t bit_shift               = 0;
 	int8_t sign                    = 1;
 	double value_fraction          = 0.0;
 
 	if( utf16_string == NULL )
 	{
 		libcerror_error_set(
@@ -2431,15 +2431,15 @@
 	}
 	value_64bit = 0;
 
 	if( string_format_type == LIBFVALUE_FLOATING_POINT_FORMAT_TYPE_HEXADECIMAL )
 	{
 		character_value = utf16_string[ safe_utf16_string_index++ ];
 
-		if(character_value != (uint16_t) '0' )
+		if( character_value != (uint16_t) '0' )
 		{
 			libcerror_error_set(
 			 error,
 			 LIBCERROR_ERROR_DOMAIN_RUNTIME,
 			 LIBCERROR_RUNTIME_ERROR_UNSUPPORTED_VALUE,
 			 "%s: unsupported character value: 0x%02" PRIx16 " at index: %d.",
 			 function,
@@ -2793,20 +2793,20 @@
 		 "%s: unsupported string format type.",
 		 function );
 
 		return( -1 );
 	}
 	if( string_format_type == LIBFVALUE_FLOATING_POINT_FORMAT_TYPE_HEXADECIMAL )
 	{
-		number_of_characters = (uint32_t) ( floating_point_value_size >> 2 ) + 3;
+		number_of_characters = (uint8_t) ( floating_point_value_size >> 2 ) + 3;
 	}
 	else
 	{
-		bit_shift = (uint32_t) ( floating_point_value_size - 1 );
-		is_signed = (uint32_t) ( floating_point_value >> bit_shift );
+		bit_shift = (int8_t) ( floating_point_value_size - 1 );
+		is_signed = (uint8_t) ( floating_point_value >> bit_shift );
 
 		if( is_signed != 0 )
 		{
 			floating_point_value &= ~( (uint64_t) 1 << bit_shift );
 		}
 		switch( floating_point_value_size )
 		{
@@ -2931,15 +2931,15 @@
 		return( -1 );
 	}
 	if( string_format_type == LIBFVALUE_FLOATING_POINT_FORMAT_TYPE_HEXADECIMAL )
 	{
 		utf32_string[ safe_utf32_string_index++ ] = (uint32_t) '0';
 		utf32_string[ safe_utf32_string_index++ ] = (uint32_t) 'x';
 
-		bit_shift = (uint32_t) ( floating_point_value_size - 4 );
+		bit_shift = (int8_t) ( floating_point_value_size - 4 );
 
 		do
 		{
 			byte_value = (uint32_t) ( ( floating_point_value >> bit_shift ) & 0x0f );
 
 			if( byte_value <= 9 )
 			{
@@ -3101,18 +3101,18 @@
 
 	static char *function          = "libfvalue_utf32_string_with_index_copy_to_floating_point";
 	size_t fraction_index          = 0;
 	size_t maximum_string_index    = 0;
 	size_t safe_utf32_string_index = 0;
 	uint64_t divider               = 0;
 	uint64_t value_64bit           = 0;
+	uint32_t character_value       = 0;
 	uint32_t string_format_type    = 0;
 	uint32_t supported_flags       = 0;
 	uint8_t byte_value             = 0;
-	uint8_t character_value        = 0;
 	int8_t bit_shift               = 0;
 	int8_t sign                    = 1;
 	double value_fraction          = 0.0;
 
 	if( utf32_string == NULL )
 	{
 		libcerror_error_set(
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_types.h` & `libfvde-20240502/libfvalue/libfvalue_types.h`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The internal type definitions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_string.c` & `libfvde-20240502/libfvalue/libfvalue_string.c`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * String value functions
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libfvalue/libfvalue_libuna.h` & `libfvde-20240502/libfvalue/libfvalue_libuna.h`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * The libuna header wrapper
  *
- * Copyright (C) 2010-2022, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
```

### Comparing `libfvde-20240113/libcnotify/libcnotify_definitions.h` & `libfvde-20240502/libcnotify/libcnotify_definitions.h`

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

### Comparing `libfvde-20240113/libcnotify/libcnotify_extern.h` & `libfvde-20240502/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcnotify/libcnotify_support.c` & `libfvde-20240502/libfdata/libfdata_support.c`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 /*
  * Support functions
  *
- * Copyright (C) 2008-2024, Joachim Metz <joachim.metz@gmail.com>
+ * Copyright (C) 2010-2024, Joachim Metz <joachim.metz@gmail.com>
  *
  * Refer to AUTHORS for acknowledgements.
  *
  * This program is free software: you can redistribute it and/or modify
  * it under the terms of the GNU Lesser General Public License as published by
  * the Free Software Foundation, either version 3 of the License, or
  * (at your option) any later version.
@@ -18,22 +18,24 @@
  * You should have received a copy of the GNU Lesser General Public License
  * along with this program.  If not, see <https://www.gnu.org/licenses/>.
  */
 
 #include <common.h>
 #include <types.h>
 
-#include "libcnotify_definitions.h"
-#include "libcnotify_support.h"
+#include <stdio.h>
 
-#if !defined( HAVE_LOCAL_LIBCNOTIFY )
+#include "libfdata_definitions.h"
+#include "libfdata_support.h"
+
+#if !defined( HAVE_LOCAL_LIBFDATA )
 
 /* Returns the library version as a string
  */
-const char *libcnotify_get_version(
+const char *libfdata_get_version(
              void )
 {
-	return( (const char *) LIBCNOTIFY_VERSION_STRING );
+	return( (const char *) LIBFDATA_VERSION_STRING );
 }
 
-#endif /* !defined( HAVE_LOCAL_LIBCNOTIFY ) */
+#endif /* !defined( HAVE_LOCAL_LIBFDATA ) */
```

### Comparing `libfvde-20240113/libcnotify/libcnotify_stream.h` & `libfvde-20240502/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcnotify/Makefile.am` & `libfvde-20240502/libcnotify/Makefile.am`

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

### Comparing `libfvde-20240113/libcnotify/libcnotify_unused.h` & `libfvde-20240502/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcnotify/libcnotify_verbose.h` & `libfvde-20240502/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcnotify/libcnotify_print.h` & `libfvde-20240502/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcnotify/libcnotify_stream.c` & `libfvde-20240502/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcnotify/libcnotify_support.h` & `libfvde-20240502/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcnotify/libcnotify_verbose.c` & `libfvde-20240502/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcnotify/Makefile.in` & `libfvde-20240502/libcnotify/Makefile.in`

 * *Files 2% similar despite different names*

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
@@ -567,30 +569,31 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -793,24 +796,30 @@
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
 
@@ -897,17 +906,14 @@
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

### Comparing `libfvde-20240113/libcnotify/libcnotify_libcerror.h` & `libfvde-20240502/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcnotify/libcnotify_print.c` & `libfvde-20240502/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcerror/libcerror_system.c` & `libfvde-20240502/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcerror/libcerror_error.c` & `libfvde-20240502/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcerror/libcerror_extern.h` & `libfvde-20240502/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcerror/Makefile.am` & `libfvde-20240502/libcerror/Makefile.am`

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

### Comparing `libfvde-20240113/libcerror/libcerror_types.h` & `libfvde-20240502/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcerror/libcerror_support.h` & `libfvde-20240502/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcerror/libcerror_error.h` & `libfvde-20240502/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcerror/libcerror_system.h` & `libfvde-20240502/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcerror/libcerror_definitions.h` & `libfvde-20240502/libcerror/libcerror_definitions.h`

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

### Comparing `libfvde-20240113/libcerror/libcerror_unused.h` & `libfvde-20240502/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/libcerror/Makefile.in` & `libfvde-20240502/libcerror/Makefile.in`

 * *Files 1% similar despite different names*

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
@@ -564,28 +566,29 @@
 target_alias = @target_alias@
 top_build_prefix = @top_build_prefix@
 top_builddir = @top_builddir@
 top_srcdir = @top_srcdir@
 zlib_CFLAGS = @zlib_CFLAGS@
 zlib_LIBS = @zlib_LIBS@
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
@@ -787,24 +790,29 @@
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
 
@@ -890,17 +898,14 @@
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

### Comparing `libfvde-20240113/aclocal.m4` & `libfvde-20240502/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libfvde-20240113/configure.ac` & `libfvde-20240502/configure.ac`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libfvde],
- [20240113],
+ [20240502],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libfvde.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
 AM_EXTRA_RECURSIVE_TARGETS([sources splint])
```

