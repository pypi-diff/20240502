# Comparing `tmp/data_horizon-0.1.2.tar.gz` & `tmp/data_horizon-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_horizon-0.1.2.tar", max compression
+gzip compressed data, was "data_horizon-0.1.3.tar", max compression
```

## Comparing `data_horizon-0.1.2.tar` & `data_horizon-0.1.3.tar`

### file list

```diff
@@ -1,146 +1,145 @@
--rw-r--r--   0        0        0    11426 2024-04-02 09:28:21.174010 data_horizon-0.1.2/LICENSE.txt
--rw-r--r--   0        0        0     2843 2024-04-02 09:28:50.678362 data_horizon-0.1.2/README.rst
--rw-r--r--   0        0        0      530 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/__init__.py
--rw-r--r--   0        0        0     2540 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/__init__.py
--rwxr-xr-x   0        0        0      815 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/__main__.py
--rw-r--r--   0        0        0       99 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/api/__init__.py
--rw-r--r--   0        0        0     4168 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/api/handlers.py
--rw-r--r--   0        0        0      362 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/api/monitoring.py
--rw-r--r--   0        0        0      372 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/api/router.py
--rw-r--r--   0        0        0       99 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/api/v1/__init__.py
--rw-r--r--   0        0        0      997 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/api/v1/router/__init__.py
--rw-r--r--   0        0        0     1252 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/api/v1/router/auth.py
--rw-r--r--   0        0        0     6454 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/api/v1/router/hwm.py
--rw-r--r--   0        0        0      975 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/api/v1/router/hwm_history.py
--rw-r--r--   0        0        0     1029 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/api/v1/router/namespace_history.py
--rw-r--r--   0        0        0     4226 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/api/v1/router/namespaces.py
--rw-r--r--   0        0        0     3650 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/api/v1/router/permission.py
--rw-r--r--   0        0        0      854 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/api/v1/router/users.py
--rw-r--r--   0        0        0     6148 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/db/.DS_Store
--rw-r--r--   0        0        0       99 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/db/__init__.py
--rw-r--r--   0        0        0      669 2024-04-02 09:28:21.178010 data_horizon-0.1.2/horizon/backend/db/factory.py
--rw-r--r--   0        0        0       58 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/README
--rwxr-xr-x   0        0        0      868 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/__main__.py
--rw-r--r--   0        0        0      673 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/alembic.ini
--rw-r--r--   0        0        0     2360 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/env.py
--rw-r--r--   0        0        0      510 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/script.py.mako
--rw-r--r--   0        0        0        0 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/versions/.keep
--rw-r--r--   0        0        0     1498 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/versions/2023-10-09_b91de692624e_.py
--rw-r--r--   0        0        0     1723 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/versions/2023-10-13_e29b66594970_.py
--rw-r--r--   0        0        0     2283 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/versions/2023-10-16_edd2e353ca38_.py
--rw-r--r--   0        0        0     2302 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/versions/2023-10-19_6b9001985cd2_.py
--rw-r--r--   0        0        0     1684 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/versions/2023-11-24_dfce9f35c00e_.py
--rw-r--r--   0        0        0     1375 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/versions/2023-12-23_4bc3fffc0209_.py
--rw-r--r--   0        0        0     1877 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/versions/2024-02-22_c2d6da81f9ec_.py
--rw-r--r--   0        0        0      670 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/versions/2024-02-27_2452f82ae06c_.py
--rw-r--r--   0        0        0     2345 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/versions/2024-02-27_5c7a5c5a193b_.py
--rw-r--r--   0        0        0     1799 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/versions/2024-02-29_09be8fd79dbc_.py
--rw-r--r--   0        0        0     2564 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/versions/2024-03-01_4c60578f3f1d_.py
--rw-r--r--   0        0        0      599 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/migrations/versions/2024-03-18_ec64f7b42221_.py
--rw-r--r--   0        0        0       99 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/mixins/__init__.py
--rw-r--r--   0        0        0     1091 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/mixins/changed_by.py
--rw-r--r--   0        0        0      634 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/mixins/timestamp.py
--rw-r--r--   0        0        0      595 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/models/__init__.py
--rw-r--r--   0        0        0     1044 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/models/base.py
--rw-r--r--   0        0        0     1112 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/models/credentials_cache.py
--rw-r--r--   0        0        0     1380 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/models/hwm.py
--rw-r--r--   0        0        0     1266 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/models/hwm_history.py
--rw-r--r--   0        0        0     1223 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/models/namespace.py
--rw-r--r--   0        0        0     1174 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/models/namespace_history.py
--rw-r--r--   0        0        0      723 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/models/namespace_user.py
--rw-r--r--   0        0        0      758 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/models/user.py
--rw-r--r--   0        0        0      554 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/repositories/__init__.py
--rw-r--r--   0        0        0     3797 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/repositories/base.py
--rw-r--r--   0        0        0      915 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/repositories/credentials_cache.py
--rw-r--r--   0        0        0     5178 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/repositories/hwm.py
--rw-r--r--   0        0        0     1312 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/repositories/hwm_history.py
--rw-r--r--   0        0        0     6275 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/repositories/namespace.py
--rw-r--r--   0        0        0     1102 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/repositories/namespace_history.py
--rw-r--r--   0        0        0     1509 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/db/repositories/user.py
--rw-r--r--   0        0        0      151 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/dependencies/__init__.py
--rw-r--r--   0        0        0     1636 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/dependencies/stub.py
--rwxr-xr-x   0        0        0      482 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/export_openapi_schema.py
--rw-r--r--   0        0        0     1555 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/middlewares/__init__.py
--rw-r--r--   0        0        0     1600 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/middlewares/application_version.py
--rw-r--r--   0        0        0      522 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/middlewares/cors.py
--rw-r--r--   0        0        0      752 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/middlewares/logging.py
--rw-r--r--   0        0        0      303 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/middlewares/monitoring/__init__.py
--rw-r--r--   0        0        0     1337 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/middlewares/monitoring/metrics.py
--rw-r--r--   0        0        0     2912 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/middlewares/monitoring/stats.py
--rw-r--r--   0        0        0     4252 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/middlewares/openapi.py
--rw-r--r--   0        0        0      629 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/middlewares/request_id.py
--rw-r--r--   0        0        0      633 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/middlewares/static_files.py
--rw-r--r--   0        0        0       99 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/providers/__init__.py
--rw-r--r--   0        0        0      160 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/providers/auth/__init__.py
--rw-r--r--   0        0        0     3119 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/providers/auth/base.py
--rw-r--r--   0        0        0     5817 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/providers/auth/cached_ldap.py
--rw-r--r--   0        0        0     3791 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/providers/auth/dummy.py
--rw-r--r--   0        0        0    10594 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/providers/auth/ldap.py
--rwxr-xr-x   0        0        0     3656 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/scripts/manage_admins.py
--rw-r--r--   0        0        0      215 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/services/__init__.py
--rw-r--r--   0        0        0      654 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/services/current_user.py
--rw-r--r--   0        0        0     1241 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/services/uow.py
--rw-r--r--   0        0        0     2136 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/__init__.py
--rw-r--r--   0        0        0     1078 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/auth/__init__.py
--rw-r--r--   0        0        0     2758 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/auth/cached_ldap.py
--rw-r--r--   0        0        0      567 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/auth/dummy.py
--rw-r--r--   0        0        0     1166 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/auth/jwt.py
--rw-r--r--   0        0        0     7103 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/auth/ldap.py
--rw-r--r--   0        0        0     1133 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/database.py
--rw-r--r--   0        0        0     2678 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/server/__init__.py
--rw-r--r--   0        0        0      704 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/server/application_version.py
--rw-r--r--   0        0        0     2102 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/server/cors.py
--rw-r--r--   0        0        0     2862 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/server/log/__init__.py
--rw-r--r--   0        0        0      924 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/server/log/colored.yml
--rw-r--r--   0        0        0      867 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/server/log/json.yml
--rw-r--r--   0        0        0      909 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/server/log/plain.yml
--rw-r--r--   0        0        0     2203 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/server/monitoring.py
--rw-r--r--   0        0        0     4495 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/server/openapi.py
--rw-r--r--   0        0        0     1048 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/server/request_id.py
--rw-r--r--   0        0        0     1025 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/settings/server/static_files.py
--rw-r--r--   0        0        0        0 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/static/.gitkeep
--rw-r--r--   0        0        0       99 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/utils/__init__.py
--rw-r--r--   0        0        0      827 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/utils/jwt.py
--rw-r--r--   0        0        0      343 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/backend/utils/slug.py
--rw-r--r--   0        0        0       99 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/client/__init__.py
--rw-r--r--   0        0        0      335 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/client/auth/__init__.py
--rw-r--r--   0        0        0     1743 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/client/auth/access_token.py
--rw-r--r--   0        0        0      795 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/client/auth/base.py
--rw-r--r--   0        0        0     1381 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/client/auth/login_password.py
--rw-r--r--   0        0        0     6593 2024-04-02 09:28:21.182010 data_horizon-0.1.2/horizon/client/base.py
--rw-r--r--   0        0        0    34597 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/client/sync.py
--rw-r--r--   0        0        0       99 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/__init__.py
--rw-r--r--   0        0        0      244 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/dto/__init__.py
--rw-r--r--   0        0        0     1003 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/dto/pagination.py
--rw-r--r--   0        0        0      583 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/dto/unset.py
--rw-r--r--   0        0        0      480 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/errors/__init__.py
--rw-r--r--   0        0        0      860 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/errors/base.py
--rw-r--r--   0        0        0     2261 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/errors/registration.py
--rw-r--r--   0        0        0      730 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/errors/schemas/__init__.py
--rw-r--r--   0        0        0      982 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/errors/schemas/already_exists.py
--rw-r--r--   0        0        0      525 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/errors/schemas/bad_request.py
--rw-r--r--   0        0        0     1217 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/errors/schemas/invalid_request.py
--rw-r--r--   0        0        0      753 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/errors/schemas/not_authorized.py
--rw-r--r--   0        0        0      939 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/errors/schemas/not_found.py
--rw-r--r--   0        0        0      927 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/errors/schemas/permission_denied.py
--rw-r--r--   0        0        0      724 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/exceptions/__init__.py
--rw-r--r--   0        0        0      832 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/exceptions/auth.py
--rw-r--r--   0        0        0     1016 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/exceptions/bad_request.py
--rw-r--r--   0        0        0      550 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/exceptions/base.py
--rw-r--r--   0        0        0     2346 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/exceptions/entity.py
--rw-r--r--   0        0        0     1300 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/exceptions/permission.py
--rw-r--r--   0        0        0      760 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/exceptions/service.py
--rw-r--r--   0        0        0      189 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/schemas/__init__.py
--rw-r--r--   0        0        0      293 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/schemas/ping.py
--rw-r--r--   0        0        0     1929 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/schemas/v1/__init__.py
--rw-r--r--   0        0        0      305 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/schemas/v1/auth.py
--rw-r--r--   0        0        0     4589 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/schemas/v1/hwm.py
--rw-r--r--   0        0        0     1700 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/schemas/v1/hwm_history.py
--rw-r--r--   0        0        0     2358 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/schemas/v1/namespace.py
--rw-r--r--   0        0        0     1371 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/schemas/v1/namespace_history.py
--rw-r--r--   0        0        0     2174 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/schemas/v1/pagination.py
--rw-r--r--   0        0        0     2209 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/schemas/v1/permission.py
--rw-r--r--   0        0        0      770 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/commons/schemas/v1/user.py
--rw-r--r--   0        0        0        0 2024-04-02 09:28:21.186010 data_horizon-0.1.2/horizon/py.typed
--rw-r--r--   0        0        0    14954 2024-04-02 09:28:21.186010 data_horizon-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     7289 1970-01-01 00:00:00.000000 data_horizon-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11426 2024-05-02 10:58:16.721839 data_horizon-0.1.3/LICENSE.txt
+-rw-r--r--   0        0        0     2843 2024-05-02 10:58:46.689953 data_horizon-0.1.3/README.rst
+-rw-r--r--   0        0        0      530 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/__init__.py
+-rw-r--r--   0        0        0     2540 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/__init__.py
+-rwxr-xr-x   0        0        0      815 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/__main__.py
+-rw-r--r--   0        0        0       99 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/api/__init__.py
+-rw-r--r--   0        0        0     4168 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/api/handlers.py
+-rw-r--r--   0        0        0      362 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/api/monitoring.py
+-rw-r--r--   0        0        0      372 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/api/router.py
+-rw-r--r--   0        0        0       99 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/api/v1/__init__.py
+-rw-r--r--   0        0        0      997 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/api/v1/router/__init__.py
+-rw-r--r--   0        0        0     1252 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/api/v1/router/auth.py
+-rw-r--r--   0        0        0     6454 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/api/v1/router/hwm.py
+-rw-r--r--   0        0        0      975 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/api/v1/router/hwm_history.py
+-rw-r--r--   0        0        0     1029 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/api/v1/router/namespace_history.py
+-rw-r--r--   0        0        0     4226 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/api/v1/router/namespaces.py
+-rw-r--r--   0        0        0     3650 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/api/v1/router/permission.py
+-rw-r--r--   0        0        0      854 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/api/v1/router/users.py
+-rw-r--r--   0        0        0       99 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/__init__.py
+-rw-r--r--   0        0        0      669 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/factory.py
+-rw-r--r--   0        0        0       58 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/README
+-rwxr-xr-x   0        0        0      868 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/__main__.py
+-rw-r--r--   0        0        0      673 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/alembic.ini
+-rw-r--r--   0        0        0     2360 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/env.py
+-rw-r--r--   0        0        0      510 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/script.py.mako
+-rw-r--r--   0        0        0        0 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/versions/.keep
+-rw-r--r--   0        0        0     1498 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/versions/2023-10-09_b91de692624e_.py
+-rw-r--r--   0        0        0     1723 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/versions/2023-10-13_e29b66594970_.py
+-rw-r--r--   0        0        0     2283 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/versions/2023-10-16_edd2e353ca38_.py
+-rw-r--r--   0        0        0     2302 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/versions/2023-10-19_6b9001985cd2_.py
+-rw-r--r--   0        0        0     1684 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/versions/2023-11-24_dfce9f35c00e_.py
+-rw-r--r--   0        0        0     1375 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/versions/2023-12-23_4bc3fffc0209_.py
+-rw-r--r--   0        0        0     1877 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/versions/2024-02-22_c2d6da81f9ec_.py
+-rw-r--r--   0        0        0      670 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/versions/2024-02-27_2452f82ae06c_.py
+-rw-r--r--   0        0        0     2345 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/versions/2024-02-27_5c7a5c5a193b_.py
+-rw-r--r--   0        0        0     1799 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/versions/2024-02-29_09be8fd79dbc_.py
+-rw-r--r--   0        0        0     2564 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/versions/2024-03-01_4c60578f3f1d_.py
+-rw-r--r--   0        0        0      599 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/migrations/versions/2024-03-18_ec64f7b42221_.py
+-rw-r--r--   0        0        0       99 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/mixins/__init__.py
+-rw-r--r--   0        0        0     1091 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/mixins/changed_by.py
+-rw-r--r--   0        0        0      634 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/mixins/timestamp.py
+-rw-r--r--   0        0        0      595 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/models/__init__.py
+-rw-r--r--   0        0        0     1044 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/models/base.py
+-rw-r--r--   0        0        0     1112 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/models/credentials_cache.py
+-rw-r--r--   0        0        0     1380 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/models/hwm.py
+-rw-r--r--   0        0        0     1266 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/models/hwm_history.py
+-rw-r--r--   0        0        0     1223 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/models/namespace.py
+-rw-r--r--   0        0        0     1174 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/models/namespace_history.py
+-rw-r--r--   0        0        0      723 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/models/namespace_user.py
+-rw-r--r--   0        0        0      758 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/models/user.py
+-rw-r--r--   0        0        0      554 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/repositories/__init__.py
+-rw-r--r--   0        0        0     3797 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/repositories/base.py
+-rw-r--r--   0        0        0      915 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/repositories/credentials_cache.py
+-rw-r--r--   0        0        0     5178 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/repositories/hwm.py
+-rw-r--r--   0        0        0     1312 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/repositories/hwm_history.py
+-rw-r--r--   0        0        0     6275 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/repositories/namespace.py
+-rw-r--r--   0        0        0     1102 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/repositories/namespace_history.py
+-rw-r--r--   0        0        0     1509 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/db/repositories/user.py
+-rw-r--r--   0        0        0      151 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/dependencies/__init__.py
+-rw-r--r--   0        0        0     1636 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/dependencies/stub.py
+-rwxr-xr-x   0        0        0      482 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/export_openapi_schema.py
+-rw-r--r--   0        0        0     1555 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/middlewares/__init__.py
+-rw-r--r--   0        0        0     1600 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/middlewares/application_version.py
+-rw-r--r--   0        0        0      522 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/middlewares/cors.py
+-rw-r--r--   0        0        0      752 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/middlewares/logging.py
+-rw-r--r--   0        0        0      303 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/middlewares/monitoring/__init__.py
+-rw-r--r--   0        0        0     1337 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/middlewares/monitoring/metrics.py
+-rw-r--r--   0        0        0     2912 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/middlewares/monitoring/stats.py
+-rw-r--r--   0        0        0     4252 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/middlewares/openapi.py
+-rw-r--r--   0        0        0      629 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/middlewares/request_id.py
+-rw-r--r--   0        0        0      633 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/middlewares/static_files.py
+-rw-r--r--   0        0        0       99 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/providers/__init__.py
+-rw-r--r--   0        0        0      160 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/providers/auth/__init__.py
+-rw-r--r--   0        0        0     3119 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/providers/auth/base.py
+-rw-r--r--   0        0        0     5817 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/providers/auth/cached_ldap.py
+-rw-r--r--   0        0        0     3791 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/providers/auth/dummy.py
+-rw-r--r--   0        0        0    10170 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/providers/auth/ldap.py
+-rwxr-xr-x   0        0        0     3656 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/scripts/manage_admins.py
+-rw-r--r--   0        0        0      215 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/services/__init__.py
+-rw-r--r--   0        0        0      654 2024-05-02 10:58:16.729839 data_horizon-0.1.3/horizon/backend/services/current_user.py
+-rw-r--r--   0        0        0     1241 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/services/uow.py
+-rw-r--r--   0        0        0     2136 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/__init__.py
+-rw-r--r--   0        0        0     1078 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/auth/__init__.py
+-rw-r--r--   0        0        0     2758 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/auth/cached_ldap.py
+-rw-r--r--   0        0        0      567 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/auth/dummy.py
+-rw-r--r--   0        0        0     1166 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/auth/jwt.py
+-rw-r--r--   0        0        0     7103 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/auth/ldap.py
+-rw-r--r--   0        0        0     1133 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/database.py
+-rw-r--r--   0        0        0     2678 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/server/__init__.py
+-rw-r--r--   0        0        0      704 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/server/application_version.py
+-rw-r--r--   0        0        0     2102 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/server/cors.py
+-rw-r--r--   0        0        0     2862 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/server/log/__init__.py
+-rw-r--r--   0        0        0      924 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/server/log/colored.yml
+-rw-r--r--   0        0        0      867 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/server/log/json.yml
+-rw-r--r--   0        0        0      909 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/server/log/plain.yml
+-rw-r--r--   0        0        0     2203 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/server/monitoring.py
+-rw-r--r--   0        0        0     4345 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/server/openapi.py
+-rw-r--r--   0        0        0     1048 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/server/request_id.py
+-rw-r--r--   0        0        0     1025 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/settings/server/static_files.py
+-rw-r--r--   0        0        0        0 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/static/.gitkeep
+-rw-r--r--   0        0        0       99 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/utils/__init__.py
+-rw-r--r--   0        0        0      827 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/utils/jwt.py
+-rw-r--r--   0        0        0      343 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/backend/utils/slug.py
+-rw-r--r--   0        0        0       99 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/client/__init__.py
+-rw-r--r--   0        0        0      335 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/client/auth/__init__.py
+-rw-r--r--   0        0        0     1743 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/client/auth/access_token.py
+-rw-r--r--   0        0        0      795 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/client/auth/base.py
+-rw-r--r--   0        0        0     1381 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/client/auth/login_password.py
+-rw-r--r--   0        0        0     6593 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/client/base.py
+-rw-r--r--   0        0        0    34597 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/client/sync.py
+-rw-r--r--   0        0        0       99 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/__init__.py
+-rw-r--r--   0        0        0      244 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/dto/__init__.py
+-rw-r--r--   0        0        0     1003 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/dto/pagination.py
+-rw-r--r--   0        0        0      583 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/dto/unset.py
+-rw-r--r--   0        0        0      480 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/errors/__init__.py
+-rw-r--r--   0        0        0      860 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/errors/base.py
+-rw-r--r--   0        0        0     2261 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/errors/registration.py
+-rw-r--r--   0        0        0      730 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/errors/schemas/__init__.py
+-rw-r--r--   0        0        0      982 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/errors/schemas/already_exists.py
+-rw-r--r--   0        0        0      525 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/errors/schemas/bad_request.py
+-rw-r--r--   0        0        0     1200 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/errors/schemas/invalid_request.py
+-rw-r--r--   0        0        0      753 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/errors/schemas/not_authorized.py
+-rw-r--r--   0        0        0      939 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/errors/schemas/not_found.py
+-rw-r--r--   0        0        0      927 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/errors/schemas/permission_denied.py
+-rw-r--r--   0        0        0      724 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/exceptions/__init__.py
+-rw-r--r--   0        0        0      832 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/exceptions/auth.py
+-rw-r--r--   0        0        0     1016 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/exceptions/bad_request.py
+-rw-r--r--   0        0        0      550 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/exceptions/base.py
+-rw-r--r--   0        0        0     2346 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/exceptions/entity.py
+-rw-r--r--   0        0        0     1300 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/exceptions/permission.py
+-rw-r--r--   0        0        0      760 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/exceptions/service.py
+-rw-r--r--   0        0        0      189 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/schemas/__init__.py
+-rw-r--r--   0        0        0      293 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/schemas/ping.py
+-rw-r--r--   0        0        0     1929 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/schemas/v1/__init__.py
+-rw-r--r--   0        0        0      305 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/schemas/v1/auth.py
+-rw-r--r--   0        0        0     4589 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/schemas/v1/hwm.py
+-rw-r--r--   0        0        0     1700 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/schemas/v1/hwm_history.py
+-rw-r--r--   0        0        0     2358 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/schemas/v1/namespace.py
+-rw-r--r--   0        0        0     1371 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/schemas/v1/namespace_history.py
+-rw-r--r--   0        0        0     2174 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/schemas/v1/pagination.py
+-rw-r--r--   0        0        0     2209 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/schemas/v1/permission.py
+-rw-r--r--   0        0        0      770 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/commons/schemas/v1/user.py
+-rw-r--r--   0        0        0        0 2024-05-02 10:58:16.733839 data_horizon-0.1.3/horizon/py.typed
+-rw-r--r--   0        0        0    15137 2024-05-02 10:58:16.737839 data_horizon-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     7390 1970-01-01 00:00:00.000000 data_horizon-0.1.3/PKG-INFO
```

### Comparing `data_horizon-0.1.2/LICENSE.txt` & `data_horizon-0.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/README.rst` & `data_horizon-0.1.3/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     :target: https://codecov.io/gh/MobileTeleSystems/horizon
 .. |pre-commit.ci| image:: https://results.pre-commit.ci/badge/github/MobileTeleSystems/horizon/develop.svg
     :target: https://results.pre-commit.ci/latest/github/MobileTeleSystems/horizon/develop
 
 
 |Logo|
 
-.. |Logo| image:: https://raw.githubusercontent.com/MobileTeleSystems/horizon/8367012cc94e07439ad04cac1fa30644b0567934/docs/_static/logo.svg
+.. |Logo| image:: https://raw.githubusercontent.com/MobileTeleSystems/horizon/9dfa8bf2b8acf18c1ba8e78f0b48e868a59694fe/docs/_static/logo.svg
     :width: 400
     :alt: Horizon logo
     :target: https://github.com/MobileTeleSystems/horizon/
 
 What is Horizon?
 ----------------
```

### Comparing `data_horizon-0.1.2/horizon/__init__.py` & `data_horizon-0.1.3/horizon/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # SPDX-FileCopyrightText: 2023-2024 MTS (Mobile Telesystems)
 # SPDX-License-Identifier: Apache-2.0
 
 # _raw_version could contain pre-release version, like 0.0.1dev123
 # value is updated automatically by `poetry version ...` and poetry-bumpversion plugin
-_raw_version = "0.1.2"
+_raw_version = "0.1.3"
 
 # version always contain only release number like 0.0.1
 __version__ = ".".join(_raw_version.split(".")[:3])  # noqa: WPS410
 
 # version tuple always contains only integer parts, like (0, 0, 1)
 __version_tuple__ = tuple(map(int, __version__.split(".")))
```

### Comparing `data_horizon-0.1.2/horizon/backend/__init__.py` & `data_horizon-0.1.3/horizon/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/__main__.py` & `data_horizon-0.1.3/horizon/backend/__main__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/api/handlers.py` & `data_horizon-0.1.3/horizon/backend/api/handlers.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/api/v1/router/__init__.py` & `data_horizon-0.1.3/horizon/backend/api/v1/router/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/api/v1/router/auth.py` & `data_horizon-0.1.3/horizon/backend/api/v1/router/auth.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/api/v1/router/hwm.py` & `data_horizon-0.1.3/horizon/backend/api/v1/router/hwm.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/api/v1/router/hwm_history.py` & `data_horizon-0.1.3/horizon/backend/api/v1/router/hwm_history.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/api/v1/router/namespace_history.py` & `data_horizon-0.1.3/horizon/backend/api/v1/router/namespace_history.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/api/v1/router/namespaces.py` & `data_horizon-0.1.3/horizon/backend/api/v1/router/namespaces.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/api/v1/router/permission.py` & `data_horizon-0.1.3/horizon/backend/api/v1/router/permission.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/api/v1/router/users.py` & `data_horizon-0.1.3/horizon/backend/api/v1/router/users.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/factory.py` & `data_horizon-0.1.3/horizon/backend/db/factory.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/migrations/__main__.py` & `data_horizon-0.1.3/horizon/backend/db/migrations/__main__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/migrations/alembic.ini` & `data_horizon-0.1.3/horizon/backend/db/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/migrations/env.py` & `data_horizon-0.1.3/horizon/backend/db/migrations/env.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/migrations/versions/2023-10-09_b91de692624e_.py` & `data_horizon-0.1.3/horizon/backend/db/migrations/versions/2023-10-09_b91de692624e_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/migrations/versions/2023-10-13_e29b66594970_.py` & `data_horizon-0.1.3/horizon/backend/db/migrations/versions/2023-10-13_e29b66594970_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/migrations/versions/2023-10-16_edd2e353ca38_.py` & `data_horizon-0.1.3/horizon/backend/db/migrations/versions/2023-10-16_edd2e353ca38_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/migrations/versions/2023-10-19_6b9001985cd2_.py` & `data_horizon-0.1.3/horizon/backend/db/migrations/versions/2023-10-19_6b9001985cd2_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/migrations/versions/2023-11-24_dfce9f35c00e_.py` & `data_horizon-0.1.3/horizon/backend/db/migrations/versions/2023-11-24_dfce9f35c00e_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/migrations/versions/2023-12-23_4bc3fffc0209_.py` & `data_horizon-0.1.3/horizon/backend/db/migrations/versions/2023-12-23_4bc3fffc0209_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/migrations/versions/2024-02-22_c2d6da81f9ec_.py` & `data_horizon-0.1.3/horizon/backend/db/migrations/versions/2024-02-22_c2d6da81f9ec_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/migrations/versions/2024-02-27_2452f82ae06c_.py` & `data_horizon-0.1.3/horizon/backend/db/migrations/versions/2024-02-27_2452f82ae06c_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/migrations/versions/2024-02-27_5c7a5c5a193b_.py` & `data_horizon-0.1.3/horizon/backend/db/migrations/versions/2024-02-27_5c7a5c5a193b_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/migrations/versions/2024-02-29_09be8fd79dbc_.py` & `data_horizon-0.1.3/horizon/backend/db/migrations/versions/2024-02-29_09be8fd79dbc_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/migrations/versions/2024-03-01_4c60578f3f1d_.py` & `data_horizon-0.1.3/horizon/backend/db/migrations/versions/2024-03-01_4c60578f3f1d_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/migrations/versions/2024-03-18_ec64f7b42221_.py` & `data_horizon-0.1.3/horizon/backend/db/migrations/versions/2024-03-18_ec64f7b42221_.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/mixins/changed_by.py` & `data_horizon-0.1.3/horizon/backend/db/mixins/changed_by.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/mixins/timestamp.py` & `data_horizon-0.1.3/horizon/backend/db/mixins/timestamp.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/models/__init__.py` & `data_horizon-0.1.3/horizon/backend/db/models/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/models/base.py` & `data_horizon-0.1.3/horizon/backend/db/models/base.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/models/credentials_cache.py` & `data_horizon-0.1.3/horizon/backend/db/models/credentials_cache.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/models/hwm.py` & `data_horizon-0.1.3/horizon/backend/db/models/hwm.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/models/hwm_history.py` & `data_horizon-0.1.3/horizon/backend/db/models/hwm_history.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/models/namespace.py` & `data_horizon-0.1.3/horizon/backend/db/models/namespace.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/models/namespace_history.py` & `data_horizon-0.1.3/horizon/backend/db/models/namespace_history.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/models/namespace_user.py` & `data_horizon-0.1.3/horizon/backend/db/models/namespace_user.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/models/user.py` & `data_horizon-0.1.3/horizon/backend/db/models/user.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/repositories/__init__.py` & `data_horizon-0.1.3/horizon/backend/db/repositories/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/repositories/base.py` & `data_horizon-0.1.3/horizon/backend/db/repositories/base.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/repositories/credentials_cache.py` & `data_horizon-0.1.3/horizon/backend/db/repositories/credentials_cache.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/repositories/hwm.py` & `data_horizon-0.1.3/horizon/backend/db/repositories/hwm.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/repositories/hwm_history.py` & `data_horizon-0.1.3/horizon/backend/db/repositories/hwm_history.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/repositories/namespace.py` & `data_horizon-0.1.3/horizon/backend/db/repositories/namespace.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/repositories/namespace_history.py` & `data_horizon-0.1.3/horizon/backend/db/repositories/namespace_history.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/db/repositories/user.py` & `data_horizon-0.1.3/horizon/backend/db/repositories/user.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/dependencies/stub.py` & `data_horizon-0.1.3/horizon/backend/dependencies/stub.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/middlewares/__init__.py` & `data_horizon-0.1.3/horizon/backend/middlewares/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/middlewares/application_version.py` & `data_horizon-0.1.3/horizon/backend/middlewares/application_version.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/middlewares/cors.py` & `data_horizon-0.1.3/horizon/backend/middlewares/cors.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/middlewares/logging.py` & `data_horizon-0.1.3/horizon/backend/middlewares/logging.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/middlewares/monitoring/metrics.py` & `data_horizon-0.1.3/horizon/backend/middlewares/monitoring/metrics.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/middlewares/monitoring/stats.py` & `data_horizon-0.1.3/horizon/backend/middlewares/monitoring/stats.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/middlewares/openapi.py` & `data_horizon-0.1.3/horizon/backend/middlewares/openapi.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/middlewares/request_id.py` & `data_horizon-0.1.3/horizon/backend/middlewares/request_id.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/middlewares/static_files.py` & `data_horizon-0.1.3/horizon/backend/middlewares/static_files.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/providers/auth/base.py` & `data_horizon-0.1.3/horizon/backend/providers/auth/base.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/providers/auth/cached_ldap.py` & `data_horizon-0.1.3/horizon/backend/providers/auth/cached_ldap.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/providers/auth/dummy.py` & `data_horizon-0.1.3/horizon/backend/providers/auth/dummy.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/providers/auth/ldap.py` & `data_horizon-0.1.3/horizon/backend/providers/auth/ldap.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 Similar to:
 * `JupyterHub LDAPAuthenticator <https://github.com/jupyterhub/ldapauthenticator>`_
 * `Flask-AppBuilder LDAP integration <https://github.com/dpgaspar/Flask-AppBuilder/blob/master/docs/config.rst>`_, used in Apache Airflow
 """
 
 import logging
-from contextlib import asynccontextmanager, suppress
+from contextlib import asynccontextmanager
 from time import time
 from typing import Any, AsyncContextManager, AsyncGenerator, Dict, List, Optional, Tuple
 
 from bonsai import InvalidDN, LDAPClient
 from bonsai.asyncio import AIOConnectionPool, AIOLDAPConnection
 from bonsai.errors import AuthenticationError, LDAPError
 from devtools import pformat
@@ -151,23 +151,18 @@
                 log.debug("Creating non-pooled connection for lookup")
                 client = self._get_lookup_client(self._auth_settings)
                 connect = client.connect(is_async=True, timeout=self._auth_settings.ldap.timeout_seconds)
 
             async with connect as connection:
                 try:  # noqa: WPS505
                     yield connection
-                except LDAPError as err:
-                    # Explicitly closing connection to avoid returning broken connection to a pool.
-                    # Also do that twice to avoid partially closing connection,
-                    # See https://github.com/noirello/bonsai/issues/87
-                    with suppress(LDAPError):
-                        connection.close()  # noqa: WPS220
-                    with suppress(LDAPError):
-                        connection.close()  # noqa: WPS220
-                    raise ServiceError("Failed to connect to LDAP") from err
+                except LDAPError:
+                    # avoid returning connection back to the pool
+                    connection.close()
+                    raise
 
         except LDAPError as e:
             raise ServiceError("Failed to connect to LDAP") from e
 
     async def _resolve_username_from_ldap(self, login: str, password: str) -> str:
         log.info("Resolve user %r in LDAP", login)
         username = login
```

### Comparing `data_horizon-0.1.2/horizon/backend/scripts/manage_admins.py` & `data_horizon-0.1.3/horizon/backend/scripts/manage_admins.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/services/current_user.py` & `data_horizon-0.1.3/horizon/backend/services/current_user.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/services/uow.py` & `data_horizon-0.1.3/horizon/backend/services/uow.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/settings/__init__.py` & `data_horizon-0.1.3/horizon/backend/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/settings/auth/__init__.py` & `data_horizon-0.1.3/horizon/backend/settings/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/settings/auth/cached_ldap.py` & `data_horizon-0.1.3/horizon/backend/settings/auth/cached_ldap.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/settings/auth/dummy.py` & `data_horizon-0.1.3/horizon/backend/settings/auth/dummy.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/settings/auth/jwt.py` & `data_horizon-0.1.3/horizon/backend/settings/auth/jwt.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/settings/auth/ldap.py` & `data_horizon-0.1.3/horizon/backend/settings/auth/ldap.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/settings/database.py` & `data_horizon-0.1.3/horizon/backend/settings/database.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/settings/server/__init__.py` & `data_horizon-0.1.3/horizon/backend/settings/server/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/settings/server/application_version.py` & `data_horizon-0.1.3/horizon/backend/settings/server/application_version.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/settings/server/cors.py` & `data_horizon-0.1.3/horizon/backend/settings/server/cors.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/settings/server/log/__init__.py` & `data_horizon-0.1.3/horizon/backend/settings/server/log/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/settings/server/log/colored.yml` & `data_horizon-0.1.3/horizon/backend/settings/server/log/colored.yml`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/settings/server/log/json.yml` & `data_horizon-0.1.3/horizon/backend/settings/server/log/json.yml`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/settings/server/log/plain.yml` & `data_horizon-0.1.3/horizon/backend/settings/server/log/plain.yml`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/settings/server/monitoring.py` & `data_horizon-0.1.3/horizon/backend/settings/server/monitoring.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/settings/server/openapi.py` & `data_horizon-0.1.3/horizon/backend/settings/server/openapi.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
     Examples
     --------
 
     .. code-block:: bash
 
         HORIZON__SERVER__OPENAPI__SWAGGER__ENABLED=True
-        HORIZON__SERVER__OPENAPI__SWAGGER__JS_URL=/app/horizon/backend/static/swagger/swagger-ui-bundle.js
-        HORIZON__SERVER__OPENAPI__SWAGGER__CSS_URL=/app/horizon/backend/static/swagger/swagger-ui.css
+        HORIZON__SERVER__OPENAPI__SWAGGER__JS_URL=/static/swagger/swagger-ui-bundle.js
+        HORIZON__SERVER__OPENAPI__SWAGGER__CSS_URL=/static/swagger/swagger-ui.css
     """
 
     enabled: bool = Field(default=True, description="Set to ``True`` to enable Swagger UI endpoint")
     js_url: str = Field(
         default="https://cdn.jsdelivr.net/npm/swagger-ui-dist@5/swagger-ui-bundle.js",
         description="URL for Swagger UI JS",
     )
@@ -49,16 +49,15 @@
 
     Examples
     --------
 
     .. code-block:: bash
 
         HORIZON__SERVER__OPENAPI__REDOC__ENABLED=True
-        HORIZON__SERVER__OPENAPI__REDOC__JS_URL=/app/horizon/backend/static/redoc/redoc.standalone.js
-        HORIZON__SERVER__OPENAPI__REDOC__FAVICON_URL=/app/horizon/backend/static/icon.svg
+        HORIZON__SERVER__OPENAPI__REDOC__JS_URL=/static/redoc/redoc.standalone.js
     """
 
     enabled: bool = Field(default=True, description="Set to ``True`` to enable Redoc UI endpoint")
     js_url: str = Field(
         default="https://cdn.jsdelivr.net/npm/redoc@next/bundles/redoc.standalone.js",
         description="URL for Redoc UI JS, ``None`` to use default CDN URL",
     )
```

### Comparing `data_horizon-0.1.2/horizon/backend/settings/server/request_id.py` & `data_horizon-0.1.3/horizon/backend/settings/server/request_id.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/settings/server/static_files.py` & `data_horizon-0.1.3/horizon/backend/settings/server/static_files.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/backend/utils/jwt.py` & `data_horizon-0.1.3/horizon/backend/utils/jwt.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/client/auth/access_token.py` & `data_horizon-0.1.3/horizon/client/auth/access_token.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/client/auth/base.py` & `data_horizon-0.1.3/horizon/client/auth/base.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/client/auth/login_password.py` & `data_horizon-0.1.3/horizon/client/auth/login_password.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/client/base.py` & `data_horizon-0.1.3/horizon/client/base.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/client/sync.py` & `data_horizon-0.1.3/horizon/client/sync.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/commons/dto/pagination.py` & `data_horizon-0.1.3/horizon/commons/dto/pagination.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/commons/dto/unset.py` & `data_horizon-0.1.3/horizon/commons/dto/unset.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/commons/errors/base.py` & `data_horizon-0.1.3/horizon/commons/errors/base.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/commons/errors/registration.py` & `data_horizon-0.1.3/horizon/commons/errors/registration.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/commons/errors/schemas/__init__.py` & `data_horizon-0.1.3/horizon/commons/errors/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/commons/errors/schemas/already_exists.py` & `data_horizon-0.1.3/horizon/commons/errors/schemas/already_exists.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/commons/errors/schemas/bad_request.py` & `data_horizon-0.1.3/horizon/commons/errors/schemas/bad_request.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/commons/errors/schemas/invalid_request.py` & `data_horizon-0.1.3/horizon/commons/errors/schemas/invalid_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 class InvalidRequestBaseErrorSchema(BaseModel):
     loc: List[str] = Field(alias="location")
     msg: str = Field(alias="message")
     type: str = Field(alias="code")
 
     if pydantic_version >= "2":
-        url: str
         ctx: dict = Field(default_factory=dict, alias="context")
         input: Any = Field(default=None)
 
     class Config:
         if pydantic_version >= "2":
             populate_by_name = True
         else:
```

### Comparing `data_horizon-0.1.2/horizon/commons/errors/schemas/not_authorized.py` & `data_horizon-0.1.3/horizon/commons/errors/schemas/not_authorized.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/commons/errors/schemas/not_found.py` & `data_horizon-0.1.3/horizon/commons/errors/schemas/not_found.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/commons/errors/schemas/permission_denied.py` & `data_horizon-0.1.3/horizon/commons/errors/schemas/permission_denied.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/commons/exceptions/__init__.py` & `data_horizon-0.1.3/horizon/commons/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/commons/exceptions/auth.py` & `data_horizon-0.1.3/horizon/commons/exceptions/auth.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/commons/exceptions/bad_request.py` & `data_horizon-0.1.3/horizon/commons/exceptions/bad_request.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/commons/exceptions/base.py` & `data_horizon-0.1.3/horizon/commons/exceptions/base.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/commons/exceptions/entity.py` & `data_horizon-0.1.3/horizon/commons/exceptions/entity.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/commons/exceptions/permission.py` & `data_horizon-0.1.3/horizon/commons/exceptions/permission.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/commons/exceptions/service.py` & `data_horizon-0.1.3/horizon/commons/exceptions/service.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/commons/schemas/v1/__init__.py` & `data_horizon-0.1.3/horizon/commons/schemas/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/commons/schemas/v1/hwm.py` & `data_horizon-0.1.3/horizon/commons/schemas/v1/hwm.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/commons/schemas/v1/hwm_history.py` & `data_horizon-0.1.3/horizon/commons/schemas/v1/hwm_history.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/commons/schemas/v1/namespace.py` & `data_horizon-0.1.3/horizon/commons/schemas/v1/namespace.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/commons/schemas/v1/namespace_history.py` & `data_horizon-0.1.3/horizon/commons/schemas/v1/namespace_history.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/commons/schemas/v1/pagination.py` & `data_horizon-0.1.3/horizon/commons/schemas/v1/pagination.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/commons/schemas/v1/permission.py` & `data_horizon-0.1.3/horizon/commons/schemas/v1/permission.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/horizon/commons/schemas/v1/user.py` & `data_horizon-0.1.3/horizon/commons/schemas/v1/user.py`

 * *Files identical despite different names*

### Comparing `data_horizon-0.1.2/pyproject.toml` & `data_horizon-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "data-horizon"
-version = "0.1.2"
+version = "0.1.3"
 license = "Apache-2.0"
 description = "Horizon REST API + client"
 authors = ["DataOps.ETL <onetools@mts.ru>"]
 readme = "README.rst"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Framework :: Pydantic",
@@ -44,15 +44,18 @@
 "Documentation" = "https://data-horizon.readthedocs.io/"
 "Source" = "https://github.com/MobileTeleSystems/horizon"
 "CI/CD" = "https://github.com/MobileTeleSystems/horizon/actions"
 "Tracker" = "https://github.com/MobileTeleSystems/horizon/issues"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-pydantic = "<3"
+pydantic = [
+  {version = "<2.6.0", python = "<3.8"},
+  {version = "<3", python = ">=3.8"},
+]
 typing-extensions = [
   {version = ">=4.0.0,<4.8.0", python = "<3.8"},
   {version = ">=4.0.0", python = ">=3.8"},
 ]
 python-jose = {version = "*", extras=["cryptography"]}
 fastapi = [
   {version = "^0.103.2", optional = true, python = "<3.8"},
@@ -90,15 +93,15 @@
 python-multipart = {version = "*", optional = true}
 sqlalchemy-utils = {version = "*", optional = true}
 authlib = [
   {version = "^1.2.1", optional = true, python = "<3.8"},
   {version = ">=1.2.1", optional = true, python = ">=3.8"},
 ]
 requests = {version = "*", optional = true}
-bonsai = {version = "*", optional = true}
+bonsai = {version = "^1.5.3", optional = true}
 python-json-logger = {version = "*", optional = true}
 coloredlogs = {version = "*", optional = true}
 pyyaml = {version = "*", optional = true}
 asgi-correlation-id = [
   {version = "^4.2.0", optional = true, python = "<3.8"},
   {version = ">=4.2.0", optional = true, python = ">=3.8"},
 ]
@@ -146,15 +149,16 @@
 pytest = "^7.4.4"
 httpx = [
   {version = "^0.24.1", python = "<3.8"},
   {version = "^0.26.0", python = ">=3.8"},
 ]
 pytest-asyncio = [
   {version = "^0.21.1", python = "<3.8"},
-  {version = "^0.23.3", python = ">=3.8"},
+  # TODO: remove version limit after fixing https://github.com/pytest-dev/pytest-asyncio/issues/706
+  {version = "^0.21.1", python = ">=3.8"},
 ]
 pytest-randomly = [
   {version = "^3.12.0", python = "<3.8"},
   {version = "^3.15.0", python = ">=3.8"},
 ]
 pytest-deadfixtures = "^2.2.1"
 pytest-rerunfailures = "^13.0"
```

### Comparing `data_horizon-0.1.2/PKG-INFO` & `data_horizon-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-horizon
-Version: 0.1.2
+Version: 0.1.3
 Summary: Horizon REST API + client
 License: Apache-2.0
 Keywords: Horizon,REST,API,HWM
 Author: DataOps.ETL
 Author-email: onetools@mts.ru
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -35,23 +35,24 @@
 Requires-Dist: argon2-cffi ; extra == "ldap"
 Requires-Dist: asgi-correlation-id (>=4.2.0) ; (python_version >= "3.8") and (extra == "backend")
 Requires-Dist: asgi-correlation-id (>=4.2.0,<5.0.0) ; (python_version < "3.8") and (extra == "backend")
 Requires-Dist: asyncpg (>=0.28.0) ; (python_version >= "3.8") and (extra == "postgres")
 Requires-Dist: asyncpg (>=0.28.0,<0.29.0) ; (python_version < "3.8") and (extra == "postgres")
 Requires-Dist: authlib (>=1.2.1) ; (python_version >= "3.8") and (extra == "client-sync")
 Requires-Dist: authlib (>=1.2.1,<2.0.0) ; (python_version < "3.8") and (extra == "client-sync")
-Requires-Dist: bonsai ; extra == "ldap"
+Requires-Dist: bonsai (>=1.5.3,<2.0.0) ; extra == "ldap"
 Requires-Dist: coloredlogs ; extra == "backend"
 Requires-Dist: devtools ; extra == "backend"
 Requires-Dist: fastapi (>=0.103.0) ; (python_version >= "3.8") and (extra == "backend")
 Requires-Dist: fastapi (>=0.103.2,<0.104.0) ; (python_version < "3.8") and (extra == "backend")
 Requires-Dist: importlib-resources (>=5.12.0) ; (python_version >= "3.8") and (extra == "backend")
 Requires-Dist: importlib-resources (>=5.12.0,<6.0.0) ; (python_version < "3.8") and (extra == "backend")
 Requires-Dist: passlib ; extra == "backend"
-Requires-Dist: pydantic (<3)
+Requires-Dist: pydantic (<2.6.0) ; python_version < "3.8"
+Requires-Dist: pydantic (<3) ; python_version >= "3.8"
 Requires-Dist: pydantic-settings (>=2.0.3) ; (python_version >= "3.8") and (extra == "backend")
 Requires-Dist: pydantic-settings (>=2.0.3,<3.0.0) ; (python_version < "3.8") and (extra == "backend")
 Requires-Dist: python-jose[cryptography]
 Requires-Dist: python-json-logger ; extra == "backend"
 Requires-Dist: python-multipart ; extra == "backend"
 Requires-Dist: pyyaml ; extra == "backend"
 Requires-Dist: requests ; extra == "client-sync"
@@ -100,15 +101,15 @@
     :target: https://codecov.io/gh/MobileTeleSystems/horizon
 .. |pre-commit.ci| image:: https://results.pre-commit.ci/badge/github/MobileTeleSystems/horizon/develop.svg
     :target: https://results.pre-commit.ci/latest/github/MobileTeleSystems/horizon/develop
 
 
 |Logo|
 
-.. |Logo| image:: https://raw.githubusercontent.com/MobileTeleSystems/horizon/8367012cc94e07439ad04cac1fa30644b0567934/docs/_static/logo.svg
+.. |Logo| image:: https://raw.githubusercontent.com/MobileTeleSystems/horizon/9dfa8bf2b8acf18c1ba8e78f0b48e868a59694fe/docs/_static/logo.svg
     :width: 400
     :alt: Horizon logo
     :target: https://github.com/MobileTeleSystems/horizon/
 
 What is Horizon?
 ----------------
```

