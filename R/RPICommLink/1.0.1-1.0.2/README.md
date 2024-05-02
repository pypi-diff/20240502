# Comparing `tmp/RPICommLink-1.0.1.tar.gz` & `tmp/RPICommLink-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RPICommLink-1.0.1.tar", last modified: Tue Apr 30 02:45:19 2024, max compression
+gzip compressed data, was "RPICommLink-1.0.2.tar", last modified: Thu May  2 08:43:47 2024, max compression
```

## Comparing `RPICommLink-1.0.1.tar` & `RPICommLink-1.0.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 02:45:19.394815 RPICommLink-1.0.1/
--rw-rw-rw-   0        0        0      159 2024-04-30 02:45:19.393816 RPICommLink-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-30 02:45:19.386430 RPICommLink-1.0.1/RPICommLink/
--rw-rw-rw-   0        0        0    16050 2024-04-30 02:39:19.000000 RPICommLink-1.0.1/RPICommLink/rpicommlink.py
-drwxrwxrwx   0        0        0        0 2024-04-30 02:45:19.391787 RPICommLink-1.0.1/RPICommLink.egg-info/
--rw-rw-rw-   0        0        0      159 2024-04-30 02:45:19.000000 RPICommLink-1.0.1/RPICommLink.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      175 2024-04-30 02:45:19.000000 RPICommLink-1.0.1/RPICommLink.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 02:45:19.000000 RPICommLink-1.0.1/RPICommLink.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-30 02:45:19.000000 RPICommLink-1.0.1/RPICommLink.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 02:45:19.395811 RPICommLink-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      270 2024-04-30 02:45:01.000000 RPICommLink-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 08:43:47.506676 RPICommLink-1.0.2/
+-rw-rw-rw-   0        0        0      159 2024-05-02 08:43:47.505679 RPICommLink-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-02 08:43:47.501690 RPICommLink-1.0.2/RPICommLink/
+-rw-rw-rw-   0        0        0    14854 2024-05-02 08:43:36.000000 RPICommLink-1.0.2/RPICommLink/rpicommlink.py
+drwxrwxrwx   0        0        0        0 2024-05-02 08:43:47.505679 RPICommLink-1.0.2/RPICommLink.egg-info/
+-rw-rw-rw-   0        0        0      159 2024-05-02 08:43:47.000000 RPICommLink-1.0.2/RPICommLink.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      175 2024-05-02 08:43:47.000000 RPICommLink-1.0.2/RPICommLink.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 08:43:47.000000 RPICommLink-1.0.2/RPICommLink.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-02 08:43:47.000000 RPICommLink-1.0.2/RPICommLink.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 08:43:47.506676 RPICommLink-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      270 2024-05-02 08:26:32.000000 RPICommLink-1.0.2/setup.py
```

### Comparing `RPICommLink-1.0.1/RPICommLink/rpicommlink.py` & `RPICommLink-1.0.2/RPICommLink/rpicommlink.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,31 +7,32 @@
     def __init__(self, rpi_port: int = 11451, password: str = '88888888'):
         """
         self.return_data:返回的数据，等待数据返回时为None。
         self.return_data:发送的数据，等待数据发送时为None。
         self.socket_list:当前连接的套接字列表。
         self.thread_now:当前正在运行的线程列表，用于存储正在等待接受数据的线程。
         self.data_event:线程间的事件通信。
-        self.rpi_port:服务器打开的端口与客户端连接的端口，默认为11451
-        self.password:发送请求的密码
-        self.target_name:存储扫描到的设备名
-        self.connect_device:客户端已连接的设备
+        self.rpi_port:服务器打开的端口与客户端连接的端口，默认为11451。
+        self.password:发送请求的密码。
+        self.target_name:存储扫描到的设备名。
+        self.connect_device:客户端已连接的设备。
+        self.send_server_socket:发送的服务器套接字。
         """
         self.return_data = None
-        self.send_data = None
         self.socket_list = []
         self.threading_now = []
         self.data_event = threading.Event()
         self.data_event.clear()
         self.rpi_port = rpi_port
         self.password = password
         self.target_name = []
         self.connect_device = []
+        self.send_server_socket = None
 
-    def server_open(self, device_name: str = None, max_connect: int = 0, ip: str = None):
+    def open(self, device_name: str = None, max_connect: int = 0, ip: str = None):
         """打开_server线程的函数
 
         它使用线程来启动服务器是为了实现非阻塞式的服务器启动。如果直接调用 _server 方法而不使用线程，
         那么在服务器启动过程中，主程序会被阻塞，直到服务器关闭或者达到最大连接数为止。
 
         通过在新的线程中启动服务器，主程序可以继续执行后续的操作，而不必等待服务器启动完成。
         当服务器启动后，它会在后台处理连接请求，而主程序可以继续执行其他任务，
@@ -64,14 +65,15 @@
             server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             host_address = (host_ip, self.rpi_port)
             server_socket.bind(host_address)
             server_socket.listen(5)
             print(f'\033[92m已在{host_ip}打开服务器\033[0m')
         except Exception:
             print('\033[93m无效IP地址\033[0m')
+            return
 
         while True:
             client_socket, client_address = server_socket.accept()
             print(f'\033[92m{client_address}已连接成功\033[0m')
             if max_connect == 0 or len(self.socket_list) < max_connect:
                 client_socket.settimeout(0.1)
                 try:
@@ -106,27 +108,27 @@
         """
         sock_list = []
         for info in self.socket_list:
             ip_address = info[0].getpeername()[0]
             sock_list.append(ip_address)
         return sock_list
 
-    def wait_connect(self):  # 等待连接，如果有连接返回True,阻塞线程
+    def wait(self):  # 等待连接，如果有连接返回True,阻塞线程
         """等待连接的函数
 
         使用无限循环来阻塞线程运行，通常和接收数据的recv_data函数组合使用
 
         :return: 当服务器有套接字连接时，返回True
         """
         while True:
             if len(self.socket_list) != 0:
                 break
         return True
 
-    def recv_data(self):
+    def recv(self):
         """从已连接的多个套接字中异步接收数据的函数
 
         首先调用 wait_connect 方法，该方法会阻塞线程直到有连接建立。
         这是因为在没有连接的情况下，接收数据是没有意义的，所以该方法会一直等待直到至少有一个连接建立。
 
         一旦有连接建立，recv_data 方法会遍历当前连接的套接字列表 self.socket_list，
         为每个套接字创建一个接收数据的线程 recv_threading。如果某个套接字已经有对应的接收数据线程在运行，则不会重复创建。
@@ -135,15 +137,15 @@
         直到有数据被成功接收并存储在 self.return_data 中。
 
          一旦数据事件被设置，表示数据已经接收到，线程将继续执行。recv_data 方法将 self.return_data 中存储的数据返回给调用者，
          并将 self.return_data 设置为 None，以便下一次接收新的数据。
 
         :return:返回接收到的数据
         """
-        if self.wait_connect():
+        if self.wait():
             for i in self.socket_list:
                 if i not in self.threading_now:
                     recv_thread = threading.Thread(target=self._recv_threading, args=(i,), daemon=True)
                     self.threading_now.append(i)
                     recv_thread.start()
             if len(self.threading_now) == 0:
                 try:
@@ -220,23 +222,22 @@
                     if state == 'cjs8e77e':
                         print(f'\033[93mWarning:由于申请密码不正确被拒绝 \033[0m')
                         self.target_name.pop()
                         self.target_name.append(f"{device_name.decode('utf-8')}(密码错误)")
                         sock.close()
                     elif state == 'ng3mxz7g':
                         self.connect_device.append(device_name.decode('utf-8'))
-                        send_thread = threading.Thread(target=self._send_msg_thread, args=(sock,))
-                        send_thread.start()
+                        self.send_server_socket = sock
                     elif state == 'ny6cz4ln':
                         print(f'\033[91mError:已达到服务器的设备连接上限 \033[0m')
             return
         except Exception:
             return None
 
-    def connect_server(self, target_name, subnet_ip: str = None):
+    def connect(self, target_name, subnet_ip: str = None):
         """连接到服务器并尝试与指定设备建立连接的函数。
 
         如果无法构建局域网，请自行修改。
 
         获取本地主机的 IP 地址并构建局域网的子网。
         用线程遍历子网中的所有可能 IP 地址，并尝试连接到每个 IP 地址的指定端口。
         在连接成功时，发送密码给服务器端，并接收服务器返回的设备名称和状态。
@@ -272,44 +273,20 @@
                 check.append(item)
         else:
             if len(self.target_name) == 0:
                 print(f'\033[91mError:无法找到任何设备 \033[0m')
             elif target_name not in self.connect_device:
                 print(f'\033[93mError:没有找到{target_name}设备或密码不正确 \033[0m')
 
-    def _send_msg_thread(self, sock):
-        """与服务器建立连接后发送消息的线程
-
-        进入一个无限循环，不断检查是否有要发送的消息。
-        如果 self.send_data 不为 None，表示有消息需要发送，则将消息编码为 UTF-8 格式并发送给服务器。
-        在发送完成后，将 self.send_data 设置为 None，表示消息已发送。
-        如果在发送消息的过程中出现异常，则输出错误信息，并退出循环，结束线程。
-
-        :param sock: 套接字
-        :return:
-        """
-        while True:
-            if self.send_data is not None:
-                try:
-                    sock.send(self.send_data.encode('utf-8'))
-                except Exception:
-                    print(f'\033[91mError:服务器强制关闭了连接 \033[0m')
-                    break
-                self.send_data = None
-
-    def send_msg(self, msg: str):
+    def send(self, msg: str):
         """向服务器发送消息的函数
 
-        该方法的主要作用是将消息内容存储在 self.send_data 中，然后等待一小段时间以确保消息被发送。
-        如果发送成功，将不会有额外的输出；如果发送失败，则会输出错误信息提示。
-
-        :param msg:
-        :return:
+        :param msg:发送的信息
         """
-        self.send_data = msg
-        time.sleep(0.001)
-        if self.send_data is not None:
+        try:
+            self.send_server_socket.send(msg.encode('utf-8'))
+        except Exception:
             print('\033[91mError:发送失败！请确认是否有连接服务器 \033[0m')
 
 
 if __name__ == "__main__":
     pass
```

