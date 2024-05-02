# Comparing `tmp/ilcdlib-4.3.0.tar.gz` & `tmp/ilcdlib-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ilcdlib-4.3.0.tar", max compression
+gzip compressed data, was "ilcdlib-4.4.0.tar", max compression
```

## Comparing `ilcdlib-4.3.0.tar` & `ilcdlib-4.4.0.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0    11357 2024-04-30 22:40:00.065117 ilcdlib-4.3.0/LICENSE
--rw-r--r--   0        0        0     4949 2024-04-30 22:40:00.065117 ilcdlib-4.3.0/README.md
--rw-r--r--   0        0        0     3525 2024-04-30 22:40:00.065117 ilcdlib-4.3.0/pyproject.toml
--rw-r--r--   0        0        0      837 2024-04-30 22:40:00.065117 ilcdlib-4.3.0/src/ilcdlib/__init__.py
--rw-r--r--   0        0        0      910 2024-04-30 22:40:00.065117 ilcdlib-4.3.0/src/ilcdlib/__main__.py
--rw-r--r--   0        0        0      855 2024-04-30 22:40:00.065117 ilcdlib-4.3.0/src/ilcdlib/__version__.py
--rw-r--r--   0        0        0     2959 2024-04-30 22:40:00.065117 ilcdlib-4.3.0/src/ilcdlib/cli.py
--rw-r--r--   0        0        0    17587 2024-04-30 22:40:00.065117 ilcdlib-4.3.0/src/ilcdlib/common.py
--rw-r--r--   0        0        0      837 2024-04-30 22:40:00.065117 ilcdlib-4.3.0/src/ilcdlib/compat/__init__.py
--rw-r--r--   0        0        0     1158 2024-04-30 22:40:00.065117 ilcdlib-4.3.0/src/ilcdlib/compat/pydantic.py
--rw-r--r--   0        0        0     1835 2024-04-30 22:40:00.065117 ilcdlib-4.3.0/src/ilcdlib/const.py
--rw-r--r--   0        0        0     4934 2024-04-30 22:40:00.065117 ilcdlib-4.3.0/src/ilcdlib/data/category_mapping/epdnorge.csv
--rw-r--r--   0        0        0    51577 2024-04-30 22:40:00.065117 ilcdlib-4.3.0/src/ilcdlib/data/category_mapping/oekobaudat.csv
--rw-r--r--   0        0        0   172140 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/data/ilcd_epd_ref.zip
--rw-r--r--   0        0        0     6454 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/dto.py
--rw-r--r--   0        0        0      837 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/entity/__init__.py
--rw-r--r--   0        0        0     7064 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/entity/base_scope_set_reader.py
--rw-r--r--   0        0        0     3361 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/entity/category.py
--rw-r--r--   0        0        0     3052 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/entity/compliance.py
--rw-r--r--   0        0        0     6003 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/entity/contact.py
--rw-r--r--   0        0        0     4173 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/entity/exchage.py
--rw-r--r--   0        0        0     7981 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/entity/flow.py
--rw-r--r--   0        0        0     4224 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/entity/lcia.py
--rw-r--r--   0        0        0     5213 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/entity/material.py
--rw-r--r--   0        0        0     3930 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/entity/pcr.py
--rw-r--r--   0        0        0     3437 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/entity/source.py
--rw-r--r--   0        0        0     3788 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/entity/unit.py
--rw-r--r--   0        0        0     3331 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/entity/validation.py
--rw-r--r--   0        0        0      837 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/epd/__init__.py
--rw-r--r--   0        0        0    10064 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/epd/cli.py
--rw-r--r--   0        0        0      837 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/epd/dialect/__init__.py
--rw-r--r--   0        0        0     6864 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/epd/dialect/environdec.py
--rw-r--r--   0        0        0     2170 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/epd/dialect/epditaly.py
--rw-r--r--   0        0        0     2341 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/epd/dialect/epdnorge.py
--rw-r--r--   0        0        0     1329 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/epd/dialect/indata.py
--rw-r--r--   0        0        0     2105 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/epd/dialect/itb.py
--rw-r--r--   0        0        0     3876 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/epd/dialect/oekobaudat.py
--rw-r--r--   0        0        0     3644 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/epd/factory.py
--rw-r--r--   0        0        0    35343 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/epd/reader.py
--rw-r--r--   0        0        0     2248 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/extension.py
--rw-r--r--   0        0        0     7895 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/http_common.py
--rw-r--r--   0        0        0      837 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/mapping/__init__.py
--rw-r--r--   0        0        0    10680 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/mapping/category.py
--rw-r--r--   0        0        0     3603 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/mapping/common.py
--rw-r--r--   0        0        0     1168 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/mapping/compliance.py
--rw-r--r--   0        0        0     1512 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/mapping/flows.py
--rw-r--r--   0        0        0     3522 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/mapping/impacts.py
--rw-r--r--   0        0        0     1651 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/mapping/indicators.py
--rw-r--r--   0        0        0     1212 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/mapping/properties.py
--rw-r--r--   0        0        0     6247 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/mapping/units.py
--rw-r--r--   0        0        0      837 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/medium/__init__.py
--rw-r--r--   0        0        0     7531 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/medium/archive.py
--rw-r--r--   0        0        0     6496 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/medium/soda4lca.py
--rw-r--r--   0        0        0        0 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/py.typed
--rw-r--r--   0        0        0     1435 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/reference_data.py
--rw-r--r--   0        0        0      837 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/sanitizing/__init__.py
--rw-r--r--   0        0        0     1866 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/sanitizing/domain.py
--rw-r--r--   0        0        0     1336 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/sanitizing/phone.py
--rw-r--r--   0        0        0     1122 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/sanitizing/text.py
--rw-r--r--   0        0        0      837 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/soda4lca/__init__.py
--rw-r--r--   0        0        0    11347 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/soda4lca/api_client.py
--rw-r--r--   0        0        0     2755 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/soda4lca/api_client_4x.py
--rw-r--r--   0        0        0     1206 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/type.py
--rw-r--r--   0        0        0     6465 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/utils.py
--rw-r--r--   0        0        0     2399 2024-04-30 22:40:00.069117 ilcdlib-4.3.0/src/ilcdlib/xml_parser.py
--rw-r--r--   0        0        0     6082 1970-01-01 00:00:00.000000 ilcdlib-4.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-02 16:18:55.689420 ilcdlib-4.4.0/LICENSE
+-rw-r--r--   0        0        0     4949 2024-05-02 16:18:55.689420 ilcdlib-4.4.0/README.md
+-rw-r--r--   0        0        0     3525 2024-05-02 16:18:55.689420 ilcdlib-4.4.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2024-05-02 16:18:55.689420 ilcdlib-4.4.0/src/ilcdlib/__init__.py
+-rw-r--r--   0        0        0      910 2024-05-02 16:18:55.689420 ilcdlib-4.4.0/src/ilcdlib/__main__.py
+-rw-r--r--   0        0        0      855 2024-05-02 16:18:55.689420 ilcdlib-4.4.0/src/ilcdlib/__version__.py
+-rw-r--r--   0        0        0     2959 2024-05-02 16:18:55.689420 ilcdlib-4.4.0/src/ilcdlib/cli.py
+-rw-r--r--   0        0        0    17587 2024-05-02 16:18:55.689420 ilcdlib-4.4.0/src/ilcdlib/common.py
+-rw-r--r--   0        0        0      837 2024-05-02 16:18:55.689420 ilcdlib-4.4.0/src/ilcdlib/compat/__init__.py
+-rw-r--r--   0        0        0     1158 2024-05-02 16:18:55.689420 ilcdlib-4.4.0/src/ilcdlib/compat/pydantic.py
+-rw-r--r--   0        0        0     1835 2024-05-02 16:18:55.689420 ilcdlib-4.4.0/src/ilcdlib/const.py
+-rw-r--r--   0        0        0     4934 2024-05-02 16:18:55.689420 ilcdlib-4.4.0/src/ilcdlib/data/category_mapping/epdnorge.csv
+-rw-r--r--   0        0        0    51577 2024-05-02 16:18:55.689420 ilcdlib-4.4.0/src/ilcdlib/data/category_mapping/oekobaudat.csv
+-rw-r--r--   0        0        0   172140 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/data/ilcd_epd_ref.zip
+-rw-r--r--   0        0        0     6454 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/dto.py
+-rw-r--r--   0        0        0      837 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/entity/__init__.py
+-rw-r--r--   0        0        0     7064 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/entity/base_scope_set_reader.py
+-rw-r--r--   0        0        0     3361 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/entity/category.py
+-rw-r--r--   0        0        0     3052 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/entity/compliance.py
+-rw-r--r--   0        0        0     6003 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/entity/contact.py
+-rw-r--r--   0        0        0     4173 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/entity/exchage.py
+-rw-r--r--   0        0        0     7981 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/entity/flow.py
+-rw-r--r--   0        0        0     4224 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/entity/lcia.py
+-rw-r--r--   0        0        0     5213 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/entity/material.py
+-rw-r--r--   0        0        0     3930 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/entity/pcr.py
+-rw-r--r--   0        0        0     3437 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/entity/source.py
+-rw-r--r--   0        0        0     3788 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/entity/unit.py
+-rw-r--r--   0        0        0     3331 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/entity/validation.py
+-rw-r--r--   0        0        0      837 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/epd/__init__.py
+-rw-r--r--   0        0        0    10064 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/epd/cli.py
+-rw-r--r--   0        0        0      837 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/epd/dialect/__init__.py
+-rw-r--r--   0        0        0     6864 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/epd/dialect/environdec.py
+-rw-r--r--   0        0        0     2170 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/epd/dialect/epditaly.py
+-rw-r--r--   0        0        0     2341 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/epd/dialect/epdnorge.py
+-rw-r--r--   0        0        0     1329 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/epd/dialect/indata.py
+-rw-r--r--   0        0        0     2105 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/epd/dialect/itb.py
+-rw-r--r--   0        0        0     3876 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/epd/dialect/oekobaudat.py
+-rw-r--r--   0        0        0     3644 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/epd/factory.py
+-rw-r--r--   0        0        0    35343 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/epd/reader.py
+-rw-r--r--   0        0        0     2248 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/extension.py
+-rw-r--r--   0        0        0     7895 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/http_common.py
+-rw-r--r--   0        0        0      837 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/mapping/__init__.py
+-rw-r--r--   0        0        0    10680 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/mapping/category.py
+-rw-r--r--   0        0        0     3603 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/mapping/common.py
+-rw-r--r--   0        0        0     1168 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/mapping/compliance.py
+-rw-r--r--   0        0        0     1512 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/mapping/flows.py
+-rw-r--r--   0        0        0     3524 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/mapping/impacts.py
+-rw-r--r--   0        0        0     1651 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/mapping/indicators.py
+-rw-r--r--   0        0        0     1212 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/mapping/properties.py
+-rw-r--r--   0        0        0     6247 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/mapping/units.py
+-rw-r--r--   0        0        0      837 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/medium/__init__.py
+-rw-r--r--   0        0        0     7531 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/medium/archive.py
+-rw-r--r--   0        0        0     6496 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/medium/soda4lca.py
+-rw-r--r--   0        0        0        0 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/py.typed
+-rw-r--r--   0        0        0     1435 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/reference_data.py
+-rw-r--r--   0        0        0      837 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/sanitizing/__init__.py
+-rw-r--r--   0        0        0     1866 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/sanitizing/domain.py
+-rw-r--r--   0        0        0     1336 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/sanitizing/phone.py
+-rw-r--r--   0        0        0     1122 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/sanitizing/text.py
+-rw-r--r--   0        0        0      837 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/soda4lca/__init__.py
+-rw-r--r--   0        0        0    11347 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/soda4lca/api_client.py
+-rw-r--r--   0        0        0     2755 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/soda4lca/api_client_4x.py
+-rw-r--r--   0        0        0     1206 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/type.py
+-rw-r--r--   0        0        0     6465 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/utils.py
+-rw-r--r--   0        0        0     2399 2024-05-02 16:18:55.693420 ilcdlib-4.4.0/src/ilcdlib/xml_parser.py
+-rw-r--r--   0        0        0     6082 1970-01-01 00:00:00.000000 ilcdlib-4.4.0/PKG-INFO
```

### Comparing `ilcdlib-4.3.0/LICENSE` & `ilcdlib-4.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/README.md` & `ilcdlib-4.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/pyproject.toml` & `ilcdlib-4.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ilcdlib"
-version = "4.3.0"
+version = "4.4.0"
 license = "Apache-2.0"
 description = "A toolkit for reading and writing ILCD format and it's derivatives"
 authors = ["C-Change Labs <support@c-change-labs.com>"]
 maintainers = ["C-Change Labs <open-source@c-change-labs.com>"]
 repository = "https://github.com/cchangelabs/ilcdlib"
 keywords = []
 classifiers = [
```

### Comparing `ilcdlib-4.3.0/src/ilcdlib/__init__.py` & `ilcdlib-4.4.0/src/ilcdlib/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/__main__.py` & `ilcdlib-4.4.0/src/ilcdlib/__main__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/__version__.py` & `ilcdlib-4.4.0/src/ilcdlib/__version__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/cli.py` & `ilcdlib-4.4.0/src/ilcdlib/cli.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/common.py` & `ilcdlib-4.4.0/src/ilcdlib/common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/compat/__init__.py` & `ilcdlib-4.4.0/src/ilcdlib/compat/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/compat/pydantic.py` & `ilcdlib-4.4.0/src/ilcdlib/compat/pydantic.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/const.py` & `ilcdlib-4.4.0/src/ilcdlib/const.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/data/category_mapping/epdnorge.csv` & `ilcdlib-4.4.0/src/ilcdlib/data/category_mapping/epdnorge.csv`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/data/category_mapping/oekobaudat.csv` & `ilcdlib-4.4.0/src/ilcdlib/data/category_mapping/oekobaudat.csv`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/data/ilcd_epd_ref.zip` & `ilcdlib-4.4.0/src/ilcdlib/data/ilcd_epd_ref.zip`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/dto.py` & `ilcdlib-4.4.0/src/ilcdlib/dto.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/entity/__init__.py` & `ilcdlib-4.4.0/src/ilcdlib/entity/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/entity/base_scope_set_reader.py` & `ilcdlib-4.4.0/src/ilcdlib/entity/base_scope_set_reader.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/entity/category.py` & `ilcdlib-4.4.0/src/ilcdlib/entity/category.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/entity/compliance.py` & `ilcdlib-4.4.0/src/ilcdlib/entity/compliance.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/entity/contact.py` & `ilcdlib-4.4.0/src/ilcdlib/entity/contact.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/entity/exchage.py` & `ilcdlib-4.4.0/src/ilcdlib/entity/exchage.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/entity/flow.py` & `ilcdlib-4.4.0/src/ilcdlib/entity/flow.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/entity/lcia.py` & `ilcdlib-4.4.0/src/ilcdlib/entity/lcia.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/entity/material.py` & `ilcdlib-4.4.0/src/ilcdlib/entity/material.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/entity/pcr.py` & `ilcdlib-4.4.0/src/ilcdlib/entity/pcr.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/entity/source.py` & `ilcdlib-4.4.0/src/ilcdlib/entity/source.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/entity/unit.py` & `ilcdlib-4.4.0/src/ilcdlib/entity/unit.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/entity/validation.py` & `ilcdlib-4.4.0/src/ilcdlib/entity/validation.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/epd/__init__.py` & `ilcdlib-4.4.0/src/ilcdlib/epd/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/epd/cli.py` & `ilcdlib-4.4.0/src/ilcdlib/epd/cli.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/epd/dialect/__init__.py` & `ilcdlib-4.4.0/src/ilcdlib/epd/dialect/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/epd/dialect/environdec.py` & `ilcdlib-4.4.0/src/ilcdlib/epd/dialect/environdec.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/epd/dialect/epditaly.py` & `ilcdlib-4.4.0/src/ilcdlib/epd/dialect/epditaly.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/epd/dialect/epdnorge.py` & `ilcdlib-4.4.0/src/ilcdlib/epd/dialect/epdnorge.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/epd/dialect/indata.py` & `ilcdlib-4.4.0/src/ilcdlib/epd/dialect/indata.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/epd/dialect/itb.py` & `ilcdlib-4.4.0/src/ilcdlib/epd/dialect/itb.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/epd/dialect/oekobaudat.py` & `ilcdlib-4.4.0/src/ilcdlib/epd/dialect/oekobaudat.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/epd/factory.py` & `ilcdlib-4.4.0/src/ilcdlib/epd/factory.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/epd/reader.py` & `ilcdlib-4.4.0/src/ilcdlib/epd/reader.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/extension.py` & `ilcdlib-4.4.0/src/ilcdlib/extension.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/http_common.py` & `ilcdlib-4.4.0/src/ilcdlib/http_common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/mapping/__init__.py` & `ilcdlib-4.4.0/src/ilcdlib/mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/mapping/category.py` & `ilcdlib-4.4.0/src/ilcdlib/mapping/category.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/mapping/common.py` & `ilcdlib-4.4.0/src/ilcdlib/mapping/common.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/mapping/compliance.py` & `ilcdlib-4.4.0/src/ilcdlib/mapping/compliance.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/mapping/flows.py` & `ilcdlib-4.4.0/src/ilcdlib/mapping/flows.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/mapping/impacts.py` & `ilcdlib-4.4.0/src/ilcdlib/mapping/impacts.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     KV = {
         "gwp-biogenic": ["biogenic"],
         "gwp-luluc": ["luluc"],
         "gwp-nonCO2": ["CO2"],
         "ep-marine": ["marine"],
         "ep-fresh": ["freshwater", "fw"],
         "ep-terr": ["terrestrial"],
-        "odp": ["odp", "depletion"],
+        "odp": ["odp", "ozone layer"],
         "ap": ["ap", "acidification"],
         "pocp": ["pocp", "photochemical", "smog", "ozone creation"],
     }
 
 
 class ImpactsRegexToOpenIdMapper(RegexMapper[str]):
     """Map impact names using regex.""" ""
```

### Comparing `ilcdlib-4.3.0/src/ilcdlib/mapping/indicators.py` & `ilcdlib-4.4.0/src/ilcdlib/mapping/indicators.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/mapping/properties.py` & `ilcdlib-4.4.0/src/ilcdlib/mapping/properties.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/mapping/units.py` & `ilcdlib-4.4.0/src/ilcdlib/mapping/units.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/medium/__init__.py` & `ilcdlib-4.4.0/src/ilcdlib/medium/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/medium/archive.py` & `ilcdlib-4.4.0/src/ilcdlib/medium/archive.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/medium/soda4lca.py` & `ilcdlib-4.4.0/src/ilcdlib/medium/soda4lca.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/reference_data.py` & `ilcdlib-4.4.0/src/ilcdlib/reference_data.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/sanitizing/__init__.py` & `ilcdlib-4.4.0/src/ilcdlib/sanitizing/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/sanitizing/domain.py` & `ilcdlib-4.4.0/src/ilcdlib/sanitizing/domain.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/sanitizing/phone.py` & `ilcdlib-4.4.0/src/ilcdlib/sanitizing/phone.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/sanitizing/text.py` & `ilcdlib-4.4.0/src/ilcdlib/sanitizing/text.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/soda4lca/__init__.py` & `ilcdlib-4.4.0/src/ilcdlib/soda4lca/__init__.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/soda4lca/api_client.py` & `ilcdlib-4.4.0/src/ilcdlib/soda4lca/api_client.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/soda4lca/api_client_4x.py` & `ilcdlib-4.4.0/src/ilcdlib/soda4lca/api_client_4x.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/type.py` & `ilcdlib-4.4.0/src/ilcdlib/type.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/utils.py` & `ilcdlib-4.4.0/src/ilcdlib/utils.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/src/ilcdlib/xml_parser.py` & `ilcdlib-4.4.0/src/ilcdlib/xml_parser.py`

 * *Files identical despite different names*

### Comparing `ilcdlib-4.3.0/PKG-INFO` & `ilcdlib-4.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ilcdlib
-Version: 4.3.0
+Version: 4.4.0
 Summary: A toolkit for reading and writing ILCD format and it's derivatives
 Home-page: https://github.com/cchangelabs/ilcdlib
 License: Apache-2.0
 Author: C-Change Labs
 Author-email: support@c-change-labs.com
 Maintainer: C-Change Labs
 Maintainer-email: open-source@c-change-labs.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ilcdlib Version: 4.3.0 Summary: A toolkit for
+Metadata-Version: 2.1 Name: ilcdlib Version: 4.4.0 Summary: A toolkit for
 reading and writing ILCD format and it's derivatives Home-page: https://
 github.com/cchangelabs/ilcdlib License: Apache-2.0 Author: C-Change Labs
 Author-email: support@c-change-labs.com Maintainer: C-Change Labs Maintainer-
 email: open-source@c-change-labs.com Requires-Python: >=3.11,<4.0 Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Operating System :: OS Independent Classifier: Programming Language :: Python
```

