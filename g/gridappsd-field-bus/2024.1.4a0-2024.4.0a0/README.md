# Comparing `tmp/gridappsd_field_bus-2024.1.4a0.tar.gz` & `tmp/gridappsd_field_bus-2024.4.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridappsd_field_bus-2024.1.4a0.tar", max compression
+gzip compressed data, was "gridappsd_field_bus-2024.4.0a0.tar", max compression
```

## Comparing `gridappsd_field_bus-2024.1.4a0.tar` & `gridappsd_field_bus-2024.4.0a0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0        0 2024-01-25 21:54:57.918464 gridappsd_field_bus-2024.1.4a0/README.md
--rw-r--r--   0        0        0        0 2024-01-25 21:54:57.918464 gridappsd_field_bus-2024.1.4a0/gridappsd/__no_init__here
--rw-r--r--   0        0        0      227 2024-01-25 21:54:57.918464 gridappsd_field_bus-2024.1.4a0/gridappsd/field_interface/__init__.py
--rw-r--r--   0        0        0      280 2024-01-25 21:54:57.918464 gridappsd_field_bus-2024.1.4a0/gridappsd/field_interface/agents/__init__.py
--rw-r--r--   0        0        0    16365 2024-01-25 21:54:57.918464 gridappsd_field_bus-2024.1.4a0/gridappsd/field_interface/agents/agents.py
--rw-r--r--   0        0        0     2556 2024-01-25 21:54:57.918464 gridappsd_field_bus-2024.1.4a0/gridappsd/field_interface/context.py
--rw-r--r--   0        0        0    12087 2024-01-25 21:54:57.918464 gridappsd_field_bus-2024.1.4a0/gridappsd/field_interface/context_manager.py
--rw-r--r--   0        0        0     1856 2024-01-25 21:54:57.918464 gridappsd_field_bus-2024.1.4a0/gridappsd/field_interface/gridappsd_field_bus.py
--rw-r--r--   0        0        0     7538 2024-01-25 21:54:57.918464 gridappsd_field_bus-2024.1.4a0/gridappsd/field_interface/interfaces.py
--rw-r--r--   0        0        0     1264 2024-01-25 21:55:52.602276 gridappsd_field_bus-2024.1.4a0/pyproject.toml
--rw-r--r--   0        0        0      854 1970-01-01 00:00:00.000000 gridappsd_field_bus-2024.1.4a0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-02 16:40:43.790433 gridappsd_field_bus-2024.4.0a0/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 16:40:43.790433 gridappsd_field_bus-2024.4.0a0/gridappsd/__no_init__here
+-rw-r--r--   0        0        0      217 2024-05-02 16:40:43.790433 gridappsd_field_bus-2024.4.0a0/gridappsd/field_interface/__init__.py
+-rw-r--r--   0        0        0      350 2024-05-02 16:40:43.790433 gridappsd_field_bus-2024.4.0a0/gridappsd/field_interface/agents/__init__.py
+-rw-r--r--   0        0        0    15723 2024-05-02 16:40:43.790433 gridappsd_field_bus-2024.4.0a0/gridappsd/field_interface/agents/agents.py
+-rw-r--r--   0        0        0     3361 2024-05-02 16:40:43.790433 gridappsd_field_bus-2024.4.0a0/gridappsd/field_interface/context.py
+-rw-r--r--   0        0        0    12316 2024-05-02 16:40:43.790433 gridappsd_field_bus-2024.4.0a0/gridappsd/field_interface/context_manager.py
+-rw-r--r--   0        0        0     1829 2024-05-02 16:40:43.790433 gridappsd_field_bus-2024.4.0a0/gridappsd/field_interface/gridappsd_field_bus.py
+-rw-r--r--   0        0        0     7544 2024-05-02 16:40:43.790433 gridappsd_field_bus-2024.4.0a0/gridappsd/field_interface/interfaces.py
+-rw-r--r--   0        0        0     1264 2024-05-02 16:41:40.206314 gridappsd_field_bus-2024.4.0a0/pyproject.toml
+-rw-r--r--   0        0        0      854 1970-01-01 00:00:00.000000 gridappsd_field_bus-2024.4.0a0/PKG-INFO
```

### Comparing `gridappsd_field_bus-2024.1.4a0/gridappsd/field_interface/agents/agents.py` & `gridappsd_field_bus-2024.4.0a0/gridappsd/field_interface/agents/agents.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,17 +11,15 @@
 from cimgraph.models import FeederModel
 from cimgraph.models.distributed_area import DistributedArea
 
 from gridappsd import DifferenceBuilder
 import gridappsd.topics as t
 from gridappsd.field_interface.context import LocalContext
 from gridappsd.field_interface.gridappsd_field_bus import GridAPPSDMessageBus
-from gridappsd.field_interface.interfaces import (FieldMessageBus,
-                                                  MessageBusDefinition)
-                                                  
+from gridappsd.field_interface.interfaces import (FieldMessageBus, MessageBusDefinition)
 
 CIM_PROFILE = None
 IEC61970_301 = None
 cim = None
 
 _log = logging.getLogger(__name__)
 
@@ -60,16 +58,15 @@
         _log.debug(f"Creating DistributedAgent: {self.__class__.__name__}")
         self.upstream_message_bus = None
         self.downstream_message_bus = None
         self.simulation_id = simulation_id
         self.context = None
 
         # TODO: Change params and connection to local connection
-        self.params = ConnectionParameters(cim_profile=CIM_PROFILE,
-                                           iec61970_301=IEC61970_301)
+        self.params = ConnectionParameters(cim_profile=CIM_PROFILE, iec61970_301=IEC61970_301)
 
         self.connection = GridappsdConnection(self.params)
         self.connection.cim_profile = cim_profile
 
         self.app_id = agent_config['app_id']
         self.description = agent_config['description']
         dt = datetime.now()
@@ -79,23 +76,21 @@
         else:
             self.agent_id = downstream_message_bus_def.id + '.context_manager'
 
         self.agent_area_dict = agent_area_dict
 
         if upstream_message_bus_def is not None:
             if upstream_message_bus_def.is_ot_bus:
-                self.upstream_message_bus = GridAPPSDMessageBus(
-                    upstream_message_bus_def)
+                self.upstream_message_bus = GridAPPSDMessageBus(upstream_message_bus_def)
         #            else:
         #                self.upstream_message_bus = VolttronMessageBus(upstream_message_bus_def)
 
         if downstream_message_bus_def is not None:
             if downstream_message_bus_def.is_ot_bus:
-                self.downstream_message_bus = GridAPPSDMessageBus(
-                    downstream_message_bus_def)
+                self.downstream_message_bus = GridAPPSDMessageBus(downstream_message_bus_def)
         #            else:
         #                self.downstream_message_bus = VolttronMessageBus(downstream_message_bus_def)
 
         # self.context = ContextManager.get(self.feeder_id, self.area_id)
 
         # if agent_dict is not None:
         #    self.addressable_equipments = agent_dict['addressable_equipment']
@@ -104,157 +99,138 @@
     def _connect(self):
 
         if self.upstream_message_bus is not None:
             self.upstream_message_bus.connect()
         if self.downstream_message_bus is not None:
             self.downstream_message_bus.connect()
         if self.downstream_message_bus is None and self.upstream_message_bus is None:
-            raise ValueError(
-                "Either upstream or downstream bus must be specified!")
+            raise ValueError("Either upstream or downstream bus must be specified!")
 
         if ('context_manager' not in self.app_id):
             self.agent_id = "da_" + self.app_id + "_" + self.downstream_message_bus.id
 
         if self.agent_area_dict is None:
-            context = LocalContext.get_context_by_message_bus(
-                self.downstream_message_bus)
+            context = LocalContext.get_context_by_message_bus(self.downstream_message_bus)
             self.agent_area_dict = context['data']
 
         self.subscribe_to_measurement()
         self.subscribe_to_messages()
         self.subscribe_to_requests()
 
         if ('context_manager' not in self.app_id):
-            LocalContext.register_agent(self.downstream_message_bus,
-                                        self.upstream_message_bus, self)
+            LocalContext.register_agent(self.downstream_message_bus, self.upstream_message_bus,
+                                        self)
 
     def disconnect(self):
 
         if self.upstream_message_bus is not None:
             self.upstream_message_bus.disconnect()
         if self.downstream_message_bus is not None:
             self.downstream_message_bus.disconnect()
 
     def subscribe_to_measurement(self):
         if self.simulation_id is None:
             self.downstream_message_bus.subscribe(
-                t.field_output_topic(self.downstream_message_bus.id),
-                self.on_measurement)
+                t.field_output_topic(self.downstream_message_bus.id), self.on_measurement)
         else:
-            topic = t.field_output_topic(self.downstream_message_bus.id,
-                                         self.simulation_id)
+            topic = t.field_output_topic(self.downstream_message_bus.id, self.simulation_id)
             _log.debug(f"subscribing to simulation output on topic {topic}")
-            self.downstream_message_bus.subscribe(topic,
-                                                  self.on_simulation_output)
+            self.downstream_message_bus.subscribe(topic, self.on_simulation_output)
 
     def subscribe_to_messages(self):
 
         self.downstream_message_bus.subscribe(
-            t.field_message_bus_topic(self.downstream_message_bus.id),
-            self.on_downstream_message)
+            t.field_message_bus_topic(self.downstream_message_bus.id), self.on_downstream_message)
         self.upstream_message_bus.subscribe(
-            t.field_message_bus_topic(self.upstream_message_bus.id),
-            self.on_upstream_message)
+            t.field_message_bus_topic(self.upstream_message_bus.id), self.on_upstream_message)
 
         _log.debug(
             f"Subscribing to messages on application topics: \n {t.field_message_bus_app_topic(self.downstream_message_bus.id, self.app_id)} \
                                                                     \n {t.field_message_bus_app_topic(self.upstream_message_bus.id, self.app_id)}"
         )
         self.downstream_message_bus.subscribe(
-            t.field_message_bus_app_topic(self.downstream_message_bus.id,
-                                          self.app_id),
+            t.field_message_bus_app_topic(self.downstream_message_bus.id, self.app_id),
             self.on_downstream_message)
         self.upstream_message_bus.subscribe(
-            t.field_message_bus_app_topic(self.upstream_message_bus.id,
-                                          self.app_id),
+            t.field_message_bus_app_topic(self.upstream_message_bus.id, self.app_id),
             self.on_upstream_message)
 
         if ('context_manager' not in self.app_id):
             _log.debug(
                 f"Subscribing to message on agents topics: \n {t.field_message_bus_agent_topic(self.downstream_message_bus.id, self.agent_id)} \
                                                                 \n {t.field_message_bus_agent_topic(self.upstream_message_bus.id, self.agent_id)}"
             )
             self.downstream_message_bus.subscribe(
-                t.field_message_bus_agent_topic(self.downstream_message_bus.id,
-                                                self.agent_id),
+                t.field_message_bus_agent_topic(self.downstream_message_bus.id, self.agent_id),
                 self.on_downstream_message)
             self.upstream_message_bus.subscribe(
-                t.field_message_bus_agent_topic(self.upstream_message_bus.id,
-                                                self.agent_id),
+                t.field_message_bus_agent_topic(self.upstream_message_bus.id, self.agent_id),
                 self.on_upstream_message)
 
     def subscribe_to_requests(self):
 
         _log.debug(
             f"Subscribing to requests on agents queue: \n {t.field_agent_request_queue(self.downstream_message_bus.id, self.agent_id)} \
                                                             \n {t.field_agent_request_queue(self.upstream_message_bus.id, self.agent_id)}"
         )
         self.downstream_message_bus.subscribe(
-            t.field_agent_request_queue(self.downstream_message_bus.id,
-                                        self.agent_id),
+            t.field_agent_request_queue(self.downstream_message_bus.id, self.agent_id),
             self.on_request_from_downstream)
         self.upstream_message_bus.subscribe(
-            t.field_agent_request_queue(self.upstream_message_bus.id,
-                                        self.agent_id),
+            t.field_agent_request_queue(self.upstream_message_bus.id, self.agent_id),
             self.on_request_from_uptream)
 
     def on_measurement(self, headers: Dict, message) -> None:
-        raise NotImplementedError(
-            f"{self.__class__.__name__} must be overriden in child class")
+        raise NotImplementedError(f"{self.__class__.__name__} must be overriden in child class")
 
     def on_simulation_output(self, headers, message):
         self.on_measurement(headers=headers, message=message)
 
     def on_upstream_message(self, headers: Dict, message) -> None:
-        raise NotImplementedError(
-            f"{self.__class__.__name__} must be overriden in child class")
+        raise NotImplementedError(f"{self.__class__.__name__} must be overriden in child class")
 
     def on_downstream_message(self, headers: Dict, message) -> None:
-        raise NotImplementedError(
-            f"{self.__class__.__name__} must be overriden in child class")
+        raise NotImplementedError(f"{self.__class__.__name__} must be overriden in child class")
 
     def on_request_from_uptream(self, headers: Dict, message):
         self.on_request(self.upstream_message_bus, headers, message)
 
     def on_request_from_downstream(self, headers: Dict, message):
         self.on_request(self.downstream_message_bus, headers, message)
 
     def on_request(self, message_bus, headers: Dict, message):
-        raise NotImplementedError(
-            f"{self.__class__.__name__} must be overriden in child class")
+        raise NotImplementedError(f"{self.__class__.__name__} must be overriden in child class")
 
     def get_registration_details(self):
-        details = AgentRegistrationDetails(str(self.agent_id), self.app_id,
-                                           self.description,
+        details = AgentRegistrationDetails(str(self.agent_id), self.app_id, self.description,
                                            self.upstream_message_bus.id,
                                            self.downstream_message_bus.id)
         return dataclasses.asdict(details)
 
     def publish_downstream(self, message):
-        self.downstream_message_bus.send(
-            t.field_message_bus_topic(self.downstream_message_bus.id), message)
+        self.downstream_message_bus.send(t.field_message_bus_topic(self.downstream_message_bus.id),
+                                         message)
 
     def publish_upstream(self, message):
-        self.upstream_message_bus.send(
-            t.field_message_bus_topic(self.upstream_message_bus.id), message)
+        self.upstream_message_bus.send(t.field_message_bus_topic(self.upstream_message_bus.id),
+                                       message)
 
     def send_control_command(self, differenceBuilder: DifferenceBuilder):
         if self.simulation_id is not None:
-            LocalContext.send_control_command(self.downstream_message_bus,
-                                              differenceBuilder)
+            LocalContext.send_control_command(self.downstream_message_bus, differenceBuilder)
 
     '''
         TODO This block needs to be tested with device interface
         else:
         self.downstream_message_bus.send(devie_interface_topic, differenceBuilder)
     '''
 
 
 '''  TODO this has not been implemented yet, so we are commented them out for now.
-    # not all agent would use this    
+    # not all agent would use this
     def on_control(self, control):
         device_id = control.get('device')
         command = control.get('command')
         self.control_device(device_id, command)
 '''
 
 
@@ -262,83 +238,80 @@
 
     def __init__(self,
                  upstream_message_bus_def: MessageBusDefinition,
                  downstream_message_bus_def: MessageBusDefinition,
                  agent_config: Dict,
                  feeder_dict=None,
                  simulation_id=None):
-        super().__init__(upstream_message_bus_def, downstream_message_bus_def,
-                         agent_config, feeder_dict, simulation_id)
+        super().__init__(upstream_message_bus_def, downstream_message_bus_def, agent_config,
+                         feeder_dict, simulation_id)
         self.feeder_area = None
         self.downstream_message_bus_def = downstream_message_bus_def
 
         self._connect()
 
         if self.agent_area_dict is not None:
-            feeder = cim.EquipmentContainer(
-                mRID=self.downstream_message_bus_def.id)
+            feeder = cim.EquipmentContainer(mRID=self.downstream_message_bus_def.id)
             self.feeder_area = DistributedArea(connection=self.connection,
                                                container=feeder,
                                                distributed=True)
-            self.feeder_area.build_from_topo_message(
-                topology_dict=self.agent_area_dict, centralized_graph=None)
+            self.feeder_area.build_from_topo_message(topology_dict=self.agent_area_dict,
+                                                     centralized_graph=None)
 
 
 class SwitchAreaAgent(DistributedAgent):
 
     def __init__(self,
                  upstream_message_bus_def: MessageBusDefinition,
                  downstream_message_bus_def: MessageBusDefinition,
                  agent_config: Dict,
                  switch_area_dict=None,
                  simulation_id=None):
-        super().__init__(upstream_message_bus_def, downstream_message_bus_def,
-                         agent_config, switch_area_dict, simulation_id)
+        super().__init__(upstream_message_bus_def, downstream_message_bus_def, agent_config,
+                         switch_area_dict, simulation_id)
         self.switch_area = None
         self.downstream_message_bus_def = downstream_message_bus_def
 
         self._connect()
 
         if self.agent_area_dict is not None:
-            container = cim.EquipmentContainer(
-                mRID=self.downstream_message_bus_def.id)
+            container = cim.EquipmentContainer(mRID=self.downstream_message_bus_def.id)
             self.switch_area = DistributedArea(container=container,
                                                connection=self.connection,
                                                distributed=True)
-            self.switch_area.build_from_topo_message(
-                topology_dict=self.agent_area_dict, centralized_graph=None)
+            self.switch_area.build_from_topo_message(topology_dict=self.agent_area_dict,
+                                                     centralized_graph=None)
 
 
 class SecondaryAreaAgent(DistributedAgent):
 
     def __init__(self,
                  upstream_message_bus_def: MessageBusDefinition,
                  downstream_message_bus_def: MessageBusDefinition,
                  agent_config: Dict,
                  secondary_area_dict=None,
                  simulation_id=None):
-        super().__init__(upstream_message_bus_def, downstream_message_bus_def,
-                         agent_config, secondary_area_dict, simulation_id)
+        super().__init__(upstream_message_bus_def, downstream_message_bus_def, agent_config,
+                         secondary_area_dict, simulation_id)
         self.secondary_area = None
         self.downstream_message_bus_def = downstream_message_bus_def
 
         self._connect()
 
         if self.agent_area_dict is not None:
             if len(self.agent_area_dict['addressable_equipment']) == 0:
                 _log.warning(
                     f"No addressable equipment in the secondary area with down stream message bus id: {self.downstream_message_bus.id}."
                 )
-            container = cim.EquipmentContainer(
-                mRID=self.downstream_message_bus_def.id)
+            container = cim.EquipmentContainer(mRID=self.downstream_message_bus_def.id)
             self.secondary_area = DistributedArea(container=container,
                                                   connection=self.connection,
                                                   distributed=True)
-            self.secondary_area.build_from_topo_message(
-                topology_dict=self.agent_area_dict, centralized_graph=None)
+            self.secondary_area.build_from_topo_message(topology_dict=self.agent_area_dict,
+                                                        centralized_graph=None)
 
 
 class CoordinatingAgent:
     """
     A CoordinatingAgent performs following functions:
         1. Spawns distributed agents
         2. Publishes compiled output to centralized OT bus
```

### Comparing `gridappsd_field_bus-2024.1.4a0/gridappsd/field_interface/context_manager.py` & `gridappsd_field_bus-2024.4.0a0/gridappsd/field_interface/context_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,20 @@
 import time
 from typing import Dict
 
 import gridappsd.field_interface.agents.agents as agents_mod
 import gridappsd.topics as t
 from cimgraph.data_profile import CIM_PROFILE
 from gridappsd import GridAPPSD
-from gridappsd.field_interface.agents import (FeederAgent, SecondaryAreaAgent,
-                                              SwitchAreaAgent)
+from gridappsd.field_interface.agents import (FeederAgent, SecondaryAreaAgent, SwitchAreaAgent)
 from gridappsd.field_interface.interfaces import MessageBusDefinition
 
-
 cim_profile = CIM_PROFILE.RC4_2021.value
 
-agents_mod.set_cim_profile(cim_profile=cim_profile,iec61970_301=7)
+agents_mod.set_cim_profile(cim_profile=cim_profile, iec61970_301=7)
 
 cim = agents_mod.cim
 
 logging.basicConfig(level=logging.DEBUG)
 logging.getLogger('goss').setLevel(logging.ERROR)
 logging.getLogger('stomp.py').setLevel(logging.ERROR)
 
@@ -36,266 +34,257 @@
                  downstream_message_bus_def: MessageBusDefinition,
                  agent_config: Dict,
                  feeder_dict: Dict = None,
                  simulation_id: str = None):
 
         self.ot_connection = GridAPPSD()
         if feeder_dict is None:
-            request = {'request_type':'get_context',
-                       'modelId': downstream_message_bus_def.id}
+            request = {'request_type': 'get_context', 'modelId': downstream_message_bus_def.id}
             feeder_dict = None
             while feeder_dict is None:
-                self.ot_connection.get_logger().info(f"Requesting topology for {self.__class__}")
+                self.ot_connection.get_logger().debug(f"Requesting topology for {self.__class__}")
                 response = self.ot_connection.get_response(REQUEST_FIELD, request, timeout=10)
                 if 'data' in response:
                     feeder_dict = response['data']
-                    self.ot_connection.send_status("******RCVD FEEDER *************", '/topic/goss.gridappsd.platform.log', 'DEBUG')
+                    self.ot_connection.get_logger().debug("Topology received at Feeder Area Context Manager")
                 else:
                     time.sleep(5)
-        super().__init__(upstream_message_bus_def, downstream_message_bus_def,
-                         agent_config, feeder_dict, simulation_id)
+        super().__init__(upstream_message_bus_def, downstream_message_bus_def, agent_config,
+                         feeder_dict, simulation_id)
 
         #Override agent_id to a static value
         self.agent_id = downstream_message_bus_def.id + '.context_manager'
-        
+
         self.context = None
 
         self.registered_agents = {}
         self.registered_agents[self.agent_id] = self.get_registration_details()
 
         self.neighbouring_agents = {}
         self.upstream_agents = {}
         self.downstream_agents = {}
+        self.ot_connection.get_logger().info("Feeder Area Context Manager Created")
 
     def on_request(self, message_bus, headers: Dict, message):
 
         _log.debug(f"Received request: {message}")
 
         if message['request_type'] == 'get_context':
             reply_to = headers['reply-to']
             if self.context is None:
                 self.context = self.ot_connection.get_response(REQUEST_FIELD, message)
-            message_bus.send(reply_to,self.context)
+            message_bus.send(reply_to, self.context)
 
         elif message['request_type'] == 'register_agent':
             self.ot_connection.send(t.REGISTER_AGENT_QUEUE, message)
-            self.registered_agents[message['agent']
-                                   ['agent_id']] = message['agent']
+            self.registered_agents[message['agent']['agent_id']] = message['agent']
 
         elif message['request_type'] == 'get_agents':
             reply_to = headers['reply-to']
             message_bus.send(reply_to, self.registered_agents)
 
         elif message['request_type'] == 'is_initialized':
             reply_to = headers['reply-to']
-            message = {'initialized':True}
+            message = {'initialized': True}
             message_bus.send(reply_to, message)
 
         elif message['request_type'] == 'control_command':
             simulation_id = message['input']['simulation_id']
-            self.ot_connection.send(t.simulation_input_topic(simulation_id),
-                                    message)
+            self.ot_connection.send(t.simulation_input_topic(simulation_id), message)
 
 
 class SwitchAreaContextManager(SwitchAreaAgent):
 
     def __init__(self,
                  upstream_message_bus_def: MessageBusDefinition,
                  downstream_message_bus_def: MessageBusDefinition,
                  agent_config: Dict,
                  switch_area_dict: Dict = None,
                  simulation_id: str = None):
 
         self.ot_connection = GridAPPSD()
         if switch_area_dict is None:
-            request = {'request_type':'get_context',
-                       'areaId': downstream_message_bus_def.id}
-            switch_area_dict = self.ot_connection.get_response(
-                REQUEST_FIELD, request, timeout=10)['data']
+            request = {'request_type': 'get_context', 'areaId': downstream_message_bus_def.id}
+            switch_area_dict = self.ot_connection.get_response(REQUEST_FIELD, request,
+                                                               timeout=10)['data']
 
-        super().__init__(upstream_message_bus_def, downstream_message_bus_def,
-                         agent_config, switch_area_dict, simulation_id)
+        super().__init__(upstream_message_bus_def, downstream_message_bus_def, agent_config,
+                         switch_area_dict, simulation_id)
 
         #Override agent_id to a static value
         self.agent_id = downstream_message_bus_def.id + '.context_manager'
-        
+
         self.context = None
 
         self.registered_agents = {}
         self.registered_agents[self.agent_id] = self.get_registration_details()
+        self.ot_connection.get_logger().info("Switch Area "+self.agent_id+" Context Manager Created")
 
     def on_request(self, message_bus, headers: Dict, message):
 
         _log.debug(f"Received request: {message}")
 
         if message['request_type'] == 'get_context':
             #TODO: check for initialization
             reply_to = headers['reply-to']
             if self.context is None:
                 self.context = self.ot_connection.get_response(REQUEST_FIELD, message)
-            message_bus.send(reply_to,self.context)
+            message_bus.send(reply_to, self.context)
 
         elif message['request_type'] == 'register_agent':
             #TODO: check for initialization
             self.ot_connection.send(t.REGISTER_AGENT_QUEUE, message)
-            self.registered_agents[message['agent']
-                                   ['agent_id']] = message['agent']
+            self.registered_agents[message['agent']['agent_id']] = message['agent']
 
         elif message['request_type'] == 'get_agents':
             #TODO: check for initialization
             reply_to = headers['reply-to']
             message_bus.send(reply_to, self.registered_agents)
-            
+
         elif message['request_type'] == 'is_initialized':
             reply_to = headers['reply-to']
-            message = {'initialized':True}
+            message = {'initialized': True}
             message_bus.send(reply_to, message)
 
         elif message['request_type'] == 'control_command':
             simulation_id = message['input']['simulation_id']
-            self.ot_connection.send(t.simulation_input_topic(simulation_id),
-                                    message)
+            self.ot_connection.send(t.simulation_input_topic(simulation_id), message)
 
 
 class SecondaryAreaContextManager(SecondaryAreaAgent):
 
     def __init__(self,
                  upstream_message_bus_def: MessageBusDefinition,
                  downstream_message_bus_def: MessageBusDefinition,
                  agent_config: Dict,
                  secondary_area_dict: Dict = None,
                  simulation_id: str = None):
 
         self.ot_connection = GridAPPSD()
         if secondary_area_dict is None:
-            request = {'request_type':'get_context',
-                       'areaId': downstream_message_bus_def.id}
-            secondary_area_dict = self.ot_connection.get_response(
-                REQUEST_FIELD, request, timeout=10)['data']
+            request = {'request_type': 'get_context', 'areaId': downstream_message_bus_def.id}
+            secondary_area_dict = self.ot_connection.get_response(REQUEST_FIELD,
+                                                                  request,
+                                                                  timeout=10)['data']
 
-        super().__init__(upstream_message_bus_def, downstream_message_bus_def,
-                         agent_config, secondary_area_dict, simulation_id)
+        super().__init__(upstream_message_bus_def, downstream_message_bus_def, agent_config,
+                         secondary_area_dict, simulation_id)
 
         #Override agent_id to a static value
         self.agent_id = downstream_message_bus_def.id + '.context_manager'
-        
+
         self.context = None
 
         self.registered_agents = {}
         self.registered_agents[self.agent_id] = self.get_registration_details()
+        self.ot_connection.get_logger().info("Secondary Area "+self.agent_id+" Context Manager Created")
 
     def on_request(self, message_bus, headers: Dict, message):
 
         _log.debug(f"Received request: {message}")
         _log.debug(f"Received request: {headers}")
 
         if message['request_type'] == 'get_context':
             reply_to = headers['reply-to']
             if self.context is None:
                 self.context = self.ot_connection.get_response(REQUEST_FIELD, message)
-            message_bus.send(reply_to,self.context)
-
+            message_bus.send(reply_to, self.context)
 
         elif message['request_type'] == 'register_agent':
             self.ot_connection.send(t.REGISTER_AGENT_QUEUE, message)
-            self.registered_agents[message['agent']
-                                   ['agent_id']] = message['agent']
+            self.registered_agents[message['agent']['agent_id']] = message['agent']
 
         elif message['request_type'] == 'get_agents':
             reply_to = headers['reply-to']
             message_bus.send(reply_to, self.registered_agents)
 
         elif message['request_type'] == 'is_initialized':
             reply_to = headers['reply-to']
-            message = {'initialized':True}
+            message = {'initialized': True}
             message_bus.send(reply_to, message)
 
         elif message['request_type'] == 'control_command':
             simulation_id = message['input']['simulation_id']
-            self.ot_connection.send(t.simulation_input_topic(simulation_id),
-                                    message)
+            self.ot_connection.send(t.simulation_input_topic(simulation_id), message)
+
 
 def get_MessageBusDefinition(area_id: str) -> MessageBusDefinition:
-    
-    connection_args = {"GRIDAPPSD_ADDRESS": os.environ.get('GRIDAPPSD_ADDRESS',"tcp://gridappsd:61613"),
-                       "GRIDAPPSD_USER": os.environ.get('GRIDAPPSD_USER'),
-                       "GRIDAPPSD_PASSWORD": os.environ.get('GRIDAPPSD_PASSWORD'),
-                       "GRIDAPPSD_APPLICATION_ID": os.environ.get('GRIDAPPSD_APPLICATION_ID')}
-    
-    bus = MessageBusDefinition(id=area_id, 
-                               is_ot_bus= True, 
-                               connection_type = "GRIDAPPSD_TYPE_GRIDAPPSD",
-                               conneciton_args = connection_args)
-    
+
+    connection_args = {
+        "GRIDAPPSD_ADDRESS": os.environ.get('GRIDAPPSD_ADDRESS', "tcp://gridappsd:61613"),
+        "GRIDAPPSD_USER": os.environ.get('GRIDAPPSD_USER'),
+        "GRIDAPPSD_PASSWORD": os.environ.get('GRIDAPPSD_PASSWORD'),
+        "GRIDAPPSD_APPLICATION_ID": os.environ.get('GRIDAPPSD_APPLICATION_ID')
+    }
+
+    bus = MessageBusDefinition(id=area_id,
+                               is_ot_bus=True,
+                               connection_type="GRIDAPPSD_TYPE_GRIDAPPSD",
+                               conneciton_args=connection_args)
+
     return bus
 
+
 def _main():
 
     time.sleep(10)
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "--simulation_id",
-        help=
-        "Simulation id to use for communicating with simulated devices on the message bus. \
+        help="Simulation id to use for communicating with simulated devices on the message bus. \
                         If simulation_id is not provided then Context Manager assumes to run on deployed field with real devices.",
         required=False)
     opts = parser.parse_args()
     simulation_id = opts.simulation_id
 
     agent_config = {
         "app_id":
         "context_manager",
         "description":
         "This agent provides topological context information like neighboring agents and devices to other distributed agents"
     }
 
-
     gapps = GridAPPSD()
-    response = gapps.get_response(t.PLATFORM_STATUS, {"isField":True})
+    response = gapps.get_response(t.PLATFORM_STATUS, {"isField": True})
     field_model_mrid = response['fieldModelMrid']
 
     is_field_initialized = False
 
     while not is_field_initialized:
-        response = gapps.get_response(REQUEST_FIELD, {"request_type":"is_initilized"})
+        response = gapps.get_response(REQUEST_FIELD, {"request_type": "is_initilized"})
         print(response)
         is_field_initialized = response['data']['initialized']
         time.sleep(1)
 
     system_message_bus_def = get_MessageBusDefinition(field_model_mrid)
     feeder_message_bus_def = get_MessageBusDefinition(field_model_mrid)
 
     #TODO: create access control for agents for different layers
     feeder_agent = FeederAreaContextManager(system_message_bus_def,
                                             feeder_message_bus_def,
                                             agent_config,
                                             simulation_id=simulation_id)
 
-
-
     for switch_area in feeder_agent.agent_area_dict['switch_areas']:
         switch_area_message_bus_def = get_MessageBusDefinition(str(switch_area['message_bus_id']))
-        print("Creating switch area agent " +
-              str(switch_area['message_bus_id']))
-        switch_area_agent = SwitchAreaContextManager(
-            feeder_message_bus_def,
-            switch_area_message_bus_def,
-            agent_config,
-            simulation_id=simulation_id)
-    
+        print("Creating switch area agent " + str(switch_area['message_bus_id']))
+        switch_area_agent = SwitchAreaContextManager(feeder_message_bus_def,
+                                                     switch_area_message_bus_def,
+                                                     agent_config,
+                                                     simulation_id=simulation_id)
+
         # create secondary area distributed agents
         for secondary_area in switch_area['secondary_areas']:
-            secondary_area_message_bus_def = get_MessageBusDefinition(str(secondary_area['message_bus_id']))
-            print("Creating secondary area agent " +
-                  str(secondary_area['message_bus_id']))
-            secondary_area_agent = SecondaryAreaContextManager(
-                switch_area_message_bus_def,
-                secondary_area_message_bus_def,
-                agent_config,
-                simulation_id=simulation_id)
+            secondary_area_message_bus_def = get_MessageBusDefinition(
+                str(secondary_area['message_bus_id']))
+            print("Creating secondary area agent " + str(secondary_area['message_bus_id']))
+            secondary_area_agent = SecondaryAreaContextManager(switch_area_message_bus_def,
+                                                               secondary_area_message_bus_def,
+                                                               agent_config,
+                                                               simulation_id=simulation_id)
 
     while True:
         try:
             time.sleep(0.1)
         except KeyboardInterrupt:
             print("Exiting sample")
             break
```

### Comparing `gridappsd_field_bus-2024.1.4a0/gridappsd/field_interface/gridappsd_field_bus.py` & `gridappsd_field_bus-2024.4.0a0/gridappsd/field_interface/gridappsd_field_bus.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from gridappsd import GridAPPSD
 from gridappsd.field_interface.interfaces import FieldMessageBus
 from gridappsd.field_interface.interfaces import MessageBusDefinition
 from typing import Any
 
 
 class GridAPPSDMessageBus(FieldMessageBus):
+
     def __init__(self, definition: MessageBusDefinition):
         super(GridAPPSDMessageBus, self).__init__(definition)
         self._id = definition.id
 
         self._user = definition.conneciton_args["GRIDAPPSD_USER"]
         self._password = definition.conneciton_args["GRIDAPPSD_PASSWORD"]
         self._address = definition.conneciton_args["GRIDAPPSD_ADDRESS"]
 
         self.gridappsd_obj = None
-        
+
     def query_devices(self) -> dict:
         pass
 
     def is_connected(self) -> bool:
         """
         Is this object connected to the message bus
         """
@@ -39,20 +40,20 @@
 
     def send(self, topic: str, message: Any):
         """
         Publish device specific data to the concrete message bus.
         """
         if self.gridappsd_obj is not None:
             self.gridappsd_obj.send(topic, message)
-            
+
     def get_response(self, topic, message, timeout=5):
         """
         Sends a message on a specific concrete queue, waits and returns the response
         """
         if self.gridappsd_obj is not None:
             return self.gridappsd_obj.get_response(topic, message, timeout)
-        
+
     def disconnect(self):
         """
         Disconnect from the concrete message bus.
         """
         self.gridappsd_obj.disconnect()
```

### Comparing `gridappsd_field_bus-2024.1.4a0/gridappsd/field_interface/interfaces.py` & `gridappsd_field_bus-2024.4.0a0/gridappsd/field_interface/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,18 +5,16 @@
 from enum import Enum
 import gridappsd.topics as t
 import logging
 from os import PathLike
 from pathlib import Path
 from typing import Dict, List, Optional, Union
 
-
 import yaml
 
-
 _log = logging.getLogger(__name__)
 
 
 class FieldProtocol(Enum):
     PROTOCOL_2030_5 = "2030.5"
     PROTOCOL_DNP3 = "DNP3"
 
@@ -33,14 +31,15 @@
     # CONNECTION_TYPE_WS = "WS"
     # CONNECTION_TYPE_HTTP = "HTTP"
     # CONNECTION_TYPE_TCP = "TCP"
     CONNECTION_TYPE_GRIDAPPSD = "CONNECTION_TYPE_GRIDAPPSD"
 
 
 class ProtocolTransformer(ABC):
+
     @staticmethod
     @abstractmethod
     def to_cim(data) -> str:
         """
         Create a cim message based upon the data passed for a given
         concrete protocol.  This is set as a static class because
         all transformers should have this capability.
@@ -54,75 +53,72 @@
     @abstractmethod
     def to_protocol(cim_data: str, from_format: Optional[str] = None):
         """
         Change passed cim data into a protocol complient data stream
         and return it.
 
         cim_data: string representing cim data structures/change structure
-        from_format: specifies the type 
+        from_format: specifies the type
         """
         pass
 
 
-
 @dataclass
 class MessageBusDefinition:
     """
     A `MessageBusDefinition` class is used to define how to connect to the
     message bus.
     """
-
     """
     A global unique string representing a specific message bus.
     """
     id: str
-
     """
     connection_type describes how the agent/endpoint will connect to the message bus
     """
     connection_type: ConnectionType
-
     """
     connection_args allows dynamic key/value paired strings to be added to allow connections.
     """
     conneciton_args: Dict[str, str]
-
     """
     Determines whether or not this message bus has the role of ot bus.
     """
     is_ot_bus: bool = False
 
     @staticmethod
     def load(config_file) -> MessageBusDefinition:
         """
 
         """
-        config = yaml.load(open(config_file),Loader=yaml.FullLoader)['connections']
-        
+        config = yaml.load(open(config_file), Loader=yaml.FullLoader)['connections']
+
         required = ["id", "connection_type", "connection_args"]
         for k in required:
             if k not in config:
                 raise ValueError(f"Missing keys for connection {k}")
 
-        definition = MessageBusDefinition(config[required[0]], config[required[1]], config[required[2]])
+        definition = MessageBusDefinition(config[required[0]], config[required[1]],
+                                          config[required[2]])
         for k in config:
             if k == "connection_args":
                 definition.conneciton_args = dict()
                 for k1, v1 in config[k].items():
                     definition.conneciton_args[k1] = v1
             else:
                 setattr(definition, k, config[k])
 
         if not hasattr(definition, "is_ot_bus"):
             setattr(definition, "is_ot_bus", False)
-            
+
         return definition
 
 
 class FieldMessageBus:
+
     def __init__(self, config: MessageBusDefinition):
         self._devices = dict()
         self._is_ot_bus = config.is_ot_bus
         self._id = config.id
 
     @property
     def id(self):
@@ -166,37 +162,38 @@
 
     @abstractmethod
     def send(self, topic, message):
         """
         Publish device specific message to the concrete message bus.
         """
         pass
-    
+
     @abstractmethod
     def get_response(self, topic, message, timeout):
         """
         Sends a message on a specific queue, waits and returns the response
         """
-        
+
     def get_agent_response(self, agent_id, message, timeout):
         """
         Sends a message on a specific agent's request queue, waits and returns the response
         """
-        topic = "{}.request.{}.{}".format(t.BASE_FIELD_QUEUE,self.id, agent_id)
+        topic = "{}.request.{}.{}".format(t.BASE_FIELD_QUEUE, self.id, agent_id)
         self.get_response(topic, message, timeout)
 
     @abstractmethod
     def disconnect(self):
         """
         Disconnect the device from the concrete message bus.
         """
         pass
 
 
 class MessageBusDefinitions:
+
     def __init__(
         self,
         config: Optional[Union[dict, str]] = None,
         yamlfile: Optional[Union[str, PathLike]] = None,
     ):
         self._buses = dict()
 
@@ -241,14 +238,15 @@
             self._iterator = None
             return None
         else:
             return definition
 
 
 class DeviceFieldInterface:
+
     def __init__(
         self,
         id: str,
         field_bus: FieldMessageBus,
         publish_topic: str,
         control_topic: str,
     ):
@@ -277,10 +275,10 @@
     def on_control_message(self, message):
         pass
 
     @abstractmethod
     def on_state_change(self):
         """
         This event should be triggered by the device/protocol that
-        is used.  
+        is used.
         """
         pass
```

### Comparing `gridappsd_field_bus-2024.1.4a0/pyproject.toml` & `gridappsd_field_bus-2024.4.0a0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridappsd-field-bus"
-version = "2024.1.4a0"
+version = "2024.4.0a0"
 description = "GridAPPS-D Field Bus Implementation"
 authors = [
     "C. Allwardt <3979063+craig8@users.noreply.github.com>",
     "P. Sharma <poorva.sharma@pnnl.gov",
     "A. Fisher <andrew.fisher@pnnl.gov"
 ]
 license = "BSD-3-Clause"
@@ -24,15 +24,15 @@
 [tool.poetry.scripts]
 # Add things in the form
 # myscript = 'my_package:main'
 context_manager = 'gridappsd.field_interface.context_manager:_main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-gridappsd-python = "^2024.1.4a0"
+gridappsd-python = "^2024.4.0a0"
 cim-graph = ">=0.1.1a0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.2.2"
 pytest-html = "^3.1.1"
 mock = "^4.0.3"
 docker = "^4.4.4"
```

### Comparing `gridappsd_field_bus-2024.1.4a0/PKG-INFO` & `gridappsd_field_bus-2024.4.0a0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: gridappsd-field-bus
-Version: 2024.1.4a0
+Version: 2024.4.0a0
 Summary: GridAPPS-D Field Bus Implementation
 Home-page: https://gridappsd.readthedocs.io
 License: BSD-3-Clause
 Keywords: gridappsd,grid,activmq,powergrid,simulation,library
 Author: C. Allwardt
 Author-email: 3979063+craig8@users.noreply.github.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cim-graph (>=0.1.1a0)
-Requires-Dist: gridappsd-python (>=2024.1.4a0,<2025.0.0)
+Requires-Dist: gridappsd-python (>=2024.4.0a0,<2025.0.0)
 Project-URL: Repository, https://github.com/GRIDAPPSD/gridappsd-python
 Description-Content-Type: text/markdown
```

