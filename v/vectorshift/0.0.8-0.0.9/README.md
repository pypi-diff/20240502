# Comparing `tmp/vectorshift-0.0.8.tar.gz` & `tmp/vectorshift-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectorshift-0.0.8.tar", last modified: Sun Apr  2 08:31:55 2023, max compression
+gzip compressed data, was "vectorshift-0.0.9.tar", last modified: Tue Apr  4 02:53:55 2023, max compression
```

## Comparing `vectorshift-0.0.8.tar` & `vectorshift-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-04-02 08:31:55.939478 vectorshift-0.0.8/
--rw-rw-rw-   0        0        0      499 2023-04-02 08:31:55.938978 vectorshift-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-04-02 08:31:55.939979 vectorshift-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      724 2023-04-02 08:31:49.000000 vectorshift-0.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-02 08:31:55.933977 vectorshift-0.0.8/vectorshift/
--rw-rw-rw-   0        0        0       31 2023-04-02 08:31:43.000000 vectorshift-0.0.8/vectorshift/__init__.py
--rw-rw-rw-   0        0        0     4367 2023-04-02 06:52:50.000000 vectorshift-0.0.8/vectorshift/main.py
-drwxrwxrwx   0        0        0        0 2023-04-02 08:31:55.937979 vectorshift-0.0.8/vectorshift.egg-info/
--rw-rw-rw-   0        0        0      499 2023-04-02 08:31:55.000000 vectorshift-0.0.8/vectorshift.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2023-04-02 08:31:55.000000 vectorshift-0.0.8/vectorshift.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-02 08:31:55.000000 vectorshift-0.0.8/vectorshift.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-04-02 08:31:55.000000 vectorshift-0.0.8/vectorshift.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-04 02:53:55.750166 vectorshift-0.0.9/
+-rw-rw-rw-   0        0        0      499 2023-04-04 02:53:55.749166 vectorshift-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-04-04 02:53:55.750666 vectorshift-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      724 2023-04-04 02:53:28.000000 vectorshift-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-04 02:53:55.743166 vectorshift-0.0.9/vectorshift/
+-rw-rw-rw-   0        0        0       31 2023-04-02 08:31:43.000000 vectorshift-0.0.9/vectorshift/__init__.py
+-rw-rw-rw-   0        0        0     4417 2023-04-04 02:53:20.000000 vectorshift-0.0.9/vectorshift/main.py
+drwxrwxrwx   0        0        0        0 2023-04-04 02:53:55.748165 vectorshift-0.0.9/vectorshift.egg-info/
+-rw-rw-rw-   0        0        0      499 2023-04-04 02:53:55.000000 vectorshift-0.0.9/vectorshift.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2023-04-04 02:53:55.000000 vectorshift-0.0.9/vectorshift.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-04 02:53:55.000000 vectorshift-0.0.9/vectorshift.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-04-04 02:53:55.000000 vectorshift-0.0.9/vectorshift.egg-info/top_level.txt
```

### Comparing `vectorshift-0.0.8/setup.py` & `vectorshift-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'A connector to VectorShift'
 
 # Setting up
 setup(
     name="vectorshift",
     version=VERSION,
     author="AlexLeonardi",
```

### Comparing `vectorshift-0.0.8/vectorshift/main.py` & `vectorshift-0.0.9/vectorshift/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,13 +83,14 @@
         query_params = f'''?{'&'.join([f'{k}={v}' for k, v in query_dict.items() if v != ''])}'''
         response = requests.get(f'https://api.vector-shift.com/api/sources/info{query_params}',
                             data={'api_key': self.api_key}).text
         return json.loads(response)
 
     def get_transformation_info(self,
                                 id: str = '',
-                                name: str = ''):
+                                name: str = '',
+                                scope='user'):
         query_dict = {'id': id, 'name': name}
         query_params = f'''?{'&'.join([f'{k}={v}' for k, v in query_dict.items() if v != ''])}'''
-        response = requests.get(f'https://api.vector-shift.com/api/transformations/user/info{query_params}',
+        response = requests.get(f'https://api.vector-shift.com/api/transformations/{scope}/info{query_params}',
                             data={'api_key': self.api_key}).text
         return json.loads(response)
```

