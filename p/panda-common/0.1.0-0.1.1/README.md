# Comparing `tmp/panda_common-0.1.0.tar.gz` & `tmp/panda_common-0.1.1.tar.gz`

## Comparing `panda_common-0.1.0.tar` & `panda_common-0.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 panda_common-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 panda_common-0.1.0/ChangeLog.txt
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 panda_common-0.1.0/INSTALL.txt
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 panda_common-0.1.0/MANIFEST.in
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 panda_common-0.1.0/PandaPkgInfo.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 panda_common-0.1.0/package/hatch_build.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_common-0.1.0/pandacommon/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_common-0.1.0/pandacommon/commonconfig/__init__.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 panda_common-0.1.0/pandacommon/commonconfig/common_config.py
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 panda_common-0.1.0/pandacommon/kafkapublisher/KafkaPublisher.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_common-0.1.0/pandacommon/kafkapublisher/__init__.py
--rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 panda_common-0.1.0/pandacommon/liveconfigparser/LiveConfigParser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_common-0.1.0/pandacommon/liveconfigparser/__init__.py
--rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 panda_common-0.1.0/pandacommon/pandalogger/LogWrapper.py
--rwxr-xr-x   0        0        0    12064 2020-02-02 00:00:00.000000 panda_common-0.1.0/pandacommon/pandalogger/PandaLogger.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_common-0.1.0/pandacommon/pandalogger/__init__.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 panda_common-0.1.0/pandacommon/pandalogger/logger_config.py
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 panda_common-0.1.0/pandacommon/pandalogger/logger_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_common-0.1.0/pandacommon/pandamsgbkr/__init__.py
--rw-r--r--   0        0        0    29757 2020-02-02 00:00:00.000000 panda_common-0.1.0/pandacommon/pandamsgbkr/msg_bkr_utils.py
--rw-r--r--   0        0        0    27263 2020-02-02 00:00:00.000000 panda_common-0.1.0/pandacommon/pandamsgbkr/msg_processor.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 panda_common-0.1.0/pandacommon/pandautils/ConfigUtils.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 panda_common-0.1.0/pandacommon/pandautils/PandaUtils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_common-0.1.0/pandacommon/pandautils/__init__.py
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 panda_common-0.1.0/pandacommon/pandautils/net_utils.py
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 panda_common-0.1.0/pandacommon/pandautils/plugin_factory.py
--rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 panda_common-0.1.0/pandacommon/pandautils/thread_utils.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 panda_common-0.1.0/pandacommon/pandautils/utils_config.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_common-0.1.0/pandacommon/test/__init__.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 panda_common-0.1.0/pandacommon/test/logtest.py
--rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 panda_common-0.1.0/pandacommon/test/mb_test.py
--rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 panda_common-0.1.0/templates/conda_meta.yaml.template
--rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 panda_common-0.1.0/templates/panda_common.cfg.rpmnew
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 panda_common-0.1.0/tools/panda_common-install_igtf_ca
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 panda_common-0.1.0/LICENSE
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 panda_common-0.1.0/README.md
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 panda_common-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 panda_common-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 panda_common-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2361 2020-02-02 00:00:00.000000 panda_common-0.1.1/ChangeLog.txt
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 panda_common-0.1.1/INSTALL.txt
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 panda_common-0.1.1/MANIFEST.in
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 panda_common-0.1.1/PandaPkgInfo.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 panda_common-0.1.1/package/hatch_build.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_common-0.1.1/pandacommon/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_common-0.1.1/pandacommon/commonconfig/__init__.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 panda_common-0.1.1/pandacommon/commonconfig/common_config.py
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 panda_common-0.1.1/pandacommon/kafkapublisher/KafkaPublisher.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_common-0.1.1/pandacommon/kafkapublisher/__init__.py
+-rw-r--r--   0        0        0     2988 2020-02-02 00:00:00.000000 panda_common-0.1.1/pandacommon/liveconfigparser/LiveConfigParser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_common-0.1.1/pandacommon/liveconfigparser/__init__.py
+-rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 panda_common-0.1.1/pandacommon/pandalogger/LogWrapper.py
+-rwxr-xr-x   0        0        0    12064 2020-02-02 00:00:00.000000 panda_common-0.1.1/pandacommon/pandalogger/PandaLogger.py
+-rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 panda_common-0.1.1/pandacommon/pandalogger/__init__.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 panda_common-0.1.1/pandacommon/pandalogger/logger_config.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 panda_common-0.1.1/pandacommon/pandalogger/logger_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_common-0.1.1/pandacommon/pandamsgbkr/__init__.py
+-rw-r--r--   0        0        0    29757 2020-02-02 00:00:00.000000 panda_common-0.1.1/pandacommon/pandamsgbkr/msg_bkr_utils.py
+-rw-r--r--   0        0        0    27295 2020-02-02 00:00:00.000000 panda_common-0.1.1/pandacommon/pandamsgbkr/msg_processor.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 panda_common-0.1.1/pandacommon/pandautils/ConfigUtils.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 panda_common-0.1.1/pandacommon/pandautils/PandaUtils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_common-0.1.1/pandacommon/pandautils/__init__.py
+-rw-r--r--   0        0        0     3697 2020-02-02 00:00:00.000000 panda_common-0.1.1/pandacommon/pandautils/net_utils.py
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 panda_common-0.1.1/pandacommon/pandautils/plugin_factory.py
+-rw-r--r--   0        0        0     5364 2020-02-02 00:00:00.000000 panda_common-0.1.1/pandacommon/pandautils/thread_utils.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 panda_common-0.1.1/pandacommon/pandautils/utils_config.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panda_common-0.1.1/pandacommon/test/__init__.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 panda_common-0.1.1/pandacommon/test/logtest.py
+-rw-r--r--   0        0        0     6691 2020-02-02 00:00:00.000000 panda_common-0.1.1/pandacommon/test/mb_test.py
+-rw-r--r--   0        0        0      633 2020-02-02 00:00:00.000000 panda_common-0.1.1/templates/conda_meta.yaml.template
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 panda_common-0.1.1/templates/panda_common.cfg.rpmnew
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 panda_common-0.1.1/tools/panda_common-install_igtf_ca
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 panda_common-0.1.1/LICENSE
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 panda_common-0.1.1/README.md
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 panda_common-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 panda_common-0.1.1/PKG-INFO
```

### Comparing `panda_common-0.1.0/ChangeLog.txt` & `panda_common-0.1.1/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `panda_common-0.1.0/pandacommon/kafkapublisher/KafkaPublisher.py` & `panda_common-0.1.1/pandacommon/kafkapublisher/KafkaPublisher.py`

 * *Files identical despite different names*

### Comparing `panda_common-0.1.0/pandacommon/liveconfigparser/LiveConfigParser.py` & `panda_common-0.1.1/pandacommon/liveconfigparser/LiveConfigParser.py`

 * *Files identical despite different names*

### Comparing `panda_common-0.1.0/pandacommon/pandalogger/LogWrapper.py` & `panda_common-0.1.1/pandacommon/pandalogger/LogWrapper.py`

 * *Files identical despite different names*

### Comparing `panda_common-0.1.0/pandacommon/pandalogger/PandaLogger.py` & `panda_common-0.1.1/pandacommon/pandalogger/PandaLogger.py`

 * *Files identical despite different names*

### Comparing `panda_common-0.1.0/pandacommon/pandalogger/logger_utils.py` & `panda_common-0.1.1/pandacommon/pandalogger/logger_utils.py`

 * *Files identical despite different names*

### Comparing `panda_common-0.1.0/pandacommon/pandamsgbkr/msg_bkr_utils.py` & `panda_common-0.1.1/pandacommon/pandamsgbkr/msg_bkr_utils.py`

 * *Files identical despite different names*

### Comparing `panda_common-0.1.0/pandacommon/pandamsgbkr/msg_processor.py` & `panda_common-0.1.1/pandacommon/pandamsgbkr/msg_processor.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         send_heartbeat_ms=sconf.get("send_heartbeat_ms", 60000),
         recv_heartbeat_ms=sconf.get("recv_heartbeat_ms", 0),
         wait=True,
         ack_mode=qconf.get("ack_mode", "client-individual"),
         max_buffer_len=qconf.get("max_buffer_len", 999),
         buffer_block_sec=qconf.get("buffer_block_sec", 10),
         use_transaction=qconf.get("use_transaction", True),
-        verbose=sconf.get("verbose", False),
+        verbose=sconf.get("verbose", False) or qconf.get("verbose", False),
         **kwargs
     )
     return mb_proxy
 
 
 # simple message processor plugin Base
 class SimpleMsgProcPluginBase:
@@ -260,35 +260,35 @@
                     'host_port_list': ['192.168.0.1:777', '192.168.0.2:777'],
                     'use_ssl': True,
                     'cert_file': 'aaa.cert.pem',
                     'key_file': 'bbb.key.pem',
                     'username': 'someuser',
                     'passcode': 'xxxxyyyyzzzz',
                     'vhost': '/somehost',
-                    'verbose': True,
+                    'verbose': False,
                 },
                 ...
             }
         queues_dict = {
                 'Queue_1': {
                     'enable': True,
                     'server': 'Server_1',
                     'destination': '/queue/some_queue',
+                    'verbose': True,
                 },
                 ...
             }
         processors_dict = {
                 'Processor_1': {
                     'enable': True,
                     'module': 'plugin.module',
                     'name': 'PluginClassName',
                     'n_threads': 1,
                     'in_queue': 'Queue_1',
                     'out_queue': 'Queue_2',
-                    'verbose': True,
                 },
                 ...
             }
         """
         # logger
         tmp_logger = logger_utils.make_logger(base_logger, token=self.get_pid(), method_name="_parse_config")
         tmp_logger.debug("start")
```

### Comparing `panda_common-0.1.0/pandacommon/pandautils/ConfigUtils.py` & `panda_common-0.1.1/pandacommon/pandautils/ConfigUtils.py`

 * *Files identical despite different names*

### Comparing `panda_common-0.1.0/pandacommon/pandautils/PandaUtils.py` & `panda_common-0.1.1/pandacommon/pandautils/PandaUtils.py`

 * *Files identical despite different names*

### Comparing `panda_common-0.1.0/pandacommon/pandautils/net_utils.py` & `panda_common-0.1.1/pandacommon/pandautils/net_utils.py`

 * *Files 25% similar despite different names*

```diff
@@ -18,55 +18,100 @@
 dnsMap = MapWithLockAndTimeout()
 
 
 # HTTP adaptor with randomized DNS resolution
 class HTTPAdapterWithRandomDnsResolver(HTTPAdapter):
     # override to get connection to random host
     def get_connection(self, url, proxies=None):
+        # resolve cname to hostnames
+        dns_records = resolve_host_in_url(url)
+        random.shuffle(dns_records)
         # parse URL
         parsed = urlparse(url)
-        host = parsed.hostname
-        port = parsed.port
-        if port is None:
-            if parsed.scheme == "http":
-                port = 80
-            else:
-                port = 443
-        # check record
-        if parsed.hostname in dnsMap:
-            dns_records = dnsMap[parsed.hostname]
-        else:
-            family = allowed_gai_family()
-            dns_records = socket.getaddrinfo(host, port, family, socket.SOCK_STREAM)
-            dns_records = list(set([socket.getfqdn(record[4][0]) for record in dns_records]))
-            dnsMap[parsed.hostname] = dns_records
-        dns_records = copy.copy(dns_records)
-        random.shuffle(dns_records)
         # loop over all hosts
         err = None
         for hostname in dns_records:
-            addr = hostname
-            if parsed.port is not None:
-                addr += ":{0}".format(parsed.port)
-            tmp_url = parsed._replace(netloc=addr).geturl()
+            tmp_url = replace_hostname_in_url(url, hostname)
             try:
                 con = HTTPAdapter.get_connection(self, tmp_url, proxies=proxies)
                 # return if valid
                 if con is not None:
                     return con
             except Exception as e:
                 err = e
         if err is not None:
             raise err
         return None
 
 
-# utility function to get HTTPAdapterWithRandomDnsResolver
-def get_http_adapter_with_random_dns_resolution():
+# utility function to get a session object with HTTPAdapterWithRandomDnsResolver
+def get_http_adapter_with_random_dns_resolution() -> requests.Session:
+    """
+    Utility function to get a session object with custom HTTPAdapter which resolves host in URL randomly to distribute access to DNS load balanced HTTP services
+    :return: session object
+    """
     session = requests.Session()
     # no randomization if panda is behind real load balancer than DNS LB
     if "PANDA_BEHIND_REAL_LB" in os.environ:
         return session
     adapter = HTTPAdapterWithRandomDnsResolver(max_retries=0)
     session.mount("http://", adapter)
     session.mount("https://", adapter)
     return session
+
+
+# resolve a host in a given URL to hostnames
+def resolve_host_in_url(url: str) -> list[str]:
+    """
+    Resolve a host in a given URL to hostnames
+    :param url: URL
+    :return: list of hostnames
+    """
+    # parse URL
+    parsed = urlparse(url)
+    host = parsed.hostname
+    port = parsed.port
+    if port is None:
+        if parsed.scheme == "http":
+            port = 80
+        else:
+            port = 443
+    # check record
+    if parsed.hostname in dnsMap:
+        dns_records = dnsMap[parsed.hostname]
+    else:
+        family = allowed_gai_family()
+        dns_records = socket.getaddrinfo(host, port, family, socket.SOCK_STREAM)
+        dns_records = list(set([socket.getfqdn(record[4][0]) for record in dns_records]))
+        dnsMap[parsed.hostname] = dns_records
+    return copy.copy(dns_records)
+
+
+# replace hostname in URL
+def replace_hostname_in_url(url: str, new_host: str) -> str:
+    """
+    Replace hostname in URL
+    :param url: original URL
+    :param new_host: new hostname
+    :return: new URL with replaced hostname
+    """
+    parsed = urlparse(url)
+    if parsed.port is not None:
+        new_host += f":{parsed.port}"
+    return parsed._replace(netloc=new_host).geturl()
+
+
+# replace hostname in URL randomly
+def replace_hostname_in_url_randomly(url: str) -> str:
+    """
+    Replace hostname in URL randomly
+    :param url: original URL
+    :return: new URL with new hostname randomly chosen from resolved hostnames
+    """
+    # no replacement if panda is behind real load balancer than DNS LB
+    if "PANDA_BEHIND_REAL_LB" in os.environ:
+        return url
+    # resolve cname to hostnames
+    dns_records = resolve_host_in_url(url)
+    # choose one IP randomly
+    random.shuffle(dns_records)
+    return replace_hostname_in_url(url, dns_records[0])
```

### Comparing `panda_common-0.1.0/pandacommon/pandautils/plugin_factory.py` & `panda_common-0.1.1/pandacommon/pandautils/plugin_factory.py`

 * *Files identical despite different names*

### Comparing `panda_common-0.1.0/pandacommon/pandautils/thread_utils.py` & `panda_common-0.1.1/pandacommon/pandautils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `panda_common-0.1.0/pandacommon/test/mb_test.py` & `panda_common-0.1.1/pandacommon/test/mb_test.py`

 * *Files identical despite different names*

### Comparing `panda_common-0.1.0/templates/conda_meta.yaml.template` & `panda_common-0.1.1/templates/conda_meta.yaml.template`

 * *Files identical despite different names*

### Comparing `panda_common-0.1.0/templates/panda_common.cfg.rpmnew` & `panda_common-0.1.1/templates/panda_common.cfg.rpmnew`

 * *Files identical despite different names*

### Comparing `panda_common-0.1.0/LICENSE` & `panda_common-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `panda_common-0.1.0/pyproject.toml` & `panda_common-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `panda_common-0.1.0/PKG-INFO` & `panda_common-0.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: panda-common
-Version: 0.1.0
+Version: 0.1.1
 Summary:  PanDA Common Package
 Project-URL: Homepage, https://panda-wms.readthedocs.io/en/latest/
 Author-email: PanDA Team <panda-support@cern.ch>
 License: Apache-2.0
 License-File: LICENSE
 Requires-Python: >=3.8
 Requires-Dist: configparser
```

