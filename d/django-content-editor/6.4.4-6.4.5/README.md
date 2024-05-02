# Comparing `tmp/django_content_editor-6.4.4.tar.gz` & `tmp/django_content_editor-6.4.5.tar.gz`

## Comparing `django_content_editor-6.4.4.tar` & `django_content_editor-6.4.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/__init__.py
--rw-r--r--   0        0        0     7900 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/admin.py
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/contents.py
--rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/models.py
--rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14201 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/ca/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16734 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/cs/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14394 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11079 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/hr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    14307 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/hr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    10397 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    13934 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/nb/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/nl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/nl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    11813 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/pl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/pt/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18077 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/pt/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/pt/LC_MESSAGES/djangojs.mo
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/pt/LC_MESSAGES/djangojs.po
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16962 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/ro/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    22555 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    18043 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/tr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    15334 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/locale/zh_CN/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    10547 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/static/content_editor/content_editor.css
--rw-r--r--   0        0        0    23212 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/static/content_editor/content_editor.js
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/static/content_editor/material-icons.css
--rw-r--r--   0        0        0   124372 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/static/content_editor/material-icons.woff2
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/static/content_editor/save_shortcut.js
--rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/content_editor/static/content_editor/tabbed_fieldsets.js
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/.gitignore
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/AUTHORS
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/LICENSE
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/README.rst
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/pyproject.toml
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 django_content_editor-6.4.4/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/__init__.py
+-rw-r--r--   0        0        0     8036 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/admin.py
+-rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/contents.py
+-rw-r--r--   0        0        0     2163 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/models.py
+-rw-r--r--   0        0        0      490 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14201 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/ca/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      466 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16734 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1906 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14394 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11079 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/hr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    14307 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/hr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10397 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    13934 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/nb/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/nl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18224 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/nl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    11813 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/pl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/pt/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18077 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/pt/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/pt/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/pt/LC_MESSAGES/djangojs.po
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16962 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10942 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/ro/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    22555 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18043 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/tr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    15334 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/locale/zh_CN/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    10547 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/static/content_editor/content_editor.css
+-rw-r--r--   0        0        0    23344 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/static/content_editor/content_editor.js
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/static/content_editor/material-icons.css
+-rw-r--r--   0        0        0   128616 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/static/content_editor/material-icons.woff2
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/static/content_editor/save_shortcut.js
+-rw-r--r--   0        0        0     1862 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/content_editor/static/content_editor/tabbed_fieldsets.js
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/.gitignore
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/AUTHORS
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/LICENSE
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/README.rst
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/pyproject.toml
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 django_content_editor-6.4.5/PKG-INFO
```

### Comparing `django_content_editor-6.4.4/content_editor/admin.py` & `django_content_editor-6.4.5/content_editor/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,29 +121,32 @@
     the standard ``ModelAdmin`` class.
     """
 
     checks_class = ContentEditorChecks
 
     def _content_editor_context(self, request, context):
         instance = context.get("original")
-        if not instance:
+        show_plugins = True
+        if instance is None:
             instance = self.model()
+        else:
+            show_plugins = self.has_change_permission(request, instance)
 
         plugins = []
         adding_not_allowed = ["_adding_not_allowed"]
         for iaf in context.get("inline_admin_formsets", []):
             if not isinstance(iaf.opts, ContentEditorInline):
                 continue
             regions = (
                 (
                     iaf.opts.regions({region.key for region in instance.regions})
                     if callable(iaf.opts.regions)
                     else iaf.opts.regions
                 )
-                if iaf.opts.has_add_permission(request, instance)
+                if show_plugins and iaf.opts.has_add_permission(request, instance)
                 else adding_not_allowed
             )
             plugins.append(
                 {
                     "title": capfirst(str(iaf.opts.verbose_name)),
                     "regions": list(regions) if regions else None,
                     "prefix": iaf.formset.prefix,
```

### Comparing `django_content_editor-6.4.4/content_editor/contents.py` & `django_content_editor-6.4.5/content_editor/contents.py`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/content_editor/models.py` & `django_content_editor-6.4.5/content_editor/models.py`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/content_editor/locale/ca/LC_MESSAGES/django.po` & `django_content_editor-6.4.5/content_editor/locale/ca/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/content_editor/locale/cs/LC_MESSAGES/django.po` & `django_content_editor-6.4.5/content_editor/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/content_editor/locale/de/LC_MESSAGES/django.mo` & `django_content_editor-6.4.5/content_editor/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/content_editor/locale/de/LC_MESSAGES/django.po` & `django_content_editor-6.4.5/content_editor/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/content_editor/locale/es/LC_MESSAGES/django.po` & `django_content_editor-6.4.5/content_editor/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/content_editor/locale/fr/LC_MESSAGES/django.po` & `django_content_editor-6.4.5/content_editor/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/content_editor/locale/hr/LC_MESSAGES/django.mo` & `django_content_editor-6.4.5/content_editor/locale/hr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/content_editor/locale/hr/LC_MESSAGES/django.po` & `django_content_editor-6.4.5/content_editor/locale/hr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/content_editor/locale/it/LC_MESSAGES/django.po` & `django_content_editor-6.4.5/content_editor/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/content_editor/locale/nb/LC_MESSAGES/django.po` & `django_content_editor-6.4.5/content_editor/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/content_editor/locale/nl/LC_MESSAGES/django.po` & `django_content_editor-6.4.5/content_editor/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/content_editor/locale/pl/LC_MESSAGES/django.mo` & `django_content_editor-6.4.5/content_editor/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/content_editor/locale/pl/LC_MESSAGES/django.po` & `django_content_editor-6.4.5/content_editor/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/content_editor/locale/pt/LC_MESSAGES/django.po` & `django_content_editor-6.4.5/content_editor/locale/pt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/content_editor/locale/pt/LC_MESSAGES/djangojs.po` & `django_content_editor-6.4.5/content_editor/locale/pt/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/content_editor/locale/pt_BR/LC_MESSAGES/django.po` & `django_content_editor-6.4.5/content_editor/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/content_editor/locale/ro/LC_MESSAGES/django.mo` & `django_content_editor-6.4.5/content_editor/locale/ro/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/content_editor/locale/ro/LC_MESSAGES/django.po` & `django_content_editor-6.4.5/content_editor/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/content_editor/locale/ru/LC_MESSAGES/django.mo` & `django_content_editor-6.4.5/content_editor/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/content_editor/locale/ru/LC_MESSAGES/django.po` & `django_content_editor-6.4.5/content_editor/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/content_editor/locale/tr/LC_MESSAGES/django.po` & `django_content_editor-6.4.5/content_editor/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/content_editor/locale/zh_CN/LC_MESSAGES/django.po` & `django_content_editor-6.4.5/content_editor/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/content_editor/static/content_editor/content_editor.css` & `django_content_editor-6.4.5/content_editor/static/content_editor/content_editor.css`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/content_editor/static/content_editor/content_editor.js` & `django_content_editor-6.4.5/content_editor/static/content_editor/content_editor.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -361,15 +361,18 @@
     }
 
     // Assing data-region to all inlines.
     // We also want to the data attribute to be visible to selectors (that's why we're using $.attr)
     function assignRegionDataAttribute() {
         orderMachine.find(".inline-related:not(.empty-form)").each(function() {
             const $this = $(this)
-            let region = $this.find(".field-region input").val()
+            // Try input first and fall back to the readonly presentation
+            let region =
+                $this.find(".field-region input").val() ||
+                $this.find(".field-region .readonly").text()
 
             if (!ContentEditor.regionsByKey[region]) {
                 const key = `_unknown_${region}`
                 if (!ContentEditor.regionsByKey[key]) {
                     const spec = {
                         key: `_unknown_${region}`,
                         title: `${ContentEditor.messages.unknownRegion}: ${region}`,
```

### Comparing `django_content_editor-6.4.4/content_editor/static/content_editor/tabbed_fieldsets.js` & `django_content_editor-6.4.5/content_editor/static/content_editor/tabbed_fieldsets.js`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/AUTHORS` & `django_content_editor-6.4.5/AUTHORS`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/LICENSE` & `django_content_editor-6.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/README.rst` & `django_content_editor-6.4.5/README.rst`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/pyproject.toml` & `django_content_editor-6.4.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_content_editor-6.4.4/PKG-INFO` & `django_content_editor-6.4.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-content-editor
-Version: 6.4.4
+Version: 6.4.5
 Summary: Editing structured content
 Project-URL: Homepage, https://github.com/matthiask/django-content-editor/
 Author-email: Matthias Kestenholz <mk@feinheit.ch>
 License: BSD-3-Clause
 License-File: AUTHORS
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
```

