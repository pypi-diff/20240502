# Comparing `tmp/ReverseBox-0.8.0.tar.gz` & `tmp/ReverseBox-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReverseBox-0.8.0.tar", last modified: Thu May  2 09:34:10 2024, max compression
+gzip compressed data, was "ReverseBox-0.8.1.tar", last modified: Thu May  2 10:36:40 2024, max compression
```

## Comparing `ReverseBox-0.8.0.tar` & `ReverseBox-0.8.1.tar`

### file list

```diff
@@ -1,94 +1,95 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 09:34:10.896768 ReverseBox-0.8.0/
--rw-rw-rw-   0        0        0    35821 2022-03-18 16:59:48.000000 ReverseBox-0.8.0/LICENSE
--rw-rw-rw-   0        0        0     6882 2024-05-02 09:34:10.895771 ReverseBox-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     5530 2024-05-02 09:31:21.000000 ReverseBox-0.8.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 09:34:10.828950 ReverseBox-0.8.0/ReverseBox.egg-info/
--rw-rw-rw-   0        0        0     6882 2024-05-02 09:34:10.000000 ReverseBox-0.8.0/ReverseBox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2662 2024-05-02 09:34:10.000000 ReverseBox-0.8.0/ReverseBox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 09:34:10.000000 ReverseBox-0.8.0/ReverseBox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       26 2024-05-02 09:34:10.000000 ReverseBox-0.8.0/ReverseBox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-05-02 09:34:10.000000 ReverseBox-0.8.0/ReverseBox.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-02 09:34:10.829975 ReverseBox-0.8.0/reversebox/
--rw-rw-rw-   0        0        0        0 2022-06-25 12:19:28.000000 ReverseBox-0.8.0/reversebox/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 09:34:10.834964 ReverseBox-0.8.0/reversebox/checksum/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.8.0/reversebox/checksum/__init__.py
--rw-rw-rw-   0        0        0      404 2023-01-08 20:51:08.000000 ReverseBox-0.8.0/reversebox/checksum/checksum_adler32.py
--rw-rw-rw-   0        0        0      404 2023-07-06 21:19:52.000000 ReverseBox-0.8.0/reversebox/checksum/checksum_bsd16.py
--rw-rw-rw-   0        0        0      403 2023-01-09 21:19:58.000000 ReverseBox-0.8.0/reversebox/checksum/checksum_fletcher16.py
--rw-rw-rw-   0        0        0      510 2023-01-09 22:41:54.000000 ReverseBox-0.8.0/reversebox/checksum/checksum_fletcher32.py
-drwxrwxrwx   0        0        0        0 2024-05-02 09:34:10.836960 ReverseBox-0.8.0/reversebox/common/
--rw-rw-rw-   0        0        0        0 2022-06-25 16:29:14.000000 ReverseBox-0.8.0/reversebox/common/__init__.py
--rw-rw-rw-   0        0        0      491 2023-07-05 21:46:48.000000 ReverseBox-0.8.0/reversebox/common/common.py
--rw-rw-rw-   0        0        0      730 2022-09-07 19:55:28.000000 ReverseBox-0.8.0/reversebox/common/logger.py
-drwxrwxrwx   0        0        0        0 2024-05-02 09:34:10.840948 ReverseBox-0.8.0/reversebox/compression/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.8.0/reversebox/compression/__init__.py
--rw-rw-rw-   0        0        0      482 2023-04-23 00:00:02.000000 ReverseBox-0.8.0/reversebox/compression/compression_jcalg1.py
--rw-rw-rw-   0        0        0      335 2022-12-27 14:57:00.000000 ReverseBox-0.8.0/reversebox/compression/compression_lzo.py
--rw-rw-rw-   0        0        0      330 2022-10-15 10:41:40.000000 ReverseBox-0.8.0/reversebox/compression/compression_zlib.py
-drwxrwxrwx   0        0        0        0 2024-05-02 09:34:10.851916 ReverseBox-0.8.0/reversebox/crc/
--rw-rw-rw-   0        0        0        0 2023-01-09 18:26:30.000000 ReverseBox-0.8.0/reversebox/crc/__init__.py
--rw-rw-rw-   0        0        0     1018 2022-07-17 23:25:20.000000 ReverseBox-0.8.0/reversebox/crc/crc16_arc.py
--rw-rw-rw-   0        0        0     1656 2022-07-24 14:41:32.000000 ReverseBox-0.8.0/reversebox/crc/crc16_ccitt.py
--rw-rw-rw-   0        0        0     1189 2022-07-21 21:16:08.000000 ReverseBox-0.8.0/reversebox/crc/crc16_dnp.py
--rw-rw-rw-   0        0        0     1211 2022-07-17 23:25:20.000000 ReverseBox-0.8.0/reversebox/crc/crc16_kermit.py
--rw-rw-rw-   0        0        0     1103 2022-07-24 15:12:38.000000 ReverseBox-0.8.0/reversebox/crc/crc16_modbus.py
--rw-rw-rw-   0        0        0      735 2022-07-21 21:35:32.000000 ReverseBox-0.8.0/reversebox/crc/crc16_sick.py
--rw-rw-rw-   0        0        0     3784 2023-09-13 22:28:42.000000 ReverseBox-0.8.0/reversebox/crc/crc32_asobo.py
--rw-rw-rw-   0        0        0     1008 2022-07-17 23:25:20.000000 ReverseBox-0.8.0/reversebox/crc/crc32_iso_hdlc.py
--rw-rw-rw-   0        0        0     6040 2023-11-15 15:34:51.000000 ReverseBox-0.8.0/reversebox/crc/crc64_asobo.py
--rw-rw-rw-   0        0        0     1402 2023-07-08 10:59:02.000000 ReverseBox-0.8.0/reversebox/crc/crc8.py
-drwxrwxrwx   0        0        0        0 2024-05-02 09:34:10.857896 ReverseBox-0.8.0/reversebox/encryption/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.8.0/reversebox/encryption/__init__.py
--rw-rw-rw-   0        0        0     1094 2023-11-16 14:56:06.000000 ReverseBox-0.8.0/reversebox/encryption/encryption_rot13.py
--rw-rw-rw-   0        0        0      579 2022-07-17 23:25:20.000000 ReverseBox-0.8.0/reversebox/encryption/encryption_xor_basic.py
--rw-rw-rw-   0        0        0     1551 2024-03-17 21:48:42.000000 ReverseBox-0.8.0/reversebox/encryption/encryption_xor_basic_key_guesser.py
--rw-rw-rw-   0        0        0     1175 2023-04-15 13:23:02.000000 ReverseBox-0.8.0/reversebox/encryption/encryption_xor_gianas_return_zda.py
--rw-rw-rw-   0        0        0      574 2022-07-17 23:25:20.000000 ReverseBox-0.8.0/reversebox/encryption/encryption_xor_retro64_eco.py
-drwxrwxrwx   0        0        0        0 2024-05-02 09:34:10.862882 ReverseBox-0.8.0/reversebox/hash/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.8.0/reversebox/hash/__init__.py
--rw-rw-rw-   0        0        0     2127 2024-04-29 16:13:10.000000 ReverseBox-0.8.0/reversebox/hash/hash_fnv.py
--rw-rw-rw-   0        0        0      386 2023-11-15 15:27:56.000000 ReverseBox-0.8.0/reversebox/hash/hash_md2.py
--rw-rw-rw-   0        0        0      280 2022-09-11 18:48:38.000000 ReverseBox-0.8.0/reversebox/hash/hash_md5.py
--rw-rw-rw-   0        0        0      283 2023-01-08 14:05:02.000000 ReverseBox-0.8.0/reversebox/hash/hash_sha1.py
--rw-rw-rw-   0        0        0      289 2023-01-08 14:07:32.000000 ReverseBox-0.8.0/reversebox/hash/hash_sha2.py
-drwxrwxrwx   0        0        0        0 2024-05-02 09:34:10.868871 ReverseBox-0.8.0/reversebox/image/
--rw-rw-rw-   0        0        0        0 2022-12-27 21:18:26.000000 ReverseBox-0.8.0/reversebox/image/__init__.py
--rw-rw-rw-   0        0        0     2836 2024-05-02 09:31:33.000000 ReverseBox-0.8.0/reversebox/image/image_dds.py
--rw-rw-rw-   0        0        0    12401 2024-05-02 09:33:01.000000 ReverseBox-0.8.0/reversebox/image/image_decoder.py
--rw-rw-rw-   0        0        0    13727 2023-01-06 23:05:20.000000 ReverseBox-0.8.0/reversebox/image/image_finder_gui.py
--rw-rw-rw-   0        0        0      713 2023-04-23 00:00:02.000000 ReverseBox-0.8.0/reversebox/image/image_finder_main.py
--rw-rw-rw-   0        0        0      614 2024-05-02 09:31:21.000000 ReverseBox-0.8.0/reversebox/image/image_formats.py
-drwxrwxrwx   0        0        0        0 2024-05-02 09:34:10.875852 ReverseBox-0.8.0/reversebox/image/swizzling/
--rw-rw-rw-   0        0        0        0 2024-04-12 20:30:39.000000 ReverseBox-0.8.0/reversebox/image/swizzling/__init__.py
--rw-rw-rw-   0        0        0      848 2024-04-14 22:08:19.000000 ReverseBox-0.8.0/reversebox/image/swizzling/swizzle_3ds.py
--rw-rw-rw-   0        0        0     2045 2024-04-14 21:57:16.000000 ReverseBox-0.8.0/reversebox/image/swizzling/swizzle_cmpr.py
--rw-rw-rw-   0        0        0     2457 2024-04-14 21:57:16.000000 ReverseBox-0.8.0/reversebox/image/swizzling/swizzle_ps2.py
--rw-rw-rw-   0        0        0     1529 2024-04-14 21:59:10.000000 ReverseBox-0.8.0/reversebox/image/swizzling/swizzle_psp.py
--rw-rw-rw-   0        0        0     1854 2024-04-14 22:03:05.000000 ReverseBox-0.8.0/reversebox/image/swizzling/swizzle_psvita.py
--rw-rw-rw-   0        0        0     1571 2024-04-14 22:03:55.000000 ReverseBox-0.8.0/reversebox/image/swizzling/swizzle_switch.py
--rw-rw-rw-   0        0        0       93 2024-04-14 21:57:16.000000 ReverseBox-0.8.0/reversebox/image/swizzling/swizzle_xbox.py
-drwxrwxrwx   0        0        0        0 2024-05-02 09:34:10.881837 ReverseBox-0.8.0/reversebox/io_files/
--rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.8.0/reversebox/io_files/__init__.py
--rw-rw-rw-   0        0        0     1420 2024-04-26 22:10:36.000000 ReverseBox-0.8.0/reversebox/io_files/bytes_handler.py
--rw-rw-rw-   0        0        0     1026 2023-04-22 01:54:50.000000 ReverseBox-0.8.0/reversebox/io_files/check_file.py
--rw-rw-rw-   0        0        0     8126 2023-04-23 18:16:42.000000 ReverseBox-0.8.0/reversebox/io_files/file_handler.py
--rw-rw-rw-   0        0        0     5195 2023-05-08 21:42:16.000000 ReverseBox-0.8.0/reversebox/io_files/mod_handler.py
--rw-rw-rw-   0        0        0    11372 2023-05-08 21:44:24.000000 ReverseBox-0.8.0/reversebox/io_files/translation_text_handler.py
--rw-rw-rw-   0        0        0       42 2024-05-02 09:34:10.896768 ReverseBox-0.8.0/setup.cfg
--rw-rw-rw-   0        0        0     1844 2024-05-02 08:18:11.000000 ReverseBox-0.8.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-02 09:34:10.882843 ReverseBox-0.8.0/tests/
--rw-rw-rw-   0        0        0        0 2022-07-19 22:27:12.000000 ReverseBox-0.8.0/tests/__init__.py
--rw-rw-rw-   0        0        0      879 2024-03-17 21:42:22.000000 ReverseBox-0.8.0/tests/common.py
-drwxrwxrwx   0        0        0        0 2024-05-02 09:34:10.893777 ReverseBox-0.8.0/tests/tests_crc/
--rw-rw-rw-   0        0        0        0 2023-01-09 18:28:34.000000 ReverseBox-0.8.0/tests/tests_crc/__init__.py
--rw-rw-rw-   0        0        0     2301 2023-01-09 18:34:10.000000 ReverseBox-0.8.0/tests/tests_crc/test_crc16_arc.py
--rw-rw-rw-   0        0        0     4539 2023-01-09 18:34:10.000000 ReverseBox-0.8.0/tests/tests_crc/test_crc16_ccitt.py
--rw-rw-rw-   0        0        0     1633 2023-01-09 18:34:10.000000 ReverseBox-0.8.0/tests/tests_crc/test_crc16_dnp.py
--rw-rw-rw-   0        0        0     1651 2023-01-09 18:34:10.000000 ReverseBox-0.8.0/tests/tests_crc/test_crc16_kermit.py
--rw-rw-rw-   0        0        0     1660 2023-01-09 18:34:10.000000 ReverseBox-0.8.0/tests/tests_crc/test_crc16_modbus.py
--rw-rw-rw-   0        0        0     1632 2023-01-09 18:34:10.000000 ReverseBox-0.8.0/tests/tests_crc/test_crc16_sick.py
--rw-rw-rw-   0        0        0     2209 2023-09-13 22:24:14.000000 ReverseBox-0.8.0/tests/tests_crc/test_crc32_asobo.py
--rw-rw-rw-   0        0        0     2655 2023-04-23 00:00:02.000000 ReverseBox-0.8.0/tests/tests_crc/test_crc32_iso_hdlc.py
--rw-rw-rw-   0        0        0     1822 2023-07-08 10:59:02.000000 ReverseBox-0.8.0/tests/tests_crc/test_crc8.py
--rw-rw-rw-   0        0        0     1850 2023-07-08 10:59:02.000000 ReverseBox-0.8.0/tests/tests_crc/test_crc8_cdma_2000.py
--rw-rw-rw-   0        0        0     1832 2023-07-08 10:59:02.000000 ReverseBox-0.8.0/tests/tests_crc/test_crc8_darc.py
+drwxrwxrwx   0        0        0        0 2024-05-02 10:36:40.391104 ReverseBox-0.8.1/
+-rw-rw-rw-   0        0        0    35821 2022-03-18 16:59:48.000000 ReverseBox-0.8.1/LICENSE
+-rw-rw-rw-   0        0        0     6882 2024-05-02 10:36:40.390106 ReverseBox-0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5530 2024-05-02 09:31:21.000000 ReverseBox-0.8.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 10:36:40.326277 ReverseBox-0.8.1/ReverseBox.egg-info/
+-rw-rw-rw-   0        0        0     6882 2024-05-02 10:36:40.000000 ReverseBox-0.8.1/ReverseBox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2708 2024-05-02 10:36:40.000000 ReverseBox-0.8.1/ReverseBox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 10:36:40.000000 ReverseBox-0.8.1/ReverseBox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       26 2024-05-02 10:36:40.000000 ReverseBox-0.8.1/ReverseBox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-02 10:36:40.000000 ReverseBox-0.8.1/ReverseBox.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 10:36:40.327274 ReverseBox-0.8.1/reversebox/
+-rw-rw-rw-   0        0        0        0 2022-06-25 12:19:28.000000 ReverseBox-0.8.1/reversebox/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 10:36:40.331264 ReverseBox-0.8.1/reversebox/checksum/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.8.1/reversebox/checksum/__init__.py
+-rw-rw-rw-   0        0        0      404 2023-01-08 20:51:08.000000 ReverseBox-0.8.1/reversebox/checksum/checksum_adler32.py
+-rw-rw-rw-   0        0        0      404 2023-07-06 21:19:52.000000 ReverseBox-0.8.1/reversebox/checksum/checksum_bsd16.py
+-rw-rw-rw-   0        0        0      403 2023-01-09 21:19:58.000000 ReverseBox-0.8.1/reversebox/checksum/checksum_fletcher16.py
+-rw-rw-rw-   0        0        0      510 2023-01-09 22:41:54.000000 ReverseBox-0.8.1/reversebox/checksum/checksum_fletcher32.py
+drwxrwxrwx   0        0        0        0 2024-05-02 10:36:40.333258 ReverseBox-0.8.1/reversebox/common/
+-rw-rw-rw-   0        0        0        0 2022-06-25 16:29:14.000000 ReverseBox-0.8.1/reversebox/common/__init__.py
+-rw-rw-rw-   0        0        0      491 2023-07-05 21:46:48.000000 ReverseBox-0.8.1/reversebox/common/common.py
+-rw-rw-rw-   0        0        0      730 2022-09-07 19:55:28.000000 ReverseBox-0.8.1/reversebox/common/logger.py
+drwxrwxrwx   0        0        0        0 2024-05-02 10:36:40.337247 ReverseBox-0.8.1/reversebox/compression/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.8.1/reversebox/compression/__init__.py
+-rw-rw-rw-   0        0        0      482 2023-04-23 00:00:02.000000 ReverseBox-0.8.1/reversebox/compression/compression_jcalg1.py
+-rw-rw-rw-   0        0        0      335 2022-12-27 14:57:00.000000 ReverseBox-0.8.1/reversebox/compression/compression_lzo.py
+-rw-rw-rw-   0        0        0      330 2022-10-15 10:41:40.000000 ReverseBox-0.8.1/reversebox/compression/compression_zlib.py
+drwxrwxrwx   0        0        0        0 2024-05-02 10:36:40.347221 ReverseBox-0.8.1/reversebox/crc/
+-rw-rw-rw-   0        0        0        0 2023-01-09 18:26:30.000000 ReverseBox-0.8.1/reversebox/crc/__init__.py
+-rw-rw-rw-   0        0        0     1018 2022-07-17 23:25:20.000000 ReverseBox-0.8.1/reversebox/crc/crc16_arc.py
+-rw-rw-rw-   0        0        0     1656 2022-07-24 14:41:32.000000 ReverseBox-0.8.1/reversebox/crc/crc16_ccitt.py
+-rw-rw-rw-   0        0        0     1189 2022-07-21 21:16:08.000000 ReverseBox-0.8.1/reversebox/crc/crc16_dnp.py
+-rw-rw-rw-   0        0        0     1211 2022-07-17 23:25:20.000000 ReverseBox-0.8.1/reversebox/crc/crc16_kermit.py
+-rw-rw-rw-   0        0        0     1103 2022-07-24 15:12:38.000000 ReverseBox-0.8.1/reversebox/crc/crc16_modbus.py
+-rw-rw-rw-   0        0        0      735 2022-07-21 21:35:32.000000 ReverseBox-0.8.1/reversebox/crc/crc16_sick.py
+-rw-rw-rw-   0        0        0     3784 2023-09-13 22:28:42.000000 ReverseBox-0.8.1/reversebox/crc/crc32_asobo.py
+-rw-rw-rw-   0        0        0     1008 2022-07-17 23:25:20.000000 ReverseBox-0.8.1/reversebox/crc/crc32_iso_hdlc.py
+-rw-rw-rw-   0        0        0     6040 2023-11-15 15:34:51.000000 ReverseBox-0.8.1/reversebox/crc/crc64_asobo.py
+-rw-rw-rw-   0        0        0     1402 2023-07-08 10:59:02.000000 ReverseBox-0.8.1/reversebox/crc/crc8.py
+drwxrwxrwx   0        0        0        0 2024-05-02 10:36:40.352207 ReverseBox-0.8.1/reversebox/encryption/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.8.1/reversebox/encryption/__init__.py
+-rw-rw-rw-   0        0        0     1094 2023-11-16 14:56:06.000000 ReverseBox-0.8.1/reversebox/encryption/encryption_rot13.py
+-rw-rw-rw-   0        0        0      579 2022-07-17 23:25:20.000000 ReverseBox-0.8.1/reversebox/encryption/encryption_xor_basic.py
+-rw-rw-rw-   0        0        0     1551 2024-03-17 21:48:42.000000 ReverseBox-0.8.1/reversebox/encryption/encryption_xor_basic_key_guesser.py
+-rw-rw-rw-   0        0        0     1175 2023-04-15 13:23:02.000000 ReverseBox-0.8.1/reversebox/encryption/encryption_xor_gianas_return_zda.py
+-rw-rw-rw-   0        0        0      574 2022-07-17 23:25:20.000000 ReverseBox-0.8.1/reversebox/encryption/encryption_xor_retro64_eco.py
+drwxrwxrwx   0        0        0        0 2024-05-02 10:36:40.358192 ReverseBox-0.8.1/reversebox/hash/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.8.1/reversebox/hash/__init__.py
+-rw-rw-rw-   0        0        0     2127 2024-04-29 16:13:10.000000 ReverseBox-0.8.1/reversebox/hash/hash_fnv.py
+-rw-rw-rw-   0        0        0      386 2023-11-15 15:27:56.000000 ReverseBox-0.8.1/reversebox/hash/hash_md2.py
+-rw-rw-rw-   0        0        0      280 2022-09-11 18:48:38.000000 ReverseBox-0.8.1/reversebox/hash/hash_md5.py
+-rw-rw-rw-   0        0        0      283 2023-01-08 14:05:02.000000 ReverseBox-0.8.1/reversebox/hash/hash_sha1.py
+-rw-rw-rw-   0        0        0      289 2023-01-08 14:07:32.000000 ReverseBox-0.8.1/reversebox/hash/hash_sha2.py
+drwxrwxrwx   0        0        0        0 2024-05-02 10:36:40.363178 ReverseBox-0.8.1/reversebox/image/
+-rw-rw-rw-   0        0        0        0 2022-12-27 21:18:26.000000 ReverseBox-0.8.1/reversebox/image/__init__.py
+-rw-rw-rw-   0        0        0     2836 2024-05-02 09:31:33.000000 ReverseBox-0.8.1/reversebox/image/image_dds.py
+-rw-rw-rw-   0        0        0    11817 2024-05-02 10:36:19.000000 ReverseBox-0.8.1/reversebox/image/image_decoder.py
+-rw-rw-rw-   0        0        0    13727 2023-01-06 23:05:20.000000 ReverseBox-0.8.1/reversebox/image/image_finder_gui.py
+-rw-rw-rw-   0        0        0      713 2023-04-23 00:00:02.000000 ReverseBox-0.8.1/reversebox/image/image_finder_main.py
+-rw-rw-rw-   0        0        0      614 2024-05-02 09:31:21.000000 ReverseBox-0.8.1/reversebox/image/image_formats.py
+drwxrwxrwx   0        0        0        0 2024-05-02 10:36:40.370165 ReverseBox-0.8.1/reversebox/image/swizzling/
+-rw-rw-rw-   0        0        0        0 2024-04-12 20:30:39.000000 ReverseBox-0.8.1/reversebox/image/swizzling/__init__.py
+-rw-rw-rw-   0        0        0      848 2024-04-14 22:08:19.000000 ReverseBox-0.8.1/reversebox/image/swizzling/swizzle_3ds.py
+-rw-rw-rw-   0        0        0     2045 2024-04-14 21:57:16.000000 ReverseBox-0.8.1/reversebox/image/swizzling/swizzle_cmpr.py
+-rw-rw-rw-   0        0        0     2457 2024-04-14 21:57:16.000000 ReverseBox-0.8.1/reversebox/image/swizzling/swizzle_ps2.py
+-rw-rw-rw-   0        0        0     1529 2024-04-14 21:59:10.000000 ReverseBox-0.8.1/reversebox/image/swizzling/swizzle_psp.py
+-rw-rw-rw-   0        0        0     1854 2024-04-14 22:03:05.000000 ReverseBox-0.8.1/reversebox/image/swizzling/swizzle_psvita.py
+-rw-rw-rw-   0        0        0     1571 2024-04-14 22:03:55.000000 ReverseBox-0.8.1/reversebox/image/swizzling/swizzle_switch.py
+-rw-rw-rw-   0        0        0       93 2024-04-14 21:57:16.000000 ReverseBox-0.8.1/reversebox/image/swizzling/swizzle_xbox.py
+drwxrwxrwx   0        0        0        0 2024-05-02 10:36:40.376144 ReverseBox-0.8.1/reversebox/io_files/
+-rw-rw-rw-   0        0        0        0 2022-06-16 10:36:14.000000 ReverseBox-0.8.1/reversebox/io_files/__init__.py
+-rw-rw-rw-   0        0        0     1420 2024-04-26 22:10:36.000000 ReverseBox-0.8.1/reversebox/io_files/bytes_handler.py
+-rw-rw-rw-   0        0        0      789 2024-05-02 10:36:13.000000 ReverseBox-0.8.1/reversebox/io_files/bytes_helper_functions.py
+-rw-rw-rw-   0        0        0     1026 2023-04-22 01:54:50.000000 ReverseBox-0.8.1/reversebox/io_files/check_file.py
+-rw-rw-rw-   0        0        0     8126 2023-04-23 18:16:42.000000 ReverseBox-0.8.1/reversebox/io_files/file_handler.py
+-rw-rw-rw-   0        0        0     5195 2023-05-08 21:42:16.000000 ReverseBox-0.8.1/reversebox/io_files/mod_handler.py
+-rw-rw-rw-   0        0        0    11372 2023-05-08 21:44:24.000000 ReverseBox-0.8.1/reversebox/io_files/translation_text_handler.py
+-rw-rw-rw-   0        0        0       42 2024-05-02 10:36:40.391104 ReverseBox-0.8.1/setup.cfg
+-rw-rw-rw-   0        0        0     1844 2024-05-02 10:36:13.000000 ReverseBox-0.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 10:36:40.378137 ReverseBox-0.8.1/tests/
+-rw-rw-rw-   0        0        0        0 2022-07-19 22:27:12.000000 ReverseBox-0.8.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      879 2024-03-17 21:42:22.000000 ReverseBox-0.8.1/tests/common.py
+drwxrwxrwx   0        0        0        0 2024-05-02 10:36:40.389109 ReverseBox-0.8.1/tests/tests_crc/
+-rw-rw-rw-   0        0        0        0 2023-01-09 18:28:34.000000 ReverseBox-0.8.1/tests/tests_crc/__init__.py
+-rw-rw-rw-   0        0        0     2301 2023-01-09 18:34:10.000000 ReverseBox-0.8.1/tests/tests_crc/test_crc16_arc.py
+-rw-rw-rw-   0        0        0     4539 2023-01-09 18:34:10.000000 ReverseBox-0.8.1/tests/tests_crc/test_crc16_ccitt.py
+-rw-rw-rw-   0        0        0     1633 2023-01-09 18:34:10.000000 ReverseBox-0.8.1/tests/tests_crc/test_crc16_dnp.py
+-rw-rw-rw-   0        0        0     1651 2023-01-09 18:34:10.000000 ReverseBox-0.8.1/tests/tests_crc/test_crc16_kermit.py
+-rw-rw-rw-   0        0        0     1660 2023-01-09 18:34:10.000000 ReverseBox-0.8.1/tests/tests_crc/test_crc16_modbus.py
+-rw-rw-rw-   0        0        0     1632 2023-01-09 18:34:10.000000 ReverseBox-0.8.1/tests/tests_crc/test_crc16_sick.py
+-rw-rw-rw-   0        0        0     2209 2023-09-13 22:24:14.000000 ReverseBox-0.8.1/tests/tests_crc/test_crc32_asobo.py
+-rw-rw-rw-   0        0        0     2655 2023-04-23 00:00:02.000000 ReverseBox-0.8.1/tests/tests_crc/test_crc32_iso_hdlc.py
+-rw-rw-rw-   0        0        0     1822 2023-07-08 10:59:02.000000 ReverseBox-0.8.1/tests/tests_crc/test_crc8.py
+-rw-rw-rw-   0        0        0     1850 2023-07-08 10:59:02.000000 ReverseBox-0.8.1/tests/tests_crc/test_crc8_cdma_2000.py
+-rw-rw-rw-   0        0        0     1832 2023-07-08 10:59:02.000000 ReverseBox-0.8.1/tests/tests_crc/test_crc8_darc.py
```

### Comparing `ReverseBox-0.8.0/LICENSE` & `ReverseBox-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/PKG-INFO` & `ReverseBox-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseBox
-Version: 0.8.0
+Version: 0.8.1
 Summary: A set of functions useful in reverse engineering.
 Home-page: https://github.com/bartlomiejduda/ReverseBox
 Author: Bartlomiej Duda
 Author-email: ikskoks@gmail.com
 Keywords: ReverseBox,reverse engineering,RE,CRC,Hash,Encryption,Compression,Checksum,Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `ReverseBox-0.8.0/README.md` & `ReverseBox-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/ReverseBox.egg-info/PKG-INFO` & `ReverseBox-0.8.1/ReverseBox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReverseBox
-Version: 0.8.0
+Version: 0.8.1
 Summary: A set of functions useful in reverse engineering.
 Home-page: https://github.com/bartlomiejduda/ReverseBox
 Author: Bartlomiej Duda
 Author-email: ikskoks@gmail.com
 Keywords: ReverseBox,reverse engineering,RE,CRC,Hash,Encryption,Compression,Checksum,Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `ReverseBox-0.8.0/ReverseBox.egg-info/SOURCES.txt` & `ReverseBox-0.8.1/ReverseBox.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,15 @@
 reversebox/image/swizzling/swizzle_ps2.py
 reversebox/image/swizzling/swizzle_psp.py
 reversebox/image/swizzling/swizzle_psvita.py
 reversebox/image/swizzling/swizzle_switch.py
 reversebox/image/swizzling/swizzle_xbox.py
 reversebox/io_files/__init__.py
 reversebox/io_files/bytes_handler.py
+reversebox/io_files/bytes_helper_functions.py
 reversebox/io_files/check_file.py
 reversebox/io_files/file_handler.py
 reversebox/io_files/mod_handler.py
 reversebox/io_files/translation_text_handler.py
 tests/__init__.py
 tests/common.py
 tests/tests_crc/__init__.py
```

### Comparing `ReverseBox-0.8.0/reversebox/common/logger.py` & `ReverseBox-0.8.1/reversebox/common/logger.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/crc/crc16_arc.py` & `ReverseBox-0.8.1/reversebox/crc/crc16_arc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/crc/crc16_ccitt.py` & `ReverseBox-0.8.1/reversebox/crc/crc16_ccitt.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/crc/crc16_dnp.py` & `ReverseBox-0.8.1/reversebox/crc/crc16_dnp.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/crc/crc16_kermit.py` & `ReverseBox-0.8.1/reversebox/crc/crc16_kermit.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/crc/crc16_modbus.py` & `ReverseBox-0.8.1/reversebox/crc/crc16_modbus.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/crc/crc16_sick.py` & `ReverseBox-0.8.1/reversebox/crc/crc16_sick.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/crc/crc32_asobo.py` & `ReverseBox-0.8.1/reversebox/crc/crc32_asobo.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/crc/crc32_iso_hdlc.py` & `ReverseBox-0.8.1/reversebox/crc/crc32_iso_hdlc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/crc/crc64_asobo.py` & `ReverseBox-0.8.1/reversebox/crc/crc64_asobo.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/crc/crc8.py` & `ReverseBox-0.8.1/reversebox/crc/crc8.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/encryption/encryption_rot13.py` & `ReverseBox-0.8.1/reversebox/encryption/encryption_rot13.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/encryption/encryption_xor_basic.py` & `ReverseBox-0.8.1/reversebox/encryption/encryption_xor_basic.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/encryption/encryption_xor_basic_key_guesser.py` & `ReverseBox-0.8.1/reversebox/encryption/encryption_xor_basic_key_guesser.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/encryption/encryption_xor_gianas_return_zda.py` & `ReverseBox-0.8.1/reversebox/encryption/encryption_xor_gianas_return_zda.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/encryption/encryption_xor_retro64_eco.py` & `ReverseBox-0.8.1/reversebox/encryption/encryption_xor_retro64_eco.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/hash/hash_fnv.py` & `ReverseBox-0.8.1/reversebox/hash/hash_fnv.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/image/image_dds.py` & `ReverseBox-0.8.1/reversebox/image/image_dds.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/image/image_decoder.py` & `ReverseBox-0.8.1/reversebox/image/image_decoder.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 import struct
 
 from PIL import Image
 
 from reversebox.common.logger import get_logger
 from reversebox.image.image_formats import ImageFormats
 from reversebox.io_files.bytes_handler import BytesHandler
+from reversebox.io_files.bytes_helper_functions import (
+    get_uint16,
+    get_uint24,
+    get_uint32,
+)
 
 logger = get_logger(__name__)
 
 # fmt: off
 # mypy: ignore-errors
 
 
@@ -127,52 +132,35 @@
 
         p[0] = (b << 4) | (b >> 0)
         p[1] = (g << 4) | (g >> 0)
         p[2] = (r << 4) | (r >> 0)
         p[3] = (a << 4) | (a >> 0)
         return p
 
-    def _get_uint16(self, in_bytes: bytes, endianess: str) -> int:
-        result = struct.unpack(endianess + "H", in_bytes)[0]
-        return result
-
-    def _get_uint24(self, in_bytes: bytes, endianess: str) -> int:
-        if endianess == "<":
-            result = struct.unpack(endianess + "I", in_bytes + b"\x00")[0]
-        elif endianess == ">":
-            result = struct.unpack(endianess + "I", b"\x00" + in_bytes)[0]
-        else:
-            raise Exception("Wrong endianess!")
-        return result
-
-    def _get_uint32(self, in_bytes: bytes, endianess: str) -> int:
-        result = struct.unpack(endianess + "I", in_bytes)[0]
-        return result
-
     generic_data_formats = {
         # image_format: (decode_function, bits_per_pixel, image_entry_read_function)
-        ImageFormats.RGB565: (_decode_rgb565_pixel, 16, _get_uint16),
-        ImageFormats.RGB888: (_decode_rgb888_pixel, 24, _get_uint24),
-        ImageFormats.BGR888: (_decode_bgr888_pixel, 24, _get_uint24),
-        ImageFormats.ARGB4444: (_decode_argb4444_pixel, 16, _get_uint16),
-        ImageFormats.RGBA4444: (_decode_rgba4444_pixel, 16, _get_uint16),
-        ImageFormats.XRGB1555: (_decode_xrgb1555_pixel, 16, _get_uint16),
-        ImageFormats.ABGR1555: (_decode_abgr1555_pixel, 16, _get_uint16),
-        ImageFormats.XBGR1555: (_decode_xbgr1555_pixel, 16, _get_uint16),
-        ImageFormats.ARGB8888: (_decode_argb8888_pixel, 32, _get_uint32),
+        ImageFormats.RGB565: (_decode_rgb565_pixel, 16, get_uint16),
+        ImageFormats.RGB888: (_decode_rgb888_pixel, 24, get_uint24),
+        ImageFormats.BGR888: (_decode_bgr888_pixel, 24, get_uint24),
+        ImageFormats.ARGB4444: (_decode_argb4444_pixel, 16, get_uint16),
+        ImageFormats.RGBA4444: (_decode_rgba4444_pixel, 16, get_uint16),
+        ImageFormats.XRGB1555: (_decode_xrgb1555_pixel, 16, get_uint16),
+        ImageFormats.ABGR1555: (_decode_abgr1555_pixel, 16, get_uint16),
+        ImageFormats.XBGR1555: (_decode_xbgr1555_pixel, 16, get_uint16),
+        ImageFormats.ARGB8888: (_decode_argb8888_pixel, 32, get_uint32),
     }
 
     indexed_data_formats = {
         # image_format: (decode_function, bits_per_pixel, palette_entry_size, palette_entry_read_function)
-        ImageFormats.PAL4_RGBX5551: (_decode_rgbx5551_pixel, 4, 2, _get_uint16),
-        ImageFormats.PAL4_RGB888: (_decode_rgb888_pixel, 4, 3, _get_uint24),
-        ImageFormats.PAL4_RGBA8888: (_decode_rgba8888_pixel, 4, 4, _get_uint32),
-        ImageFormats.PAL8_RGBX5551: (_decode_rgbx5551_pixel, 8, 2, _get_uint16),
-        ImageFormats.PAL8_RGB888: (_decode_rgb888_pixel, 8, 3, _get_uint24),
-        ImageFormats.PAL8_RGBA8888: (_decode_rgba8888_pixel, 8, 4, _get_uint32),
+        ImageFormats.PAL4_RGBX5551: (_decode_rgbx5551_pixel, 4, 2, get_uint16),
+        ImageFormats.PAL4_RGB888: (_decode_rgb888_pixel, 4, 3, get_uint24),
+        ImageFormats.PAL4_RGBA8888: (_decode_rgba8888_pixel, 4, 4, get_uint32),
+        ImageFormats.PAL8_RGBX5551: (_decode_rgbx5551_pixel, 8, 2, get_uint16),
+        ImageFormats.PAL8_RGB888: (_decode_rgb888_pixel, 8, 3, get_uint24),
+        ImageFormats.PAL8_RGBA8888: (_decode_rgba8888_pixel, 8, 4, get_uint32),
     }
 
     compressed_data_formats = {
         # image format: (decoder_name, decoder_arg)
         ImageFormats.DXT1: ("bcn", 1),
         ImageFormats.DXT3: ("bcn", 2)
     }
```

### Comparing `ReverseBox-0.8.0/reversebox/image/image_finder_gui.py` & `ReverseBox-0.8.1/reversebox/image/image_finder_gui.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/image/image_finder_main.py` & `ReverseBox-0.8.1/reversebox/image/image_finder_main.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/image/image_formats.py` & `ReverseBox-0.8.1/reversebox/image/image_formats.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/image/swizzling/swizzle_3ds.py` & `ReverseBox-0.8.1/reversebox/image/swizzling/swizzle_3ds.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/image/swizzling/swizzle_cmpr.py` & `ReverseBox-0.8.1/reversebox/image/swizzling/swizzle_cmpr.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/image/swizzling/swizzle_ps2.py` & `ReverseBox-0.8.1/reversebox/image/swizzling/swizzle_ps2.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/image/swizzling/swizzle_psp.py` & `ReverseBox-0.8.1/reversebox/image/swizzling/swizzle_psp.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/image/swizzling/swizzle_psvita.py` & `ReverseBox-0.8.1/reversebox/image/swizzling/swizzle_psvita.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/image/swizzling/swizzle_switch.py` & `ReverseBox-0.8.1/reversebox/image/swizzling/swizzle_switch.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/io_files/bytes_handler.py` & `ReverseBox-0.8.1/reversebox/io_files/bytes_handler.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/io_files/check_file.py` & `ReverseBox-0.8.1/reversebox/io_files/check_file.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/io_files/file_handler.py` & `ReverseBox-0.8.1/reversebox/io_files/file_handler.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/io_files/mod_handler.py` & `ReverseBox-0.8.1/reversebox/io_files/mod_handler.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/reversebox/io_files/translation_text_handler.py` & `ReverseBox-0.8.1/reversebox/io_files/translation_text_handler.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/setup.py` & `ReverseBox-0.8.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 License: GPL-3.0 License
 """
 
 import os
 
 import setuptools
 
-VERSION_NUM = "0.8.0"
+VERSION_NUM = "0.8.1"
 
 
 def get_long_description() -> str:
     with open(
         os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf8"
     ) as readme:
         readme_text = readme.read()
```

### Comparing `ReverseBox-0.8.0/tests/common.py` & `ReverseBox-0.8.1/tests/common.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/tests/tests_crc/test_crc16_arc.py` & `ReverseBox-0.8.1/tests/tests_crc/test_crc16_arc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/tests/tests_crc/test_crc16_ccitt.py` & `ReverseBox-0.8.1/tests/tests_crc/test_crc16_ccitt.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/tests/tests_crc/test_crc16_dnp.py` & `ReverseBox-0.8.1/tests/tests_crc/test_crc16_dnp.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/tests/tests_crc/test_crc16_kermit.py` & `ReverseBox-0.8.1/tests/tests_crc/test_crc16_kermit.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/tests/tests_crc/test_crc16_modbus.py` & `ReverseBox-0.8.1/tests/tests_crc/test_crc16_modbus.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/tests/tests_crc/test_crc16_sick.py` & `ReverseBox-0.8.1/tests/tests_crc/test_crc16_sick.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/tests/tests_crc/test_crc32_asobo.py` & `ReverseBox-0.8.1/tests/tests_crc/test_crc32_asobo.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/tests/tests_crc/test_crc32_iso_hdlc.py` & `ReverseBox-0.8.1/tests/tests_crc/test_crc32_iso_hdlc.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/tests/tests_crc/test_crc8.py` & `ReverseBox-0.8.1/tests/tests_crc/test_crc8.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/tests/tests_crc/test_crc8_cdma_2000.py` & `ReverseBox-0.8.1/tests/tests_crc/test_crc8_cdma_2000.py`

 * *Files identical despite different names*

### Comparing `ReverseBox-0.8.0/tests/tests_crc/test_crc8_darc.py` & `ReverseBox-0.8.1/tests/tests_crc/test_crc8_darc.py`

 * *Files identical despite different names*

