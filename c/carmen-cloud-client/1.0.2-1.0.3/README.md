# Comparing `tmp/carmen_cloud_client-1.0.2.tar.gz` & `tmp/carmen_cloud_client-1.0.3.tar.gz`

## Comparing `carmen_cloud_client-1.0.2.tar` & `carmen_cloud_client-1.0.3.tar`

### file list

```diff
@@ -1,61 +1,60 @@
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/.editorconfig
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/.env.example
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/DEVELOPMENT.md
--rwxr-xr-x   0        0        0      305 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/generate-response.sh
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/requirements-dev.txt
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/requirements.txt
--rwxr-xr-x   0        0        0      303 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/update-openapi-spec.sh
--rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/.github/workflows/ci.yml
--rw-r--r--   0        0        0    11533 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/assets/transport/response.schema.json
--rw-r--r--   0        0        0    35039 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/assets/vehicle/response.schema.json
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/__init__.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/errors.py
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/__init__.py
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/__init__.py
--rw-r--r--   0        0        0    53584 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/accr_usa01.jpg
--rw-r--r--   0        0        0    50105 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/accr_usa02.jpg
--rw-r--r--   0        0        0    50896 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/accr_usa03.jpg
--rw-r--r--   0        0        0   174381 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/accr_usa20.jpg
--rw-r--r--   0        0        0   407461 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/bra01.jpg
--rw-r--r--   0        0        0   464913 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/bra02.jpg
--rw-r--r--   0        0        0   444103 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/bra03.jpg
--rw-r--r--   0        0        0   290590 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/bra20.jpg
--rw-r--r--   0        0        0    58721 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/chassis01.jpg
--rw-r--r--   0        0        0    55968 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/chassis02.jpg
--rw-r--r--   0        0        0    54027 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/chassis03.jpg
--rw-r--r--   0        0        0    51029 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/chassis20.jpg
--rw-r--r--   0        0        0   591726 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/ilu01.jpg
--rw-r--r--   0        0        0   631603 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/ilu02.jpg
--rw-r--r--   0        0        0   591726 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/ilu03.jpg
--rw-r--r--   0        0        0   322324 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/ilu20.jpg
--rw-r--r--   0        0        0    37129 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/iso01.jpg
--rw-r--r--   0        0        0    37277 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/iso02.jpg
--rw-r--r--   0        0        0    37085 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/iso03.jpg
--rw-r--r--   0        0        0  1671730 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/iso20.jpg
--rw-r--r--   0        0        0     8930 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/test_client.py
--rw-r--r--   0        0        0    18554 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/uic01.jpg
--rw-r--r--   0        0        0    18263 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/uic02.jpg
--rw-r--r--   0        0        0    18360 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/uic03.jpg
--rw-r--r--   0        0        0   134606 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/uic20.jpg
--rw-r--r--   0        0        0    56764 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/usdot01.jpg
--rw-r--r--   0        0        0    56799 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/usdot02.jpg
--rw-r--r--   0        0        0    57487 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/usdot03.jpg
--rw-r--r--   0        0        0   984026 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/usdot20.jpg
--rw-r--r--   0        0        0    62487 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/vehicle/adr-test.jpg
--rwxr-xr-x   0        0        0   221278 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/vehicle/many_plates_hun.jpg
--rw-r--r--   0        0        0   287526 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/vehicle/test.jpg
--rw-r--r--   0        0        0     8068 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/test/vehicle/test_client.py
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/transport/__init__.py
--rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/transport/client.py
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/transport/options.py
--rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/transport/response.py
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/vehicle/__init__.py
--rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/vehicle/client.py
--rw-r--r--   0        0        0    21298 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/vehicle/options.py
--rw-r--r--   0        0        0    19472 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/carmen_cloud_client/vehicle/response.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/LICENSE
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/README.md
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2181 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/.dockerignore
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/.editorconfig
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/.env.example
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/DEVELOPMENT.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/Dockerfile
+-rwxr-xr-x   0        0        0      305 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/generate-response.sh
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/requirements-dev.txt
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/requirements.txt
+-rwxr-xr-x   0        0        0      303 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/update-openapi-spec.sh
+-rw-r--r--   0        0        0      812 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/.github/workflows/ci.yml
+-rw-r--r--   0        0        0    11533 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/assets/transport/response.schema.json
+-rw-r--r--   0        0        0    35039 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/assets/vehicle/response.schema.json
+-rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/__init__.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/errors.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/__init__.py
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/__init__.py
+-rw-r--r--   0        0        0    53584 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/accr_usa01.jpg
+-rw-r--r--   0        0        0    50105 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/accr_usa02.jpg
+-rw-r--r--   0        0        0    50896 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/accr_usa03.jpg
+-rw-r--r--   0        0        0   174381 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/accr_usa20.jpg
+-rw-r--r--   0        0        0   407461 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/bra01.jpg
+-rw-r--r--   0        0        0   464913 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/bra02.jpg
+-rw-r--r--   0        0        0   444103 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/bra03.jpg
+-rw-r--r--   0        0        0   290590 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/bra20.jpg
+-rw-r--r--   0        0        0    58721 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/chassis01.jpg
+-rw-r--r--   0        0        0    55968 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/chassis02.jpg
+-rw-r--r--   0        0        0    54027 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/chassis03.jpg
+-rw-r--r--   0        0        0    51029 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/chassis20.jpg
+-rw-r--r--   0        0        0   591726 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/ilu01.jpg
+-rw-r--r--   0        0        0   631603 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/ilu02.jpg
+-rw-r--r--   0        0        0   591726 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/ilu03.jpg
+-rw-r--r--   0        0        0   322324 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/ilu20.jpg
+-rwxr-xr-x   0        0        0  1310563 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/iso01.jpg
+-rwxr-xr-x   0        0        0  1303972 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/iso02.jpg
+-rwxr-xr-x   0        0        0   568572 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/iso20.jpg
+-rw-r--r--   0        0        0     8457 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/test_client.py
+-rw-r--r--   0        0        0    18554 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/uic01.jpg
+-rw-r--r--   0        0        0    18263 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/uic02.jpg
+-rw-r--r--   0        0        0    18360 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/uic03.jpg
+-rw-r--r--   0        0        0   134606 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/uic20.jpg
+-rwxr-xr-x   0        0        0   111561 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/usdot01.jpg
+-rwxr-xr-x   0        0        0   117809 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/usdot20.jpg
+-rw-r--r--   0        0        0    62487 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/vehicle/adr-test.jpg
+-rwxr-xr-x   0        0        0   221278 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/vehicle/many_plates_hun.jpg
+-rw-r--r--   0        0        0   287526 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/vehicle/test.jpg
+-rw-r--r--   0        0        0     8068 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/test/vehicle/test_client.py
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/transport/__init__.py
+-rw-r--r--   0        0        0     5587 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/transport/client.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/transport/options.py
+-rw-r--r--   0        0        0     6249 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/transport/response.py
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/vehicle/__init__.py
+-rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/vehicle/client.py
+-rw-r--r--   0        0        0    21298 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/vehicle/options.py
+-rw-r--r--   0        0        0    19472 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/carmen_cloud_client/vehicle/response.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/LICENSE
+-rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/README.md
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 carmen_cloud_client-1.0.3/PKG-INFO
```

### Comparing `carmen_cloud_client-1.0.2/requirements-dev.txt` & `carmen_cloud_client-1.0.3/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/.github/workflows/ci.yml` & `carmen_cloud_client-1.0.3/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/assets/transport/response.schema.json` & `carmen_cloud_client-1.0.3/assets/transport/response.schema.json`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/assets/vehicle/response.schema.json` & `carmen_cloud_client-1.0.3/assets/vehicle/response.schema.json`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/errors.py` & `carmen_cloud_client-1.0.3/carmen_cloud_client/errors.py`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/accr_usa01.jpg` & `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/accr_usa01.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/accr_usa02.jpg` & `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/accr_usa02.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/accr_usa03.jpg` & `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/accr_usa03.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/accr_usa20.jpg` & `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/accr_usa20.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/bra01.jpg` & `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/bra01.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/bra02.jpg` & `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/bra02.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/bra03.jpg` & `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/bra03.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/bra20.jpg` & `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/bra20.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/chassis01.jpg` & `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/chassis01.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/chassis02.jpg` & `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/chassis02.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/chassis03.jpg` & `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/chassis03.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/chassis20.jpg` & `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/chassis20.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/ilu01.jpg` & `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/ilu01.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/ilu02.jpg` & `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/ilu02.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/ilu03.jpg` & `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/ilu03.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/ilu20.jpg` & `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/ilu20.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/test_client.py` & `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/test_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,31 +14,31 @@
 api_key = os.getenv("TEST_DEV_API_KEY", "")
 endpoint = os.getenv("TEST_DEV_ENDPOINT_URL", "")
 eu_prod_api_key = os.getenv("TEST_EU_PROD_API_KEY", "")
 us_prod_api_key = os.getenv("TEST_US_PROD_API_KEY", "")
 
 test_options = TransportAPIOptions(
     api_key=api_key,
-    type=CodeType.ACCR_USA,
+    type=CodeType.TRUCK,
     endpoint=endpoint
 )
 
 def test_invalid_options_throws():
     invalid_options = TransportAPIOptions(
         api_key=api_key,
-        type=CodeType.ACCR_USA,
+        type=CodeType.TRUCK,
         cloud_service_region="INVALID",
     )
     with pytest.raises(CarmenAPIConfigError):
         TransportAPIClient(invalid_options)
 
 def test_maxreads_zero_throws():
     invalid_options = TransportAPIOptions(
         api_key=api_key,
-        type=CodeType.ACCR_USA,
+        type=CodeType.TRUCK,
         max_reads=0,
         endpoint=endpoint,
     )
     with pytest.raises(CarmenAPIConfigError):
         TransportAPIClient(invalid_options)
 
 def test_empty_imagedataorpaths_throws():
@@ -80,15 +80,15 @@
     assert response.data is not None
     assert response.data.codes is not None
     assert len(response.data.codes) == 1
     assert response.data.codes[0].code == "NFLZ049511"
     assert response.data.codes[0].imageResults is not None
     assert len(response.data.codes[0].imageResults) == 4
 
-def test_can_read_ACCR_USA_codes():
+def test_can_read_TRUCK_codes():
     client = TransportAPIClient(test_options)
     response = client.send(
         os.path.join(current_directory, "accr_usa01.jpg"),
         os.path.join(current_directory, "accr_usa02.jpg"),
         os.path.join(current_directory, "accr_usa03.jpg"),
         os.path.join(current_directory, "accr_usa20.jpg"),
     )
@@ -98,15 +98,15 @@
     assert response.data.codes[0].code == "NFLZ049511"
     assert response.data.codes[0].imageResults is not None
     assert len(response.data.codes[0].imageResults) == 4
 
 def test_can_read_BRA_codes():
     client = TransportAPIClient(TransportAPIOptions(
         api_key=api_key,
-        type=CodeType.BRA,
+        type=CodeType.AM_RAIL,
         endpoint=endpoint
     ))
     response = client.send(
         os.path.join(current_directory, "bra01.jpg"),
         os.path.join(current_directory, "bra02.jpg"),
         os.path.join(current_directory, "bra03.jpg"),
         os.path.join(current_directory, "bra20.jpg"),
@@ -117,15 +117,15 @@
     assert response.data.codes[0].code == "HFE0599760"
     assert response.data.codes[0].imageResults is not None
     assert len(response.data.codes[0].imageResults) == 4
 
 def test_can_read_chassis_codes():
     client = TransportAPIClient(TransportAPIOptions(
         api_key=api_key,
-        type=CodeType.CHASSIS,
+        type=CodeType.TRUCK,
         endpoint=endpoint
     ))
     response = client.send(
         os.path.join(current_directory, "chassis01.jpg"),
         os.path.join(current_directory, "chassis02.jpg"),
         os.path.join(current_directory, "chassis03.jpg"),
         os.path.join(current_directory, "chassis20.jpg"),
@@ -136,53 +136,49 @@
     assert response.data.codes[0].code == "MAEC623857"
     assert response.data.codes[0].imageResults is not None
     assert len(response.data.codes[0].imageResults) == 4
 
 def test_can_read_ilu_codes():
     client = TransportAPIClient(TransportAPIOptions(
         api_key=api_key,
-        type=CodeType.ILU,
+        type=CodeType.ISO,
         endpoint=endpoint
     ))
     response = client.send(
         os.path.join(current_directory, "ilu01.jpg"),
         os.path.join(current_directory, "ilu02.jpg"),
         os.path.join(current_directory, "ilu03.jpg"),
-        os.path.join(current_directory, "ilu20.jpg"),
     )
     assert response.data is not None
     assert response.data.codes is not None
     assert len(response.data.codes) == 1
-    assert response.data.codes[0].code == "LKWA06011300WI1"
+    assert response.data.codes[0].code == "REID0008406"
     assert response.data.codes[0].imageResults is not None
-    assert len(response.data.codes[0].imageResults) == 4
+    assert len(response.data.codes[0].imageResults) == 3
 
 def test_can_read_iso_codes():
     client = TransportAPIClient(TransportAPIOptions(
         api_key=api_key,
         type=CodeType.ISO,
         endpoint=endpoint
     ))
     response = client.send(
         os.path.join(current_directory, "iso01.jpg"),
-        os.path.join(current_directory, "iso02.jpg"),
-        os.path.join(current_directory, "iso03.jpg"),
-        os.path.join(current_directory, "iso20.jpg"),
     )
     assert response.data is not None
     assert response.data.codes is not None
     assert len(response.data.codes) == 1
-    assert response.data.codes[0].code == "NOSU2463454SG2210"
+    assert response.data.codes[0].code == "TCKU387869122G1"
     assert response.data.codes[0].imageResults is not None
-    assert len(response.data.codes[0].imageResults) == 4
+    assert len(response.data.codes[0].imageResults) == 1
 
 def test_can_read_uic_codes():
     client = TransportAPIClient(TransportAPIOptions(
         api_key=api_key,
-        type=CodeType.UIC,
+        type=CodeType.EU_RAIL,
         endpoint=endpoint
     ))
     response = client.send(
         os.path.join(current_directory, "uic01.jpg"),
         os.path.join(current_directory, "uic02.jpg"),
         os.path.join(current_directory, "uic03.jpg"),
         os.path.join(current_directory, "uic20.jpg"),
@@ -193,39 +189,35 @@
     assert response.data.codes[0].code == "818068616353"
     assert response.data.codes[0].imageResults is not None
     assert len(response.data.codes[0].imageResults) == 4
 
 def test_can_read_usdot_codes():
     client = TransportAPIClient(TransportAPIOptions(
         api_key=api_key,
-        type=CodeType.USDOT,
+        type=CodeType.TRUCK,
         endpoint=endpoint
     ))
     response = client.send(
         os.path.join(current_directory, "usdot01.jpg"),
-        os.path.join(current_directory, "usdot02.jpg"),
-        os.path.join(current_directory, "usdot03.jpg"),
-        os.path.join(current_directory, "usdot20.jpg"),
     )
     assert response.data is not None
     assert response.data.codes is not None
     assert len(response.data.codes) == 1
-    assert response.data.codes[0].code == "1201193"
+    assert response.data.codes[0].code == "USDOT95406"
     assert response.data.codes[0].imageResults is not None
-    assert len(response.data.codes[0].imageResults) == 4
+    assert len(response.data.codes[0].imageResults) == 1
 
 def test_has_a_package_version_that_matches_the_api_response_version():
     client = TransportAPIClient(test_options)
     response = client.send(
         os.path.join(current_directory, "accr_usa01.jpg"),
         os.path.join(current_directory, "accr_usa02.jpg"),
         os.path.join(current_directory, "accr_usa03.jpg"),
-        os.path.join(current_directory, "accr_usa20.jpg"),
     )
     assert response.version is not None
-    client_version = version.parse(client.supported_api_version + '.0')
-    response_version = version.parse(response.version + '.0')
-    readme_version = version.parse(extract_api_version_from_readme("Transportation & Cargo API") + '.0')
+    client_version = version.parse(client.supported_api_version)
+    response_version = version.parse(response.version)
+    readme_version = version.parse(extract_api_version_from_readme("Transportation & Cargo API"))
     assert client_version.major == response_version.major
     assert client_version.minor == response_version.minor
     assert client_version.major == readme_version.major
     assert client_version.minor == readme_version.minor
```

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/uic01.jpg` & `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/uic01.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/uic02.jpg` & `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/uic02.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/uic03.jpg` & `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/uic03.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/test/transport/uic20.jpg` & `carmen_cloud_client-1.0.3/carmen_cloud_client/test/transport/uic20.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/test/vehicle/adr-test.jpg` & `carmen_cloud_client-1.0.3/carmen_cloud_client/test/vehicle/adr-test.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/test/vehicle/many_plates_hun.jpg` & `carmen_cloud_client-1.0.3/carmen_cloud_client/test/vehicle/many_plates_hun.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/test/vehicle/test.jpg` & `carmen_cloud_client-1.0.3/carmen_cloud_client/test/vehicle/test.jpg`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/test/vehicle/test_client.py` & `carmen_cloud_client-1.0.3/carmen_cloud_client/test/vehicle/test_client.py`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/transport/client.py` & `carmen_cloud_client-1.0.3/carmen_cloud_client/transport/client.py`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/transport/options.py` & `carmen_cloud_client-1.0.3/carmen_cloud_client/transport/options.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,24 +2,18 @@
 from typing import Optional
 from enum import Enum
 
 class CodeType(Enum):
     """
     The type of code to read.
     """
-    ACCR_USA = "accr_usa"
-    ILU = "ilu"
     ISO = "iso"
-    MOCO = "moco"
-    BRA = "bra"
-    RUS = "rus"
-    UIC = "uic"
-    AAR = "aar"
-    CHASSIS = "chassis"
-    USDOT = "usdot"
+    TRUCK = "truck"
+    AM_RAIL = "am-rail"
+    EU_RAIL = "eu-rail"
 
 @dataclass
 class TransportAPIOptions:
     """
     Options for configuring the TransportAPI client.
     """
     api_key: str
```

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/transport/response.py` & `carmen_cloud_client-1.0.3/carmen_cloud_client/transport/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  response.schema.json
-#   timestamp: 2024-01-23T15:28:50+00:00
+#   timestamp: 2024-04-26T11:06:14+00:00
 
 from __future__ import annotations
 
 from typing import List, Optional
 
 from pydantic import BaseModel, Field, conint
```

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/vehicle/client.py` & `carmen_cloud_client-1.0.3/carmen_cloud_client/vehicle/client.py`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/vehicle/options.py` & `carmen_cloud_client-1.0.3/carmen_cloud_client/vehicle/options.py`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/carmen_cloud_client/vehicle/response.py` & `carmen_cloud_client-1.0.3/carmen_cloud_client/vehicle/response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # generated by datamodel-codegen:
 #   filename:  response.schema.json
-#   timestamp: 2024-01-23T15:28:51+00:00
+#   timestamp: 2024-04-26T11:06:15+00:00
 
 from __future__ import annotations
 
 from typing import List, Optional
 
 from pydantic import BaseModel, Field, conint
```

### Comparing `carmen_cloud_client-1.0.2/LICENSE` & `carmen_cloud_client-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `carmen_cloud_client-1.0.2/README.md` & `carmen_cloud_client-1.0.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,54 @@
 # Carmen Cloud Client by Adaptive Recognition
 
 Python client for [Carmen Cloud](https://carmencloud.com/) by [Adaptive Recognition](https://adaptiverecognition.com/). This unified library provides you with access to both the **Vehicle API** and the **Transportation & Cargo API**.
 
 ## Supported API Versions
 
-- Vehicle API: v1.4
-- Transportation & Cargo API: v1.0
+- Vehicle API: v1.4.1
+- Transportation & Cargo API: v1.0.1
 
 ## 🛠️ How to Install
 
 ```sh
 pip install carmen-cloud-client
 ```
 
 ## 🚀 Usage
 
 You can utilize either the Vehicle API or the Transportation & Cargo API based on your needs.
 
 ### 🚗 Vehicle API
 
 ```python
-from carmen_cloud_client import VehicleAPIClient, SelectedServices,  Locations
+from carmen_cloud_client import VehicleAPIClient, VehicleAPIOptions, SelectedServices, Locations
 
-client = VehicleAPIClient(
+options = VehicleAPIOptions(
     api_key="<YOUR_API_KEY>",
     services=SelectedServices(anpr=True, mmr=True),
     input_image_location=Locations.Europe.Hungary,
     cloud_service_region="EU"
 )
+client = VehicleAPIClient(options)
 
 response = client.send("./car.jpg")
 print(response)
 ```
 
 ### 🚚 Transportation & Cargo API
 
 ```python
-from carmen_cloud_client import TransportAPIClient, CodeType
+from carmen_cloud_client import TransportAPIClient, TransportAPIOptions, CodeType
 
-client = TransportAPIClient(
+options = TransportAPIOptions(
     api_key="<YOUR_API_KEY>",
-    code_type=CodeType.ISO,
+    type=CodeType.ISO,
     cloud_service_region="EU"
 )
+client = TransportAPIClient(options)
 
 response = client.send("./container.jpg")
 print(response)
 ```
 
 ## 🔧 Development
```

### Comparing `carmen_cloud_client-1.0.2/pyproject.toml` & `carmen_cloud_client-1.0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "carmen_cloud_client"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Botond BALÁZS", email="botond.balazs@arip.hu" },
 ]
 description = "Python client for Carmen Cloud by Adaptive Recognition. Efficiently read license plates, recognize vehicle details, and process container, railway wagon, and US DOT codes."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -22,7 +22,11 @@
     "pydantic>=1.10.9",
     "urllib3>=2.0.3",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/adaptiverecognition/python-carmen-cloud-client"
 "Bug Tracker" = "https://github.com/adaptiverecognition/python-carmen-cloud-client/issues"
+
+[[tool.pydoc-markdown.loaders]]
+type = "python"
+search_path = [ "./carmen_cloud_client" ]
```

### Comparing `carmen_cloud_client-1.0.2/PKG-INFO` & `carmen_cloud_client-1.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: carmen_cloud_client
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python client for Carmen Cloud by Adaptive Recognition. Efficiently read license plates, recognize vehicle details, and process container, railway wagon, and US DOT codes.
 Project-URL: Homepage, https://github.com/adaptiverecognition/python-carmen-cloud-client
 Project-URL: Bug Tracker, https://github.com/adaptiverecognition/python-carmen-cloud-client/issues
 Author-email: Botond BALÁZS <botond.balazs@arip.hu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -18,53 +18,55 @@
 
 # Carmen Cloud Client by Adaptive Recognition
 
 Python client for [Carmen Cloud](https://carmencloud.com/) by [Adaptive Recognition](https://adaptiverecognition.com/). This unified library provides you with access to both the **Vehicle API** and the **Transportation & Cargo API**.
 
 ## Supported API Versions
 
-- Vehicle API: v1.4
-- Transportation & Cargo API: v1.0
+- Vehicle API: v1.4.1
+- Transportation & Cargo API: v1.0.1
 
 ## 🛠️ How to Install
 
 ```sh
 pip install carmen-cloud-client
 ```
 
 ## 🚀 Usage
 
 You can utilize either the Vehicle API or the Transportation & Cargo API based on your needs.
 
 ### 🚗 Vehicle API
 
 ```python
-from carmen_cloud_client import VehicleAPIClient, SelectedServices,  Locations
+from carmen_cloud_client import VehicleAPIClient, VehicleAPIOptions, SelectedServices, Locations
 
-client = VehicleAPIClient(
+options = VehicleAPIOptions(
     api_key="<YOUR_API_KEY>",
     services=SelectedServices(anpr=True, mmr=True),
     input_image_location=Locations.Europe.Hungary,
     cloud_service_region="EU"
 )
+client = VehicleAPIClient(options)
 
 response = client.send("./car.jpg")
 print(response)
 ```
 
 ### 🚚 Transportation & Cargo API
 
 ```python
-from carmen_cloud_client import TransportAPIClient, CodeType
+from carmen_cloud_client import TransportAPIClient, TransportAPIOptions, CodeType
 
-client = TransportAPIClient(
+options = TransportAPIOptions(
     api_key="<YOUR_API_KEY>",
-    code_type=CodeType.ISO,
+    type=CodeType.ISO,
     cloud_service_region="EU"
 )
+client = TransportAPIClient(options)
 
 response = client.send("./container.jpg")
 print(response)
 ```
 
 ## 🔧 Development
```

