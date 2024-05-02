# Comparing `tmp/viggopayfac-1.0.8.tar.gz` & `tmp/viggopayfac-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viggopayfac-1.0.8.tar", last modified: Wed Mar 13 11:38:21 2024, max compression
+gzip compressed data, was "viggopayfac-1.0.9.tar", last modified: Mon Mar 18 19:24:59 2024, max compression
```

## Comparing `viggopayfac-1.0.8.tar` & `viggopayfac-1.0.9.tar`

### file list

```diff
@@ -1,35 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 11:38:21.726752 viggopayfac-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 11:37:23.000000 viggopayfac-1.0.8/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-13 11:37:23.000000 viggopayfac-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-13 11:37:23.000000 viggopayfac-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-13 11:38:21.726752 viggopayfac-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-13 11:37:23.000000 viggopayfac-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-13 11:37:23.000000 viggopayfac-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 11:38:21.726752 viggopayfac-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-13 11:37:23.000000 viggopayfac-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 11:38:21.722752 viggopayfac-1.0.8/viggopayfac/
--rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-03-13 11:37:23.000000 viggopayfac-1.0.8/viggopayfac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-13 11:37:23.000000 viggopayfac-1.0.8/viggopayfac/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-13 11:37:23.000000 viggopayfac-1.0.8/viggopayfac/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 11:38:21.722752 viggopayfac-1.0.8/viggopayfac/subsystem/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 11:37:23.000000 viggopayfac-1.0.8/viggopayfac/subsystem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 11:38:21.722752 viggopayfac-1.0.8/viggopayfac/subsystem/controle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-13 11:37:23.000000 viggopayfac-1.0.8/viggopayfac/subsystem/controle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 11:38:21.722752 viggopayfac-1.0.8/viggopayfac/subsystem/controle/configuracao_pay_fac/
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-13 11:37:23.000000 viggopayfac-1.0.8/viggopayfac/subsystem/controle/configuracao_pay_fac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-03-13 11:37:23.000000 viggopayfac-1.0.8/viggopayfac/subsystem/controle/configuracao_pay_fac/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-03-13 11:37:23.000000 viggopayfac-1.0.8/viggopayfac/subsystem/controle/configuracao_pay_fac/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-13 11:37:23.000000 viggopayfac-1.0.8/viggopayfac/subsystem/controle/configuracao_pay_fac/router.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 11:38:21.726752 viggopayfac-1.0.8/viggopayfac/subsystem/controle/pay_fac/
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-13 11:37:23.000000 viggopayfac-1.0.8/viggopayfac/subsystem/controle/pay_fac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9102 2024-03-13 11:37:23.000000 viggopayfac-1.0.8/viggopayfac/subsystem/controle/pay_fac/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)    22812 2024-03-13 11:37:23.000000 viggopayfac-1.0.8/viggopayfac/subsystem/controle/pay_fac/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-13 11:37:23.000000 viggopayfac-1.0.8/viggopayfac/subsystem/controle/pay_fac/resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-03-13 11:37:23.000000 viggopayfac-1.0.8/viggopayfac/subsystem/controle/pay_fac/router.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-03-13 11:37:23.000000 viggopayfac-1.0.8/viggopayfac/subsystem/controle/pay_fac/transaction_hash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 11:38:21.722752 viggopayfac-1.0.8/viggopayfac.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-13 11:38:21.000000 viggopayfac-1.0.8/viggopayfac.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-03-13 11:38:21.000000 viggopayfac-1.0.8/viggopayfac.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 11:38:21.000000 viggopayfac-1.0.8/viggopayfac.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-13 11:38:21.000000 viggopayfac-1.0.8/viggopayfac.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-13 11:38:21.000000 viggopayfac-1.0.8/viggopayfac.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:24:58.999548 viggopayfac-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 19:24:00.000000 viggopayfac-1.0.9/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-18 19:24:00.000000 viggopayfac-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-18 19:24:00.000000 viggopayfac-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-18 19:24:58.999548 viggopayfac-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-18 19:24:00.000000 viggopayfac-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-18 19:24:00.000000 viggopayfac-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 19:24:58.999548 viggopayfac-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-18 19:24:00.000000 viggopayfac-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:24:58.995548 viggopayfac-1.0.9/viggopayfac/
+-rw-r--r--   0 runner    (1001) docker     (127)     1284 2024-03-18 19:24:00.000000 viggopayfac-1.0.9/viggopayfac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-18 19:24:00.000000 viggopayfac-1.0.9/viggopayfac/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-18 19:24:00.000000 viggopayfac-1.0.9/viggopayfac/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:24:58.999548 viggopayfac-1.0.9/viggopayfac/subsystem/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 19:24:00.000000 viggopayfac-1.0.9/viggopayfac/subsystem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:24:58.999548 viggopayfac-1.0.9/viggopayfac/subsystem/controle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 19:24:00.000000 viggopayfac-1.0.9/viggopayfac/subsystem/controle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:24:58.999548 viggopayfac-1.0.9/viggopayfac/subsystem/controle/configuracao_pay_fac/
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-18 19:24:00.000000 viggopayfac-1.0.9/viggopayfac/subsystem/controle/configuracao_pay_fac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-03-18 19:24:00.000000 viggopayfac-1.0.9/viggopayfac/subsystem/controle/configuracao_pay_fac/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-03-18 19:24:00.000000 viggopayfac-1.0.9/viggopayfac/subsystem/controle/configuracao_pay_fac/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-18 19:24:00.000000 viggopayfac-1.0.9/viggopayfac/subsystem/controle/configuracao_pay_fac/router.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:24:58.999548 viggopayfac-1.0.9/viggopayfac/subsystem/controle/pay_fac/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-03-18 19:24:00.000000 viggopayfac-1.0.9/viggopayfac/subsystem/controle/pay_fac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-18 19:24:00.000000 viggopayfac-1.0.9/viggopayfac/subsystem/controle/pay_fac/config_ambiente.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9001 2024-03-18 19:24:00.000000 viggopayfac-1.0.9/viggopayfac/subsystem/controle/pay_fac/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22812 2024-03-18 19:24:00.000000 viggopayfac-1.0.9/viggopayfac/subsystem/controle/pay_fac/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-18 19:24:00.000000 viggopayfac-1.0.9/viggopayfac/subsystem/controle/pay_fac/resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-03-18 19:24:00.000000 viggopayfac-1.0.9/viggopayfac/subsystem/controle/pay_fac/router.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-03-18 19:24:00.000000 viggopayfac-1.0.9/viggopayfac/subsystem/controle/pay_fac/transaction_hash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 19:24:58.999548 viggopayfac-1.0.9/viggopayfac.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-18 19:24:58.000000 viggopayfac-1.0.9/viggopayfac.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-03-18 19:24:58.000000 viggopayfac-1.0.9/viggopayfac.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 19:24:58.000000 viggopayfac-1.0.9/viggopayfac.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-18 19:24:58.000000 viggopayfac-1.0.9/viggopayfac.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-18 19:24:58.000000 viggopayfac-1.0.9/viggopayfac.egg-info/top_level.txt
```

### Comparing `viggopayfac-1.0.8/LICENSE` & `viggopayfac-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `viggopayfac-1.0.8/viggopayfac/__init__.py` & `viggopayfac-1.0.9/viggopayfac/__init__.py`

 * *Files identical despite different names*

### Comparing `viggopayfac-1.0.8/viggopayfac/resources.py` & `viggopayfac-1.0.9/viggopayfac/resources.py`

 * *Files identical despite different names*

### Comparing `viggopayfac-1.0.8/viggopayfac/subsystem/controle/configuracao_pay_fac/manager.py` & `viggopayfac-1.0.9/viggopayfac/subsystem/controle/configuracao_pay_fac/manager.py`

 * *Files identical despite different names*

### Comparing `viggopayfac-1.0.8/viggopayfac/subsystem/controle/configuracao_pay_fac/resource.py` & `viggopayfac-1.0.9/viggopayfac/subsystem/controle/configuracao_pay_fac/resource.py`

 * *Files identical despite different names*

### Comparing `viggopayfac-1.0.8/viggopayfac/subsystem/controle/configuracao_pay_fac/router.py` & `viggopayfac-1.0.9/viggopayfac/subsystem/controle/configuracao_pay_fac/router.py`

 * *Files identical despite different names*

### Comparing `viggopayfac-1.0.8/viggopayfac/subsystem/controle/pay_fac/controller.py` & `viggopayfac-1.0.9/viggopayfac/subsystem/controle/pay_fac/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 import flask
 import json
 import uuid
 
 from viggocore.common import exception, utils, controller
-from viggopayfac.subsystem.controle.configuracao_pay_fac.resource \
-    import ConfiguracaoPayFacTipo as cpf_tipo
+from viggopayfac.subsystem.controle.pay_fac.config_ambiente \
+    import get_api_payfac
 
 
 class Controller(controller.CommonController):
-    # TODO(JorgeSilva): trocar por ambiente de PRODUCAO antes de subir
-    API_PAYFAC = cpf_tipo.HOMOLOGACAO
+    API_PAYFAC = get_api_payfac()
 
     def __init__(self, manager, resource_wrap, collection_wrap):
         super(Controller, self).__init__(
             manager, resource_wrap, collection_wrap)
 
     def montar_response_dict(self, response):
         try:
```

### Comparing `viggopayfac-1.0.8/viggopayfac/subsystem/controle/pay_fac/manager.py` & `viggopayfac-1.0.9/viggopayfac/subsystem/controle/pay_fac/manager.py`

 * *Files identical despite different names*

### Comparing `viggopayfac-1.0.8/viggopayfac/subsystem/controle/pay_fac/router.py` & `viggopayfac-1.0.9/viggopayfac/subsystem/controle/pay_fac/router.py`

 * *Files identical despite different names*

### Comparing `viggopayfac-1.0.8/viggopayfac/subsystem/controle/pay_fac/transaction_hash.py` & `viggopayfac-1.0.9/viggopayfac/subsystem/controle/pay_fac/transaction_hash.py`

 * *Files identical despite different names*

### Comparing `viggopayfac-1.0.8/viggopayfac.egg-info/SOURCES.txt` & `viggopayfac-1.0.9/viggopayfac.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -15,12 +15,13 @@
 viggopayfac/subsystem/__init__.py
 viggopayfac/subsystem/controle/__init__.py
 viggopayfac/subsystem/controle/configuracao_pay_fac/__init__.py
 viggopayfac/subsystem/controle/configuracao_pay_fac/manager.py
 viggopayfac/subsystem/controle/configuracao_pay_fac/resource.py
 viggopayfac/subsystem/controle/configuracao_pay_fac/router.py
 viggopayfac/subsystem/controle/pay_fac/__init__.py
+viggopayfac/subsystem/controle/pay_fac/config_ambiente.py
 viggopayfac/subsystem/controle/pay_fac/controller.py
 viggopayfac/subsystem/controle/pay_fac/manager.py
 viggopayfac/subsystem/controle/pay_fac/resource.py
 viggopayfac/subsystem/controle/pay_fac/router.py
 viggopayfac/subsystem/controle/pay_fac/transaction_hash.py
```

