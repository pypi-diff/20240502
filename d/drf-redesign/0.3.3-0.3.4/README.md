# Comparing `tmp/drf_redesign-0.3.3.tar.gz` & `tmp/drf_redesign-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drf_redesign-0.3.3.tar", max compression
+gzip compressed data, was "drf_redesign-0.3.4.tar", max compression
```

## Comparing `drf_redesign-0.3.3.tar` & `drf_redesign-0.3.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0     1074 2024-04-25 17:25:52.836688 drf_redesign-0.3.3/LICENSE
--rw-r--r--   0        0        0     3566 2024-04-25 17:25:52.836688 drf_redesign-0.3.3/README.md
--rw-r--r--   0        0        0       91 2024-04-25 17:25:52.836688 drf_redesign-0.3.3/drf_redesign/__init__.py
--rw-r--r--   0        0        0      235 2024-04-25 17:25:52.836688 drf_redesign-0.3.3/drf_redesign/apps.py
--rw-r--r--   0        0        0    26838 2024-04-25 17:25:52.836688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/api.html
--rw-r--r--   0        0        0     1056 2024-04-25 17:25:52.836688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/filters/base.html
--rw-r--r--   0        0        0      684 2024-04-25 17:25:52.836688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/filters/ordering.html
--rw-r--r--   0        0        0      585 2024-04-25 17:25:52.836688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/filters/search.html
--rw-r--r--   0        0        0     1004 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/checkbox.html
--rw-r--r--   0        0        0     1762 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/dict_field.html
--rw-r--r--   0        0        0      427 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/fieldset.html
--rw-r--r--   0        0        0      150 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/form.html
--rw-r--r--   0        0        0     1636 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/input.html
--rw-r--r--   0        0        0      262 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/list_field.html
--rw-r--r--   0        0        0      330 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/list_fieldset.html
--rw-r--r--   0        0        0     1617 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/radio.html
--rw-r--r--   0        0        0     1398 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/select.html
--rw-r--r--   0        0        0     1433 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/select_multiple.html
--rw-r--r--   0        0        0     1006 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/textarea.html
--rw-r--r--   0        0        0     1004 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/checkbox.html
--rw-r--r--   0        0        0     1766 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/dict_field.html
--rw-r--r--   0        0        0      427 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/fieldset.html
--rw-r--r--   0        0        0      150 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/form.html
--rw-r--r--   0        0        0     1307 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/input.html
--rw-r--r--   0        0        0      262 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/list_field.html
--rw-r--r--   0        0        0      330 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/list_fieldset.html
--rw-r--r--   0        0        0     1637 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/radio.html
--rw-r--r--   0        0        0     1487 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/select.html
--rw-r--r--   0        0        0     1411 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/select_multiple.html
--rw-r--r--   0        0        0     1054 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/textarea.html
--rw-r--r--   0        0        0     5226 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/login.html
--rw-r--r--   0        0        0     2065 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/pagination/numbers.html
--rw-r--r--   0        0        0     1272 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/pagination/previous_and_next.html
--rw-r--r--   0        0        0      296 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/raw_data_form.html
--rw-r--r--   0        0        0     1004 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/checkbox.html
--rw-r--r--   0        0        0     1766 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/checkbox_multiple.html
--rw-r--r--   0        0        0      269 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/dict_field.html
--rw-r--r--   0        0        0      427 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/fieldset.html
--rw-r--r--   0        0        0      150 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/form.html
--rw-r--r--   0        0        0     1281 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/input.html
--rw-r--r--   0        0        0      262 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/list_field.html
--rw-r--r--   0        0        0      330 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/list_fieldset.html
--rw-r--r--   0        0        0     1637 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/radio.html
--rw-r--r--   0        0        0     1461 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/select.html
--rw-r--r--   0        0        0     1474 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/select_multiple.html
--rw-r--r--   0        0        0     1051 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/textarea.html
--rw-r--r--   0        0        0       51 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templatetags/__init__.py
--rw-r--r--   0        0        0     1682 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/drf_redesign/templatetags/rest_framework_redesign.py
--rw-r--r--   0        0        0      576 2024-04-25 17:25:52.840688 drf_redesign-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     4449 1970-01-01 00:00:00.000000 drf_redesign-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-02 09:16:39.865143 drf_redesign-0.3.4/LICENSE
+-rw-r--r--   0        0        0     3566 2024-05-02 09:16:39.865143 drf_redesign-0.3.4/README.md
+-rw-r--r--   0        0        0       91 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/__init__.py
+-rw-r--r--   0        0        0      235 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/apps.py
+-rw-r--r--   0        0        0    27873 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/api.html
+-rw-r--r--   0        0        0     1056 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/filters/base.html
+-rw-r--r--   0        0        0      684 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/filters/ordering.html
+-rw-r--r--   0        0        0      585 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/filters/search.html
+-rw-r--r--   0        0        0     1004 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/horizontal/checkbox.html
+-rw-r--r--   0        0        0     1762 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/horizontal/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/horizontal/dict_field.html
+-rw-r--r--   0        0        0      427 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/horizontal/fieldset.html
+-rw-r--r--   0        0        0      150 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/horizontal/form.html
+-rw-r--r--   0        0        0     1636 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/horizontal/input.html
+-rw-r--r--   0        0        0      262 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/horizontal/list_field.html
+-rw-r--r--   0        0        0      330 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/horizontal/list_fieldset.html
+-rw-r--r--   0        0        0     1617 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/horizontal/radio.html
+-rw-r--r--   0        0        0     1398 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/horizontal/select.html
+-rw-r--r--   0        0        0     1433 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/horizontal/select_multiple.html
+-rw-r--r--   0        0        0     1006 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/horizontal/textarea.html
+-rw-r--r--   0        0        0     1004 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/inline/checkbox.html
+-rw-r--r--   0        0        0     1766 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/inline/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/inline/dict_field.html
+-rw-r--r--   0        0        0      427 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/inline/fieldset.html
+-rw-r--r--   0        0        0      150 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/inline/form.html
+-rw-r--r--   0        0        0     1307 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/inline/input.html
+-rw-r--r--   0        0        0      262 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/inline/list_field.html
+-rw-r--r--   0        0        0      330 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/inline/list_fieldset.html
+-rw-r--r--   0        0        0     1637 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/inline/radio.html
+-rw-r--r--   0        0        0     1487 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/inline/select.html
+-rw-r--r--   0        0        0     1411 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/inline/select_multiple.html
+-rw-r--r--   0        0        0     1054 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/inline/textarea.html
+-rw-r--r--   0        0        0     5226 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/login.html
+-rw-r--r--   0        0        0     2065 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/pagination/numbers.html
+-rw-r--r--   0        0        0     1272 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/pagination/previous_and_next.html
+-rw-r--r--   0        0        0      296 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/raw_data_form.html
+-rw-r--r--   0        0        0     1004 2024-05-02 09:16:39.869143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/vertical/checkbox.html
+-rw-r--r--   0        0        0     1766 2024-05-02 09:16:39.873143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/vertical/checkbox_multiple.html
+-rw-r--r--   0        0        0      269 2024-05-02 09:16:39.873143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/vertical/dict_field.html
+-rw-r--r--   0        0        0      427 2024-05-02 09:16:39.873143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/vertical/fieldset.html
+-rw-r--r--   0        0        0      150 2024-05-02 09:16:39.873143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/vertical/form.html
+-rw-r--r--   0        0        0     1281 2024-05-02 09:16:39.873143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/vertical/input.html
+-rw-r--r--   0        0        0      262 2024-05-02 09:16:39.873143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/vertical/list_field.html
+-rw-r--r--   0        0        0      330 2024-05-02 09:16:39.873143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/vertical/list_fieldset.html
+-rw-r--r--   0        0        0     1637 2024-05-02 09:16:39.873143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/vertical/radio.html
+-rw-r--r--   0        0        0     1461 2024-05-02 09:16:39.873143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/vertical/select.html
+-rw-r--r--   0        0        0     1474 2024-05-02 09:16:39.873143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/vertical/select_multiple.html
+-rw-r--r--   0        0        0     1051 2024-05-02 09:16:39.873143 drf_redesign-0.3.4/drf_redesign/templates/rest_framework/vertical/textarea.html
+-rw-r--r--   0        0        0       51 2024-05-02 09:16:39.873143 drf_redesign-0.3.4/drf_redesign/templatetags/__init__.py
+-rw-r--r--   0        0        0     1682 2024-05-02 09:16:39.873143 drf_redesign-0.3.4/drf_redesign/templatetags/rest_framework_redesign.py
+-rw-r--r--   0        0        0      576 2024-05-02 09:16:39.873143 drf_redesign-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     4449 1970-01-01 00:00:00.000000 drf_redesign-0.3.4/PKG-INFO
```

### Comparing `drf_redesign-0.3.3/LICENSE` & `drf_redesign-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/README.md` & `drf_redesign-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/api.html` & `drf_redesign-0.3.4/drf_redesign/templates/rest_framework/api.html`

 * *Files 18% similar despite different names*

```diff
@@ -8,28 +8,29 @@
 {% endblock %}
 
 {% block style %}
   {% block bootstrap_theme %}
     <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet"
       integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
     <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@latest/font/bootstrap-icons.css">
+    <link id="hljs-theme" rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/styles/a11y-dark.min.css">
   {% endblock %}
 
   <style>
     {% if code_style %}
       {{ code_style }}
     {% endif %}
 
     .dropdown-toggle::after {
       content: none;
     }
   </style>
  
   <script>
-    /*!
+  /*!
     * Color mode toggler for Bootstrap's docs (https://getbootstrap.com/)
     * Copyright 2011-2023 The Bootstrap Authors
     * Licensed under the Creative Commons Attribution 3.0 Unported License.
     */
 
     (() => {
       'use strict'
@@ -45,16 +46,22 @@
 
         return window.matchMedia('(prefers-color-scheme: dark)').matches ? 'dark' : 'light'
       }
 
       const setTheme = theme => {
         if (theme === 'auto' && window.matchMedia('(prefers-color-scheme: dark)').matches) {
           document.documentElement.setAttribute('data-bs-theme', 'dark')
+          document.getElementById('hljs-theme').setAttribute('href', 'https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/styles/a11y-dark.min.css')
         } else {
           document.documentElement.setAttribute('data-bs-theme', theme)
+          if (theme === 'light') {
+            document.getElementById('hljs-theme').setAttribute('href', 'https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/styles/a11y-light.min.css')
+          } else {
+            document.getElementById('hljs-theme').setAttribute('href', 'https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/styles/a11y-dark.min.css')
+          }
         }
       }
 
       setTheme(getPreferredTheme())
 
       window.matchMedia('(prefers-color-scheme: dark)').addEventListener('change', () => {
         const storedTheme = getStoredTheme()
@@ -70,15 +77,15 @@
               const theme = toggle.getAttribute('data-bs-theme-value')
               setStoredTheme(theme)
               setTheme(theme)
             })
           })
       })
     })()
-  </script>
+</script>
 {% endblock %}
 
 
 {% block navbar %}
   <header class="fixed-top p-1 p-md-2">
     <div class="bg-danger px-2 px-md-3 shadow-sm rounded-4 border border-danger">
       <div class="bg-dark px-2 px-md-3 rounded-4 shadow-sm">
@@ -392,19 +399,24 @@
       </section>
     {% endif %}
 
     <div class="row g-4 mb-4" aria-label="{% translate 'Main content' %}">
       <section class="col-12 col-lg-8 order-last order-lg-first" role="main" aria-label="{% translate 'Main content' %}">
         <div class="card card-body rounded-4 p-4 shadow-sm">
           <div class="request-info" aria-label="{% translate 'Request info' %}">
-            <pre class="prettyprint"><b>{{ request.method }}</b> {{ request.get_full_path }}</pre>
+            <pre class="prettyprint"><code class="language-http" style="padding: 0; background-color: transparent;">{{ request.method }} {{ request.get_full_path }}</code></pre>
           </div>
 
           <div class="response-info" aria-label="{% translate 'response info' %}">
-            <pre class="prettyprint d-grid gap-4"><div class="overflow-auto"><div><strong>HTTP {{ response.status_code }} {{ response.status_text }}</strong></div>{% for key, val in response_headers|items %}<div><strong>{{ key }}:</strong> <span class="lit">{{ val|break_long_headers|urlize }}</span></div>{% endfor %}</div><code>{{ content|urlize }}</code></pre>
+<pre class="prettyprint d-grid gap-4">
+<code class="language-http" style="padding: 0; background-color: transparent;">HTTP {{ response.status_code }} {{ response.status_text }}
+{% for key, val in response_headers|items %}{{ key }}: {{ val|break_long_headers|urlize }}
+{% endfor %}</code>
+<code class="language-json" style="padding: 0; background-color: transparent;">{{ content|urlize }}</code>
+</pre>
           </div>
         </div>
       </section>
 
       <section class="col-12 col-lg-4">
         {% if display_edit_forms %}
           {% if post_form or raw_data_post_form %}
@@ -569,13 +581,16 @@
   {{ filter_form }}
 {% endif %}
 
 {% block script %}
   {{ block.super }}
   <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"
     integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" crossorigin="anonymous"></script>
+  <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/highlight.min.js"></script>
+  <script src="https://cdnjs.cloudflare.com/ajax/libs/highlight.js/11.9.0/languages/http.min.js"></script>
+  <script>hljs.highlightAll()</script>
 
   <script>
     const tooltipTriggerList = document.querySelectorAll('[data-bs-toggle="tooltip"]')
     const tooltipList = [...tooltipTriggerList].map(tooltipTriggerEl => new bootstrap.Tooltip(tooltipTriggerEl))
   </script>
 {% endblock %}
```

### Comparing `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/filters/base.html` & `drf_redesign-0.3.4/drf_redesign/templates/rest_framework/filters/base.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/filters/ordering.html` & `drf_redesign-0.3.4/drf_redesign/templates/rest_framework/filters/ordering.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/filters/search.html` & `drf_redesign-0.3.4/drf_redesign/templates/rest_framework/filters/search.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/checkbox.html` & `drf_redesign-0.3.4/drf_redesign/templates/rest_framework/horizontal/checkbox.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/checkbox_multiple.html` & `drf_redesign-0.3.4/drf_redesign/templates/rest_framework/horizontal/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/input.html` & `drf_redesign-0.3.4/drf_redesign/templates/rest_framework/horizontal/input.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/radio.html` & `drf_redesign-0.3.4/drf_redesign/templates/rest_framework/horizontal/radio.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/select.html` & `drf_redesign-0.3.4/drf_redesign/templates/rest_framework/horizontal/select.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/select_multiple.html` & `drf_redesign-0.3.4/drf_redesign/templates/rest_framework/horizontal/select_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/horizontal/textarea.html` & `drf_redesign-0.3.4/drf_redesign/templates/rest_framework/horizontal/textarea.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/checkbox.html` & `drf_redesign-0.3.4/drf_redesign/templates/rest_framework/inline/checkbox.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/checkbox_multiple.html` & `drf_redesign-0.3.4/drf_redesign/templates/rest_framework/inline/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/input.html` & `drf_redesign-0.3.4/drf_redesign/templates/rest_framework/inline/input.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/radio.html` & `drf_redesign-0.3.4/drf_redesign/templates/rest_framework/inline/radio.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/select.html` & `drf_redesign-0.3.4/drf_redesign/templates/rest_framework/inline/select.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/select_multiple.html` & `drf_redesign-0.3.4/drf_redesign/templates/rest_framework/inline/select_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/inline/textarea.html` & `drf_redesign-0.3.4/drf_redesign/templates/rest_framework/inline/textarea.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/login.html` & `drf_redesign-0.3.4/drf_redesign/templates/rest_framework/login.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/pagination/numbers.html` & `drf_redesign-0.3.4/drf_redesign/templates/rest_framework/pagination/numbers.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/pagination/previous_and_next.html` & `drf_redesign-0.3.4/drf_redesign/templates/rest_framework/pagination/previous_and_next.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/checkbox.html` & `drf_redesign-0.3.4/drf_redesign/templates/rest_framework/vertical/checkbox.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/checkbox_multiple.html` & `drf_redesign-0.3.4/drf_redesign/templates/rest_framework/vertical/checkbox_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/input.html` & `drf_redesign-0.3.4/drf_redesign/templates/rest_framework/vertical/input.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/radio.html` & `drf_redesign-0.3.4/drf_redesign/templates/rest_framework/vertical/radio.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/select.html` & `drf_redesign-0.3.4/drf_redesign/templates/rest_framework/vertical/select.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/select_multiple.html` & `drf_redesign-0.3.4/drf_redesign/templates/rest_framework/vertical/select_multiple.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/drf_redesign/templates/rest_framework/vertical/textarea.html` & `drf_redesign-0.3.4/drf_redesign/templates/rest_framework/vertical/textarea.html`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/drf_redesign/templatetags/rest_framework_redesign.py` & `drf_redesign-0.3.4/drf_redesign/templatetags/rest_framework_redesign.py`

 * *Files identical despite different names*

### Comparing `drf_redesign-0.3.3/pyproject.toml` & `drf_redesign-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "drf-redesign"
-version = "0.3.3"
+version = "0.3.4"
 description = "Redesign of the browse-able api of Django REST Framework with Bootstrap 5"
 authors = ["Yousef Abu Shanab <josephyousef249@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "drf_redesign"}]
 homepage = "https://github.com/youzarsiph/drf-redesign/"
 repository = "https://github.com/youzarsiph/drf-redesign/"
```

### Comparing `drf_redesign-0.3.3/PKG-INFO` & `drf_redesign-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drf-redesign
-Version: 0.3.3
+Version: 0.3.4
 Summary: Redesign of the browse-able api of Django REST Framework with Bootstrap 5
 Home-page: https://github.com/youzarsiph/drf-redesign/
 License: MIT
 Author: Yousef Abu Shanab
 Author-email: josephyousef249@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
```

