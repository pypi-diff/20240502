# Comparing `tmp/django_typesense-0.1.3.tar.gz` & `tmp/django_typesense-0.1.3a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_typesense-0.1.3.tar", last modified: Thu May  2 14:24:45 2024, max compression
+gzip compressed data, was "django_typesense-0.1.3a0.tar", last modified: Thu May  2 14:13:44 2024, max compression
```

## Comparing `django_typesense-0.1.3.tar` & `django_typesense-0.1.3a0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:24:45.139361 django_typesense-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-02 14:24:42.000000 django_typesense-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-02 14:24:42.000000 django_typesense-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10069 2024-05-02 14:24:45.139361 django_typesense-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9542 2024-05-02 14:24:42.000000 django_typesense-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:24:45.135361 django_typesense-0.1.3/django_typesense/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 14:24:42.000000 django_typesense-0.1.3/django_typesense/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-02 14:24:42.000000 django_typesense-0.1.3/django_typesense/admin.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-02 14:24:42.000000 django_typesense-0.1.3/django_typesense/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    17445 2024-05-02 14:24:42.000000 django_typesense-0.1.3/django_typesense/changelist.py
--rw-r--r--   0 runner    (1001) docker     (127)    13259 2024-05-02 14:24:42.000000 django_typesense-0.1.3/django_typesense/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-02 14:24:42.000000 django_typesense-0.1.3/django_typesense/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-02 14:24:42.000000 django_typesense-0.1.3/django_typesense/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:24:45.135361 django_typesense-0.1.3/django_typesense/management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:24:42.000000 django_typesense-0.1.3/django_typesense/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:24:45.135361 django_typesense-0.1.3/django_typesense/management/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:24:42.000000 django_typesense-0.1.3/django_typesense/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-02 14:24:42.000000 django_typesense-0.1.3/django_typesense/management/commands/updatecollections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:24:45.135361 django_typesense-0.1.3/django_typesense/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:24:42.000000 django_typesense-0.1.3/django_typesense/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-02 14:24:42.000000 django_typesense-0.1.3/django_typesense/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-02 14:24:42.000000 django_typesense-0.1.3/django_typesense/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-02 14:24:42.000000 django_typesense-0.1.3/django_typesense/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:24:45.131361 django_typesense-0.1.3/django_typesense/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:24:45.131361 django_typesense-0.1.3/django_typesense/static/admin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:24:45.135361 django_typesense-0.1.3/django_typesense/static/admin/js/
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-02 14:24:42.000000 django_typesense-0.1.3/django_typesense/static/admin/js/search-typesense.js
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-02 14:24:42.000000 django_typesense-0.1.3/django_typesense/typesense_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-05-02 14:24:42.000000 django_typesense-0.1.3/django_typesense/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:24:45.139361 django_typesense-0.1.3/django_typesense.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10069 2024-05-02 14:24:45.000000 django_typesense-0.1.3/django_typesense.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-02 14:24:45.000000 django_typesense-0.1.3/django_typesense.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:24:45.000000 django_typesense-0.1.3/django_typesense.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-02 14:24:45.000000 django_typesense-0.1.3/django_typesense.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 14:24:45.000000 django_typesense-0.1.3/django_typesense.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 14:24:45.139361 django_typesense-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-02 14:24:42.000000 django_typesense-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:24:45.139361 django_typesense-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:24:42.000000 django_typesense-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-02 14:24:42.000000 django_typesense-0.1.3/tests/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-02 14:24:42.000000 django_typesense-0.1.3/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-02 14:24:42.000000 django_typesense-0.1.3/tests/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-02 14:24:42.000000 django_typesense-0.1.3/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:24:42.000000 django_typesense-0.1.3/tests/test_typesense_admin_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:24:42.000000 django_typesense-0.1.3/tests/test_typesense_changelist.py
--rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-05-02 14:24:42.000000 django_typesense-0.1.3/tests/test_typesense_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:24:42.000000 django_typesense-0.1.3/tests/test_typesense_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-02 14:24:42.000000 django_typesense-0.1.3/tests/test_typesense_model_mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:24:42.000000 django_typesense-0.1.3/tests/test_typesense_paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-02 14:24:42.000000 django_typesense-0.1.3/tests/test_typesense_signals.py
--rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-05-02 14:24:42.000000 django_typesense-0.1.3/tests/test_typesense_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-02 14:24:42.000000 django_typesense-0.1.3/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:13:44.161923 django_typesense-0.1.3a0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10071 2024-05-02 14:13:44.161923 django_typesense-0.1.3a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9542 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:13:44.157923 django_typesense-0.1.3a0/django_typesense/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/django_typesense/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/django_typesense/admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/django_typesense/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17660 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/django_typesense/changelist.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/django_typesense/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/django_typesense/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/django_typesense/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:13:44.157923 django_typesense-0.1.3a0/django_typesense/management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/django_typesense/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:13:44.157923 django_typesense-0.1.3a0/django_typesense/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/django_typesense/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/django_typesense/management/commands/updatecollections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:13:44.157923 django_typesense-0.1.3a0/django_typesense/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/django_typesense/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/django_typesense/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/django_typesense/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/django_typesense/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:13:44.153923 django_typesense-0.1.3a0/django_typesense/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:13:44.153923 django_typesense-0.1.3a0/django_typesense/static/admin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:13:44.157923 django_typesense-0.1.3a0/django_typesense/static/admin/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/django_typesense/static/admin/js/search-typesense.js
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/django_typesense/typesense_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7062 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/django_typesense/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:13:44.161923 django_typesense-0.1.3a0/django_typesense.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10071 2024-05-02 14:13:44.000000 django_typesense-0.1.3a0/django_typesense.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1199 2024-05-02 14:13:44.000000 django_typesense-0.1.3a0/django_typesense.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:13:44.000000 django_typesense-0.1.3a0/django_typesense.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-02 14:13:44.000000 django_typesense-0.1.3a0/django_typesense.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-02 14:13:44.000000 django_typesense-0.1.3a0/django_typesense.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 14:13:44.161923 django_typesense-0.1.3a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:13:44.161923 django_typesense-0.1.3a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      832 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/tests/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/tests/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/tests/test_typesense_admin_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/tests/test_typesense_changelist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8048 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/tests/test_typesense_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/tests/test_typesense_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/tests/test_typesense_model_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/tests/test_typesense_paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/tests/test_typesense_signals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7677 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/tests/test_typesense_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-02 14:13:41.000000 django_typesense-0.1.3a0/tests/utils.py
```

### Comparing `django_typesense-0.1.3/LICENSE` & `django_typesense-0.1.3a0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_typesense-0.1.3/PKG-INFO` & `django_typesense-0.1.3a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_typesense
-Version: 0.1.3
+Version: 0.1.3a0
 Author: Siege Software
 Author-email: info@siege.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `django_typesense-0.1.3/README.md` & `django_typesense-0.1.3a0/README.md`

 * *Files identical despite different names*

### Comparing `django_typesense-0.1.3/django_typesense/admin.py` & `django_typesense-0.1.3a0/django_typesense/admin.py`

 * *Files identical despite different names*

### Comparing `django_typesense-0.1.3/django_typesense/changelist.py` & `django_typesense-0.1.3a0/django_typesense/changelist.py`

 * *Files 2% similar despite different names*

```diff
@@ -423,34 +423,39 @@
         qs = self.root_queryset
 
         for filter_spec in self.filter_specs:
             new_qs = filter_spec.queryset(request, qs)
             if new_qs is not None:
                 qs = new_qs
 
-        for param, value in remaining_lookup_params.items():
-            try:
-                # Finally, we apply the remaining lookup parameters from the query
-                # string (i.e. those that haven't already been processed by the
-                # filters).
-                qs = qs.filter(**{param: value})
-            except (SuspiciousOperation, ImproperlyConfigured):
-                # Allow certain types of errors to be re-raised as-is so that the
-                # caller can treat them in a special way.
-                raise
-            except Exception as e:
-                # Every other error is caught with a naked except, because we don't
-                # have any other way of validating lookup parameters. They might be
-                # invalid if the keyword arguments are incorrect, or if the values
-                # are not in the correct type, so we might get FieldError,
-                # ValueError, ValidationError, or ?.
+        lookup_params_keys = remaining_lookup_params.keys()
+        model_field_names = set((local_field.name for local_field in self.model._meta.local_fields))
+        for key in lookup_params_keys:
+            if key not in model_field_names:
+                # means k only available in typesense
+                value = remaining_lookup_params.pop(key)
+                new_lookup_params = self.model.collection_class.get_django_lookup(key, value)
+                remaining_lookup_params.update(new_lookup_params)
 
-                # for django-typesense, possibly means k only available in typesense
-                new_lookup_params = self.model.collection_class.get_django_lookup(param, value, e)
-                qs = qs.filter(**new_lookup_params)
+        try:
+            # Finally, we apply the remaining lookup parameters from the query
+            # string (i.e. those that haven't already been processed by the
+            # filters).
+            qs = qs.filter(**remaining_lookup_params)
+        except (SuspiciousOperation, ImproperlyConfigured):
+            # Allow certain types of errors to be re-raised as-is so that the
+            # caller can treat them in a special way.
+            raise
+        except Exception as e:
+            # Every other error is caught with a naked except, because we don't
+            # have any other way of validating lookup parameters. They might be
+            # invalid if the keyword arguments are incorrect, or if the values
+            # are not in the correct type, so we might get FieldError,
+            # ValueError, ValidationError, or ?.
+            raise IncorrectLookupParameters(e)
 
         # Apply search results
         qs, search_may_have_duplicates = self.model_admin.get_search_results(
             request,
             qs,
             self.query,
         )
```

### Comparing `django_typesense-0.1.3/django_typesense/collections.py` & `django_typesense-0.1.3a0/django_typesense/collections.py`

 * *Files 4% similar despite different names*

```diff
@@ -194,33 +194,29 @@
         Returns:
             A TypesenseField
         """
         fields = cls.get_fields()
         return fields[name]
 
     @classmethod
-    def get_django_lookup(cls, field, value, exception: Exception) -> dict:
+    def get_django_lookup(cls, field, value) -> dict:
         """
         Get the lookup that would have been used for this field in django. Expects to find a method on
         the collection called `get_FIELD_lookup` otherwise a NotImplementedError is raised
 
         Args:
-            field: the name of the field in the collection
+            collection_field_name: the name of the field in the collection
             value: the value to look for
-            exception: the django exception that led us here
 
         Returns:
             A dictionary of the fields to the value.
         """
 
         if "get_%s_lookup" % field not in cls.__dict__:
-            raise Exception([
-                exception,
-                NotImplementedError("get_%s_lookup is not implemented" % field)
-            ])
+            raise NotImplementedError
 
         method = methodcaller("get_%s_lookup" % field, value)
         return method(cls)
 
     @cached_property
     def schema_fields(self) -> list:
         """
```

### Comparing `django_typesense-0.1.3/django_typesense/fields.py` & `django_typesense-0.1.3a0/django_typesense/fields.py`

 * *Files identical despite different names*

### Comparing `django_typesense-0.1.3/django_typesense/management/commands/updatecollections.py` & `django_typesense-0.1.3a0/django_typesense/management/commands/updatecollections.py`

 * *Files identical despite different names*

### Comparing `django_typesense-0.1.3/django_typesense/mixins.py` & `django_typesense-0.1.3a0/django_typesense/mixins.py`

 * *Files identical despite different names*

### Comparing `django_typesense-0.1.3/django_typesense/paginator.py` & `django_typesense-0.1.3a0/django_typesense/paginator.py`

 * *Files identical despite different names*

### Comparing `django_typesense-0.1.3/django_typesense/signals.py` & `django_typesense-0.1.3a0/django_typesense/signals.py`

 * *Files identical despite different names*

### Comparing `django_typesense-0.1.3/django_typesense/static/admin/js/search-typesense.js` & `django_typesense-0.1.3a0/django_typesense/static/admin/js/search-typesense.js`

 * *Files identical despite different names*

### Comparing `django_typesense-0.1.3/django_typesense/utils.py` & `django_typesense-0.1.3a0/django_typesense/utils.py`

 * *Files identical despite different names*

### Comparing `django_typesense-0.1.3/django_typesense.egg-info/PKG-INFO` & `django_typesense-0.1.3a0/django_typesense.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_typesense
-Version: 0.1.3
+Version: 0.1.3a0
 Author: Siege Software
 Author-email: info@siege.ai
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `django_typesense-0.1.3/django_typesense.egg-info/SOURCES.txt` & `django_typesense-0.1.3a0/django_typesense.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_typesense-0.1.3/setup.py` & `django_typesense-0.1.3a0/setup.py`

 * *Files identical despite different names*

### Comparing `django_typesense-0.1.3/tests/collections.py` & `django_typesense-0.1.3a0/tests/collections.py`

 * *Files identical despite different names*

### Comparing `django_typesense-0.1.3/tests/factories.py` & `django_typesense-0.1.3a0/tests/factories.py`

 * *Files identical despite different names*

### Comparing `django_typesense-0.1.3/tests/models.py` & `django_typesense-0.1.3a0/tests/models.py`

 * *Files identical despite different names*

### Comparing `django_typesense-0.1.3/tests/settings.py` & `django_typesense-0.1.3a0/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_typesense-0.1.3/tests/test_typesense_fields.py` & `django_typesense-0.1.3a0/tests/test_typesense_fields.py`

 * *Files identical despite different names*

### Comparing `django_typesense-0.1.3/tests/test_typesense_model_mixin.py` & `django_typesense-0.1.3a0/tests/test_typesense_model_mixin.py`

 * *Files identical despite different names*

### Comparing `django_typesense-0.1.3/tests/test_typesense_signals.py` & `django_typesense-0.1.3a0/tests/test_typesense_signals.py`

 * *Files identical despite different names*

### Comparing `django_typesense-0.1.3/tests/test_typesense_utils.py` & `django_typesense-0.1.3a0/tests/test_typesense_utils.py`

 * *Files identical despite different names*

