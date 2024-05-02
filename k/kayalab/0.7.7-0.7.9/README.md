# Comparing `tmp/kayalab-0.7.7.tar.gz` & `tmp/kayalab-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kayalab-0.7.7.tar", max compression
+gzip compressed data, was "kayalab-0.7.9.tar", max compression
```

## Comparing `kayalab-0.7.7.tar` & `kayalab-0.7.9.tar`

### file list

```diff
@@ -1,101 +1,103 @@
--rw-r--r--   0        0        0    35148 2024-02-06 20:43:13.799294 kayalab-0.7.7/LICENSE
--rw-r--r--   0        0        0     3989 2024-02-13 01:29:35.378839 kayalab-0.7.7/README.md
--rw-r--r--   0        0        0       47 2024-02-26 17:23:20.484455 kayalab-0.7.7/ezinfra/__init__.py
--rw-r--r--   0        0        0     1056 2024-02-11 21:18:15.397470 kayalab-0.7.7/ezinfra/cloudinit.py
--rw-r--r--   0        0        0    16003 2024-02-26 17:33:02.998195 kayalab-0.7.7/ezinfra/kvm.py
--rw-r--r--   0        0        0      699 2024-02-07 22:53:09.428873 kayalab-0.7.7/ezinfra/proxy.py
--rw-r--r--   0        0        0     8237 2024-02-26 17:33:01.869736 kayalab-0.7.7/ezinfra/pve.py
--rw-r--r--   0        0        0     1462 2024-02-26 17:33:00.029845 kayalab-0.7.7/ezinfra/queue.py
--rw-r--r--   0        0        0     3290 2024-02-10 23:44:30.466175 kayalab-0.7.7/ezinfra/remote.py
--rw-r--r--   0        0        0      900 2024-02-15 13:03:56.578087 kayalab-0.7.7/ezinfra/repo.py
--rw-r--r--   0        0        0     2675 2024-02-08 00:53:15.651687 kayalab-0.7.7/ezinfra/sshkeys.py
--rw-r--r--   0        0        0     6591 2024-02-26 17:32:58.904216 kayalab-0.7.7/ezinfra/vms.py
--rw-r--r--   0        0        0    28000 2024-02-16 00:10:17.168965 kayalab-0.7.7/ezinfra/vmw.py
--rw-r--r--   0        0        0     4498 2024-02-06 20:42:59.534097 kayalab-0.7.7/ezinfra/vmw_pchelper.py
--rw-r--r--   0        0        0     1756 2024-02-07 18:18:31.010715 kayalab-0.7.7/ezlab/USAGE.md
--rw-r--r--   0        0        0       45 2024-02-26 18:19:45.231697 kayalab-0.7.7/ezlab/__init__.py
--rw-r--r--   0        0        0       85 2024-02-15 22:46:20.743011 kayalab-0.7.7/ezlab/__main__.py
--rw-r--r--   0        0        0    13966 2024-02-26 17:33:09.450593 kayalab-0.7.7/ezlab/ezmeral/ezdf.py
--rw-r--r--   0        0        0    12116 2024-02-26 17:33:07.860111 kayalab-0.7.7/ezlab/ezmeral/ezua.py
--rw-r--r--   0        0        0     5672 2024-02-24 23:24:04.267183 kayalab-0.7.7/ezlab/main.py
--rw-r--r--   0        0        0     7242 2024-02-26 17:33:08.576075 kayalab-0.7.7/ezlab/pages/df.py
--rw-r--r--   0        0        0     5681 2024-02-21 01:56:39.793453 kayalab-0.7.7/ezlab/pages/ezmeral.py
--rw-r--r--   0        0        0     6033 2024-02-15 21:16:23.540593 kayalab-0.7.7/ezlab/pages/settings.py
--rw-r--r--   0        0        0     1911 2024-02-26 17:33:07.152423 kayalab-0.7.7/ezlab/pages/sshkeys.py
--rw-r--r--   0        0        0     4780 2024-02-26 17:33:06.411633 kayalab-0.7.7/ezlab/pages/targets.py
--rw-r--r--   0        0        0       62 2024-02-15 02:29:15.589145 kayalab-0.7.7/ezlab/pages/ua.py
--rw-r--r--   0        0        0     8257 2024-02-26 17:33:05.694127 kayalab-0.7.7/ezlab/pages/vms.py
--rw-r--r--   0        0        0     4641 2024-02-20 21:54:28.126778 kayalab-0.7.7/ezlab/parameters.py
--rw-r--r--   0        0        0     1344 2024-02-06 21:17:14.449592 kayalab-0.7.7/ezlab/requirements.txt
--rw-r--r--   0        0        0     2162 2024-02-26 17:58:38.998953 kayalab-0.7.7/ezlab/utils.py
--rw-r--r--   0        0        0     6334 2024-02-16 00:09:51.099648 kayalab-0.7.7/ezlabctl/USAGE.md
--rw-r--r--   0        0        0       48 2024-02-26 18:19:45.231766 kayalab-0.7.7/ezlabctl/__init__.py
--rw-r--r--   0        0        0       72 2024-02-06 22:31:38.092805 kayalab-0.7.7/ezlabctl/__main__.py
--rw-r--r--   0        0        0    18667 2024-02-16 12:20:08.300021 kayalab-0.7.7/ezlabctl/common.py
--rw-r--r--   0        0        0     4336 2024-02-16 00:03:13.385050 kayalab-0.7.7/ezlabctl/config.py
--rw-r--r--   0        0        0     1644 2024-01-08 02:00:25.550726 kayalab-0.7.7/ezlabctl/connect.py
--rw-r--r--   0        0        0     3980 2024-01-12 23:42:44.403968 kayalab-0.7.7/ezlabctl/create.py
--rw-r--r--   0        0        0     2174 2024-01-08 02:01:45.764185 kayalab-0.7.7/ezlabctl/delete.py
--rw-r--r--   0        0        0     9180 2024-02-26 17:24:56.834075 kayalab-0.7.7/ezlabctl/ezdf.py
--rw-r--r--   0        0        0    15646 2024-02-16 00:50:25.063477 kayalab-0.7.7/ezlabctl/ezua.py
--rw-r--r--   0        0        0     4023 2024-02-16 11:59:22.183975 kayalab-0.7.7/ezlabctl/main.py
--rw-r--r--   0        0        0     4557 2024-02-16 00:54:32.973947 kayalab-0.7.7/ezlabctl/parameters.py
--rw-r--r--   0        0        0    17078 2024-02-16 00:55:44.673816 kayalab-0.7.7/ezlabctl/pve.py
--rw-r--r--   0        0        0      726 2024-02-06 21:12:35.592066 kayalab-0.7.7/ezlabctl/requirements.txt
--rw-r--r--   0        0        0    26875 2024-02-16 00:35:29.434009 kayalab-0.7.7/ezlabctl/vmw.py
--rw-r--r--   0        0        0       46 2024-02-26 18:19:45.231819 kayalab-0.7.7/ezshow/__init__.py
--rw-r--r--   0        0        0       86 2024-02-21 17:02:55.317870 kayalab-0.7.7/ezshow/__main__.py
--rw-r--r--   0        0        0    14509 2024-02-26 17:33:04.812959 kayalab-0.7.7/ezshow/apprunner.py
--rw-r--r--   0        0        0     2193 2024-02-20 16:38:06.117981 kayalab-0.7.7/ezshow/confluent.kafka.py
--rw-r--r--   0        0        0    97559 2024-02-18 12:03:14.045634 kayalab-0.7.7/ezshow/demos/banking/banking.jpg
--rw-r--r--   0        0        0   183254 2024-02-16 16:56:01.814735 kayalab-0.7.7/ezshow/demos/core-to-edge/core-edge.png
--rw-r--r--   0        0        0    86887 2024-02-17 23:06:32.776215 kayalab-0.7.7/ezshow/demos/telecom/data/basestation.csv
--rw-r--r--   0        0        0      300 2024-02-17 23:06:32.776900 kayalab-0.7.7/ezshow/demos/telecom/data/call.avsc
--rw-r--r--   0        0        0 43705638 2024-02-17 23:06:32.821190 kayalab-0.7.7/ezshow/demos/telecom/data/calls.csv
--rw-r--r--   0        0        0  2572296 2024-02-17 23:06:32.825652 kayalab-0.7.7/ezshow/demos/telecom/data/subscribers.csv
--rw-r--r--   0        0        0     1841 2024-02-17 23:06:39.197447 kayalab-0.7.7/ezshow/demos/telecom/myApp/app.js
--rwxr-xr-x   0        0        0     1638 2024-02-17 23:06:39.198180 kayalab-0.7.7/ezshow/demos/telecom/myApp/bin/www
--rw-r--r--   0        0        0      215 2024-02-17 23:06:39.198641 kayalab-0.7.7/ezshow/demos/telecom/myApp/config.js
--rw-r--r--   0        0        0   164393 2024-02-17 23:06:39.199133 kayalab-0.7.7/ezshow/demos/telecom/myApp/package-lock.json
--rw-r--r--   0        0        0      562 2024-02-17 23:06:39.209125 kayalab-0.7.7/ezshow/demos/telecom/myApp/package.json
--rw-r--r--   0        0        0    26975 2024-02-17 23:06:39.210204 kayalab-0.7.7/ezshow/demos/telecom/myApp/public/index.html
--rw-r--r--   0        0        0      111 2024-02-17 23:06:39.211620 kayalab-0.7.7/ezshow/demos/telecom/myApp/public/stylesheets/style.css
--rw-r--r--   0        0        0     2986 2024-02-17 23:06:39.212689 kayalab-0.7.7/ezshow/demos/telecom/myApp/routes/basedb.js
--rw-r--r--   0        0        0     1319 2024-02-17 23:06:39.213101 kayalab-0.7.7/ezshow/demos/telecom/myApp/routes/convertTiff2Png.js
--rw-r--r--   0        0        0      879 2024-02-17 23:06:39.213496 kayalab-0.7.7/ezshow/demos/telecom/myApp/routes/graphdb.js
--rw-r--r--   0        0        0     2820 2024-02-17 23:06:39.213885 kayalab-0.7.7/ezshow/demos/telecom/myApp/routes/graphdb_dyn.js
--rw-r--r--   0        0        0     2120 2024-02-17 23:06:39.214353 kayalab-0.7.7/ezshow/demos/telecom/myApp/routes/graphdb_stat.js
--rw-r--r--   0        0        0      205 2024-02-17 23:06:39.214665 kayalab-0.7.7/ezshow/demos/telecom/myApp/routes/index.js
--rw-r--r--   0        0        0     1034 2024-02-17 23:06:39.214959 kayalab-0.7.7/ezshow/demos/telecom/myApp/routes/maprdb.js
--rw-r--r--   0        0        0     1056 2024-02-17 23:06:39.215555 kayalab-0.7.7/ezshow/demos/telecom/myApp/routes/marker.js
--rw-r--r--   0        0        0      605 2024-02-17 23:06:39.215861 kayalab-0.7.7/ezshow/demos/telecom/myApp/routes/model.js
--rw-r--r--   0        0        0      844 2024-02-17 23:06:39.216432 kayalab-0.7.7/ezshow/demos/telecom/myApp/routes/opentsdb.js
--rw-r--r--   0        0        0     1062 2024-02-17 23:06:39.216932 kayalab-0.7.7/ezshow/demos/telecom/myApp/routes/process.js
--rw-r--r--   0        0        0      696 2024-02-17 23:06:39.217850 kayalab-0.7.7/ezshow/demos/telecom/myApp/routes/upload.js
--rw-r--r--   0        0        0      203 2024-02-17 23:06:39.218313 kayalab-0.7.7/ezshow/demos/telecom/myApp/routes/users.js
--rw-r--r--   0        0        0      512 2024-02-17 23:06:39.218858 kayalab-0.7.7/ezshow/demos/telecom/myApp/tsdb.json
--rw-r--r--   0        0        0       84 2024-02-17 23:06:39.219880 kayalab-0.7.7/ezshow/demos/telecom/myApp/views/error.pug
--rw-r--r--   0        0        0       66 2024-02-17 23:06:39.220316 kayalab-0.7.7/ezshow/demos/telecom/myApp/views/index.pug
--rw-r--r--   0        0        0      125 2024-02-17 23:06:39.220657 kayalab-0.7.7/ezshow/demos/telecom/myApp/views/layout.pug
--rw-r--r--   0        0        0     1277 2024-02-17 23:06:46.384244 kayalab-0.7.7/ezshow/demos/telecom/py/baseStationDB.py
--rw-r--r--   0        0        0      910 2024-02-17 23:06:46.384651 kayalab-0.7.7/ezshow/demos/telecom/py/baseStationDelta.py
--rw-r--r--   0        0        0      647 2024-02-17 23:06:46.385029 kayalab-0.7.7/ezshow/demos/telecom/py/consumer.py
--rw-r--r--   0        0        0      998 2024-02-17 23:06:46.390937 kayalab-0.7.7/ezshow/demos/telecom/py/consumerAvro.py
--rw-r--r--   0        0        0     1297 2024-02-17 23:06:46.391852 kayalab-0.7.7/ezshow/demos/telecom/py/consumerCallDB.py
--rw-r--r--   0        0        0     1393 2024-02-17 23:06:46.392726 kayalab-0.7.7/ezshow/demos/telecom/py/consumerCallDelta.py
--rw-r--r--   0        0        0     1253 2024-02-17 23:06:46.393963 kayalab-0.7.7/ezshow/demos/telecom/py/ingest.py
--rw-r--r--   0        0        0     1209 2024-02-17 23:06:46.394412 kayalab-0.7.7/ezshow/demos/telecom/py/joinCallBaseDelta.py
--rw-r--r--   0        0        0     1237 2024-02-17 23:06:46.396284 kayalab-0.7.7/ezshow/demos/telecom/py/joinCallSubcriberDelta.py
--rw-r--r--   0        0        0     1398 2024-02-17 23:06:46.396793 kayalab-0.7.7/ezshow/demos/telecom/py/opentsdb.py
--rw-r--r--   0        0        0     1499 2024-02-17 23:06:46.397469 kayalab-0.7.7/ezshow/demos/telecom/py/producer.py
--rwxr-xr-x   0        0        0      774 2024-02-17 23:06:46.397867 kayalab-0.7.7/ezshow/demos/telecom/py/readCSV.py
--rw-r--r--   0        0        0      905 2024-02-17 23:06:46.398613 kayalab-0.7.7/ezshow/demos/telecom/py/subscriberDelta.py
--rw-r--r--   0        0        0   900770 2024-02-16 16:56:01.822080 kayalab-0.7.7/ezshow/demos/telecom/telecom.png
--rw-r--r--   0        0        0     9533 2024-02-26 15:09:52.338964 kayalab-0.7.7/ezshow/demos.json
--rw-r--r--   0        0        0    20002 2024-02-26 17:33:13.615577 kayalab-0.7.7/ezshow/main.py
--rw-r--r--   0        0        0     1754 2024-02-20 16:38:16.759221 kayalab-0.7.7/ezshow/python-kafka.py
--rw-r--r--   0        0        0     7378 2024-02-26 18:17:17.559965 kayalab-0.7.7/ezshow/restrunner.py
--rw-r--r--   0        0        0     1260 2024-02-17 16:48:25.243841 kayalab-0.7.7/ezshow/s3runner.py
--rw-r--r--   0        0        0      499 2024-02-26 18:19:37.937043 kayalab-0.7.7/ezshow/shrunner.py
--rw-r--r--   0        0        0     2831 2024-02-26 18:19:47.103049 kayalab-0.7.7/pyproject.toml
--rw-r--r--   0        0        0     8304 1970-01-01 00:00:00.000000 kayalab-0.7.7/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-02-06 20:43:13.799294 kayalab-0.7.9/LICENSE
+-rw-r--r--   0        0        0     3989 2024-02-13 01:29:35.378839 kayalab-0.7.9/README.md
+-rw-r--r--   0        0        0       47 2024-02-26 17:23:20.484455 kayalab-0.7.9/ezinfra/__init__.py
+-rw-r--r--   0        0        0     1056 2024-02-11 21:18:15.397470 kayalab-0.7.9/ezinfra/cloudinit.py
+-rw-r--r--   0        0        0    16003 2024-02-26 17:33:02.998195 kayalab-0.7.9/ezinfra/kvm.py
+-rw-r--r--   0        0        0      699 2024-02-07 22:53:09.428873 kayalab-0.7.9/ezinfra/proxy.py
+-rw-r--r--   0        0        0     8237 2024-02-26 17:33:01.869736 kayalab-0.7.9/ezinfra/pve.py
+-rw-r--r--   0        0        0     1462 2024-02-26 17:33:00.029845 kayalab-0.7.9/ezinfra/queue.py
+-rw-r--r--   0        0        0     3290 2024-02-10 23:44:30.466175 kayalab-0.7.9/ezinfra/remote.py
+-rw-r--r--   0        0        0      900 2024-02-15 13:03:56.578087 kayalab-0.7.9/ezinfra/repo.py
+-rw-r--r--   0        0        0     2675 2024-02-08 00:53:15.651687 kayalab-0.7.9/ezinfra/sshkeys.py
+-rw-r--r--   0        0        0     6591 2024-02-26 17:32:58.904216 kayalab-0.7.9/ezinfra/vms.py
+-rw-r--r--   0        0        0    28000 2024-02-16 00:10:17.168965 kayalab-0.7.9/ezinfra/vmw.py
+-rw-r--r--   0        0        0     4498 2024-02-06 20:42:59.534097 kayalab-0.7.9/ezinfra/vmw_pchelper.py
+-rw-r--r--   0        0        0     1756 2024-02-07 18:18:31.010715 kayalab-0.7.9/ezlab/USAGE.md
+-rw-r--r--   0        0        0       45 2024-02-29 10:45:38.071547 kayalab-0.7.9/ezlab/__init__.py
+-rw-r--r--   0        0        0       85 2024-02-15 22:46:20.743011 kayalab-0.7.9/ezlab/__main__.py
+-rw-r--r--   0        0        0    13966 2024-02-26 17:33:09.450593 kayalab-0.7.9/ezlab/ezmeral/ezdf.py
+-rw-r--r--   0        0        0    12116 2024-02-26 17:33:07.860111 kayalab-0.7.9/ezlab/ezmeral/ezua.py
+-rw-r--r--   0        0        0     5709 2024-02-28 03:05:32.111626 kayalab-0.7.9/ezlab/main.py
+-rw-r--r--   0        0        0     7242 2024-02-26 17:33:08.576075 kayalab-0.7.9/ezlab/pages/df.py
+-rw-r--r--   0        0        0     5681 2024-02-21 01:56:39.793453 kayalab-0.7.9/ezlab/pages/ezmeral.py
+-rw-r--r--   0        0        0     6033 2024-02-15 21:16:23.540593 kayalab-0.7.9/ezlab/pages/settings.py
+-rw-r--r--   0        0        0     1911 2024-02-26 17:33:07.152423 kayalab-0.7.9/ezlab/pages/sshkeys.py
+-rw-r--r--   0        0        0     4780 2024-02-26 17:33:06.411633 kayalab-0.7.9/ezlab/pages/targets.py
+-rw-r--r--   0        0        0       62 2024-02-15 02:29:15.589145 kayalab-0.7.9/ezlab/pages/ua.py
+-rw-r--r--   0        0        0     8257 2024-02-26 17:33:05.694127 kayalab-0.7.9/ezlab/pages/vms.py
+-rw-r--r--   0        0        0     4641 2024-02-20 21:54:28.126778 kayalab-0.7.9/ezlab/parameters.py
+-rw-r--r--   0        0        0     1344 2024-02-06 21:17:14.449592 kayalab-0.7.9/ezlab/requirements.txt
+-rw-r--r--   0        0        0     2228 2024-02-28 03:28:49.968430 kayalab-0.7.9/ezlab/utils.py
+-rw-r--r--   0        0        0     6334 2024-02-16 00:09:51.099648 kayalab-0.7.9/ezlabctl/USAGE.md
+-rw-r--r--   0        0        0       48 2024-02-29 10:45:38.071605 kayalab-0.7.9/ezlabctl/__init__.py
+-rw-r--r--   0        0        0       72 2024-02-06 22:31:38.092805 kayalab-0.7.9/ezlabctl/__main__.py
+-rw-r--r--   0        0        0    18667 2024-02-16 12:20:08.300021 kayalab-0.7.9/ezlabctl/common.py
+-rw-r--r--   0        0        0     4336 2024-02-16 00:03:13.385050 kayalab-0.7.9/ezlabctl/config.py
+-rw-r--r--   0        0        0     1644 2024-01-08 02:00:25.550726 kayalab-0.7.9/ezlabctl/connect.py
+-rw-r--r--   0        0        0     3980 2024-01-12 23:42:44.403968 kayalab-0.7.9/ezlabctl/create.py
+-rw-r--r--   0        0        0     2174 2024-01-08 02:01:45.764185 kayalab-0.7.9/ezlabctl/delete.py
+-rw-r--r--   0        0        0     9180 2024-02-26 17:24:56.834075 kayalab-0.7.9/ezlabctl/ezdf.py
+-rw-r--r--   0        0        0    15646 2024-02-16 00:50:25.063477 kayalab-0.7.9/ezlabctl/ezua.py
+-rw-r--r--   0        0        0     4023 2024-02-16 11:59:22.183975 kayalab-0.7.9/ezlabctl/main.py
+-rw-r--r--   0        0        0     4557 2024-02-16 00:54:32.973947 kayalab-0.7.9/ezlabctl/parameters.py
+-rw-r--r--   0        0        0    17078 2024-02-16 00:55:44.673816 kayalab-0.7.9/ezlabctl/pve.py
+-rw-r--r--   0        0        0      726 2024-02-06 21:12:35.592066 kayalab-0.7.9/ezlabctl/requirements.txt
+-rw-r--r--   0        0        0    26875 2024-02-16 00:35:29.434009 kayalab-0.7.9/ezlabctl/vmw.py
+-rw-r--r--   0        0        0       46 2024-02-29 10:45:38.071658 kayalab-0.7.9/ezshow/__init__.py
+-rw-r--r--   0        0        0       86 2024-02-21 17:02:55.317870 kayalab-0.7.9/ezshow/__main__.py
+-rw-r--r--   0        0        0    16429 2024-02-29 02:49:24.779395 kayalab-0.7.9/ezshow/apprunner.py
+-rw-r--r--   0        0        0     2193 2024-02-20 16:38:06.117981 kayalab-0.7.9/ezshow/confluent.kafka.py
+-rw-r--r--   0        0        0        0 2024-02-28 02:14:58.250082 kayalab-0.7.9/ezshow/demos/__init__.py
+-rw-r--r--   0        0        0    97559 2024-02-18 12:03:14.045634 kayalab-0.7.9/ezshow/demos/banking.jpg
+-rw-r--r--   0        0        0   183254 2024-02-16 16:56:01.814735 kayalab-0.7.9/ezshow/demos/core-edge.png
+-rw-r--r--   0        0        0    10541 2024-02-29 02:53:46.075586 kayalab-0.7.9/ezshow/demos/demos.json
+-rw-r--r--   0        0        0    86887 2024-02-17 23:06:32.776215 kayalab-0.7.9/ezshow/demos/telecom/data/basestation.csv
+-rw-r--r--   0        0        0      300 2024-02-17 23:06:32.776900 kayalab-0.7.9/ezshow/demos/telecom/data/call.avsc
+-rw-r--r--   0        0        0 43705638 2024-02-17 23:06:32.821190 kayalab-0.7.9/ezshow/demos/telecom/data/calls.csv
+-rw-r--r--   0        0        0  2572296 2024-02-17 23:06:32.825652 kayalab-0.7.9/ezshow/demos/telecom/data/subscribers.csv
+-rw-r--r--   0        0        0     1841 2024-02-17 23:06:39.197447 kayalab-0.7.9/ezshow/demos/telecom/myApp/app.js
+-rwxr-xr-x   0        0        0     1638 2024-02-17 23:06:39.198180 kayalab-0.7.9/ezshow/demos/telecom/myApp/bin/www
+-rw-r--r--   0        0        0      215 2024-02-17 23:06:39.198641 kayalab-0.7.9/ezshow/demos/telecom/myApp/config.js
+-rw-r--r--   0        0        0   164393 2024-02-17 23:06:39.199133 kayalab-0.7.9/ezshow/demos/telecom/myApp/package-lock.json
+-rw-r--r--   0        0        0      562 2024-02-17 23:06:39.209125 kayalab-0.7.9/ezshow/demos/telecom/myApp/package.json
+-rw-r--r--   0        0        0    26975 2024-02-17 23:06:39.210204 kayalab-0.7.9/ezshow/demos/telecom/myApp/public/index.html
+-rw-r--r--   0        0        0      111 2024-02-17 23:06:39.211620 kayalab-0.7.9/ezshow/demos/telecom/myApp/public/stylesheets/style.css
+-rw-r--r--   0        0        0     2986 2024-02-17 23:06:39.212689 kayalab-0.7.9/ezshow/demos/telecom/myApp/routes/basedb.js
+-rw-r--r--   0        0        0     1319 2024-02-17 23:06:39.213101 kayalab-0.7.9/ezshow/demos/telecom/myApp/routes/convertTiff2Png.js
+-rw-r--r--   0        0        0      879 2024-02-17 23:06:39.213496 kayalab-0.7.9/ezshow/demos/telecom/myApp/routes/graphdb.js
+-rw-r--r--   0        0        0     2820 2024-02-17 23:06:39.213885 kayalab-0.7.9/ezshow/demos/telecom/myApp/routes/graphdb_dyn.js
+-rw-r--r--   0        0        0     2120 2024-02-17 23:06:39.214353 kayalab-0.7.9/ezshow/demos/telecom/myApp/routes/graphdb_stat.js
+-rw-r--r--   0        0        0      205 2024-02-17 23:06:39.214665 kayalab-0.7.9/ezshow/demos/telecom/myApp/routes/index.js
+-rw-r--r--   0        0        0     1034 2024-02-17 23:06:39.214959 kayalab-0.7.9/ezshow/demos/telecom/myApp/routes/maprdb.js
+-rw-r--r--   0        0        0     1056 2024-02-17 23:06:39.215555 kayalab-0.7.9/ezshow/demos/telecom/myApp/routes/marker.js
+-rw-r--r--   0        0        0      605 2024-02-17 23:06:39.215861 kayalab-0.7.9/ezshow/demos/telecom/myApp/routes/model.js
+-rw-r--r--   0        0        0      844 2024-02-17 23:06:39.216432 kayalab-0.7.9/ezshow/demos/telecom/myApp/routes/opentsdb.js
+-rw-r--r--   0        0        0     1062 2024-02-17 23:06:39.216932 kayalab-0.7.9/ezshow/demos/telecom/myApp/routes/process.js
+-rw-r--r--   0        0        0      696 2024-02-17 23:06:39.217850 kayalab-0.7.9/ezshow/demos/telecom/myApp/routes/upload.js
+-rw-r--r--   0        0        0      203 2024-02-17 23:06:39.218313 kayalab-0.7.9/ezshow/demos/telecom/myApp/routes/users.js
+-rw-r--r--   0        0        0      512 2024-02-17 23:06:39.218858 kayalab-0.7.9/ezshow/demos/telecom/myApp/tsdb.json
+-rw-r--r--   0        0        0       84 2024-02-17 23:06:39.219880 kayalab-0.7.9/ezshow/demos/telecom/myApp/views/error.pug
+-rw-r--r--   0        0        0       66 2024-02-17 23:06:39.220316 kayalab-0.7.9/ezshow/demos/telecom/myApp/views/index.pug
+-rw-r--r--   0        0        0      125 2024-02-17 23:06:39.220657 kayalab-0.7.9/ezshow/demos/telecom/myApp/views/layout.pug
+-rw-r--r--   0        0        0     1277 2024-02-17 23:06:46.384244 kayalab-0.7.9/ezshow/demos/telecom/py/baseStationDB.py
+-rw-r--r--   0        0        0      910 2024-02-17 23:06:46.384651 kayalab-0.7.9/ezshow/demos/telecom/py/baseStationDelta.py
+-rw-r--r--   0        0        0      647 2024-02-17 23:06:46.385029 kayalab-0.7.9/ezshow/demos/telecom/py/consumer.py
+-rw-r--r--   0        0        0      998 2024-02-17 23:06:46.390937 kayalab-0.7.9/ezshow/demos/telecom/py/consumerAvro.py
+-rw-r--r--   0        0        0     1297 2024-02-17 23:06:46.391852 kayalab-0.7.9/ezshow/demos/telecom/py/consumerCallDB.py
+-rw-r--r--   0        0        0     1393 2024-02-17 23:06:46.392726 kayalab-0.7.9/ezshow/demos/telecom/py/consumerCallDelta.py
+-rw-r--r--   0        0        0     1253 2024-02-17 23:06:46.393963 kayalab-0.7.9/ezshow/demos/telecom/py/ingest.py
+-rw-r--r--   0        0        0     1209 2024-02-17 23:06:46.394412 kayalab-0.7.9/ezshow/demos/telecom/py/joinCallBaseDelta.py
+-rw-r--r--   0        0        0     1237 2024-02-17 23:06:46.396284 kayalab-0.7.9/ezshow/demos/telecom/py/joinCallSubcriberDelta.py
+-rw-r--r--   0        0        0     1398 2024-02-17 23:06:46.396793 kayalab-0.7.9/ezshow/demos/telecom/py/opentsdb.py
+-rw-r--r--   0        0        0     1499 2024-02-17 23:06:46.397469 kayalab-0.7.9/ezshow/demos/telecom/py/producer.py
+-rwxr-xr-x   0        0        0      774 2024-02-17 23:06:46.397867 kayalab-0.7.9/ezshow/demos/telecom/py/readCSV.py
+-rw-r--r--   0        0        0      905 2024-02-17 23:06:46.398613 kayalab-0.7.9/ezshow/demos/telecom/py/subscriberDelta.py
+-rw-r--r--   0        0        0   900770 2024-02-16 16:56:01.822080 kayalab-0.7.9/ezshow/demos/telecom.png
+-rw-r--r--   0        0        0     3262 2024-02-29 02:19:37.701740 kayalab-0.7.9/ezshow/elements.py
+-rw-r--r--   0        0        0    15096 2024-02-29 02:03:58.567249 kayalab-0.7.9/ezshow/main.py
+-rw-r--r--   0        0        0     1754 2024-02-20 16:38:16.759221 kayalab-0.7.9/ezshow/python-kafka.py
+-rw-r--r--   0        0        0     7626 2024-02-27 22:51:30.376127 kayalab-0.7.9/ezshow/restrunner.py
+-rw-r--r--   0        0        0     1260 2024-02-17 16:48:25.243841 kayalab-0.7.9/ezshow/s3runner.py
+-rw-r--r--   0        0        0      499 2024-02-26 18:19:37.937043 kayalab-0.7.9/ezshow/shrunner.py
+-rw-r--r--   0        0        0     2831 2024-02-29 10:45:40.215851 kayalab-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0     8304 1970-01-01 00:00:00.000000 kayalab-0.7.9/PKG-INFO
```

### Comparing `kayalab-0.7.7/LICENSE` & `kayalab-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/README.md` & `kayalab-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezinfra/cloudinit.py` & `kayalab-0.7.9/ezinfra/cloudinit.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezinfra/kvm.py` & `kayalab-0.7.9/ezinfra/kvm.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezinfra/proxy.py` & `kayalab-0.7.9/ezinfra/proxy.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezinfra/pve.py` & `kayalab-0.7.9/ezinfra/pve.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezinfra/queue.py` & `kayalab-0.7.9/ezinfra/queue.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezinfra/remote.py` & `kayalab-0.7.9/ezinfra/remote.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezinfra/repo.py` & `kayalab-0.7.9/ezinfra/repo.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezinfra/sshkeys.py` & `kayalab-0.7.9/ezinfra/sshkeys.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezinfra/vms.py` & `kayalab-0.7.9/ezinfra/vms.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezinfra/vmw.py` & `kayalab-0.7.9/ezinfra/vmw.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezinfra/vmw_pchelper.py` & `kayalab-0.7.9/ezinfra/vmw_pchelper.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezlab/USAGE.md` & `kayalab-0.7.9/ezlab/USAGE.md`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezlab/ezmeral/ezdf.py` & `kayalab-0.7.9/ezlab/ezmeral/ezdf.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezlab/ezmeral/ezua.py` & `kayalab-0.7.9/ezlab/ezmeral/ezua.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezlab/main.py` & `kayalab-0.7.9/ezlab/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from nicegui import ui, app, native
 import requests
 
 from ezlab.parameters import DF, SUPPORTED_HVES, UA
 from ezlab.pages import ezmeral
 from ezlab.pages import settings
 from ezlab.pages import targets
+from ezlab.utils import README
 from ezshow import main as ezshow
 
 # Disable annoying messages in log view
 # Thanks to: https://sam.hooke.me/note/2023/10/nicegui-binding-propagation-warning/
 import nicegui.binding
 
 
@@ -109,19 +110,19 @@
             "Readme",
             icon="description",
             caption="how to use this app?",
         )
         .classes("w-full")
         .classes("text-bold")
     ):
-        readme = ""
-        with open(os.path.dirname(__file__) + "/USAGE.md", "r") as readmefile:
-            readme = readmefile.read()
+        # readme = ""
+        # with open(os.path.dirname(__file__) + "/USAGE.md", "r") as readmefile:
+        #     readme = readmefile.read()
 
-        ui.markdown(readme)
+        ui.markdown(README)
 
     # Settings section
     settings.menu()
 
     ui.separator()
 
     # Infrastructure section
```

### Comparing `kayalab-0.7.7/ezlab/pages/df.py` & `kayalab-0.7.9/ezlab/pages/df.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezlab/pages/ezmeral.py` & `kayalab-0.7.9/ezlab/pages/ezmeral.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezlab/pages/settings.py` & `kayalab-0.7.9/ezlab/pages/settings.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezlab/pages/sshkeys.py` & `kayalab-0.7.9/ezlab/pages/sshkeys.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezlab/pages/targets.py` & `kayalab-0.7.9/ezlab/pages/targets.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezlab/pages/vms.py` & `kayalab-0.7.9/ezlab/pages/vms.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezlab/parameters.py` & `kayalab-0.7.9/ezlab/parameters.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezlab/requirements.txt` & `kayalab-0.7.9/ezlab/requirements.txt`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezlab/utils.py` & `kayalab-0.7.9/ezlab/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,24 +18,24 @@
         pass
 
 ezapp = ModuleContext()
 ezapp.queue = Queue(1000)
 
 
 # Read the demos
-demopath = f"{pathlib.Path().resolve()}/ezshow/demos"
-demos: list = None
-
-demos = json.loads(importlib.resources.read_text("ezshow", "demos.json"))
+DEMOS = json.loads(importlib.resources.read_text("ezshow.demos", "demos.json"))
+# Read the usage
+README = importlib.resources.read_text("ezlab", "USAGE.md")
+# demopath = f"{pathlib.Path().resolve()}/ezshow/demos"
 # with open(f"{demopath}/demos.json", "r") as f:
 #     demos = json.load(f)
 
 
 def getdemo(name: str):
-    return [d for d in demos if d['name'] == name].pop()
+    return [d for d in DEMOS if d['name'] == name].pop()
 
 
 # validation for non-zero entry
 def nonzero(val):
     return len(val) != 0
 
 # wrapper to make sync calls async-like
@@ -86,7 +86,8 @@
 def get_fqdn(ip_string: str) -> str:
     fqdn, _, _ = socket.gethostbyaddr(ip_string)
     return fqdn
 
 
 def is_file(file):
     return os.path.isfile(os.path.abspath(file))
+
```

### Comparing `kayalab-0.7.7/ezlabctl/USAGE.md` & `kayalab-0.7.9/ezlabctl/USAGE.md`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezlabctl/common.py` & `kayalab-0.7.9/ezlabctl/common.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezlabctl/config.py` & `kayalab-0.7.9/ezlabctl/config.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezlabctl/connect.py` & `kayalab-0.7.9/ezlabctl/connect.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezlabctl/create.py` & `kayalab-0.7.9/ezlabctl/create.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezlabctl/delete.py` & `kayalab-0.7.9/ezlabctl/delete.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezlabctl/ezdf.py` & `kayalab-0.7.9/ezlabctl/ezdf.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezlabctl/ezua.py` & `kayalab-0.7.9/ezlabctl/ezua.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezlabctl/main.py` & `kayalab-0.7.9/ezlabctl/main.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezlabctl/parameters.py` & `kayalab-0.7.9/ezlabctl/parameters.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezlabctl/pve.py` & `kayalab-0.7.9/ezlabctl/pve.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezlabctl/requirements.txt` & `kayalab-0.7.9/ezlabctl/requirements.txt`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezlabctl/vmw.py` & `kayalab-0.7.9/ezlabctl/vmw.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/apprunner.py` & `kayalab-0.7.9/ezshow/apprunner.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,19 +31,17 @@
                 "currency": "GBP", #fake.currency_code(),
                 "transaction_date": fake.past_datetime(start_date="-12M").timestamp(),
             }
         )
 
     # logger.debug("Creating monitoring table")
     demo = getdemo(app.storage.general["demo"]["name"])
-    table_path = f"{demo['volume']}/{demo['table']}"
     stream_path = f"{demo['volume']}/{demo['stream']}"
-    create_monitoring_table(table_path=table_path)
 
-    logger.info("Sending %s messages to %s", len(transactions), topic)
+    logger.info("Sending %s messages to %s:%s", len(transactions), stream_path, topic)
     import timeit
     tic = timeit.default_timer()
 
     stream_publish(
         stream=stream_path,
         topic=topic,
         messages=transactions,
@@ -67,16 +65,19 @@
     ):
 
         if message == TASK_FINISHED:
             break
 
         # logger.debug(f"CONSUMING TRANSACTION: {message}")
         # yield message
-        print(f"Simulating txn processing for {message['id']}")
-        sleep(0.1)
+        # print(f"Simulating txn processing for {message['id']}")
+        # _id field requires string
+        profile = {"_id": str(message['transaction_date']), "sender": message["sender_account"], "receiver": message['receiver_account']}
+        logger.info("Update DB %s", profile)
+        send_to_profileDB(profile)
         count += 1
 
     toc = timeit.default_timer()
     logger.info(f"Processed %s transactions in %i seconds", count, toc - tic)
 
 
 def generate_calls(params: list, count: int):
@@ -101,14 +102,31 @@
     # logger.debug("MONITOR PUSH RESPONSE: %s", response)
 
     if isinstance(response, Exception):
         logger.warning("MONITOR PUSH FAILED: %s", response)
         return
 
 
+def send_to_profileDB(json_obj: str):
+    demo = getdemo(app.storage.general["demo"]["name"])
+    table_path = f"{demo['volume']}/{demo['table']}"
+
+    # logger.debug("Writing %s to %s", json_obj['_id'], table_path)
+
+    response = restrunner.dagpost(
+        f"/api/v2/table/{quote(table_path)}", json_obj=json_obj
+    )
+
+    # logger.debug("DB POST RESPONSE: %s", response.text)
+
+    if isinstance(response, Exception):
+        logger.warning("DB POST FAILED: %s", response)
+        return
+
+
 def create_monitoring_table(table_path):
     # create monitoring table if not exist
     path = quote(table_path, safe="")
     response = restrunner.dagput(f"/api/v2/table/{path}")
     if isinstance(response, Exception):
         if response.response.status_code != 409:
             logger.warning(f"MonitorDB creation FAILED: {response}")
@@ -226,15 +244,15 @@
         response = restrunner.kafkapost(path=f"/topics/{topic_path}", data={"records": [{"value": msg}]})
         if isinstance(response, Exception):
             logger.info(f"Message failed to push: {response}")
         else:
             # logger.debug(f"STREAM PUSH {msg}")
             app.storage.general["demo"]["counting"] += 1
     
-    logger.info("%s messages are sent to %s:%s", len(messages), stream, topic)
+    logger.info("Sent %s messages to %s:%s", len(messages), stream, topic)
 
 
 def stream_consume(stream: str, topic: str):
     topic_path = f"{stream}:{topic}"
 
     try:
         # Create consumer instance
@@ -249,38 +267,29 @@
 
         if not response:
             yield TASK_FINISHED
             return
 
         # logger.debug("CONSUMER INSTANCE CREATED: %s", response.text)
 
-        # Expected output from preceding command
-        # {
-        # "instance_id":"my_consumer_instance",
-        # "base_uri":"http://localhost:8082/consumers/my_json_consumer_group/instances/my_consumer_instance"
-        # }
         consumer_instance = response.json()
         consumer_instance_path = urlparse(consumer_instance['base_uri']).path
         # logger.debug("CONSUMER INSTANCE PATH: %s", consumer_instance_path)
 
         # subscribe to consumer
         restrunner.kafkapost(f"{consumer_instance_path}/subscription", data={ "topics": [ topic_path ] })
         # No content in response
 
         # get records
         records = restrunner.kafkaget(f"{consumer_instance_path}/records")
         if records.ok:
             for message in records.json():
                 # logger.debug("CONSUMER GOT MESSAGE: %s", message)
-                yield message["value"]
+                    yield message["value"]
 
-        # Expected output from preceding command
-        # [
-        # {"key":null,"value":{"foo":"bar"},"partition":0,"offset":0,"topic":"jsontest"}
-        # ]
     except Exception as error:
         logger.warning("STREAM CONSUMER ERROR %s", error)
 
     finally:
         # Unsubscribe from consumer instance
         restrunner.kafkadelete(
             f"/consumers/{topic}_consumer_group/instances/{topic}_consumer_instance"
@@ -307,75 +316,92 @@
 
 
 def topic_stats(topic: str):
     demo = getdemo(app.storage.general["demo"]["name"])
     stream_path = f"{demo['volume']}/{demo['stream']}"
     # topic_path = quote(f"{stream_path}:{topic}", safe="")
 
-    response = restrunner.get(f"/rest/stream/topic/info?path={stream_path}&topic={topic}")
-    if isinstance(response, Exception):
-        logger.warning(f"Failed to get metrics for {topic}: {response}")
-    else:
-        metrics = response.json()
-        # logger.debug("GOT METRICS %s", metrics)
-        series = []
-        for m in metrics["data"]:
-            series.append({"publishedMsgs": m["maxoffset"]})
-            series.append({"consumedMsgs": m["minoffsetacrossconsumers"]})
-            series.append(
-                {
-                    "latestAgo(s)": (
-                        datetime.now().astimezone() - dt_from_iso(m["maxtimestamp"])
-                    ).total_seconds()
-                }
-            )
-            series.append(
-                {
-                    "consumerLag(s)": (
-                        dt_from_iso(m["maxtimestamp"])
-                        - dt_from_iso(m["mintimestampacrossconsumers"])
-                    ).total_seconds()
+    try:
+        response = restrunner.get(f"/rest/stream/topic/info?path={stream_path}&topic={topic}")
+        if isinstance(response, Exception):
+            logger.warning(f"Failed to get topic stats for {topic}: {response}")
+        else:
+            metrics = response.json()
+            if not metrics["status"] == "ERROR":            
+                logger.debug("TOPIC STAT %s", metrics)
+
+                series = []
+                for m in metrics["data"]:
+                    series.append({"publishedMsgs": m["maxoffset"]}) # interestingly, maxoffset starts from -1
+                    series.append({"consumedMsgs": m["minoffsetacrossconsumers"]}) # this metric starts at 0
+                    series.append(
+                        {
+                            "latestAgo(s)": (
+                                datetime.now().astimezone() - dt_from_iso(m["maxtimestamp"])
+                            ).total_seconds()
+                        }
+                    )
+                    series.append(
+                        {
+                            "consumerLag(s)": (
+                                dt_from_iso(m["maxtimestamp"])
+                                - dt_from_iso(m["mintimestampacrossconsumers"])
+                            ).total_seconds()
+                        }
+                    )
+                # logger.info("Metrics %s", series)
+                return {
+                    "name": topic,
+                    "time": datetime.fromtimestamp(metrics["timestamp"]/(10**3)).strftime("%H:%M:%S"),
+                    "values": series,
                 }
-            )
-        # logger.info("Metrics %s", series)
-        return {
-            "name": topic,
-            "time": datetime.fromtimestamp(metrics["timestamp"]/(10**3)).strftime("%H:%M:%S"),
-            "values": series,
-        }
+            else:
+                logger.warn("Topic stat query error %s", metrics["errors"])
+
+    except Exception as error:
+        logger.warning("Topic stat request error %s", error)
 
 
 def consumer_stats(topic: str):
     demo = getdemo(app.storage.general["demo"]["name"])
     stream_path = f"{demo['volume']}/{demo['stream']}"
 
-    response = restrunner.get(
-        f"/rest/stream/cursor/list?path={stream_path}&topic={topic}"
-    )
-    if isinstance(response, Exception):
-        logger.warning(f"Failed to get metrics for {topic}: {response}")
-    else:
-        metrics = response.json()
-        # logger.debug("GOT METRICS %s", metrics)
-        series = []
-        for m in metrics["data"]:
-            series.append({ f"{m['consumergroup']}_{m['partitionid']}_lag(s)": float(m["consumerlagmillis"])/1000})
-            series.append({ f"{m['consumergroup']}_{m['partitionid']}_offsetBehind": int(m["produceroffset"]) - int(m['committedoffset'])})
-        # logger.info("Metrics %s", series)
-        return {
-            "name": "Consumer",
-            "time": datetime.fromtimestamp(metrics["timestamp"]/(10**3)).strftime("%H:%M:%S"),
-            "values": series,
-        }
+    try:
+        response = restrunner.get(
+            f"/rest/stream/cursor/list?path={stream_path}&topic={topic}"
+        )
+        if isinstance(response, Exception):
+            logger.warning(f"Failed to get consumer stats for {topic}: {response}")
+        else:
+            metrics = response.json()
+
+            if not metrics["status"] == "ERROR":
+                logger.debug("CONSUMER STAT %s", metrics)
+                series = []
+                for m in metrics["data"]:
+                    series.append({ f"{m['consumergroup']}_{m['partitionid']}_lag(s)": float(m["consumerlagmillis"])/1000})
+                    series.append({ f"{m['consumergroup']}_{m['partitionid']}_offsetBehind": int(m["produceroffset"]) - int(m['committedoffset'])})
+                # logger.info("Metrics %s", series)
+                return {
+                    "name": "Consumer",
+                    "time": datetime.fromtimestamp(metrics["timestamp"]/(10**3)).strftime("%H:%M:%S"),
+                    "values": series,
+                }
+            else:
+                logger.warn("Consumer stat query error %s", metrics["errors"])
+
+    except Exception as error:
+        logger.warning("Consumer stat request error %s", error)
 
 
 # Dummy function for informational steps
 def noop():
     return True
 
+
 # def get_jmx_metrics():
 #     buffertimestamp = (
 #         datetime.now() - timedelta(minutes=0)
 #     ).timestamp() * 10**6  # convert to microseconds
 
 #     # logger.debug(
 #     #     "Getting metrics from %s",
@@ -425,7 +451,27 @@
 
 
 # def null_metrics():
 #     # fake = Faker()
 #     df = pd.DataFrame(columns=("timestamp", "metricA", "metricB"))
 #     df.loc[0] = [datetime().now().timestamp(), 10*10, 5*10]
 #     yield df
+
+
+def detect_fraud(params: list, count: int):
+    demo = getdemo(app.storage.general["demo"]["name"])
+    table_path = f"{demo['volume']}/{demo['table']}"
+
+    response = restrunner.dagget(f"/api/v2/table/{quote(table_path, safe='')}?limit={count}")
+
+    if response is None:
+        logger.warning("DB GET FAILED: %s", response)
+        return
+
+    records = response.json()
+    # logger.info("DB GET RESPONSE: %s", records)
+
+    for record in records["DocumentStream"]:
+        # a dumb way to simulate a truth function by comparing accountIds
+        logger.info('#%s is fraud' if record['sender'] > record['receiver'] else 'safe transaction #%s', record['_id'])
+        sleep(0.2)
+        app.storage.general["demo"]["counting"] += 1
```

### Comparing `kayalab-0.7.7/ezshow/confluent.kafka.py` & `kayalab-0.7.9/ezshow/confluent.kafka.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/banking/banking.jpg` & `kayalab-0.7.9/ezshow/demos/banking.jpg`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/core-to-edge/core-edge.png` & `kayalab-0.7.9/ezshow/demos/core-edge.png`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/data/basestation.csv` & `kayalab-0.7.9/ezshow/demos/telecom/data/basestation.csv`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/data/calls.csv` & `kayalab-0.7.9/ezshow/demos/telecom/data/calls.csv`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/data/subscribers.csv` & `kayalab-0.7.9/ezshow/demos/telecom/data/subscribers.csv`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/myApp/app.js` & `kayalab-0.7.9/ezshow/demos/telecom/myApp/app.js`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/myApp/bin/www` & `kayalab-0.7.9/ezshow/demos/telecom/myApp/bin/www`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/myApp/package-lock.json` & `kayalab-0.7.9/ezshow/demos/telecom/myApp/package-lock.json`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/myApp/package.json` & `kayalab-0.7.9/ezshow/demos/telecom/myApp/package.json`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/myApp/public/index.html` & `kayalab-0.7.9/ezshow/demos/telecom/myApp/public/index.html`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/myApp/routes/basedb.js` & `kayalab-0.7.9/ezshow/demos/telecom/myApp/routes/basedb.js`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/myApp/routes/convertTiff2Png.js` & `kayalab-0.7.9/ezshow/demos/telecom/myApp/routes/convertTiff2Png.js`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/myApp/routes/graphdb.js` & `kayalab-0.7.9/ezshow/demos/telecom/myApp/routes/graphdb.js`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/myApp/routes/graphdb_dyn.js` & `kayalab-0.7.9/ezshow/demos/telecom/myApp/routes/graphdb_dyn.js`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/myApp/routes/graphdb_stat.js` & `kayalab-0.7.9/ezshow/demos/telecom/myApp/routes/graphdb_stat.js`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/myApp/routes/maprdb.js` & `kayalab-0.7.9/ezshow/demos/telecom/myApp/routes/maprdb.js`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/myApp/routes/marker.js` & `kayalab-0.7.9/ezshow/demos/telecom/myApp/routes/marker.js`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/myApp/routes/model.js` & `kayalab-0.7.9/ezshow/demos/telecom/myApp/routes/model.js`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/myApp/routes/opentsdb.js` & `kayalab-0.7.9/ezshow/demos/telecom/myApp/routes/opentsdb.js`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/myApp/routes/process.js` & `kayalab-0.7.9/ezshow/demos/telecom/myApp/routes/process.js`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/myApp/routes/upload.js` & `kayalab-0.7.9/ezshow/demos/telecom/myApp/routes/upload.js`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/myApp/tsdb.json` & `kayalab-0.7.9/ezshow/demos/telecom/myApp/tsdb.json`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/py/baseStationDB.py` & `kayalab-0.7.9/ezshow/demos/telecom/py/baseStationDB.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/py/baseStationDelta.py` & `kayalab-0.7.9/ezshow/demos/telecom/py/baseStationDelta.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/py/consumer.py` & `kayalab-0.7.9/ezshow/demos/telecom/py/consumer.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/py/consumerAvro.py` & `kayalab-0.7.9/ezshow/demos/telecom/py/consumerAvro.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/py/consumerCallDB.py` & `kayalab-0.7.9/ezshow/demos/telecom/py/consumerCallDB.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/py/consumerCallDelta.py` & `kayalab-0.7.9/ezshow/demos/telecom/py/consumerCallDelta.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/py/ingest.py` & `kayalab-0.7.9/ezshow/demos/telecom/py/ingest.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/py/joinCallBaseDelta.py` & `kayalab-0.7.9/ezshow/demos/telecom/py/joinCallBaseDelta.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/py/joinCallSubcriberDelta.py` & `kayalab-0.7.9/ezshow/demos/telecom/py/joinCallSubcriberDelta.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/py/opentsdb.py` & `kayalab-0.7.9/ezshow/demos/telecom/py/opentsdb.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/py/producer.py` & `kayalab-0.7.9/ezshow/demos/telecom/py/producer.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/py/readCSV.py` & `kayalab-0.7.9/ezshow/demos/telecom/py/readCSV.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/py/subscriberDelta.py` & `kayalab-0.7.9/ezshow/demos/telecom/py/subscriberDelta.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos/telecom/telecom.png` & `kayalab-0.7.9/ezshow/demos/telecom.png`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/demos.json` & `kayalab-0.7.9/ezshow/demos/demos.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.967846912202381%*

 * *Differences: {'0': "{'steps': {0: {'runner_target': "*

 * *      "'/rest/volume/create?name=banking&path=/apps/banking&tieringenable=true', delete: "*

 * *      "['runner_parameters']}, 1: {'runner_target': "*

 * *      "'/rest/stream/create?path=/apps/banking/activity&ttl=86400&compression=lz4', delete: "*

 * *      "['runner_parameters']}, 2: {'runner_parameters': ['transactions'], 'count': 20, "*

 * *      "'runner_target': 'send_transactions', delete: ['app_parameters']}, 3: {'runner_parameters': "*

 * *      "['transactions'], 'runner_target':  […]*

```diff
@@ -9,72 +9,88 @@
         "name": "banking",
         "steps": [
             {
                 "description": "We will start with creating a volume to place all app content. This will hold our data and provides an isolation for different apps and users. Volumes are also the primary construct to define data placement and distribution, replication/mirroring capabilities. It is easy to create a volume using REST API. \n\n!! If you get a warning that volume already exists, you can ignore it (forgot to clean up after previous run?). \n\nLet's create this stream by sending this request to Data Fabric REST API endpoint:",
                 "id": 1,
                 "name": "create the volume",
                 "runner": "rest",
-                "runner_parameters": "/rest/volume/create?name=banking&path=/apps/banking&tieringenable=true"
+                "runner_target": "/rest/volume/create?name=banking&path=/apps/banking&tieringenable=true"
             },
             {
                 "description": "Lets start with creating a stream for our application to send messages. The messages will be sent to their respective topics, and topics will be automatically created if they don't exist. This behaviour can be changed with stream settings, but we are not interested in that now. If needed, we can also create a topic manually using the same method (or any other available management interface, such as CLI & GUI). \n\nLet's submit this request to create the stream (don't worry if stream already exists, as a leftover from previous run):",
                 "id": 2,
                 "name": "create the stream",
                 "runner": "rest",
-                "runner_parameters": "/rest/stream/create?path=/apps/banking/activity&ttl=86400&compression=lz4"
+                "runner_target": "/rest/stream/create?path=/apps/banking/activity&ttl=86400&compression=lz4"
             },
             {
-                "app_parameters": [
-                    "transactions"
-                ],
                 "codes": [
                     "restrunner.kafkapost",
                     "apprunner.kafka_publish"
                 ],
-                "count": 500,
+                "count": 20,
                 "description": "Now we would like to push some transactions into the topic. We will use the `faker` library to generate random transactions and use Kafka REST interface to push these transactions into the `transactions` topic in our stream. It is preferred to use native clients and libraries, ie, Java, C, Python clients, in production for performance and scalability. \n\nYou can see below sample code for both REST API and Python library but we will be using only the REST API for its simplicity. For performance and flexibility, language-native APIs and libraries would be preferred in real-world.",
                 "id": 3,
                 "name": "create transactions",
                 "runner": "app",
-                "runner_parameters": "send_transactions"
-            },
-            {
-                "app_parameters": [
+                "runner_parameters": [
                     "transactions"
                 ],
+                "runner_target": "send_transactions"
+            },
+            {
                 "codes": [
                     "apprunner.stream_consume",
                     "apprunner.kafka_consume"
                 ],
                 "description": "We will capture the messages using Kafka REST interface and fake a transformation to strip relevant information from the messages. It is possible to do the same processing using any other client/library that is available for other programming languages. And an example code is provided below. \n\nEach message we will consume will correspond to a transaction and should be transformed to a format that is suitable for our fraud detection ML model. For low-latency access, we will use certain fields in the messages and push them into a JSON DocumentDB so our ML model can perform fast querying with filters and selects for specific accounts and timeframes, rather than trying to read all messages or transactions. \n\nIn a real-world scenario, we would run this process as a service across multiple instances to increase the throughput and reduce processing/response times. In our simple scenario, it is acceptable to process messages that are available right now in the topic and we are not concerned about future transactions now. \n\nLet's run the consumer code as shown below to process these messages.",
                 "id": 4,
                 "name": "process transactions",
                 "runner": "app",
-                "runner_parameters": "process_transactions"
+                "runner_parameters": [
+                    "transactions"
+                ],
+                "runner_target": "process_transactions"
             },
             {
-                "description": "Lets see what is currently going on with our transactions, using Kafka monitoring metrics. \n\nSelect the knobs below to activate metric collection from Streams, using REST API calls. They would provide visibility to published and consumed messages, and how much the consumers are lagging behind, for example. Enabling more in-depth metric collection is also possible using the JMX but we are not getting into those details here.",
+                "codes": [
+                    "apprunner.topic_stats",
+                    "apprunner.consumer_stats"
+                ],
+                "description": "Lets see what is currently going on with our transactions, using REST calls to capture topic and consumer/cursor information. \n\nSelect the knobs at the end of the page to activate metric collection from Streams. They would provide visibility to published and consumed messages, and how much the consumers are lagging behind, for example. Enabling more in-depth metric collection is also possible using the JMX but we are not getting into those details here.",
                 "id": 5,
                 "name": "monitor transaction flow",
                 "runner": "noop",
-                "runner_parameters": "monitor_transactions"
+                "runner_target": "monitor_transactions"
+            },
+            {
+                "codes": [
+                    "apprunner.detect_fraud"
+                ],
+                "count": 5,
+                "description": "A backend service would process the transaction history and build patterns to identify if a give transaction is fradulent or not. We assume you already have your [Fraud Detection Model](https://github.com/HPEEzmeral/ezua-tutorials/tree/release-1.2.0/demos/fraud-detection), so we can use that service to inference every incoming transaction to check if they match these trained patterns or not.\n\n Again, for simplicity, we will simply return a random result from that inferencing rather than actually asking an AI model to detect our transaction validity.",
+                "id": 6,
+                "name": "fraud detection for new transactions",
+                "runner": "app",
+                "runner_parameters": [],
+                "runner_target": "detect_fraud"
             },
             {
-                "description": "Since the kafka topics are created on a separate (internally managed) volume, we would delete the topic first.",
+                "description": "First we need to delete the stream that holds our topic (or topics where applicable but not in this scenario). We use a REST API call for that for simplicity.",
                 "id": 98,
-                "name": "clean up - delete the topic",
+                "name": "clean up - delete the stream",
                 "runner": "rest",
-                "runner_parameters": "/rest/kafkatopic/delete?topic=banking"
+                "runner_target": "/rest/stream/delete?path=/apps/banking/activity"
             },
             {
                 "description": "Once finished, we can delete the volume to get rid off all artifacts we created with this demo",
                 "id": 99,
                 "name": "clean up - delete the volume",
                 "runner": "rest",
-                "runner_parameters": "/rest/volume/remove?name=banking&force=true"
+                "runner_target": "/rest/volume/remove?name=banking&force=true"
             }
         ],
         "stream": "activity",
         "table": "profiles",
         "volume": "/apps/banking"
     },
     {
@@ -83,100 +99,100 @@
         "name": "telecom",
         "steps": [
             {
                 "description": "We will create a volume to store all app related information...",
                 "id": 1,
                 "name": "Create the volume",
                 "runner": "rest",
-                "runner_parameters": "/rest/volume/create?name=telecom&path=/apps/telecom&tieringenable=true"
+                "runner_target": "/rest/volume/create?name=telecom&path=/apps/telecom&tieringenable=true"
             },
             {
                 "description": "using REST",
                 "id": 2,
                 "name": "Copy files to the volume",
                 "runner": "restfile",
-                "runner_parameters": "data/"
+                "runner_target": "data/"
             },
             {
                 "description": "using pyspark",
                 "id": 3,
                 "name": "Insert base station details into delta table",
                 "runner": "shell",
-                "runner_parameters": "/opt/mapr/spark/spark-3.3.2/bin/pyspark < ./py/baseStationDelta.py"
+                "runner_target": "/opt/mapr/spark/spark-3.3.2/bin/pyspark < ./py/baseStationDelta.py"
             },
             {
                 "description": "using REST API",
                 "id": 4,
                 "name": "Create table for base stations",
                 "runner": "rest",
-                "runner_parameters": "/rest/table/create?path=/apps/telecom/basestations&tabletype=json"
+                "runner_target": "/rest/table/create?path=/apps/telecom/basestations&tabletype=json"
             },
             {
                 "description": "using REST API",
                 "id": 5,
                 "name": "Create table for calls",
                 "runner": "rest",
-                "runner_parameters": "/rest/table/create?path=/apps/telecom/calls&tabletype=json"
+                "runner_target": "/rest/table/create?path=/apps/telecom/calls&tabletype=json"
             },
             {
                 "description": "into delta table",
                 "id": 6,
                 "name": "Insert base station details",
                 "runner": "shell",
-                "runner_parameters": "/opt/mapr/spark/spark-3.3.2/bin/pyspark < ./py/baseStationDB.py"
+                "runner_target": "/opt/mapr/spark/spark-3.3.2/bin/pyspark < ./py/baseStationDB.py"
             },
             {
                 "description": "using CLI",
                 "id": 7,
                 "name": "Create Topic telecom:calls",
                 "runner": "shell",
-                "runner_parameters": "maprcli kafkatopic create -topic telecom:calls -ttl 36000 -compression lz4"
+                "runner_target": "maprcli kafkatopic create -topic telecom:calls -ttl 36000 -compression lz4"
             },
             {
                 "count": 200,
                 "description": "using Java",
                 "id": 8,
                 "name": "Publish calls into topic: telecom:calls",
                 "runner": "app",
-                "runner_parameters": "generate_calls"
+                "runner_target": "generate_calls"
             },
             {
                 "description": "using python",
                 "id": 9,
                 "name": "Process messages in topic telecom:calls",
                 "runner": "shell",
-                "runner_parameters": "./py/opentsdb.py"
+                "runner_target": "./py/opentsdb.py"
             },
             {
                 "description": "for dashboard",
                 "id": 10,
                 "name": "Start Web Service",
                 "runner": "shell",
-                "runner_parameters": "node ./myApp/bin/www &"
+                "runner_target": "node ./myApp/bin/www &"
             }
         ],
         "volume": "/apps/telecom"
     },
     {
         "description": "Hopefully available soon",
         "diagram": "core-edge.png",
         "name": "core to edge",
         "steps": [
             {
-                "description": "We need to create a remote volume to ...",
+                "description": "Let's start with creating a volume on our core cluster. This volume will be used to hold all our streaming and file data.",
                 "id": 1,
                 "name": "Create volume",
                 "runner": "rest",
-                "runner_parameters": "/rest/volume/create?name=core-to-edge&path=/apps/core-to-edge&tieringenable=true"
+                "runner_target": "/rest/volume/create?name=core-to-edge&path=/apps/core-to-edge&tieringenable=true"
             },
             {
                 "description": "We need to create a remote volume to ...",
                 "id": 2,
                 "input": "remote_cluster_host",
                 "name": "Create remote volume",
                 "runner": "rest",
-                "runner_parameters": "/rest/volume/create?name=core-to-edge&path=/apps/core-to-edge&tieringenable=true"
+                "runner_target": "/rest/volume/create?name=core-to-edge&path=/apps/core-to-edge&tieringenable=true"
             }
         ],
         "volume": "/apps/core-to-edge"
     }
 ]
```

### Comparing `kayalab-0.7.7/ezshow/main.py` & `kayalab-0.7.9/ezshow/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,32 @@
 from datetime import datetime
 import logging
+import importlib_resources
 from nicegui import app, ui, run, native
 import inspect
 
 import requests
 
 from ezshow import apprunner
 from ezshow import shrunner
 from ezshow import restrunner
 import ezshow
-from ezlab.utils import demos, demopath
+from ezlab.utils import DEMOS
+from ezshow.elements import get_echart, monitor_chart
 
 logger = logging.getLogger("ezshow")
 # Disable annoying messages in log view
 # Thanks to: https://sam.hooke.me/note/2023/10/nicegui-binding-propagation-warning/
 import nicegui.binding
 
 
 # Increase threshold for binding propagation warning from 0.01 to 0.02 seconds
 nicegui.binding.MAX_PROPAGATION_TIME = 0.03
 
-if not demos:
+if not DEMOS:
     print("Failed to load demos!")
     exit(1)
 
 
 @ui.page("/")
 def menu():
     # initialize app storage for demos
@@ -68,42 +70,44 @@
             # ).bind_enabled_from(
             #     app.storage.user, "busy", backward=lambda x: not x
             # ).bind_visibility_from(app.storage.user, "cookiejar", lambda x: x is None)
 
         demo_tabs = {}
         # Demos (Tabs)
         with ui.tabs().classes("w-full") as tabs:
-            for demo in demos:
+            for demo in DEMOS:
                 demo_tabs[demo["name"]] = ui.tab(demo["name"])
 
         # Demo content
         with (
             ui.tab_panels(tabs)
             .classes("w-full")
             .bind_value(app.storage.general["demo"], "name")
         ):
-            for demo in demos:
+            for demo in DEMOS:
 
                 # Demo panel
                 with ui.tab_panel(demo_tabs[demo["name"]]):
                     ui.markdown(demo["description"]).classes("font-normal")
                     ui.separator()
                     ui.image(
-                        f"{demopath}/{demo['name'].replace(' ', '-')}/{demo['diagram']}"
+                        importlib_resources.files("ezshow.demos").joinpath(
+                            f"{demo['diagram']}"
+                        )
                     ).classes("object-scale-down g-10")
 
                     ui.link(
                         "Source",
                         target=demo.get("link", "https://github.com/mapr-demos/"),
                         new_tab=True,
                     ).bind_visibility_from(
                         demo, "link", backward=lambda x: x is not None
                     )
                     ui.separator()
-                    ui.label("Follow the step by step demo flow")
+                    ui.label("Follow the steps...")
                     with ui.row():
                         ui.label("Using volume:")
                         ui.label(demo.get("volume", "/"))
 
                     # Steps
                     with (
                         ui.stepper()
@@ -115,18 +119,18 @@
                             # Step #
                             with ui.step(step["id"], title=step["name"].title()).props(
                                 f"active-icon=play_arrow caption=\"using {step['runner']}\""
                             ):
                                 ui.markdown(step["description"]).classes("font-normal")
                                 if step["runner"] == "rest":
                                     ui.label(
-                                        f"https://{appstore['host']}:8443{step['runner_parameters']}"
+                                        f"https://{appstore['host']}:8443{step['runner_target']}"
                                     )
 
-                                elif step['runner'] == 'app':
+                                elif step['runner'] in ['app', 'noop']:
                                     # Display source code if 'codes' provided
                                     if 'codes' in step.keys():
                                         for c in step['codes']:
                                             t = c.split('.')
                                             module_name=getattr(ezshow, t[0])
                                             function_name=t[1]
 
@@ -134,29 +138,30 @@
                                                 inspect.getsource(
                                                     getattr(
                                                         module_name,
                                                         function_name
                                                     )
                                                 )
                                             ).classes("w-full")
+                                            ui.separator()
                                     else:
-                                        ui.label(step["runner_parameters"])
-
-                                    # Display function params if 'count' is provided
-                                    if 'count' in step.keys():
-                                        ui.label().bind_text_from(
-                                            app.storage.user,
-                                            f"count__{demo['name'].replace(' ', '_')}__{step['id']}",
-                                            # format message to show function(param, count) format
-                                            backward=lambda x, y=step.get(
-                                                "app_parameters", None
-                                            ), p=step["runner_parameters"]: f"Will be running: {p}( {y}, {x} )"
-                                        )
-                                    else:
-                                        ui.label(f"Will be running: {step['runner_parameters']} ( {step.get('app_parameters', None)} )" )
+                                        ui.label(step["runner_target"])
+                                    if step['runner'] != "noop":
+                                        # Display function params if 'count' is provided
+                                        if 'count' in step.keys():
+                                            ui.label().bind_text_from(
+                                                app.storage.user,
+                                                f"count__{demo['name'].replace(' ', '_')}__{step['id']}",
+                                                # format message to show function(param, count) format
+                                                backward=lambda x, y=step.get(
+                                                    "runner_parameters", None
+                                                ), p=step["runner_target"]: f"Will be running: {p}( {y}, {x} )"
+                                            )
+                                        else:
+                                            ui.label(f"Will be running: {step['runner_target']} ( {step.get('runner_parameters', None)} )" )
 
                                 # Insert count slider if step wants one
                                 if step.get("count", None):
                                     with ui.row().classes("w-full"):
                                         slider = ui.slider(
                                             min=0,
                                             max=3*step['count'],
@@ -207,112 +212,23 @@
                                         on_click=stepper.previous,
                                     ).props("flat").bind_visibility_from(
                                         step, "id", backward=lambda x: x != 1
                                     )  # don't show for the first step
 
                     if "monitors" in demo.keys():
                         for mon in demo['monitors']:
-                            mon_chart = ui.echart(
-                                {
-                                    "tooltip": {
-                                        "trigger": "axis",
-                                        # "axisPointer": {"type": "cross"},
-                                    },
-                                    # "toolbox": {
-                                    #     "show": "true",
-                                    #     "right": 10,
-                                    #     "feature": {
-                                    #         "saveAsImage": {},
-                                    #     },
-                                    # },
-                                    "title": {"left": 10, "text": ""},
-                                    "legend": {"right": "center"},
-                                    "xAxis": {
-                                        "type": "category",
-                                        "boundaryGap": False,
-                                        "axisLine": {"onZero": "true"},
-                                        "splitLine": {"show": "false"},
-                                        "data": [],
-                                    },
-                                    "yAxis": [
-                                        {
-                                            "type": "value",
-                                            "name": "Count",
-                                            "boundaryGap": [0, "100%"],
-                                        },
-                                        {
-                                            "type": "value",
-                                            "name": "Milliseconds",
-                                            "axisLabel": {
-                                                "formatter": "{value} s",
-                                            },
-                                            "boundaryGap": [0, "100%"],
-                                        },
-                                    ],
-                                    "series": [  # manually set max series to display (TODO: find a pythonic way)
-                                        {
-                                            "type": "line",
-                                            "smooth": True,
-                                            "data": [],
-                                        },
-                                        {
-                                            "type": "line",
-                                            "symbol": "triangle",
-                                            "smooth": True,
-                                            "data": [],
-                                        },
-                                        {
-                                            "type": "line",
-                                            "symbol": "roundRect",
-                                            "smooth": True,
-                                            "data": [],
-                                        },
-                                        {
-                                            "type": "line",
-                                            "symbol": "pin",
-                                            "smooth": True,
-                                            "data": [],
-                                        },
-                                    ],
-                                },
-                            )
+                            mon_chart = get_echart()
                             # MONITOR FUNCTION SHOULD RETURN
                             # "name": dict_item["type"],
                             # "time": dict_item["time"],
                             # "values": [
                             #     {"Tx": dict_item["tx"]},
                             #     {"Rx": dict_item["rx"]},
                             # ],
-                            def add_metric(monitor_name, chart_name):
-                                t = monitor_name.split('.')
-                                module_name=getattr(ezshow, t[0])
-                                function_name=t[1]
-                                function_param=t[2]
-                                func = getattr(module_name, function_name)
-
-                                # collect the metrics
-                                metric = func(function_param)
-
-                                chart_name.options['xAxis']['data'].append(metric['time'])
-                                chart_name.options['title']['text'] = metric['name'].title()
-
-                                for idx, serie in enumerate(metric["values"]):
-                                    chart_series = chart_name.options['series'][idx]
-                                    for key in serie.keys():
-                                        if not chart_series.get('name', None):
-                                            chart_series['name'] = key
-                                        # if name ends with (s), place it onto second yAxis
-                                        if "(s)" in key:
-                                            chart_series["yAxisIndex"] = 1
-                                        chart_series['data'].append(int(serie[key]))
-                                chart_name.update()
-
-                            # Using lambda below so we capture the function name for individual steps
-                            timer = ui.timer(interval=5.0, callback=lambda monitor=mon, chart=mon_chart: add_metric(monitor, chart), active=False)
-                            ui.switch("->".join(mon.split('.')[1:]).title().replace('_', ' ')).bind_value(timer, "active")
+                            monitor_chart(mon, mon_chart)
 
     ezshow_menu.bind_value(app.storage.general["ui"], "ezshow")
 
 
 # async def login():
 #     app.storage.user["busy"] = True
 #     response = await run.io_bound(rest.get_session)
@@ -326,15 +242,15 @@
 #     app.storage.user["busy"] = False
 
 
 async def run_step(demo, step, pager: ui.stepper):
     app.storage.user["busy"] = True
 
     if step["runner"] == "rest":
-        response = await run.io_bound(restrunner.post, step["runner_parameters"])
+        response = await run.io_bound(restrunner.post, step["runner_target"])
         if isinstance(response, Exception):
             ui.notify(response, type="negative")
         elif response.ok:
             resjson = response.json()
             # print("DEBUG RESTRUNNER", resjson)
             # ts = resjson["timestamp"] / 1000 # ignore nanoseconds precision from timestamp
             # st = resjson.get("status", None)
@@ -351,15 +267,15 @@
             pager.next()
 
         else:  # http error returned
             ui.notify(message=response.text, html=True, type="warning")
 
     elif step["runner"] == "restfile":
         for response in await run.io_bound(
-            restrunner.postfile, demos, step["runner_parameters"]
+            restrunner.postfile, DEMOS, step["runner_target"]
         ):
             if isinstance(response, Exception):
                 ui.notify(response, type="negative")
             elif response.ok:
                 try:
                     # logging.debug("DEBUG: RESPONSE FROM RESTRUNNER: %s", response)
                     if response.status_code == 201:
@@ -371,42 +287,42 @@
                     print(error)
 
                 pager.next()
             else:  # http error returned
                 ui.notify(message=response.text, html=True, type="warning")
 
     elif step["runner"] == "shell":
-        ui.notify(shrunner.run_command(step["runner_parameters"]))
+        ui.notify(shrunner.run_command(step["runner_target"]))
         pager.next()
 
     elif step["runner"] == "app":
-        func = getattr(apprunner, step["runner_parameters"])
+        func = getattr(apprunner, step["runner_target"])
 
         if "count" in step.keys():
             # Reset the counter
             app.storage.general["demo"]["counting"] = 0
             # keep user selected count in sync
             count = app.storage.user[f"count__{demo['name'].replace(' ', '_')}__{step['id']}"]
 
             # add progressbar if 'count'ing
             ui.linear_progress().bind_value_from(
                 app.storage.general["demo"],
                 "counting",
                 backward=lambda x: f"{100 * int(x/count)} %",
             )
             
-            await run.io_bound(func, step["app_parameters"], count)
+            await run.io_bound(func, step["runner_parameters"], count)
 
         else:
-            await run.io_bound(func, step["app_parameters"])
+            await run.io_bound(func, step["runner_parameters"])
 
         # pager.next()
 
     else:
-        ui.notify(f"Would run {step['runner_parameters']} using {step['runner']}")
+        ui.notify(f"Would run {step['runner_target']} using {step['runner']}")
         pager.next()
 
     app.storage.user["busy"] = False
 
 
 # Entry point for the module
 def enter():
```

### Comparing `kayalab-0.7.7/ezshow/python-kafka.py` & `kayalab-0.7.9/ezshow/python-kafka.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/ezshow/restrunner.py` & `kayalab-0.7.9/ezshow/restrunner.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,49 +6,48 @@
 from nicegui import app
 
 logger = logging.getLogger("restrunner")
 
 if "demo" not in app.storage.general.keys():
     app.storage.general["demo"] = {}
 
-demostore = app.storage.general["demo"]
 
-AUTH_CREDENTIALS = (demostore.get("username", ""), demostore.get("password", ""))
+AUTH_CREDENTIALS = (app.storage.general["demo"].get("username", ""), app.storage.general["demo"].get("password", ""))
 
 
 def get(path: str):
-    REST_URL = f"https://{demostore['host']}:8443{path}"
+    REST_URL = f"https://{app.storage.general['demo']['host']}:8443{path}"
     try:
         response = requests.get(url=REST_URL, auth=AUTH_CREDENTIALS, verify=False)
         # logger.debug("GET RESPONSE: %s", response.text)
         response.raise_for_status()
         return response
 
     except Exception as error:
         logger.warning("GET ERROR %s", error)
         return None
 
 
 def post(path: str):
-    REST_URL = f"https://{demostore['host']}:8443{path}"
+    REST_URL = f"https://{app.storage.general['demo']['host']}:8443{path}"
     # logger.debug("POST URL: %s", REST_URL)
     try:
         response = requests.post(url=REST_URL, auth=AUTH_CREDENTIALS, verify=False)
         # logger.debug("POSTRESPONSE: %s", response)
         response.raise_for_status()
         return response
 
     except Exception as error:
         logger.warning("POST ERROR %s", error)
         return None
 
 
 def postfile(demos: list, path: str):
 
-    demo = [demo for demo in demos if demo["name"] == demostore["name"]].pop()
+    demo = [demo for demo in demos if demo["name"] == app.storage.general["demo"]["name"]].pop()
 
     basedir = (
         f"{pathlib.Path().resolve()}/ezshow/demos/{demo['name'].replace(' ', '-')}"
     )
     fileorfolder = f"{basedir}/{path}"
     volume = demo["volume"]
 
@@ -61,15 +60,15 @@
         source_files = [fileorfolder]
         target_dir = ""
 
     for file in source_files:
         filename = pathlib.Path(file).name
         destination = volume + "/" + target_dir + filename
         # files = {filename: open(file, "rb")}
-        REST_URL = f"https://{demostore['host']}:8443/files{destination}"
+        REST_URL = f"https://{app.storage.general['demo']['host']}:8443/files{destination}"
         try:
             with open(file, "rb") as f:
                 response = requests.put(
                     url=REST_URL,
                     auth=AUTH_CREDENTIALS,
                     verify=False,
                     data=f,
@@ -80,29 +79,29 @@
 
         except Exception as error:
             logger.warning("POSTFILE ERROR %s", error)
             return None
 
 
 def dagget(path: str):
-    REST_URL = f"https://{demostore['host']}:8243{path}"
+    REST_URL = f"https://{app.storage.general['demo']['host']}:8243{path}"
     # logger.debug("DAG GET %s", REST_URL)
     try:
         response = requests.get(url=REST_URL, auth=AUTH_CREDENTIALS, verify=False)
         # logger.debug("DAG GET RESPONSE: %s", response)
         response.raise_for_status()
         return response
 
     except Exception as error:
         logger.warning("DAG GET ERROR %s", error)
         return None
 
 
 def dagput(path: str, data=None):
-    REST_URL = f"https://{demostore['host']}:8243{path}"
+    REST_URL = f"https://{app.storage.general['demo']['host']}:8243{path}"
     # logger.debug("DAG PUT: %s", REST_URL)
     try:
         response = requests.put(url=REST_URL, auth=AUTH_CREDENTIALS, verify=False, data=data)
         # logger.debug("DAG PUT RESPONSE: %s", response)
         response.raise_for_status()
         return response
 
@@ -112,15 +111,15 @@
 
     except Exception as error:
         logger.warning("DAG PUT ERROR %s", error)
         return None
 
 
 def dagpost(path: str, json_obj=None):
-    REST_URL = f"https://{demostore['host']}:8243{path}"
+    REST_URL = f"https://{app.storage.general['demo']['host']}:8243{path}"
     # logger.debug("DAGPOSTDATA: %s", type(json_obj))
 
     try:
         response = requests.post(
             url=REST_URL,
             auth=AUTH_CREDENTIALS,
             verify=False,
@@ -133,15 +132,15 @@
 
     except Exception as error:
         logger.warning("DAG POST ERROR %s", error)
         return None
 
 
 def kafkaget(path: str):
-    REST_URL = f"https://{demostore['host']}:8082{path}"
+    REST_URL = f"https://{app.storage.general['demo']['host']}:8082{path}"
     # logger.debug("KAFKA GET %s", REST_URL)
     try:
         response = requests.get(
             url=REST_URL,
             auth=AUTH_CREDENTIALS,
             verify=False,
             headers={
@@ -156,15 +155,15 @@
     except Exception as error:
         # print(f"KAFKA GET ERROR {error}")
         logger.warning("KAFKA GET ERROR %s", error)
         return None
 
 
 def kafkaput(path: str, data=None):
-    REST_URL = f"https://{demostore['host']}:8082{path}"
+    REST_URL = f"https://{app.storage.general['demo']['host']}:8082{path}"
     # logger.debug("KAFKA PUT: %s", REST_URL)
     try:
         response = requests.put(
             url=REST_URL,
             auth=AUTH_CREDENTIALS,
             verify=False,
             data=json.dumps({"records": [{"value": data}]}),
@@ -176,15 +175,15 @@
 
     except Exception as error:
         logger.warning("KAFKA PUT ERROR %s", error)
         return None
 
 
 def kafkapost(path: str, data=None):
-    REST_URL = f"https://{demostore['host']}:8082{path}"
+    REST_URL = f"https://{app.storage.general['demo']['host']}:8082{path}"
     # logger.debug("KAFKA POST DATA: %s", data)
 
     try:
         response = requests.post(
             url=REST_URL,
             auth=AUTH_CREDENTIALS,
             verify=False,
@@ -198,15 +197,15 @@
     except Exception as error:
         # print(error.text)
         logger.warning("KAFKA POST ERROR %s", error)
         return None
 
 
 def kafkadelete(path: str):
-    REST_URL = f"https://{demostore['host']}:8082{path}"
+    REST_URL = f"https://{app.storage.general['demo']['host']}:8082{path}"
 
     try:
         response = requests.delete(
             url=REST_URL,
             auth=AUTH_CREDENTIALS,
             verify=False,
             headers={"Content-Type": "application/vnd.kafka.v2+json"},
@@ -224,17 +223,17 @@
         # print(f"KAFKA DELETE ERROR {error}")
         logger.warning("KAFKA DELETE ERROR %s", error)
         return None
 
 
 # Not used - basic auth used instead
 # def get_session():
-#     REST_URL = f"https://{demostore['target']}:8443/"
+#     REST_URL = f"https://{app.storage.general['demo']['target']}:8443/"
 #     AUTH_CREDENTIALS = (
-#         demostore["username"],
-#         demostore["password"],
+#         app.storage.general['demo']["username"],
+#         app.storage.general['demo']["password"],
 #     )
 #     try:
 #         return requests.get(url=REST_URL, auth=AUTH_CREDENTIALS, verify=False)
 
 #     except Exception as error:
 #         return error
```

### Comparing `kayalab-0.7.7/ezshow/s3runner.py` & `kayalab-0.7.9/ezshow/s3runner.py`

 * *Files identical despite different names*

### Comparing `kayalab-0.7.7/pyproject.toml` & `kayalab-0.7.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kayalab"
-version = "0.7.7"
+version = "0.7.9"
 description = "UI to create virtual machines and install HPE Ezmeral products."
 authors = ["Erdinc Kaya <erdincka@msn.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [
     {include = "ezlab"},
     {include = "ezlabctl"},
```

### Comparing `kayalab-0.7.7/PKG-INFO` & `kayalab-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kayalab
-Version: 0.7.7
+Version: 0.7.9
 Summary: UI to create virtual machines and install HPE Ezmeral products.
 License: MIT
 Author: Erdinc Kaya
 Author-email: erdincka@msn.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

