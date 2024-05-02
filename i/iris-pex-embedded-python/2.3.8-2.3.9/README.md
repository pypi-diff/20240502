# Comparing `tmp/iris_pex_embedded_python-2.3.8.tar.gz` & `tmp/iris_pex_embedded_python-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iris_pex_embedded_python-2.3.8.tar", last modified: Thu Jul 13 08:44:14 2023, max compression
+gzip compressed data, was "iris_pex_embedded_python-2.3.9.tar", last modified: Tue Oct  3 14:42:09 2023, max compression
```

## Comparing `iris_pex_embedded_python-2.3.8.tar` & `iris_pex_embedded_python-2.3.9.tar`

### file list

```diff
@@ -1,60 +1,61 @@
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-07-13 08:44:14.381668 iris_pex_embedded_python-2.3.8/
--rw-r--r--   0 grongier (902446405) 1252422112     1089 2021-08-27 09:20:59.000000 iris_pex_embedded_python-2.3.8/LICENSE
--rw-r--r--   0 grongier (902446405) 1252422112    49406 2023-07-13 08:44:14.380628 iris_pex_embedded_python-2.3.8/PKG-INFO
--rw-r--r--   0 grongier (902446405) 1252422112    48497 2023-05-31 16:31:35.000000 iris_pex_embedded_python-2.3.8/README.md
--rw-r--r--   0 grongier (902446405) 1252422112        0 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.3.8/pyproject.toml
--rw-r--r--   0 grongier (902446405) 1252422112       38 2023-07-13 08:44:14.381939 iris_pex_embedded_python-2.3.8/setup.cfg
--rw-r--r--   0 grongier (902446405) 1252422112     2323 2023-07-13 08:41:58.000000 iris_pex_embedded_python-2.3.8/setup.py
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-07-13 08:44:14.285791 iris_pex_embedded_python-2.3.8/src/
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-07-13 08:44:14.294156 iris_pex_embedded_python-2.3.8/src/grongier/
--rw-r--r--   0 grongier (902446405) 1252422112        0 2023-04-17 14:18:04.000000 iris_pex_embedded_python-2.3.8/src/grongier/__init__.py
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-07-13 08:44:14.282203 iris_pex_embedded_python-2.3.8/src/grongier/cls/
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-07-13 08:44:14.282702 iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-07-13 08:44:14.318793 iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/
--rw-r--r--   0 grongier (902446405) 1252422112      932 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/BusinessOperation.cls
--rw-r--r--   0 grongier (902446405) 1252422112     2633 2023-07-05 11:49:17.000000 iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/BusinessProcess.cls
--rw-r--r--   0 grongier (902446405) 1252422112     1039 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/BusinessService.cls
--rw-r--r--   0 grongier (902446405) 1252422112     3538 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/Common.cls
--rw-r--r--   0 grongier (902446405) 1252422112     1894 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/Director.cls
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-07-13 08:44:14.324854 iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/Duplex/
--rw-r--r--   0 grongier (902446405) 1252422112      543 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/Duplex/Operation.cls
--rw-r--r--   0 grongier (902446405) 1252422112     7103 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/Duplex/Process.cls
--rw-r--r--   0 grongier (902446405) 1252422112      179 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/Duplex/Service.cls
--rw-r--r--   0 grongier (902446405) 1252422112      628 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/InboundAdapter.cls
--rw-r--r--   0 grongier (902446405) 1252422112     8227 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/Message.cls
--rw-r--r--   0 grongier (902446405) 1252422112      976 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/OutboundAdapter.cls
--rw-r--r--   0 grongier (902446405) 1252422112     1691 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/PickleMessage.cls
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-07-13 08:44:14.327294 iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/PrivateSession/
--rw-r--r--   0 grongier (902446405) 1252422112     8065 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/PrivateSession/Duplex.cls
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-07-13 08:44:14.335118 iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/PrivateSession/Message/
--rw-r--r--   0 grongier (902446405) 1252422112      986 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/PrivateSession/Message/Ack.cls
--rw-r--r--   0 grongier (902446405) 1252422112      987 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/PrivateSession/Message/Poll.cls
--rw-r--r--   0 grongier (902446405) 1252422112      994 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/PrivateSession/Message/Start.cls
--rw-r--r--   0 grongier (902446405) 1252422112     1435 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/PrivateSession/Message/Stop.cls
--rw-r--r--   0 grongier (902446405) 1252422112     1622 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/Test.cls
--rw-r--r--   0 grongier (902446405) 1252422112    13498 2023-06-20 09:38:32.000000 iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/Utils.cls
--rw-r--r--   0 grongier (902446405) 1252422112     2908 2023-06-21 15:28:25.000000 iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/WSGI.cls
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-07-13 08:44:14.366025 iris_pex_embedded_python-2.3.8/src/grongier/pex/
--rw-r--r--   0 grongier (902446405) 1252422112     1166 2023-05-29 19:57:15.000000 iris_pex_embedded_python-2.3.8/src/grongier/pex/__init__.py
--rw-r--r--   0 grongier (902446405) 1252422112      107 2023-05-31 08:54:05.000000 iris_pex_embedded_python-2.3.8/src/grongier/pex/__main__.py
--rw-r--r--   0 grongier (902446405) 1252422112    20152 2023-06-19 12:50:33.000000 iris_pex_embedded_python-2.3.8/src/grongier/pex/_business_host.py
--rw-r--r--   0 grongier (902446405) 1252422112     3509 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.8/src/grongier/pex/_business_operation.py
--rw-r--r--   0 grongier (902446405) 1252422112    11838 2023-07-05 11:49:08.000000 iris_pex_embedded_python-2.3.8/src/grongier/pex/_business_process.py
--rw-r--r--   0 grongier (902446405) 1252422112     3735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.8/src/grongier/pex/_business_service.py
--rw-r--r--   0 grongier (902446405) 1252422112     5647 2023-06-16 15:49:29.000000 iris_pex_embedded_python-2.3.8/src/grongier/pex/_cli.py
--rw-r--r--   0 grongier (902446405) 1252422112    15158 2023-06-20 09:39:24.000000 iris_pex_embedded_python-2.3.8/src/grongier/pex/_common.py
--rw-r--r--   0 grongier (902446405) 1252422112     8810 2023-06-02 13:08:23.000000 iris_pex_embedded_python-2.3.8/src/grongier/pex/_director.py
--rw-r--r--   0 grongier (902446405) 1252422112     1661 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.8/src/grongier/pex/_inbound_adapter.py
--rw-r--r--   0 grongier (902446405) 1252422112      325 2023-06-19 10:23:02.000000 iris_pex_embedded_python-2.3.8/src/grongier/pex/_message.py
--rw-r--r--   0 grongier (902446405) 1252422112      735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.8/src/grongier/pex/_outbound_adapter.py
--rw-r--r--   0 grongier (902446405) 1252422112      331 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.8/src/grongier/pex/_pickle_message.py
--rw-r--r--   0 grongier (902446405) 1252422112     5033 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.8/src/grongier/pex/_private_session_duplex.py
--rw-r--r--   0 grongier (902446405) 1252422112     1722 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.8/src/grongier/pex/_private_session_process.py
--rw-r--r--   0 grongier (902446405) 1252422112    15326 2023-07-13 08:43:41.000000 iris_pex_embedded_python-2.3.8/src/grongier/pex/_utils.py
-drwxr-xr-x   0 grongier (902446405) 1252422112        0 2023-07-13 08:44:14.378376 iris_pex_embedded_python-2.3.8/src/iris_pex_embedded_python.egg-info/
--rw-r--r--   0 grongier (902446405) 1252422112    49406 2023-07-13 08:44:14.000000 iris_pex_embedded_python-2.3.8/src/iris_pex_embedded_python.egg-info/PKG-INFO
--rw-r--r--   0 grongier (902446405) 1252422112     1924 2023-07-13 08:44:14.000000 iris_pex_embedded_python-2.3.8/src/iris_pex_embedded_python.egg-info/SOURCES.txt
--rw-r--r--   0 grongier (902446405) 1252422112        1 2023-07-13 08:44:14.000000 iris_pex_embedded_python-2.3.8/src/iris_pex_embedded_python.egg-info/dependency_links.txt
--rw-r--r--   0 grongier (902446405) 1252422112       47 2023-07-13 08:44:14.000000 iris_pex_embedded_python-2.3.8/src/iris_pex_embedded_python.egg-info/entry_points.txt
--rw-r--r--   0 grongier (902446405) 1252422112       43 2023-07-13 08:44:14.000000 iris_pex_embedded_python-2.3.8/src/iris_pex_embedded_python.egg-info/requires.txt
--rw-r--r--   0 grongier (902446405) 1252422112        9 2023-07-13 08:44:14.000000 iris_pex_embedded_python-2.3.8/src/iris_pex_embedded_python.egg-info/top_level.txt
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-10-03 14:42:09.712916 iris_pex_embedded_python-2.3.9/
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1089 2021-08-27 09:20:59.000000 iris_pex_embedded_python-2.3.9/LICENSE
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    49494 2023-10-03 14:42:09.711824 iris_pex_embedded_python-2.3.9/PKG-INFO
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    48497 2023-05-31 16:31:35.000000 iris_pex_embedded_python-2.3.9/README.md
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2022-12-16 16:40:23.000000 iris_pex_embedded_python-2.3.9/pyproject.toml
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)       38 2023-10-03 14:42:09.713161 iris_pex_embedded_python-2.3.9/setup.cfg
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     2323 2023-10-03 14:41:24.000000 iris_pex_embedded_python-2.3.9/setup.py
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-10-03 14:42:09.638229 iris_pex_embedded_python-2.3.9/src/
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-10-03 14:42:09.643818 iris_pex_embedded_python-2.3.9/src/grongier/
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-04-17 14:18:04.000000 iris_pex_embedded_python-2.3.9/src/grongier/__init__.py
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-10-03 14:42:09.633734 iris_pex_embedded_python-2.3.9/src/grongier/cls/
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-10-03 14:42:09.636688 iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-10-03 14:42:09.663609 iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      932 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/BusinessOperation.cls
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     2633 2023-07-05 11:49:17.000000 iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/BusinessProcess.cls
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1039 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/BusinessService.cls
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     3745 2023-08-30 08:59:26.000000 iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/Common.cls
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1894 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/Director.cls
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-10-03 14:42:09.668699 iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/Duplex/
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      543 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/Duplex/Operation.cls
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     7103 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/Duplex/Process.cls
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      179 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/Duplex/Service.cls
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      628 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/InboundAdapter.cls
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     8227 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/Message.cls
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      976 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/OutboundAdapter.cls
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1691 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/PickleMessage.cls
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-10-03 14:42:09.670377 iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/PrivateSession/
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     8065 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/PrivateSession/Duplex.cls
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-10-03 14:42:09.676664 iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/PrivateSession/Message/
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      986 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/PrivateSession/Message/Ack.cls
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      987 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/PrivateSession/Message/Poll.cls
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      994 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/PrivateSession/Message/Start.cls
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1435 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/PrivateSession/Message/Stop.cls
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1622 2023-06-16 14:23:19.000000 iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/Test.cls
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    13498 2023-06-20 09:38:32.000000 iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/Utils.cls
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-10-03 14:42:09.678375 iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/Service/
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     2979 2023-08-28 14:39:29.000000 iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/Service/WSGI.cls
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-10-03 14:42:09.701755 iris_pex_embedded_python-2.3.9/src/grongier/pex/
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1166 2023-05-29 19:57:15.000000 iris_pex_embedded_python-2.3.9/src/grongier/pex/__init__.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      107 2023-05-31 08:54:05.000000 iris_pex_embedded_python-2.3.9/src/grongier/pex/__main__.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    19672 2023-08-23 12:45:00.000000 iris_pex_embedded_python-2.3.9/src/grongier/pex/_business_host.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     3509 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.9/src/grongier/pex/_business_operation.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    11838 2023-07-05 11:49:08.000000 iris_pex_embedded_python-2.3.9/src/grongier/pex/_business_process.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     3735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.9/src/grongier/pex/_business_service.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     5645 2023-10-03 14:40:19.000000 iris_pex_embedded_python-2.3.9/src/grongier/pex/_cli.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    15158 2023-06-20 09:39:24.000000 iris_pex_embedded_python-2.3.9/src/grongier/pex/_common.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     8810 2023-06-02 13:08:23.000000 iris_pex_embedded_python-2.3.9/src/grongier/pex/_director.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1661 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.9/src/grongier/pex/_inbound_adapter.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      325 2023-06-19 10:23:02.000000 iris_pex_embedded_python-2.3.9/src/grongier/pex/_message.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      735 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.9/src/grongier/pex/_outbound_adapter.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)      331 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.9/src/grongier/pex/_pickle_message.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     5033 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.9/src/grongier/pex/_private_session_duplex.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1722 2023-01-18 11:25:56.000000 iris_pex_embedded_python-2.3.9/src/grongier/pex/_private_session_process.py
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    15877 2023-10-03 14:20:58.000000 iris_pex_embedded_python-2.3.9/src/grongier/pex/_utils.py
+drwxr-xr-x   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        0 2023-10-03 14:42:09.709868 iris_pex_embedded_python-2.3.9/src/iris_pex_embedded_python.egg-info/
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)    49494 2023-10-03 14:42:09.000000 iris_pex_embedded_python-2.3.9/src/iris_pex_embedded_python.egg-info/PKG-INFO
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)     1928 2023-10-03 14:42:09.000000 iris_pex_embedded_python-2.3.9/src/iris_pex_embedded_python.egg-info/SOURCES.txt
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        1 2023-10-03 14:42:09.000000 iris_pex_embedded_python-2.3.9/src/iris_pex_embedded_python.egg-info/dependency_links.txt
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)       47 2023-10-03 14:42:09.000000 iris_pex_embedded_python-2.3.9/src/iris_pex_embedded_python.egg-info/entry_points.txt
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)       43 2023-10-03 14:42:09.000000 iris_pex_embedded_python-2.3.9/src/iris_pex_embedded_python.egg-info/requires.txt
+-rw-r--r--   0 grongier (902446405) ISCINTERNAL\Domain Users (1252422112)        9 2023-10-03 14:42:09.000000 iris_pex_embedded_python-2.3.9/src/iris_pex_embedded_python.egg-info/top_level.txt
```

### Comparing `iris_pex_embedded_python-2.3.8/LICENSE` & `iris_pex_embedded_python-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/PKG-INFO` & `iris_pex_embedded_python-2.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iris_pex_embedded_python
-Version: 2.3.8
+Version: 2.3.9
 Summary: iris_pex_embedded_python
 Home-page: https://github.com/grongierisc/interoperability-embedded-python
 Author: grongier
 Author-email: guillaume.rongier@intersystems.com
 License: MIT
 Keywords: iris_pex_embedded_python
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,14 +17,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: dacite>=1.6.0
+Requires-Dist: xmltodict>=0.12.0
+Requires-Dist: irissqlcli
 
 # 1. interoperability-embedded-python
 
 This proof of concept aims to show how the **iris interoperability framework** can be use with **embedded python**.
 
 ## 1.1. Table of Contents
```

### Comparing `iris_pex_embedded_python-2.3.8/README.md` & `iris_pex_embedded_python-2.3.9/README.md`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/setup.py` & `iris_pex_embedded_python-2.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
     # Do the setup
     setup(
         name='iris_pex_embedded_python',
         description='iris_pex_embedded_python',
         long_description=long_description,
         long_description_content_type='text/markdown',
-        version='2.3.8',
+        version='2.3.9',
         author='grongier',
         author_email='guillaume.rongier@intersystems.com',
         keywords='iris_pex_embedded_python',
         url='https://github.com/grongierisc/interoperability-embedded-python',
         license='MIT',
         classifiers=[
             'Development Status :: 5 - Production/Stable',
```

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/BusinessOperation.cls` & `iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/BusinessOperation.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/BusinessProcess.cls` & `iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/BusinessProcess.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/BusinessService.cls` & `iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/BusinessService.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/Common.cls` & `iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/Common.cls`

 * *Files 16% similar despite different names*

```diff
@@ -45,31 +45,47 @@
 		do ..%class."_dispatch_on_init"($this)
 	} catch ex {
 		set tSC = ex.AsStatus()
 	}
 	quit tSC
 }
 
+ClassMethod SetPythonPath(pClasspaths)
+{
+    set sys = ##class(%SYS.Python).Import("sys")
+
+    for i=0:1:(sys.path."__len__"()-1) {
+        Try {
+            if sys.path."__getitem__"(i) = pClasspaths {
+                do sys.path."__delitem__"(i)
+            }
+        }
+        Catch ex {
+            // do nothing
+        }
+
+    }
+    do sys.path.insert(0, pClasspaths)
+}
+
 Method Connect() As %Status
 {
 	set tSC = $$$OK
 	try {
 		
 		set container = $this
 		
 		//set classpass
 		if ..%classpaths '="" {
-			set sys = ##class(%SYS.Python).Import("sys")
 			set delimiter = $s($system.Version.GetOS()="Windows":";",1:":")
 			set extraClasspaths = $tr(container.%classpaths,delimiter,"|")
 			for i=1:1:$l(extraClasspaths,"|") {
 				set onePath = $p(extraClasspaths,"|",i)
 				set onePath = ##class(%File).NormalizeDirectory(onePath)
-				if onePath?1"$$IRISHOME"1P.E set onePath = $e($system.Util.InstallDirectory(),1,*-1)_$e(onePath,11,*)
-				if onePath'="" do sys.path.append(onePath)
+				do ..SetPythonPath(onePath)
 			}
 		}
 		if $isObject(..%class)=0 {
 			set importlib = ##class(%SYS.Python).Import("importlib")
 			set builtins = ##class(%SYS.Python).Import("builtins")
 			set module = importlib."import_module"(..%module)
 			set class = builtins.getattr(module, ..%classname)
```

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/Director.cls` & `iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/Director.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/Duplex/Operation.cls` & `iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/Duplex/Operation.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/Duplex/Process.cls` & `iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/Duplex/Process.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/InboundAdapter.cls` & `iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/InboundAdapter.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/Message.cls` & `iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/Message.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/OutboundAdapter.cls` & `iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/OutboundAdapter.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/PickleMessage.cls` & `iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/PickleMessage.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/PrivateSession/Duplex.cls` & `iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/PrivateSession/Duplex.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/PrivateSession/Message/Ack.cls` & `iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/PrivateSession/Message/Ack.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/PrivateSession/Message/Poll.cls` & `iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/PrivateSession/Message/Poll.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/PrivateSession/Message/Start.cls` & `iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/PrivateSession/Message/Start.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/PrivateSession/Message/Stop.cls` & `iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/PrivateSession/Message/Stop.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/Test.cls` & `iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/Test.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/Utils.cls` & `iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/PEX/Utils.cls`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/cls/Grongier/PEX/WSGI.cls` & `iris_pex_embedded_python-2.3.9/src/grongier/cls/Grongier/Service/WSGI.cls`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,16 @@
-Class Grongier.PEX.WSGI Extends (%RegisteredObject, %CSP.REST) [ ServerOnly = 1 ]
+Class Grongier.Service.WSGI Extends (%RegisteredObject, %CSP.REST) [ ServerOnly = 1 ]
 {
 
 Parameter CLASSPATHS;
 
 Parameter MODULENAME;
 
 Parameter APPNAME;
 
-/// Instance of class
-Property app As %SYS.Python;
-
 /// Helper method to write data to the output stream
 ClassMethod write(data)
 {
     w data
 }
 
 /// Helper to build the environ
@@ -40,30 +37,45 @@
     do dict."__setitem__"("PATH_INFO", $extract(updatedurl,$length(path),*))
 
     // to extract the query string
 
     return dict
 }
 
-ClassMethod Page(skipheader As %Boolean = 1) As %Status [ Internal, ServerOnly = 1 ]
+/// Implement a singleton pattern to get the python app
+ClassMethod GetPyhonApp() As %SYS.Python
 {
-    Try {
-        //set classpass
-        if ..#CLASSPATHS '="" {
-            set sys = ##class(%SYS.Python).Import("sys")
-            set delimiter = $s($system.Version.GetOS()="Windows":";",1:":")
-            set extraClasspaths = $tr(..#CLASSPATHS,delimiter,"|")
-            for i=1:1:$l(extraClasspaths,"|") {
-                set onePath = $p(extraClasspaths,"|",i)
-                set onePath = ##class(%File).NormalizeDirectory(onePath)
-                if onePath?1"$$IRISHOME"1P.E set onePath = $e($system.Util.InstallDirectory(),1,*-1)_$e(onePath,11,*)
-                if onePath'="" do sys.path.append(onePath)
-            }
+    if ..#CLASSPATHS '="" {
+        set sys = ##class(%SYS.Python).Import("sys")
+        set delimiter = $s($system.Version.GetOS()="Windows":";",1:":")
+        set extraClasspaths = $tr(..#CLASSPATHS,delimiter,"|")
+        for i=1:1:$l(extraClasspaths,"|") {
+            set onePath = $p(extraClasspaths,"|",i)
+            set onePath = ##class(%File).NormalizeDirectory(onePath)
+            if onePath?1"$$IRISHOME"1P.E set onePath = $e($system.Util.InstallDirectory(),1,*-1)_$e(onePath,11,*)
+            if onePath'="" do sys.path.append(onePath)
         }
+    }
+
+    //import module
+    set module = ##class(%SYS.Python).Import(..#MODULENAME)
+
+    //set builtins
+    set builtins = ##class(%SYS.Python).Import("builtins")
+
+    //set app
+    set application = builtins.getattr(module, ..#APPNAME)
 
+    Return application
+}
+
+ClassMethod Page(skipheader As %Boolean = 1) As %Status [ Internal, ServerOnly = 1 ]
+{
+    Try {
+        
         //set environ
         set environ = ..GetEnviron()
 
         //import sys
         set sys = ##class(%SYS.Python).Import("sys")
 
         //set stdin
@@ -72,22 +84,16 @@
         
         while %request.Content.AtEnd = 0 {
             do ba.extend(##class(%SYS.Python).Bytes(%request.Content.Read()))
         }
         //set handler
         set handler = ##class(%SYS.Python).Import("grongier.pex.wsgi.handlers").IrisHandler(ba, sys.stdout, sys.stderr,environ)
 
-        //set module
-        set module = ##class(%SYS.Python).Import(..#MODULENAME)
-
-        //set builtins
-        set builtins = ##class(%SYS.Python).Import("builtins")
-
-        //set app
-        set application = builtins.getattr(module, ..#APPNAME)
+        // get a singleton app
+        set application = ..GetPyhonApp()
 
         //run app
         do handler.run(application)
 
     }
     Catch ex {
         return ex.AsStatus()
```

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/pex/__init__.py` & `iris_pex_embedded_python-2.3.9/src/grongier/pex/__init__.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/pex/_business_host.py` & `iris_pex_embedded_python-2.3.9/src/grongier/pex/_business_host.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import iris
 
 from inspect import signature
 
 from dacite import from_dict, Config
 
 from grongier.pex._common import _Common
+from grongier.pex._utils import _Utils
 
 class _BusinessHost(_Common):
     """ This is a superclass for BusinessService, BusinesProcess, and BusinessOperation that
     defines common methods. It is a subclass of Common.
     """
 
     buffer:int = 64000
@@ -127,19 +128,15 @@
         pickle_string = codecs.encode(pickle.dumps(message), "base64").decode()
         module = message.__class__.__module__
         classname = message.__class__.__name__
 
         msg = iris.cls('Grongier.PEX.PickleMessage')._New()
         msg.classname = module + "." + classname
 
-        stream = iris.cls('%Stream.GlobalCharacter')._New()
-        n = self.buffer
-        chunks = [pickle_string[i:i+n] for i in range(0, len(pickle_string), n)]
-        for chunk in chunks:
-            stream.Write(chunk)
+        stream = _Utils.string_to_stream(pickle_string)
         msg.jstr = stream
 
         return msg
 
 
     def _dispatch_serializer(self,message):
         """
@@ -172,19 +169,15 @@
         json_string = json.dumps(message, cls=IrisJSONEncoder)
         module = message.__class__.__module__
         classname = message.__class__.__name__
 
         msg = iris.cls('Grongier.PEX.Message')._New()
         msg.classname = module + "." + classname
 
-        stream = iris.cls('%Stream.GlobalCharacter')._New()
-        n = self.buffer
-        chunks = [json_string[i:i+n] for i in range(0, len(json_string), n)]
-        for chunk in chunks:
-            stream.Write(chunk)
+        stream = _Utils.string_to_stream(json_string)
         msg.jstr = stream
 
         return msg
 
 
     def _serialize(self,message):
         """ Converts a message into json format.
@@ -204,18 +197,15 @@
             return None
 
     def _deserialize_pickle_message(self,serial):
         """ 
         Converts an iris grongier.pex.message into an python dataclass message.
         
         """
-        string = ""
-        serial.jstr.Rewind()
-        while not serial.jstr.AtEnd:
-            string += serial.jstr.Read(self.buffer)
+        string = _Utils.stream_to_string(serial.jstr)
 
         msg = pickle.loads(codecs.decode(string.encode(), "base64"))
         return msg
 
     def _dispatch_deserializer(self,serial):
         """
         If the serialized object is a Message, deserialize it as a Message, otherwise deserialize it as a
@@ -245,18 +235,15 @@
             raise ValueError("Classname must include a module: " + classname)
         try:
             module = importlib.import_module(classname[:j])
             msg = getattr(module, classname[j+1:])
         except Exception:
             raise ImportError("Class not found: " + classname)
 
-        string = ""
-        serial.jstr.Rewind()
-        while not serial.jstr.AtEnd:
-            string += serial.jstr.Read(self.buffer)
+        string = _Utils.stream_to_string(serial.jstr)
 
         jdict = json.loads(string, cls=IrisJSONDecoder)
         msg = self._dataclass_from_dict(msg,jdict)
         return msg
 
 
     def _deserialize(self,serial):
```

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/pex/_business_operation.py` & `iris_pex_embedded_python-2.3.9/src/grongier/pex/_business_operation.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/pex/_business_process.py` & `iris_pex_embedded_python-2.3.9/src/grongier/pex/_business_process.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/pex/_business_service.py` & `iris_pex_embedded_python-2.3.9/src/grongier/pex/_business_service.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/pex/_cli.py` & `iris_pex_embedded_python-2.3.9/src/grongier/pex/_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,18 +87,17 @@
         _Director.stop_production()
 
     elif args.status:
         dikt=_Director.status_production()
         print(json.dumps(dikt, indent=4))
 
     elif args.export:
-
         if args.export == 'not_set':
             # export default production
-            args.export= _Director.get_default_production()
+            args.export=_Director.get_default_production()
 
         dikt = _Utils.export_production(args.export)
         print(json.dumps(dikt, indent=4))
 
     else:
         # display help and default production name
         print("usage: iop [-h] [-d DEFAULT] [-l] [-s START] [-k] [-S] [-r] [-M MIGRATE] [-e EXPORT] [-x] [-v] [-L]")
```

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/pex/_common.py` & `iris_pex_embedded_python-2.3.9/src/grongier/pex/_common.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/pex/_director.py` & `iris_pex_embedded_python-2.3.9/src/grongier/pex/_director.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/pex/_inbound_adapter.py` & `iris_pex_embedded_python-2.3.9/src/grongier/pex/_inbound_adapter.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/pex/_outbound_adapter.py` & `iris_pex_embedded_python-2.3.9/src/grongier/pex/_outbound_adapter.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/pex/_private_session_duplex.py` & `iris_pex_embedded_python-2.3.9/src/grongier/pex/_private_session_duplex.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/pex/_private_session_process.py` & `iris_pex_embedded_python-2.3.9/src/grongier/pex/_private_session_process.py`

 * *Files identical despite different names*

### Comparing `iris_pex_embedded_python-2.3.8/src/grongier/pex/_utils.py` & `iris_pex_embedded_python-2.3.9/src/grongier/pex/_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -162,70 +162,75 @@
             module = packages+'.'+mod
         else:
             module = mod
 
         return module
 
     @staticmethod
-    def migrate(filename=None):
+    def migrate(filename=None,root_path=None):
         """ 
         Read the settings.py file and register all the components
         settings.py file has two dictionaries:
             * CLASSES
                 * key: the name of the class
                 * value: an instance of the class
             * PRODUCTIONS
                 list of dictionaries:
                 * key: the name of the production
                 * value: a dictionary containing the settings for the production
         """
         # try to load the settings file
-        try:
-            if filename:
-                import sys
-                path = None
-                # check if the filename is absolute or relative
-                if os.path.isabs(filename):
-                    path = os.path.dirname(filename)
-                else:
-                    raise ValueError("The filename must be absolute")
-                # add the path to the system path
-                sys.path.append(path)
-            import settings
-        except ImportError:
-            # return an error if the settings file is not found
-            # and explain how to create it
-            raise ImportError("settings.py file not found. Please create it in the same directory as the main.py file. See the documentation for more information.")
+        if filename:
+            import sys
+            path = None
+            # check if the filename is absolute or relative
+            if os.path.isabs(filename):
+                path = os.path.dirname(filename)
+            else:
+                raise ValueError("The filename must be absolute")
+            # add the path to the system path
+            sys.path.append(path)
+        import settings
+        # get the path of the settings file
+        path = os.path.dirname(inspect.getfile(settings))
         try:
             # set the classes settings
-            _Utils.set_classes_settings(settings.CLASSES)
+            _Utils.set_classes_settings(settings.CLASSES,path)
         except AttributeError:
             print("No classes to register")
         try:
             # set the productions settings
-            _Utils.set_productions_settings(settings.PRODUCTIONS)
+            _Utils.set_productions_settings(settings.PRODUCTIONS,path)
         except AttributeError:
             print("No productions to register")
 
 
 
     @staticmethod
-    def set_classes_settings(class_items):
+    def set_classes_settings(class_items,root_path=None):
         """
         It takes a dictionary of classes and returns a dictionary of settings for each class
         
         :param class_items: a dictionary of classes
         :return: a dictionary of settings for each class
         """
         for key, value in class_items.items():
             if inspect.isclass(value):
-                path = os.path.dirname(inspect.getfile(value))
+                path = None
+                if root_path:
+                    path = root_path
+                else:
+                    path = os.path.dirname(inspect.getfile(value))
                 _Utils.register_component(value.__module__,value.__name__,path,1,key)
             elif inspect.ismodule(value):
-                path = os.path.dirname(inspect.getfile(value))
+                path = None
+                if root_path:
+                    path = root_path
+                else:
+                    path = os.path.dirname(inspect.getfile(value))
                 _Utils._register_file(value.__name__+'.py',path,1,key)
             # if the value is a dict
             elif isinstance(value,dict):
                 # if the dict has a key 'path' and a key 'module' and a key 'class'
                 if 'path' in value and 'module' in value and 'class' in value:
                     # register the component
                     _Utils.register_component(value['module'],value['class'],value['path'],1,key)
@@ -240,54 +245,59 @@
                 # if the dict has a key 'path'
                 elif 'path' in value:
                     # register folder
                     _Utils.register_folder(value['path'],1,key)
                 else:
                     raise ValueError(f"Invalid value for {key}.")
 
-
     @staticmethod
-    def set_productions_settings(production_list):
+    def set_productions_settings(production_list,root_path=None):
         """
         It takes a list of dictionaries and registers the productions
         """
         # for each production in the list
         for production in production_list:
             # get the production name (first key in the dictionary)
             production_name = list(production.keys())[0]
             # set the first key to 'production'
             production['Production'] = production.pop(production_name)
             # handle Items
-            production = _Utils.handle_items(production)
+            production = _Utils.handle_items(production,root_path)
             # transform the json as an xml
             xml = _Utils.dict_to_xml(production)
             # register the production
             _Utils.register_production(production_name,xml)
 
     @staticmethod
-    def handle_items(production):
+    def handle_items(production,root_path=None):
         # if an item is a class, register it and replace it with the name of the class
         if 'Item' in production['Production']:
             # for each item in the list
             for i,item in enumerate(production['Production']['Item']):
                 # if the attribute "@ClassName" is a class, register it and replace it with the name of the class
                 if '@ClassName' in item:
                     if inspect.isclass(item['@ClassName']):
-                        path = os.path.dirname(inspect.getfile(item['@ClassName']))
+                        path = None
+                        if root_path:
+                            path = root_path
+                        else:
+                            path = os.path.dirname(inspect.getfile(item['@ClassName']))
                         _Utils.register_component(item['@ClassName'].__module__,item['@ClassName'].__name__,path,1,item['@Name'])
                         # replace the class with the name of the class
                         production['Production']['Item'][i]['@ClassName'] = item['@Name']
                 # if the attribute "@ClassName" is a dict
                 elif isinstance(item['@ClassName'],dict):
                     # create a new dict where the key is the name of the class and the value is the dict
                     class_dict = {item['@Name']:item['@ClassName']}
                     # pass the new dict to set_classes_settings
                     _Utils.set_classes_settings(class_dict)
                     # replace the class with the name of the class
                     production['Production']['Item'][i]['@ClassName'] = item['@Name']
+                else:
+                    raise ValueError(f"Invalid value for {item['@Name']}.")
 
         return production
 
     @staticmethod
     def dict_to_xml(json):
         """
         It takes a json and returns an xml
@@ -312,19 +322,15 @@
         :param xml: the xml of the production
         :type xml: str
         """
         # split the production name in the package name and the production name
         # the production name is the last part of the string
         package = '.'.join(production_name.split('.')[:-1])
         production_name = production_name.split('.')[-1]
-        stream = iris.cls('%Stream.GlobalCharacter')._New()
-        # for each chunk of 1024 characters
-        for i in range(0, len(xml), 1024):
-            # write the chunk to the stream
-            stream.Write(xml[i:i+1024])
+        stream = _Utils.string_to_stream(xml)
         # register the production
         _Utils.raise_on_error(iris.cls('Grongier.PEX.Utils').CreateProduction(package,production_name,stream))
 
     @staticmethod
     def export_production(production_name):
         """
         It takes a production name and exports the production
@@ -335,15 +341,29 @@
         def postprocessor(path, key, value):
             if value is None:
                 return key, ''
             return key, value
         # export the production
         xdata = iris.cls('Grongier.PEX.Utils').ExportProduction(production_name)
         # for each chunk of 1024 characters
-        string = ""
-        xdata.Rewind()
-        while not xdata.AtEnd:
-            string += xdata.Read(1024)
+        string = _Utils.stream_to_string(xdata)
         # convert the xml to a dictionary
         data = xmltodict.parse(string,postprocessor=postprocessor)
         # return the dictionary
         return data
+
+    @staticmethod
+    def stream_to_string(stream)-> str:
+        string = ""
+        stream.Rewind()
+        while not stream.AtEnd:
+            string += stream.Read(4092)
+        return string
+    
+    @staticmethod
+    def string_to_stream(string:str):
+        stream = iris.cls('%Stream.GlobalCharacter')._New()
+        n = 4092
+        chunks = [string[i:i+n] for i in range(0, len(string), n)]
+        for chunk in chunks:
+            stream.Write(chunk)
+        return stream
```

### Comparing `iris_pex_embedded_python-2.3.8/src/iris_pex_embedded_python.egg-info/PKG-INFO` & `iris_pex_embedded_python-2.3.9/src/iris_pex_embedded_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iris-pex-embedded-python
-Version: 2.3.8
+Version: 2.3.9
 Summary: iris_pex_embedded_python
 Home-page: https://github.com/grongierisc/interoperability-embedded-python
 Author: grongier
 Author-email: guillaume.rongier@intersystems.com
 License: MIT
 Keywords: iris_pex_embedded_python
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,14 +17,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: dacite>=1.6.0
+Requires-Dist: xmltodict>=0.12.0
+Requires-Dist: irissqlcli
 
 # 1. interoperability-embedded-python
 
 This proof of concept aims to show how the **iris interoperability framework** can be use with **embedded python**.
 
 ## 1.1. Table of Contents
```

### Comparing `iris_pex_embedded_python-2.3.8/src/iris_pex_embedded_python.egg-info/SOURCES.txt` & `iris_pex_embedded_python-2.3.9/src/iris_pex_embedded_python.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 src/grongier/cls/Grongier/PEX/Director.cls
 src/grongier/cls/Grongier/PEX/InboundAdapter.cls
 src/grongier/cls/Grongier/PEX/Message.cls
 src/grongier/cls/Grongier/PEX/OutboundAdapter.cls
 src/grongier/cls/Grongier/PEX/PickleMessage.cls
 src/grongier/cls/Grongier/PEX/Test.cls
 src/grongier/cls/Grongier/PEX/Utils.cls
-src/grongier/cls/Grongier/PEX/WSGI.cls
 src/grongier/cls/Grongier/PEX/Duplex/Operation.cls
 src/grongier/cls/Grongier/PEX/Duplex/Process.cls
 src/grongier/cls/Grongier/PEX/Duplex/Service.cls
 src/grongier/cls/Grongier/PEX/PrivateSession/Duplex.cls
 src/grongier/cls/Grongier/PEX/PrivateSession/Message/Ack.cls
 src/grongier/cls/Grongier/PEX/PrivateSession/Message/Poll.cls
 src/grongier/cls/Grongier/PEX/PrivateSession/Message/Start.cls
 src/grongier/cls/Grongier/PEX/PrivateSession/Message/Stop.cls
+src/grongier/cls/Grongier/Service/WSGI.cls
 src/grongier/pex/__init__.py
 src/grongier/pex/__main__.py
 src/grongier/pex/_business_host.py
 src/grongier/pex/_business_operation.py
 src/grongier/pex/_business_process.py
 src/grongier/pex/_business_service.py
 src/grongier/pex/_cli.py
```

