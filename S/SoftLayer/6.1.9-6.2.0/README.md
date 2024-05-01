# Comparing `tmp/SoftLayer-6.1.9.tar.gz` & `tmp/softlayer-6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SoftLayer-6.1.9.tar", last modified: Thu Sep 21 21:24:26 2023, max compression
+gzip compressed data, was "softlayer-6.2.0.tar", last modified: Wed May  1 22:33:54 2024, max compression
```

## Comparing `SoftLayer-6.1.9.tar` & `softlayer-6.2.0.tar`

### file list

```diff
@@ -1,674 +1,678 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.735067 SoftLayer-6.1.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8152 2023-09-21 21:24:26.735067 SoftLayer-6.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6776 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.651065 SoftLayer-6.1.9/SoftLayer/
--rw-r--r--   0 runner    (1001) docker     (127)    22932 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/API.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.655065 SoftLayer-6.1.9/SoftLayer/CLI/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.659066 SoftLayer-6.1.9/SoftLayer/CLI/account/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/account/billing_items.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/account/cancel_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/account/event_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     5144 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/account/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/account/hook_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/account/hook_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/account/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/account/invoice_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/account/invoices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/account/item_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/account/licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/account/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/account/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.659066 SoftLayer-6.1.9/SoftLayer/CLI/bandwidth/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/bandwidth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/bandwidth/pools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/bandwidth/pools_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/bandwidth/pools_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/bandwidth/pools_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/bandwidth/pools_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/bandwidth/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.659066 SoftLayer-6.1.9/SoftLayer/CLI/block/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.663066 SoftLayer-6.1.9/SoftLayer/CLI/block/access/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/access/authorize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/access/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/access/password.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/access/revoke.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/count.py
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/duplicate_convert_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/lun.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/modify.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/object_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/object_storage_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/object_storage_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     5778 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5249 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/order.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/refresh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.663066 SoftLayer-6.1.9/SoftLayer/CLI/block/replication/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/replication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/replication/disaster_recovery_failover.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/replication/failback.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/replication/failover.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/replication/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/replication/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/replication/partners.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/set_note.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.663066 SoftLayer-6.1.9/SoftLayer/CLI/block/snapshot/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/snapshot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/snapshot/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/snapshot/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/snapshot/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/snapshot/disable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/snapshot/enable.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/snapshot/get_notify_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/snapshot/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/snapshot/order.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/snapshot/restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/snapshot/schedule_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/snapshot/set_notify_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.663066 SoftLayer-6.1.9/SoftLayer/CLI/block/subnets/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/subnets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/subnets/assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/subnets/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/block/subnets/remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     7255 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/call_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.667066 SoftLayer-6.1.9/SoftLayer/CLI/cdn/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/cdn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/cdn/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/cdn/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/cdn/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/cdn/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/cdn/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/cdn/origin_add.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/cdn/origin_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/cdn/origin_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/cdn/purge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     8794 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.667066 SoftLayer-6.1.9/SoftLayer/CLI/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10609 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/config/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/config/show.py
--rw-r--r--   0 runner    (1001) docker     (127)     7264 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/custom_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.667066 SoftLayer-6.1.9/SoftLayer/CLI/dedicatedhost/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/dedicatedhost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/dedicatedhost/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/dedicatedhost/cancel_guests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/dedicatedhost/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/dedicatedhost/create_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/dedicatedhost/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/dedicatedhost/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/dedicatedhost/list_guests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.667066 SoftLayer-6.1.9/SoftLayer/CLI/dns/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/dns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/dns/record_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/dns/record_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/dns/record_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/dns/record_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/dns/zone_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/dns/zone_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/dns/zone_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/dns/zone_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/dns/zone_print.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.671066 SoftLayer-6.1.9/SoftLayer/CLI/email/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/email/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/email/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/email/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     8791 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.671066 SoftLayer-6.1.9/SoftLayer/CLI/event_log/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/event_log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/event_log/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/event_log/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.671066 SoftLayer-6.1.9/SoftLayer/CLI/file/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.671066 SoftLayer-6.1.9/SoftLayer/CLI/file/access/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/access/authorize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/access/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/access/revoke.py
--rw-r--r--   0 runner    (1001) docker     (127)     1694 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/count.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/duplicate_convert_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3169 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/modify.py
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5674 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/refresh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.675066 SoftLayer-6.1.9/SoftLayer/CLI/file/replication/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/replication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/replication/disaster_recovery_failover.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/replication/failback.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/replication/failover.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/replication/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/replication/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/replication/partners.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/set_note.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.675066 SoftLayer-6.1.9/SoftLayer/CLI/file/snapshot/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/snapshot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/snapshot/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/snapshot/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/snapshot/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/snapshot/disable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/snapshot/enable.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/snapshot/get_notify_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/snapshot/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/snapshot/order.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/snapshot/restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/snapshot/schedule_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/file/snapshot/set_notify_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.675066 SoftLayer-6.1.9/SoftLayer/CLI/firewall/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/firewall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/firewall/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/firewall/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/firewall/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     6485 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/firewall/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3837 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/firewall/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/firewall/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    17108 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/formatting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.675066 SoftLayer-6.1.9/SoftLayer/CLI/globalip/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/globalip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/globalip/assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/globalip/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/globalip/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/globalip/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/globalip/unassign.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.679066 SoftLayer-6.1.9/SoftLayer/CLI/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/hardware/authorize_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/hardware/bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/hardware/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/hardware/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/hardware/cancel_reasons.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/hardware/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/hardware/create_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     6630 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/hardware/create_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/hardware/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     7498 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/hardware/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/hardware/dns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/hardware/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/hardware/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/hardware/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/hardware/notification_add.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/hardware/notification_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/hardware/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/hardware/power.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/hardware/ready.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/hardware/reflash_firmware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/hardware/reload.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/hardware/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/hardware/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/hardware/toggle_ipmi.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/hardware/update_firmware.py
--rw-r--r--   0 runner    (1001) docker     (127)     7557 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/hardware/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.683066 SoftLayer-6.1.9/SoftLayer/CLI/image/
--rw-r--r--   0 runner    (1001) docker     (127)      848 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/image/datacenter.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/image/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/image/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/image/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/image/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/image/import.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/image/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/image/share.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/image/share_deny.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.683066 SoftLayer-6.1.9/SoftLayer/CLI/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/licenses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/licenses/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/licenses/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/licenses/create_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.683066 SoftLayer-6.1.9/SoftLayer/CLI/loadbal/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/loadbal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6447 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/loadbal/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/loadbal/health.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/loadbal/layer7_policy_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/loadbal/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/loadbal/members.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/loadbal/ns_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/loadbal/ns_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     7648 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/loadbal/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     9306 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/loadbal/pools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/loadbal/protocol_add.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/loadbal/protocol_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/loadbal/protocol_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.683066 SoftLayer-6.1.9/SoftLayer/CLI/nas/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/nas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/nas/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/nas/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.683066 SoftLayer-6.1.9/SoftLayer/CLI/object_storage/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/object_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/object_storage/cancel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.687066 SoftLayer-6.1.9/SoftLayer/CLI/object_storage/credential/
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/object_storage/credential/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/object_storage/credential/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/object_storage/credential/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/object_storage/credential/limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/object_storage/credential/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/object_storage/list_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/object_storage/list_endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.687066 SoftLayer-6.1.9/SoftLayer/CLI/order/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/order/cancelation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/order/category_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/order/item_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/order/lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/order/package_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/order/package_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/order/place.py
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/order/place_quote.py
--rw-r--r--   0 runner    (1001) docker     (127)     6259 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/order/preset_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5656 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/order/quote.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/order/quote_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/order/quote_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/order/quote_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/order/quote_save.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.687066 SoftLayer-6.1.9/SoftLayer/CLI/report/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5519 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/report/dc_closures.py
--rw-r--r--   0 runner    (1001) docker     (127)    25258 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.691066 SoftLayer-6.1.9/SoftLayer/CLI/security/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/security/cert_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/security/cert_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/security/cert_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/security/cert_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/security/cert_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/security/sshkey_add.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/security/sshkey_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/security/sshkey_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/security/sshkey_print.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/security/sshkey_remove.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.691066 SoftLayer-6.1.9/SoftLayer/CLI/securitygroup/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/securitygroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/securitygroup/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/securitygroup/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/securitygroup/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/securitygroup/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/securitygroup/event_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/securitygroup/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/securitygroup/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/securitygroup/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.691066 SoftLayer-6.1.9/SoftLayer/CLI/sshkey/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/sshkey/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.691066 SoftLayer-6.1.9/SoftLayer/CLI/ssl/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/ssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/storage_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.691066 SoftLayer-6.1.9/SoftLayer/CLI/subnet/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/subnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/subnet/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/subnet/clear_route.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/subnet/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/subnet/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/subnet/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/subnet/edit_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/subnet/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/subnet/lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/subnet/route.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.695066 SoftLayer-6.1.9/SoftLayer/CLI/tags/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/tags/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/tags/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/tags/details.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/tags/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/tags/set.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/tags/taggable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.695066 SoftLayer-6.1.9/SoftLayer/CLI/ticket/
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/ticket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/ticket/attach.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/ticket/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/ticket/detach.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/ticket/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/ticket/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/ticket/subjects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/ticket/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/ticket/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/ticket/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.699066 SoftLayer-6.1.9/SoftLayer/CLI/user/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/user/apikey.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/user/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/user/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     6394 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/user/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/user/device_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/user/edit_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/user/edit_notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/user/edit_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/user/grant_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/user/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/user/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/user/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/user/remove_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/user/vpn_enable_or_disable.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/user/vpn_manual.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/user/vpn_password.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/user/vpn_subnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.703066 SoftLayer-6.1.9/SoftLayer/CLI/virt/
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/access.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/authorize_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/cancel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.703066 SoftLayer-6.1.9/SoftLayer/CLI/virt/capacity/
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/capacity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/capacity/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/capacity/create_guest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/capacity/create_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/capacity/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/capacity/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/capture.py
--rw-r--r--   0 runner    (1001) docker     (127)    14724 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/create.py
--rw-r--r--   0 runner    (1001) docker     (127)    11386 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/create_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     8526 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/dns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4384 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/migrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/notification_add.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/notification_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/os_available.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.703066 SoftLayer-6.1.9/SoftLayer/CLI/virt/placementgroup/
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/placementgroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/placementgroup/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/placementgroup/create_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/placementgroup/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/placementgroup/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/placementgroup/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/power.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/ready.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/reload.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/virt/usage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.703066 SoftLayer-6.1.9/SoftLayer/CLI/vlan/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/vlan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/vlan/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/vlan/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/vlan/create_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5475 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/vlan/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/vlan/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/vlan/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.703066 SoftLayer-6.1.9/SoftLayer/CLI/vpn/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/vpn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.703066 SoftLayer-6.1.9/SoftLayer/CLI/vpn/ipsec/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/vpn/ipsec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/vpn/ipsec/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/vpn/ipsec/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7675 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/vpn/ipsec/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/vpn/ipsec/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/vpn/ipsec/order.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.707066 SoftLayer-6.1.9/SoftLayer/CLI/vpn/ipsec/subnet/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/vpn/ipsec/subnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/vpn/ipsec/subnet/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/vpn/ipsec/subnet/remove.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.707066 SoftLayer-6.1.9/SoftLayer/CLI/vpn/ipsec/translation/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/vpn/ipsec/translation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/vpn/ipsec/translation/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/vpn/ipsec/translation/remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/vpn/ipsec/translation/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/CLI/vpn/ipsec/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4053 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/decoration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.719066 SoftLayer-6.1.9/SoftLayer/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/BluePages_Search.py
--rw-r--r--   0 runner    (1001) docker     (127)    44611 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Account.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Billing_Invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Billing_Invoice_Item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Billing_Item.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Billing_Item_Cancellation_Request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Billing_Order.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Billing_Order_Quote.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Dns_Domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Dns_Domain_ResourceRecord.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Email_Subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Event_Log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)    11328 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Hardware_Server.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Location.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Location_Datacenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Location_Group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Metric_Tracking_Object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Health_Check_Type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Routing_Method.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Routing_Type.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Service.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Service_Group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_VirtualIpAddress.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_VirtualServer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Bandwidth_Version1_Allotment.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Cache_Purge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Mapping_Path.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Component_Firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Firewall_Update_Request.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_LBaaS_HealthMonitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_LBaaS_L7Pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_LBaaS_Listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     5814 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_LBaaS_LoadBalancer.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_LBaaS_Member.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Message_Delivery_Email_Sendgrid.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Pod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_SecurityGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Service_Vpn_Overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)    10038 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Storage_Allowed_Host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Storage_Hub_Cleversafe_Account.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Storage_Iscsi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Subnet.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Subnet_IpAddress.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Subnet_IpAddress_Global.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Subnet_Rwhois_Data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5088 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Vlan.py
--rw-r--r--   0 runner    (1001) docker     (127)     8928 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Vlan_Firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Notification_Occurrence_Event.py
--rw-r--r--   0 runner    (1001) docker     (127)     9163 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Product_Order.py
--rw-r--r--   0 runner    (1001) docker     (127)    75145 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Product_Package.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Product_Package_Preset.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Provisioning_Hook.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Provisioning_Maintenance_Window.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Resource_Metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    16122 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Scale_Group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Scale_Policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Security_Certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Security_Ssh_Key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Software_AccountLicense.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Software_Component_Password.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Ticket.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Ticket_Subject.py
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_User_Customer.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_User_Customer_CustomerPermission_Permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_User_Customer_Notification_Hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_User_Customer_Notification_Virtual_Guest.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_User_Permission_Action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Virtual_DedicatedHost.py
--rw-r--r--   0 runner    (1001) docker     (127)    29326 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Virtual_Guest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Virtual_Guest_Block_Device_Template_Group.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Virtual_Host.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Virtual_PlacementGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Virtual_PlacementGroup_Rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Virtual_ReservedCapacityGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.723066 SoftLayer-6.1.9/SoftLayer/managers/
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15614 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (127)     8548 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/block.py
--rw-r--r--   0 runner    (1001) docker     (127)    14570 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/cdn.py
--rw-r--r--   0 runner    (1001) docker     (127)    19234 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/dedicated_host.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/dns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/email.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/event_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     6647 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    13364 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)    53249 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)    10000 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    15244 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/ipsec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/license.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)    13010 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    34611 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/object_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    33086 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/ordering.py
--rw-r--r--   0 runner    (1001) docker     (127)     3889 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/sshkey.py
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)    26132 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    42298 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9106 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     5407 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/ticket.py
--rw-r--r--   0 runner    (1001) docker     (127)    20179 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    63463 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/vs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7542 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/vs_capacity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/managers/vs_placement.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.723066 SoftLayer-6.1.9/SoftLayer/shell/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/shell/cmd_env.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/shell/cmd_exit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/shell/cmd_help.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/shell/completer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/shell/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/shell/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.723066 SoftLayer-6.1.9/SoftLayer/testing/
--rw-r--r--   0 runner    (1001) docker     (127)     6628 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/testing/xmlrpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.723066 SoftLayer-6.1.9/SoftLayer/transports/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/transports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/transports/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/transports/fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     6062 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/transports/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/transports/timing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4325 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/transports/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     6748 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/transports/xmlrpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15228 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/SoftLayer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.655065 SoftLayer-6.1.9/SoftLayer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8152 2023-09-21 21:24:26.000000 SoftLayer-6.1.9/SoftLayer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22767 2023-09-21 21:24:26.000000 SoftLayer-6.1.9/SoftLayer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-21 21:24:26.000000 SoftLayer-6.1.9/SoftLayer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2023-09-21 21:24:26.000000 SoftLayer-6.1.9/SoftLayer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-21 21:24:26.000000 SoftLayer-6.1.9/SoftLayer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      110 2023-09-21 21:24:26.000000 SoftLayer-6.1.9/SoftLayer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-09-21 21:24:26.000000 SoftLayer-6.1.9/SoftLayer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2023-09-21 21:24:26.739066 SoftLayer-6.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.651065 SoftLayer-6.1.9/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.723066 SoftLayer-6.1.9/tests/CLI/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/core_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/custom_types_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/environment_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    17189 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/helper_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.731067 SoftLayer-6.1.9/tests/CLI/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9126 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/account_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    11282 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/bandwidth_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    43925 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/block_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    12903 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/call_api_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/cdn_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8172 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/config_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    17724 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/dedicatedhost_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    11932 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/dns_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/email_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/event_log_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    36599 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/file_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8769 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/firewall_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/globalip_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/image_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    27405 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/ipsec_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/licenses_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    15854 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/loadbal_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/nas_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/object_storage_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    23416 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/order_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5911 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/report_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/search_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     6075 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/security_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    14341 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/securitygroup_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    45345 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/server_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/sshkey_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/ssl_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     7832 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/subnet_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/summary_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/tag_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    15445 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/ticket_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    20619 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/user_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    14986 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/vlan_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.731067 SoftLayer-6.1.9/tests/CLI/modules/vs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/vs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4074 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/vs/vs_capacity_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    33577 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/vs/vs_create_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5052 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/vs/vs_placement_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    43881 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/CLI/modules/vs/vs_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.735067 SoftLayer-6.1.9/tests/managers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7771 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/account_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/bandwidth_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    42152 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/block_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/cdn_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    24093 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/dedicated_host_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     7520 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/dns_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/email_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     7922 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/event_log_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    34792 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/file_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    12808 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/firewall_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    43036 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/hardware_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8859 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/image_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    16589 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/ipsec_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     9915 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/loadbal_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/metadata_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    28050 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/network_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/object_storage_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    40766 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/ordering_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/search_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/sshkey_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/ssl_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/storage_generic_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)   142912 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/storage_utils_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     9155 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/tag_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/ticket_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    15851 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/user_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.735067 SoftLayer-6.1.9/tests/managers/vs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/vs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8014 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/vs/vs_capacity_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    10772 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/vs/vs_order_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/vs/vs_placement_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    45298 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/vs/vs_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     6490 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/managers/vs/vs_waiting_for_ready_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:26.735067 SoftLayer-6.1.9/tests/transports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/transports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/transports/debug_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    11809 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/transports/rest_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/transports/transport_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    14582 2023-09-21 21:24:15.000000 SoftLayer-6.1.9/tests/transports/xmlrpc_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:54.000584 softlayer-6.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-01 22:33:50.000000 softlayer-6.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-01 22:33:50.000000 softlayer-6.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7998 2024-05-01 22:33:54.000584 softlayer-6.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-05-01 22:33:50.000000 softlayer-6.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.912583 softlayer-6.2.0/SoftLayer/
+-rw-r--r--   0 runner    (1001) docker     (127)    33115 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/API.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.916583 softlayer-6.2.0/SoftLayer/CLI/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.916583 softlayer-6.2.0/SoftLayer/CLI/account/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/account/billing_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/account/cancel_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/account/event_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/account/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/account/hook_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/account/hook_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/account/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/account/invoice_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/account/invoices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/account/item_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/account/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/account/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/account/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.920583 softlayer-6.2.0/SoftLayer/CLI/bandwidth/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/bandwidth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/bandwidth/pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/bandwidth/pools_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/bandwidth/pools_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/bandwidth/pools_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/bandwidth/pools_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/bandwidth/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.920583 softlayer-6.2.0/SoftLayer/CLI/block/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.920583 softlayer-6.2.0/SoftLayer/CLI/block/access/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/access/authorize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/access/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/access/password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/access/revoke.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/duplicate_convert_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/lun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/modify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/object_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/object_storage_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/object_storage_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/refresh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.924583 softlayer-6.2.0/SoftLayer/CLI/block/replication/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/replication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/replication/disaster_recovery_failover.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/replication/failback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/replication/failover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/replication/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/replication/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/replication/partners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/set_note.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.924583 softlayer-6.2.0/SoftLayer/CLI/block/snapshot/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/snapshot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/snapshot/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/snapshot/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/snapshot/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/snapshot/disable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/snapshot/enable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/snapshot/get_notify_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/snapshot/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/snapshot/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/snapshot/restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/snapshot/schedule_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/snapshot/set_notify_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.924583 softlayer-6.2.0/SoftLayer/CLI/block/subnets/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/subnets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/subnets/assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/subnets/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/block/subnets/remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/call_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.928583 softlayer-6.2.0/SoftLayer/CLI/cdn/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/cdn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/cdn/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/cdn/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/cdn/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/cdn/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/cdn/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/cdn/origin_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/cdn/origin_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/cdn/origin_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/cdn/purge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.928583 softlayer-6.2.0/SoftLayer/CLI/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10609 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/config/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/config/show.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7555 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/custom_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.928583 softlayer-6.2.0/SoftLayer/CLI/dedicatedhost/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/dedicatedhost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/dedicatedhost/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/dedicatedhost/cancel_guests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/dedicatedhost/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/dedicatedhost/create_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/dedicatedhost/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/dedicatedhost/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/dedicatedhost/list_guests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.928583 softlayer-6.2.0/SoftLayer/CLI/dns/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/dns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/dns/record_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/dns/record_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/dns/record_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/dns/record_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/dns/zone_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/dns/zone_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/dns/zone_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/dns/zone_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/dns/zone_print.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.928583 softlayer-6.2.0/SoftLayer/CLI/email/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/email/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/email/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/email/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.932583 softlayer-6.2.0/SoftLayer/CLI/event_log/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/event_log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/event_log/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/event_log/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.932583 softlayer-6.2.0/SoftLayer/CLI/file/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.932583 softlayer-6.2.0/SoftLayer/CLI/file/access/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/access/authorize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/access/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/access/revoke.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1694 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/duplicate_convert_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/modify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/refresh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.932583 softlayer-6.2.0/SoftLayer/CLI/file/replication/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/replication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/replication/disaster_recovery_failover.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/replication/failback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/replication/failover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/replication/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/replication/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/replication/partners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/set_note.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.936583 softlayer-6.2.0/SoftLayer/CLI/file/snapshot/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/snapshot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/snapshot/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/snapshot/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/snapshot/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/snapshot/disable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/snapshot/enable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/snapshot/get_notify_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/snapshot/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/snapshot/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/snapshot/restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/snapshot/schedule_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/file/snapshot/set_notify_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.936583 softlayer-6.2.0/SoftLayer/CLI/firewall/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/firewall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/firewall/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/firewall/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/firewall/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/firewall/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/firewall/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/firewall/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17828 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/formatting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.936583 softlayer-6.2.0/SoftLayer/CLI/globalip/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/globalip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/globalip/assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/globalip/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/globalip/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/globalip/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/globalip/unassign.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.940583 softlayer-6.2.0/SoftLayer/CLI/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/authorize_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/cancel_reasons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/create_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/create_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/notification_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/notification_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/power.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/ready.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/reflash_firmware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/reload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/toggle_ipmi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/update_firmware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/vlan_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/vlan_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/hardware/vlan_trunkable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.944583 softlayer-6.2.0/SoftLayer/CLI/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/image/datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/image/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/image/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/image/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/image/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/image/import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/image/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/image/share.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/image/share_deny.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.944583 softlayer-6.2.0/SoftLayer/CLI/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/licenses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/licenses/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/licenses/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/licenses/create_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.944583 softlayer-6.2.0/SoftLayer/CLI/loadbal/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/loadbal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/loadbal/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/loadbal/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/loadbal/layer7_policy_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/loadbal/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/loadbal/members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/loadbal/ns_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/loadbal/ns_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/loadbal/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/loadbal/pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/loadbal/protocol_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/loadbal/protocol_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/loadbal/protocol_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.948583 softlayer-6.2.0/SoftLayer/CLI/nas/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/nas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/nas/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/nas/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.948583 softlayer-6.2.0/SoftLayer/CLI/object_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/object_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/object_storage/cancel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.948583 softlayer-6.2.0/SoftLayer/CLI/object_storage/credential/
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/object_storage/credential/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/object_storage/credential/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/object_storage/credential/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/object_storage/credential/limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/object_storage/credential/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/object_storage/list_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/object_storage/list_endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.948583 softlayer-6.2.0/SoftLayer/CLI/order/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/order/cancelation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/order/category_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/order/item_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/order/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/order/package_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/order/package_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/order/place.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/order/place_quote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/order/preset_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/order/quote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/order/quote_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/order/quote_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/order/quote_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/order/quote_save.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.948583 softlayer-6.2.0/SoftLayer/CLI/report/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/report/dc_closures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25519 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.952583 softlayer-6.2.0/SoftLayer/CLI/security/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/security/cert_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/security/cert_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/security/cert_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/security/cert_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/security/cert_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/security/sshkey_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/security/sshkey_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/security/sshkey_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/security/sshkey_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/security/sshkey_remove.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.952583 softlayer-6.2.0/SoftLayer/CLI/securitygroup/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/securitygroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/securitygroup/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/securitygroup/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/securitygroup/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/securitygroup/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/securitygroup/event_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/securitygroup/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/securitygroup/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/securitygroup/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.952583 softlayer-6.2.0/SoftLayer/CLI/sshkey/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/sshkey/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.952583 softlayer-6.2.0/SoftLayer/CLI/ssl/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/ssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/storage_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.956583 softlayer-6.2.0/SoftLayer/CLI/subnet/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/subnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/subnet/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/subnet/clear_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/subnet/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/subnet/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/subnet/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/subnet/edit_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/subnet/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/subnet/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/subnet/route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.956583 softlayer-6.2.0/SoftLayer/CLI/tags/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/tags/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/tags/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/tags/details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/tags/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/tags/set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/tags/taggable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.956583 softlayer-6.2.0/SoftLayer/CLI/ticket/
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/ticket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/ticket/attach.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/ticket/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/ticket/detach.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/ticket/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/ticket/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/ticket/subjects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/ticket/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/ticket/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/ticket/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.960584 softlayer-6.2.0/SoftLayer/CLI/user/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/user/apikey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/user/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/user/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/user/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/user/device_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/user/edit_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/user/edit_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/user/edit_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/user/grant_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/user/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/user/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/user/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/user/remove_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/user/vpn_enable_or_disable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/user/vpn_manual.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/user/vpn_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/user/vpn_subnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.964583 softlayer-6.2.0/SoftLayer/CLI/virt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/authorize_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/cancel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.964583 softlayer-6.2.0/SoftLayer/CLI/virt/capacity/
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/capacity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/capacity/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/capacity/create_guest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/capacity/create_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/capacity/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/capacity/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14724 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11386 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/create_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/notification_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/notification_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/os_available.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.964583 softlayer-6.2.0/SoftLayer/CLI/virt/placementgroup/
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/placementgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/placementgroup/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/placementgroup/create_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/placementgroup/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/placementgroup/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/placementgroup/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/power.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/ready.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/reload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/virt/usage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.964583 softlayer-6.2.0/SoftLayer/CLI/vlan/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/vlan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/vlan/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/vlan/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/vlan/create_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/vlan/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/vlan/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/vlan/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.964583 softlayer-6.2.0/SoftLayer/CLI/vpn/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/vpn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.968583 softlayer-6.2.0/SoftLayer/CLI/vpn/ipsec/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/vpn/ipsec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/vpn/ipsec/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/vpn/ipsec/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/vpn/ipsec/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/vpn/ipsec/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/vpn/ipsec/order.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.968583 softlayer-6.2.0/SoftLayer/CLI/vpn/ipsec/subnet/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/vpn/ipsec/subnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/vpn/ipsec/subnet/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/vpn/ipsec/subnet/remove.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.968583 softlayer-6.2.0/SoftLayer/CLI/vpn/ipsec/translation/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/vpn/ipsec/translation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/vpn/ipsec/translation/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/vpn/ipsec/translation/remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/vpn/ipsec/translation/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/CLI/vpn/ipsec/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4173 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/decoration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.980584 softlayer-6.2.0/SoftLayer/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/BluePages_Search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44611 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Billing_Invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Billing_Invoice_Item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Billing_Item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Billing_Item_Cancellation_Request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Billing_Order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Billing_Order_Quote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Dns_Domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Dns_Domain_ResourceRecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Email_Subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Event_Log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14237 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Hardware_Server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Location_Datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Location_Group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Metric_Tracking_Object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Health_Check_Type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Routing_Method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Routing_Type.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Service.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Service_Group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_VirtualIpAddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_VirtualServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Bandwidth_Version1_Allotment.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Cache_Purge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Mapping_Path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Component_Firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Firewall_Update_Request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_LBaaS_HealthMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_LBaaS_L7Pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_LBaaS_Listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_LBaaS_LoadBalancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_LBaaS_Member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Message_Delivery_Email_Sendgrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Pod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_SecurityGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Service_Vpn_Overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10038 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Storage_Allowed_Host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Storage_Hub_Cleversafe_Account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Storage_Iscsi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Subnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Subnet_IpAddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Subnet_IpAddress_Global.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Subnet_Rwhois_Data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Vlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Vlan_Firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Notification_Occurrence_Event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9163 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Product_Order.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75145 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Product_Package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Product_Package_Preset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Provisioning_Hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Provisioning_Maintenance_Window.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Resource_Metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16122 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Scale_Group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Scale_Policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Security_Certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Security_Ssh_Key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Software_AccountLicense.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Software_Component_Password.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Ticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Ticket_Subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_User_Customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_User_Customer_CustomerPermission_Permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_User_Customer_Notification_Hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_User_Customer_Notification_Virtual_Guest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_User_Permission_Action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Virtual_DedicatedHost.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29326 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Virtual_Guest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Virtual_Guest_Block_Device_Template_Group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Virtual_Host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Virtual_PlacementGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Virtual_PlacementGroup_Rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Virtual_ReservedCapacityGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.984584 softlayer-6.2.0/SoftLayer/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14570 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/cdn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19234 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/dedicated_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/event_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13364 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60808 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10000 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15244 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/ipsec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/license.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13010 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35045 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/object_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33118 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/sshkey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26014 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42269 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9168 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/ticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20345 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62894 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/vs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/vs_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/managers/vs_placement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.988584 softlayer-6.2.0/SoftLayer/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/shell/cmd_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/shell/cmd_exit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/shell/cmd_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/shell/completer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/shell/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/shell/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.988584 softlayer-6.2.0/SoftLayer/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/testing/xmlrpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.988584 softlayer-6.2.0/SoftLayer/transports/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/transports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/transports/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/transports/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/transports/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/transports/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/transports/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/transports/xmlrpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15411 2024-05-01 22:33:50.000000 softlayer-6.2.0/SoftLayer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:54.000584 softlayer-6.2.0/SoftLayer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7998 2024-05-01 22:33:53.000000 softlayer-6.2.0/SoftLayer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22925 2024-05-01 22:33:53.000000 softlayer-6.2.0/SoftLayer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 22:33:53.000000 softlayer-6.2.0/SoftLayer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-01 22:33:53.000000 softlayer-6.2.0/SoftLayer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 22:33:53.000000 softlayer-6.2.0/SoftLayer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-01 22:33:53.000000 softlayer-6.2.0/SoftLayer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 22:33:53.000000 softlayer-6.2.0/SoftLayer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-01 22:33:54.000584 softlayer-6.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-01 22:33:50.000000 softlayer-6.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.908583 softlayer-6.2.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.988584 softlayer-6.2.0/tests/CLI/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/core_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/custom_types_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/environment_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/formatting_table_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15347 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/helper_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.992584 softlayer-6.2.0/tests/CLI/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9126 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/account_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11282 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/bandwidth_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43925 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/block_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12903 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/call_api_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/cdn_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/config_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17724 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/dedicatedhost_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11932 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/dns_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/email_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/event_log_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36599 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/file_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8769 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/firewall_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/globalip_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/image_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27405 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/ipsec_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/licenses_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15854 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/loadbal_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/nas_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/object_storage_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23416 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/order_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/report_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/search_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/security_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14341 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/securitygroup_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/sshkey_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/ssl_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/subnet_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/summary_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/tag_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15445 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/ticket_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20619 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/user_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15070 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/vlan_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:53.996584 softlayer-6.2.0/tests/CLI/modules/vs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/vs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/vs/vs_capacity_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33577 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/vs/vs_create_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/vs/vs_placement_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43881 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/CLI/modules/vs/vs_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:54.000584 softlayer-6.2.0/tests/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/account_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/bandwidth_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42152 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/block_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/cdn_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24093 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/dedicated_host_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/dns_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/email_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/event_log_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34792 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/file_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12808 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/firewall_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42426 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/hardware_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/image_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16589 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/ipsec_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9915 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/loadbal_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/metadata_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28050 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/network_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/object_storage_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40766 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/ordering_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/search_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/sshkey_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/ssl_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/storage_generic_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)   142912 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/storage_utils_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9155 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/tag_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/ticket_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15851 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/user_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:54.000584 softlayer-6.2.0/tests/managers/vs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/vs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/vs/vs_capacity_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/vs/vs_order_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/vs/vs_placement_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45298 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/vs/vs_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/managers/vs/vs_waiting_for_ready_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:54.000584 softlayer-6.2.0/tests/transports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/transports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/transports/debug_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11809 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/transports/rest_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/transports/transport_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14582 2024-05-01 22:33:50.000000 softlayer-6.2.0/tests/transports/xmlrpc_tests.py
```

### Comparing `SoftLayer-6.1.9/LICENSE` & `softlayer-6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/PKG-INFO` & `softlayer-6.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,52 @@
 Metadata-Version: 2.1
 Name: SoftLayer
-Version: 6.1.9
+Version: 6.2.0
 Summary: A library for SoftLayer's API
-Home-page: http://github.com/softlayer/softlayer-python
+Home-page: https://github.com/SoftLayer/softlayer-python
 Author: SoftLayer, Inc., an IBM Company
 Author-email: SLDNDeveloperRelations@wwpdl.vnet.ibm.com
 License: MIT
-Keywords: softlayer,cloud,slcli
+Keywords: softlayer,cloud,slcli,ibmcloud
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: prettytable>=2.5.0
 Requires-Dist: click>=8.0.4
 Requires-Dist: requests>=2.20.0
 Requires-Dist: prompt_toolkit>=2
 Requires-Dist: pygments>=2.0.0
 Requires-Dist: urllib3>=1.24
-Requires-Dist: rich==13.5.3
+Requires-Dist: rich==13.7.1
 
 SoftLayer API Python Client
 ===========================
 .. image:: https://github.com/softlayer/softlayer-python/workflows/Tests/badge.svg
     :target: https://github.com/softlayer/softlayer-python/actions?query=workflow%3ATests
-
 .. image:: https://github.com/softlayer/softlayer-python/workflows/documentation/badge.svg
     :target: https://github.com/softlayer/softlayer-python/actions?query=workflow%3Adocumentation
-
-.. image:: https://landscape.io/github/softlayer/softlayer-python/master/landscape.svg
-    :target: https://landscape.io/github/softlayer/softlayer-python/master
-
 .. image:: https://badge.fury.io/py/SoftLayer.svg
     :target: http://badge.fury.io/py/SoftLayer
-
 .. image:: https://coveralls.io/repos/github/softlayer/softlayer-python/badge.svg?branch=master
     :target: https://coveralls.io/github/softlayer/softlayer-python?branch=master
-
 .. image:: https://snapcraft.io//slcli/badge.svg
     :target: https://snapcraft.io/slcli
 
 
 This library provides a simple Python client to interact with `SoftLayer's
 XML-RPC API <https://softlayer.github.io/reference/softlayerapi>`_.
```

### Comparing `SoftLayer-6.1.9/README.rst` & `softlayer-6.2.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,17 @@
 SoftLayer API Python Client
 ===========================
 .. image:: https://github.com/softlayer/softlayer-python/workflows/Tests/badge.svg
     :target: https://github.com/softlayer/softlayer-python/actions?query=workflow%3ATests
-
 .. image:: https://github.com/softlayer/softlayer-python/workflows/documentation/badge.svg
     :target: https://github.com/softlayer/softlayer-python/actions?query=workflow%3Adocumentation
-
-.. image:: https://landscape.io/github/softlayer/softlayer-python/master/landscape.svg
-    :target: https://landscape.io/github/softlayer/softlayer-python/master
-
 .. image:: https://badge.fury.io/py/SoftLayer.svg
     :target: http://badge.fury.io/py/SoftLayer
-
 .. image:: https://coveralls.io/repos/github/softlayer/softlayer-python/badge.svg?branch=master
     :target: https://coveralls.io/github/softlayer/softlayer-python?branch=master
-
 .. image:: https://snapcraft.io//slcli/badge.svg
     :target: https://snapcraft.io/slcli
 
 
 This library provides a simple Python client to interact with `SoftLayer's
 XML-RPC API <https://softlayer.github.io/reference/softlayerapi>`_.
```

### Comparing `SoftLayer-6.1.9/SoftLayer/API.py` & `softlayer-6.2.0/SoftLayer/API.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,39 +3,41 @@
     ~~~~~~~~~~~~~
     SoftLayer API bindings
 
     :license: MIT, see LICENSE for more details.
 """
 # pylint: disable=invalid-name
 import time
-import warnings
 
+import concurrent.futures as cf
 import json
 import logging
+import math
 import requests
 
-
 from SoftLayer import auth as slauth
 from SoftLayer import config
 from SoftLayer import consts
 from SoftLayer import exceptions
 from SoftLayer import transports
 
 LOGGER = logging.getLogger(__name__)
 API_PUBLIC_ENDPOINT = consts.API_PUBLIC_ENDPOINT
 API_PRIVATE_ENDPOINT = consts.API_PRIVATE_ENDPOINT
 CONFIG_FILE = consts.CONFIG_FILE
 
 __all__ = [
     'create_client_from_env',
+    'employee_client',
     'Client',
     'BaseClient',
     'API_PUBLIC_ENDPOINT',
     'API_PRIVATE_ENDPOINT',
     'IAMClient',
+    'CertificateClient'
 ]
 
 VALID_CALL_ARGS = set((
     'id',
     'mask',
     'filter',
     'headers',
@@ -138,41 +140,120 @@
                 settings.get('username'),
                 settings.get('api_key'),
             )
 
     return BaseClient(auth=auth, transport=transport, config_file=config_file)
 
 
-def Client(**kwargs):
-    """Get a SoftLayer API Client using environmental settings.
-
-    Deprecated in favor of create_client_from_env()
+def employee_client(username=None,
+                    access_token=None,
+                    endpoint_url=None,
+                    timeout=None,
+                    auth=None,
+                    config_file=None,
+                    proxy=None,
+                    user_agent=None,
+                    transport=None,
+                    verify=True):
+    """Creates an INTERNAL SoftLayer API client using your environment.
+
+    Settings are loaded via keyword arguments, environemtal variables and config file.
+
+    :param username: your user ID
+    :param access_token: hash from SoftLayer_User_Employee::performExternalAuthentication(username, password, token)
+    :param password: password to use for employee authentication
+    :param endpoint_url: the API endpoint base URL you wish to connect to.
+        Set this to API_PRIVATE_ENDPOINT to connect via SoftLayer's private network.
+    :param proxy: proxy to be used to make API calls
+    :param integer timeout: timeout for API requests
+    :param auth: an object which responds to get_headers() to be inserted into the xml-rpc headers.
+        Example: `BasicAuthentication`
+    :param config_file: A path to a configuration file used to load settings
+    :param user_agent: an optional User Agent to report when making API
+        calls if you wish to bypass the packages built in User Agent string
+    :param transport: An object that's callable with this signature: transport(SoftLayer.transports.Request)
+    :param bool verify: decide to verify the server's SSL/TLS cert.
     """
-    warnings.warn("use SoftLayer.create_client_from_env() instead",
-                  DeprecationWarning)
+    settings = config.get_client_settings(username=username,
+                                          api_key=None,
+                                          endpoint_url=endpoint_url,
+                                          timeout=timeout,
+                                          proxy=proxy,
+                                          verify=None,
+                                          config_file=config_file)
+
+    url = settings.get('endpoint_url')
+    verify = settings.get('verify', True)
+
+    if 'internal' not in url:
+        raise exceptions.SoftLayerError(f"{url} does not look like an Internal Employee url.")
+
+    if transport is None:
+        if url is not None and '/rest' in url:
+            # If this looks like a rest endpoint, use the rest transport
+            transport = transports.RestTransport(
+                endpoint_url=settings.get('endpoint_url'),
+                proxy=settings.get('proxy'),
+                timeout=settings.get('timeout'),
+                user_agent=user_agent,
+                verify=verify,
+            )
+        else:
+            # Default the transport to use XMLRPC
+            transport = transports.XmlRpcTransport(
+                endpoint_url=settings.get('endpoint_url'),
+                proxy=settings.get('proxy'),
+                timeout=settings.get('timeout'),
+                user_agent=user_agent,
+                verify=verify,
+            )
+
+    if access_token is None:
+        access_token = settings.get('access_token')
+
+    user_id = settings.get('userid')
+
+    # Assume access_token is valid for now, user has logged in before at least.
+    if access_token and user_id:
+        auth = slauth.EmployeeAuthentication(user_id, access_token)
+        return EmployeeClient(auth=auth, transport=transport)
+    else:
+        # This is for logging in mostly.
+        LOGGER.info("No access_token or userid found in settings, creating a No Auth client for now.")
+        return EmployeeClient(auth=None, transport=transport)
+
+
+def Client(**kwargs):
+    """Get a SoftLayer API Client using environmental settings."""
     return create_client_from_env(**kwargs)
 
 
 class BaseClient(object):
     """Base SoftLayer API client.
 
     :param auth: auth driver that looks like SoftLayer.auth.AuthenticationBase
-    :param transport: An object that's callable with this signature:
-                      transport(SoftLayer.transports.Request)
+    :param transport: An object that's callable with this signature: transport(SoftLayer.transports.Request)
     """
-
     _prefix = "SoftLayer_"
+    auth: slauth.AuthenticationBase
 
     def __init__(self, auth=None, transport=None, config_file=None):
         if config_file is None:
             config_file = CONFIG_FILE
-        self.auth = auth
         self.config_file = config_file
         self.settings = config.get_config(self.config_file)
+        self.__setAuth(auth)
+        self.__setTransport(transport)
 
+    def __setAuth(self, auth=None):
+        """Prepares the authentication property"""
+        self.auth = auth
+
+    def __setTransport(self, transport=None):
+        """Prepares the transport property"""
         if transport is None:
             url = self.settings['softlayer'].get('endpoint_url')
             if url is not None and '/rest' in url:
                 # If this looks like a rest endpoint, use the rest transport
                 transport = transports.RestTransport(
                     endpoint_url=url,
                     proxy=self.settings['softlayer'].get('proxy'),
@@ -189,17 +270,15 @@
                     timeout=int(self.settings['softlayer'].getfloat('timeout', 0)),
                     user_agent=consts.USER_AGENT,
                     verify=self.settings['softlayer'].getboolean('verify'),
                 )
 
         self.transport = transport
 
-    def authenticate_with_password(self, username, password,
-                                   security_question_id=None,
-                                   security_question_answer=None):
+    def authenticate_with_password(self, username, password, security_question_id=None, security_question_answer=None):
         """Performs Username/Password Authentication
 
         :param string username: your SoftLayer username
         :param string password: your SoftLayer password
         :param int security_question_id: The security question id to answer
         :param string security_question_answer: The answer to the security question
 
@@ -254,16 +333,15 @@
         if kwargs.pop('iter', False):
             # Most of the codebase assumes a non-generator will be returned, so casting to list
             # keeps those sections working
             return list(self.iter_call(service, method, *args, **kwargs))
 
         invalid_kwargs = set(kwargs.keys()) - VALID_CALL_ARGS
         if invalid_kwargs:
-            raise TypeError(
-                'Invalid keyword arguments: %s' % ','.join(invalid_kwargs))
+            raise TypeError('Invalid keyword arguments: %s' % ','.join(invalid_kwargs))
 
         prefixes = (self._prefix, 'BluePages_Search', 'IntegratedOfferingTeam_Region')
         if self._prefix and not service.startswith(prefixes):
             service = self._prefix + service
 
         http_headers = {'Accept': '*/*'}
 
@@ -281,25 +359,19 @@
         request.args = args
         request.transport_headers = http_headers
         request.identifier = kwargs.get('id')
         request.mask = kwargs.get('mask')
         request.filter = kwargs.get('filter')
         request.limit = kwargs.get('limit')
         request.offset = kwargs.get('offset')
+        request.url = self.settings['softlayer'].get('endpoint_url')
         if kwargs.get('verify') is not None:
             request.verify = kwargs.get('verify')
 
         if self.auth:
-            extra_headers = self.auth.get_headers()
-            if extra_headers:
-                warnings.warn("auth.get_headers() is deprecated and will be "
-                              "removed in the next major version",
-                              DeprecationWarning)
-                request.headers.update(extra_headers)
-
             request = self.auth.get_request(request)
 
         request.headers.update(kwargs.get('headers', {}))
         return self.transport(request)
 
     __call__ = call
 
@@ -348,23 +420,84 @@
                 keep_looping = False
             # Got all the needed items
             if result_count >= results.total_count:
                 keep_looping = False
 
             offset += limit
 
+    def cf_call(self, service, method, *args, **kwargs):
+        """Uses threads to iterate through API calls.
+
+        :param service: the name of the SoftLayer API service
+        :param method: the method to call on the service
+        :param integer limit: result size for each API call (defaults to 100)
+        :param \\*args: same optional arguments that ``Service.call`` takes
+        :param \\*\\*kwargs: same optional keyword arguments that ``Service.call`` takes
+        """
+        limit = kwargs.pop('limit', 100)
+        offset = kwargs.pop('offset', 0)
+
+        if limit <= 0:
+            raise AttributeError("Limit size should be greater than zero.")
+        # This initial API call is to determine how many API calls we need to make after this first one.
+        first_call = self.call(service, method, offset=offset, limit=limit, *args, **kwargs)
+
+        # This was not a list result, just return it.
+        if not isinstance(first_call, transports.SoftLayerListResult):
+            return first_call
+        # How many more API calls we have to make
+        api_calls = math.ceil((first_call.total_count - limit) / limit)
+
+        def this_api(offset):
+            """Used to easily call executor.map() on this fuction"""
+            return self.call(service, method, offset=offset, limit=limit, *args, **kwargs)
+
+        with cf.ThreadPoolExecutor(max_workers=10) as executor:
+            future_results = {}
+            offset_map = [x * limit for x in range(1, api_calls)]
+            future_results = list(executor.map(this_api, offset_map))
+        # Append the results in the order they were called
+        for call_result in future_results:
+            first_call = first_call + call_result
+        return first_call
+
     def __repr__(self):
         return "Client(transport=%r, auth=%r)" % (self.transport, self.auth)
 
     __str__ = __repr__
 
     def __len__(self):
         return 0
 
 
+class CertificateClient(BaseClient):
+    """Client that works with a X509 Certificate for authentication.
+
+    Will read the certificate file from the config file (~/.softlayer usually).
+    > auth_cert = /path/to/authentication/cert.pm
+    > server_cert = /path/to/CAcert.pem
+    Set auth to a SoftLayer.auth.Authentication class to manually set authentication
+    """
+
+    def __init__(self, auth=None, transport=None, config_file=None):
+        BaseClient.__init__(self, auth, transport, config_file)
+        self.__setAuth(auth)
+
+    def __setAuth(self, auth=None):
+        """Prepares the authentication property"""
+        if auth is None:
+            auth_cert = self.settings['softlayer'].get('auth_cert')
+            serv_cert = self.settings['softlayer'].get('server_cert', None)
+            auth = slauth.X509Authentication(auth_cert, serv_cert)
+        self.auth = auth
+
+    def __repr__(self):
+        return "CertificateClient(transport=%r, auth=%r)" % (self.transport, self.auth)
+
+
 class IAMClient(BaseClient):
     """IBM ID Client for using IAM authentication
 
     :param auth: auth driver that looks like SoftLayer.auth.AuthenticationBase
     :param transport: An object that's callable with this signature: transport(SoftLayer.transports.Request)
     """
 
@@ -541,14 +674,102 @@
             else:
                 raise ex
 
     def __repr__(self):
         return "IAMClient(transport=%r, auth=%r)" % (self.transport, self.auth)
 
 
+class EmployeeClient(BaseClient):
+    """Internal SoftLayer Client
+
+    :param auth: auth driver that looks like SoftLayer.auth.AuthenticationBase
+    :param transport: An object that's callable with this signature: transport(SoftLayer.transports.Request)
+    """
+
+    def __init__(self, auth=None, transport=None, config_file=None, account_id=None):
+        BaseClient.__init__(self, auth, transport, config_file)
+        self.account_id = account_id
+
+    def authenticate_with_internal(self, username, password, security_token=None):
+        """Performs internal authentication
+
+        :param string username: your softlayer username
+        :param string password: your softlayer password
+        :param int security_token: your 2FA token, prompt if None
+        """
+
+        self.auth = None
+        if security_token is None:
+            security_token = input("Enter your 2FA Token now: ")
+            if len(security_token) != 6:
+                raise exceptions.SoftLayerAPIError("Invalid security token: {}".format(security_token))
+
+        auth_result = self.call('SoftLayer_User_Employee', 'performExternalAuthentication',
+                                username, password, security_token)
+
+        self.settings['softlayer']['access_token'] = auth_result['hash']
+        self.settings['softlayer']['userid'] = str(auth_result['userId'])
+        # self.settings['softlayer']['refresh_token'] = tokens['refresh_token']
+
+        config.write_config(self.settings, self.config_file)
+        self.auth = slauth.EmployeeAuthentication(auth_result['userId'], auth_result['hash'])
+
+        return auth_result
+
+    def authenticate_with_hash(self, userId, access_token):
+        """Authenticates to the Internal SL API with an employee userid + token
+
+        :param string userId: Employee UserId
+        :param string access_token: Employee Hash Token
+        """
+        self.auth = slauth.EmployeeAuthentication(userId, access_token)
+
+    def refresh_token(self, userId, auth_token):
+        """Refreshes the login token"""
+
+        # Go directly to base client, to avoid infite loop if the token is super expired.
+        auth_result = BaseClient.call(self, 'SoftLayer_User_Employee', 'refreshEncryptedToken', auth_token, id=userId)
+        if len(auth_result) > 1:
+            for returned_data in auth_result:
+                # Access tokens should be 188 characters, but just incase its longer or something.
+                if len(returned_data) > 180:
+                    self.settings['softlayer']['access_token'] = returned_data
+        else:
+            message = "Excepted 2 properties from refreshEncryptedToken, got {}|".format(auth_result)
+            raise exceptions.SoftLayerAPIError(message)
+
+        config.write_config(self.settings, self.config_file)
+        self.auth = slauth.EmployeeAuthentication(userId, auth_result[0])
+        return auth_result
+
+    def call(self, service, method, *args, **kwargs):
+        """Handles refreshing Employee tokens in case of a HTTP 401 error"""
+        if (service == 'SoftLayer_Account' or service == 'Account') and not kwargs.get('id'):
+            if not self.account_id:
+                raise exceptions.SoftLayerError("SoftLayer_Account service requires an ID")
+            kwargs['id'] = self.account_id
+
+        try:
+            return BaseClient.call(self, service, method, *args, **kwargs)
+        except exceptions.SoftLayerAPIError as ex:
+            if ex.faultCode == "SoftLayer_Exception_EncryptedToken_Expired":
+                userId = self.settings['softlayer'].get('userid')
+                access_token = self.settings['softlayer'].get('access_token')
+                LOGGER.warning("Token has expired, trying to refresh. %s", ex.faultString)
+                self.refresh_token(userId, access_token)
+                # Try the Call again this time....
+                return BaseClient.call(self, service, method, *args, **kwargs)
+
+            else:
+                raise ex
+
+    def __repr__(self):
+        return "EmployeeClient(transport=%r, auth=%r)" % (self.transport, self.auth)
+
+
 class Service(object):
     """A SoftLayer Service.
 
         :param client: A SoftLayer.API.Client instance
         :param name str: The service name
 
     """
```

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/account/billing_items.py` & `softlayer-6.2.0/SoftLayer/CLI/account/billing_items.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/account/cancel_item.py` & `softlayer-6.2.0/SoftLayer/CLI/account/cancel_item.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/account/event_detail.py` & `softlayer-6.2.0/SoftLayer/CLI/account/event_detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/account/events.py` & `softlayer-6.2.0/SoftLayer/CLI/account/events.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/account/hook_create.py` & `softlayer-6.2.0/SoftLayer/CLI/account/hook_create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/account/hook_delete.py` & `softlayer-6.2.0/SoftLayer/CLI/account/hook_delete.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/account/hooks.py` & `softlayer-6.2.0/SoftLayer/CLI/account/hooks.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/account/invoice_detail.py` & `softlayer-6.2.0/SoftLayer/CLI/account/invoice_detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/account/invoices.py` & `softlayer-6.2.0/SoftLayer/CLI/account/invoices.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/account/item_detail.py` & `softlayer-6.2.0/SoftLayer/CLI/account/item_detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/account/licenses.py` & `softlayer-6.2.0/SoftLayer/CLI/account/licenses.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/account/orders.py` & `softlayer-6.2.0/SoftLayer/CLI/account/orders.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/account/summary.py` & `softlayer-6.2.0/SoftLayer/CLI/account/summary.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/bandwidth/pools.py` & `softlayer-6.2.0/SoftLayer/CLI/bandwidth/pools.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/bandwidth/pools_create.py` & `softlayer-6.2.0/SoftLayer/CLI/bandwidth/pools_create.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,18 +21,19 @@
     "FRA": "FRA"
 }
 
 regions = ['SJC/DAL/WDC/TOR/MON', 'AMS/LON/MAD/PAR', 'SNG/HKG/OSA/TOK', 'SYD', 'MEX', 'SAO', 'CHE', 'MIL', 'SEO', 'FRA']
 
 
 def check_region_param(ctx, param, value):  # pylint: disable=unused-argument
-    """Check if provided region is region group or part of region"""
+    """Check if provided region is region group or part of region
 
-    # :params string value: Region or Region-Groups
-    # return string Region-Groups
+    :params string value: Region or Region-Groups
+    return string Region-Groups
+    """
 
     region_group = None
     for key in location_groups:
         if value in key or value is key:
             region_group = key
 
     if region_group:
@@ -49,18 +50,19 @@
               help=f"Choose Region/Region-Group {regions}", callback=check_region_param)
 @click.help_option('--help', '-h')
 @environment.pass_env
 def cli(env, name, region):
     """Create bandwidth pool.
 
     Region can be the full zone name 'SJC/DAL/WDC/TOR/MON', or just a single datacenter like 'SJC'.
+
     Example::
         slcli bandwidth pool-create --name testPool --region DAL
         slcli bandwidth pool-create --name testPool --region SJC/DAL/WDC/TOR/MON
-        """
+    """
 
     manager = BandwidthManager(env.client)
     locations = manager.get_location_group()
     id_location_group = get_id_from_location_group(locations, location_groups[region])
     created_pool = manager.create_pool(name, id_location_group)
 
     table = formatting.KeyValueTable(['Name', 'Value'])
```

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/bandwidth/pools_delete.py` & `softlayer-6.2.0/SoftLayer/CLI/bandwidth/pools_delete.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/bandwidth/pools_detail.py` & `softlayer-6.2.0/SoftLayer/CLI/bandwidth/pools_detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/bandwidth/pools_edit.py` & `softlayer-6.2.0/SoftLayer/CLI/bandwidth/pools_edit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/bandwidth/summary.py` & `softlayer-6.2.0/SoftLayer/CLI/bandwidth/summary.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/access/authorize.py` & `softlayer-6.2.0/SoftLayer/CLI/block/access/authorize.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/access/list.py` & `softlayer-6.2.0/SoftLayer/CLI/block/access/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/access/password.py` & `softlayer-6.2.0/SoftLayer/CLI/block/access/password.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/access/revoke.py` & `softlayer-6.2.0/SoftLayer/CLI/block/access/revoke.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/cancel.py` & `softlayer-6.2.0/SoftLayer/CLI/block/cancel.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/convert.py` & `softlayer-6.2.0/SoftLayer/CLI/block/convert.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/count.py` & `softlayer-6.2.0/SoftLayer/CLI/block/count.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/detail.py` & `softlayer-6.2.0/SoftLayer/CLI/block/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/duplicate.py` & `softlayer-6.2.0/SoftLayer/CLI/block/duplicate.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/duplicate_convert_status.py` & `softlayer-6.2.0/SoftLayer/CLI/block/duplicate_convert_status.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/limit.py` & `softlayer-6.2.0/SoftLayer/CLI/block/limit.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 @environment.pass_env
 def cli(env, sortby, datacenter):
     """List number of block storage volumes limit per datacenter.
 
     Example::
         slcli block volume-limits
         This command lists the storage limits per datacenter for this account.
-"""
+    """
 
     block_manager = SoftLayer.BlockStorageManager(env.client)
     block_volumes = block_manager.list_block_volume_limit()
 
     table = formatting.KeyValueTable(DEFAULT_COLUMNS)
     table.sortby = sortby
```

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/list.py` & `softlayer-6.2.0/SoftLayer/CLI/block/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/lun.py` & `softlayer-6.2.0/SoftLayer/CLI/block/lun.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/modify.py` & `softlayer-6.2.0/SoftLayer/CLI/file/modify.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,59 +1,60 @@
-"""Modify an existing block storage volume."""
+"""Modify an existing file storage volume."""
 # :license: MIT, see LICENSE for more details.
 
 import click
 import SoftLayer
 from SoftLayer.CLI import environment
 from SoftLayer.CLI import exceptions
+from SoftLayer.CLI import formatting
 
 
 CONTEXT_SETTINGS = {'token_normalize_func': lambda x: x.upper()}
 
 
 @click.command(cls=SoftLayer.CLI.command.SLCommand, context_settings=CONTEXT_SETTINGS)
 @click.argument('volume-id')
 @click.option('--new-size', '-c',
               type=int,
-              help='New Size of block volume in GB. ***If no size is given, the original size of volume is used.***\n'
+              help='New Size of file volume in GB. ***If no size is given, the original size of volume is used.***\n'
                    'Potential Sizes: [20, 40, 80, 100, 250, 500, 1000, 2000, 4000, 8000, 12000]\n'
                    'Minimum: [the original size of the volume]')
 @click.option('--new-iops', '-i',
               type=int,
               help='Performance Storage IOPS, between 100 and 6000 in multiples of 100 [only for performance volumes] '
-                   '***If no IOPS value is specified, the original IOPS value of the volume will be used.***\n'
-                   'Requirements: [If original IOPS/GB for the volume is less than 0.3, new IOPS/GB must also be '
-                   'less than 0.3. If original IOPS/GB for the volume is greater than or equal to 0.3, new IOPS/GB '
-                   'for the volume must also be greater than or equal to 0.3.]')
+                   '***If no IOPS value is specified, the original IOPS value of the volume will be used.***')
 @click.option('--new-tier', '-t',
               help='Endurance Storage Tier (IOPS per GB) [only for endurance volumes] '
-                   '***If no tier is specified, the original tier of the volume will be used.***\n'
-                   'Requirements: [If original IOPS/GB for the volume is 0.25, new IOPS/GB for the volume must also '
-                   'be 0.25. If original IOPS/GB for the volume is greater than 0.25, new IOPS/GB for the volume '
-                   'must also be greater than 0.25.]',
+                   '***If no tier is specified, the original tier of the volume will be used.***',
               type=click.Choice(['0.25', '2', '4', '10']))
+@click.option('--force',  default=False, is_flag=True, help="Force modify")
 @environment.pass_env
-def cli(env, volume_id, new_size, new_iops, new_tier):
-    """Modify an existing block storage volume.
+def cli(env, volume_id, new_size, new_iops, new_tier, force):
+    """Modify an existing file storage volume.
+
+    Valid size and iops options can be found here:
+        https://cloud.ibm.com/docs/FileStorage/index.html#provisioning-considerations
+        https://cloud.ibm.com/docs/FileStorage?topic=FileStorage-orderingFileStorage&interface=cli
 
     Example::
-        slcli block volume-modify 12345678 --new-size 1000 --new-iops 4000
-        This command modify a volume 12345678 with size is 1000GB, IOPS is 4000.
 
-        slcli block volume-modify 12345678 --new-size 500 --new-tier 4
-        This command modify a volume 12345678 with size is 500GB, tier level is 4 IOPS per GB.
-"""
+            slcli file volume-modify 12345678 --new-size 1000 --new-iops 400
+    """
+    if not force:
+        if not (env.skip_confirmations or
+                formatting.confirm("This action will incur charges on your account. Continue?")):
+            raise exceptions.CLIAbort('Aborted')
 
-    block_manager = SoftLayer.BlockStorageManager(env.client)
+    file_manager = SoftLayer.FileStorageManager(env.client)
 
     if new_tier is not None:
         new_tier = float(new_tier)
 
     try:
-        order = block_manager.order_modified_volume(
+        order = file_manager.order_modified_volume(
             volume_id,
             new_size=new_size,
             new_iops=new_iops,
             new_tier_level=new_tier,
         )
     except ValueError as ex:
         raise exceptions.ArgumentError(str(ex))
```

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/object_list.py` & `softlayer-6.2.0/SoftLayer/CLI/block/object_list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/object_storage_detail.py` & `softlayer-6.2.0/SoftLayer/CLI/block/object_storage_detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/object_storage_permission.py` & `softlayer-6.2.0/SoftLayer/CLI/block/object_storage_permission.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/options.py` & `softlayer-6.2.0/SoftLayer/CLI/block/options.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/order.py` & `softlayer-6.2.0/SoftLayer/CLI/block/order.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/refresh.py` & `softlayer-6.2.0/SoftLayer/CLI/block/refresh.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/replication/disaster_recovery_failover.py` & `softlayer-6.2.0/SoftLayer/CLI/block/replication/disaster_recovery_failover.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/replication/failback.py` & `softlayer-6.2.0/SoftLayer/CLI/block/replication/failback.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/replication/failover.py` & `softlayer-6.2.0/SoftLayer/CLI/block/replication/failover.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/replication/locations.py` & `softlayer-6.2.0/SoftLayer/CLI/block/replication/locations.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/replication/order.py` & `softlayer-6.2.0/SoftLayer/CLI/block/replication/order.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/replication/partners.py` & `softlayer-6.2.0/SoftLayer/CLI/block/replication/partners.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/set_note.py` & `softlayer-6.2.0/SoftLayer/CLI/block/set_note.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/snapshot/cancel.py` & `softlayer-6.2.0/SoftLayer/CLI/block/snapshot/cancel.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/snapshot/create.py` & `softlayer-6.2.0/SoftLayer/CLI/block/snapshot/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/snapshot/delete.py` & `softlayer-6.2.0/SoftLayer/CLI/block/snapshot/delete.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/snapshot/disable.py` & `softlayer-6.2.0/SoftLayer/CLI/block/snapshot/disable.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/snapshot/enable.py` & `softlayer-6.2.0/SoftLayer/CLI/block/snapshot/enable.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/snapshot/get_notify_status.py` & `softlayer-6.2.0/SoftLayer/CLI/block/snapshot/get_notify_status.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/snapshot/list.py` & `softlayer-6.2.0/SoftLayer/CLI/block/snapshot/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/snapshot/order.py` & `softlayer-6.2.0/SoftLayer/CLI/block/snapshot/order.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/snapshot/restore.py` & `softlayer-6.2.0/SoftLayer/CLI/block/snapshot/restore.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/snapshot/schedule_list.py` & `softlayer-6.2.0/SoftLayer/CLI/block/snapshot/schedule_list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/snapshot/set_notify_status.py` & `softlayer-6.2.0/SoftLayer/CLI/block/snapshot/set_notify_status.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/subnets/assign.py` & `softlayer-6.2.0/SoftLayer/CLI/block/subnets/assign.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/subnets/list.py` & `softlayer-6.2.0/SoftLayer/CLI/block/subnets/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/block/subnets/remove.py` & `softlayer-6.2.0/SoftLayer/CLI/block/subnets/remove.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/call_api.py` & `softlayer-6.2.0/SoftLayer/CLI/call_api.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/cdn/create.py` & `softlayer-6.2.0/SoftLayer/CLI/cdn/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/cdn/detail.py` & `softlayer-6.2.0/SoftLayer/CLI/cdn/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/cdn/edit.py` & `softlayer-6.2.0/SoftLayer/CLI/cdn/edit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/cdn/list.py` & `softlayer-6.2.0/SoftLayer/CLI/cdn/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/cdn/origin_add.py` & `softlayer-6.2.0/SoftLayer/CLI/cdn/origin_add.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/cdn/origin_list.py` & `softlayer-6.2.0/SoftLayer/CLI/cdn/origin_list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/cdn/origin_remove.py` & `softlayer-6.2.0/SoftLayer/CLI/cdn/origin_remove.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/cdn/purge.py` & `softlayer-6.2.0/SoftLayer/CLI/cdn/purge.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/columns.py` & `softlayer-6.2.0/SoftLayer/CLI/columns.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/command.py` & `softlayer-6.2.0/SoftLayer/CLI/command.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,17 @@
     Defined in SoftLayer\\utils.py console_color_themes()
     """
     highlights = [
         r"(?P<switch>^\-\w)",  # single options like -v
         r"(?P<option>\-\-[\w\-]+)",  # long options like --verbose
         r"(?P<default_option>\[[^\]]+\])",  # anything between [], usually default options
         r"(?P<option_choices>Choices: )",
+        r"(?P<example_block>Example::)",
+        r"(?P<url>(file|https|http|ws|wss)://[-0-9a-zA-Z$_+!`(),.?/;:&=%#~]*)"
+        r"(?P<args_keyword>^[A-Z]+$)",
     ]
 
 
 class CommandLoader(click.MultiCommand):
     """Loads module for click."""
 
     def __init__(self, *path, **attrs):
@@ -86,15 +89,15 @@
         text = self.help if self.help is not None else ""
 
         if self.deprecated:
             text = f"(Deprecated) {text}"
 
         if text:
             text = inspect.cleandoc(text).partition("\f")[0]
-        self.console.print(f"\n\t{text}\n")
+        self.console.print(f"\n\t{text}\n", highlight=True)
 
     def format_epilog(self, ctx: click.Context, formatter: click.formatting.HelpFormatter) -> None:
         """Writes the epilog if it exists, then prints out any sub-commands if they exist."""
         if self.epilog:
             epilog = inspect.cleandoc(self.epilog)
             epilog = epilog.replace("\n", " ")
             self.console.print(epilog)
@@ -173,67 +176,78 @@
         self.ensure_env(ctx)
         pieces = self.collect_usage_pieces(ctx)
         for index, piece in enumerate(pieces):
             if piece == "[OPTIONS]":
                 pieces[index] = "[options][OPTIONS][/]"
             elif piece == "COMMAND [ARGS]...":
                 pieces[index] = "[command]COMMAND[/] [args][ARGS][/] ..."
+            else:
+                pieces[index] = f"[args_keyword]{piece}[/]"
 
         self.console.print(f"Usage: [path]{ctx.command_path}[/] {' '.join(pieces)}")
 
     def format_help_text(self, ctx: click.Context, formatter: click.formatting.HelpFormatter) -> None:
         """Writes the help text"""
         text = self.help if self.help is not None else ""
 
         if self.deprecated:
             text = f"(Deprecated) {text}"
 
         if text:
-            text = inspect.cleandoc(text)
+            text = f"\n\t{inspect.cleandoc(text)}\n"
 
-        self.console.print(f"\n\t{text}\n", highlight=False)
+        # Can't use F-string here because it messes with highlights
+        self.console.print(self.highlighter(text))
 
     def format_epilog(self, ctx: click.Context, formatter: click.formatting.HelpFormatter) -> None:
         """Writes the epilog if it exists, then prints out any sub-commands if they exist."""
         if self.epilog:
             epilog = inspect.cleandoc(self.epilog)
             epilog = epilog.replace("\n", " ")
             self.console.print(epilog)
 
     def format_options(self, ctx, formatter):
         """Prints out the options in a table format"""
 
-        # NEXT support binary options --yes/--no
-        # NEXT SUPPORT color for IDENTIFIER and such
         options_table = Table(highlight=True, box=box.SQUARE, show_header=False)
 
         for param in self.get_params(ctx):
+            # useful for showing whats in a param
+            # print(param.to_info_dict())
+
+            # Set Arguments to all uppercase
+            if param.param_type_name == 'argument':
+                param.opts[0] = param.opts[0].upper()
+
+            # This option has a short (-v) and long (--verbose) options
             if len(param.opts) == 2:
                 opt1 = self.highlighter(param.opts[1])
                 opt2 = self.highlighter(param.opts[0])
             else:
                 opt2 = self.highlighter(param.opts[0])
+                # Needs to be the Text() type because rich.Text doesn't mesh with string
                 opt1 = Text("")
 
             # Ensures the short option is always in opt1.
             if len(opt2) == 2:
                 opt1, opt2 = opt2, opt1
 
             if param.metavar:
                 opt2 += Text(f" {param.metavar}", style="bold yellow")
 
-            options = Text(" ".join(reversed(param.opts)))
+            # secondary_opts are usually for flags --enable/--disable
+            if len(param.secondary_opts) == 1:
+                opt2 += Text("|") + self.highlighter(param.secondary_opts[0])
+
             help_record = param.get_help_record(ctx)
             help_message = ""
             if help_record:
-                help_message = param.get_help_record(ctx)[-1]
+                help_message = Text(param.get_help_record(ctx)[-1])
 
             # Add Click choices to help message
             if isinstance(param.type, click.Choice):
                 choices = ", ".join(param.type.choices)
                 help_message += f" Choices: {choices}"
 
-            if param.metavar:
-                options += f" {param.metavar}"
             options_table.add_row(opt1, opt2, self.highlighter(help_message))
 
         self.console.print(options_table)
```

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/config/__init__.py` & `softlayer-6.2.0/SoftLayer/CLI/config/__init__.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/config/setup.py` & `softlayer-6.2.0/SoftLayer/CLI/config/setup.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/core.py` & `softlayer-6.2.0/SoftLayer/CLI/core.py`

 * *Files 7% similar despite different names*

```diff
@@ -70,73 +70,73 @@
 
 
 @click.group(help="SoftLayer Command-line Client",
              epilog="""To use most commands your SoftLayer username and api_key need to be configured.
 The easiest way to do that is to use: 'slcli setup'""",
              cls=CommandLoader,
              context_settings=CONTEXT_SETTINGS)
-@click.option('--format',
-              default=DEFAULT_FORMAT,
-              show_default=True,
+@click.option('--format', default=DEFAULT_FORMAT, show_default=True,
               help="Output format",
               type=click.Choice(VALID_FORMATS))
-@click.option('-C', '--config',
-              required=False,
+@click.option('-C', '--config', required=False, show_default=True,
               default=click.get_app_dir('softlayer', force_posix=True),
-              show_default=True,
               help="Config file location",
               type=click.Path(resolve_path=True))
 @click.option('--verbose', '-v',
               help="Sets the debug noise level, specify multiple times for more verbosity.",
               type=click.IntRange(0, 3, clamp=True),
               count=True)
-@click.option('--proxy',
-              required=False,
+@click.option('--proxy', required=False,
               help="HTTPS or HTTP proxy to be use to make API calls")
-@click.option('--really / --not-really', '-y',
-              is_flag=True,
-              required=False,
+@click.option('--really / --not-really', '-y', is_flag=True, required=False,
               help="Confirm all prompt actions")
-@click.option('--demo / --no-demo',
-              is_flag=True,
-              required=False,
+@click.option('--demo / --no-demo', is_flag=True, required=False,
               help="Use demo data instead of actually making API calls")
 @click.option('--version', is_flag=True, expose_value=False, is_eager=True, callback=get_version_message,
               help="Show version information.",  allow_from_autoenv=False,)
+@click.option('--account', '-a', help="Account Id, only needed for some API calls.")
+@click.option('--internal', '-i', is_flag=True, required=False,
+              help="Use the Employee Client instead of the Customer Client.")
 @environment.pass_env
 def cli(env,
         format='table',
         config=None,
         verbose=0,
         proxy=None,
         really=False,
         demo=False,
+        account=None,
+        internal=False,
         **kwargs):
     """Main click CLI entry-point."""
 
     # Populate environment with client and set it as the context object
     env.skip_confirmations = really
     env.config_file = config
     env.format = format
     env.set_env_theme(config_file=config)
-    env.ensure_client(config_file=config, is_demo=demo, proxy=proxy)
+    if internal:
+        env.ensure_emp_client(config_file=config, is_demo=demo, proxy=proxy)
+    else:
+        env.ensure_client(config_file=config, is_demo=demo, proxy=proxy)
     env.vars['_start'] = time.time()
     logger = logging.getLogger()
 
     if demo is False:
         logger.addHandler(logging.StreamHandler())
     else:
         # This section is for running CLI tests.
         logging.getLogger("urllib3").setLevel(logging.WARNING)
         logger.addHandler(logging.NullHandler())
 
     logger.setLevel(DEBUG_LOGGING_MAP.get(verbose, logging.DEBUG))
     env.vars['_timings'] = SoftLayer.DebugTransport(env.client.transport)
     env.vars['verbose'] = verbose
     env.client.transport = env.vars['_timings']
+    env.client.account_id = account
 
 
 @cli.result_callback()
 @environment.pass_env
 def output_diagnostics(env, result, verbose=0, **kwargs):
     """Output diagnostic information."""
```

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/custom_types.py` & `softlayer-6.2.0/SoftLayer/CLI/custom_types.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/dedicatedhost/cancel.py` & `softlayer-6.2.0/SoftLayer/CLI/dedicatedhost/cancel.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/dedicatedhost/cancel_guests.py` & `softlayer-6.2.0/SoftLayer/CLI/dedicatedhost/cancel_guests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/dedicatedhost/create.py` & `softlayer-6.2.0/SoftLayer/CLI/dedicatedhost/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/dedicatedhost/create_options.py` & `softlayer-6.2.0/SoftLayer/CLI/dedicatedhost/create_options.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/dedicatedhost/detail.py` & `softlayer-6.2.0/SoftLayer/CLI/dedicatedhost/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/dedicatedhost/list.py` & `softlayer-6.2.0/SoftLayer/CLI/dedicatedhost/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/dedicatedhost/list_guests.py` & `softlayer-6.2.0/SoftLayer/CLI/dedicatedhost/list_guests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/dns/record_add.py` & `softlayer-6.2.0/SoftLayer/CLI/dns/record_add.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/dns/record_edit.py` & `softlayer-6.2.0/SoftLayer/CLI/dns/record_edit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/dns/record_list.py` & `softlayer-6.2.0/SoftLayer/CLI/dns/record_list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/dns/record_remove.py` & `softlayer-6.2.0/SoftLayer/CLI/dns/record_remove.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/dns/zone_delete.py` & `softlayer-6.2.0/SoftLayer/CLI/dns/zone_delete.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/dns/zone_import.py` & `softlayer-6.2.0/SoftLayer/CLI/dns/zone_import.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/dns/zone_list.py` & `softlayer-6.2.0/SoftLayer/CLI/dns/zone_list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/dns/zone_print.py` & `softlayer-6.2.0/SoftLayer/CLI/dns/zone_print.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/email/detail.py` & `softlayer-6.2.0/SoftLayer/CLI/email/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/email/edit.py` & `softlayer-6.2.0/SoftLayer/CLI/email/edit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/email/list.py` & `softlayer-6.2.0/SoftLayer/CLI/email/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/environment.py` & `softlayer-6.2.0/SoftLayer/CLI/environment.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,28 +8,25 @@
 import configparser
 import os
 
 import importlib
 from json.decoder import JSONDecodeError
 
 import click
-import pkg_resources
+
 from rich.console import Console
 from rich.syntax import Syntax
 
 import SoftLayer
 from SoftLayer.CLI import formatting
 from SoftLayer.CLI import routes
 from SoftLayer import utils
 
 # pylint: disable=too-many-instance-attributes, invalid-name
 
-# Calling pkg_resources.iter_entry_points shows a false-positive
-# pylint: disable=no-member
-
 
 class Environment(object):
     """Provides access to the current CLI environment."""
 
     def __init__(self):
         # {'path:to:command': ModuleLoader()}
         # {'vs:list': ModuleLoader()}
@@ -161,61 +158,55 @@
     def load(self):
         """Loads all modules."""
         if self._modules_loaded is True:
             return
 
         self.load_modules_from_python(routes.ALL_ROUTES)
         self.aliases.update(routes.ALL_ALIASES)
-        self._load_modules_from_entry_points('softlayer.cli')
-
         self._modules_loaded = True
 
     def load_modules_from_python(self, route_list):
         """Load modules from the native python source."""
         for name, modpath in route_list:
             if ':' in modpath:
                 path, attr = modpath.split(':', 1)
             else:
                 path, attr = modpath, None
             self.commands[name] = ModuleLoader(path, attr=attr)
 
-    def _load_modules_from_entry_points(self, entry_point_group):
-        """Load modules from the entry_points (slower).
-
-        Entry points can be used to add new commands to the CLI.
-
-        Usage:
-
-            entry_points={'softlayer.cli': ['new-cmd = mymodule.new_cmd.cli']}
+    def ensure_client(self, config_file=None, is_demo=False, proxy=None):
+        """Create a new SLAPI client to the environment.
 
+        This will be a no-op if there is already a client in this environment.
         """
-        for obj in pkg_resources.iter_entry_points(group=entry_point_group,
-                                                   name=None):
-            self.commands[obj.name] = obj
+        if self.client is not None:
+            return
 
-    def ensure_client(self, config_file=None, is_demo=False, proxy=None):
+        # Environment can be passed in explicitly. This is used for testing
+        if is_demo:
+            client = SoftLayer.BaseClient(transport=SoftLayer.FixtureTransport(), auth=None)
+        else:
+            # Create SL Client
+            client = SoftLayer.create_client_from_env(proxy=proxy, config_file=config_file)
+        self.client = client
+
+    def ensure_emp_client(self, config_file=None, is_demo=False, proxy=None):
         """Create a new SLAPI client to the environment.
 
         This will be a no-op if there is already a client in this environment.
         """
         if self.client is not None:
             return
 
         # Environment can be passed in explicitly. This is used for testing
         if is_demo:
-            client = SoftLayer.BaseClient(
-                transport=SoftLayer.FixtureTransport(),
-                auth=None,
-            )
+            client = SoftLayer.BaseClient(transport=SoftLayer.FixtureTransport(), auth=None)
         else:
             # Create SL Client
-            client = SoftLayer.create_client_from_env(
-                proxy=proxy,
-                config_file=config_file,
-            )
+            client = SoftLayer.employee_client(proxy=proxy, config_file=config_file)
         self.client = client
 
     def set_env_theme(self, config_file=None):
         """Get theme to color console and set in env"""
         theme = os.environ.get('SL_THEME')
         if theme:
             return theme
```

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/event_log/get.py` & `softlayer-6.2.0/SoftLayer/CLI/event_log/get.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,16 @@
               help="Display metadata if present")
 @click.option('--limit', '-l', type=click.INT, default=50, show_default=True,
               help="Total number of result to return. -1 to return ALL, there may be a LOT of these.")
 @environment.pass_env
 def cli(env, date_min, date_max, obj_event, obj_id, obj_type, utc_offset, metadata, limit):
     """Get Event Logs
 
-    Example:
+    Example::
+
         slcli event-log get -d 01/01/2019 -D 02/01/2019 -t User -l 10
     """
     columns = ['Event', 'Object', 'Type', 'Date', 'Username']
 
     event_mgr = SoftLayer.EventLogManager(env.client)
     user_mgr = SoftLayer.UserManager(env.client)
     request_filter = event_mgr.build_filter(date_min, date_max, obj_event, obj_id, obj_type, utc_offset)
@@ -71,13 +72,13 @@
             metadata_data = log['metaData'].strip("\n\t")
 
             click.secho(f"'{log['eventName']}','{label}','{log['objectName']}',"
                         f"'{utils.clean_time(log['eventCreateDate'], in_format=log_time)}',"
                         f"'{user}','{metadata_data}'")
         else:
             click.secho(f"'{log['eventName']}','{label}','{log['objectName']}',"
-                        f"'{utils.clean_time(log['eventCreateDate'],in_format=log_time)}',"
+                        f"'{utils.clean_time(log['eventCreateDate'], in_format=log_time)}',"
                         f"'{user}'")
 
         row_count = row_count + 1
         if row_count >= limit and limit != -1:
             return
```

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/event_log/types.py` & `softlayer-6.2.0/SoftLayer/CLI/event_log/types.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/exceptions.py` & `softlayer-6.2.0/SoftLayer/CLI/exceptions.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/access/authorize.py` & `softlayer-6.2.0/SoftLayer/CLI/file/access/authorize.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/access/list.py` & `softlayer-6.2.0/SoftLayer/CLI/file/access/list.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 
 @click.command(cls=SoftLayer.CLI.command.SLCommand, )
 @click.argument('volume_id')
 @click.option('--sortby', help='Column to sort by', default='name')
 @click.option('--columns',
               callback=column_helper.get_formatter(storage_utils.COLUMNS),
-              help=f"Columns to display. Options: { ', '.join(column.name for column in storage_utils.COLUMNS)}",
+              help=f"Columns to display. Options: {', '.join(column.name for column in storage_utils.COLUMNS)}",
               default=','.join(storage_utils.DEFAULT_COLUMNS))
 @environment.pass_env
 def cli(env, columns, sortby, volume_id):
     """List ACLs.
 
     Example::
         slcli file access-list 12345678 --sortby id
```

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/access/revoke.py` & `softlayer-6.2.0/SoftLayer/CLI/file/access/revoke.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/cancel.py` & `softlayer-6.2.0/SoftLayer/CLI/file/cancel.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/convert.py` & `softlayer-6.2.0/SoftLayer/CLI/file/convert.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/count.py` & `softlayer-6.2.0/SoftLayer/CLI/file/count.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/detail.py` & `softlayer-6.2.0/SoftLayer/CLI/file/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/duplicate.py` & `softlayer-6.2.0/SoftLayer/CLI/file/duplicate.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/duplicate_convert_status.py` & `softlayer-6.2.0/SoftLayer/CLI/file/duplicate_convert_status.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/limit.py` & `softlayer-6.2.0/SoftLayer/CLI/file/limit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/list.py` & `softlayer-6.2.0/SoftLayer/CLI/file/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/options.py` & `softlayer-6.2.0/SoftLayer/CLI/file/options.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/order.py` & `softlayer-6.2.0/SoftLayer/CLI/file/order.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/refresh.py` & `softlayer-6.2.0/SoftLayer/CLI/file/refresh.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/replication/disaster_recovery_failover.py` & `softlayer-6.2.0/SoftLayer/CLI/file/replication/disaster_recovery_failover.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/replication/failback.py` & `softlayer-6.2.0/SoftLayer/CLI/file/replication/failback.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/replication/failover.py` & `softlayer-6.2.0/SoftLayer/CLI/file/replication/failover.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/replication/locations.py` & `softlayer-6.2.0/SoftLayer/CLI/file/replication/locations.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/replication/order.py` & `softlayer-6.2.0/SoftLayer/CLI/file/replication/order.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/replication/partners.py` & `softlayer-6.2.0/SoftLayer/CLI/file/replication/partners.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/set_note.py` & `softlayer-6.2.0/SoftLayer/CLI/file/set_note.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/snapshot/cancel.py` & `softlayer-6.2.0/SoftLayer/CLI/file/snapshot/cancel.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/snapshot/create.py` & `softlayer-6.2.0/SoftLayer/CLI/file/snapshot/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/snapshot/delete.py` & `softlayer-6.2.0/SoftLayer/CLI/file/snapshot/delete.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/snapshot/disable.py` & `softlayer-6.2.0/SoftLayer/CLI/file/snapshot/disable.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/snapshot/enable.py` & `softlayer-6.2.0/SoftLayer/CLI/file/snapshot/enable.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/snapshot/get_notify_status.py` & `softlayer-6.2.0/SoftLayer/CLI/file/snapshot/get_notify_status.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/snapshot/list.py` & `softlayer-6.2.0/SoftLayer/CLI/file/snapshot/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/snapshot/order.py` & `softlayer-6.2.0/SoftLayer/CLI/file/snapshot/order.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/snapshot/restore.py` & `softlayer-6.2.0/SoftLayer/CLI/file/snapshot/restore.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/snapshot/schedule_list.py` & `softlayer-6.2.0/SoftLayer/CLI/file/snapshot/schedule_list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/file/snapshot/set_notify_status.py` & `softlayer-6.2.0/SoftLayer/CLI/file/snapshot/set_notify_status.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/firewall/add.py` & `softlayer-6.2.0/SoftLayer/CLI/firewall/add.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/firewall/cancel.py` & `softlayer-6.2.0/SoftLayer/CLI/firewall/cancel.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/firewall/detail.py` & `softlayer-6.2.0/SoftLayer/CLI/firewall/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/firewall/edit.py` & `softlayer-6.2.0/SoftLayer/CLI/firewall/edit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/firewall/list.py` & `softlayer-6.2.0/SoftLayer/CLI/firewall/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/firewall/monitoring.py` & `softlayer-6.2.0/SoftLayer/CLI/firewall/monitoring.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/formatting.py` & `softlayer-6.2.0/SoftLayer/CLI/formatting.py`

 * *Files 6% similar despite different names*

```diff
@@ -255,16 +255,15 @@
 
     :param confirmation str: the string the user has to enter in order to
                              confirm their action.
     """
     if not confirmation:
         confirmation = 'yes'
 
-    prompt = ('This action cannot be undone! Type "%s" or press Enter '
-              'to abort' % confirmation)
+    prompt = f"This action cannot be undone! Type '{confirmation}' or press Enter to abort"
 
     ans = click.prompt(prompt, default='', show_default=False)
     if ans.lower() == str(confirmation):
         return True
 
     return False
 
@@ -314,14 +313,30 @@
                                       % ','.join(duplicated_cols))
 
         self.columns = columns
         self.rows = []
         self.align = align or {}
         self.sortby = None
         self.title = title
+        # Used to print a message if the table is empty
+        self.empty_message = None
+
+    def __bool__(self):
+        """Useful for seeing if the table has any rows"""
+        return len(self.rows) > 0
+
+    def set_empty_message(self, message):
+        """Sets the empty message for this table for env.fout
+
+        Set this message if you want to print a message instead of a table to the user
+        but still want the json output to print an empty list `[]`
+
+        :param message str: Message to print if the table has no rows
+        """
+        self.empty_message = message
 
     def add_row(self, row):
         """Add a row to the table.
 
         :param list row: the row of string to be added
         """
         self.rows.append(row)
@@ -333,14 +348,18 @@
         for row in self.rows:
             formatted_row = [_format_python_value(v) for v in row]
             items.append(dict(zip(self.columns, formatted_row)))
         return items
 
     def prettytable(self, fmt='table', theme=None):
         """Returns a RICH table instance."""
+
+        # Used to print a message instead of a bad looking empty table
+        if not self and self.empty_message:
+            return self.empty_message
         box_style = box.SQUARE
         if fmt == 'raw':
             box_style = None
         color_table = utils.table_color_theme(theme)
         table = rTable(title=self.title, box=box_style, header_style=color_table['header'])
         if self.sortby:
             try:
```

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/globalip/assign.py` & `softlayer-6.2.0/SoftLayer/CLI/globalip/assign.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/globalip/cancel.py` & `softlayer-6.2.0/SoftLayer/CLI/globalip/cancel.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/globalip/create.py` & `softlayer-6.2.0/SoftLayer/CLI/globalip/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/globalip/list.py` & `softlayer-6.2.0/SoftLayer/CLI/globalip/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/globalip/unassign.py` & `softlayer-6.2.0/SoftLayer/CLI/globalip/unassign.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/hardware/authorize_storage.py` & `softlayer-6.2.0/SoftLayer/CLI/hardware/authorize_storage.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/hardware/bandwidth.py` & `softlayer-6.2.0/SoftLayer/CLI/hardware/bandwidth.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/hardware/billing.py` & `softlayer-6.2.0/SoftLayer/CLI/hardware/billing.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/hardware/cancel.py` & `softlayer-6.2.0/SoftLayer/CLI/hardware/cancel.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/hardware/cancel_reasons.py` & `softlayer-6.2.0/SoftLayer/CLI/hardware/cancel_reasons.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/hardware/create.py` & `softlayer-6.2.0/SoftLayer/CLI/hardware/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/hardware/create_credential.py` & `softlayer-6.2.0/SoftLayer/CLI/hardware/create_credential.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/hardware/create_options.py` & `softlayer-6.2.0/SoftLayer/CLI/hardware/create_options.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/hardware/credentials.py` & `softlayer-6.2.0/SoftLayer/CLI/hardware/credentials.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/hardware/detail.py` & `softlayer-6.2.0/SoftLayer/CLI/hardware/detail.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,22 +25,22 @@
     hardware = SoftLayer.HardwareManager(env.client)
 
     table = formatting.KeyValueTable(['name', 'value'])
     table.align['name'] = 'r'
     table.align['value'] = 'l'
 
     hardware_id = helpers.resolve_id(hardware.resolve_ids, identifier, 'hardware')
-    result = hardware.get_hardware(hardware_id)
+    result = hardware.get_hardware_fast(hardware_id)
     result = utils.NestedDict(result)
     hard_drives = hardware.get_hard_drives(hardware_id)
 
     operating_system = utils.lookup(result, 'operatingSystem', 'softwareLicense', 'softwareDescription') or {}
     memory = formatting.gb(result.get('memoryCapacity', 0))
     owner = None
-    if utils.lookup(result, 'billingItem') != []:
+    if utils.lookup(result, 'billingItem'):
         owner = utils.lookup(result, 'billingItem', 'orderItem', 'order', 'userRecord', 'username')
 
     table_hard_drives = formatting.Table(['Name', 'Capacity', 'Serial #'])
     for drives in hard_drives:
         name = drives['hardwareComponentModel']['manufacturer'] + " " + drives['hardwareComponentModel']['name']
         capacity = str(drives['hardwareComponentModel']['hardwareGenericComponentModel']['capacity']) + " " + str(
             drives['hardwareComponentModel']['hardwareGenericComponentModel']['units'])
@@ -68,19 +68,38 @@
 
     last_transaction = f"{utils.lookup(result, 'lastTransaction', 'transactionGroup', 'name')} \
         ({utils.clean_time(utils.lookup(result, 'lastTransaction', 'modifyDate'))})"
 
     table.add_row(['last_transaction', last_transaction])
     table.add_row(['billing', 'Hourly' if result['hourlyBillingFlag'] else 'Monthly'])
 
-    vlan_table = formatting.Table(['type', 'number', 'id', 'name', 'netmask'])
+    vlan_table = formatting.Table(['Network', 'Number', 'Id', 'Name', 'Type'])
     for vlan in result['networkVlans']:
-        vlan_table.add_row([vlan['networkSpace'], vlan['vlanNumber'],
-                            vlan['id'], vlan['fullyQualifiedName'],
-                            vlan['primarySubnets'][0]['netmask']])
+        vlan_table.add_row([
+            vlan.get('networkSpace'),
+            vlan.get('vlanNumber'),
+            vlan['id'],
+            vlan['fullyQualifiedName'],
+            'Primary'
+        ])
+
+    # Shows any VLANS trunked/tagged on this server
+    for component in result.get('networkComponents', []):
+        # These are the Primary network components
+        if component.get('primaryIpAddress', False):
+            uplink = component.get('uplinkComponent', {})
+            for trunk in uplink.get('networkVlanTrunks', []):
+                trunk_vlan = trunk.get('networkVlan')
+                vlan_table.add_row([
+                    trunk_vlan.get('networkSpace'),
+                    trunk_vlan.get('vlanNumber'),
+                    trunk_vlan.get('id'),
+                    trunk_vlan.get('fullyQualifiedName'),
+                    'Trunked'
+                ])
 
     table.add_row(['vlans', vlan_table])
 
     bandwidth = hardware.get_bandwidth_allocation(hardware_id)
     bw_table = _bw_table(bandwidth)
     table.add_row(['Bandwidth', bw_table])
     system_table = _system_table(result['activeComponents'])
```

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/hardware/dns.py` & `softlayer-6.2.0/SoftLayer/CLI/hardware/dns.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/hardware/edit.py` & `softlayer-6.2.0/SoftLayer/CLI/hardware/edit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/hardware/list.py` & `softlayer-6.2.0/SoftLayer/CLI/hardware/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/hardware/monitoring.py` & `softlayer-6.2.0/SoftLayer/CLI/hardware/monitoring.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/hardware/notification_add.py` & `softlayer-6.2.0/SoftLayer/CLI/hardware/notification_add.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/hardware/notification_delete.py` & `softlayer-6.2.0/SoftLayer/CLI/hardware/notification_delete.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/hardware/notifications.py` & `softlayer-6.2.0/SoftLayer/CLI/hardware/notifications.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/hardware/power.py` & `softlayer-6.2.0/SoftLayer/CLI/hardware/power.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/hardware/ready.py` & `softlayer-6.2.0/SoftLayer/CLI/hardware/ready.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/hardware/reflash_firmware.py` & `softlayer-6.2.0/SoftLayer/CLI/hardware/reflash_firmware.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/hardware/reload.py` & `softlayer-6.2.0/SoftLayer/CLI/hardware/reload.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/hardware/sensor.py` & `softlayer-6.2.0/SoftLayer/CLI/hardware/sensor.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/hardware/storage.py` & `softlayer-6.2.0/SoftLayer/CLI/hardware/storage.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/hardware/toggle_ipmi.py` & `softlayer-6.2.0/SoftLayer/CLI/hardware/toggle_ipmi.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/hardware/update_firmware.py` & `softlayer-6.2.0/SoftLayer/CLI/user/delete.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,33 @@
-"""Update firmware."""
+"""Delete user."""
 # :license: MIT, see LICENSE for more details.
 
 import click
 
 import SoftLayer
 from SoftLayer.CLI import environment
-from SoftLayer.CLI import exceptions
-from SoftLayer.CLI import formatting
 from SoftLayer.CLI import helpers
 
 
 @click.command(cls=SoftLayer.CLI.command.SLCommand, )
 @click.argument('identifier')
 @environment.pass_env
 def cli(env, identifier):
-    """Update server firmware."""
+    """Sets a user's status to CANCEL_PENDING, which will immediately disable the account,
 
-    mgr = SoftLayer.HardwareManager(env.client)
-    hw_id = helpers.resolve_id(mgr.resolve_ids, identifier, 'hardware')
-    if not (env.skip_confirmations or
-            formatting.confirm('This will power off the server with id %s and '
-                               'update device firmware. Continue?' % hw_id)):
-        raise exceptions.CLIAbort('Aborted.')
+    and will eventually be fully removed from the account by an automated internal process.
 
-    mgr.update_firmware(hw_id)
+    Example: slcli user delete userId
+
+    """
+
+    mgr = SoftLayer.UserManager(env.client)
+
+    user_id = helpers.resolve_id(mgr.resolve_ids, identifier, 'username')
+
+    user_template = {'userStatusId': 1021}
+
+    result = mgr.edit_user(user_id, user_template)
+    if result:
+        click.secho(f"{identifier} deleted successfully", fg='green')
+    else:
+        click.secho(f"Failed to delete {identifier}", fg='red')
```

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/hardware/upgrade.py` & `softlayer-6.2.0/SoftLayer/CLI/hardware/upgrade.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/helpers.py` & `softlayer-6.2.0/SoftLayer/CLI/helpers.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/image/__init__.py` & `softlayer-6.2.0/SoftLayer/CLI/image/__init__.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/image/datacenter.py` & `softlayer-6.2.0/SoftLayer/CLI/image/datacenter.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/image/detail.py` & `softlayer-6.2.0/SoftLayer/CLI/image/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/image/edit.py` & `softlayer-6.2.0/SoftLayer/CLI/image/edit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/image/export.py` & `softlayer-6.2.0/SoftLayer/CLI/image/export.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/image/import.py` & `softlayer-6.2.0/SoftLayer/CLI/image/import.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/image/list.py` & `softlayer-6.2.0/SoftLayer/CLI/image/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/image/share.py` & `softlayer-6.2.0/SoftLayer/CLI/image/share.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/image/share_deny.py` & `softlayer-6.2.0/SoftLayer/CLI/image/share_deny.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/licenses/cancel.py` & `softlayer-6.2.0/SoftLayer/CLI/licenses/cancel.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/licenses/create.py` & `softlayer-6.2.0/SoftLayer/CLI/licenses/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/licenses/create_options.py` & `softlayer-6.2.0/SoftLayer/CLI/licenses/create_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # :license: MIT, see LICENSE for more details.
 
 import click
 
 from SoftLayer.CLI.command import SLCommand as SLCommand
 from SoftLayer.CLI import environment
 from SoftLayer.CLI import formatting
-from SoftLayer.managers.licenses import LicensesManager
+from SoftLayer.managers.license import LicensesManager
 from SoftLayer import utils
 
 
 @click.command(cls=SLCommand)
 @environment.pass_env
 def cli(env):
     """Server order options for a given chassis."""
```

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/loadbal/detail.py` & `softlayer-6.2.0/SoftLayer/CLI/loadbal/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/loadbal/health.py` & `softlayer-6.2.0/SoftLayer/CLI/loadbal/health.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/loadbal/layer7_policy_list.py` & `softlayer-6.2.0/SoftLayer/CLI/loadbal/layer7_policy_list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/loadbal/list.py` & `softlayer-6.2.0/SoftLayer/CLI/loadbal/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/loadbal/members.py` & `softlayer-6.2.0/SoftLayer/CLI/loadbal/members.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/loadbal/ns_detail.py` & `softlayer-6.2.0/SoftLayer/CLI/loadbal/ns_detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/loadbal/ns_list.py` & `softlayer-6.2.0/SoftLayer/CLI/loadbal/ns_list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/loadbal/order.py` & `softlayer-6.2.0/SoftLayer/CLI/loadbal/order.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/loadbal/pools.py` & `softlayer-6.2.0/SoftLayer/CLI/loadbal/pools.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/loadbal/protocol_add.py` & `softlayer-6.2.0/SoftLayer/CLI/loadbal/protocol_add.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/loadbal/protocol_delete.py` & `softlayer-6.2.0/SoftLayer/CLI/loadbal/protocol_delete.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/loadbal/protocol_edit.py` & `softlayer-6.2.0/SoftLayer/CLI/loadbal/protocol_edit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/metadata.py` & `softlayer-6.2.0/SoftLayer/CLI/metadata.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/nas/credentials.py` & `softlayer-6.2.0/SoftLayer/CLI/nas/credentials.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/nas/list.py` & `softlayer-6.2.0/SoftLayer/CLI/nas/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/object_storage/cancel.py` & `softlayer-6.2.0/SoftLayer/CLI/object_storage/cancel.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/object_storage/credential/__init__.py` & `softlayer-6.2.0/SoftLayer/CLI/object_storage/credential/__init__.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/object_storage/credential/create.py` & `softlayer-6.2.0/SoftLayer/CLI/object_storage/credential/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/object_storage/credential/delete.py` & `softlayer-6.2.0/SoftLayer/CLI/object_storage/credential/delete.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/object_storage/credential/limit.py` & `softlayer-6.2.0/SoftLayer/CLI/object_storage/credential/limit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/object_storage/credential/list.py` & `softlayer-6.2.0/SoftLayer/CLI/object_storage/credential/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/object_storage/list_accounts.py` & `softlayer-6.2.0/SoftLayer/CLI/object_storage/list_accounts.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/object_storage/list_endpoints.py` & `softlayer-6.2.0/SoftLayer/CLI/object_storage/list_endpoints.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/order/cancelation.py` & `softlayer-6.2.0/SoftLayer/CLI/order/cancelation.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/order/category_list.py` & `softlayer-6.2.0/SoftLayer/CLI/order/category_list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/order/item_list.py` & `softlayer-6.2.0/SoftLayer/CLI/order/item_list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/order/lookup.py` & `softlayer-6.2.0/SoftLayer/CLI/order/lookup.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/order/package_list.py` & `softlayer-6.2.0/SoftLayer/CLI/order/package_list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/order/package_locations.py` & `softlayer-6.2.0/SoftLayer/CLI/order/package_locations.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/order/place.py` & `softlayer-6.2.0/SoftLayer/CLI/order/place.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/order/place_quote.py` & `softlayer-6.2.0/SoftLayer/CLI/order/place_quote.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/order/preset_list.py` & `softlayer-6.2.0/SoftLayer/CLI/order/preset_list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/order/quote.py` & `softlayer-6.2.0/SoftLayer/CLI/order/quote.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/order/quote_delete.py` & `softlayer-6.2.0/SoftLayer/CLI/order/quote_delete.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/order/quote_detail.py` & `softlayer-6.2.0/SoftLayer/CLI/order/quote_detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/order/quote_list.py` & `softlayer-6.2.0/SoftLayer/CLI/order/quote_list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/order/quote_save.py` & `softlayer-6.2.0/SoftLayer/CLI/order/quote_save.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/report/dc_closures.py` & `softlayer-6.2.0/SoftLayer/CLI/report/dc_closures.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/routes.py` & `softlayer-6.2.0/SoftLayer/CLI/routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
     This is how all commands are registered with the CLI.
 
     :license: MIT, see LICENSE for more details.
 """
 
 ALL_ROUTES = [
     ('shell', 'SoftLayer.shell.core:cli'),
+    ('emplogin', 'SoftLayer.CLI.login:cli'),
 
     ('call-api', 'SoftLayer.CLI.call_api:cli'),
 
     ('account', 'SoftLayer.CLI.account'),
     ('account:invoice-detail', 'SoftLayer.CLI.account.invoice_detail:cli'),
     ('account:invoices', 'SoftLayer.CLI.account.invoices:cli'),
     ('account:events', 'SoftLayer.CLI.account.events:cli'),
@@ -311,14 +312,17 @@
     ('hardware:upgrade', 'SoftLayer.CLI.hardware.upgrade:cli'),
     ('hardware:sensor', 'SoftLayer.CLI.hardware.sensor:cli'),
     ('hardware:monitoring', 'SoftLayer.CLI.hardware.monitoring:cli'),
     ('hardware:notifications', 'SoftLayer.CLI.hardware.notifications:cli'),
     ('hardware:notification-add', 'SoftLayer.CLI.hardware.notification_add:cli'),
     ('hardware:notification-delete', 'SoftLayer.CLI.hardware.notification_delete:cli'),
     ('hardware:create-credential', 'SoftLayer.CLI.hardware.create_credential:cli'),
+    ('hardware:vlan-trunkable', 'SoftLayer.CLI.hardware.vlan_trunkable:cli'),
+    ('hardware:vlan-add', 'SoftLayer.CLI.hardware.vlan_add:cli'),
+    ('hardware:vlan-remove', 'SoftLayer.CLI.hardware.vlan_remove:cli'),
 
     ('securitygroup', 'SoftLayer.CLI.securitygroup'),
     ('securitygroup:list', 'SoftLayer.CLI.securitygroup.list:cli'),
     ('securitygroup:detail', 'SoftLayer.CLI.securitygroup.detail:cli'),
     ('securitygroup:create', 'SoftLayer.CLI.securitygroup.create:cli'),
     ('securitygroup:edit', 'SoftLayer.CLI.securitygroup.edit:cli'),
     ('securitygroup:delete', 'SoftLayer.CLI.securitygroup.delete:cli'),
```

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/search.py` & `softlayer-6.2.0/SoftLayer/CLI/search.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/security/cert_add.py` & `softlayer-6.2.0/SoftLayer/CLI/security/cert_edit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,43 @@
-"""Add and upload SSL certificate details."""
+"""Edit SSL certificate."""
 # :license: MIT, see LICENSE for more details.
 
 import click
 
 import SoftLayer
 from SoftLayer.CLI import environment
 
 
 @click.command(cls=SoftLayer.CLI.command.SLCommand, )
+@click.argument('identifier')
 @click.option('--crt',
               type=click.Path(exists=True),
               help="Certificate file")
 @click.option('--csr',
               type=click.Path(exists=True),
               help="Certificate Signing Request file")
 @click.option('--icc',
               type=click.Path(exists=True),
               help="Intermediate Certificate file")
 @click.option('--key', type=click.Path(exists=True), help="Private Key file")
 @click.option('--notes', help="Additional notes")
 @environment.pass_env
-def cli(env, crt, csr, icc, key, notes):
-    """Add and upload SSL certificate details."""
-
-    template = {
-        'intermediateCertificate': '',
-        'certificateSigningRequest': '',
-        'notes': notes,
-    }
+def cli(env, identifier, crt, csr, icc, key, notes):
+    """Edit SSL certificate."""
+    template = {'id': identifier}
     with open(crt, encoding="utf-8") as file_crt:
-        template['certificate'] = file_crt.read()
+        if crt:
+            template['certificate'] = file_crt.read()
     with open(key, encoding="utf-8") as file_key:
-        template['privateKey'] = file_key.read()
+        if key:
+            template['privateKey'] = file_key.read()
     with open(csr, encoding="utf-8") as file_csr:
         if csr:
-            body = file_csr.read()
-            template['certificateSigningRequest'] = body
-
+            template['certificateSigningRequest'] = file_csr.read()
     with open(icc, encoding="utf-8") as file_icc:
         if icc:
-            body = file_icc.read()
-            template['intermediateCertificate'] = body
+            template['intermediateCertificate'] = file_icc.read()
+    if notes:
+        template['notes'] = notes
 
     manager = SoftLayer.SSLManager(env.client)
-    manager.add_certificate(template)
+    manager.edit_certificate(template)
```

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/security/cert_download.py` & `softlayer-6.2.0/SoftLayer/CLI/security/cert_download.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/security/cert_edit.py` & `softlayer-6.2.0/SoftLayer/CLI/security/cert_add.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,40 @@
-"""Edit SSL certificate."""
+"""Add and upload SSL certificate details."""
 # :license: MIT, see LICENSE for more details.
 
 import click
 
 import SoftLayer
 from SoftLayer.CLI import environment
 
 
 @click.command(cls=SoftLayer.CLI.command.SLCommand, )
-@click.argument('identifier')
-@click.option('--crt',
-              type=click.Path(exists=True),
-              help="Certificate file")
-@click.option('--csr',
-              type=click.Path(exists=True),
-              help="Certificate Signing Request file")
-@click.option('--icc',
-              type=click.Path(exists=True),
-              help="Intermediate Certificate file")
-@click.option('--key', type=click.Path(exists=True), help="Private Key file")
+@click.option('--crt', required=True, type=click.Path(exists=True), help="Certificate file")
+@click.option('--key', type=click.Path(exists=True), required=True, help="Private Key file")
+@click.option('--csr', type=click.Path(exists=True), help="Certificate Signing Request file")
+@click.option('--icc', type=click.Path(exists=True), help="Intermediate Certificate file")
 @click.option('--notes', help="Additional notes")
 @environment.pass_env
-def cli(env, identifier, crt, csr, icc, key, notes):
-    """Edit SSL certificate."""
-    template = {'id': identifier}
+def cli(env, crt, csr, icc, key, notes):
+    """Add and upload SSL certificate details."""
+
+    template = {
+        'intermediateCertificate': '',
+        'certificateSigningRequest': '',
+        'notes': notes,
+    }
     with open(crt, encoding="utf-8") as file_crt:
-        if crt:
-            template['certificate'] = file_crt.read()
+        template['certificate'] = file_crt.read()
     with open(key, encoding="utf-8") as file_key:
-        if key:
-            template['privateKey'] = file_key.read()
-    with open(csr, encoding="utf-8") as file_csr:
-        if csr:
-            template['certificateSigningRequest'] = file_csr.read()
-    with open(icc, encoding="utf-8") as file_icc:
-        if icc:
-            template['intermediateCertificate'] = file_icc.read()
-    if notes:
-        template['notes'] = notes
+        template['privateKey'] = file_key.read()
+    if csr:
+        with open(csr, encoding="utf-8") as file_csr:
+            body = file_csr.read()
+            template['certificateSigningRequest'] = body
+
+    if icc:
+        with open(icc, encoding="utf-8") as file_icc:
+            body = file_icc.read()
+            template['intermediateCertificate'] = body
 
     manager = SoftLayer.SSLManager(env.client)
-    manager.edit_certificate(template)
+    manager.add_certificate(template)
```

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/security/cert_list.py` & `softlayer-6.2.0/SoftLayer/CLI/security/cert_list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/security/cert_remove.py` & `softlayer-6.2.0/SoftLayer/CLI/security/cert_remove.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/security/sshkey_add.py` & `softlayer-6.2.0/SoftLayer/CLI/security/sshkey_add.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/security/sshkey_edit.py` & `softlayer-6.2.0/SoftLayer/CLI/security/sshkey_edit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/security/sshkey_list.py` & `softlayer-6.2.0/SoftLayer/CLI/security/sshkey_list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/security/sshkey_print.py` & `softlayer-6.2.0/SoftLayer/CLI/security/sshkey_print.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/security/sshkey_remove.py` & `softlayer-6.2.0/SoftLayer/CLI/security/sshkey_remove.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/securitygroup/create.py` & `softlayer-6.2.0/SoftLayer/CLI/securitygroup/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/securitygroup/delete.py` & `softlayer-6.2.0/SoftLayer/CLI/securitygroup/delete.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/securitygroup/detail.py` & `softlayer-6.2.0/SoftLayer/CLI/securitygroup/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/securitygroup/edit.py` & `softlayer-6.2.0/SoftLayer/CLI/securitygroup/edit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/securitygroup/event_log.py` & `softlayer-6.2.0/SoftLayer/CLI/securitygroup/event_log.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/securitygroup/interface.py` & `softlayer-6.2.0/SoftLayer/CLI/securitygroup/interface.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/securitygroup/list.py` & `softlayer-6.2.0/SoftLayer/CLI/securitygroup/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/securitygroup/rule.py` & `softlayer-6.2.0/SoftLayer/CLI/securitygroup/rule.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/storage_utils.py` & `softlayer-6.2.0/SoftLayer/CLI/storage_utils.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/subnet/cancel.py` & `softlayer-6.2.0/SoftLayer/CLI/subnet/cancel.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/subnet/clear_route.py` & `softlayer-6.2.0/SoftLayer/CLI/subnet/clear_route.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/subnet/create.py` & `softlayer-6.2.0/SoftLayer/CLI/subnet/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/subnet/detail.py` & `softlayer-6.2.0/SoftLayer/CLI/subnet/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/subnet/edit.py` & `softlayer-6.2.0/SoftLayer/CLI/subnet/edit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/subnet/edit_ip.py` & `softlayer-6.2.0/SoftLayer/CLI/subnet/edit_ip.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/subnet/list.py` & `softlayer-6.2.0/SoftLayer/CLI/subnet/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/subnet/lookup.py` & `softlayer-6.2.0/SoftLayer/CLI/subnet/lookup.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/subnet/route.py` & `softlayer-6.2.0/SoftLayer/CLI/subnet/route.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/summary.py` & `softlayer-6.2.0/SoftLayer/CLI/summary.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/tags/cleanup.py` & `softlayer-6.2.0/SoftLayer/CLI/tags/cleanup.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/tags/delete.py` & `softlayer-6.2.0/SoftLayer/CLI/tags/delete.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/tags/details.py` & `softlayer-6.2.0/SoftLayer/CLI/tags/details.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/tags/list.py` & `softlayer-6.2.0/SoftLayer/CLI/tags/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/tags/set.py` & `softlayer-6.2.0/SoftLayer/CLI/tags/set.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/tags/taggable.py` & `softlayer-6.2.0/SoftLayer/CLI/tags/taggable.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/template.py` & `softlayer-6.2.0/SoftLayer/CLI/template.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/ticket/__init__.py` & `softlayer-6.2.0/SoftLayer/CLI/ticket/__init__.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/ticket/attach.py` & `softlayer-6.2.0/SoftLayer/CLI/ticket/attach.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/ticket/create.py` & `softlayer-6.2.0/SoftLayer/CLI/ticket/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/ticket/detach.py` & `softlayer-6.2.0/SoftLayer/CLI/ticket/detach.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/ticket/detail.py` & `softlayer-6.2.0/SoftLayer/CLI/ticket/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/ticket/list.py` & `softlayer-6.2.0/SoftLayer/CLI/ticket/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/ticket/subjects.py` & `softlayer-6.2.0/SoftLayer/CLI/ticket/subjects.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/ticket/summary.py` & `softlayer-6.2.0/SoftLayer/CLI/ticket/summary.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/ticket/update.py` & `softlayer-6.2.0/SoftLayer/CLI/ticket/update.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/ticket/upload.py` & `softlayer-6.2.0/SoftLayer/CLI/ticket/upload.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/user/apikey.py` & `softlayer-6.2.0/SoftLayer/CLI/user/apikey.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/user/create.py` & `softlayer-6.2.0/SoftLayer/CLI/user/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/user/delete.py` & `softlayer-6.2.0/SoftLayer/CLI/user/edit_details.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,46 @@
-"""Delete user."""
+"""List Users."""
 # :license: MIT, see LICENSE for more details.
 
+
+import json
+
 import click
 
 import SoftLayer
 from SoftLayer.CLI import environment
+from SoftLayer.CLI import exceptions
 from SoftLayer.CLI import helpers
 
 
 @click.command(cls=SoftLayer.CLI.command.SLCommand, )
-@click.argument('identifier')
+@click.argument('user')
+@click.option('--template', '-t', required=True,
+              help="A json string describing https://softlayer.github.io/reference/datatypes/SoftLayer_User_Customer/")
 @environment.pass_env
-def cli(env, identifier):
-    """Sets a user's status to CANCEL_PENDING, which will immediately disable the account,
+def cli(env, user, template):
+    """Edit a Users details
 
-    and will eventually be fully removed from the account by an automated internal process.
+    JSON strings should be enclosed in '' and each item should be enclosed in ""
 
-    Example: slcli user delete userId
+    Example::
 
-    """
+        slcli user edit-details testUser -t '{"firstName": "Test", "lastName": "Testerson"}'
 
+    """
     mgr = SoftLayer.UserManager(env.client)
+    user_id = helpers.resolve_id(mgr.resolve_ids, user, 'username')
 
-    user_id = helpers.resolve_id(mgr.resolve_ids, identifier, 'username')
-
-    user_template = {'userStatusId': 1021}
+    user_template = {}
+    if template is not None:
+        try:
+            template_object = json.loads(template)
+            for key in template_object:
+                user_template[key] = template_object[key]
+        except ValueError as ex:
+            raise exceptions.ArgumentError(f"Unable to parse --template. {ex}")
 
     result = mgr.edit_user(user_id, user_template)
     if result:
-        click.secho(f"{identifier} deleted successfully", fg='green')
+        click.secho(f"{user} updated successfully", fg='green')
     else:
-        click.secho(f"Failed to delete {identifier}", fg='red')
+        click.secho(f"Failed to update {user}", fg='red')
```

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/user/detail.py` & `softlayer-6.2.0/SoftLayer/CLI/user/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/user/device_access.py` & `softlayer-6.2.0/SoftLayer/CLI/user/device_access.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/user/edit_details.py` & `softlayer-6.2.0/SoftLayer/CLI/user/vpn_subnet.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,30 @@
-"""List Users."""
+"""Add or remove specific subnets access for a user."""
 # :license: MIT, see LICENSE for more details.
 
 
-import json
-
 import click
 
 import SoftLayer
 from SoftLayer.CLI import environment
-from SoftLayer.CLI import exceptions
 from SoftLayer.CLI import helpers
 
 
 @click.command(cls=SoftLayer.CLI.command.SLCommand, )
-@click.argument('user')
-@click.option('--template', '-t', required=True,
-              help="A json string describing https://softlayer.github.io/reference/datatypes/SoftLayer_User_Customer/")
+@click.option('--add/--remove', default=True,
+              help="Add or remove access to subnets.")
+@click.argument('user', nargs=1, required=True)
+@click.argument('subnet', nargs=-1, required=True)
 @environment.pass_env
-def cli(env, user, template):
-    """Edit a Users details
-
-    JSON strings should be enclosed in '' and each item should be enclosed in ""
-
-    Example::
-
-        slcli user edit-details testUser -t '{"firstName": "Test", "lastName": "Testerson"}'
-
-    """
+def cli(env, user, add, subnet):
+    """Add or remove subnets access for a user."""
     mgr = SoftLayer.UserManager(env.client)
     user_id = helpers.resolve_id(mgr.resolve_ids, user, 'username')
+    if add:
+        result = mgr.vpn_subnet_add(user_id, subnet)
+    else:
+        result = mgr.vpn_subnet_remove(user_id, subnet)
 
-    user_template = {}
-    if template is not None:
-        try:
-            template_object = json.loads(template)
-            for key in template_object:
-                user_template[key] = template_object[key]
-        except ValueError as ex:
-            raise exceptions.ArgumentError(f"Unable to parse --template. {ex}")
-
-    result = mgr.edit_user(user_id, user_template)
     if result:
         click.secho(f"{user} updated successfully", fg='green')
     else:
         click.secho(f"Failed to update {user}", fg='red')
```

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/user/edit_notifications.py` & `softlayer-6.2.0/SoftLayer/CLI/user/edit_notifications.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/user/edit_permissions.py` & `softlayer-6.2.0/SoftLayer/CLI/user/edit_permissions.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/user/grant_access.py` & `softlayer-6.2.0/SoftLayer/CLI/user/grant_access.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/user/list.py` & `softlayer-6.2.0/SoftLayer/CLI/user/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/user/notifications.py` & `softlayer-6.2.0/SoftLayer/CLI/user/notifications.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/user/permissions.py` & `softlayer-6.2.0/SoftLayer/CLI/user/permissions.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/user/remove_access.py` & `softlayer-6.2.0/SoftLayer/CLI/user/remove_access.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/user/vpn_enable_or_disable.py` & `softlayer-6.2.0/SoftLayer/CLI/user/vpn_enable_or_disable.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/user/vpn_manual.py` & `softlayer-6.2.0/SoftLayer/CLI/user/vpn_manual.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/user/vpn_password.py` & `softlayer-6.2.0/SoftLayer/CLI/user/vpn_password.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/__init__.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/__init__.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/access.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/access.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/authorize_storage.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/authorize_storage.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/bandwidth.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/bandwidth.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/billing.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/billing.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/cancel.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/cancel.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/capacity/__init__.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/capacity/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 """Manages Reserved Capacity."""
 # :license: MIT, see LICENSE for more details.
 
 import importlib
 import os
 
 import click
+from SoftLayer.CLI.command import CommandLoader
+from SoftLayer.CLI.command import OptionHighlighter
 
 CONTEXT = {'help_option_names': ['-h', '--help'],
            'max_content_width': 999}
 
 
-class CapacityCommands(click.MultiCommand):
+class CapacityCommands(CommandLoader):
     """Loads module for capacity related commands.
 
     Will automatically replace _ with - where appropriate.
     I'm not sure if this is better or worse than using a long list of manual routes, so I'm trying it here.
     CLI/virt/capacity/create_guest.py -> slcli vs capacity create-guest
     """
 
     def __init__(self, **attrs):
-        click.MultiCommand.__init__(self, **attrs)
+        CommandLoader.__init__(self, **attrs)
         self.path = os.path.dirname(__file__)
+        self.highlighter = OptionHighlighter()
+        self.env = None
+        self.console = None
 
     def list_commands(self, ctx):
         """List all sub-commands."""
         commands = []
         for filename in os.listdir(self.path):
             if filename == '__init__.py':
                 continue
```

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/capacity/create.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/capacity/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/capacity/create_guest.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/capacity/create_guest.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/capacity/create_options.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/capacity/create_options.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/capacity/detail.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/capacity/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/capacity/list.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/capacity/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/capture.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/capture.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/create.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/create_options.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/create_options.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/credentials.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/credentials.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/detail.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/dns.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/dns.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/edit.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/edit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/list.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/list.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,26 +15,19 @@
 
 COLUMNS = [
     column_helper.Column('guid', ('globalIdentifier',)),
     column_helper.Column('primary_ip', ('primaryIpAddress',)),
     column_helper.Column('backend_ip', ('primaryBackendIpAddress',)),
     column_helper.Column('datacenter', ('datacenter', 'name')),
     column_helper.Column('action', lambda guest: formatting.active_txn(guest),
-                         mask='''
-                         activeTransaction[
-                            id,transactionStatus[name,friendlyName]
-                         ]'''),
+                         mask='activeTransaction[id,transactionStatus[name,friendlyName]]'),
     column_helper.Column('power_state', ('powerState', 'name')),
-    column_helper.Column(
-        'created_by',
-        ('billingItem', 'orderItem', 'order', 'userRecord', 'username')),
-    column_helper.Column(
-        'tags',
-        lambda server: formatting.tags(server.get('tagReferences')),
-        mask="tagReferences.tag.name"),
+    column_helper.Column('created_by', ('billingItem', 'orderItem', 'order', 'userRecord', 'username')),
+    column_helper.Column('tags', lambda server: formatting.tags(server.get('tagReferences')),
+                         mask="tagReferences.tag.name"),
     column_helper.Column(
         'createDate',
         lambda guest: utils.clean_time(guest.get('createDate'),
                                        in_format='%Y-%m-%dT%H:%M:%S', out_format='%Y-%m-%d %H:%M'), mask="createDate"),
 ]
 
 DEFAULT_COLUMNS = [
@@ -55,15 +48,15 @@
 @click.option('--domain', '-D', help='Domain portion of the FQDN')
 @click.option('--datacenter', '-d', help='Datacenter shortname')
 @click.option('--hostname', '-H', help='Host portion of the FQDN')
 @click.option('--memory', '-m', help='Memory in mebibytes', type=click.INT)
 @click.option('--network', '-n', help='Network port speed in Mbps')
 @click.option('--hourly', is_flag=True, help='Show only hourly instances')
 @click.option('--monthly', is_flag=True, help='Show only monthly instances')
-@click.option('--tag', '-t', help='list of tags')
+@click.option('--tag', '-t', help='list of tags', multiple=True)
 @click.option('--transient', help='Filter by transient instances', type=click.BOOL)
 @click.option('--search', is_flag=False, flag_value="", default=None,
               help="Use the more flexible Search API to list instances. See `slcli search --types` for list " +
               "of searchable fields.")
 @helpers.multi_option('--tag', help='Filter by tags')
 @click.option('--sortby', default='hostname', show_default=True, help='Column to sort by')
 @click.option('--columns',
```

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/migrate.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/migrate.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/monitoring.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/monitoring.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/notification_add.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/notification_add.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/notification_delete.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/notification_delete.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/notifications.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/notifications.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/os_available.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/os_available.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/placementgroup/__init__.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/placementgroup/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 """Manages Reserved Capacity."""
 # :license: MIT, see LICENSE for more details.
 
 import importlib
 import os
 
 import click
+from SoftLayer.CLI.command import CommandLoader
+from SoftLayer.CLI.command import OptionHighlighter
 
 CONTEXT = {'help_option_names': ['-h', '--help'],
            'max_content_width': 999}
 
 
-class PlacementGroupCommands(click.MultiCommand):
+class PlacementGroupCommands(CommandLoader):
     """Loads module for placement group related commands.
 
     Currently the base command loader only supports going two commands deep.
     So this small loader is required for going that third level.
     """
 
     def __init__(self, **attrs):
-        click.MultiCommand.__init__(self, **attrs)
+        CommandLoader.__init__(self, **attrs)
         self.path = os.path.dirname(__file__)
+        self.highlighter = OptionHighlighter()
+        self.env = None
+        self.console = None
 
     def list_commands(self, ctx):
         """List all sub-commands."""
         commands = []
         for filename in os.listdir(self.path):
             if filename == '__init__.py':
                 continue
```

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/placementgroup/create.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/placementgroup/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/placementgroup/create_options.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/placementgroup/create_options.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/placementgroup/delete.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/placementgroup/delete.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/placementgroup/detail.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/placementgroup/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/placementgroup/list.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/placementgroup/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/power.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/power.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/ready.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/ready.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/reload.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/reload.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/storage.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/storage.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/upgrade.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/upgrade.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/virt/usage.py` & `softlayer-6.2.0/SoftLayer/CLI/virt/usage.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/vlan/cancel.py` & `softlayer-6.2.0/SoftLayer/CLI/vlan/cancel.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/vlan/create.py` & `softlayer-6.2.0/SoftLayer/CLI/vlan/create.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/vlan/create_options.py` & `softlayer-6.2.0/SoftLayer/CLI/vlan/create_options.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/vlan/detail.py` & `softlayer-6.2.0/SoftLayer/CLI/vlan/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/vlan/edit.py` & `softlayer-6.2.0/SoftLayer/CLI/vlan/edit.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/vlan/list.py` & `softlayer-6.2.0/SoftLayer/CLI/vlan/list.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,25 +21,21 @@
            'Virtual servers',
            'Public ips',
            'Premium',
            'Tags']
 
 
 @click.command(cls=SoftLayer.CLI.command.SLCommand, )
-@click.option('--sortby',
-              help='Column to sort by',
-              type=click.Choice(COLUMNS))
+@click.option('--sortby', help='Column to sort by', type=click.Choice(COLUMNS))
 @click.option('--datacenter', '-d',
               help='Filter by datacenter shortname (sng01, dal05, ...)')
 @click.option('--number', '-n', help='Filter by VLAN number')
 @click.option('--name', help='Filter by VLAN name')
-@click.option('--limit', '-l',
-              help='How many results to get in one api call, default is 100',
-              default=100,
-              show_default=True)
+@click.option('--limit', '-l', default=100, show_default=True,
+              help='How many results to get in one api call, default is 100')
 @environment.pass_env
 def cli(env, sortby, datacenter, number, name, limit):
     """List VLANs.
 
     Note: A * Indicates a POD is closing soon. Ex:[red] Pod01* [/red]
     """
```

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/vpn/ipsec/cancel.py` & `softlayer-6.2.0/SoftLayer/CLI/vpn/ipsec/cancel.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/vpn/ipsec/configure.py` & `softlayer-6.2.0/SoftLayer/CLI/vpn/ipsec/configure.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/vpn/ipsec/detail.py` & `softlayer-6.2.0/SoftLayer/CLI/vpn/ipsec/detail.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/vpn/ipsec/list.py` & `softlayer-6.2.0/SoftLayer/CLI/vpn/ipsec/list.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/vpn/ipsec/order.py` & `softlayer-6.2.0/SoftLayer/CLI/vpn/ipsec/order.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/vpn/ipsec/subnet/add.py` & `softlayer-6.2.0/SoftLayer/CLI/vpn/ipsec/subnet/add.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/vpn/ipsec/subnet/remove.py` & `softlayer-6.2.0/SoftLayer/CLI/vpn/ipsec/subnet/remove.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/vpn/ipsec/translation/add.py` & `softlayer-6.2.0/SoftLayer/CLI/vpn/ipsec/translation/add.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/vpn/ipsec/translation/remove.py` & `softlayer-6.2.0/SoftLayer/CLI/vpn/ipsec/translation/remove.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/vpn/ipsec/translation/update.py` & `softlayer-6.2.0/SoftLayer/CLI/vpn/ipsec/translation/update.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/CLI/vpn/ipsec/update.py` & `softlayer-6.2.0/SoftLayer/CLI/vpn/ipsec/update.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/__init__.py` & `softlayer-6.2.0/SoftLayer/__init__.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/auth.py` & `softlayer-6.2.0/SoftLayer/auth.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 
 __all__ = [
     'BasicAuthentication',
     'TokenAuthentication',
     'BasicHTTPAuthentication',
     'AuthenticationBase',
+    'X509Authentication',
+    'EmployeeAuthentication'
 ]
 
 
 class AuthenticationBase(object):
     """A base authentication class intended to be overridden."""
 
     def get_request(self, request):
@@ -133,7 +135,54 @@
         """Sets token-based auth headers."""
         request.transport_headers['Authorization'] = f'Bearer {self.api_key}'
         request.transport_user = self.username
         return request
 
     def __repr__(self):
         return f"BearerAuthentication(username={self.username}, token={self.api_key})"
+
+
+class X509Authentication(AuthenticationBase):
+    """X509Authentication authentication class.
+
+        :param certificate str:  Path to a users SSL certificate for authentication
+        :param CA Cert str: Path to the Servers signed certificate.
+    """
+
+    def __init__(self, cert, ca_cert):
+        self.cert = cert
+        self.ca_cert = ca_cert
+
+    def get_request(self, request):
+        """Sets token-based auth headers."""
+        request.cert = self.cert
+        request.verify = self.ca_cert
+        return request
+
+    def __repr__(self):
+        return f"X509Authentication(cert={self.cert}, ca_cert={self.ca_cert})"
+
+
+class EmployeeAuthentication(AuthenticationBase):
+    """Token-based authentication class.
+
+        :param username str: a user's username
+        :param user_hash str: a user's Authentication hash
+    """
+    def __init__(self, user_id, user_hash):
+        self.user_id = user_id
+        self.hash = user_hash
+
+    def get_request(self, request):
+        """Sets token-based auth headers."""
+        if 'xml' in request.url:
+            request.headers['employeesession'] = {
+                'userId': self.user_id,
+                'authToken': self.hash,
+            }
+        else:
+            request.transport_user = self.user_id
+            request.transport_password = self.hash
+        return request
+
+    def __repr__(self):
+        return "EmployeeAuthentication(userId=%r,hash=%s)" % (self.user_id, self.hash)
```

### Comparing `SoftLayer-6.1.9/SoftLayer/config.py` & `softlayer-6.2.0/SoftLayer/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -55,24 +55,30 @@
     config_files = [os.path.expanduser(f) for f in config_files]
     config = configparser.RawConfigParser({
         'username': '',
         'api_key': '',
         'endpoint_url': '',
         'timeout': '0',
         'proxy': '',
+        'userid': '',
+        'access_token': '',
+        'verify': True
     })
     config.read(config_files)
 
     if config.has_section('softlayer'):
         return {
             'endpoint_url': config.get('softlayer', 'endpoint_url'),
             'timeout': config.getfloat('softlayer', 'timeout'),
             'proxy': config.get('softlayer', 'proxy'),
             'username': config.get('softlayer', 'username'),
             'api_key': config.get('softlayer', 'api_key'),
+            'userid': config.get('softlayer', 'userid'),
+            'access_token': config.get('softlayer', 'access_token'),
+            'verify':   config.get('softlayer', 'verify')
         }
 
 
 SETTING_RESOLVERS = [get_client_settings_args,
                      get_client_settings_env,
                      get_client_settings_config_file]
 
@@ -105,14 +111,16 @@
     # No configuration file found.
     if not config.has_section('softlayer'):
         config.add_section('softlayer')
         config['softlayer']['username'] = ''
         config['softlayer']['endpoint_url'] = ''
         config['softlayer']['api_key'] = ''
         config['softlayer']['timeout'] = '0'
+        config['softlayer']['userid'] = ''
+        config['softlayer']['access_tokne'] = ''
 
     return config
 
 
 def write_config(configuration, config_file=None):
     """Writes a configuration to config_file"""
     if config_file is None:
```

### Comparing `SoftLayer-6.1.9/SoftLayer/consts.py` & `softlayer-6.2.0/SoftLayer/consts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
     SoftLayer.consts
     ~~~~~~~~~~~~~~~~
     Contains constants used throughout the library
 
     :license: MIT, see LICENSE for more details.
 """
-VERSION = 'v6.1.9'
+VERSION = 'v6.2.0'
 API_PUBLIC_ENDPOINT = 'https://api.softlayer.com/xmlrpc/v3.1/'
 API_PRIVATE_ENDPOINT = 'https://api.service.softlayer.com/xmlrpc/v3.1/'
 API_PUBLIC_ENDPOINT_REST = 'https://api.softlayer.com/rest/v3.1/'
 API_PRIVATE_ENDPOINT_REST = 'https://api.service.softlayer.com/rest/v3.1/'
 USER_AGENT = "softlayer-python/%s" % VERSION
 CONFIG_FILE = "~/.softlayer"
```

### Comparing `SoftLayer-6.1.9/SoftLayer/decoration.py` & `softlayer-6.2.0/SoftLayer/decoration.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/exceptions.py` & `softlayer-6.2.0/SoftLayer/exceptions.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Account.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Account.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Billing_Invoice.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Billing_Invoice.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Billing_Item.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Billing_Item.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Billing_Item_Cancellation_Request.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Billing_Item_Cancellation_Request.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Billing_Order.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Billing_Order.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Billing_Order_Quote.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Billing_Order_Quote.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Dns_Domain.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Dns_Domain.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Event_Log.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Event_Log.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Hardware.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Hardware.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Hardware_Server.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Hardware_Server.py`

 * *Files 18% similar despite different names*

```diff
@@ -108,14 +108,15 @@
                 'actionDescription': 'Notify Users',
                 'id': 2,
                 'level': 0
             }
         }
     ]
 }
+
 editObject = True
 setTags = True
 setPrivateNetworkInterfaceSpeed = True
 setPublicNetworkInterfaceSpeed = True
 toggleManagementInterface = True
 powerOff = True
 powerOn = True
@@ -126,45 +127,59 @@
 createFirmwareUpdateTransaction = True
 createFirmwareReflashTransaction = True
 setUserMetadata = ['meta']
 reloadOperatingSystem = 'OK'
 getReverseDomainRecords = [
     {'resourceRecords': [{'data': '2.0.1.10.in-addr.arpa'}]}]
 bootToRescueLayer = True
-getFrontendNetworkComponents = [
+
+getNetworkComponents = [
     {'maxSpeed': 100},
     {
         'maxSpeed': 1000,
         'networkComponentGroup': {
             'groupTypeId': 2,
             'networkComponents': [{'maxSpeed': 1000}, {'maxSpeed': 1000}]
-        }
+        },
+        'primaryIpAddress': '192.168.1.1',
+        'id': 998877,
+        'uplinkComponent': {}
     },
     {
         'maxSpeed': 1000,
         'networkComponentGroup': {
             'groupTypeId': 2,
             'networkComponents': [{'maxSpeed': 1000}, {'maxSpeed': 1000}]
-        }
+        },
+        'id': 665544,
+        'uplinkComponent': {}
     },
     {
         'maxSpeed': 1000,
         'networkComponentGroup': {
             'groupTypeId': 2,
             'networkComponents': [{'maxSpeed': 1000}, {'maxSpeed': 1000}]
-        }
+        },
+        'id': 112233,
+        'uplinkComponent': {}
     },
     {
         'maxSpeed': 1000,
         'networkComponentGroup': {
             'groupTypeId': 2,
             'networkComponents': [{'maxSpeed': 1000}, {'maxSpeed': 1000}]
-        }
+        },
+        'primaryIpAddress': '10.0.0.1',
+        'id': 123456,
+        'uplinkComponent': {}
     }
 ]
+# This splits out the network components into 2 sections so they are different enough for tests
+getFrontendNetworkComponents = getNetworkComponents[:2]
+getBackendNetworkComponents = getNetworkComponents[3:]
 
 getBandwidthAllotmentDetail = {
     'allocationId': 25465663,
     'bandwidthAllotmentId': 138442,
     'effectiveDate': '2019-04-03T23:00:00-06:00',
     'endEffectiveDate': None,
     'id': 25888247,
@@ -406,8 +421,77 @@
             {
                 "createDate": "2020-09-24T13:46:29-06:00",
                 "version": "5.60"
             },
             {
                 "createDate": "2019-10-14T16:51:12-06:00",
                 "version": "5.10"
-            }]}}]
+            }
+        ]
+    }
+}]
+getActiveComponents = getComponents
+getActiveTransaction = getObject['activeTransaction']
+getOperatingSystem = getObject['operatingSystem']
+getSoftwareComponents = [
+    {
+        "hardwareId": 1907356,
+        "id": 59003868,
+        "manufacturerLicenseInstance": "",
+        "softwareLicense": {
+            "id": 20658,
+            "softwareDescriptionId": 2888,
+            "softwareDescription": {
+                "controlPanel": 0,
+                "id": 2888,
+                "licenseTermValue": 0,
+                "longDescription": "Juniper vSRX 1G 19.4R2-S3 Standard 19.4.2.3",
+                "manufacturer": "Juniper",
+                "name": "vSRX 1G 19.4R2-S3 Standard",
+                "operatingSystem": 1,
+                "referenceCode": "UBUNTU_18_64",
+                "upgradeSoftwareDescriptionId": None,
+                "upgradeSwDescId": None,
+                "version": "19.4.2.3",
+                "virtualLicense": 0,
+                "virtualizationPlatform": 0,
+                "requiredUser": "root"
+            }
+        }
+    },
+    {
+        "hardwareId": 1907356,
+        "id": 59003870,
+        "manufacturerLicenseInstance": "",
+        "softwareLicense": {
+            "id": 147,
+            "softwareDescriptionId": 148,
+            "softwareDescription": {
+                "controlPanel": 0,
+                "id": 148,
+                "licenseTermValue": None,
+                "longDescription": "Passmark Suite Latest",
+                "manufacturer": "Passmark",
+                "name": "Passmark Suite",
+                "operatingSystem": 0,
+                "upgradeSoftwareDescriptionId": None,
+                "upgradeSwDescId": None,
+                "version": "Latest",
+                "virtualLicense": 0,
+                "virtualizationPlatform": 0
+            }
+        }
+    }
+]
+getBillingItem = getObject['billingItem']
+getTagReferences = getObject['tagReferences']
+getNetworkVlans = getObject['networkVlans']
+getRemoteManagementAccounts = getObject['remoteManagementAccounts']
+
+
+# Setup for hardwareManager.clear_vlan related tests
+getObjectVlanClear = {
+    'backendNetworkComponent': getBackendNetworkComponents,
+    'frontendNetworkComponent': getFrontendNetworkComponents
+}
+getObjectVlanClear['backendNetworkComponent'][1]['networkVlanTrunks'] = [{'id': 99}]
+getObjectVlanClear['frontendNetworkComponent'][1]['networkVlanTrunks'] = [{'id': 11}]
```

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Location_Group.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Location_Group.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Metric_Tracking_Object.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Metric_Tracking_Object.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Routing_Method.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Routing_Method.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_VirtualIpAddress.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_VirtualIpAddress.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Bandwidth_Version1_Allotment.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Bandwidth_Version1_Allotment.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Mapping.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Mapping.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Mapping_Path.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Mapping_Path.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Component_Firewall.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Component_Firewall.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_LBaaS_L7Pool.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_LBaaS_L7Pool.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_LBaaS_Listener.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_LBaaS_Listener.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_LBaaS_LoadBalancer.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_LBaaS_LoadBalancer.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Message_Delivery_Email_Sendgrid.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Message_Delivery_Email_Sendgrid.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Pod.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Pod.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_SecurityGroup.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_SecurityGroup.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Storage.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Storage.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Storage_Allowed_Host.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Storage_Allowed_Host.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Storage_Hub_Cleversafe_Account.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Storage_Hub_Cleversafe_Account.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Storage_Iscsi.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Storage_Iscsi.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Subnet.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Subnet.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Subnet_IpAddress.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Subnet_IpAddress.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Vlan.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Vlan.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Network_Vlan_Firewall.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Network_Vlan_Firewall.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Notification_Occurrence_Event.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Notification_Occurrence_Event.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Product_Order.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Product_Order.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Product_Package.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Product_Package.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Product_Package_Preset.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Product_Package_Preset.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Provisioning_Maintenance_Window.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Provisioning_Maintenance_Window.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Scale_Group.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Scale_Group.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Scale_Policy.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Scale_Policy.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Security_Certificate.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Security_Certificate.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Software_AccountLicense.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Software_AccountLicense.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Tag.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Tag.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Ticket.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Ticket.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_User_Customer.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_User_Customer.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_User_Customer_CustomerPermission_Permission.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_User_Customer_CustomerPermission_Permission.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_User_Customer_Notification_Hardware.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_User_Customer_Notification_Hardware.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_User_Customer_Notification_Virtual_Guest.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_User_Customer_Notification_Virtual_Guest.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_User_Permission_Action.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_User_Permission_Action.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Virtual_DedicatedHost.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Virtual_DedicatedHost.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Virtual_Guest.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Virtual_Guest.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Virtual_Guest_Block_Device_Template_Group.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Virtual_Guest_Block_Device_Template_Group.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Virtual_Host.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Virtual_Host.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Virtual_PlacementGroup.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Virtual_PlacementGroup.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/fixtures/SoftLayer_Virtual_ReservedCapacityGroup.py` & `softlayer-6.2.0/SoftLayer/fixtures/SoftLayer_Virtual_ReservedCapacityGroup.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/__init__.py` & `softlayer-6.2.0/SoftLayer/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/account.py` & `softlayer-6.2.0/SoftLayer/managers/account.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/bandwidth.py` & `softlayer-6.2.0/SoftLayer/managers/bandwidth.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/block.py` & `softlayer-6.2.0/SoftLayer/managers/block.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/cdn.py` & `softlayer-6.2.0/SoftLayer/managers/cdn.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/dedicated_host.py` & `softlayer-6.2.0/SoftLayer/managers/dedicated_host.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/dns.py` & `softlayer-6.2.0/SoftLayer/managers/dns.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/email.py` & `softlayer-6.2.0/SoftLayer/managers/email.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/event_log.py` & `softlayer-6.2.0/SoftLayer/managers/event_log.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/file.py` & `softlayer-6.2.0/SoftLayer/managers/file.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/firewall.py` & `softlayer-6.2.0/SoftLayer/managers/firewall.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/hardware.py` & `softlayer-6.2.0/SoftLayer/managers/hardware.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
     SoftLayer.hardware
     ~~~~~~~~~~~~~~~~~~
     Hardware Manager/helpers
 
     :license: MIT, see LICENSE for more details.
 """
+import concurrent.futures as cf
 import datetime
 import logging
 import socket
 import time
 
 from SoftLayer.decoration import retry
 from SoftLayer import exceptions
@@ -16,15 +17,15 @@
 from SoftLayer.managers import ordering
 from SoftLayer.managers.ticket import TicketManager
 from SoftLayer import utils
 
 LOGGER = logging.getLogger(__name__)
 
 # Invalid names are ignored due to long method names and short argument names
-# pylint: disable=invalid-name, too-many-lines
+# pylint: disable=invalid-name, too-many-lines, too-many-public-methods
 
 EXTRA_CATEGORIES = ['pri_ipv6_addresses',
                     'static_ipv6_addresses',
                     'sec_ip_addresses',
                     'trusted_platform_module',
                     'software_guard_extensions']
 
@@ -272,14 +273,105 @@
                 'networkVlans[id,vlanNumber,networkSpace, fullyQualifiedName,primarySubnets[ipAddresses]],'
                 'monitoringServiceComponent,networkMonitors[queryType,lastResult,responseAction],'
                 'remoteManagementAccounts[username,password]'
             )
 
         return self.hardware.getObject(id=hardware_id, **kwargs)
 
+    @retry(logger=LOGGER)
+    def get_hardware_fast(self, hardware_id):
+        """Get details about a hardware device. Similar to get_hardware() but this uses threads
+
+        :param integer id: the hardware ID
+        :returns: A dictionary containing a large amount of information about the specified server.
+        """
+
+        hw_mask = (
+            'id, globalIdentifier, fullyQualifiedDomainName, hostname, domain,'
+            'provisionDate, hardwareStatus, bareMetalInstanceFlag, processorPhysicalCoreAmount,'
+            'memoryCapacity, notes, privateNetworkOnlyFlag, primaryBackendIpAddress,'
+            'primaryIpAddress, networkManagementIpAddress, userData, datacenter, hourlyBillingFlag,'
+            'lastTransaction[transactionGroup], hardwareChassis[id,name]'
+        )
+        server = self.client.call('SoftLayer_Hardware_Server', 'getObject', id=hardware_id, mask=hw_mask)
+        with cf.ThreadPoolExecutor(max_workers=10) as executor:
+            networkComponentsMask = (
+                "id, status, speed, maxSpeed, name, ipmiMacAddress, ipmiIpAddress, macAddress, primaryIpAddress,"
+                "port, primarySubnet[id, netmask, broadcastAddress, networkIdentifier, gateway],"
+                "uplinkComponent[networkVlanTrunks[networkVlan[networkSpace]]]"
+            )
+            networkComponents = executor.submit(
+                self.client.call, 'SoftLayer_Hardware_Server', 'getNetworkComponents',
+                id=hardware_id, mask=networkComponentsMask
+            )
+            activeComponentsMask = (
+               'id,hardwareComponentModel[hardwareGenericComponentModel[id,hardwareComponentType[keyName]]]'
+            )
+            activeComponents = executor.submit(
+                self.client.call, 'SoftLayer_Hardware_Server', 'getActiveComponents',
+                id=hardware_id, mask=activeComponentsMask
+            )
+
+            activeTransaction = executor.submit(
+                self.client.call, 'SoftLayer_Hardware_Server', 'getActiveTransaction',
+                id=hardware_id, mask="id, transactionStatus[friendlyName,name]"
+            )
+
+            operatingSystemMask = (
+                'softwareLicense[softwareDescription[manufacturer, name, version, referenceCode]],'
+                'passwords[id,username,password]'
+            )
+            operatingSystem = executor.submit(
+                self.client.call, 'SoftLayer_Hardware_Server', 'getOperatingSystem',
+                id=hardware_id, mask=operatingSystemMask
+            )
+
+            # Intentionally reusing the operatingSystemMask here. They are both softwareComponents
+            softwareComponents = executor.submit(
+                self.client.call, 'SoftLayer_Hardware_Server', 'getSoftwareComponents',
+                id=hardware_id, mask=operatingSystemMask
+            )
+
+            billingItemMask = (
+                'id,nextInvoiceTotalRecurringAmount,'
+                'nextInvoiceChildren[nextInvoiceTotalRecurringAmount],'
+                'orderItem.order.userRecord[username]'
+            )
+            billingItem = executor.submit(
+                self.client.call, 'SoftLayer_Hardware_Server', 'getBillingItem',
+                id=hardware_id, mask=billingItemMask
+            )
+
+            tagReferences = executor.submit(
+                self.client.call, 'SoftLayer_Hardware_Server', 'getTagReferences',
+                id=hardware_id, mask="id,tag[name,id]"
+            )
+
+            networkVlans = executor.submit(
+                self.client.call, 'SoftLayer_Hardware_Server', 'getNetworkVlans',
+                id=hardware_id, mask="id,vlanNumber,networkSpace,fullyQualifiedName,primarySubnets[ipAddresses]"
+            )
+
+            remoteManagementAccounts = executor.submit(
+                self.client.call, 'SoftLayer_Hardware_Server', 'getRemoteManagementAccounts',
+                id=hardware_id, mask="username,password"
+            )
+
+            server['networkComponents'] = networkComponents.result()
+            server['activeComponents'] = activeComponents.result()
+            server['activeTransaction'] = activeTransaction.result()
+            server['operatingSystem'] = operatingSystem.result()
+            server['softwareComponents'] = softwareComponents.result()
+            server['billingItem'] = billingItem.result()
+            server['networkVlans'] = networkVlans.result()
+            server['remoteManagementAccounts'] = remoteManagementAccounts.result()
+            server['tagReferences'] = tagReferences.result()
+
+        return server
+
     def reload(self, hardware_id, post_uri=None, ssh_keys=None, lvm=False):
         """Perform an OS reload of a server with its current configuration.
 
         https://sldn.softlayer.com/reference/datatypes/SoftLayer_Container_Hardware_Server_Configuration/
         :param integer hardware_id: the instance ID to reload
         :param string post_uri: The URI of the post-install script to run after reload
         :param list ssh_keys: The SSH keys to add to the root user
@@ -627,52 +719,54 @@
             obj['notes'] = notes
 
         if not obj:
             return True
 
         return self.hardware.editObject(obj, id=hardware_id)
 
-    def update_firmware(self,
-                        hardware_id,
-                        ipmi=True,
-                        raid_controller=True,
-                        bios=True,
-                        hard_drive=True):
+    def update_firmware(self, hardware_id: int,
+                        ipmi: bool = True,
+                        raid_controller: bool = True,
+                        bios: bool = True,
+                        hard_drive: bool = True,
+                        network: bool = True):
         """Update hardware firmware.
 
         This will cause the server to be unavailable for ~20 minutes.
+        https://sldn.softlayer.com/reference/services/SoftLayer_Hardware_Server/createFirmwareUpdateTransaction/
 
-        :param int hardware_id: The ID of the hardware to have its firmware
-                                updated.
+        :param int hardware_id: The ID of the hardware to have its firmware updated.
         :param bool ipmi: Update the ipmi firmware.
         :param bool raid_controller: Update the raid controller firmware.
         :param bool bios: Update the bios firmware.
         :param bool hard_drive: Update the hard drive firmware.
+        :param bool network: Update the network card firmware
 
         Example::
 
             # Check the servers active transactions to see progress
             result = mgr.update_firmware(hardware_id=1234)
         """
 
-        return self.hardware.createFirmwareUpdateTransaction(
-            bool(ipmi), bool(raid_controller), bool(bios), bool(hard_drive), id=hardware_id)
+        return self.client.call(
+            'SoftLayer_Hardware_Server', 'createFirmwareUpdateTransaction',
+            bool(ipmi), bool(raid_controller), bool(bios), bool(hard_drive), bool(network), id=hardware_id
+        )
 
-    def reflash_firmware(self,
-                         hardware_id,
-                         ipmi=True,
-                         raid_controller=True,
-                         bios=True):
+    def reflash_firmware(self, hardware_id: int,
+                         ipmi: bool = True,
+                         raid_controller: bool = True,
+                         bios: bool = True,):
         """Reflash hardware firmware.
 
         This will cause the server to be unavailable for ~60 minutes.
         The firmware will not be upgraded but rather reflashed to the version installed.
+        https://sldn.softlayer.com/reference/services/SoftLayer_Hardware_Server/createFirmwareReflashTransaction/
 
-        :param int hardware_id: The ID of the hardware to have its firmware
-                                reflashed.
+        :param int hardware_id: The ID of the hardware to have its firmware reflashed.
         :param bool ipmi: Reflash the ipmi firmware.
         :param bool raid_controller: Reflash the raid controller firmware.
         :param bool bios: Reflash the bios firmware.
 
         Example::
 
             # Check the servers active transactions to see progress
@@ -1068,30 +1162,79 @@
         if not filter_component:
             filter_component = {"components": {
                 "hardwareComponentModel": {
                     "firmwares": {
                         "createDate": {
                             "operation": "orderBy",
                             "options": [
-                                {
-                                    "name": "sort",
-                                    "value": [
-                                        "DESC"
-                                    ]
-                                },
-                                {
-                                    "name": "sortOrder",
-                                    "value": [
-                                        1
-                                    ]}]}
-                    }}}}
+                                {"name": "sort", "value": ["DESC"]},
+                                {"name": "sortOrder", "value": [1]}
+                            ]
+                        }
+                    }
+                }}}
 
         return self.client.call('Hardware_Server', 'getComponents',
                                 mask=mask, filter=filter_component, id=hardware_id)
 
+    def get_network_components(self, hardware_id, mask=None, space=None):
+        """Calls SoftLayer_Hardware_Server::getNetworkComponents()
+
+        :param int hardware_id: SoftLayer_Hardware_Server id
+        :param string mask: The object mask to use if you do not want the default
+        :param string space: 'public', 'private', or None for both.
+        :returns: https://sldn.softlayer.com/reference/datatypes/SoftLayer_Network_Component/
+        """
+
+        if mask is None:
+            mask = "mask[uplinkComponent, router, redundancyEnabledFlag, redundancyCapableFlag]"
+        method = "getNetworkComponents"
+        if space == "public":
+            method = "getFrontendNetworkComponents"
+        elif space == "private":
+            method = "getBackendNetworkComponents"
+        return self.client.call("SoftLayer_Hardware_Server", method, id=hardware_id, mask=mask)
+
+    def trunk_vlan(self, component_id, vlans):
+        """Calls SoftLayer_Network_Component::addNetworkVlanTrunks()
+
+        :param int component_id: SoftLayer_Network_Component id
+        :param list vlans: list of SoftLayer_Network_Vlan objects to add. Each object needs at least id or vlanNumber
+        """
+        return self.client.call('SoftLayer_Network_Component', 'addNetworkVlanTrunks', vlans, id=component_id)
+
+    def remove_vlan(self, component_id, vlans):
+        """Calls SoftLayer_Network_Component::removeNetworkVlanTrunks()
+
+        :param int component_id: SoftLayer_Network_Component id
+        :param list vlans: list of SoftLayer_Network_Vlan objects to remove. Each object needs at least id or vlanNumber
+        """
+        return self.client.call('SoftLayer_Network_Component', 'removeNetworkVlanTrunks', vlans, id=component_id)
+
+    def clear_vlan(self, hardware_id):
+        """Clears all vlan trunks from a hardware_id
+
+        :param int hardware_id: server to clear vlans from
+        """
+        component_mask = (
+            "mask[id, "
+            "backendNetworkComponents[id,networkVlanTrunks[networkVlanId]], "
+            "frontendNetworkComponents[id,networkVlanTrunks[networkVlanId]]"
+            "]"
+        )
+        components = self.client.call('SoftLayer_Hardware_Server', 'getObject', id=hardware_id, mask=component_mask)
+        # We only want to call this API on components with actual trunks.
+        # Calling this on the primary and redundant components might cause exceptions.
+        for c in components.get('backendNetworkComponent', []):
+            if len(c.get('networkVlanTrunks', [])):
+                self.client.call('SoftLayer_Network_Component', 'clearNetworkVlanTrunks', id=c.get('id'))
+        for c in components.get('frontendNetworkComponent', []):
+            if len(c.get('networkVlanTrunks', [])):
+                self.client.call('SoftLayer_Network_Component', 'clearNetworkVlanTrunks', id=c.get('id'))
+
     def get_sensors(self, hardware_id):
         """Returns Hardware sensor data"""
         return self.client.call('Hardware', 'getSensorData', id=hardware_id)
 
     def get_notifications(self, hardware_id):
         """Returns all hardware notifications."""
         return self.client.call('SoftLayer_User_Customer_Notification_Hardware', 'findByHardwareId', hardware_id)
```

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/image.py` & `softlayer-6.2.0/SoftLayer/managers/image.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/ipsec.py` & `softlayer-6.2.0/SoftLayer/managers/ipsec.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/license.py` & `softlayer-6.2.0/SoftLayer/managers/license.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """
     SoftLayer.license
-    ~~~~~~~~~~~~~~~
+    ~~~~~~~~~~~~~~~~~
     License Manager
 
     :license: MIT, see LICENSE for more details.
 """
 
 # pylint: disable=too-many-public-methods
 from SoftLayer.CLI import exceptions
 from SoftLayer.managers import ordering
 from SoftLayer import utils
 
+LICENSE_PACKAGE_ID = 301
+
 
 class LicensesManager(object):
     """Manages account license."""
 
     def __init__(self, client):
         self.client = client
 
@@ -59,7 +61,11 @@
         complex_type = 'SoftLayer_Container_Product_Order_Software_License'
         ordering_manager = ordering.OrderingManager(self.client)
         return ordering_manager.place_order(package_keyname='SOFTWARE_LICENSE_PACKAGE',
                                             location=datacenter,
                                             item_keynames=item_package,
                                             complex_type=complex_type,
                                             hourly=False)
+
+    def get_create_options(self):
+        """Returns valid options for ordering Licenses."""
+        return self.client.call('SoftLayer_Product_Package', 'getItems', id=LICENSE_PACKAGE_ID)
```

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/load_balancer.py` & `softlayer-6.2.0/SoftLayer/managers/load_balancer.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/metadata.py` & `softlayer-6.2.0/SoftLayer/managers/metadata.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/network.py` & `softlayer-6.2.0/SoftLayer/managers/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
     def __init__(self, client):
         self.client = client
         self.account = client['Account']
         self.vlan = client['Network_Vlan']
         self.subnet = client['Network_Subnet']
         self.network_storage = self.client['Network_Storage']
         self.security_group = self.client['Network_SecurityGroup']
+        self.resolvers = [self.search_for_vlan]
 
     def add_global_ip(self, version=4, test_order=False):
         """Adds a global IP address to the account.
 
         :param int version: Specifies whether this is IPv4 or IPv6
         :param bool test_order: If true, this will only verify the order.
         """
@@ -510,54 +511,45 @@
             _filter['subnets']['networkVlan']['networkSpace'] = (
                 utils.query_filter(network_space))
 
         kwargs['filter'] = _filter.to_dict()
         kwargs['iter'] = True
         return self.client.call('Account', 'getSubnets', **kwargs)
 
-    def list_vlans(self, datacenter=None, vlan_number=None, name=None, limit=100, **kwargs):
+    def list_vlans(self, datacenter=None, vlan_number=None, name=None, limit=100, mask=None, _filter=None):
         """Display a list of all VLANs on the account.
 
         This provides a quick overview of all VLANs including information about
         data center residence and the number of devices attached.
 
-        :param string datacenter: If specified, the list will only contain
-                                    VLANs in the specified data center.
-        :param int vlan_number: If specified, the list will only contain the
-                                  VLAN matching this VLAN number.
-        :param int name: If specified, the list will only contain the
-                                  VLAN matching this VLAN name.
+        :param string datacenter: If specified, the list will only contain  VLANs in the specified data center.
+        :param int vlan_number: If specified, the list will only contain the VLAN matching this VLAN number.
+        :param int name: If specified, the list will only contain the VLAN matching this VLAN name.
         :param dict \\*\\*kwargs: response-level options (mask, limit, etc.)
 
         """
-        _filter = utils.NestedDict(kwargs.get('filter') or {})
+        _filter = utils.NestedDict(_filter or {})
 
         _filter['networkVlans']['id'] = utils.query_filter_orderby()
 
         if vlan_number:
-            _filter['networkVlans']['vlanNumber'] = (
-                utils.query_filter(vlan_number))
+            _filter['networkVlans']['vlanNumber'] = utils.query_filter(vlan_number)
 
         if name:
             _filter['networkVlans']['name'] = utils.query_filter(name)
 
         if datacenter:
-            _filter['networkVlans']['primaryRouter']['datacenter']['name'] = (
-                utils.query_filter(datacenter))
+            _filter['networkVlans']['primaryRouter']['datacenter']['name'] = utils.query_filter(datacenter)
 
-        kwargs['filter'] = _filter.to_dict()
+        if mask is None:
+            mask = DEFAULT_VLAN_MASK
 
-        if 'mask' not in kwargs:
-            kwargs['mask'] = DEFAULT_VLAN_MASK
-
-        kwargs['iter'] = True
-        if limit > 0:
-            return self.account.getNetworkVlans(mask=kwargs['mask'], filter=_filter.to_dict(), limit=limit, iter=True)
-        else:
-            return self.account.getNetworkVlans(mask=kwargs['mask'], filter=_filter.to_dict(), iter=True)
+        # cf_call uses threads to get all results.
+        return self.client.cf_call('SoftLayer_Account', 'getNetworkVlans',
+                                   mask=mask, filter=_filter.to_dict(), limit=limit)
 
     def list_securitygroups(self, **kwargs):
         """List security groups."""
         kwargs['iter'] = True
         return self.security_group.getAllObjects(**kwargs)
 
     def list_securitygroup_rules(self, group_id):
@@ -883,7 +875,21 @@
 
     def clear_route(self, identifier):
         """Calls SoftLayer_Network_Subnet::clearRoute()
 
         returns  true or false.
         """
         return self.client.call('SoftLayer_Network_Subnet', 'clearRoute', id=identifier)
+
+    def search_for_vlan(self, vlan):
+        """Returns a list of matching VLAN objects.
+
+        :param string vlan: Could be either vlan name, number, id, or fully qualified name
+        :return list: List of SoftLayer_Network_Vlan objects
+        """
+
+        query = f"_objectType:SoftLayer_Network_Vlan {vlan}"
+        mask = "mask[resource(SoftLayer_Network_Vlan)[id,name,vlanNumber,fullyQualifiedName,networkSpace]]"
+
+        results = self.client.call('SoftLayer_Search', 'advancedSearch', query, mask=mask)
+        # This returns JUST the Network_Vlan information, none of the search information.
+        return [result.get('resource') for result in results]
```

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/object_storage.py` & `softlayer-6.2.0/SoftLayer/managers/object_storage.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/ordering.py` & `softlayer-6.2.0/SoftLayer/managers/ordering.py`

 * *Files 1% similar despite different names*

```diff
@@ -264,15 +264,15 @@
         If no packages are found, returns None
 
         :param package_keyname: string representing the package key name we are interested in.
         :param string mask: Mask to specify the properties we want to retrieve
         """
         _filter = {'keyName': {'operation': package_keyname}}
 
-        packages = self.package_svc.getAllObjects(mask=mask, filter=_filter)
+        packages = self.client.call('SoftLayer_Product_Package', 'getAllObjects', mask=mask, filter=_filter)
         if len(packages) == 0:
             raise exceptions.SoftLayerError(f"Package {package_keyname} does not exist")
 
         return packages.pop()
 
     def list_categories(self, package_keyname, **kwargs):
         """List the categories for the given package.
```

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/search.py` & `softlayer-6.2.0/SoftLayer/managers/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,16 +43,16 @@
         if kwargs.get('hostname'):
             search_string = f"{search_string} hostname: *{kwargs.get('hostname')}*"
         if kwargs.get('domain'):
             search_string = f"{search_string} domain: *{kwargs.get('domain')}*"
         if kwargs.get('datacenter'):
             search_string = f"{search_string} datacenter.longName: *{kwargs.get('datacenter')}*"
         if kwargs.get('tags'):
-            tags = " ".join(kwargs.get("tags", []))
-            search_string = f"{search_string} internalTagReferences.tag.name: {tags}"
+            tags = " ".join(f"tagReferences.tag.name: \"{t}\"" for t in kwargs.get("tags", []))
+            search_string = f"{search_string} {tags}"
         result = self.search_manager.advancedSearch(search_string, mask=mask)
         guests = []
         for resource in result:
             guests.append(resource.get('resource'))
 
         return guests
```

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/sshkey.py` & `softlayer-6.2.0/SoftLayer/managers/sshkey.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/ssl.py` & `softlayer-6.2.0/SoftLayer/managers/ssl.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/storage.py` & `softlayer-6.2.0/SoftLayer/managers/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
     SoftLayer.storage
-    ~~~~~~~~~~~~~~~
+    ~~~~~~~~~~~~~~~~~
     Network Storage Manager
 
     :license: MIT, see LICENSE for more details.
 """
 from SoftLayer import exceptions
 from SoftLayer.managers import storage_utils
 from SoftLayer import utils
@@ -309,19 +309,15 @@
             order['duplicateOriginSnapshotId'] = origin_snapshot_id
         if dependent_duplicate:
             # if isDependentDuplicateFlag is set to ANYTHING, it is considered dependent.
             order['isDependentDuplicateFlag'] = 1
 
         return self.client.call('Product_Order', 'placeOrder', order)
 
-    def order_modified_volume(self,
-                              volume_id,
-                              new_size=None,
-                              new_iops=None,
-                              new_tier_level=None):
+    def order_modified_volume(self, volume_id, new_size=None, new_iops=None, new_tier_level=None):
         """Places an order for modifying an existing block volume.
 
         :param volume_id: The ID of the volume to be modified
         :param new_size: The new size/capacity for the volume
         :param new_iops: The new IOPS for the volume
         :param new_tier_level: The new tier level for the volume
         :return: Returns a SoftLayer_Container_Product_Order_Receipt
```

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/storage_utils.py` & `softlayer-6.2.0/SoftLayer/managers/storage_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
     SoftLayer.storage_utils
-    ~~~~~~~~~~~~~~~
+    ~~~~~~~~~~~~~~~~~~~~~~~
     Utility functions used by File and Block Storage Managers
 
     :license: MIT, see LICENSE for more details.
 """
 from SoftLayer import exceptions
 from SoftLayer import utils
 
@@ -415,16 +415,15 @@
     :return: Returns an int value indicating the volume's snapshot schedule ID
     """
     for schedule in volume['schedules']:
         if 'type' in schedule and 'keyname' in schedule['type']:
             if schedule['type']['keyname'] == snapshot_schedule_keyname:
                 return schedule['id']
 
-    raise ValueError("The given snapshot schedule ID was not found for "
-                     "the given storage volume")
+    raise ValueError("The given snapshot schedule ID was not found for the given storage volume")
 
 
 def prepare_snapshot_order_object(manager, volume, capacity, tier, upgrade, iops):
     """Prepare the snapshot space order object for the placeOrder() method
 
     :param manager: The File or Block manager calling this function
     :param integer volume: The volume for which snapshot space is ordered
@@ -432,16 +431,15 @@
     :param float tier: The tier level of the volume, in IOPS per GB (optional)
     :param boolean upgrade: Flag to indicate if this order is an upgrade
     :return: Returns the order object for the
              Product_Order service's placeOrder() method
     """
     # Ensure the storage volume has not been cancelled
     if 'billingItem' not in volume:
-        raise exceptions.SoftLayerError(
-            'This volume has been cancelled; unable to order snapshot space')
+        raise exceptions.SoftLayerError('This volume has been cancelled; unable to order snapshot space')
 
     # Determine and validate the storage volume's billing item category
     billing_item_category_code = volume['billingItem']['categoryCode']
     if billing_item_category_code == 'storage_as_a_service':
         order_type_is_saas = True
     elif billing_item_category_code == 'storage_service_enterprise':
         order_type_is_saas = False
```

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/tags.py` & `softlayer-6.2.0/SoftLayer/managers/tags.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
     SoftLayer.tags
-    ~~~~~~~~~~~~
+    ~~~~~~~~~~~~~~
     Tag Manager
 
     :license: MIT, see LICENSE for more details.
 """
 import re
 
 from SoftLayer.exceptions import SoftLayerAPIError
@@ -79,26 +79,28 @@
         """Returns the SoftLayer Service for the corresponding type
 
         :param int resource_table_id: Tag_Reference::resourceTableId
         :param string tag_type: Tag_Reference->tagType->keyName
 
         From  SoftLayer_Tag::getAllTagTypes()
 
-        |Type                             |Service |
-        | -----------------------------   | ------ |
-        |Hardware                         |HARDWARE|
-        |CCI                              |GUEST|
-        |Account Document                 |ACCOUNT_DOCUMENT|
-        |Ticket                           |TICKET|
-        |Vlan Firewall                    |NETWORK_VLAN_FIREWALL|
-        |Contract                         |CONTRACT|
-        |Image Template                   |IMAGE_TEMPLATE|
-        |Application Delivery Controller  |APPLICATION_DELIVERY_CONTROLLER|
-        |Vlan                             |NETWORK_VLAN|
-        |Dedicated Host                   |DEDICATED_HOST|
+        ::
+
+            |Type                             |Service |
+            | -----------------------------   | ------ |
+            |Hardware                         |HARDWARE|
+            |CCI                              |GUEST|
+            |Account Document                 |ACCOUNT_DOCUMENT|
+            |Ticket                           |TICKET|
+            |Vlan Firewall                    |NETWORK_VLAN_FIREWALL|
+            |Contract                         |CONTRACT|
+            |Image Template                   |IMAGE_TEMPLATE|
+            |Application Delivery Controller  |APPLICATION_DELIVERY_CONTROLLER|
+            |Vlan                             |NETWORK_VLAN|
+            |Dedicated Host                   |DEDICATED_HOST|
         """
         service = self.type_to_service(tag_type)
         if service is None:
             raise SoftLayerAPIError(404, f"Unable to lookup {tag_type} types")
         return self.client.call(service, 'getObject', id=resource_table_id)
 
     def delete_tag(self, name):
```

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/ticket.py` & `softlayer-6.2.0/SoftLayer/managers/ticket.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/user.py` & `softlayer-6.2.0/SoftLayer/managers/user.py`

 * *Files 12% similar despite different names*

```diff
@@ -97,14 +97,15 @@
     def enable_notifications(self, notifications_names):
         """Enables a list of notifications for the current a user profile.
 
         :param list notifications_names: List of notifications names to enable
         :returns: True on success
 
         Example::
+
             enable_notifications(['Order Approved','Reload Complete'])
         """
 
         result = False
         notifications = self.gather_notifications(notifications_names)
         for notification in notifications:
             notification_id = notification.get('id')
@@ -116,14 +117,15 @@
     def disable_notifications(self, notifications_names):
         """Disable a list of notifications for the current a user profile.
 
         :param list notifications_names: List of notifications names to disable
         :returns: True on success
 
         Example::
+
             disable_notifications(['Order Approved','Reload Complete'])
         """
 
         result = False
         notifications = self.gather_notifications(notifications_names)
         for notification in notifications:
             notification_id = notification.get('id')
@@ -136,28 +138,30 @@
         """Enables a list of permissions for a user
 
         :param int id: user id to set
         :param list permissions: List of permissions keynames to enable
         :returns: True on success, Exception otherwise
 
         Example::
+
             add_permissions(123, ['BANDWIDTH_MANAGE'])
         """
         pretty_permissions = self.format_permission_object(permissions)
         LOGGER.warning("Adding the following permissions to %s: %s", user_id, pretty_permissions)
         return self.user_service.addBulkPortalPermission(pretty_permissions, id=user_id)
 
     def remove_permissions(self, user_id, permissions):
         """Disables a list of permissions for a user
 
         :param int id: user id to set
         :param list permissions: List of permissions keynames to disable
         :returns: True on success, Exception otherwise
 
         Example::
+
             remove_permissions(123, ['BANDWIDTH_MANAGE'])
         """
         pretty_permissions = self.format_permission_object(permissions)
         LOGGER.warning("Removing the following permissions to %s: %s", user_id, pretty_permissions)
         return self.user_service.removeBulkPortalPermission(pretty_permissions, id=user_id)
 
     def permissions_from_user(self, user_id, from_user_id):
@@ -192,15 +196,17 @@
 
     def get_logins(self, user_id, start_date=None):
         """Gets the login history for a user, default start_date is 30 days ago
 
         :param int id: User id to get
         :param string start_date: "%m/%d/%Y %H:%M:%s" formatted string.
         :returns: list https://softlayer.github.io/reference/datatypes/SoftLayer_User_Customer_Access_Authentication/
+
         Example::
+
             get_logins(123, '04/08/2018 0:0:0')
         """
 
         if start_date is None:
             date_object = datetime.datetime.today() - datetime.timedelta(days=30)
             start_date = date_object.strftime("%m/%d/%Y 0:0:0")
 
@@ -362,15 +368,14 @@
         return self.edit_user(user_id, user_object)
 
     def vpn_enable_or_disable(self, user_id, value):
         """Enable or Disable vpn for a user.
 
         :param int user_id: User to edit.
         :param bool value: Value for vpn enable flag.
-        or
         :param bool value: Value for vpn disable flag.
         """
         user_object = {'sslVpnAllowedFlag': value}
         return self.edit_user(user_id, user_object)
 
     def vpn_subnet_add(self, user_id, subnet_ids):
         """Add subnets for a user.
@@ -422,101 +427,94 @@
             overrides_list.append(matching_overrides)
 
         return overrides_list
 
     def grant_hardware_access(self, user_id, hardware_id):
         """Grants the user access to a single hardware device.
 
-        :param int user_id:
-        :param int hardware_id
-
+        :param int user_id: User Id
+        :param int hardware_id: Hardware Id
         :returns: true
         """
         return self.user_service.addHardwareAccess(hardware_id, id=user_id)
 
     def grant_virtual_access(self, user_id, virtual_id):
         """Grants the user access to a single VS device.
 
-        :param int user_id:
-        :param int virtual_id
-
+        :param int user_id: User Id
+        :param int virtual_id: Hardware Id
         :returns: true
         """
         return self.user_service.addVirtualGuestAccess(virtual_id, id=user_id)
 
     def grant_dedicated_access(self, user_id, dedicated_id):
         """Grants the user access to a single dedicated host device.
 
-        :param int user_id:
-        :param int dedicated_id
-
+        :param int user_id: User Id
+        :param int dedicated_id: Dedicatd Host Id
         :returns: true
         """
         return self.user_service.addDedicatedHostAccess(dedicated_id, id=user_id)
 
     def remove_hardware_access(self, user_id, hardware_id):
         """Remove hardware from a portal user’s hardware access list.
 
-        :param int user_id:
-        :param int hardware_id
-
+        :param int user_id: User Id
+        :param int hardware_id: Hardware Id
         :returns: true
         """
         return self.user_service.removeHardwareAccess(hardware_id, id=user_id)
 
     def remove_virtual_access(self, user_id, virtual_id):
         """Remove hardware from a portal user’s virtual guests access list.
 
-        :param int user_id:
-        :param int hardware_id
-
+        :param int user_id: User Id
+        :param int hardware_id: Hardware Id
         :returns: true
         """
         return self.user_service.removeVirtualGuestAccess(virtual_id, id=user_id)
 
     def remove_dedicated_access(self, user_id, dedicated_id):
         """Remove hardware from a portal user’s dedicated host access list.
 
-        :param int user_id:
-        :param int dedicated_id
-
+        :param int user_id: User Id
+        :param int dedicated_id: Dedicated Host Id
         :returns: true
         """
         return self.user_service.removeDedicatedHostAccess(dedicated_id, id=user_id)
 
     def get_user_hardware(self, user_id):
         """User Hardware list.
 
-        :param int user_id:
+        :param int user_id: User Id
         :return: List hardware relate to user
         """
         return self.user_service.getHardware(id=user_id)
 
     def get_user_dedicated_host(self, user_id):
         """User dedicate host list.
 
-        :param int user_id:
+        :param int user_id: User Id
         :return: List dedicated host relate to user
         """
         return self.user_service.getDedicatedHosts(id=user_id)
 
     def get_user_virtuals(self, user_id):
         """User virtual guest list.
 
-        :param int user_id:
+        :param int user_id: User Id
         :return: List virtual guest relate to user
         """
         return self.user_service.getVirtualGuests(id=user_id)
 
     def update_vpn_password(self, user_id, password):
         """Update a user's VPN password.
 
-        :param int user_id:
-        :param string password:
-
+        :param int user_id: User Id
+        :param string password: Password
         :returns: true
         """
         return self.user_service.updateVpnPassword(password, id=user_id)
 
 
 def _keyname_search(haystack, needle):
     for item in haystack:
```

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/vs.py` & `softlayer-6.2.0/SoftLayer/managers/vs.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
             elif monthly:
                 call = 'getMonthlyVirtualGuests'
 
         _filter = utils.NestedDict(kwargs.get('filter') or {})
         if tags:
             _filter['virtualGuests']['tagReferences']['tag']['name'] = {
                 'operation': 'in',
-                'options': [{'name': 'data', 'value': tags}],
+                'options': [{'name': 'data', 'value': list(tags)}],
             }
 
         if cpus:
             _filter['virtualGuests']['maxCpu'] = utils.query_filter(cpus)
 
         if memory:
             _filter['virtualGuests']['maxMemory'] = utils.query_filter(memory)
@@ -1044,33 +1044,28 @@
         }
 
         if disk:
             disk_number = 0
             vsi_disk = self.get_instance(instance_id)
             for item in vsi_disk.get('billingItem').get('children'):
                 if 'guest_disk' in item.get('categoryCode'):
-                    if disk_number < int("".join(filter(str.isdigit, item.get('categoryCode')))):
-                        disk_number = int("".join(filter(str.isdigit, item.get('categoryCode'))))
+                    disk_number = max(disk_number, int("".join(filter(str.isdigit, item.get('categoryCode')))))
             for disk_guest in disk:
                 if disk_guest.get('number') > 0:
-                    price_id = self._get_price_id_for_upgrade_option(upgrade_prices, 'disk',
-                                                                     disk_guest.get('capacity'),
-                                                                     public)
                     disk_number = disk_guest.get('number')
-
                 else:
-                    price_id = self._get_price_id_for_upgrade_option(upgrade_prices, 'disk',
-                                                                     disk_guest.get('capacity'),
-                                                                     public)
                     disk_number = disk_number + 1
+                price_id = self._get_price_id_for_upgrade_option(upgrade_prices,
+                                                                 'disk',
+                                                                 disk_guest.get('capacity'),
+                                                                 public)
 
                 if price_id is None:
-                    raise exceptions.SoftLayerAPIError(500,
-                                                       'Unable to find %s option with value %s' % (
-                                                           ('disk', disk_guest.get('capacity'))))
+                    error = f"Unable to find disk option with value {disk_guest.get('capacity')}"
+                    raise exceptions.SoftLayerAPIError(500, error)
 
                 category_id = self.get_disk_category_id_by_disk_number(disk_guest.get('capacity'), disk_number)
                 if category_id is None:
                     raise exceptions.SoftLayerError('Invalid disk number to this disk capacity')
                 category = {'categories': [{
                     'id': category_id,
                     'complexType': "SoftLayer_Product_Item_Category"}],
@@ -1079,18 +1074,15 @@
 
                 prices.append(category)
             order['prices'] = prices
 
         for option, value in data.items():
             if not value:
                 continue
-            price_id = self._get_price_id_for_upgrade_option(upgrade_prices,
-                                                             option,
-                                                             value,
-                                                             public)
+            price_id = self._get_price_id_for_upgrade_option(upgrade_prices, option, value, public)
             if not price_id:
                 # Every option provided is expected to have a price
                 raise exceptions.SoftLayerError(
                     "Unable to find %s option with value %s" % (option, value))
 
             prices.append({'id': price_id})
```

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/vs_capacity.py` & `softlayer-6.2.0/SoftLayer/managers/vs_capacity.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/managers/vs_placement.py` & `softlayer-6.2.0/SoftLayer/managers/vs_placement.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/shell/cmd_help.py` & `softlayer-6.2.0/SoftLayer/shell/cmd_help.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/shell/completer.py` & `softlayer-6.2.0/SoftLayer/shell/completer.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/shell/core.py` & `softlayer-6.2.0/SoftLayer/shell/core.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/testing/__init__.py` & `softlayer-6.2.0/SoftLayer/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/testing/xmlrpc.py` & `softlayer-6.2.0/SoftLayer/testing/xmlrpc.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 import SoftLayer
 from SoftLayer import transports
 from SoftLayer import utils
 
 # pylint: disable=invalid-name, broad-except, arguments-differ
 
 
-class TestServer(http.server.HTTPServer):
+class TestServer(http.server.ThreadingHTTPServer):
     """Test HTTP server which holds a given transport."""
 
     def __init__(self, transport, *args, **kw):
-        http.server.HTTPServer.__init__(self, *args, **kw)
+        http.server.ThreadingHTTPServer.__init__(self, *args, **kw)
         self.transport = transport
 
 
 class TestHandler(http.server.BaseHTTPRequestHandler):
     """Test XML-RPC Handler which converts XML-RPC to transport requests."""
 
     def do_POST(self):
```

### Comparing `SoftLayer-6.1.9/SoftLayer/transports/__init__.py` & `softlayer-6.2.0/SoftLayer/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/transports/debug.py` & `softlayer-6.2.0/SoftLayer/transports/debug.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/transports/fixture.py` & `softlayer-6.2.0/SoftLayer/transports/fixture.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/transports/rest.py` & `softlayer-6.2.0/SoftLayer/transports/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,14 @@
 
         if request.method is not None:
             url_parts.append(request.method)
 
         request.url = '%s.%s' % ('/'.join(url_parts), 'json')
 
         # Prefer the request setting, if it's not None
-
         if request.verify is None:
             request.verify = self.verify
 
         try:
             resp = self.client.request(method, request.url,
                                        auth=auth,
                                        headers=request.transport_headers,
```

### Comparing `SoftLayer-6.1.9/SoftLayer/transports/timing.py` & `softlayer-6.2.0/SoftLayer/transports/timing.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/SoftLayer/transports/transport.py` & `softlayer-6.2.0/SoftLayer/transports/transport.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,18 +52,20 @@
 
         #: Transport password.
         self.transport_password = None
 
         #: Transport headers.
         self.transport_headers = {}
 
-        #: Boolean specifying if the server certificate should be verified.
+        #: False -> Don't verify the SSL certificate
+        #: True -> Verify the SSL certificate
+        #: Path String -> Verify the SSL certificate with the .pem file at path
         self.verify = None
 
-        #: Client certificate file path.
+        #: Client certificate file path. (Used by X509Authentication)
         self.cert = None
 
         #: InitParameter/identifier of an object.
         self.identifier = None
 
         #: SoftLayer mask (dict or string).
         self.mask = None
@@ -95,17 +97,20 @@
         #: Exception any exceptions that got caught
         self.exception = None
 
     def __repr__(self):
         """Prints out what this call is all about"""
         pretty_mask = utils.clean_string(self.mask)
         pretty_filter = self.filter
-        param_string = "id={id}, mask='{mask}', filter='{filter}', args={args}, limit={limit}, offset={offset}".format(
-            id=self.identifier, mask=pretty_mask, filter=pretty_filter,
-            args=self.args, limit=self.limit, offset=self.offset)
+        clean_args = self.args
+        # Passwords can show up here, so censor them before logging.
+        if self.method in ["performExternalAuthentication", "refreshEncryptedToken", "getPortalLoginToken"]:
+            clean_args = "*************"
+        param_string = (f"id={self.identifier}, mask='{pretty_mask}', filter='{pretty_filter}', args={clean_args}, "
+                        f"limit={self.limit}, offset={self.offset}")
         return "{service}::{method}({params})".format(
             service=self.service, method=self.method, params=param_string)
 
 
 class SoftLayerListResult(list):
     """A SoftLayer API list result."""
```

### Comparing `SoftLayer-6.1.9/SoftLayer/transports/xmlrpc.py` & `softlayer-6.2.0/SoftLayer/transports/xmlrpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,16 +80,15 @@
         request.url = '/'.join([self.endpoint_url, request.service])
         request.payload = xmlrpc.client.dumps(tuple(largs),
                                               methodname=request.method,
                                               allow_none=True,
                                               encoding="iso-8859-1")
 
         # Prefer the request setting, if it's not None
-        verify = request.verify
-        if verify is None:
+        if request.verify is None:
             request.verify = self.verify
 
         try:
             resp = self.client.request('POST', request.url,
                                        data=request.payload.encode(),
                                        auth=auth,
                                        headers=request.transport_headers,
```

### Comparing `SoftLayer-6.1.9/SoftLayer/utils.py` & `softlayer-6.2.0/SoftLayer/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,15 +269,15 @@
 
     :param string identifier: identifier string
     :param list resolvers: a list of functions
     :returns list:
     """
 
     # Before doing anything, let's see if this is an integer
-    if type(identifier) == int:
+    if isinstance(identifier, int):
         return [int(identifier)]
     # It was worth a shot
 
     elif len(identifier) == 36 and UUID_RE.match(identifier):
         return [identifier]
     for resolver in resolvers:
         ids = resolver(identifier)
@@ -470,15 +470,15 @@
         pos = match.start()
         obj, pos = decoder.raw_decode(document, pos)
 
         yield obj
 
 
 def console_color_themes(theme):
-    """Colors in https://rich.readthedocs.io/en/stable/appendix/colors.html?highlight=light_pink1#standard-colors"""
+    """Colors in https://rich.readthedocs.io/en/stable/appendix/colors.html#standard-colors"""
 
     if theme == 'light':
         return Console(theme=Theme(
             {
                 "options": "bold dark_cyan",  # OPTIONS
                 "command": "orange3",  # COMMAND
                 "args": "bold dark_cyan",  # ARGS
@@ -486,16 +486,18 @@
                 "name_sub_command": "orange3",  # sub command name
                 "sub_command": "orange3",  # sub command list
                 # Help table colors options
                 "option": "bold dark_cyan",
                 "switch": "bold green4",
                 "default_option": "light_coral",
                 "option_keyword": "bold dark_cyan",
-                "args_keyword": "bold green4",
+                "args_keyword": "underline orange4",
                 "option_choices": "gold3",
+                "example_block": "underline deep_pink3",
+                "url": "underline blue",
             })
         )
     return Console(theme=Theme(
         {
             "options": "bold cyan",  # OPTIONS
             "command": "orange3",  # COMMAND
             "args": "bold cyan",  # ARGS
@@ -503,16 +505,18 @@
             "name_sub_command": "orange3",  # sub command name
             "sub_command": "orange3",  # sub command list
             # Help table colors options
             "option": "bold cyan",
             "switch": "bold green",
             "default_option": "light_pink1",
             "option_keyword": "bold cyan",
-            "args_keyword": "bold green",
+            "args_keyword": "underline yellow",
             "option_choices": "gold3",
+            "example_block": "underline light_coral",
+            "url": "underline blue",
         })
     )
 
 
 def table_color_theme(theme):
     """Define result table colors"""
     if theme == 'light':
```

### Comparing `SoftLayer-6.1.9/SoftLayer.egg-info/PKG-INFO` & `softlayer-6.2.0/SoftLayer.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,59 +1,52 @@
 Metadata-Version: 2.1
 Name: SoftLayer
-Version: 6.1.9
+Version: 6.2.0
 Summary: A library for SoftLayer's API
-Home-page: http://github.com/softlayer/softlayer-python
+Home-page: https://github.com/SoftLayer/softlayer-python
 Author: SoftLayer, Inc., an IBM Company
 Author-email: SLDNDeveloperRelations@wwpdl.vnet.ibm.com
 License: MIT
-Keywords: softlayer,cloud,slcli
+Keywords: softlayer,cloud,slcli,ibmcloud
 Classifier: Environment :: Console
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: prettytable>=2.5.0
 Requires-Dist: click>=8.0.4
 Requires-Dist: requests>=2.20.0
 Requires-Dist: prompt_toolkit>=2
 Requires-Dist: pygments>=2.0.0
 Requires-Dist: urllib3>=1.24
-Requires-Dist: rich==13.5.3
+Requires-Dist: rich==13.7.1
 
 SoftLayer API Python Client
 ===========================
 .. image:: https://github.com/softlayer/softlayer-python/workflows/Tests/badge.svg
     :target: https://github.com/softlayer/softlayer-python/actions?query=workflow%3ATests
-
 .. image:: https://github.com/softlayer/softlayer-python/workflows/documentation/badge.svg
     :target: https://github.com/softlayer/softlayer-python/actions?query=workflow%3Adocumentation
-
-.. image:: https://landscape.io/github/softlayer/softlayer-python/master/landscape.svg
-    :target: https://landscape.io/github/softlayer/softlayer-python/master
-
 .. image:: https://badge.fury.io/py/SoftLayer.svg
     :target: http://badge.fury.io/py/SoftLayer
-
 .. image:: https://coveralls.io/repos/github/softlayer/softlayer-python/badge.svg?branch=master
     :target: https://coveralls.io/github/softlayer/softlayer-python?branch=master
-
 .. image:: https://snapcraft.io//slcli/badge.svg
     :target: https://snapcraft.io/slcli
 
 
 This library provides a simple Python client to interact with `SoftLayer's
 XML-RPC API <https://softlayer.github.io/reference/softlayerapi>`_.
```

### Comparing `SoftLayer-6.1.9/SoftLayer.egg-info/SOURCES.txt` & `softlayer-6.2.0/SoftLayer.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 SoftLayer/CLI/command.py
 SoftLayer/CLI/core.py
 SoftLayer/CLI/custom_types.py
 SoftLayer/CLI/environment.py
 SoftLayer/CLI/exceptions.py
 SoftLayer/CLI/formatting.py
 SoftLayer/CLI/helpers.py
+SoftLayer/CLI/login.py
 SoftLayer/CLI/metadata.py
 SoftLayer/CLI/routes.py
 SoftLayer/CLI/search.py
 SoftLayer/CLI/storage_utils.py
 SoftLayer/CLI/summary.py
 SoftLayer/CLI/template.py
 SoftLayer/CLI/account/__init__.py
@@ -212,14 +213,17 @@
 SoftLayer/CLI/hardware/reflash_firmware.py
 SoftLayer/CLI/hardware/reload.py
 SoftLayer/CLI/hardware/sensor.py
 SoftLayer/CLI/hardware/storage.py
 SoftLayer/CLI/hardware/toggle_ipmi.py
 SoftLayer/CLI/hardware/update_firmware.py
 SoftLayer/CLI/hardware/upgrade.py
+SoftLayer/CLI/hardware/vlan_add.py
+SoftLayer/CLI/hardware/vlan_remove.py
+SoftLayer/CLI/hardware/vlan_trunkable.py
 SoftLayer/CLI/image/__init__.py
 SoftLayer/CLI/image/datacenter.py
 SoftLayer/CLI/image/delete.py
 SoftLayer/CLI/image/detail.py
 SoftLayer/CLI/image/edit.py
 SoftLayer/CLI/image/export.py
 SoftLayer/CLI/image/import.py
@@ -426,14 +430,15 @@
 SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_VirtualIpAddress.py
 SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_VirtualServer.py
 SoftLayer/fixtures/SoftLayer_Network_Bandwidth_Version1_Allotment.py
 SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Cache_Purge.py
 SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Mapping.py
 SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Mapping_Path.py
 SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Metrics.py
+SoftLayer/fixtures/SoftLayer_Network_Component.py
 SoftLayer/fixtures/SoftLayer_Network_Component_Firewall.py
 SoftLayer/fixtures/SoftLayer_Network_Firewall_Update_Request.py
 SoftLayer/fixtures/SoftLayer_Network_LBaaS_HealthMonitor.py
 SoftLayer/fixtures/SoftLayer_Network_LBaaS_L7Pool.py
 SoftLayer/fixtures/SoftLayer_Network_LBaaS_Listener.py
 SoftLayer/fixtures/SoftLayer_Network_LBaaS_LoadBalancer.py
 SoftLayer/fixtures/SoftLayer_Network_LBaaS_Member.py
@@ -492,15 +497,14 @@
 SoftLayer/managers/event_log.py
 SoftLayer/managers/file.py
 SoftLayer/managers/firewall.py
 SoftLayer/managers/hardware.py
 SoftLayer/managers/image.py
 SoftLayer/managers/ipsec.py
 SoftLayer/managers/license.py
-SoftLayer/managers/licenses.py
 SoftLayer/managers/load_balancer.py
 SoftLayer/managers/metadata.py
 SoftLayer/managers/network.py
 SoftLayer/managers/object_storage.py
 SoftLayer/managers/ordering.py
 SoftLayer/managers/search.py
 SoftLayer/managers/sshkey.py
@@ -529,14 +533,15 @@
 SoftLayer/transports/timing.py
 SoftLayer/transports/transport.py
 SoftLayer/transports/xmlrpc.py
 tests/CLI/__init__.py
 tests/CLI/core_tests.py
 tests/CLI/custom_types_tests.py
 tests/CLI/environment_tests.py
+tests/CLI/formatting_table_tests.py
 tests/CLI/helper_tests.py
 tests/CLI/modules/__init__.py
 tests/CLI/modules/account_tests.py
 tests/CLI/modules/bandwidth_tests.py
 tests/CLI/modules/block_tests.py
 tests/CLI/modules/call_api_tests.py
 tests/CLI/modules/cdn_tests.py
@@ -555,15 +560,14 @@
 tests/CLI/modules/nas_tests.py
 tests/CLI/modules/object_storage_tests.py
 tests/CLI/modules/order_tests.py
 tests/CLI/modules/report_tests.py
 tests/CLI/modules/search_tests.py
 tests/CLI/modules/security_tests.py
 tests/CLI/modules/securitygroup_tests.py
-tests/CLI/modules/server_tests.py
 tests/CLI/modules/sshkey_tests.py
 tests/CLI/modules/ssl_tests.py
 tests/CLI/modules/subnet_tests.py
 tests/CLI/modules/summary_tests.py
 tests/CLI/modules/tag_tests.py
 tests/CLI/modules/ticket_tests.py
 tests/CLI/modules/user_tests.py
```

### Comparing `SoftLayer-6.1.9/setup.py` & `softlayer-6.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,63 +1,61 @@
 from __future__ import print_function
 import codecs
 import os
 
 from setuptools import setup, find_packages
-
 # pylint: disable=inconsistent-return-statements
 
 DESCRIPTION = "A library for SoftLayer's API"
 
 if os.path.exists('README.rst'):
     with codecs.open('README.rst', 'r', 'utf-8') as readme_file:
         LONG_DESCRIPTION = readme_file.read()
 else:
     LONG_DESCRIPTION = DESCRIPTION
 
 setup(
     name='SoftLayer',
-    version='6.1.9',
+    version='v6.2.0',
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/x-rst',
     author='SoftLayer, Inc., an IBM Company',
     author_email='SLDNDeveloperRelations@wwpdl.vnet.ibm.com',
     packages=find_packages(exclude=['tests']),
     license='MIT',
     zip_safe=False,
-    url='http://github.com/softlayer/softlayer-python',
+    url='https://github.com/SoftLayer/softlayer-python',
     entry_points={
         'console_scripts': [
             'slcli = SoftLayer.CLI.core:main',
-            'sl = SoftLayer.CLI.deprecated:main',
         ],
     },
     python_requires='>=3.7',
     install_requires=[
         'prettytable >= 2.5.0',
         'click >= 8.0.4',
         'requests >= 2.20.0',
         'prompt_toolkit >= 2',
         'pygments >= 2.0.0',
         'urllib3 >= 1.24',
-        'rich == 13.5.3'
+        'rich == 13.7.1'
     ],
-    keywords=['softlayer', 'cloud', 'slcli'],
+    keywords=['softlayer', 'cloud', 'slcli', 'ibmcloud'],
     classifiers=[
         'Environment :: Console',
         'Environment :: Web Environment',
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Topic :: Software Development :: Libraries :: Python Modules',
-        'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy',
     ],
 )
```

### Comparing `SoftLayer-6.1.9/tests/CLI/core_tests.py` & `softlayer-6.2.0/tests/CLI/core_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/custom_types_tests.py` & `softlayer-6.2.0/tests/CLI/custom_types_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/environment_tests.py` & `softlayer-6.2.0/tests/CLI/environment_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/helper_tests.py` & `softlayer-6.2.0/tests/CLI/helper_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -251,20 +251,14 @@
             exceptions.CLIAbort, helpers.resolve_id, lambda r: [], 'test')
 
     def test_resolve_id_multiple(self):
         self.assertRaises(
             exceptions.CLIAbort, helpers.resolve_id, lambda r: [12345, 54321], 'test')
 
 
-class TestTable(testing.TestCase):
-
-    def test_table_with_duplicated_columns(self):
-        self.assertRaises(exceptions.CLIHalt, formatting.Table, ['col', 'col'])
-
-
 class TestFormatOutput(testing.TestCase):
 
     def test_format_output_string(self):
         t = formatting.format_output('just a string', 'raw')
         self.assertEqual('just a string', t)
 
     def test_format_output_json(self):
@@ -450,47 +444,7 @@
 
             with open(tmp.name) as f:
                 data = f.read()
 
                 self.assertEqual(len(data.splitlines()), 2)
                 self.assertIn('datacenter=ams01\n', data)
                 self.assertIn('disk=disk1,disk2\n', data)
-
-
-class IterToTableTests(testing.TestCase):
-
-    def test_format_api_dict(self):
-        result = formatting._format_dict({'key': 'value'})
-
-        self.assertIsInstance(result, formatting.Table)
-        self.assertEqual(result.columns, ['name', 'value'])
-        self.assertEqual(result.rows, [['key', 'value']])
-
-    def test_format_api_list(self):
-        result = formatting._format_list([{'key': 'value'}])
-
-        self.assertIsInstance(result, formatting.Table)
-        self.assertEqual(result.columns, ['key'])
-        self.assertEqual(result.rows, [['value']])
-
-    def test_format_api_list_non_objects(self):
-        result = formatting._format_list(['a', 'b', 'c'])
-
-        self.assertIsInstance(result, formatting.Table)
-        self.assertEqual(result.columns, ['value'])
-        self.assertEqual(result.rows, [['a'], ['b'], ['c']])
-
-    def test_format_api_list_with_none_value(self):
-        result = formatting._format_list([{'key': [None, 'value']}, None])
-
-        self.assertIsInstance(result, formatting.Table)
-        self.assertEqual(result.columns, ['key'])
-
-    def test_format_api_list_with_empty_array(self):
-        result = formatting.iter_to_table([{'id': 130224450, 'activeTickets': []}])
-        self.assertIsInstance(result, formatting.Table)
-        self.assertIn('id', result.columns)
-        self.assertIn('activeTickets', result.columns)
-        formatted = formatting.format_output(result, "table")
-        # No good ways to test whats actually in a Rich.Table without going through the hassel of
-        # printing it out. As long as this didn't throw and exception it should be fine.
-        self.assertEqual(formatted.row_count, 1)
```

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/account_tests.py` & `softlayer-6.2.0/tests/CLI/modules/account_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/bandwidth_tests.py` & `softlayer-6.2.0/tests/CLI/modules/bandwidth_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/block_tests.py` & `softlayer-6.2.0/tests/CLI/modules/block_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/call_api_tests.py` & `softlayer-6.2.0/tests/CLI/modules/call_api_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/cdn_tests.py` & `softlayer-6.2.0/tests/CLI/modules/cdn_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/config_tests.py` & `softlayer-6.2.0/tests/CLI/modules/config_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/dedicatedhost_tests.py` & `softlayer-6.2.0/tests/CLI/modules/dedicatedhost_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/dns_tests.py` & `softlayer-6.2.0/tests/CLI/modules/dns_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/email_tests.py` & `softlayer-6.2.0/tests/CLI/modules/email_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/event_log_tests.py` & `softlayer-6.2.0/tests/CLI/modules/event_log_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/file_tests.py` & `softlayer-6.2.0/tests/CLI/modules/file_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/firewall_tests.py` & `softlayer-6.2.0/tests/CLI/modules/firewall_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/globalip_tests.py` & `softlayer-6.2.0/tests/CLI/modules/globalip_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/image_tests.py` & `softlayer-6.2.0/tests/CLI/modules/image_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/ipsec_tests.py` & `softlayer-6.2.0/tests/CLI/modules/ipsec_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/licenses_test.py` & `softlayer-6.2.0/tests/CLI/modules/licenses_test.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/loadbal_tests.py` & `softlayer-6.2.0/tests/CLI/modules/loadbal_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/nas_tests.py` & `softlayer-6.2.0/tests/CLI/modules/nas_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/object_storage_tests.py` & `softlayer-6.2.0/tests/CLI/modules/object_storage_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/order_tests.py` & `softlayer-6.2.0/tests/CLI/modules/order_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/report_tests.py` & `softlayer-6.2.0/tests/CLI/modules/report_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/search_tests.py` & `softlayer-6.2.0/tests/CLI/modules/search_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/security_tests.py` & `softlayer-6.2.0/tests/CLI/modules/security_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/securitygroup_tests.py` & `softlayer-6.2.0/tests/CLI/modules/securitygroup_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/server_tests.py` & `softlayer-6.2.0/tests/managers/vs/vs_tests.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,1085 +1,1312 @@
 """
-    SoftLayer.tests.CLI.modules.server_tests
-    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-    This is a series of integration tests designed to test the complete
-    command line interface.
+    SoftLayer.tests.managers.vs.vs_tests
+    ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
     :license: MIT, see LICENSE for more details.
-"""
 
-import json
-import sys
-import tempfile
+"""
 from unittest import mock as mock
 
-from SoftLayer.CLI import exceptions
-from SoftLayer.fixtures import SoftLayer_Product_Order
-from SoftLayer import SoftLayerError
+import SoftLayer
+from SoftLayer import exceptions
+from SoftLayer import fixtures
 from SoftLayer import testing
-from SoftLayer import utils
 
 
-class ServerCLITests(testing.TestCase):
+class VSTests(testing.TestCase):
 
-    def test_server_cancel_reasons(self):
-        result = self.run_command(['server', 'cancel-reasons'])
-        output = json.loads(result.output)
-        self.assert_no_fail(result)
-        self.assertEqual(len(output), 10)
+    def set_up(self):
+        self.vs = SoftLayer.VSManager(self.client, SoftLayer.OrderingManager(self.client))
 
-    def test_server_credentials(self):
-        mock = self.set_mock('SoftLayer_Hardware_Server', 'getObject')
-        mock.return_value = {
-            "accountId": 11111,
-            "domain": "chechu.com",
-            "fullyQualifiedDomainName": "host3.vmware.chechu.com",
-            "hardwareStatusId": 5,
-            "hostname": "host3.vmware",
-            "id": 12345,
-            "softwareComponents": [{"passwords": [
-                {
-                    "password": "abc123",
-                    "username": "root"
-                }],
-                'softwareLicense': {
-                    'softwareDescription':
-                        {
-                            'referenceCode': 'CENTOS_7_64',
-                            'version': '7.8 - 64',
-                            'name': 'Centos'
-                        }}}]
-        }
-        result = self.run_command(['hardware', 'credentials', '12345'])
-
-        self.assert_no_fail(result)
-        self.assertEqual(json.loads(result.output), [
-            {'Password': 'abc123',
-             'Software': 'Centos',
-             'Username': 'root',
-             'Version': '7.8 - 64'}
-        ])
+    def test_list_instances(self):
+        results = self.vs.list_instances(hourly=True, monthly=True)
 
-    def test_server_credentials_exception_passwords_not_found(self):
-        mock = self.set_mock('SoftLayer_Hardware_Server', 'getObject')
-        mock.return_value = {
-            "accountId": 11111,
-            "domain": "chechu.com",
-            "fullyQualifiedDomainName": "host3.vmware.chechu.com",
-            "hardwareStatusId": 5,
-            "hostname": "host3.vmware",
-            "id": 12345,
-            "softwareComponents": [{}]
+        for result in results:
+            self.assertIn(result['id'], [100, 104])
+        self.assert_called_with('SoftLayer_Account', 'getVirtualGuests')
+
+    def test_list_instances_neither(self):
+        results = self.vs.list_instances(hourly=False, monthly=False)
+
+        for result in results:
+            self.assertIn(result['id'], [100, 104])
+        self.assert_called_with('SoftLayer_Account', 'getVirtualGuests')
+
+    def test_list_instances_monthly(self):
+        results = self.vs.list_instances(hourly=False, monthly=True)
+
+        for result in results:
+            self.assertIn(result['id'], [100])
+        self.assert_called_with('SoftLayer_Account', 'getMonthlyVirtualGuests')
+
+    def test_list_instances_hourly(self):
+        results = self.vs.list_instances(hourly=True, monthly=False)
+
+        for result in results:
+            self.assertIn(result['id'], [104])
+        self.assert_called_with('SoftLayer_Account', 'getHourlyVirtualGuests')
+
+    def test_list_instances_with_filters(self):
+        self.vs.list_instances(
+            hourly=True,
+            monthly=True,
+            tags=['tag1', 'tag2'],
+            cpus=2,
+            memory=1024,
+            hostname='hostname',
+            domain='example.com',
+            local_disk=True,
+            datacenter='dal05',
+            nic_speed=100,
+            public_ip='1.2.3.4',
+            private_ip='4.3.2.1',
+            transient=False,
+        )
+
+        _filter = {
+            'virtualGuests': {
+                'datacenter': {
+                    'name': {'operation': '_= dal05'}},
+                'domain': {'operation': '_= example.com'},
+                'tagReferences': {
+                    'tag': {'name': {
+                        'operation': 'in',
+                        'options': [{
+                            'name': 'data', 'value': ['tag1', 'tag2']}]}}},
+                'maxCpu': {'operation': 2},
+                'localDiskFlag': {'operation': True},
+                'maxMemory': {'operation': 1024},
+                'hostname': {'operation': '_= hostname'},
+                'networkComponents': {'maxSpeed': {'operation': 100}},
+                'primaryIpAddress': {'operation': '_= 1.2.3.4'},
+                'primaryBackendIpAddress': {'operation': '_= 4.3.2.1'},
+                'transientGuestFlag': {'operation': False},
+            }
         }
+        self.assert_called_with('SoftLayer_Account', 'getVirtualGuests',
+                                filter=_filter)
 
-        result = self.run_command(['hardware', 'credentials', '12345'])
+    def test_resolve_ids_ip(self):
+        _id = self.vs._get_ids_from_ip('172.16.240.2')
 
-        self.assertEqual(
-            'No passwords found in softwareComponents',
-            str(result.exception)
-        )
+        self.assertEqual(_id, [100, 104])
 
-    def test_server_credentials_exception_password_not_found(self):
-        mock = self.set_mock('SoftLayer_Hardware_Server', 'getObject')
-        mock.return_value = {
-            "accountId": 11111,
-            "domain": "chechu.com",
-            "fullyQualifiedDomainName": "host3.vmware.chechu.com",
-            "hardwareStatusId": 5,
-            "hostname": "host3.vmware",
-            "id": 12345,
-            "softwareComponents": [
+    def test_resolve_ids_ip_private(self):
+        # Now simulate a private IP test
+        mock = self.set_mock('SoftLayer_Account', 'getVirtualGuests')
+        mock.side_effect = [[], [{'id': 99}]]
+
+        _id = self.vs._get_ids_from_ip('10.0.1.87')
+
+        self.assertEqual(_id, [99])
+
+    def test_resolve_ids_ip_invalid(self):
+        _id = self.vs._get_ids_from_ip('nope')
+        self.assertEqual(_id, [])
+
+    def test_resolve_ids_hostname(self):
+        _id = self.vs._get_ids_from_hostname('vs-test1')
+        self.assertEqual(_id, [100, 104])
+
+    def test_get_instance(self):
+        result = self.vs.get_instance(100)
+
+        self.assertEqual(fixtures.SoftLayer_Virtual_Guest.getObject, result)
+        self.assert_called_with('SoftLayer_Virtual_Guest', 'getObject',
+                                identifier=100)
+
+    def test_get_create_options(self):
+        options = self.vs.get_create_options()
+
+        extras = {'key': '1_IPV6_ADDRESS', 'name': '1 IPv6 Address'}
+        locations = {'key': 'wdc07', 'name': 'Washington 7'}
+        operating_systems = {
+            'key': 'OS_UBUNTU_14_04_LTS_TRUSTY_TAHR_64_BIT',
+            'name': 'Ubuntu / 14.04-64',
+            'referenceCode': 'UBUNTU_14_64'
+        }
+
+        port_speeds = {
+            'key': '10',
+            'name': '10 Mbps Public & Private Network Uplinks'
+        }
+        sizes = {
+            'key': 'M1_64X512X25',
+            'name': 'M1.64x512x25',
+            'hourlyRecurringFee': 0.0,
+            'recurringFee': 0.0
+        }
+
+        self.assertEqual(options['extras'][0]['key'], extras['key'])
+        self.assertEqual(options['locations'][0], locations)
+        self.assertEqual(options['operating_systems'][0]['referenceCode'],
+                         operating_systems['referenceCode'])
+        self.assertEqual(options['port_speed'][0]['name'], port_speeds['name'])
+        self.assertEqual(options['sizes'][0], sizes)
+
+    def test_get_create_options_prices_by_location(self):
+        options = self.vs.get_create_options('wdc07')
+
+        extras = {'key': '1_IPV6_ADDRESS', 'name': '1 IPv6 Address',
+                  'prices': [
+                      {
+                          'hourlyRecurringFee': '0',
+                          'id': 272,
+                          'locationGroupId': '',
+                          'recurringFee': '0',
+                      }
+                  ]
+                  }
+        locations = {'key': 'wdc07', 'name': 'Washington 7'}
+        operating_systems = {
+            'key': 'OS_UBUNTU_14_04_LTS_TRUSTY_TAHR_64_BIT',
+            'name': 'Ubuntu / 14.04-64',
+            'referenceCode': 'UBUNTU_14_64',
+            'prices': [
+                {
+                    'hourlyRecurringFee': '0',
+                    'id': 272,
+                    'locationGroupId': '',
+                    'recurringFee': '0',
+                }
+            ]
+        }
+
+        port_speeds = {
+            'key': '10',
+            'name': '10 Mbps Public & Private Network Uplinks',
+            'prices': [
                 {
-                    "hardwareId": 22222,
-                    "id": 333333,
-                    "passwords": [{}],
-                    "softwareLicense": {
-                        "softwareDescription": {
-                            "name": None,
-                            "version": None
-                        }
-                    }
+                    'hourlyRecurringFee': '0',
+                    'id': 272,
+                    'locationGroupId': '',
+                    'recurringFee': '0',
                 }
             ]
         }
+        sizes = {
+            'key': 'M1_64X512X25',
+            'name': 'M1.64x512x25',
+            'hourlyRecurringFee': 0.0,
+            'recurringFee': 0.0
+        }
 
-        result = self.run_command(['hardware', 'credentials', '12345'])
+        self.assertEqual(options['extras'][0]['prices'][0]['hourlyRecurringFee'],
+                         extras['prices'][0]['hourlyRecurringFee'])
+        self.assertEqual(options['locations'][0], locations)
+        self.assertEqual(options['operating_systems'][0]['prices'][0]['locationGroupId'],
+                         operating_systems['prices'][0]['locationGroupId'])
+        self.assertEqual(options['port_speed'][0]['prices'][0]['id'], port_speeds['prices'][0]['id'])
+        self.assertEqual(options['sizes'][0], sizes)
+
+    def test_cancel_instance(self):
+        result = self.vs.cancel_instance(1)
+
+        self.assertEqual(result, True)
+        self.assert_called_with('SoftLayer_Virtual_Guest', 'deleteObject',
+                                identifier=1)
+
+    def test_reload_instance(self):
+        self.vs.reload_instance(1)
+
+        self.assert_called_with('SoftLayer_Virtual_Guest',
+                                'reloadOperatingSystem',
+                                args=('FORCE', {}),
+                                identifier=1)
+
+    def test_reload_instance_posturi_sshkeys(self):
+        post_uri = 'http://test.sftlyr.ws/test.sh'
+
+        self.vs.reload_instance(1, post_uri=post_uri, ssh_keys=[1701])
+
+        args = ('FORCE', {'customProvisionScriptUri': post_uri,
+                          'sshKeyIds': [1701]})
+        self.assert_called_with('SoftLayer_Virtual_Guest',
+                                'reloadOperatingSystem',
+                                args=args,
+                                identifier=1)
+
+    def test_reload_instance_with_new_os(self):
+        self.vs.reload_instance(1, image_id=1234)
+
+        args = ('FORCE', {'imageTemplateId': 1234})
+        self.assert_called_with('SoftLayer_Virtual_Guest',
+                                'reloadOperatingSystem',
+                                args=args,
+                                identifier=1)
+
+    @mock.patch('SoftLayer.managers.vs.VSManager._generate_create_dict')
+    def test_create_instance(self, create_dict):
+        create_dict.return_value = {'test': 1, 'verify': 1}
+
+        self.vs.create_instance(test=1, verify=1, tags='dev,green')
+
+        create_dict.assert_called_once_with(test=1, verify=1)
+        self.assert_called_with('SoftLayer_Virtual_Guest', 'createObject',
+                                args=({'test': 1, 'verify': 1},))
+        self.assert_called_with('SoftLayer_Virtual_Guest', 'setTags',
+                                args=('dev,green',),
+                                identifier=100)
+
+    def test_create_instances(self):
+        self.vs.create_instances([{'cpus': 1,
+                                   'memory': 1024,
+                                   'hostname': 'server',
+                                   'domain': 'example.com',
+                                   'tags': 'dev,green'}])
+
+        args = ([{'domain': 'example.com',
+                  'hourlyBillingFlag': True,
+                  'localDiskFlag': True,
+                  'maxMemory': 1024,
+                  'hostname': 'server',
+                  'startCpus': 1,
+                  'supplementalCreateObjectOptions': {'bootMode': None}}],)
+        self.assert_called_with('SoftLayer_Virtual_Guest', 'createObjects',
+                                args=args)
+        self.assert_called_with('SoftLayer_Virtual_Guest', 'setTags',
+                                args=('dev,green',),
+                                identifier=100)
+
+    def test_generate_os_and_image(self):
+        self.assertRaises(
+            ValueError,
+            self.vs._generate_create_dict,
+            cpus=1,
+            memory=1,
+            hostname='test',
+            domain='example.com',
+            os_code=1,
+            image_id=1,
+        )
 
-        self.assertEqual(
-            'None',
-            str(result.exception)
-        )
-
-    def test_server_details(self):
-        result = self.run_command(['server', 'detail', '1234', '--passwords', '--price'])
-
-        self.assert_no_fail(result)
-        output = json.loads(result.output)
-        self.assertEqual(output['notes'], 'These are test notes.')
-        self.assertEqual(output['prices'][0]['Recurring Price'], 16.08)
-        self.assertEqual(output['remote users'][0]['password'], 'abc123')
-        self.assertEqual(output['users'][0]['username'], 'root')
-        self.assertEqual(output['vlans'][0]['number'], 1800)
-        self.assertEqual(output['owner'], 'chechu')
-        self.assertEqual(output['Bandwidth'][0]['Allotment'], '250')
+    def test_generate_missing(self):
+        self.assertRaises(ValueError, self.vs._generate_create_dict)
+        self.assertRaises(ValueError, self.vs._generate_create_dict, cpus=1)
+
+    def test_generate_basic(self):
+        data = self.vs._generate_create_dict(
+            cpus=1,
+            memory=1,
+            hostname='test',
+            domain='example.com',
+            os_code="STRING",
+        )
 
-    def test_detail_vs_empty_tag(self):
-        mock = self.set_mock('SoftLayer_Hardware_Server', 'getObject')
-        mock.return_value = {
-            'id': 100,
-            'processorPhysicalCoreAmount': 2,
-            'memoryCapacity': 2,
-            'tagReferences': [
-                {'tag': {'name': 'example-tag'}},
-                {},
-            ],
-        }
-        result = self.run_command(['server', 'detail', '100'])
-
-        self.assert_no_fail(result)
-        self.assertEqual(
-            json.loads(result.output)['tags'],
-            ['example-tag'],
+        assert_data = {
+            'startCpus': 1,
+            'maxMemory': 1,
+            'hostname': 'test',
+            'domain': 'example.com',
+            'localDiskFlag': True,
+            'operatingSystemReferenceCode': "STRING",
+            'hourlyBillingFlag': True,
+            'supplementalCreateObjectOptions': {'bootMode': None},
+        }
+
+        self.assertEqual(data, assert_data)
+
+    def test_generate_monthly(self):
+        data = self.vs._generate_create_dict(
+            cpus=1,
+            memory=1,
+            hostname='test',
+            domain='example.com',
+            os_code="STRING",
+            hourly=False,
         )
 
-    def test_detail_empty_allotment(self):
-        mock = self.set_mock('SoftLayer_Hardware_Server', 'getBandwidthAllotmentDetail')
-        mock.return_value = None
-        result = self.run_command(['server', 'detail', '100'])
+        assert_data = {
+            'hourlyBillingFlag': False,
+            'startCpus': 1,
+            'maxMemory': 1,
+            'hostname': 'test',
+            'domain': 'example.com',
+            'localDiskFlag': True,
+            'operatingSystemReferenceCode': "STRING",
+            'supplementalCreateObjectOptions': {'bootMode': None},
+        }
+
+        self.assertEqual(data, assert_data)
+
+    def test_generate_image_id(self):
+        data = self.vs._generate_create_dict(
+            cpus=1,
+            memory=1,
+            hostname='test',
+            domain='example.com',
+            image_id="45",
+        )
+
+        assert_data = {
+            'startCpus': 1,
+            'maxMemory': 1,
+            'hostname': 'test',
+            'domain': 'example.com',
+            'localDiskFlag': True,
+            'blockDeviceTemplateGroup': {"globalIdentifier": "45"},
+            'hourlyBillingFlag': True,
+            'supplementalCreateObjectOptions': {'bootMode': None},
+        }
+
+        self.assertEqual(data, assert_data)
+
+    def test_generate_dedicated(self):
+        data = self.vs._generate_create_dict(
+            cpus=1,
+            memory=1,
+            hostname='test',
+            domain='example.com',
+            os_code="STRING",
+            dedicated=True,
+        )
+
+        assert_data = {
+            'startCpus': 1,
+            'maxMemory': 1,
+            'hostname': 'test',
+            'domain': 'example.com',
+            'localDiskFlag': True,
+            'operatingSystemReferenceCode': "STRING",
+            'hourlyBillingFlag': True,
+            'dedicatedAccountHostOnlyFlag': True,
+            'supplementalCreateObjectOptions': {'bootMode': None},
+        }
+
+        self.assertEqual(data, assert_data)
+
+    def test_generate_datacenter(self):
+        data = self.vs._generate_create_dict(
+            cpus=1,
+            memory=1,
+            hostname='test',
+            domain='example.com',
+            os_code="STRING",
+            datacenter="sng01",
+        )
+
+        assert_data = {
+            'startCpus': 1,
+            'maxMemory': 1,
+            'hostname': 'test',
+            'domain': 'example.com',
+            'localDiskFlag': True,
+            'operatingSystemReferenceCode': "STRING",
+            'hourlyBillingFlag': True,
+            'datacenter': {"name": 'sng01'},
+            'supplementalCreateObjectOptions': {'bootMode': None},
+        }
+
+        self.assertEqual(data, assert_data)
+
+    def test_generate_public_vlan(self):
+        data = self.vs._generate_create_dict(
+            cpus=1,
+            memory=1,
+            hostname='test',
+            domain='example.com',
+            os_code="STRING",
+            public_vlan=1,
+        )
+
+        assert_data = {
+            'startCpus': 1,
+            'maxMemory': 1,
+            'hostname': 'test',
+            'domain': 'example.com',
+            'localDiskFlag': True,
+            'operatingSystemReferenceCode': "STRING",
+            'hourlyBillingFlag': True,
+            'primaryNetworkComponent': {"networkVlan": {"id": 1}},
+            'supplementalCreateObjectOptions': {'bootMode': None},
+        }
+
+        self.assertEqual(data, assert_data)
+
+    def test_generate_public_vlan_with_public_subnet(self):
+        data = self.vs._generate_create_dict(
+            cpus=1,
+            memory=1,
+            hostname='test',
+            domain='example.com',
+            os_code="STRING",
+            public_vlan=1,
+            public_subnet=1
+        )
+
+        assert_data = {
+            'startCpus': 1,
+            'maxMemory': 1,
+            'hostname': 'test',
+            'domain': 'example.com',
+            'localDiskFlag': True,
+            'operatingSystemReferenceCode': "STRING",
+            'hourlyBillingFlag': True,
+            'primaryNetworkComponent': {'networkVlan': {'id': 1,
+                                                        'primarySubnet': {'id': 1}}},
+            'supplementalCreateObjectOptions': {'bootMode': None},
+        }
+
+        self.assertEqual(data, assert_data)
+
+    def test_generate_private_vlan_with_private_subnet(self):
+        data = self.vs._generate_create_dict(
+            cpus=1,
+            memory=1,
+            hostname='test',
+            domain='example.com',
+            os_code="STRING",
+            private_vlan=1,
+            private_subnet=1
+        )
+
+        assert_data = {
+            'startCpus': 1,
+            'maxMemory': 1,
+            'hostname': 'test',
+            'domain': 'example.com',
+            'localDiskFlag': True,
+            'operatingSystemReferenceCode': "STRING",
+            'hourlyBillingFlag': True,
+            'primaryBackendNetworkComponent': {'networkVlan': {'id': 1,
+                                                               'primarySubnet': {'id': 1}}},
+            'supplementalCreateObjectOptions': {'bootMode': None},
+        }
+
+        self.assertEqual(data, assert_data)
+
+    def test_generate_private_vlan_subnet_public_vlan_subnet(self):
+        data = self.vs._generate_create_dict(
+            cpus=1,
+            memory=1,
+            hostname='test',
+            domain='example.com',
+            os_code="STRING",
+            private_vlan=1,
+            private_subnet=1,
+            public_vlan=1,
+            public_subnet=1,
+        )
+
+        assert_data = {
+            'startCpus': 1,
+            'maxMemory': 1,
+            'hostname': 'test',
+            'domain': 'example.com',
+            'localDiskFlag': True,
+            'operatingSystemReferenceCode': "STRING",
+            'hourlyBillingFlag': True,
+            'primaryBackendNetworkComponent': {'networkVlan': {'id': 1,
+                                                               'primarySubnet': {'id': 1}}},
+            'primaryNetworkComponent': {'networkVlan': {'id': 1,
+                                                        'primarySubnet': {'id': 1}}},
+            'supplementalCreateObjectOptions': {'bootMode': None},
+        }
+
+        self.assertEqual(data, assert_data)
+
+    def test_generate_private_subnet(self):
+        actual = self.assertRaises(
+            exceptions.SoftLayerError,
+            self.vs._generate_create_dict,
+            cpus=1,
+            memory=1,
+            hostname='test',
+            domain='example.com',
+            os_code="STRING",
+            private_subnet=1,
+        )
+
+        self.assertEqual(str(actual), "You need to specify a private_vlan with private_subnet")
+
+    def test_generate_public_subnet(self):
+        actual = self.assertRaises(
+            exceptions.SoftLayerError,
+            self.vs._generate_create_dict,
+            cpus=1,
+            memory=1,
+            hostname='test',
+            domain='example.com',
+            os_code="STRING",
+            public_subnet=1,
+        )
+
+        self.assertEqual(str(actual), "You need to specify a public_vlan with public_subnet")
+
+    def test_generate_private_vlan(self):
+        data = self.vs._generate_create_dict(
+            cpus=1,
+            memory=1,
+            hostname='test',
+            domain='example.com',
+            os_code="STRING",
+            private_vlan=1,
+        )
+
+        assert_data = {
+            'startCpus': 1,
+            'maxMemory': 1,
+            'hostname': 'test',
+            'domain': 'example.com',
+            'localDiskFlag': True,
+            'operatingSystemReferenceCode': "STRING",
+            'hourlyBillingFlag': True,
+            'primaryBackendNetworkComponent': {'networkVlan': {'id': 1}},
+            'supplementalCreateObjectOptions': {'bootMode': None},
+        }
+
+        self.assertEqual(data, assert_data)
+
+    def test_generate_by_router_and_vlan(self):
+        actual = self.assertRaises(
+            exceptions.SoftLayerError,
+            self.vs._generate_create_dict,
+            cpus=1,
+            memory=1,
+            hostname='test',
+            domain='example.com',
+            os_code="STRING",
+            private_router=1,
+            private_vlan=1
+        )
+
+        self.assertEqual(str(actual), "You have to select network vlan or network vlan with a subnet or only router, "
+                                      "not all options")
+
+    def test_generate_by_router_and_subnet(self):
+        actual = self.assertRaises(
+            exceptions.SoftLayerError,
+            self.vs._generate_create_dict,
+            cpus=1,
+            memory=1,
+            hostname='test',
+            domain='example.com',
+            os_code="STRING",
+            private_router=1,
+            private_subnet=1
+        )
+
+        self.assertEqual(str(actual), "You have to select network vlan or network vlan with a subnet or only router, "
+                                      "not all options")
+
+    def test_generate_sec_group(self):
+        data = self.vs._generate_create_dict(
+            cpus=1,
+            memory=1,
+            hostname='test',
+            domain='test.com',
+            os_code="OS",
+            public_security_groups=[1, 2, 3],
+            private_security_groups=[4, 5, 6]
+        )
+
+        pub_sec_binding = data['primaryNetworkComponent']['securityGroupBindings']
+        prv_sec_binding = data['primaryBackendNetworkComponent']['securityGroupBindings']
+        # Public
+        self.assertEqual(pub_sec_binding[0]['securityGroup']['id'], 1)
+        self.assertEqual(pub_sec_binding[1]['securityGroup']['id'], 2)
+        self.assertEqual(pub_sec_binding[2]['securityGroup']['id'], 3)
+        # Private
+        self.assertEqual(prv_sec_binding[0]['securityGroup']['id'], 4)
+        self.assertEqual(prv_sec_binding[1]['securityGroup']['id'], 5)
+        self.assertEqual(prv_sec_binding[2]['securityGroup']['id'], 6)
+
+    def test_create_network_components_vlan_subnet_private_vlan_subnet_public(self):
+        data = self.vs._create_network_components(
+            private_vlan=1,
+            private_subnet=1,
+            public_vlan=1,
+            public_subnet=1,
+        )
+
+        assert_data = {
+            'primaryBackendNetworkComponent': {'networkVlan': {'id': 1,
+                                                               'primarySubnet': {'id': 1}}},
+            'primaryNetworkComponent': {'networkVlan': {'id': 1,
+                                                        'primarySubnet': {'id': 1}}},
+        }
+
+        self.assertEqual(data, assert_data)
+
+    def test_create_network_components_by_routers(self):
+        data = self.vs._create_network_components(
+            private_router=1,
+            public_router=1
+        )
+
+        assert_data = {
+            'primaryBackendNetworkComponent': {'router': {'id': 1}},
+            'primaryNetworkComponent': {'router': {'id': 1}},
+        }
+
+        self.assertEqual(data, assert_data)
+
+    def test_create_network_components_by_routers_and_vlan(self):
+        actual = self.assertRaises(
+            exceptions.SoftLayerError,
+            self.vs._create_network_components,
+            private_router=1,
+            public_router=1,
+            private_vlan=1
+        )
+
+        self.assertEqual(str(actual), "You have to select network vlan or network vlan with a subnet or only router, "
+                                      "not all options")
+
+    def test_create_network_components_vlan_subnet_private(self):
+        data = self.vs._create_network_components(
+            private_vlan=1,
+            private_subnet=1,
+        )
+
+        assert_data = {
+            'primaryBackendNetworkComponent': {'networkVlan': {'id': 1,
+                                                               'primarySubnet': {'id': 1}}},
+        }
+
+        self.assertEqual(data, assert_data)
+
+    def test_create_network_components_vlan_subnet_public(self):
+        data = self.vs._create_network_components(
+            public_vlan=1,
+            public_subnet=1,
+        )
+
+        assert_data = {
+            'primaryNetworkComponent': {'networkVlan': {'id': 1,
+                                                        'primarySubnet': {'id': 1}}},
+        }
+
+        self.assertEqual(data, assert_data)
+
+    def test_create_network_components_private_subnet(self):
+        actual = self.assertRaises(
+            exceptions.SoftLayerError,
+            self.vs._create_network_components,
+            private_subnet=1,
+        )
+
+        self.assertEqual(str(actual), "You need to specify a private_vlan with private_subnet")
 
-        self.assert_no_fail(result)
-        self.assertEqual(
-            json.loads(result.output)['Bandwidth'][0]['Allotment'],
-            '-',
+    def test_create_network_components_public_subnet(self):
+        actual = self.assertRaises(
+            exceptions.SoftLayerError,
+            self.vs._create_network_components,
+            public_subnet=1,
         )
 
-    def test_detail_drives(self):
-        mock = self.set_mock('SoftLayer_Hardware_Server', 'getHardDrives')
+        self.assertEqual(str(actual), "You need to specify a public_vlan with public_subnet")
+
+    def test_generate_userdata(self):
+        data = self.vs._generate_create_dict(
+            cpus=1,
+            memory=1,
+            hostname='test',
+            domain='example.com',
+            os_code="STRING",
+            userdata="ICANHAZVSI",
+        )
+
+        assert_data = {
+            'startCpus': 1,
+            'maxMemory': 1,
+            'hostname': 'test',
+            'domain': 'example.com',
+            'localDiskFlag': True,
+            'operatingSystemReferenceCode': "STRING",
+            'hourlyBillingFlag': True,
+            'userData': [{'value': "ICANHAZVSI"}],
+            'supplementalCreateObjectOptions': {'bootMode': None},
+        }
+
+        self.assertEqual(data, assert_data)
+
+    def test_generate_network(self):
+        data = self.vs._generate_create_dict(
+            cpus=1,
+            memory=1,
+            hostname='test',
+            domain='example.com',
+            os_code="STRING",
+            nic_speed=9001,
+        )
+
+        assert_data = {
+            'startCpus': 1,
+            'maxMemory': 1,
+            'hostname': 'test',
+            'domain': 'example.com',
+            'localDiskFlag': True,
+            'operatingSystemReferenceCode': "STRING",
+            'hourlyBillingFlag': True,
+            'networkComponents': [{'maxSpeed': 9001}],
+            'supplementalCreateObjectOptions': {'bootMode': None},
+        }
+
+        self.assertEqual(data, assert_data)
+
+    def test_generate_private_network_only(self):
+        data = self.vs._generate_create_dict(
+            cpus=1,
+            memory=1,
+            hostname='test',
+            domain='example.com',
+            os_code="STRING",
+            nic_speed=9001,
+            private=True
+        )
+
+        assert_data = {
+            'startCpus': 1,
+            'maxMemory': 1,
+            'hostname': 'test',
+            'domain': 'example.com',
+            'localDiskFlag': True,
+            'operatingSystemReferenceCode': "STRING",
+            'privateNetworkOnlyFlag': True,
+            'hourlyBillingFlag': True,
+            'networkComponents': [{'maxSpeed': 9001}],
+            'supplementalCreateObjectOptions': {'bootMode': None},
+        }
+
+        self.assertEqual(data, assert_data)
+
+    def test_generate_post_uri(self):
+        data = self.vs._generate_create_dict(
+            cpus=1,
+            memory=1,
+            hostname='test',
+            domain='example.com',
+            os_code="STRING",
+            post_uri='https://example.com/boostrap.sh',
+        )
+
+        assert_data = {
+            'startCpus': 1,
+            'maxMemory': 1,
+            'hostname': 'test',
+            'domain': 'example.com',
+            'localDiskFlag': True,
+            'operatingSystemReferenceCode': "STRING",
+            'hourlyBillingFlag': True,
+            'postInstallScriptUri': 'https://example.com/boostrap.sh',
+            'supplementalCreateObjectOptions': {'bootMode': None},
+        }
+
+        self.assertEqual(data, assert_data)
+
+    def test_generate_sshkey(self):
+        data = self.vs._generate_create_dict(
+            cpus=1,
+            memory=1,
+            hostname='test',
+            domain='example.com',
+            os_code="STRING",
+            ssh_keys=[543],
+        )
+
+        assert_data = {
+            'startCpus': 1,
+            'maxMemory': 1,
+            'hostname': 'test',
+            'domain': 'example.com',
+            'localDiskFlag': True,
+            'operatingSystemReferenceCode': "STRING",
+            'hourlyBillingFlag': True,
+            'sshKeys': [{'id': 543}],
+            'supplementalCreateObjectOptions': {'bootMode': None},
+        }
+
+        self.assertEqual(data, assert_data)
+
+    def test_generate_no_disks(self):
+        data = self.vs._generate_create_dict(
+            cpus=1,
+            memory=1,
+            hostname='test',
+            domain='example.com',
+            os_code="STRING"
+        )
+
+        self.assertEqual(data.get('blockDevices'), None)
+
+    def test_generate_single_disk(self):
+        data = self.vs._generate_create_dict(
+            cpus=1,
+            memory=1,
+            hostname='test',
+            domain='example.com',
+            os_code="STRING",
+            disks=[50]
+        )
+
+        assert_data = {
+            'blockDevices': [
+                {"device": "0", "diskImage": {"capacity": 50}}]
+        }
+
+        self.assertTrue(data.get('blockDevices'))
+        self.assertEqual(data['blockDevices'], assert_data['blockDevices'])
+
+    def test_generate_multi_disk(self):
+        data = self.vs._generate_create_dict(
+            cpus=1,
+            memory=1,
+            hostname='test',
+            domain='example.com',
+            os_code="STRING",
+            disks=[50, 70, 100]
+        )
+
+        assert_data = {
+            'blockDevices': [
+                {"device": "0", "diskImage": {"capacity": 50}},
+                {"device": "2", "diskImage": {"capacity": 70}},
+                {"device": "3", "diskImage": {"capacity": 100}}]
+        }
+
+        self.assertTrue(data.get('blockDevices'))
+        self.assertEqual(data['blockDevices'], assert_data['blockDevices'])
+
+    def test_generate_boot_mode(self):
+        data = self.vs._generate_create_dict(
+            cpus=1,
+            memory=1,
+            hostname='test',
+            domain='example.com',
+            os_code="STRING",
+            boot_mode="HVM"
+        )
+
+        assert_data = {
+            'startCpus': 1,
+            'maxMemory': 1,
+            'hostname': 'test',
+            'domain': 'example.com',
+            'localDiskFlag': True,
+            'operatingSystemReferenceCode': "STRING",
+            'hourlyBillingFlag': True,
+            'supplementalCreateObjectOptions': {'bootMode': 'HVM'},
+        }
+
+        self.assertEqual(data, assert_data)
+
+    def test_change_port_speed_public(self):
+        result = self.vs.change_port_speed(1, True, 100)
+
+        self.assertEqual(result, True)
+        self.assert_called_with('SoftLayer_Virtual_Guest',
+                                'setPublicNetworkInterfaceSpeed',
+                                identifier=1,
+                                args=(100,))
+
+    def test_change_port_speed_private(self):
+        result = self.vs.change_port_speed(2, False, 10)
+
+        self.assertEqual(result, True)
+        self.assert_called_with('SoftLayer_Virtual_Guest',
+                                'setPrivateNetworkInterfaceSpeed',
+                                identifier=2,
+                                args=(10,))
+
+    def test_rescue(self):
+        # Test rescue environment
+        result = self.vs.rescue(1234)
+
+        self.assertEqual(result, True)
+        self.assert_called_with('SoftLayer_Virtual_Guest',
+                                'executeRescueLayer',
+                                identifier=1234)
+
+    def test_edit_metadata(self):
+        # Test editing user data
+        result = self.vs.edit(100, userdata='my data')
+
+        self.assertEqual(result, True)
+        self.assert_called_with('SoftLayer_Virtual_Guest', 'setUserMetadata',
+                                identifier=100,
+                                args=(['my data'],))
+
+    def test_edit_blank(self):
+        # Now test a blank edit
+        self.assertTrue(self.vs.edit, 100)
+
+    def test_edit_full(self):
+        result = self.vs.edit(100,
+                              hostname='new-host',
+                              domain='new.sftlyr.ws',
+                              notes='random notes')
+
+        self.assertEqual(result, True)
+        args = ({
+                    'hostname': 'new-host',
+                    'domain': 'new.sftlyr.ws',
+                    'notes': 'random notes',
+                },)
+        self.assert_called_with('SoftLayer_Virtual_Guest', 'editObject',
+                                identifier=100,
+                                args=args)
+
+    def test_edit_tags(self):
+        # Test tag support
+        result = self.vs.edit(100, tags='dev,green')
+
+        self.assertEqual(result, True)
+        self.assert_called_with('SoftLayer_Virtual_Guest', 'setTags',
+                                identifier=100,
+                                args=('dev,green',))
+
+    def test_edit_tags_blank(self):
+        result = self.vs.edit(100, tags='')
+
+        self.assertEqual(result, True)
+        self.assert_called_with('SoftLayer_Virtual_Guest', 'setTags',
+                                identifier=100,
+                                args=('',))
+
+    def test_captures(self):
+        # capture only the OS disk
+        result = self.vs.capture(1, 'a')
+
+        expected = fixtures.SoftLayer_Virtual_Guest.createArchiveTemplate
+        self.assertEqual(result, expected)
+        args = ('a', [{'device': 0, 'uuid': 1, 'mountType': 'Disk'}], None)
+        self.assert_called_with('SoftLayer_Virtual_Guest',
+                                'createArchiveTemplate',
+                                args=args,
+                                identifier=1)
+
+    def test_capture_additional_disks(self):
+        # capture all the disks, minus the swap
+        # make sure the data is carried along with it
+        result = self.vs.capture(1, 'a', additional_disks=True)
+
+        expected = fixtures.SoftLayer_Virtual_Guest.createArchiveTemplate
+        self.assertEqual(result, expected)
+        args = ('a', [{'device': 0, 'mountType': 'Disk', 'uuid': 1},
+                      {'device': 3, 'mountType': 'Disk', 'uuid': 3}], None)
+        self.assert_called_with('SoftLayer_Virtual_Guest',
+                                'createArchiveTemplate',
+                                args=args,
+                                identifier=1)
+
+    def test_usage_vs_cpu(self):
+        result = self.vs.get_summary_data_usage('100',
+                                                start_date='2019-3-4',
+                                                end_date='2019-4-2',
+                                                valid_type='CPU0',
+                                                summary_period=300)
+
+        expected = fixtures.SoftLayer_Metric_Tracking_Object.getSummaryData
+        self.assertEqual(result, expected)
+
+        args = ('2019-3-4', '2019-4-2', [{"keyName": "CPU0", "summaryType": "max"}], 300)
+
+        self.assert_called_with('SoftLayer_Metric_Tracking_Object',
+                                'getSummaryData', args=args, identifier=1000)
+
+    def test_usage_vs_memory(self):
+        result = self.vs.get_summary_data_usage('100',
+                                                start_date='2019-3-4',
+                                                end_date='2019-4-2',
+                                                valid_type='MEMORY_USAGE',
+                                                summary_period=300)
+
+        expected = fixtures.SoftLayer_Metric_Tracking_Object.getSummaryData
+        self.assertEqual(result, expected)
+
+        args = ('2019-3-4', '2019-4-2', [{"keyName": "MEMORY_USAGE", "summaryType": "max"}], 300)
+
+        self.assert_called_with('SoftLayer_Metric_Tracking_Object', 'getSummaryData', args=args, identifier=1000)
+
+    def test_get_tracking_id(self):
+        result = self.vs.get_tracking_id(1234)
+        self.assert_called_with('SoftLayer_Virtual_Guest', 'getMetricTrackingObjectId')
+        self.assertEqual(result, 1000)
+
+    def test_get_bandwidth_data(self):
+        result = self.vs.get_bandwidth_data(1234, '2019-01-01', '2019-02-01', 'public', 1000)
+        self.assert_called_with('SoftLayer_Metric_Tracking_Object',
+                                'getBandwidthData',
+                                args=('2019-01-01', '2019-02-01', 'public', 1000),
+                                identifier=1000)
+        self.assertEqual(result[0]['type'], 'cpu0')
+
+    def test_get_bandwidth_allocation(self):
+        result = self.vs.get_bandwidth_allocation(1234)
+        self.assert_called_with('SoftLayer_Virtual_Guest', 'getBandwidthAllotmentDetail', identifier=1234)
+        self.assert_called_with('SoftLayer_Virtual_Guest', 'getBillingCycleBandwidthUsage', identifier=1234)
+        self.assertEqual(result['allotment']['amount'], '250')
+        self.assertEqual(result['usage'][0]['amountIn'], '.448')
+
+    def test_get_bandwidth_allocation_no_allotment(self):
+        mock = self.set_mock('SoftLayer_Virtual_Guest', 'getBandwidthAllotmentDetail')
+        mock.return_value = None
+
+        result = self.vs.get_bandwidth_allocation(1234)
+
+        self.assertEqual(None, result['allotment'])
+
+    def test_get_bandwidth_allocation_with_allotment(self):
+        mock = self.set_mock('SoftLayer_Virtual_Guest', 'getBandwidthAllotmentDetail')
+        mock.return_value = {
+            "allocationId": 11111,
+            "id": 22222,
+            "allocation": {
+                "amount": "2000"
+            }
+        }
+
+        result = self.vs.get_bandwidth_allocation(1234)
+
+        self.assertEqual(2000, int(result['allotment']['amount']))
+
+    def test_get_storage_iscsi_details(self):
+        mock = self.set_mock('SoftLayer_Virtual_Guest', 'getAttachedNetworkStorages')
         mock.return_value = [
             {
-                "id": 11111,
-                "serialNumber": "z1w4sdf",
-                "hardwareComponentModel": {
-                    "capacity": "1000",
-                    "description": "SATAIII:2000:8300:Constellation",
-                    "id": 111,
-                    "manufacturer": "Seagate",
-                    "name": "Constellation ES",
-                    "hardwareGenericComponentModel": {
-                        "capacity": "1000",
-                        "units": "GB",
-                        "hardwareComponentType": {
-                            "id": 1,
-                            "keyName": "HARD_DRIVE",
-                            "type": "Hard Drive",
-                            "typeParentId": 5
-                        }
-                    }
-                }
+                "accountId": 11111,
+                "capacityGb": 12000,
+                "id": 3777123,
+                "nasType": "ISCSI",
+                "username": "SL02SEL31111-9",
             }
         ]
-        result = self.run_command(['server', 'detail', '100'])
 
-        self.assert_no_fail(result)
-        output = json.loads(result.output)
-        self.assertEqual(output['drives'][0]['Capacity'], '1000 GB')
-        self.assertEqual(output['drives'][0]['Name'], 'Seagate Constellation ES')
-        self.assertEqual(output['drives'][0]['Serial #'], 'z1w4sdf')
+        result = self.vs.get_storage_details(1234, 'ISCSI')
 
-    def test_list_servers(self):
-        result = self.run_command(['server', 'list', '--tag=openstack'])
+        self.assertEqual([{
+            "accountId": 11111,
+            "capacityGb": 12000,
+            "id": 3777123,
+            "nasType": "ISCSI",
+            "username": "SL02SEL31111-9",
+        }], result)
+
+    def test_get_storage_iscsi_empty_details(self):
+        mock = self.set_mock('SoftLayer_Virtual_Guest', 'getAttachedNetworkStorages')
+        mock.return_value = []
 
-        expected = [
-            {
-                'datacenter': 'TEST00',
-                'primary_ip': '172.16.1.100',
-                'hostname': 'hardware-test1',
-                'id': 1000,
-                'backend_ip': '10.1.0.2',
-                'action': 'TXN_NAME',
-            },
+        result = self.vs.get_storage_details(1234, 'ISCSI')
+
+        self.assertEqual([], result)
+
+    def test_get_storage_nas_details(self):
+        mock = self.set_mock('SoftLayer_Virtual_Guest', 'getAttachedNetworkStorages')
+        mock.return_value = [
             {
-                'datacenter': 'TEST00',
-                'primary_ip': '172.16.4.94',
-                'hostname': 'hardware-test2',
-                'id': 1001,
-                'backend_ip': '10.1.0.3',
-                'action': None,
-            },
+                "accountId": 11111,
+                "capacityGb": 12000,
+                "id": 3777111,
+                "nasType": "NAS",
+                "username": "SL02SEL32222-9",
+            }
+        ]
+
+        result = self.vs.get_storage_details(1234, 'NAS')
+
+        self.assertEqual([{
+            "accountId": 11111,
+            "capacityGb": 12000,
+            "id": 3777111,
+            "nasType": "NAS",
+            "username": "SL02SEL32222-9",
+        }], result)
+
+    def test_get_storage_nas_empty_details(self):
+        mock = self.set_mock('SoftLayer_Virtual_Guest', 'getAttachedNetworkStorages')
+        mock.return_value = []
+
+        result = self.vs.get_storage_details(1234, 'NAS')
+
+        self.assertEqual([], result)
+
+    def test_get_storage_credentials(self):
+        mock = self.set_mock('SoftLayer_Virtual_Guest', 'getAllowedHost')
+        mock.return_value = {
+            "accountId": 11111,
+            "id": 33333,
+            "name": "iqn.2020-03.com.ibm:sl02su11111-v62941551",
+            "resourceTableName": "VIRTUAL_GUEST",
+            "credential": {
+                "accountId": "11111",
+                "id": 44444,
+                "password": "SjFDCpHrjskfj",
+                "username": "SL02SU11111-V62941551"
+            }
+        }
+
+        result = self.vs.get_storage_credentials(1234)
+
+        self.assertEqual({
+            "accountId": 11111,
+            "id": 33333,
+            "name": "iqn.2020-03.com.ibm:sl02su11111-v62941551",
+            "resourceTableName": "VIRTUAL_GUEST",
+            "credential": {
+                "accountId": "11111",
+                "id": 44444,
+                "password": "SjFDCpHrjskfj",
+                "username": "SL02SU11111-V62941551"
+            }
+        }, result)
+
+    def test_get_none_storage_credentials(self):
+        mock = self.set_mock('SoftLayer_Virtual_Guest', 'getAllowedHost')
+        mock.return_value = None
+
+        result = self.vs.get_storage_credentials(1234)
+
+        self.assertEqual(None, result)
+
+    def test_get_portable_storage(self):
+        result = self.vs.get_portable_storage(1234)
+        self.assert_called_with('SoftLayer_Account',
+                                'getPortableStorageVolumes')
+
+        self.assertEqual([
             {
-                'datacenter': 'TEST00',
-                'primary_ip': '172.16.4.95',
-                'hostname': 'hardware-bad-memory',
-                'id': 1002,
-                'backend_ip': '10.1.0.4',
-                'action': None,
-            },
+                "capacity": 200,
+                "createDate": "2018-10-06T04:27:59-06:00",
+                "description": "Disk 2",
+                "id": 11111,
+                "modifyDate": "",
+                "name": "Disk 2",
+                "parentId": "",
+                "storageRepositoryId": 22222,
+                "typeId": 241,
+                "units": "GB",
+                "uuid": "fd477feb-bf32-408e-882f-02540gghgh111"
+            }
+        ], result)
+
+    def test_get_portable_storage_empty(self):
+        mock = self.set_mock('SoftLayer_Account', 'getPortableStorageVolumes')
+        mock.return_value = []
+
+        result = self.vs.get_portable_storage(1234)
+
+        self.assertEqual([], result)
+
+    def test_get_local_disks_system(self):
+        mock = self.set_mock('SoftLayer_Virtual_Guest', 'getBlockDevices')
+        mock.return_value = [
             {
-                'action': None,
-                'backend_ip': None,
-                'datacenter': None,
-                'hostname': None,
-                'id': 1003,
-                'primary_ip': None,
-            },
+                "createDate": "2018-10-06T04:27:35-06:00",
+                "device": "0",
+                "id": 11111,
+                "mountType": "Disk",
+                "diskImage": {
+                    "capacity": 100,
+                    "description": "adns.vmware.com",
+                    "id": 72222,
+                    "name": "adns.vmware.com",
+                    "units": "GB",
+                }
+            }
         ]
 
-        self.assert_no_fail(result)
-        self.assertEqual(expected, json.loads(result.output))
+        result = self.vs.get_local_disks(1234)
 
-    @mock.patch('SoftLayer.CLI.formatting.no_going_back')
-    @mock.patch('SoftLayer.HardwareManager.reload')
-    def test_server_reload(self, reload_mock, ngb_mock):
-        ngb_mock.return_value = False
-
-        # Check the positive case
-        result = self.run_command(['--really', 'server', 'reload', '12345', '--key=4567'])
-
-        self.assert_no_fail(result)
-        reload_mock.assert_called_with(12345, None, [4567], False)
-
-        # LVM switch
-        result = self.run_command(['--really', 'server', 'reload', '12345', '--lvm'])
-        self.assert_no_fail(result)
-        reload_mock.assert_called_with(12345, None, [], True)
-
-        # Now check to make sure we properly call CLIAbort in the negative case
-        result = self.run_command(['server', 'reload', '12345'])
-
-        self.assertEqual(result.exit_code, 2)
-        self.assertIsInstance(result.exception, exceptions.CLIAbort)
-
-    @mock.patch('SoftLayer.CLI.formatting.no_going_back')
-    @mock.patch('SoftLayer.HardwareManager.cancel_hardware')
-    def test_cancel_server(self, cancel_mock, ngb_mock):
-        ngb_mock.return_value = False
-
-        # Check the positive case
-        result = self.run_command(['--really', 'server', 'cancel', '12345',
-                                   '--reason=Test', '--comment=Test'])
-
-        self.assert_no_fail(result)
-        cancel_mock.assert_called_with(12345, "Test", "Test", False)
-
-        # Test
-        result = self.run_command(['server', 'cancel', '12345',
-                                   '--reason=Test', '--comment=Test'])
-
-        self.assertEqual(result.exit_code, 2)
-        self.assertIsInstance(result.exception, exceptions.CLIAbort)
-
-    @mock.patch('SoftLayer.CLI.formatting.confirm')
-    def test_server_power_off(self, confirm_mock):
-        # Check the positive case
-        result = self.run_command(['--really', 'server', 'power-off', '12345'])
-
-        self.assert_called_with('SoftLayer_Hardware_Server', 'powerOff',
-                                identifier=12345)
-
-        # Now check to make sure we properly call CLIAbort in the negative case
-        confirm_mock.return_value = False
-        result = self.run_command(['server', 'power-off', '12345'])
-
-        self.assertEqual(result.exit_code, 2)
-        self.assertIsInstance(result.exception, exceptions.CLIAbort)
-
-    def test_server_reboot_default(self):
-        result = self.run_command(['--really', 'server', 'reboot', '12345'])
-
-        self.assert_no_fail(result)
-        self.assert_called_with('SoftLayer_Hardware_Server', 'rebootDefault',
-                                identifier=12345)
-
-    def test_server_reboot_soft(self):
-        result = self.run_command(['--really', 'server', 'reboot', '12345',
-                                   '--soft'])
-
-        self.assert_no_fail(result)
-        self.assert_called_with('SoftLayer_Hardware_Server', 'rebootSoft',
-                                identifier=12345)
-
-    def test_server_reboot_hard(self):
-        result = self.run_command(['--really', 'server', 'reboot', '12345',
-                                   '--hard'])
-
-        self.assert_no_fail(result)
-        self.assert_called_with('SoftLayer_Hardware_Server', 'rebootHard',
-                                identifier=12345)
-
-    @mock.patch('SoftLayer.CLI.formatting.confirm')
-    def test_server_reboot_negative(self, confirm_mock):
-        confirm_mock.return_value = False
-        result = self.run_command(['server', 'reboot', '12345'])
-
-        self.assertEqual(result.exit_code, 2)
-        self.assertIsInstance(result.exception, exceptions.CLIAbort)
-
-    def test_server_power_on(self):
-        result = self.run_command(['--really', 'server', 'power-on', '12345'])
-
-        self.assert_no_fail(result)
-        self.assert_called_with('SoftLayer_Hardware_Server', 'powerOn',
-                                identifier=12345)
-
-    @mock.patch('SoftLayer.CLI.formatting.confirm')
-    def test_harware_power_on_force(self, confirm_mock):
-        confirm_mock.return_value = False
-        result = self.run_command(['hardware', 'power-on', '12345'])
-        self.assertEqual(2, result.exit_code)
-        self.assertEqual('Aborted.', result.exception.message)
-
-    @mock.patch('SoftLayer.CLI.formatting.confirm')
-    def test_harware_power_off_force(self, confirm_mock):
-        confirm_mock.return_value = False
-        result = self.run_command(['hardware', 'power-off', '12345'])
-        self.assertEqual(2, result.exit_code)
-        self.assertEqual('Aborted.', result.exception.message)
-
-    def test_server_power_cycle(self):
-        result = self.run_command(['--really', 'server', 'power-cycle',
-                                   '12345'])
-
-        self.assert_no_fail(result)
-        self.assert_called_with('SoftLayer_Hardware_Server', 'powerCycle',
-                                identifier=12345)
-
-    @mock.patch('SoftLayer.CLI.formatting.confirm')
-    def test_server_power_cycle_negative(self, confirm_mock):
-        confirm_mock.return_value = False
-        result = self.run_command(['server', 'power-cycle', '12345'])
-
-        self.assertEqual(result.exit_code, 2)
-        self.assertIsInstance(result.exception, exceptions.CLIAbort)
-
-    @mock.patch('SoftLayer.HardwareManager.verify_order')
-    def test_create_server_test_flag(self, verify_mock):
-        verify_mock.return_value = {
-            'prices': [
-                {
-                    'recurringFee': 0.0,
-                    'setupFee': 0.0,
-                    'item': {'description': 'First Item'},
-                },
-                {
-                    'recurringFee': 25.0,
-                    'setupFee': 0.0,
-                    'item': {'description': 'Second Item'},
+        self.assertEqual([
+            {
+                "createDate": "2018-10-06T04:27:35-06:00",
+                "device": "0",
+                "id": 11111,
+                "mountType": "Disk",
+                "diskImage": {
+                    "capacity": 100,
+                    "description": "adns.vmware.com",
+                    "id": 72222,
+                    "name": "adns.vmware.com",
+                    "units": "GB",
                 }
-            ]
-        }
+            }
+        ], result)
 
-        result = self.run_command(['--really', 'server', 'create',
-                                   '--size=S1270_8GB_2X1TBSATA_NORAID',
-                                   '--hostname=test',
-                                   '--domain=example.com',
-                                   '--datacenter=TEST00',
-                                   '--port-speed=100',
-                                   '--os=UBUNTU_12_64',
-                                   '--test'],
-                                  fmt='raw')
-
-        self.assert_no_fail(result)
-        self.assertIn("First Item", result.output)
-        self.assertIn("Second Item", result.output)
-        self.assertIn("Total monthly cost", result.output)
-
-    def test_create_options(self):
-        result = self.run_command(['server', 'create-options'])
-
-        self.assert_no_fail(result)
-        output = json.loads(result.output)
-        self.assertEqual(output[0][0]['Value'], 'wdc07')
-
-    def test_create_options_prices(self):
-        result = self.run_command(['server', 'create-options', '--prices'])
-
-        self.assert_no_fail(result)
-        output = json.loads(result.output)
-        self.assertEqual(output[2][0]['Monthly'], str(0.1))
-        self.assertEqual(output[2][0]['Key'], 'OS_UBUNTU_14_04_LTS_TRUSTY_TAHR_64_BIT')
-
-    def test_create_options_location(self):
-        result = self.run_command(['server', 'create-options', '--prices', 'dal13'])
-
-        self.assert_no_fail(result)
-        output = json.loads(result.output)
-        self.assertEqual(output[2][0]['Monthly'], str(0.1))
-        self.assertEqual(output[2][0]['Key'], 'OS_UBUNTU_14_04_LTS_TRUSTY_TAHR_64_BIT')
-
-    @mock.patch('SoftLayer.HardwareManager.place_order')
-    def test_create_server(self, order_mock):
-        order_mock.return_value = {
-            'orderId': 98765,
-            'orderDate': '2013-08-02 15:23:47'
-        }
-
-        result = self.run_command(['--really', 'server', 'create',
-                                   '--size=S1270_8GB_2X1TBSATA_NORAID',
-                                   '--hostname=test',
-                                   '--domain=example.com',
-                                   '--datacenter=TEST00',
-                                   '--port-speed=100',
-                                   '--os=OS_UBUNTU_14_04_LTS_TRUSTY_TAHR_64_BIT',
-                                   '--no-public',
-                                   '--key=10',
-                                   ])
-
-        self.assert_no_fail(result)
-        self.assertIn('Warning: Closed soon: TEST00.pod2', result.output)
-        self.assertIn('"id": 98765', result.output)
-
-        result = self.run_command(['--really', 'server', 'create',
-                                   '--size=S1270_8GB_2X1TBSATA_NORAID',
-                                   '--hostname=test',
-                                   '--domain=example.com',
-                                   '--datacenter=mex01',
-                                   '--os=OS_UBUNTU_14_04_LTS_TRUSTY_TAHR_64_BIT',
-                                   ])
-
-        self.assert_no_fail(result)
-        self.assertNotIn('Warning: Closed soon: mex01', result.output)
-
-    @mock.patch('SoftLayer.CLI.template.export_to_template')
-    def test_create_server_with_export(self, export_mock):
-
-        result = self.run_command(['--really', 'server', 'create',
-                                   '--size=S1270_8GB_2X1TBSATA_NORAID',
-                                   '--hostname=test',
-                                   '--domain=example.com',
-                                   '--datacenter=TEST00',
-                                   '--port-speed=100',
-                                   '--os=UBUNTU_12_64',
-                                   '--no-public',
-                                   '--export=/path/to/test_file.txt'],
-                                  fmt='raw')
-
-        self.assert_no_fail(result)
-        self.assertIn("Successfully exported options to a template file.", result.output)
-        export_mock.assert_called_once()
-
-    @mock.patch('SoftLayer.HardwareManager.place_order')
-    def test_create_server_with_router(self, order_mock):
-        order_mock.return_value = {
-            'orderId': 98765,
-            'orderDate': '2013-08-02 15:23:47'
-        }
-
-        result = self.run_command(['--really', 'server', 'create',
-                                   '--size=S1270_8GB_2X1TBSATA_NORAID',
-                                   '--hostname=test',
-                                   '--domain=example.com',
-                                   '--datacenter=TEST00',
-                                   '--port-speed=100',
-                                   '--os=OS_UBUNTU_14_04_LTS_TRUSTY_TAHR_64_BIT',
-                                   '--router-private=123',
-                                   '--router-public=1234'
-                                   ])
-
-        self.assert_no_fail(result)
-
-    def test_edit_server_userdata_and_file(self):
-        # Test both userdata and userfile at once
-        with tempfile.NamedTemporaryFile() as userfile:
-            result = self.run_command(['server', 'edit', '1000',
-                                       '--hostname=hardware-test1',
-                                       '--domain=test.sftlyr.ws',
-                                       '--userdata=My data',
-                                       '--userfile=%s' % userfile.name])
-
-            self.assertEqual(result.exit_code, 2)
-            self.assertIsInstance(result.exception, exceptions.ArgumentError)
-
-    def test_edit_server_userdata(self):
-        result = self.run_command(['server', 'edit', '1000',
-                                   '--hostname=hardware-test1',
-                                   '--domain=test.sftlyr.ws',
-                                   '--userdata=My data'])
-
-        self.assert_no_fail(result)
-        self.assertEqual(result.output, "")
-        self.assert_called_with('SoftLayer_Hardware_Server', 'editObject',
-                                args=({'domain': 'test.sftlyr.ws',
-                                       'hostname': 'hardware-test1'},),
-                                identifier=1000)
+    def test_get_local_disks_empty(self):
+        mock = self.set_mock('SoftLayer_Virtual_Guest', 'getBlockDevices')
+        mock.return_value = []
 
-    @mock.patch('SoftLayer.HardwareManager.edit')
-    def test_edit_server_failed(self, edit_mock):
-        edit_mock.return_value = False
-        result = self.run_command(['server', 'edit', '1000',
-                                   '--hostname=hardware-test1',
-                                   '--domain=test.sftlyr.ws',
-                                   '--userdata=My data'])
-
-        self.assertEqual(result.exit_code, 2)
-        self.assertEqual(result.output, "")
-        edit_mock.assert_called_with(1000,
-                                     userdata='My data',
-                                     domain='test.sftlyr.ws',
-                                     hostname='hardware-test1')
-
-    def test_edit_server_userfile(self):
-        if (sys.platform.startswith("win")):
-            self.skipTest("Test doesn't work in Windows")
-        with tempfile.NamedTemporaryFile() as userfile:
-            userfile.write(b"some data")
-            userfile.flush()
-            result = self.run_command(['server', 'edit', '1000',
-                                       '--userfile=%s' % userfile.name])
-
-            self.assert_no_fail(result)
-            self.assertEqual(result.output, "")
-            self.assert_called_with('SoftLayer_Hardware_Server',
-                                    'setUserMetadata',
-                                    args=(['some data'],),
-                                    identifier=1000)
-
-    @mock.patch('SoftLayer.CLI.formatting.confirm')
-    def test_update_firmware(self, confirm_mock):
-        confirm_mock.return_value = True
-        result = self.run_command(['server', 'update-firmware', '1000'])
-
-        self.assert_no_fail(result)
-        self.assertEqual(result.output, "")
-        self.assert_called_with('SoftLayer_Hardware_Server',
-                                'createFirmwareUpdateTransaction',
-                                args=((1, 1, 1, 1)), identifier=1000)
-
-    @mock.patch('SoftLayer.CLI.formatting.confirm')
-    def test_reflash_firmware(self, confirm_mock):
-        confirm_mock.return_value = True
-        result = self.run_command(['server', 'reflash-firmware', '1000'])
-
-        self.assert_no_fail(result)
-        self.assertEqual(result.output, 'Successfully device firmware reflashed\n')
-        self.assert_called_with('SoftLayer_Hardware_Server',
-                                'createFirmwareReflashTransaction',
-                                args=((1, 1, 1)), identifier=1000)
-
-    def test_edit(self):
-        result = self.run_command(['server', 'edit',
-                                   '--domain=example.com',
-                                   '--hostname=host',
-                                   '--userdata="testdata"',
-                                   '--tag=dev',
-                                   '--tag=green',
-                                   '--public-speed=10',
-                                   '--redundant',
-                                   '--private-speed=100',
-                                   '--degraded',
-                                   '100'])
-
-        self.assert_no_fail(result)
-        self.assertEqual(result.output, '')
-
-        self.assert_called_with(
-            'SoftLayer_Hardware_Server', 'editObject',
-            args=({'domain': 'example.com', 'hostname': 'host'},),
-            identifier=100,
-        )
-        self.assert_called_with(
-            'SoftLayer_Hardware_Server', 'setUserMetadata',
-            args=(['"testdata"'],),
-            identifier=100,
-        )
-        self.assert_called_with(
-            'SoftLayer_Hardware_Server', 'setPublicNetworkInterfaceSpeed',
-            args=([10, 'redundant'],),
-            identifier=100,
-        )
-        self.assert_called_with(
-            'SoftLayer_Hardware_Server', 'setPrivateNetworkInterfaceSpeed',
-            args=([100, 'degraded'],),
-            identifier=100,
-        )
-
-    @mock.patch('SoftLayer.CLI.formatting.confirm')
-    def test_rescue(self, confirm_mock):
-        confirm_mock.return_value = True
-        result = self.run_command(['server', 'rescue', '1000'])
-
-        self.assert_no_fail(result)
-        self.assertEqual(result.output, "")
-        self.assert_called_with('SoftLayer_Hardware_Server', 'bootToRescueLayer', identifier=1000)
-
-    @mock.patch('SoftLayer.CLI.formatting.confirm')
-    def test_server_rescue_negative(self, confirm_mock):
-        confirm_mock.return_value = False
-        result = self.run_command(['server', 'rescue', '1000'])
+        result = self.vs.get_local_disks(1234)
 
-        self.assertEqual(result.exit_code, 2)
-        self.assertIsInstance(result.exception, exceptions.CLIAbort)
+        self.assertEqual([], result)
 
-    def test_ready(self):
-        mock = self.set_mock('SoftLayer_Hardware_Server', 'getObject')
-        mock.return_value = {
-            "provisionDate": "2017-10-17T11:21:53-07:00",
-            "id": 41957081
-        }
-        result = self.run_command(['hw', 'ready', '100'])
-        self.assert_no_fail(result)
-        self.assertEqual(result.output, '"READY"\n')
-
-    def test_not_ready(self):
-        mock = self.set_mock('SoftLayer_Hardware_Server', 'getObject')
-        not_ready = {
-            'activeTransaction': {
-                'transactionStatus': {'friendlyName': 'Attach Primary Disk'}
-            },
-            'provisionDate': '',
-            'id': 47392219
-        }
-        ready = {
-            "provisionDate": "2017-10-17T11:21:53-07:00",
-            "id": 41957081
-        }
-        mock.side_effect = [not_ready, ready]
-        result = self.run_command(['hw', 'ready', '100'])
-        self.assertEqual(result.exit_code, 2)
-        self.assertIsInstance(result.exception, exceptions.CLIAbort)
-
-    @mock.patch('time.sleep')
-    def test_going_ready(self, _sleep):
-        mock = self.set_mock('SoftLayer_Hardware_Server', 'getObject')
-        not_ready = {
-            'activeTransaction': {
-                'transactionStatus': {'friendlyName': 'Attach Primary Disk'}
-            },
-            'provisionDate': '',
-            'id': 47392219
-        }
-        ready = {
-            "provisionDate": "2017-10-17T11:21:53-07:00",
-            "id": 41957081
-        }
-        mock.side_effect = [not_ready, ready]
-        result = self.run_command(['hw', 'ready', '100', '--wait=100'])
-        self.assert_no_fail(result)
-        self.assertEqual(result.output, '"READY"\n')
-
-    def test_toggle_ipmi_on(self):
-        mock.return_value = True
-        result = self.run_command(['server', 'toggle-ipmi', '--enable', '12345'])
-        self.assert_no_fail(result)
-        self.assertEqual(result.output, 'true\n')
-
-    def test_toggle_ipmi_off(self):
-        mock.return_value = True
-        result = self.run_command(['server', 'toggle-ipmi', '--disable', '12345'])
-        self.assert_no_fail(result)
-        self.assertEqual(result.output, 'true\n')
-
-    def test_bandwidth_hw(self):
-        if sys.version_info < (3, 6):
-            self.skipTest("Test requires python 3.6+")
-        result = self.run_command(['server', 'bandwidth', '100', '--start_date=2019-01-01', '--end_date=2019-02-01'])
-        self.assert_no_fail(result)
-
-        date = '2019-05-20 23:00'
-        # only pyhon 3.7 supports the timezone format slapi uses
-        if sys.version_info < (3, 7):
-            date = '2019-05-20T23:00:00-06:00'
-
-        split_output = []
-        for table in utils.decode_stacked(result.output):
-            split_output.append(table)
-
-        self.assertEqual(len(split_output), 2)
-        output_summary = split_output[0]
-        output_list = split_output[1]
-
-        self.assertEqual(output_summary[0]['Average MBps'], 0.3841)
-        self.assertEqual(output_summary[1]['Max Date'], date)
-        self.assertEqual(output_summary[2]['Max GB'], 0.1172)
-        self.assertEqual(output_summary[3]['Sum GB'], 0.0009)
-
-        self.assertEqual(output_list[0]['Date'], date)
-        self.assertEqual(output_list[0]['Pub In'], 1.3503)
-
-    def test_bandwidth_hw_quite(self):
-        result = self.run_command(['server', 'bandwidth', '100', '--start_date=2019-01-01',
-                                   '--end_date=2019-02-01', '-q'])
-        self.assert_no_fail(result)
-        date = '2019-05-20 23:00'
-
-        # only pyhon 3.7 supports the timezone format slapi uses
-        if sys.version_info < (3, 7):
-            date = '2019-05-20T23:00:00-06:00'
-
-        output_summary = json.loads(result.output)
-
-        self.assertEqual(output_summary[0]['Average MBps'], 0.3841)
-        self.assertEqual(output_summary[1]['Max Date'], date)
-        self.assertEqual(output_summary[2]['Max GB'], 0.1172)
-        self.assertEqual(output_summary[3]['Sum GB'], 0.0009)
-
-    @mock.patch('SoftLayer.CLI.formatting.confirm')
-    def test_dns_sync_both(self, confirm_mock):
-        confirm_mock.return_value = True
-        getReverseDomainRecords = self.set_mock('SoftLayer_Hardware_Server',
-                                                'getReverseDomainRecords')
-        getReverseDomainRecords.return_value = [{
-            'networkAddress': '172.16.1.100',
-            'name': '2.240.16.172.in-addr.arpa',
-            'resourceRecords': [{'data': 'test.softlayer.com.',
-                                 'id': 100,
-                                 'host': '12'}],
-            'updateDate': '2013-09-11T14:36:57-07:00',
-            'serial': 1234665663,
-            'id': 123456,
-        }]
-        getResourceRecords = self.set_mock('SoftLayer_Dns_Domain',
-                                           'getResourceRecords')
-        getResourceRecords.return_value = []
-        createAargs = ({
-                           'type': 'a',
-                           'host': 'hardware-test1',
-                           'domainId': 12345,  # from SoftLayer_Account::getDomains
-                           'data': '172.16.1.100',
-                           'ttl': 7200
-                       },)
-        createPTRargs = ({
-                             'type': 'ptr',
-                             'host': '100',
-                             'domainId': 123456,
-                             'data': 'hardware-test1.test.sftlyr.ws',
-                             'ttl': 7200
-                         },)
-
-        result = self.run_command(['hw', 'dns-sync', '1000'])
-
-        self.assert_no_fail(result)
-        self.assert_called_with('SoftLayer_Dns_Domain', 'getResourceRecords')
-        self.assert_called_with('SoftLayer_Hardware_Server',
-                                'getReverseDomainRecords')
-        self.assert_called_with('SoftLayer_Dns_Domain_ResourceRecord',
-                                'createObject',
-                                args=createAargs)
-        self.assert_called_with('SoftLayer_Dns_Domain_ResourceRecord',
-                                'createObject',
-                                args=createPTRargs)
-
-    @mock.patch('SoftLayer.CLI.formatting.confirm')
-    def test_dns_sync_v6(self, confirm_mock):
-        confirm_mock.return_value = True
-        getResourceRecords = self.set_mock('SoftLayer_Dns_Domain',
-                                           'getResourceRecords')
-        getResourceRecords.return_value = []
-        server = self.set_mock('SoftLayer_Hardware_Server', 'getObject')
-        test_server = {
-            'id': 1000,
-            'hostname': 'hardware-test1',
-            'domain': 'sftlyr.ws',
-            'primaryIpAddress': '172.16.1.100',
-            'fullyQualifiedDomainName': 'hw-test1.sftlyr.ws',
-            "primaryNetworkComponent": {}
-        }
-        server.return_value = test_server
-
-        result = self.run_command(['hw', 'dns-sync', '--aaaa-record', '1000'])
-
-        self.assertEqual(result.exit_code, 2)
-        self.assertIsInstance(result.exception, exceptions.CLIAbort)
-
-        test_server['primaryNetworkComponent'] = {
-            'primaryVersion6IpAddressRecord': {
-                'ipAddress': '2607:f0d0:1b01:0023:0000:0000:0000:0004'
+    def test_get_local_disks_swap(self):
+        mock = self.set_mock('SoftLayer_Virtual_Guest', 'getBlockDevices')
+        mock.return_value = [
+            {
+                "device": "1",
+                "id": 22222,
+                "mountType": "Disk",
+                "statusId": 1,
+                "diskImage": {
+                    "capacity": 2,
+                    "description": "6211111-SWAP",
+                    "id": 33333,
+                    "name": "6211111-SWAP",
+                    "units": "GB",
+                }
             }
-        }
-        createV6args = ({
-                            'type': 'aaaa',
-                            'host': 'hardware-test1',
-                            'domainId': 12345,  # from SoftLayer_Account::getDomains
-                            'data': '2607:f0d0:1b01:0023:0000:0000:0000:0004',
-                            'ttl': 7200
-                        },)
-        server.return_value = test_server
-        result = self.run_command(['hw', 'dns-sync', '--aaaa-record', '1000'])
-        self.assert_no_fail(result)
-        self.assert_called_with('SoftLayer_Dns_Domain_ResourceRecord',
-                                'createObject',
-                                args=createV6args)
-
-        v6Record = {
-            'id': 1,
-            'ttl': 7200,
-            'data': '2607:f0d0:1b01:0023:0000:0000:0000:0004',
-            'host': 'hardware-test1',
-            'type': 'aaaa'
-        }
-
-        getResourceRecords = self.set_mock('SoftLayer_Dns_Domain',
-                                           'getResourceRecords')
-        getResourceRecords.return_value = [v6Record]
-        editArgs = (v6Record,)
-        result = self.run_command(['hw', 'dns-sync', '--aaaa-record', '1000'])
-        self.assert_no_fail(result)
-        self.assert_called_with('SoftLayer_Dns_Domain_ResourceRecord',
-                                'editObject',
-                                args=editArgs)
-
-        getResourceRecords = self.set_mock('SoftLayer_Dns_Domain',
-                                           'getResourceRecords')
-        getResourceRecords.return_value = [v6Record, v6Record]
-        result = self.run_command(['hw', 'dns-sync', '--aaaa-record', '1000'])
-        self.assertEqual(result.exit_code, 1)
-        self.assertIsInstance(result.exception, SoftLayerError)
-
-    @mock.patch('SoftLayer.CLI.formatting.confirm')
-    def test_dns_sync_edit_a(self, confirm_mock):
-        confirm_mock.return_value = True
-        getResourceRecords = self.set_mock('SoftLayer_Dns_Domain',
-                                           'getResourceRecords')
-        getResourceRecords.return_value = [
-            {'id': 1, 'ttl': 7200, 'data': '1.1.1.1',
-             'host': 'hardware-test1', 'type': 'a'}
         ]
-        editArgs = (
-            {'type': 'a', 'host': 'hardware-test1', 'data': '172.16.1.100',
-             'id': 1, 'ttl': 7200},
-        )
-        result = self.run_command(['hw', 'dns-sync', '-a', '1000'])
-        self.assert_no_fail(result)
-        self.assert_called_with('SoftLayer_Dns_Domain_ResourceRecord',
-                                'editObject',
-                                args=editArgs)
-
-        getResourceRecords = self.set_mock('SoftLayer_Dns_Domain',
-                                           'getResourceRecords')
-        getResourceRecords.return_value = [
-            {'id': 1, 'ttl': 7200, 'data': '1.1.1.1',
-             'host': 'hardware-test1', 'type': 'a'},
-            {'id': 2, 'ttl': 7200, 'data': '1.1.1.1',
-             'host': 'hardware-test1', 'type': 'a'}
-        ]
-        result = self.run_command(['hw', 'dns-sync', '-a', '1000'])
-        self.assertEqual(result.exit_code, 1)
-        self.assertIsInstance(result.exception, SoftLayerError)
-
-    @mock.patch('SoftLayer.CLI.formatting.confirm')
-    def test_dns_sync_edit_ptr(self, confirm_mock):
-        confirm_mock.return_value = True
-        getReverseDomainRecords = self.set_mock('SoftLayer_Hardware_Server',
-                                                'getReverseDomainRecords')
-        getReverseDomainRecords.return_value = [{
-            'networkAddress': '172.16.1.100',
-            'name': '100.1.16.172.in-addr.arpa',
-            'resourceRecords': [{'data': 'test.softlayer.com.',
-                                 'id': 123,
-                                 'host': '100'}],
-            'updateDate': '2013-09-11T14:36:57-07:00',
-            'serial': 1234665663,
-            'id': 123456,
-        }]
-        editArgs = ({'host': '100', 'data': 'hardware-test1.test.sftlyr.ws',
-                     'id': 123, 'ttl': 7200},)
-        result = self.run_command(['hw', 'dns-sync', '--ptr', '1000'])
-        self.assert_no_fail(result)
-        self.assert_called_with('SoftLayer_Dns_Domain_ResourceRecord',
-                                'editObject',
-                                args=editArgs)
-
-    @mock.patch('SoftLayer.CLI.formatting.confirm')
-    def test_dns_sync_misc_exception(self, confirm_mock):
-        confirm_mock.return_value = False
-        result = self.run_command(['hw', 'dns-sync', '-a', '1000'])
-        self.assertEqual(result.exit_code, 2)
-        self.assertIsInstance(result.exception, exceptions.CLIAbort)
-
-        guest = self.set_mock('SoftLayer_Hardware_Server', 'getObject')
-        test_guest = {
-            'id': 1000,
-            'primaryIpAddress': '',
-            'hostname': 'hardware-test1',
-            'domain': 'sftlyr.ws',
-            'fullyQualifiedDomainName': 'hardware-test1.sftlyr.ws',
-            "primaryNetworkComponent": {}
-        }
-        guest.return_value = test_guest
-        result = self.run_command(['hw', 'dns-sync', '-a', '1000'])
-        self.assertEqual(result.exit_code, 2)
-        self.assertIsInstance(result.exception, exceptions.CLIAbort)
-
-    def test_hardware_storage(self):
-        result = self.run_command(
-            ['hw', 'storage', '100'])
-
-        self.assert_no_fail(result)
-
-    def test_billing(self):
-        result = self.run_command(['hw', 'billing', '123456'])
-        hardware_server_billing = {
-            'Billing Item Id': 6327,
-            'Id': '123456',
-            'Provision Date': None,
-            'Recurring Fee': 1.54,
-            'Total': 16.08,
-            'prices': [
-                {
-                    'Item': 'test',
-                    'Recurring Price': 1
-                },
-                {
-                    'Item': 'test2',
-                    'Recurring Price': 2
-                },
-            ]
-        }
-        self.assert_no_fail(result)
-        self.assertEqual(json.loads(result.output), hardware_server_billing)
 
-    @mock.patch('SoftLayer.CLI.formatting.confirm')
-    def test_create_hw_no_confirm(self, confirm_mock):
-        confirm_mock.return_value = False
-
-        result = self.run_command(['hw', 'create', '--hostname=test', '--size=S1270_8GB_2X1TBSATA_NORAID',
-                                   '--domain=example.com', '--datacenter=TEST00',
-                                   '--network=TEST_NETWORK', '--os=UBUNTU_12_64'])
-
-        self.assertEqual(result.exit_code, 2)
-        self.assertEqual('Aborting dedicated server order.', result.exception.message)
-
-    @mock.patch('SoftLayer.CLI.formatting.confirm')
-    def test_authorize_hw_no_confirm(self, confirm_mock):
-        confirm_mock.return_value = False
-        result = self.run_command(['hw', 'authorize-storage', '-u', '1234'])
-
-        self.assertEqual(result.exit_code, 2)
-
-    @mock.patch('SoftLayer.CLI.formatting.confirm')
-    def test_authorize_hw_empty(self, confirm_mock):
-        confirm_mock.return_value = True
-        storage_result = self.set_mock('SoftLayer_Account', 'getNetworkStorage')
-        storage_result.return_value = []
-        result = self.run_command(['hw', 'authorize-storage', '--username-storage=#', '1234'])
-
-        self.assertEqual(str(result.exception), "The Storage with username: # was not found, "
-                                                "please enter a valid storage username")
-
-    def test_authorize_hw(self):
-        result = self.run_command(['hw', 'authorize-storage', '--username-storage=SL01SEL301234-11', '1234'])
-        self.assert_no_fail(result)
-
-    def test_upgrade_no_options(self, ):
-        result = self.run_command(['hw', 'upgrade', '100'])
-        self.assertEqual(result.exit_code, 2)
-        self.assertIsInstance(result.exception, exceptions.ArgumentError)
-
-    @mock.patch('SoftLayer.CLI.formatting.confirm')
-    def test_upgrade_aborted(self, confirm_mock):
-        confirm_mock.return_value = False
-        result = self.run_command(['hw', 'upgrade', '100', '--memory=1'])
-        self.assertEqual(result.exit_code, 2)
-        self.assertIsInstance(result.exception, exceptions.CLIAbort)
-
-    def test_upgrade_test(self):
-        order_mock = self.set_mock('SoftLayer_Product_Order', 'verifyOrder')
-        order_mock.return_value = SoftLayer_Product_Order.hardware_verifyOrder
-        result = self.run_command(['hw', 'upgrade', '100', '--test', '--memory=32', '--public-bandwidth=500',
-                                   '--drive-controller=RAID', '--network=10000 Redundant'])
-        self.assert_no_fail(result)
-
-    @mock.patch('SoftLayer.CLI.formatting.confirm')
-    def test_upgrade_add_disk(self, confirm_mock):
-        confirm_mock.return_value = True
-        order_mock = self.set_mock('SoftLayer_Product_Order', 'placeOrder')
-        order_mock.return_value = SoftLayer_Product_Order.hardware_placeOrder
-        result = self.run_command(['hw', 'upgrade', '100', '--add-disk=1000', '2'])
-
-        self.assert_no_fail(result)
-
-    @mock.patch('SoftLayer.CLI.formatting.confirm')
-    def test_upgrade_resize_disk(self, confirm_mock):
-        confirm_mock.return_value = True
-        order_mock = self.set_mock('SoftLayer_Product_Order', 'placeOrder')
-        order_mock.return_value = SoftLayer_Product_Order.hardware_placeOrder
-        result = self.run_command(['hw', 'upgrade', '100', '--resize-disk=1000', '1'])
-
-        self.assert_no_fail(result)
-
-    @mock.patch('SoftLayer.CLI.formatting.confirm')
-    def test_upgrade_disk_not_price_found(self, confirm_mock):
-        confirm_mock.return_value = False
-        result = self.run_command(['hw', 'upgrade', '100', '--add-disk=1000', '3'])
-        self.assertEqual(result.exit_code, 2)
-        self.assertIsInstance(result.exception, exceptions.CLIAbort)
-
-    @mock.patch('SoftLayer.CLI.formatting.confirm')
-    def test_upgrade_disk_already_exist(self, confirm_mock):
-        confirm_mock.return_value = False
-        result = self.run_command(['hw', 'upgrade', '100', '--add-disk=1000', '1'])
-        self.assertEqual(result.exit_code, 2)
-        self.assertIsInstance(result.exception, exceptions.CLIAbort)
-
-    @mock.patch('SoftLayer.CLI.formatting.confirm')
-    def test_upgrade_disk_does_not_exist(self, confirm_mock):
-        confirm_mock.return_value = False
-        result = self.run_command(['hw', 'upgrade', '100', '--resize-disk=1000', '3'])
-        self.assertEqual(result.exit_code, 2)
-        self.assertIsInstance(result.exception, exceptions.CLIAbort)
-
-    @mock.patch('SoftLayer.CLI.formatting.confirm')
-    def test_upgrade(self, confirm_mock):
-        confirm_mock.return_value = True
-        order_mock = self.set_mock('SoftLayer_Product_Order', 'placeOrder')
-        order_mock.return_value = SoftLayer_Product_Order.hardware_placeOrder
-        result = self.run_command(['hw', 'upgrade', '100', '--memory=32', '--public-bandwidth=500',
-                                   '--drive-controller=RAID', '--network=10000 Redundant'])
-
-        self.assert_no_fail(result)
-
-    def test_components(self):
-        result = self.run_command(['hardware', 'detail', '100', '--components'])
-        self.assert_no_fail(result)
-
-    def test_sensor(self):
-        result = self.run_command(['hardware', 'sensor', '100'])
-        self.assert_no_fail(result)
-
-    def test_sensor_discrete(self):
-        result = self.run_command(['hardware', 'sensor', '100', '--discrete'])
-        self.assert_no_fail(result)
-
-    def test_monitoring(self):
-        result = self.run_command(['hardware', 'monitoring', '100'])
-        self.assert_no_fail(result)
-
-    @mock.patch('SoftLayer.CLI.formatting.confirm')
-    def test_check_for_closing(self, confirm_mock):
-        confirm_mock.return_value = True
-        result = self.run_command(['vs', 'create', '--hostname', 'TEST', '--domain', 'TESTING',
-                                   '--flavor', 'B1_2X8X25', '--datacenter', 'ams01', '--os', 'UBUNTU_LATEST'])
-        self.assert_no_fail(result)
-        self.assertIn('Warning: Closed soon: ams01', result.output)
-        result = self.run_command(['vs', 'create', '--hostname', 'TEST', '--domain', 'TESTING',
-                                   '--flavor', 'B1_2X8X25', '--datacenter', 'mex01', '--os', 'UBUNTU_LATEST'])
-        self.assert_no_fail(result)
-        self.assertNotIn('Warning: Closed soon: mex01', result.output)
-
-    def test_notifications(self):
-        result = self.run_command(['hardware', 'notifications', '100'])
-        self.assert_no_fail(result)
+        result = self.vs.get_local_disks(1234)
+
+        self.assertEqual([
+            {
+                "device": "1",
+                "id": 22222,
+                "mountType": "Disk",
+                "statusId": 1,
+                "diskImage": {
+                    "capacity": 2,
+                    "description": "6211111-SWAP",
+                    "id": 33333,
+                    "name": "6211111-SWAP",
+                    "units": "GB",
+                }
+            }
+        ], result)
+
+    def test_migrate(self):
+        result = self.vs.migrate(1234)
+        self.assertTrue(result)
+        self.assert_called_with('SoftLayer_Virtual_Guest', 'migrate', identifier=1234)
+
+    def test_migrate_dedicated(self):
+        result = self.vs.migrate_dedicated(1234, 5555)
+        self.assertTrue(result)
+        self.assert_called_with('SoftLayer_Virtual_Guest', 'migrateDedicatedHost', args=(5555,), identifier=1234)
+
+    def test_authorize_storage(self):
+        options = self.vs.authorize_storage(1234, "SL01SEL301234-11")
+
+        self.assertEqual(True, options)
+
+    def test_authorize_storage_empty(self):
+        mock = self.set_mock('SoftLayer_Account', 'getNetworkStorage')
+        mock.return_value = []
+        self.assertRaises(SoftLayer.exceptions.SoftLayerError,
+                          self.vs.authorize_storage,
+                          1234, "#")
+
+    def test_authorize_portable_storage(self):
+        options = self.vs.attach_portable_storage(1234, 1234567)
+        self.assertEqual(1234567, options['id'])
+
+    def test_browser_access_log(self):
+        result = self.vs.browser_access_log(1234)
+        self.assertTrue(result)
+        self.assert_called_with('SoftLayer_Virtual_Guest', 'getBrowserConsoleAccessLogs', identifier=1234)
+
+    def test_notification(self):
+        self.vs.get_notifications(100)
+        self.assert_called_with('SoftLayer_User_Customer_Notification_Virtual_Guest', 'findByGuestId')
 
     def test_add_notification(self):
-        result = self.run_command(['hardware', 'notification-add', '100', '--users', '123456'])
-        self.assert_no_fail(result)
+        self.vs.add_notification(100, 123456)
+        self.assert_called_with('SoftLayer_User_Customer_Notification_Virtual_Guest', 'createObject')
 
-    def test_notification_delete(self):
-        result = self.run_command(['hardware', 'notification-delete', '100'])
-        self.assert_no_fail(result)
-
-    def test_create_credential(self):
-        result = self.run_command(['hw', 'create-credential', '123456',
-                                   '--username', 'testslcli', '--password', 'test-123456',
-                                   '--notes', 'test slcli', '--software', 'system'])
-        self.assert_no_fail(result)
-
-    def test_list_hw_search_noargs(self):
-        result = self.run_command(['hw', 'list', '--search'])
-        self.assert_no_fail(result)
-        self.assert_called_with('SoftLayer_Search', 'advancedSearch', args=('_objectType:SoftLayer_Hardware ',))
-
-    def test_list_hw_search_noargs_domain(self):
-        result = self.run_command(['hw', 'list', '--search', '-Dtest'])
-        self.assert_no_fail(result)
-        self.assert_called_with('SoftLayer_Search', 'advancedSearch',
-                                args=('_objectType:SoftLayer_Hardware  domain: *test*',))
+    def test_notification_del(self):
+        self.vs.remove_notification(100)
+        self.assert_called_with('SoftLayer_User_Customer_Notification_Virtual_Guest', 'deleteObjects')
```

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/sshkey_tests.py` & `softlayer-6.2.0/tests/CLI/modules/sshkey_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/ssl_tests.py` & `softlayer-6.2.0/tests/CLI/modules/ssl_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/subnet_tests.py` & `softlayer-6.2.0/tests/CLI/modules/subnet_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/summary_tests.py` & `softlayer-6.2.0/tests/CLI/modules/summary_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/tag_tests.py` & `softlayer-6.2.0/tests/CLI/modules/tag_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/ticket_tests.py` & `softlayer-6.2.0/tests/CLI/modules/ticket_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/user_tests.py` & `softlayer-6.2.0/tests/CLI/modules/user_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/vlan_tests.py` & `softlayer-6.2.0/tests/CLI/modules/vlan_tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,17 +143,23 @@
         self.assert_no_fail(result)
 
     @mock.patch('SoftLayer.CLI.formatting.no_going_back')
     def test_vlan_list_get_pod_with_closed_announcement(self, ngb_mock):
         ngb_mock.return_value = True
         vlan_mock = self.set_mock('SoftLayer_Account', 'getNetworkVlans')
         gpods_mock = self.set_mock('SoftLayer_Network_Pod', 'getAllObjects')
-        vlan_mock.return_value = {'primaryRouter': {'fullyQualifiedDomainName': 'bcr01a.fra02.softlayer.com',
-                                                    'id': 462912},
-                                  'tagReferences': ''}
+        vlan_mock.return_value = [
+            {
+                "primaryRouter": {
+                    "fullyQualifiedDomainName": "bcr01a.fra02.softlayer.com",
+                    "id": 462912
+                },
+                "tagReferences": ""
+            }
+        ]
         gpods_mock.return_value = [{'backendRouterId': 462912,
                                     'backendRouterName': 'bcr01a.fra02',
                                     'datacenterId': 449506,
                                     'datacenterLongName': 'Frankfurt 2',
                                     'frontendRouterId': 335916,
                                     'frontendRouterName': 'fcr01a.fra02',
                                     'name': 'fra02.pod01',
@@ -162,17 +168,23 @@
         self.assert_no_fail(result)
 
     @mock.patch('SoftLayer.CLI.formatting.no_going_back')
     def test_vlan_list_get_pod_with_closed_announcement_no_closure(self, ngb_mock):
         ngb_mock.return_value = True
         vlan_mock = self.set_mock('SoftLayer_Account', 'getNetworkVlans')
         gpods_mock = self.set_mock('SoftLayer_Network_Pod', 'getAllObjects')
-        vlan_mock.return_value = {'primaryRouter': {'fullyQualifiedDomainName': 'bcr01a.fra02.softlayer.com',
-                                                    'id': 462912},
-                                  'tagReferences': ''}
+        vlan_mock.return_value = [
+            {
+                "primaryRouter": {
+                    "fullyQualifiedDomainName": "bcr01a.fra02.softlayer.com",
+                    "id": 462912
+                },
+                "tagReferences": ""
+            }
+        ]
         gpods_mock.return_value = [{'backendRouterId': 462912,
                                     'backendRouterName': 'bcr01a.fra02',
                                     'datacenterId': 449506,
                                     'datacenterLongName': 'Frankfurt 2',
                                     'frontendRouterId': 335916,
                                     'frontendRouterName': 'fcr01a.fra02',
                                     'name': 'fra02.pod01',
```

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/vs/vs_capacity_tests.py` & `softlayer-6.2.0/tests/CLI/modules/vs/vs_capacity_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/vs/vs_create_tests.py` & `softlayer-6.2.0/tests/CLI/modules/vs/vs_create_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/vs/vs_placement_tests.py` & `softlayer-6.2.0/tests/CLI/modules/vs/vs_placement_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/CLI/modules/vs/vs_tests.py` & `softlayer-6.2.0/tests/CLI/modules/vs/vs_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/managers/account_tests.py` & `softlayer-6.2.0/tests/managers/account_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/managers/bandwidth_tests.py` & `softlayer-6.2.0/tests/managers/bandwidth_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/managers/block_tests.py` & `softlayer-6.2.0/tests/managers/block_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/managers/cdn_tests.py` & `softlayer-6.2.0/tests/managers/cdn_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/managers/dedicated_host_tests.py` & `softlayer-6.2.0/tests/managers/dedicated_host_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/managers/dns_tests.py` & `softlayer-6.2.0/tests/managers/dns_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/managers/email_tests.py` & `softlayer-6.2.0/tests/managers/email_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/managers/event_log_tests.py` & `softlayer-6.2.0/tests/managers/event_log_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/managers/file_tests.py` & `softlayer-6.2.0/tests/managers/file_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/managers/firewall_tests.py` & `softlayer-6.2.0/tests/managers/firewall_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/managers/hardware_tests.py` & `softlayer-6.2.0/tests/managers/hardware_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -271,18 +271,15 @@
                     "id": 503,
                     "locations": [
                         {
                             "id": 449610,
                             "longName": "Montreal 1",
                             "name": "mon01",
                             "regions": [
-                                {
-                                    "description": "MON01 - Montreal",
-                                    "keyname": "MONTREAL",
-                                }
+                                {"description": "MON01 - Montreal",  "keyname": "MONTREAL"}
                             ]
                         }
                     ]
                 }
             }
         ]
 
@@ -299,16 +296,15 @@
     def test_generate_create_dict_no_regions(self):
         packages = self.set_mock('SoftLayer_Product_Package', 'getAllObjects')
         packages_copy = copy.deepcopy(
             fixtures.SoftLayer_Product_Package.getAllObjects)
         packages_copy[0]['regions'] = []
         packages.return_value = packages_copy
 
-        ex = self.assertRaises(SoftLayer.SoftLayerError,
-                               self.hardware._generate_create_dict,
+        ex = self.assertRaises(SoftLayer.SoftLayerError, self.hardware._generate_create_dict,
                                **MINIMAL_TEST_CREATE_ARGS)
         self.assertIn("Could not find valid location for: 'wdc01'", str(ex))
 
     def test_generate_create_dict(self):
         args = {
             'size': 'S1270_8GB_2X1TBSATA_NORAID',
             'hostname': 'unicorn',
@@ -368,24 +364,16 @@
             'private_router': 1234
         }
 
         extras = {
             'hardware': [{
                 'domain': 'giggles.woo',
                 'hostname': 'unicorn',
-                'primaryNetworkComponent': {
-                    "router": {
-                        "id": 1111
-                    }
-                },
-                'primaryBackendNetworkComponent': {
-                    "router": {
-                        "id": 1234
-                    }
-                }
+                'primaryNetworkComponent': {"router": {"id": 1111}},
+                'primaryBackendNetworkComponent': {"router": {"id": 1234}}
             }]
         }
 
         data = self.hardware._generate_create_dict(**args)
         self.assertEqual(extras, data['extras'])
 
     def test_generate_create_dict_network_key(self):
@@ -425,28 +413,26 @@
         result = self.hardware.place_order(test=1, verify=1)
         self.assertEqual(1, result['test'])
         create_dict.assert_called_once_with(test=1, verify=1)
         place_order.assert_called_once_with(test=1, verify=1)
 
     def test_cancel_hardware_without_reason(self):
         mock = self.set_mock('SoftLayer_Hardware_Server', 'getObject')
-        mock.return_value = {'id': 987, 'billingItem': {'id': 1234},
-                             'openCancellationTicket': {'id': 1234}}
+        mock.return_value = {'id': 987, 'billingItem': {'id': 1234}, 'openCancellationTicket': {'id': 1234}}
 
         result = self.hardware.cancel_hardware(987)
 
         self.assertEqual(result, True)
         reasons = self.hardware.get_cancellation_reasons()
         args = (False, False, reasons['unneeded'], '')
         self.assert_called_with('SoftLayer_Billing_Item', 'cancelItem', identifier=1234, args=args)
 
     def test_cancel_hardware_with_reason_and_comment(self):
         mock = self.set_mock('SoftLayer_Hardware_Server', 'getObject')
-        mock.return_value = {'id': 987, 'billingItem': {'id': 1234},
-                             'openCancellationTicket': {'id': 1234}}
+        mock.return_value = {'id': 987, 'billingItem': {'id': 1234}, 'openCancellationTicket': {'id': 1234}}
 
         result = self.hardware.cancel_hardware(6327, reason='sales', comment='Test Comment')
 
         self.assertEqual(result, True)
         reasons = self.hardware.get_cancellation_reasons()
         args = (False, False, reasons['sales'], 'Test Comment')
         self.assert_called_with('SoftLayer_Billing_Item', 'cancelItem', identifier=1234, args=args)
@@ -461,26 +447,22 @@
         self.assert_called_with('SoftLayer_Billing_Item', 'cancelItem',
                                 identifier=6327, args=(False, False, 'No longer needed', ''))
 
     def test_cancel_hardware_no_billing_item(self):
         mock = self.set_mock('SoftLayer_Hardware_Server', 'getObject')
         mock.return_value = {'id': 987, 'openCancellationTicket': {'id': 1234}}
 
-        ex = self.assertRaises(SoftLayer.SoftLayerError,
-                               self.hardware.cancel_hardware,
-                               6327)
+        ex = self.assertRaises(SoftLayer.SoftLayerError, self.hardware.cancel_hardware, 6327)
         self.assertEqual("Ticket #1234 already exists for this server", str(ex))
 
     def test_cancel_hardwareno_billing_item_or_ticket(self):
         mock = self.set_mock('SoftLayer_Hardware_Server', 'getObject')
         mock.return_value = {'id': 987}
 
-        ex = self.assertRaises(SoftLayer.SoftLayerError,
-                               self.hardware.cancel_hardware,
-                               6327)
+        ex = self.assertRaises(SoftLayer.SoftLayerError, self.hardware.cancel_hardware, 6327)
         self.assertEqual("Cannot locate billing for the server. The server may already be cancelled.", str(ex))
 
     def test_cancel_hardware_monthly_now(self):
         mock = self.set_mock('SoftLayer_Hardware_Server', 'getObject')
         mock.return_value = {'id': 987, 'billingItem': {'id': 1234},
                              'openCancellationTicket': {'id': 4567},
                              'hourlyBillingFlag': False}
@@ -509,119 +491,94 @@
         self.assert_called_with('SoftLayer_Billing_Item', 'cancelItem',
                                 identifier=6327, args=(False, False, 'No longer needed', ''))
 
     def test_cancel_running_transaction(self):
         mock = self.set_mock('SoftLayer_Hardware_Server', 'getObject')
         mock.return_value = {'id': 987, 'billingItem': {'id': 6327},
                              'activeTransaction': {'id': 4567}}
-        self.assertRaises(SoftLayer.SoftLayerError,
-                          self.hardware.cancel_hardware,
-                          12345)
+        self.assertRaises(SoftLayer.SoftLayerError, self.hardware.cancel_hardware, 12345)
 
     def test_change_port_speed_public(self):
         self.hardware.change_port_speed(2, True, 100, 'degraded')
 
-        self.assert_called_with('SoftLayer_Hardware_Server',
-                                'setPublicNetworkInterfaceSpeed',
-                                identifier=2,
-                                args=([100, 'degraded'],))
+        self.assert_called_with('SoftLayer_Hardware_Server', 'setPublicNetworkInterfaceSpeed',
+                                identifier=2, args=([100, 'degraded'],))
 
     def test_change_port_speed_private(self):
         self.hardware.change_port_speed(2, False, 10, 'redundant')
 
-        self.assert_called_with('SoftLayer_Hardware_Server',
-                                'setPrivateNetworkInterfaceSpeed',
-                                identifier=2,
-                                args=([10, 'redundant'],))
+        self.assert_called_with('SoftLayer_Hardware_Server', 'setPrivateNetworkInterfaceSpeed',
+                                identifier=2, args=([10, 'redundant'],))
 
     def test_edit_meta(self):
         # Test editing user data
         self.hardware.edit(100, userdata='my data')
 
-        self.assert_called_with('SoftLayer_Hardware_Server',
-                                'setUserMetadata',
-                                args=(['my data'],),
-                                identifier=100)
+        self.assert_called_with('SoftLayer_Hardware_Server', 'setUserMetadata', args=(['my data'],), identifier=100)
 
     def test_edit_blank(self):
         # Now test a blank edit
         self.assertTrue(self.hardware.edit, 100)
         self.assertEqual(self.calls(), [])
 
     def test_edit(self):
         # Finally, test a full edit
-        self.hardware.edit(100,
-                           hostname='new-host',
-                           domain='new.sftlyr.ws',
-                           notes='random notes')
+        self.hardware.edit(100, hostname='new-host', domain='new.sftlyr.ws', notes='random notes')
 
-        self.assert_called_with('SoftLayer_Hardware_Server',
-                                'editObject',
+        self.assert_called_with('SoftLayer_Hardware_Server', 'editObject',
                                 args=({
                                           'hostname': 'new-host',
                                           'domain': 'new.sftlyr.ws',
                                           'notes': 'random notes',
                                       },),
                                 identifier=100)
 
     def test_rescue(self):
         result = self.hardware.rescue(1234)
 
         self.assertEqual(result, True)
-        self.assert_called_with('SoftLayer_Hardware_Server',
-                                'bootToRescueLayer',
-                                identifier=1234)
+        self.assert_called_with('SoftLayer_Hardware_Server', 'bootToRescueLayer', identifier=1234)
 
     def test_update_firmware(self):
         result = self.hardware.update_firmware(100)
 
         self.assertEqual(result, True)
-        self.assert_called_with('SoftLayer_Hardware_Server',
-                                'createFirmwareUpdateTransaction',
-                                identifier=100, args=(1, 1, 1, 1))
+        self.assert_called_with('SoftLayer_Hardware_Server', 'createFirmwareUpdateTransaction',
+                                identifier=100, args=(1, 1, 1, 1, 1))
 
     def test_update_firmware_selective(self):
-        result = self.hardware.update_firmware(100,
-                                               ipmi=False,
-                                               hard_drive=False)
+        result = self.hardware.update_firmware(100, ipmi=False, hard_drive=False)
 
         self.assertEqual(result, True)
-        self.assert_called_with('SoftLayer_Hardware_Server',
-                                'createFirmwareUpdateTransaction',
-                                identifier=100, args=(0, 1, 1, 0))
+        self.assert_called_with('SoftLayer_Hardware_Server', 'createFirmwareUpdateTransaction',
+                                identifier=100, args=(0, 1, 1, 0, 1))
 
     def test_reflash_firmware(self):
         result = self.hardware.reflash_firmware(100)
 
         self.assertEqual(result, True)
-        self.assert_called_with('SoftLayer_Hardware_Server',
-                                'createFirmwareReflashTransaction',
+        self.assert_called_with('SoftLayer_Hardware_Server', 'createFirmwareReflashTransaction',
                                 identifier=100, args=(1, 1, 1))
 
     def test_reflash_firmware_selective(self):
-        result = self.hardware.reflash_firmware(100,
-                                                raid_controller=False,
-                                                bios=False)
+        result = self.hardware.reflash_firmware(100, raid_controller=False, bios=False)
 
         self.assertEqual(result, True)
-        self.assert_called_with('SoftLayer_Hardware_Server',
-                                'createFirmwareReflashTransaction',
+        self.assert_called_with('SoftLayer_Hardware_Server', 'createFirmwareReflashTransaction',
                                 identifier=100, args=(1, 0, 0))
 
     def test_get_tracking_id(self):
         result = self.hardware.get_tracking_id(1234)
         self.assert_called_with('SoftLayer_Hardware_Server', 'getMetricTrackingObjectId')
         self.assertEqual(result, 1000)
 
     def test_get_bandwidth_data(self):
         result = self.hardware.get_bandwidth_data(1234, '2019-01-01', '2019-02-01', 'public', 1000)
-        self.assert_called_with('SoftLayer_Metric_Tracking_Object',
-                                'getBandwidthData',
-                                args=('2019-01-01', '2019-02-01', 'public', 1000),
-                                identifier=1000)
+        self.assert_called_with('SoftLayer_Metric_Tracking_Object', 'getBandwidthData',
+                                args=('2019-01-01', '2019-02-01', 'public', 1000), identifier=1000)
         self.assertEqual(result[0]['type'], 'cpu0')
 
     def test_get_bandwidth_allocation(self):
         result = self.hardware.get_bandwidth_allocation(1234)
         self.assert_called_with('SoftLayer_Hardware_Server', 'getBandwidthAllotmentDetail', identifier=1234)
         self.assert_called_with('SoftLayer_Hardware_Server', 'getBillingCycleBandwidthUsage', identifier=1234)
         self.assertEqual(result['allotment']['amount'], '250')
@@ -677,83 +634,63 @@
 
         result = self.hardware.get_storage_details(1234, 'ISCSI')
 
         self.assertEqual([], result)
 
     def test_get_storage_nas_details(self):
         mock = self.set_mock('SoftLayer_Hardware_Server', 'getAttachedNetworkStorages')
-        mock.return_value = [
+        getAttachedNetworkStorages = [
             {
                 "accountId": 11111,
                 "capacityGb": 12000,
                 "id": 3777111,
                 "nasType": "NAS",
                 "username": "SL02SEL32222-9",
             }
         ]
 
+        mock.return_value = getAttachedNetworkStorages
         result = self.hardware.get_storage_details(1234, 'NAS')
-
-        self.assertEqual([{
-            "accountId": 11111,
-            "capacityGb": 12000,
-            "id": 3777111,
-            "nasType": "NAS",
-            "username": "SL02SEL32222-9",
-        }], result)
+        self.assertEqual(getAttachedNetworkStorages, result)
 
     def test_get_storage_nas_empty_details(self):
         mock = self.set_mock('SoftLayer_Hardware_Server', 'getAttachedNetworkStorages')
         mock.return_value = []
 
         result = self.hardware.get_storage_details(1234, 'NAS')
 
         self.assertEqual([], result)
 
     def test_get_storage_credentials(self):
         mock = self.set_mock('SoftLayer_Hardware_Server', 'getAllowedHost')
-        mock.return_value = {
+        getAllowedHost = {
             "accountId": 11111,
             "id": 33333,
             "name": "iqn.2020-03.com.ibm:sl02su11111-v62941551",
             "resourceTableName": "HARDWARE",
             "credential": {
                 "accountId": "11111",
                 "id": 44444,
                 "password": "SjFDCpHrjskfj",
                 "username": "SL02SU11111-V62941551"
             }
         }
-
+        mock.return_value = getAllowedHost
         result = self.hardware.get_storage_credentials(1234)
-
-        self.assertEqual({
-            "accountId": 11111,
-            "id": 33333,
-            "name": "iqn.2020-03.com.ibm:sl02su11111-v62941551",
-            "resourceTableName": "HARDWARE",
-            "credential": {
-                "accountId": "11111",
-                "id": 44444,
-                "password": "SjFDCpHrjskfj",
-                "username": "SL02SU11111-V62941551"
-            }
-        }, result)
+        self.assertEqual(getAllowedHost, result)
 
     def test_get_none_storage_credentials(self):
         mock = self.set_mock('SoftLayer_Hardware_Server', 'getAllowedHost')
         mock.return_value = None
-
         result = self.hardware.get_storage_credentials(1234)
-
         self.assertEqual(None, result)
 
     def test_get_hard_drives(self):
         mock = self.set_mock('SoftLayer_Hardware_Server', 'getHardDrives')
-        mock.return_value = [
+        hd_return = [
             {
                 "id": 11111,
                 "serialNumber": "z1w4sdf",
                 "serviceProviderId": 1,
                 "hardwareComponentModel": {
                     "capacity": "1000",
                     "description": "SATAIII:2000:8300:Constellation",
@@ -769,41 +706,17 @@
                             "type": "Hard Drive",
                             "typeParentId": 5
                         }
                     }
                 }
             }
         ]
-
+        mock.return_value = hd_return
         result = self.hardware.get_hard_drives(1234)
-
-        self.assertEqual([
-            {
-                "id": 11111,
-                "serialNumber": "z1w4sdf",
-                "serviceProviderId": 1,
-                "hardwareComponentModel": {
-                    "capacity": "1000",
-                    "description": "SATAIII:2000:8300:Constellation",
-                    "id": 111,
-                    "manufacturer": "Seagate",
-                    "name": "Constellation ES",
-                    "hardwareGenericComponentModel": {
-                        "capacity": "1000",
-                        "units": "GB",
-                        "hardwareComponentType": {
-                            "id": 1,
-                            "keyName": "HARD_DRIVE",
-                            "type": "Hard Drive",
-                            "typeParentId": 5
-                        }
-                    }
-                }
-            }
-        ], result)
+        self.assertEqual(hd_return, result)
 
     def test_get_hard_drive_empty(self):
         mock = self.set_mock('SoftLayer_Hardware_Server', 'getHardDrives')
         mock.return_value = []
 
         result = self.hardware.get_hard_drives(1234)
 
@@ -813,17 +726,15 @@
         options = self.hardware.authorize_storage(1234, "SL01SEL301234-11")
 
         self.assertEqual(True, options)
 
     def test_authorize_storage_empty(self):
         mock = self.set_mock('SoftLayer_Account', 'getNetworkStorage')
         mock.return_value = []
-        self.assertRaises(SoftLayer.exceptions.SoftLayerError,
-                          self.hardware.authorize_storage,
-                          1234, "#")
+        self.assertRaises(SoftLayer.exceptions.SoftLayerError, self.hardware.authorize_storage, 1234, "#")
 
     def test_get_price_id_memory_capacity(self):
         upgrade_prices = [
             {'categories': [{'categoryCode': 'ram'}], 'item': {'capacity': 1}, 'id': 99}
         ]
         result = self.hardware._get_prices_for_upgrade_option(upgrade_prices, 'memory', 1)
         self.assertEqual(99, result)
@@ -941,22 +852,64 @@
             "notes": 'notes',
             "password": 'password',
             "softwareId": 'sw_id',
             "username": 'username',
             "software": {
                 "hardwareId": 123456,
                 "softwareLicense": {
-                    "softwareDescription": {
-                        "name": 'system'
-                    }
+                    "softwareDescription": {"name": 'system'}
                 }
-            }}
+            }
+        }
         self.hardware.create_credential(template)
         self.assert_called_with('SoftLayer_Software_Component_Password', 'createObject')
 
+    def test_get_hardware_fast(self):
+        result = self.hardware.get_hardware_fast(1234)
+        self.assertIn('networkComponents', result)
+        self.assertIn('activeComponents', result)
+        self.assertIn('activeTransaction', result)
+        self.assertIn('operatingSystem', result)
+        self.assertIn('softwareComponents', result)
+        self.assertIn('billingItem', result)
+        self.assertIn('networkVlans', result)
+        self.assertIn('remoteManagementAccounts', result)
+        self.assertIn('tagReferences', result)
+        self.assert_called_with('SoftLayer_Hardware_Server', 'getNetworkComponents')
+        self.assert_called_with('SoftLayer_Hardware_Server', 'getActiveComponents')
+        self.assert_called_with('SoftLayer_Hardware_Server', 'getOperatingSystem')
+        self.assert_called_with('SoftLayer_Hardware_Server', 'getSoftwareComponents')
+        self.assert_called_with('SoftLayer_Hardware_Server', 'getBillingItem')
+        self.assert_called_with('SoftLayer_Hardware_Server', 'getTagReferences')
+        self.assert_called_with('SoftLayer_Hardware_Server', 'getNetworkVlans')
+        self.assert_called_with('SoftLayer_Hardware_Server', 'getRemoteManagementAccounts')
+
+    def test_trunk_vlan(self):
+        vlans = [{'id': 9999}]
+        vlan_id = 1234
+        self.hardware.trunk_vlan(vlan_id, vlans)
+        self.assert_called_with('SoftLayer_Network_Component', 'addNetworkVlanTrunks',
+                                identifier=vlan_id, args=(vlans,))
+
+    def test_remove_vlan(self):
+        vlans = [{'id': 9999}]
+        vlan_id = 1234
+        self.hardware.remove_vlan(vlan_id, vlans)
+        self.assert_called_with('SoftLayer_Network_Component', 'removeNetworkVlanTrunks',
+                                identifier=vlan_id, args=(vlans,))
+
+    def test_clear_vlan(self):
+        hardware_mock = self.set_mock('SoftLayer_Hardware_Server', 'getObject')
+        hardware_mock.return_value = fixtures.SoftLayer_Hardware_Server.getObjectVlanClear
+        server_id = 1234
+        self.hardware.clear_vlan(server_id)
+        self.assert_called_with('SoftLayer_Hardware_Server', 'getObject', identifier=server_id)
+        self.assert_called_with('SoftLayer_Network_Component', 'clearNetworkVlanTrunks', identifier=998877)
+        self.assert_called_with('SoftLayer_Network_Component', 'clearNetworkVlanTrunks', identifier=123456)
+
 
 class HardwareHelperTests(testing.TestCase):
 
     def set_up(self):
         self.items = [
             {
                 "itemCategory": {"categoryCode": "port_speed"},
@@ -1048,15 +1001,7 @@
         self.assertTrue(managers.hardware._is_bonded(item_lacp))
 
     def test_is_private(self):
         item_private = {'attributes': [{'attributeTypeKeyName': 'IS_PRIVATE_NETWORK_ONLY'}]}
         item_public = {'attributes': [{'attributeTypeKeyName': 'NOT_PRIVATE_NETWORK_ONLY'}]}
         self.assertTrue(managers.hardware._is_private_port_speed_item(item_private))
         self.assertFalse(managers.hardware._is_private_port_speed_item(item_public))
-
-    @mock.patch('SoftLayer.CLI.formatting.confirm')
-    def test_hardware_cancel_no_force(self, confirm_mock):
-        confirm_mock.return_value = False
-        result = self.run_command(['hardware', 'cancel', '102'])
-
-        self.assertEqual(2, result.exit_code)
-        self.assertEqual('Aborted', result.exception.message)
```

### Comparing `SoftLayer-6.1.9/tests/managers/image_tests.py` & `softlayer-6.2.0/tests/managers/image_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/managers/ipsec_tests.py` & `softlayer-6.2.0/tests/managers/ipsec_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/managers/loadbal_tests.py` & `softlayer-6.2.0/tests/managers/loadbal_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/managers/metadata_tests.py` & `softlayer-6.2.0/tests/managers/metadata_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/managers/network_tests.py` & `softlayer-6.2.0/tests/managers/network_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/managers/object_storage_tests.py` & `softlayer-6.2.0/tests/managers/object_storage_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/managers/ordering_tests.py` & `softlayer-6.2.0/tests/managers/ordering_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/managers/search_tests.py` & `softlayer-6.2.0/tests/managers/search_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,8 +39,8 @@
         self.assert_called_with('SoftLayer_Search', 'advancedSearch',
                                 args=(f"{expected} domain: *thisDomain*",))
         self.search.search_instances(search_string, datacenter="dal13")
         self.assert_called_with('SoftLayer_Search', 'advancedSearch',
                                 args=(f"{expected} datacenter.longName: *dal13*",))
         self.search.search_instances(search_string, tags=["thisTag"])
         self.assert_called_with('SoftLayer_Search', 'advancedSearch',
-                                args=(f"{expected} internalTagReferences.tag.name: thisTag",))
+                                args=(f"{expected} tagReferences.tag.name: \"thisTag\"",))
```

### Comparing `SoftLayer-6.1.9/tests/managers/sshkey_tests.py` & `softlayer-6.2.0/tests/managers/sshkey_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/managers/ssl_tests.py` & `softlayer-6.2.0/tests/managers/ssl_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/managers/storage_generic_tests.py` & `softlayer-6.2.0/tests/managers/storage_generic_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/managers/storage_utils_tests.py` & `softlayer-6.2.0/tests/managers/storage_utils_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/managers/tag_tests.py` & `softlayer-6.2.0/tests/managers/tag_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/managers/ticket_tests.py` & `softlayer-6.2.0/tests/managers/ticket_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/managers/user_tests.py` & `softlayer-6.2.0/tests/managers/user_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/managers/vs/vs_capacity_tests.py` & `softlayer-6.2.0/tests/managers/vs/vs_capacity_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/managers/vs/vs_order_tests.py` & `softlayer-6.2.0/tests/managers/vs/vs_order_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/managers/vs/vs_placement_tests.py` & `softlayer-6.2.0/tests/managers/vs/vs_placement_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/managers/vs/vs_waiting_for_ready_tests.py` & `softlayer-6.2.0/tests/managers/vs/vs_waiting_for_ready_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/transports/debug_tests.py` & `softlayer-6.2.0/tests/transports/debug_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/transports/rest_tests.py` & `softlayer-6.2.0/tests/transports/rest_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/transports/transport_tests.py` & `softlayer-6.2.0/tests/transports/transport_tests.py`

 * *Files identical despite different names*

### Comparing `SoftLayer-6.1.9/tests/transports/xmlrpc_tests.py` & `softlayer-6.2.0/tests/transports/xmlrpc_tests.py`

 * *Files identical despite different names*

