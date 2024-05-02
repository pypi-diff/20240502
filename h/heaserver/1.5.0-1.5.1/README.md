# Comparing `tmp/heaserver-1.5.0.tar.gz` & `tmp/heaserver-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-1.5.0.tar", last modified: Wed Apr 24 17:42:46 2024, max compression
+gzip compressed data, was "heaserver-1.5.1.tar", last modified: Thu May  2 20:03:09 2024, max compression
```

## Comparing `heaserver-1.5.0.tar` & `heaserver-1.5.1.tar`

### file list

```diff
@@ -1,298 +1,298 @@
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.595402 heaserver-1.5.0/
--rw-rw-rw-   0        0        0      261 2022-03-11 01:28:19.000000 heaserver-1.5.0/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-16 23:04:09.000000 heaserver-1.5.0/.gitignore
--rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:19.000000 heaserver-1.5.0/LICENSE
--rw-rw-rw-   0        0        0      243 2023-12-16 23:04:09.000000 heaserver-1.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     7410 2024-04-24 17:42:46.593402 heaserver-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     5415 2024-04-24 17:41:47.000000 heaserver-1.5.0/README.md
--rw-rw-rw-   0        0        0     1612 2023-12-16 23:04:09.000000 heaserver-1.5.0/RELEASING.md
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.099751 heaserver-1.5.0/awss3integrationtests/
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.100753 heaserver-1.5.0/awss3integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.130874 heaserver-1.5.0/awss3integrationtests/heaserver/awss3tests/
--rw-rw-rw-   0        0        0        0 2023-12-16 23:04:09.000000 heaserver-1.5.0/awss3integrationtests/heaserver/awss3tests/__init__.py
--rw-rw-rw-   0        0        0    34976 2024-04-01 23:40:09.000000 heaserver-1.5.0/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py
--rw-rw-rw-   0        0        0     1416 2023-12-16 23:04:09.000000 heaserver-1.5.0/awss3integrationtests/heaserver/awss3tests/service.py
--rw-rw-rw-   0        0        0    19401 2024-04-08 18:06:35.000000 heaserver-1.5.0/awss3integrationtests/heaserver/awss3tests/test_all.py
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.132874 heaserver-1.5.0/awss3integrationtests/heaserver/awss3tests/wstl/
--rw-rw-rw-   0        0        0    16955 2023-12-16 23:04:09.000000 heaserver-1.5.0/awss3integrationtests/heaserver/awss3tests/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.101753 heaserver-1.5.0/awss3tests/
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.102753 heaserver-1.5.0/awss3tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.134874 heaserver-1.5.0/awss3tests/heaserver/awss3tests/
--rw-rw-rw-   0        0        0        0 2023-12-16 23:04:09.000000 heaserver-1.5.0/awss3tests/heaserver/awss3tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.143993 heaserver-1.5.0/awss3tests/heaserver/awss3tests/__pycache__/
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.16864
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.27996
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29888
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0     3169 2023-12-16 23:04:09.000000 heaserver-1.5.0/awss3tests/heaserver/awss3tests/test_all.py
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.103752 heaserver-1.5.0/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.104751 heaserver-1.5.0/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.171990 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.204244 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/
--rw-rw-rw-   0        0        0     1722 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0     1722 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160
--rw-rw-rw-   0        0        0      612 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-310-pytest-7.4.0.pyc.28520
--rw-rw-rw-   0        0        0     1465 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0     1465 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0      630 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0      630 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.35160
--rw-rw-rw-   0        0        0     3839 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0     3839 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0     6100 2024-04-16 21:05:42.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-311-pytest-7.4.4.pyc.40780
--rw-rw-rw-   0        0        0     1290 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.28520
--rw-rw-rw-   0        0        0     1290 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160
--rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.28520
--rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.35160
--rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0     1723 2024-03-19 23:29:00.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.24968
--rw-rw-rw-   0        0        0     1043 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.28520
--rw-rw-rw-   0        0        0     1043 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0      627 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0      627 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0     5996 2023-12-16 23:04:09.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/clienttestcase.py
--rw-rw-rw-   0        0        0     6620 2023-12-16 23:04:09.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py
--rw-rw-rw-   0        0        0     5992 2024-04-09 21:13:46.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py
--rw-rw-rw-   0        0        0     5775 2024-04-22 16:37:36.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py
--rw-rw-rw-   0        0        0     5544 2024-04-22 17:09:51.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py
--rw-rw-rw-   0        0        0    12856 2023-12-16 23:04:10.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/service.py
--rw-rw-rw-   0        0        0     1024 2023-12-16 23:04:10.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_client.py
--rw-rw-rw-   0        0        0     1193 2023-12-16 23:04:10.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py
--rw-rw-rw-   0        0        0      198 2023-12-16 23:04:10.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_delete_component.py
--rw-rw-rw-   0        0        0      194 2022-03-11 01:28:19.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_get_all_components.py
--rw-rw-rw-   0        0        0      888 2023-12-16 23:04:10.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_get_component.py
--rw-rw-rw-   0        0        0      207 2023-12-16 23:04:10.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_get_organization_permissions.py
--rw-rw-rw-   0        0        0     4749 2024-04-09 21:13:46.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py
--rw-rw-rw-   0        0        0     1011 2023-12-16 23:04:10.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py
--rw-rw-rw-   0        0        0      521 2023-12-16 23:04:10.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_post_component.py
--rw-rw-rw-   0        0        0      404 2023-12-16 23:04:10.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_put_component.py
--rw-rw-rw-   0        0        0      203 2023-12-16 23:04:10.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_put_organization_permissions.py
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.206799 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/wstl/
--rw-rw-rw-   0        0        0    16440 2023-12-16 23:04:10.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/wstl/all.json
--rw-rw-rw-   0        0        0      132 2023-12-16 23:04:10.000000 heaserver-1.5.0/pytest.ini
--rw-rw-rw-   0        0        0      237 2023-12-16 23:04:10.000000 heaserver-1.5.0/requirements_dev.txt
--rw-rw-rw-   0        0        0       42 2024-04-24 17:42:46.595402 heaserver-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0     2870 2024-04-24 17:42:09.000000 heaserver-1.5.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.106753 heaserver-1.5.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.106753 heaserver-1.5.0/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.290086 heaserver-1.5.0/src/heaserver/service/
--rw-rw-rw-   0        0        0     1176 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/__init__.py
--rw-rw-rw-   0        0        0     7213 2024-01-04 00:01:31.000000 heaserver-1.5.0/src/heaserver/service/activity.py
--rw-rw-rw-   0        0        0    14193 2024-02-07 00:24:57.000000 heaserver-1.5.0/src/heaserver/service/aiohttp.py
--rw-rw-rw-   0        0        0     1688 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/appfactory.py
--rw-rw-rw-   0        0        0      758 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/appproperty.py
--rw-rw-rw-   0        0        0     8521 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/backgroundtasks.py
--rw-rw-rw-   0        0        0     1497 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/caching.py
--rw-rw-rw-   0        0        0       64 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/caching_strategy.py
--rw-rw-rw-   0        0        0    23443 2024-04-22 20:13:28.000000 heaserver-1.5.0/src/heaserver/service/client.py
--rw-rw-rw-   0        0        0     2460 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/config.py
--rw-rw-rw-   0        0        0      256 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/customhdrs.py
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.312079 heaserver-1.5.0/src/heaserver/service/db/
--rw-rw-rw-   0        0        0      392 2022-03-11 01:28:19.000000 heaserver-1.5.0/src/heaserver/service/db/__init__.py
--rw-rw-rw-   0        0        0    27286 2024-04-22 15:45:21.000000 heaserver-1.5.0/src/heaserver/service/db/aws.py
--rw-rw-rw-   0        0        0    58921 2024-03-27 00:01:36.000000 heaserver-1.5.0/src/heaserver/service/db/awsservicelib.py
--rw-rw-rw-   0        0        0    31583 2024-04-18 02:12:50.000000 heaserver-1.5.0/src/heaserver/service/db/database.py
--rw-rw-rw-   0        0        0     6599 2022-03-11 01:28:19.000000 heaserver-1.5.0/src/heaserver/service/db/dbapi2.py
--rw-rw-rw-   0        0        0    31960 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/db/mongo.py
--rw-rw-rw-   0        0        0     4515 2024-04-05 18:40:52.000000 heaserver-1.5.0/src/heaserver/service/db/mongoexpr.py
--rw-rw-rw-   0        0        0    26453 2024-04-03 23:37:27.000000 heaserver-1.5.0/src/heaserver/service/db/mongoservicelib.py
--rw-rw-rw-   0        0        0      252 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/defaults.py
--rw-rw-rw-   0        0        0      150 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/error.py
--rw-rw-rw-   0        0        0     4709 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/expression.py
--rw-rw-rw-   0        0        0      773 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/functional.py
--rw-rw-rw-   0        0        0    19840 2024-03-21 03:54:08.000000 heaserver-1.5.0/src/heaserver/service/heaobjectsupport.py
--rw-rw-rw-   0        0        0      683 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/jsonschema.py
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.321078 heaserver-1.5.0/src/heaserver/service/jsonschemafiles/
--rw-rw-rw-   0        0        0      606 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/jsonschemafiles/__init__.py
--rw-rw-rw-   0        0        0      787 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/jsonschemafiles/cjtemplate.json
--rw-rw-rw-   0        0        0       87 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/jsonschemafiles/nvpjson.json
--rw-rw-rw-   0        0        0     2214 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/jsonschemafiles/wstl.json
--rw-rw-rw-   0        0        0     4970 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/jsonschemafiles/wstlaction.json
--rw-rw-rw-   0        0        0      987 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/jsonschemavalidator.py
--rw-rw-rw-   0        0        0    21655 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/messagebroker.py
--rw-rw-rw-   0        0        0      539 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/mimetypes.py
--rw-rw-rw-   0        0        0      639 2022-03-11 01:28:19.000000 heaserver-1.5.0/src/heaserver/service/oidcclaimhdrs.py
--rw-rw-rw-   0        0        0     1558 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/openapi.py
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.5.0/src/heaserver/service/py.typed
--rw-rw-rw-   0        0        0      103 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/registryproperty.py
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.340081 heaserver-1.5.0/src/heaserver/service/representor/
--rw-rw-rw-   0        0        0     1426 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/representor/__init__.py
--rw-rw-rw-   0        0        0    26065 2024-04-22 23:13:47.000000 heaserver-1.5.0/src/heaserver/service/representor/cj.py
--rw-rw-rw-   0        0        0      170 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/representor/error.py
--rw-rw-rw-   0        0        0     7259 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/representor/factory.py
--rw-rw-rw-   0        0        0     2231 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/representor/nvpjson.py
--rw-rw-rw-   0        0        0     3244 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/representor/representor.py
--rw-rw-rw-   0        0        0     1551 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/representor/wstljson.py
--rw-rw-rw-   0        0        0     1742 2024-03-19 23:15:41.000000 heaserver-1.5.0/src/heaserver/service/representor/xwwwformurlencoded.py
--rw-rw-rw-   0        0        0      114 2022-03-11 01:28:19.000000 heaserver-1.5.0/src/heaserver/service/requestproperty.py
--rw-rw-rw-   0        0        0    29114 2024-04-01 23:40:09.000000 heaserver-1.5.0/src/heaserver/service/response.py
--rw-rw-rw-   0        0        0    15617 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/runner.py
--rw-rw-rw-   0        0        0       32 2024-03-26 22:51:02.000000 heaserver-1.5.0/src/heaserver/service/sources.py
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.371271 heaserver-1.5.0/src/heaserver/service/testcase/
--rw-rw-rw-   0        0        0      167 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/testcase/__init__.py
--rw-rw-rw-   0        0        0     2123 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/testcase/aiohttptestcase.py
--rw-rw-rw-   0        0        0     1508 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/testcase/awsdockermongo.py
--rw-rw-rw-   0        0        0     3944 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/testcase/awss3microservicetestcase.py
--rw-rw-rw-   0        0        0    15471 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/testcase/collection.py
--rw-rw-rw-   0        0        0     6655 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/testcase/docker.py
--rw-rw-rw-   0        0        0     8062 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/testcase/dockermongo.py
--rw-rw-rw-   0        0        0    40481 2024-04-22 17:03:29.000000 heaserver-1.5.0/src/heaserver/service/testcase/expectedvalues.py
--rw-rw-rw-   0        0        0    17534 2024-04-01 23:40:09.000000 heaserver-1.5.0/src/heaserver/service/testcase/microservicetestcase.py
--rw-rw-rw-   0        0        0   130477 2024-04-01 23:40:09.000000 heaserver-1.5.0/src/heaserver/service/testcase/mixin.py
--rw-rw-rw-   0        0        0    18431 2024-04-05 18:40:52.000000 heaserver-1.5.0/src/heaserver/service/testcase/mockaws.py
--rw-rw-rw-   0        0        0      662 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/testcase/mockdatabase.py
--rw-rw-rw-   0        0        0    21242 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/testcase/mockmongo.py
--rw-rw-rw-   0        0        0      555 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/testcase/simpleaiohttptestcase.py
--rw-rw-rw-   0        0        0     7531 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/testcase/swaggerui.py
--rw-rw-rw-   0        0        0    29140 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/testcase/testenv.py
--rw-rw-rw-   0        0        0     2132 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/testcase/util.py
--rw-rw-rw-   0        0        0     2877 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/uritemplate.py
--rw-rw-rw-   0        0        0    11636 2024-01-04 00:01:31.000000 heaserver-1.5.0/src/heaserver/service/util.py
--rw-rw-rw-   0        0        0    36804 2024-04-01 23:40:09.000000 heaserver-1.5.0/src/heaserver/service/wstl.py
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.592402 heaserver-1.5.0/src/heaserver.egg-info/
--rw-rw-rw-   0        0        0     7410 2024-04-24 17:42:46.000000 heaserver-1.5.0/src/heaserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    17591 2024-04-24 17:42:46.000000 heaserver-1.5.0/src/heaserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-24 17:42:46.000000 heaserver-1.5.0/src/heaserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      455 2024-04-24 17:42:46.000000 heaserver-1.5.0/src/heaserver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-24 17:42:46.000000 heaserver-1.5.0/src/heaserver.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.109751 heaserver-1.5.0/tests/
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.110752 heaserver-1.5.0/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.448098 heaserver-1.5.0/tests/heaserver/servicetest/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.493402 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/
--rw-rw-rw-   0        0        0    11044 2024-03-19 23:09:55.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.19788
--rw-rw-rw-   0        0        0    11044 2024-03-19 23:09:55.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     5139 2024-03-19 23:09:55.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_caching.cpython-311-pytest-7.4.4.pyc.29888
--rw-rw-rw-   0        0        0    13515 2024-03-19 23:09:55.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.29888
--rw-rw-rw-   0        0        0     2266 2024-03-19 23:09:55.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.19788
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     2605 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0      826 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0    21674 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     1870 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.27996
--rw-rw-rw-   0        0        0     1870 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0    18112 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0    18112 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0    12001 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0    12001 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.3836
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.495403 heaserver-1.5.0/tests/heaserver/servicetest/aiohttpdata/
--rw-rw-rw-   0        0        0      258 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/aiohttpdata/requirements_dev.txt
--rw-rw-rw-   0        0        0     6442 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/componentpermissionstestcase.py
--rw-rw-rw-   0        0        0    17429 2024-04-09 21:13:46.000000 heaserver-1.5.0/tests/heaserver/servicetest/componenttestcase.py
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.498402 heaserver-1.5.0/tests/heaserver/servicetest/db/
--rw-rw-rw-   0        0        0        0 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.506403 heaserver-1.5.0/tests/heaserver/servicetest/db/__pycache__/
--rw-rw-rw-   0        0        0     1344 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.27996
--rw-rw-rw-   0        0        0     1344 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0      551 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/db/test_mongo.py
--rw-rw-rw-   0        0        0     7303 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/db/test_mongoexpr.py
--rw-rw-rw-   0        0        0     5571 2024-04-22 17:04:47.000000 heaserver-1.5.0/tests/heaserver/servicetest/organizationpermissionstestcase.py
--rw-rw-rw-   0        0        0     5997 2024-04-22 17:06:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/organizationtestcase.py
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.527403 heaserver-1.5.0/tests/heaserver/servicetest/representor/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.589403 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/
--rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.27996
--rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.28016
--rw-rw-rw-   0        0        0    54596 2024-03-29 23:13:01.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35228
--rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35444
--rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.37360
--rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     7286 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.19788
--rw-rw-rw-   0        0        0     7286 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11224
--rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11864
--rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13080
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13852
--rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.15488
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.1816
--rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.19788
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.28016
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.30312
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.34620
--rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.37360
--rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.16864
--rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.19712
--rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23624
--rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29888
--rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.4904
--rw-rw-rw-   0        0        0      192 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/all.json
--rw-rw-rw-   0        0        0      268 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/all_cj_item_href.json
--rw-rw-rw-   0        0        0      268 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/all_cj_item_link.json
--rw-rw-rw-   0        0        0      642 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/all_cj_queries.json
--rw-rw-rw-   0        0        0     2670 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/all_cj_template.json
--rw-rw-rw-   0        0        0      267 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_item.json
--rw-rw-rw-   0        0        0      263 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_list.json
--rw-rw-rw-   0        0        0    62769 2024-04-01 23:40:09.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/test_cj.py
--rw-rw-rw-   0        0        0     2671 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/test_factory.py
--rw-rw-rw-   0        0        0     4181 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/test_nvpjson.py
--rw-rw-rw-   0        0        0      281 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/test_supports_links.py
--rw-rw-rw-   0        0        0     5676 2024-04-01 23:40:09.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/test_wstljson.py
--rw-rw-rw-   0        0        0     2396 2024-03-21 03:54:08.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py
--rw-rw-rw-   0        0        0    13067 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/service.py
--rw-rw-rw-   0        0        0     9455 2024-01-04 00:01:31.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_activity.py
--rw-rw-rw-   0        0        0     3976 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_aiohttp.py
--rw-rw-rw-   0        0        0     5894 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_backgroundtasks.py
--rw-rw-rw-   0        0        0     2506 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_caching.py
--rw-rw-rw-   0        0        0     7131 2024-04-09 21:13:46.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_client.py
--rw-rw-rw-   0        0        0     1193 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_component_with_bad_permissions.py
--rw-rw-rw-   0        0        0     1127 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_configuration.py
--rw-rw-rw-   0        0        0      819 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_database_classes.py
--rw-rw-rw-   0        0        0      204 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_delete_component.py
--rw-rw-rw-   0        0        0     6181 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_expression.py
--rw-rw-rw-   0        0        0      405 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_functional.py
--rw-rw-rw-   0        0        0      422 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_get_all_components.py
--rw-rw-rw-   0        0        0     3070 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_get_component.py
--rw-rw-rw-   0        0        0      209 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_get_organization_permissions.py
--rw-rw-rw-   0        0        0     5366 2024-04-09 21:13:46.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_heaobjectsupport.py
--rw-rw-rw-   0        0        0     5746 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_jsonschemavalidator.py
--rw-rw-rw-   0        0        0      909 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_mimetypes.py
--rw-rw-rw-   0        0        0      331 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_not_imported.py
--rw-rw-rw-   0        0        0     1005 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_organization_with_bad_permissions.py
--rw-rw-rw-   0        0        0     1274 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_post_component.py
--rw-rw-rw-   0        0        0     1265 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_put_component.py
--rw-rw-rw-   0        0        0      253 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_put_organization_permissions.py
--rw-rw-rw-   0        0        0     2488 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_response.py
--rw-rw-rw-   0        0        0      570 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_testenv.py
--rw-rw-rw-   0        0        0     1929 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_uritemplate.py
--rw-rw-rw-   0        0        0     8782 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_util.py
--rw-rw-rw-   0        0        0     6255 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_wstl.py
-drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.591403 heaserver-1.5.0/tests/heaserver/servicetest/wstl/
--rw-rw-rw-   0        0        0    16436 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/wstl/all.json
--rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/wstl_1.json
--rw-rw-rw-   0        0        0     1214 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/wstl_10a.json
--rw-rw-rw-   0        0        0     1240 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/wstl_10b.json
--rw-rw-rw-   0        0        0     2355 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/wstl_11.json
--rw-rw-rw-   0        0        0     1187 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/wstl_2.json
--rw-rw-rw-   0        0        0     1190 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/wstl_3.json
--rw-rw-rw-   0        0        0     1158 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/wstl_4.json
--rw-rw-rw-   0        0        0      269 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/wstl_5.json
--rw-rw-rw-   0        0        0      531 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/wstl_6.json
--rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/wstl_7.json
--rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/wstl_8.json
--rw-rw-rw-   0        0        0      204 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/wstl_9.json
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.507836 heaserver-1.5.1/
+-rw-rw-rw-   0        0        0      261 2022-03-11 01:28:19.000000 heaserver-1.5.1/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-16 23:04:09.000000 heaserver-1.5.1/.gitignore
+-rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:19.000000 heaserver-1.5.1/LICENSE
+-rw-rw-rw-   0        0        0      243 2023-12-16 23:04:09.000000 heaserver-1.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     7539 2024-05-02 20:03:09.506836 heaserver-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5544 2024-05-02 20:00:06.000000 heaserver-1.5.1/README.md
+-rw-rw-rw-   0        0        0     1612 2023-12-16 23:04:09.000000 heaserver-1.5.1/RELEASING.md
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.011263 heaserver-1.5.1/awss3integrationtests/
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.011263 heaserver-1.5.1/awss3integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.050263 heaserver-1.5.1/awss3integrationtests/heaserver/awss3tests/
+-rw-rw-rw-   0        0        0        0 2023-12-16 23:04:09.000000 heaserver-1.5.1/awss3integrationtests/heaserver/awss3tests/__init__.py
+-rw-rw-rw-   0        0        0    34976 2024-04-01 23:40:09.000000 heaserver-1.5.1/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py
+-rw-rw-rw-   0        0        0     1416 2023-12-16 23:04:09.000000 heaserver-1.5.1/awss3integrationtests/heaserver/awss3tests/service.py
+-rw-rw-rw-   0        0        0    19401 2024-04-08 18:06:35.000000 heaserver-1.5.1/awss3integrationtests/heaserver/awss3tests/test_all.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.052264 heaserver-1.5.1/awss3integrationtests/heaserver/awss3tests/wstl/
+-rw-rw-rw-   0        0        0    16955 2023-12-16 23:04:09.000000 heaserver-1.5.1/awss3integrationtests/heaserver/awss3tests/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.013261 heaserver-1.5.1/awss3tests/
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.014263 heaserver-1.5.1/awss3tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.057263 heaserver-1.5.1/awss3tests/heaserver/awss3tests/
+-rw-rw-rw-   0        0        0        0 2023-12-16 23:04:09.000000 heaserver-1.5.1/awss3tests/heaserver/awss3tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.068262 heaserver-1.5.1/awss3tests/heaserver/awss3tests/__pycache__/
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.16864
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.27996
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29888
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0     3169 2023-12-16 23:04:09.000000 heaserver-1.5.1/awss3tests/heaserver/awss3tests/test_all.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.016263 heaserver-1.5.1/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.016263 heaserver-1.5.1/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.102261 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.140260 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/
+-rw-rw-rw-   0        0        0     1722 2023-12-20 00:04:02.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0     1722 2023-12-20 00:04:02.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160
+-rw-rw-rw-   0        0        0      612 2023-12-20 00:04:02.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-310-pytest-7.4.0.pyc.28520
+-rw-rw-rw-   0        0        0     1465 2023-12-20 00:04:02.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0     1465 2023-12-20 00:04:02.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0      630 2023-12-20 00:04:02.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0      630 2023-12-20 00:04:02.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.35160
+-rw-rw-rw-   0        0        0     3839 2023-12-20 00:04:02.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0     3839 2023-12-20 00:04:02.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0     6100 2024-04-16 21:05:42.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-311-pytest-7.4.4.pyc.40780
+-rw-rw-rw-   0        0        0     1290 2023-12-20 00:04:02.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.28520
+-rw-rw-rw-   0        0        0     1290 2023-12-20 00:04:02.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160
+-rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.28520
+-rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.35160
+-rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0     1723 2024-03-19 23:29:00.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.24968
+-rw-rw-rw-   0        0        0     1043 2023-12-20 00:04:02.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.28520
+-rw-rw-rw-   0        0        0     1043 2023-12-20 00:04:02.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0      627 2023-12-20 00:04:02.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0      627 2023-12-20 00:04:02.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0     5996 2023-12-16 23:04:09.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/clienttestcase.py
+-rw-rw-rw-   0        0        0     6620 2023-12-16 23:04:09.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py
+-rw-rw-rw-   0        0        0     5992 2024-04-09 21:13:46.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py
+-rw-rw-rw-   0        0        0     5775 2024-05-02 19:49:49.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py
+-rw-rw-rw-   0        0        0     5544 2024-05-02 19:49:49.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py
+-rw-rw-rw-   0        0        0    12856 2023-12-16 23:04:10.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/service.py
+-rw-rw-rw-   0        0        0     1024 2023-12-16 23:04:10.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/test_client.py
+-rw-rw-rw-   0        0        0     1193 2023-12-16 23:04:10.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py
+-rw-rw-rw-   0        0        0      198 2023-12-16 23:04:10.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/test_delete_component.py
+-rw-rw-rw-   0        0        0      194 2022-03-11 01:28:19.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/test_get_all_components.py
+-rw-rw-rw-   0        0        0      888 2023-12-16 23:04:10.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/test_get_component.py
+-rw-rw-rw-   0        0        0      207 2023-12-16 23:04:10.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/test_get_organization_permissions.py
+-rw-rw-rw-   0        0        0     4749 2024-05-02 19:49:49.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py
+-rw-rw-rw-   0        0        0     1011 2023-12-16 23:04:10.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py
+-rw-rw-rw-   0        0        0      521 2023-12-16 23:04:10.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/test_post_component.py
+-rw-rw-rw-   0        0        0      404 2023-12-16 23:04:10.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/test_put_component.py
+-rw-rw-rw-   0        0        0      203 2023-12-16 23:04:10.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/test_put_organization_permissions.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.141260 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/wstl/
+-rw-rw-rw-   0        0        0    16440 2023-12-16 23:04:10.000000 heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/wstl/all.json
+-rw-rw-rw-   0        0        0      132 2023-12-16 23:04:10.000000 heaserver-1.5.1/pytest.ini
+-rw-rw-rw-   0        0        0      237 2023-12-16 23:04:10.000000 heaserver-1.5.1/requirements_dev.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 20:03:09.508836 heaserver-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0     2870 2024-05-02 20:02:29.000000 heaserver-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.020273 heaserver-1.5.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.021263 heaserver-1.5.1/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.201933 heaserver-1.5.1/src/heaserver/service/
+-rw-rw-rw-   0        0        0     1176 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/__init__.py
+-rw-rw-rw-   0        0        0     7213 2024-01-04 00:01:31.000000 heaserver-1.5.1/src/heaserver/service/activity.py
+-rw-rw-rw-   0        0        0    14193 2024-05-02 19:49:49.000000 heaserver-1.5.1/src/heaserver/service/aiohttp.py
+-rw-rw-rw-   0        0        0     1688 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/appfactory.py
+-rw-rw-rw-   0        0        0      758 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/appproperty.py
+-rw-rw-rw-   0        0        0     8521 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/backgroundtasks.py
+-rw-rw-rw-   0        0        0     1497 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/caching.py
+-rw-rw-rw-   0        0        0       64 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/caching_strategy.py
+-rw-rw-rw-   0        0        0    24059 2024-05-02 19:53:04.000000 heaserver-1.5.1/src/heaserver/service/client.py
+-rw-rw-rw-   0        0        0     2460 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/config.py
+-rw-rw-rw-   0        0        0      256 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/customhdrs.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.215937 heaserver-1.5.1/src/heaserver/service/db/
+-rw-rw-rw-   0        0        0      392 2022-03-11 01:28:19.000000 heaserver-1.5.1/src/heaserver/service/db/__init__.py
+-rw-rw-rw-   0        0        0    27286 2024-05-02 19:49:49.000000 heaserver-1.5.1/src/heaserver/service/db/aws.py
+-rw-rw-rw-   0        0        0    58921 2024-03-27 00:01:36.000000 heaserver-1.5.1/src/heaserver/service/db/awsservicelib.py
+-rw-rw-rw-   0        0        0    31583 2024-05-02 19:49:49.000000 heaserver-1.5.1/src/heaserver/service/db/database.py
+-rw-rw-rw-   0        0        0     6599 2022-03-11 01:28:19.000000 heaserver-1.5.1/src/heaserver/service/db/dbapi2.py
+-rw-rw-rw-   0        0        0    31960 2024-05-02 19:49:49.000000 heaserver-1.5.1/src/heaserver/service/db/mongo.py
+-rw-rw-rw-   0        0        0     4515 2024-04-05 18:40:52.000000 heaserver-1.5.1/src/heaserver/service/db/mongoexpr.py
+-rw-rw-rw-   0        0        0    26453 2024-04-03 23:37:27.000000 heaserver-1.5.1/src/heaserver/service/db/mongoservicelib.py
+-rw-rw-rw-   0        0        0      252 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/defaults.py
+-rw-rw-rw-   0        0        0      150 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/error.py
+-rw-rw-rw-   0        0        0     4709 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/expression.py
+-rw-rw-rw-   0        0        0      773 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/functional.py
+-rw-rw-rw-   0        0        0    19840 2024-03-21 03:54:08.000000 heaserver-1.5.1/src/heaserver/service/heaobjectsupport.py
+-rw-rw-rw-   0        0        0      683 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/jsonschema.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.225935 heaserver-1.5.1/src/heaserver/service/jsonschemafiles/
+-rw-rw-rw-   0        0        0      606 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/jsonschemafiles/__init__.py
+-rw-rw-rw-   0        0        0      787 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/jsonschemafiles/cjtemplate.json
+-rw-rw-rw-   0        0        0       87 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/jsonschemafiles/nvpjson.json
+-rw-rw-rw-   0        0        0     2214 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/jsonschemafiles/wstl.json
+-rw-rw-rw-   0        0        0     4970 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/jsonschemafiles/wstlaction.json
+-rw-rw-rw-   0        0        0      987 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/jsonschemavalidator.py
+-rw-rw-rw-   0        0        0    21655 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/messagebroker.py
+-rw-rw-rw-   0        0        0      539 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/mimetypes.py
+-rw-rw-rw-   0        0        0      639 2022-03-11 01:28:19.000000 heaserver-1.5.1/src/heaserver/service/oidcclaimhdrs.py
+-rw-rw-rw-   0        0        0     1558 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/openapi.py
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.5.1/src/heaserver/service/py.typed
+-rw-rw-rw-   0        0        0      103 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/registryproperty.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.237933 heaserver-1.5.1/src/heaserver/service/representor/
+-rw-rw-rw-   0        0        0     1426 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/representor/__init__.py
+-rw-rw-rw-   0        0        0    26065 2024-04-22 23:13:47.000000 heaserver-1.5.1/src/heaserver/service/representor/cj.py
+-rw-rw-rw-   0        0        0      170 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/representor/error.py
+-rw-rw-rw-   0        0        0     7259 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/representor/factory.py
+-rw-rw-rw-   0        0        0     2231 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/representor/nvpjson.py
+-rw-rw-rw-   0        0        0     3244 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/representor/representor.py
+-rw-rw-rw-   0        0        0     1551 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/representor/wstljson.py
+-rw-rw-rw-   0        0        0     1742 2024-03-19 23:15:41.000000 heaserver-1.5.1/src/heaserver/service/representor/xwwwformurlencoded.py
+-rw-rw-rw-   0        0        0      114 2022-03-11 01:28:19.000000 heaserver-1.5.1/src/heaserver/service/requestproperty.py
+-rw-rw-rw-   0        0        0    29114 2024-04-01 23:40:09.000000 heaserver-1.5.1/src/heaserver/service/response.py
+-rw-rw-rw-   0        0        0    15617 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/runner.py
+-rw-rw-rw-   0        0        0       32 2024-03-26 22:51:02.000000 heaserver-1.5.1/src/heaserver/service/sources.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.269931 heaserver-1.5.1/src/heaserver/service/testcase/
+-rw-rw-rw-   0        0        0      167 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/testcase/__init__.py
+-rw-rw-rw-   0        0        0     2123 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/testcase/aiohttptestcase.py
+-rw-rw-rw-   0        0        0     1508 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/testcase/awsdockermongo.py
+-rw-rw-rw-   0        0        0     3944 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/testcase/awss3microservicetestcase.py
+-rw-rw-rw-   0        0        0    15471 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/testcase/collection.py
+-rw-rw-rw-   0        0        0     6655 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/testcase/docker.py
+-rw-rw-rw-   0        0        0     8062 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/testcase/dockermongo.py
+-rw-rw-rw-   0        0        0    40481 2024-04-22 17:03:29.000000 heaserver-1.5.1/src/heaserver/service/testcase/expectedvalues.py
+-rw-rw-rw-   0        0        0    17534 2024-04-01 23:40:09.000000 heaserver-1.5.1/src/heaserver/service/testcase/microservicetestcase.py
+-rw-rw-rw-   0        0        0   130477 2024-04-01 23:40:09.000000 heaserver-1.5.1/src/heaserver/service/testcase/mixin.py
+-rw-rw-rw-   0        0        0    18431 2024-05-02 19:49:49.000000 heaserver-1.5.1/src/heaserver/service/testcase/mockaws.py
+-rw-rw-rw-   0        0        0      662 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/testcase/mockdatabase.py
+-rw-rw-rw-   0        0        0    21242 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/testcase/mockmongo.py
+-rw-rw-rw-   0        0        0      555 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/testcase/simpleaiohttptestcase.py
+-rw-rw-rw-   0        0        0     7531 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/testcase/swaggerui.py
+-rw-rw-rw-   0        0        0    29140 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/testcase/testenv.py
+-rw-rw-rw-   0        0        0     2132 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/testcase/util.py
+-rw-rw-rw-   0        0        0     2877 2023-12-16 23:04:10.000000 heaserver-1.5.1/src/heaserver/service/uritemplate.py
+-rw-rw-rw-   0        0        0    11636 2024-01-04 00:01:31.000000 heaserver-1.5.1/src/heaserver/service/util.py
+-rw-rw-rw-   0        0        0    36804 2024-04-01 23:40:09.000000 heaserver-1.5.1/src/heaserver/service/wstl.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.505836 heaserver-1.5.1/src/heaserver.egg-info/
+-rw-rw-rw-   0        0        0     7539 2024-05-02 20:03:08.000000 heaserver-1.5.1/src/heaserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    17591 2024-05-02 20:03:09.000000 heaserver-1.5.1/src/heaserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 20:03:08.000000 heaserver-1.5.1/src/heaserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      455 2024-05-02 20:03:08.000000 heaserver-1.5.1/src/heaserver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-02 20:03:08.000000 heaserver-1.5.1/src/heaserver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.024261 heaserver-1.5.1/tests/
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.025261 heaserver-1.5.1/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.353233 heaserver-1.5.1/tests/heaserver/servicetest/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.5.1/tests/heaserver/servicetest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.397232 heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/
+-rw-rw-rw-   0        0        0    11044 2024-03-19 23:09:55.000000 heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.19788
+-rw-rw-rw-   0        0        0    11044 2024-03-19 23:09:55.000000 heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     5139 2024-03-19 23:09:55.000000 heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_caching.cpython-311-pytest-7.4.4.pyc.29888
+-rw-rw-rw-   0        0        0    13515 2024-03-19 23:09:55.000000 heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.29888
+-rw-rw-rw-   0        0        0     2266 2024-03-19 23:09:55.000000 heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.19788
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     2605 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0      826 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0    21674 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     1870 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.27996
+-rw-rw-rw-   0        0        0     1870 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0    18112 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0    18112 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0    12001 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0    12001 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.3836
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.399231 heaserver-1.5.1/tests/heaserver/servicetest/aiohttpdata/
+-rw-rw-rw-   0        0        0      258 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/aiohttpdata/requirements_dev.txt
+-rw-rw-rw-   0        0        0     6442 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/componentpermissionstestcase.py
+-rw-rw-rw-   0        0        0    17429 2024-04-09 21:13:46.000000 heaserver-1.5.1/tests/heaserver/servicetest/componenttestcase.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.403232 heaserver-1.5.1/tests/heaserver/servicetest/db/
+-rw-rw-rw-   0        0        0        0 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.411231 heaserver-1.5.1/tests/heaserver/servicetest/db/__pycache__/
+-rw-rw-rw-   0        0        0     1344 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.27996
+-rw-rw-rw-   0        0        0     1344 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0      551 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/db/test_mongo.py
+-rw-rw-rw-   0        0        0     7303 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/db/test_mongoexpr.py
+-rw-rw-rw-   0        0        0     5571 2024-05-02 19:49:49.000000 heaserver-1.5.1/tests/heaserver/servicetest/organizationpermissionstestcase.py
+-rw-rw-rw-   0        0        0     5997 2024-05-02 19:49:49.000000 heaserver-1.5.1/tests/heaserver/servicetest/organizationtestcase.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.434234 heaserver-1.5.1/tests/heaserver/servicetest/representor/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.501837 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/
+-rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.27996
+-rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.28016
+-rw-rw-rw-   0        0        0    54596 2024-03-29 23:13:01.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35228
+-rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35444
+-rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.37360
+-rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     7286 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.19788
+-rw-rw-rw-   0        0        0     7286 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11224
+-rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11864
+-rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13080
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13852
+-rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.15488
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.1816
+-rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.19788
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.28016
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.30312
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.34620
+-rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.37360
+-rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.16864
+-rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.19712
+-rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23624
+-rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29888
+-rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.4904
+-rw-rw-rw-   0        0        0      192 2022-03-11 01:28:19.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/all.json
+-rw-rw-rw-   0        0        0      268 2022-03-11 01:28:19.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/all_cj_item_href.json
+-rw-rw-rw-   0        0        0      268 2022-03-11 01:28:19.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/all_cj_item_link.json
+-rw-rw-rw-   0        0        0      642 2022-03-11 01:28:19.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/all_cj_queries.json
+-rw-rw-rw-   0        0        0     2670 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/all_cj_template.json
+-rw-rw-rw-   0        0        0      267 2022-03-11 01:28:19.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_item.json
+-rw-rw-rw-   0        0        0      263 2022-03-11 01:28:19.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_list.json
+-rw-rw-rw-   0        0        0    62769 2024-04-01 23:40:09.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/test_cj.py
+-rw-rw-rw-   0        0        0     2671 2022-03-11 01:28:19.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/test_factory.py
+-rw-rw-rw-   0        0        0     4181 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/test_nvpjson.py
+-rw-rw-rw-   0        0        0      281 2022-03-11 01:28:19.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/test_supports_links.py
+-rw-rw-rw-   0        0        0     5676 2024-04-01 23:40:09.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/test_wstljson.py
+-rw-rw-rw-   0        0        0     2396 2024-03-21 03:54:08.000000 heaserver-1.5.1/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py
+-rw-rw-rw-   0        0        0    13067 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/service.py
+-rw-rw-rw-   0        0        0     9455 2024-01-04 00:01:31.000000 heaserver-1.5.1/tests/heaserver/servicetest/test_activity.py
+-rw-rw-rw-   0        0        0     3976 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/test_aiohttp.py
+-rw-rw-rw-   0        0        0     5894 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/test_backgroundtasks.py
+-rw-rw-rw-   0        0        0     2506 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/test_caching.py
+-rw-rw-rw-   0        0        0     7131 2024-04-09 21:13:46.000000 heaserver-1.5.1/tests/heaserver/servicetest/test_client.py
+-rw-rw-rw-   0        0        0     1193 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/test_component_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     1127 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/test_configuration.py
+-rw-rw-rw-   0        0        0      819 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/test_database_classes.py
+-rw-rw-rw-   0        0        0      204 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/test_delete_component.py
+-rw-rw-rw-   0        0        0     6181 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/test_expression.py
+-rw-rw-rw-   0        0        0      405 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/test_functional.py
+-rw-rw-rw-   0        0        0      422 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/test_get_all_components.py
+-rw-rw-rw-   0        0        0     3070 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/test_get_component.py
+-rw-rw-rw-   0        0        0      209 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/test_get_organization_permissions.py
+-rw-rw-rw-   0        0        0     5366 2024-04-09 21:13:46.000000 heaserver-1.5.1/tests/heaserver/servicetest/test_heaobjectsupport.py
+-rw-rw-rw-   0        0        0     5746 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/test_jsonschemavalidator.py
+-rw-rw-rw-   0        0        0      909 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/test_mimetypes.py
+-rw-rw-rw-   0        0        0      331 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/test_not_imported.py
+-rw-rw-rw-   0        0        0     1005 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/test_organization_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     1274 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/test_post_component.py
+-rw-rw-rw-   0        0        0     1265 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/test_put_component.py
+-rw-rw-rw-   0        0        0      253 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/test_put_organization_permissions.py
+-rw-rw-rw-   0        0        0     2488 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/test_response.py
+-rw-rw-rw-   0        0        0      570 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/test_testenv.py
+-rw-rw-rw-   0        0        0     1929 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/test_uritemplate.py
+-rw-rw-rw-   0        0        0     8782 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/test_util.py
+-rw-rw-rw-   0        0        0     6255 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/test_wstl.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:03:09.503837 heaserver-1.5.1/tests/heaserver/servicetest/wstl/
+-rw-rw-rw-   0        0        0    16436 2023-12-16 23:04:10.000000 heaserver-1.5.1/tests/heaserver/servicetest/wstl/all.json
+-rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.5.1/tests/heaserver/servicetest/wstl_1.json
+-rw-rw-rw-   0        0        0     1214 2022-03-11 01:28:19.000000 heaserver-1.5.1/tests/heaserver/servicetest/wstl_10a.json
+-rw-rw-rw-   0        0        0     1240 2022-03-11 01:28:19.000000 heaserver-1.5.1/tests/heaserver/servicetest/wstl_10b.json
+-rw-rw-rw-   0        0        0     2355 2022-03-11 01:28:19.000000 heaserver-1.5.1/tests/heaserver/servicetest/wstl_11.json
+-rw-rw-rw-   0        0        0     1187 2022-03-11 01:28:19.000000 heaserver-1.5.1/tests/heaserver/servicetest/wstl_2.json
+-rw-rw-rw-   0        0        0     1190 2022-03-11 01:28:19.000000 heaserver-1.5.1/tests/heaserver/servicetest/wstl_3.json
+-rw-rw-rw-   0        0        0     1158 2022-03-11 01:28:19.000000 heaserver-1.5.1/tests/heaserver/servicetest/wstl_4.json
+-rw-rw-rw-   0        0        0      269 2022-03-11 01:28:19.000000 heaserver-1.5.1/tests/heaserver/servicetest/wstl_5.json
+-rw-rw-rw-   0        0        0      531 2022-03-11 01:28:19.000000 heaserver-1.5.1/tests/heaserver/servicetest/wstl_6.json
+-rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.5.1/tests/heaserver/servicetest/wstl_7.json
+-rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.5.1/tests/heaserver/servicetest/wstl_8.json
+-rw-rw-rw-   0        0        0      204 2022-03-11 01:28:19.000000 heaserver-1.5.1/tests/heaserver/servicetest/wstl_9.json
```

### Comparing `heaserver-1.5.0/LICENSE` & `heaserver-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/PKG-INFO` & `heaserver-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver
-Version: 1.5.0
+Version: 1.5.1
 Summary: The server side of HEA.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -47,14 +47,17 @@
 Requires-Dist: types-cachetools~=5.3.0
 
 # HEA Server Framework
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Server Framework contains shared code for creating HEA microservices.
 
+## Version 1.5.1
+* Ensure the Content-Type header is set to application/json in heaserver.service.client put and post calls.
+
 ## Version 1.5.0
 * Added attribute-level permissions.
 * Temporarily restored the role check that was removed in version 1.4.1 in case an AWS credentials object with overly
 permissive permissions is altered.
 
 ## Version 1.4.2
 * Synchronize around getting temporary credentials.
```

### Comparing `heaserver-1.5.0/README.md` & `heaserver-1.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # HEA Server Framework
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Server Framework contains shared code for creating HEA microservices.
 
+## Version 1.5.1
+* Ensure the Content-Type header is set to application/json in heaserver.service.client put and post calls.
+
 ## Version 1.5.0
 * Added attribute-level permissions.
 * Temporarily restored the role check that was removed in version 1.4.1 in case an AWS credentials object with overly
 permissive permissions is altered.
 
 ## Version 1.4.2
 * Synchronize around getting temporary credentials.
```

### Comparing `heaserver-1.5.0/RELEASING.md` & `heaserver-1.5.1/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py` & `heaserver-1.5.1/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/awss3integrationtests/heaserver/awss3tests/service.py` & `heaserver-1.5.1/awss3integrationtests/heaserver/awss3tests/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/awss3integrationtests/heaserver/awss3tests/test_all.py` & `heaserver-1.5.1/awss3integrationtests/heaserver/awss3tests/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/awss3integrationtests/heaserver/awss3tests/wstl/all.json` & `heaserver-1.5.1/awss3integrationtests/heaserver/awss3tests/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.16864` & `heaserver-1.5.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.16864`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.27996` & `heaserver-1.5.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.27996`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.5.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29888` & `heaserver-1.5.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29888`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.5.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/awss3tests/heaserver/awss3tests/test_all.py` & `heaserver-1.5.1/awss3tests/heaserver/awss3tests/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-310-pytest-7.4.0.pyc.28520` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-310-pytest-7.4.0.pyc.28520`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.35160` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.35160`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-311-pytest-7.4.4.pyc.40780` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-311-pytest-7.4.4.pyc.40780`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.28520` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.28520`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.28520` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.28520`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.35160` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.35160`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.24968` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.24968`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.28520` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.28520`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/clienttestcase.py` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/clienttestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/service.py` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_client.py` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/test_client.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_get_component.py` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/test_get_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_post_component.py` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/test_post_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/wstl/all.json` & `heaserver-1.5.1/integrationtests/heaserver/serviceintegrationtest/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/setup.py` & `heaserver-1.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='heaserver',
-      version='1.5.0',
+      version='1.5.1',
       description='The server side of HEA.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://risr.hci.utah.edu',
       author='Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT',
       author_email='Andrew.Post@hci.utah.edu',
       python_requires='>=3.10',
```

### Comparing `heaserver-1.5.0/src/heaserver/service/__init__.py` & `heaserver-1.5.1/src/heaserver/service/__init__.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/activity.py` & `heaserver-1.5.1/src/heaserver/service/activity.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/aiohttp.py` & `heaserver-1.5.1/src/heaserver/service/aiohttp.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/appfactory.py` & `heaserver-1.5.1/src/heaserver/service/appfactory.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/appproperty.py` & `heaserver-1.5.1/src/heaserver/service/appproperty.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/backgroundtasks.py` & `heaserver-1.5.1/src/heaserver/service/backgroundtasks.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/caching.py` & `heaserver-1.5.1/src/heaserver/service/caching.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/client.py` & `heaserver-1.5.1/src/heaserver/service/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from aiohttp import ClientResponse, ClientResponseError, hdrs, web, ClientSession
 from aiohttp.client_exceptions import ClientConnectionError
 from heaobject import root
-from heaobject.root import DesktopObject, DesktopObjectTypeVar, DesktopObjectDict, desktop_object_from_dict
-from heaobject.registry import Component, Property, Collection
+from heaobject.root import DesktopObjectTypeVar, DesktopObjectDict, desktop_object_from_dict
+from heaobject.registry import Component, Property
 from heaobject.volume import DEFAULT_FILE_SYSTEM, MongoDBFileSystem, FileSystem
 from heaserver.service.util import retry
 from . import appproperty, response
 from .aiohttp import StreamReaderWrapper, SupportsAsyncRead
 from .representor import nvpjson
 from yarl import URL
 from typing import Optional, Union, Dict, Type, Mapping, AsyncGenerator, Sequence
+from copy import copy
 import logging
 
 
 async def get_streaming(request: web.Request, url: Union[str, URL],
                         headers: Optional[Dict[str, str]] = None,
                         client_session: ClientSession | None = None) -> web.StreamResponse:
     """
@@ -231,50 +232,58 @@
         for r in result:
             obj__ = obj___()
             obj__.from_dict(r)
             yield obj__
 
 
 async def post(app: web.Application, url: Union[URL, str], data: root.DesktopObject | root.DesktopObjectDict,
-               headers: Dict[str, str] = None,
+               headers: Mapping[str, str] = None,
                client_session: ClientSession | None = None) -> str:  # type: ignore[return]
     """
     Coroutine that posts a HEAObject to a HEA service.
 
     :param app: the aiohttp application context (required).
     :param url: the The URL (str or URL) of the resource (required).
     :param data: the DesktopObject or DesktopObjectDict (required).
-    :param headers: optional dict of headers.
+    :param headers: optional headers. The Content-Type header is set to application/json, regardless of what it was set
+    to in the passed-in headers.
     :param client_session: a client session. If None, the default session will be used.
     :return: the URL string in the response's Location header.
     :raises ClientResponseError: if the response's status code was unexpected.
     """
     session = client_session if client_session is not None else app[appproperty.HEA_CLIENT_SESSION]
-    async with session.post(url, json=data, headers=headers, raise_for_status=False) as response_:
+    headers_ = copy(headers) if headers is not None else {}
+    headers_[hdrs.CONTENT_TYPE] = nvpjson.MIME_TYPE
+    async with session.post(url, json=data, headers=headers_, raise_for_status=False) as response_:
         if response_.status != 201:
             await _raise_client_response_error(response_)
         return response_.headers['Location']
 
 
 async def put(app: web.Application, url: Union[URL, str], data: root.DesktopObject | root.DesktopObjectDict,
-              headers: Dict[str, str] = None,
+              headers: Mapping[str, str] = None,
               client_session: ClientSession | None = None) -> None:
     """
     Coroutine that updates a HEAObject.
 
     :param app: the aiohttp application context (required).
     :param url: the The URL (str or URL) of the resource (required).
     :param data: the DesktopObject or DesktopObjectDict (required).
-    :param headers: optional dict of headers.
+    :param headers: optional dict of headers. The Content-Type header is set to application/json, regardless of what
+    it was set to in the passed-in headers.
     :param client_session: a client session. If None, the default session will be used.
     :returns if successful it returns None else if it fails it will raise HttpError
     :raises ClientResponseError: if the response's status code was unexpected.
     """
     session = client_session if client_session is not None else app[appproperty.HEA_CLIENT_SESSION]
-    async with session.put(url, json=data, headers=headers, raise_for_status=False) as response_:
+    # You can pass a desktop object into the json parameter because the session object is configured with a custom
+    # json encoder that handles HEAObject.
+    headers_ = copy(headers) if headers is not None else {}
+    headers_[hdrs.CONTENT_TYPE] = nvpjson.MIME_TYPE
+    async with session.put(url, json=data, headers=headers_, raise_for_status=False) as response_:
         if response_.status != 204:
             await _raise_client_response_error(response_)
 
 
 async def delete(app: web.Application, url: Union[URL, str],
                  headers: Dict[str, str] = None,
                  client_session: ClientSession | None = None) -> None:
```

### Comparing `heaserver-1.5.0/src/heaserver/service/config.py` & `heaserver-1.5.1/src/heaserver/service/config.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/db/aws.py` & `heaserver-1.5.1/src/heaserver/service/db/aws.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/db/awsservicelib.py` & `heaserver-1.5.1/src/heaserver/service/db/awsservicelib.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/db/database.py` & `heaserver-1.5.1/src/heaserver/service/db/database.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/db/dbapi2.py` & `heaserver-1.5.1/src/heaserver/service/db/dbapi2.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/db/mongo.py` & `heaserver-1.5.1/src/heaserver/service/db/mongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/db/mongoexpr.py` & `heaserver-1.5.1/src/heaserver/service/db/mongoexpr.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/db/mongoservicelib.py` & `heaserver-1.5.1/src/heaserver/service/db/mongoservicelib.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/expression.py` & `heaserver-1.5.1/src/heaserver/service/expression.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/functional.py` & `heaserver-1.5.1/src/heaserver/service/functional.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/heaobjectsupport.py` & `heaserver-1.5.1/src/heaserver/service/heaobjectsupport.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/jsonschema.py` & `heaserver-1.5.1/src/heaserver/service/jsonschema.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/jsonschemafiles/__init__.py` & `heaserver-1.5.1/src/heaserver/service/jsonschemafiles/__init__.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/jsonschemafiles/cjtemplate.json` & `heaserver-1.5.1/src/heaserver/service/jsonschemafiles/cjtemplate.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/jsonschemafiles/wstl.json` & `heaserver-1.5.1/src/heaserver/service/jsonschemafiles/wstl.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/jsonschemafiles/wstlaction.json` & `heaserver-1.5.1/src/heaserver/service/jsonschemafiles/wstlaction.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/jsonschemavalidator.py` & `heaserver-1.5.1/src/heaserver/service/jsonschemavalidator.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/messagebroker.py` & `heaserver-1.5.1/src/heaserver/service/messagebroker.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/mimetypes.py` & `heaserver-1.5.1/src/heaserver/service/mimetypes.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/oidcclaimhdrs.py` & `heaserver-1.5.1/src/heaserver/service/oidcclaimhdrs.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/openapi.py` & `heaserver-1.5.1/src/heaserver/service/openapi.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/representor/__init__.py` & `heaserver-1.5.1/src/heaserver/service/representor/__init__.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/representor/cj.py` & `heaserver-1.5.1/src/heaserver/service/representor/cj.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/representor/factory.py` & `heaserver-1.5.1/src/heaserver/service/representor/factory.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/representor/nvpjson.py` & `heaserver-1.5.1/src/heaserver/service/representor/nvpjson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/representor/representor.py` & `heaserver-1.5.1/src/heaserver/service/representor/representor.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/representor/wstljson.py` & `heaserver-1.5.1/src/heaserver/service/representor/wstljson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/representor/xwwwformurlencoded.py` & `heaserver-1.5.1/src/heaserver/service/representor/xwwwformurlencoded.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/response.py` & `heaserver-1.5.1/src/heaserver/service/response.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/runner.py` & `heaserver-1.5.1/src/heaserver/service/runner.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/testcase/aiohttptestcase.py` & `heaserver-1.5.1/src/heaserver/service/testcase/aiohttptestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/testcase/awsdockermongo.py` & `heaserver-1.5.1/src/heaserver/service/testcase/awsdockermongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/testcase/awss3microservicetestcase.py` & `heaserver-1.5.1/src/heaserver/service/testcase/awss3microservicetestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/testcase/collection.py` & `heaserver-1.5.1/src/heaserver/service/testcase/collection.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/testcase/docker.py` & `heaserver-1.5.1/src/heaserver/service/testcase/docker.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/testcase/dockermongo.py` & `heaserver-1.5.1/src/heaserver/service/testcase/dockermongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/testcase/expectedvalues.py` & `heaserver-1.5.1/src/heaserver/service/testcase/expectedvalues.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/testcase/microservicetestcase.py` & `heaserver-1.5.1/src/heaserver/service/testcase/microservicetestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/testcase/mixin.py` & `heaserver-1.5.1/src/heaserver/service/testcase/mixin.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/testcase/mockaws.py` & `heaserver-1.5.1/src/heaserver/service/testcase/mockaws.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/testcase/mockdatabase.py` & `heaserver-1.5.1/src/heaserver/service/testcase/mockdatabase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/testcase/mockmongo.py` & `heaserver-1.5.1/src/heaserver/service/testcase/mockmongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/testcase/simpleaiohttptestcase.py` & `heaserver-1.5.1/src/heaserver/service/testcase/simpleaiohttptestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/testcase/swaggerui.py` & `heaserver-1.5.1/src/heaserver/service/testcase/swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/testcase/testenv.py` & `heaserver-1.5.1/src/heaserver/service/testcase/testenv.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/testcase/util.py` & `heaserver-1.5.1/src/heaserver/service/testcase/util.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/uritemplate.py` & `heaserver-1.5.1/src/heaserver/service/uritemplate.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/util.py` & `heaserver-1.5.1/src/heaserver/service/util.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver/service/wstl.py` & `heaserver-1.5.1/src/heaserver/service/wstl.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/src/heaserver.egg-info/PKG-INFO` & `heaserver-1.5.1/src/heaserver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver
-Version: 1.5.0
+Version: 1.5.1
 Summary: The server side of HEA.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -47,14 +47,17 @@
 Requires-Dist: types-cachetools~=5.3.0
 
 # HEA Server Framework
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Server Framework contains shared code for creating HEA microservices.
 
+## Version 1.5.1
+* Ensure the Content-Type header is set to application/json in heaserver.service.client put and post calls.
+
 ## Version 1.5.0
 * Added attribute-level permissions.
 * Temporarily restored the role check that was removed in version 1.4.1 in case an AWS credentials object with overly
 permissive permissions is altered.
 
 ## Version 1.4.2
 * Synchronize around getting temporary credentials.
```

### Comparing `heaserver-1.5.0/src/heaserver.egg-info/SOURCES.txt` & `heaserver-1.5.1/src/heaserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.19788` & `heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.19788`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_caching.cpython-311-pytest-7.4.4.pyc.29888` & `heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_caching.cpython-311-pytest-7.4.4.pyc.29888`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.29888` & `heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.29888`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.19788` & `heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.19788`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.27996` & `heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.27996`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.5.1/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/componentpermissionstestcase.py` & `heaserver-1.5.1/tests/heaserver/servicetest/componentpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/componenttestcase.py` & `heaserver-1.5.1/tests/heaserver/servicetest/componenttestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.27996` & `heaserver-1.5.1/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.27996`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.5.1/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.5.1/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.5.1/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.5.1/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/db/test_mongo.py` & `heaserver-1.5.1/tests/heaserver/servicetest/db/test_mongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/db/test_mongoexpr.py` & `heaserver-1.5.1/tests/heaserver/servicetest/db/test_mongoexpr.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/organizationpermissionstestcase.py` & `heaserver-1.5.1/tests/heaserver/servicetest/organizationpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/organizationtestcase.py` & `heaserver-1.5.1/tests/heaserver/servicetest/organizationtestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.27996` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.27996`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.28016` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.28016`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35228` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35228`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35444` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35444`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.37360` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.37360`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.19788` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.19788`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11224` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11224`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11864` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11864`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13080` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13080`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13852` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13852`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.15488` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.15488`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.1816` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.1816`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.19788` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.19788`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.28016` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.28016`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.30312` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.30312`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.34620` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.34620`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.37360` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.37360`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.16864` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.16864`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.19712` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.19712`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23624` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23624`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29888` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29888`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.4904` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.4904`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/all_cj_queries.json` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/all_cj_queries.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/all_cj_template.json` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/all_cj_template.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/test_cj.py` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/test_cj.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/test_factory.py` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/test_factory.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/test_nvpjson.py` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/test_nvpjson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/test_wstljson.py` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/test_wstljson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py` & `heaserver-1.5.1/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/service.py` & `heaserver-1.5.1/tests/heaserver/servicetest/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/test_activity.py` & `heaserver-1.5.1/tests/heaserver/servicetest/test_activity.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/test_aiohttp.py` & `heaserver-1.5.1/tests/heaserver/servicetest/test_aiohttp.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/test_backgroundtasks.py` & `heaserver-1.5.1/tests/heaserver/servicetest/test_backgroundtasks.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/test_caching.py` & `heaserver-1.5.1/tests/heaserver/servicetest/test_caching.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/test_client.py` & `heaserver-1.5.1/tests/heaserver/servicetest/test_client.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/test_component_with_bad_permissions.py` & `heaserver-1.5.1/tests/heaserver/servicetest/test_component_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/test_configuration.py` & `heaserver-1.5.1/tests/heaserver/servicetest/test_configuration.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/test_database_classes.py` & `heaserver-1.5.1/tests/heaserver/servicetest/test_database_classes.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/test_expression.py` & `heaserver-1.5.1/tests/heaserver/servicetest/test_expression.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/test_get_component.py` & `heaserver-1.5.1/tests/heaserver/servicetest/test_get_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/test_heaobjectsupport.py` & `heaserver-1.5.1/tests/heaserver/servicetest/test_heaobjectsupport.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/test_jsonschemavalidator.py` & `heaserver-1.5.1/tests/heaserver/servicetest/test_jsonschemavalidator.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/test_mimetypes.py` & `heaserver-1.5.1/tests/heaserver/servicetest/test_mimetypes.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/test_organization_with_bad_permissions.py` & `heaserver-1.5.1/tests/heaserver/servicetest/test_organization_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/test_post_component.py` & `heaserver-1.5.1/tests/heaserver/servicetest/test_post_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/test_put_component.py` & `heaserver-1.5.1/tests/heaserver/servicetest/test_put_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/test_response.py` & `heaserver-1.5.1/tests/heaserver/servicetest/test_response.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/test_testenv.py` & `heaserver-1.5.1/tests/heaserver/servicetest/test_testenv.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/test_uritemplate.py` & `heaserver-1.5.1/tests/heaserver/servicetest/test_uritemplate.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/test_util.py` & `heaserver-1.5.1/tests/heaserver/servicetest/test_util.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/test_wstl.py` & `heaserver-1.5.1/tests/heaserver/servicetest/test_wstl.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/wstl/all.json` & `heaserver-1.5.1/tests/heaserver/servicetest/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/wstl_1.json` & `heaserver-1.5.1/tests/heaserver/servicetest/wstl_1.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/wstl_10a.json` & `heaserver-1.5.1/tests/heaserver/servicetest/wstl_10a.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/wstl_10b.json` & `heaserver-1.5.1/tests/heaserver/servicetest/wstl_10b.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/wstl_11.json` & `heaserver-1.5.1/tests/heaserver/servicetest/wstl_11.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/wstl_2.json` & `heaserver-1.5.1/tests/heaserver/servicetest/wstl_2.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/wstl_3.json` & `heaserver-1.5.1/tests/heaserver/servicetest/wstl_3.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/wstl_4.json` & `heaserver-1.5.1/tests/heaserver/servicetest/wstl_4.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/wstl_6.json` & `heaserver-1.5.1/tests/heaserver/servicetest/wstl_6.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/wstl_7.json` & `heaserver-1.5.1/tests/heaserver/servicetest/wstl_7.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.5.0/tests/heaserver/servicetest/wstl_8.json` & `heaserver-1.5.1/tests/heaserver/servicetest/wstl_8.json`

 * *Files identical despite different names*

