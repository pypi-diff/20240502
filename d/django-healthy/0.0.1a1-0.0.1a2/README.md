# Comparing `tmp/django_healthy-0.0.1a1.tar.gz` & `tmp/django_healthy-0.0.1a2.tar.gz`

## Comparing `django_healthy-0.0.1a1.tar` & `django_healthy-0.0.1a2.tar`

### file list

```diff
@@ -1,13 +1,19 @@
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 django_healthy-0.0.1a1/src/healthy/__init__.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 django_healthy-0.0.1a1/src/healthy/apps.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 django_healthy-0.0.1a1/src/healthy/urls.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 django_healthy-0.0.1a1/src/healthy/views.py
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 django_healthy-0.0.1a1/tests/__init__.py
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 django_healthy-0.0.1a1/tests/settings.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 django_healthy-0.0.1a1/tests/test_views.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 django_healthy-0.0.1a1/tests/urls.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 django_healthy-0.0.1a1/.gitignore
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 django_healthy-0.0.1a1/LICENSE.txt
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 django_healthy-0.0.1a1/README.md
--rw-r--r--   0        0        0     2670 2020-02-02 00:00:00.000000 django_healthy-0.0.1a1/pyproject.toml
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 django_healthy-0.0.1a1/PKG-INFO
+-rw-r--r--   0        0        0     6072 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/ruff_defaults.toml
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/src/healthy/__init__.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/src/healthy/apps.py
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/src/healthy/backends.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/src/healthy/compat.py
+-rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/src/healthy/responses.py
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/src/healthy/urls.py
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/src/healthy/views.py
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/tests/__init__.py
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/tests/settings.py
+-rw-r--r--   0        0        0     2744 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/tests/test_backends.py
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/tests/test_responses.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/tests/test_views.py
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/tests/urls.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/.gitignore
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/LICENSE.txt
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/README.md
+-rw-r--r--   0        0        0     2946 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/pyproject.toml
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 django_healthy-0.0.1a2/PKG-INFO
```

### Comparing `django_healthy-0.0.1a1/tests/settings.py` & `django_healthy-0.0.1a2/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django_healthy-0.0.1a1/tests/test_views.py` & `django_healthy-0.0.1a2/tests/test_views.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,22 +18,22 @@
     django_client_method = getattr(client, method)
 
     response = django_client_method(reverse("healthy:ping"))
 
     assert response.status_code == HTTPStatus.METHOD_NOT_ALLOWED
 
 
-@pytest.mark.asyncio()
+@pytest.mark.asyncio
 async def test_get_ping_async(async_client):
     response = await async_client.get(reverse("healthy:ping"))
 
     assert response.status_code == HTTPStatus.OK
 
 
-@pytest.mark.asyncio()
+@pytest.mark.asyncio
 @pytest.mark.parametrize("method", ["post", "put", "patch", "delete"])
 async def test_methods_not_allowed_async(method, async_client):
     django_client_method = getattr(async_client, method)
 
     response = await django_client_method(reverse("healthy:ping"))
 
     assert response.status_code == HTTPStatus.METHOD_NOT_ALLOWED
```

### Comparing `django_healthy-0.0.1a1/LICENSE.txt` & `django_healthy-0.0.1a2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_healthy-0.0.1a1/README.md` & `django_healthy-0.0.1a2/README.md`

 * *Files identical despite different names*

### Comparing `django_healthy-0.0.1a1/pyproject.toml` & `django_healthy-0.0.1a2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
   "Framework :: Django :: 4.2",
   "Framework :: Django :: 5.0",
 ]
 dependencies = [
   "django>=4.2",
+  "typing-extensions; python_version<'3.12'"
 ]
 
 [project.urls]
 Documentation = "https://github.com/olist/django-healthy#readme"
 Issues = "https://github.com/olist/django-healthy/issues"
 Source = "https://github.com/olist/django-healthy"
 
@@ -105,7 +106,19 @@
 
 [tool.hatch.envs.types]
 dependencies = [
   "mypy>=1.0.0",
 ]
 [tool.hatch.envs.types.scripts]
 check = "mypy --install-types --non-interactive {args:src/healthy tests}"
+
+[tool.hatch.envs.hatch-static-analysis]
+config-path = "ruff_defaults.toml"
+
+[tool.ruff]
+extend = "ruff_defaults.toml"
+
+[tool.ruff.lint]
+extend-select = ["DJ"]
+
+[tool.ruff.lint.flake8-tidy-imports]
+ban-relative-imports = "parents"
```

### Comparing `django_healthy-0.0.1a1/PKG-INFO` & `django_healthy-0.0.1a2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: django-healthy
-Version: 0.0.1a1
+Version: 0.0.1a2
 Summary: Simple health checking for django applications
 Project-URL: Documentation, https://github.com/olist/django-healthy#readme
 Project-URL: Issues, https://github.com/olist/django-healthy/issues
 Project-URL: Source, https://github.com/olist/django-healthy
 Author-email: Christian Hartung <christian.hartung@olist.com>
 License-Expression: MIT
 License-File: LICENSE.txt
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: django>=4.2
+Requires-Dist: typing-extensions; python_version < '3.12'
 Description-Content-Type: text/markdown
 
 # django-healthy
 
 [![PyPI - Version](https://img.shields.io/pypi/v/django-healthy.svg)](https://pypi.org/project/django-healthy)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/django-healthy.svg)](https://pypi.org/project/django-healthy)
```

