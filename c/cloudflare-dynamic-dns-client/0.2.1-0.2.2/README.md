# Comparing `tmp/cloudflare-dynamic-dns-client-0.2.1.tar.gz` & `tmp/cloudflare-dynamic-dns-client-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudflare-dynamic-dns-client-0.2.1.tar", last modified: Wed May  1 22:03:48 2024, max compression
+gzip compressed data, was "cloudflare-dynamic-dns-client-0.2.2.tar", last modified: Wed May  1 22:10:40 2024, max compression
```

## Comparing `cloudflare-dynamic-dns-client-0.2.1.tar` & `cloudflare-dynamic-dns-client-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-01 22:03:48.487664 cloudflare-dynamic-dns-client-0.2.1/
--rw-rw-rw-   0        0        0     1066 2024-05-01 21:41:51.000000 cloudflare-dynamic-dns-client-0.2.1/LICENSE
--rw-rw-rw-   0        0        0     1946 2024-05-01 22:03:48.486665 cloudflare-dynamic-dns-client-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1600 2024-05-01 21:58:36.000000 cloudflare-dynamic-dns-client-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-01 22:03:48.470623 cloudflare-dynamic-dns-client-0.2.1/cloudflare_dynamic_dns/
--rw-rw-rw-   0        0        0       39 2024-05-01 21:59:54.000000 cloudflare-dynamic-dns-client-0.2.1/cloudflare_dynamic_dns/__init__.py
--rw-rw-rw-   0        0        0     4154 2024-05-01 21:53:39.000000 cloudflare-dynamic-dns-client-0.2.1/cloudflare_dynamic_dns/__main__.py
-drwxrwxrwx   0        0        0        0 2024-05-01 22:03:48.485669 cloudflare-dynamic-dns-client-0.2.1/cloudflare_dynamic_dns_client.egg-info/
--rw-rw-rw-   0        0        0     1946 2024-05-01 22:03:48.000000 cloudflare-dynamic-dns-client-0.2.1/cloudflare_dynamic_dns_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2024-05-01 22:03:48.000000 cloudflare-dynamic-dns-client-0.2.1/cloudflare_dynamic_dns_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-01 22:03:48.000000 cloudflare-dynamic-dns-client-0.2.1/cloudflare_dynamic_dns_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-05-01 22:03:48.000000 cloudflare-dynamic-dns-client-0.2.1/cloudflare_dynamic_dns_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2024-05-01 22:03:48.000000 cloudflare-dynamic-dns-client-0.2.1/cloudflare_dynamic_dns_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-01 22:03:48.000000 cloudflare-dynamic-dns-client-0.2.1/cloudflare_dynamic_dns_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-01 22:03:48.487664 cloudflare-dynamic-dns-client-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      554 2024-05-01 22:03:31.000000 cloudflare-dynamic-dns-client-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:10:40.429406 cloudflare-dynamic-dns-client-0.2.2/
+-rw-rw-rw-   0        0        0     1066 2024-05-01 21:41:51.000000 cloudflare-dynamic-dns-client-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     2029 2024-05-01 22:10:40.428398 cloudflare-dynamic-dns-client-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1600 2024-05-01 21:58:36.000000 cloudflare-dynamic-dns-client-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-01 22:10:40.412309 cloudflare-dynamic-dns-client-0.2.2/cloudflare_dynamic_dns/
+-rw-rw-rw-   0        0        0       39 2024-05-01 21:59:54.000000 cloudflare-dynamic-dns-client-0.2.2/cloudflare_dynamic_dns/__init__.py
+-rw-rw-rw-   0        0        0     4154 2024-05-01 21:53:39.000000 cloudflare-dynamic-dns-client-0.2.2/cloudflare_dynamic_dns/__main__.py
+drwxrwxrwx   0        0        0        0 2024-05-01 22:10:40.427334 cloudflare-dynamic-dns-client-0.2.2/cloudflare_dynamic_dns_client.egg-info/
+-rw-rw-rw-   0        0        0     2029 2024-05-01 22:10:40.000000 cloudflare-dynamic-dns-client-0.2.2/cloudflare_dynamic_dns_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2024-05-01 22:10:40.000000 cloudflare-dynamic-dns-client-0.2.2/cloudflare_dynamic_dns_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-01 22:10:40.000000 cloudflare-dynamic-dns-client-0.2.2/cloudflare_dynamic_dns_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-05-01 22:10:40.000000 cloudflare-dynamic-dns-client-0.2.2/cloudflare_dynamic_dns_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2024-05-01 22:10:40.000000 cloudflare-dynamic-dns-client-0.2.2/cloudflare_dynamic_dns_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-01 22:10:40.000000 cloudflare-dynamic-dns-client-0.2.2/cloudflare_dynamic_dns_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-01 22:10:40.429406 cloudflare-dynamic-dns-client-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      635 2024-05-01 22:10:37.000000 cloudflare-dynamic-dns-client-0.2.2/setup.py
```

### Comparing `cloudflare-dynamic-dns-client-0.2.1/LICENSE` & `cloudflare-dynamic-dns-client-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudflare-dynamic-dns-client-0.2.1/PKG-INFO` & `cloudflare-dynamic-dns-client-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: cloudflare-dynamic-dns-client
-Version: 0.2.1
+Version: 0.2.2
 Summary: Allows selfhosting on cloudflare with a dynamic ip address
+Home-page: https://github.com/Littlewhinging/cloudflare-dynamic-dns
 Author: Littlewhinging
+License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cloudflare==2.11.1
 Requires-Dist: requests==2.31.0
 
 # Cloudflare Dynamic DNS
```

### Comparing `cloudflare-dynamic-dns-client-0.2.1/README.md` & `cloudflare-dynamic-dns-client-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `cloudflare-dynamic-dns-client-0.2.1/cloudflare_dynamic_dns/__main__.py` & `cloudflare-dynamic-dns-client-0.2.2/cloudflare_dynamic_dns/__main__.py`

 * *Files identical despite different names*

### Comparing `cloudflare-dynamic-dns-client-0.2.1/cloudflare_dynamic_dns_client.egg-info/PKG-INFO` & `cloudflare-dynamic-dns-client-0.2.2/cloudflare_dynamic_dns_client.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 Metadata-Version: 2.1
 Name: cloudflare-dynamic-dns-client
-Version: 0.2.1
+Version: 0.2.2
 Summary: Allows selfhosting on cloudflare with a dynamic ip address
+Home-page: https://github.com/Littlewhinging/cloudflare-dynamic-dns
 Author: Littlewhinging
+License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cloudflare==2.11.1
 Requires-Dist: requests==2.31.0
 
 # Cloudflare Dynamic DNS
```

### Comparing `cloudflare-dynamic-dns-client-0.2.1/setup.py` & `cloudflare-dynamic-dns-client-0.2.2/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 	description = f.read()
 
 setup(
 	name='cloudflare-dynamic-dns-client',
 	description='Allows selfhosting on cloudflare with a dynamic ip address',
 	long_description=description,
 	long_description_content_type='text/markdown',
-	version='0.2.1',
+	version='0.2.2',
+	license='MIT',
+	url='https://github.com/Littlewhinging/cloudflare-dynamic-dns',
 	packages=['cloudflare_dynamic_dns'],
 	author="Littlewhinging",
 	install_requires=[
 		"cloudflare==2.11.1",
 		"requests==2.31.0"
 	],
 	entry_points={
```

