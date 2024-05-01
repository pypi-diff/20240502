# Comparing `tmp/cloudflare-dynamic-dns-client-0.1.1.tar.gz` & `tmp/cloudflare-dynamic-dns-client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudflare-dynamic-dns-client-0.1.1.tar", last modified: Tue Apr 30 23:24:59 2024, max compression
+gzip compressed data, was "cloudflare-dynamic-dns-client-0.1.2.tar", last modified: Tue Apr 30 23:27:30 2024, max compression
```

## Comparing `cloudflare-dynamic-dns-client-0.1.1.tar` & `cloudflare-dynamic-dns-client-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 23:24:59.994026 cloudflare-dynamic-dns-client-0.1.1/
--rw-rw-rw-   0        0        0      168 2024-04-30 23:24:59.992520 cloudflare-dynamic-dns-client-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0        6 2024-04-30 21:50:57.000000 cloudflare-dynamic-dns-client-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 23:24:59.973481 cloudflare-dynamic-dns-client-0.1.1/cloudflare_dynamic_dns/
--rw-rw-rw-   0        0        0       64 2024-04-30 22:38:15.000000 cloudflare-dynamic-dns-client-0.1.1/cloudflare_dynamic_dns/__init__.py
--rw-rw-rw-   0        0        0     3253 2024-04-30 22:59:20.000000 cloudflare-dynamic-dns-client-0.1.1/cloudflare_dynamic_dns/__main__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 23:24:59.991517 cloudflare-dynamic-dns-client-0.1.1/cloudflare_dynamic_dns_client.egg-info/
--rw-rw-rw-   0        0        0      168 2024-04-30 23:24:59.000000 cloudflare-dynamic-dns-client-0.1.1/cloudflare_dynamic_dns_client.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      408 2024-04-30 23:24:59.000000 cloudflare-dynamic-dns-client-0.1.1/cloudflare_dynamic_dns_client.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 23:24:59.000000 cloudflare-dynamic-dns-client-0.1.1/cloudflare_dynamic_dns_client.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-04-30 23:24:59.000000 cloudflare-dynamic-dns-client-0.1.1/cloudflare_dynamic_dns_client.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2024-04-30 23:24:59.000000 cloudflare-dynamic-dns-client-0.1.1/cloudflare_dynamic_dns_client.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-04-30 23:24:59.000000 cloudflare-dynamic-dns-client-0.1.1/cloudflare_dynamic_dns_client.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 23:24:59.994026 cloudflare-dynamic-dns-client-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      370 2024-04-30 23:24:44.000000 cloudflare-dynamic-dns-client-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-30 23:27:30.613798 cloudflare-dynamic-dns-client-0.1.2/
+-rw-rw-rw-   0        0        0      237 2024-04-30 23:27:30.612790 cloudflare-dynamic-dns-client-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0        6 2024-04-30 21:50:57.000000 cloudflare-dynamic-dns-client-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-30 23:27:30.598215 cloudflare-dynamic-dns-client-0.1.2/cloudflare_dynamic_dns/
+-rw-rw-rw-   0        0        0       64 2024-04-30 22:38:15.000000 cloudflare-dynamic-dns-client-0.1.2/cloudflare_dynamic_dns/__init__.py
+-rw-rw-rw-   0        0        0     3253 2024-04-30 22:59:20.000000 cloudflare-dynamic-dns-client-0.1.2/cloudflare_dynamic_dns/__main__.py
+drwxrwxrwx   0        0        0        0 2024-04-30 23:27:30.611285 cloudflare-dynamic-dns-client-0.1.2/cloudflare_dynamic_dns_client.egg-info/
+-rw-rw-rw-   0        0        0      237 2024-04-30 23:27:30.000000 cloudflare-dynamic-dns-client-0.1.2/cloudflare_dynamic_dns_client.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      408 2024-04-30 23:27:30.000000 cloudflare-dynamic-dns-client-0.1.2/cloudflare_dynamic_dns_client.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-30 23:27:30.000000 cloudflare-dynamic-dns-client-0.1.2/cloudflare_dynamic_dns_client.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       80 2024-04-30 23:27:30.000000 cloudflare-dynamic-dns-client-0.1.2/cloudflare_dynamic_dns_client.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2024-04-30 23:27:30.000000 cloudflare-dynamic-dns-client-0.1.2/cloudflare_dynamic_dns_client.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-04-30 23:27:30.000000 cloudflare-dynamic-dns-client-0.1.2/cloudflare_dynamic_dns_client.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-30 23:27:30.614796 cloudflare-dynamic-dns-client-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      446 2024-04-30 23:27:25.000000 cloudflare-dynamic-dns-client-0.1.2/setup.py
```

### Comparing `cloudflare-dynamic-dns-client-0.1.1/cloudflare_dynamic_dns/__main__.py` & `cloudflare-dynamic-dns-client-0.1.2/cloudflare_dynamic_dns/__main__.py`

 * *Files identical despite different names*

