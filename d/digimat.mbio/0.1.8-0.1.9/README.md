# Comparing `tmp/digimat.mbio-0.1.8.tar.gz` & `tmp/digimat.mbio-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "digimat.mbio-0.1.8.tar", last modified: Fri Dec  8 15:18:54 2023, max compression
+gzip compressed data, was "digimat.mbio-0.1.9.tar", last modified: Fri Dec  8 16:12:45 2023, max compression
```

## Comparing `digimat.mbio-0.1.8.tar` & `digimat.mbio-0.1.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-12-08 15:18:54.991591 digimat.mbio-0.1.8/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       19 2017-08-22 20:23:51.000000 digimat.mbio-0.1.8/MANIFEST.in
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      509 2023-12-08 15:18:54.991070 digimat.mbio-0.1.8/PKG-INFO
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       67 2023-09-19 19:14:35.000000 digimat.mbio-0.1.8/README.rst
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       38 2023-12-08 15:18:54.991727 digimat.mbio-0.1.8/setup.cfg
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     1343 2023-12-08 15:18:14.000000 digimat.mbio-0.1.8/setup.py
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-12-08 15:18:54.981129 digimat.mbio-0.1.8/src/
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-12-08 15:18:54.982208 digimat.mbio-0.1.8/src/digimat/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       57 2014-09-24 08:13:04.000000 digimat.mbio-0.1.8/src/digimat/__init__.py
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-12-08 15:18:54.990387 digimat.mbio-0.1.8/src/digimat/mbio/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      514 2023-12-04 14:43:21.000000 digimat.mbio-0.1.8/src/digimat/mbio/__init__.py
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     8358 2023-10-31 07:43:47.000000 digimat.mbio-0.1.8/src/digimat/mbio/belimo.py
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     3014 2023-11-09 20:16:37.000000 digimat.mbio-0.1.8/src/digimat/mbio/config.py
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)    23695 2023-10-31 15:29:28.000000 digimat.mbio-0.1.8/src/digimat/mbio/device.py
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)    12509 2023-11-23 17:04:32.000000 digimat.mbio-0.1.8/src/digimat/mbio/digimatplc.py
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)    14583 2023-12-01 09:09:50.000000 digimat.mbio-0.1.8/src/digimat/mbio/gateway.py
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     1430 2023-10-31 15:21:50.000000 digimat.mbio-0.1.8/src/digimat/mbio/items.py
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     7122 2023-12-08 15:18:04.000000 digimat.mbio-0.1.8/src/digimat/mbio/linknotifier.py
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)    11515 2023-12-04 14:43:45.000000 digimat.mbio-0.1.8/src/digimat/mbio/mbio.py
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)    11021 2023-12-01 09:11:14.000000 digimat.mbio-0.1.8/src/digimat/mbio/metzconnect.py
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     6885 2023-10-19 14:42:17.000000 digimat.mbio-0.1.8/src/digimat/mbio/task.py
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     1011 2023-10-12 16:24:03.000000 digimat.mbio-0.1.8/src/digimat/mbio/tasktest.py
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)    13493 2023-12-01 21:48:06.000000 digimat.mbio-0.1.8/src/digimat/mbio/value.py
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     1927 2023-10-19 21:30:17.000000 digimat.mbio-0.1.8/src/digimat/mbio/valuenotifier.py
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      785 2023-11-13 19:47:02.000000 digimat.mbio-0.1.8/src/digimat/mbio/webapi.py
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     2642 2023-10-13 14:28:14.000000 digimat.mbio-0.1.8/src/digimat/mbio/xmlconfig.py
-drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-12-08 15:18:54.984255 digimat.mbio-0.1.8/src/digimat.mbio.egg-info/
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      509 2023-12-08 15:18:54.000000 digimat.mbio-0.1.8/src/digimat.mbio.egg-info/PKG-INFO
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      798 2023-12-08 15:18:54.000000 digimat.mbio-0.1.8/src/digimat.mbio.egg-info/SOURCES.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-12-08 15:18:54.000000 digimat.mbio-0.1.8/src/digimat.mbio.egg-info/dependency_links.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-12-08 15:18:54.000000 digimat.mbio-0.1.8/src/digimat.mbio.egg-info/namespace_packages.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-09-23 08:52:45.000000 digimat.mbio-0.1.8/src/digimat.mbio.egg-info/not-zip-safe
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       60 2023-12-08 15:18:54.000000 digimat.mbio-0.1.8/src/digimat.mbio.egg-info/requires.txt
--rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-12-08 15:18:54.000000 digimat.mbio-0.1.8/src/digimat.mbio.egg-info/top_level.txt
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-12-08 16:12:45.150613 digimat.mbio-0.1.9/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       19 2017-08-22 20:23:51.000000 digimat.mbio-0.1.9/MANIFEST.in
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      509 2023-12-08 16:12:45.150066 digimat.mbio-0.1.9/PKG-INFO
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       67 2023-09-19 19:14:35.000000 digimat.mbio-0.1.9/README.rst
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       38 2023-12-08 16:12:45.150768 digimat.mbio-0.1.9/setup.cfg
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     1343 2023-12-08 16:12:40.000000 digimat.mbio-0.1.9/setup.py
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-12-08 16:12:45.138525 digimat.mbio-0.1.9/src/
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-12-08 16:12:45.139672 digimat.mbio-0.1.9/src/digimat/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       57 2014-09-24 08:13:04.000000 digimat.mbio-0.1.9/src/digimat/__init__.py
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-12-08 16:12:45.149373 digimat.mbio-0.1.9/src/digimat/mbio/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      514 2023-12-04 14:43:21.000000 digimat.mbio-0.1.9/src/digimat/mbio/__init__.py
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     8358 2023-10-31 07:43:47.000000 digimat.mbio-0.1.9/src/digimat/mbio/belimo.py
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     3014 2023-11-09 20:16:37.000000 digimat.mbio-0.1.9/src/digimat/mbio/config.py
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)    23695 2023-10-31 15:29:28.000000 digimat.mbio-0.1.9/src/digimat/mbio/device.py
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)    12509 2023-11-23 17:04:32.000000 digimat.mbio-0.1.9/src/digimat/mbio/digimatplc.py
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)    14583 2023-12-01 09:09:50.000000 digimat.mbio-0.1.9/src/digimat/mbio/gateway.py
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     1430 2023-10-31 15:21:50.000000 digimat.mbio-0.1.9/src/digimat/mbio/items.py
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     7176 2023-12-08 16:12:25.000000 digimat.mbio-0.1.9/src/digimat/mbio/linknotifier.py
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)    11515 2023-12-04 14:43:45.000000 digimat.mbio-0.1.9/src/digimat/mbio/mbio.py
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)    11021 2023-12-01 09:11:14.000000 digimat.mbio-0.1.9/src/digimat/mbio/metzconnect.py
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     6885 2023-10-19 14:42:17.000000 digimat.mbio-0.1.9/src/digimat/mbio/task.py
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     1011 2023-10-12 16:24:03.000000 digimat.mbio-0.1.9/src/digimat/mbio/tasktest.py
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)    13493 2023-12-01 21:48:06.000000 digimat.mbio-0.1.9/src/digimat/mbio/value.py
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     1927 2023-10-19 21:30:17.000000 digimat.mbio-0.1.9/src/digimat/mbio/valuenotifier.py
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      785 2023-11-13 19:47:02.000000 digimat.mbio-0.1.9/src/digimat/mbio/webapi.py
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)     2642 2023-10-13 14:28:14.000000 digimat.mbio-0.1.9/src/digimat/mbio/xmlconfig.py
+drwxr-xr-x   0 laloutrejoyeuse   (501) staff       (20)        0 2023-12-08 16:12:45.141879 digimat.mbio-0.1.9/src/digimat.mbio.egg-info/
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      509 2023-12-08 16:12:45.000000 digimat.mbio-0.1.9/src/digimat.mbio.egg-info/PKG-INFO
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)      798 2023-12-08 16:12:45.000000 digimat.mbio-0.1.9/src/digimat.mbio.egg-info/SOURCES.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-12-08 16:12:45.000000 digimat.mbio-0.1.9/src/digimat.mbio.egg-info/dependency_links.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-12-08 16:12:45.000000 digimat.mbio-0.1.9/src/digimat.mbio.egg-info/namespace_packages.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        1 2023-09-23 08:52:45.000000 digimat.mbio-0.1.9/src/digimat.mbio.egg-info/not-zip-safe
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)       60 2023-12-08 16:12:45.000000 digimat.mbio-0.1.9/src/digimat.mbio.egg-info/requires.txt
+-rw-r--r--   0 laloutrejoyeuse   (501) staff       (20)        8 2023-12-08 16:12:45.000000 digimat.mbio-0.1.9/src/digimat.mbio.egg-info/top_level.txt
```

### Comparing `digimat.mbio-0.1.8/setup.py` & `digimat.mbio-0.1.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # Get the long description from the relevant file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='digimat.mbio',
-    version='0.1.8',
+    version='0.1.9',
     description='Digimat MBIO System',
     long_description=long_description,
     namespace_packages=['digimat'],
     author='Frederic Hess',
     author_email='fhess@st-sa.ch',
     url='https://github.com/digimat/digimat-mbio',
     license='PSF',
```

### Comparing `digimat.mbio-0.1.8/src/digimat/mbio/__init__.py` & `digimat.mbio-0.1.9/src/digimat/mbio/__init__.py`

 * *Files identical despite different names*

### Comparing `digimat.mbio-0.1.8/src/digimat/mbio/belimo.py` & `digimat.mbio-0.1.9/src/digimat/mbio/belimo.py`

 * *Files identical despite different names*

### Comparing `digimat.mbio-0.1.8/src/digimat/mbio/config.py` & `digimat.mbio-0.1.9/src/digimat/mbio/config.py`

 * *Files identical despite different names*

### Comparing `digimat.mbio-0.1.8/src/digimat/mbio/device.py` & `digimat.mbio-0.1.9/src/digimat/mbio/device.py`

 * *Files identical despite different names*

### Comparing `digimat.mbio-0.1.8/src/digimat/mbio/digimatplc.py` & `digimat.mbio-0.1.9/src/digimat/mbio/digimatplc.py`

 * *Files identical despite different names*

### Comparing `digimat.mbio-0.1.8/src/digimat/mbio/gateway.py` & `digimat.mbio-0.1.9/src/digimat/mbio/gateway.py`

 * *Files identical despite different names*

### Comparing `digimat.mbio-0.1.8/src/digimat/mbio/items.py` & `digimat.mbio-0.1.9/src/digimat/mbio/items.py`

 * *Files identical despite different names*

### Comparing `digimat.mbio-0.1.8/src/digimat/mbio/linknotifier.py` & `digimat.mbio-0.1.9/src/digimat/mbio/linknotifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,16 @@
             if not self._connected:
                 if time.time()>=self._timeoutInhibit:
                     self.logger.info('Opening link %s:%d' % (self._host, self._port))
                     self._socket=socket.socket(socket.AF_INET, socket.SOCK_STREAM)
                     self._socket.settimeout(3)
                     if self._interface:
                         self.logger.info('Using interface %s' % self._interface)
-                        self._socket.setsockopt(socket.SOL_SOCKET, 25, self._interface + '\0')
+                        ifname=(self._interface+'\0').encode('utf-8')
+                        self._socket.setsockopt(socket.SOL_SOCKET, 25, ifname)
                     address=(self._host, self._port)
                     self._socket.connect(address)
                     self._socket.settimeout(0)
                     self._connected=True
                     self._timeoutInhibit=time.time()+5
                     self.logger.info("Link connected to %s:%d" % (self._host, self._port))
                     self.resetActivityTimeout()
```

### Comparing `digimat.mbio-0.1.8/src/digimat/mbio/mbio.py` & `digimat.mbio-0.1.9/src/digimat/mbio/mbio.py`

 * *Files identical despite different names*

### Comparing `digimat.mbio-0.1.8/src/digimat/mbio/metzconnect.py` & `digimat.mbio-0.1.9/src/digimat/mbio/metzconnect.py`

 * *Files identical despite different names*

### Comparing `digimat.mbio-0.1.8/src/digimat/mbio/task.py` & `digimat.mbio-0.1.9/src/digimat/mbio/task.py`

 * *Files identical despite different names*

### Comparing `digimat.mbio-0.1.8/src/digimat/mbio/tasktest.py` & `digimat.mbio-0.1.9/src/digimat/mbio/tasktest.py`

 * *Files identical despite different names*

### Comparing `digimat.mbio-0.1.8/src/digimat/mbio/value.py` & `digimat.mbio-0.1.9/src/digimat/mbio/value.py`

 * *Files identical despite different names*

### Comparing `digimat.mbio-0.1.8/src/digimat/mbio/valuenotifier.py` & `digimat.mbio-0.1.9/src/digimat/mbio/valuenotifier.py`

 * *Files identical despite different names*

### Comparing `digimat.mbio-0.1.8/src/digimat/mbio/webapi.py` & `digimat.mbio-0.1.9/src/digimat/mbio/webapi.py`

 * *Files identical despite different names*

### Comparing `digimat.mbio-0.1.8/src/digimat/mbio/xmlconfig.py` & `digimat.mbio-0.1.9/src/digimat/mbio/xmlconfig.py`

 * *Files identical despite different names*

### Comparing `digimat.mbio-0.1.8/src/digimat.mbio.egg-info/SOURCES.txt` & `digimat.mbio-0.1.9/src/digimat.mbio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

