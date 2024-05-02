# Comparing `tmp/naimco-0.0.1.tar.gz` & `tmp/naimco-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "naimco-0.0.1.tar", max compression
+gzip compressed data, was "naimco-0.1.0.tar", max compression
```

## Comparing `naimco-0.0.1.tar` & `naimco-0.1.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1082 2023-03-03 22:30:23.553362 naimco-0.0.1/LICENSE
--rw-r--r--   0        0        0     1558 2024-02-23 17:52:39.055320 naimco-0.0.1/README.rst
--rw-r--r--   0        0        0      334 2023-05-25 17:49:11.706729 naimco-0.0.1/naimco/__init__.py
--rw-r--r--   0        0        0     2125 2023-03-16 23:11:31.046835 naimco-0.0.1/naimco/connection.py
--rw-r--r--   0        0        0    14271 2023-05-25 18:04:36.042685 naimco-0.0.1/naimco/controllers.py
--rw-r--r--   0        0        0     9615 2024-01-03 21:25:36.131352 naimco-0.0.1/naimco/core.py
--rw-r--r--   0        0        0     3949 2023-03-10 23:58:31.820099 naimco-0.0.1/naimco/msg_processing.py
--rw-r--r--   0        0        0      650 2024-02-23 17:57:25.023054 naimco-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     2633 1970-01-01 00:00:00.000000 naimco-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1082 2024-05-02 14:22:16.396847 naimco-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1604 2024-05-02 14:22:16.396847 naimco-0.1.0/README.rst
+-rw-r--r--   0        0        0      357 2024-05-02 14:22:16.396847 naimco-0.1.0/naimco/__init__.py
+-rw-r--r--   0        0        0     2116 2024-05-02 14:22:16.396847 naimco-0.1.0/naimco/connection.py
+-rw-r--r--   0        0        0    16178 2024-05-02 14:22:16.396847 naimco-0.1.0/naimco/controllers.py
+-rw-r--r--   0        0        0     9378 2024-05-02 14:22:16.396847 naimco-0.1.0/naimco/core.py
+-rw-r--r--   0        0        0     3995 2024-05-02 14:22:16.400847 naimco-0.1.0/naimco/msg_processing.py
+-rw-r--r--   0        0        0     1580 2024-05-02 14:22:16.400847 naimco-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2540 1970-01-01 00:00:00.000000 naimco-0.1.0/PKG-INFO
```

### Comparing `naimco-0.0.1/LICENSE` & `naimco-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `naimco-0.0.1/README.rst` & `naimco-0.1.0/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 
 NaimCo
 ======
 NaimCo (NaimController) is package to control Naim Mu-so sound systems.
 
+The main purpose of this package integration with Home Assistant.
+
 Nothing much to see for the moment but you can turn on the radio to preset #2:
 ::
-  
-  $ python scripts/naim_control.py 192.168.1.183 --preset 2 --volume 10
+
+  $ naim_control 192.168.1.183 --preset 2 --volume 10
 
   usage: naim_control.py [-h] [-i {IRADIO,DIGITAL1,SPOTIFY,USB,UPNP,TIDAL,FRONT} | -p PRESET | -o] [-v VOLUME] address
 
   Turn on Radio on naim Mu-so
 
   positional arguments:
     address               ip address of Mu-so
@@ -24,15 +26,15 @@
     -o, --off             Turn receiver off
     -v VOLUME, --volume VOLUME
                           Volume [0-100]
 
 Motivation
 ----------
 
-Naim Mu-so implements DLNA to some extent and it is possible to control it in home automation systems. 
+Naim Mu-so implements DLNA to some extent and it is possible to control it in home automation systems.
 Basic stuff like volume up down and play some media works.
 
 But there are functions that as far as I can tell can't be controlled with upnp/DLNA such as:
 
 - On/Off ( Standby off or standby on í Naim terms )
 - Input selection
     - iRadio
```

### Comparing `naimco-0.0.1/naimco/connection.py` & `naimco-0.1.0/naimco/connection.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,75 +1,72 @@
 import logging
 import asyncio
-import base64
-import xml.etree.ElementTree as ET
 
-NAIM_SOCKET_API_PORT=15555
+NAIM_SOCKET_API_PORT = 15555
 _LOG = logging.getLogger(__name__)
 
+
 class Connection:
     """Class that takes care of actual connection to device.
 
-    Creates a asyncio socket connection to the Mu-so device. 
+    Creates a asyncio socket connection to the Mu-so device.
     """
-    def __init__(self,reader,writer):
-        self.reader=reader
-        self.writer=writer
+
+    def __init__(self, reader, writer):
+        self.reader = reader
+        self.writer = writer
 
     @classmethod
-    async def create_connection(self, ip_address,socket_api_port=NAIM_SOCKET_API_PORT):
-        """Make the connection 
-    
+    async def create_connection(self, ip_address, socket_api_port=NAIM_SOCKET_API_PORT):
+        """Make the connection
+
         Parameters
         ----------
         ip_address : str
             IP-address of the Mu-so speaker.
         socket_api_port : int
             TCP port for communicating with Mu-so.
 
         Returns
         -------
         Connection
             a connection object that has opened a TCP connection to device.
         """
-    
-        reader, writer =  await asyncio.open_connection(ip_address,socket_api_port)
-        conn = Connection(reader,writer)
+        _LOG.debug("Connecting to  Naim Mu-So on ip: %s", ip_address)
+
+        reader, writer = await asyncio.open_connection(ip_address, socket_api_port)
+        conn = Connection(reader, writer)
         return conn
 
-        #_LOG.debug("Created NaimCo instance for ip: %s", ip_address)
-    
+        # _LOG.debug("Created NaimCo instance for ip: %s", ip_address)
+
     async def receive(self):
         """Receive one packet of data from Mu-so device.
-        
+
         Returns
         -------
         str
             Received data as a UTF-8 string.
         """
         if not self.reader.at_eof():
             data = await self.reader.read(2000)
-            # FIXME: I guess it is possible that the incoming packets get split in 
-            # such a way that a multibyte char gets split. 
+            # FIXME: I guess it is possible that the incoming packets get split in
+            # such a way that a multibyte char gets split.
             return data.decode()
         else:
             # What just happened? TODO:deal with connection failures and dropped connections
             # for now just throw exception
             raise ConnectionAbortedError("EOF on reader")
 
-        #await self.reader.close()        
+        # await self.reader.close()
 
-    async def send(self,message):
-        _LOG.debug(f'Send: {message!r}')
+    async def send(self, message):
+        _LOG.debug(f"Send: {message!r}")
         self.writer.write(message.encode())
         await self.writer.drain()
 
     async def close(self):
-        """"Close the connection
-        
+        """Close the connection
+
         Closing the writer causes the whole connection to close
         """
         self.writer.close()
-
-
-
-
```

### Comparing `naimco-0.0.1/naimco/core.py` & `naimco-0.1.0/naimco/core.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,20 +2,22 @@
 import socket
 import asyncio
 
 from .controllers import Controller
 
 _LOG = logging.getLogger(__name__)
 
+
 class NaimCo:
     """The main class for interacting with a Naim Mu-so device.
 
-    This is the class that the "end user" will interact with. 
+    This is the class that the "end user" will interact with.
+    This is the class that the "end user" will interact with.
     """
-    
+
     def __init__(self, ip_address):
         """Initialize a NaimCo instance.
 
         Parameters
         ----------
         ip_address : str
             IP-address of the Mu-so speaker.
@@ -35,69 +37,55 @@
         #: The systems's ip address
         self.ip_address = ip_address
         self.cmd_id = 0
         self.state = NaimState()
         self.controller = None
         self.version = None
         _LOG.debug("Created NaimCo instance for ip: %s", ip_address)
-  
-    async def startup(self):
+
+    async def startup(self, timeout=None):
         """Connect to the Mu-so device and get the initial state.
 
         This method should be called before any other interaction with the device.
         """
         # Note: This method should be called after the event loop is running
         # and before any other interaction with the device is attempted.
         _LOG.debug("Starting up NaimCo instance for ip: %s", self.ip_address)
-        self.controller=Controller(self)
-        await self.controller.startup()
-
-    async def run_connection(self,timeout=None):
-        """Run a connection to the Mu-so device.
+        self.controller = Controller(self)
+        await self.controller.startup(timeout)
 
-        This method is a convenience method that calls `startup()`, `connect()` and `shutdown()` in sequence.
+    async def shutdown(self):
+        """Close the connection to the Mu-so device."""
+        await self.controller.shutdown()
 
-        Parameters
-        ----------
-        timeout : int, optional
-            timeout in seconds for the `keep_alive()` method. If `None` then no keep alive is sent.
-        """
-        #await self.connect()
-        
-        asyncio.create_task(self.controller.receiver())
-        if timeout:
-            await(self.controller.keep_alive(timeout))
-
-        _LOG.warn("Connection to naim closed")
-        # what just happened, how did it happen?
-             
     async def on(self):
-        await self.controller.nvm.send_command('SETSTANDBY OFF')
+        await self.controller.nvm.send_command("SETSTANDBY OFF")
         await asyncio.sleep(3)
-        await self.controller.nvm.send_command('GETSTANDBYSTATUS')
+        await self.controller.nvm.send_command("GETSTANDBYSTATUS")
 
     async def off(self):
-        await self.controller.nvm.send_command('SETSTANDBY ON')
+        await self.controller.nvm.send_command("SETSTANDBY ON")
 
-    @property 
+    @property
     def standbystatus(self):
         return self.state.standbystatus
+
     @property
     def volume(self):
         return self.state.volume
-    
-    async def set_volume(self,volume):
-        await self.controller.nvm.send_command(f'SETRVOL {volume}')
+
+    async def set_volume(self, volume):
+        await self.controller.nvm.send_command(f"SETRVOL {volume}")
 
     async def volume_up(self):
-        await self.controller.nvm.send_command(f'VOL+')
+        await self.controller.nvm.send_command("VOL+")
 
     async def volume_down(self):
-        await self.controller.nvm.send_command(f'VOL-')
-    
+        await self.controller.nvm.send_command("VOL-")
+
     @property
     def input(self):
         return self.state.input
 
     @property
     def product(self):
         return self.state.product
@@ -107,32 +95,35 @@
         return self.state.serialnum
 
     @property
     def roomname(self):
         return self.state.roomname
 
     @property
-    def inputs(self) -> dict[int,dict]:
-        return {inp['id']:inp['name'] for inp in self.state.inputblk.values()}
-    
-    @property
-    def presets(self) -> dict[int,dict]:
-        return {index:preset['name'] for index,preset in self.state.presetblk.items()}
-
-    async def select_input(self,input):
-        await self.controller.nvm.send_command(f'SETINPUT {input}')
-    
-    async def select_preset(self,preset):
-        await self.controller.nvm.send_command(f'GOTOPRESET {preset}')
-    
+    def name(self):
+        return self.state.roomname
+
+    @property
+    def inputs(self) -> dict[int, dict]:
+        return {inp["id"]: inp["name"] for inp in self.state.inputblk.values()}
+
+    @property
+    def presets(self) -> dict[int, dict]:
+        return {index: preset["name"] for index, preset in self.state.presetblk.items()}
+
+    async def select_input(self, input):
+        await self.controller.nvm.send_command(f"SETINPUT {input}")
+
+    async def select_preset(self, preset):
+        await self.controller.nvm.send_command(f"GOTOPRESET {preset}")
 
     @property
     def viewstate(self):
         return self.state.viewstate
-    
+
     @property
     def media_image_url(self) -> str | None:
         """Image url of current playing media."""
         if not self.state.briefnp:
             return None
         return self.state.briefnp.get("logo_url", None)
         # self.state.briefnp = {'state':state,'description':description,'logo_url':logo_url}
@@ -165,155 +156,171 @@
         if not self.state.now_playing:
             return None
         if metadata := self.state.now_playing.get("metadata", None):
             return metadata.get("album", None)
         return None
 
     def get_now_playing(self):
-        resp={}
-        try :    
-            md = self.state.now_playing['metadata']
-            resp['artist'] = md.get('artist')
-            resp['album'] = md.get('album')
+        resp = {}
+        try:
+            md = self.state.now_playing["metadata"]
+            resp["artist"] = md.get("artist")
+            resp["album"] = md.get("album")
         except Exception:
-            #_LOG.debug("No metadata for now playing")
+            # _LOG.debug("No metadata for now playing")
             pass
-        try :    
-            resp['source'] = self.state.now_playing['source']
-            resp['title'] = self.state.now_playing.get('title')
+        try:
+            resp["source"] = self.state.now_playing["source"]
+            resp["title"] = self.state.now_playing.get("title")
         except Exception:
-            #_LOG.debug(f"No playback for now playing {self.state.now_playing}")
+            # _LOG.debug(f"No playback for now playing {self.state.now_playing}")
             pass
-        try :    
-            if resp['source'] == 'iradio':
-                resp['string'] = f'{resp.get("artist")} {resp.get("title")}' 
+        try:
+            if resp["source"] == "iradio":
+                resp["string"] = f'{resp.get("artist")} {resp.get("title")}'
             else:
-                resp['string'] = f'{resp.get("artist")} / {resp.get("title")} / {resp.get("album")}' 
+                resp["string"] = (
+                    f'{resp.get("artist")} / {resp.get("title")} / {resp.get("album")}'
+                )
 
-        except Exception as e:            
-            #_LOG.debug(f"failed to make string {resp} {e}")
-            resp['string'] = f'No information available' 
+        except Exception:
+            # _LOG.debug(f"failed to make string {resp} {e}")
+            resp["string"] = "No information available"
         return resp
 
-class NaimState:
 
- 
+class NaimState:
     def __init__(self):
         # NVM properties
-        self._input:str = None 
-        self._volume:int = None
-        self._standbystatus:dict = None
-        self._bufferstate:int = None
-        self._inputblk:dict[int,dict] = {}
-        self._viewstate:dict = None
-        self._briefnp:dict = None
-        self._product:str = None
-        self._serialnum:str = None
-        self._roomname:str = None
-        self._totalpresets:int|None = None
-        self._presetblk:dict[int,dict] = {}
-
+        self._input: str = None
+        self._volume: int = None
+        self._standbystatus: dict = None
+        self._bufferstate: int = None
+        self._inputblk: dict[int, dict] = {}
+        self._viewstate: dict = None
+        self._briefnp: dict = None
+        self._product: str = None
+        self._serialnum: str = None
+        self._roomname: str = None
+        self._totalpresets: int | None = None
+        self._presetblk: dict[int, dict] = {}
 
         # XML properties
         self.view_state = None
         self.now_playing = None
         self.now_playing_time = None
         self.active_list = None
-    
+        self.bridge_co_app_versions = None
+
     @property
     def volume(self) -> int:
         return self._volume
+
     @volume.setter
-    def volume(self,volume:int):
-        self._volume=volume
-    
+    def volume(self, volume: int):
+        self._volume = volume
+
     @property
     def input(self) -> str:
         return self._input
+
     @input.setter
-    def input(self,input:str):
-        self._input=input
+    def input(self, input: str):
+        self._input = input
 
     @property
-    def viewstate(self)->dict:
+    def viewstate(self) -> dict:
         return self._viewstate
+
     @viewstate.setter
-    def viewstate(self,state:dict):
-        """ NVM view state"""
-        self._viewstate=state
-    
+    def viewstate(self, state: dict):
+        """NVM view state"""
+        self._viewstate = state
+
     @property
-    def briefnp(self)->dict:
+    def briefnp(self) -> dict:
         return self._briefnp
+
     @briefnp.setter
-    def briefnp(self,briefnp):
-        self._briefnp=briefnp
-    
+    def briefnp(self, briefnp):
+        self._briefnp = briefnp
+
     @property
     def bufferstate(self) -> int:
         return self._bufferstate
+
     @bufferstate.setter
-    def bufferstate(self,bufferstate:int):
-        self._bufferstate=bufferstate
-    
+    def bufferstate(self, bufferstate: int):
+        self._bufferstate = bufferstate
+
     @property
     def standbystatus(self) -> dict:
         return self._standbystatus
+
     @standbystatus.setter
-    def standbystatus(self,standbystatus:dict):
-        self._standbystatus=standbystatus
-    
+    def standbystatus(self, standbystatus: dict):
+        self._standbystatus = standbystatus
+
     @property
     def inputblk(self) -> list[dict]:
         return self._inputblk
-    def set_inputblk_entry(self,index:int,val:dict):
+
+    def set_inputblk_entry(self, index: int, val: dict):
         self._inputblk[index] = val
 
     @property
     def product(self) -> str:
         return self._product
+
     @product.setter
-    def product(self,product:str):
+    def product(self, product: str):
         self._product = product
 
     @property
     def serialnum(self) -> str:
         return self._serialnum
+
     @serialnum.setter
-    def serialnum(self,serialnum:str):
-        self._serialnum = serialnum    
-        
+    def serialnum(self, serialnum: str):
+        self._serialnum = serialnum
+
     @property
     def roomname(self) -> str:
         return self._roomname
+
     @roomname.setter
-    def roomname(self,roomname:str):
+    def roomname(self, roomname: str):
         self._roomname = roomname
 
     @property
-    def totalpresets(self) -> int|None:
+    def totalpresets(self) -> int | None:
         return self._totalpresets
+
     @totalpresets.setter
-    def totalpresets(self,totalpresets:int|None):
+    def totalpresets(self, totalpresets: int | None):
         self._totalpresets = totalpresets
-    
+
     @property
     def presetblk(self) -> list[dict]:
         return self._presetblk
-    def set_presetblk_entry(self,index:int,val:dict):
+
+    def set_presetblk_entry(self, index: int, val: dict):
         _LOG.debug(f"presetblk_entry {index} {val}")
-        if val['state']=='USED':
+        if val["state"] == "USED":
             self._presetblk[index] = val
         else:
             self._presetblk.pop(index, None)
 
-    def set_view_state(self,state):
-        self.view_state=state
-    
-    def set_now_playing(self,state):
-        self.now_playing=state
-    
-    def set_active_list(self,state):
-        self.active_list=state
-    
-    def set_now_playing_time(self,state):
-        self.now_playing_time=state
+    def set_view_state(self, state):
+        self.view_state = state
+
+    def set_now_playing(self, state):
+        self.now_playing = state
+
+    def set_active_list(self, state):
+        self.active_list = state
+
+    def set_now_playing_time(self, state):
+        self.now_playing_time = state
+
+    def set_bridge_co_app_versions(self, state):
+        self.bridge_co_app_versions = state
```

### Comparing `naimco-0.0.1/naimco/msg_processing.py` & `naimco-0.1.0/naimco/msg_processing.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,118 +1,121 @@
 import logging
-import  xml.etree.ElementTree as ET
+import xml.etree.ElementTree as ET
 import base64
 
 _LOG = logging.getLogger(__name__)
 
-def dict_to_etree(d):
 
-    def _to_etree(parent,d):
+def dict_to_etree(d):
+    def _to_etree(parent, d):
         if not d:
             pass
         elif isinstance(d, str):
-            parent.text=d
+            parent.text = d
         elif isinstance(d, int):
-            parent.text=str(d)
-        elif isinstance(d,dict):
-            for k,v in d.items():
+            parent.text = str(d)
+        elif isinstance(d, dict):
+            for k, v in d.items():
                 assert isinstance(k, str)
-                _to_etree(ET.SubElement(parent,k),v)
-        elif isinstance(d,list):
+                _to_etree(ET.SubElement(parent, k), v)
+        elif isinstance(d, list):
             for i in d:
                 _LOG.debug(f"recursing this {i}")
                 parent.append(dict_to_etree(i))
         else:
-            assert d == 'invalid type', (type(d), d)
+            assert d == "invalid type", (type(d), d)
 
     assert isinstance(d, dict) and len(d) == 1
     tag, data = next(iter(d.items()))
     root = ET.Element(tag)
-    _to_etree(root,data)
+    _to_etree(root, data)
     return root
 
-def gen_xml_command(command,id,map=None):
-    cmd = ET.Element('command')
-    name = ET.SubElement(cmd,'name')
+
+def gen_xml_command(command, id, map=None):
+    cmd = ET.Element("command")
+    name = ET.SubElement(cmd, "name")
     name.text = command
-    idel = ET.SubElement(cmd,'id')
+    idel = ET.SubElement(cmd, "id")
     idel.text = id
-    if(map):
-        cmd.append(dict_to_etree( {'map':map}))
+    if map:
+        cmd.append(dict_to_etree({"map": map}))
     return ET.tostring(cmd).decode("utf-8")
 
+
 def tree_to_dict(element):
-    if (tag := element.tag ) in ['reply','event','item','error']:
-        #name = element.attrib['name']
+    if (tag := element.tag) in ["reply", "event", "item", "error"]:
+        # name = element.attrib['name']
         me = {}
-        val=None
-        for k,v in element.items():
+        val = None
+        for k, v in element.items():
             match k:
-                case 'name':
+                case "name":
                     name = v
-                case 'id':
-                    me['id']=v
-                case 'int':
-                    val=int(v)
-                case 'string':
-                    val=v
+                case "id":
+                    me["id"] = v
+                case "int":
+                    val = int(v)
+                case "string":
+                    val = v
                 case _:
-                    raise NotImplementedError(f'Unknown attribute {k} in {tag}')
+                    raise NotImplementedError(f"Unknown attribute {k} in {tag}")
         for child in element:
             match child.tag:
-                case 'name':
+                case "name":
                     name = child.text
-                case 'string':
-                    val=child.text
-                case 'map':
-                    val={}
+                case "string":
+                    val = child.text
+                case "map":
+                    val = {}
                     for item in child:
-                        subtag,d = tree_to_dict(item) 
+                        subtag, d = tree_to_dict(item)
                         val.update(d)
-                case 'array':
-                    val=[]
+                case "array":
+                    val = []
                     for item in child:
-                        if item.tag == 'map':
+                        if item.tag == "map":
                             for it2 in item:
-                                _LOG.debug(f'item: {ET.tostring(it2)}')
-                                subtag,d = tree_to_dict(it2)
+                                _LOG.debug(f"item: {ET.tostring(it2)}")
+                                subtag, d = tree_to_dict(it2)
                                 val.append(d)
                         else:
-                            subtag,d = tree_to_dict(item) 
+                            subtag, d = tree_to_dict(item)
                             val.append(d)
-                case 'base64':
-                    val=base64.b64decode(child.text).decode("utf-8")
+                case "base64":
+                    val = base64.b64decode(child.text).decode("utf-8")
                 case _:
-                    if child.tag in ['id','code','description']:
+                    if child.tag in ["id", "code", "description"]:
                         me[child.tag] = child.text
                     else:
-                        raise NotImplementedError(f'Unknown child {child.tag} in {tag}')
+                        raise NotImplementedError(f"Unknown child {child.tag} in {tag}")
         me[name] = val
-        return tag,me
-    raise NotImplementedError(f'Unknown element {element.tag}')
+        return tag, me
+    raise NotImplementedError(f"Unknown element {element.tag}")
+
 
 class MessageStreamProcessor:
     def __init__(self):
-        self.parser= ET.XMLPullParser(['start','end'])
+        self.parser = ET.XMLPullParser(["start", "end"])
         # fake tag to allow parsing of a stream og xml elements.
         # TODO: Figure out if this leaks memory.
-        self.parser.feed('<stream>') 
+        self.parser.feed("<stream>")
         self.lvl = 0
-        self.tree_buffer=[]
+        self.tree_buffer = []
 
-    def feed(self,data):    
+    def feed(self, data):
         self.parser.feed(data)
         for event, elem in self.parser.read_events():
-            if event == 'start':
+            if event == "start":
                 self.lvl += 1
-            elif event == 'end':
+            elif event == "end":
                 self.lvl -= 1
                 if self.lvl == 1:
-                    #print(event)
-                    #print(elem.tag, 'name=', elem.get('name'))
-                    tag,dict = tree_to_dict(elem)
-                    self.tree_buffer.append((tag,dict))
+                    # print(event)
+                    # print(elem.tag, 'name=', elem.get('name'))
+                    tag, dict = tree_to_dict(elem)
+                    self.tree_buffer.append((tag, dict))
 
     def read_messages(self):
         res = iter(self.tree_buffer)
-        self.tree_buffer=[]
+        self.tree_buffer = []
         return res
```

