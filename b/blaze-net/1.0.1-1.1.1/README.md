# Comparing `tmp/blaze-net-1.0.1.tar.gz` & `tmp/blaze-net-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blaze-net-1.0.1.tar", last modified: Tue Apr 30 17:21:45 2024, max compression
+gzip compressed data, was "blaze-net-1.1.1.tar", last modified: Wed May  1 23:25:50 2024, max compression
```

## Comparing `blaze-net-1.0.1.tar` & `blaze-net-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 17:21:45.027671 blaze-net-1.0.1/
--rw-rw-rw-   0        0        0     1924 2024-04-30 17:21:45.027671 blaze-net-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1176 2024-04-30 17:20:52.000000 blaze-net-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 17:21:45.012043 blaze-net-1.0.1/blaze_net/
--rw-rw-rw-   0        0        0       25 2024-04-30 14:00:22.000000 blaze-net-1.0.1/blaze_net/__init__.py
--rw-rw-rw-   0        0        0     2177 2024-04-30 17:16:10.000000 blaze-net-1.0.1/blaze_net/app.py
--rw-rw-rw-   0        0        0      134 2024-04-30 17:10:24.000000 blaze-net-1.0.1/blaze_net/routes.py
-drwxrwxrwx   0        0        0        0 2024-04-30 17:21:45.027671 blaze-net-1.0.1/blaze_net.egg-info/
--rw-rw-rw-   0        0        0     1924 2024-04-30 17:21:44.000000 blaze-net-1.0.1/blaze_net.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2024-04-30 17:21:44.000000 blaze-net-1.0.1/blaze_net.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 17:21:44.000000 blaze-net-1.0.1/blaze_net.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       27 2024-04-30 17:21:44.000000 blaze-net-1.0.1/blaze_net.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-04-30 17:21:44.000000 blaze-net-1.0.1/blaze_net.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 17:21:45.027671 blaze-net-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      944 2024-04-30 17:17:55.000000 blaze-net-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 17:21:45.027671 blaze-net-1.0.1/tests/
--rw-rw-rw-   0        0        0       31 2024-04-30 13:59:48.000000 blaze-net-1.0.1/tests/__init__.py
--rw-rw-rw-   0        0        0      325 2024-04-30 13:33:33.000000 blaze-net-1.0.1/tests/test_app.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:25:50.212153 blaze-net-1.1.1/
+-rw-rw-rw-   0        0        0     3737 2024-05-01 23:25:50.212153 blaze-net-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2989 2024-05-01 23:17:42.000000 blaze-net-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 23:25:50.196816 blaze-net-1.1.1/blaze_net/
+-rw-rw-rw-   0        0        0       25 2024-04-30 14:00:22.000000 blaze-net-1.1.1/blaze_net/__init__.py
+-rw-rw-rw-   0        0        0     3447 2024-05-01 23:15:29.000000 blaze-net-1.1.1/blaze_net/app.py
+-rw-rw-rw-   0        0        0      951 2024-05-01 22:43:58.000000 blaze-net-1.1.1/blaze_net/model_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:25:50.212153 blaze-net-1.1.1/blaze_net.egg-info/
+-rw-rw-rw-   0        0        0     3737 2024-05-01 23:25:49.000000 blaze-net-1.1.1/blaze_net.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2024-05-01 23:25:49.000000 blaze-net-1.1.1/blaze_net.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 23:25:49.000000 blaze-net-1.1.1/blaze_net.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       27 2024-05-01 23:25:49.000000 blaze-net-1.1.1/blaze_net.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-01 23:25:49.000000 blaze-net-1.1.1/blaze_net.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 23:25:50.212153 blaze-net-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      944 2024-05-01 23:21:36.000000 blaze-net-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 23:25:50.212153 blaze-net-1.1.1/tests/
+-rw-rw-rw-   0        0        0       31 2024-04-30 13:59:48.000000 blaze-net-1.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      325 2024-04-30 13:33:33.000000 blaze-net-1.1.1/tests/test_app.py
```

### Comparing `blaze-net-1.0.1/blaze_net/app.py` & `blaze-net-1.1.1/blaze_net/app.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,56 +1,84 @@
-from werkzeug.exceptions import HTTPException
+import os
+from werkzeug.exceptions import HTTPException, NotFound
 from werkzeug.wrappers import Request, Response
 from werkzeug.routing import Map, Rule
 from jinja2 import Environment, FileSystemLoader
 from sqlalchemy import create_engine
 from sqlalchemy.orm import sessionmaker
 from werkzeug.serving import run_simple
+import json
 
 class BlazeNet:
-    def __init__(self, template_path='blaze_net/templates/'):
+    def __init__(self, template_path='blaze_net/templates/', static_path='static', database_url='sqlite:///blazenet.db'):
         self.url_map = Map()
         self.template_env = Environment(loader=FileSystemLoader(template_path))
-        self.engine = create_engine('sqlite:///:memory:', echo=True)
+        self.engine = create_engine(database_url, echo=True)
         self.Session = sessionmaker(bind=self.engine)
+        self.static_path = static_path
 
     def route(self, rule):
         def decorator(f):
             def wrapper(*args, **kwargs):
                 return f(*args, **kwargs)
             rule_obj = Rule(rule, endpoint=f)
             self.url_map.add(rule_obj)
             return wrapper
         return decorator
 
     def __call__(self, environ, start_response):
         request = Request(environ)
-        response = self.dispatch_request(request)
-        
-        # Check if response is a string
-        if isinstance(response, str):
-            # If response is a string, create a Response object
-            response = Response(response, content_type='text/html')
+        if request.path.startswith('/static/'):
+            return self.serve_static(environ, start_response)
+        else:
+            response = self.dispatch_request(request)
+            if isinstance(response, str):
+                response = Response(response, content_type='text/html')
+            return response(environ, start_response)
         
-        return response(environ, start_response)
+    def json_response(self, data, status_code=200):
+        json_data = json.dumps(data)
+        return Response(json_data, status=status_code, content_type='application/json')
+
+    def serve_static(self, environ, start_response):
+        path = environ['PATH_INFO']
+        if path.startswith('/static/'):
+            full_path = os.path.join(self.static_path, path.lstrip('/static/'))
+            if os.path.exists(full_path) and os.path.isfile(full_path):
+                with open(full_path, 'rb') as f:
+                    content = f.read()
+                mime_type = self.get_mimetype(full_path)
+                response = Response(content, mimetype=mime_type)
+                return response(environ, start_response)
+        raise NotFound()
+
+    def get_mimetype(self, path):
+        mime_types = {
+            '.css': 'text/css',
+            '.js': 'application/javascript',
+            '.png': 'image/png',
+            '.jpg': 'image/jpeg',
+            '.jpeg': 'image/jpeg',
+            '.gif': 'image/gif',
+            '.svg': 'image/svg+xml'
+        }
+        _, ext = os.path.splitext(path)
+        return mime_types.get(ext.lower(), 'application/octet-stream')
 
     def dispatch_request(self, request):
         adapter = self.url_map.bind_to_environ(request.environ)
         try:
             endpoint, values = adapter.match()
             return endpoint(request, **values)
         except HTTPException as e:
             # Handle HTTP exceptions
             return e
-    
+
     def wsgi_app(self, environ, start_response):
         request = Request(environ)
         response = self.dispatch_request(request)
         if isinstance(response, str):
-            # If response is a string, create a Response object
             response = Response(response, content_type='text/html')
         return response(environ, start_response)
 
     def run(self, host='localhost', port=5000, use_reloader=False):
         run_simple(host, port, self.wsgi_app, use_reloader=use_reloader)
-
-app = BlazeNet()
```

### Comparing `blaze-net-1.0.1/setup.py` & `blaze-net-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='blaze-net',
-    version='1.0.1',
+    version='1.1.1',
     author='McLovinAlan69',
     author_email='gameg1676@gmail.com',
     description='A Python web framework',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/Alan69/blaze_net',
     packages=find_packages(),
```

