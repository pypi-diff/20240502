# Comparing `tmp/gridappsd_python-2024.1.4a0.tar.gz` & `tmp/gridappsd_python-2024.4.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gridappsd_python-2024.1.4a0.tar", max compression
+gzip compressed data, was "gridappsd_python-2024.4.0a0.tar", max compression
```

## Comparing `gridappsd_python-2024.1.4a0.tar` & `gridappsd_python-2024.4.0a0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    10500 2024-01-25 21:54:57.918464 gridappsd_python-2024.1.4a0/README.md
--rw-r--r--   0        0        0     3796 2024-01-25 21:54:57.918464 gridappsd_python-2024.1.4a0/gridappsd/__init__.py
--rw-r--r--   0        0        0     4620 2024-01-25 21:54:57.918464 gridappsd_python-2024.1.4a0/gridappsd/__main__.py
--rw-r--r--   0        0        0     7214 2024-01-25 21:54:57.918464 gridappsd_python-2024.1.4a0/gridappsd/app_registration.py
--rw-r--r--   0        0        0     4689 2024-01-25 21:54:57.918464 gridappsd_python-2024.1.4a0/gridappsd/difference_builder.py
--rw-r--r--   0        0        0    30366 2024-01-25 21:54:57.922464 gridappsd_python-2024.1.4a0/gridappsd/docker_handler.py
--rw-r--r--   0        0        0    17177 2024-01-25 21:54:57.922464 gridappsd_python-2024.1.4a0/gridappsd/goss.py
--rw-r--r--   0        0        0    12696 2024-01-25 21:54:57.922464 gridappsd_python-2024.1.4a0/gridappsd/gridappsd.py
--rw-r--r--   0        0        0     3318 2024-01-25 21:54:57.922464 gridappsd_python-2024.1.4a0/gridappsd/houses.py
--rw-r--r--   0        0        0     1289 2024-01-25 21:54:57.922464 gridappsd_python-2024.1.4a0/gridappsd/json_extension.py
--rw-r--r--   0        0        0     2723 2024-01-25 21:54:57.922464 gridappsd_python-2024.1.4a0/gridappsd/loghandler.py
--rw-r--r--   0        0        0     2544 2024-01-25 21:54:57.922464 gridappsd_python-2024.1.4a0/gridappsd/register_app.py
--rw-r--r--   0        0        0    12258 2024-01-25 21:54:57.922464 gridappsd_python-2024.1.4a0/gridappsd/simulation.py
--rw-r--r--   0        0        0     3259 2024-01-25 21:54:57.922464 gridappsd_python-2024.1.4a0/gridappsd/timeseries.py
--rw-r--r--   0        0        0    12028 2024-01-25 21:54:57.922464 gridappsd_python-2024.1.4a0/gridappsd/topics.py
--rw-r--r--   0        0        0     3177 2024-01-25 21:54:57.922464 gridappsd_python-2024.1.4a0/gridappsd/utils.py
--rw-r--r--   0        0        0     1384 2024-01-25 21:55:53.802272 gridappsd_python-2024.1.4a0/pyproject.toml
--rw-r--r--   0        0        0    11484 1970-01-01 00:00:00.000000 gridappsd_python-2024.1.4a0/PKG-INFO
+-rw-r--r--   0        0        0    10489 2024-05-02 16:40:43.790433 gridappsd_python-2024.4.0a0/README.md
+-rw-r--r--   0        0        0     3794 2024-05-02 16:40:43.790433 gridappsd_python-2024.4.0a0/gridappsd/__init__.py
+-rw-r--r--   0        0        0     4685 2024-05-02 16:40:43.790433 gridappsd_python-2024.4.0a0/gridappsd/__main__.py
+-rw-r--r--   0        0        0     7012 2024-05-02 16:40:43.790433 gridappsd_python-2024.4.0a0/gridappsd/app_registration.py
+-rw-r--r--   0        0        0     4687 2024-05-02 16:40:43.790433 gridappsd_python-2024.4.0a0/gridappsd/difference_builder.py
+-rw-r--r--   0        0        0    30366 2024-05-02 16:40:43.790433 gridappsd_python-2024.4.0a0/gridappsd/docker_handler.py
+-rw-r--r--   0        0        0    17354 2024-05-02 16:40:43.790433 gridappsd_python-2024.4.0a0/gridappsd/goss.py
+-rw-r--r--   0        0        0    12737 2024-05-02 16:40:43.790433 gridappsd_python-2024.4.0a0/gridappsd/gridappsd.py
+-rw-r--r--   0        0        0     3275 2024-05-02 16:40:43.790433 gridappsd_python-2024.4.0a0/gridappsd/houses.py
+-rw-r--r--   0        0        0     3388 2024-05-02 16:40:43.790433 gridappsd_python-2024.4.0a0/gridappsd/json_extension.py
+-rw-r--r--   0        0        0     2703 2024-05-02 16:40:43.794433 gridappsd_python-2024.4.0a0/gridappsd/loghandler.py
+-rw-r--r--   0        0        0     2570 2024-05-02 16:40:43.794433 gridappsd_python-2024.4.0a0/gridappsd/register_app.py
+-rw-r--r--   0        0        0    12234 2024-05-02 16:40:43.794433 gridappsd_python-2024.4.0a0/gridappsd/simulation.py
+-rw-r--r--   0        0        0     3201 2024-05-02 16:40:43.794433 gridappsd_python-2024.4.0a0/gridappsd/timeseries.py
+-rw-r--r--   0        0        0    12128 2024-05-02 16:40:43.794433 gridappsd_python-2024.4.0a0/gridappsd/topics.py
+-rw-r--r--   0        0        0     3167 2024-05-02 16:40:43.794433 gridappsd_python-2024.4.0a0/gridappsd/utils.py
+-rw-r--r--   0        0        0     1383 2024-05-02 16:41:41.478312 gridappsd_python-2024.4.0a0/pyproject.toml
+-rw-r--r--   0        0        0    11473 1970-01-01 00:00:00.000000 gridappsd_python-2024.4.0a0/PKG-INFO
```

### Comparing `gridappsd_python-2024.1.4a0/README.md` & `gridappsd_python-2024.4.0a0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -174,48 +174,48 @@
 ## Testing
 
 Testing has become an integral part of the software lifecycle.  The `gridappsd-python` library has both unit and
 integration tests available to be run.  In order to execute these, you must have installed the gridappsd-python library
 as above with dev-dependencies.
 
 During the testing phase the docker containers required for the tests are downloaded from
-dockerhub and started.  By default the `develop` tag is used to test the library using pytest.  
+dockerhub and started.  By default the `develop` tag is used to test the library using pytest.
 One can customize the docker image tag by setting the environmental
-variable `GRIDAPPSD_TAG_ENV` either by `export GRIDAPPSD_TAG_ENV=other_tag` or by executing 
+variable `GRIDAPPSD_TAG_ENV` either by `export GRIDAPPSD_TAG_ENV=other_tag` or by executing
 pytest with the following:
 
 ```shell script
 
 # Export environmental variables and all tests will use the same tag (other_tag) to pull from docker hub.
 # Default tag is develop
 export GRIDAPPSD_TAG_ENV=other_tag
 pytest
 
-# Tests also require the username and password to be avaialable as environmental variables 
+# Tests also require the username and password to be avaialable as environmental variables
 # in order for them to properly run these tests
 export GRIDAPPSD_USER=user
 export GRIDAPPSD_PASSWORD=pass
 
 pytest
 ```
 
  ***NOTE: the first running the tests will download all of the docker images associated with the
  [GOSS-GridAPPS-D](http://github.com/GRIDAPPSD/GOSS-GridAPPS-D) repository.  This process may take some time.***
- 
+
 ### Running tests created in a new project
 
 The `gridappsd-python` library exposes a testing environment through the `gridappsd.docker_handler` module.  Including the following
 `conftest.py` in the root of your base test directory allows tests to reference these.  Using these fixtures will start all of the
-base containers required for `gridappsd` to run.  
+base containers required for `gridappsd` to run.
 
 ```python
 
 # conftest.py
-# Create a conftest.py file in the root of the tests directory to enable usage throughout the tests directory and below. 
-# 
+# Create a conftest.py file in the root of the tests directory to enable usage throughout the tests directory and below.
+#
 # Tested project structure an layout
 #
 # project-folder\
 #   mainmodule\
 #     __init__.py
 #     myapplication.py
 #   tests\
@@ -299,15 +299,15 @@
 
 ```
 
 Using the above fixtures from inside a test module and test function looks like the following:
 
 ```python
 
-# Example test function using the gridappsd_client fixture 
+# Example test function using the gridappsd_client fixture
 
 @mock.patch.dict(os.environ, {"GRIDAPPSD_APPLICATION_ID": "helics_goss_bridge.py"})
 def test_gridappsd_status(gridappsd_client):
     gappsd = gridappsd_client
     assert "helics_goss_bridge.py" == gappsd.get_application_id()
     assert gappsd.get_application_status() == ProcessStatusEnum.STARTING.value
     assert gappsd.get_service_status() == ProcessStatusEnum.STARTING.value
@@ -321,8 +321,7 @@
     assert gappsd.get_application_status() == ProcessStatusEnum.COMPLETE.value
 
     # Invalid
     gappsd.set_service_status("Foo")
     assert gappsd.get_service_status() == ProcessStatusEnum.COMPLETE.value
     assert gappsd.get_application_status() == ProcessStatusEnum.COMPLETE.value
 ```
-
```

### Comparing `gridappsd_python-2024.1.4a0/gridappsd/__init__.py` & `gridappsd_python-2024.4.0a0/gridappsd/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,9 +50,7 @@
 
 from gridappsd.goss import GOSS
 from gridappsd.utils import ProcessStatusEnum
 from gridappsd.gridappsd import GridAPPSD
 from gridappsd.difference_builder import DifferenceBuilder
 from gridappsd.app_registration import ApplicationController
 import gridappsd.json_extension as json
-
-
```

### Comparing `gridappsd_python-2024.1.4a0/gridappsd/__main__.py` & `gridappsd_python-2024.4.0a0/gridappsd/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,27 +45,29 @@
 from time import sleep
 import yaml
 
 from gridappsd import GridAPPSD
 
 assert sys.version_info >= (3, 6), "Minimum version is python 3.6"
 
-logging.basicConfig(stream=sys.stdout, level=logging.INFO,
+logging.basicConfig(stream=sys.stdout,
+                    level=logging.INFO,
                     format="'%(asctime)s: %(name)-20s - %(levelname)-6s - %(message)s")
 
 logging.getLogger('stomp.py').setLevel(logging.WARNING)
 _log = logging.getLogger("gridappsd.__main__")
 
-
 if __name__ == '__main__':
 
     parser = ArgumentParser()
 
     group = parser.add_mutually_exclusive_group(required=True)
-    group.add_argument("-s", "--run-simulation", type=argparse.FileType('r'),
+    group.add_argument("-s",
+                       "--run-simulation",
+                       type=argparse.FileType('r'),
                        help="Start running a simulation from a passed simulation file.")
 
     opts = parser.parse_args()
 
     if opts.run_simulation:
         # Example of how to pause simulation
         def next_timestep(simulation, timestep):
```

### Comparing `gridappsd_python-2024.1.4a0/gridappsd/app_registration.py` & `gridappsd_python-2024.4.0a0/gridappsd/app_registration.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,27 +9,28 @@
 import select
 import subprocess
 import threading
 import shlex
 import sys
 import os
 
-from . gridappsd import GridAPPSD
-from . topics import REQUEST_REGISTER_APP
+from .gridappsd import GridAPPSD
+from .topics import REQUEST_REGISTER_APP
 from . import utils, json_extension as json
 
 _log = logging.getLogger(__name__)
 
 # determine OS type
 posix = False
 if os.name == 'posix':
     posix = True
 
 
 class Job(threading.Thread):
+
     def __init__(self, args, out=sys.stdout, err=sys.stderr):
         threading.Thread.__init__(self)
         _log.debug("Creating job")
         self.running = False
         self._args = args
         self._out = out
         self._err = err
@@ -38,18 +39,15 @@
         self.running = False
 
     def run(self):
         try:
             self.running = True
             os.environ['GRIDAPPSD_APPLICATION_STATUS'] = 'RUNNING'
 
-            p = subprocess.Popen(args=self._args,
-                                 shell=False,
-                                 stdout=self._out,
-                                 stderr=self._err)
+            p = subprocess.Popen(args=self._args, shell=False, stdout=self._out, stderr=self._err)
 
             # Loop while process is executing
             while p.poll() is None and self.running:
                 os.environ['GRIDAPPSD_APPLICATION_STATUS'] = 'RUNNING'
                 time.sleep(1)
 
         except Exception as e:
@@ -108,21 +106,18 @@
         return self._application_id
 
     @property
     def heartbeat_valid(self):
         return self._heartbeat_thread is not None
 
     def register_app(self, end_callback):
-        print("Sending {}\n\tto {}".format(self._configDict,
-                                           REQUEST_REGISTER_APP))
+        print("Sending {}\n\tto {}".format(self._configDict, REQUEST_REGISTER_APP))
         self._gapd.get_logger().debug("Started App Registration")
 
-        response = self._gapd.get_response(REQUEST_REGISTER_APP,
-                                           self._configDict,
-                                           60)
+        response = self._gapd.get_response(REQUEST_REGISTER_APP, self._configDict, 60)
         if 'message' in response:
             _log.error("An error regisering the application occured")
             _log.error(response.get('message'))
             raise ValueError(response.get('message'))
         self._application_id = response.get('applicationId')
         self._heartbeat_topic = response.get('heartbeatTopic')
         self._heartbeat_period = response.get('heartbeatPeriod', 10)
@@ -152,15 +147,16 @@
 
         try:
             while True:
                 self._print_queue.put("Sending heartbeat for {}".format(self._application_id))
                 # print("Seanding heartbeat {} {}".format(self._heartbeat_topic, self._application_id))
                 # print("Heartbeat period: {}".format(self._heartbeat_period))
                 self._gapd.send(self._heartbeat_topic, self._application_id)
-                time.sleep(self._heartbeat_period - ((time.time() - starttime) % self._heartbeat_period))
+                time.sleep(self._heartbeat_period -
+                           ((time.time() - starttime) % self._heartbeat_period))
         except:
             error_callback()
 
     def __print_from_queue(self):
         while True:
             buff = self._print_queue.get(block=True)
             print(buff)
```

### Comparing `gridappsd_python-2024.1.4a0/gridappsd/difference_builder.py` & `gridappsd_python-2024.4.0a0/gridappsd/difference_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
         self._forward.append(forward)
         self._reverse.append(reverse)
 
     def clear(self):
         self._forward = []
         self._reverse = []
 
-    def get_message(self, epoch = None):
+    def get_message(self, epoch=None):
         if epoch is None:
             epoch = calendar.timegm(time.gmtime())
         msg = dict(command="update",
                    input=dict(simulation_id=self._simulation_id,
                               message=dict(timestamp=epoch,
                                            difference_mrid=str(uuid4()),
                                            reverse_differences=self._reverse,
```

### Comparing `gridappsd_python-2024.1.4a0/gridappsd/docker_handler.py` & `gridappsd_python-2024.4.0a0/gridappsd/docker_handler.py`

 * *Files identical despite different names*

### Comparing `gridappsd_python-2024.1.4a0/gridappsd/goss.py` & `gridappsd_python-2024.4.0a0/gridappsd/goss.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,15 +33,14 @@
 # or otherwise does not necessarily constitute or imply its endorsement, recommendation, or favoring by the United
 # States Government or any agency thereof, or Battelle Memorial Institute. The views and opinions of authors expressed
 # herein do not necessarily state or reflect those of the United States Government or any agency thereof.
 #
 # PACIFIC NORTHWEST NATIONAL LABORATORY operated by BATTELLE for the
 # UNITED STATES DEPARTMENT OF ENERGY under Contract DE-AC05-76RL01830
 # -------------------------------------------------------------------------------
-
 """
 Created on March 1, 2018
 
 @author: Craig Allwardt
 """
 import base64
 import inspect
@@ -77,18 +76,22 @@
     pass
 
 
 class GOSS(object):
     """ Base class providing connections to a GOSS instance via stomp protocol
     """
 
-    def __init__(self, username=None, password=None,
-                 stomp_address='localhost', stomp_port='61613',
+    def __init__(self,
+                 username=None,
+                 password=None,
+                 stomp_address='localhost',
+                 stomp_port='61613',
                  attempt_connection=True,
-                 override_threading=None, stomp_log_level=logging.WARNING,
+                 override_threading=None,
+                 stomp_log_level=logging.WARNING,
                  goss_log_level=logging.INFO):
 
         logging.getLogger('stomp.py').setLevel(stomp_log_level)
         logging.getLogger('goss').setLevel(goss_log_level)
 
         self.__user__ = username
         self.__pass__ = password
@@ -142,50 +145,54 @@
         self._override_thread_fc = callback
 
     def send(self, topic, message):
         self._make_connection()
         if isinstance(message, list) or isinstance(message, dict):
             message = json.dumps(message)
         _log.debug("Sending topic: {} body: {}".format(topic, message))
-        self._conn.send(body=message, destination=topic,
-                        headers={'GOSS_HAS_SUBJECT': True,
-                                  'GOSS_SUBJECT': self.__token})
-                                 
+        self._conn.send(body=message,
+                        destination=topic,
+                        headers={
+                            'GOSS_HAS_SUBJECT': True,
+                            'GOSS_SUBJECT': self.__token
+                        })
+
     def get_response(self, topic, message, timeout=5):
-        id = datetime.now().strftime("%Y%m%d%h%M%S")
+        id = datetime.now().strftime("%Y%m%d%h%M%S%f")[:-3]
         reply_to = "/temp-queue/response.{}".format(id)
-        
+
         if isinstance(message, str):
             message = json.loads(message)
-        
+
         if 'resultFormat' in message:
-            self.result_format = message['resultFormat'] 
+            self.result_format = message['resultFormat']
 
         # Change message to string if we have a dictionary.
         if isinstance(message, dict):
             message = json.dumps(message)
         elif isinstance(message, list):
             message = json.dumps(message)
-            
+
         class ResponseListener(object):
+
             def __init__(self, topic, result_format):
                 self.response = None
                 self._topic = topic
                 self.result_format = result_format
 
             def on_message(self, header, message):
 
                 _log.debug("Internal on message is: {} {}".format(header, message))
                 try:
                     if self.result_format == 'JSON':
                         if isinstance(message, dict):
                             self.response = message
                         else:
                             self.response = json.loads(message)
-                    else:   
+                    else:
                         self.response = message
                 except ValueError:
                     self.response = dict(error="Invalid json returned",
                                          header=header,
                                          message=message)
 
             def on_error(self, headers, message):
@@ -194,17 +201,21 @@
 
             def on_disconnect(self, header, message):
                 _log.debug("Disconnected")
 
         listener = ResponseListener(reply_to, self.result_format)
         self.subscribe(reply_to, listener)
 
-        self._conn.send(body=message, destination=topic,
-                        headers={'reply-to': reply_to, 'GOSS_HAS_SUBJECT': True,
-                                 'GOSS_SUBJECT': self.__token})
+        self._conn.send(body=message,
+                        destination=topic,
+                        headers={
+                            'reply-to': reply_to,
+                            'GOSS_HAS_SUBJECT': True,
+                            'GOSS_SUBJECT': self.__token
+                        })
         count = 0
 
         while count < timeout:
             if listener.response is not None:
                 break
 
             sleep(1)
@@ -278,57 +289,59 @@
     def _make_connection(self):
         if self._conn is None or not self._conn.is_connected():
             _log.debug("Creating connection")
             if not self.__token:
 
                 # get token
                 # get initial connection
-                dt=datetime.now()
+                dt = datetime.now()
                 replyDest = f"temp.token_resp.{self.__user__}-{dt}"
 
                 # create token request string
                 userAuthStr = f"{self.__user__}:{self.__pass__}"
                 base64Str = base64.b64encode(userAuthStr.encode())
 
                 # set up token callback
                 # send request to token topic
                 tokenTopic = "/topic/pnnl.goss.token.topic"
 
                 tmpConn = Connection([(self.stomp_address, self.stomp_port)])
                 if self._override_thread_fc is not None:
                     tmpConn.transport.override_threading(self._override_thread_fc)
                 tmpConn.connect(self.__user__, self.__pass__, wait=True)
-                
+
                 class TokenResponseListener():
+
                     def __init__(self):
                         self.__token = None
 
                     def get_token(self):
                         return self.__token
 
                     def on_message(self, header, message):
                         _log.debug("Internal on message is: {} {}".format(header, message))
-                        
+
                         self.__token = str(message)
 
                     def on_error(self, headers, message):
                         _log.error("ERR: {}".format(headers))
                         _log.error("OUR ERROR: {}".format(message))
 
                     def on_disconnect(self, header, message):
                         _log.debug("Disconnected")
 
                 # receive token and set token variable
                 # set callback
                 listener = TokenResponseListener()
 
                 # self.subscribe(replyDest, listener)
-                tmpConn.subscribe('/queue/'+replyDest, 123)
+                tmpConn.subscribe('/queue/' + replyDest, 123)
                 tmpConn.set_listener('token_resp', listener)
-                tmpConn.send(body=base64Str, destination=tokenTopic,
+                tmpConn.send(body=base64Str,
+                             destination=tokenTopic,
                              headers={'reply-to': replyDest})
                 # while token is null or for x iterations
                 iter = 0
                 while not self.__token and iter < 10:
                     # wait
                     self.__token = listener.get_token()
                     sleep(1)
```

### Comparing `gridappsd_python-2024.1.4a0/gridappsd/gridappsd.py` & `gridappsd_python-2024.4.0a0/gridappsd/gridappsd.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,31 +61,28 @@
 class InvalidSimulationIdError(Exception):
     pass
 
 
 class GridAPPSD(GOSS):
     """ The main :class:`GridAPPSD` interface for connecting to a GridAPPSD instance
     """
+
     # TODO Get the caller from the traceback/inspect module.
-    def __init__(self, simulation_id=None,
-                 address=None, **kwargs):
+    def __init__(self, simulation_id=None, address=None, **kwargs):
 
         if address is None:
             address = utils.get_gridappsd_address()
 
         if 'stomp_address' in kwargs and 'stomp_port' in kwargs:
             address = (kwargs.pop('stomp_address'), kwargs.pop('stomp_port'))
         elif 'stomp_address' in kwargs and not 'stomp_port' in kwargs or \
              'stomp_port' in kwargs and not 'stomp_address' in kwargs:
             raise ValueError("If stomp_address is specified the so should stomp_port")
 
-        super(GridAPPSD, self).__init__(
-            stomp_address=address[0],
-            stomp_port=address[1],
-            **kwargs)
+        super(GridAPPSD, self).__init__(stomp_address=address[0], stomp_port=address[1], **kwargs)
         self._houses = Houses(self)
         self._simulation_log_topic = None
         self._simulation_id = None
         # Transfer simulation_id from environment if its not passed
         # through the constructor.
         if simulation_id is None:
             simulation_id = utils.get_gridappsd_simulation_id()
@@ -100,48 +97,48 @@
 
         :return: :class:`gridappsd.loghandler.Logger`
         """
         return Logger(self)
 
     def get_houses(self) -> Houses:
         return self._houses
-    
+
     def get_simulation_id(self):
-        """ 
+        """
         Return the simulation_id given to the GridAPPSD instance
-        
+
         :return:
         """
         if not self._simulation_id:
             self._simulation_id = utils.get_gridappsd_simulation_id()
             if self._simulation_id:
                 self._simulation_log_topic = t.simulation_log_topic(self._simulation_id)
         return self._simulation_id
-    
+
     def set_application_status(self, status):
         """
         Set the application status.
         :param status:
         """
         try:
             self._process_status = ProcessStatusEnum(status)
         except ValueError:
-            self.get_logger().warning("Unsuccessful change of application status."
-                            + f"Valid statuses are {ProcessStatusEnum.__members__}.")
+            self.get_logger().warning("Unsuccessful change of application status." +
+                                      f"Valid statuses are {ProcessStatusEnum.__members__}.")
 
     def set_service_status(self, status):
         """
         Set the service status.
         :param status:
         """
         try:
             self._process_status = ProcessStatusEnum(status)
         except ValueError:
-            self.get_logger().warning("Unsuccessful change of service status."
-                                      + f"Valid statuses are {ProcessStatusEnum.__members__}.")
+            self.get_logger().warning("Unsuccessful change of service status." +
+                                      f"Valid statuses are {ProcessStatusEnum.__members__}.")
 
     def set_simulation_id(self, simulation_id):
         if simulation_id is None:
             self.get_logger().warning("None value for simulation_id set.")
         else:
             simulation_id = str(simulation_id)
             self._simulation_id = simulation_id
@@ -152,25 +149,25 @@
         Return the application status
         :return:
         """
         return self._process_status.value
 
     def get_application_id(self):
         return utils.get_gridappsd_application_id()
-    
+
     def get_service_status(self):
         """
         Return the service status
         :return:
         """
         return self._process_status.value
-    
+
     def query_object_types(self, model_id=None):
         """ Allows the caller to query the different object types.
-                
+
         :param model_id:
         :return:
         """
         args = {}
         if model_id:
             args["modelId"] = model_id
         payload = self._build_query_payload("QUERY_OBJECT_TYPES", **args)
@@ -182,43 +179,43 @@
             args["modelId"] = model_id
         payload = self._build_query_payload("QUERY_MODEL_NAMES", **args)
         return self.get_response(t.REQUEST_POWERGRID_DATA, payload, timeout=30)
 
     def query_model_info(self):
         payload = self._build_query_payload("QUERY_MODEL_INFO")
         return self.get_response(t.REQUEST_POWERGRID_DATA, payload, timeout=30)
-    
+
     def query_model(self, model_id=None, object_type=None, object_id=None, response_format='JSON'):
         args = {}
         if model_id is not None:
             args["modelId"] = model_id
         if object_type is not None:
             args["objectType"] = object_type
         if object_id is not None:
-            args["objectId"] = object_id   
+            args["objectId"] = object_id
         if response_format is not None:
-            args["resultFormat"] = response_format   
+            args["resultFormat"] = response_format
         payload = self._build_query_payload("QUERY_MODEL", **args)
         return self.get_response(t.REQUEST_POWERGRID_DATA, payload, timeout=30)
 
     def query_object(self, object_id, model_id=None):
         if not object_id:
             raise ValueError("Invalid object_id specified.")
         args = dict(objectId=object_id)
         if model_id is not None:
             args["modelId"] = model_id
         payload = self._build_query_payload("QUERY_OBJECT", **args)
         return self.get_response(t.REQUEST_POWERGRID_DATA, payload, timeout=30)
-    
+
     def query_object_dictionary(self, model_id, object_type=None, object_id=None):
         if not model_id:
             raise ValueError("model_id is not specified.")
         if not object_id and not object_type:
             raise ValueError("No obejct_id or object_type specified.")
-        args={}
+        args = {}
         args["modelId"] = model_id
         if object_id is not None:
             args["objectId"] = object_id
         if object_type is not None:
             args["objectType"] = object_type
         payload = self._build_query_payload("QUERY_OBJECT_DICT", **args)
         return self.get_response(t.REQUEST_POWERGRID_DATA, payload, timeout=30)
@@ -231,17 +228,23 @@
             raise ValueError("Only supported {} currently".format(POWERGRID_MODEL))
 
         payload = self._build_query_payload(request_type, queryString=query)
         # Do this so we can eventually support other db through this mechanism.
         request_topic = '.'.join((t.REQUEST_DATA, database_type))
         return self.get_response(request_topic, json.dumps(payload), timeout=timeout)
 
-    def get_platform_status(self, applications=True, services=True, appInstances=True, serviceInstances=True):
+    def get_platform_status(self,
+                            applications=True,
+                            services=True,
+                            appInstances=True,
+                            serviceInstances=True):
         _log.debug("Retrieving platform status from GridAPPSD")
-        msg = dict(appInstances=appInstances, applications=applications, services=services,
+        msg = dict(appInstances=appInstances,
+                   applications=applications,
+                   services=services,
                    serviceInstances=serviceInstances)
         return self.get_response(t.REQUEST_PLATFORM_STATUS, json.dumps(msg), timeout=30)
 
     def send_simulation_status(self, status, message, log_level=INFO):
         _log.debug("SEND SIM STATUS: {} message: {}".format(status, message))
         # Transform log level into something for use if we can.
         if isinstance(log_level, str):
@@ -252,33 +255,29 @@
             raise InvalidSimulationIdError()
         gad_log = self.get_logger()
         self.set_service_status(status)
         gad_log.log(message, log_level)
 
     def send_status(self, status, topic, log_level=INFO):
         self.set_application_status(status)
-        status_message = self.build_message_json(self.get_application_status(),
-            "", log_level)
+        status_message = self.build_message_json(self.get_application_status(), "", log_level)
         self.send(topic, status_message)
 
     def build_message_json(self, status, message, log_level):
         t_now = datetime.utcnow()
         status_message = {
             "source": utils.get_gridappsd_application_id(),
             "processId": f"{self._simulation_id}",
-            "timestamp": int(time.mktime(t_now.timetuple()))*1000,
+            "timestamp": int(time.mktime(t_now.timetuple())) * 1000,
             "procesStatus": status,
             "logMessage": str(message),
             "logLevel": logging.getLevelName(log_level),
             "storeToDb": True
         }
         data = json.dumps(status_message)
 
         return data
 
     def _build_query_payload(self, request_type, response_format='JSON', **kwargs):
         d = dict(requestType=request_type, resultFormat=response_format)
         d.update(**kwargs)
         return d
-
-
-
```

### Comparing `gridappsd_python-2024.1.4a0/gridappsd/houses.py` & `gridappsd_python-2024.4.0a0/gridappsd/houses.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 from collections import namedtuple
 
 house_keys = [
-    'name',
-    'parent',
-    'coolingSetpoint',
-    'coolingSystem',
-    'floorArea',
-    'heatingSetpoint',
-    'heatingSystem',
-    'hvacPowerFactor',
-    'numberOfStories',
-    'thermalIntegrity',
-    'id',
-    'fdrid'
+    'name', 'parent', 'coolingSetpoint', 'coolingSystem', 'floorArea', 'heatingSetpoint',
+    'heatingSystem', 'hvacPowerFactor', 'numberOfStories', 'thermalIntegrity', 'id', 'fdrid'
 ]
 House = namedtuple('House', house_keys)
 
 # class House(HouseBase):
 #     def __dict__
 
 
 class Houses:
+
     class __SingltonHouses:
+
         def __init__(self, gappsd: 'GridAPPSD'):
             self._gappsd = gappsd
             self._houses = {}
 
         def __str__(self):
             return repr(self) + self._gappsd
 
@@ -34,31 +26,31 @@
                 self._populate(feeder)
             return self._houses.get(feeder)
 
         def _populate(self, feeder):
             query = """# list houses - DistHouse
 PREFIX r:  <http://www.w3.org/1999/02/22-rdf-syntax-ns#>
 PREFIX c:  <http://iec.ch/TC57/CIM100#>
-SELECT ?fdrname ?name ?parent ?coolingSetpoint ?coolingSystem ?floorArea ?heatingSetpoint ?heatingSystem ?hvacPowerFactor ?numberOfStories ?thermalIntegrity ?id ?fdrid 
-WHERE { 
+SELECT ?fdrname ?name ?parent ?coolingSetpoint ?coolingSystem ?floorArea ?heatingSetpoint ?heatingSystem ?hvacPowerFactor ?numberOfStories ?thermalIntegrity ?id ?fdrid
+WHERE {
 #	VALUES ?fdrid {"_9CE150A8-8CC5-A0F9-B67E-BBD8C79D3095"}  # R2 12.47 3
 #	VALUES ?fdrid {"_4F76A5F9-271D-9EB8-5E31-AA362D86F2C3"}  # 8500-node
 # VALUES ?fdrid {"_E407CBB6-8C8D-9BC9-589C-AB83FBF0826D"}  # 123 PV/Triplex
 #   VALUES ?fdrid {"_503D6E20-F499-4CC7-8051-971E23D0BF79"}  # 123 Transactive
    VALUES ?fdrid {"%s"}
    ?h r:type c:House.
    ?h c:IdentifiedObject.name ?name.
    ?h c:IdentifiedObject.mRID ?id.
    ?h c:House.floorArea ?floorArea.
    ?h c:House.numberOfStories ?numberOfStories.
    OPTIONAL{?h c:House.coolingSetpoint ?coolingSetpoint.}
    OPTIONAL{?h c:House.heatingSetpoint ?heatingSetpoint.}
    OPTIONAL{?h c:House.hvacPowerFactor ?hvacPowerFactor.}
    ?h c:House.coolingSystem ?coolingSystemRaw.
-   	bind(strafter(str(?coolingSystemRaw),"HouseCooling.") as ?coolingSystem) 
+   	bind(strafter(str(?coolingSystemRaw),"HouseCooling.") as ?coolingSystem)
    ?h c:House.heatingSystem ?heatingSystemRaw.
    	bind(strafter(str(?heatingSystemRaw),"HouseHeating.") as ?heatingSystem)
    ?h c:House.thermalIntegrity ?thermalIntegrityRaw.
    	bind(strafter(str(?thermalIntegrityRaw),"HouseThermalIntegrity.") as ?thermalIntegrity)
    ?h c:House.EnergyConsumer ?econ.
    ?econ c:IdentifiedObject.name ?parent.
    ?fdr c:IdentifiedObject.mRID ?fdrid.
@@ -79,19 +71,17 @@
                     except KeyError:
                         create_order[d] = None
 
                 houses[name] = House(**create_order)
 
             self._houses[feeder] = houses
 
-
     instance = None
 
     def __init__(self, gappsd):
         if not Houses.instance:
             Houses.instance = Houses.__SingltonHouses(gappsd)
         else:
             Houses.instance._gappsd = gappsd
 
     def __getattr__(self, name):
         return getattr(self.instance, name)
-
```

### Comparing `gridappsd_python-2024.1.4a0/gridappsd/loghandler.py` & `gridappsd_python-2024.4.0a0/gridappsd/loghandler.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
     return _nameToLevel.get(data, NOTSET)
 
 
 class Logger:
     """
     The `Logger` class handles logging to the main gridappsd server.
     """
+
     def __init__(self, gaps, level=INFO):
         self._gaps = gaps
         self._level = level
 
     def setLevel(self, level):
         self._level = level
 
@@ -67,16 +68,17 @@
         """
         process_identifier = self._gaps.get_application_id()
 
         if not level in VALID_LOG_LEVELS:
             raise AttributeError(f"Log level must be one of {[x for x in _levelToName.values()]}")
 
         if not process_identifier:
-            raise AttributeError(f"Must have GRIDAPPSD_APPLICATION_ID or GRIDAPPSD_SERVICE_ID or GRIDAPPSD_PROCESS_ID "
-                                 "set in os environments.")
+            raise AttributeError(
+                f"Must have GRIDAPPSD_APPLICATION_ID or GRIDAPPSD_SERVICE_ID or GRIDAPPSD_PROCESS_ID "
+                "set in os environments.")
         status = self._gaps.get_application_status()
         sim_id = self._gaps.get_simulation_id()
 
         if sim_id is not None:
             topic = t.simulation_log_topic(sim_id)
         else:
             topic = t.platform_log_topic()
@@ -85,17 +87,16 @@
             "source": process_identifier,
             "processId": f"{sim_id}",
             "processStatus": str(status),
             "logMessage": str(message),
             "logLevel": _levelToName[level],
             "storeToDb": True
         }
-        
+
         gridappsd_log_level = os.getenv('GRIDAPPSD_LOG_LEVEL')
         if gridappsd_log_level == None:
             gridappsd_log_level = level
         else:
             gridappsd_log_level = _nameToLevel[gridappsd_log_level]
-            
+
         if level >= gridappsd_log_level:
             self._gaps.send(topic, status_message)
-
```

### Comparing `gridappsd_python-2024.1.4a0/gridappsd/register_app.py` & `gridappsd_python-2024.4.0a0/gridappsd/register_app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import logging
 import os
 import sys
 import time
 import stomp
 from gridappsd import ApplicationController, GridAPPSD, utils, json_extension as json
 
+
 def main():
     loglevel = logging.INFO
-    logging.basicConfig(stream=sys.stdout, level=loglevel,
+    logging.basicConfig(stream=sys.stdout,
+                        level=loglevel,
                         format="%(asctime)s - %(name)s;%(levelname)s|%(message)s",
                         datefmt="%Y-%m-%d %H:%M:%S")
     logging.getLogger('stomp.py').setLevel(logging.ERROR)
     _log = logging.getLogger(__name__)
 
     problems = utils.validate_gridappsd_uri()
 
@@ -39,28 +41,29 @@
     gap = None
     while True:
 
         try:
             if gap is None:
                 gap = GridAPPSD()
 
-        except ConnectionRefusedError:  # Python 3 specific error code
+        except ConnectionRefusedError:    # Python 3 specific error code
             _log.debug("Retry in 10 seconds")
             gap = appreg = None
             time.sleep(10)
         except (stomp.exception.ConnectFailedException, OSError):
             _log.debug("Connect failed Retry in 10 seconds")
             gap = appreg = None
             time.sleep(10)
         except KeyboardInterrupt:
             gap = appreg = None
             _log.info("Exiting app")
             break
         else:
             if appreg is None:
+
                 def end_app():
                     sys.exit(0)
 
                 # app_config_minimal = {
                 #     'id': 'an-app-id',
                 #     'execution_path': '/home/osboxes/git/gridappsd-python/testapp.sh'
                 # }
@@ -74,9 +77,7 @@
                     gap = None
             else:
                 if not appreg.heartbeat_valid:
                     appreg = None
                     gap = None
 
             time.sleep(2)
-
-
```

### Comparing `gridappsd_python-2024.1.4a0/gridappsd/simulation.py` & `gridappsd_python-2024.4.0a0/gridappsd/simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 class SimulationArgs(ConfigBase):
     start_time: str = "1655321830"
     duration: str = "300"
     simulator: str = "GridLAB-D"
     timestep_frequency: str = "1000"
     timestep_increment: str = "1000"
     run_realtime: bool = True
+    pause_after_measurements: bool = False
     simulation_name: str = "ieee13nodeckt"
     power_flow_solver_method: str = "NR"
     model_creation_config: ModelCreationConfig = __default_model_creation_config__
 
 
 __default_simulation_args__ = SimulationArgs()
 
@@ -116,20 +117,22 @@
     that are run on GridAPPSD.
 
     There are four events that can be registered: ontimestep, onmeasurement, oncomplete, and
     onstart.  To register one of the events call the method add_ontimestep_callback,
     add_onmeasurement_callback, add_oncomplete_callback or add_onstart_callback method respectively.
     """
 
-    def __init__(self, gapps: 'GridAPPSD',
-                 run_config: Union[Dict, SimulationConfig]):
-        assert type(
-            gapps).__name__ == 'GridAPPSD', "Must be an instance of GridAPPSD"
-
-        self._run_config = run_config
+    def __init__(self, gapps: 'GridAPPSD', run_config: Union[Dict, SimulationConfig]):
+        assert type(gapps).__name__ == 'GridAPPSD', "Must be an instance of GridAPPSD"
+        if isinstance(run_config, SimulationConfig):
+            self._run_config = run_config.asdict()
+        elif isinstance(run_config, dict):
+            self._run_config = run_config
+        else:
+            raise TypeError("run_config must be a dictionary or a SimulationConfig")
         # if isinstance(run_config, SimulationConfig):
         #     self._run_config = run_config
         # else:
         #     psconfig = PowerSystemConfig(**run_config['power_system_config'])
         #     appconfig = ApplicationConfig(**run_config['application_config'])
         #     simconfig = SimulationConfig(**run_config["simulation_config"])
         #     testconfig = TestConfig(**run_config['test_config'])
@@ -153,72 +156,64 @@
         self.__on_next_timestep_callbacks = set()
         self.__on_simulation_complete_callbacks = set()
 
         self._measurement_count = 0
         self._log_count = 0
         self._platform_log_count = 0
 
-        self._num_timesteps = round(
-            float(self._run_config["simulation_config"]["duration"]))
+        self._num_timesteps = round(float(self._run_config["simulation_config"]["duration"]))
 
         # self._num_timesteps = round(
         #     float(self._run_config.simulation_config.duration))
 
         # Devices that the user wants measurements from
         self._device_measurement_filter = {}
 
         self.__filterable_measurement_callback_set = set()
 
     def start_simulation(self, timeout=30):
         """ Start the configured simulation by calling the REQUEST_SIMULATION endpoint.
         """
-        resp = self._gapps.get_response(t.REQUEST_SIMULATION,
-                                        self._run_config,
-                                        timeout=timeout)
+        resp = self._gapps.get_response(t.REQUEST_SIMULATION, self._run_config, timeout=timeout)
 
         if 'simulationId' not in resp:
             message = "Simulation was not able to run\n" + str(resp)
             raise SimulationFailedToStartError(message)
 
         self._running_or_paused = True
         self.simulation_id = resp['simulationId']
 
         # Subscribe to the different components necessary to run and receive
         # simulated measurements and messages.
-        self._gapps.subscribe(t.simulation_log_topic(self.simulation_id),
-                              self.__on_simulation_log)
-        self._gapps.subscribe(t.simulation_output_topic(self.simulation_id),
-                              self.__onmeasurement)
+        self._gapps.subscribe(t.simulation_log_topic(self.simulation_id), self.__on_simulation_log)
+        self._gapps.subscribe(t.simulation_output_topic(self.simulation_id), self.__onmeasurement)
         self._gapps.subscribe(t.platform_log_topic(), self.__on_platformlog)
 
         for p in self.__on_start:
             p(self)
 
     def pause(self):
         """ Pause simulation"""
         _log.debug("Pausing simulation")
         command = dict(command="pause")
-        self._gapps.send(t.simulation_input_topic(self.simulation_id),
-                         json.dumps(command))
+        self._gapps.send(t.simulation_input_topic(self.simulation_id), json.dumps(command))
         self._running_or_paused = True
 
     def stop(self):
         """ Stop the simulation"""
         _log.debug("Stopping simulation")
         command = dict(command="stop")
-        self._gapps.send(t.simulation_input_topic(self.simulation_id),
-                         json.dumps(command))
+        self._gapps.send(t.simulation_input_topic(self.simulation_id), json.dumps(command))
         self._running_or_paused = True
 
     def resume(self):
         """ Resume the simulation"""
         _log.debug("Resuming simulation")
         command = dict(command="resume")
-        self._gapps.send(t.simulation_input_topic(self.simulation_id),
-                         json.dumps(command))
+        self._gapps.send(t.simulation_input_topic(self.simulation_id), json.dumps(command))
         self._running_or_paused = True
 
     def run_loop(self):
         """ Loop around the running of the simulation itself.
 
         Example:
 
@@ -238,22 +233,20 @@
             self.start_simulation()
 
         while self._running_or_paused:
             time.sleep(0.01)
 
     def resume_pause_at(self, pause_in):
         """ Resume the simulation and have it automatically pause after specified amount of seconds later.
-        
+
         :param pause_in: number of seconds to run before pausing the simulation
         """
-        _log.debug("Resuming simulation. Will pause after {} seconds".format(
-            pause_in))
+        _log.debug("Resuming simulation. Will pause after {} seconds".format(pause_in))
         command = dict(command="resumePauseAt", input=dict(pauseIn=pause_in))
-        self._gapps.send(t.simulation_input_topic(self.simulation_id),
-                         json.dumps(command))
+        self._gapps.send(t.simulation_input_topic(self.simulation_id), json.dumps(command))
         self._running_or_paused = True
 
     def add_onmeasurement_callback(self, callback, device_filter=()):
         """ registers an onmeasurment callback to be called when measurements have come through.
 
         Note:
 
@@ -267,16 +260,15 @@
             def onmeasurment(sim, timestep, measurements):
                 print("timestep: {}, measurement: {}".format(timestep, measurements))
 
         :param callback: Function to be called during running of simulation
         :param device_filter: Future filter of measurements
         :return:
         """
-        self.__filterable_measurement_callback_set.add(
-            (callback, device_filter))
+        self.__filterable_measurement_callback_set.add((callback, device_filter))
 
     def add_onstart_callback(self, callback):
         """ registers a start callback that is called when the simulation is started
 
         Callback Example:
 
             def onstart(sim):
@@ -357,8 +349,8 @@
 if __name__ == '__main__':
     from pprint import pprint
     psc = PowerSystemConfig(Line_name="_49AD8E07-3BF9-A4E2-CB8F-C3722F837B62")
     sim = SimulationConfig(power_system_config=psc)
 
     print(psc.asjson())
     print(sim.asjson())
-    pprint(json.loads(sim.asjson()), indent=2)
+    pprint(json.loads(sim.asjson()), indent=2)
```

### Comparing `gridappsd_python-2024.1.4a0/gridappsd/timeseries.py` & `gridappsd_python-2024.4.0a0/gridappsd/timeseries.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,105 +1,105 @@
 #import json
 from gridappsd import topics, json_extension as json
 from typing import Optional
 
 
-
 class Query:
     """ Class to create and execute request to query timeseries data
     """
-    
+
     def __init__(self, measurement):
         self.queryMeasurement = measurement
         self.queryFilter = []
         self.selectCriteria = []
         self.key = None
 
     def select(self, *keys):
         """ Defines what fields should be returned from the query.
-        
-        If this function is not called or is called without argument then 
+
+        If this function is not called or is called without argument then
         all the fields are returned.
-        
-        :param keys: list of fields to be returned 
+
+        :param keys: list of fields to be returned
         """
         for key in keys:
             self.selectCriteria.append(key)
         return self
 
     def first(self, n=Optional[int]):
         """ Method to add request to return first or oldest data to the query.
-        
+
         When n is specified, query will return first or oldest 'n' rows.
-        
-        :param n:  
+
+        :param n:
         """
         if n is not None:
-            self.first = n;
+            self.first = n
         return self
 
     def last(self, n=Optional[int]):
         """ Method to add request to return last or latest data to the query.
-        
+
         When n is specified, query will return last or latest 'n' rows.
-        
-        :param n:  
+
+        :param n:
         """
         if n is not None:
-            self.last = n;
+            self.last = n
         return self
-    
+
     def ge(self, value):
         """ Method to add 'value greater than or equal to' filter to a key.
-        
-        :param value:  
+
+        :param value:
         """
         if self.key is None:
             raise ValueError("Key is not specified. Call where_key first.")
-        obj = {"key":self.key,"ge":value}
+        obj = {"key": self.key, "ge": value}
         self.queryFilter.append(obj)
         return self
-    
+
     def le(self, value):
         """ Method to add 'value less than or equal to' filter to a key.
-        
-        :param value:  
+
+        :param value:
         """
         if self.key is None:
             raise ValueError("Key is not specified. Call where_key first.")
-        obj = {"key":self.key,"le":value}
+        obj = {"key": self.key, "le": value}
         self.queryFilter.append(obj)
         return self
-    
+
     def eq(self, value):
         """ Method to add 'value equal to' filter to a key.
-        
-        :param value:  
+
+        :param value:
         """
         if self.key is None:
             raise ValueError("Key is not specified. Call where_key first.")
-        obj = {"key":self.key,"eq":value}
+        obj = {"key": self.key, "eq": value}
         self.queryFilter.append(obj)
         return self
-    
+
     def between(self, value1, value2):
         """ Method to add 'value between' value1 and value2 filter to a key.
-        
+
         :param value1: defines 'greater than equal to' filter for key's value
         :param value2: defines 'less than equal to' filter for key's value
         """
         if self.key is None:
             raise ValueError("Key is not specified. Call where_key first.")
-        obj = {"key":self.key,"ge":value1}
+        obj = {"key": self.key, "ge": value1}
         self.queryFilter.append(obj)
-        obj = {"key":self.key,"le":value2}
+        obj = {"key": self.key, "le": value2}
         self.queryFilter.append(obj)
         return self
-    
+
     def where_key(self, key):
         self.key = key
         return self
 
     def execute(self, gridappsd_obj):
-        del self.key 
-        response = gridappsd_obj.get_response(topics.REQUEST_TIMESERIES_DATA, json.dumps(self.__dict__))
-        return response
+        del self.key
+        response = gridappsd_obj.get_response(topics.REQUEST_TIMESERIES_DATA,
+                                              json.dumps(self.__dict__))
+        return response
```

### Comparing `gridappsd_python-2024.1.4a0/gridappsd/topics.py` & `gridappsd_python-2024.4.0a0/gridappsd/topics.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 REQUEST_POWERGRID_DATA = ".".join((REQUEST_DATA, "powergridmodel"))
 REQUEST_TIMESERIES_DATA = ".".join((REQUEST_DATA, "timeseries"))
 
 REQUEST_REGISTER_APP = ".".join((PROCESS_PREFIX, "request.app.remote.register"))
 REQUEST_APP_START = ".".join((PROCESS_PREFIX, "request.app.start"))
 BASE_APPLICATION_HEARTBEAT = ".".join((BASE_TOPIC_PREFIX, "heartbeat"))
 
+
 def platform_log_topic():
     """ Utility method for getting the platform.log base topic
     """
     return "/topic/{}.{}".format(BASE_TOPIC_PREFIX, "platform.log")
 
 
 def service_input_topic(service_id, simulation_id):
@@ -171,89 +172,98 @@
 
 
 def simulation_log_topic(simulation_id):
     """https://gridappsd.readthedocs.io/en/latest/using_gridappsd/index.html#subscribing-to-logs
     """
     return "{}.{}".format(BASE_SIMULATION_LOG_TOPIC, simulation_id)
 
-def field_message_bus_topic(message_bus_id:str, app_id: str=None, agent_id: str=None):
+
+def field_message_bus_topic(message_bus_id: str, app_id: str = None, agent_id: str = None):
     """ Utility method for getting the publish/subscribe topic for a specific message bus.
 
     :param message_bus_id:
     :param app_id:
     :param agent_id:
     :return:
     """
     assert message_bus_id, "message_bus_id cannot be empty"
 
-    return f"{BASE_FIELD_TOPIC}.{message_bus_id}" 
+    return f"{BASE_FIELD_TOPIC}.{message_bus_id}"
 
 
 def field_message_bus_app_topic(message_bus_id, app_id=None):
     """ Utility method for getting the publish/subscribe topic for a specific message bus.
 
     :param message_bus_id:
     :param app_id:
     :return:
     """
     assert message_bus_id, "message_bus_id cannot be empty"
     return "{}.{}.{}".format(BASE_FIELD_TOPIC, message_bus_id, app_id)
 
+
 def field_message_bus_agent_topic(message_bus_id, agent_id=None):
     """ Utility method for getting the publish/subscribe topic for a specific message bus.
 
     :param message_bus_id:
     :param agent_id:
     :return:
     """
     assert message_bus_id, "message_bus_id cannot be empty"
     return "{}.{}.{}".format(BASE_FIELD_TOPIC, message_bus_id, agent_id)
 
+
 def field_agent_request_queue(message_bus_id, agent_id):
     """ Utility method for getting the request topic for a specific distributed agent
 
     :param message_bus_id:
     :param agent_id:
     :return:
     """
     assert message_bus_id, "message_bus_id cannot be empty"
     return "{}.request.{}.{}".format(BASE_FIELD_QUEUE, message_bus_id, agent_id)
 
+
 def context_request_queue(message_bus_id):
     """ Utility method for getting the request topic for context manager
 
     :param message_bus_id:
     :return:
     """
     assert message_bus_id, "message_bus_id cannot be empty"
-    
-    return "{}.request.{}.{}".format(BASE_FIELD_QUEUE, message_bus_id, message_bus_id+'.context_manager')
+
+    return "{}.request.{}.{}".format(BASE_FIELD_QUEUE, message_bus_id,
+                                     message_bus_id + '.context_manager')
+
 
 def field_output_topic(message_bus_id=None, simulation_id=None):
     """ Utility method for getting the field output topic.
     If message_bus_id is None, it returns topic used by centralized device interfaces to publish measurements.
-    If message_bus_id is not None, it returns topic used by distributed devices interfaces to publish measurements which is then subscribed by distributed agents. 
-    
+    If message_bus_id is not None, it returns topic used by distributed devices interfaces to publish measurements which is then subscribed by distributed agents.
+
     :param message_bus_id:
     :param simulation_id
-    :return: str: Topic to receive field measurements 
+    :return: str: Topic to receive field measurements
     """
-    
+
     if simulation_id is None:
         return "{}.{}".format(BASE_FIELD_TOPIC, "output")
     else:
-        return "{}.{}.{}.{}".format(BASE_FIELD_TOPIC,"simulation.output",simulation_id,message_bus_id)
-    
+        return "{}.{}.{}.{}".format(BASE_FIELD_TOPIC, "simulation.output", simulation_id,
+                                    message_bus_id)
+
+
 def field_input_topic(message_bus_id=None, simulation_id=None):
     """ Utility method for getting the field input topic.
     If message_bus_id is None, it returns topic used by centralized device interfaces to subscribe to control commands.
-    If message_bus_id is not None, it returns topic used by distributed devices interfaces to subscribe to control commands. 
-    
+    If message_bus_id is not None, it returns topic used by distributed devices interfaces to subscribe to control commands.
+
     :param message_bus_id:
     :param simulation_id
-    :return: str: Topic to receive input control commands 
+    :return: str: Topic to receive input control commands
     """
-    
+
     if simulation_id is None:
         return "{}.{}".format(BASE_FIELD_TOPIC, "input")
     else:
-        return "{}.{}.{}.{}".format(BASE_FIELD_TOPIC,"simulation.input",simulation_id,message_bus_id)
+        return "{}.{}.{}.{}".format(BASE_FIELD_TOPIC, "simulation.input", simulation_id,
+                                    message_bus_id)
```

### Comparing `gridappsd_python-2024.1.4a0/gridappsd/utils.py` & `gridappsd_python-2024.4.0a0/gridappsd/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import datetime, time
 from enum import Enum
 from typing import Optional
 
 from dateutil import parser
 import os
-try: # python2.7
+try:    # python2.7
     from urlparse import urlparse
 except ImportError:
     from urllib.parse import urlparse
 
-
 __GRIDAPPSD_URI__ = os.environ.get("GRIDAPPSD_URI", "localhost:61613")
 
 if not __GRIDAPPSD_URI__.startswith("tcp://"):
     __GRIDAPPSD_URI__ = "tcp://" + __GRIDAPPSD_URI__
 __GRIDAPPSD_URI_PARSED__ = urlparse(__GRIDAPPSD_URI__)
 
 
@@ -64,16 +63,15 @@
     if address:
         port = os.environ.get("GRIDAPPS_PORT", "61613")
         if address.startswith("tcp://"):
             address = address.replace("tcp://", "")
 
         return address, port
 
-    return (__GRIDAPPSD_URI_PARSED__.hostname,
-            __GRIDAPPSD_URI_PARSED__.port)
+    return (__GRIDAPPSD_URI_PARSED__.hostname, __GRIDAPPSD_URI_PARSED__.port)
 
 
 def get_gridappsd_application_id():
     """ Retrieve the application_id from the environment.
 
     In order to use this function an environmental variable `GRIDAPPSD_APPLICATION_ID`
     must have been set.  For docker containers this is done in the
```

### Comparing `gridappsd_python-2024.1.4a0/pyproject.toml` & `gridappsd_python-2024.4.0a0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gridappsd-python"
-version = "2024.1.4a0"
+version = "2024.4.0a0"
 description = "A GridAPPS-D Python Adapter"
 authors = [
     "C. Allwardt <3979063+craig8@users.noreply.github.com>",
     "P. Sharma <poorva.sharma@pnnl.gov",
     "A. Fisher <andrew.fisher@pnnl.gov"
 ]
 license = "BSD-3-Clause"
@@ -52,13 +52,13 @@
 [tool.yapfignore]
 ignore_patterns = [
     ".venv/**",
     ".pytest_cache/**",
     "dist/**",
     "docs/**"
 ]
- 
+
 [tool.yapf]
 based_on_style = "pep8"
 spaces_before_comment = 4
 column_limit = 99
 split_before_logical_operator = true
```

### Comparing `gridappsd_python-2024.1.4a0/PKG-INFO` & `gridappsd_python-2024.4.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gridappsd-python
-Version: 2024.1.4a0
+Version: 2024.4.0a0
 Summary: A GridAPPS-D Python Adapter
 Home-page: https://gridappsd.readthedocs.io
 License: BSD-3-Clause
 Keywords: gridappsd,grid,activmq,powergrid,simulation,library
 Author: C. Allwardt
 Author-email: 3979063+craig8@users.noreply.github.com
 Requires-Python: >=3.7.9,<4.0
@@ -199,48 +199,48 @@
 ## Testing
 
 Testing has become an integral part of the software lifecycle.  The `gridappsd-python` library has both unit and
 integration tests available to be run.  In order to execute these, you must have installed the gridappsd-python library
 as above with dev-dependencies.
 
 During the testing phase the docker containers required for the tests are downloaded from
-dockerhub and started.  By default the `develop` tag is used to test the library using pytest.  
+dockerhub and started.  By default the `develop` tag is used to test the library using pytest.
 One can customize the docker image tag by setting the environmental
-variable `GRIDAPPSD_TAG_ENV` either by `export GRIDAPPSD_TAG_ENV=other_tag` or by executing 
+variable `GRIDAPPSD_TAG_ENV` either by `export GRIDAPPSD_TAG_ENV=other_tag` or by executing
 pytest with the following:
 
 ```shell script
 
 # Export environmental variables and all tests will use the same tag (other_tag) to pull from docker hub.
 # Default tag is develop
 export GRIDAPPSD_TAG_ENV=other_tag
 pytest
 
-# Tests also require the username and password to be avaialable as environmental variables 
+# Tests also require the username and password to be avaialable as environmental variables
 # in order for them to properly run these tests
 export GRIDAPPSD_USER=user
 export GRIDAPPSD_PASSWORD=pass
 
 pytest
 ```
 
  ***NOTE: the first running the tests will download all of the docker images associated with the
  [GOSS-GridAPPS-D](http://github.com/GRIDAPPSD/GOSS-GridAPPS-D) repository.  This process may take some time.***
- 
+
 ### Running tests created in a new project
 
 The `gridappsd-python` library exposes a testing environment through the `gridappsd.docker_handler` module.  Including the following
 `conftest.py` in the root of your base test directory allows tests to reference these.  Using these fixtures will start all of the
-base containers required for `gridappsd` to run.  
+base containers required for `gridappsd` to run.
 
 ```python
 
 # conftest.py
-# Create a conftest.py file in the root of the tests directory to enable usage throughout the tests directory and below. 
-# 
+# Create a conftest.py file in the root of the tests directory to enable usage throughout the tests directory and below.
+#
 # Tested project structure an layout
 #
 # project-folder\
 #   mainmodule\
 #     __init__.py
 #     myapplication.py
 #   tests\
@@ -324,15 +324,15 @@
 
 ```
 
 Using the above fixtures from inside a test module and test function looks like the following:
 
 ```python
 
-# Example test function using the gridappsd_client fixture 
+# Example test function using the gridappsd_client fixture
 
 @mock.patch.dict(os.environ, {"GRIDAPPSD_APPLICATION_ID": "helics_goss_bridge.py"})
 def test_gridappsd_status(gridappsd_client):
     gappsd = gridappsd_client
     assert "helics_goss_bridge.py" == gappsd.get_application_id()
     assert gappsd.get_application_status() == ProcessStatusEnum.STARTING.value
     assert gappsd.get_service_status() == ProcessStatusEnum.STARTING.value
@@ -347,8 +347,7 @@
 
     # Invalid
     gappsd.set_service_status("Foo")
     assert gappsd.get_service_status() == ProcessStatusEnum.COMPLETE.value
     assert gappsd.get_application_status() == ProcessStatusEnum.COMPLETE.value
 ```
 
-
```

