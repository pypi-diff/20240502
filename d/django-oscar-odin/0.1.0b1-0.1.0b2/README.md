# Comparing `tmp/django_oscar_odin-0.1.0b1.tar.gz` & `tmp/django_oscar_odin-0.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_oscar_odin-0.1.0b1.tar", max compression
+gzip compressed data, was "django_oscar_odin-0.1.0b2.tar", max compression
```

## Comparing `django_oscar_odin-0.1.0b1.tar` & `django_oscar_odin-0.1.0b2.tar`

### file list

```diff
@@ -1,31 +1,36 @@
--rw-r--r--   0        0        0      547 2024-01-09 14:34:20.479673 django_oscar_odin-0.1.0b1/README.md
--rw-r--r--   0        0        0       65 2024-01-04 10:53:08.121289 django_oscar_odin-0.1.0b1/oscar_odin/__init__.py
--rw-r--r--   0        0        0      567 2024-02-16 14:27:46.031106 django_oscar_odin-0.1.0b1/oscar_odin/apps.py
--rw-r--r--   0        0        0      732 2024-01-26 08:29:29.675553 django_oscar_odin-0.1.0b1/oscar_odin/django_resolver.py
--rw-r--r--   0        0        0       46 2024-01-09 14:34:20.481029 django_oscar_odin-0.1.0b1/oscar_odin/exceptions.py
--rw-r--r--   0        0        0     1169 2024-01-09 14:34:20.481116 django_oscar_odin-0.1.0b1/oscar_odin/fields.py
--rw-r--r--   0        0        0     1081 2023-11-22 08:00:39.259519 django_oscar_odin-0.1.0b1/oscar_odin/fixtures/oscar_odin/address.json
--rw-r--r--   0        0        0      523 2023-11-22 08:00:39.259579 django_oscar_odin-0.1.0b1/oscar_odin/fixtures/oscar_odin/auth.json
--rw-r--r--   0        0        0   232255 2023-11-22 08:00:39.260362 django_oscar_odin-0.1.0b1/oscar_odin/fixtures/oscar_odin/catalogue.json
--rw-r--r--   0        0        0    18340 2024-01-09 14:34:20.481385 django_oscar_odin-0.1.0b1/oscar_odin/fixtures/oscar_odin/csv/products.csv
--rw-r--r--   0        0        0     1625 2023-11-22 08:00:39.260441 django_oscar_odin-0.1.0b1/oscar_odin/fixtures/oscar_odin/offer.json
--rw-r--r--   0        0        0     4165 2023-11-22 08:00:39.260506 django_oscar_odin-0.1.0b1/oscar_odin/fixtures/oscar_odin/order.json
--rw-r--r--   0        0        0      556 2023-11-22 08:00:39.260568 django_oscar_odin-0.1.0b1/oscar_odin/fixtures/oscar_odin/partner.json
--rw-r--r--   0        0        0      102 2023-11-22 08:00:39.260655 django_oscar_odin-0.1.0b1/oscar_odin/mappings/__init__.py
--rw-r--r--   0        0        0     1071 2024-02-22 16:00:44.902566 django_oscar_odin-0.1.0b1/oscar_odin/mappings/_common.py
--rw-r--r--   0        0        0     4251 2024-02-22 16:00:44.902852 django_oscar_odin-0.1.0b1/oscar_odin/mappings/_model_mapper.py
--rw-r--r--   0        0        0     1295 2024-02-22 16:00:44.903061 django_oscar_odin-0.1.0b1/oscar_odin/mappings/address.py
--rw-r--r--   0        0        0      375 2024-02-22 16:00:44.903326 django_oscar_odin-0.1.0b1/oscar_odin/mappings/auth.py
--rw-r--r--   0        0        0    13736 2024-02-22 16:00:44.903541 django_oscar_odin-0.1.0b1/oscar_odin/mappings/catalogue.py
--rw-r--r--   0        0        0     2778 2024-01-09 14:34:20.482154 django_oscar_odin-0.1.0b1/oscar_odin/mappings/constants.py
--rw-r--r--   0        0        0    13398 2024-02-16 14:27:46.031302 django_oscar_odin-0.1.0b1/oscar_odin/mappings/context.py
--rw-r--r--   0        0        0     6170 2024-02-22 16:00:44.903668 django_oscar_odin-0.1.0b1/oscar_odin/mappings/order.py
--rw-r--r--   0        0        0      182 2024-01-09 14:34:20.482517 django_oscar_odin-0.1.0b1/oscar_odin/resources/__init__.py
--rw-r--r--   0        0        0      213 2023-12-01 08:56:41.007588 django_oscar_odin-0.1.0b1/oscar_odin/resources/_base.py
--rw-r--r--   0        0        0     2831 2024-01-09 14:34:20.482570 django_oscar_odin-0.1.0b1/oscar_odin/resources/address.py
--rw-r--r--   0        0        0      331 2024-01-09 14:34:20.482617 django_oscar_odin-0.1.0b1/oscar_odin/resources/auth.py
--rw-r--r--   0        0        0     2614 2024-02-21 10:52:46.228378 django_oscar_odin-0.1.0b1/oscar_odin/resources/catalogue.py
--rw-r--r--   0        0        0     6007 2024-01-09 14:34:20.482905 django_oscar_odin-0.1.0b1/oscar_odin/resources/order.py
--rw-r--r--   0        0        0     2043 2024-01-26 10:25:10.207829 django_oscar_odin-0.1.0b1/oscar_odin/utils.py
--rw-r--r--   0        0        0     2156 2024-02-23 10:41:23.770372 django_oscar_odin-0.1.0b1/pyproject.toml
--rw-r--r--   0        0        0     2345 1970-01-01 00:00:00.000000 django_oscar_odin-0.1.0b1/PKG-INFO
+-rw-r--r--   0        0        0      547 2024-01-09 14:34:20.479673 django_oscar_odin-0.1.0b2/README.md
+-rw-r--r--   0        0        0       65 2024-01-04 10:53:08.121289 django_oscar_odin-0.1.0b2/oscar_odin/__init__.py
+-rw-r--r--   0        0        0      567 2024-03-12 09:26:15.033293 django_oscar_odin-0.1.0b2/oscar_odin/apps.py
+-rw-r--r--   0        0        0      732 2024-03-12 09:26:33.551476 django_oscar_odin-0.1.0b2/oscar_odin/django_resolver.py
+-rw-r--r--   0        0        0       46 2024-01-09 14:34:20.481029 django_oscar_odin-0.1.0b2/oscar_odin/exceptions.py
+-rw-r--r--   0        0        0     1169 2024-03-12 09:26:33.552050 django_oscar_odin-0.1.0b2/oscar_odin/fields.py
+-rw-r--r--   0        0        0     1081 2023-11-22 08:00:39.259519 django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/address.json
+-rw-r--r--   0        0        0      523 2023-11-22 08:00:39.259579 django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/auth.json
+-rw-r--r--   0        0        0   232255 2023-11-22 08:00:39.260362 django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/catalogue.json
+-rw-r--r--   0        0        0    18340 2024-01-09 14:34:20.481385 django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/csv/products.csv
+-rw-r--r--   0        0        0     1625 2023-11-22 08:00:39.260441 django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/offer.json
+-rw-r--r--   0        0        0     4165 2023-11-22 08:00:39.260506 django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/order.json
+-rw-r--r--   0        0        0      556 2023-11-22 08:00:39.260568 django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/partner.json
+-rw-r--r--   0        0        0    72609 2024-03-12 08:43:00.328897 django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/test_discount/address.json
+-rw-r--r--   0        0        0      515 2024-03-12 08:43:00.329014 django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/test_discount/auth.json
+-rw-r--r--   0        0        0     6315 2024-03-12 08:43:00.329125 django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/test_discount/catalogue.json
+-rw-r--r--   0        0        0    12582 2024-03-12 08:43:00.329241 django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/test_discount/order.json
+-rw-r--r--   0        0        0     2422 2024-03-12 08:43:00.329342 django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/test_discount/partner.json
+-rw-r--r--   0        0        0      102 2023-11-22 08:00:39.260655 django_oscar_odin-0.1.0b2/oscar_odin/mappings/__init__.py
+-rw-r--r--   0        0        0     1071 2024-03-12 09:26:33.552999 django_oscar_odin-0.1.0b2/oscar_odin/mappings/_common.py
+-rw-r--r--   0        0        0     4115 2024-03-12 09:26:33.553628 django_oscar_odin-0.1.0b2/oscar_odin/mappings/_model_mapper.py
+-rw-r--r--   0        0        0     1295 2024-03-12 09:26:33.554478 django_oscar_odin-0.1.0b2/oscar_odin/mappings/address.py
+-rw-r--r--   0        0        0      375 2024-03-12 09:26:33.555000 django_oscar_odin-0.1.0b2/oscar_odin/mappings/auth.py
+-rw-r--r--   0        0        0    14370 2024-05-02 11:37:32.133629 django_oscar_odin-0.1.0b2/oscar_odin/mappings/catalogue.py
+-rw-r--r--   0        0        0     3106 2024-02-23 13:21:29.278952 django_oscar_odin-0.1.0b2/oscar_odin/mappings/constants.py
+-rw-r--r--   0        0        0    20905 2024-05-02 11:37:32.133916 django_oscar_odin-0.1.0b2/oscar_odin/mappings/context.py
+-rw-r--r--   0        0        0     8199 2024-03-12 09:26:33.555693 django_oscar_odin-0.1.0b2/oscar_odin/mappings/order.py
+-rw-r--r--   0        0        0      182 2024-01-09 14:34:20.482517 django_oscar_odin-0.1.0b2/oscar_odin/resources/__init__.py
+-rw-r--r--   0        0        0      250 2024-05-02 11:37:32.134160 django_oscar_odin-0.1.0b2/oscar_odin/resources/_base.py
+-rw-r--r--   0        0        0     2942 2024-05-02 11:37:32.134385 django_oscar_odin-0.1.0b2/oscar_odin/resources/address.py
+-rw-r--r--   0        0        0      368 2024-05-02 11:37:32.134571 django_oscar_odin-0.1.0b2/oscar_odin/resources/auth.py
+-rw-r--r--   0        0        0     3145 2024-05-02 11:37:32.134767 django_oscar_odin-0.1.0b2/oscar_odin/resources/catalogue.py
+-rw-r--r--   0        0        0     6630 2024-05-02 11:37:32.134990 django_oscar_odin-0.1.0b2/oscar_odin/resources/order.py
+-rw-r--r--   0        0        0     2647 2024-05-02 11:37:32.135194 django_oscar_odin-0.1.0b2/oscar_odin/utils.py
+-rw-r--r--   0        0        0     2284 2024-05-02 15:07:49.004932 django_oscar_odin-0.1.0b2/pyproject.toml
+-rw-r--r--   0        0        0     2418 1970-01-01 00:00:00.000000 django_oscar_odin-0.1.0b2/PKG-INFO
```

### Comparing `django_oscar_odin-0.1.0b1/README.md` & `django_oscar_odin-0.1.0b2/README.md`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b1/oscar_odin/apps.py` & `django_oscar_odin-0.1.0b2/oscar_odin/apps.py`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b1/oscar_odin/django_resolver.py` & `django_oscar_odin-0.1.0b2/oscar_odin/django_resolver.py`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b1/oscar_odin/fields.py` & `django_oscar_odin-0.1.0b2/oscar_odin/fields.py`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b1/oscar_odin/fixtures/oscar_odin/address.json` & `django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/address.json`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b1/oscar_odin/fixtures/oscar_odin/auth.json` & `django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/auth.json`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b1/oscar_odin/fixtures/oscar_odin/catalogue.json` & `django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/catalogue.json`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b1/oscar_odin/fixtures/oscar_odin/csv/products.csv` & `django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/csv/products.csv`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b1/oscar_odin/fixtures/oscar_odin/offer.json` & `django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/offer.json`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b1/oscar_odin/fixtures/oscar_odin/order.json` & `django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/order.json`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b1/oscar_odin/fixtures/oscar_odin/partner.json` & `django_oscar_odin-0.1.0b2/oscar_odin/fixtures/oscar_odin/partner.json`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b1/oscar_odin/mappings/_common.py` & `django_oscar_odin-0.1.0b2/oscar_odin/mappings/_common.py`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b1/oscar_odin/mappings/_model_mapper.py` & `django_oscar_odin-0.1.0b2/oscar_odin/mappings/_model_mapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -103,21 +103,15 @@
         for relation, instances in related_field_values["m2o_related_values"].items():
             if instances:
                 self.context.add_instances_to_m2o_relation(
                     relation, (parent, instances)
                 )
 
         for relation, instances in related_field_values["m2m_related_values"].items():
-            if instances:
-                self.context.add_instances_to_m2m_relation(
-                    relation, (parent, instances)
-                )
+            self.context.add_instances_to_m2m_relation(relation, (parent, instances))
 
         for relation, instances in related_field_values["o2m_related_values"].items():
-            if instances:
-                self.context.add_instances_to_o2m_relation(
-                    relation, (parent, instances)
-                )
+            self.context.add_instances_to_o2m_relation(relation, (parent, instances))
 
         for field, instance in related_field_values["fk_related_values"].items():
             if instance:
                 self.context.add_instance_to_fk_items(field, instance)
```

### Comparing `django_oscar_odin-0.1.0b1/oscar_odin/mappings/address.py` & `django_oscar_odin-0.1.0b2/oscar_odin/mappings/address.py`

 * *Files identical despite different names*

### Comparing `django_oscar_odin-0.1.0b1/oscar_odin/mappings/catalogue.py` & `django_oscar_odin-0.1.0b2/oscar_odin/mappings/catalogue.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 """Mappings between odin and django-oscar models."""
 import odin
 
 from decimal import Decimal
 from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 
 from django.contrib.auth.models import AbstractUser
-from django.db.models import QuerySet, Model, ManyToManyField, ForeignKey
+from django.db.models import QuerySet
 from django.db.models.fields.files import ImageFieldFile
 from django.http import HttpRequest
 from oscar.apps.partner.strategy import Default as DefaultStrategy
 from oscar.core.loading import get_class, get_model
 
 from datetime import datetime
 
 from .. import resources
-from ..resources.catalogue import Structure
 from ._common import map_queryset, OscarBaseMapping
 from ._model_mapper import ModelMapping
+from ..utils import validate_resources
 
 from .context import ProductModelMapperContext
 from .constants import ALL_CATALOGUE_FIELDS, MODEL_IDENTIFIERS_MAPPING
 
 __all__ = (
     "ProductImageToResource",
     "CategoryToResource",
@@ -139,19 +139,14 @@
 
 class ProductToResource(OscarBaseMapping):
     """Map from a product model to a resource."""
 
     from_obj = ProductModel
     to_obj = resources.catalogue.Product
 
-    @odin.map_field
-    def structure(self, value: str) -> Structure:
-        """Map structure to enum."""
-        return Structure(value)
-
     @odin.assign_field
     def title(self) -> str:
         """Map title field."""
         return self.source.get_title()
 
     @odin.assign_field
     def meta_title(self) -> str:
@@ -219,27 +214,36 @@
             return (
                 map_queryset(
                     ProductToResource, self.source.children, context=self.context
                 ),
             )
         return (None,)
 
-    @odin.assign_field(to_field=("price", "currency", "availability"))
+    @odin.assign_field(
+        to_field=("price", "currency", "availability", "is_available_to_buy")
+    )
     def map_stock_price(self) -> Tuple[Decimal, str, int]:
         """Resolve stock price using strategy and decompose into price/currency/availability."""
         stock_strategy: DefaultStrategy = self.context["stock_strategy"]
 
-        # Switch here based on if this is a parent or child product
-        price, availability, _ = stock_strategy.fetch_for_product(self.source)
+        if self.source.is_parent:
+            price, availability, _ = stock_strategy.fetch_for_parent(self.source)
+        else:
+            price, availability, _ = stock_strategy.fetch_for_product(self.source)
 
         if availability.is_available_to_buy:
-            return price.excl_tax, price.currency, availability.num_available
+            return (
+                price.excl_tax,
+                price.currency,
+                getattr(availability, "num_available", 0),
+                True,
+            )
         else:
             # There is no stock record for this product.
-            return Decimal(0), "", 0
+            return Decimal(0), "", 0, False
 
 
 class ProductToModel(ModelMapping):
     """Map from a product resource to a model."""
 
     from_obj = resources.catalogue.Product
     to_obj = ProductModel
@@ -290,22 +294,34 @@
                     partner=partner,
                     partner_sku=upc,
                 )
             ]
 
         return []
 
+    @odin.map_list_field
+    def recommended_products(self, values):
+        if values:
+            return RecommendedProductToModel.apply(values)
+
+        return []
+
     @odin.map_field
     def product_class(self, value) -> ProductClassModel:
-        if not value and self.source.structure == ProductModel.CHILD:
+        if not value or self.source.structure == ProductModel.CHILD:
             return None
 
         return ProductClassToModel.apply(value)
 
 
+class RecommendedProductToModel(OscarBaseMapping):
+    from_obj = resources.catalogue.ProductRecommentation
+    to_obj = ProductModel
+
+
 class ParentToModel(OscarBaseMapping):
     from_obj = resources.catalogue.ParentProduct
     to_obj = ProductModel
 
     @odin.assign_field
     def structure(self):
         return ProductModel.PARENT
@@ -387,38 +403,52 @@
 
     return product_to_resource(
         query_set, request, user, include_children=include_children, **kwargs
     )
 
 
 def products_to_model(
-    products: List[resources.catalogue.Product], product_mapper=ProductToModel
+    products: List[resources.catalogue.Product],
+    product_mapper=ProductToModel,
+    delete_related=False,
 ) -> Tuple[List[ProductModel], Dict]:
-    context = ProductModelMapperContext(ProductModel)
+    context = ProductModelMapperContext(ProductModel, delete_related=delete_related)
 
     result = product_mapper.apply(products, context=context)
 
     try:
         return (list(result), context)
     except TypeError:  # it is not a list
         return ([result], context)
 
 
 def products_to_db(
     products,
     fields_to_update=ALL_CATALOGUE_FIELDS,
     identifier_mapping=MODEL_IDENTIFIERS_MAPPING,
     product_mapper=ProductToModel,
+    delete_related=False,
+    clean_instances=True,
 ) -> Tuple[List[ProductModel], Dict]:
     """Map mulitple products to a model and store them in the database.
 
     The method will first bulk update or create the foreign keys like parent products and productclasses
     After that all the products will be bulk saved.
     At last all related models like images, stockrecords, and related_products can will be saved and set on the product.
     """
-    instances, context = products_to_model(products, product_mapper=product_mapper)
+    errors = validate_resources(products)
+    if errors:
+        return [], errors
+    instances, context = products_to_model(
+        products,
+        product_mapper=product_mapper,
+        delete_related=delete_related,
+    )
 
     products, errors = context.bulk_save(
-        instances, fields_to_update, identifier_mapping
+        instances,
+        fields_to_update,
+        identifier_mapping,
+        clean_instances,
     )
 
     return products, errors
```

### Comparing `django_oscar_odin-0.1.0b1/oscar_odin/mappings/constants.py` & `django_oscar_odin-0.1.0b2/oscar_odin/mappings/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,18 +12,22 @@
 PRODUCT_UPC = "Product.upc"
 PRODUCT_PARENT = "Product.parent"
 PRODUCT_TITLE = "Product.title"
 PRODUCT_SLUG = "Product.slug"
 PRODUCT_DESCRIPTION = "Product.description"
 PRODUCT_META_TITLE = "Product.meta_title"
 PRODUCT_META_DESCRIPTION = "Product.meta_description"
-PRODUCT_PRODUCT_CLASS = "Product.product_class"
 PRODUCT_PARENT = "Product.parent"
 PRODUCT_IS_DISCOUNTABLE = "Product.is_discountable"
 
+PRODUCTCLASS_SLUG = "ProductClass.slug"
+PRODUCTCLASS_REQUIRESSHIPPING = "ProductClass.requires_shipping"
+PRODUCTCLASS_TRACKSTOCK = "ProductClass.track_stock"
+PRODUCTCLASS_NAME = "ProductClass.name"
+
 CATEGORY_NAME = "Category.name"
 CATEGORY_CODE = "Category.code"
 CATEGORY_DESCRIPTION = "Category.description"
 CATEGORY_META_TITLE = "Category.meta_title"
 CATEGORY_META_DESCRIPTION = "Category.meta_description"
 CATEGORY_IMAGE = "Category.image"
 CATEGORY_SLUG = "Category.slug"
@@ -47,19 +51,25 @@
     PRODUCT_UPC,
     PRODUCT_PARENT,
     PRODUCT_TITLE,
     PRODUCT_SLUG,
     PRODUCT_DESCRIPTION,
     PRODUCT_META_TITLE,
     PRODUCT_META_DESCRIPTION,
-    PRODUCT_PRODUCT_CLASS,
     PRODUCT_IS_DISCOUNTABLE,
     PRODUCT_PARENT,
 ]
 
+ALL_PRODUCTCLASS_FIELDS = [
+    PRODUCTCLASS_SLUG,
+    PRODUCTCLASS_REQUIRESSHIPPING,
+    PRODUCTCLASS_TRACKSTOCK,
+    PRODUCTCLASS_NAME,
+]
+
 ALL_CATEGORY_FIELDS = [
     CATEGORY_NAME,
     CATEGORY_CODE,
     CATEGORY_DESCRIPTION,
     CATEGORY_META_TITLE,
     CATEGORY_META_DESCRIPTION,
     CATEGORY_IMAGE,
@@ -81,18 +91,21 @@
     STOCKRECORD_PRICE,
     STOCKRECORD_NUM_IN_STOCK,
     STOCKRECORD_NUM_ALLOCATED,
 ]
 
 
 ALL_CATALOGUE_FIELDS = (
-    ALL_PRODUCT_FIELDS + ALL_PRODUCTIMAGE_FIELDS + ALL_STOCKRECORD_FIELDS
+    ALL_PRODUCT_FIELDS
+    + ALL_PRODUCTIMAGE_FIELDS
+    + ALL_STOCKRECORD_FIELDS
+    + [PRODUCTCLASS_SLUG, CATEGORY_CODE]
 )
 
 MODEL_IDENTIFIERS_MAPPING = {
     Category: ("code",),
     Product: ("upc",),
-    StockRecord: ("product_id",),
+    StockRecord: ("partner_id", "partner_sku"),
     ProductClass: ("slug",),
     ProductImage: ("code",),
     Partner: ("slug",),
 }
```

### Comparing `django_oscar_odin-0.1.0b1/oscar_odin/mappings/context.py` & `django_oscar_odin-0.1.0b2/oscar_odin/mappings/context.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,88 +1,121 @@
 from collections import defaultdict
 from operator import attrgetter
 
 from django.db import transaction
+from django.db.models import Q
 from django.core.exceptions import ValidationError
 
-from oscar_odin.utils import in_bulk
-from oscar_odin.exceptions import OscarOdinException
-
 from oscar.core.loading import get_model
+from oscar.apps.catalogue.product_attributes import QuerysetCache
+
+from ..utils import in_bulk
+from ..exceptions import OscarOdinException
+from .constants import MODEL_IDENTIFIERS_MAPPING
 
 Product = get_model("catalogue", "Product")
+ProductClass = get_model("catalogue", "ProductClass")
 ProductAttributeValue = get_model("catalogue", "ProductAttributeValue")
+ProductAttribute = get_model("catalogue", "ProductAttribute")
 
 
 def separate_instances_to_create_and_update(Model, instances, identifier_mapping):
     instances_to_create = []
     instances_to_update = []
+    identifiying_keys = []
 
     identifiers = identifier_mapping.get(Model, {})
 
-    if identifiers:
+    if identifiers and instances:
         # pylint: disable=protected-access
         id_mapping = in_bulk(Model._default_manager, instances, identifiers)
 
         get_key_values = attrgetter(*identifiers)
         for instance in instances:
             key = get_key_values(instance)
+            identifiying_keys.append(key)
 
             if not isinstance(key, tuple):
                 key = (key,)
 
             if key in id_mapping:
                 instance.pk = id_mapping[key]
                 # pylint: disable=protected-access
                 instance._state.db = "default"
                 instance._state.adding = False
                 instances_to_update.append(instance)
             else:
                 instances_to_create.append(instance)
 
-        return instances_to_create, instances_to_update
+        return instances_to_create, instances_to_update, identifiying_keys
     else:
-        return instances, []
+        return instances, [], []
 
 
 class ModelMapperContext(dict):
     foreign_key_items = None
     many_to_many_items = None
     many_to_one_items = None
     one_to_many_items = None
     attribute_data = None
     identifier_mapping = None
+    instance_keys = None
     Model = None
     errors = None
+    clean_instances = True
+
+    update_related_models_same_type = True
 
-    def __init__(self, Model, *args, **kwargs):
+    def __init__(self, Model, *args, delete_related=False, **kwargs):
         super().__init__(*args, **kwargs)
         self.foreign_key_items = defaultdict(list)
         self.many_to_many_items = defaultdict(list)
         self.many_to_one_items = defaultdict(list)
         self.one_to_many_items = defaultdict(list)
         self.fields_to_update = defaultdict(list)
         self.identifier_mapping = defaultdict(tuple)
         self.attribute_data = []
         self.errors = []
+        self.delete_related = delete_related
         self.Model = Model
 
     def __bool__(self):
         return True
 
-    def validate_instances(self, instances, validate_unique=True):
+    def prepare_instance_for_validation(self, instance):
+        return instance
+
+    def validate_instances(self, instances, validate_unique=True, fields=None):
+        if not self.clean_instances:
+            return instances
         validated_instances = []
+        identities = []
+        exclude = ()
+        if fields and instances:
+            all_fields = instances[0]._meta.fields
+            exclude = [f.name for f in all_fields if f.name not in fields]
+
+        try:
+            identifier = self.identifier_mapping.get(instances[0].__class__)[0]
+        except (IndexError, TypeError):
+            identifier = None
 
         for instance in instances:
-            try:
-                instance.full_clean(validate_unique=validate_unique)
-            except ValidationError as e:
-                self.errors.append(e)
-            else:
-                validated_instances.append(instance)
+            if identifier is None or getattr(instance, identifier) not in identities:
+                if identifier is not None:
+                    identities.append(getattr(instance, identifier))
+                try:
+                    instance = self.prepare_instance_for_validation(instance)
+                    instance.full_clean(
+                        validate_unique=validate_unique, exclude=exclude
+                    )
+                except ValidationError as e:
+                    self.errors.append(e)
+                else:
+                    validated_instances.append(instance)
 
         return validated_instances
 
     def add_attribute_data(self, attribute_data):
         self.attribute_data.append(attribute_data)
 
     def add_instances_to_m2m_relation(self, relation, instances):
@@ -105,31 +138,34 @@
             for f in self.fields_to_update
             if f.startswith(modelname)
         ] or None
 
     def get_create_and_update_relations(self, related_instance_items):
         to_create = defaultdict(list)
         to_update = defaultdict(list)
+        identities = defaultdict(list)
 
         for relation in related_instance_items.keys():
             all_instances = []
             for _, instances in related_instance_items[relation]:
                 all_instances.extend(instances)
 
             (
                 instances_to_create,
                 instances_to_update,
+                identifying_keys,
             ) = separate_instances_to_create_and_update(
                 relation.related_model, all_instances, self.identifier_mapping
             )
 
             to_create[relation].extend(instances_to_create)
             to_update[relation].extend(instances_to_update)
+            identities[relation].extend(identifying_keys)
 
-        return (to_create, to_update)
+        return (to_create, to_update, identities)
 
     @property
     def get_all_m2m_relations(self):
         return self.get_create_and_update_relations(self.many_to_many_items)
 
     @property
     def get_o2m_relations(self):
@@ -140,14 +176,15 @@
         to_create = defaultdict(list)
         to_update = defaultdict(list)
 
         for relation, instances in self.foreign_key_items.items():
             (
                 instances_to_create,
                 instances_to_update,
+                _,
             ) = separate_instances_to_create_and_update(
                 relation.related_model, instances, self.identifier_mapping
             )
 
             to_create[relation].extend(instances_to_create)
             to_update[relation].extend(instances_to_update)
 
@@ -164,23 +201,27 @@
 
         for field, instances in instances_to_create.items():
             validated_fk_instances = self.validate_instances(instances)
             field.related_model.objects.bulk_create(validated_fk_instances)
 
         for field, instances in instances_to_update.items():
             Model = field.related_model
-            fields = self.get_fields_to_update(Model)
-            if fields is not None:
-                validated_instances_to_update = self.validate_instances(instances)
-                Model.objects.bulk_update(validated_instances_to_update, fields=fields)
+            if self.update_related_models_same_type or Model != self.Model:
+                fields = self.get_fields_to_update(Model)
+                if fields is not None:
+                    instances_to_update = self.validate_instances(
+                        instances, fields=fields
+                    )
+                    Model.objects.bulk_update(instances_to_update, fields=fields)
 
     def bulk_update_or_create_instances(self, instances):
         (
             instances_to_create,
             instances_to_update,
+            self.instance_keys,
         ) = separate_instances_to_create_and_update(
             self.Model, instances, self.identifier_mapping
         )
 
         validated_create_instances = self.validate_instances(instances_to_create)
         self.Model.objects.bulk_create(validated_create_instances)
         for instance in validated_create_instances:
@@ -190,106 +231,217 @@
                         oscar_odin.mappings.catalogue.products_to_db does not support sqlite3 with Django < 4.
                         Please use engines that have can_return_rows_from_bulk_insert set to True (like Postgres) or upgrade your Django version to 4 or higher.
                     """
                 )
 
         fields = self.get_fields_to_update(self.Model)
         if fields is not None:
-            validated_instances_to_update = self.validate_instances(instances_to_update)
+            validated_instances_to_update = self.validate_instances(
+                instances_to_update, fields=fields
+            )
             for instance in validated_instances_to_update:
                 # This should be removed once support for django 3.2 is dropped
                 # pylint: disable=protected-access
                 instance._prepare_related_fields_for_save("bulk_update")
             self.Model.objects.bulk_update(validated_instances_to_update, fields=fields)
 
     def bulk_update_or_create_one_to_many(self):
         for relation, product, instances in self.get_all_o2m_instances:
             for instance in instances:
                 setattr(instance, relation.field.name, product)
 
-        instances_to_create, instances_to_update = self.get_o2m_relations
+        instances_to_create, instances_to_update, identities = self.get_o2m_relations
 
-        for relation, instances in instances_to_create.items():
-            validated_instances_to_create = self.validate_instances(instances)
-            relation.related_model.objects.bulk_create(validated_instances_to_create)
+        for relation, instances_to_create in instances_to_create.items():
+            if (
+                self.update_related_models_same_type
+                or relation.related_model != self.Model
+            ):
+                fields = self.get_fields_to_update(relation.related_model)
+                if fields is not None:
+                    instances_to_create = self.validate_instances(instances_to_create)
+                    relation.related_model.objects.bulk_create(instances_to_create)
+
+        for relation, instances_to_update in instances_to_update.items():
+            if (
+                self.update_related_models_same_type
+                or relation.related_model != self.Model
+            ):
+                fields = self.get_fields_to_update(relation.related_model)
+                if fields is not None:
+                    instances_to_update = self.validate_instances(
+                        instances_to_update, fields=fields
+                    )
+                    relation.related_model.objects.bulk_update(
+                        instances_to_update, fields=fields
+                    )
 
-        for relation, instances in instances_to_update.items():
-            fields = self.get_fields_to_update(relation.related_model)
-            if fields is not None:
-                validated_instances_to_update = self.validate_instances(instances)
-                relation.related_model.objects.bulk_update(
-                    validated_instances_to_update, fields=fields
-                )
+        if self.delete_related:
+            for relation, keys in identities.items():
+                instance_identifier = self.identifier_mapping.get(
+                    relation.remote_field.related_model
+                )[0]
+                fields = self.get_fields_to_update(relation.related_model)
+                if fields is not None:
+                    conditions = Q()
+                    identifiers = self.identifier_mapping[relation.related_model]
+                    for key in keys:
+                        if isinstance(key, (list, tuple)):
+                            conditions |= Q(**dict(list(zip(identifiers, key))))
+                        else:
+                            conditions |= Q(**{f"{identifiers[0]}": key})
+                    field_name = relation.remote_field.attname.replace(
+                        "_", "__"
+                    ).replace("id", instance_identifier)
+                    # Delete all related one_to_many instances where product is in the
+                    # given list of resources and excluding any instances present in
+                    # those resources
+                    relation.related_model.objects.filter(
+                        **{f"{field_name}__in": self.instance_keys}
+                    ).exclude(conditions).delete()
 
     def bulk_update_or_create_many_to_many(self):
-        m2m_to_create, m2m_to_update = self.get_all_m2m_relations
+        m2m_to_create, m2m_to_update, _ = self.get_all_m2m_relations
 
         # Create many to many's
-        for relation, instances in m2m_to_create.items():
-            validated_m2m_instances = self.validate_instances(instances)
-            relation.related_model.objects.bulk_create(validated_m2m_instances)
+        for relation, instances_to_create in m2m_to_create.items():
+            if (
+                self.update_related_models_same_type
+                or relation.related_model != self.Model
+            ):
+                fields = self.get_fields_to_update(relation.related_model)
+                if fields is not None:
+                    instances_to_create = self.validate_instances(instances_to_create)
+                    relation.related_model.objects.bulk_create(instances_to_create)
 
         # Update many to many's
-        for relation, instances in m2m_to_update.items():
-            fields = self.get_fields_to_update(relation.related_model)
-            if fields is not None:
-                validated_instances_to_update = self.validate_instances(instances)
-                relation.related_model.objects.bulk_update(
-                    validated_instances_to_update, fields=fields
-                )
+        for relation, instances_to_update in m2m_to_update.items():
+            if (
+                self.update_related_models_same_type
+                or relation.related_model != self.Model
+            ):
+                fields = self.get_fields_to_update(relation.related_model)
+                if fields is not None:
+                    instances_to_update = self.validate_instances(
+                        instances_to_update, fields=fields
+                    )
+                    relation.related_model.objects.bulk_update(
+                        instances_to_update, fields=fields
+                    )
 
         for relation, values in self.many_to_many_items.items():
-            Through = getattr(self.Model, relation.name).through
+            fields = self.get_fields_to_update(relation.related_model)
+            if fields is not None:
+                Through = getattr(self.Model, relation.name).through
 
-            # Create all through models that are needed for the products and many to many
-            throughs = defaultdict(Through)
-            for product, instances in values:
-                for instance in instances:
-                    throughs[(product.pk, instance.pk)] = Through(
+                # Create all through models that are needed for the products and
+                # many to many
+                throughs = defaultdict(Through)
+                to_delete_throughs_product_ids = []
+                for product, instances in values:
+                    if not instances:
+                        # Delete throughs if no instances are passed for the field
+                        to_delete_throughs_product_ids.append(product.id)
+                    for instance in instances:
+                        throughs[(product.pk, instance.pk)] = Through(
+                            **{
+                                relation.m2m_field_name(): product,
+                                relation.m2m_reverse_field_name(): instance,
+                            }
+                        )
+
+                # Delete throughs if no instances are passed for the field
+                if self.delete_related:
+                    Through.objects.filter(
                         **{
-                            relation.m2m_field_name(): product,
-                            relation.m2m_reverse_field_name(): instance,
+                            "%s_id__in"
+                            % relation.m2m_field_name(): to_delete_throughs_product_ids
                         }
-                    )
+                    ).all().delete()
 
-            # Bulk query the through models to see if some already exist
-            bulk_troughs = in_bulk(
-                Through.objects,
-                instances=list(throughs.values()),
-                field_names=(
-                    relation.m2m_field_name(),
-                    relation.m2m_reverse_field_name(),
-                ),
-            )
-
-            # Remove existing through models
-            for b in bulk_troughs.keys():
-                if b in throughs:
-                    throughs.pop(b)
-
-            # Save only new through models
-            Through.objects.bulk_create(throughs.values())
+                if throughs:
+                    # Bulk query the through models to see if some already exist
+                    bulk_troughs = in_bulk(
+                        Through.objects,
+                        instances=list(throughs.values()),
+                        field_names=(
+                            relation.m2m_field_name(),
+                            relation.m2m_reverse_field_name(),
+                        ),
+                    )
 
-    def bulk_save(self, instances, fields_to_update, identifier_mapping):
+                    # Remove existing through models
+                    for b in bulk_troughs.keys():
+                        if b in throughs:
+                            throughs.pop(b)
+
+                    # Delete remaining non-existing through models
+                    if self.delete_related:
+                        Through.objects.filter(
+                            **{
+                                "%s_id__in"
+                                % relation.m2m_field_name(): [
+                                    item[0] for item in bulk_troughs.keys()
+                                ]
+                            }
+                        ).exclude(id__in=bulk_troughs.values()).delete()
+
+                    try:
+                        # Save only new through models
+                        Through.objects.bulk_create(throughs.values())
+                    except ValueError as e:
+                        raise OscarOdinException(
+                            "Failed creating Trough models for %s. Maybe the related model does NOT exist?"
+                            % relation.name
+                        ) from e
+
+    def bulk_save(
+        self, instances, fields_to_update, identifier_mapping, clean_instances
+    ):
         self.fields_to_update = fields_to_update
         self.identifier_mapping = identifier_mapping
+        self.clean_instances = clean_instances
 
         with transaction.atomic():
             self.bulk_update_or_create_foreign_keys()
 
             self.bulk_update_or_create_instances(instances)
 
             self.bulk_update_or_create_one_to_many()
 
             self.bulk_update_or_create_many_to_many()
 
             return instances, self.errors
 
 
 class ProductModelMapperContext(ModelMapperContext):
+    update_related_models_same_type = False
+    product_class_identifier = MODEL_IDENTIFIERS_MAPPING[ProductClass][0]
+    product_class_keys = set()
+    attributes = defaultdict(list)
+
+    def prepare_instance_for_validation(self, instance):
+        if hasattr(instance, "attr"):
+            self.set_product_class_attributes(instance)
+        return super().prepare_instance_for_validation(instance)
+
+    def set_product_class_attributes(self, instance):
+        if instance.product_class:
+            key = getattr(instance.product_class, self.product_class_identifier)
+            if key and key in self.attributes:
+                instance.attr.cache.set_attributes(self.attributes[key])
+
+    def add_instance_to_fk_items(self, field, instance):
+        if instance is not None and not instance.pk:
+            self.foreign_key_items[field] += [instance]
+            if instance.__class__ == ProductClass:
+                self.product_class_keys.add(
+                    getattr(instance, self.product_class_identifier)
+                )
+
     @property
     def get_fk_relations(self):
         to_create, to_update = super().get_fk_relations
 
         for relation, instances in to_create.items():
             if relation.related_model == self.Model and instances:
                 raise OscarOdinException(
@@ -307,14 +459,15 @@
         attributes_to_update = []
         attributes_to_create = []
         attributes_to_delete = []
         fields_to_be_updated = set()
 
         for product in instances:
             product.attr.invalidate()
+            self.set_product_class_attributes(product)
             (
                 to_be_updated,
                 to_be_created,
                 to_be_deleted,
                 update_fields,
             ) = product.attr.prepare_save()
 
@@ -327,15 +480,15 @@
             if to_be_deleted:
                 attributes_to_delete.extend(to_be_deleted)
 
             if update_fields:
                 fields_to_be_updated.update(update_fields)
 
         # now save all the attributes in bulk
-        if attributes_to_delete:
+        if attributes_to_delete and self.delete_related:
             ProductAttributeValue.objects.filter(pk__in=attributes_to_delete).delete()
         if attributes_to_update:
             validated_attributes_to_update = self.validate_instances(
                 attributes_to_update
             )
             ProductAttributeValue.objects.bulk_update(
                 validated_attributes_to_update, fields_to_be_updated, batch_size=500
@@ -344,11 +497,22 @@
             validated_attributes_to_create = self.validate_instances(
                 attributes_to_create
             )
             ProductAttributeValue.objects.bulk_create(
                 validated_attributes_to_create, batch_size=500, ignore_conflicts=False
             )
 
+    def fetch_product_class_attributes(self):
+        product_classes = ProductClass.objects.filter(
+            **{f"{self.product_class_identifier}__in": self.product_class_keys}
+        )
+
+        for product_class in product_classes:
+            self.attributes[
+                getattr(product_class, self.product_class_identifier)
+            ] = QuerysetCache(product_class.attributes.all())
+
     def bulk_update_or_create_instances(self, instances):
+        self.fetch_product_class_attributes()
         super().bulk_update_or_create_instances(instances)
 
         self.bulk_update_or_create_product_attributes(instances)
```

### Comparing `django_oscar_odin-0.1.0b1/oscar_odin/mappings/order.py` & `django_oscar_odin-0.1.0b2/oscar_odin/mappings/order.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,53 +1,116 @@
 """Mappings between odin and django-oscar models."""
 from typing import Any, Dict, Iterable, List, Optional, Union
 
 import odin
 from django.http import HttpRequest
 from oscar.core.loading import get_model
+from oscar_odin.resources.order import DiscountPerTaxCodeResource
 
 from .. import resources
 from ._common import map_queryset, OscarBaseMapping
 from .address import BillingAddressToResource, ShippingAddressToResource
 from .auth import UserToResource
 
+from decimal import Decimal
+from django.db.models import Sum
+from django.db.models.functions import Coalesce
+
 __all__ = (
     "OrderToResource",
     "order_to_resource",
 )
 
 OrderModel = get_model("order", "Order")
 OrderNoteModel = get_model("order", "OrderNote")
 OrderStatusChangeModel = get_model("order", "OrderStatusChange")
 LineModel = get_model("order", "Line")
 LinePriceModel = get_model("order", "LinePrice")
 PaymentEventModel = get_model("order", "PaymentEvent")
 ShippingEventModel = get_model("order", "ShippingEvent")
 OrderDiscountModel = get_model("order", "OrderDiscount")
+OrderLineDiscountModel = get_model("order", "OrderLineDiscount")
 SurchargeModel = get_model("order", "Surcharge")
 
 
 class SurchargeToResource(OscarBaseMapping):
     """Mapping from a surcharge model to a resource."""
 
     from_obj = SurchargeModel
     to_obj = resources.order.Surcharge
 
 
+class DiscountLineToResource(OscarBaseMapping):
+    """Mapping from an order discount line model to a resource"""
+
+    from_obj = OrderLineDiscountModel
+    to_obj = resources.order.DiscountLine
+
+    @odin.assign_field
+    def line(self):
+        """map line object as resource"""
+        return LineToResource.apply(self.source.line)
+
+
 class DiscountToResource(OscarBaseMapping):
     """Mapping from an order discount model to a resource."""
 
     from_obj = OrderDiscountModel
     to_obj = resources.order.Discount
 
     @odin.map_field
-    def category(self, value: str) -> resources.order.DiscountCategory:
+    def category(self, value: str):
         """Map category."""
         return resources.order.DiscountCategory(value)
 
+    @odin.assign_field
+    def is_basket_discount(self) -> bool:
+        """map is basket discount function"""
+        return self.source.is_basket_discount
+
+    @odin.assign_field
+    def is_shipping_discount(self) -> bool:
+        """map is shipping discount function"""
+        return self.source.is_shipping_discount
+
+    @odin.assign_field
+    def is_post_order_action(self) -> bool:
+        """map is post order action function"""
+        return self.source.is_post_order_action
+
+    @odin.assign_field
+    def description(self) -> str:
+        """map description function"""
+        return self.source.description()
+
+    @odin.assign_field(to_list=True)
+    def discount_lines(self):
+        """map discount lines"""
+        return map_queryset(
+            DiscountLineToResource, self.source.discount_lines, context=self.context
+        )
+
+    @odin.assign_field(to_list=True)
+    def discount_lines_per_tax_code(self):
+        """get the total discount of all lines for each tax code"""
+        discount_lines = []
+
+        for tax_code in sorted(
+            set(self.source.discount_lines.values_list("line__tax_code", flat=True))
+        ):
+            amount = self.source.discount_lines.filter(
+                line__tax_code=tax_code
+            ).aggregate(amount=Coalesce(Sum("amount"), Decimal(0)))["amount"]
+
+            discount_lines.append(
+                DiscountPerTaxCodeResource(amount=amount, tax_code=tax_code)
+            )
+
+        return discount_lines
+
 
 class ShippingEventToResource(OscarBaseMapping):
     """Mapping from a shipping event model to a resource."""
 
     from_obj = ShippingEventModel
     to_obj = resources.order.ShippingEvent
```

### Comparing `django_oscar_odin-0.1.0b1/oscar_odin/resources/address.py` & `django_oscar_odin-0.1.0b2/oscar_odin/resources/address.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from ._base import OscarResource
 
 
 class OscarAddress(OscarResource, abstract=True):
     """Base resource for Oscar order application."""
 
     class Meta:
+        allow_field_shadowing = True
         namespace = "oscar.address"
 
 
 class Country(OscarAddress):
     """A country."""
 
     iso_3166_1_a2: str = odin.Options(
@@ -66,22 +67,24 @@
     country: Country
 
 
 class BillingAddress(Address):
     """Address for billing."""
 
     class Meta:
+        allow_field_shadowing = True
         verbose_name = "Billing address"
         verbose_name_plural = "Billing addresses"
 
 
 class ShippingAddress(Address):
     """Address for shipping."""
 
     class Meta:
+        allow_field_shadowing = True
         verbose_name = "Shipping address"
         verbose_name_plural = "Shipping addresses"
 
     phone_number: str = odin.Options(
         empty=True,
         verbose_name="Phone number",
         doc_text="In case we need to call you about your order",
```

### Comparing `django_oscar_odin-0.1.0b1/oscar_odin/resources/order.py` & `django_oscar_odin-0.1.0b2/oscar_odin/resources/order.py`

 * *Files 19% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from .auth import User
 
 
 class OscarOrder(OscarResource, abstract=True):
     """Base resource for Oscar order application."""
 
     class Meta:
+        allow_field_shadowing = True
         namespace = "oscar.order"
 
 
 class LinePrice(OscarOrder):
     """For tracking the prices paid for each unit within a line.
 
     This is necessary as offers can lead to units within a line
@@ -120,25 +121,48 @@
     """Category of discount."""
 
     BASKET = "Basket"
     SHIPPING = "Shipping"
     DEFERRED = "Deferred"
 
 
+class DiscountLine(OscarOrder):
+    """Line of a discount"""
+
+    line: Line
+    order_discount_id: int
+    is_incl_tax: bool
+    amount: Decimal = DecimalField()
+
+
+class DiscountPerTaxCodeResource(OscarOrder):
+    """Total discount for each tax code in a discount"""
+
+    amount: Decimal = DecimalField()
+    tax_code: str
+
+
 class Discount(OscarOrder):
     """A discount against an order."""
 
+    id: int
     category: DiscountCategory
     offer_id: Optional[int]
     offer_name: Optional[str]
     voucher_id: Optional[int]
     voucher_code: Optional[str]
     frequency: Optional[int]
     amount: Decimal = DecimalField()
     message: str = odin.Options(empty=True)
+    discount_lines: List[DiscountLine]
+    is_basket_discount: bool
+    is_shipping_discount: bool
+    is_post_order_action: bool
+    description: str
+    discount_lines_per_tax_code: DiscountPerTaxCodeResource
 
 
 class Surcharge(OscarOrder):
     """A surcharge against an order."""
 
     name: str
     code: str
@@ -180,14 +204,15 @@
     date_created: datetime
 
 
 class Order(OscarOrder):
     """An order within Django Oscar."""
 
     class Meta:
+        allow_field_shadowing = True
         verbose_name = "Order"
 
     number: str = odin.Options(
         key=True,
         verbose_name="Order number",
     )
     site_id: Optional[int] = odin.Options(
```

### Comparing `django_oscar_odin-0.1.0b1/oscar_odin/utils.py` & `django_oscar_odin-0.1.0b2/oscar_odin/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 from collections import defaultdict
 import contextlib
 import time
 import math
 
 from django.db import connection, connections, reset_queries
 from django.db.models import Q
+from django.conf import settings
+
+from odin.exceptions import ValidationError
+from odin.mapping import MappingResult
 
 
 def get_filters(instances, field_names):
     for ui in instances:
         klaas = {}
         for field_name in field_names:
             field_value = getattr(ui, field_name)
             klaas[field_name] = field_value
 
         yield Q(**klaas)
 
 
 def get_query(instances, field_names):
-    filters = list(get_filters(instances, field_names))
+    filters = list((get_filters(instances, field_names)))
 
     query = filters.pop()
     for query_filter in filters:
         query = query | query_filter
 
     return query
 
@@ -34,15 +38,15 @@
     """
 
     max_query_params = connections[self.db].features.max_query_params
 
     if max_query_params is not None:
         batch_size = math.floor(max_query_params / len(field_names)) - 1
     else:
-        batch_size = None
+        batch_size = getattr(settings, "ODIN_BATCH_SIZE", 500)
 
     if batch_size and batch_size < len(instances):
         qs = ()
         for offset in range(0, len(instances), batch_size):
             batch = instances[offset : offset + batch_size]
             query = get_query(batch, field_names)
             qs += tuple(self.filter(query).order_by().values("pk", *field_names))
@@ -65,7 +69,24 @@
     yield
     print(" ".join([str(l) for l in labels]), "--------------" * 6)
     print("time: ", time.time() - start)
     print("num queries", len(connection.queries))
     if print_queries:
         for q in connection.queries:
             print("   ", q)
+
+
+def validate_resources(resources):
+    errors = []
+    if not resources:
+        return
+    if not isinstance(resources, (list, tuple)):
+        if isinstance(resources, MappingResult):
+            resources = resources.items
+        else:
+            resources = [resources]
+    for resource in resources:
+        try:
+            resource.full_clean()
+        except ValidationError as error:
+            errors.append(error)
+    return errors
```

### Comparing `django_oscar_odin-0.1.0b1/pyproject.toml` & `django_oscar_odin-0.1.0b2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-oscar-odin"
-version = "0.1.0b1"
+version = "0.1.0b2"
 description = "Odin Resources and mappings to Oscar models"
 authors = ["Tim Savage <tim@savage.company>"]
 maintainers = [
     "Viggo de Vries <viggo@highbiza.nl>",
 ]
 license = "BSD-3-Clause"
 readme = "README.md"
@@ -23,29 +23,33 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.1",
     "Programming Language :: Python :: Implementation :: CPython",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-odin = "^2.9"
-django-oscar = {version = "^3.2.2", allow-prereleases = true}
+django-oscar = {version = "^3.2.5a2", allow-prereleases = true}
 coverage = { version = "^7.3", optional = true }
 pylint = { version = "^3.0.2", optional = true }
 black = { version = "^23.11.0", optional = true }
 pylint-django = { version = "^2.5.5", optional = true }
 isort = {version = "^5.13.2", optional = true}
 ruff = {version = "^0.1.8", optional = true}
 poetry = {version = "^1.7.1", optional = true}
 pre-commit = {version = "*", optional = true}
 responses = {version = "^0.24.1", optional = true}
+sorl-thumbnail = {version = "^12.8.0", optional = true}
+odin = {version = "^2.10rc2", allow-prereleases = true}
 
 
 [tool.poetry.extras]
-test = ["coverage", "pylint", "black", "pylint-django", "poetry", "responses"]
+test = [
+    "coverage", "pylint", "black", "pylint-django", "poetry", "responses",
+    "sorl-thumbnail"
+]
 dev = ["ruff", "isort", "pre-commit"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
```

### Comparing `django_oscar_odin-0.1.0b1/PKG-INFO` & `django_oscar_odin-0.1.0b2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-oscar-odin
-Version: 0.1.0b1
+Version: 0.1.0b2
 Summary: Odin Resources and mappings to Oscar models
 Home-page: https://github.com/django-oscar/oscar-odin
 License: BSD-3-Clause
 Keywords: data-structure,validation,data-mapping
 Author: Tim Savage
 Author-email: tim@savage.company
 Maintainer: Viggo de Vries
@@ -23,23 +23,24 @@
 Classifier: Programming Language :: Python :: 3.1
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: dev
 Provides-Extra: test
 Requires-Dist: black (>=23.11.0,<24.0.0) ; extra == "test"
 Requires-Dist: coverage (>=7.3,<8.0) ; extra == "test"
-Requires-Dist: django-oscar (>=3.2.2,<4.0.0)
+Requires-Dist: django-oscar (>=3.2.5a2,<4.0.0)
 Requires-Dist: isort (>=5.13.2,<6.0.0) ; extra == "dev"
-Requires-Dist: odin (>=2.9,<3.0)
+Requires-Dist: odin (>=2.10rc2,<3.0)
 Requires-Dist: poetry (>=1.7.1,<2.0.0) ; extra == "test"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: pylint (>=3.0.2,<4.0.0) ; extra == "test"
 Requires-Dist: pylint-django (>=2.5.5,<3.0.0) ; extra == "test"
 Requires-Dist: responses (>=0.24.1,<0.25.0) ; extra == "test"
 Requires-Dist: ruff (>=0.1.8,<0.2.0) ; extra == "dev"
+Requires-Dist: sorl-thumbnail (>=12.8.0,<13.0.0) ; extra == "test"
 Project-URL: Repository, https://github.com/django-oscar/oscar-odin
 Description-Content-Type: text/markdown
 
 # Oscar Odin
 
 Mapping of Oscar eCommerce models to Odin resources.
```

