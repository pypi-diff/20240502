# Comparing `tmp/cloudflare-dynamic-dns-client-0.2.0.tar.gz` & `tmp/cloudflare-dynamic-dns-client-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudflare-dynamic-dns-client-0.2.0.tar", last modified: Wed May  1 22:01:40 2024, max compression
+gzip compressed data, was "cloudflare-dynamic-dns-client-0.2.1.tar", last modified: Wed May  1 22:03:48 2024, max compression
```

## Comparing `cloudflare-dynamic-dns-client-0.2.0.tar` & `cloudflare-dynamic-dns-client-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 22:01:40.779195 cloudflare-dynamic-dns-client-0.2.0/
--rw-rw-rw-   0        0        0     1066 2024-05-01 21:41:51.000000 cloudflare-dynamic-dns-client-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     1905 2024-05-01 22:01:40.778196 cloudflare-dynamic-dns-client-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1600 2024-05-01 21:58:36.000000 cloudflare-dynamic-dns-client-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 22:01:40.761664 cloudflare-dynamic-dns-client-0.2.0/cloudflare_dynamic_dns/
--rw-rw-rw-   0        0        0       39 2024-05-01 21:59:54.000000 cloudflare-dynamic-dns-client-0.2.0/cloudflare_dynamic_dns/__init__.py
--rw-rw-rw-   0        0        0     4154 2024-05-01 21:53:39.000000 cloudflare-dynamic-dns-client-0.2.0/cloudflare_dynamic_dns/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 22:01:40.777191 cloudflare-dynamic-dns-client-0.2.0/cloudflare_dynamic_dns_client.egg-info/
--rw-rw-rw-   0        0        0     1905 2024-05-01 22:01:40.000000 cloudflare-dynamic-dns-client-0.2.0/cloudflare_dynamic_dns_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2024-05-01 22:01:40.000000 cloudflare-dynamic-dns-client-0.2.0/cloudflare_dynamic_dns_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 22:01:40.000000 cloudflare-dynamic-dns-client-0.2.0/cloudflare_dynamic_dns_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-05-01 22:01:40.000000 cloudflare-dynamic-dns-client-0.2.0/cloudflare_dynamic_dns_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2024-05-01 22:01:40.000000 cloudflare-dynamic-dns-client-0.2.0/cloudflare_dynamic_dns_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-01 22:01:40.000000 cloudflare-dynamic-dns-client-0.2.0/cloudflare_dynamic_dns_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 22:01:40.779195 cloudflare-dynamic-dns-client-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      506 2024-05-01 22:01:27.000000 cloudflare-dynamic-dns-client-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:03:48.487664 cloudflare-dynamic-dns-client-0.2.1/
+-rw-rw-rw-   0        0        0     1066 2024-05-01 21:41:51.000000 cloudflare-dynamic-dns-client-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     1946 2024-05-01 22:03:48.486665 cloudflare-dynamic-dns-client-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1600 2024-05-01 21:58:36.000000 cloudflare-dynamic-dns-client-0.2.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 22:03:48.470623 cloudflare-dynamic-dns-client-0.2.1/cloudflare_dynamic_dns/
+-rw-rw-rw-   0        0        0       39 2024-05-01 21:59:54.000000 cloudflare-dynamic-dns-client-0.2.1/cloudflare_dynamic_dns/__init__.py
+-rw-rw-rw-   0        0        0     4154 2024-05-01 21:53:39.000000 cloudflare-dynamic-dns-client-0.2.1/cloudflare_dynamic_dns/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:03:48.485669 cloudflare-dynamic-dns-client-0.2.1/cloudflare_dynamic_dns_client.egg-info/
+-rw-rw-rw-   0        0        0     1946 2024-05-01 22:03:48.000000 cloudflare-dynamic-dns-client-0.2.1/cloudflare_dynamic_dns_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2024-05-01 22:03:48.000000 cloudflare-dynamic-dns-client-0.2.1/cloudflare_dynamic_dns_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 22:03:48.000000 cloudflare-dynamic-dns-client-0.2.1/cloudflare_dynamic_dns_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-01 22:03:48.000000 cloudflare-dynamic-dns-client-0.2.1/cloudflare_dynamic_dns_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2024-05-01 22:03:48.000000 cloudflare-dynamic-dns-client-0.2.1/cloudflare_dynamic_dns_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-01 22:03:48.000000 cloudflare-dynamic-dns-client-0.2.1/cloudflare_dynamic_dns_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 22:03:48.487664 cloudflare-dynamic-dns-client-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      554 2024-05-01 22:03:31.000000 cloudflare-dynamic-dns-client-0.2.1/setup.py
```

### Comparing `cloudflare-dynamic-dns-client-0.2.0/LICENSE` & `cloudflare-dynamic-dns-client-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudflare-dynamic-dns-client-0.2.0/PKG-INFO` & `cloudflare-dynamic-dns-client-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: cloudflare-dynamic-dns-client
-Version: 0.2.0
+Version: 0.2.1
 Summary: Allows selfhosting on cloudflare with a dynamic ip address
 Author: Littlewhinging
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cloudflare==2.11.1
 Requires-Dist: requests==2.31.0
 
 # Cloudflare Dynamic DNS
 
 Cloudflare Dynamic DNS is a Python package designed to automate the process of updating Cloudflare A records whenever your server's IP address changes. This can be particularly useful for users with dynamic IP addresses, ensuring that your domain always points to the correct server.
```

### Comparing `cloudflare-dynamic-dns-client-0.2.0/README.md` & `cloudflare-dynamic-dns-client-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `cloudflare-dynamic-dns-client-0.2.0/cloudflare_dynamic_dns/__main__.py` & `cloudflare-dynamic-dns-client-0.2.1/cloudflare_dynamic_dns/__main__.py`

 * *Files identical despite different names*

### Comparing `cloudflare-dynamic-dns-client-0.2.0/cloudflare_dynamic_dns_client.egg-info/PKG-INFO` & `cloudflare-dynamic-dns-client-0.2.1/cloudflare_dynamic_dns_client.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: cloudflare-dynamic-dns-client
-Version: 0.2.0
+Version: 0.2.1
 Summary: Allows selfhosting on cloudflare with a dynamic ip address
 Author: Littlewhinging
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cloudflare==2.11.1
 Requires-Dist: requests==2.31.0
 
 # Cloudflare Dynamic DNS
 
 Cloudflare Dynamic DNS is a Python package designed to automate the process of updating Cloudflare A records whenever your server's IP address changes. This can be particularly useful for users with dynamic IP addresses, ensuring that your domain always points to the correct server.
```

