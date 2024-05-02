# Comparing `tmp/cast_bootstrap5-0.0.8.tar.gz` & `tmp/cast_bootstrap5-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cast_bootstrap5-0.0.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cast_bootstrap5-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cast_bootstrap5-0.0.8.tar` & `cast_bootstrap5-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     3077 2023-05-14 19:45:16.622485 cast_bootstrap5-0.0.8/.gitignore
--rw-r--r--   0        0        0     1281 2023-05-14 19:46:05.392913 cast_bootstrap5-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1505 2023-05-14 05:53:16.406076 cast_bootstrap5-0.0.8/LICENSE
--rw-r--r--   0        0        0     1212 2023-05-14 19:45:16.622564 cast_bootstrap5-0.0.8/README.md
--rw-r--r--   0        0        0       63 2023-09-02 07:27:25.125244 cast_bootstrap5-0.0.8/cast_bootstrap5/__init__.py
--rw-r--r--   0        0        0      104 2023-05-14 06:02:59.592444 cast_bootstrap5-0.0.8/cast_bootstrap5/apps.py
--rw-r--r--   0        0        0   194902 2023-05-14 19:45:16.623441 cast_bootstrap5-0.0.8/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/bootstrap.min.css
--rw-r--r--   0        0        0   522640 2023-05-14 19:45:16.626769 cast_bootstrap5-0.0.8/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/bootstrap.min.css.map
--rw-r--r--   0        0        0     6287 2023-05-14 12:11:23.910525 cast_bootstrap5-0.0.8/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/cast.css
--rw-r--r--   0        0        0    80421 2023-05-14 19:45:16.623332 cast_bootstrap5-0.0.8/cast_bootstrap5/static/cast_bootstrap5/js/bootstrap5/bootstrap.bundle.min.js
--rw-r--r--   0        0        0   333079 2023-05-14 19:45:16.623393 cast_bootstrap5-0.0.8/cast_bootstrap5/static/cast_bootstrap5/js/bootstrap5/bootstrap.bundle.min.js.map
--rw-r--r--   0        0        0    42820 2023-05-14 19:45:16.626371 cast_bootstrap5-0.0.8/cast_bootstrap5/static/cast_bootstrap5/js/htmx.min.js
--rw-r--r--   0        0        0    87533 1991-10-18 12:00:00.000000 cast_bootstrap5-0.0.8/cast_bootstrap5/static/cast_bootstrap5/js/jquery/jquery-3.7.1.min.js
--rw-r--r--   0        0        0      196 2023-05-14 05:59:16.067158 cast_bootstrap5-0.0.8/cast_bootstrap5/templates/cast/bootstrap5/400.html
--rw-r--r--   0        0        0      184 2023-05-14 05:59:16.067612 cast_bootstrap5-0.0.8/cast_bootstrap5/templates/cast/bootstrap5/403.html
--rw-r--r--   0        0        0      200 2023-05-14 05:59:16.068027 cast_bootstrap5-0.0.8/cast_bootstrap5/templates/cast/bootstrap5/403_csrf.html
--rw-r--r--   0        0        0      198 2023-05-14 05:59:16.068410 cast_bootstrap5-0.0.8/cast_bootstrap5/templates/cast/bootstrap5/404.html
--rw-r--r--   0        0        0      319 2023-05-14 05:59:16.068832 cast_bootstrap5-0.0.8/cast_bootstrap5/templates/cast/bootstrap5/500.html
--rw-r--r--   0        0        0      748 2023-05-14 05:59:16.069442 cast_bootstrap5-0.0.8/cast_bootstrap5/templates/cast/bootstrap5/_list_of_posts_and_paging_controls.html
--rw-r--r--   0        0        0     3568 2023-08-31 17:30:26.644733 cast_bootstrap5-0.0.8/cast_bootstrap5/templates/cast/bootstrap5/base.html
--rw-r--r--   0        0        0     2984 2023-09-01 22:41:26.328791 cast_bootstrap5-0.0.8/cast_bootstrap5/templates/cast/bootstrap5/blog_list_of_posts.html
--rw-r--r--   0        0        0      213 2023-05-14 05:59:16.070689 cast_bootstrap5-0.0.8/cast_bootstrap5/templates/cast/bootstrap5/episode.html
--rw-r--r--   0        0        0     2367 2023-05-14 05:59:16.071108 cast_bootstrap5-0.0.8/cast_bootstrap5/templates/cast/bootstrap5/pagination.html
--rw-r--r--   0        0        0     1919 2023-08-30 06:25:48.894856 cast_bootstrap5-0.0.8/cast_bootstrap5/templates/cast/bootstrap5/post.html
--rw-r--r--   0        0        0      573 2023-05-14 05:59:16.071911 cast_bootstrap5-0.0.8/cast_bootstrap5/templates/cast/bootstrap5/post_body.html
--rw-r--r--   0        0        0     1267 2023-09-02 07:23:58.839321 cast_bootstrap5-0.0.8/cast_bootstrap5/templates/cast/bootstrap5/select_theme.html
--rw-r--r--   0        0        0     1431 2023-05-16 20:47:59.028895 cast_bootstrap5-0.0.8/cast_bootstrap5/templates/cast/gallery.html
--rw-r--r--   0        0        0     2146 2023-05-14 07:08:10.337131 cast_bootstrap5-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1929 1970-01-01 00:00:00.000000 cast_bootstrap5-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     3077 2023-05-14 19:45:16.622485 cast_bootstrap5-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1281 2023-05-14 19:46:05.392913 cast_bootstrap5-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1505 2023-05-14 05:53:16.406076 cast_bootstrap5-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1212 2023-05-14 19:45:16.622564 cast_bootstrap5-0.0.9/README.md
+-rw-r--r--   0        0        0       63 2023-09-03 19:35:56.096390 cast_bootstrap5-0.0.9/cast_bootstrap5/__init__.py
+-rw-r--r--   0        0        0      104 2023-05-14 06:02:59.592444 cast_bootstrap5-0.0.9/cast_bootstrap5/apps.py
+-rw-r--r--   0        0        0   194902 2023-05-14 19:45:16.623441 cast_bootstrap5-0.0.9/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/bootstrap.min.css
+-rw-r--r--   0        0        0   522640 2023-05-14 19:45:16.626769 cast_bootstrap5-0.0.9/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/bootstrap.min.css.map
+-rw-r--r--   0        0        0     6287 2023-05-14 12:11:23.910525 cast_bootstrap5-0.0.9/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/cast.css
+-rw-r--r--   0        0        0    80421 2023-05-14 19:45:16.623332 cast_bootstrap5-0.0.9/cast_bootstrap5/static/cast_bootstrap5/js/bootstrap5/bootstrap.bundle.min.js
+-rw-r--r--   0        0        0   333079 2023-05-14 19:45:16.623393 cast_bootstrap5-0.0.9/cast_bootstrap5/static/cast_bootstrap5/js/bootstrap5/bootstrap.bundle.min.js.map
+-rw-r--r--   0        0        0    42820 2023-05-14 19:45:16.626371 cast_bootstrap5-0.0.9/cast_bootstrap5/static/cast_bootstrap5/js/htmx.min.js
+-rw-r--r--   0        0        0    87533 1991-10-18 12:00:00.000000 cast_bootstrap5-0.0.9/cast_bootstrap5/static/cast_bootstrap5/js/jquery/jquery-3.7.1.min.js
+-rw-r--r--   0        0        0      196 2023-05-14 05:59:16.067158 cast_bootstrap5-0.0.9/cast_bootstrap5/templates/cast/bootstrap5/400.html
+-rw-r--r--   0        0        0      184 2023-05-14 05:59:16.067612 cast_bootstrap5-0.0.9/cast_bootstrap5/templates/cast/bootstrap5/403.html
+-rw-r--r--   0        0        0      200 2023-05-14 05:59:16.068027 cast_bootstrap5-0.0.9/cast_bootstrap5/templates/cast/bootstrap5/403_csrf.html
+-rw-r--r--   0        0        0      198 2023-05-14 05:59:16.068410 cast_bootstrap5-0.0.9/cast_bootstrap5/templates/cast/bootstrap5/404.html
+-rw-r--r--   0        0        0      319 2023-05-14 05:59:16.068832 cast_bootstrap5-0.0.9/cast_bootstrap5/templates/cast/bootstrap5/500.html
+-rw-r--r--   0        0        0      748 2023-05-14 05:59:16.069442 cast_bootstrap5-0.0.9/cast_bootstrap5/templates/cast/bootstrap5/_list_of_posts_and_paging_controls.html
+-rw-r--r--   0        0        0     3568 2023-08-31 17:30:26.644733 cast_bootstrap5-0.0.9/cast_bootstrap5/templates/cast/bootstrap5/base.html
+-rw-r--r--   0        0        0     2984 2023-09-01 22:41:26.328791 cast_bootstrap5-0.0.9/cast_bootstrap5/templates/cast/bootstrap5/blog_list_of_posts.html
+-rw-r--r--   0        0        0      213 2023-05-14 05:59:16.070689 cast_bootstrap5-0.0.9/cast_bootstrap5/templates/cast/bootstrap5/episode.html
+-rw-r--r--   0        0        0     2367 2023-05-14 05:59:16.071108 cast_bootstrap5-0.0.9/cast_bootstrap5/templates/cast/bootstrap5/pagination.html
+-rw-r--r--   0        0        0     1919 2023-08-30 06:25:48.894856 cast_bootstrap5-0.0.9/cast_bootstrap5/templates/cast/bootstrap5/post.html
+-rw-r--r--   0        0        0      573 2023-05-14 05:59:16.071911 cast_bootstrap5-0.0.9/cast_bootstrap5/templates/cast/bootstrap5/post_body.html
+-rw-r--r--   0        0        0     1362 2023-09-03 11:50:09.874503 cast_bootstrap5-0.0.9/cast_bootstrap5/templates/cast/bootstrap5/select_theme.html
+-rw-r--r--   0        0        0     1431 2023-05-16 20:47:59.028895 cast_bootstrap5-0.0.9/cast_bootstrap5/templates/cast/gallery.html
+-rw-r--r--   0        0        0     2146 2023-05-14 07:08:10.337131 cast_bootstrap5-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1929 1970-01-01 00:00:00.000000 cast_bootstrap5-0.0.9/PKG-INFO
```

### Comparing `cast_bootstrap5-0.0.8/.gitignore` & `cast_bootstrap5-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.8/.pre-commit-config.yaml` & `cast_bootstrap5-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.8/LICENSE` & `cast_bootstrap5-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.8/README.md` & `cast_bootstrap5-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.8/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/bootstrap.min.css` & `cast_bootstrap5-0.0.9/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.8/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/bootstrap.min.css.map` & `cast_bootstrap5-0.0.9/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.8/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/cast.css` & `cast_bootstrap5-0.0.9/cast_bootstrap5/static/cast_bootstrap5/css/bootstrap5/cast.css`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.8/cast_bootstrap5/static/cast_bootstrap5/js/bootstrap5/bootstrap.bundle.min.js` & `cast_bootstrap5-0.0.9/cast_bootstrap5/static/cast_bootstrap5/js/bootstrap5/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.8/cast_bootstrap5/static/cast_bootstrap5/js/bootstrap5/bootstrap.bundle.min.js.map` & `cast_bootstrap5-0.0.9/cast_bootstrap5/static/cast_bootstrap5/js/bootstrap5/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.8/cast_bootstrap5/static/cast_bootstrap5/js/htmx.min.js` & `cast_bootstrap5-0.0.9/cast_bootstrap5/static/cast_bootstrap5/js/htmx.min.js`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.8/cast_bootstrap5/static/cast_bootstrap5/js/jquery/jquery-3.7.1.min.js` & `cast_bootstrap5-0.0.9/cast_bootstrap5/static/cast_bootstrap5/js/jquery/jquery-3.7.1.min.js`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.8/cast_bootstrap5/templates/cast/bootstrap5/_list_of_posts_and_paging_controls.html` & `cast_bootstrap5-0.0.9/cast_bootstrap5/templates/cast/bootstrap5/_list_of_posts_and_paging_controls.html`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.8/cast_bootstrap5/templates/cast/bootstrap5/base.html` & `cast_bootstrap5-0.0.9/cast_bootstrap5/templates/cast/bootstrap5/base.html`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.8/cast_bootstrap5/templates/cast/bootstrap5/blog_list_of_posts.html` & `cast_bootstrap5-0.0.9/cast_bootstrap5/templates/cast/bootstrap5/blog_list_of_posts.html`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.8/cast_bootstrap5/templates/cast/bootstrap5/pagination.html` & `cast_bootstrap5-0.0.9/cast_bootstrap5/templates/cast/bootstrap5/pagination.html`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.8/cast_bootstrap5/templates/cast/bootstrap5/post.html` & `cast_bootstrap5-0.0.9/cast_bootstrap5/templates/cast/bootstrap5/post.html`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.8/cast_bootstrap5/templates/cast/bootstrap5/post_body.html` & `cast_bootstrap5-0.0.9/cast_bootstrap5/templates/cast/bootstrap5/post_body.html`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.8/cast_bootstrap5/templates/cast/bootstrap5/select_theme.html` & `cast_bootstrap5-0.0.9/cast_bootstrap5/templates/cast/bootstrap5/select_theme.html`

 * *Files 15% similar despite different names*

```diff
@@ -5,19 +5,19 @@
       <path d="M5.062 12h3.475c1.804 0 2.888-.908 2.888-2.396 0-1.102-.761-1.916-1.904-2.034v-.1c.832-.14 1.482-.93 1.482-1.816 0-1.3-.955-2.11-2.542-2.11H5.062V12zm1.313-4.875V4.658h1.78c.973 0 1.542.457 1.542 1.237 0 .802-.604 1.23-1.764 1.23H6.375zm0 3.762V8.162h1.822c1.236 0 1.887.463 1.887 1.348 0 .896-.627 1.377-1.811 1.377H6.375z"/>
       <path d="M0 4a4 4 0 0 1 4-4h8a4 4 0 0 1 4 4v8a4 4 0 0 1-4 4H4a4 4 0 0 1-4-4V4zm4-3a3 3 0 0 0-3 3v8a3 3 0 0 0 3 3h8a3 3 0 0 0 3-3V4a3 3 0 0 0-3-3H4z"/>
     </svg>
   </button>
   <ul class="dropdown-menu dropdown-menu-light">
     {% for theme_slug, theme_name in template_base_dir_choices %}
       <li>
-        <a class="dropdown-item"
-           hx-post="{% url 'cast:select-theme' %}"
-           hx-vals='{"template_base_dir": "{{ theme_slug }}", "next": "{{ next_url }}"}'
-           hx-trigger="click"
-           href="#"
-        >
-          {{ theme_name }}
-        </a>
+        <form action="{% url 'cast:select-theme' %}" method="post">
+          {% csrf_token %}
+          <input type="hidden" name="template_base_dir" value="{{ theme_slug }}">
+          <input type="hidden" name="next" value="{{ next_url }}">
+          <button type="submit" class="btn dropdown-item">
+            {{ theme_name }}
+          </button>
+        </form>
       </li>
     {% endfor %}
   </ul>
 </li>
```

### Comparing `cast_bootstrap5-0.0.8/cast_bootstrap5/templates/cast/gallery.html` & `cast_bootstrap5-0.0.9/cast_bootstrap5/templates/cast/gallery.html`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.8/pyproject.toml` & `cast_bootstrap5-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cast_bootstrap5-0.0.8/PKG-INFO` & `cast_bootstrap5-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cast-bootstrap5
-Version: 0.0.8
+Version: 0.0.9
 Summary: Bootstrap5 theme for django-cast
 Keywords: blog,podcast,video,audio
 Author-email: Jochen Wersdörfer <jochen-castbootstrap5@wersdoerfer.de>
 Requires-Python: >=3.9
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.0
```

