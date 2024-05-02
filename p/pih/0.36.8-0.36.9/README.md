# Comparing `tmp/pih-0.36.8.tar.gz` & `tmp/pih-0.36.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-0.36.8.tar", last modified: Wed Apr 17 06:02:47 2024, max compression
+gzip compressed data, was "pih-0.36.9.tar", last modified: Wed Apr 17 14:06:34 2024, max compression
```

## Comparing `pih-0.36.8.tar` & `pih-0.36.9.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2024-04-17 06:02:47.363865 pih-0.36.8/
--rw-rw-rw-   0        0        0      249 2024-04-17 06:02:47.285745 pih-0.36.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-17 06:02:45.126439 pih-0.36.8/pih/
--rw-rw-rw-   0        0        0       21 2024-02-19 22:30:08.000000 pih-0.36.8/pih/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:02:45.472782 pih-0.36.8/pih/collections/
--rw-rw-rw-   0        0        0    28524 2024-04-17 05:26:38.000000 pih-0.36.8/pih/collections/__init__.py
--rw-rw-rw-   0        0        0     3051 2024-04-05 09:11:32.000000 pih-0.36.8/pih/collections/service.py
--rw-rw-rw-   0        0        0   104103 2024-04-09 23:48:39.000000 pih-0.36.8/pih/console_api.py
--rw-rw-rw-   0        0        0     1951 2024-03-26 01:01:32.000000 pih-0.36.8/pih/console_api_wrapper.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:02:46.877888 pih-0.36.8/pih/consts/
--rw-rw-rw-   0        0        0    25249 2024-04-17 06:00:46.000000 pih-0.36.8/pih/consts/__init__.py
--rw-rw-rw-   0        0        0     3645 2024-04-09 23:35:29.000000 pih-0.36.8/pih/consts/ad.py
--rw-rw-rw-   0        0        0     1623 2024-04-09 23:36:40.000000 pih-0.36.8/pih/consts/addresses.py
--rw-rw-rw-   0        0        0      893 2024-02-29 00:30:59.000000 pih-0.36.8/pih/consts/date_time.py
--rw-rw-rw-   0        0        0      145 2024-03-06 05:57:31.000000 pih-0.36.8/pih/consts/document.py
--rw-rw-rw-   0        0        0      936 2024-02-24 11:05:43.000000 pih-0.36.8/pih/consts/errors.py
--rw-rw-rw-   0        0        0    30004 2024-04-15 23:46:38.000000 pih-0.36.8/pih/consts/events.py
--rw-rw-rw-   0        0        0      494 2024-03-08 07:55:52.000000 pih-0.36.8/pih/consts/facade.py
--rw-rw-rw-   0        0        0      439 2024-03-28 06:36:09.000000 pih-0.36.8/pih/consts/file.py
--rw-rw-rw-   0        0        0     1347 2024-02-14 12:47:46.000000 pih-0.36.8/pih/consts/hosts.py
--rw-rw-rw-   0        0        0      187 2024-04-17 05:22:16.000000 pih-0.36.8/pih/consts/iot.py
--rw-rw-rw-   0        0        0    19521 2024-02-29 09:16:45.000000 pih-0.36.8/pih/consts/names.py
--rw-rw-rw-   0        0        0     1148 2024-02-09 14:42:12.000000 pih-0.36.8/pih/consts/password.py
--rw-rw-rw-   0        0        0    11944 2024-04-10 22:09:05.000000 pih-0.36.8/pih/consts/paths.py
--rw-rw-rw-   0        0        0    11122 2024-04-16 01:31:15.000000 pih-0.36.8/pih/consts/polibase.py
--rw-rw-rw-   0        0        0      494 2024-03-28 06:45:52.000000 pih-0.36.8/pih/consts/python.py
--rw-rw-rw-   0        0        0       62 2024-02-16 12:50:10.000000 pih-0.36.8/pih/consts/recognize.py
--rw-rw-rw-   0        0        0      329 2024-02-09 16:21:36.000000 pih-0.36.8/pih/consts/rpc.py
--rw-rw-rw-   0        0        0     1020 2024-04-05 09:11:55.000000 pih-0.36.8/pih/consts/service.py
--rw-rw-rw-   0        0        0     6540 2024-04-17 04:46:50.000000 pih-0.36.8/pih/consts/service_commands.py
--rw-rw-rw-   0        0        0    12225 2024-04-17 04:51:50.000000 pih-0.36.8/pih/consts/service_roles.py
--rw-rw-rw-   0        0        0    13173 2024-04-05 02:55:38.000000 pih-0.36.8/pih/consts/settings.py
--rw-rw-rw-   0        0        0      291 2024-02-23 12:19:53.000000 pih-0.36.8/pih/consts/ssh_hosts.py
--rw-rw-rw-   0        0        0      216 2024-03-26 23:33:29.000000 pih-0.36.8/pih/consts/zabbix.py
--rw-rw-rw-   0        0        0   549799 2024-04-17 05:31:22.000000 pih-0.36.8/pih/pih.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:02:47.065757 pih-0.36.8/pih/rpc/
--rw-rw-rw-   0        0        0    34058 2024-04-09 12:59:11.000000 pih-0.36.8/pih/rpc/__init__.py
--rw-rw-rw-   0        0        0     1941 2023-08-11 06:40:35.000000 pih-0.36.8/pih/rpc/rpcCommandCall_pb2.py
--rw-rw-rw-   0        0        0     2469 2024-02-09 15:23:51.000000 pih-0.36.8/pih/rpc/rpcCommandCall_pb2_grpc.py
--rw-rw-rw-   0        0        0      485 2024-02-09 14:42:12.000000 pih-0.36.8/pih/service_example.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:02:47.206371 pih-0.36.8/pih/tools/
--rw-rw-rw-   0        0        0    51621 2024-04-16 02:10:50.000000 pih-0.36.8/pih/tools/__init__.py
--rw-rw-rw-   0        0        0     3851 2024-04-09 23:31:04.000000 pih-0.36.8/pih/tools/service.py
--rw-rw-rw-   0        0        0     2244 2024-02-10 10:21:19.000000 pih-0.36.8/pih/widgets.py
-drwxrwxrwx   0        0        0        0 2024-04-17 06:02:47.254478 pih-0.36.8/pih.egg-info/
--rw-rw-rw-   0        0        0      249 2024-04-17 06:02:44.000000 pih-0.36.8/pih.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      956 2024-04-17 06:02:44.000000 pih-0.36.8/pih.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-17 06:02:44.000000 pih-0.36.8/pih.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-17 06:02:44.000000 pih-0.36.8/pih.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-17 06:02:44.000000 pih-0.36.8/pih.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-17 06:02:47.363865 pih-0.36.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-17 14:06:34.243077 pih-0.36.9/
+-rw-rw-rw-   0        0        0      249 2024-04-17 14:06:34.196313 pih-0.36.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-17 14:06:32.211168 pih-0.36.9/pih/
+-rw-rw-rw-   0        0        0       21 2024-02-19 22:30:08.000000 pih-0.36.9/pih/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-17 14:06:32.514860 pih-0.36.9/pih/collections/
+-rw-rw-rw-   0        0        0    28524 2024-04-17 05:26:38.000000 pih-0.36.9/pih/collections/__init__.py
+-rw-rw-rw-   0        0        0     3051 2024-04-05 09:11:32.000000 pih-0.36.9/pih/collections/service.py
+-rw-rw-rw-   0        0        0   104103 2024-04-09 23:48:39.000000 pih-0.36.9/pih/console_api.py
+-rw-rw-rw-   0        0        0     1951 2024-03-26 01:01:32.000000 pih-0.36.9/pih/console_api_wrapper.py
+drwxrwxrwx   0        0        0        0 2024-04-17 14:06:33.819127 pih-0.36.9/pih/consts/
+-rw-rw-rw-   0        0        0    25249 2024-04-17 14:05:45.000000 pih-0.36.9/pih/consts/__init__.py
+-rw-rw-rw-   0        0        0     3645 2024-04-09 23:35:29.000000 pih-0.36.9/pih/consts/ad.py
+-rw-rw-rw-   0        0        0     1623 2024-04-09 23:36:40.000000 pih-0.36.9/pih/consts/addresses.py
+-rw-rw-rw-   0        0        0      893 2024-02-29 00:30:59.000000 pih-0.36.9/pih/consts/date_time.py
+-rw-rw-rw-   0        0        0      145 2024-03-06 05:57:31.000000 pih-0.36.9/pih/consts/document.py
+-rw-rw-rw-   0        0        0      936 2024-02-24 11:05:43.000000 pih-0.36.9/pih/consts/errors.py
+-rw-rw-rw-   0        0        0    30004 2024-04-15 23:46:38.000000 pih-0.36.9/pih/consts/events.py
+-rw-rw-rw-   0        0        0      494 2024-03-08 07:55:52.000000 pih-0.36.9/pih/consts/facade.py
+-rw-rw-rw-   0        0        0      439 2024-03-28 06:36:09.000000 pih-0.36.9/pih/consts/file.py
+-rw-rw-rw-   0        0        0     1347 2024-02-14 12:47:46.000000 pih-0.36.9/pih/consts/hosts.py
+-rw-rw-rw-   0        0        0      187 2024-04-17 05:22:16.000000 pih-0.36.9/pih/consts/iot.py
+-rw-rw-rw-   0        0        0    19521 2024-02-29 09:16:45.000000 pih-0.36.9/pih/consts/names.py
+-rw-rw-rw-   0        0        0     1148 2024-02-09 14:42:12.000000 pih-0.36.9/pih/consts/password.py
+-rw-rw-rw-   0        0        0    11944 2024-04-10 22:09:05.000000 pih-0.36.9/pih/consts/paths.py
+-rw-rw-rw-   0        0        0    11122 2024-04-16 01:31:15.000000 pih-0.36.9/pih/consts/polibase.py
+-rw-rw-rw-   0        0        0      494 2024-03-28 06:45:52.000000 pih-0.36.9/pih/consts/python.py
+-rw-rw-rw-   0        0        0       62 2024-02-16 12:50:10.000000 pih-0.36.9/pih/consts/recognize.py
+-rw-rw-rw-   0        0        0      329 2024-02-09 16:21:36.000000 pih-0.36.9/pih/consts/rpc.py
+-rw-rw-rw-   0        0        0     1020 2024-04-05 09:11:55.000000 pih-0.36.9/pih/consts/service.py
+-rw-rw-rw-   0        0        0     6540 2024-04-17 04:46:50.000000 pih-0.36.9/pih/consts/service_commands.py
+-rw-rw-rw-   0        0        0    12239 2024-04-17 13:50:24.000000 pih-0.36.9/pih/consts/service_roles.py
+-rw-rw-rw-   0        0        0    13173 2024-04-05 02:55:38.000000 pih-0.36.9/pih/consts/settings.py
+-rw-rw-rw-   0        0        0      291 2024-02-23 12:19:53.000000 pih-0.36.9/pih/consts/ssh_hosts.py
+-rw-rw-rw-   0        0        0      216 2024-03-26 23:33:29.000000 pih-0.36.9/pih/consts/zabbix.py
+-rw-rw-rw-   0        0        0   549782 2024-04-17 12:36:18.000000 pih-0.36.9/pih/pih.py
+drwxrwxrwx   0        0        0        0 2024-04-17 14:06:33.993085 pih-0.36.9/pih/rpc/
+-rw-rw-rw-   0        0        0    34058 2024-04-09 12:59:11.000000 pih-0.36.9/pih/rpc/__init__.py
+-rw-rw-rw-   0        0        0     1941 2023-08-11 06:40:35.000000 pih-0.36.9/pih/rpc/rpcCommandCall_pb2.py
+-rw-rw-rw-   0        0        0     2469 2024-02-09 15:23:51.000000 pih-0.36.9/pih/rpc/rpcCommandCall_pb2_grpc.py
+-rw-rw-rw-   0        0        0      485 2024-02-09 14:42:12.000000 pih-0.36.9/pih/service_example.py
+drwxrwxrwx   0        0        0        0 2024-04-17 14:06:34.102456 pih-0.36.9/pih/tools/
+-rw-rw-rw-   0        0        0    51621 2024-04-16 02:10:50.000000 pih-0.36.9/pih/tools/__init__.py
+-rw-rw-rw-   0        0        0     3851 2024-04-09 23:31:04.000000 pih-0.36.9/pih/tools/service.py
+-rw-rw-rw-   0        0        0     2244 2024-02-10 10:21:19.000000 pih-0.36.9/pih/widgets.py
+drwxrwxrwx   0        0        0        0 2024-04-17 14:06:34.164949 pih-0.36.9/pih.egg-info/
+-rw-rw-rw-   0        0        0      249 2024-04-17 14:06:31.000000 pih-0.36.9/pih.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      956 2024-04-17 14:06:31.000000 pih-0.36.9/pih.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-17 14:06:31.000000 pih-0.36.9/pih.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-17 14:06:31.000000 pih-0.36.9/pih.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-17 14:06:31.000000 pih-0.36.9/pih.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-17 14:06:34.243077 pih-0.36.9/setup.cfg
```

### Comparing `pih-0.36.8/pih/collections/__init__.py` & `pih-0.36.9/pih/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.8/pih/collections/service.py` & `pih-0.36.9/pih/collections/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.8/pih/console_api.py` & `pih-0.36.9/pih/console_api.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.8/pih/console_api_wrapper.py` & `pih-0.36.9/pih/console_api_wrapper.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.8/pih/consts/__init__.py` & `pih-0.36.9/pih/consts/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     OrderedNameCaptionDescription,
     IconedOrderedNameCaptionDescription,
 )
 from pih.consts.password import *
 from pih.consts.date_time import *
 from pih.consts.service_commands import *
 
-VERSION: str = "0.36.8"
+VERSION: str = "0.36.9"
 
 class DATA:
     # deprecated
     class EXTRACTOR:
         USER_NAME_FULL: str = "user_name_full"
         USER_NAME: str = "user_name"
         AS_IS: str = "as_is"
```

### Comparing `pih-0.36.8/pih/consts/ad.py` & `pih-0.36.9/pih/consts/ad.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.8/pih/consts/addresses.py` & `pih-0.36.9/pih/consts/addresses.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.8/pih/consts/date_time.py` & `pih-0.36.9/pih/consts/date_time.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.8/pih/consts/errors.py` & `pih-0.36.9/pih/consts/errors.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.8/pih/consts/events.py` & `pih-0.36.9/pih/consts/events.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.8/pih/consts/hosts.py` & `pih-0.36.9/pih/consts/hosts.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.8/pih/consts/names.py` & `pih-0.36.9/pih/consts/names.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.8/pih/consts/password.py` & `pih-0.36.9/pih/consts/password.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.8/pih/consts/paths.py` & `pih-0.36.9/pih/consts/paths.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.8/pih/consts/polibase.py` & `pih-0.36.9/pih/consts/polibase.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.8/pih/consts/service.py` & `pih-0.36.9/pih/consts/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.8/pih/consts/service_commands.py` & `pih-0.36.9/pih/consts/service_commands.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.8/pih/consts/service_roles.py` & `pih-0.36.9/pih/consts/service_roles.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,16 +260,16 @@
     )
     
     
     ZABBIX = ServiceDescription(
         name="Zabbix",
     )
     
-    IOT = ServiceDescription(
-        name="iot",
+    IOTDevices = ServiceDescription(
+        name="IOTDevices",
     )
 
     POLIBASE_DATABASE = ServiceDescription(
         name="PolibaseDatabase",
         commands=(ServiceCommands.create_polibase_database_backup,),
     )
```

### Comparing `pih-0.36.8/pih/consts/settings.py` & `pih-0.36.9/pih/consts/settings.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.8/pih/pih.py` & `pih-0.36.9/pih/pih.py`

 * *Files 0% similar despite different names*

```diff
@@ -3002,15 +3002,15 @@
                     )
                 else:
                     complete_process: CompletedProcess = PIH.EXECUTOR.execute(
                         (
                             command_list
                             if host_is_local
                             else PIH.EXECUTOR.create_command_for_psexec(
-                                command_list, host, interactive=show_output
+                                command_list, host, interactive=True
                             )
                         ),
                         show_output,
                     )
                     result = PIH.DATA.CHECK.returncode(complete_process)
                 CACHE[cache_name] = result
             return CACHE[cache_name]
@@ -3254,26 +3254,29 @@
                         return lost_count == 0
                     return lost_count < count
             return False
 
         @staticmethod
         @cache
         def python_version(host: str | None = None) -> str | None:
+            def parse_version(value: str) -> str:
+                return j(value.strip().split(" ")[1:])
+
             if PIH.SYS.host_is_local(host):
                 return sys.version.split(" ")[0]
             result: str | None = None
             host_is_linux: bool = PIH.SYS.is_linux(host)
             if host_is_linux:
                 result = one(
                     PIH.RESULT.SSH.execute(
                         js((PYTHON.EXECUTOR3, PYTHON.COMMAND.VERSION)), host
                     ).data
                 )
             else:
-                result_list: list[str | None] = []
+                # result_list: list[str | None] = []
                 for executor_name in (
                     PYTHON.EXECUTOR_ALIAS,
                     PYTHON.EXECUTOR,
                 ):
                     command: tuple[str, ...] = (
                         executor_name,
                         PYTHON.COMMAND.VERSION,
@@ -3284,20 +3287,19 @@
                         ),
                         True,
                         True,
                     )
                     stderr: str = complete_process.stderr
                     if ne(stderr):
                         if stderr.find(js(("could not start", executor_name))) != -1:
-                            result_list.append(None)
-                    result_list.append(str(complete_process.stdout))
-                result = one(DataTool.filter(ne, result_list))
-                if n(result):
-                    return None
-            return j(result.strip().split(" ")[1:])
+                            continue
+                    result = str(complete_process.stdout)
+                    if nn(result):
+                        return parse_version(result)
+            return None
 
         @staticmethod
         def get_disk_statistics_list(host: str) -> list[DiskStatistics]:
             output: str = PIH.EXECUTOR.execute(
                 js(
                     (
                         CONST.POWERSHELL.NAME,
@@ -7944,30 +7946,32 @@
         @staticmethod
         def kill_process_by_port(
             value: int,
         ) -> bool | None:
             return PIH.EXECUTOR.kill_process_by_port(value)
 
     class RESULT(ResultTool):
-        
+
         class IOTDevices:
 
             @staticmethod
-            def _call(command: IOT.Commands, parameters: tuple[Any, ...] | None = None) -> bool:
+            def _call(
+                command: IOT.Commands, parameters: tuple[Any, ...] | None = None
+            ) -> bool:
                 return PIH.SERVICE.call_command_for_service(
                     ServiceRoles.IOT,
                     ServiceCommands.serve_command,
                     (command.name, *(parameters or ())),
                 )
-                
+
             @staticmethod
             def devices() -> Result[list[IOTDevice]]:
                 return DataTool.to_result(
                     PIH.RESULT.IOTDevices._call(IOT.Commands.device_list), IOTDevice
-                ) 
+                )
 
         class ZABBIX:
 
             @staticmethod
             def _call(
                 command: ZABBIX.Commands, parameters: tuple[Any, ...] | None = None
             ) -> str | None:
@@ -12928,15 +12932,14 @@
             @staticmethod
             def start_windows_service(name: str, computer_name: str) -> bool | None:
                 return PIH.EXECUTOR.start_windows_service(name, computer_name)
 
             @staticmethod
             def stop_windows_service(name: str, computer_name: str) -> bool | None:
                 return PIH.EXECUTOR.stop_windows_service(name, computer_name)
-            
 
         class DOOR:
 
             @staticmethod
             def _command(name: str, operation_name: str) -> bool:
                 return DataTool.rpc_decode(
                     PIH.SERVICE.call_command(
@@ -13217,15 +13220,15 @@
     R_F = R.FILES
     R_TT = R.TIME_TRACKING
     R_P = R.POLIBASE
     R_PR = R.PRINTER
     R_SRVS = R.SERVER
     R_EM = R.EMAIL
     R_IOT = R.IOTDevices
-    
+
     D = root.DATA
     D_V = D.VARIABLE
     D_V_T = D_V.TIMESTAMP
     D_V_T_E = D_V_T.EXPIRED
     D_V_E = D_V.ENVIRONMENT
     D_TN = D.TELEPHONE_NUMBER
     D_MR = D.MATERIALIZED_RESOURCES
@@ -13309,43 +13312,43 @@
     D_CO = D.CONVERT
     A_P = A.POLIBASE
     A_INV = A.INVENTORY
     C_E = C.EVENTS
     C_P = C.POLIBASE
     C_P_DB = C_P.DATABASE
     D_P = D.POLIBASE
-   
+
     R_IND_D = R_IND.DEVICE
     #
     A_Z = A.ZABBIX
     A_PTH = A.PATH
     A_P_V = A_P.VISIT
     A_P_V_DS = A_P_V.DATA_STORAGE
     R_P_V = R_P.VISIT
     R_P_V_DS = R_P_V.DATA_STORAGE
     A_P_N = A_P.NOTIFICATION
     A_P_N_C = A_P_N.CONFIRMATION
     R_P_N = R_P.NOTIFICATION
     R_P_N_C = R_P_N.CONFIRMATION
     C_P_N = C_P.NOTIFICATION
     C_P_N_С = C_P_N.CONFIRMATION
-   
+
     C_WS = C.WORKSTATION
     A_P_IQ = A_P.INFORMATION_QUEST
     R_P_IQ = R_P.INFORMATION_QUEST
     SRV = root.SERVICE
     SRV_A = SRV.ADMIN
     I = root.input
     I_U = I.user
     A_B = A.BACKUP
 
     O = root.output
     SE = root.session
     A_DS = A.DATA_STORAGE
-    
+
     V = root.VERSION
     SYS = root.SYS
     U = root.UPDATER
     EXC = root.EXECUTOR
     ER = root.ERROR
     E = root.EVENT
     E_B = E.BUILDER
@@ -13358,15 +13361,14 @@
     PTH_QR = PTH.QR_CODE
     PTH_FNT = PTH.FONTS
     PTH_IND = PTH.INDICATIONS
     PTH_MIO = PTH.MOBILE_HELPER
     PTH_FCD = PTH.FACADE
     PTH_FCD_DIST = PTH_FCD.DITRIBUTIVE
     L = root.LOG
- 
 
     CT = CONST
     CT_FACADE = FACADE
     CT_PY = PYTHON
     CT_PORT = CONST.PORT
     CT_CMDT = CommandTypes
     CT_LNK = LINK
@@ -13417,15 +13419,14 @@
     CT_I = INDICATIONS
     CT_T = Tags
     CT_CR = CT.CARD_REGISTRY
     C_P_DB = C_P.DATABASE
     CT_PI = PARAM_ITEMS
 
     D_P = D.POLIBASE
-  
 
     CR = root.CARD_REGISTRY
     #
 
     C_V_T_E = D_C.VARIABLE.TIMESTAMP.EXPIRED
```

### Comparing `pih-0.36.8/pih/rpc/__init__.py` & `pih-0.36.9/pih/rpc/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.8/pih/rpc/rpcCommandCall_pb2.py` & `pih-0.36.9/pih/rpc/rpcCommandCall_pb2.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.8/pih/rpc/rpcCommandCall_pb2_grpc.py` & `pih-0.36.9/pih/rpc/rpcCommandCall_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.8/pih/tools/__init__.py` & `pih-0.36.9/pih/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.8/pih/tools/service.py` & `pih-0.36.9/pih/tools/service.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.8/pih/widgets.py` & `pih-0.36.9/pih/widgets.py`

 * *Files identical despite different names*

### Comparing `pih-0.36.8/pih.egg-info/SOURCES.txt` & `pih-0.36.9/pih.egg-info/SOURCES.txt`

 * *Files identical despite different names*

