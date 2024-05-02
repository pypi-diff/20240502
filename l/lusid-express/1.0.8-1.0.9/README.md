# Comparing `tmp/lusid_express-1.0.8.tar.gz` & `tmp/lusid_express-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lusid_express-1.0.8.tar", last modified: Sat Apr 27 19:41:53 2024, max compression
+gzip compressed data, was "lusid_express-1.0.9.tar", last modified: Sat Apr 27 22:22:16 2024, max compression
```

## Comparing `lusid_express-1.0.8.tar` & `lusid_express-1.0.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:41:53.575486 lusid_express-1.0.8/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-27 19:41:12.000000 lusid_express-1.0.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-27 19:41:12.000000 lusid_express-1.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6659 2024-04-27 19:41:53.575486 lusid_express-1.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6019 2024-04-27 19:41:12.000000 lusid_express-1.0.8/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-27 19:41:53.575486 lusid_express-1.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-27 19:41:12.000000 lusid_express-1.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:41:53.569486 lusid_express-1.0.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:41:53.571486 lusid_express-1.0.8/src/lusid_express/
--rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-27 19:41:12.000000 lusid_express-1.0.8/src/lusid_express/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5616 2024-04-27 19:41:12.000000 lusid_express-1.0.8/src/lusid_express/__main__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:41:53.573486 lusid_express-1.0.8/src/lusid_express/apis/
--rw-rw-rw-   0 root         (0) root         (0)  2240138 2024-04-27 19:41:53.000000 lusid_express-1.0.8/src/lusid_express/apis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:41:53.574486 lusid_express-1.0.8/src/lusid_express/config/
--rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-27 19:41:12.000000 lusid_express-1.0.8/src/lusid_express/config/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:41:53.575486 lusid_express-1.0.8/src/lusid_express/display/
--rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-27 19:41:12.000000 lusid_express-1.0.8/src/lusid_express/display/PRELOADED_VARS.md
--rw-rw-rw-   0 root         (0) root         (0)    10716 2024-04-27 19:41:12.000000 lusid_express-1.0.8/src/lusid_express/display/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2352 2024-04-27 19:41:12.000000 lusid_express-1.0.8/src/lusid_express/load.le
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 19:41:53.572486 lusid_express-1.0.8/src/lusid_express.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6659 2024-04-27 19:41:53.000000 lusid_express-1.0.8/src/lusid_express.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      482 2024-04-27 19:41:53.000000 lusid_express-1.0.8/src/lusid_express.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-27 19:41:53.000000 lusid_express-1.0.8/src/lusid_express.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      479 2024-04-27 19:41:53.000000 lusid_express-1.0.8/src/lusid_express.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2024-04-27 19:41:53.000000 lusid_express-1.0.8/src/lusid_express.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:22:16.803777 lusid_express-1.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-27 22:21:34.000000 lusid_express-1.0.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)       85 2024-04-27 22:21:34.000000 lusid_express-1.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6659 2024-04-27 22:22:16.803777 lusid_express-1.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6019 2024-04-27 22:21:34.000000 lusid_express-1.0.9/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-27 22:22:16.803777 lusid_express-1.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1536 2024-04-27 22:21:34.000000 lusid_express-1.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:22:16.797777 lusid_express-1.0.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:22:16.799777 lusid_express-1.0.9/src/lusid_express/
+-rw-rw-rw-   0 root         (0) root         (0)       30 2024-04-27 22:21:34.000000 lusid_express-1.0.9/src/lusid_express/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5616 2024-04-27 22:21:34.000000 lusid_express-1.0.9/src/lusid_express/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:22:16.800777 lusid_express-1.0.9/src/lusid_express/apis/
+-rw-rw-rw-   0 root         (0) root         (0)  2240138 2024-04-27 22:22:16.000000 lusid_express-1.0.9/src/lusid_express/apis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:22:16.802777 lusid_express-1.0.9/src/lusid_express/config/
+-rw-rw-rw-   0 root         (0) root         (0)      369 2024-04-27 22:21:34.000000 lusid_express-1.0.9/src/lusid_express/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:22:16.803777 lusid_express-1.0.9/src/lusid_express/display/
+-rw-rw-rw-   0 root         (0) root         (0)      518 2024-04-27 22:21:34.000000 lusid_express-1.0.9/src/lusid_express/display/PRELOADED_VARS.md
+-rw-rw-rw-   0 root         (0) root         (0)    11383 2024-04-27 22:21:34.000000 lusid_express-1.0.9/src/lusid_express/display/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2352 2024-04-27 22:21:34.000000 lusid_express-1.0.9/src/lusid_express/load.le
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-27 22:22:16.800777 lusid_express-1.0.9/src/lusid_express.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6659 2024-04-27 22:22:16.000000 lusid_express-1.0.9/src/lusid_express.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      482 2024-04-27 22:22:16.000000 lusid_express-1.0.9/src/lusid_express.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-27 22:22:16.000000 lusid_express-1.0.9/src/lusid_express.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      479 2024-04-27 22:22:16.000000 lusid_express-1.0.9/src/lusid_express.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2024-04-27 22:22:16.000000 lusid_express-1.0.9/src/lusid_express.egg-info/top_level.txt
```

### Comparing `lusid_express-1.0.8/LICENSE` & `lusid_express-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.8/PKG-INFO` & `lusid_express-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid_express
-Version: 1.0.8
+Version: 1.0.9
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `lusid_express-1.0.8/README.md` & `lusid_express-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.8/setup.py` & `lusid_express-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 ]
 
 
 
 
 setup(
     name='lusid_express',
-    version='1.0.8',
+    version='1.0.9',
     package_dir={'': 'src'},  # tells setuptools that packages are under src
     packages=find_packages(where='src'),  # tells setuptools to look for packages in src
     install_requires=requirements,
     description='lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.',
     long_description=open('README.md').read(),
     include_package_data=True,  
     long_description_content_type='text/markdown',
```

### Comparing `lusid_express-1.0.8/src/lusid_express/__main__.py` & `lusid_express-1.0.9/src/lusid_express/__main__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.8/src/lusid_express/apis/__init__.py` & `lusid_express-1.0.9/src/lusid_express/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.8/src/lusid_express/display/PRELOADED_VARS.md` & `lusid_express-1.0.9/src/lusid_express/display/PRELOADED_VARS.md`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.8/src/lusid_express/display/__init__.py` & `lusid_express-1.0.9/src/lusid_express/display/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -73,36 +73,35 @@
 }
 </style>
 <button 
 class="button"
 
 onclick='copyTable("REPLACEMENT_HOOK")'>Copy to Clipboard</button>
  <script>
+
 function copyTable(tableId) {
     var table = document.getElementById(tableId);
     if (!table) {
         alert("Table not found!");
         return;
     }
     var rows = table.querySelectorAll('tr');
     var csvContent = '';
     rows.forEach(function(row) {
-        var isExpandableRow = row.classList.contains('expandable');
         var cols = row.querySelectorAll('th, td');
         var rowData = [];
         cols.forEach(function(col) {
-            // Skip cells that contain the 'expand-link' class or are in expandable rows
-            if (!col.querySelector('.expand-link') && !isExpandableRow) {
-                var text = col.innerText.replace(/(\r\n|\n|\r)/gm, '').trim();
+
+                var text = col.innerText.replace(/(\\r\\n|\\n|\\r)/gm, '').trim();
                 rowData.push(text);
-            }
+
         });
         // Only add non-empty rows to the CSV content
-        if (rowData.length > 0 && !isExpandableRow) {
-            csvContent += rowData.join('\t') + '\n';
+        if (rowData.length > 0 ) {
+            csvContent += rowData.join('\\t') + '\\n';
         }
     });
     // Create a temporary textarea element to copy the content
     var el = document.createElement('textarea');
     el.value = csvContent;
     document.body.appendChild(el);
     el.select();
@@ -205,15 +204,17 @@
     border-color: #FF5500;
     color: #FF5500
 }
     tr:nth-child(odd) td {
     border-color: #415464;
     color: #FF5500;
 }
-
+.muted-text {
+    color: #728A9F !important;
+}
 </style>
 
 """
 }
 
 
 def __convert_data(data):
@@ -253,39 +254,54 @@
         col_name_key (str): Custom name for the column header of the keys.
         col_name_value (str): Custom name for the column header of the values.
         title (str): Title of the table.
     """
 
     table = ""
 
+    def format_url(text):
+        """ Check if the text is a URL and format it as a hyperlink if true. """
+        url_pattern = __re.compile(r'https?://[^\s]+')
+        if isinstance(text, str) and url_pattern.match(text):
+            return f"<a href='{text}' target='_blank'>{text}</a>"
+        return text
 
-
-    def get_rows(key, value, depth=0):
-        """ Generate HTML rows for any nested structures, with CSS class and non-breaking spaces for indentation """
+    def get_rows(key, value, depth=0,is_list_item=False):
+        """ Generate HTML rows for any nested structures, making URLs clickable. """
         rows = ""
         nbsp_indent = "&nbsp;" * (depth * 4)  # Non-breaking spaces for indentation
         indent_class = f"indent-{depth}"  # CSS class for indentation
+        muted_class = "muted-text" if depth > 0 or is_list_item else ""
 
         if isinstance(value, dict):
-            # Include the key for the dictionary
-            rows += f"<tr><td class='{indent_class}'>{nbsp_indent}<strong>{key}</strong></td><td></td></tr>"
-            # Recursively handle dictionary items
+            # Handle dictionaries by recursively adding rows for each key-value pair
+            rows += f"<tr><td class='{indent_class} {muted_class}'>{nbsp_indent}<strong>{key}</strong></td><td></td></tr>"
             for sub_key, sub_value in value.items():
                 rows += get_rows(sub_key, sub_value, depth + 1)
         elif isinstance(value, list):
-            # Start with the key for the list
-            rows += f"<tr><td class='{indent_class}'>{nbsp_indent}<strong>{key}</strong></td><td>{str(value[0]) if value else '(empty list)'}</td></tr>"
-            # Continue with the rest of the items without the key
-            for item in value[1:]:
-                rows += f"<tr><td class='{indent_class}'>{nbsp_indent}</td><td>{str(item)}</td></tr>"
+            # Handle lists and check if the first item is a dictionary
+            rows += f"<tr><td class='{indent_class} {muted_class}'>{nbsp_indent}<strong>{key}</strong></td><td></td></tr>"
+            for item in value:
+                if isinstance(item, dict):
+                    # Expand dictionary items
+                    for sub_key, sub_value in item.items():
+                        rows += get_rows(sub_key, sub_value, depth + 1,is_list_item=True)
+                else:
+                    # Format item as URL if applicable, and handle regular list items
+                    formatted_item = format_url(item)
+                    rows += f"<tr><td class='{indent_class} muted-text'>{nbsp_indent}</td><td class='muted-text'>{formatted_item}</td></tr>"
         else:
-            # Handle simple key-value pairs
-            rows += f"<tr><td class='{indent_class}'>{nbsp_indent}<strong>{key}</strong></td><td>{str(value)}</td></tr>"
+            # Handle simple key-value pairs and format as URL if applicable
+            display_value = format_url(value)
+            rows += f"<tr><td class='{indent_class} {muted_class}'>{nbsp_indent}<strong>{key}</strong></td><td class='{muted_class}'>{display_value}</td></tr>"
+
         return rows
 
+
+
     
     def clean(data):
         if isinstance(data, dict):
             return {k: clean(v) for k, v in data.items() if v is not None}
         elif isinstance(data, list):
             return [clean(item) for item in data if item is not None]
         else:
@@ -296,14 +312,15 @@
     table = ""
     for key, value in data.items():
         table += get_rows(key, value)
 
     # Ensure the table ID is correctly set and used in the COPY_SCRIPT
     table_id = f"DATA_TABLE-{__uuid.uuid4()}"  # Unique ID for each table instance
     html_output = f"""<h1>{title}</h1> <table id='{table_id}'><tr><th>{col_name_key}</th><th>{col_name_value}</th></tr>{table}</table>{COPY_SCRIPT.replace('REPLACEMENT_HOOK', table_id)}"""
+    print(html_output)
     return html_output
 
 def render_table(data, col_name_key="Key", col_name_value="Value", title="table"):
     """
     Renders table from data.
 
     Parameters:
```

### Comparing `lusid_express-1.0.8/src/lusid_express/load.le` & `lusid_express-1.0.9/src/lusid_express/load.le`

 * *Files identical despite different names*

### Comparing `lusid_express-1.0.8/src/lusid_express.egg-info/PKG-INFO` & `lusid_express-1.0.9/src/lusid_express.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lusid-express
-Version: 1.0.8
+Version: 1.0.9
 Summary: lusid-express is a python package that makes it quick and easy to get started using Lusid and Luminesce.
 Home-page: https://gitlab.com/orlando.calvo1/lusid-express
 Author: Orlando Calvo
 Author-email: orlando.calvo@finbourne.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

