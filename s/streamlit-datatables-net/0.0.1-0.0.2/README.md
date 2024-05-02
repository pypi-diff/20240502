# Comparing `tmp/streamlit_datatables_net-0.0.1-py3-none-any.whl.zip` & `tmp/streamlit_datatables_net-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 3477 bytes, number of entries: 5
--rw-r--r--  2.0 unx     4660 b- defN 24-May-02 19:59 streamlit_datatables_net/__init__.py
--rw-r--r--  2.0 unx      694 b- defN 24-May-02 19:59 streamlit_datatables_net-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-02 19:59 streamlit_datatables_net-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       25 b- defN 24-May-02 19:59 streamlit_datatables_net-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      458 b- defN 24-May-02 19:59 streamlit_datatables_net-0.0.1.dist-info/RECORD
-5 files, 5929 bytes uncompressed, 2611 bytes compressed:  56.0%
+Zip file size: 3490 bytes, number of entries: 5
+-rw-r--r--  2.0 unx     4820 b- defN 24-May-02 20:24 streamlit_datatables_net/__init__.py
+-rw-r--r--  2.0 unx      694 b- defN 24-May-02 20:24 streamlit_datatables_net-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-02 20:24 streamlit_datatables_net-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       25 b- defN 24-May-02 20:24 streamlit_datatables_net-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      458 b- defN 24-May-02 20:24 streamlit_datatables_net-0.0.2.dist-info/RECORD
+5 files, 6089 bytes uncompressed, 2624 bytes compressed:  56.9%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: streamlit_datatables_net/__init__.py
 Comment: 
 
-Filename: streamlit_datatables_net-0.0.1.dist-info/METADATA
+Filename: streamlit_datatables_net-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: streamlit_datatables_net-0.0.1.dist-info/WHEEL
+Filename: streamlit_datatables_net-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: streamlit_datatables_net-0.0.1.dist-info/top_level.txt
+Filename: streamlit_datatables_net-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: streamlit_datatables_net-0.0.1.dist-info/RECORD
+Filename: streamlit_datatables_net-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## streamlit_datatables_net/__init__.py

```diff
@@ -8,44 +8,45 @@
 st.set_page_config(layout="wide")
 
 
 # Create a _RELEASE constant. We'll set this to False while we're developing
 # the component, and True when we're ready to package and distribute it.
 # (This is, of course, optional - there are innumerable ways to manage your
 # release process.)
-_RELEASE = False
+_RELEASE = True
 
 # Declare a Streamlit component. `declare_component` returns a function
 # that is used to create instances of the component. We're naming this
 # function "_component_func", with an underscore prefix, because we don't want
 # to expose it directly to users. Instead, we will create a custom wrapper
 # function, below, that will serve as our component's public API.
 
 # It's worth noting that this call to `declare_component` is the
 # *only thing* you need to do to create the binding between Streamlit and
 # your component frontend. Everything else we do in this file is simply a
 # best practice.
 
-if not _RELEASE:
-    _component_func = components.declare_component(
-        "streamlit_datatables_net",
-        # Pass `url` here to tell Streamlit that the component will be served
-        # by the local dev server that you run via `npm run start`.
-        # (This is useful while your component is in development.)
-        url="http://localhost:3001",
-    )
-else:
+if _RELEASE:
     # When we're distributing a production version of the component, we'll
     # replace the `url` param with `path`, and point it to the component's
     # build directory:
     parent_dir = os.path.dirname(os.path.abspath(__file__))
     build_dir = os.path.join(parent_dir, "frontend/build")
     _component_func = components.declare_component(
         "streamlit_datatables_net", path=build_dir)
 
+else:
+    _component_func = components.declare_component(
+        "streamlit_datatables_net",
+        # Pass `url` here to tell Streamlit that the component will be served
+        # by the local dev server that you run via `npm run start`.
+        # (This is useful while your component is in development.)
+        url="http://localhost:3001",
+    )
+
 # Create a wrapper function for the component. This is an optional
 # best practice - we could simply expose the component function returned by
 # `declare_component` and call it done. The wrapper allows us to customize
 # our component's API: we can pre-process its input args, post-process its
 # output value, and add a docstring for users.
 
 
@@ -81,50 +82,50 @@
         props=props, class_name=class_name, stylesheets=stylesheets, key=key, default=0)
 
     # We could modify the value returned from the component if we wanted.
     # There's no need to do this in our simple example - but it's an option.
     return component_value
 
 
-data = [
-    {
-        "id": "1",
-        "name": "Tiger Nixon",
-        "position": "System Architect",
-        "salary": 320800,
-        "start_date": "2011/04/25",
-        "office": "Edinburgh",
-        "extn": "5421",
-    },
-    {
-        "id": "2",
-        "name": "Garrett Summers",
-        "position": "Accountant",
-        "salary": 170750,
-        "start_date": "2011/07/25",
-        "office": "Tokyo",
-        "extn": "8422",
-    },
-]
-
-columns = [
-    {"data": "name", "title": "Name"},
-    {"data": "position", "title": "Position"},
-    {"data": "office", "title": "Office"},
-    {"data": "salary", "title": "Salary",
-        "render": ['number', ',', '.', 0, '$']},
-]
-
-
-props = {}
-props["data"] = data
-props["columns"] = columns
-
-stylesheets = [
-    "https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css"]
-
-class_name = "compact row-border hover"
-
-col_l, col_m, col_r = st.columns([1, 10, 1])
-with col_m:
-    dt_response = streamlit_datatable(
-        props, class_name=None, stylesheets=stylesheets, key="bar")
+if not _RELEASE:
+    data = [
+        {
+            "id": "1",
+            "name": "Tiger Nixon",
+            "position": "System Architect",
+            "salary": 320800,
+            "start_date": "2011/04/25",
+            "office": "Edinburgh",
+            "extn": "5421",
+        },
+        {
+            "id": "2",
+            "name": "Garrett Summers",
+            "position": "Accountant",
+            "salary": 170750,
+            "start_date": "2011/07/25",
+            "office": "Tokyo",
+            "extn": "8422",
+        },
+    ]
+
+    columns = [
+        {"data": "name", "title": "Name"},
+        {"data": "position", "title": "Position"},
+        {"data": "office", "title": "Office"},
+        {"data": "salary", "title": "Salary",
+            "render": ['number', ',', '.', 0, '$']},
+    ]
+
+    props = {}
+    props["data"] = data
+    props["columns"] = columns
+
+    stylesheets = [
+        "https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css"]
+
+    class_name = "compact row-border hover"
+
+    col_l, col_m, col_r = st.columns([1, 10, 1])
+    with col_m:
+        dt_response = streamlit_datatable(
+            props, class_name=None, stylesheets=stylesheets, key="bar")
```

## Comparing `streamlit_datatables_net-0.0.1.dist-info/METADATA` & `streamlit_datatables_net-0.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-datatables-net
-Version: 0.0.1
+Version: 0.0.2
 Summary: Streamlit component for Datatables.net
 Home-page: 
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: streamlit >=0.63
 Provides-Extra: devel
 Requires-Dist: wheel ; extra == 'devel'
```

