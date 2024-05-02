# Comparing `tmp/fastapi_xroad_soap-0.4.2.tar.gz` & `tmp/fastapi_xroad_soap-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_xroad_soap-0.4.2.tar", max compression
+gzip compressed data, was "fastapi_xroad_soap-0.4.3.tar", max compression
```

## Comparing `fastapi_xroad_soap-0.4.2.tar` & `fastapi_xroad_soap-0.4.3.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0    13831 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/LICENSE
--rw-r--r--   0        0        0     6684 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/README.md
--rw-r--r--   0        0        0      524 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/__init__.py
--rw-r--r--   0        0        0      574 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/elements.py
--rw-r--r--   0        0        0      431 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/faults.py
--rw-r--r--   0        0        0      340 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/__init__.py
--rw-r--r--   0        0        0      666 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/base/__init__.py
--rw-r--r--   0        0        0     2953 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/base/base_element_spec.py
--rw-r--r--   0        0        0     1194 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/base/composite_meta.py
--rw-r--r--   0        0        0      988 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/base/dynamic_spec.py
--rw-r--r--   0        0        0     4392 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/base/message_body.py
--rw-r--r--   0        0        0     2705 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/base/validators.py
--rw-r--r--   0        0        0     1067 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/constants.py
--rw-r--r--   0        0        0      486 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/elements/__init__.py
--rw-r--r--   0        0        0     1061 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/elements/models/__init__.py
--rw-r--r--   0        0        0     1479 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/elements/models/boolean.py
--rw-r--r--   0        0        0     1195 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/elements/models/date.py
--rw-r--r--   0        0        0     1243 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/elements/models/datetime.py
--rw-r--r--   0        0        0     1180 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/elements/models/float.py
--rw-r--r--   0        0        0     1223 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/elements/models/integer.py
--rw-r--r--   0        0        0     1247 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/elements/models/netres.py
--rw-r--r--   0        0        0     1284 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/elements/models/string.py
--rw-r--r--   0        0        0     6437 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/elements/models/swaref.py
--rw-r--r--   0        0        0     1195 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/elements/models/time.py
--rw-r--r--   0        0        0     2125 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/elements/numeric_type_spec.py
--rw-r--r--   0        0        0     2276 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/elements/string_type_spec.py
--rw-r--r--   0        0        0     3767 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/elements/validators.py
--rw-r--r--   0        0        0      679 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/envelope/__init__.py
--rw-r--r--   0        0        0     2836 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/envelope/factory.py
--rw-r--r--   0        0        0     1413 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/envelope/generics.py
--rw-r--r--   0        0        0     1912 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/envelope/header.py
--rw-r--r--   0        0        0     2020 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/file_size.py
--rw-r--r--   0        0        0      742 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/multipart/__init__.py
--rw-r--r--   0        0        0     2608 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/multipart/bodypart.py
--rw-r--r--   0        0        0     1898 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/multipart/decoder.py
--rw-r--r--   0        0        0     2493 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/multipart/encoder.py
--rw-r--r--   0        0        0     1020 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/multipart/errors.py
--rw-r--r--   0        0        0      955 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/soap/__init__.py
--rw-r--r--   0        0        0     5257 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/soap/action.py
--rw-r--r--   0        0        0     5223 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/soap/faults.py
--rw-r--r--   0        0        0     1654 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/soap/response.py
--rw-r--r--   0        0        0     5291 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/soap/service.py
--rw-r--r--   0        0        0     2071 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/soap/service.pyi
--rw-r--r--   0        0        0     2004 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/soap/validators.py
--rw-r--r--   0        0        0     5172 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/storage.py
--rw-r--r--   0        0        0     3249 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/uid_gen.py
--rw-r--r--   0        0        0     1068 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/utils/__init__.py
--rw-r--r--   0        0        0     3057 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/utils/content_utils.py
--rw-r--r--   0        0        0     2673 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/utils/path_utils.py
--rw-r--r--   0        0        0      851 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/utils/route_utils.py
--rw-r--r--   0        0        0      397 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/wsdl/__init__.py
--rw-r--r--   0        0        0     5349 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/wsdl/generator.py
--rw-r--r--   0        0        0     4274 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/wsdl/helpers.py
--rw-r--r--   0        0        0     2050 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/wsdl/models/__init__.py
--rw-r--r--   0        0        0     2864 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/wsdl/models/binding.py
--rw-r--r--   0        0        0     1270 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/wsdl/models/conditions.py
--rw-r--r--   0        0        0     1360 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/wsdl/models/definitions.py
--rw-r--r--   0        0        0     1698 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/wsdl/models/port_type.py
--rw-r--r--   0        0        0     1315 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/wsdl/models/restrictions.py
--rw-r--r--   0        0        0     2139 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/wsdl/models/schema.py
--rw-r--r--   0        0        0     1361 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/wsdl/models/service.py
--rw-r--r--   0        0        0      561 2024-04-25 18:42:21.429129 fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/utils.py
--rw-r--r--   0        0        0     2587 2024-04-25 18:42:21.525129 fastapi_xroad_soap-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     8405 1970-01-01 00:00:00.000000 fastapi_xroad_soap-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0    13831 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/LICENSE
+-rw-r--r--   0        0        0     6684 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/README.md
+-rw-r--r--   0        0        0      524 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/__init__.py
+-rw-r--r--   0        0        0      574 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/elements.py
+-rw-r--r--   0        0        0      431 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/faults.py
+-rw-r--r--   0        0        0      340 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/__init__.py
+-rw-r--r--   0        0        0      666 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/base/__init__.py
+-rw-r--r--   0        0        0     2953 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/base/base_element_spec.py
+-rw-r--r--   0        0        0     1194 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/base/composite_meta.py
+-rw-r--r--   0        0        0      988 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/base/dynamic_spec.py
+-rw-r--r--   0        0        0     4392 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/base/message_body.py
+-rw-r--r--   0        0        0     2705 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/base/validators.py
+-rw-r--r--   0        0        0     1067 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/constants.py
+-rw-r--r--   0        0        0      486 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/__init__.py
+-rw-r--r--   0        0        0     1061 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/__init__.py
+-rw-r--r--   0        0        0     1479 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/boolean.py
+-rw-r--r--   0        0        0     1195 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/date.py
+-rw-r--r--   0        0        0     1243 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/datetime.py
+-rw-r--r--   0        0        0     1180 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/float.py
+-rw-r--r--   0        0        0     1223 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/integer.py
+-rw-r--r--   0        0        0     1247 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/netres.py
+-rw-r--r--   0        0        0     1284 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/string.py
+-rw-r--r--   0        0        0     6437 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/swaref.py
+-rw-r--r--   0        0        0     1195 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/time.py
+-rw-r--r--   0        0        0     2125 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/numeric_type_spec.py
+-rw-r--r--   0        0        0     2276 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/string_type_spec.py
+-rw-r--r--   0        0        0     3767 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/validators.py
+-rw-r--r--   0        0        0      679 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/envelope/__init__.py
+-rw-r--r--   0        0        0     2836 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/envelope/factory.py
+-rw-r--r--   0        0        0     1425 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/envelope/generics.py
+-rw-r--r--   0        0        0     1912 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/envelope/header.py
+-rw-r--r--   0        0        0     2020 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/file_size.py
+-rw-r--r--   0        0        0      742 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/multipart/__init__.py
+-rw-r--r--   0        0        0     2608 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/multipart/bodypart.py
+-rw-r--r--   0        0        0     1898 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/multipart/decoder.py
+-rw-r--r--   0        0        0     2493 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/multipart/encoder.py
+-rw-r--r--   0        0        0     1020 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/multipart/errors.py
+-rw-r--r--   0        0        0      955 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/soap/__init__.py
+-rw-r--r--   0        0        0     5257 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/soap/action.py
+-rw-r--r--   0        0        0     5223 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/soap/faults.py
+-rw-r--r--   0        0        0     1654 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/soap/response.py
+-rw-r--r--   0        0        0     5291 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/soap/service.py
+-rw-r--r--   0        0        0     2071 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/soap/service.pyi
+-rw-r--r--   0        0        0     2004 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/soap/validators.py
+-rw-r--r--   0        0        0     5172 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/storage.py
+-rw-r--r--   0        0        0     3249 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/uid_gen.py
+-rw-r--r--   0        0        0     1068 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/utils/__init__.py
+-rw-r--r--   0        0        0     3057 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/utils/content_utils.py
+-rw-r--r--   0        0        0     2673 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/utils/path_utils.py
+-rw-r--r--   0        0        0      851 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/utils/route_utils.py
+-rw-r--r--   0        0        0      397 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/__init__.py
+-rw-r--r--   0        0        0     5381 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/generator.py
+-rw-r--r--   0        0        0     4274 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/helpers.py
+-rw-r--r--   0        0        0     2050 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/__init__.py
+-rw-r--r--   0        0        0     2864 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/binding.py
+-rw-r--r--   0        0        0     1270 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/conditions.py
+-rw-r--r--   0        0        0     1360 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/definitions.py
+-rw-r--r--   0        0        0     1698 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/port_type.py
+-rw-r--r--   0        0        0     1315 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/restrictions.py
+-rw-r--r--   0        0        0     2139 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/schema.py
+-rw-r--r--   0        0        0     1361 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/service.py
+-rw-r--r--   0        0        0      561 2024-05-02 11:13:55.511642 fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/utils.py
+-rw-r--r--   0        0        0     2587 2024-05-02 11:13:55.607643 fastapi_xroad_soap-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0     8405 1970-01-01 00:00:00.000000 fastapi_xroad_soap-0.4.3/PKG-INFO
```

### Comparing `fastapi_xroad_soap-0.4.2/LICENSE` & `fastapi_xroad_soap-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/README.md` & `fastapi_xroad_soap-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/__init__.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/elements.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/elements.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/base/__init__.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/base/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/base/base_element_spec.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/base/base_element_spec.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/base/composite_meta.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/base/composite_meta.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/base/dynamic_spec.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/base/dynamic_spec.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/base/message_body.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/base/message_body.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/base/validators.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/base/validators.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/constants.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/constants.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/elements/models/__init__.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/elements/models/boolean.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/boolean.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/elements/models/date.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/date.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/elements/models/datetime.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/datetime.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/elements/models/float.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/float.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/elements/models/integer.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/integer.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/elements/models/netres.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/netres.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/elements/models/string.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/string.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/elements/models/swaref.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/swaref.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/elements/models/time.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/models/time.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/elements/numeric_type_spec.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/numeric_type_spec.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/elements/string_type_spec.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/string_type_spec.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/elements/validators.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/elements/validators.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/envelope/__init__.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/envelope/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/envelope/factory.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/envelope/factory.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/envelope/generics.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/envelope/generics.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 	body: t.Optional[MessageBodyType] = element(tag="Body", default=None)
 
 
 class GenericFault(*bases, tag="Fault", ns="soapenv", nsmap=ENV_NSMAP):
 	faultcode: str = element(tag="faultcode", ns='')
 	faultstring: str = element(tag="faultstring", ns='')
 	faultactor: t.Optional[str] = element(tag="faultactor", ns='', default=None)
-	detail: MessageBodyType = element(tag="detail", ns='', default=None)
+	detail: t.Optional[MessageBodyType] = element(tag="detail", ns='', default=None)
 
 
 class GenericBody(*bases, tag="Body", nsmap=ENV_NSMAP):
 	content: MessageBodyType
 
 
 class AnyBody(MessageBody, tag="Body", nsmap=ENV_NSMAP):
```

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/envelope/header.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/envelope/header.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/file_size.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/file_size.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/multipart/__init__.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/multipart/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/multipart/bodypart.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/multipart/bodypart.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/multipart/decoder.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/multipart/decoder.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/multipart/encoder.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/multipart/encoder.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/multipart/errors.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/multipart/errors.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/soap/__init__.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/soap/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/soap/action.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/soap/action.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/soap/faults.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/soap/faults.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/soap/response.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/soap/response.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/soap/service.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/soap/service.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/soap/service.pyi` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/soap/service.pyi`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/soap/validators.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/soap/validators.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/storage.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/storage.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/uid_gen.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/uid_gen.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/utils/__init__.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/utils/content_utils.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/utils/content_utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/utils/path_utils.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/utils/route_utils.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/utils/route_utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/wsdl/generator.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,16 +106,16 @@
 			*complex_types,
 			mod.ComplexType(
 				name="FaultResponse",
 				sequence=mod.Sequence(
 					elements=[
 						mod.Element(name="faultcode", type="string"),
 						mod.Element(name="faultstring", type="string"),
-						mod.Element(name="faultactor", type="string"),
-						mod.Element(name="detail", type="tns:FaultResponseDetail")
+						mod.Element(name="faultactor", type="string", min_occurs="0"),
+						mod.Element(name="detail", type="tns:FaultResponseDetail", min_occurs="0")
 					]
 				)
 			),
 			mod.ComplexType(
 				name="FaultResponseDetail",
 				sequence=mod.Sequence(
 					elements=[mod.AnyXML()]
```

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/wsdl/helpers.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/helpers.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/wsdl/models/__init__.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/__init__.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/wsdl/models/binding.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/binding.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/wsdl/models/conditions.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/conditions.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/wsdl/models/definitions.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/definitions.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/wsdl/models/port_type.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/port_type.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/wsdl/models/restrictions.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/restrictions.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/wsdl/models/schema.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/schema.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/internal/wsdl/models/service.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/internal/wsdl/models/service.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/fastapi_xroad_soap/utils.py` & `fastapi_xroad_soap-0.4.3/fastapi_xroad_soap/utils.py`

 * *Files identical despite different names*

### Comparing `fastapi_xroad_soap-0.4.2/pyproject.toml` & `fastapi_xroad_soap-0.4.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fastapi-xroad-soap"
-version = "0.4.2"
+version = "0.4.3"
 description = "FastAPI Extension for X-Road SOAP"
 authors = ["Zero Reports Team <zero.dev@rik.ee>"]
 license = "EUPL-1.2"
 readme = "README.md"
 keywords = ["fastapi", "xroad", "soap"]
 classifiers = [
     "Development Status :: 4 - Beta",
```

### Comparing `fastapi_xroad_soap-0.4.2/PKG-INFO` & `fastapi_xroad_soap-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-xroad-soap
-Version: 0.4.2
+Version: 0.4.3
 Summary: FastAPI Extension for X-Road SOAP
 License: EUPL-1.2
 Keywords: fastapi,xroad,soap
 Author: Zero Reports Team
 Author-email: zero.dev@rik.ee
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

