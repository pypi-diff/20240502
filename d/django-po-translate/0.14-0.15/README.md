# Comparing `tmp/django-po-translate-0.14.tar.gz` & `tmp/django_po_translate-0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-po-translate-0.14.tar", last modified: Mon Oct 16 15:54:40 2023, max compression
+gzip compressed data, was "django_po_translate-0.15.tar", last modified: Thu May  2 12:54:24 2024, max compression
```

## Comparing `django-po-translate-0.14.tar` & `django_po_translate-0.15.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 den       (1000) den       (1000)        0 2023-10-16 15:54:40.150697 django-po-translate-0.14/
--rw-rw-r--   0 den       (1000) den       (1000)     1073 2023-09-15 08:24:34.000000 django-po-translate-0.14/LICENSE
--rw-rw-r--   0 den       (1000) den       (1000)       59 2023-09-15 08:26:13.000000 django-po-translate-0.14/MANIFEST.in
--rw-r--r--   0 den       (1000) den       (1000)     1631 2023-10-16 15:54:40.150697 django-po-translate-0.14/PKG-INFO
--rw-rw-r--   0 den       (1000) den       (1000)      834 2023-09-15 15:06:17.000000 django-po-translate-0.14/README.rst
-drwxrwxr-x   0 den       (1000) den       (1000)        0 2023-10-16 15:54:40.146697 django-po-translate-0.14/django_po_translate.egg-info/
--rw-r--r--   0 den       (1000) den       (1000)     1631 2023-10-16 15:54:40.000000 django-po-translate-0.14/django_po_translate.egg-info/PKG-INFO
--rw-rw-r--   0 den       (1000) den       (1000)      579 2023-10-16 15:54:40.000000 django-po-translate-0.14/django_po_translate.egg-info/SOURCES.txt
--rw-rw-r--   0 den       (1000) den       (1000)        1 2023-10-16 15:54:40.000000 django-po-translate-0.14/django_po_translate.egg-info/dependency_links.txt
--rw-rw-r--   0 den       (1000) den       (1000)       13 2023-10-16 15:54:40.000000 django-po-translate-0.14/django_po_translate.egg-info/requires.txt
--rw-rw-r--   0 den       (1000) den       (1000)       13 2023-10-16 15:54:40.000000 django-po-translate-0.14/django_po_translate.egg-info/top_level.txt
-drwxrwxr-x   0 den       (1000) den       (1000)        0 2023-10-16 15:54:40.150697 django-po-translate-0.14/po_translate/
--rw-rw-r--   0 den       (1000) den       (1000)        0 2023-09-15 08:17:17.000000 django-po-translate-0.14/po_translate/__init__.py
--rw-rw-r--   0 den       (1000) den       (1000)       63 2023-09-15 08:17:17.000000 django-po-translate-0.14/po_translate/admin.py
--rw-rw-r--   0 den       (1000) den       (1000)      155 2023-09-15 08:17:17.000000 django-po-translate-0.14/po_translate/apps.py
-drwxrwxr-x   0 den       (1000) den       (1000)        0 2023-10-16 15:54:40.150697 django-po-translate-0.14/po_translate/management/
--rw-rw-r--   0 den       (1000) den       (1000)        0 2023-09-15 08:17:28.000000 django-po-translate-0.14/po_translate/management/__init__.py
-drwxrwxr-x   0 den       (1000) den       (1000)        0 2023-10-16 15:54:40.150697 django-po-translate-0.14/po_translate/management/commands/
--rw-rw-r--   0 den       (1000) den       (1000)        0 2023-09-15 08:17:37.000000 django-po-translate-0.14/po_translate/management/commands/__init__.py
--rw-rw-r--   0 den       (1000) den       (1000)     3144 2023-10-16 15:52:30.000000 django-po-translate-0.14/po_translate/management/commands/makemessages.py
-drwxrwxr-x   0 den       (1000) den       (1000)        0 2023-10-16 15:54:40.150697 django-po-translate-0.14/po_translate/migrations/
--rw-rw-r--   0 den       (1000) den       (1000)        0 2023-09-15 08:17:17.000000 django-po-translate-0.14/po_translate/migrations/__init__.py
--rw-rw-r--   0 den       (1000) den       (1000)       57 2023-09-15 08:17:17.000000 django-po-translate-0.14/po_translate/models.py
--rw-rw-r--   0 den       (1000) den       (1000)       60 2023-09-15 08:17:17.000000 django-po-translate-0.14/po_translate/tests.py
--rw-rw-r--   0 den       (1000) den       (1000)       63 2023-09-15 08:17:17.000000 django-po-translate-0.14/po_translate/views.py
--rw-rw-r--   0 den       (1000) den       (1000)       89 2023-09-15 11:07:42.000000 django-po-translate-0.14/pyproject.toml
--rw-rw-r--   0 den       (1000) den       (1000)      813 2023-10-16 15:54:40.150697 django-po-translate-0.14/setup.cfg
--rw-rw-r--   0 den       (1000) den       (1000)       37 2023-09-15 08:25:35.000000 django-po-translate-0.14/setup.py
+drwxrwxr-x   0 den       (1000) den       (1000)        0 2024-05-02 12:54:24.773710 django_po_translate-0.15/
+-rw-rw-r--   0 den       (1000) den       (1000)     1073 2023-09-15 08:24:34.000000 django_po_translate-0.15/LICENSE
+-rw-rw-r--   0 den       (1000) den       (1000)       59 2023-09-15 08:26:13.000000 django_po_translate-0.15/MANIFEST.in
+-rw-r--r--   0 den       (1000) den       (1000)     1631 2024-05-02 12:54:24.773710 django_po_translate-0.15/PKG-INFO
+-rw-rw-r--   0 den       (1000) den       (1000)      834 2023-09-15 15:06:17.000000 django_po_translate-0.15/README.rst
+drwxrwxr-x   0 den       (1000) den       (1000)        0 2024-05-02 12:54:24.773710 django_po_translate-0.15/django_po_translate.egg-info/
+-rw-r--r--   0 den       (1000) den       (1000)     1631 2024-05-02 12:54:24.000000 django_po_translate-0.15/django_po_translate.egg-info/PKG-INFO
+-rw-rw-r--   0 den       (1000) den       (1000)      579 2024-05-02 12:54:24.000000 django_po_translate-0.15/django_po_translate.egg-info/SOURCES.txt
+-rw-rw-r--   0 den       (1000) den       (1000)        1 2024-05-02 12:54:24.000000 django_po_translate-0.15/django_po_translate.egg-info/dependency_links.txt
+-rw-rw-r--   0 den       (1000) den       (1000)       13 2024-05-02 12:54:24.000000 django_po_translate-0.15/django_po_translate.egg-info/requires.txt
+-rw-rw-r--   0 den       (1000) den       (1000)       13 2024-05-02 12:54:24.000000 django_po_translate-0.15/django_po_translate.egg-info/top_level.txt
+drwxrwxr-x   0 den       (1000) den       (1000)        0 2024-05-02 12:54:24.773710 django_po_translate-0.15/po_translate/
+-rw-rw-r--   0 den       (1000) den       (1000)        0 2023-09-15 08:17:17.000000 django_po_translate-0.15/po_translate/__init__.py
+-rw-rw-r--   0 den       (1000) den       (1000)       63 2023-09-15 08:17:17.000000 django_po_translate-0.15/po_translate/admin.py
+-rw-rw-r--   0 den       (1000) den       (1000)      155 2023-09-15 08:17:17.000000 django_po_translate-0.15/po_translate/apps.py
+drwxrwxr-x   0 den       (1000) den       (1000)        0 2024-05-02 12:54:24.773710 django_po_translate-0.15/po_translate/management/
+-rw-rw-r--   0 den       (1000) den       (1000)        0 2023-09-15 08:17:28.000000 django_po_translate-0.15/po_translate/management/__init__.py
+drwxrwxr-x   0 den       (1000) den       (1000)        0 2024-05-02 12:54:24.773710 django_po_translate-0.15/po_translate/management/commands/
+-rw-rw-r--   0 den       (1000) den       (1000)        0 2023-09-15 08:17:37.000000 django_po_translate-0.15/po_translate/management/commands/__init__.py
+-rw-rw-r--   0 den       (1000) den       (1000)     3180 2024-05-02 12:12:53.000000 django_po_translate-0.15/po_translate/management/commands/makemessages.py
+drwxrwxr-x   0 den       (1000) den       (1000)        0 2024-05-02 12:54:24.773710 django_po_translate-0.15/po_translate/migrations/
+-rw-rw-r--   0 den       (1000) den       (1000)        0 2023-09-15 08:17:17.000000 django_po_translate-0.15/po_translate/migrations/__init__.py
+-rw-rw-r--   0 den       (1000) den       (1000)       57 2023-09-15 08:17:17.000000 django_po_translate-0.15/po_translate/models.py
+-rw-rw-r--   0 den       (1000) den       (1000)       60 2023-09-15 08:17:17.000000 django_po_translate-0.15/po_translate/tests.py
+-rw-rw-r--   0 den       (1000) den       (1000)       63 2023-09-15 08:17:17.000000 django_po_translate-0.15/po_translate/views.py
+-rw-rw-r--   0 den       (1000) den       (1000)       89 2023-09-15 11:07:42.000000 django_po_translate-0.15/pyproject.toml
+-rw-rw-r--   0 den       (1000) den       (1000)      813 2024-05-02 12:54:24.773710 django_po_translate-0.15/setup.cfg
+-rw-rw-r--   0 den       (1000) den       (1000)       37 2023-09-15 08:25:35.000000 django_po_translate-0.15/setup.py
```

### Comparing `django-po-translate-0.14/LICENSE` & `django_po_translate-0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `django-po-translate-0.14/PKG-INFO` & `django_po_translate-0.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-po-translate
-Version: 0.14
+Version: 0.15
 Summary: Django app with updated makemessages command to add automatic translation.
 Home-page: https://github.com/KokocGroup/django-po-translate
 Author: KokocGroup
 Author-email: dev@kokoc.com
 License: BSD
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-po-translate-0.14/README.rst` & `django_po_translate-0.15/README.rst`

 * *Files identical despite different names*

### Comparing `django-po-translate-0.14/django_po_translate.egg-info/PKG-INFO` & `django_po_translate-0.15/django_po_translate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-po-translate
-Version: 0.14
+Version: 0.15
 Summary: Django app with updated makemessages command to add automatic translation.
 Home-page: https://github.com/KokocGroup/django-po-translate
 Author: KokocGroup
 Author-email: dev@kokoc.com
 License: BSD
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
```

### Comparing `django-po-translate-0.14/django_po_translate.egg-info/SOURCES.txt` & `django_po_translate-0.15/django_po_translate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-po-translate-0.14/po_translate/management/commands/makemessages.py` & `django_po_translate-0.15/po_translate/management/commands/makemessages.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,27 +28,30 @@
     def po_translate(self, po_file, locale):
         untranslated_list = [entry.msgid for entry in po_file.untranslated_entries()]
         translated_list = self.translator.translate(untranslated_list, dest=locale)
 
         for entry, translated in zip(po_file.untranslated_entries(), translated_list):
             variables_msgid = re.findall(self.RE_PATTERN, entry.msgid)
             is_msgid_starts_with_newline = entry.msgid.startswith("\n")
+            is_msgid_end_with_newline = entry.msgid.endswith("\n")
 
             if not variables_msgid:
                 entry.msgstr = translated.text
-                if is_msgid_starts_with_newline:
-                    entry.msgstr = "\n" + translated.text
             else:
                 variables_msgstr = re.findall(self.RE_PATTERN, translated.text)
 
                 for var_msgstr, var_msgid in zip(variables_msgstr, variables_msgid):
                     translated.text = translated.text.replace(var_msgstr, var_msgid)
                     entry.msgstr = translated.text
-                    if is_msgid_starts_with_newline:
-                        entry.msgstr = "\n" + translated.text
+
+            if is_msgid_starts_with_newline:
+                entry.msgstr = "\n" + entry.msgstr
+            if is_msgid_end_with_newline:
+                entry.msgstr = entry.msgstr + "\n"
+
         po_file.save()
 
     def add_arguments(self, parser):
         super().add_arguments(parser)
         parser.add_argument(
             '--no-clear-fuzzy',
             dest='no_clear_fuzzy',
```

### Comparing `django-po-translate-0.14/setup.cfg` & `django_po_translate-0.15/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-po-translate
-version = 0.14
+version = 0.15
 description = Django app with updated makemessages command to add automatic translation.
 long_description = file: README.rst
 url = https://github.com/KokocGroup/django-po-translate
 author = KokocGroup
 author_email = dev@kokoc.com
 license = BSD
 classifiers =
```

