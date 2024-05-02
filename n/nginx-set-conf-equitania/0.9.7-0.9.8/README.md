# Comparing `tmp/nginx-set-conf-equitania-0.9.7.tar.gz` & `tmp/nginx-set-conf-equitania-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nginx-set-conf-equitania-0.9.7.tar", last modified: Thu Feb 15 09:29:46 2024, max compression
+gzip compressed data, was "nginx-set-conf-equitania-0.9.8.tar", last modified: Thu May  2 07:25:28 2024, max compression
```

## Comparing `nginx-set-conf-equitania-0.9.7.tar` & `nginx-set-conf-equitania-0.9.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2024-02-15 09:29:46.621258 nginx-set-conf-equitania-0.9.7/
--rw-r--r--   0 picard     (501) staff       (20)    33892 2021-05-25 14:23:55.000000 nginx-set-conf-equitania-0.9.7/LICENSE.txt
--rw-r--r--   0 picard     (501) staff       (20)     3695 2024-02-15 09:29:46.621003 nginx-set-conf-equitania-0.9.7/PKG-INFO
--rw-r--r--   0 picard     (501) staff       (20)     3160 2024-02-14 16:50:42.000000 nginx-set-conf-equitania-0.9.7/README.md
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2024-02-15 09:29:46.611052 nginx-set-conf-equitania-0.9.7/nginx_set_conf/
--rw-r--r--   0 picard     (501) staff       (20)       38 2024-02-14 16:42:35.000000 nginx-set-conf-equitania-0.9.7/nginx_set_conf/__init__.py
--rw-r--r--   0 picard     (501) staff       (20)    23176 2024-02-15 09:21:31.000000 nginx-set-conf-equitania-0.9.7/nginx_set_conf/config_templates.py
--rw-r--r--   0 picard     (501) staff       (20)     4343 2024-02-14 16:42:35.000000 nginx-set-conf-equitania-0.9.7/nginx_set_conf/nginx_set_conf.py
--rw-r--r--   0 picard     (501) staff       (20)     8838 2024-02-15 09:26:04.000000 nginx-set-conf-equitania-0.9.7/nginx_set_conf/utils.py
-drwxr-xr-x   0 picard     (501) staff       (20)        0 2024-02-15 09:29:46.620678 nginx-set-conf-equitania-0.9.7/nginx_set_conf_equitania.egg-info/
--rw-r--r--   0 picard     (501) staff       (20)     3695 2024-02-15 09:29:46.000000 nginx-set-conf-equitania-0.9.7/nginx_set_conf_equitania.egg-info/PKG-INFO
--rw-r--r--   0 picard     (501) staff       (20)      439 2024-02-15 09:29:46.000000 nginx-set-conf-equitania-0.9.7/nginx_set_conf_equitania.egg-info/SOURCES.txt
--rw-r--r--   0 picard     (501) staff       (20)        1 2024-02-15 09:29:46.000000 nginx-set-conf-equitania-0.9.7/nginx_set_conf_equitania.egg-info/dependency_links.txt
--rw-r--r--   0 picard     (501) staff       (20)       86 2024-02-15 09:29:46.000000 nginx-set-conf-equitania-0.9.7/nginx_set_conf_equitania.egg-info/entry_points.txt
--rw-r--r--   0 picard     (501) staff       (20)       27 2024-02-15 09:29:46.000000 nginx-set-conf-equitania-0.9.7/nginx_set_conf_equitania.egg-info/requires.txt
--rw-r--r--   0 picard     (501) staff       (20)       15 2024-02-15 09:29:46.000000 nginx-set-conf-equitania-0.9.7/nginx_set_conf_equitania.egg-info/top_level.txt
--rw-r--r--   0 picard     (501) staff       (20)       38 2024-02-15 09:29:46.621313 nginx-set-conf-equitania-0.9.7/setup.cfg
--rw-r--r--   0 picard     (501) staff       (20)      860 2024-02-15 09:26:47.000000 nginx-set-conf-equitania-0.9.7/setup.py
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2024-05-02 07:25:28.955955 nginx-set-conf-equitania-0.9.8/
+-rw-r--r--   0 picard     (501) staff       (20)    33892 2021-05-25 14:23:55.000000 nginx-set-conf-equitania-0.9.8/LICENSE.txt
+-rw-r--r--   0 picard     (501) staff       (20)     3695 2024-05-02 07:25:28.955700 nginx-set-conf-equitania-0.9.8/PKG-INFO
+-rw-r--r--   0 picard     (501) staff       (20)     3160 2024-02-14 16:50:42.000000 nginx-set-conf-equitania-0.9.8/README.md
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2024-05-02 07:25:28.953598 nginx-set-conf-equitania-0.9.8/nginx_set_conf/
+-rw-r--r--   0 picard     (501) staff       (20)       38 2024-02-14 16:42:35.000000 nginx-set-conf-equitania-0.9.8/nginx_set_conf/__init__.py
+-rw-r--r--   0 picard     (501) staff       (20)    23095 2024-05-02 07:23:36.000000 nginx-set-conf-equitania-0.9.8/nginx_set_conf/config_templates.py
+-rw-r--r--   0 picard     (501) staff       (20)     4343 2024-02-14 16:42:35.000000 nginx-set-conf-equitania-0.9.8/nginx_set_conf/nginx_set_conf.py
+-rw-r--r--   0 picard     (501) staff       (20)     8838 2024-02-15 09:26:04.000000 nginx-set-conf-equitania-0.9.8/nginx_set_conf/utils.py
+drwxr-xr-x   0 picard     (501) staff       (20)        0 2024-05-02 07:25:28.955383 nginx-set-conf-equitania-0.9.8/nginx_set_conf_equitania.egg-info/
+-rw-r--r--   0 picard     (501) staff       (20)     3695 2024-05-02 07:25:28.000000 nginx-set-conf-equitania-0.9.8/nginx_set_conf_equitania.egg-info/PKG-INFO
+-rw-r--r--   0 picard     (501) staff       (20)      439 2024-05-02 07:25:28.000000 nginx-set-conf-equitania-0.9.8/nginx_set_conf_equitania.egg-info/SOURCES.txt
+-rw-r--r--   0 picard     (501) staff       (20)        1 2024-05-02 07:25:28.000000 nginx-set-conf-equitania-0.9.8/nginx_set_conf_equitania.egg-info/dependency_links.txt
+-rw-r--r--   0 picard     (501) staff       (20)       86 2024-05-02 07:25:28.000000 nginx-set-conf-equitania-0.9.8/nginx_set_conf_equitania.egg-info/entry_points.txt
+-rw-r--r--   0 picard     (501) staff       (20)       27 2024-05-02 07:25:28.000000 nginx-set-conf-equitania-0.9.8/nginx_set_conf_equitania.egg-info/requires.txt
+-rw-r--r--   0 picard     (501) staff       (20)       15 2024-05-02 07:25:28.000000 nginx-set-conf-equitania-0.9.8/nginx_set_conf_equitania.egg-info/top_level.txt
+-rw-r--r--   0 picard     (501) staff       (20)       38 2024-05-02 07:25:28.956007 nginx-set-conf-equitania-0.9.8/setup.cfg
+-rw-r--r--   0 picard     (501) staff       (20)      860 2024-05-02 07:24:07.000000 nginx-set-conf-equitania-0.9.8/setup.py
```

### Comparing `nginx-set-conf-equitania-0.9.7/LICENSE.txt` & `nginx-set-conf-equitania-0.9.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.9.7/PKG-INFO` & `nginx-set-conf-equitania-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nginx-set-conf-equitania
-Version: 0.9.7
+Version: 0.9.8
 Summary: A package to create configurations for nginx for different web applications
 Author: Equitania Software GmbH
 Author-email: info@equitania.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `nginx-set-conf-equitania-0.9.7/README.md` & `nginx-set-conf-equitania-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.9.7/nginx_set_conf/config_templates.py` & `nginx-set-conf-equitania-0.9.8/nginx_set_conf/config_templates.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 config_template_dict = {
     "ngx_code_server": """# Template for code-server configuration nginx incl. SSL/http2
-# Version 4.1 from 15.02.2024
+# 02.05.2024
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ https://$host$request_uri? permanent;
 }
 
 server {
-    listen server.domain.de:443 ssl http2;
+    listen server.domain.de:443 ssl;
+    http2 on;
     server_name server.domain.de;
 
     add_header Strict-Transport-Security "max-age=15552000; includeSubDomains" always;
 
     access_log /var/log/nginx/server.domain.de-access.log combined buffer=512k flush=1m;
     error_log /var/log/nginx/server.domain.de-error.log warn;
 
@@ -73,27 +74,28 @@
         # Connect to local port
         #authentication
         proxy_pass http://127.0.0.1:oldport;
     }
 }
 """,
     "ngx_fast_report": """# Template for FastReport configuration nginx incl. SSL/http2
-# Version 4.1 from 15.02.2024
+# 02.05.2024
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ https://$host$request_uri? permanent;
 }
 
 server {
-    listen server.domain.de:443 ssl http2;
+    listen server.domain.de:443 ssl;
+    http2 on;
     server_name server.domain.de;
 
     add_header Strict-Transport-Security "max-age=15552000; includeSubDomains" always;
 
     access_log /var/log/nginx/server.domain.de-access.log combined buffer=512k flush=1m;
     error_log /var/log/nginx/server.domain.de-error.log warn;
 
@@ -150,27 +152,28 @@
         # Connect to local port
         #authentication
         proxy_pass http://127.0.0.1:oldport;
     }
 }
 """,
     "ngx_nextcloud": """# Template for NextCloud configuration nginx incl. SSL/http2
-# Version 4.1 from 15.02.2024
+# 02.05.2024
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ https://$host$request_uri? permanent;
 }
 
 server {
-    listen server.domain.de:443 ssl http2;
+    listen server.domain.de:443 ssl;
+    http2 on;
     server_name server.domain.de;
 
     add_header Strict-Transport-Security "max-age=15552000; includeSubDomains" always;
     add_header Referrer-Policy no-referrer always;
 
     access_log /var/log/nginx/server.domain.de-access.log combined buffer=512k flush=1m;
     error_log /var/log/nginx/server.domain.de-error.log;
@@ -239,27 +242,28 @@
         proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
         proxy_set_header X-Forwarded-Proto $scheme;        # Connect to local port
         proxy_pass http://127.0.0.1:oldport;
     }
 }
 """,
     "ngx_portainer": """# Template for Portainer configuration nginx incl. SSL/http2
-# Version 4.1 from 15.02.2024
+# 02.05.2024
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ https://$host$request_uri? permanent;
 }
 
 server {
-    listen server.domain.de:443 ssl http2;
+    listen server.domain.de:443 ssl;
+    http2 on;
     server_name server.domain.de;
 
     add_header Strict-Transport-Security "max-age=15552000; includeSubDomains" always;
     add_header Referrer-Policy no-referrer always;
 
     access_log /var/log/nginx/server.domain.de-access.log combined buffer=512k flush=1m;
     error_log /var/log/nginx/server.domain.de-error.log;
@@ -381,27 +385,28 @@
         proxy_buffering    on;
         expires 864000;
         proxy_pass http://127.0.0.1:oldport;
     }
 }
 """,
     "ngx_odoo_ssl": """# Template for Odoo configuration nginx incl. SSL
-# Version 4.1 from 15.02.2024
+# 02.05.2024
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ https://$host$request_uri? permanent;
 }
 
 server {
-    listen server.domain.de:443 ssl http2;
+    listen server.domain.de:443 ssl;
+    http2 on;
     server_name server.domain.de;
     client_max_body_size 8192m;
     access_log /var/log/nginx/server.domain.de-access.log combined buffer=512k flush=1m;
     error_log /var/log/nginx/server.domain.de-error.log;
 
     # ssl certificate files
     ssl_certificate /etc/letsencrypt/live/zertifikat.crt/fullchain.pem;
@@ -469,27 +474,28 @@
         proxy_buffering    on;
         expires 864000;
         proxy_pass http://127.0.0.1:oldport;
     }
 }
 """,
     "ngx_pgadmin": """# Template for pgAdmin configuration nginx incl. SSL/http2
-# Version 4.1 from 15.02.2024
+# 02.05.2024
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ https://$host$request_uri? permanent;
 }
 
 server {
-    listen server.domain.de:443 ssl http2;
+    listen server.domain.de:443 ssl;
+    http2 on;
     server_name server.domain.de;
 
     add_header Strict-Transport-Security "max-age=15552000; includeSubDomains" always;
 
     access_log /var/log/nginx/server.domain.de-access.log combined buffer=512k flush=1m;
     error_log /var/log/nginx/server.domain.de-error.log;
 
@@ -538,27 +544,28 @@
         proxy_set_header X-Forwarded-For $proxy_add_x_forwarded_for;
         proxy_set_header X-Forwarded-Proto https;
         proxy_pass http://127.0.0.1:oldport;
     }
 }
 """,
     "ngx_pwa": """# Template for Progressive Web App .NET Core configuration nginx incl. SSL/http2
-# Version 4.1 from 15.02.2024
+# 02.05.2024
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ https://$host$request_uri? permanent;
 }
 
 server {
-    listen server.domain.de:443 ssl http2;
+    listen server.domain.de:443 ssl;
+    http2 on;
     server_name server.domain.de;
 
     add_header Strict-Transport-Security "max-age=15552000; includeSubDomains" always;
 
     access_log /var/log/nginx/server.domain.de-access.log combined buffer=512k flush=1m;
     error_log /var/log/nginx/server.domain.de-error.log;
 
@@ -611,27 +618,28 @@
         # Connect to local port
         #authentication
         proxy_pass http://127.0.0.1:oldport;
     }
 }
 """,
     "ngx_mailhog": """# Template for mailhog https://github.com/mailhog/MailHog/tree/master configuration nginx incl. SSL/http2
-# Version 1.0 from 15.02.2024
+# 02.05.2024
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
     rewrite ^/.*$ https://$host$request_uri? permanent;
 }
 
 server {
-    listen server.domain.de:443 ssl http2;
+    listen server.domain.de:443 ssl;
+    http2 on;
     server_name server.domain.de;
 
     add_header Strict-Transport-Security "max-age=15552000; includeSubDomains" always;
 
     access_log /var/log/nginx/server.domain.de-access.log combined buffer=512k flush=1m;
     error_log /var/log/nginx/server.domain.de-error.log;
 
@@ -698,15 +706,15 @@
     server_name server.domain.de;
     rewrite ^/.*$ http://target.domain.de$request_uri? permanent;
     access_log /var/log/nginx/target.domain.de-access.log combined buffer=512k flush=1m;
     error_log /var/log/nginx/target.domain.de-error.log;
 }
 """,
     "ngx_redirect_ssl": """# Template for Redirect domain configuration nginx ssl/http2
-# Version 4.0 from 10.07.2023
+# 02.05.2024
 # upstream server.domain.de {
 #     server ip.ip.ip.ip weight=1 fail_timeout=0;
 # }
 
 server {
     listen server.domain.de:80;
     server_name server.domain.de;
@@ -715,15 +723,16 @@
     error_log /var/log/nginx/target.domain.de-error.log;
 
     # additional config
     include                 nginxconfig.io/general.conf;
 }
 
 server {
-    listen server.domain.de:443 ssl http2;
+    listen server.domain.de:443 ssl;
+    http2 on;
     server_name server.domain.de;
     rewrite ^/.*$ https://target.domain.de$request_uri? permanent;
     access_log /var/log/nginx/target.domain.de-access.log;
     error_log /var/log/nginx/target.domain.de-error.log;
 
     # ssl certificate files
     ssl_certificate /etc/letsencrypt/live/zertifikat.crt/fullchain.pem;
```

### Comparing `nginx-set-conf-equitania-0.9.7/nginx_set_conf/nginx_set_conf.py` & `nginx-set-conf-equitania-0.9.8/nginx_set_conf/nginx_set_conf.py`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.9.7/nginx_set_conf/utils.py` & `nginx-set-conf-equitania-0.9.8/nginx_set_conf/utils.py`

 * *Files identical despite different names*

### Comparing `nginx-set-conf-equitania-0.9.7/nginx_set_conf_equitania.egg-info/PKG-INFO` & `nginx-set-conf-equitania-0.9.8/nginx_set_conf_equitania.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nginx-set-conf-equitania
-Version: 0.9.7
+Version: 0.9.8
 Summary: A package to create configurations for nginx for different web applications
 Author: Equitania Software GmbH
 Author-email: info@equitania.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `nginx-set-conf-equitania-0.9.7/setup.py` & `nginx-set-conf-equitania-0.9.8/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="nginx-set-conf-equitania",
-    version="0.9.7",
+    version="0.9.8",
     author="Equitania Software GmbH",
     author_email="info@equitania.de",
     description="A package to create configurations for nginx for different web applications",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["nginx_set_conf"],
     classifiers=[
```

