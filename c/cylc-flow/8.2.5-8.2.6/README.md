# Comparing `tmp/cylc-flow-8.2.5.tar.gz` & `tmp/cylc_flow-8.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cylc-flow-8.2.5.tar", last modified: Thu Apr  4 14:40:36 2024, max compression
+gzip compressed data, was "cylc_flow-8.2.6.tar", last modified: Thu May  2 11:24:53 2024, max compression
```

## Comparing `cylc-flow-8.2.5.tar` & `cylc_flow-8.2.6.tar`

### file list

```diff
@@ -1,320 +1,321 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.799552 cylc-flow-8.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-04-04 14:40:36.799552 cylc-flow-8.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.735550 cylc-flow-8.2.5/cylc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.755551 cylc-flow-8.2.5/cylc/flow/
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15539 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/async_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    17061 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/broadcast_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/broadcast_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/c3mro.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.755551 cylc-flow-8.2.5/cylc/flow/cfgspec/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/cfgspec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/cfgspec/glbl_cfg.py
--rw-r--r--   0 runner    (1001) docker     (127)    73203 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/cfgspec/globalcfg.py
--rw-r--r--   0 runner    (1001) docker     (127)    85291 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/cfgspec/workflow.py
--rw-r--r--   0 runner    (1001) docker     (127)    16960 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/command_polling.py
--rw-r--r--   0 runner    (1001) docker     (127)    99069 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7238 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/context_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.759551 cylc-flow-8.2.5/cylc/flow/cycling/
--rw-r--r--   0 runner    (1001) docker     (127)    14729 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/cycling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23211 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/cycling/integer.py
--rw-r--r--   0 runner    (1001) docker     (127)    36439 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/cycling/iso8601.py
--rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/cycling/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/cycling/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/cylc_subproc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/daemonize.py
--rw-r--r--   0 runner    (1001) docker     (127)    22099 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/data_messages_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)   103056 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/data_store_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/dbstatecheck.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.759551 cylc-flow-8.2.5/cylc/flow/etc/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     7934 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/cylc
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/cylc-completion.bash
--rw-r--r--   0 runner    (1001) docker     (127)    14537 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/job.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.759551 cylc-flow-8.2.5/cylc/flow/etc/syntax/
--rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/syntax/cylc-mode.el
--rw-r--r--   0 runner    (1001) docker     (127)    25186 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/syntax/cylc.lang
--rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/syntax/cylc.vim
--rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/syntax/cylc.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.759551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/api-keys
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.759551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/
--rwxr-xr-x   0 runner    (1001) docker     (127)      802 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/.validate
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.759551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4265 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/bin/consolidate-observations
--rwxr-xr-x   0 runner    (1001) docker     (127)     9168 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/bin/forecast
--rwxr-xr-x   0 runner    (1001) docker     (127)     7246 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-observations
--rwxr-xr-x   0 runner    (1001) docker     (127)     6512 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-rainfall
--rwxr-xr-x   0 runner    (1001) docker     (127)     3738 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/bin/post-process
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.763551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/etc/
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/etc/met-office-sites.dat
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/etc/python-job.settings
--rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.735550 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.763551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/mercator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.763551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/map.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.763551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1139 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/.validate
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.763551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4265 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/consolidate-observations
--rwxr-xr-x   0 runner    (1001) docker     (127)     9168 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/forecast
--rwxr-xr-x   0 runner    (1001) docker     (127)     7246 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-observations
--rwxr-xr-x   0 runner    (1001) docker     (127)     6512 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-rainfall
--rwxr-xr-x   0 runner    (1001) docker     (127)     3738 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/post-process
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.763551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/met-office-sites.dat
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/python-job.settings
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.735550 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.763551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/mercator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.763551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/map.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.763551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/forecast-script/
--rwxr-xr-x   0 runner    (1001) docker     (127)     9168 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/forecast-script/forecast
--rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/forecast-script/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.763551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/inheritance-tutorial/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/inheritance-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.763551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/map-template/
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/map-template/map-template.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.735550 cylc-flow-8.2.5/cylc/flow/etc/tutorial/message-trigger-tutorial/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.763551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/message-trigger-tutorial/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      180 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/message-trigger-tutorial/bin/random.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.763551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/retries-tutorial/
--rwxr-xr-x   0 runner    (1001) docker     (127)      819 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/retries-tutorial/.validate
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/retries-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.767551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-introduction/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1125 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-introduction/.validate
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.767551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-introduction/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      459 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-introduction/bin/get-observations
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.767551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-introduction/etc/
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-introduction/etc/python-job.settings
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-introduction/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.767551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.767551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)     4265 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/bin/consolidate-observations
--rwxr-xr-x   0 runner    (1001) docker     (127)     9168 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/bin/forecast
--rwxr-xr-x   0 runner    (1001) docker     (127)     7246 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-observations
--rwxr-xr-x   0 runner    (1001) docker     (127)     6512 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-rainfall
--rwxr-xr-x   0 runner    (1001) docker     (127)     3738 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/bin/post-process
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.767551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/etc/
--rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/etc/met-office-sites.dat
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/etc/python-job.settings
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/flow.cylc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.739550 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/lib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.767551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/mercator.py
--rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.767551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/map.html
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/runtime
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.767551 cylc-flow-8.2.5/cylc/flow/etc/tutorial/test-data/
--rw-r--r--   0 runner    (1001) docker     (127)    33085 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/test-data/rainfall.csv
--rw-r--r--   0 runner    (1001) docker     (127)    35829 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_x.csv
--rw-r--r--   0 runner    (1001) docker     (127)    38004 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_y.csv
--rw-r--r--   0 runner    (1001) docker     (127)    14108 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/flags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/flow_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)    36301 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/graph_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/graphnode.py
--rw-r--r--   0 runner    (1001) docker     (127)    18192 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/host_select.py
--rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/hostuserutil.py
--rw-r--r--   0 runner    (1001) docker     (127)    24799 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/id.py
--rw-r--r--   0 runner    (1001) docker     (127)    17959 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/id_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/id_match.py
--rw-r--r--   0 runner    (1001) docker     (127)    21546 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/install.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.767551 cylc-flow-8.2.5/cylc/flow/install_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/install_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11208 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/install_plugins/log_vc_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.739550 cylc-flow-8.2.5/cylc/flow/jinja/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.771551 cylc-flow-8.2.5/cylc/flow/jinja/filters/
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/jinja/filters/duration_as.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/jinja/filters/pad.py
--rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/jinja/filters/strftime.py
--rw-r--r--   0 runner    (1001) docker     (127)    15445 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/job_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.771551 cylc-flow-8.2.5/cylc/flow/job_runner_handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/job_runner_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/job_runner_handlers/at.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/job_runner_handlers/background.py
--rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/job_runner_handlers/documentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/job_runner_handlers/loadleveler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/job_runner_handlers/lsf.py
--rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/job_runner_handlers/moab.py
--rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/job_runner_handlers/pbs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/job_runner_handlers/pbs_multi_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/job_runner_handlers/sge.py
--rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/job_runner_handlers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/job_runner_handlers/slurm_packjob.py
--rw-r--r--   0 runner    (1001) docker     (127)    33926 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/job_runner_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/listify.py
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/log_diagnosis.py
--rw-r--r--   0 runner    (1001) docker     (127)    15366 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/loggingutil.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.771551 cylc-flow-8.2.5/cylc/flow/main_loop/
--rw-r--r--   0 runner    (1001) docker     (127)    10547 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/main_loop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9564 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/main_loop/auto_restart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/main_loop/health_check.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/main_loop/log_data_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/main_loop/log_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/main_loop/log_main_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/main_loop/log_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/main_loop/reset_bad_hosts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.775551 cylc-flow-8.2.5/cylc/flow/network/
--rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/authorisation.py
--rw-r--r--   0 runner    (1001) docker     (127)    11999 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/client_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    16257 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/multi.py
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/publisher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/replier.py
--rw-r--r--   0 runner    (1001) docker     (127)    31093 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (127)    16241 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/scan.py
--rw-r--r--   0 runner    (1001) docker     (127)    80335 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    14723 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/ssh_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/network/subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)    30974 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/option_parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/param_expand.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.779551 cylc-flow-8.2.5/cylc/flow/parsec/
--rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/parsec/OrderedDict.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/parsec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10823 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/parsec/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/parsec/empysupport.py
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/parsec/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    22080 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/parsec/fileparse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/parsec/include.py
--rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/parsec/jinja2support.py
--rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/parsec/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (127)    14533 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/parsec/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    43559 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/parsec/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)    17608 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/pathutil.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/pipe_poller.py
--rw-r--r--   0 runner    (1001) docker     (127)    24924 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/platforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    10759 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/prerequisite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/print_tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    13932 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    39982 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/rundb.py
--rw-r--r--   0 runner    (1001) docker     (127)    86592 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    20823 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scheduler_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.787551 cylc-flow-8.2.5/cylc/flow/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15378 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/broadcast.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    21078 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/cat_log.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4986 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/check_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/clean.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2617 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    20905 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/completion_server.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6429 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/config.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8932 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/cycle_point.py
--rw-r--r--   0 runner    (1001) docker     (127)    21259 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/cylc.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5986 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/diff.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8083 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/dump.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4460 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/ext_trigger.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1491 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/function_run.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2513 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/get_resources.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1871 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/get_workflow_contact.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2311 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/get_workflow_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    14974 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/graph.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4638 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/hold.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10942 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/install.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1722 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/jobs_kill.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1697 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/jobs_poll.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2846 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/jobs_submit.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2503 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/kill.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    40990 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/lint.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6228 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/list.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6417 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/pause.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3955 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/play.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2564 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/poll.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/psutil.py
--rw-r--r--   0 runner    (1001) docker     (127)    12602 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/reinstall.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3739 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/release.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3266 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/reload.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2106 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/remote_init.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1533 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/remote_tidy.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2225 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/remove.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13206 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/report_timings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16118 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/scan.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3516 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/set_outputs.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2536 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/set_verbosity.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13108 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/show.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8380 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/stop.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3658 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/subscribe.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5272 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/tui.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     6488 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/validate_install_play.py
--rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/validate_reinstall.py
--rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/view.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10163 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/scripts/workflow_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     6233 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/subprocctx.py
--rw-r--r--   0 runner    (1001) docker     (127)    23937 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/subprocpool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_action_timer.py
--rw-r--r--   0 runner    (1001) docker     (127)    65738 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_events_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_id.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_job_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    55839 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_job_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    80634 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)    18265 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_qualifiers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.787551 cylc-flow-8.2.5/cylc/flow/task_queues/
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_queues/independent.py
--rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_remote_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)    25368 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_remote_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)    18225 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_state_prop.py
--rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/task_trigger.py
--rw-r--r--   0 runner    (1001) docker     (127)    14419 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/taskdef.py
--rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/templatevars.py
--rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/terminal.py
--rw-r--r--   0 runner    (1001) docker     (127)    19578 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/time_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.787551 cylc-flow-8.2.5/cylc/flow/tui/
--rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18799 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/tui/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/tui/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/tui/overlay.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/tui/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/tui/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/unicode_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    10729 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/wallclock.py
--rw-r--r--   0 runner    (1001) docker     (127)    32499 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/workflow_db_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/workflow_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    34487 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/workflow_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/workflow_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    18380 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/xtrigger_mgr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.791552 cylc-flow-8.2.5/cylc/flow/xtriggers/
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/xtriggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/xtriggers/echo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/xtriggers/wall_clock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/xtriggers/workflow_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/cylc/flow/xtriggers/xrandom.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 14:40:36.791552 cylc-flow-8.2.5/cylc_flow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11333 2024-04-04 14:40:36.000000 cylc-flow-8.2.5/cylc_flow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9410 2024-04-04 14:40:36.000000 cylc-flow-8.2.5/cylc_flow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 14:40:36.000000 cylc-flow-8.2.5/cylc_flow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-04-04 14:40:36.000000 cylc-flow-8.2.5/cylc_flow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-04 14:40:36.000000 cylc-flow-8.2.5/cylc_flow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-04 14:40:36.000000 cylc-flow-8.2.5/cylc_flow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     5877 2024-04-04 14:40:36.799552 cylc-flow-8.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-04 14:40:29.000000 cylc-flow-8.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.788079 cylc_flow-8.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-05-02 11:24:53.788079 cylc_flow-8.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5337 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.728078 cylc_flow-8.2.6/cylc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.748078 cylc_flow-8.2.6/cylc/flow/
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15539 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/async_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17061 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/broadcast_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/broadcast_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4800 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/c3mro.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.748078 cylc_flow-8.2.6/cylc/flow/cfgspec/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/cfgspec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/cfgspec/glbl_cfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73285 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/cfgspec/globalcfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85291 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/cfgspec/workflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16960 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/command_polling.py
+-rw-r--r--   0 runner    (1001) docker     (127)    98634 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7850 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/context_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.748078 cylc_flow-8.2.6/cylc/flow/cycling/
+-rw-r--r--   0 runner    (1001) docker     (127)    14729 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/cycling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23211 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/cycling/integer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36439 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/cycling/iso8601.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5488 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/cycling/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/cycling/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2238 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/cylc_subproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/daemonize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22099 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/data_messages_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)   103056 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/data_store_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5947 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/dbstatecheck.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.748078 cylc_flow-8.2.6/cylc/flow/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7934 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/cylc
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/cylc-completion.bash
+-rw-r--r--   0 runner    (1001) docker     (127)    14537 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/job.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.752078 cylc_flow-8.2.6/cylc/flow/etc/syntax/
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/syntax/cylc-mode.el
+-rw-r--r--   0 runner    (1001) docker     (127)    25186 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/syntax/cylc.lang
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/syntax/cylc.nanorc
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/syntax/cylc.vim
+-rw-r--r--   0 runner    (1001) docker     (127)    10612 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/syntax/cylc.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.752078 cylc_flow-8.2.6/cylc/flow/etc/tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/api-keys
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.752078 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      802 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/.validate
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.752078 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4265 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/bin/consolidate-observations
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9168 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/bin/forecast
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7246 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-observations
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6512 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-rainfall
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3738 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/bin/post-process
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.752078 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/etc/met-office-sites.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/etc/python-job.settings
+-rw-r--r--   0 runner    (1001) docker     (127)     4255 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.728078 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.752078 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/mercator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.752078 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/map.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.752078 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1139 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/.validate
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4265 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/consolidate-observations
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9168 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/forecast
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7246 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-observations
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6512 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-rainfall
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3738 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/post-process
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/met-office-sites.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/python-job.settings
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.728078 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/mercator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/map.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/forecast-script/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9168 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/forecast-script/forecast
+-rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/forecast-script/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/inheritance-tutorial/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/inheritance-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/map-template/
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/map-template/map-template.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.728078 cylc_flow-8.2.6/cylc/flow/etc/tutorial/message-trigger-tutorial/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/message-trigger-tutorial/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      180 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/message-trigger-tutorial/bin/random.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/retries-tutorial/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      819 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/retries-tutorial/.validate
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/retries-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-introduction/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1125 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-introduction/.validate
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-introduction/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      459 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-introduction/bin/get-observations
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-introduction/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-introduction/etc/python-job.settings
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-introduction/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4265 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/bin/consolidate-observations
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9168 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/bin/forecast
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7246 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-observations
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6512 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-rainfall
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3738 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/bin/post-process
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.756079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/etc/
+-rw-r--r--   0 runner    (1001) docker     (127)     7485 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/etc/met-office-sites.dat
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/etc/python-job.settings
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/flow.cylc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.732078 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/lib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.760079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/mercator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10232 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.760079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/map.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/runtime
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.760079 cylc_flow-8.2.6/cylc/flow/etc/tutorial/test-data/
+-rw-r--r--   0 runner    (1001) docker     (127)    33085 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/test-data/rainfall.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    35829 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_x.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    38004 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_y.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    14108 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/flags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/flow_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36301 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/graph_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/graphnode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18192 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/host_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10624 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/hostuserutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24799 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17959 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/id_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/id_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21546 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/install.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.760079 cylc_flow-8.2.6/cylc/flow/install_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/install_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11208 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/install_plugins/log_vc_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.732078 cylc_flow-8.2.6/cylc/flow/jinja/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.760079 cylc_flow-8.2.6/cylc/flow/jinja/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/jinja/filters/duration_as.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/jinja/filters/pad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/jinja/filters/strftime.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15445 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/job_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.760079 cylc_flow-8.2.6/cylc/flow/job_runner_handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/job_runner_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/job_runner_handlers/at.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/job_runner_handlers/background.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13028 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/job_runner_handlers/documentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5037 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/job_runner_handlers/loadleveler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/job_runner_handlers/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3653 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/job_runner_handlers/moab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4522 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/job_runner_handlers/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/job_runner_handlers/pbs_multi_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/job_runner_handlers/sge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6648 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/job_runner_handlers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/job_runner_handlers/slurm_packjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33926 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/job_runner_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/listify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/log_diagnosis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15366 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/loggingutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.764078 cylc_flow-8.2.6/cylc/flow/main_loop/
+-rw-r--r--   0 runner    (1001) docker     (127)    10547 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/main_loop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9564 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/main_loop/auto_restart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/main_loop/health_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/main_loop/log_data_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/main_loop/log_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3013 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/main_loop/log_main_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4691 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/main_loop/log_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/main_loop/reset_bad_hosts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.764078 cylc_flow-8.2.6/cylc/flow/network/
+-rw-r--r--   0 runner    (1001) docker     (127)     9916 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/authorisation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11999 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16257 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3011 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/multi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4627 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/replier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31093 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16241 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/scan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80335 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14723 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/ssh_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/network/subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30974 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/option_parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17877 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/param_expand.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.768079 cylc_flow-8.2.6/cylc/flow/parsec/
+-rw-r--r--   0 runner    (1001) docker     (127)     6642 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/parsec/OrderedDict.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/parsec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10946 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/parsec/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/parsec/empysupport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/parsec/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22080 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/parsec/fileparse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2946 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/parsec/include.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11240 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/parsec/jinja2support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/parsec/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14308 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/parsec/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43559 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/parsec/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17608 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/pathutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/pipe_poller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24924 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/platforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10759 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/prerequisite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/print_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    13932 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6932 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39982 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/rundb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86354 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20636 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scheduler_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.776079 cylc_flow-8.2.6/cylc/flow/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15378 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/broadcast.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    21078 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/cat_log.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4986 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/check_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6879 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/clean.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2617 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1973 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20905 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/completion_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6429 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8932 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/cycle_point.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21259 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/cylc.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5986 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/diff.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8083 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4460 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/ext_trigger.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1491 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/function_run.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2513 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/get_resources.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1871 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/get_workflow_contact.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2311 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/get_workflow_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14974 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4638 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/hold.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10942 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/install.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1722 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/jobs_kill.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1697 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/jobs_poll.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2846 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/jobs_submit.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2503 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/kill.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    40024 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/lint.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6228 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/list.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6417 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/pause.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3955 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/play.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2564 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/poll.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/psutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12602 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/reinstall.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3739 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/release.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3266 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/reload.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2106 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/remote_init.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1533 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/remote_tidy.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2225 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/remove.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13206 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/report_timings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16118 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/scan.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3516 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/set_outputs.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2536 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/set_verbosity.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13108 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/show.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8380 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/stop.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3658 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/subscribe.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5272 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/tui.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6488 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/validate_install_play.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6270 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/validate_reinstall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4320 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/view.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10163 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/scripts/workflow_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/subprocctx.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23937 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/subprocpool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_action_timer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65738 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_events_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_job_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55839 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_job_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6883 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8683 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80634 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18265 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_qualifiers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.776079 cylc_flow-8.2.6/cylc/flow/task_queues/
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_queues/independent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6752 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_remote_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25368 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_remote_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18225 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3035 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_state_prop.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/task_trigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14419 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/taskdef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/templatevars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11265 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/terminal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19578 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/time_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3487 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.776079 cylc_flow-8.2.6/cylc/flow/tui/
+-rw-r--r--   0 runner    (1001) docker     (127)     4434 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18799 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/tui/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6389 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/tui/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6981 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/tui/overlay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/tui/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13257 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/tui/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/unicode_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3530 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10729 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/wallclock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32499 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/workflow_db_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/workflow_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34487 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/workflow_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7249 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/workflow_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18387 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/xtrigger_mgr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.776079 cylc_flow-8.2.6/cylc/flow/xtriggers/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/xtriggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/xtriggers/echo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/xtriggers/wall_clock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3955 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/xtriggers/workflow_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3314 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/cylc/flow/xtriggers/xrandom.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 11:24:53.780079 cylc_flow-8.2.6/cylc_flow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11337 2024-05-02 11:24:53.000000 cylc_flow-8.2.6/cylc_flow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9443 2024-05-02 11:24:53.000000 cylc_flow-8.2.6/cylc_flow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 11:24:53.000000 cylc_flow-8.2.6/cylc_flow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-02 11:24:53.000000 cylc_flow-8.2.6/cylc_flow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-02 11:24:53.000000 cylc_flow-8.2.6/cylc_flow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 11:24:53.000000 cylc_flow-8.2.6/cylc_flow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     5879 2024-05-02 11:24:53.788079 cylc_flow-8.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-02 11:24:45.000000 cylc_flow-8.2.6/setup.py
```

### Comparing `cylc-flow-8.2.5/COPYING` & `cylc_flow-8.2.6/COPYING`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/PKG-INFO` & `cylc_flow-8.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cylc-flow
-Version: 8.2.5
+Version: 8.2.6
 Summary: A workflow engine for cycling systems
 Home-page: https://cylc.org/
 Author: Hilary Oliver
 License: GPL
 Project-URL: Documentation, https://cylc.github.io/cylc-doc/stable/html/index.html
 Project-URL: Source, https://github.com/cylc/cylc-flow
 Project-URL: Tracker, https://github.com/cylc/cylc-flow/issues
@@ -70,15 +70,15 @@
 Requires-Dist: flake8-builtins>=1.5.0; extra == "tests"
 Requires-Dist: flake8-comprehensions>=3.5.0; extra == "tests"
 Requires-Dist: flake8-debugger>=4.0.0; extra == "tests"
 Requires-Dist: flake8-mutable>=1.2.0; extra == "tests"
 Requires-Dist: flake8-simplify>=0.14.0; extra == "tests"
 Requires-Dist: flake8>=3.0.0; extra == "tests"
 Requires-Dist: mypy<1.9,>=0.910; extra == "tests"
-Requires-Dist: pytest-asyncio!=0.23.*,>=0.17; extra == "tests"
+Requires-Dist: pytest-asyncio!=0.23.*,>=0.21.2; extra == "tests"
 Requires-Dist: pytest-cov>=2.8.0; extra == "tests"
 Requires-Dist: pytest-xdist>=2; extra == "tests"
 Requires-Dist: pytest-env>=0.6.2; extra == "tests"
 Requires-Dist: pytest-mock>=3.7; extra == "tests"
 Requires-Dist: pytest>=6; extra == "tests"
 Requires-Dist: testfixtures>=6.11.0; extra == "tests"
 Requires-Dist: towncrier>=23; extra == "tests"
@@ -109,15 +109,15 @@
 Requires-Dist: flake8-builtins>=1.5.0; extra == "all"
 Requires-Dist: flake8-comprehensions>=3.5.0; extra == "all"
 Requires-Dist: flake8-debugger>=4.0.0; extra == "all"
 Requires-Dist: flake8-mutable>=1.2.0; extra == "all"
 Requires-Dist: flake8-simplify>=0.14.0; extra == "all"
 Requires-Dist: flake8>=3.0.0; extra == "all"
 Requires-Dist: mypy<1.9,>=0.910; extra == "all"
-Requires-Dist: pytest-asyncio!=0.23.*,>=0.17; extra == "all"
+Requires-Dist: pytest-asyncio!=0.23.*,>=0.21.2; extra == "all"
 Requires-Dist: pytest-cov>=2.8.0; extra == "all"
 Requires-Dist: pytest-xdist>=2; extra == "all"
 Requires-Dist: pytest-env>=0.6.2; extra == "all"
 Requires-Dist: pytest-mock>=3.7; extra == "all"
 Requires-Dist: pytest>=6; extra == "all"
 Requires-Dist: testfixtures>=6.11.0; extra == "all"
 Requires-Dist: towncrier>=23; extra == "all"
```

### Comparing `cylc-flow-8.2.5/README.md` & `cylc_flow-8.2.6/README.md`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/__init__.py` & `cylc_flow-8.2.6/cylc/flow/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     # running pre-5.0 cylc via the posix nohup command; is it still the
     # case in post-5.0 daemon-mode cylc?)
     os.environ['PYTHONUNBUFFERED'] = 'true'
 
 
 environ_init()
 
-__version__ = '8.2.5'
+__version__ = '8.2.6'
 
 
 def iter_entry_points(entry_point_name):
     """Iterate over Cylc entry points."""
     import pkg_resources
     yield from (
         entry_point
```

### Comparing `cylc-flow-8.2.5/cylc/flow/async_util.py` & `cylc_flow-8.2.6/cylc/flow/async_util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/broadcast_mgr.py` & `cylc_flow-8.2.6/cylc/flow/broadcast_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/broadcast_report.py` & `cylc_flow-8.2.6/cylc/flow/broadcast_report.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/c3mro.py` & `cylc_flow-8.2.6/cylc/flow/c3mro.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/cfgspec/__init__.py` & `cylc_flow-8.2.6/cylc/flow/cfgspec/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/cfgspec/glbl_cfg.py` & `cylc_flow-8.2.6/cylc/flow/cfgspec/glbl_cfg.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/cfgspec/globalcfg.py` & `cylc_flow-8.2.6/cylc/flow/cfgspec/globalcfg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1990,30 +1990,33 @@
         self,
         print_platform_names: bool = True,
         print_platforms: bool = True
     ) -> None:
         """Print informations about platforms currently defined.
         """
         if print_platform_names:
-            with suppress(ItemNotFoundError):
-                self.dump_platform_names(self)
+            self.dump_platform_names(self)
         if print_platforms:
-            with suppress(ItemNotFoundError):
-                self.dump_platform_details(self)
+            self.dump_platform_details(self)
 
     @staticmethod
     def dump_platform_names(cfg) -> None:
         """Print a list of defined platforms and groups.
         """
+        # [platforms] is always defined with at least localhost
         platforms = '\n'.join(cfg.get(['platforms']).keys())
-        platform_groups = '\n'.join(cfg.get(['platform groups']).keys())
         print(f'{PLATFORM_REGEX_TEXT}\n\nPlatforms\n---------', file=stderr)
         print(platforms)
-        print('\n\nPlatform Groups\n--------------', file=stderr)
+        try:
+            platform_groups = '\n'.join(cfg.get(['platform groups']).keys())
+        except ItemNotFoundError:
+            return
+        print('\nPlatform Groups\n--------------', file=stderr)
         print(platform_groups)
 
     @staticmethod
     def dump_platform_details(cfg) -> None:
         """Print platform and platform group configs.
         """
         for config in ['platforms', 'platform groups']:
-            printcfg({config: cfg.get([config], sparse=True)})
+            with suppress(ItemNotFoundError):
+                printcfg({config: cfg.get([config], sparse=True)})
```

### Comparing `cylc-flow-8.2.5/cylc/flow/cfgspec/workflow.py` & `cylc_flow-8.2.6/cylc/flow/cfgspec/workflow.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/clean.py` & `cylc_flow-8.2.6/cylc/flow/clean.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/command_polling.py` & `cylc_flow-8.2.6/cylc/flow/command_polling.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/config.py` & `cylc_flow-8.2.6/cylc/flow/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,15 @@
 from cylc.flow.graph_parser import GraphParser
 from cylc.flow.listify import listify
 from cylc.flow.option_parsers import verbosity_to_env
 from cylc.flow.graphnode import GraphNodeParser
 from cylc.flow.param_expand import NameExpander
 from cylc.flow.parsec.exceptions import ItemNotFoundError
 from cylc.flow.parsec.OrderedDict import OrderedDictWithDefaults
-from cylc.flow.parsec.util import replicate
+from cylc.flow.parsec.util import dequote, replicate
 from cylc.flow.pathutil import (
     get_workflow_name_from_id,
     get_cylc_run_dir,
     is_relative_to,
 )
 from cylc.flow.platforms import FORBIDDEN_WITH_PLATFORM
 from cylc.flow.print_tree import print_tree
@@ -194,37 +194,14 @@
         raise ParamExpandError('bad parameter')
     except TypeError:
         raise ParamExpandError('wrong data type for parameter')
     except ValueError:
         raise ParamExpandError('bad template syntax')
 
 
-def dequote(string):
-    """Strip quotes off a string.
-
-    Examples:
-        >>> dequote('"foo"')
-        'foo'
-        >>> dequote("'foo'")
-        'foo'
-        >>> dequote('foo')
-        'foo'
-        >>> dequote('"f')
-        '"f'
-        >>> dequote('f')
-        'f'
-
-    """
-    if len(string) < 2:
-        return string
-    if (string[0] == string[-1]) and string.startswith(("'", '"')):
-        return string[1:-1]
-    return string
-
-
 class WorkflowConfig:
     """Class for workflow configuration items and derived quantities."""
 
     CHECK_CIRCULAR_LIMIT = 100  # If no. tasks > this, don't check circular
     VIS_N_POINTS = 3
     MAX_WARNING_LINES = 5
```

### Comparing `cylc-flow-8.2.5/cylc/flow/context_node.py` & `cylc_flow-8.2.6/cylc/flow/context_node.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,21 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 
-from typing import Optional
+from typing import TYPE_CHECKING, Optional
+
+if TYPE_CHECKING:
+    # BACK COMPAT: typing_extensions.Self
+    # FROM: Python 3.7
+    # TO: Python 3.11
+    from typing_extensions import Self
 
 
 class ContextNode():
     """A class for defining nested objects.
 
     Attributes:
         name (str):
@@ -89,15 +95,15 @@
 
     def __init__(self, name: str):
         self.name = name
         self._parent = None
         self._children = None
         self.DATA[self] = set(self.DATA)
 
-    def __enter__(self):
+    def __enter__(self) -> 'Self':
         return self
 
     def __exit__(self, *args):
         # list the nodes already present on this node
         older_siblings = self._children or {}
         # list the nodes which were created since we
         # __entered__ this node
@@ -125,32 +131,44 @@
         if self._children:
             return iter(self._children.values())
         return iter([])
 
     def __contains__(self, name: str) -> bool:
         return name in self._children  # type: ignore[operator]  # TODO
 
-    def __getitem__(self, name: str):
+    def __getitem__(self, name: str) -> 'Self':
         if self._children:
             return self._children.__getitem__(name)
         raise TypeError('This is not a leaf node')
 
-    def get(self, *names: str):
+    def get(self, *names: str) -> 'Self':
         """Retrieve the node given by the list of names.
 
         Example:
             >>> with ContextNode('a') as a:
-            ...     with ContextNode('b') as b:
+            ...     with ContextNode('b'):
             ...          c = ContextNode('c')
             >>> a.get('b', 'c')
             a/b/c
+
+            >>> with ContextNode('a') as a:
+            ...     with ContextNode('b'):
+            ...         with ContextNode('__MANY__'):
+            ...             c = ContextNode('c')
+            >>> a.get('b', 'foo', 'c')
+            a/b/__MANY__/c
         """
         node = self
         for name in names:
-            node = node[name]
+            try:
+                node = node[name]
+            except KeyError as exc:
+                if '__MANY__' not in node:
+                    raise exc
+                node = node['__MANY__']
         return node
 
     def __str__(self) -> str:
         if self.is_root():
             fmt = self.ROOT_NAME_FMT
         elif not self.is_leaf():
             fmt = self.NODE_NAME_FMT
```

### Comparing `cylc-flow-8.2.5/cylc/flow/cycling/__init__.py` & `cylc_flow-8.2.6/cylc/flow/cycling/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/cycling/integer.py` & `cylc_flow-8.2.6/cylc/flow/cycling/integer.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/cycling/iso8601.py` & `cylc_flow-8.2.6/cylc/flow/cycling/iso8601.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/cycling/loader.py` & `cylc_flow-8.2.6/cylc/flow/cycling/loader.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/cycling/util.py` & `cylc_flow-8.2.6/cylc/flow/cycling/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/cylc_subproc.py` & `cylc_flow-8.2.6/cylc/flow/cylc_subproc.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/daemonize.py` & `cylc_flow-8.2.6/cylc/flow/daemonize.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/data_messages_pb2.py` & `cylc_flow-8.2.6/cylc/flow/data_messages_pb2.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/data_store_mgr.py` & `cylc_flow-8.2.6/cylc/flow/data_store_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/dbstatecheck.py` & `cylc_flow-8.2.6/cylc/flow/dbstatecheck.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/cylc` & `cylc_flow-8.2.6/cylc/flow/etc/cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/cylc-completion.bash` & `cylc_flow-8.2.6/cylc/flow/etc/cylc-completion.bash`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/job.sh` & `cylc_flow-8.2.6/cylc/flow/etc/job.sh`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/syntax/cylc-mode.el` & `cylc_flow-8.2.6/cylc/flow/etc/syntax/cylc-mode.el`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/syntax/cylc.lang` & `cylc_flow-8.2.6/cylc/flow/etc/syntax/cylc.lang`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/syntax/cylc.vim` & `cylc_flow-8.2.6/cylc/flow/etc/syntax/cylc.vim`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/syntax/cylc.xml` & `cylc_flow-8.2.6/cylc/flow/etc/syntax/cylc.xml`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/.validate` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/.validate`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/bin/consolidate-observations` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/bin/consolidate-observations`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/bin/forecast` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/bin/forecast`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-observations` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-observations`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-rainfall` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/bin/get-rainfall`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/bin/post-process` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/bin/post-process`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/etc/met-office-sites.dat` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/etc/met-office-sites.dat`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/flow.cylc` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/mercator.py` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/mercator.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/util.py` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/lib/python/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/map.html` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/consolidation-tutorial/lib/template/map.html`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/.validate` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/.validate`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/consolidate-observations` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/consolidate-observations`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/forecast` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/forecast`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-observations` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-observations`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-rainfall` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/get-rainfall`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/post-process` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/bin/post-process`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/met-office-sites.dat` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/etc/met-office-sites.dat`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/flow.cylc` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/mercator.py` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/mercator.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/util.py` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/python/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/map.html` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/cylc-forecasting-workflow/lib/template/map.html`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/forecast-script/forecast` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/forecast-script/forecast`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/forecast-script/util.py` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/forecast-script/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/inheritance-tutorial/flow.cylc` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/inheritance-tutorial/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/map-template/map-template.html` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/map-template/map-template.html`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/retries-tutorial/.validate` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/retries-tutorial/.validate`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-introduction/.validate` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-introduction/.validate`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-introduction/flow.cylc` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-introduction/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/bin/consolidate-observations` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/bin/consolidate-observations`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/bin/forecast` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/bin/forecast`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-observations` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-observations`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-rainfall` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/bin/get-rainfall`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/bin/post-process` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/bin/post-process`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/etc/met-office-sites.dat` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/etc/met-office-sites.dat`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/flow.cylc` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/flow.cylc`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/mercator.py` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/mercator.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/util.py` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/lib/python/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/map.html` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/lib/template/map.html`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/runtime-tutorial/runtime` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/runtime-tutorial/runtime`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/test-data/rainfall.csv` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/test-data/rainfall.csv`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_x.csv` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_x.csv`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_y.csv` & `cylc_flow-8.2.6/cylc/flow/etc/tutorial/test-data/wind_20171101T0000Z_y.csv`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/exceptions.py` & `cylc_flow-8.2.6/cylc/flow/exceptions.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/flags.py` & `cylc_flow-8.2.6/cylc/flow/flags.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/flow_mgr.py` & `cylc_flow-8.2.6/cylc/flow/flow_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/graph_parser.py` & `cylc_flow-8.2.6/cylc/flow/graph_parser.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/graphnode.py` & `cylc_flow-8.2.6/cylc/flow/graphnode.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/host_select.py` & `cylc_flow-8.2.6/cylc/flow/host_select.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/hostuserutil.py` & `cylc_flow-8.2.6/cylc/flow/hostuserutil.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/id.py` & `cylc_flow-8.2.6/cylc/flow/id.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/id_cli.py` & `cylc_flow-8.2.6/cylc/flow/id_cli.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/id_match.py` & `cylc_flow-8.2.6/cylc/flow/id_match.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/install.py` & `cylc_flow-8.2.6/cylc/flow/install.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/install_plugins/__init__.py` & `cylc_flow-8.2.6/cylc/flow/install_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/install_plugins/log_vc_info.py` & `cylc_flow-8.2.6/cylc/flow/install_plugins/log_vc_info.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/jinja/filters/duration_as.py` & `cylc_flow-8.2.6/cylc/flow/jinja/filters/duration_as.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/jinja/filters/pad.py` & `cylc_flow-8.2.6/cylc/flow/jinja/filters/pad.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/jinja/filters/strftime.py` & `cylc_flow-8.2.6/cylc/flow/jinja/filters/strftime.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/job_file.py` & `cylc_flow-8.2.6/cylc/flow/job_file.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/job_runner_handlers/__init__.py` & `cylc_flow-8.2.6/cylc/flow/job_runner_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/job_runner_handlers/at.py` & `cylc_flow-8.2.6/cylc/flow/job_runner_handlers/at.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/job_runner_handlers/background.py` & `cylc_flow-8.2.6/cylc/flow/job_runner_handlers/background.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/job_runner_handlers/documentation.py` & `cylc_flow-8.2.6/cylc/flow/job_runner_handlers/documentation.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/job_runner_handlers/loadleveler.py` & `cylc_flow-8.2.6/cylc/flow/job_runner_handlers/loadleveler.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/job_runner_handlers/lsf.py` & `cylc_flow-8.2.6/cylc/flow/job_runner_handlers/lsf.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/job_runner_handlers/moab.py` & `cylc_flow-8.2.6/cylc/flow/job_runner_handlers/moab.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/job_runner_handlers/pbs.py` & `cylc_flow-8.2.6/cylc/flow/job_runner_handlers/pbs.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/job_runner_handlers/pbs_multi_cluster.py` & `cylc_flow-8.2.6/cylc/flow/job_runner_handlers/pbs_multi_cluster.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/job_runner_handlers/sge.py` & `cylc_flow-8.2.6/cylc/flow/job_runner_handlers/sge.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/job_runner_handlers/slurm.py` & `cylc_flow-8.2.6/cylc/flow/job_runner_handlers/slurm.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/job_runner_handlers/slurm_packjob.py` & `cylc_flow-8.2.6/cylc/flow/job_runner_handlers/slurm_packjob.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/job_runner_mgr.py` & `cylc_flow-8.2.6/cylc/flow/job_runner_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/listify.py` & `cylc_flow-8.2.6/cylc/flow/listify.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/log_diagnosis.py` & `cylc_flow-8.2.6/cylc/flow/log_diagnosis.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/loggingutil.py` & `cylc_flow-8.2.6/cylc/flow/loggingutil.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/main_loop/__init__.py` & `cylc_flow-8.2.6/cylc/flow/main_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/main_loop/auto_restart.py` & `cylc_flow-8.2.6/cylc/flow/main_loop/auto_restart.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/main_loop/health_check.py` & `cylc_flow-8.2.6/cylc/flow/main_loop/health_check.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/main_loop/log_data_store.py` & `cylc_flow-8.2.6/cylc/flow/main_loop/log_data_store.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/main_loop/log_db.py` & `cylc_flow-8.2.6/cylc/flow/main_loop/log_db.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/main_loop/log_main_loop.py` & `cylc_flow-8.2.6/cylc/flow/main_loop/log_main_loop.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/main_loop/log_memory.py` & `cylc_flow-8.2.6/cylc/flow/main_loop/log_memory.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/main_loop/reset_bad_hosts.py` & `cylc_flow-8.2.6/cylc/flow/main_loop/reset_bad_hosts.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/network/__init__.py` & `cylc_flow-8.2.6/cylc/flow/network/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/network/authentication.py` & `cylc_flow-8.2.6/cylc/flow/network/authentication.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/network/authorisation.py` & `cylc_flow-8.2.6/cylc/flow/network/authorisation.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/network/client.py` & `cylc_flow-8.2.6/cylc/flow/network/client.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/network/client_factory.py` & `cylc_flow-8.2.6/cylc/flow/network/client_factory.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/network/graphql.py` & `cylc_flow-8.2.6/cylc/flow/network/graphql.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/network/multi.py` & `cylc_flow-8.2.6/cylc/flow/network/multi.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/network/publisher.py` & `cylc_flow-8.2.6/cylc/flow/network/publisher.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/network/replier.py` & `cylc_flow-8.2.6/cylc/flow/network/replier.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/network/resolvers.py` & `cylc_flow-8.2.6/cylc/flow/network/resolvers.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/network/scan.py` & `cylc_flow-8.2.6/cylc/flow/network/scan.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/network/schema.py` & `cylc_flow-8.2.6/cylc/flow/network/schema.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/network/server.py` & `cylc_flow-8.2.6/cylc/flow/network/server.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/network/ssh_client.py` & `cylc_flow-8.2.6/cylc/flow/network/ssh_client.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/network/subscriber.py` & `cylc_flow-8.2.6/cylc/flow/network/subscriber.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/option_parsers.py` & `cylc_flow-8.2.6/cylc/flow/option_parsers.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/param_expand.py` & `cylc_flow-8.2.6/cylc/flow/param_expand.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/parsec/OrderedDict.py` & `cylc_flow-8.2.6/cylc/flow/parsec/OrderedDict.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/parsec/__init__.py` & `cylc_flow-8.2.6/cylc/flow/parsec/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/parsec/config.py` & `cylc_flow-8.2.6/cylc/flow/parsec/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,17 @@
         parents: List[str] = []
         if keys:
             for key in keys:
                 try:
                     cfg = cfg[key]
                 except (KeyError, TypeError):
                     if (
+                        # __MANY__ setting not present:
                         parents in self.manyparents or
+                        # setting not present in __MANY__ section:
                         key in self.spec.get(*parents)
                     ):
                         raise ItemNotFoundError(itemstr(parents, key))
                     raise InvalidConfigError(
                         itemstr(parents, key), self.spec.name
                     )
                 else:
```

### Comparing `cylc-flow-8.2.5/cylc/flow/parsec/empysupport.py` & `cylc_flow-8.2.6/cylc/flow/parsec/empysupport.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/parsec/exceptions.py` & `cylc_flow-8.2.6/cylc/flow/parsec/exceptions.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/parsec/fileparse.py` & `cylc_flow-8.2.6/cylc/flow/parsec/fileparse.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/parsec/include.py` & `cylc_flow-8.2.6/cylc/flow/parsec/include.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/parsec/jinja2support.py` & `cylc_flow-8.2.6/cylc/flow/parsec/jinja2support.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/parsec/upgrade.py` & `cylc_flow-8.2.6/cylc/flow/parsec/upgrade.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/parsec/util.py` & `cylc_flow-8.2.6/cylc/flow/parsec/util.py`

 * *Files 6% similar despite different names*

```diff
@@ -402,20 +402,11 @@
     user defined.
 
     Returns the expanded config i.e. does not modify it in place (this is
     necessary to preserve definition order).
     """
     ret = {}
     for section_name, section in config.items():
-        expanded_names = [
-            dequote(name.strip()).strip()
-            for name in SECTION_EXPAND_PATTERN.findall(section_name)
-        ]
-        for name in expanded_names:
-            if name in ret:
-                # already defined -> merge
-                replicate(ret[name], section)
-
-            else:
-                ret[name] = {}
-                replicate(ret[name], section)
+        for name in SECTION_EXPAND_PATTERN.findall(section_name):
+            name = dequote(name.strip()).strip()
+            replicate(ret.setdefault(name, {}), section)
     return ret
```

### Comparing `cylc-flow-8.2.5/cylc/flow/parsec/validate.py` & `cylc_flow-8.2.6/cylc/flow/parsec/validate.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/pathutil.py` & `cylc_flow-8.2.6/cylc/flow/pathutil.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/pipe_poller.py` & `cylc_flow-8.2.6/cylc/flow/pipe_poller.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/platforms.py` & `cylc_flow-8.2.6/cylc/flow/platforms.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/prerequisite.py` & `cylc_flow-8.2.6/cylc/flow/prerequisite.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/print_tree.py` & `cylc_flow-8.2.6/cylc/flow/print_tree.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/profiler.py` & `cylc_flow-8.2.6/cylc/flow/profiler.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/remote.py` & `cylc_flow-8.2.6/cylc/flow/remote.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/resources.py` & `cylc_flow-8.2.6/cylc/flow/resources.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/rundb.py` & `cylc_flow-8.2.6/cylc/flow/rundb.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scheduler.py` & `cylc_flow-8.2.6/cylc/flow/scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1258,19 +1258,14 @@
         # Write workflow contact file.
         # Preserve contact data in memory, for regular health check.
         workflow_files.dump_contact_file(self.workflow, contact_data)
         self.contact_data = contact_data
 
     def load_flow_file(self, is_reload=False):
         """Load, and log the workflow definition."""
-        # Local workflow environment set therein.
-        # Allow -S and -D to take effect in Cylc VR.
-        # https://github.com/cylc/cylc-flow/issues/5968
-        self.options.rose_template_vars = []
-        self.options.defines = []
         return WorkflowConfig(
             self.workflow,
             self.flow_file,
             self.options,
             self.template_vars,
             xtrigger_mgr=self.xtrigger_mgr,
             mem_log_func=self.profiler.log_memory,
```

### Comparing `cylc-flow-8.2.5/cylc/flow/scheduler_cli.py` & `cylc_flow-8.2.6/cylc/flow/scheduler_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -305,20 +305,16 @@
     parser = COP(
         PLAY_DOC,
         jset=True,
         comms=True,
         argdoc=[WORKFLOW_ID_ARG_DOC]
     )
 
-    options = parser.get_cylc_rose_options() + PLAY_OPTIONS
-    for option in options:
-        if isinstance(option, OptionSettings):
-            parser.add_option(*option.args, **option.kwargs)
-        else:
-            parser.add_option(*option['args'], **option['kwargs'])
+    for option in PLAY_OPTIONS:
+        parser.add_option(*option.args, **option.kwargs)
 
     if add_std_opts:
         # This is for the API wrapper for integration tests. Otherwise (CLI
         # use) "standard options" are added later in options.parse_args().
         # They should really be added in options.__init__() but that requires a
         # bit of refactoring because option clashes are handled bass-ackwards
         # ("overrides" are added before standard options).
```

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/__init__.py` & `cylc_flow-8.2.6/cylc/flow/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/broadcast.py` & `cylc_flow-8.2.6/cylc/flow/scripts/broadcast.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/cat_log.py` & `cylc_flow-8.2.6/cylc/flow/scripts/cat_log.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/check_versions.py` & `cylc_flow-8.2.6/cylc/flow/scripts/check_versions.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/clean.py` & `cylc_flow-8.2.6/cylc/flow/scripts/clean.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/client.py` & `cylc_flow-8.2.6/cylc/flow/scripts/client.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/common.py` & `cylc_flow-8.2.6/cylc/flow/scripts/common.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/completion_server.py` & `cylc_flow-8.2.6/cylc/flow/scripts/completion_server.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/config.py` & `cylc_flow-8.2.6/cylc/flow/scripts/config.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/cycle_point.py` & `cylc_flow-8.2.6/cylc/flow/scripts/cycle_point.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/cylc.py` & `cylc_flow-8.2.6/cylc/flow/scripts/cylc.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/diff.py` & `cylc_flow-8.2.6/cylc/flow/scripts/diff.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/dump.py` & `cylc_flow-8.2.6/cylc/flow/scripts/dump.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/ext_trigger.py` & `cylc_flow-8.2.6/cylc/flow/scripts/ext_trigger.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/function_run.py` & `cylc_flow-8.2.6/cylc/flow/scripts/function_run.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/get_resources.py` & `cylc_flow-8.2.6/cylc/flow/scripts/get_resources.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/get_workflow_contact.py` & `cylc_flow-8.2.6/cylc/flow/scripts/get_workflow_contact.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/get_workflow_version.py` & `cylc_flow-8.2.6/cylc/flow/scripts/get_workflow_version.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/graph.py` & `cylc_flow-8.2.6/cylc/flow/scripts/graph.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/hold.py` & `cylc_flow-8.2.6/cylc/flow/scripts/hold.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/install.py` & `cylc_flow-8.2.6/cylc/flow/scripts/install.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/jobs_kill.py` & `cylc_flow-8.2.6/cylc/flow/scripts/jobs_kill.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/jobs_poll.py` & `cylc_flow-8.2.6/cylc/flow/scripts/jobs_poll.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/jobs_submit.py` & `cylc_flow-8.2.6/cylc/flow/scripts/jobs_submit.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/kill.py` & `cylc_flow-8.2.6/cylc/flow/scripts/kill.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/lint.py` & `cylc_flow-8.2.6/cylc/flow/scripts/lint.py`

 * *Files 3% similar despite different names*

```diff
@@ -261,14 +261,46 @@
     """
     match = INDENTATION.findall(line)[0]
     if not match[0] or not match[1] or match[1].startswith('['):
         return False
     return bool(len(match[0]) % 4 != 0)
 
 
+INHERIT_REGEX = re.compile(r'\s*inherit\s*=\s*(.*)')
+FAM_NAME_IGNORE_REGEX = re.compile(
+    # Stuff we want to ignore when checking for lowercase in family names
+    r'''
+        # comments
+        (?<!{)\#.*
+        # or Cylc parameters
+        | <[^>]+>
+        # or Jinja2
+        | {{.*?}} | {%.*?%} | {\#.*?\#}
+        # or EmPy
+        | (@[\[{\(]).*([\]\}\)])
+    ''',
+    re.X
+)
+LOWERCASE_REGEX = re.compile(r'[a-z]')
+
+
+def check_lowercase_family_names(line: str) -> bool:
+    """Check for lowercase in family names."""
+    match = INHERIT_REGEX.match(line)
+    if not match:
+        return False
+    # Replace stuff we want to ignore with a neutral char (tilde will do):
+    content = FAM_NAME_IGNORE_REGEX.sub('~', match.group(1))
+    return any(
+        LOWERCASE_REGEX.search(i)
+        for i in content.split(',')
+        if i.strip(' \'"') not in {'None', 'none', 'root'}
+    )
+
+
 FUNCTION = 'function'
 
 STYLE_GUIDE = (
     'https://cylc.github.io/cylc-doc/stable/html/workflow-design-guide/'
     'style-guide.html#'
 )
 SECTION2 = r'\[\[\s*{}\s*\]\]'
@@ -347,70 +379,18 @@
         FUNCTION: re.compile(r'^(|\s{1,7}|\s{9,})\[\[\[[^\[.]*\]\]\]').findall
     },
     "S006": {
         'short': 'trailing whitespace.',
         'url': STYLE_GUIDE + 'trailing-whitespace',
         FUNCTION: re.compile(r'[ \t]$').findall
     },
-    # Look for families both from inherit=FAMILY and FAMILY:trigger-all/any.
-    # Do not match inherit lines with `None` at the start.
     "S007": {
         'short': 'Family name contains lowercase characters.',
         'url': STYLE_GUIDE + 'task-naming-conventions',
-        FUNCTION: re.compile(
-            r'''
-            # match all inherit statements
-            ^\s*inherit\s*=
-            # filtering out those which match only valid family names
-            (?!
-                \s*
-                # none, None and root are valid family names
-                # and `inherit =` or `inherit = # x` are valid too
-                (['"]?(none|None|root|\#.*|$)['"]?|
-                (
-                    # as are families named with capital letters
-                    [A-Z0-9_-]+
-                    # and optional quotes
-                    | [\'\"]
-                    # which may include Cylc parameters
-                    | (<[^>]+>)
-                    # or Jinja2
-                    | ({[{%].*[%}]})
-                    # or EmPy
-                    | (@[\[{\(]).*([\]\}\)])
-                )+
-                )
-                # this can be a comma separated list
-                (
-                \s*,\s*
-                # none, None and root are valid family names
-                (['"]?(none|None|root)['"]?|
-                    (
-                    # as are families named with capital letters
-                    [A-Z0-9_-]+
-                    # and optional quotes
-                    | [\'\"]
-                    # which may include Cylc parameters
-                    | (<[^>]+>)
-                    # or Jinja2
-                    | ({[{%].*[%}]})
-                    # or EmPy
-                    | (@[\[{\(]).*([\]\}\)])
-                    )+
-                )
-                )*
-                # allow trailing commas and whitespace
-                \s*,?\s*
-                # allow trailing comments
-                (\#.*)?
-                $
-            )
-            ''',
-            re.X
-        ).findall,
+        FUNCTION: check_lowercase_family_names,
     },
     "S008": {
         'short': JINJA2_FOUND_WITHOUT_SHEBANG,
         'url': '',
         'kwargs': True,
         FUNCTION: functools.partial(
             check_jinja2_no_shebang,
```

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/list.py` & `cylc_flow-8.2.6/cylc/flow/scripts/list.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/message.py` & `cylc_flow-8.2.6/cylc/flow/scripts/message.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/pause.py` & `cylc_flow-8.2.6/cylc/flow/scripts/pause.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/ping.py` & `cylc_flow-8.2.6/cylc/flow/scripts/ping.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/play.py` & `cylc_flow-8.2.6/cylc/flow/scripts/play.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/poll.py` & `cylc_flow-8.2.6/cylc/flow/scripts/poll.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/psutil.py` & `cylc_flow-8.2.6/cylc/flow/scripts/psutil.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/reinstall.py` & `cylc_flow-8.2.6/cylc/flow/scripts/reinstall.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/release.py` & `cylc_flow-8.2.6/cylc/flow/scripts/release.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/reload.py` & `cylc_flow-8.2.6/cylc/flow/scripts/reload.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/remote_init.py` & `cylc_flow-8.2.6/cylc/flow/scripts/remote_init.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/remote_tidy.py` & `cylc_flow-8.2.6/cylc/flow/scripts/remote_tidy.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/remove.py` & `cylc_flow-8.2.6/cylc/flow/scripts/remove.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/report_timings.py` & `cylc_flow-8.2.6/cylc/flow/scripts/report_timings.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/scan.py` & `cylc_flow-8.2.6/cylc/flow/scripts/scan.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/set_outputs.py` & `cylc_flow-8.2.6/cylc/flow/scripts/set_outputs.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/set_verbosity.py` & `cylc_flow-8.2.6/cylc/flow/scripts/set_verbosity.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/show.py` & `cylc_flow-8.2.6/cylc/flow/scripts/show.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/stop.py` & `cylc_flow-8.2.6/cylc/flow/scripts/stop.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/subscribe.py` & `cylc_flow-8.2.6/cylc/flow/scripts/subscribe.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/trigger.py` & `cylc_flow-8.2.6/cylc/flow/scripts/trigger.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/tui.py` & `cylc_flow-8.2.6/cylc/flow/scripts/tui.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/validate.py` & `cylc_flow-8.2.6/cylc/flow/scripts/validate.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/validate_install_play.py` & `cylc_flow-8.2.6/cylc/flow/scripts/validate_install_play.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/validate_reinstall.py` & `cylc_flow-8.2.6/cylc/flow/scripts/validate_reinstall.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/view.py` & `cylc_flow-8.2.6/cylc/flow/scripts/view.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/scripts/workflow_state.py` & `cylc_flow-8.2.6/cylc/flow/scripts/workflow_state.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/subprocctx.py` & `cylc_flow-8.2.6/cylc/flow/subprocctx.py`

 * *Files 6% similar despite different names*

```diff
@@ -154,7 +154,21 @@
 
     def get_signature(self):
         """Return the function call signature (as a string)."""
         skeys = sorted(self.func_kwargs.keys())
         args = self.func_args + [
             "%s=%s" % (i, self.func_kwargs[i]) for i in skeys]
         return "%s(%s)" % (self.func_name, ", ".join([str(a) for a in args]))
+
+    def dump(self) -> str:
+        """Output for logging."""
+        return SubProcContext.__str__(self)
+
+    def __str__(self) -> str:
+        """
+        >>> str(SubFuncContext('label', 'my_func', [1, 2], {'a': 3}))
+        'my_func(1, 2, a=3):10.0'
+        """
+        return f"{self.get_signature()}:{self.intvl}"
+
+    def __repr__(self) -> str:
+        return f"<{type(self).__name__} {self}>"
```

### Comparing `cylc-flow-8.2.5/cylc/flow/subprocpool.py` & `cylc_flow-8.2.6/cylc/flow/subprocpool.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/task_action_timer.py` & `cylc_flow-8.2.6/cylc/flow/task_action_timer.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/task_events_mgr.py` & `cylc_flow-8.2.6/cylc/flow/task_events_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/task_id.py` & `cylc_flow-8.2.6/cylc/flow/task_id.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/task_job_logs.py` & `cylc_flow-8.2.6/cylc/flow/task_job_logs.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/task_job_mgr.py` & `cylc_flow-8.2.6/cylc/flow/task_job_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/task_message.py` & `cylc_flow-8.2.6/cylc/flow/task_message.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/task_outputs.py` & `cylc_flow-8.2.6/cylc/flow/task_outputs.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/task_pool.py` & `cylc_flow-8.2.6/cylc/flow/task_pool.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/task_proxy.py` & `cylc_flow-8.2.6/cylc/flow/task_proxy.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/task_qualifiers.py` & `cylc_flow-8.2.6/cylc/flow/task_qualifiers.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/task_queues/__init__.py` & `cylc_flow-8.2.6/cylc/flow/task_queues/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/task_queues/independent.py` & `cylc_flow-8.2.6/cylc/flow/task_queues/independent.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/task_remote_cmd.py` & `cylc_flow-8.2.6/cylc/flow/task_remote_cmd.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/task_remote_mgr.py` & `cylc_flow-8.2.6/cylc/flow/task_remote_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/task_state.py` & `cylc_flow-8.2.6/cylc/flow/task_state.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/task_state_prop.py` & `cylc_flow-8.2.6/cylc/flow/task_state_prop.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/task_trigger.py` & `cylc_flow-8.2.6/cylc/flow/task_trigger.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/taskdef.py` & `cylc_flow-8.2.6/cylc/flow/taskdef.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/templatevars.py` & `cylc_flow-8.2.6/cylc/flow/templatevars.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/terminal.py` & `cylc_flow-8.2.6/cylc/flow/terminal.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/time_parser.py` & `cylc_flow-8.2.6/cylc/flow/time_parser.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/timer.py` & `cylc_flow-8.2.6/cylc/flow/timer.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/tui/__init__.py` & `cylc_flow-8.2.6/cylc/flow/tui/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/tui/app.py` & `cylc_flow-8.2.6/cylc/flow/tui/app.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/tui/data.py` & `cylc_flow-8.2.6/cylc/flow/tui/data.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/tui/overlay.py` & `cylc_flow-8.2.6/cylc/flow/tui/overlay.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/tui/tree.py` & `cylc_flow-8.2.6/cylc/flow/tui/tree.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/tui/util.py` & `cylc_flow-8.2.6/cylc/flow/tui/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/unicode_rules.py` & `cylc_flow-8.2.6/cylc/flow/unicode_rules.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/util.py` & `cylc_flow-8.2.6/cylc/flow/util.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/wallclock.py` & `cylc_flow-8.2.6/cylc/flow/wallclock.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/workflow_db_mgr.py` & `cylc_flow-8.2.6/cylc/flow/workflow_db_mgr.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/workflow_events.py` & `cylc_flow-8.2.6/cylc/flow/workflow_events.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/workflow_files.py` & `cylc_flow-8.2.6/cylc/flow/workflow_files.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/workflow_status.py` & `cylc_flow-8.2.6/cylc/flow/workflow_status.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/xtrigger_mgr.py` & `cylc_flow-8.2.6/cylc/flow/xtrigger_mgr.py`

 * *Files 0% similar despite different names*

```diff
@@ -498,15 +498,15 @@
         Record satisfaction status and function results dict.
 
         Args:
             ctx (SubFuncContext): function context
         Raises:
             ValueError: if the context given is not active
         """
-        LOG.debug(ctx)
+        LOG.debug(ctx.dump())
         sig = ctx.get_signature()
         self.active.remove(sig)
         try:
             satisfied, results = json.loads(ctx.out)
         except (ValueError, TypeError):
             return
         LOG.debug('%s: returned %s', sig, results)
```

### Comparing `cylc-flow-8.2.5/cylc/flow/xtriggers/__init__.py` & `cylc_flow-8.2.6/cylc/flow/xtriggers/__init__.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/xtriggers/echo.py` & `cylc_flow-8.2.6/cylc/flow/xtriggers/echo.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/xtriggers/wall_clock.py` & `cylc_flow-8.2.6/cylc/flow/xtriggers/wall_clock.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/xtriggers/workflow_state.py` & `cylc_flow-8.2.6/cylc/flow/xtriggers/workflow_state.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc/flow/xtriggers/xrandom.py` & `cylc_flow-8.2.6/cylc/flow/xtriggers/xrandom.py`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc_flow.egg-info/PKG-INFO` & `cylc_flow-8.2.6/cylc_flow.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cylc-flow
-Version: 8.2.5
+Version: 8.2.6
 Summary: A workflow engine for cycling systems
 Home-page: https://cylc.org/
 Author: Hilary Oliver
 License: GPL
 Project-URL: Documentation, https://cylc.github.io/cylc-doc/stable/html/index.html
 Project-URL: Source, https://github.com/cylc/cylc-flow
 Project-URL: Tracker, https://github.com/cylc/cylc-flow/issues
@@ -70,15 +70,15 @@
 Requires-Dist: flake8-builtins>=1.5.0; extra == "tests"
 Requires-Dist: flake8-comprehensions>=3.5.0; extra == "tests"
 Requires-Dist: flake8-debugger>=4.0.0; extra == "tests"
 Requires-Dist: flake8-mutable>=1.2.0; extra == "tests"
 Requires-Dist: flake8-simplify>=0.14.0; extra == "tests"
 Requires-Dist: flake8>=3.0.0; extra == "tests"
 Requires-Dist: mypy<1.9,>=0.910; extra == "tests"
-Requires-Dist: pytest-asyncio!=0.23.*,>=0.17; extra == "tests"
+Requires-Dist: pytest-asyncio!=0.23.*,>=0.21.2; extra == "tests"
 Requires-Dist: pytest-cov>=2.8.0; extra == "tests"
 Requires-Dist: pytest-xdist>=2; extra == "tests"
 Requires-Dist: pytest-env>=0.6.2; extra == "tests"
 Requires-Dist: pytest-mock>=3.7; extra == "tests"
 Requires-Dist: pytest>=6; extra == "tests"
 Requires-Dist: testfixtures>=6.11.0; extra == "tests"
 Requires-Dist: towncrier>=23; extra == "tests"
@@ -109,15 +109,15 @@
 Requires-Dist: flake8-builtins>=1.5.0; extra == "all"
 Requires-Dist: flake8-comprehensions>=3.5.0; extra == "all"
 Requires-Dist: flake8-debugger>=4.0.0; extra == "all"
 Requires-Dist: flake8-mutable>=1.2.0; extra == "all"
 Requires-Dist: flake8-simplify>=0.14.0; extra == "all"
 Requires-Dist: flake8>=3.0.0; extra == "all"
 Requires-Dist: mypy<1.9,>=0.910; extra == "all"
-Requires-Dist: pytest-asyncio!=0.23.*,>=0.17; extra == "all"
+Requires-Dist: pytest-asyncio!=0.23.*,>=0.21.2; extra == "all"
 Requires-Dist: pytest-cov>=2.8.0; extra == "all"
 Requires-Dist: pytest-xdist>=2; extra == "all"
 Requires-Dist: pytest-env>=0.6.2; extra == "all"
 Requires-Dist: pytest-mock>=3.7; extra == "all"
 Requires-Dist: pytest>=6; extra == "all"
 Requires-Dist: testfixtures>=6.11.0; extra == "all"
 Requires-Dist: towncrier>=23; extra == "all"
```

### Comparing `cylc-flow-8.2.5/cylc_flow.egg-info/SOURCES.txt` & `cylc_flow-8.2.6/cylc_flow.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -89,14 +89,15 @@
 cylc/flow/cycling/util.py
 cylc/flow/etc/README.md
 cylc/flow/etc/cylc
 cylc/flow/etc/cylc-completion.bash
 cylc/flow/etc/job.sh
 cylc/flow/etc/syntax/cylc-mode.el
 cylc/flow/etc/syntax/cylc.lang
+cylc/flow/etc/syntax/cylc.nanorc
 cylc/flow/etc/syntax/cylc.vim
 cylc/flow/etc/syntax/cylc.xml
 cylc/flow/etc/tutorial/api-keys
 cylc/flow/etc/tutorial/consolidation-tutorial/.validate
 cylc/flow/etc/tutorial/consolidation-tutorial/flow.cylc
 cylc/flow/etc/tutorial/consolidation-tutorial/bin/consolidate-observations
 cylc/flow/etc/tutorial/consolidation-tutorial/bin/forecast
```

### Comparing `cylc-flow-8.2.5/cylc_flow.egg-info/entry_points.txt` & `cylc_flow-8.2.6/cylc_flow.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/cylc_flow.egg-info/requires.txt` & `cylc_flow-8.2.6/cylc_flow.egg-info/requires.txt`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 flake8-builtins>=1.5.0
 flake8-comprehensions>=3.5.0
 flake8-debugger>=4.0.0
 flake8-mutable>=1.2.0
 flake8-simplify>=0.14.0
 flake8>=3.0.0
 mypy<1.9,>=0.910
-pytest-asyncio!=0.23.*,>=0.17
+pytest-asyncio!=0.23.*,>=0.21.2
 pytest-cov>=2.8.0
 pytest-xdist>=2
 pytest-env>=0.6.2
 pytest-mock>=3.7
 pytest>=6
 testfixtures>=6.11.0
 towncrier>=23
@@ -85,15 +85,15 @@
 flake8-builtins>=1.5.0
 flake8-comprehensions>=3.5.0
 flake8-debugger>=4.0.0
 flake8-mutable>=1.2.0
 flake8-simplify>=0.14.0
 flake8>=3.0.0
 mypy<1.9,>=0.910
-pytest-asyncio!=0.23.*,>=0.17
+pytest-asyncio!=0.23.*,>=0.21.2
 pytest-cov>=2.8.0
 pytest-xdist>=2
 pytest-env>=0.6.2
 pytest-mock>=3.7
 pytest>=6
 testfixtures>=6.11.0
 towncrier>=23
```

### Comparing `cylc-flow-8.2.5/pyproject.toml` & `cylc_flow-8.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cylc-flow-8.2.5/setup.cfg` & `cylc_flow-8.2.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 	flake8-builtins>=1.5.0
 	flake8-comprehensions>=3.5.0
 	flake8-debugger>=4.0.0
 	flake8-mutable>=1.2.0
 	flake8-simplify>=0.14.0
 	flake8>=3.0.0
 	mypy>=0.910,<1.9
-	pytest-asyncio>=0.17,!=0.23.*
+	pytest-asyncio>=0.21.2,!=0.23.*
 	pytest-cov>=2.8.0
 	pytest-xdist>=2
 	pytest-env>=0.6.2
 	pytest-mock>=3.7
 	pytest>=6
 	testfixtures>=6.11.0
 	towncrier>=23
```

### Comparing `cylc-flow-8.2.5/setup.py` & `cylc_flow-8.2.6/setup.py`

 * *Files identical despite different names*

