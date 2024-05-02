# Comparing `tmp/biftest-0.0.9.tar.gz` & `tmp/biftest-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "biftest-0.0.9.tar", last modified: Thu Apr 25 06:29:04 2024, max compression
+gzip compressed data, was "biftest-0.1.0.tar", last modified: Thu May  2 08:06:59 2024, max compression
```

## Comparing `biftest-0.0.9.tar` & `biftest-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
-drwxr-xr-x   0 youngjin   (501) staff       (20)        0 2024-04-25 06:29:04.739680 biftest-0.0.9/
--rw-r--r--   0 youngjin   (501) staff       (20)      132 2024-04-25 06:29:04.739575 biftest-0.0.9/PKG-INFO
-drwxr-xr-x   0 youngjin   (501) staff       (20)        0 2024-04-25 06:29:04.738733 biftest-0.0.9/biftest/
--rw-r--r--   0 youngjin   (501) staff       (20)        0 2024-04-05 00:39:13.000000 biftest-0.0.9/biftest/__init__.py
--rw-r--r--   0 youngjin   (501) staff       (20)     2215 2024-04-25 06:23:57.000000 biftest-0.0.9/biftest/data_manager.py
--rw-r--r--   0 youngjin   (501) staff       (20)      747 2024-04-15 11:54:36.000000 biftest-0.0.9/biftest/hel.py
--rw-r--r--   0 youngjin   (501) staff       (20)     2315 2024-04-25 05:48:51.000000 biftest-0.0.9/biftest/request.py
-drwxr-xr-x   0 youngjin   (501) staff       (20)        0 2024-04-25 06:29:04.739424 biftest-0.0.9/biftest.egg-info/
--rw-r--r--   0 youngjin   (501) staff       (20)      132 2024-04-25 06:29:04.000000 biftest-0.0.9/biftest.egg-info/PKG-INFO
--rw-r--r--   0 youngjin   (501) staff       (20)      240 2024-04-25 06:29:04.000000 biftest-0.0.9/biftest.egg-info/SOURCES.txt
--rw-r--r--   0 youngjin   (501) staff       (20)        1 2024-04-25 06:29:04.000000 biftest-0.0.9/biftest.egg-info/dependency_links.txt
--rw-r--r--   0 youngjin   (501) staff       (20)       51 2024-04-25 06:29:04.000000 biftest-0.0.9/biftest.egg-info/requires.txt
--rw-r--r--   0 youngjin   (501) staff       (20)        8 2024-04-25 06:29:04.000000 biftest-0.0.9/biftest.egg-info/top_level.txt
--rw-r--r--   0 youngjin   (501) staff       (20)       38 2024-04-25 06:29:04.739745 biftest-0.0.9/setup.cfg
--rw-r--r--   0 youngjin   (501) staff       (20)      235 2024-04-25 06:29:02.000000 biftest-0.0.9/setup.py
+drwxr-xr-x   0 youngjin   (501) staff       (20)        0 2024-05-02 08:06:59.583870 biftest-0.1.0/
+-rw-r--r--   0 youngjin   (501) staff       (20)      132 2024-05-02 08:06:59.583250 biftest-0.1.0/PKG-INFO
+drwxr-xr-x   0 youngjin   (501) staff       (20)        0 2024-05-02 08:06:59.582320 biftest-0.1.0/biftest/
+-rw-r--r--   0 youngjin   (501) staff       (20)        0 2024-04-05 00:39:13.000000 biftest-0.1.0/biftest/__init__.py
+-rw-r--r--   0 youngjin   (501) staff       (20)     2206 2024-05-02 08:05:15.000000 biftest-0.1.0/biftest/dashboard_manager.py
+-rw-r--r--   0 youngjin   (501) staff       (20)     4538 2024-05-02 07:55:57.000000 biftest-0.1.0/biftest/data_manager.py
+-rw-r--r--   0 youngjin   (501) staff       (20)      747 2024-04-15 11:54:36.000000 biftest-0.1.0/biftest/hel.py
+-rw-r--r--   0 youngjin   (501) staff       (20)     2332 2024-05-02 08:04:13.000000 biftest-0.1.0/biftest/request.py
+-rw-r--r--   0 youngjin   (501) staff       (20)     1931 2024-05-02 08:02:17.000000 biftest-0.1.0/biftest/system_manager.py
+drwxr-xr-x   0 youngjin   (501) staff       (20)        0 2024-05-02 08:06:59.583055 biftest-0.1.0/biftest.egg-info/
+-rw-r--r--   0 youngjin   (501) staff       (20)      132 2024-05-02 08:06:59.000000 biftest-0.1.0/biftest.egg-info/PKG-INFO
+-rw-r--r--   0 youngjin   (501) staff       (20)      295 2024-05-02 08:06:59.000000 biftest-0.1.0/biftest.egg-info/SOURCES.txt
+-rw-r--r--   0 youngjin   (501) staff       (20)        1 2024-05-02 08:06:59.000000 biftest-0.1.0/biftest.egg-info/dependency_links.txt
+-rw-r--r--   0 youngjin   (501) staff       (20)       51 2024-05-02 08:06:59.000000 biftest-0.1.0/biftest.egg-info/requires.txt
+-rw-r--r--   0 youngjin   (501) staff       (20)        8 2024-05-02 08:06:59.000000 biftest-0.1.0/biftest.egg-info/top_level.txt
+-rw-r--r--   0 youngjin   (501) staff       (20)       38 2024-05-02 08:06:59.583936 biftest-0.1.0/setup.cfg
+-rw-r--r--   0 youngjin   (501) staff       (20)      235 2024-05-02 08:06:18.000000 biftest-0.1.0/setup.py
```

### Comparing `biftest-0.0.9/biftest/data_manager.py` & `biftest-0.1.0/biftest/dashboard_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     def __init__(self, url, token):
         super().__init__(url, token)
 
     def get_list(self, params):
         endpoint = self.url + 'dashboards'
         return self._get_request(endpoint, params)
         
-    def create(self, inputId, data):
+    def create(self, data):
         endpoint = self.url + 'dashboards'
         return self._post_request(endpoint, data)
     
     def clone(self, inputId, data):
         endpoint = self.url + 'dashboards/' + inputId + '/clone'
         return self._post_request(endpoint, data)
```

### Comparing `biftest-0.0.9/biftest/hel.py` & `biftest-0.1.0/biftest/hel.py`

 * *Files identical despite different names*

### Comparing `biftest-0.0.9/biftest/request.py` & `biftest-0.1.0/biftest/request.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         
     def _post_request(self, endpoint, data=None):
         headers = {
             'Content-Type': 'application/json',
             'Authorization': 'Bearer ' + self.token
         }
         try:
-            response = requests.post(endpoint, json=data, timeout=10) # 10초 타임아웃 설정
+            response = requests.post(endpoint, headers=headers ,json=data, timeout=10) # 10초 타임아웃 설정
             response.raise_for_status()  # HTTPError 예외 발생 시키기
             return response.json()
         except requests.exceptions.HTTPError as e:
             print(f"HTTP 에러 발생: {e.response.status_code} - {e.response.text}")
         except requests.exceptions.ConnectionError:
             print("서버에 연결할 수 없습니다.")
         except requests.exceptions.Timeout:
```

