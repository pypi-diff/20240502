# Comparing `tmp/oracledb-2.1.1.tar.gz` & `tmp/oracledb-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oracledb-2.1.1.tar", last modified: Thu Mar 21 17:22:35 2024, max compression
+gzip compressed data, was "oracledb-2.1.2.tar", last modified: Thu Apr 11 16:59:08 2024, max compression
```

## Comparing `oracledb-2.1.1.tar` & `oracledb-2.1.2.tar`

### file list

```diff
@@ -1,208 +1,208 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 17:22:35.090522 oracledb-2.1.1/
--rw-rw-r--   0 root         (0) root         (0)    12570 2024-02-25 03:35:14.000000 oracledb-2.1.1/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)      398 2022-05-20 21:47:15.000000 oracledb-2.1.1/MANIFEST.in
--rw-rw-r--   0 root         (0) root         (0)       56 2024-02-25 03:35:14.000000 oracledb-2.1.1/NOTICE.txt
--rw-r--r--   0 root         (0) root         (0)     5208 2024-03-21 17:22:35.090522 oracledb-2.1.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     3730 2024-02-25 03:35:14.000000 oracledb-2.1.1/README.md
--rw-rw-r--   0 root         (0) root         (0)      166 2024-02-25 03:35:14.000000 oracledb-2.1.1/README.txt
--rw-rw-r--   0 root         (0) root         (0)    28103 2024-02-25 03:35:14.000000 oracledb-2.1.1/THIRD_PARTY_LICENSES.txt
--rw-rw-r--   0 root         (0) root         (0)      310 2024-03-12 23:07:01.000000 oracledb-2.1.1/pyproject.toml
--rw-rw-r--   0 root         (0) root         (0)     1608 2024-03-21 17:22:35.091522 oracledb-2.1.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     3878 2024-02-25 03:35:14.000000 oracledb-2.1.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 17:22:35.064522 oracledb-2.1.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 17:22:35.070522 oracledb-2.1.1/src/oracledb/
--rw-rw-r--   0 root         (0) root         (0)    11121 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    19011 2024-02-25 03:35:14.000000 oracledb-2.1.1/src/oracledb/aq.py
--rw-rw-r--   0 root         (0) root         (0)    25768 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/base_impl.pxd
--rw-rw-r--   0 root         (0) root         (0)     3681 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/base_impl.pyx
--rw-rw-r--   0 root         (0) root         (0)    36342 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/connect_params.py
--rw-rw-r--   0 root         (0) root         (0)    75308 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/connection.py
--rw-rw-r--   0 root         (0) root         (0)     4144 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/constants.py
--rw-rw-r--   0 root         (0) root         (0)     2909 2024-02-25 03:35:14.000000 oracledb-2.1.1/src/oracledb/constructors.py
--rw-rw-r--   0 root         (0) root         (0)    44011 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/cursor.py
--rw-rw-r--   0 root         (0) root         (0)    11862 2024-02-25 03:35:14.000000 oracledb-2.1.1/src/oracledb/dbobject.py
--rw-rw-r--   0 root         (0) root         (0)     3492 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/defaults.py
--rw-rw-r--   0 root         (0) root         (0)     5483 2024-02-25 03:35:14.000000 oracledb-2.1.1/src/oracledb/driver_mode.py
--rw-rw-r--   0 root         (0) root         (0)     3160 2024-02-25 03:35:14.000000 oracledb-2.1.1/src/oracledb/dsn.py
--rw-rw-r--   0 root         (0) root         (0)    28396 2024-03-21 16:38:49.000000 oracledb-2.1.1/src/oracledb/errors.py
--rw-rw-r--   0 root         (0) root         (0)     1812 2024-02-25 03:35:14.000000 oracledb-2.1.1/src/oracledb/exceptions.py
--rw-rw-r--   0 root         (0) root         (0)     7448 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/fetch_info.py
--rw-rw-r--   0 root         (0) root         (0)     1717 2024-02-25 03:35:14.000000 oracledb-2.1.1/src/oracledb/future.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 17:22:35.065522 oracledb-2.1.1/src/oracledb/impl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 17:22:35.073522 oracledb-2.1.1/src/oracledb/impl/base/
--rw-r--r--   0 root         (0) root         (0)     7341 2022-05-20 21:47:15.000000 oracledb-2.1.1/src/oracledb/impl/base/bind_var.pyx
--rw-rw-r--   0 root         (0) root         (0)    46402 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/base/buffer.pyx
--rw-rw-r--   0 root         (0) root         (0)    41898 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/base/connect_params.pyx
--rw-rw-r--   0 root         (0) root         (0)    13869 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/base/connection.pyx
--rw-rw-r--   0 root         (0) root         (0)     3478 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/base/constants.pxi
--rw-rw-r--   0 root         (0) root         (0)    25501 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/base/cursor.pyx
--rw-rw-r--   0 root         (0) root         (0)     7066 2024-02-25 03:35:14.000000 oracledb-2.1.1/src/oracledb/impl/base/dbobject.pyx
--rw-rw-r--   0 root         (0) root         (0)     1702 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/base/defaults.pyx
--rw-r--r--   0 root         (0) root         (0)     2741 2022-05-20 21:47:15.000000 oracledb-2.1.1/src/oracledb/impl/base/lob.pyx
--rw-rw-r--   0 root         (0) root         (0)    33590 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/base/oson.pyx
--rw-r--r--   0 root         (0) root         (0)     4215 2022-05-20 21:47:15.000000 oracledb-2.1.1/src/oracledb/impl/base/pool.pyx
--rw-rw-r--   0 root         (0) root         (0)     4288 2024-02-25 03:35:14.000000 oracledb-2.1.1/src/oracledb/impl/base/pool_params.pyx
--rw-rw-r--   0 root         (0) root         (0)     6379 2023-12-12 01:18:55.000000 oracledb-2.1.1/src/oracledb/impl/base/queue.pyx
--rw-rw-r--   0 root         (0) root         (0)     4799 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/base/soda.pyx
--rw-r--r--   0 root         (0) root         (0)     1933 2022-05-20 21:47:15.000000 oracledb-2.1.1/src/oracledb/impl/base/subscr.pyx
--rw-rw-r--   0 root         (0) root         (0)    10365 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/base/types.pyx
--rw-rw-r--   0 root         (0) root         (0)     8561 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/base/utils.pyx
--rw-rw-r--   0 root         (0) root         (0)    11659 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/base/var.pyx
--rw-rw-r--   0 root         (0) root         (0)     6470 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/base/vector.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 17:22:35.074522 oracledb-2.1.1/src/oracledb/impl/thick/
--rw-rw-r--   0 root         (0) root         (0)     2264 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/thick/buffer.pyx
--rw-rw-r--   0 root         (0) root         (0)    32798 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/thick/connection.pyx
--rw-rw-r--   0 root         (0) root         (0)    21510 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/thick/cursor.pyx
--rw-rw-r--   0 root         (0) root         (0)    14836 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/thick/dbobject.pyx
--rw-rw-r--   0 root         (0) root         (0)     9894 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/thick/json.pyx
--rw-r--r--   0 root         (0) root         (0)     7534 2022-05-20 21:47:15.000000 oracledb-2.1.1/src/oracledb/impl/thick/lob.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 17:22:35.065522 oracledb-2.1.1/src/oracledb/impl/thick/odpi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 17:22:35.075522 oracledb-2.1.1/src/oracledb/impl/thick/odpi/embed/
--rw-rw-r--   0 root         (0) root         (0)     2633 2024-03-11 15:29:55.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/embed/dpi.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 17:22:35.075522 oracledb-2.1.1/src/oracledb/impl/thick/odpi/include/
--rw-rw-r--   0 root         (0) root         (0)    86869 2024-03-11 15:29:55.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/include/dpi.h
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 17:22:35.080522 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/
--rw-rw-r--   0 root         (0) root         (0)   117539 2024-03-11 15:29:55.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiConn.c
--rw-rw-r--   0 root         (0) root         (0)    16874 2024-03-11 15:29:55.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiContext.c
--rw-r--r--   0 root         (0) root         (0)    34806 2022-05-20 22:11:04.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiData.c
--rw-r--r--   0 root         (0) root         (0)     7443 2022-05-20 22:11:04.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiDebug.c
--rw-r--r--   0 root         (0) root         (0)    15574 2022-05-20 22:11:04.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiDeqOptions.c
--rw-r--r--   0 root         (0) root         (0)     7552 2022-05-20 22:11:04.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiEnqOptions.c
--rw-r--r--   0 root         (0) root         (0)     9569 2022-05-20 22:11:04.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiEnv.c
--rw-rw-r--   0 root         (0) root         (0)    14038 2024-02-28 17:15:47.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiError.c
--rw-rw-r--   0 root         (0) root         (0)     9348 2024-03-11 15:29:55.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiErrorMessages.h
--rw-rw-r--   0 root         (0) root         (0)    13273 2024-03-11 15:29:55.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiGen.c
--rw-r--r--   0 root         (0) root         (0)    15039 2022-11-07 17:19:09.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiGlobal.c
--rw-r--r--   0 root         (0) root         (0)     5184 2022-05-20 22:11:04.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiHandleList.c
--rw-r--r--   0 root         (0) root         (0)     5399 2022-05-20 22:11:04.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiHandlePool.c
--rw-rw-r--   0 root         (0) root         (0)   111354 2024-03-11 15:29:55.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiImpl.h
--rw-rw-r--   0 root         (0) root         (0)    37212 2024-03-11 15:29:55.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiJson.c
--rw-rw-r--   0 root         (0) root         (0)    19868 2024-02-03 18:38:13.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiLob.c
--rw-r--r--   0 root         (0) root         (0)    23232 2022-08-27 21:56:08.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiMsgProps.c
--rw-r--r--   0 root         (0) root         (0)    40061 2022-05-20 22:11:04.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiObject.c
--rw-rw-r--   0 root         (0) root         (0)     5372 2024-02-03 18:38:13.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiObjectAttr.c
--rw-rw-r--   0 root         (0) root         (0)    15195 2024-02-03 18:38:13.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiObjectType.c
--rw-rw-r--   0 root         (0) root         (0)   182440 2024-03-11 15:29:55.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiOci.c
--rw-rw-r--   0 root         (0) root         (0)    32160 2024-03-11 15:29:55.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiOracleType.c
--rw-r--r--   0 root         (0) root         (0)    32638 2022-08-02 17:00:34.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiPool.c
--rw-rw-r--   0 root         (0) root         (0)    23704 2024-03-11 15:29:55.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiQueue.c
--rw-r--r--   0 root         (0) root         (0)     5712 2022-05-20 22:11:04.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiRowid.c
--rw-rw-r--   0 root         (0) root         (0)    42311 2024-03-11 15:29:55.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiSodaColl.c
--rw-r--r--   0 root         (0) root         (0)     6131 2022-05-20 22:11:04.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiSodaCollCursor.c
--rw-rw-r--   0 root         (0) root         (0)    16800 2024-03-11 15:29:55.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiSodaDb.c
--rw-rw-r--   0 root         (0) root         (0)    12671 2024-03-11 15:29:55.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiSodaDoc.c
--rw-r--r--   0 root         (0) root         (0)     6134 2022-05-20 22:11:04.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiSodaDocCursor.c
--rw-rw-r--   0 root         (0) root         (0)    79506 2024-02-03 18:38:13.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiStmt.c
--rw-rw-r--   0 root         (0) root         (0)     4221 2024-01-05 20:41:23.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiStringList.c
--rw-r--r--   0 root         (0) root         (0)    29091 2022-05-20 22:11:04.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiSubscr.c
--rw-r--r--   0 root         (0) root         (0)    23589 2022-11-01 20:30:53.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiUtils.c
--rw-rw-r--   0 root         (0) root         (0)    81960 2024-03-11 15:29:55.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiVar.c
--rw-rw-r--   0 root         (0) root         (0)     7710 2024-03-11 15:29:55.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiVector.c
--rw-rw-r--   0 root         (0) root         (0)    41686 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/thick/odpi.pxd
--rw-rw-r--   0 root         (0) root         (0)    13993 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/thick/pool.pyx
--rw-rw-r--   0 root         (0) root         (0)    21424 2023-12-12 01:18:55.000000 oracledb-2.1.1/src/oracledb/impl/thick/queue.pyx
--rw-rw-r--   0 root         (0) root         (0)    25297 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/thick/soda.pyx
--rw-rw-r--   0 root         (0) root         (0)     7310 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/thick/subscr.pyx
--rw-rw-r--   0 root         (0) root         (0)    23386 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/thick/utils.pyx
--rw-rw-r--   0 root         (0) root         (0)    11661 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/thick/var.pyx
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 17:22:35.082522 oracledb-2.1.1/src/oracledb/impl/thin/
--rw-rw-r--   0 root         (0) root         (0)     5909 2024-03-13 18:14:53.000000 oracledb-2.1.1/src/oracledb/impl/thin/capabilities.pyx
--rw-rw-r--   0 root         (0) root         (0)    21891 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/thin/connection.pyx
--rw-rw-r--   0 root         (0) root         (0)    23100 2024-03-13 18:14:53.000000 oracledb-2.1.1/src/oracledb/impl/thin/constants.pxi
--rw-rw-r--   0 root         (0) root         (0)     7891 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/thin/conversions.pyx
--rw-rw-r--   0 root         (0) root         (0)     3949 2024-02-25 03:35:14.000000 oracledb-2.1.1/src/oracledb/impl/thin/crypto.pyx
--rw-rw-r--   0 root         (0) root         (0)    12900 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/thin/cursor.pyx
--rw-rw-r--   0 root         (0) root         (0)    23990 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/thin/data_types.pyx
--rw-rw-r--   0 root         (0) root         (0)    23860 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/thin/dbobject.pyx
--rw-rw-r--   0 root         (0) root         (0)    30374 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/thin/dbobject_cache.pyx
--rw-rw-r--   0 root         (0) root         (0)    12546 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/thin/lob.pyx
--rw-rw-r--   0 root         (0) root         (0)   110019 2024-03-13 18:14:53.000000 oracledb-2.1.1/src/oracledb/impl/thin/messages.pyx
--rw-rw-r--   0 root         (0) root         (0)    34409 2024-03-13 18:14:53.000000 oracledb-2.1.1/src/oracledb/impl/thin/packet.pyx
--rw-rw-r--   0 root         (0) root         (0)    35748 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/thin/pool.pyx
--rw-rw-r--   0 root         (0) root         (0)    39127 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/thin/protocol.pyx
--rw-rw-r--   0 root         (0) root         (0)    18199 2024-03-21 16:38:49.000000 oracledb-2.1.1/src/oracledb/impl/thin/statement.pyx
--rw-rw-r--   0 root         (0) root         (0)     7444 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/thin/statement_cache.pyx
--rw-rw-r--   0 root         (0) root         (0)    13869 2024-03-21 16:37:56.000000 oracledb-2.1.1/src/oracledb/impl/thin/transport.pyx
--rw-rw-r--   0 root         (0) root         (0)     4776 2024-02-25 03:35:14.000000 oracledb-2.1.1/src/oracledb/impl/thin/utils.pyx
--rw-rw-r--   0 root         (0) root         (0)     5544 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/impl/thin/var.pyx
--rw-rw-r--   0 root         (0) root         (0)    11397 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/lob.py
--rw-rw-r--   0 root         (0) root         (0)    56457 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/pool.py
--rw-rw-r--   0 root         (0) root         (0)    33746 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/pool_params.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-05-20 21:47:15.000000 oracledb-2.1.1/src/oracledb/py.typed
--rw-rw-r--   0 root         (0) root         (0)    28590 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/soda.py
--rw-rw-r--   0 root         (0) root         (0)    11067 2024-02-25 03:35:14.000000 oracledb-2.1.1/src/oracledb/subscr.py
--rw-rw-r--   0 root         (0) root         (0)     3312 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/thick_impl.pyx
--rw-rw-r--   0 root         (0) root         (0)     5126 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/thin_impl.pyx
--rw-rw-r--   0 root         (0) root         (0)     3422 2024-02-25 03:35:14.000000 oracledb-2.1.1/src/oracledb/utils.py
--rw-rw-r--   0 root         (0) root         (0)     6604 2024-02-25 03:35:14.000000 oracledb-2.1.1/src/oracledb/var.py
--rw-rw-r--   0 root         (0) root         (0)     1533 2024-03-12 23:07:01.000000 oracledb-2.1.1/src/oracledb/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 17:22:35.090522 oracledb-2.1.1/src/oracledb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5208 2024-03-21 17:22:34.000000 oracledb-2.1.1/src/oracledb.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     6455 2024-03-21 17:22:35.000000 oracledb-2.1.1/src/oracledb.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2024-03-21 17:22:34.000000 oracledb-2.1.1/src/oracledb.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2024-03-21 16:50:08.000000 oracledb-2.1.1/src/oracledb.egg-info/not-zip-safe
--rw-rw-r--   0 root         (0) root         (0)       20 2024-03-21 17:22:34.000000 oracledb-2.1.1/src/oracledb.egg-info/requires.txt
--rw-rw-r--   0 root         (0) root         (0)        9 2024-03-21 17:22:34.000000 oracledb-2.1.1/src/oracledb.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-21 17:22:35.090522 oracledb-2.1.1/tests/
--rw-rw-r--   0 root         (0) root         (0)     2403 2024-02-25 03:35:14.000000 oracledb-2.1.1/tests/create_schema.py
--rw-rw-r--   0 root         (0) root         (0)     1897 2024-02-25 03:35:14.000000 oracledb-2.1.1/tests/drop_schema.py
--rw-rw-r--   0 root         (0) root         (0)     6790 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_1000_module.py
--rw-rw-r--   0 root         (0) root         (0)    29873 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_1100_connection.py
--rw-rw-r--   0 root         (0) root         (0)    13794 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_1300_cursor_var.py
--rw-rw-r--   0 root         (0) root         (0)    11040 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_1400_datetime_var.py
--rw-rw-r--   0 root         (0) root         (0)     8894 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_1500_types.py
--rw-rw-r--   0 root         (0) root         (0)    19708 2024-03-21 16:38:49.000000 oracledb-2.1.1/tests/test_1600_dml_returning.py
--rw-rw-r--   0 root         (0) root         (0)     7433 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_1700_error.py
--rw-rw-r--   0 root         (0) root         (0)     8179 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_1800_interval_var.py
--rw-rw-r--   0 root         (0) root         (0)    21081 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_1900_lob_var.py
--rw-rw-r--   0 root         (0) root         (0)     5045 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_2000_long_var.py
--rw-rw-r--   0 root         (0) root         (0)    11361 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_2100_nchar_var.py
--rw-rw-r--   0 root         (0) root         (0)    20614 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_2200_number_var.py
--rw-rw-r--   0 root         (0) root         (0)    29697 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_2300_object_var.py
--rw-rw-r--   0 root         (0) root         (0)    32235 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_2400_pool.py
--rw-rw-r--   0 root         (0) root         (0)    20848 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_2500_string_var.py
--rw-rw-r--   0 root         (0) root         (0)     7757 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_2600_timestamp_var.py
--rw-rw-r--   0 root         (0) root         (0)    29474 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_2700_aq.py
--rw-rw-r--   0 root         (0) root         (0)     8653 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_2800_bulk_aq.py
--rw-rw-r--   0 root         (0) root         (0)     7929 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_2900_rowid.py
--rw-rw-r--   0 root         (0) root         (0)    16130 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_3000_subscription.py
--rw-rw-r--   0 root         (0) root         (0)     4360 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_3100_boolean_var.py
--rw-rw-r--   0 root         (0) root         (0)    23087 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_3200_features_12_1.py
--rw-rw-r--   0 root         (0) root         (0)     6168 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_3300_soda_database.py
--rw-rw-r--   0 root         (0) root         (0)    41623 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_3400_soda_collection.py
--rw-rw-r--   0 root         (0) root         (0)    13612 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_3500_json.py
--rw-rw-r--   0 root         (0) root         (0)    24207 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_3600_outputtypehandler.py
--rw-rw-r--   0 root         (0) root         (0)    21053 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_3700_var.py
--rw-rw-r--   0 root         (0) root         (0)    11285 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_3800_typehandler.py
--rw-rw-r--   0 root         (0) root         (0)    20810 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_3900_cursor_execute.py
--rw-rw-r--   0 root         (0) root         (0)    16487 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_4000_cursor_executemany.py
--rw-rw-r--   0 root         (0) root         (0)     5444 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_4100_cursor_callproc.py
--rw-rw-r--   0 root         (0) root         (0)     8939 2024-03-21 16:44:33.000000 oracledb-2.1.1/tests/test_4200_cursor_scrollable.py
--rw-rw-r--   0 root         (0) root         (0)    38166 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_4300_cursor_other.py
--rw-rw-r--   0 root         (0) root         (0)    13877 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_4400_tpc.py
--rw-rw-r--   0 root         (0) root         (0)    37043 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_4500_connect_params.py
--rw-rw-r--   0 root         (0) root         (0)     8819 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_4600_type_changes.py
--rw-rw-r--   0 root         (0) root         (0)     5061 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_4700_pool_params.py
--rw-rw-r--   0 root         (0) root         (0)     7736 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_4800_timestamp_ltz_var.py
--rw-rw-r--   0 root         (0) root         (0)     7437 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_4900_timestamp_tz_var.py
--rw-rw-r--   0 root         (0) root         (0)    10665 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_5000_externalauth.py
--rw-rw-r--   0 root         (0) root         (0)     3696 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_5100_arrayvar.py
--rw-rw-r--   0 root         (0) root         (0)     7089 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_5200_sql_parser.py
--rw-rw-r--   0 root         (0) root         (0)    22230 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_5300_connection_async.py
--rw-rw-r--   0 root         (0) root         (0)    22347 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_5400_cursor_execute_async.py
--rw-rw-r--   0 root         (0) root         (0)    18058 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_5500_pool_async.py
--rw-rw-r--   0 root         (0) root         (0)    22278 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_5600_dbobject_async.py
--rw-rw-r--   0 root         (0) root         (0)    17851 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_5700_lob_var_async.py
--rw-rw-r--   0 root         (0) root         (0)    14480 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_5800_cursor_var_async.py
--rw-rw-r--   0 root         (0) root         (0)    19301 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_5900_dml_returning_async.py
--rw-rw-r--   0 root         (0) root         (0)    10133 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_6000_typehandler_async.py
--rw-rw-r--   0 root         (0) root         (0)    14724 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_6100_cursor_executemany_async.py
--rw-rw-r--   0 root         (0) root         (0)     5052 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_6200_cursor_callproc_async.py
--rw-rw-r--   0 root         (0) root         (0)    33553 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_6300_cursor_other_async.py
--rw-rw-r--   0 root         (0) root         (0)     3815 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_6600_defaults.py
--rw-rw-r--   0 root         (0) root         (0)     6689 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_6700_json_23.py
--rw-rw-r--   0 root         (0) root         (0)     5422 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_6800_error_async.py
--rw-rw-r--   0 root         (0) root         (0)     2884 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_6900_oson.py
--rw-rw-r--   0 root         (0) root         (0)     5397 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_7000_connection_async_shortcut_methods.py
--rw-rw-r--   0 root         (0) root         (0)    24050 2024-03-12 23:07:01.000000 oracledb-2.1.1/tests/test_env.py
--rw-rw-r--   0 root         (0) root         (0)      596 2024-02-25 03:35:14.000000 oracledb-2.1.1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:59:08.287334 oracledb-2.1.2/
+-rw-rw-r--   0 root         (0) root         (0)    12570 2024-03-22 04:07:57.000000 oracledb-2.1.2/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)      398 2022-05-20 21:47:15.000000 oracledb-2.1.2/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)       56 2024-03-22 04:07:57.000000 oracledb-2.1.2/NOTICE.txt
+-rw-r--r--   0 root         (0) root         (0)     5208 2024-04-11 16:59:08.287334 oracledb-2.1.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     3730 2024-03-22 04:07:57.000000 oracledb-2.1.2/README.md
+-rw-rw-r--   0 root         (0) root         (0)      166 2024-03-22 04:07:57.000000 oracledb-2.1.2/README.txt
+-rw-rw-r--   0 root         (0) root         (0)    28103 2024-03-22 04:07:57.000000 oracledb-2.1.2/THIRD_PARTY_LICENSES.txt
+-rw-rw-r--   0 root         (0) root         (0)      310 2024-03-22 04:07:57.000000 oracledb-2.1.2/pyproject.toml
+-rw-rw-r--   0 root         (0) root         (0)     1608 2024-04-11 16:59:08.287334 oracledb-2.1.2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     3878 2024-03-22 04:07:57.000000 oracledb-2.1.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:59:08.259334 oracledb-2.1.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:59:08.264334 oracledb-2.1.2/src/oracledb/
+-rw-rw-r--   0 root         (0) root         (0)    11121 2024-04-11 16:18:56.000000 oracledb-2.1.2/src/oracledb/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    19011 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/aq.py
+-rw-rw-r--   0 root         (0) root         (0)    25768 2024-04-11 16:18:56.000000 oracledb-2.1.2/src/oracledb/base_impl.pxd
+-rw-rw-r--   0 root         (0) root         (0)     3681 2024-04-11 16:18:56.000000 oracledb-2.1.2/src/oracledb/base_impl.pyx
+-rw-rw-r--   0 root         (0) root         (0)    36342 2024-04-11 16:18:56.000000 oracledb-2.1.2/src/oracledb/connect_params.py
+-rw-rw-r--   0 root         (0) root         (0)    75308 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/connection.py
+-rw-rw-r--   0 root         (0) root         (0)     4144 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/constants.py
+-rw-rw-r--   0 root         (0) root         (0)     2909 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/constructors.py
+-rw-rw-r--   0 root         (0) root         (0)    44011 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/cursor.py
+-rw-rw-r--   0 root         (0) root         (0)    11862 2024-04-11 16:18:56.000000 oracledb-2.1.2/src/oracledb/dbobject.py
+-rw-rw-r--   0 root         (0) root         (0)     3492 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/defaults.py
+-rw-rw-r--   0 root         (0) root         (0)     5483 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/driver_mode.py
+-rw-rw-r--   0 root         (0) root         (0)     3160 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/dsn.py
+-rw-rw-r--   0 root         (0) root         (0)    28396 2024-04-11 16:18:56.000000 oracledb-2.1.2/src/oracledb/errors.py
+-rw-rw-r--   0 root         (0) root         (0)     1812 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)     7448 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/fetch_info.py
+-rw-rw-r--   0 root         (0) root         (0)     1717 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/future.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:59:08.259334 oracledb-2.1.2/src/oracledb/impl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:59:08.268334 oracledb-2.1.2/src/oracledb/impl/base/
+-rw-r--r--   0 root         (0) root         (0)     7341 2022-05-20 21:47:15.000000 oracledb-2.1.2/src/oracledb/impl/base/bind_var.pyx
+-rw-rw-r--   0 root         (0) root         (0)    46402 2024-04-11 16:18:56.000000 oracledb-2.1.2/src/oracledb/impl/base/buffer.pyx
+-rw-rw-r--   0 root         (0) root         (0)    41902 2024-04-11 16:19:49.000000 oracledb-2.1.2/src/oracledb/impl/base/connect_params.pyx
+-rw-rw-r--   0 root         (0) root         (0)    13869 2024-04-11 16:18:56.000000 oracledb-2.1.2/src/oracledb/impl/base/connection.pyx
+-rw-rw-r--   0 root         (0) root         (0)     3478 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/base/constants.pxi
+-rw-rw-r--   0 root         (0) root         (0)    25501 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/base/cursor.pyx
+-rw-rw-r--   0 root         (0) root         (0)     7066 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/base/dbobject.pyx
+-rw-rw-r--   0 root         (0) root         (0)     1702 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/base/defaults.pyx
+-rw-r--r--   0 root         (0) root         (0)     2741 2022-05-20 21:47:15.000000 oracledb-2.1.2/src/oracledb/impl/base/lob.pyx
+-rw-rw-r--   0 root         (0) root         (0)    33590 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/base/oson.pyx
+-rw-r--r--   0 root         (0) root         (0)     4215 2022-05-20 21:47:15.000000 oracledb-2.1.2/src/oracledb/impl/base/pool.pyx
+-rw-rw-r--   0 root         (0) root         (0)     4288 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/base/pool_params.pyx
+-rw-rw-r--   0 root         (0) root         (0)     6379 2023-12-12 01:18:55.000000 oracledb-2.1.2/src/oracledb/impl/base/queue.pyx
+-rw-rw-r--   0 root         (0) root         (0)     4799 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/base/soda.pyx
+-rw-r--r--   0 root         (0) root         (0)     1933 2022-05-20 21:47:15.000000 oracledb-2.1.2/src/oracledb/impl/base/subscr.pyx
+-rw-rw-r--   0 root         (0) root         (0)    10365 2024-04-11 16:18:56.000000 oracledb-2.1.2/src/oracledb/impl/base/types.pyx
+-rw-rw-r--   0 root         (0) root         (0)     8561 2024-04-11 16:18:56.000000 oracledb-2.1.2/src/oracledb/impl/base/utils.pyx
+-rw-rw-r--   0 root         (0) root         (0)    11659 2024-04-11 16:18:56.000000 oracledb-2.1.2/src/oracledb/impl/base/var.pyx
+-rw-rw-r--   0 root         (0) root         (0)     6470 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/base/vector.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:59:08.269334 oracledb-2.1.2/src/oracledb/impl/thick/
+-rw-rw-r--   0 root         (0) root         (0)     2264 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/thick/buffer.pyx
+-rw-rw-r--   0 root         (0) root         (0)    32798 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/thick/connection.pyx
+-rw-rw-r--   0 root         (0) root         (0)    21510 2024-04-11 16:18:56.000000 oracledb-2.1.2/src/oracledb/impl/thick/cursor.pyx
+-rw-rw-r--   0 root         (0) root         (0)    14836 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/thick/dbobject.pyx
+-rw-rw-r--   0 root         (0) root         (0)     9894 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/thick/json.pyx
+-rw-r--r--   0 root         (0) root         (0)     7534 2022-05-20 21:47:15.000000 oracledb-2.1.2/src/oracledb/impl/thick/lob.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:59:08.259334 oracledb-2.1.2/src/oracledb/impl/thick/odpi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:59:08.270334 oracledb-2.1.2/src/oracledb/impl/thick/odpi/embed/
+-rw-rw-r--   0 root         (0) root         (0)     2633 2024-03-11 15:29:55.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/embed/dpi.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:59:08.270334 oracledb-2.1.2/src/oracledb/impl/thick/odpi/include/
+-rw-rw-r--   0 root         (0) root         (0)    86869 2024-03-11 15:29:55.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/include/dpi.h
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:59:08.275334 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/
+-rw-rw-r--   0 root         (0) root         (0)   117539 2024-03-11 15:29:55.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiConn.c
+-rw-rw-r--   0 root         (0) root         (0)    16874 2024-03-11 15:29:55.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiContext.c
+-rw-r--r--   0 root         (0) root         (0)    34806 2022-05-20 22:11:04.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiData.c
+-rw-r--r--   0 root         (0) root         (0)     7443 2022-05-20 22:11:04.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiDebug.c
+-rw-r--r--   0 root         (0) root         (0)    15574 2022-05-20 22:11:04.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiDeqOptions.c
+-rw-r--r--   0 root         (0) root         (0)     7552 2022-05-20 22:11:04.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiEnqOptions.c
+-rw-r--r--   0 root         (0) root         (0)     9569 2022-05-20 22:11:04.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiEnv.c
+-rw-rw-r--   0 root         (0) root         (0)    14038 2024-02-28 17:15:47.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiError.c
+-rw-rw-r--   0 root         (0) root         (0)     9348 2024-03-11 15:29:55.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiErrorMessages.h
+-rw-rw-r--   0 root         (0) root         (0)    13273 2024-03-11 15:29:55.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiGen.c
+-rw-r--r--   0 root         (0) root         (0)    15039 2022-11-07 17:19:09.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiGlobal.c
+-rw-r--r--   0 root         (0) root         (0)     5184 2022-05-20 22:11:04.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiHandleList.c
+-rw-r--r--   0 root         (0) root         (0)     5399 2022-05-20 22:11:04.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiHandlePool.c
+-rw-rw-r--   0 root         (0) root         (0)   111354 2024-03-11 15:29:55.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiImpl.h
+-rw-rw-r--   0 root         (0) root         (0)    37212 2024-03-11 15:29:55.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiJson.c
+-rw-rw-r--   0 root         (0) root         (0)    19868 2024-02-03 18:38:13.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiLob.c
+-rw-r--r--   0 root         (0) root         (0)    23232 2022-08-27 21:56:08.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiMsgProps.c
+-rw-r--r--   0 root         (0) root         (0)    40061 2022-05-20 22:11:04.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiObject.c
+-rw-rw-r--   0 root         (0) root         (0)     5372 2024-02-03 18:38:13.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiObjectAttr.c
+-rw-rw-r--   0 root         (0) root         (0)    15195 2024-02-03 18:38:13.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiObjectType.c
+-rw-rw-r--   0 root         (0) root         (0)   182440 2024-03-11 15:29:55.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiOci.c
+-rw-rw-r--   0 root         (0) root         (0)    32160 2024-03-11 15:29:55.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiOracleType.c
+-rw-r--r--   0 root         (0) root         (0)    32638 2022-08-02 17:00:34.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiPool.c
+-rw-rw-r--   0 root         (0) root         (0)    23704 2024-03-11 15:29:55.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiQueue.c
+-rw-r--r--   0 root         (0) root         (0)     5712 2022-05-20 22:11:04.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiRowid.c
+-rw-rw-r--   0 root         (0) root         (0)    42311 2024-03-11 15:29:55.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiSodaColl.c
+-rw-r--r--   0 root         (0) root         (0)     6131 2022-05-20 22:11:04.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiSodaCollCursor.c
+-rw-rw-r--   0 root         (0) root         (0)    16800 2024-03-11 15:29:55.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiSodaDb.c
+-rw-rw-r--   0 root         (0) root         (0)    12671 2024-03-11 15:29:55.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiSodaDoc.c
+-rw-r--r--   0 root         (0) root         (0)     6134 2022-05-20 22:11:04.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiSodaDocCursor.c
+-rw-rw-r--   0 root         (0) root         (0)    79506 2024-02-03 18:38:13.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiStmt.c
+-rw-rw-r--   0 root         (0) root         (0)     4221 2024-01-05 20:41:23.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiStringList.c
+-rw-r--r--   0 root         (0) root         (0)    29091 2022-05-20 22:11:04.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiSubscr.c
+-rw-r--r--   0 root         (0) root         (0)    23589 2022-11-01 20:30:53.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiUtils.c
+-rw-rw-r--   0 root         (0) root         (0)    81960 2024-03-11 15:29:55.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiVar.c
+-rw-rw-r--   0 root         (0) root         (0)     7710 2024-03-11 15:29:55.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiVector.c
+-rw-rw-r--   0 root         (0) root         (0)    41686 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/thick/odpi.pxd
+-rw-rw-r--   0 root         (0) root         (0)    13993 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/thick/pool.pyx
+-rw-rw-r--   0 root         (0) root         (0)    21424 2023-12-12 01:18:55.000000 oracledb-2.1.2/src/oracledb/impl/thick/queue.pyx
+-rw-rw-r--   0 root         (0) root         (0)    25297 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/thick/soda.pyx
+-rw-rw-r--   0 root         (0) root         (0)     7310 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/thick/subscr.pyx
+-rw-rw-r--   0 root         (0) root         (0)    23386 2024-04-11 16:18:56.000000 oracledb-2.1.2/src/oracledb/impl/thick/utils.pyx
+-rw-rw-r--   0 root         (0) root         (0)    11661 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/thick/var.pyx
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:59:08.278334 oracledb-2.1.2/src/oracledb/impl/thin/
+-rw-rw-r--   0 root         (0) root         (0)     5909 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/thin/capabilities.pyx
+-rw-rw-r--   0 root         (0) root         (0)    21891 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/thin/connection.pyx
+-rw-rw-r--   0 root         (0) root         (0)    23100 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/thin/constants.pxi
+-rw-rw-r--   0 root         (0) root         (0)     7891 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/thin/conversions.pyx
+-rw-rw-r--   0 root         (0) root         (0)     3949 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/thin/crypto.pyx
+-rw-rw-r--   0 root         (0) root         (0)    12900 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/thin/cursor.pyx
+-rw-rw-r--   0 root         (0) root         (0)    23990 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/thin/data_types.pyx
+-rw-rw-r--   0 root         (0) root         (0)    23860 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/thin/dbobject.pyx
+-rw-rw-r--   0 root         (0) root         (0)    30374 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/thin/dbobject_cache.pyx
+-rw-rw-r--   0 root         (0) root         (0)    12546 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/thin/lob.pyx
+-rw-rw-r--   0 root         (0) root         (0)   110037 2024-04-11 16:21:08.000000 oracledb-2.1.2/src/oracledb/impl/thin/messages.pyx
+-rw-rw-r--   0 root         (0) root         (0)    34409 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/thin/packet.pyx
+-rw-rw-r--   0 root         (0) root         (0)    35748 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/thin/pool.pyx
+-rw-rw-r--   0 root         (0) root         (0)    39127 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/thin/protocol.pyx
+-rw-rw-r--   0 root         (0) root         (0)    18199 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/thin/statement.pyx
+-rw-rw-r--   0 root         (0) root         (0)     7444 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/thin/statement_cache.pyx
+-rw-rw-r--   0 root         (0) root         (0)    13869 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/thin/transport.pyx
+-rw-rw-r--   0 root         (0) root         (0)     4776 2024-04-11 16:18:56.000000 oracledb-2.1.2/src/oracledb/impl/thin/utils.pyx
+-rw-rw-r--   0 root         (0) root         (0)     5544 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/impl/thin/var.pyx
+-rw-rw-r--   0 root         (0) root         (0)    11397 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/lob.py
+-rw-rw-r--   0 root         (0) root         (0)    56457 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/pool.py
+-rw-rw-r--   0 root         (0) root         (0)    33746 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/pool_params.py
+-rw-r--r--   0 root         (0) root         (0)        0 2022-05-20 21:47:15.000000 oracledb-2.1.2/src/oracledb/py.typed
+-rw-rw-r--   0 root         (0) root         (0)    28590 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/soda.py
+-rw-rw-r--   0 root         (0) root         (0)    11067 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/subscr.py
+-rw-rw-r--   0 root         (0) root         (0)     3312 2024-04-11 16:18:56.000000 oracledb-2.1.2/src/oracledb/thick_impl.pyx
+-rw-rw-r--   0 root         (0) root         (0)     5126 2024-04-11 16:18:56.000000 oracledb-2.1.2/src/oracledb/thin_impl.pyx
+-rw-rw-r--   0 root         (0) root         (0)     3422 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/utils.py
+-rw-rw-r--   0 root         (0) root         (0)     6604 2024-03-22 04:07:57.000000 oracledb-2.1.2/src/oracledb/var.py
+-rw-rw-r--   0 root         (0) root         (0)     1533 2024-04-11 16:19:28.000000 oracledb-2.1.2/src/oracledb/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:59:08.286334 oracledb-2.1.2/src/oracledb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5208 2024-04-11 16:59:08.000000 oracledb-2.1.2/src/oracledb.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     6455 2024-04-11 16:59:08.000000 oracledb-2.1.2/src/oracledb.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2024-04-11 16:59:08.000000 oracledb-2.1.2/src/oracledb.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2024-04-11 16:23:27.000000 oracledb-2.1.2/src/oracledb.egg-info/not-zip-safe
+-rw-rw-r--   0 root         (0) root         (0)       20 2024-04-11 16:59:08.000000 oracledb-2.1.2/src/oracledb.egg-info/requires.txt
+-rw-rw-r--   0 root         (0) root         (0)        9 2024-04-11 16:59:08.000000 oracledb-2.1.2/src/oracledb.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 16:59:08.286334 oracledb-2.1.2/tests/
+-rw-rw-r--   0 root         (0) root         (0)     2403 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/create_schema.py
+-rw-rw-r--   0 root         (0) root         (0)     1897 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/drop_schema.py
+-rw-rw-r--   0 root         (0) root         (0)     6790 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_1000_module.py
+-rw-rw-r--   0 root         (0) root         (0)    29873 2024-04-11 16:18:56.000000 oracledb-2.1.2/tests/test_1100_connection.py
+-rw-rw-r--   0 root         (0) root         (0)    13794 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_1300_cursor_var.py
+-rw-rw-r--   0 root         (0) root         (0)    11040 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_1400_datetime_var.py
+-rw-rw-r--   0 root         (0) root         (0)     8894 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_1500_types.py
+-rw-rw-r--   0 root         (0) root         (0)    19708 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_1600_dml_returning.py
+-rw-rw-r--   0 root         (0) root         (0)     7433 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_1700_error.py
+-rw-rw-r--   0 root         (0) root         (0)     8179 2024-04-11 16:18:56.000000 oracledb-2.1.2/tests/test_1800_interval_var.py
+-rw-rw-r--   0 root         (0) root         (0)    21081 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_1900_lob_var.py
+-rw-rw-r--   0 root         (0) root         (0)     5045 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_2000_long_var.py
+-rw-rw-r--   0 root         (0) root         (0)    11361 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_2100_nchar_var.py
+-rw-rw-r--   0 root         (0) root         (0)    20614 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_2200_number_var.py
+-rw-rw-r--   0 root         (0) root         (0)    29697 2024-04-11 16:18:56.000000 oracledb-2.1.2/tests/test_2300_object_var.py
+-rw-rw-r--   0 root         (0) root         (0)    32235 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_2400_pool.py
+-rw-rw-r--   0 root         (0) root         (0)    20848 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_2500_string_var.py
+-rw-rw-r--   0 root         (0) root         (0)     7757 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_2600_timestamp_var.py
+-rw-rw-r--   0 root         (0) root         (0)    29474 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_2700_aq.py
+-rw-rw-r--   0 root         (0) root         (0)     8653 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_2800_bulk_aq.py
+-rw-rw-r--   0 root         (0) root         (0)     7929 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_2900_rowid.py
+-rw-rw-r--   0 root         (0) root         (0)    16130 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_3000_subscription.py
+-rw-rw-r--   0 root         (0) root         (0)     4360 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_3100_boolean_var.py
+-rw-rw-r--   0 root         (0) root         (0)    23087 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_3200_features_12_1.py
+-rw-rw-r--   0 root         (0) root         (0)     6168 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_3300_soda_database.py
+-rw-rw-r--   0 root         (0) root         (0)    41623 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_3400_soda_collection.py
+-rw-rw-r--   0 root         (0) root         (0)    13612 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_3500_json.py
+-rw-rw-r--   0 root         (0) root         (0)    24207 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_3600_outputtypehandler.py
+-rw-rw-r--   0 root         (0) root         (0)    21053 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_3700_var.py
+-rw-rw-r--   0 root         (0) root         (0)    11285 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_3800_typehandler.py
+-rw-rw-r--   0 root         (0) root         (0)    21010 2024-04-11 16:21:08.000000 oracledb-2.1.2/tests/test_3900_cursor_execute.py
+-rw-rw-r--   0 root         (0) root         (0)    16487 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_4000_cursor_executemany.py
+-rw-rw-r--   0 root         (0) root         (0)     5444 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_4100_cursor_callproc.py
+-rw-rw-r--   0 root         (0) root         (0)     8939 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_4200_cursor_scrollable.py
+-rw-rw-r--   0 root         (0) root         (0)    38166 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_4300_cursor_other.py
+-rw-rw-r--   0 root         (0) root         (0)    13877 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_4400_tpc.py
+-rw-rw-r--   0 root         (0) root         (0)    37043 2024-04-11 16:18:56.000000 oracledb-2.1.2/tests/test_4500_connect_params.py
+-rw-rw-r--   0 root         (0) root         (0)     8819 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_4600_type_changes.py
+-rw-rw-r--   0 root         (0) root         (0)     5061 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_4700_pool_params.py
+-rw-rw-r--   0 root         (0) root         (0)     7736 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_4800_timestamp_ltz_var.py
+-rw-rw-r--   0 root         (0) root         (0)     7437 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_4900_timestamp_tz_var.py
+-rw-rw-r--   0 root         (0) root         (0)    10665 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_5000_externalauth.py
+-rw-rw-r--   0 root         (0) root         (0)     3696 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_5100_arrayvar.py
+-rw-rw-r--   0 root         (0) root         (0)     7089 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_5200_sql_parser.py
+-rw-rw-r--   0 root         (0) root         (0)    22230 2024-04-11 16:18:56.000000 oracledb-2.1.2/tests/test_5300_connection_async.py
+-rw-rw-r--   0 root         (0) root         (0)    22559 2024-04-11 16:21:08.000000 oracledb-2.1.2/tests/test_5400_cursor_execute_async.py
+-rw-rw-r--   0 root         (0) root         (0)    18058 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_5500_pool_async.py
+-rw-rw-r--   0 root         (0) root         (0)    22278 2024-04-11 16:18:56.000000 oracledb-2.1.2/tests/test_5600_dbobject_async.py
+-rw-rw-r--   0 root         (0) root         (0)    17851 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_5700_lob_var_async.py
+-rw-rw-r--   0 root         (0) root         (0)    14480 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_5800_cursor_var_async.py
+-rw-rw-r--   0 root         (0) root         (0)    19301 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_5900_dml_returning_async.py
+-rw-rw-r--   0 root         (0) root         (0)    10133 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_6000_typehandler_async.py
+-rw-rw-r--   0 root         (0) root         (0)    14724 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_6100_cursor_executemany_async.py
+-rw-rw-r--   0 root         (0) root         (0)     5052 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_6200_cursor_callproc_async.py
+-rw-rw-r--   0 root         (0) root         (0)    33553 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_6300_cursor_other_async.py
+-rw-rw-r--   0 root         (0) root         (0)     3815 2024-04-11 16:18:56.000000 oracledb-2.1.2/tests/test_6600_defaults.py
+-rw-rw-r--   0 root         (0) root         (0)     6689 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_6700_json_23.py
+-rw-rw-r--   0 root         (0) root         (0)     5422 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_6800_error_async.py
+-rw-rw-r--   0 root         (0) root         (0)     2884 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_6900_oson.py
+-rw-rw-r--   0 root         (0) root         (0)     5397 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_7000_connection_async_shortcut_methods.py
+-rw-rw-r--   0 root         (0) root         (0)    24050 2024-03-22 04:07:57.000000 oracledb-2.1.2/tests/test_env.py
+-rw-rw-r--   0 root         (0) root         (0)      596 2024-03-22 04:07:57.000000 oracledb-2.1.2/tox.ini
```

### Comparing `oracledb-2.1.1/LICENSE.txt` & `oracledb-2.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/PKG-INFO` & `oracledb-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oracledb
-Version: 2.1.1
+Version: 2.1.2
 Summary: Python interface to Oracle Database
 Home-page: https://oracle.github.io/python-oracledb
 Author: Anthony Tuininga
 Author-email: anthony.tuininga@oracle.com
 License: Apache and/or UPL
 Project-URL: Installation, https://python-oracledb.readthedocs.io/en/latest/user_guide/installation.html
 Project-URL: Samples, https://github.com/oracle/python-oracledb/tree/main/samples
```

### Comparing `oracledb-2.1.1/README.md` & `oracledb-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/THIRD_PARTY_LICENSES.txt` & `oracledb-2.1.2/THIRD_PARTY_LICENSES.txt`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/setup.cfg` & `oracledb-2.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/setup.py` & `oracledb-2.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/__init__.py` & `oracledb-2.1.2/src/oracledb/__init__.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/aq.py` & `oracledb-2.1.2/src/oracledb/aq.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/base_impl.pxd` & `oracledb-2.1.2/src/oracledb/base_impl.pxd`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/base_impl.pyx` & `oracledb-2.1.2/src/oracledb/base_impl.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/connect_params.py` & `oracledb-2.1.2/src/oracledb/connect_params.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/connection.py` & `oracledb-2.1.2/src/oracledb/connection.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/constants.py` & `oracledb-2.1.2/src/oracledb/constants.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/constructors.py` & `oracledb-2.1.2/src/oracledb/constructors.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/cursor.py` & `oracledb-2.1.2/src/oracledb/cursor.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/dbobject.py` & `oracledb-2.1.2/src/oracledb/dbobject.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/defaults.py` & `oracledb-2.1.2/src/oracledb/defaults.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/driver_mode.py` & `oracledb-2.1.2/src/oracledb/driver_mode.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/dsn.py` & `oracledb-2.1.2/src/oracledb/dsn.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/errors.py` & `oracledb-2.1.2/src/oracledb/errors.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/exceptions.py` & `oracledb-2.1.2/src/oracledb/exceptions.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/fetch_info.py` & `oracledb-2.1.2/src/oracledb/fetch_info.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/future.py` & `oracledb-2.1.2/src/oracledb/future.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/base/bind_var.pyx` & `oracledb-2.1.2/src/oracledb/impl/base/bind_var.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/base/buffer.pyx` & `oracledb-2.1.2/src/oracledb/impl/base/buffer.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/base/connect_params.pyx` & `oracledb-2.1.2/src/oracledb/impl/base/connect_params.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     "description",
     "address"
 ))
 
 # regular expression used for determining if a connect string refers to an Easy
 # Connect string or not
 EASY_CONNECT_PATTERN = \
-        "((?P<protocol>\w+)://)?(?P<host>[^:/]+)(:(?P<port>\d+)?)?/" \
+        "^((?P<protocol>\w+)://)?(?P<host>[\w\d.-]+)(:(?P<port>\d+)?)?/" \
         "(?P<service_name>[^:?]*)(:(?P<server_type>\w+))?"
 
 # dictionary of tnsnames.ora files, indexed by the directory in which the file
 # is found; the results are cached in order to avoid parsing a file multiple
 # times; the modification time of the file is checked each time, though, to
 # ensure that no changes were made since the last time that the file was read
 # and parsed.
```

### Comparing `oracledb-2.1.1/src/oracledb/impl/base/connection.pyx` & `oracledb-2.1.2/src/oracledb/impl/base/connection.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/base/constants.pxi` & `oracledb-2.1.2/src/oracledb/impl/base/constants.pxi`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/base/cursor.pyx` & `oracledb-2.1.2/src/oracledb/impl/base/cursor.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/base/dbobject.pyx` & `oracledb-2.1.2/src/oracledb/impl/base/dbobject.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/base/defaults.pyx` & `oracledb-2.1.2/src/oracledb/impl/base/defaults.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/base/lob.pyx` & `oracledb-2.1.2/src/oracledb/impl/base/lob.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/base/oson.pyx` & `oracledb-2.1.2/src/oracledb/impl/base/oson.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/base/pool.pyx` & `oracledb-2.1.2/src/oracledb/impl/base/pool.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/base/pool_params.pyx` & `oracledb-2.1.2/src/oracledb/impl/base/pool_params.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/base/queue.pyx` & `oracledb-2.1.2/src/oracledb/impl/base/queue.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/base/soda.pyx` & `oracledb-2.1.2/src/oracledb/impl/base/soda.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/base/subscr.pyx` & `oracledb-2.1.2/src/oracledb/impl/base/subscr.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/base/types.pyx` & `oracledb-2.1.2/src/oracledb/impl/base/types.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/base/utils.pyx` & `oracledb-2.1.2/src/oracledb/impl/base/utils.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/base/var.pyx` & `oracledb-2.1.2/src/oracledb/impl/base/var.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/base/vector.pyx` & `oracledb-2.1.2/src/oracledb/impl/base/vector.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/buffer.pyx` & `oracledb-2.1.2/src/oracledb/impl/thick/buffer.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/connection.pyx` & `oracledb-2.1.2/src/oracledb/impl/thick/connection.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/cursor.pyx` & `oracledb-2.1.2/src/oracledb/impl/thick/cursor.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/dbobject.pyx` & `oracledb-2.1.2/src/oracledb/impl/thick/dbobject.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/json.pyx` & `oracledb-2.1.2/src/oracledb/impl/thick/json.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/lob.pyx` & `oracledb-2.1.2/src/oracledb/impl/thick/lob.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/embed/dpi.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/embed/dpi.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/include/dpi.h` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/include/dpi.h`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiConn.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiConn.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiContext.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiContext.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiData.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiData.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiDebug.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiDebug.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiDeqOptions.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiDeqOptions.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiEnqOptions.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiEnqOptions.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiEnv.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiEnv.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiError.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiError.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiErrorMessages.h` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiErrorMessages.h`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiGen.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiGen.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiGlobal.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiGlobal.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiHandleList.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiHandleList.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiHandlePool.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiHandlePool.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiImpl.h` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiImpl.h`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiJson.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiJson.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiLob.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiLob.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiMsgProps.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiMsgProps.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiObject.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiObject.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiObjectAttr.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiObjectAttr.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiObjectType.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiObjectType.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiOci.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiOci.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiOracleType.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiOracleType.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiPool.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiPool.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiQueue.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiQueue.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiRowid.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiRowid.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiSodaColl.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiSodaColl.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiSodaCollCursor.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiSodaCollCursor.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiSodaDb.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiSodaDb.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiSodaDoc.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiSodaDoc.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiSodaDocCursor.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiSodaDocCursor.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiStmt.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiStmt.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiStringList.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiStringList.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiSubscr.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiSubscr.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiUtils.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiUtils.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiVar.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiVar.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi/src/dpiVector.c` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi/src/dpiVector.c`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/odpi.pxd` & `oracledb-2.1.2/src/oracledb/impl/thick/odpi.pxd`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/pool.pyx` & `oracledb-2.1.2/src/oracledb/impl/thick/pool.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/queue.pyx` & `oracledb-2.1.2/src/oracledb/impl/thick/queue.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/soda.pyx` & `oracledb-2.1.2/src/oracledb/impl/thick/soda.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/subscr.pyx` & `oracledb-2.1.2/src/oracledb/impl/thick/subscr.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/utils.pyx` & `oracledb-2.1.2/src/oracledb/impl/thick/utils.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thick/var.pyx` & `oracledb-2.1.2/src/oracledb/impl/thick/var.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thin/capabilities.pyx` & `oracledb-2.1.2/src/oracledb/impl/thin/capabilities.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thin/connection.pyx` & `oracledb-2.1.2/src/oracledb/impl/thin/connection.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thin/constants.pxi` & `oracledb-2.1.2/src/oracledb/impl/thin/constants.pxi`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thin/conversions.pyx` & `oracledb-2.1.2/src/oracledb/impl/thin/conversions.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thin/crypto.pyx` & `oracledb-2.1.2/src/oracledb/impl/thin/crypto.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thin/cursor.pyx` & `oracledb-2.1.2/src/oracledb/impl/thin/cursor.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thin/data_types.pyx` & `oracledb-2.1.2/src/oracledb/impl/thin/data_types.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thin/dbobject.pyx` & `oracledb-2.1.2/src/oracledb/impl/thin/dbobject.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thin/dbobject_cache.pyx` & `oracledb-2.1.2/src/oracledb/impl/thin/dbobject_cache.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thin/lob.pyx` & `oracledb-2.1.2/src/oracledb/impl/thin/lob.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thin/messages.pyx` & `oracledb-2.1.2/src/oracledb/impl/thin/messages.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -770,15 +770,15 @@
             cursor_impl._statement._cursor_id = self.error_info.cursor_id
         if not cursor_impl._statement._is_plsql and not self.in_fetch:
             cursor_impl.rowcount = self.error_info.rowcount
         cursor_impl._lastrowid = self.error_info.rowid
         cursor_impl._batcherrors = self.error_info.batcherrors
         if self.batcherrors and cursor_impl._batcherrors is None:
             cursor_impl._batcherrors = []
-        if self.error_info.num == TNS_ERR_NO_DATA_FOUND:
+        if self.error_info.num == TNS_ERR_NO_DATA_FOUND and self.in_fetch:
             self.error_info.num = 0
             cursor_impl._more_rows_to_fetch = False
             cursor_impl._last_row_index = 0
             self.error_occurred = False
         elif self.error_info.num == TNS_ERR_ARRAY_DML_ERRORS:
             self.error_info.num = 0
             self.error_occurred = False
```

### Comparing `oracledb-2.1.1/src/oracledb/impl/thin/packet.pyx` & `oracledb-2.1.2/src/oracledb/impl/thin/packet.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thin/pool.pyx` & `oracledb-2.1.2/src/oracledb/impl/thin/pool.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thin/protocol.pyx` & `oracledb-2.1.2/src/oracledb/impl/thin/protocol.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thin/statement.pyx` & `oracledb-2.1.2/src/oracledb/impl/thin/statement.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thin/statement_cache.pyx` & `oracledb-2.1.2/src/oracledb/impl/thin/statement_cache.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thin/transport.pyx` & `oracledb-2.1.2/src/oracledb/impl/thin/transport.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thin/utils.pyx` & `oracledb-2.1.2/src/oracledb/impl/thin/utils.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/impl/thin/var.pyx` & `oracledb-2.1.2/src/oracledb/impl/thin/var.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/lob.py` & `oracledb-2.1.2/src/oracledb/lob.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/pool.py` & `oracledb-2.1.2/src/oracledb/pool.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/pool_params.py` & `oracledb-2.1.2/src/oracledb/pool_params.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/soda.py` & `oracledb-2.1.2/src/oracledb/soda.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/subscr.py` & `oracledb-2.1.2/src/oracledb/subscr.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/thick_impl.pyx` & `oracledb-2.1.2/src/oracledb/thick_impl.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/thin_impl.pyx` & `oracledb-2.1.2/src/oracledb/thin_impl.pyx`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/utils.py` & `oracledb-2.1.2/src/oracledb/utils.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/var.py` & `oracledb-2.1.2/src/oracledb/var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/src/oracledb/version.py` & `oracledb-2.1.2/src/oracledb/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 # version.py
 #
 # Defines the version of the package. This is the only place where this is
 # found. The setup.cfg configuration file and the documentation configuration
 # file doc/src/conf.py both reference this file directly.
 # -----------------------------------------------------------------------------
 
-__version__ = "2.1.1"
+__version__ = "2.1.2"
```

### Comparing `oracledb-2.1.1/src/oracledb.egg-info/PKG-INFO` & `oracledb-2.1.2/src/oracledb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oracledb
-Version: 2.1.1
+Version: 2.1.2
 Summary: Python interface to Oracle Database
 Home-page: https://oracle.github.io/python-oracledb
 Author: Anthony Tuininga
 Author-email: anthony.tuininga@oracle.com
 License: Apache and/or UPL
 Project-URL: Installation, https://python-oracledb.readthedocs.io/en/latest/user_guide/installation.html
 Project-URL: Samples, https://github.com/oracle/python-oracledb/tree/main/samples
```

### Comparing `oracledb-2.1.1/src/oracledb.egg-info/SOURCES.txt` & `oracledb-2.1.2/src/oracledb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/create_schema.py` & `oracledb-2.1.2/tests/create_schema.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/drop_schema.py` & `oracledb-2.1.2/tests/drop_schema.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_1000_module.py` & `oracledb-2.1.2/tests/test_1000_module.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_1100_connection.py` & `oracledb-2.1.2/tests/test_1100_connection.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_1300_cursor_var.py` & `oracledb-2.1.2/tests/test_1300_cursor_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_1400_datetime_var.py` & `oracledb-2.1.2/tests/test_1400_datetime_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_1500_types.py` & `oracledb-2.1.2/tests/test_1500_types.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_1600_dml_returning.py` & `oracledb-2.1.2/tests/test_1600_dml_returning.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_1700_error.py` & `oracledb-2.1.2/tests/test_1700_error.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_1800_interval_var.py` & `oracledb-2.1.2/tests/test_1800_interval_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_1900_lob_var.py` & `oracledb-2.1.2/tests/test_1900_lob_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_2000_long_var.py` & `oracledb-2.1.2/tests/test_2000_long_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_2100_nchar_var.py` & `oracledb-2.1.2/tests/test_2100_nchar_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_2200_number_var.py` & `oracledb-2.1.2/tests/test_2200_number_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_2300_object_var.py` & `oracledb-2.1.2/tests/test_2300_object_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_2400_pool.py` & `oracledb-2.1.2/tests/test_2400_pool.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_2500_string_var.py` & `oracledb-2.1.2/tests/test_2500_string_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_2600_timestamp_var.py` & `oracledb-2.1.2/tests/test_2600_timestamp_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_2700_aq.py` & `oracledb-2.1.2/tests/test_2700_aq.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_2800_bulk_aq.py` & `oracledb-2.1.2/tests/test_2800_bulk_aq.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_2900_rowid.py` & `oracledb-2.1.2/tests/test_2900_rowid.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_3000_subscription.py` & `oracledb-2.1.2/tests/test_3000_subscription.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_3100_boolean_var.py` & `oracledb-2.1.2/tests/test_3100_boolean_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_3200_features_12_1.py` & `oracledb-2.1.2/tests/test_3200_features_12_1.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_3300_soda_database.py` & `oracledb-2.1.2/tests/test_3300_soda_database.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_3400_soda_collection.py` & `oracledb-2.1.2/tests/test_3400_soda_collection.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_3500_json.py` & `oracledb-2.1.2/tests/test_3500_json.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_3600_outputtypehandler.py` & `oracledb-2.1.2/tests/test_3600_outputtypehandler.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_3700_var.py` & `oracledb-2.1.2/tests/test_3700_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_3800_typehandler.py` & `oracledb-2.1.2/tests/test_3800_typehandler.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_3900_cursor_execute.py` & `oracledb-2.1.2/tests/test_3900_cursor_execute.py`

 * *Files 1% similar despite different names*

```diff
@@ -550,10 +550,15 @@
         self.assertEqual(self.cursor.rowcount, 0)
         self.cursor.execute("select user from dual")
         self.cursor.fetchall()
         self.assertEqual(self.cursor.rowcount, 1)
         self.cursor.execute("begin null; end;")
         self.assertEqual(self.cursor.rowcount, 0)
 
+    def test_3935(self):
+        "3935 - test raising no_data_found in PL/SQL"
+        with self.assertRaisesFullCode("ORA-01403"):
+            self.cursor.execute("begin raise no_data_found; end;")
+
 
 if __name__ == "__main__":
     test_env.run_test_cases()
```

### Comparing `oracledb-2.1.1/tests/test_4000_cursor_executemany.py` & `oracledb-2.1.2/tests/test_4000_cursor_executemany.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_4100_cursor_callproc.py` & `oracledb-2.1.2/tests/test_4100_cursor_callproc.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_4200_cursor_scrollable.py` & `oracledb-2.1.2/tests/test_4200_cursor_scrollable.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_4300_cursor_other.py` & `oracledb-2.1.2/tests/test_4300_cursor_other.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_4400_tpc.py` & `oracledb-2.1.2/tests/test_4400_tpc.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_4500_connect_params.py` & `oracledb-2.1.2/tests/test_4500_connect_params.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_4600_type_changes.py` & `oracledb-2.1.2/tests/test_4600_type_changes.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_4700_pool_params.py` & `oracledb-2.1.2/tests/test_4700_pool_params.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_4800_timestamp_ltz_var.py` & `oracledb-2.1.2/tests/test_4800_timestamp_ltz_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_4900_timestamp_tz_var.py` & `oracledb-2.1.2/tests/test_4900_timestamp_tz_var.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_5000_externalauth.py` & `oracledb-2.1.2/tests/test_5000_externalauth.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_5100_arrayvar.py` & `oracledb-2.1.2/tests/test_5100_arrayvar.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_5200_sql_parser.py` & `oracledb-2.1.2/tests/test_5200_sql_parser.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_5300_connection_async.py` & `oracledb-2.1.2/tests/test_5300_connection_async.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_5400_cursor_execute_async.py` & `oracledb-2.1.2/tests/test_5400_cursor_execute_async.py`

 * *Files 1% similar despite different names*

```diff
@@ -587,10 +587,15 @@
         values = [f"Test value 5435 - {i}" for i in range(1, 301)]
         columns = ", ".join(f"'{v}'" for v in values)
         query = f"select {columns} from dual"
         await self.cursor.execute(query)
         row = await self.cursor.fetchone()
         self.assertEqual(row, tuple(values))
 
+    async def test_5436(self):
+        "5436 - test raising no_data_found in PL/SQL"
+        with self.assertRaisesFullCode("ORA-01403"):
+            await self.cursor.execute("begin raise no_data_found; end;")
+
 
 if __name__ == "__main__":
     test_env.run_test_cases()
```

### Comparing `oracledb-2.1.1/tests/test_5500_pool_async.py` & `oracledb-2.1.2/tests/test_5500_pool_async.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_5600_dbobject_async.py` & `oracledb-2.1.2/tests/test_5600_dbobject_async.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_5700_lob_var_async.py` & `oracledb-2.1.2/tests/test_5700_lob_var_async.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_5800_cursor_var_async.py` & `oracledb-2.1.2/tests/test_5800_cursor_var_async.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_5900_dml_returning_async.py` & `oracledb-2.1.2/tests/test_5900_dml_returning_async.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_6000_typehandler_async.py` & `oracledb-2.1.2/tests/test_6000_typehandler_async.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_6100_cursor_executemany_async.py` & `oracledb-2.1.2/tests/test_6100_cursor_executemany_async.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_6200_cursor_callproc_async.py` & `oracledb-2.1.2/tests/test_6200_cursor_callproc_async.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_6300_cursor_other_async.py` & `oracledb-2.1.2/tests/test_6300_cursor_other_async.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_6600_defaults.py` & `oracledb-2.1.2/tests/test_6600_defaults.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_6700_json_23.py` & `oracledb-2.1.2/tests/test_6700_json_23.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_6800_error_async.py` & `oracledb-2.1.2/tests/test_6800_error_async.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_6900_oson.py` & `oracledb-2.1.2/tests/test_6900_oson.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_7000_connection_async_shortcut_methods.py` & `oracledb-2.1.2/tests/test_7000_connection_async_shortcut_methods.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tests/test_env.py` & `oracledb-2.1.2/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `oracledb-2.1.1/tox.ini` & `oracledb-2.1.2/tox.ini`

 * *Files identical despite different names*

