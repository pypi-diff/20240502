# Comparing `tmp/cicflowmeter-0.1.9.tar.gz` & `tmp/cicflowmeter-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cicflowmeter-0.1.9.tar", max compression
+gzip compressed data, was "cicflowmeter-0.2.0.tar", max compression
```

## Comparing `cicflowmeter-0.1.9.tar` & `cicflowmeter-0.2.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1064 2023-12-06 10:59:39.876738 cicflowmeter-0.1.9/LICENSE
--rw-r--r--   0        0        0     1104 2024-02-04 13:45:23.393478 cicflowmeter-0.1.9/README.md
--rw-r--r--   0        0        0      609 2024-02-23 03:24:05.840952 cicflowmeter-0.1.9/pyproject.toml
--rw-r--r--   0        0        0        0 2023-12-07 04:42:03.793231 cicflowmeter-0.1.9/src/cicflowmeter/__init__.py
--rw-r--r--   0        0        0      112 2024-02-04 06:23:29.105905 cicflowmeter-0.1.9/src/cicflowmeter/constants.py
--rw-r--r--   0        0        0        0 2023-12-06 10:59:39.876738 cicflowmeter-0.1.9/src/cicflowmeter/features/__init__.py
--rw-r--r--   0        0        0     1489 2024-02-04 05:34:39.677672 cicflowmeter-0.1.9/src/cicflowmeter/features/context/__init__.py
--rw-r--r--   0        0        0      952 2024-02-04 05:36:43.389897 cicflowmeter-0.1.9/src/cicflowmeter/features/flag_count.py
--rw-r--r--   0        0        0     7197 2024-02-11 09:44:04.803973 cicflowmeter-0.1.9/src/cicflowmeter/features/flow_bytes.py
--rw-r--r--   0        0        0     2324 2024-02-11 09:47:57.448576 cicflowmeter-0.1.9/src/cicflowmeter/features/packet_count.py
--rw-r--r--   0        0        0     5806 2024-02-04 06:00:07.694659 cicflowmeter-0.1.9/src/cicflowmeter/features/packet_length.py
--rw-r--r--   0        0        0     4743 2024-02-04 05:12:02.809193 cicflowmeter-0.1.9/src/cicflowmeter/features/packet_time.py
--rw-r--r--   0        0        0     3815 2024-02-04 05:40:00.839510 cicflowmeter-0.1.9/src/cicflowmeter/features/response_time.py
--rw-r--r--   0        0        0    14631 2024-02-04 06:25:30.218361 cicflowmeter-0.1.9/src/cicflowmeter/flow.py
--rw-r--r--   0        0        0     4196 2024-02-04 05:39:11.781287 cicflowmeter-0.1.9/src/cicflowmeter/flow_session.py
--rw-r--r--   0        0        0     2170 2024-02-03 11:05:10.082651 cicflowmeter-0.1.9/src/cicflowmeter/sniffer.py
--rw-r--r--   0        0        0     1086 2024-02-11 09:26:05.176724 cicflowmeter-0.1.9/src/cicflowmeter/utils.py
--rw-r--r--   0        0        0      776 2024-02-04 05:12:40.006305 cicflowmeter-0.1.9/src/cicflowmeter/writer.py
--rw-r--r--   0        0        0     1768 1970-01-01 00:00:00.000000 cicflowmeter-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-12-06 10:59:39.876738 cicflowmeter-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1360 2024-05-02 03:36:21.503508 cicflowmeter-0.2.0/README.md
+-rw-r--r--   0        0        0      630 2024-05-02 03:43:35.704005 cicflowmeter-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-12-07 04:42:03.793231 cicflowmeter-0.2.0/src/cicflowmeter/__init__.py
+-rw-r--r--   0        0        0      112 2024-05-01 15:49:25.572363 cicflowmeter-0.2.0/src/cicflowmeter/constants.py
+-rw-r--r--   0        0        0        0 2023-12-06 10:59:39.876738 cicflowmeter-0.2.0/src/cicflowmeter/features/__init__.py
+-rw-r--r--   0        0        0     1489 2024-02-04 05:34:39.677672 cicflowmeter-0.2.0/src/cicflowmeter/features/context/__init__.py
+-rw-r--r--   0        0        0      952 2024-02-04 05:36:43.389897 cicflowmeter-0.2.0/src/cicflowmeter/features/flag_count.py
+-rw-r--r--   0        0        0     7197 2024-02-11 09:44:04.803973 cicflowmeter-0.2.0/src/cicflowmeter/features/flow_bytes.py
+-rw-r--r--   0        0        0     2324 2024-02-11 09:47:57.448576 cicflowmeter-0.2.0/src/cicflowmeter/features/packet_count.py
+-rw-r--r--   0        0        0     5806 2024-02-04 06:00:07.694659 cicflowmeter-0.2.0/src/cicflowmeter/features/packet_length.py
+-rw-r--r--   0        0        0     4743 2024-02-04 05:12:02.809193 cicflowmeter-0.2.0/src/cicflowmeter/features/packet_time.py
+-rw-r--r--   0        0        0     3815 2024-02-04 05:40:00.839510 cicflowmeter-0.2.0/src/cicflowmeter/features/response_time.py
+-rw-r--r--   0        0        0    14766 2024-05-02 03:32:38.674242 cicflowmeter-0.2.0/src/cicflowmeter/flow.py
+-rw-r--r--   0        0        0     3867 2024-05-02 03:32:38.674242 cicflowmeter-0.2.0/src/cicflowmeter/flow_session.py
+-rw-r--r--   0        0        0     2714 2024-05-02 03:32:38.674242 cicflowmeter-0.2.0/src/cicflowmeter/sniffer.py
+-rw-r--r--   0        0        0     1086 2024-05-01 15:52:35.831738 cicflowmeter-0.2.0/src/cicflowmeter/utils.py
+-rw-r--r--   0        0        0     1179 2024-05-02 03:32:38.674242 cicflowmeter-0.2.0/src/cicflowmeter/writer.py
+-rw-r--r--   0        0        0     2066 1970-01-01 00:00:00.000000 cicflowmeter-0.2.0/PKG-INFO
```

### Comparing `cicflowmeter-0.1.9/LICENSE` & `cicflowmeter-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cicflowmeter-0.1.9/README.md` & `cicflowmeter-0.2.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -9,36 +9,40 @@
 cd cicflowmeter
 poetry install
 ```
 
 ### Usage
 
 ```sh
-usage: cicflowmeter [-h] (-i INPUT_INTERFACE | -f INPUT_FILE) [-c] [-v] output
+usage: cicflowmeter [-h] (-i INPUT_INTERFACE | -f INPUT_FILE) (-c | -u) [--fields FIELDS] [-v] output
 
 positional arguments:
-  output                output file name (in flow mode) or directory (in sequence mode)
+  output                output file name (in csv mode) or url (in url mode)
 
 options:
   -h, --help            show this help message and exit
-  -i INPUT_INTERFACE    capture online data from INPUT_INTERFACE
-  -f INPUT_FILE         capture offline data from INPUT_FILE
+  -i INPUT_INTERFACE, --interface INPUT_INTERFACE
+                        capture online data from INPUT_INTERFACE
+  -f INPUT_FILE, --file INPUT_FILE
+                        capture offline data from INPUT_FILE
   -c, --csv             output flows as csv
-  -v, --verbose         more verbosity
+  -u, --url             output flows as request to url
+  --fields FIELDS       comma separated fields to include in output (default: all)
+  -v, --verbose         more verbose
 ```
 
 Convert pcap file to flow csv:
 
 ```
 cicflowmeter -f example.pcap -c flows.csv
 ```
 
-Sniff packets real-time from interface to flow csv: (**need root permission**)
+Sniff packets real-time from interface to flow request: (**need root permission**)
 
 ```
-cicflowmeter -i eth0 -c flows.csv
+cicflowmeter -i eth0 -u http://localhost:8080/predict
 ```
 
 ### References:
 
 1. https://www.unb.ca/cic/research/applications.html#CICFlowMeter
 2. https://github.com/ahlashkari/CICFlowMeter
```

### Comparing `cicflowmeter-0.1.9/pyproject.toml` & `cicflowmeter-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cicflowmeter"
-version = "0.1.9"
+version = "0.2.0"
 description = "CICFlowMeter Python Implementation"
 authors = ["Hieu Le <hieulw99@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/hieulw/cicflowmeter"
 packages = [
     { include = "cicflowmeter", from = "src" },
@@ -15,14 +15,15 @@
 
 
 [tool.poetry.dependencies]
 python = "^3.11"
 numpy = "^1.26.2"
 scipy = "^1.11.4"
 scapy = "^2.5.0"
+requests = "^2.31.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `cicflowmeter-0.1.9/src/cicflowmeter/features/context/__init__.py` & `cicflowmeter-0.2.0/src/cicflowmeter/features/context/__init__.py`

 * *Files identical despite different names*

### Comparing `cicflowmeter-0.1.9/src/cicflowmeter/features/flag_count.py` & `cicflowmeter-0.2.0/src/cicflowmeter/features/flag_count.py`

 * *Files identical despite different names*

### Comparing `cicflowmeter-0.1.9/src/cicflowmeter/features/flow_bytes.py` & `cicflowmeter-0.2.0/src/cicflowmeter/features/flow_bytes.py`

 * *Files identical despite different names*

### Comparing `cicflowmeter-0.1.9/src/cicflowmeter/features/packet_count.py` & `cicflowmeter-0.2.0/src/cicflowmeter/features/packet_count.py`

 * *Files identical despite different names*

### Comparing `cicflowmeter-0.1.9/src/cicflowmeter/features/packet_length.py` & `cicflowmeter-0.2.0/src/cicflowmeter/features/packet_length.py`

 * *Files identical despite different names*

### Comparing `cicflowmeter-0.1.9/src/cicflowmeter/features/packet_time.py` & `cicflowmeter-0.2.0/src/cicflowmeter/features/packet_time.py`

 * *Files identical despite different names*

### Comparing `cicflowmeter-0.1.9/src/cicflowmeter/features/response_time.py` & `cicflowmeter-0.2.0/src/cicflowmeter/features/response_time.py`

 * *Files identical despite different names*

### Comparing `cicflowmeter-0.1.9/src/cicflowmeter/flow.py` & `cicflowmeter-0.2.0/src/cicflowmeter/flow.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         self.backward_bulk_count = 0
         self.backward_bulk_count_tmp = 0
         self.backward_bulk_duration = 0
         self.backward_bulk_packet_count = 0
         self.backward_bulk_size = 0
         self.backward_bulk_size_tmp = 0
 
-    def get_data(self) -> dict:
+    def get_data(self, include_fields=None) -> dict:
         """This method obtains the values of the features extracted from each flow.
 
         Note:
             Only some of the network data plays well together in this list.
             Time-to-live values, window values, and flags cause the data to
             separate out too much.
 
@@ -177,14 +177,17 @@
         data["bwd_seg_size_avg"] = data["bwd_pkt_len_mean"]
         data["cwr_flag_count"] = data["fwd_urg_flags"]
         data["subflow_fwd_pkts"] = data["tot_fwd_pkts"]
         data["subflow_bwd_pkts"] = data["tot_bwd_pkts"]
         data["subflow_fwd_byts"] = data["totlen_fwd_pkts"]
         data["subflow_bwd_byts"] = data["totlen_bwd_pkts"]
 
+        if include_fields is not None:
+            data = {k: v for k, v in data.items() if k in include_fields}
+
         return data
 
     def add_packet(self, packet: Packet, direction: PacketDirection) -> None:
         """Adds a packet to the current list of packets.
 
         Args:
             packet: Packet to be added to a flow
```

### Comparing `cicflowmeter-0.1.9/src/cicflowmeter/flow_session.py` & `cicflowmeter-0.2.0/src/cicflowmeter/flow_session.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,111 +8,100 @@
 from .flow import Flow
 from .utils import get_logger
 
 
 class FlowSession(DefaultSession):
     """Creates a list of network flows."""
 
+    verbose = False
+    fields = None
+    output_mode = None
+    output = None
+
     def __init__(self, *args, **kwargs):
-        self.flows = {}
+        self.flows: dict[tuple, Flow] = {}
         self.logger = get_logger(self.verbose)
         self.packets_count = 0
-        self.output_writer = output_writer_factory(self.output_mode, self.output_file)
+        self.output_writer = output_writer_factory(self.output_mode, self.output)
 
         super(FlowSession, self).__init__(*args, **kwargs)
 
     def toPacketList(self):
         # Sniffer finished all the packets it needed to sniff.
         # It is not a good place for this, we need to somehow define a finish signal for AsyncSniffer
         self.garbage_collect(None)
         del self.output_writer
         return super(FlowSession, self).toPacketList()
 
-    def on_packet_received(self, packet: Packet):
+    def on_packet_received(self, pkt: Packet):
         count = 0
         direction = PacketDirection.FORWARD
 
-        if self.output_mode != "csv":
-            if "TCP" not in packet:
-                return
-            elif "UDP" not in packet:
-                return
+        if "TCP" not in pkt and "UDP" not in pkt:
+            return
 
         try:
             # Creates a key variable to check
-            packet_flow_key = get_packet_flow_key(packet, direction)
+            packet_flow_key = get_packet_flow_key(pkt, direction)
             flow = self.flows.get((packet_flow_key, count))
         except Exception:
             return
 
         self.packets_count += 1
+        self.logger.debug(f"Packet {self.packets_count}: {pkt}")
 
         # If there is no forward flow with a count of 0
         if flow is None:
             # There might be one of it in reverse
             direction = PacketDirection.REVERSE
-            packet_flow_key = get_packet_flow_key(packet, direction)
+            packet_flow_key = get_packet_flow_key(pkt, direction)
             flow = self.flows.get((packet_flow_key, count))
 
         if flow is None:
             # If no flow exists create a new flow
             direction = PacketDirection.FORWARD
-            flow = Flow(packet, direction)
-            packet_flow_key = get_packet_flow_key(packet, direction)
+            flow = Flow(pkt, direction)
+            packet_flow_key = get_packet_flow_key(pkt, direction)
             self.flows[(packet_flow_key, count)] = flow
 
-        elif (packet.time - flow.latest_timestamp) > EXPIRED_UPDATE:
+        elif (pkt.time - flow.latest_timestamp) > EXPIRED_UPDATE:
             # If the packet exists in the flow but the packet is sent
             # after too much of a delay than it is a part of a new flow.
             expired = EXPIRED_UPDATE
-            while (packet.time - flow.latest_timestamp) > expired:
+            while (pkt.time - flow.latest_timestamp) > expired:
                 count += 1
                 expired += EXPIRED_UPDATE
                 flow = self.flows.get((packet_flow_key, count))
 
                 if flow is None:
-                    flow = Flow(packet, direction)
+                    flow = Flow(pkt, direction)
                     self.flows[(packet_flow_key, count)] = flow
                     break
-        elif "F" in packet.flags:
+        elif "F" in pkt.flags:
             # If it has FIN flag then early collect flow and continue
-            flow.add_packet(packet, direction)
-            self.garbage_collect(packet.time)
+            flow.add_packet(pkt, direction)
+            self.garbage_collect(pkt.time)
             return
 
-        flow.add_packet(packet, direction)
+        flow.add_packet(pkt, direction)
 
         if self.packets_count % GARBAGE_COLLECT_PACKETS == 0 or flow.duration > 120:
-            self.garbage_collect(packet.time)
+            self.garbage_collect(pkt.time)
 
-    def get_flows(self) -> list:
+    def get_flows(self):
         return self.flows.values()
 
     def garbage_collect(self, latest_time) -> None:
         # TODO: Garbage Collection / Feature Extraction should have a separate thread
-        self.logger.debug(f"Garbage Collection Began. Flows = {len(self.flows)}")
-        keys = list(self.flows.keys())
-        for k in keys:
+        for k in list(self.flows.keys()):
             flow = self.flows.get(k)
 
-            if (
+            if not flow or (
                 latest_time is not None
                 and latest_time - flow.latest_timestamp < EXPIRED_UPDATE
                 and flow.duration < 90
             ):
                 continue
 
-            self.output_writer.write(flow.get_data())
+            self.output_writer.write(flow.get_data(self.fields))
             del self.flows[k]
-        self.logger.debug(f"Garbage Collection Finished. Flows = {len(self.flows)}")
-
-
-def generate_session_class(output_mode, output_file, verbose):
-    return type(
-        "NewFlowSession",
-        (FlowSession,),
-        {
-            "output_mode": output_mode,
-            "output_file": output_file,
-            "verbose": verbose,
-        },
-    )
+            self.logger.debug(f"Flow Collected! Remain Flows = {len(self.flows)}")
```

### Comparing `cicflowmeter-0.1.9/src/cicflowmeter/sniffer.py` & `cicflowmeter-0.2.0/src/cicflowmeter/sniffer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 import argparse
 
 from scapy.sendrecv import AsyncSniffer
 
-from .flow_session import generate_session_class
+from cicflowmeter.flow_session import FlowSession
 
 
 def create_sniffer(
-    input_file, input_interface, output_mode, output_file, verbose=False
+    input_file, input_interface, output_mode, output, fields=None, verbose=False
 ):
     assert (input_file is None) ^ (
         input_interface is None
     ), "Either provide interface input or file input not both"
+    if fields is not None:
+        fields = fields.split(",")
 
-    NewFlowSession = generate_session_class(output_mode, output_file, verbose)
+    setattr(FlowSession, "output_mode", output_mode)
+    setattr(FlowSession, "output", output)
+    setattr(FlowSession, "fields", fields)
+    setattr(FlowSession, "verbose", verbose)
 
     if input_file:
         return AsyncSniffer(
             offline=input_file,
             filter="ip and (tcp or udp)",
             prn=None,
-            session=NewFlowSession,
+            session=FlowSession,
             store=False,
         )
     else:
         return AsyncSniffer(
             iface=input_interface,
             filter="ip and (tcp or udp)",
             prn=None,
-            session=NewFlowSession,
+            session=FlowSession,
             store=False,
         )
 
 
 def main():
     parser = argparse.ArgumentParser()
 
@@ -39,46 +44,62 @@
     input_group.add_argument(
         "-i",
         "--interface",
         action="store",
         dest="input_interface",
         help="capture online data from INPUT_INTERFACE",
     )
-
     input_group.add_argument(
         "-f",
         "--file",
         action="store",
         dest="input_file",
         help="capture offline data from INPUT_FILE",
     )
 
-    output_group = parser.add_mutually_exclusive_group(required=False)
+    output_group = parser.add_mutually_exclusive_group(required=True)
     output_group.add_argument(
         "-c",
         "--csv",
         action="store_const",
         const="csv",
         dest="output_mode",
         help="output flows as csv",
     )
+    output_group.add_argument(
+        "-u",
+        "--url",
+        action="store_const",
+        const="url",
+        dest="output_mode",
+        help="output flows as request to url",
+    )
 
     parser.add_argument(
         "output",
-        help="output file name (in flow mode) or directory (in sequence mode)",
+        help="output file name (in csv mode) or url (in url mode)",
     )
-    parser.add_argument("-v", "--verbose", action="store_true", help="more verbosity")
+
+    parser.add_argument(
+        "--fields",
+        action="store",
+        dest="fields",
+        help="comma separated fields to include in output (default: all)",
+    )
+
+    parser.add_argument("-v", "--verbose", action="store_true", help="more verbose")
 
     args = parser.parse_args()
 
     sniffer = create_sniffer(
         args.input_file,
         args.input_interface,
         args.output_mode,
         args.output,
+        args.fields,
         args.verbose,
     )
     sniffer.start()
 
     try:
         sniffer.join()
     except KeyboardInterrupt:
```

### Comparing `cicflowmeter-0.1.9/src/cicflowmeter/utils.py` & `cicflowmeter-0.2.0/src/cicflowmeter/utils.py`

 * *Files identical despite different names*

### Comparing `cicflowmeter-0.1.9/PKG-INFO` & `cicflowmeter-0.2.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: cicflowmeter
-Version: 0.1.9
+Version: 0.2.0
 Summary: CICFlowMeter Python Implementation
 Home-page: https://github.com/hieulw/cicflowmeter
 License: MIT
 Author: Hieu Le
 Author-email: hieulw99@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: numpy (>=1.26.2,<2.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: scapy (>=2.5.0,<3.0.0)
 Requires-Dist: scipy (>=1.11.4,<2.0.0)
 Project-URL: Repository, https://github.com/hieulw/cicflowmeter
 Description-Content-Type: text/markdown
 
 # Python CICFlowMeter
 
@@ -28,37 +29,41 @@
 cd cicflowmeter
 poetry install
 ```
 
 ### Usage
 
 ```sh
-usage: cicflowmeter [-h] (-i INPUT_INTERFACE | -f INPUT_FILE) [-c] [-v] output
+usage: cicflowmeter [-h] (-i INPUT_INTERFACE | -f INPUT_FILE) (-c | -u) [--fields FIELDS] [-v] output
 
 positional arguments:
-  output                output file name (in flow mode) or directory (in sequence mode)
+  output                output file name (in csv mode) or url (in url mode)
 
 options:
   -h, --help            show this help message and exit
-  -i INPUT_INTERFACE    capture online data from INPUT_INTERFACE
-  -f INPUT_FILE         capture offline data from INPUT_FILE
+  -i INPUT_INTERFACE, --interface INPUT_INTERFACE
+                        capture online data from INPUT_INTERFACE
+  -f INPUT_FILE, --file INPUT_FILE
+                        capture offline data from INPUT_FILE
   -c, --csv             output flows as csv
-  -v, --verbose         more verbosity
+  -u, --url             output flows as request to url
+  --fields FIELDS       comma separated fields to include in output (default: all)
+  -v, --verbose         more verbose
 ```
 
 Convert pcap file to flow csv:
 
 ```
 cicflowmeter -f example.pcap -c flows.csv
 ```
 
-Sniff packets real-time from interface to flow csv: (**need root permission**)
+Sniff packets real-time from interface to flow request: (**need root permission**)
 
 ```
-cicflowmeter -i eth0 -c flows.csv
+cicflowmeter -i eth0 -u http://localhost:8080/predict
 ```
 
 ### References:
 
 1. https://www.unb.ca/cic/research/applications.html#CICFlowMeter
 2. https://github.com/ahlashkari/CICFlowMeter
```

