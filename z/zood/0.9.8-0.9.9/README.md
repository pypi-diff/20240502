# Comparing `tmp/zood-0.9.8.tar.gz` & `tmp/zood-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zood-0.9.8.tar", max compression
+gzip compressed data, was "zood-0.9.9.tar", max compression
```

## Comparing `zood-0.9.8.tar` & `zood-0.9.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0      572 2024-03-18 03:36:20.359240 zood-0.9.8/pyproject.toml
--rw-r--r--   0        0        0      731 2023-10-18 11:45:31.458494 zood-0.9.8/README.md
--rw-r--r--   0        0        0       24 2023-01-06 12:50:33.818825 zood-0.9.8/zood/__init__.py
--rw-r--r--   0        0        0     4940 2024-02-17 14:31:07.055404 zood-0.9.8/zood/config/_config.yml
--rw-r--r--   0        0        0      236 2024-03-18 03:36:00.797266 zood-0.9.8/zood/config/error.log
--rw-r--r--   0        0        0      209 2022-12-30 16:25:34.984515 zood-0.9.8/zood/config/img/after_copy.png
--rw-r--r--   0        0        0      215 2022-12-30 15:33:16.742079 zood-0.9.8/zood/config/img/before_copy.png
--rw-r--r--   0        0        0     2720 2023-01-14 08:58:35.867485 zood-0.9.8/zood/config/img/enter.png
--rw-r--r--   0        0        0      247 2023-01-14 09:31:22.970712 zood-0.9.8/zood/config/img/enter.svg
--rw-r--r--   0        0        0      454 2022-12-30 16:25:01.986421 zood-0.9.8/zood/config/img/moon.png
--rw-r--r--   0        0        0      446 2023-01-13 11:27:05.445651 zood-0.9.8/zood/config/img/search.svg
--rw-r--r--   0        0        0      428 2022-12-30 16:24:58.219147 zood-0.9.8/zood/config/img/sun.png
--rw-r--r--   0        0        0    17308 2024-03-11 06:55:26.191672 zood-0.9.8/zood/config/index.css
--rw-r--r--   0        0        0     3991 2023-07-13 02:52:54.473602 zood-0.9.8/zood/config/js/change_mode.js
--rw-r--r--   0        0        0     2664 2023-09-24 03:12:51.445148 zood-0.9.8/zood/config/js/copy_code.js
--rw-r--r--   0        0        0     2276 2024-01-28 01:12:38.779532 zood-0.9.8/zood/config/js/global_js_configuration.js
--rw-r--r--   0        0        0     2916 2024-02-06 13:20:55.479733 zood-0.9.8/zood/config/js/navigator.js
--rw-r--r--   0        0        0     1120 2024-01-26 15:20:27.636640 zood-0.9.8/zood/config/js/next_front.js
--rw-r--r--   0        0        0   100811 2023-10-18 11:13:08.290210 zood-0.9.8/zood/config/js/picture_preview.js
--rw-r--r--   0        0        0      285 2023-01-02 13:48:40.110725 zood-0.9.8/zood/config/js/picture_title.js
--rw-r--r--   0        0        0      583 2023-07-29 15:25:41.350255 zood-0.9.8/zood/config/template.html
--rw-r--r--   0        0        0       69 2023-06-24 15:37:55.849962 zood-0.9.8/zood/extensions/__init__.py
--rw-r--r--   0        0        0     4224 2024-02-24 09:20:09.712629 zood-0.9.8/zood/extensions/poetry_update.py
--rw-r--r--   0        0        0     8446 2024-03-18 03:35:55.900786 zood-0.9.8/zood/gen_doc.py
--rw-r--r--   0        0        0     6555 2024-02-20 12:05:06.472105 zood-0.9.8/zood/main.py
--rw-r--r--   0        0        0     6022 2024-01-26 14:44:13.525835 zood-0.9.8/zood/util.py
--rw-r--r--   0        0        0     6916 2024-01-26 14:42:02.493631 zood-0.9.8/zood/zood.py
--rw-r--r--   0        0        0     1586 1970-01-01 00:00:00.000000 zood-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0      578 2024-03-24 08:03:28.482033 zood-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0      731 2023-10-18 11:45:31.458494 zood-0.9.9/README.md
+-rw-r--r--   0        0        0       24 2023-01-06 12:50:33.818825 zood-0.9.9/zood/__init__.py
+-rw-r--r--   0        0        0     4940 2024-02-17 14:31:07.055404 zood-0.9.9/zood/config/_config.yml
+-rw-r--r--   0        0        0        0 2024-03-24 08:02:27.045710 zood-0.9.9/zood/config/error.log
+-rw-r--r--   0        0        0      209 2022-12-30 16:25:34.984515 zood-0.9.9/zood/config/img/after_copy.png
+-rw-r--r--   0        0        0      215 2022-12-30 15:33:16.742079 zood-0.9.9/zood/config/img/before_copy.png
+-rw-r--r--   0        0        0     2720 2023-01-14 08:58:35.867485 zood-0.9.9/zood/config/img/enter.png
+-rw-r--r--   0        0        0      247 2023-01-14 09:31:22.970712 zood-0.9.9/zood/config/img/enter.svg
+-rw-r--r--   0        0        0      454 2022-12-30 16:25:01.986421 zood-0.9.9/zood/config/img/moon.png
+-rw-r--r--   0        0        0      446 2023-01-13 11:27:05.445651 zood-0.9.9/zood/config/img/search.svg
+-rw-r--r--   0        0        0      428 2022-12-30 16:24:58.219147 zood-0.9.9/zood/config/img/sun.png
+-rw-r--r--   0        0        0    17484 2024-03-24 08:01:44.401326 zood-0.9.9/zood/config/index.css
+-rw-r--r--   0        0        0     3991 2023-07-13 02:52:54.473602 zood-0.9.9/zood/config/js/change_mode.js
+-rw-r--r--   0        0        0     2664 2023-09-24 03:12:51.445148 zood-0.9.9/zood/config/js/copy_code.js
+-rw-r--r--   0        0        0     2276 2024-01-28 01:12:38.779532 zood-0.9.9/zood/config/js/global_js_configuration.js
+-rw-r--r--   0        0        0     2916 2024-02-06 13:20:55.479733 zood-0.9.9/zood/config/js/navigator.js
+-rw-r--r--   0        0        0     1120 2024-01-26 15:20:27.636640 zood-0.9.9/zood/config/js/next_front.js
+-rw-r--r--   0        0        0   100811 2023-10-18 11:13:08.290210 zood-0.9.9/zood/config/js/picture_preview.js
+-rw-r--r--   0        0        0      285 2023-01-02 13:48:40.110725 zood-0.9.9/zood/config/js/picture_title.js
+-rw-r--r--   0        0        0      583 2023-07-29 15:25:41.350255 zood-0.9.9/zood/config/template.html
+-rw-r--r--   0        0        0       69 2023-06-24 15:37:55.849962 zood-0.9.9/zood/extensions/__init__.py
+-rw-r--r--   0        0        0     4224 2024-02-24 09:20:09.712629 zood-0.9.9/zood/extensions/poetry_update.py
+-rw-r--r--   0        0        0     8446 2024-03-18 03:35:55.900786 zood-0.9.9/zood/gen_doc.py
+-rw-r--r--   0        0        0     6555 2024-02-20 12:05:06.472105 zood-0.9.9/zood/main.py
+-rw-r--r--   0        0        0     6022 2024-01-26 14:44:13.525835 zood-0.9.9/zood/util.py
+-rw-r--r--   0        0        0     6916 2024-01-26 14:42:02.493631 zood-0.9.9/zood/zood.py
+-rw-r--r--   0        0        0     1604 1970-01-01 00:00:00.000000 zood-0.9.9/PKG-INFO
```

### Comparing `zood-0.9.8/pyproject.toml` & `zood-0.9.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "zood"
-version = "0.9.8"
+version = "0.9.9"
 description = "web page documentation & comment generation documentation"
 license = "MIT"
 authors = ["kamilu <luzhixing12345@163.com>"]
 readme = "README.md"
 repository = "https://github.com/luzhixing12345/zood"
 documentation = "https://luzhixing12345.github.io/zood/"
 
 
 [tool.poetry.dependencies]
 python = "^3.7"
 PyYAML = "*"
 MarkdownParser = "^0.5.20"
-syntaxlight = '*'
+syntaxlight = '^0.1.36'
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 zood = 'zood.main:main'
```

### Comparing `zood-0.9.8/README.md` & `zood-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `zood-0.9.8/zood/config/_config.yml` & `zood-0.9.9/zood/config/_config.yml`

 * *Files identical despite different names*

### Comparing `zood-0.9.8/zood/config/img/enter.png` & `zood-0.9.9/zood/config/img/enter.png`

 * *Files identical despite different names*

### Comparing `zood-0.9.8/zood/config/index.css` & `zood-0.9.9/zood/config/index.css`

 * *Files 1% similar despite different names*

```diff
@@ -203,25 +203,25 @@
 
 .markdown-body ul {
     padding-left: 0;
     margin-top: 0;
     margin-bottom: 0;
 }
 
-.markdown-body ol ol,
+/* .markdown-body ol ol,
 .markdown-body ul ol {
     list-style-type: lower-roman;
 }
 
 .markdown-body ol ol ol,
 .markdown-body ol ul ol,
 .markdown-body ul ol ol,
 .markdown-body ul ul ol {
     list-style-type: lower-alpha;
-}
+} */
 
 .markdown-body ul {
     margin-top: 0;
     margin-bottom: 8px;
 }
 
 .markdown-body ol,
@@ -358,14 +358,20 @@
 
 .markdown-body pre #code_copy:hover {
     background-color: #ffffff;
     box-shadow: rgba(149, 157, 165, 0.2) 0px 8px 24px;
     border-radius: 5px;
 }
 
+.markdown-body ol ul,
+.markdown-body ul ol {
+    padding-left: 1em;
+    margin-top: 10px;
+}
+
 .markdown-body ol li blockquote {
     margin-top: 10px;
 }
 
 .markdown-body ul li blockquote {
     margin-top: 10px;
 }
@@ -417,14 +423,16 @@
 }
 
 .next-front .change-article:active {
     width: 95%;
     height: 90px;
 }
 
+/* 对目录树的调整 */
+
 .dir-tree::-webkit-scrollbar {
     display: none;
     /* Chrome Safari */
 }
 
 .dir-tree {
     font-family: "<%font_family%>";
@@ -577,14 +585,16 @@
 }
 
 .markdown-body input[type="checkbox"] {
     margin-right: 0.5em;
     /* 复选框和文本之间的间距 */
 }
 
+/* 对小标题索引树的调整 */
+
 .header-navigator {
     display: none;
     position: fixed;
     width: "<%navigator_max_width%>";
     left: "<%navigator_left%>";
     top: "<%navigator_top%>";
     font-family: "<%font_family%>";
```

### Comparing `zood-0.9.8/zood/config/js/change_mode.js` & `zood-0.9.9/zood/config/js/change_mode.js`

 * *Files identical despite different names*

### Comparing `zood-0.9.8/zood/config/js/copy_code.js` & `zood-0.9.9/zood/config/js/copy_code.js`

 * *Files identical despite different names*

### Comparing `zood-0.9.8/zood/config/js/global_js_configuration.js` & `zood-0.9.9/zood/config/js/global_js_configuration.js`

 * *Files identical despite different names*

### Comparing `zood-0.9.8/zood/config/js/navigator.js` & `zood-0.9.9/zood/config/js/navigator.js`

 * *Files identical despite different names*

### Comparing `zood-0.9.8/zood/config/js/next_front.js` & `zood-0.9.9/zood/config/js/next_front.js`

 * *Files identical despite different names*

### Comparing `zood-0.9.8/zood/config/js/picture_preview.js` & `zood-0.9.9/zood/config/js/picture_preview.js`

 * *Files identical despite different names*

### Comparing `zood-0.9.8/zood/config/template.html` & `zood-0.9.9/zood/config/template.html`

 * *Files identical despite different names*

### Comparing `zood-0.9.8/zood/extensions/poetry_update.py` & `zood-0.9.9/zood/extensions/poetry_update.py`

 * *Files identical despite different names*

### Comparing `zood-0.9.8/zood/gen_doc.py` & `zood-0.9.9/zood/gen_doc.py`

 * *Files identical despite different names*

### Comparing `zood-0.9.8/zood/main.py` & `zood-0.9.9/zood/main.py`

 * *Files identical despite different names*

### Comparing `zood-0.9.8/zood/util.py` & `zood-0.9.9/zood/util.py`

 * *Files identical despite different names*

### Comparing `zood-0.9.8/zood/zood.py` & `zood-0.9.9/zood/zood.py`

 * *Files identical despite different names*

### Comparing `zood-0.9.8/PKG-INFO` & `zood-0.9.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zood
-Version: 0.9.8
+Version: 0.9.9
 Summary: web page documentation & comment generation documentation
 Home-page: https://github.com/luzhixing12345/zood
 License: MIT
 Author: kamilu
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: MarkdownParser (>=0.5.20,<0.6.0)
 Requires-Dist: PyYAML
-Requires-Dist: syntaxlight
+Requires-Dist: syntaxlight (>=0.1.36,<0.2.0)
 Project-URL: Documentation, https://luzhixing12345.github.io/zood/
 Project-URL: Repository, https://github.com/luzhixing12345/zood
 Description-Content-Type: text/markdown
 
 # zood
 
 zood 网页文档生成的 python 库, 可以将本地 Markdown 文件转为 Web 网页
```

