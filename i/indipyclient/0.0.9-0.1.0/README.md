# Comparing `tmp/indipyclient-0.0.9.tar.gz` & `tmp/indipyclient-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indipyclient-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "indipyclient-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `indipyclient-0.0.9.tar` & `indipyclient-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1078 2024-03-29 22:07:10.000000 indipyclient-0.0.9/LICENSE
--rw-r--r--   0        0        0     2646 2024-04-13 20:38:26.000000 indipyclient-0.0.9/README.md
--rw-r--r--   0        0        0      330 2024-04-28 19:27:59.000000 indipyclient-0.0.9/indipyclient/__init__.py
--rw-r--r--   0        0        0     3089 2024-04-03 21:43:04.000000 indipyclient-0.0.9/indipyclient/__main__.py
--rw-r--r--   0        0        0        0 2023-08-14 16:40:46.000000 indipyclient-0.0.9/indipyclient/console/__init__.py
--rw-r--r--   0        0        0    19759 2024-04-28 18:10:23.000000 indipyclient-0.0.9/indipyclient/console/consoleclient.py
--rw-r--r--   0        0        0    48356 2024-04-28 18:54:10.000000 indipyclient-0.0.9/indipyclient/console/widgets.py
--rw-r--r--   0        0        0   144085 2024-04-28 18:17:36.000000 indipyclient-0.0.9/indipyclient/console/windows.py
--rw-r--r--   0        0        0      192 2023-09-20 21:15:05.000000 indipyclient-0.0.9/indipyclient/error.py
--rw-r--r--   0        0        0    26765 2024-04-28 19:07:19.000000 indipyclient-0.0.9/indipyclient/events.py
--rw-r--r--   0        0        0    34733 2024-04-28 18:01:26.000000 indipyclient-0.0.9/indipyclient/ipyclient.py
--rw-r--r--   0        0        0    16189 2024-04-28 19:10:31.000000 indipyclient-0.0.9/indipyclient/propertymembers.py
--rw-r--r--   0        0        0    27645 2024-04-28 18:21:13.000000 indipyclient-0.0.9/indipyclient/propertyvectors.py
--rw-r--r--   0        0        0      935 2024-04-28 19:27:49.000000 indipyclient-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     3417 1970-01-01 00:00:00.000000 indipyclient-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-03-29 22:07:10.000000 indipyclient-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2646 2024-04-13 20:38:26.000000 indipyclient-0.1.0/README.md
+-rw-r--r--   0        0        0      416 2024-05-02 12:33:18.000000 indipyclient-0.1.0/indipyclient/__init__.py
+-rw-r--r--   0        0        0     3245 2024-05-02 10:21:26.000000 indipyclient-0.1.0/indipyclient/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-14 16:40:46.000000 indipyclient-0.1.0/indipyclient/console/__init__.py
+-rw-r--r--   0        0        0    21197 2024-05-02 11:05:08.000000 indipyclient-0.1.0/indipyclient/console/consoleclient.py
+-rw-r--r--   0        0        0    48356 2024-04-28 18:54:10.000000 indipyclient-0.1.0/indipyclient/console/widgets.py
+-rw-r--r--   0        0        0   144085 2024-04-28 18:17:36.000000 indipyclient-0.1.0/indipyclient/console/windows.py
+-rw-r--r--   0        0        0      192 2023-09-20 21:15:05.000000 indipyclient-0.1.0/indipyclient/error.py
+-rw-r--r--   0        0        0    26765 2024-05-02 11:52:00.000000 indipyclient-0.1.0/indipyclient/events.py
+-rw-r--r--   0        0        0    32116 2024-05-02 11:56:45.000000 indipyclient-0.1.0/indipyclient/ipyclient.py
+-rw-r--r--   0        0        0    16211 2024-04-28 20:08:14.000000 indipyclient-0.1.0/indipyclient/propertymembers.py
+-rw-r--r--   0        0        0    27645 2024-04-28 18:21:13.000000 indipyclient-0.1.0/indipyclient/propertyvectors.py
+-rw-r--r--   0        0        0      935 2024-05-02 12:33:02.000000 indipyclient-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3417 1970-01-01 00:00:00.000000 indipyclient-0.1.0/PKG-INFO
```

### Comparing `indipyclient-0.0.9/LICENSE` & `indipyclient-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.9/README.md` & `indipyclient-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.9/indipyclient/__main__.py` & `indipyclient-0.1.0/indipyclient/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,17 +28,17 @@
     parser = argparse.ArgumentParser(usage="indipyclient [options]",
                                      formatter_class=argparse.RawDescriptionHelpFormatter,
                                      description="Terminal client to communicate to an INDI service.",
                                      epilog="""The BLOB's folder can also be set from within the session.
 Setting loglevel and logfile should only be used for brief
 diagnostic purposes, the logfile could grow very big.
 loglevel:1 Information and error messages only,
-loglevel:2 log vector tags without members or contents,
-loglevel:3 log vectors and members - but not BLOB contents,
-loglevel:4 log vectors and all contents
+loglevel:2 As 1 plus xml vector tags without members or contents,
+loglevel:3 As 1 plus xml vectors and members - but not BLOB contents,
+loglevel:4 As 1 plus xml vectors and all contents
 """)
     parser.add_argument("-p", "--port", type=int, default=7624, help="Port of the INDI server (default 7624).")
     parser.add_argument("--host", default="localhost", help="Hostname/IP of the INDI server (default localhost).")
     parser.add_argument("-b", "--blobs", help="Optional folder where BLOB's will be saved.")
     parser.add_argument("--loglevel", help="Enables logging, value 1, 2, 3 or 4.")
     parser.add_argument("--logfile", help="File where logs will be saved")
 
@@ -59,27 +59,30 @@
                 return 1
     else:
         blobfolder = None
 
     # On receiving an event, the client appends it into eventque
     client = ConsoleClient(indihost=args.host, indiport=args.port, eventque=eventque)
 
+    # Monitors eventque and acts on the events, creates the console screens
+    control = ConsoleControl(client, blobfolder=blobfolder)
+
     if args.loglevel and args.logfile:
         try:
             loglevel = int(args.loglevel)
             if loglevel not in (1,2,3,4):
                 print("Error: If given, the loglevel should be 1, 2, 3 or 4")
                 return 1
+            level = control.setlogging(loglevel, args.logfile)
+            if level != loglevel:
+                print("Error: Failed to set logging")
+                return 1
         except:
             print("Error: If given, the loglevel should be 1, 2, 3 or 4")
             return 1
-        client.setlogging(loglevel, args.logfile)
-
-    # Monitors eventque and acts on the events, creates the console screens
-    control = ConsoleControl(client, blobfolder=blobfolder)
 
     asyncio.run(runclient(client, control))
 
     return 0
 
 
 if __name__ == "__main__":
```

### Comparing `indipyclient-0.0.9/indipyclient/console/consoleclient.py` & `indipyclient-0.1.0/indipyclient/console/consoleclient.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 
-import asyncio, sys, traceback
+import asyncio, sys, traceback, pathlib
 
 import curses
 
+import logging
+logger = logging.getLogger('indipyclient')
+
 from ..ipyclient import IPyClient
 from ..events import (delProperty, defSwitchVector, defTextVector, defNumberVector, defLightVector, defBLOBVector,
                      setSwitchVector, setTextVector, setNumberVector, setLightVector, setBLOBVector, Message, VectorTimeOut)
 
 from . import windows
 from . import widgets
 
@@ -85,14 +88,48 @@
         # list of known device names, this is needed to send
         # BLOB's enabled
         self.devicenames = []
 
         # BLOBfiles, is a dictionary of {(devicename,vectorname,membername):filepath}
         self.BLOBfiles = {}
 
+    def setlogging(self, level, logfile):
+        """Sets the logging level and logfile, returns the level, which will be None on failure.
+           As default, no logging is enabled. If logging is required, this can be called, level
+           should be an integer, one of 1, 2, 3 or 4.
+           Be warned, there is no logfile rotation, files can become large.
+           Note: it may be useful in another terminal to try tail -f logfile"""
+
+        # loglevel:1 Information and error messages only,  -> error
+        # loglevel:2 log vector tags without members or contents  -> warning
+        # loglevel:3 log vectors and members - but not BLOB contents  -> info
+        # loglevel:4 log vectors and all contents   -> debug
+
+        try:
+            if not level in (1, 2, 3, 4):
+                return None
+            logfile = pathlib.Path(logfile).expanduser().resolve()
+
+            if level == 4:
+                logger.setLevel(logging.DEBUG)
+                self.client.debug_verbosity(3)
+            elif level == 3:
+                logger.setLevel(logging.DEBUG)
+                self.client.debug_verbosity(2)
+            elif level == 2:
+                logger.setLevel(logging.DEBUG)
+                self.client.debug_verbosity(1)
+            elif level == 1:
+                logger.setLevel(logging.INFO)
+            logfile = pathlib.Path(logfile).expanduser().resolve()
+            fh = logging.FileHandler(logfile)
+            logger.addHandler(fh)
+        except:
+            return
+        return level
 
 
     def color(self, state):
         "Returns curses.color_pair given a state"
         if not curses.has_colors():
             return curses.color_pair(0)
         state = state.lower()
@@ -100,26 +137,23 @@
             return curses.color_pair(1)
         elif state == "busy":
             return curses.color_pair(2)
         elif state == "alert":
             return curses.color_pair(3)
         return curses.color_pair(0)
 
+
     @property
     def connected(self):
         return self.client.connected
 
 
-    def shutdown(self, exc=None):
-        """If exc is an exception, and logs are enabled, logs it.
-           Sets self._shutdown to True which shuts down the client"""
+    def shutdown(self):
+        "Sets self._shutdown to True which shuts down the client"
         self._shutdown = True
-        if self.client.level and not(exc is None):
-            bytex = "".join(traceback.format_exception(exc)).encode()
-            self.client.logfp.write(b"\n"+bytex)
 
 
     async def _checkshutdown(self):
         "If self._shutdown becomes True, shutdown"
         while not self._shutdown:
             await asyncio.sleep(0)
         await self.client.report("Shutting down client - please wait")
@@ -237,16 +271,17 @@
                 if isinstance(self.screen, windows.VectorScreen) and (self.screen.vectorname == event.vectorname):
                     # The event refers to this vector
                     self.screen.update(event)
 
         except asyncio.CancelledError:
             self.shutdown()
             raise
-        except Exception as e:
-            self.shutdown(e)
+        except Exception:
+            logger.exception("Error in updatescreen")
+            self.shutdown()
         finally:
             self.updatescreenstopped = True
 
 
     async def getinput(self):
         try:
             while not self.stop:
@@ -406,16 +441,17 @@
                         self.screen = windows.ChooseVectorScreen(self.stdscr, self, self.screen.devicename, group=self.screen.vector.group)
                         self.screen.show()
                         continue
 
         except asyncio.CancelledError:
             self.shutdown()
             raise
-        except Exception as e:
-            self.shutdown(e)
+        except Exception:
+            logger.exception("Error in getinput")
+            self.shutdown()
         finally:
             self.getinputstopped = True
 
 
     def send_enableBLOB(self):
         "Sends Also to enable blobs for all devices"
         if not self.blobenabled:
```

### Comparing `indipyclient-0.0.9/indipyclient/console/widgets.py` & `indipyclient-0.1.0/indipyclient/console/widgets.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.9/indipyclient/console/windows.py` & `indipyclient-0.1.0/indipyclient/console/windows.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.9/indipyclient/events.py` & `indipyclient-0.1.0/indipyclient/events.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.9/indipyclient/ipyclient.py` & `indipyclient-0.1.0/indipyclient/ipyclient.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 
 from datetime import datetime, timezone
 
 from base64 import standard_b64encode
 
 import xml.etree.ElementTree as ET
 
+import logging
+logger = logging.getLogger(__name__)
+
 from . import events
 
 from .error import ParseException, ConnectionTimeOut
 
 
 # All xml data received from the driver should be contained in one of the following tags
 TAGS = (b'message',
@@ -139,112 +142,47 @@
         self.vector_timeout_max = 10
 
         # and shutdown routine sets this to True to stop coroutines
         self._stop = False
         # this is set to True when asyncrun is finished
         self.stopped = False
 
-        # logging level and filepointer to logfile
-        # level, None for no logging, 1 for informtion and errors only,
-        #                             2 for transmitted/received vector tags only,
-        #                             3 for transmitted/received vectors, members and contents (apart from BLOB's)
-        #                             4 for all transmitted/received data
-        self._level = None
-        self._logfile = None
-        self._logfp = None
-
-    @property
-    def level(self):
-        "Can be read, but only set via setlogging method"
-        return self._level
-
-    @property
-    def logfile(self):
-        "Can be read, but only set via setlogging method"
-        return self._logfile
-
-    @property
-    def logfp(self):
-        "Can be read, but only set via setlogging method"
-        return self._logfp
-
-    def setlogging(self, level, logfile):
-        """Sets the logging level and logfile, returns the level, which will be None on failure.
-           As default, the level is None, indicating no logging. Apart from None, level should
-           be an integer, one of 1, 2, 3 or 4.
-           Be warned, there is no logfile rotation, files can become large.
-           Note: it may be useful in another terminal to try tail -f logfile"""
-        try:
-            if self._logfp:
-                self._logfp.close()
-                self._logfp = None
-
-            if level in (1, 2, 3, 4):
-                self._level = level
-            else:
-                self._level = None
-                self._logfile = None
-                return None
-
-            logfile = pathlib.Path(logfile).expanduser().resolve()
-            self._logfp = open(logfile, "wb", buffering=0)
-            if not self._logfp.writable():
-                self._logfp.close()
-                self._level = None
-                self._logfp = None
-                self._logfile = None
-                return None
-        except:
-            self._level = None
-            if self._logfp:
-                self._logfp.close()
-            self._logfp = None
-            self._logfile = None
-            return None
-        self._logfile = logfile
-        return self._level
+        # Indicates how verbose the debug xml logs will be when created.
+        self._verbose = 1
+
+
+    def debug_verbosity(self, verbose):
+        """Indicate how verbose the debug xml logs will be when created.
+           1 for transmitted/received vector tags only,
+           2 for transmitted/received vectors, members and contents (apart from BLOBs)
+           3 for all transmitted/received data including BLOBs."""
+        if verbose not in (1,2,3):
+            raise ValueError
+        self._verbose = verbose
+
 
     def shutdown(self):
         "Shuts down the client"
-        if self._logfp:
-            self._logfp.close()
-            self._level = None
-            self._logfp = None
-            self._logfile = None
         self._stop = True
 
     async def report(self, message):
         """This injects a message into the received data, which will be
            picked up by the rxevent method. It is a way to set a message
            on to your client display, in the same way messages come from
            the INDI service. If logging is enabled the message will also
-           be written to the logfile"""
+           be logged at level INFO"""
         try:
             timestamp = datetime.now(tz=timezone.utc)
             timestamp = timestamp.replace(tzinfo=None)
-            if self._level:
-                reportmessage  = f"\n{timestamp.isoformat(sep='T')} {message}"
-                self._logfp.write(reportmessage.encode())
+            logger.info(message)
             root = ET.fromstring(f"<message timestamp=\"{timestamp.isoformat(sep='T')}\" message=\"{message}\" />")
             event = events.Message(root, None, self)
             await self.rxevent(event)
-        except Exception as e:
-            if self._level:
-                bytex = "".join(traceback.format_exception(e)).encode()
-                self._logfp.write(bytex)
-
-
-    def log(self, message):
-        """If logging is enabled, this writes the message, with a timestamp
-           to the logfile"""
-        if self._level:
-            timestamp = datetime.now(tz=timezone.utc)
-            timestamp = timestamp.replace(tzinfo=None)
-            reportmessage  = f"\n{timestamp.isoformat(sep='T')} {message}"
-            self._logfp.write(reportmessage.encode())
+        except Exception :
+            logger.exception("Error in IPyClient.report method")
 
 
     def enabledlen(self):
         "Returns the number of enabled devices"
         return sum(map(lambda x:1 if x.enable else 0, self.data.values()))
 
 
@@ -273,14 +211,15 @@
                                          self._check_alive(writer)
                                          )
                 except ConnectionRefusedError:
                     await self.report(f"Error: Connection refused on {self.indihost}:{self.indiport}")
                 except ConnectionResetError:
                     await self.report("Error: Connection Lost")
                 except Exception:
+                    logger.exception("Connection Error")
                     await self.report("Error: Connection failed")
                 self._clear_connection()
                 if self._stop:
                     break
                 else:
                     await self.report(f"Connection failed, re-trying...")
 
@@ -288,18 +227,16 @@
                 # that self._stop has not been set
                 count = 0
                 while not self._stop:
                     await asyncio.sleep(0.5)
                     count += 1
                     if count >= 10:
                         break
-        except Exception as e:
-            if self._level:
-                bytex = "".join(traceback.format_exception(e)).encode()
-                self._logfp.write(bytex)
+        except Exception:
+            logger.exception("Error in IPyClient._comms method")
         finally:
             self.shutdown()
 
 
     def _clear_connection(self):
         "On a connection closing down, clears queues"
         self.connected = False
@@ -346,40 +283,34 @@
         except KeyboardInterrupt:
             self.shutdown()
         finally:
             self.connected = False
 
 
     def _logtx(self, txdata):
-        "log data to file"
-        if (not self._level) or (self._level == 1):
-            return
-        self._logfp.write(b"\nTX:: ")
-        if self._level == 2:
-            for element in txdata:
-                txdata.remove(element)
-            txdata.text = ""
-            binarydata = ET.tostring(txdata, short_empty_elements=False).split(b">")
-            self._logfp.write(binarydata[0]+b">")
-        if self._level == 3:
+        "log tx data with level debug, and detail depends on self._verbose"
+
+        startlog = "TX:: "
+        if self._verbose == 3:
+            binarydata = ET.tostring(txdata)
+            logger.debug(startlog + binarydata.decode())
+        elif self._verbose == 2:
             tag = txdata.tag
             for element in txdata:
-                if tag  == "newBLOBVector":
+                if tag == "newBLOBVector":
                     element.text = "NOT LOGGED"
             binarydata = ET.tostring(txdata)
-            self._logfp.write(binarydata)
-        if self._level == 4:
-            if txdata.tag == "newBLOBVector" and len(txdata):
-                # txdata is a newBLOBVector containing blobs
-                # the generator blob_xml_bytes yields bytes
-                for binarydata in blob_xml_bytes(txdata):
-                    self._logfp.write(binarydata)
-            else:
-                binarydata = ET.tostring(txdata)
-                self._logfp.write(binarydata)
+            logger.debug(startlog + binarydata.decode())
+        elif self._verbose == 1:
+            for element in txdata:
+                txdata.remove(element)
+            txdata.text = ""
+            binarydata = ET.tostring(txdata, short_empty_elements=False).split(b">")
+            logger.debug(startlog + binarydata[0].decode()+">")
+
 
 
     async def _run_tx(self, writer):
         "Monitors self.writerque and if it has data, uses writer to send it"
         try:
             while self.connected and (not self._stop):
                 await asyncio.sleep(0)
@@ -403,42 +334,40 @@
                     await writer.drain()
 
                 # data has been transmitted set timers going, do not set timer
                 # for enableBLOB as no answer is expected for that
                 if (self.tx_timer is None) and (txdata.tag != "enableBLOB"):
                     self.tx_timer = time.time()
                 self.idle_timer = time.time()
-
-                if self._level:
+                if logger.isEnabledFor(logging.DEBUG):
                     self._logtx(txdata)
         except KeyboardInterrupt:
             self.shutdown()
 
     def _logrx(self, rxdata):
-        "log data to file"
-        if (not self._level) or (self._level == 1):
-            return
-        data = copy.deepcopy(rxdata)
-        self._logfp.write(b"\nRX:: ")
-        if self._level == 2:
-            for element in data:
-                data.remove(element)
-            data.text = ""
-            binarydata = ET.tostring(data, short_empty_elements=False).split(b">")
-            self._logfp.write(binarydata[0]+b">")
-        if self._level == 3:
+        "log rx data to file"
+        startlog = "RX:: "
+        if self._verbose == 3:
+            binarydata = ET.tostring(rxdata)
+            logger.debug(startlog + binarydata.decode())
+        elif self._verbose == 2:
+            data = copy.deepcopy(rxdata)
             tag = data.tag
             for element in data:
                 if tag  == "newBLOBVector":
                     element.text = "NOT LOGGED"
             binarydata = ET.tostring(data)
-            self._logfp.write(binarydata)
-        if self._level == 4:
-            binarydata = ET.tostring(data)
-            self._logfp.write(binarydata)
+            logger.debug(startlog + binarydata.decode())
+        elif self._verbose == 1:
+            data = copy.deepcopy(rxdata)
+            for element in data:
+                data.remove(element)
+            data.text = ""
+            binarydata = ET.tostring(data, short_empty_elements=False).split(b">")
+            logger.debug(startlog + binarydata[0].decode() + ">")
 
 
     async def _run_rx(self, reader):
         "pass xml.etree.ElementTree data to readerque"
         try:
             source = self._datasource(reader)
             while self.connected and (not self._stop):
@@ -450,21 +379,26 @@
                     # and place rxdata into readerque
                     try:
                         self.readerque.put_nowait(rxdata)
                     except asyncio.QueueFull:
                         # The queue is full, something may be wrong
                         # discard this data and continue
                         pass
-                if self._level:
-                    self._logrx(rxdata)
+                    else:
+                        if logger.isEnabledFor(logging.DEBUG):
+                            self._logrx(rxdata)
         except RuntimeError:
             # catches StopAsyncIteration and stops this coroutine
             pass
         except KeyboardInterrupt:
             self.shutdown()
+        except Exception:
+            logger.exception("Error in _run_rx")
+            self.shutdown()
+
 
 
     async def _datasource(self, reader):
         "get received data, parse it, and yield it as xml.etree.ElementTree object"
         data_in = self._datainput(reader)
         message = b''
         messagetagnumber = None
@@ -612,17 +546,15 @@
                     self.readerque.task_done()
                 # and to get here, continue has not been called
                 # and an event has been created, call the user event handling function
                 await self.rxevent(event)
         except asyncio.CancelledError:
             raise
         except Exception as e:
-            if self._level:
-                bytex = "".join(traceback.format_exception(e)).encode()
-                self._logfp.write(bytex)
+            logger.exception("Error in IPyClient._rxhandler method")
         finally:
             self.shutdown()
 
 
     def snapshot(self):
         """Take a snapshot of the devices and returns a dictionary of device
            names to objects which are restricted copies of the current state of devices and
@@ -718,17 +650,15 @@
                             await self.report("getProperties sent")
                         count += 1
                         if count >= 10:
                             count = 0
         except asyncio.CancelledError:
              raise
         except Exception as e:
-            if self._level:
-                bytex = "".join(traceback.format_exception(e)).encode()
-                self._logfp.write(bytex)
+            logger.exception("Error in IPyClient._timeout_monitor method")
         finally:
             self.shutdown()
 
 
     def send_getProperties(self, devicename=None, vectorname=None):
         """Sends a getProperties request. On startup the IPyClient object
            will automatically send getProperties, so typically you will
```

### Comparing `indipyclient-0.0.9/indipyclient/propertymembers.py` & `indipyclient-0.1.0/indipyclient/propertymembers.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 import sys, pathlib
 
 from .error import ParseException
 
 
 def getfloat(value):
-    """The INDI spec allows a number of different number formats, given a number,
-       this returns a float.
+    """The INDI spec specifies several different number formats, given a number
+       in any of these formats, this returns a float.
        If an error occurs while parsing the number, a TypeError exception is raised."""
     try:
         if isinstance(value, float):
             return value
         if isinstance(value, int):
             return float(value)
         if not isinstance(value, str):
@@ -188,15 +188,15 @@
         super().__init__(name, label, membervalue)
         self.format = format
         self.min = min
         self.max = max
         self.step = step
 
     def getfloat(self, value):
-        """The INDI spec allows a number of different number formats, this method returns
+        """The INDI spec specifies several different number formats, this method returns
            the given value as a float.
            If an error occurs while parsing the number, a TypeError exception is raised."""
         return getfloat(value)
 
 
     def getfloatvalue(self):
         """The INDI spec allows a number of different number formats, this method returns
```

### Comparing `indipyclient-0.0.9/indipyclient/propertyvectors.py` & `indipyclient-0.1.0/indipyclient/propertyvectors.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.9/pyproject.toml` & `indipyclient-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "indipyclient"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License", "Operating System :: POSIX :: Linux","Topic :: Scientific/Engineering :: Astronomy", "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator"]
-version = "0.0.9"
+version = "0.1.0"
 description="Pure python package, providing a terminal client and a set of classes which can be used to create scripts or clients to control remote instruments using the INDI protocol."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords=['indi', 'client', 'astronomy', 'instrument']
 
 [project.urls]
 Documentation = "https://indipyclient.readthedocs.io"
```

### Comparing `indipyclient-0.0.9/PKG-INFO` & `indipyclient-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indipyclient
-Version: 0.0.9
+Version: 0.1.0
 Summary: Pure python package, providing a terminal client and a set of classes which can be used to create scripts or clients to control remote instruments using the INDI protocol.
 Keywords: indi,client,astronomy,instrument
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

