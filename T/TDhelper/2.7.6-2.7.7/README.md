# Comparing `tmp/TDhelper-2.7.6.tar.gz` & `tmp/TDhelper-2.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TDhelper-2.7.6.tar", last modified: Fri Apr  5 17:00:58 2024, max compression
+gzip compressed data, was "TDhelper-2.7.7.tar", last modified: Thu May  2 12:33:35 2024, max compression
```

## Comparing `TDhelper-2.7.6.tar` & `TDhelper-2.7.7.tar`

### file list

```diff
@@ -1,246 +1,246 @@
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.561638 TDhelper-2.7.6/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11361 2024-03-30 13:11:32.000000 TDhelper-2.7.6/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2889 2024-04-05 17:00:58.561638 TDhelper-2.7.6/PKG-INFO
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2573 2024-03-30 13:11:32.000000 TDhelper-2.7.6/README.md
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.451639 TDhelper-2.7.6/TDhelper/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.451639 TDhelper-2.7.6/TDhelper/Decorators/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Decorators/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      904 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Decorators/log.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      649 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Decorators/performance.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.451639 TDhelper-2.7.6/TDhelper/Event/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4150 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Event/Event.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Event/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.451639 TDhelper-2.7.6/TDhelper/Event/classEvent/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Event/classEvent/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1273 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Event/classEvent/event.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      966 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Event/classEvent/meta.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.451639 TDhelper-2.7.6/TDhelper/Event/webEvent/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    31736 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Event/webEvent/Events.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Event/webEvent/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.461639 TDhelper-2.7.6/TDhelper/MagicCls/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      105 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/MagicCls/FieldsType.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1740 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/MagicCls/MagicMeta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       74 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/MagicCls/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1978 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/MagicCls/model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      892 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/MagicCls/test.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.461639 TDhelper-2.7.6/TDhelper/Msg/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1165 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Msg/AppPush.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2564 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Msg/Config.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2170 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Msg/Email.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1438 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Msg/InterfaceMsg.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2112 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/Msg/SMS.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Msg/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.471639 TDhelper-2.7.6/TDhelper/Scheduler/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Scheduler/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      742 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Scheduler/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      750 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Scheduler/example_scheduler.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      828 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Scheduler/interface.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1620 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Scheduler/log_config.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4208 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Scheduler/service.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.471639 TDhelper-2.7.6/TDhelper/Spider/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Spider/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       63 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Spider/cfg.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8542 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/Spider/contentExtraction.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.471639 TDhelper-2.7.6/TDhelper/Spider/models/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      976 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Spider/models/BadRequestModel.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2619 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Spider/models/Cache_L1.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1332 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Spider/models/Cache_L2.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2137 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Spider/models/Cache_L2_Model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Spider/models/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      853 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Spider/models/fingerprint.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      243 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Spider/models/spider_event.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1702 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Spider/models/status.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    43496 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Spider/regex.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       50 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/Spider/spiderFactory.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    10838 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/Spider/spiderPools.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       73 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5366 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/apiCore.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.471639 TDhelper-2.7.6/TDhelper/bin/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/bin/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      541 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/bin/globalvar.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.471639 TDhelper-2.7.6/TDhelper/cache/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/cache/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      948 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/cache/memcache.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1130 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/cache/pools.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2739 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/cache/ring.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.471639 TDhelper-2.7.6/TDhelper/cache/webCache/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/cache/webCache/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      861 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/cache/webCache/interface.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2964 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/cache/webCache/mongo.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/cache/webCache/redis.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1228 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/cache/webCache/webCacheFactory.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.471639 TDhelper-2.7.6/TDhelper/db/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.471639 TDhelper-2.7.6/TDhelper/db/Db/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/db/Db/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1235 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/db/Db/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      238 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/db/Db/helper.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/db/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.481639 TDhelper-2.7.6/TDhelper/db/mongodb/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/db/mongodb/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1116 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/db/mongodb/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3718 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/db/mongodb/dbhelper.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1919 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/db/mongodb/objectId.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.481639 TDhelper-2.7.6/TDhelper/db/mongodb/orm/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      737 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/db/mongodb/orm/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.481639 TDhelper-2.7.6/TDhelper/db/mongodb/orm/core/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/db/mongodb/orm/core/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1093 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/db/mongodb/orm/core/attribute.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      691 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/db/mongodb/orm/core/field.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      194 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/db/mongodb/orm/core/field_type.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5506 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/db/mongodb/orm/core/meta copy.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5811 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/db/mongodb/orm/core/meta.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.481639 TDhelper-2.7.6/TDhelper/db/mongodb/orm/drives/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/db/mongodb/orm/drives/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1356 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/db/mongodb/orm/drives/conn.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       44 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/db/mongodb/setting.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.481639 TDhelper-2.7.6/TDhelper/db/mysql/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/db/mysql/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      510 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/db/mysql/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/db/mysql/model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1151 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/db/mysql/mysql_x.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      126 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/db/mysql/setting.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.481639 TDhelper-2.7.6/TDhelper/document/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       24 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/document/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.481639 TDhelper-2.7.6/TDhelper/document/excel/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.481639 TDhelper-2.7.6/TDhelper/document/excel/FieldType/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      104 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/document/excel/FieldType/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       36 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/document/excel/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.481639 TDhelper-2.7.6/TDhelper/document/excel/meta/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       21 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/document/excel/meta/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3942 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/document/excel/meta/modelMeta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      818 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/document/excel/model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      622 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/document/file.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.481639 TDhelper-2.7.6/TDhelper/document/ini/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/document/ini/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      123 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/document/ini/fields.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1718 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/document/ini/meta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      440 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/document/ini/model.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      309 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/document/ini/test.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.491639 TDhelper-2.7.6/TDhelper/generic/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2222 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/generic/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1402 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/generic/classDocCfg.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.491639 TDhelper-2.7.6/TDhelper/generic/crypto/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1413 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/generic/crypto/MD5.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/generic/crypto/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4668 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/generic/dictHelper.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.491639 TDhelper-2.7.6/TDhelper/generic/dynamic/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/generic/dynamic/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.491639 TDhelper-2.7.6/TDhelper/generic/dynamic/base/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2782 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/generic/dynamic/base/Meta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/generic/dynamic/base/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2825 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/generic/dynamic/delete__test.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1417 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/generic/findAttribute.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      144 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/generic/randGetValue.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1146 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/generic/recursion.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5634 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/generic/requier.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3721 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/generic/standard_result.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4808 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/generic/threadPools.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3886 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/generic/transformationType.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.491639 TDhelper-2.7.6/TDhelper/network/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.491639 TDhelper-2.7.6/TDhelper/network/http/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8002 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/network/http/REST_HTTP.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    61039 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/http/RPC.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    34603 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/http/RPC1.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/http/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4663 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/http/http_helper.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3588 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/http/http_postdataformat.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    26267 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/http/m3u8.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    26805 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/http/m3u8_backup.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.491639 TDhelper-2.7.6/TDhelper/network/http/status/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      165 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/http/status/M3U8_STATUS.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/http/status/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.491639 TDhelper-2.7.6/TDhelper/network/rpc/
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.491639 TDhelper-2.7.6/TDhelper/network/rpc/Client/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/rpc/Client/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6791 2024-04-05 16:53:00.000000 TDhelper-2.7.6/TDhelper/network/rpc/Client/rpc.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13184 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/network/rpc/Client/service.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.531638 TDhelper-2.7.6/TDhelper/network/rpc/Core/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2141 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/rpc/Core/Meta.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/rpc/Core/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    16875 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/network/rpc/Core/obsolete_struct.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    17314 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/network/rpc/Core/struct.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2452 2024-04-05 16:57:20.000000 TDhelper-2.7.6/TDhelper/network/rpc/Core/token.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.531638 TDhelper-2.7.6/TDhelper/network/rpc/Generic/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7538 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/network/rpc/Generic/Host.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/rpc/Generic/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.531638 TDhelper-2.7.6/TDhelper/network/rpc/Server/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/rpc/Server/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7837 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/rpc/Server/obsolete_Service.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4207 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/network/rpc/Server/server.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.531638 TDhelper-2.7.6/TDhelper/network/rpc/Struct/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2202 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/rpc/Struct/Result.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/rpc/Struct/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/rpc/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.531638 TDhelper-2.7.6/TDhelper/network/socket/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2001 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/socket/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.531638 TDhelper-2.7.6/TDhelper/network/socket/cache/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/socket/cache/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      518 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/socket/cache/queue.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2371 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/socket/client.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.531638 TDhelper-2.7.6/TDhelper/network/socket/model/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      757 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/socket/model/SOCKET_MODELS.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/socket/model/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.531638 TDhelper-2.7.6/TDhelper/network/socket/protocol/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/socket/protocol/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4531 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/socket/protocol/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4163 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/socket/server.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.531638 TDhelper-2.7.6/TDhelper/network/websocket/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/websocket/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3485 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/websocket/protocol.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1433 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/network/websocket/server.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1901 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/reflect.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.531638 TDhelper-2.7.6/TDhelper/robot/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/robot/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.531638 TDhelper-2.7.6/TDhelper/robot/control/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1149 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/robot/control/D_33890.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/robot/control/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1296 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/robot/control/device.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.531638 TDhelper-2.7.6/TDhelper/robot/people/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1117 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/robot/people/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5622 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/robot/people/leg.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.531638 TDhelper-2.7.6/TDhelper/robot/people/scripts/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/robot/people/scripts/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3111 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/robot/people/scripts/runScript.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1142 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/robot/people/scripts/script.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/robot/people/upperLimb.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/robot/people/vertebra.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.551638 TDhelper-2.7.6/TDhelper/robot/struct/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/robot/struct/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      621 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/robot/struct/ankle.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2131 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/robot/struct/base.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      613 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/robot/struct/hip.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      618 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/robot/struct/knee.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      697 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/robot/struct/toe.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.551638 TDhelper-2.7.6/TDhelper/shellScripts/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      335 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/shellScripts/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3431 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/shellScripts/saasHelper.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.561638 TDhelper-2.7.6/TDhelper/simulate/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/simulate/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2713 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/simulate/json.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.561638 TDhelper-2.7.6/TDhelper/structs/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/structs/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4359 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/structs/dir.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.561638 TDhelper-2.7.6/TDhelper/web/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.6/TDhelper/web/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8255 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/web/obsolete_permission.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6908 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/web/obsolete_permissionHelper.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.561638 TDhelper-2.7.6/TDhelper/web/utils/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/web/utils/__init__.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.561638 TDhelper-2.7.6/TDhelper/web/utils/event/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/web/utils/event/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/web/utils/event/client.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/web/utils/event/server.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.561638 TDhelper-2.7.6/TDhelper/web/utils/permission/
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/web/utils/permission/__init__.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3478 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/web/utils/permission/client.py
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3903 2024-03-30 15:55:54.000000 TDhelper-2.7.6/TDhelper/web/utils/permission/server.py
-drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-05 17:00:58.451639 TDhelper-2.7.6/TDhelper.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     2889 2024-04-05 17:00:58.000000 TDhelper-2.7.6/TDhelper.egg-info/PKG-INFO
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6204 2024-04-05 17:00:58.000000 TDhelper-2.7.6/TDhelper.egg-info/SOURCES.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-05 17:00:58.000000 TDhelper-2.7.6/TDhelper.egg-info/dependency_links.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       62 2024-04-05 17:00:58.000000 TDhelper-2.7.6/TDhelper.egg-info/entry_points.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       91 2024-04-05 17:00:58.000000 TDhelper-2.7.6/TDhelper.egg-info/requires.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-04-05 17:00:58.000000 TDhelper-2.7.6/TDhelper.egg-info/top_level.txt
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-05 17:00:58.561638 TDhelper-2.7.6/setup.cfg
--rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1021 2024-04-05 17:00:52.000000 TDhelper-2.7.6/setup.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.788298 TDhelper-2.7.7/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    11361 2024-03-30 13:11:32.000000 TDhelper-2.7.7/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3108 2024-05-02 12:33:35.758298 TDhelper-2.7.7/PKG-INFO
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2792 2024-04-06 07:30:35.000000 TDhelper-2.7.7/README.md
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.518298 TDhelper-2.7.7/TDhelper/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.518298 TDhelper-2.7.7/TDhelper/Decorators/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Decorators/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      904 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Decorators/log.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      649 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Decorators/performance.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.518298 TDhelper-2.7.7/TDhelper/Event/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4150 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Event/Event.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Event/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.528298 TDhelper-2.7.7/TDhelper/Event/classEvent/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Event/classEvent/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1273 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Event/classEvent/event.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      966 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Event/classEvent/meta.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.528298 TDhelper-2.7.7/TDhelper/Event/webEvent/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    31736 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Event/webEvent/Events.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Event/webEvent/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.548298 TDhelper-2.7.7/TDhelper/MagicCls/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      105 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/MagicCls/FieldsType.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1740 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/MagicCls/MagicMeta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       74 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/MagicCls/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1978 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/MagicCls/model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      892 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/MagicCls/test.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.568298 TDhelper-2.7.7/TDhelper/Msg/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1165 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Msg/AppPush.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2564 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Msg/Config.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2170 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Msg/Email.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1438 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Msg/InterfaceMsg.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2112 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/Msg/SMS.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Msg/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.568298 TDhelper-2.7.7/TDhelper/Scheduler/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Scheduler/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      742 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Scheduler/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      750 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Scheduler/example_scheduler.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      828 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Scheduler/interface.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1620 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Scheduler/log_config.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4208 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Scheduler/service.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.568298 TDhelper-2.7.7/TDhelper/Spider/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Spider/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       63 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Spider/cfg.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8542 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/Spider/contentExtraction.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.598298 TDhelper-2.7.7/TDhelper/Spider/models/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      976 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Spider/models/BadRequestModel.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2619 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Spider/models/Cache_L1.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1332 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Spider/models/Cache_L2.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2137 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Spider/models/Cache_L2_Model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Spider/models/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      853 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Spider/models/fingerprint.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      243 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Spider/models/spider_event.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1702 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Spider/models/status.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    43496 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Spider/regex.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       50 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/Spider/spiderFactory.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    10838 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/Spider/spiderPools.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       73 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5366 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/apiCore.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.598298 TDhelper-2.7.7/TDhelper/bin/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/bin/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      541 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/bin/globalvar.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.598298 TDhelper-2.7.7/TDhelper/cache/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/cache/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      948 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/cache/memcache.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1130 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/cache/pools.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2739 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/cache/ring.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.608298 TDhelper-2.7.7/TDhelper/cache/webCache/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/cache/webCache/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      861 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/cache/webCache/interface.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2964 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/cache/webCache/mongo.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/cache/webCache/redis.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1228 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/cache/webCache/webCacheFactory.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.608298 TDhelper-2.7.7/TDhelper/db/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.628298 TDhelper-2.7.7/TDhelper/db/Db/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/db/Db/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1235 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/db/Db/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      238 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/db/Db/helper.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/db/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.638298 TDhelper-2.7.7/TDhelper/db/mongodb/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/db/mongodb/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1116 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/db/mongodb/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3718 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/db/mongodb/dbhelper.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1919 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/db/mongodb/objectId.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.638298 TDhelper-2.7.7/TDhelper/db/mongodb/orm/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      737 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/db/mongodb/orm/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.658298 TDhelper-2.7.7/TDhelper/db/mongodb/orm/core/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/db/mongodb/orm/core/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1093 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/db/mongodb/orm/core/attribute.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      691 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/db/mongodb/orm/core/field.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      194 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/db/mongodb/orm/core/field_type.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5506 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/db/mongodb/orm/core/meta copy.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5811 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/db/mongodb/orm/core/meta.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.658298 TDhelper-2.7.7/TDhelper/db/mongodb/orm/drives/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/db/mongodb/orm/drives/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1356 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/db/mongodb/orm/drives/conn.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       44 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/db/mongodb/setting.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.658298 TDhelper-2.7.7/TDhelper/db/mysql/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/db/mysql/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      510 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/db/mysql/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/db/mysql/model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1151 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/db/mysql/mysql_x.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      126 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/db/mysql/setting.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.658298 TDhelper-2.7.7/TDhelper/document/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       24 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/document/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.658298 TDhelper-2.7.7/TDhelper/document/excel/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.658298 TDhelper-2.7.7/TDhelper/document/excel/FieldType/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      104 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/document/excel/FieldType/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       36 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/document/excel/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.668298 TDhelper-2.7.7/TDhelper/document/excel/meta/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)       21 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/document/excel/meta/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3942 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/document/excel/meta/modelMeta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      818 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/document/excel/model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      622 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/document/file.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.668298 TDhelper-2.7.7/TDhelper/document/ini/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/document/ini/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      123 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/document/ini/fields.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1718 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/document/ini/meta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      440 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/document/ini/model.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      309 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/document/ini/test.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.688298 TDhelper-2.7.7/TDhelper/generic/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2222 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/generic/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1402 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/generic/classDocCfg.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.688298 TDhelper-2.7.7/TDhelper/generic/crypto/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1413 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/generic/crypto/MD5.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/generic/crypto/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4668 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/generic/dictHelper.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.688298 TDhelper-2.7.7/TDhelper/generic/dynamic/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/generic/dynamic/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.688298 TDhelper-2.7.7/TDhelper/generic/dynamic/base/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2782 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/generic/dynamic/base/Meta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/generic/dynamic/base/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2825 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/generic/dynamic/delete__test.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1417 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/generic/findAttribute.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      144 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/generic/randGetValue.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1146 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/generic/recursion.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5634 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/generic/requier.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3721 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/generic/standard_result.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4808 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/generic/threadPools.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3886 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/generic/transformationType.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.688298 TDhelper-2.7.7/TDhelper/network/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.688298 TDhelper-2.7.7/TDhelper/network/http/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8002 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/network/http/REST_HTTP.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    61039 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/http/RPC.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    34603 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/http/RPC1.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/http/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4663 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/http/http_helper.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3588 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/http/http_postdataformat.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    26267 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/http/m3u8.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    26805 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/http/m3u8_backup.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.688298 TDhelper-2.7.7/TDhelper/network/http/status/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      165 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/http/status/M3U8_STATUS.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/http/status/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.688298 TDhelper-2.7.7/TDhelper/network/rpc/
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.698298 TDhelper-2.7.7/TDhelper/network/rpc/Client/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/rpc/Client/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6791 2024-04-05 16:53:00.000000 TDhelper-2.7.7/TDhelper/network/rpc/Client/rpc.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    13184 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/network/rpc/Client/service.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.698298 TDhelper-2.7.7/TDhelper/network/rpc/Core/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2141 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/rpc/Core/Meta.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/rpc/Core/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    16875 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/network/rpc/Core/obsolete_struct.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)    17314 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/network/rpc/Core/struct.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2452 2024-04-05 16:57:20.000000 TDhelper-2.7.7/TDhelper/network/rpc/Core/token.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.698298 TDhelper-2.7.7/TDhelper/network/rpc/Generic/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7538 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/network/rpc/Generic/Host.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/rpc/Generic/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.698298 TDhelper-2.7.7/TDhelper/network/rpc/Server/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/rpc/Server/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     7837 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/rpc/Server/obsolete_Service.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4207 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/network/rpc/Server/server.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.718298 TDhelper-2.7.7/TDhelper/network/rpc/Struct/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2202 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/rpc/Struct/Result.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/rpc/Struct/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/rpc/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.718298 TDhelper-2.7.7/TDhelper/network/socket/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2001 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/socket/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.718298 TDhelper-2.7.7/TDhelper/network/socket/cache/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/socket/cache/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      518 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/socket/cache/queue.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2371 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/socket/client.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.718298 TDhelper-2.7.7/TDhelper/network/socket/model/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      757 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/socket/model/SOCKET_MODELS.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/socket/model/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.738298 TDhelper-2.7.7/TDhelper/network/socket/protocol/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/socket/protocol/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4531 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/socket/protocol/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4163 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/socket/server.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.738298 TDhelper-2.7.7/TDhelper/network/websocket/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/websocket/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3485 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/websocket/protocol.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1433 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/network/websocket/server.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1901 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/reflect.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.738298 TDhelper-2.7.7/TDhelper/robot/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/robot/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.738298 TDhelper-2.7.7/TDhelper/robot/control/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1149 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/robot/control/D_33890.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/robot/control/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1296 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/robot/control/device.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.738298 TDhelper-2.7.7/TDhelper/robot/people/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1117 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/robot/people/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     5622 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/robot/people/leg.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.758298 TDhelper-2.7.7/TDhelper/robot/people/scripts/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/robot/people/scripts/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3111 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/robot/people/scripts/runScript.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1142 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/robot/people/scripts/script.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/robot/people/upperLimb.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/robot/people/vertebra.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.758298 TDhelper-2.7.7/TDhelper/robot/struct/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/robot/struct/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      621 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/robot/struct/ankle.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2131 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/robot/struct/base.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      613 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/robot/struct/hip.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      618 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/robot/struct/knee.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      697 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/robot/struct/toe.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.758298 TDhelper-2.7.7/TDhelper/shellScripts/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)      335 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/shellScripts/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3431 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/shellScripts/saasHelper.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.758298 TDhelper-2.7.7/TDhelper/simulate/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/simulate/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     2713 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/simulate/json.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.758298 TDhelper-2.7.7/TDhelper/structs/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/structs/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4359 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/structs/dir.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.758298 TDhelper-2.7.7/TDhelper/web/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 13:11:32.000000 TDhelper-2.7.7/TDhelper/web/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     8255 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/web/obsolete_permission.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     6908 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/web/obsolete_permissionHelper.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.758298 TDhelper-2.7.7/TDhelper/web/utils/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/web/utils/__init__.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.758298 TDhelper-2.7.7/TDhelper/web/utils/event/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/web/utils/event/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/web/utils/event/client.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/web/utils/event/server.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.758298 TDhelper-2.7.7/TDhelper/web/utils/permission/
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)        0 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/web/utils/permission/__init__.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     3478 2024-03-30 15:55:54.000000 TDhelper-2.7.7/TDhelper/web/utils/permission/client.py
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     4060 2024-05-02 12:33:06.000000 TDhelper-2.7.7/TDhelper/web/utils/permission/server.py
+drwxr-xr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-05-02 12:33:35.518298 TDhelper-2.7.7/TDhelper.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     3108 2024-05-02 12:33:34.000000 TDhelper-2.7.7/TDhelper.egg-info/PKG-INFO
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)     6204 2024-05-02 12:33:35.000000 TDhelper-2.7.7/TDhelper.egg-info/SOURCES.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-05-02 12:33:34.000000 TDhelper-2.7.7/TDhelper.egg-info/dependency_links.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       62 2024-05-02 12:33:34.000000 TDhelper-2.7.7/TDhelper.egg-info/entry_points.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       91 2024-05-02 12:33:34.000000 TDhelper-2.7.7/TDhelper.egg-info/requires.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-05-02 12:33:34.000000 TDhelper-2.7.7/TDhelper.egg-info/top_level.txt
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-05-02 12:33:35.788298 TDhelper-2.7.7/setup.cfg
+-rwxrwxrwx   0 ubuntu    (1000) ubuntu    (1000)     1021 2024-05-02 12:33:24.000000 TDhelper-2.7.7/setup.py
```

### Comparing `TDhelper-2.7.6/LICENSE` & `TDhelper-2.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/PKG-INFO` & `TDhelper-2.7.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-Metadata-Version: 2.1
-Name: TDhelper
-Version: 2.7.6
-Summary: reconsitution web.permissionHelper cls.
-Home-page: https://gitee.com/TonyDon/pyLib
-Author: TangJing
-Author-email: yeihizhi@163.com
-License: Apache 2.0
-Keywords: pip,TDhelper,featureextraction
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # TDhelper LIb
 helper class lib.
+# ***Saas-Framework Cli***
+## 1. Create saas project command line   
+
+### custom directory   
+```
+saas --name "project name" --path /usr/www/
+```
+### current directory
+```
+saas --name "project name" --path pathname
+```
 
 # ***Cache***
 
 ## 1. pools
 ## 2. ring cache
 
 # ***db***
```

#### html2text {}

```diff
@@ -1,21 +1,19 @@
-Metadata-Version: 2.1 Name: TDhelper Version: 2.7.6 Summary: reconsitution
-web.permissionHelper cls. Home-page: https://gitee.com/TonyDon/pyLib Author:
-TangJing Author-email: yeihizhi@163.com License: Apache 2.0 Keywords:
-pip,TDhelper,featureextraction Description-Content-Type: text/markdown License-
-File: LICENSE # TDhelper LIb helper class lib. # ***Cache*** ## 1. pools ## 2.
-ring cache # ***db*** ## 1. sqllite ## 2. mongodb ## 3. mysql #
-***Decorators*** ## 1. log # ***document*** ## 1. file ## 2. excel #
-***Event*** ## 1. Event ## 2. classEvent ## 3. webEvent # ***generic*** #
-***MagicCls*** running time dynamic create class. mapping any object to an
-object. # ***Msg*** genneric msg helper class. # ***network*** http, socket
-helper. # ***robot*** robot class. # ***Scheduler*** not finished #
-***simulate*** not finished # ***Spider*** # ***structs*** not finished #
-***web*** ## permission module ### ***1. register*** permission register class.
-#### ***Methods***
+# TDhelper LIb helper class lib. # ***Saas-Framework Cli*** ## 1. Create saas
+project command line ### custom directory ``` saas --name "project name" --path
+/usr/www/ ``` ### current directory ``` saas --name "project name" --path
+pathname ``` # ***Cache*** ## 1. pools ## 2. ring cache # ***db*** ## 1.
+sqllite ## 2. mongodb ## 3. mysql # ***Decorators*** ## 1. log # ***document***
+## 1. file ## 2. excel # ***Event*** ## 1. Event ## 2. classEvent ## 3.
+webEvent # ***generic*** # ***MagicCls*** running time dynamic create class.
+mapping any object to an object. # ***Msg*** genneric msg helper class. #
+***network*** http, socket helper. # ***robot*** robot class. # ***Scheduler***
+not finished # ***simulate*** not finished # ***Spider*** # ***structs*** not
+finished # ***web*** ## permission module ### ***1. register*** permission
+register class. #### ***Methods***
 NO.
 |
 name
 |
 description
 :---:|:---|:--- 1 | [Register](#perRegister) | - 2 | [RegisterByCfg]
 (#perRegisterByCfg) | - _*_*_*_R_e_g_i_s_t_e_r_*_*_*
```

### Comparing `TDhelper-2.7.6/TDhelper/Decorators/log.py` & `TDhelper-2.7.7/TDhelper/Decorators/log.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/Decorators/performance.py` & `TDhelper-2.7.7/TDhelper/Decorators/performance.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/Event/Event.py` & `TDhelper-2.7.7/TDhelper/Event/Event.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/Event/classEvent/event.py` & `TDhelper-2.7.7/TDhelper/Event/classEvent/event.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/Event/classEvent/meta.py` & `TDhelper-2.7.7/TDhelper/Event/classEvent/meta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/Event/webEvent/Events.py` & `TDhelper-2.7.7/TDhelper/Event/webEvent/Events.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/MagicCls/MagicMeta.py` & `TDhelper-2.7.7/TDhelper/MagicCls/MagicMeta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/MagicCls/model.py` & `TDhelper-2.7.7/TDhelper/MagicCls/model.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/MagicCls/test.py` & `TDhelper-2.7.7/TDhelper/MagicCls/test.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/Msg/AppPush.py` & `TDhelper-2.7.7/TDhelper/Msg/AppPush.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/Msg/Config.py` & `TDhelper-2.7.7/TDhelper/Msg/Config.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/Msg/Email.py` & `TDhelper-2.7.7/TDhelper/Msg/Email.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/Msg/InterfaceMsg.py` & `TDhelper-2.7.7/TDhelper/Msg/InterfaceMsg.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/Msg/SMS.py` & `TDhelper-2.7.7/TDhelper/Msg/SMS.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/Scheduler/base.py` & `TDhelper-2.7.7/TDhelper/Scheduler/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/Scheduler/example_scheduler.py` & `TDhelper-2.7.7/TDhelper/Scheduler/example_scheduler.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/Scheduler/interface.py` & `TDhelper-2.7.7/TDhelper/Scheduler/interface.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/Scheduler/log_config.py` & `TDhelper-2.7.7/TDhelper/Scheduler/log_config.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/Scheduler/service.py` & `TDhelper-2.7.7/TDhelper/Scheduler/service.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/Spider/contentExtraction.py` & `TDhelper-2.7.7/TDhelper/Spider/contentExtraction.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/Spider/models/BadRequestModel.py` & `TDhelper-2.7.7/TDhelper/Spider/models/BadRequestModel.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/Spider/models/Cache_L1.py` & `TDhelper-2.7.7/TDhelper/Spider/models/Cache_L1.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/Spider/models/Cache_L2.py` & `TDhelper-2.7.7/TDhelper/Spider/models/Cache_L2.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/Spider/models/Cache_L2_Model.py` & `TDhelper-2.7.7/TDhelper/Spider/models/Cache_L2_Model.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/Spider/models/fingerprint.py` & `TDhelper-2.7.7/TDhelper/Spider/models/fingerprint.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/Spider/models/status.py` & `TDhelper-2.7.7/TDhelper/Spider/models/status.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/Spider/regex.py` & `TDhelper-2.7.7/TDhelper/Spider/regex.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/Spider/spiderPools.py` & `TDhelper-2.7.7/TDhelper/Spider/spiderPools.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/apiCore.py` & `TDhelper-2.7.7/TDhelper/apiCore.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/bin/globalvar.py` & `TDhelper-2.7.7/TDhelper/bin/globalvar.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/cache/memcache.py` & `TDhelper-2.7.7/TDhelper/cache/memcache.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/cache/pools.py` & `TDhelper-2.7.7/TDhelper/cache/pools.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/cache/ring.py` & `TDhelper-2.7.7/TDhelper/cache/ring.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/cache/webCache/interface.py` & `TDhelper-2.7.7/TDhelper/cache/webCache/interface.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/cache/webCache/mongo.py` & `TDhelper-2.7.7/TDhelper/cache/webCache/mongo.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/cache/webCache/webCacheFactory.py` & `TDhelper-2.7.7/TDhelper/cache/webCache/webCacheFactory.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/db/Db/base.py` & `TDhelper-2.7.7/TDhelper/db/Db/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/db/mongodb/base.py` & `TDhelper-2.7.7/TDhelper/db/mongodb/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/db/mongodb/dbhelper.py` & `TDhelper-2.7.7/TDhelper/db/mongodb/dbhelper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/db/mongodb/objectId.py` & `TDhelper-2.7.7/TDhelper/db/mongodb/objectId.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/db/mongodb/orm/__init__.py` & `TDhelper-2.7.7/TDhelper/db/mongodb/orm/__init__.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/db/mongodb/orm/core/attribute.py` & `TDhelper-2.7.7/TDhelper/db/mongodb/orm/core/attribute.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/db/mongodb/orm/core/field.py` & `TDhelper-2.7.7/TDhelper/db/mongodb/orm/core/field.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/db/mongodb/orm/core/meta copy.py` & `TDhelper-2.7.7/TDhelper/db/mongodb/orm/core/meta copy.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/db/mongodb/orm/core/meta.py` & `TDhelper-2.7.7/TDhelper/db/mongodb/orm/core/meta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/db/mongodb/orm/drives/conn.py` & `TDhelper-2.7.7/TDhelper/db/mongodb/orm/drives/conn.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/db/mysql/mysql_x.py` & `TDhelper-2.7.7/TDhelper/db/mysql/mysql_x.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/document/excel/meta/modelMeta.py` & `TDhelper-2.7.7/TDhelper/document/excel/meta/modelMeta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/document/excel/model.py` & `TDhelper-2.7.7/TDhelper/document/excel/model.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/document/file.py` & `TDhelper-2.7.7/TDhelper/document/file.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/document/ini/meta.py` & `TDhelper-2.7.7/TDhelper/document/ini/meta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/generic/__init__.py` & `TDhelper-2.7.7/TDhelper/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/generic/classDocCfg.py` & `TDhelper-2.7.7/TDhelper/generic/classDocCfg.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/generic/crypto/MD5.py` & `TDhelper-2.7.7/TDhelper/generic/crypto/MD5.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/generic/dictHelper.py` & `TDhelper-2.7.7/TDhelper/generic/dictHelper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/generic/dynamic/base/Meta.py` & `TDhelper-2.7.7/TDhelper/generic/dynamic/base/Meta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/generic/dynamic/delete__test.py` & `TDhelper-2.7.7/TDhelper/generic/dynamic/delete__test.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/generic/findAttribute.py` & `TDhelper-2.7.7/TDhelper/generic/findAttribute.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/generic/recursion.py` & `TDhelper-2.7.7/TDhelper/generic/recursion.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/generic/requier.py` & `TDhelper-2.7.7/TDhelper/generic/requier.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/generic/standard_result.py` & `TDhelper-2.7.7/TDhelper/generic/standard_result.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/generic/threadPools.py` & `TDhelper-2.7.7/TDhelper/generic/threadPools.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/generic/transformationType.py` & `TDhelper-2.7.7/TDhelper/generic/transformationType.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/network/http/REST_HTTP.py` & `TDhelper-2.7.7/TDhelper/network/http/REST_HTTP.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/network/http/RPC.py` & `TDhelper-2.7.7/TDhelper/network/http/RPC.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/network/http/RPC1.py` & `TDhelper-2.7.7/TDhelper/network/http/RPC1.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/network/http/http_helper.py` & `TDhelper-2.7.7/TDhelper/network/http/http_helper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/network/http/http_postdataformat.py` & `TDhelper-2.7.7/TDhelper/network/http/http_postdataformat.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/network/http/m3u8.py` & `TDhelper-2.7.7/TDhelper/network/http/m3u8.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/network/http/m3u8_backup.py` & `TDhelper-2.7.7/TDhelper/network/http/m3u8_backup.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/network/rpc/Client/rpc.py` & `TDhelper-2.7.7/TDhelper/network/rpc/Client/rpc.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/network/rpc/Client/service.py` & `TDhelper-2.7.7/TDhelper/network/rpc/Client/service.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/network/rpc/Core/Meta.py` & `TDhelper-2.7.7/TDhelper/network/rpc/Core/Meta.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/network/rpc/Core/obsolete_struct.py` & `TDhelper-2.7.7/TDhelper/network/rpc/Core/obsolete_struct.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/network/rpc/Core/struct.py` & `TDhelper-2.7.7/TDhelper/network/rpc/Core/struct.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/network/rpc/Core/token.py` & `TDhelper-2.7.7/TDhelper/network/rpc/Core/token.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/network/rpc/Generic/Host.py` & `TDhelper-2.7.7/TDhelper/network/rpc/Generic/Host.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/network/rpc/Server/obsolete_Service.py` & `TDhelper-2.7.7/TDhelper/network/rpc/Server/obsolete_Service.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/network/rpc/Server/server.py` & `TDhelper-2.7.7/TDhelper/network/rpc/Server/server.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/network/rpc/Struct/Result.py` & `TDhelper-2.7.7/TDhelper/network/rpc/Struct/Result.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/network/socket/__init__.py` & `TDhelper-2.7.7/TDhelper/network/socket/__init__.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/network/socket/cache/queue.py` & `TDhelper-2.7.7/TDhelper/network/socket/cache/queue.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/network/socket/client.py` & `TDhelper-2.7.7/TDhelper/network/socket/client.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/network/socket/model/SOCKET_MODELS.py` & `TDhelper-2.7.7/TDhelper/network/socket/model/SOCKET_MODELS.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/network/socket/protocol/base.py` & `TDhelper-2.7.7/TDhelper/network/socket/protocol/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/network/socket/server.py` & `TDhelper-2.7.7/TDhelper/network/socket/server.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/network/websocket/protocol.py` & `TDhelper-2.7.7/TDhelper/network/websocket/protocol.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/network/websocket/server.py` & `TDhelper-2.7.7/TDhelper/network/websocket/server.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/reflect.py` & `TDhelper-2.7.7/TDhelper/reflect.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/robot/control/D_33890.py` & `TDhelper-2.7.7/TDhelper/robot/control/D_33890.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/robot/control/device.py` & `TDhelper-2.7.7/TDhelper/robot/control/device.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/robot/people/__init__.py` & `TDhelper-2.7.7/TDhelper/robot/people/__init__.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/robot/people/leg.py` & `TDhelper-2.7.7/TDhelper/robot/people/leg.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/robot/people/scripts/runScript.py` & `TDhelper-2.7.7/TDhelper/robot/people/scripts/runScript.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/robot/people/scripts/script.py` & `TDhelper-2.7.7/TDhelper/robot/people/scripts/script.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/robot/struct/ankle.py` & `TDhelper-2.7.7/TDhelper/robot/struct/ankle.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/robot/struct/base.py` & `TDhelper-2.7.7/TDhelper/robot/struct/base.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/robot/struct/hip.py` & `TDhelper-2.7.7/TDhelper/robot/struct/hip.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/robot/struct/knee.py` & `TDhelper-2.7.7/TDhelper/robot/struct/knee.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/robot/struct/toe.py` & `TDhelper-2.7.7/TDhelper/robot/struct/toe.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/shellScripts/saasHelper.py` & `TDhelper-2.7.7/TDhelper/shellScripts/saasHelper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/simulate/json.py` & `TDhelper-2.7.7/TDhelper/simulate/json.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/structs/dir.py` & `TDhelper-2.7.7/TDhelper/structs/dir.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/web/obsolete_permission.py` & `TDhelper-2.7.7/TDhelper/web/obsolete_permission.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/web/obsolete_permissionHelper.py` & `TDhelper-2.7.7/TDhelper/web/obsolete_permissionHelper.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/web/utils/permission/client.py` & `TDhelper-2.7.7/TDhelper/web/utils/permission/client.py`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/TDhelper/web/utils/permission/server.py` & `TDhelper-2.7.7/TDhelper/web/utils/permission/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,15 +32,18 @@
         if os.path.exists(self.__conf_path__):
             conf = ''
             with open(self.__conf_path__, "r", -1, encoding=self.__encoding__) as f:
                 conf = f.read()
                 f.close()
             if conf:
                 conf = json.loads(conf)
-                recursionCall(self._register_permission, 200, conf, **{})
+                if conf:
+                    recursionCall(self._register_permission, 200, conf, **{})
+                else:
+                    logging.info("permission file: '/config/regist_conf/permission.json' not configure.")
         else:
             raise Exception("Not Found '%s'" % self.__conf_path__)
 
     def _register_permission(self, config, **kwargs):
         if self.__platform_key__:
             config["permission_key"] = '.'.join(
                 [self.__platform_key__, config["permission_key"]])
```

### Comparing `TDhelper-2.7.6/TDhelper.egg-info/PKG-INFO` & `TDhelper-2.7.7/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,32 @@
 Metadata-Version: 2.1
 Name: TDhelper
-Version: 2.7.6
+Version: 2.7.7
 Summary: reconsitution web.permissionHelper cls.
 Home-page: https://gitee.com/TonyDon/pyLib
 Author: TangJing
 Author-email: yeihizhi@163.com
 License: Apache 2.0
 Keywords: pip,TDhelper,featureextraction
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TDhelper LIb
 helper class lib.
+# ***Saas-Framework Cli***
+## 1. Create saas project command line   
+
+### custom directory   
+```
+saas --name "project name" --path /usr/www/
+```
+### current directory
+```
+saas --name "project name" --path pathname
+```
 
 # ***Cache***
 
 ## 1. pools
 ## 2. ring cache
 
 # ***db***
```

#### html2text {}

```diff
@@ -1,21 +1,23 @@
-Metadata-Version: 2.1 Name: TDhelper Version: 2.7.6 Summary: reconsitution
+Metadata-Version: 2.1 Name: TDhelper Version: 2.7.7 Summary: reconsitution
 web.permissionHelper cls. Home-page: https://gitee.com/TonyDon/pyLib Author:
 TangJing Author-email: yeihizhi@163.com License: Apache 2.0 Keywords:
 pip,TDhelper,featureextraction Description-Content-Type: text/markdown License-
-File: LICENSE # TDhelper LIb helper class lib. # ***Cache*** ## 1. pools ## 2.
-ring cache # ***db*** ## 1. sqllite ## 2. mongodb ## 3. mysql #
-***Decorators*** ## 1. log # ***document*** ## 1. file ## 2. excel #
-***Event*** ## 1. Event ## 2. classEvent ## 3. webEvent # ***generic*** #
-***MagicCls*** running time dynamic create class. mapping any object to an
-object. # ***Msg*** genneric msg helper class. # ***network*** http, socket
-helper. # ***robot*** robot class. # ***Scheduler*** not finished #
-***simulate*** not finished # ***Spider*** # ***structs*** not finished #
-***web*** ## permission module ### ***1. register*** permission register class.
-#### ***Methods***
+File: LICENSE # TDhelper LIb helper class lib. # ***Saas-Framework Cli*** ## 1.
+Create saas project command line ### custom directory ``` saas --name "project
+name" --path /usr/www/ ``` ### current directory ``` saas --name "project name"
+--path pathname ``` # ***Cache*** ## 1. pools ## 2. ring cache # ***db*** ## 1.
+sqllite ## 2. mongodb ## 3. mysql # ***Decorators*** ## 1. log # ***document***
+## 1. file ## 2. excel # ***Event*** ## 1. Event ## 2. classEvent ## 3.
+webEvent # ***generic*** # ***MagicCls*** running time dynamic create class.
+mapping any object to an object. # ***Msg*** genneric msg helper class. #
+***network*** http, socket helper. # ***robot*** robot class. # ***Scheduler***
+not finished # ***simulate*** not finished # ***Spider*** # ***structs*** not
+finished # ***web*** ## permission module ### ***1. register*** permission
+register class. #### ***Methods***
 NO.
 |
 name
 |
 description
 :---:|:---|:--- 1 | [Register](#perRegister) | - 2 | [RegisterByCfg]
 (#perRegisterByCfg) | - _*_*_*_R_e_g_i_s_t_e_r_*_*_*
```

### Comparing `TDhelper-2.7.6/TDhelper.egg-info/SOURCES.txt` & `TDhelper-2.7.7/TDhelper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TDhelper-2.7.6/setup.py` & `TDhelper-2.7.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import setuptools
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 setuptools.setup(
     name="TDhelper",
-    version="2.7.6",
+    version="2.7.7",
     keywords=("pip", "TDhelper", "featureextraction"),
     description="reconsitution web.permissionHelper cls.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="Apache 2.0",
     url="https://gitee.com/TonyDon/pyLib",
     author="TangJing",
```

