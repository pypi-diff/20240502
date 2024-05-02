# Comparing `tmp/PixeraPy-0.381.1.tar.gz` & `tmp/PixeraPy-0.381.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PixeraPy-0.381.1.tar", last modified: Thu May  2 15:20:09 2024, max compression
+gzip compressed data, was "PixeraPy-0.381.2.tar", last modified: Thu May  2 17:40:18 2024, max compression
```

## Comparing `PixeraPy-0.381.1.tar` & `PixeraPy-0.381.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 15:20:09.062096 PixeraPy-0.381.1/
--rw-rw-rw-   0        0        0     1078 2023-11-24 20:54:59.000000 PixeraPy-0.381.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2260 2024-05-02 15:20:09.061600 PixeraPy-0.381.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-02 15:20:09.051680 PixeraPy-0.381.1/PixeraPy/
--rw-rw-rw-   0        0        0       92 2023-11-24 20:52:23.000000 PixeraPy-0.381.1/PixeraPy/__init__.py
--rw-rw-rw-   0        0        0   177978 2024-05-02 14:47:14.000000 PixeraPy-0.381.1/PixeraPy/api_functions.py
--rw-rw-rw-   0        0        0     8498 2023-12-13 03:05:31.000000 PixeraPy-0.381.1/PixeraPy/pixera.py
-drwxrwxrwx   0        0        0        0 2024-05-02 15:20:09.060608 PixeraPy-0.381.1/PixeraPy.egg-info/
--rw-rw-rw-   0        0        0     2260 2024-05-02 15:20:08.000000 PixeraPy-0.381.1/PixeraPy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      255 2024-05-02 15:20:09.000000 PixeraPy-0.381.1/PixeraPy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 15:20:08.000000 PixeraPy-0.381.1/PixeraPy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-05-02 15:20:08.000000 PixeraPy-0.381.1/PixeraPy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-05-02 15:20:08.000000 PixeraPy-0.381.1/PixeraPy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1740 2023-12-13 01:31:34.000000 PixeraPy-0.381.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-02 15:20:09.062096 PixeraPy-0.381.1/setup.cfg
--rw-rw-rw-   0        0        0      885 2024-05-02 14:55:25.000000 PixeraPy-0.381.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 17:40:18.030755 PixeraPy-0.381.2/
+-rw-rw-rw-   0        0        0     1078 2023-11-24 20:54:59.000000 PixeraPy-0.381.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     2408 2024-05-02 17:40:18.030259 PixeraPy-0.381.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-02 17:40:18.015380 PixeraPy-0.381.2/PixeraPy/
+-rw-rw-rw-   0        0        0       92 2023-11-24 20:52:23.000000 PixeraPy-0.381.2/PixeraPy/__init__.py
+-rw-rw-rw-   0        0        0   177978 2024-05-02 14:47:14.000000 PixeraPy-0.381.2/PixeraPy/api_functions.py
+-rw-rw-rw-   0        0        0    10207 2024-05-02 17:35:35.000000 PixeraPy-0.381.2/PixeraPy/pixera.py
+drwxrwxrwx   0        0        0        0 2024-05-02 17:40:18.029763 PixeraPy-0.381.2/PixeraPy.egg-info/
+-rw-rw-rw-   0        0        0     2408 2024-05-02 17:40:17.000000 PixeraPy-0.381.2/PixeraPy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      255 2024-05-02 17:40:17.000000 PixeraPy-0.381.2/PixeraPy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 17:40:17.000000 PixeraPy-0.381.2/PixeraPy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-05-02 17:40:17.000000 PixeraPy-0.381.2/PixeraPy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-02 17:40:17.000000 PixeraPy-0.381.2/PixeraPy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1888 2024-05-02 15:31:24.000000 PixeraPy-0.381.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-02 17:40:18.031252 PixeraPy-0.381.2/setup.cfg
+-rw-rw-rw-   0        0        0      997 2024-05-02 17:39:56.000000 PixeraPy-0.381.2/setup.py
```

### Comparing `PixeraPy-0.381.1/LICENSE.txt` & `PixeraPy-0.381.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PixeraPy-0.381.1/PKG-INFO` & `PixeraPy-0.381.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PixeraPy
-Version: 0.381.1
+Version: 0.381.2
 Summary: Python package for AVStumpfl, Pixera API
 Home-page: https://github.com/Tedcharlesbrown/Pixera-TCB/tree/main/01-Custom/03-API
 Author: Ted Charles Brown
 Author-email: tedcharlesbrown@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,22 +17,25 @@
 ## PixeraPy
 
 Made by Ted Charles Brown<br>
 
 `pip install PixeraPy`
 
 ### Usage
+#### Via PyPi (Recommended)
 ```
 from PixeraPy import Pixera, API
 ip = "127.0.0.1"  # Replace with your Pixera system's IP address
 port = 1400  # Replace with your Pixera system's port if different
 
 pixera = Pixera(ip, port)
 api = API()
 ```
+#### Manual Downlaod
+- [Download PixeraPy](01-Custom/03-API/PixeraPy) directly and place into your working directory
 
 #### Examples
 ```
 from time import sleep
 # ----------------------------- DEFAULT DEBUGGING ---------------------------- #
 output = pixera.send()
 print(output)
```

### Comparing `PixeraPy-0.381.1/PixeraPy/api_functions.py` & `PixeraPy-0.381.2/PixeraPy/api_functions.py`

 * *Files identical despite different names*

### Comparing `PixeraPy-0.381.1/PixeraPy/pixera.py` & `PixeraPy-0.381.2/PixeraPy/pixera.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,26 +8,35 @@
 class Pixera:
     DEFAULT_PORT = 1400
 
     def __init__(self, ip_address="127.0.0.1", port=DEFAULT_PORT):
         self.IP_ADDRESS = ip_address
         self.PORT = port
 
-    def send(self, array=[], protocol="TCP", port=DEFAULT_PORT, verbose=False,) -> str:
+    def send(self, array=[], protocol="TCP", port=DEFAULT_PORT, raw_output=False, verbose=False) -> str:
         """
         Send a message using the specified protocol.
 
         :param protocol: The protocol to use for sending the message. 
                          Options are "TCP", "TCP_DL", "HTTP", "DIRECT".
         :param method: The method to use.
         :param params: Parameters for the method.
         :param message: The message to send.
         :param verbose: Print the send message and the response.
         :return: Response data.
         """
+
+        # Map protocol names to method references
+        protocol_methods = {
+            "TCP": self.send_tcp,
+            "TCP_DL": self.send_tcp_dl,
+            "HTTP": self.send_http,
+            "DIRECT": self.send_direct
+        }
+
         # Default values for method, params, and message
         method, params, message = None, None, None
 
         # Unpack the array based on its length
         if len(array) >= 1:
             method = array[0]
         if len(array) >= 2:
@@ -42,46 +51,78 @@
             if message is None:
                 message = ["Hello from Python!"]
 
         result = None
 
         self.PORT = port
 
-        if protocol == "TCP":
-            result = self.send_tcp(method, params, message, verbose)
-        elif protocol == "TCP_DL":
-            result = self.send_tcp_dl(method, params, message, verbose)
-        elif protocol == "HTTP":
-            result = self.send_http(method, params, message, verbose)
-        elif protocol == "DIRECT":
-            result = self.send_direct(method, params, message, verbose)
+        # Get the method for the specified protocol
+        send_method = protocol_methods.get(protocol)
 
-        if verbose:
-            return result
-        else: 
-            result_index = result.rfind("result\":")
-            result = result[result_index + 8:-1]
+        # Check if the method exists to handle the protocol
+        if send_method:
+            result = send_method(method, params, message, verbose=verbose)
+        else:
+            return "Invalid protocol specified."
+
+        if raw_output:
             return result
+        else:
+            return self.parse_data(result, verbose)
         
     def create_params_dict(self, params, message):
         if params is not None:
             # Check if params is a single string and split it if necessary
             if isinstance(params, str):
                 params = params.split(',')
 
             # Trim whitespace from each parameter name
             params = [param.strip() for param in params]
 
             # Create and return the dictionary
             return {params[i]: message[i] for i in range(len(params))}
+        
+    def parse_data(self, data, verbose=False):
+        def parse_to_json(data):
+            if verbose:
+                print("Received raw data:", data)
+
+            # If not already JSON, decode the data
+            if not isinstance(data, dict):
+                json_start_index = data.find(b'{')
+                if json_start_index != -1:
+                    json_data = data[json_start_index:].decode('utf-8')
+                    # Parse the JSON string into a Python dictionary
+                    try:
+                        json_object = json.loads(json_data)
+                        return json_object
+                    except:
+                        print(json_data)
+                        print("Error parsing JSON data.")
+            else:
+                return data
+            
+        json_data = parse_to_json(data)
 
+        return json_data["result"]
+
+    def receive_message(socket):
+        buffer = ""
+        while True:
+            data = socket.recv(1024).decode('utf-8')
+            if not data:
+                break
+            buffer += data
+            if '\n' in data:
+                break
+        return buffer
         
-    def send_tcp(self, method=None, params=None, message=None, verbose=False):
+    def send_tcp(self, method=None, params=None, message=None, raw_output=False, verbose=False):
         params_dict = self.create_params_dict(params, message)
-                 
+        
         # Create a TCP/IP socket
         with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
             # Set a timeout for the socket operations
             s.settimeout(10)  # 10 seconds timeout
             
             # Connect the socket to the server's address and port
             s.connect((self.IP_ADDRESS, self.PORT))
@@ -100,28 +141,29 @@
             # Calculate the size of the message
             size = len(message)
 
             # Construct the header
             # "pxr1" + 4-byte size (least significant byte first)
             header = b"pxr1" + struct.pack("<I", size)
 
-            message = header + message
-            # Send the header and the message
-            if verbose: print("Sending:", message)
-            s.sendall(message)
+            # Combine the header and the message
+            full_message = header + message
 
-            # Receive the response
-            data = s.recv(1024)
-            data_start = data.decode().rfind("{")
-            data = data.decode()[data_start:]
+            # Send the complete message
+            if verbose: print("Sending:", full_message)
+            s.sendall(full_message)
 
-        return data
+            # Receive the response until the last byte is '}'
+            data = b""
+            while not data.endswith(b'}'):
+                data += s.recv(1024)
 
+            return data
 
-    def send_tcp_dl(self, method=None, params=None, message=None, verbose=False):
+    def send_tcp_dl(self, method=None, params=None, message=None, raw_output=False, verbose=False):
         params_dict = self.create_params_dict(params, message)
 
         # Create a TCP/IP socket
         with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
             # Set a timeout for the socket operations
             s.settimeout(10)  # 10 seconds timeout
             
@@ -132,114 +174,114 @@
             payload = {
                 "jsonrpc": "2.0",
                 "id": 1,
                 "method": method,
                 "params": params_dict
             }
 
+            # Convert the payload to a JSON string, append the '0xPX' delimiter, and encode it
             message = (json.dumps(payload) + '0xPX').encode()
 
-            # Send the request with the "0xPX" delimiter at the end
+            # Send the message
             if verbose: print("Sending:", message)
             s.sendall(message)
 
-            # Receive the response
-            data = s.recv(1024)
+            # Receive the response until the delimiter is found
+            data = b""
+            while not data.endswith(b'0xPX'):
+                data += s.recv(1024)
 
+            data = data[:-4]
 
-        return data.decode()
-    
+            return data
         
         
-    def send_http(self, method=None, params=None, message=None, verbose=False):
+    def send_http(self, method=None, params=None, message=None, raw_output=False, verbose=False):
         params_dict = self.create_params_dict(params, message)
 
         # Define the JSON-RPC request payload
         payload = {
             "jsonrpc": "2.0",
-            "id": 1,  # Adjusted to match the provided ID
+            "id": 1,  # Consistent ID for the JSON-RPC request
             "method": method,
             "params": params_dict
         }
 
-        # Define the headers for the HTTP POST request to match the provided example
+        # Convert the payload to a JSON formatted string to calculate the correct content length
+        json_payload = json.dumps(payload)
+
+        # Define the headers for the HTTP POST request
         headers = {
-            "Content-Type": "text/xml; encoding=utf-8",
+            "Content-Type": "application/json",  # Corrected to 'application/json' for JSON-RPC
             "HOST": f"{self.IP_ADDRESS}:{self.PORT}",
-            "Content-Length": str(len(str(payload))),  # The length of the payload in bytes
-            "Except": "100-continue",
+            "Content-Length": str(len(json_payload)),  # The length of the JSON string in bytes
+            "Expect": "100-continue",  # Corrected typo 'Except' to 'Expect'
             "Connection": "Keep-Alive"
         }
 
         # Send the HTTP POST request with headers
-        if verbose: print("Sending:", headers, payload)
-        response = requests.post(f"http://{self.IP_ADDRESS}:{self.PORT}", headers=headers, json=payload)
+        if verbose: 
+            print("Sending:", headers, payload)
+        response = requests.post(f"http://{self.IP_ADDRESS}:{self.PORT}", headers=headers, data=json_payload)
 
         # Return the response data (can be modified to return other parts of the response if needed)
-        return response.json()
+        if response.ok:
+            return response.json()
+        else:
+            if verbose:
+                print("Failed to receive valid response:", response.text)
+            return None
 
-    def send_direct(self, method=None, params=None, message=None, verbose=False):
-
-        # append direct to the method
+    def send_direct(self, method=None, params=None, message=None, raw_output=False, verbose=False):
+        # Append ".Direct" to the method after "Pixera"
         methods = method.split('.')
         method = ""
         for section in methods:
-            method += f"{section}"
-
+            method += section
             if section == "Pixera":
-                method += ".Direct."
-            else:
-                method += "."
-        method = method[:-1]
+                method += ".Direct"
+            method += "."
 
-        params_dict = self.create_params_dict(params, message)
+        method = method.rstrip('.')  # Remove the trailing dot
 
-        if params is not None:
-            # Convert the params and message lists to a dictionary
+        # Create or update params dictionary based on provided lists
+        if params is not None and message is not None:
             try:
                 params_dict = {params[i]: message[i] for i in range(len(params))}
-            except:
-                pass#TODO: handle this error - message index out of range
-            
+            except IndexError:
+                if verbose:
+                    print("Error: 'message' list is shorter than 'params' list.")
+                return "Parameter and message length mismatch."
+        else:
+            params_dict = self.create_params_dict(params, message)
+
         # Create a TCP/IP socket
         with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
-            # Set a timeout for the socket operations
             s.settimeout(10)  # 10 seconds timeout
-            
-            # Connect the socket to the server's address and port
             s.connect((self.IP_ADDRESS, self.PORT))
 
             # Define the JSON-RPC request payload
             payload = {
                 "jsonrpc": "2.0",
                 "id": 1,
                 "method": method,
                 "params": params_dict
             }
 
-            # Convert the payload to a JSON string and encode it
+            # Serialize and encode the payload
             message = json.dumps(payload).encode()
-
-            # Calculate the size of the message
             size = len(message)
-
-            # Construct the header
-            # "pxr1" + 4-byte size (least significant byte first)
             header = b"pxr1" + struct.pack("<I", size)
-
             message = header + message
-            # Send the header and the message
-            if verbose: print("Sending:", message)
+            
+            if verbose:
+                print("Sending:", message)
             s.sendall(message)
 
-            # Receive the response
+            # Receive and decode the response
             data = s.recv(1024)
 
-            data_start = data.decode().rfind("{")
-            data = data.decode()[data_start:]
-            # data = data.decode()
-
-        return data
+            return data
     
     def return_array(self, input):
         output = input[1:-1].split(',')
         return output
```

### Comparing `PixeraPy-0.381.1/PixeraPy.egg-info/PKG-INFO` & `PixeraPy-0.381.2/PixeraPy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PixeraPy
-Version: 0.381.1
+Version: 0.381.2
 Summary: Python package for AVStumpfl, Pixera API
 Home-page: https://github.com/Tedcharlesbrown/Pixera-TCB/tree/main/01-Custom/03-API
 Author: Ted Charles Brown
 Author-email: tedcharlesbrown@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,22 +17,25 @@
 ## PixeraPy
 
 Made by Ted Charles Brown<br>
 
 `pip install PixeraPy`
 
 ### Usage
+#### Via PyPi (Recommended)
 ```
 from PixeraPy import Pixera, API
 ip = "127.0.0.1"  # Replace with your Pixera system's IP address
 port = 1400  # Replace with your Pixera system's port if different
 
 pixera = Pixera(ip, port)
 api = API()
 ```
+#### Manual Downlaod
+- [Download PixeraPy](01-Custom/03-API/PixeraPy) directly and place into your working directory
 
 #### Examples
 ```
 from time import sleep
 # ----------------------------- DEFAULT DEBUGGING ---------------------------- #
 output = pixera.send()
 print(output)
```

### Comparing `PixeraPy-0.381.1/README.md` & `PixeraPy-0.381.2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -2,22 +2,25 @@
 ## PixeraPy
 
 Made by Ted Charles Brown<br>
 
 `pip install PixeraPy`
 
 ### Usage
+#### Via PyPi (Recommended)
 ```
 from PixeraPy import Pixera, API
 ip = "127.0.0.1"  # Replace with your Pixera system's IP address
 port = 1400  # Replace with your Pixera system's port if different
 
 pixera = Pixera(ip, port)
 api = API()
 ```
+#### Manual Downlaod
+- [Download PixeraPy](01-Custom/03-API/PixeraPy) directly and place into your working directory
 
 #### Examples
 ```
 from time import sleep
 # ----------------------------- DEFAULT DEBUGGING ---------------------------- #
 output = pixera.send()
 print(output)
```

### Comparing `PixeraPy-0.381.1/setup.py` & `PixeraPy-0.381.2/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #WRITTEN BY: Ted Charles Brown
 #ONLY FOR USE WITH PYPI
 
 # IN PARENT DIRECTORY TO API
 # python setup.py sdist bdist_wheel
-# twine upload dist/*
+
+# twine upload dist/* --verbose --repository-url https://upload.pypi.org/legacy/ --username __token__ --password %PYPI_API_TOKEN%
+
 
 from setuptools import setup, find_packages
 
 setup(
     name='PixeraPy',
-    version='0.381.1',
+    version='0.381.2',
     packages=find_packages(),
     description='Python package for AVStumpfl, Pixera API',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Tedcharlesbrown/Pixera-TCB/tree/main/01-Custom/03-API',
     author='Ted Charles Brown',
     author_email='tedcharlesbrown@gmail.com',
```

