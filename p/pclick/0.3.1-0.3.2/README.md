# Comparing `tmp/pclick-0.3.1.tar.gz` & `tmp/pclick-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pclick-0.3.1.tar", max compression
+gzip compressed data, was "pclick-0.3.2.tar", max compression
```

## Comparing `pclick-0.3.1.tar` & `pclick-0.3.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1369 2023-06-08 10:28:44.943628 pclick-0.3.1/README.md
--rw-r--r--   0        0        0      535 2024-03-22 14:00:24.678985 pclick-0.3.1/pyproject.toml
--rw-r--r--   0        0        0    10259 2024-03-22 14:12:14.908811 pclick-0.3.1/src/pclick/Messaging_pb2.py
--rw-r--r--   0        0        0      527 2023-12-05 15:27:56.829113 pclick-0.3.1/src/pclick/__init__.py
--rw-r--r--   0        0        0     1087 2023-06-07 20:19:13.578644 pclick-0.3.1/src/pclick/client.py
--rw-r--r--   0        0        0        0 2024-03-22 14:14:52.024331 pclick-0.3.1/src/pclick/demo/__init__.py
--rw-r--r--   0        0        0     4818 2023-12-15 11:26:19.083865 pclick-0.3.1/src/pclick/demo/client.py
--rw-r--r--   0        0        0     3877 2023-12-05 15:27:56.833113 pclick-0.3.1/src/pclick/demo/server.py
--rw-r--r--   0        0        0     2014 2023-06-07 20:19:13.578644 pclick-0.3.1/src/pclick/message_proto_helpers.py
--rw-r--r--   0        0        0     2537 2023-11-29 07:42:34.134245 pclick-0.3.1/src/pclick/server.py
--rw-r--r--   0        0        0     2157 1970-01-01 00:00:00.000000 pclick-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1369 2023-06-08 10:28:35.050860 pclick-0.3.2/README.md
+-rw-r--r--   0        0        0      535 2024-05-02 07:26:05.585878 pclick-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0    10552 2024-05-02 07:40:13.328416 pclick-0.3.2/src/pclick/Messaging_pb2.py
+-rw-r--r--   0        0        0      527 2023-12-05 15:25:16.273440 pclick-0.3.2/src/pclick/__init__.py
+-rw-r--r--   0        0        0     1087 2023-06-07 20:19:52.403023 pclick-0.3.2/src/pclick/client.py
+-rw-r--r--   0        0        0        0 2024-05-02 07:41:23.094497 pclick-0.3.2/src/pclick/demo/__init__.py
+-rw-r--r--   0        0        0     4818 2023-12-15 11:26:07.254777 pclick-0.3.2/src/pclick/demo/client.py
+-rw-r--r--   0        0        0     3877 2023-12-05 15:25:16.273440 pclick-0.3.2/src/pclick/demo/server.py
+-rw-r--r--   0        0        0     2014 2023-06-07 20:19:52.403023 pclick-0.3.2/src/pclick/message_proto_helpers.py
+-rw-r--r--   0        0        0     2537 2023-11-29 07:44:10.171067 pclick-0.3.2/src/pclick/server.py
+-rw-r--r--   0        0        0     2157 1970-01-01 00:00:00.000000 pclick-0.3.2/PKG-INFO
```

### Comparing `pclick-0.3.1/README.md` & `pclick-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `pclick-0.3.1/pyproject.toml` & `pclick-0.3.2/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "pclick"
-version = "0.3.1"
+version = "0.3.2"
 description = "Controller to AGX Dynamics messaging"
 authors = ["Algoryx Simulation <contact@algoryx.se>"]
 license = "Apache-2.0"
 repository = "https://github.com/algoryx/click-mirror"
 readme = "README.md"
 packages = [
     { include = "pclick", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
-protobuf = "3.20.3"
+protobuf = "5.26.1"
 pyzmq = "22.3.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^6.2.4"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `pclick-0.3.1/src/pclick/Messaging_pb2.py` & `pclick-0.3.2/src/pclick/Messaging_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0fMessaging.proto\x12\x0e\x63lick.protobuf\"G\n\x07Message\x12\x30\n\x0bmessageType\x18\x01 \x01(\x0e\x32\x1b.click.protobuf.MessageType\x12\n\n\x02id\x18\x02 \x01(\x05\"r\n\x14HandshakeInitMessage\x12\x30\n\x0bmessageType\x18\x01 \x01(\x0e\x32\x1b.click.protobuf.MessageType\x12(\n\x07version\x18\x02 \x01(\x0e\x32\x17.click.protobuf.Version\"H\n\x14SensorRequestMessage\x12\x30\n\x0bmessageType\x18\x01 \x01(\x0e\x32\x1b.click.protobuf.MessageType\"\xff\x07\n\x10HandshakeMessage\x12\x30\n\x0bmessageType\x18\x01 \x01(\x0e\x32\x1b.click.protobuf.MessageType\x12(\n\x07version\x18\x02 \x01(\x0e\x32\x17.click.protobuf.Version\x12.\n\x0b\x63ontrolType\x18\x03 \x01(\x0e\x32\x19.click.protobuf.ValueType\x12>\n\x07objects\x18\x04 \x03(\x0b\x32-.click.protobuf.HandshakeMessage.ObjectsEntry\x12H\n\x0bsimSettings\x18\x05 \x01(\x0b\x32\x33.click.protobuf.HandshakeMessage.SimulationSettings\x1a\x33\n\x07Sensors\x12(\n\x05types\x18\x01 \x03(\x0e\x32\x19.click.protobuf.ValueType\x1a\x9e\x04\n\x06Object\x12\x17\n\x0f\x63ontrolsInOrder\x18\x01 \x03(\t\x12\x36\n\x13\x63ontrolTypesInOrder\x18\x08 \x03(\x0e\x32\x19.click.protobuf.ValueType\x12\x1b\n\x13jointSensorsInOrder\x18\x07 \x03(\t\x12/\n\x0cjointSensors\x18\x02 \x03(\x0e\x32\x19.click.protobuf.ValueType\x12Q\n\rcontrolEvents\x18\x03 \x03(\x0b\x32:.click.protobuf.HandshakeMessage.Object.ControlEventsEntry\x12\x45\n\x07sensors\x18\x04 \x03(\x0b\x32\x34.click.protobuf.HandshakeMessage.Object.SensorsEntry\x12\x30\n\robjectSensors\x18\x06 \x03(\x0e\x32\x19.click.protobuf.ValueType\x1aO\n\x12\x43ontrolEventsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12(\n\x05value\x18\x02 \x01(\x0e\x32\x19.click.protobuf.ValueType:\x02\x38\x01\x1aX\n\x0cSensorsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x37\n\x05value\x18\x02 \x01(\x0b\x32(.click.protobuf.HandshakeMessage.Sensors:\x02\x38\x01\x1a&\n\x12SimulationSettings\x12\x10\n\x08timeStep\x18\x01 \x01(\x01\x1aW\n\x0cObjectsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x36\n\x05value\x18\x02 \x01(\x0b\x32\'.click.protobuf.HandshakeMessage.Object:\x02\x38\x01\"\xb3\x03\n\x0e\x43ontrolMessage\x12\x30\n\x0bmessageType\x18\x01 \x01(\x0e\x32\x1b.click.protobuf.MessageType\x12<\n\x07objects\x18\x02 \x03(\x0b\x32+.click.protobuf.ControlMessage.ObjectsEntry\x1a\xd9\x01\n\x06Object\x12\x0e\n\x06\x61ngles\x18\x01 \x03(\x01\x12\x17\n\x0f\x61ngleVelocities\x18\x02 \x03(\x01\x12\x0f\n\x07torques\x18\x03 \x03(\x01\x12\x0e\n\x06values\x18\x05 \x03(\x01\x12O\n\rcontrolEvents\x18\x04 \x03(\x0b\x32\x38.click.protobuf.ControlMessage.Object.ControlEventsEntry\x1a\x34\n\x12\x43ontrolEventsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x08:\x02\x38\x01\x1aU\n\x0cObjectsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x34\n\x05value\x18\x02 \x01(\x0b\x32%.click.protobuf.ControlMessage.Object:\x02\x38\x01\"\xc9\t\n\rSensorMessage\x12\x30\n\x0bmessageType\x18\x01 \x01(\x0e\x32\x1b.click.protobuf.MessageType\x12;\n\x07objects\x18\x03 \x03(\x0b\x32*.click.protobuf.SensorMessage.ObjectsEntry\x12\x42\n\x07simVars\x18\x04 \x01(\x0b\x32\x31.click.protobuf.SensorMessage.SimulationVariables\x1a\x13\n\x04Vec3\x12\x0b\n\x03\x61rr\x18\x01 \x03(\x01\x1a\xc2\x03\n\x06Sensor\x12\x0f\n\x05\x61ngle\x18\x01 \x01(\x01H\x00\x12\x17\n\rangleVelocity\x18\x02 \x01(\x01H\x00\x12\x10\n\x06torque\x18\x03 \x01(\x01H\x00\x12\x36\n\x08position\x18\x04 \x01(\x0b\x32\".click.protobuf.SensorMessage.Vec3H\x00\x12\x31\n\x03rpy\x18\x05 \x01(\x0b\x32\".click.protobuf.SensorMessage.Vec3H\x00\x12\x13\n\tactivated\x18\x06 \x01(\x08H\x00\x12:\n\x0c\x61\x63\x63\x65leration\x18\x07 \x01(\x0b\x32\".click.protobuf.SensorMessage.Vec3H\x00\x12\x33\n\x05\x66orce\x18\x08 \x01(\x0b\x32\".click.protobuf.SensorMessage.Vec3H\x00\x12?\n\x11\x64irectionalTorque\x18\t \x01(\x0b\x32\".click.protobuf.SensorMessage.Vec3H\x00\x12\x41\n\x13\x61ngularAcceleration\x18\n \x01(\x0b\x32\".click.protobuf.SensorMessage.Vec3H\x00\x42\x07\n\x05value\x1a?\n\x07Sensors\x12\x34\n\x06sensor\x18\x01 \x03(\x0b\x32$.click.protobuf.SensorMessage.Sensor\x1a\xe5\x02\n\x06Object\x12\x14\n\x0c\x61ngleSensors\x18\x01 \x03(\x01\x12\x1c\n\x14\x61ngleVelocitySensors\x18\x02 \x03(\x01\x12\x15\n\rtorqueSensors\x18\x03 \x03(\x01\x12\x38\n\x0c\x66orceSensors\x18\x05 \x03(\x0b\x32\".click.protobuf.SensorMessage.Vec3\x12;\n\robjectSensors\x18\x04 \x03(\x0b\x32$.click.protobuf.SensorMessage.Sensor\x12\x42\n\x07sensors\x18\x06 \x03(\x0b\x32\x31.click.protobuf.SensorMessage.Object.SensorsEntry\x1aU\n\x0cSensorsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x34\n\x05value\x18\x02 \x01(\x0b\x32%.click.protobuf.SensorMessage.Sensors:\x02\x38\x01\x1a,\n\x13SimulationVariables\x12\x15\n\rsimulatedTime\x18\x01 \x01(\x01\x1aT\n\x0cObjectsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x33\n\x05value\x18\x02 \x01(\x0b\x32$.click.protobuf.SensorMessage.Object:\x02\x38\x01\"@\n\x0cResetMessage\x12\x30\n\x0bmessageType\x18\x01 \x01(\x0e\x32\x1b.click.protobuf.MessageType\"\x80\x01\n\x0c\x45rrorMessage\x12\x30\n\x0bmessageType\x18\x01 \x01(\x0e\x32\x1b.click.protobuf.MessageType\x12(\n\x05\x65rror\x18\x02 \x01(\x0e\x32\x19.click.protobuf.ErrorType\x12\x14\n\x0c\x65rrormessage\x18\x03 \x01(\t*\xbe\x01\n\x0bMessageType\x12\x1c\n\x18HandshakeInitMessageType\x10\x00\x12\x18\n\x14HandshakeMessageType\x10\x01\x12\x1c\n\x18SensorRequestMessageType\x10\x06\x12\x16\n\x12\x43ontrolMessageType\x10\x02\x12\x15\n\x11SensorMessageType\x10\x03\x12\x14\n\x10ResetMessageType\x10\x04\x12\x14\n\x10\x45rrorMessageType\x10\x05*\xb6\x01\n\tValueType\x12\t\n\x05\x41ngle\x10\x00\x12\x11\n\rAngleVelocity\x10\x01\x12\n\n\x06Torque\x10\x02\x12\x0c\n\x08Position\x10\x03\x12\x07\n\x03RPY\x10\x04\x12\r\n\tActivated\x10\x05\x12\x10\n\x0c\x41\x63\x63\x65leration\x10\x06\x12\t\n\x05\x46orce\x10\x07\x12\x15\n\x11\x44irectionalTorque\x10\x08\x12\x17\n\x13\x41ngularAcceleration\x10\t\x12\x0c\n\x08Multiple\x10\x0f*-\n\x07Version\x12\r\n\tUNDEFINED\x10\x00\x12\x13\n\x0f\x43URRENT_VERSION\x10\x01*$\n\tErrorType\x12\x17\n\x13VersionNotSupported\x10\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0fMessaging.proto\x12\x0e\x63lick.protobuf\"G\n\x07Message\x12\x30\n\x0bmessageType\x18\x01 \x01(\x0e\x32\x1b.click.protobuf.MessageType\x12\n\n\x02id\x18\x02 \x01(\x05\"r\n\x14HandshakeInitMessage\x12\x30\n\x0bmessageType\x18\x01 \x01(\x0e\x32\x1b.click.protobuf.MessageType\x12(\n\x07version\x18\x02 \x01(\x0e\x32\x17.click.protobuf.Version\"H\n\x14SensorRequestMessage\x12\x30\n\x0bmessageType\x18\x01 \x01(\x0e\x32\x1b.click.protobuf.MessageType\"\xff\x07\n\x10HandshakeMessage\x12\x30\n\x0bmessageType\x18\x01 \x01(\x0e\x32\x1b.click.protobuf.MessageType\x12(\n\x07version\x18\x02 \x01(\x0e\x32\x17.click.protobuf.Version\x12.\n\x0b\x63ontrolType\x18\x03 \x01(\x0e\x32\x19.click.protobuf.ValueType\x12>\n\x07objects\x18\x04 \x03(\x0b\x32-.click.protobuf.HandshakeMessage.ObjectsEntry\x12H\n\x0bsimSettings\x18\x05 \x01(\x0b\x32\x33.click.protobuf.HandshakeMessage.SimulationSettings\x1a\x33\n\x07Sensors\x12(\n\x05types\x18\x01 \x03(\x0e\x32\x19.click.protobuf.ValueType\x1a\x9e\x04\n\x06Object\x12\x17\n\x0f\x63ontrolsInOrder\x18\x01 \x03(\t\x12\x36\n\x13\x63ontrolTypesInOrder\x18\x08 \x03(\x0e\x32\x19.click.protobuf.ValueType\x12\x1b\n\x13jointSensorsInOrder\x18\x07 \x03(\t\x12/\n\x0cjointSensors\x18\x02 \x03(\x0e\x32\x19.click.protobuf.ValueType\x12Q\n\rcontrolEvents\x18\x03 \x03(\x0b\x32:.click.protobuf.HandshakeMessage.Object.ControlEventsEntry\x12\x45\n\x07sensors\x18\x04 \x03(\x0b\x32\x34.click.protobuf.HandshakeMessage.Object.SensorsEntry\x12\x30\n\robjectSensors\x18\x06 \x03(\x0e\x32\x19.click.protobuf.ValueType\x1aO\n\x12\x43ontrolEventsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12(\n\x05value\x18\x02 \x01(\x0e\x32\x19.click.protobuf.ValueType:\x02\x38\x01\x1aX\n\x0cSensorsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x37\n\x05value\x18\x02 \x01(\x0b\x32(.click.protobuf.HandshakeMessage.Sensors:\x02\x38\x01\x1a&\n\x12SimulationSettings\x12\x10\n\x08timeStep\x18\x01 \x01(\x01\x1aW\n\x0cObjectsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x36\n\x05value\x18\x02 \x01(\x0b\x32\'.click.protobuf.HandshakeMessage.Object:\x02\x38\x01\"\xb3\x03\n\x0e\x43ontrolMessage\x12\x30\n\x0bmessageType\x18\x01 \x01(\x0e\x32\x1b.click.protobuf.MessageType\x12<\n\x07objects\x18\x02 \x03(\x0b\x32+.click.protobuf.ControlMessage.ObjectsEntry\x1a\xd9\x01\n\x06Object\x12\x0e\n\x06\x61ngles\x18\x01 \x03(\x01\x12\x17\n\x0f\x61ngleVelocities\x18\x02 \x03(\x01\x12\x0f\n\x07torques\x18\x03 \x03(\x01\x12\x0e\n\x06values\x18\x05 \x03(\x01\x12O\n\rcontrolEvents\x18\x04 \x03(\x0b\x32\x38.click.protobuf.ControlMessage.Object.ControlEventsEntry\x1a\x34\n\x12\x43ontrolEventsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\x08:\x02\x38\x01\x1aU\n\x0cObjectsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x34\n\x05value\x18\x02 \x01(\x0b\x32%.click.protobuf.ControlMessage.Object:\x02\x38\x01\"\xd6\n\n\rSensorMessage\x12\x30\n\x0bmessageType\x18\x01 \x01(\x0e\x32\x1b.click.protobuf.MessageType\x12;\n\x07objects\x18\x03 \x03(\x0b\x32*.click.protobuf.SensorMessage.ObjectsEntry\x12\x42\n\x07simVars\x18\x04 \x01(\x0b\x32\x31.click.protobuf.SensorMessage.SimulationVariables\x1a\x13\n\x04Vec3\x12\x0b\n\x03\x61rr\x18\x01 \x03(\x01\x1a\xcf\x04\n\x06Sensor\x12\x0f\n\x05\x61ngle\x18\x01 \x01(\x01H\x00\x12\x17\n\rangleVelocity\x18\x02 \x01(\x01H\x00\x12\x10\n\x06torque\x18\x03 \x01(\x01H\x00\x12\x36\n\x08position\x18\x04 \x01(\x0b\x32\".click.protobuf.SensorMessage.Vec3H\x00\x12\x31\n\x03rpy\x18\x05 \x01(\x0b\x32\".click.protobuf.SensorMessage.Vec3H\x00\x12\x13\n\tactivated\x18\x06 \x01(\x08H\x00\x12:\n\x0c\x61\x63\x63\x65leration\x18\x07 \x01(\x0b\x32\".click.protobuf.SensorMessage.Vec3H\x00\x12\x33\n\x05\x66orce\x18\x08 \x01(\x0b\x32\".click.protobuf.SensorMessage.Vec3H\x00\x12?\n\x11\x64irectionalTorque\x18\t \x01(\x0b\x32\".click.protobuf.SensorMessage.Vec3H\x00\x12\x41\n\x13\x61ngularAcceleration\x18\n \x01(\x0b\x32\".click.protobuf.SensorMessage.Vec3H\x00\x12\x41\n\x13\x64irectionalVelocity\x18\x0c \x01(\x0b\x32\".click.protobuf.SensorMessage.Vec3H\x00\x12H\n\x1a\x64irectionalAngularVelocity\x18\r \x01(\x0b\x32\".click.protobuf.SensorMessage.Vec3H\x00\x42\x07\n\x05value\x1a?\n\x07Sensors\x12\x34\n\x06sensor\x18\x01 \x03(\x0b\x32$.click.protobuf.SensorMessage.Sensor\x1a\xe5\x02\n\x06Object\x12\x14\n\x0c\x61ngleSensors\x18\x01 \x03(\x01\x12\x1c\n\x14\x61ngleVelocitySensors\x18\x02 \x03(\x01\x12\x15\n\rtorqueSensors\x18\x03 \x03(\x01\x12\x38\n\x0c\x66orceSensors\x18\x05 \x03(\x0b\x32\".click.protobuf.SensorMessage.Vec3\x12;\n\robjectSensors\x18\x04 \x03(\x0b\x32$.click.protobuf.SensorMessage.Sensor\x12\x42\n\x07sensors\x18\x06 \x03(\x0b\x32\x31.click.protobuf.SensorMessage.Object.SensorsEntry\x1aU\n\x0cSensorsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x34\n\x05value\x18\x02 \x01(\x0b\x32%.click.protobuf.SensorMessage.Sensors:\x02\x38\x01\x1a,\n\x13SimulationVariables\x12\x15\n\rsimulatedTime\x18\x01 \x01(\x01\x1aT\n\x0cObjectsEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\x33\n\x05value\x18\x02 \x01(\x0b\x32$.click.protobuf.SensorMessage.Object:\x02\x38\x01\"@\n\x0cResetMessage\x12\x30\n\x0bmessageType\x18\x01 \x01(\x0e\x32\x1b.click.protobuf.MessageType\"\x80\x01\n\x0c\x45rrorMessage\x12\x30\n\x0bmessageType\x18\x01 \x01(\x0e\x32\x1b.click.protobuf.MessageType\x12(\n\x05\x65rror\x18\x02 \x01(\x0e\x32\x19.click.protobuf.ErrorType\x12\x14\n\x0c\x65rrormessage\x18\x03 \x01(\t*\xbe\x01\n\x0bMessageType\x12\x1c\n\x18HandshakeInitMessageType\x10\x00\x12\x18\n\x14HandshakeMessageType\x10\x01\x12\x1c\n\x18SensorRequestMessageType\x10\x06\x12\x16\n\x12\x43ontrolMessageType\x10\x02\x12\x15\n\x11SensorMessageType\x10\x03\x12\x14\n\x10ResetMessageType\x10\x04\x12\x14\n\x10\x45rrorMessageType\x10\x05*\xef\x01\n\tValueType\x12\t\n\x05\x41ngle\x10\x00\x12\x11\n\rAngleVelocity\x10\x01\x12\n\n\x06Torque\x10\x02\x12\x0c\n\x08Position\x10\x03\x12\x07\n\x03RPY\x10\x04\x12\r\n\tActivated\x10\x05\x12\x10\n\x0c\x41\x63\x63\x65leration\x10\x06\x12\t\n\x05\x46orce\x10\x07\x12\x15\n\x11\x44irectionalTorque\x10\x08\x12\x17\n\x13\x41ngularAcceleration\x10\t\x12\x17\n\x13\x44irectionalVelocity\x10\n\x12\x1e\n\x1a\x44irectionalAngularVelocity\x10\x0b\x12\x0c\n\x08Multiple\x10\x0f*-\n\x07Version\x12\r\n\tUNDEFINED\x10\x00\x12\x13\n\x0f\x43URRENT_VERSION\x10\x01*$\n\tErrorType\x12\x17\n\x13VersionNotSupported\x10\x00\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'Messaging_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   _HANDSHAKEMESSAGE_OBJECT_CONTROLEVENTSENTRY._options = None
@@ -30,22 +30,22 @@
   _CONTROLMESSAGE_OBJECT_CONTROLEVENTSENTRY._serialized_options = b'8\001'
   _CONTROLMESSAGE_OBJECTSENTRY._options = None
   _CONTROLMESSAGE_OBJECTSENTRY._serialized_options = b'8\001'
   _SENSORMESSAGE_OBJECT_SENSORSENTRY._options = None
   _SENSORMESSAGE_OBJECT_SENSORSENTRY._serialized_options = b'8\001'
   _SENSORMESSAGE_OBJECTSENTRY._options = None
   _SENSORMESSAGE_OBJECTSENTRY._serialized_options = b'8\001'
-  _MESSAGETYPE._serialized_start=3188
-  _MESSAGETYPE._serialized_end=3378
-  _VALUETYPE._serialized_start=3381
-  _VALUETYPE._serialized_end=3563
-  _VERSION._serialized_start=3565
-  _VERSION._serialized_end=3610
-  _ERRORTYPE._serialized_start=3612
-  _ERRORTYPE._serialized_end=3648
+  _MESSAGETYPE._serialized_start=3329
+  _MESSAGETYPE._serialized_end=3519
+  _VALUETYPE._serialized_start=3522
+  _VALUETYPE._serialized_end=3761
+  _VERSION._serialized_start=3763
+  _VERSION._serialized_end=3808
+  _ERRORTYPE._serialized_start=3810
+  _ERRORTYPE._serialized_end=3846
   _MESSAGE._serialized_start=35
   _MESSAGE._serialized_end=106
   _HANDSHAKEINITMESSAGE._serialized_start=108
   _HANDSHAKEINITMESSAGE._serialized_end=222
   _SENSORREQUESTMESSAGE._serialized_start=224
   _SENSORREQUESTMESSAGE._serialized_end=296
   _HANDSHAKEMESSAGE._serialized_start=299
@@ -67,27 +67,27 @@
   _CONTROLMESSAGE_OBJECT._serialized_start=1456
   _CONTROLMESSAGE_OBJECT._serialized_end=1673
   _CONTROLMESSAGE_OBJECT_CONTROLEVENTSENTRY._serialized_start=1621
   _CONTROLMESSAGE_OBJECT_CONTROLEVENTSENTRY._serialized_end=1673
   _CONTROLMESSAGE_OBJECTSENTRY._serialized_start=1675
   _CONTROLMESSAGE_OBJECTSENTRY._serialized_end=1760
   _SENSORMESSAGE._serialized_start=1763
-  _SENSORMESSAGE._serialized_end=2988
+  _SENSORMESSAGE._serialized_end=3129
   _SENSORMESSAGE_VEC3._serialized_start=1959
   _SENSORMESSAGE_VEC3._serialized_end=1978
   _SENSORMESSAGE_SENSOR._serialized_start=1981
-  _SENSORMESSAGE_SENSOR._serialized_end=2431
-  _SENSORMESSAGE_SENSORS._serialized_start=2433
-  _SENSORMESSAGE_SENSORS._serialized_end=2496
-  _SENSORMESSAGE_OBJECT._serialized_start=2499
-  _SENSORMESSAGE_OBJECT._serialized_end=2856
-  _SENSORMESSAGE_OBJECT_SENSORSENTRY._serialized_start=2771
-  _SENSORMESSAGE_OBJECT_SENSORSENTRY._serialized_end=2856
-  _SENSORMESSAGE_SIMULATIONVARIABLES._serialized_start=2858
-  _SENSORMESSAGE_SIMULATIONVARIABLES._serialized_end=2902
-  _SENSORMESSAGE_OBJECTSENTRY._serialized_start=2904
-  _SENSORMESSAGE_OBJECTSENTRY._serialized_end=2988
-  _RESETMESSAGE._serialized_start=2990
-  _RESETMESSAGE._serialized_end=3054
-  _ERRORMESSAGE._serialized_start=3057
-  _ERRORMESSAGE._serialized_end=3185
+  _SENSORMESSAGE_SENSOR._serialized_end=2572
+  _SENSORMESSAGE_SENSORS._serialized_start=2574
+  _SENSORMESSAGE_SENSORS._serialized_end=2637
+  _SENSORMESSAGE_OBJECT._serialized_start=2640
+  _SENSORMESSAGE_OBJECT._serialized_end=2997
+  _SENSORMESSAGE_OBJECT_SENSORSENTRY._serialized_start=2912
+  _SENSORMESSAGE_OBJECT_SENSORSENTRY._serialized_end=2997
+  _SENSORMESSAGE_SIMULATIONVARIABLES._serialized_start=2999
+  _SENSORMESSAGE_SIMULATIONVARIABLES._serialized_end=3043
+  _SENSORMESSAGE_OBJECTSENTRY._serialized_start=3045
+  _SENSORMESSAGE_OBJECTSENTRY._serialized_end=3129
+  _RESETMESSAGE._serialized_start=3131
+  _RESETMESSAGE._serialized_end=3195
+  _ERRORMESSAGE._serialized_start=3198
+  _ERRORMESSAGE._serialized_end=3326
 # @@protoc_insertion_point(module_scope)
```

### Comparing `pclick-0.3.1/src/pclick/__init__.py` & `pclick-0.3.2/src/pclick/__init__.py`

 * *Files identical despite different names*

### Comparing `pclick-0.3.1/src/pclick/client.py` & `pclick-0.3.2/src/pclick/client.py`

 * *Files identical despite different names*

### Comparing `pclick-0.3.1/src/pclick/demo/client.py` & `pclick-0.3.2/src/pclick/demo/client.py`

 * *Files identical despite different names*

### Comparing `pclick-0.3.1/src/pclick/demo/server.py` & `pclick-0.3.2/src/pclick/demo/server.py`

 * *Files identical despite different names*

### Comparing `pclick-0.3.1/src/pclick/message_proto_helpers.py` & `pclick-0.3.2/src/pclick/message_proto_helpers.py`

 * *Files identical despite different names*

### Comparing `pclick-0.3.1/src/pclick/server.py` & `pclick-0.3.2/src/pclick/server.py`

 * *Files identical despite different names*

### Comparing `pclick-0.3.1/PKG-INFO` & `pclick-0.3.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pclick
-Version: 0.3.1
+Version: 0.3.2
 Summary: Controller to AGX Dynamics messaging
 Home-page: https://github.com/algoryx/click-mirror
 License: Apache-2.0
 Author: Algoryx Simulation
 Author-email: contact@algoryx.se
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: protobuf (==3.20.3)
+Requires-Dist: protobuf (==5.26.1)
 Requires-Dist: pyzmq (==22.3.0)
 Project-URL: Repository, https://github.com/algoryx/click-mirror
 Description-Content-Type: text/markdown
 
 # Click
 
 The main idea behind click is to enable a non-Brick controller talking to a Brick enabled [AGX Dynamics](https://www.algoryx.se/agx-dynamics/) Simulation in a way configurable by Brick.
```

