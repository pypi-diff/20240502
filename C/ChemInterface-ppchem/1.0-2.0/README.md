# Comparing `tmp/cheminterface_ppchem-1.0.tar.gz` & `tmp/cheminterface_ppchem-2.0.tar.gz`

## Comparing `cheminterface_ppchem-1.0.tar` & `cheminterface_ppchem-2.0.tar`

### file list

```diff
@@ -1,39 +1,50 @@
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/Project_ppchem.yml
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/insaturation.py
--rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/preliminary.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/setup.py
--rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/subgroups.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/.github/workflows/requirements.txt
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/.idea/misc.xml
--rw-r--r--   0        0        0     3871 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/.idea/workspace.xml
--rw-r--r--   0        0        0     4403 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/Bokeh/BOKEH_try.html
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/Bokeh/BOKEH_try.py
--rw-r--r--   0        0        0     5691 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/Bokeh/Bokeh try.py
--rw-r--r--   0        0        0    27677 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/Bokeh/Mass spectro display.html
--rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/Bokeh/Mass spectro display.py
--rw-r--r--   0        0        0   365917 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/Bokeh/Mol_display.html
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/Bokeh/Mol_display.py
--rw-r--r--   0        0        0    20922 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/Bokeh/callback.html
--rw-r--r--   0        0        0    50897 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/Bokeh/interactive_gaussian_plot.html
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/Bokeh/molecule_image.png
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/Bokeh/text.txt
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/Cheminterface/Tkinter_interface.py
--rw-r--r--   0        0        0     5280 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/THOMAS_IS_BEST/Preliminary_v2.py
--rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/THOMAS_IS_BEST/abundance.txt
--rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/THOMAS_IS_BEST/abundance_simplified.txt
--rw-r--r--   0        0        0    27522 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/THOMAS_IS_BEST/functions.html
--rw-r--r--   0        0        0    12589 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/THOMAS_IS_BEST/functions.py
--rw-r--r--   0        0        0      953 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/THOMAS_IS_BEST/test.py
--rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/Thomas/Copy_spectrometer.py
--rw-r--r--   0        0        0    49000 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/Thomas/Thomas_return.html
--rw-r--r--   0        0        0    27616 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/Thomas/Thomas_return_pyplot.html
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/Thomas/Thomas_return_pyplot.py
--rw-r--r--   0        0        0    27563 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/Thomas/functions.html
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/Thomas/random_tests.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/Thomas/tests.py
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/src/ChemInterface_ppchem/ChemInterface.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/src/ChemInterface_ppchem/__init__.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/LICENSE.txt
--rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/README.md
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/pyproject.toml
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 cheminterface_ppchem-1.0/PKG-INFO
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/insaturation.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/molecule_image.png
+-rw-r--r--   0        0        0     1816 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/preliminary.py
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/project_CH200.yml
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/setup.py
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/subgroups.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/.github/workflows/requirements.txt
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/.idea/misc.xml
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/.idea/modules.xml
+-rw-r--r--   0        0        0      291 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/.idea/ppchem-project-Christiansson-Gonteri-Humery.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/.idea/vcs.xml
+-rw-r--r--   0        0        0     3328 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/.idea/workspace.xml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     6532 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Bokeh/Bokeh try.py
+-rw-r--r--   0        0        0    53534 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Bokeh/Double plot bokeh.html
+-rw-r--r--   0        0        0     5994 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Bokeh/Double plot bokeh.py
+-rw-r--r--   0        0        0     9639 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Bokeh/Functional groups SMILES
+-rw-r--r--   0        0        0     7601 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Bokeh/Functional_group_finder.py
+-rw-r--r--   0        0        0    27677 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Bokeh/Mass spectro display.html
+-rw-r--r--   0        0        0     4365 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Bokeh/Mass spectro display.py
+-rw-r--r--   0        0        0     5959 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Bokeh/Mol_display.html
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Bokeh/Mol_display.py
+-rw-r--r--   0        0        0    20308 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Bokeh/callback.html
+-rw-r--r--   0        0        0     4978 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Bokeh/molecule_image.png
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Cheminterface/Tkinter_interface.py
+-rw-r--r--   0        0        0     5888 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/THOMAS_IS_BEST/Mol_display.html
+-rw-r--r--   0        0        0     1385 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/THOMAS_IS_BEST/Mol_display.py
+-rw-r--r--   0        0        0     5292 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/THOMAS_IS_BEST/Preliminary_v2.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/THOMAS_IS_BEST/abundance.txt
+-rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/THOMAS_IS_BEST/abundance_simplified.txt
+-rw-r--r--   0        0        0    14755 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/THOMAS_IS_BEST/copy_file.py
+-rw-r--r--   0        0        0    17100 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/THOMAS_IS_BEST/functions.py
+-rw-r--r--   0        0        0     3353 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/THOMAS_IS_BEST/molecule_image.png
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/THOMAS_IS_BEST/names.txt
+-rw-r--r--   0        0        0    19608 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/THOMAS_IS_BEST/test.py
+-rw-r--r--   0        0        0     5141 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Thomas/Copy_spectrometer.py
+-rw-r--r--   0        0        0    49000 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Thomas/Thomas_return.html
+-rw-r--r--   0        0        0    27616 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Thomas/Thomas_return_pyplot.html
+-rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Thomas/Thomas_return_pyplot.py
+-rw-r--r--   0        0        0    27563 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Thomas/functions.html
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Thomas/random_tests.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/Thomas/tests.py
+-rw-r--r--   0        0        0     5076 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/data/abundance.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/notebooks/test.ipynb
+-rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/src/ChemInterface_ppchem/ChemInterface.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/src/ChemInterface_ppchem/__init__.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/LICENSE.txt
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/README.md
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/pyproject.toml
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 cheminterface_ppchem-2.0/PKG-INFO
```

### Comparing `cheminterface_ppchem-1.0/insaturation.py` & `cheminterface_ppchem-2.0/insaturation.py`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-1.0/preliminary.py` & `cheminterface_ppchem-2.0/preliminary.py`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-1.0/subgroups.py` & `cheminterface_ppchem-2.0/subgroups.py`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-1.0/Bokeh/BOKEH_try.html` & `cheminterface_ppchem-2.0/THOMAS_IS_BEST/Mol_display.html`

 * *Files 20% similar despite different names*

```diff
@@ -14,27 +14,27 @@
     </style>
     <script type="text/javascript" src="https://cdn.bokeh.org/bokeh/release/bokeh-3.4.1.min.js"></script>
     <script type="text/javascript">
         Bokeh.set_log_level("info");
     </script>
   </head>
   <body>
-    <div id="e736f10d-e625-4fab-964b-af5fbe41e5c8" data-root-id="p1001" style="display: contents;"></div>
+    <div id="ae5708ad-472e-4b50-b9fe-ee5c821f1b30" data-root-id="p1001" style="display: contents;"></div>
   
-    <script type="application/json" id="c51ba175-b001-4ff6-833d-185361e733ff">
-      {"c79cfb15-fae5-422e-ab4f-7d753464a019":{"version":"3.4.1","title":"Bokeh Application","roots":[{"type":"object","name":"Figure","id":"p1001","attributes":{"x_range":{"type":"object","name":"DataRange1d","id":"p1002"},"y_range":{"type":"object","name":"DataRange1d","id":"p1003"},"x_scale":{"type":"object","name":"LinearScale","id":"p1010"},"y_scale":{"type":"object","name":"LinearScale","id":"p1011"},"title":{"type":"object","name":"Title","id":"p1008"},"toolbar":{"type":"object","name":"Toolbar","id":"p1009","attributes":{"tools":[{"type":"object","name":"PanTool","id":"p1022"},{"type":"object","name":"WheelZoomTool","id":"p1023","attributes":{"renderers":"auto"}},{"type":"object","name":"BoxZoomTool","id":"p1024","attributes":{"overlay":{"type":"object","name":"BoxAnnotation","id":"p1025","attributes":{"syncable":false,"level":"overlay","visible":false,"left":{"type":"number","value":"nan"},"right":{"type":"number","value":"nan"},"top":{"type":"number","value":"nan"},"bottom":{"type":"number","value":"nan"},"left_units":"canvas","right_units":"canvas","top_units":"canvas","bottom_units":"canvas","line_color":"black","line_alpha":1.0,"line_width":2,"line_dash":[4,4],"fill_color":"lightgrey","fill_alpha":0.5}}}},{"type":"object","name":"SaveTool","id":"p1030"},{"type":"object","name":"ResetTool","id":"p1031"},{"type":"object","name":"HelpTool","id":"p1032"}]}},"left":[{"type":"object","name":"LinearAxis","id":"p1017","attributes":{"ticker":{"type":"object","name":"BasicTicker","id":"p1018","attributes":{"mantissas":[1,2,5]}},"formatter":{"type":"object","name":"BasicTickFormatter","id":"p1019"},"major_label_policy":{"type":"object","name":"AllLabels","id":"p1020"}}}],"below":[{"type":"object","name":"LinearAxis","id":"p1012","attributes":{"ticker":{"type":"object","name":"BasicTicker","id":"p1013","attributes":{"mantissas":[1,2,5]}},"formatter":{"type":"object","name":"BasicTickFormatter","id":"p1014"},"major_label_policy":{"type":"object","name":"AllLabels","id":"p1015"}}}],"center":[{"type":"object","name":"Grid","id":"p1016","attributes":{"axis":{"id":"p1012"}}},{"type":"object","name":"Grid","id":"p1021","attributes":{"dimension":1,"axis":{"id":"p1017"}}}]}}]}}
+    <script type="application/json" id="f4366d67-f7c5-42e5-a808-32f3f0512b09">
+      {"88541ec7-ef03-4e7f-b0c4-b16bc3ce42ce":{"version":"3.4.1","title":"Bokeh Application","roots":[{"type":"object","name":"Figure","id":"p1001","attributes":{"width":400,"height":400,"x_range":{"type":"object","name":"Range1d","id":"p1010"},"y_range":{"type":"object","name":"Range1d","id":"p1011"},"x_scale":{"type":"object","name":"LinearScale","id":"p1012"},"y_scale":{"type":"object","name":"LinearScale","id":"p1013"},"title":{"type":"object","name":"Title","id":"p1008"},"renderers":[{"type":"object","name":"GlyphRenderer","id":"p1041","attributes":{"data_source":{"type":"object","name":"ColumnDataSource","id":"p1035","attributes":{"selected":{"type":"object","name":"Selection","id":"p1036","attributes":{"indices":[],"line_indices":[]}},"selection_policy":{"type":"object","name":"UnionRenderers","id":"p1037"},"data":{"type":"map","entries":[["url",["THOMAS_IS_BEST/molecule_image.png"]]]}}},"view":{"type":"object","name":"CDSView","id":"p1042","attributes":{"filter":{"type":"object","name":"AllIndices","id":"p1043"}}},"glyph":{"type":"object","name":"ImageURL","id":"p1038","attributes":{"url":{"type":"field","field":"url"},"x":{"type":"value","value":0},"y":{"type":"value","value":1},"w":{"type":"value","value":1},"h":{"type":"value","value":1}}},"nonselection_glyph":{"type":"object","name":"ImageURL","id":"p1039","attributes":{"url":{"type":"field","field":"url"},"x":{"type":"value","value":0},"y":{"type":"value","value":1},"w":{"type":"value","value":1},"h":{"type":"value","value":1},"global_alpha":{"type":"value","value":0.1}}},"muted_glyph":{"type":"object","name":"ImageURL","id":"p1040","attributes":{"url":{"type":"field","field":"url"},"x":{"type":"value","value":0},"y":{"type":"value","value":1},"w":{"type":"value","value":1},"h":{"type":"value","value":1},"global_alpha":{"type":"value","value":0.2}}}}}],"toolbar":{"type":"object","name":"Toolbar","id":"p1009","attributes":{"tools":[{"type":"object","name":"PanTool","id":"p1024"},{"type":"object","name":"WheelZoomTool","id":"p1025","attributes":{"renderers":"auto"}},{"type":"object","name":"BoxZoomTool","id":"p1026","attributes":{"overlay":{"type":"object","name":"BoxAnnotation","id":"p1027","attributes":{"syncable":false,"level":"overlay","visible":false,"left":{"type":"number","value":"nan"},"right":{"type":"number","value":"nan"},"top":{"type":"number","value":"nan"},"bottom":{"type":"number","value":"nan"},"left_units":"canvas","right_units":"canvas","top_units":"canvas","bottom_units":"canvas","line_color":"black","line_alpha":1.0,"line_width":2,"line_dash":[4,4],"fill_color":"lightgrey","fill_alpha":0.5}}}},{"type":"object","name":"SaveTool","id":"p1032"},{"type":"object","name":"ResetTool","id":"p1033"},{"type":"object","name":"HelpTool","id":"p1034"}]}},"toolbar_location":null,"left":[{"type":"object","name":"LinearAxis","id":"p1019","attributes":{"visible":false,"ticker":{"type":"object","name":"BasicTicker","id":"p1020","attributes":{"mantissas":[1,2,5]}},"formatter":{"type":"object","name":"BasicTickFormatter","id":"p1021"},"major_label_policy":{"type":"object","name":"AllLabels","id":"p1022"}}}],"below":[{"type":"object","name":"LinearAxis","id":"p1014","attributes":{"visible":false,"ticker":{"type":"object","name":"BasicTicker","id":"p1015","attributes":{"mantissas":[1,2,5]}},"formatter":{"type":"object","name":"BasicTickFormatter","id":"p1016"},"major_label_policy":{"type":"object","name":"AllLabels","id":"p1017"}}}],"center":[{"type":"object","name":"Grid","id":"p1018","attributes":{"axis":{"id":"p1014"},"grid_line_color":null}},{"type":"object","name":"Grid","id":"p1023","attributes":{"dimension":1,"axis":{"id":"p1019"},"grid_line_color":null}}]}}]}}
     </script>
     <script type="text/javascript">
       (function() {
         const fn = function() {
           Bokeh.safely(function() {
             (function(root) {
               function embed_document(root) {
-              const docs_json = document.getElementById('c51ba175-b001-4ff6-833d-185361e733ff').textContent;
-              const render_items = [{"docid":"c79cfb15-fae5-422e-ab4f-7d753464a019","roots":{"p1001":"e736f10d-e625-4fab-964b-af5fbe41e5c8"},"root_ids":["p1001"]}];
+              const docs_json = document.getElementById('f4366d67-f7c5-42e5-a808-32f3f0512b09').textContent;
+              const render_items = [{"docid":"88541ec7-ef03-4e7f-b0c4-b16bc3ce42ce","roots":{"p1001":"ae5708ad-472e-4b50-b9fe-ee5c821f1b30"},"root_ids":["p1001"]}];
               root.Bokeh.embed.embed_items(docs_json, render_items);
               }
               if (root.Bokeh !== undefined) {
                 embed_document(root);
               } else {
                 let attempts = 0;
                 const timer = setInterval(function(root) {
```

### Comparing `cheminterface_ppchem-1.0/Bokeh/Bokeh try.py` & `cheminterface_ppchem-2.0/Bokeh/Bokeh try.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 
 
 from bokeh.models import CustomJS, ColumnDataSource, Slider
 from bokeh.plotting import figure, output_file, show
 from bokeh.layouts import column
 from bokeh.models import WheelZoomTool, PanTool
 import numpy as np
+from bokeh.layouts import row
 
 output_file("callback.html")
 
 x = np.linspace(-5, 5, 500)
 mu = 0
 sigma = 1
 y = 1 / (sigma * np.sqrt(2 * np.pi)) * np.exp(-0.5 * ((x - mu) / sigma) ** 2)
@@ -91,22 +92,38 @@
 from bokeh.models import CustomJS, TextInput
 
 text_input = TextInput(value="default", title="Label:")
 text_input.js_on_change("value", CustomJS(code="""
     console.log('text_input: value=' + this.value, this.toString())
 """))
 
+image_url = "/Users/igorgonteri/Documents/GitHub/ppchem-project-Christiansson-Gonteri-Humery/Bokeh/molecule_image.png"
 
-layout = column(slider, plot, checkbox_button_group, dropdown, cube, range_slider, text_input)
 
+p = figure(width=400, height=400,toolbar_location=None, x_range=(0, 1), y_range=(0, 1))
+p.image_url(url=[image_url], x=0, y=1, w=1, h=1)
 
+
+p.xgrid.grid_line_color = None
+p.ygrid.grid_line_color = None
+p.xaxis.visible = False
+p.yaxis.visible = False
+
+from bokeh.layouts import gridplot
+
+# Place plots in a grid layout
+layout = row(plot, p)
+
+# Show the layout
 show(layout)
 
 
 
+
+
 from bokeh.models import PanTool, WheelZoomTool
 import numpy as np
 from bokeh.plotting import figure, output_file, show, curdoc
 from bokeh.models import Button, Div, CustomJS, TextInput
 from bokeh.layouts import column
 
 # Generate data for a Gaussian distribution with a very small standard deviation
@@ -153,12 +170,26 @@
     renderer.data_source.data['y'] = y
 
 # Attach the callback to the TextInput widgets
 mu_input.on_change('value', update_plot)
 sigma_input.on_change('value', update_plot)
 
 # Create a layout with the plot, TextInput widgets, and information
-layout = column(p, button, info, mu_input, sigma_input)
+
+image_url = "/Users/igorgonteri/Documents/GitHub/ppchem-project-Christiansson-Gonteri-Humery/Bokeh/molecule_image.png"
+
+
+plot = figure(width=400, height=400,toolbar_location=None, x_range=(0, 1), y_range=(0, 1))
+plot.image_url(url=[image_url], x=0, y=1, w=1, h=1)
+
+
+plot.xgrid.grid_line_color = None
+plot.ygrid.grid_line_color = None
+plot.xaxis.visible = False
+plot.yaxis.visible = False
+
+
 
 
+layout = column(p, button, info, mu_input, sigma_input, plot)
 show(layout)
```

### Comparing `cheminterface_ppchem-1.0/Bokeh/Mass spectro display.html` & `cheminterface_ppchem-2.0/Bokeh/Mass spectro display.html`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-1.0/Bokeh/Mass spectro display.py` & `cheminterface_ppchem-2.0/Bokeh/Mass spectro display.py`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-1.0/Bokeh/Mol_display.py` & `cheminterface_ppchem-2.0/THOMAS_IS_BEST/Mol_display.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,56 @@
-from rdkit import Chem
 from bokeh.plotting import figure, show
-import numpy as np
-from rdkit.Chem import Draw
+from rdkit.Chem import Draw, AllChem
 from rdkit import Chem
-from PIL import Image
-from io import BytesIO
-
-
+from bokeh.plotting import row
 
-def validate_smiles(smiles):
-    mol = Chem.MolFromSmiles(smiles)
-    if mol is None:
-        print("Invalid SMILES input.")
-        exit()
-    return True
 
 input_mol = input('SMILES: ')
 
+# Function to generate RDKit molecule image and save to file
+def save_molecule_image_to_file(mol_smi, file_path, show_Hs=False, show_3D = False):
+    # Generate the image from the molecule
+    mol = Chem.MolFromSmiles(mol_smi)
 
-mol = Chem.MolFromSmiles(input_mol)
+    # Adds the hydrogens to the molecule if specified
+    if show_Hs:
+        mol = Chem.AddHs(mol)
 
-image = Draw.MolToImage(mol)
-image.show()
+    # Show the molecule in 3D if specified
+    if show_3D:
+        mol = AllChem.EmbedMolecule(mol)
 
-
-# Function to generate RDKit molecule image and save to file
-def save_molecule_image_to_file(mol, file_path):
-    # Generate the image from the molecule
-    image = Chem.Draw.MolToImage(mol)
+    image = Draw.MolToImage(mol)
 
     # Save the image to a file
     image.save(file_path)
 
-if mol is None:
-    print("Invalid SMILES input.")
-    exit()
-
 output_file_path = "molecule_image.png"
-save_molecule_image_to_file(mol, output_file_path)
+save_molecule_image_to_file(input_mol, output_file_path, False, False)
+
+def mol_web_show(image_url):
+
+    # Creating a Bokeh figure
+    p = figure(width=400, height=400,toolbar_location=None, x_range=(0, 1), y_range=(0, 1))
+    p.image_url(url=[image_url], x=0, y=1, w=1, h=1)
+
+    # Hide grid lines and axes
+    p.xgrid.grid_line_color = None
+    p.ygrid.grid_line_color = None
+    p.xaxis.visible = False
+    p.yaxis.visible = False
+
+    return p
+
+
+
+image_url = "THOMAS_IS_BEST/molecule_image.png"
+
+show(mol_web_show(image_url))
+
+def final_layout(p1, p2):
+    layout = row(p1,p2)
+    show(layout)
+
+
+
```

### Comparing `cheminterface_ppchem-1.0/Bokeh/callback.html` & `cheminterface_ppchem-2.0/Bokeh/callback.html`

 * *Files 11% similar despite different names*

```diff
@@ -9,34 +9,32 @@
         display: flow-root;
         height: 100%;
         margin: 0;
         padding: 0;
       }
     </style>
     <script type="text/javascript" src="https://cdn.bokeh.org/bokeh/release/bokeh-3.4.1.min.js"></script>
-    <script type="text/javascript" src="https://cdn.bokeh.org/bokeh/release/bokeh-widgets-3.4.1.min.js"></script>
-    <script type="text/javascript" src="https://cdn.bokeh.org/bokeh/release/bokeh-tables-3.4.1.min.js"></script>
     <script type="text/javascript">
         Bokeh.set_log_level("info");
     </script>
   </head>
   <body>
-    <div id="c1a1dfc5-34de-40df-b898-f1815e4c48c9" data-root-id="p1080" style="display: contents;"></div>
+    <div id="a5d4e069-3c35-4c1b-ad36-48bd8858af0d" data-root-id="p1123" style="display: contents;"></div>
   
-    <script type="application/json" id="cc4e4858-92c4-4356-b0dc-93cdc13d03b2">
-      {"daa8f412-30e8-4b84-b91d-0e6a8e996be9":{"version":"3.4.1","title":"Bokeh Application","roots":[{"type":"object","name":"Column","id":"p1080","attributes":{"children":[{"type":"object","name":"Slider","id":"p1048","attributes":{"js_property_callbacks":{"type":"map","entries":[["change:value",[{"type":"object","name":"CustomJS","id":"p1047","attributes":{"args":{"type":"map","entries":[["source",{"type":"object","name":"ColumnDataSource","id":"p1001","attributes":{"selected":{"type":"object","name":"Selection","id":"p1002","attributes":{"indices":[],"line_indices":[]}},"selection_policy":{"type":"object","name":"UnionRenderers","id":"p1003"},"data":{"type":"map","entries":[["x",{"type":"ndarray","array":{"type":"bytes","data":"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"},"shape":[500],"dtype":"float64","order":"little"}],["y",{"type":"ndarray","array":{"type":"bytes","data":"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"},"shape":[500],"dtype":"float64","order":"little"}]]}}}]]},"code":"\n        const data = source.data;\n        const sigma = cb_obj.value;\n        const x = data['x'];\n        const y = data['y'];\n        for (let i = 0; i &lt; x.length; i++) {\n            y[i] = 1 / (sigma * Math.sqrt(2 * Math.PI)) * Math.exp(-0.5 * Math.pow((x[i] - 0) / sigma, 2));\n        }\n        source.change.emit();\n    "}}]]]},"title":"Variance","start":0.0001,"end":10,"value":1,"step":0.01}},{"type":"object","name":"Figure","id":"p1004","attributes":{"width":400,"height":400,"x_range":{"type":"object","name":"DataRange1d","id":"p1005"},"y_range":{"type":"object","name":"DataRange1d","id":"p1006"},"x_scale":{"type":"object","name":"LinearScale","id":"p1013"},"y_scale":{"type":"object","name":"LinearScale","id":"p1014"},"title":{"type":"object","name":"Title","id":"p1011"},"renderers":[{"type":"object","name":"GlyphRenderer","id":"p1042","attributes":{"data_source":{"id":"p1001"},"view":{"type":"object","name":"CDSView","id":"p1043","attributes":{"filter":{"type":"object","name":"AllIndices","id":"p1044"}}},"glyph":{"type":"object","name":"Line","id":"p1039","attributes":{"x":{"type":"field","field":"x"},"y":{"type":"field","field":"y"},"line_color":"#1f77b4","line_alpha":0.6,"line_width":3}},"nonselection_glyph":{"type":"object","name":"Line","id":"p1040","attributes":{"x":{"type":"field","field":"x"},"y":{"type":"field","field":"y"},"line_color":"#1f77b4","line_alpha":0.1,"line_width":3}},"muted_glyph":{"type":"object","name":"Line","id":"p1041","attributes":{"x":{"type":"field","field":"x"},"y":{"type":"field","field":"y"},"line_color":"#1f77b4","line_alpha":0.2,"line_width":3}}}}],"toolbar":{"type":"object","name":"Toolbar","id":"p1012","attributes":{"tools":[{"type":"object","name":"PanTool","id":"p1025"},{"type":"object","name":"WheelZoomTool","id":"p1026","attributes":{"renderers":"auto"}},{"type":"object","name":"BoxZoomTool","id":"p1027","attributes":{"overlay":{"type":"object","name":"BoxAnnotation","id":"p1028","attributes":{"syncable":false,"level":"overlay","visible":false,"left":{"type":"number","value":"nan"},"right":{"type":"number","value":"nan"},"top":{"type":"number","value":"nan"},"bottom":{"type":"number","value":"nan"},"left_units":"canvas","right_units":"canvas","top_units":"canvas","bottom_units":"canvas","line_color":"black","line_alpha":1.0,"line_width":2,"line_dash":[4,4],"fill_color":"lightgrey","fill_alpha":0.5}}}},{"type":"object","name":"SaveTool","id":"p1033"},{"type":"object","name":"ResetTool","id":"p1034"},{"type":"object","name":"HelpTool","id":"p1035"},{"type":"object","name":"PanTool","id":"p1045"},{"type":"object","name":"WheelZoomTool","id":"p1046","attributes":{"dimensions":"width","renderers":"auto"}}]}},"left":[{"type":"object","name":"LinearAxis","id":"p1020","attributes":{"ticker":{"type":"object","name":"BasicTicker","id":"p1021","attributes":{"mantissas":[1,2,5]}},"formatter":{"type":"object","name":"BasicTickFormatter","id":"p1022"},"major_label_policy":{"type":"object","name":"AllLabels","id":"p1023"}}}],"below":[{"type":"object","name":"LinearAxis","id":"p1015","attributes":{"ticker":{"type":"object","name":"BasicTicker","id":"p1016","attributes":{"mantissas":[1,2,5]}},"formatter":{"type":"object","name":"BasicTickFormatter","id":"p1017"},"major_label_policy":{"type":"object","name":"AllLabels","id":"p1018"}}}],"center":[{"type":"object","name":"Grid","id":"p1019","attributes":{"axis":{"id":"p1015"}}},{"type":"object","name":"Grid","id":"p1024","attributes":{"dimension":1,"axis":{"id":"p1020"}}}]}},{"type":"object","name":"CheckboxButtonGroup","id":"p1051","attributes":{"js_event_callbacks":{"type":"map","entries":[["button_click",[{"type":"object","name":"CustomJS","id":"p1052","attributes":{"args":{"type":"map","entries":[["btn",{"id":"p1051"}]]},"code":"\n    console.log('checkbox_button_group: active=' + btn.active, this.toString())\n"}}]]]},"labels":["Option 1","Option 2","Option 3"],"active":[0,1]}},{"type":"object","name":"Dropdown","id":"p1049","attributes":{"button_type":"warning","js_event_callbacks":{"type":"map","entries":[["menu_item_click",[{"type":"object","name":"CustomJS","id":"p1050","attributes":{"code":"console.log('dropdown: ' + this.item, this.toString())"}}]]]},"label":"Dropdown button","menu":[["Item 1","item_1"],["Item 2","item_2"],null,["Item 3","item_3"]]}},{"type":"object","name":"DataCube","id":"p1070","attributes":{"source":{"type":"object","name":"ColumnDataSource","id":"p1053","attributes":{"selected":{"type":"object","name":"Selection","id":"p1054","attributes":{"indices":[],"line_indices":[]}},"selection_policy":{"type":"object","name":"UnionRenderers","id":"p1055"},"data":{"type":"map","entries":[["d0",["A","E","E","E","J","L","M"]],["d1",["B","D","D","H","K","L","N"]],["d2",["C","F","G","H","K","L","O"]],["px",[10,20,30,40,50,60,70]]]}}},"view":{"type":"object","name":"CDSView","id":"p1074","attributes":{"filter":{"type":"object","name":"AllIndices","id":"p1075"}}},"columns":[{"type":"object","name":"TableColumn","id":"p1060","attributes":{"field":"d2","title":"Name","width":80,"formatter":{"type":"object","name":"StringFormatter","id":"p1059","attributes":{"font_style":{"type":"value","value":"bold"}}},"editor":{"type":"object","name":"StringEditor","id":"p1062"},"sortable":false}},{"type":"object","name":"TableColumn","id":"p1063","attributes":{"field":"px","title":"Price","width":40,"formatter":{"type":"object","name":"StringFormatter","id":"p1064"},"editor":{"type":"object","name":"StringEditor","id":"p1065"},"sortable":false}}],"grouping":[{"type":"object","name":"GroupingInfo","id":"p1067","attributes":{"getter":"d0","aggregators":[{"type":"object","name":"SumAggregator","id":"p1066","attributes":{"field_":"px"}}]}},{"type":"object","name":"GroupingInfo","id":"p1069","attributes":{"getter":"d1","aggregators":[{"type":"object","name":"SumAggregator","id":"p1068","attributes":{"field_":"px"}}]}}],"target":{"type":"object","name":"ColumnDataSource","id":"p1056","attributes":{"selected":{"type":"object","name":"Selection","id":"p1057","attributes":{"indices":[],"line_indices":[]}},"selection_policy":{"type":"object","name":"UnionRenderers","id":"p1058"},"data":{"type":"map","entries":[["row_indices",[]],["labels",[]]]}}}}},{"type":"object","name":"RangeSlider","id":"p1076","attributes":{"js_property_callbacks":{"type":"map","entries":[["change:value",[{"type":"object","name":"CustomJS","id":"p1077","attributes":{"code":"\n    console.log('range_slider: value=' + this.value, this.toString())\n"}}]]]},"title":"Stuff","value":[1,9],"start":0,"end":10,"step":0.1}},{"type":"object","name":"TextInput","id":"p1078","attributes":{"js_property_callbacks":{"type":"map","entries":[["change:value",[{"type":"object","name":"CustomJS","id":"p1079","attributes":{"code":"\n    console.log('text_input: value=' + this.value, this.toString())\n"}}]]]},"title":"Label:","value":"default"}}]}}]}}
+    <script type="application/json" id="ef3ac0e7-7b27-4f4e-958f-8f200b4ced30">
+      {"8a3b3a79-d67b-432b-bd76-bd60d3d11867":{"version":"3.4.1","title":"Bokeh Application","roots":[{"type":"object","name":"Row","id":"p1123","attributes":{"children":[{"type":"object","name":"Figure","id":"p1004","attributes":{"width":400,"height":400,"x_range":{"type":"object","name":"DataRange1d","id":"p1005"},"y_range":{"type":"object","name":"DataRange1d","id":"p1006"},"x_scale":{"type":"object","name":"LinearScale","id":"p1013"},"y_scale":{"type":"object","name":"LinearScale","id":"p1014"},"title":{"type":"object","name":"Title","id":"p1011"},"renderers":[{"type":"object","name":"GlyphRenderer","id":"p1042","attributes":{"data_source":{"type":"object","name":"ColumnDataSource","id":"p1001","attributes":{"selected":{"type":"object","name":"Selection","id":"p1002","attributes":{"indices":[],"line_indices":[]}},"selection_policy":{"type":"object","name":"UnionRenderers","id":"p1003"},"data":{"type":"map","entries":[["x",{"type":"ndarray","array":{"type":"bytes","data":"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"},"shape":[500],"dtype":"float64","order":"little"}],["y",{"type":"ndarray","array":{"type":"bytes","data":"P/3IZGnxuD6//6jt95C7PlE9WIoFdL4+ENjM9YHQwD6WkKuVfI/CPtCQfR7GesQ+cQkcKYmWxj4/K3eiTufIPkiL7IsFcss+GE5UUAs8zj5lss5bmqXQPi2OrcHrUtI+96WaX2op1D41S2Do0SzWPlCybikvYdg+tDCtZObK2j43Kh0dum7dPgI9qS7pKOA+eqqNP+K84T4k/gS+TXbjPmGHdmdwWOU+wM5P99Jm5z7VKHw1R6XpPtJVf1rtF+w+tj73zTnD7j5VAT2i/dXwPuSK+6Cwa/I+cgr6goEl9D4I9pdzcwb2PoZ0NBLFEfg+jgMamPRK+j6biAI/xLX8PpnnW+s+Vv8+yYrGjl4YAT/mbckW9aQCP0UGMepkUwQ/NEVJA18mBj9UjfWRxiAIP3qvvD+0RQo/bKP5oXmYDD+v1RfcpBwPP3aV5DkC6xA/YRGVrFVkEj9x1GaSevwTP6YG10bFtRU/0JWBDLOSFz+kav+C7JUZP4YBuDtIwhs/THylbs0aHj+uEwRoW1EgP9igAcS6riE/9U2MJlonIz/2ljlRLb0kP1wMdR1IciY/Or7OQOBIKD/8i4IkT0MqPwPantATZCw/lOcq69StLj9U8tJlsZEwP4z1l9Hc4zE/6ovS3AFPMz9Ek/TfzdQ0P6aJy5sHdzY/zDEeeJA3OD9qXx3NZRg6P1w0rjeiGzw/b3uM+H5DPj9gzB2vKklAPwvd2RxQhUE/4MHXrn7XQj84NDqUF0FEP1yU8guPw0U/e0/RM21gRz8ofXncThlJP/9xDWLm70o/kVtjifzlTD8X+4lhcf1OP2Qhr5QenFA/yXl1nDjMUT8TsSF3HBBTP4ogwU7taFQ/tlvGQdzXVT+zlJjdKF5XPx/3F5oh/Vg/Z17ZVSS2Wj+t9NbSnopcP0lRTjMPfF4/lc0/OwJGYD8gBX56D15hP05xFm4Ih2I/QVpbVM/BYz9LpqvPTw9lP9Cr6yF/cGY/AqjRZlzmZz9678zM8HFpP6U4TMxPFGs/mrEkXZfObD9t7Ngp8KFuP+sIPuDGR3A/x511YFdMcT9uLwqETl9yPzDk/+tWgXM/d24n/iCzdD+/UnD1YvV1PyFMJfDYSHc/gRXp+0SueD/X+UgfbyZ6P8vEuWAlsns/nPnSyjtSfT+/npttjAd/Pzi5Xa57aYA/TH8xVbFagT8eZV4v3VeCPxLm3DV4YYM/b6mFTv53hD+yZA5C7puFP0sQ8K/JzYY/+hYgABUOiD9VhYZSV12JP2SxG2wavIo/S1+YoeoqjD/0DaS/VqqNPw7VbfDvOo8/Xo1Oz6RukD+MLcSq/EiRPzCoUE/LLJI/wHsDbl0akz8/nReQABKUP4y4TQEDFJU/hzjGuLMglj9HRFZAYjiXP1nAU5peW5g/0VHVJfmJmT89XmSBgsSaP3MQIGxLC5w/lIJRpaRenT+XVnLK3r6eP9Yc1BklFqA/nohcZ5vToD8Ubj78+ZehP2nWaSpoY6I/EcGT0gw2oz/WmcFODhCkP3ONJFyS8aQ/889KBL7apT95q62FtcumP8LxozucxKc/3DPBhZTFqD+s6qquv86pPxOHbdI94Ko/aShcxC36qz//g4b0rBytP0dP0VTXR64/lEW+Pcd7rz8H03ipSlywP97iwTMs/7A/AwcXsZKmsT9lurGQh1KyPyGWsi8TA7M/7ncyyzy4sz+oemNyCnK0P3APy/iAMLU/S82e6KPztT9gzk11dbu2P/WsQG72h7c/n2jaMSZZuD9xqcSgAi+5P7H/kRGICbo/Yd3ARLHouj9GICpZd8y7P8oR5sDRtLw/icqyNrahvT/I5OazGJO+PwRf+2briL8/xr1bVY9BwD/apQR/0MDAPyq3Sn4vQsE/SisErKHFwT+JmhlpG0vCPx4r/xuQ0sI/szydLvJbwz/yI60MM+fDP/pXjiJDdMQ/JjuY3BEDxT9lbOymjZPFP5pMze2jJcY/aBx8HkG5xj9JzKGoUE7HP/dHRQC95Mc/qLJRoG98yD8rsK4NURXJPyd77NpIr8k/XCeFrD1Kyj/FC7Q9FebKP3fo42W0gss/NfKzHv8fzD8rgZOK2L3MP2yw8/siXM0/gssN/b/6zT8U9DxYkJnOP0/26CB0OM8/qs3/vErXzz9nc313+TrQP0FbNnAlitA/WmSJFhjZ0D9v+zP3vyfRP8EB2WMLdtE/aLNCeejD0T+a1dwlRRHSP+glZDAPXtI/wM/HPjSq0j9zejndofXSP9xRaIVFQNM/+jzjpQyK0z9vSp6p5NLTP/0wl/+6GtQ/m5uUIn1h1D+G1fugGKfUP6lJuCR769Q/Eiwwe5Iu1T8AikGdTHDVP4nnQreXsNU/6H4CMWLv1T92J7+1mizWP0ffFTwwaNY/SezeDRKi1j/2hvXPL9rWP2UC5Yl5ENc/kmt2rd9E1z+VoxkeU3fXP+wGJTjFp9c/Xcbm1yfW1z/KLINgbQLYPwsom8KILNg/oIm2gm1U2D8gl22/D3rYP9yoTTdkndg/2b90TmC+2D8pKuAT+tzYP6x+akYo+dg/BW51WeIS2T/aHjx5ICrZP3wGy47bPtk/Q22aQw1R2T8lDskEsGDZPxuE9AW/bdk/w3ytQzZ42T+R7oWFEoDZP0jZt19Rhdk/UGFjNPGH2T9QYWM08YfZP0nZt19Rhdk/ke6FhRKA2T/DfK1DNnjZPxuE9AW/bdk/JQ7JBLBg2T9DbZpDDVHZP3wGy47bPtk/3B48eSAq2T8GbnVZ4hLZP6x+akYo+dg/KSrgE/rc2D/bv3ROYL7YP92oTTdkndg/IJdtvw962D+gibaCbVTYPw0om8KILNg/yiyDYG0C2D9dxubXJ9bXP+8GJTjFp9c/mKMZHlN31z+Sa3at30TXP2UC5Yl5ENc/+Yb1zy/a1j9M7N4NEqLWP0ffFTwwaNY/die/tZos1j/rfgIxYu/VP4nnQreXsNU/AIpBnUxw1T8VLDB7ki7VP61JuCR769Q/htX7oBin1D+bm5QifWHUPwAxl/+6GtQ/c0qeqeTS0z/6POOlDIrTP9xRaIVFQNM/d3o53aH10j/Az8c+NKrSP+glZDAPXtI/ntXcJUUR0j9ss0J56MPRP8EB2WMLdtE/b/sz978n0T9eZIkWGNnQP0VbNnAlitA/Z3N9d/k60D+qzf+8StfPP1f26CB0OM8/F/Q8WJCZzj+Cyw39v/rNP3Ow8/siXM0/MIGTiti9zD858rMe/x/MP3fo42W0gss/zQu0PRXmyj9fJ4WsPUrKPyd77NpIr8k/K7CuDVEVyT+rslGgb3zIP/tHRQC95Mc/ScyhqFBOxz9vHHweQbnGP55Mze2jJcY/aGzspo2TxT8mO5jcEQPFPwBYjiJDdMQ/9iOtDDPnwz+zPJ0u8lvDPyUr/xuQ0sI/jZoZaRtLwj9OKwSsocXBPyq3Sn4vQsE/4KUEf9DAwD/JvVtVj0HAPwpf+2briL8/yOTmsxiTvj+UyrI2tqG9P9ER5sDRtLw/RiAqWXfMuz9s3cBEsei6P7f/kRGICbo/d6nEoAIvuT+faNoxJlm4P/+sQG72h7c/Zc5NdXW7tj9QzZ7oo/O1P3APy/iAMLU/sHpjcgpytD/zdzLLPLizPyGWsi8TA7M/bbqxkIdSsj8HBxexkqaxP+LiwTMs/7A/B9N4qUpcsD+iRb49x3uvP09P0VTXR64/BYSG9KwcrT9pKFzELfqrPxuHbdI94Ko/tOqqrr/OqT/cM8GFlMWoP9HxozucxKc/f6uthbXLpj/4z0oEvtqlP3ONJFyS8aQ/4JnBTg4QpD8WwZPSDDajP23WaSpoY6I/FG4+/PmXoT+iiFxnm9OgP9oc1BklFqA/l1Zyyt6+nj+mglGlpF6dP30QIGxLC5w/R15kgYLEmj/RUdUl+YmZP2jAU5peW5g/UERWQGI4lz+NOMa4syCWP4y4TQEDFJU/RJ0XkAASlD/HewNuXRqTPzCoUE/LLJI/mC3EqvxIkT9ljU7PpG6QPxbVbfDvOo8/9A2kv1aqjT9fX5ih6iqMP2qxG2wavIo/XIWGUlddiT/6FiAAFQ6IP1QQ8K/JzYY/u2QOQu6bhT9vqYVO/neEPx7m3DV4YYM/JmVeL91Xgj9QfzFVsVqBPzi5Xa57aYA/1p6bbYwHfz+q+dLKO1J9P9rEuWAlsns/1/lIH28mej+OFen7RK54PydMJfDYSHc/v1Jw9WL1dT+Hbif+ILN0PzXk/+tWgXM/dy8KhE5fcj/UnXVgV0xxP/cIPuDGR3A/fOzYKfChbj+asSRdl85sP6U4TMxPFGs/eu/MzPBxaT8aqNFmXOZnP+Kr6yF/cGY/W6arz08PZT9GWltUz8FjP05xFm4Ih2I/IAV+eg9eYT+VzT87AkZgPzlRTjMPfF4/xPTW0p6KXD98XtlVJLZaPzj3F5oh/Vg/vpSY3SheVz+2W8ZB3NdVP4ogwU7taFQ/CbEhdxwQUz/beXWcOMxRP3Qhr5QenFA/NfuJYXH9Tj+gW2OJ/OVMP/9xDWLm70o/KH153E4ZST97T9EzbWBHP3iU8guPw0U/RzQ6lBdBRD/vwdeuftdCPxTd2RxQhUE/YMwdrypJQD9ve4z4fkM+P1w0rjeiGzw/XV8dzWUYOj/kMR54kDc4P7eJy5sHdzY/WZP0383UND/0i9LcAU8zP4z1l9Hc4zE/VPLSZbGRMD+E5yrr1K0uPx/antATZCw/FYyCJE9DKj9Svs5A4EgoP2gMdR1IciY/9pY5US29JD/1TYwmWicjP9igAcS6riE/vhMEaFtRID9qfKVuzRoeP6EBuDtIwhs/vWr/guyVGT/QlYEMs5IXP6YG10bFtRU/cdRmknr8Ez9hEZWsVWQSP4eV5DkC6xA/z9UX3KQcDz+Jo/mheZgMP3qvvD+0RQo/VI31kcYgCD80RUkDXyYGP0UGMepkUwQ/+G3JFvWkAj/iisaOXhgBP7nnW+s+Vv8+m4gCP8S1/D6OAxqY9Er6PoZ0NBLFEfg+CPaXc3MG9j6HCvqCgSX0PvaK+6Cwa/I+ZgE9ov3V8D7WPvfNOcPuPtJVf1rtF+w+1Sh8NUel6T7Azk/30mbnPmGHdmdwWOU+OP4Evk124z6Mqo0/4rzhPho9qS7pKOA+NyodHbpu3T60MK1k5sraPlCybikvYdg+NUtg6NEs1j4MpppfainUPkmOrcHrUtI+dbLOW5ql0D4YTlRQCzzOPkiL7IsFcss+Pyt3ok7nyD5xCRwpiZbGPuSQfR7GesQ+qZCrlXyPwj4p2Mz1gdDAPn89WIoFdL4+v/+o7feQuz4//chkafG4Pg=="},"shape":[500],"dtype":"float64","order":"little"}]]}}},"view":{"type":"object","name":"CDSView","id":"p1043","attributes":{"filter":{"type":"object","name":"AllIndices","id":"p1044"}}},"glyph":{"type":"object","name":"Line","id":"p1039","attributes":{"x":{"type":"field","field":"x"},"y":{"type":"field","field":"y"},"line_color":"#1f77b4","line_alpha":0.6,"line_width":3}},"nonselection_glyph":{"type":"object","name":"Line","id":"p1040","attributes":{"x":{"type":"field","field":"x"},"y":{"type":"field","field":"y"},"line_color":"#1f77b4","line_alpha":0.1,"line_width":3}},"muted_glyph":{"type":"object","name":"Line","id":"p1041","attributes":{"x":{"type":"field","field":"x"},"y":{"type":"field","field":"y"},"line_color":"#1f77b4","line_alpha":0.2,"line_width":3}}}}],"toolbar":{"type":"object","name":"Toolbar","id":"p1012","attributes":{"tools":[{"type":"object","name":"PanTool","id":"p1025"},{"type":"object","name":"WheelZoomTool","id":"p1026","attributes":{"renderers":"auto"}},{"type":"object","name":"BoxZoomTool","id":"p1027","attributes":{"overlay":{"type":"object","name":"BoxAnnotation","id":"p1028","attributes":{"syncable":false,"level":"overlay","visible":false,"left":{"type":"number","value":"nan"},"right":{"type":"number","value":"nan"},"top":{"type":"number","value":"nan"},"bottom":{"type":"number","value":"nan"},"left_units":"canvas","right_units":"canvas","top_units":"canvas","bottom_units":"canvas","line_color":"black","line_alpha":1.0,"line_width":2,"line_dash":[4,4],"fill_color":"lightgrey","fill_alpha":0.5}}}},{"type":"object","name":"SaveTool","id":"p1033"},{"type":"object","name":"ResetTool","id":"p1034"},{"type":"object","name":"HelpTool","id":"p1035"},{"type":"object","name":"PanTool","id":"p1045"},{"type":"object","name":"WheelZoomTool","id":"p1046","attributes":{"dimensions":"width","renderers":"auto"}}]}},"left":[{"type":"object","name":"LinearAxis","id":"p1020","attributes":{"ticker":{"type":"object","name":"BasicTicker","id":"p1021","attributes":{"mantissas":[1,2,5]}},"formatter":{"type":"object","name":"BasicTickFormatter","id":"p1022"},"major_label_policy":{"type":"object","name":"AllLabels","id":"p1023"}}}],"below":[{"type":"object","name":"LinearAxis","id":"p1015","attributes":{"ticker":{"type":"object","name":"BasicTicker","id":"p1016","attributes":{"mantissas":[1,2,5]}},"formatter":{"type":"object","name":"BasicTickFormatter","id":"p1017"},"major_label_policy":{"type":"object","name":"AllLabels","id":"p1018"}}}],"center":[{"type":"object","name":"Grid","id":"p1019","attributes":{"axis":{"id":"p1015"}}},{"type":"object","name":"Grid","id":"p1024","attributes":{"dimension":1,"axis":{"id":"p1020"}}}]}},{"type":"object","name":"Figure","id":"p1080","attributes":{"width":400,"height":400,"x_range":{"type":"object","name":"Range1d","id":"p1089"},"y_range":{"type":"object","name":"Range1d","id":"p1090"},"x_scale":{"type":"object","name":"LinearScale","id":"p1091"},"y_scale":{"type":"object","name":"LinearScale","id":"p1092"},"title":{"type":"object","name":"Title","id":"p1087"},"renderers":[{"type":"object","name":"GlyphRenderer","id":"p1120","attributes":{"data_source":{"type":"object","name":"ColumnDataSource","id":"p1114","attributes":{"selected":{"type":"object","name":"Selection","id":"p1115","attributes":{"indices":[],"line_indices":[]}},"selection_policy":{"type":"object","name":"UnionRenderers","id":"p1116"},"data":{"type":"map","entries":[["url",["/Users/igorgonteri/Documents/GitHub/ppchem-project-Christiansson-Gonteri-Humery/Bokeh/molecule_image.png"]]]}}},"view":{"type":"object","name":"CDSView","id":"p1121","attributes":{"filter":{"type":"object","name":"AllIndices","id":"p1122"}}},"glyph":{"type":"object","name":"ImageURL","id":"p1117","attributes":{"url":{"type":"field","field":"url"},"x":{"type":"value","value":0},"y":{"type":"value","value":1},"w":{"type":"value","value":1},"h":{"type":"value","value":1}}},"nonselection_glyph":{"type":"object","name":"ImageURL","id":"p1118","attributes":{"url":{"type":"field","field":"url"},"x":{"type":"value","value":0},"y":{"type":"value","value":1},"w":{"type":"value","value":1},"h":{"type":"value","value":1},"global_alpha":{"type":"value","value":0.1}}},"muted_glyph":{"type":"object","name":"ImageURL","id":"p1119","attributes":{"url":{"type":"field","field":"url"},"x":{"type":"value","value":0},"y":{"type":"value","value":1},"w":{"type":"value","value":1},"h":{"type":"value","value":1},"global_alpha":{"type":"value","value":0.2}}}}}],"toolbar":{"type":"object","name":"Toolbar","id":"p1088","attributes":{"tools":[{"type":"object","name":"PanTool","id":"p1103"},{"type":"object","name":"WheelZoomTool","id":"p1104","attributes":{"renderers":"auto"}},{"type":"object","name":"BoxZoomTool","id":"p1105","attributes":{"overlay":{"type":"object","name":"BoxAnnotation","id":"p1106","attributes":{"syncable":false,"level":"overlay","visible":false,"left":{"type":"number","value":"nan"},"right":{"type":"number","value":"nan"},"top":{"type":"number","value":"nan"},"bottom":{"type":"number","value":"nan"},"left_units":"canvas","right_units":"canvas","top_units":"canvas","bottom_units":"canvas","line_color":"black","line_alpha":1.0,"line_width":2,"line_dash":[4,4],"fill_color":"lightgrey","fill_alpha":0.5}}}},{"type":"object","name":"SaveTool","id":"p1111"},{"type":"object","name":"ResetTool","id":"p1112"},{"type":"object","name":"HelpTool","id":"p1113"}]}},"toolbar_location":null,"left":[{"type":"object","name":"LinearAxis","id":"p1098","attributes":{"visible":false,"ticker":{"type":"object","name":"BasicTicker","id":"p1099","attributes":{"mantissas":[1,2,5]}},"formatter":{"type":"object","name":"BasicTickFormatter","id":"p1100"},"major_label_policy":{"type":"object","name":"AllLabels","id":"p1101"}}}],"below":[{"type":"object","name":"LinearAxis","id":"p1093","attributes":{"visible":false,"ticker":{"type":"object","name":"BasicTicker","id":"p1094","attributes":{"mantissas":[1,2,5]}},"formatter":{"type":"object","name":"BasicTickFormatter","id":"p1095"},"major_label_policy":{"type":"object","name":"AllLabels","id":"p1096"}}}],"center":[{"type":"object","name":"Grid","id":"p1097","attributes":{"axis":{"id":"p1093"},"grid_line_color":null}},{"type":"object","name":"Grid","id":"p1102","attributes":{"dimension":1,"axis":{"id":"p1098"},"grid_line_color":null}}]}}]}}]}}
     </script>
     <script type="text/javascript">
       (function() {
         const fn = function() {
           Bokeh.safely(function() {
             (function(root) {
               function embed_document(root) {
-              const docs_json = document.getElementById('cc4e4858-92c4-4356-b0dc-93cdc13d03b2').textContent;
-              const render_items = [{"docid":"daa8f412-30e8-4b84-b91d-0e6a8e996be9","roots":{"p1080":"c1a1dfc5-34de-40df-b898-f1815e4c48c9"},"root_ids":["p1080"]}];
+              const docs_json = document.getElementById('ef3ac0e7-7b27-4f4e-958f-8f200b4ced30').textContent;
+              const render_items = [{"docid":"8a3b3a79-d67b-432b-bd76-bd60d3d11867","roots":{"p1123":"a5d4e069-3c35-4c1b-ad36-48bd8858af0d"},"root_ids":["p1123"]}];
               root.Bokeh.embed.embed_items(docs_json, render_items);
               }
               if (root.Bokeh !== undefined) {
                 embed_document(root);
               } else {
                 let attempts = 0;
                 const timer = setInterval(function(root) {
```

### Comparing `cheminterface_ppchem-1.0/THOMAS_IS_BEST/Preliminary_v2.py` & `cheminterface_ppchem-2.0/THOMAS_IS_BEST/Preliminary_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import time
 import pandas as pd
 import matplotlib.pyplot as plt
 import plotly.graph_objects as go
 
 #Turn data (of Symbol | Mass | Probability) into lists 
 
-df = pd.read_csv('Thomas/abundance.txt'
+df = pd.read_csv('THOMAS_IS_BEST/abundance.txt.txt'
                  , sep='\t'
                  , header=None
                  , names=['Atom', 'Mass', 'Percentage'])
 
 
 #mass = [mass1, mass2, mass3,...]
```

### Comparing `cheminterface_ppchem-1.0/THOMAS_IS_BEST/abundance.txt` & `cheminterface_ppchem-2.0/THOMAS_IS_BEST/abundance.txt`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-1.0/THOMAS_IS_BEST/abundance_simplified.txt` & `cheminterface_ppchem-2.0/THOMAS_IS_BEST/abundance_simplified.txt`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-1.0/THOMAS_IS_BEST/functions.html` & `cheminterface_ppchem-2.0/Thomas/functions.html`

 * *Files 18% similar despite different names*

```diff
@@ -14,27 +14,27 @@
     </style>
     <script type="text/javascript" src="https://cdn.bokeh.org/bokeh/release/bokeh-3.4.1.min.js"></script>
     <script type="text/javascript">
         Bokeh.set_log_level("info");
     </script>
   </head>
   <body>
-    <div id="b188c5d6-ce2c-4b2e-b8df-2f0bfa41c640" data-root-id="p1034" style="display: contents;"></div>
+    <div id="bb07d693-12cb-44fd-a2ae-e662e409b64e" data-root-id="p1034" style="display: contents;"></div>
   
-    <script type="application/json" id="dad7ef00-fcce-44bc-86b8-ec254633b475">
-      {"49f429a0-2af3-40ad-987a-166cca72bd10":{"version":"3.4.1","title":"Bokeh Application","roots":[{"type":"object","name":"Figure","id":"p1034","attributes":{"width":700,"height":500,"x_range":{"type":"object","name":"DataRange1d","id":"p1035"},"y_range":{"type":"object","name":"DataRange1d","id":"p1036"},"x_scale":{"type":"object","name":"LinearScale","id":"p1044"},"y_scale":{"type":"object","name":"LinearScale","id":"p1045"},"title":{"type":"object","name":"Title","id":"p1037","attributes":{"text":"Mass spectrum of molecule"}},"renderers":[{"type":"object","name":"GlyphRenderer","id":"p1076","attributes":{"data_source":{"type":"object","name":"ColumnDataSource","id":"p1070","attributes":{"selected":{"type":"object","name":"Selection","id":"p1071","attributes":{"indices":[],"line_indices":[]}},"selection_policy":{"type":"object","name":"UnionRenderers","id":"p1072"},"data":{"type":"map","entries":[["x",{"type":"ndarray","array":{"type":"bytes","data":"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"},"shape":[1000],"dtype":"float64","order":"little"}],["y",{"type":"ndarray","array":{"type":"bytes","data":"AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA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AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAUdiBBAAAAAAqVCFIKBDVAQU3VkuZGCIF5QvLZpzdVggeHKY9Iz91Cyh98Q8oCX0OffAL6wwubREt/R/bh5BFFI5z8IdUcAcXAlqqdPi7shlMUjcq3gVGHDwYIY63CcMeh7swfnI0KCHyEhgJYqF2Ixh17ZxWHq8lW7IV/353zyfeT3dYFWbXKUvzuBkLl8krkBU1P5mUpC2HiH/V2FdoL93KjZuTLBUxq0XS6W8WqzJbNNe/jHspNBxVrd77oJE1Gu4Ybcbv4TbUx53MOtcaODP7FtdHiT055Ci4D8LmRzqYwN5fS3I8O1yMZmGI5Rg8SusyqwgG4DwM7kWcyFWOPYxjiNKnHSU+IebQbB6epT4hnBBMWUYQP0iRAHQsBWI/ArprmHBYnT9dE9J9NJLBP1rzi5aK8s4/W6psjpUKxD8mMdXDlxajP9FkrpIkvWo/HKGgKz+LGz98HsdOat20PjL/Km/qPjc+Gv4pg30Loz3XNbN6wfL2PB2xsiuSVTQ8Er1Pefh/WjtrB7k0ZWVpOsvCVBHN5WE56OUUEQKNQjjqnb2od0cMNy5Se/KJs781L6nZkiMiWjRdnulQSq/fMlBPW7njP0wxwOwPtI2Foi+uZGTQNtzhLcUvwztlVAksR92DjLBqGiqDmdpWhkIUKLXBQ2gy2vYlki09KpH0wiNo0Xvg1R93ITiS8Y+8vhQf8wCRzhNfmxzl9sAWtI4KGh3fBWXm8mIXR5Y/YXHioxRMfBzfcLDOETxZRvxWauEOBAOghvYR3Qs+Nd/igNfBCEkWX1HxGpAFzGiZjJhhRQJHovebAgAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA="},"shape":[1000],"dtype":"float64","order":"little"}]]}}},"view":{"type":"object","name":"CDSView","id":"p1077","attributes":{"filter":{"type":"object","name":"AllIndices","id":"p1078"}}},"glyph":{"type":"object","name":"Line","id":"p1073","attributes":{"x":{"type":"field","field":"x"},"y":{"type":"field","field":"y"},"line_color":"#1f77b4"}},"nonselection_glyph":{"type":"object","name":"Line","id":"p1074","attributes":{"x":{"type":"field","field":"x"},"y":{"type":"field","field":"y"},"line_color":"#1f77b4","line_alpha":0.1}},"muted_glyph":{"type":"object","name":"Line","id":"p1075","attributes":{"x":{"type":"field","field":"x"},"y":{"type":"field","field":"y"},"line_color":"#1f77b4","line_alpha":0.2}}}}],"toolbar":{"type":"object","name":"Toolbar","id":"p1043","attributes":{"autohide":true,"tools":[{"type":"object","name":"PanTool","id":"p1056"},{"type":"object","name":"WheelZoomTool","id":"p1057","attributes":{"renderers":"auto"}},{"type":"object","name":"BoxZoomTool","id":"p1058","attributes":{"overlay":{"type":"object","name":"BoxAnnotation","id":"p1059","attributes":{"syncable":false,"level":"overlay","visible":false,"left":{"type":"number","value":"nan"},"right":{"type":"number","value":"nan"},"top":{"type":"number","value":"nan"},"bottom":{"type":"number","value":"nan"},"left_units":"canvas","right_units":"canvas","top_units":"canvas","bottom_units":"canvas","line_color":"black","line_alpha":1.0,"line_width":2,"line_dash":[4,4],"fill_color":"lightgrey","fill_alpha":0.5}}}},{"type":"object","name":"SaveTool","id":"p1064"},{"type":"object","name":"ResetTool","id":"p1065"},{"type":"object","name":"HelpTool","id":"p1066"},{"type":"object","name":"WheelPanTool","id":"p1068","attributes":{"dimension":"height"}},{"type":"object","name":"WheelZoomTool","id":"p1069","attributes":{"dimensions":"height","renderers":"auto"}}]}},"left":[{"type":"object","name":"LinearAxis","id":"p1051","attributes":{"ticker":{"type":"object","name":"BasicTicker","id":"p1052","attributes":{"mantissas":[1,2,5]}},"formatter":{"type":"object","name":"BasicTickFormatter","id":"p1053"},"major_label_policy":{"type":"object","name":"AllLabels","id":"p1054"}}}],"below":[{"type":"object","name":"LinearAxis","id":"p1046","attributes":{"ticker":{"type":"object","name":"FixedTicker","id":"p1067","attributes":{"ticks":[36.9659,34.9689],"minor_ticks":[]}},"formatter":{"type":"object","name":"BasicTickFormatter","id":"p1048"},"major_label_policy":{"type":"object","name":"AllLabels","id":"p1049"}}}],"center":[{"type":"object","name":"Grid","id":"p1050","attributes":{"axis":{"id":"p1046"}}},{"type":"object","name":"Grid","id":"p1055","attributes":{"dimension":1,"axis":{"id":"p1051"}}},{"type":"object","name":"Legend","id":"p1079","attributes":{"items":[{"type":"object","name":"LegendItem","id":"p1080","attributes":{"label":{"type":"value","value":"Intensity"},"renderers":[{"id":"p1076"}]}}]}}]}}]}}
+    <script type="application/json" id="e41d81d3-5d03-4123-9be4-ffc9b5588c23">
+      {"fd54e0c0-d5d5-42e7-a288-3ce6c948630d":{"version":"3.4.1","title":"Bokeh Application","roots":[{"type":"object","name":"Figure","id":"p1034","attributes":{"width":700,"height":500,"x_range":{"type":"object","name":"DataRange1d","id":"p1035"},"y_range":{"type":"object","name":"DataRange1d","id":"p1036"},"x_scale":{"type":"object","name":"LinearScale","id":"p1044"},"y_scale":{"type":"object","name":"LinearScale","id":"p1045"},"title":{"type":"object","name":"Title","id":"p1037","attributes":{"text":"Mass spectrum of molecule"}},"renderers":[{"type":"object","name":"GlyphRenderer","id":"p1076","attributes":{"data_source":{"type":"object","name":"ColumnDataSource","id":"p1070","attributes":{"selected":{"type":"object","name":"Selection","id":"p1071","attributes":{"indices":[],"line_indices":[]}},"selection_policy":{"type":"object","name":"UnionRenderers","id":"p1072"},"data":{"type":"map","entries":[["x",{"type":"ndarray","array":{"type":"bytes","data":"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"},"shape":[1000],"dtype":"float64","order":"little"}],["y",{"type":"ndarray","array":{"type":"bytes","data":"AAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAADd8HIapI0lA2q+yMIk6SsLgHNxFkgOoRIh9Dk2WayDGRZo+JquatUfo5nPzAwBliXwpz+WMlbFKkZZUvvIhmMv4A5lMYbdcDP35/Uh9X7rNv4FTkRVJ9U5okhAGgi4Ljy+YepMAQ31PZUcpT2uOis/65xBkdue0D8zSADFRybjP3bWRQe00mQ/EZ3gJbdeVT4kzPIly7K0PLFMyAbE64I6XsJguudSwDeVHGtORJVqNF4pwJKhbYQwue55icehDSzwlaIfdEgEJ0g3Mm3aNGohhwe5u9P0PxvNzaBpfWOCFC8/ET4b+TMN2UQ9nXl5VAUDAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAO1tGuDvQDQDJrfyiJtJNQtGtrWczR2lEh3Ib5PoxIMZ2kKFL6x30R8Aq7eF3iGNJXyBndKF7bYqlrSdY8YHUS8etZkTo+BXM/DJhGl4mM82GVT87Ka6szkA5r6D8UAHPMYIrooA3sk9u3rWfSoo+z4SxSUlfuiaP6y09ia3Kak/MimbkEg1Jj/axytDnH8SPglGtFioFW08+dIdTUCUNTosagBhizhuNz7/hCPc+BM0Ter9Hv7pKDCH0D0l61StK3kaqZC1S6AmKPQtwsEWASEKl3zXyunQGqvul8zJmA8UUraXR+Hauwz+KqTuBS3XBAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAr61YON6JMAOc9XDelzcsC1gIyTzXt5YSLRqTqzZDcRmukBlvasK4HxhOvSEGwnAluTEQXsZolSrExCHbatApL6KznislYC0zb8j9A5iMnzZAwVlTmfp/ObNqDLygl847iyKYyeKeiz0s9/35KYm3PjwFC+t77VI/5WjG6HC7XD+OFoOA8ZTUPvx5aEJK1Ls9EDGW9LjBETwspcpVymLVOaRq/0UUTwg3KjXEWQAUqjOjdE/6SGe6L74YFajlOjkr/V/e+ejAJiaU5gh52V2DIF/CcRVGHU8a1OyRQM+WhxMO9XH16OAwDI+/eYjTy0YEAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA46m/+0KceA2u0Bf69ORUL0JLV9om9exK2VCqhvxtRGXSgcSyU6pMffIBFeLvhRSVdrTOIkLBmKmztJYhzNPYu8YlkzESC9DJFz1qZpuBhNkliNvJiaj05atb8aPXWhjuT6fkdqLxAPVctt3iYJmc+oigTLuo4/j5Q3I/vNp4CP7GGnJo0pnU+6TbmT0LCVz2Ewo1itZuoO1LQHsAiDmg5ZcX41FgxljaBoPJw01IzM4d+2jVGwj8vDmLC2ZuhuCqbKS4eiQeiJfYTpyEP6fgf9TeP/Mg9wBlZbf5F5vzzEpAZQntDN5cL1RfDbQdzqQMAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAANy0q412ogEDiBmSLADS8wpo3Iy4TQZVEh0BRiVkDCUZzTS4oTzjYx+tQV0UDbwRJefHesTm2S0qgqYqK/S1ty4xUZWsU8axMsT9O6nFJhk2b554rGPL8Djvbce/7io1OwpLb/sNLuk8E1UPodBEDD7rK1lT3POdPoShWFPc850+N80NodBEDD5LBW37DS7pPEfBxL/uKjU7GOR1rGPL8Dhs/zapxSYZNlUlkaxTxrEyDDwkK/S1ty4Kn3HE5tktKoUsVxQNvBElxquwoTzjYx/BRD0lZAwlGRBgg7hNBlUSv2+ILADS8wrCeaKNdqIBAwAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA1Fa6tVvK2QIlz8DA7YbHCspXt+F8QSQStpdUZoR18BiVGSz4iT4pH5l1lExnRdIkWJrbgSH26ClkHfWYoBdwLrpSbXEilWMyewuQVoB9xjVcia5armCYOGF5e8sm8Ng6aQCei8kTiDyJqZqlfvClPQc0wCsa3jI+YVaWWp+gLj4yJvKLCXaXPTm3rOMW9nA8b9kjNlUltzpx5GdrU89tOJmB2Vj/HZI1tcDrD6XIJDLDK7WwpYAmLlk2m5Vs/pYpSZdNx9EsdiTDbw7q6y7EHpqFc7V0VoEY8MOH2bocrBFoLgXYk4JFCnwGyrkCEU8CAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAADIiuQpU2mnAq4miQ6GVZEKXVR8Ssk56BHe4VEIPvSvGI339iyn4+MepQO5Lx1ehyR/pLwSNumZKWQFJMW0HRsuAu64vCzICjLgn4VtB/doNTZa+JKL9jU4ww17R2c8cjrVIo3dj5QcPCyKG4wkIzU9AOybiPOBvT0PPzFKQXCzPRJF4rzFKxg9Kgy7bLdd7DsPmnFT/WovOgchAjTFa+A3DqhOiUgzADVCdKK7GSuOMebxS07EgootiBb/87D89ShpB6XWzTXRI0h/XnJ6bRkehPcc8nq60ReAFrrJzFT3EPTIA4+L+owJFoBM8iH8kAEAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAACiWra7RHmgCuN76X379TAoex+1qOHGgEZhwwfE/mmEYw3LZ+gvJkR5Ww2tfufUwJB46kFnwhj4pwYLaRuztuS1px8UNO8mkMUn2oGzXc/80t6EbTGN1xjenb0KLGUX+OWTH2EybQKM70XHxn/sctzx27xciPjA6PVLglmQ6ASw9MlU3DH9DjDwE7Sd44OtaO0bSIxiNM5g5FpUU0nyIRDfOdc8QDnFgNMZc7cDA2egwBHyETXS54SyloDIRu9xHKKGq3R/PUR4j0hCFiektYh3LsCh6KZMUF5BnZ9Qc+jUQLH96xLMnxgioJejGPhTFAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAou3nejWYFQK0Xfpg0RD1CQfVAh8DZUMRaiLtxS3aABi6MAcW3KMrHsh+2XiBZMUjLj8pDMJAzyhVFmqSt4tFLavY4i6MCSwxesjW6II3gTTB0EYzvvRDN54HFbqp1HU54QjxZP2JFjvW7eh7UfYlPJKzPmh1MqQ8vmiWa56HkTxuIMCkArjsOy2Ndz3PM7Y6buMssB0z8Di9xzzqk0+WNv/Z97YFAK0zBU6Op7bJMTBOXPUcPpgkLDzWzIsBgYYn8mYRczQ1VyJ2pAFwnJaWHFkIrWXcv0QWljNuXiP9YQ9efPxqBHDtB6sJg3Bv1wIAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAA="},"shape":[1000],"dtype":"float64","order":"little"}]]}}},"view":{"type":"object","name":"CDSView","id":"p1077","attributes":{"filter":{"type":"object","name":"AllIndices","id":"p1078"}}},"glyph":{"type":"object","name":"Line","id":"p1073","attributes":{"x":{"type":"field","field":"x"},"y":{"type":"field","field":"y"},"line_color":"#1f77b4"}},"nonselection_glyph":{"type":"object","name":"Line","id":"p1074","attributes":{"x":{"type":"field","field":"x"},"y":{"type":"field","field":"y"},"line_color":"#1f77b4","line_alpha":0.1}},"muted_glyph":{"type":"object","name":"Line","id":"p1075","attributes":{"x":{"type":"field","field":"x"},"y":{"type":"field","field":"y"},"line_color":"#1f77b4","line_alpha":0.2}}}}],"toolbar":{"type":"object","name":"Toolbar","id":"p1043","attributes":{"autohide":true,"tools":[{"type":"object","name":"PanTool","id":"p1056"},{"type":"object","name":"WheelZoomTool","id":"p1057","attributes":{"renderers":"auto"}},{"type":"object","name":"BoxZoomTool","id":"p1058","attributes":{"overlay":{"type":"object","name":"BoxAnnotation","id":"p1059","attributes":{"syncable":false,"level":"overlay","visible":false,"left":{"type":"number","value":"nan"},"right":{"type":"number","value":"nan"},"top":{"type":"number","value":"nan"},"bottom":{"type":"number","value":"nan"},"left_units":"canvas","right_units":"canvas","top_units":"canvas","bottom_units":"canvas","line_color":"black","line_alpha":1.0,"line_width":2,"line_dash":[4,4],"fill_color":"lightgrey","fill_alpha":0.5}}}},{"type":"object","name":"SaveTool","id":"p1064"},{"type":"object","name":"ResetTool","id":"p1065"},{"type":"object","name":"HelpTool","id":"p1066"},{"type":"object","name":"WheelPanTool","id":"p1068","attributes":{"dimension":"height"}},{"type":"object","name":"WheelZoomTool","id":"p1069","attributes":{"dimensions":"height","renderers":"auto"}}]}},"left":[{"type":"object","name":"LinearAxis","id":"p1051","attributes":{"ticker":{"type":"object","name":"BasicTicker","id":"p1052","attributes":{"mantissas":[1,2,5]}},"formatter":{"type":"object","name":"BasicTickFormatter","id":"p1053"},"major_label_policy":{"type":"object","name":"AllLabels","id":"p1054"}}}],"below":[{"type":"object","name":"LinearAxis","id":"p1046","attributes":{"ticker":{"type":"object","name":"FixedTicker","id":"p1067","attributes":{"ticks":[115.13973499999994,114.13637999999995,113.13302499999995],"minor_ticks":[]}},"formatter":{"type":"object","name":"BasicTickFormatter","id":"p1048"},"major_label_policy":{"type":"object","name":"AllLabels","id":"p1049"}}}],"center":[{"type":"object","name":"Grid","id":"p1050","attributes":{"axis":{"id":"p1046"}}},{"type":"object","name":"Grid","id":"p1055","attributes":{"dimension":1,"axis":{"id":"p1051"}}},{"type":"object","name":"Legend","id":"p1079","attributes":{"items":[{"type":"object","name":"LegendItem","id":"p1080","attributes":{"label":{"type":"value","value":"Intensity"},"renderers":[{"id":"p1076"}]}}]}}]}}]}}
     </script>
     <script type="text/javascript">
       (function() {
         const fn = function() {
           Bokeh.safely(function() {
             (function(root) {
               function embed_document(root) {
-              const docs_json = document.getElementById('dad7ef00-fcce-44bc-86b8-ec254633b475').textContent;
-              const render_items = [{"docid":"49f429a0-2af3-40ad-987a-166cca72bd10","roots":{"p1034":"b188c5d6-ce2c-4b2e-b8df-2f0bfa41c640"},"root_ids":["p1034"]}];
+              const docs_json = document.getElementById('e41d81d3-5d03-4123-9be4-ffc9b5588c23').textContent;
+              const render_items = [{"docid":"fd54e0c0-d5d5-42e7-a288-3ce6c948630d","roots":{"p1034":"bb07d693-12cb-44fd-a2ae-e662e409b64e"},"root_ids":["p1034"]}];
               root.Bokeh.embed.embed_items(docs_json, render_items);
               }
               if (root.Bokeh !== undefined) {
                 embed_document(root);
               } else {
                 let attempts = 0;
                 const timer = setInterval(function(root) {
```

### Comparing `cheminterface_ppchem-1.0/THOMAS_IS_BEST/functions.py` & `cheminterface_ppchem-2.0/THOMAS_IS_BEST/copy_file.py`

 * *Files 10% similar despite different names*

```diff
@@ -76,19 +76,20 @@
 
     Input: molecule under SMILEs representation
     
     Output: molecule under MOL representation
     '''
     #---------------------------------------------------------------------------------------------#
 
-    #Checks that the SMILEs input is correct
+    #Checks that the SMILEs input is correct/allowed
 
     mol_without_Hs = Chem.MolFromSmiles(mol_smi)
 
     if mol_without_Hs is None:
+        print('')
         print("Invalid SMILEs input.")
         print('Please try again with a different SMILEs.')
         exit()
 
     mol = Chem.AddHs(mol_without_Hs)
 
     return mol
@@ -127,50 +128,45 @@
         #Check that there is in fact a proton to remove
         list_atoms.remove('H')
     return list_atoms
 
 
 
 
-def main_function (list_atoms):
+
+
+def main_function (list_atoms, imprecision_True_False):
     #---------------------------------------------------------------------------------------------#
     '''
     main_function(list_atoms)
     
     Input: list of atoms that enter the apparatus
     
     Output: two lists:
     1. list of the masses (of individual molecules) of each possible combination of isotopes
     2. list of the probabilities of apparation of each of the molecules 
     (the mass in list 1 at index i is associated to the probability at index i in list 2)
     '''
     #---------------------------------------------------------------------------------------------#
-
-    
-
-    '''In the case of ionisation by proton, we need to add a H+ ion, which is done in the following'''
-    
+    render_imprecise_list = imprecision_True_False #Set arg to be True for long molecules, set arg to False for short molecules/if precision for minuscule peaks is important
 
     #check for sulphur and nitrogen
 
     has_N = False
     count_N = 0
     has_S = False
     count_S = 0
-    if 'N' in list_atoms:
+    if 'N' in list_atoms and list_atoms.count('N')%2 == 1:
         has_N = True
         count_N = list_atoms.count('N')
-    elif 'S' in list_atoms:
+    elif 'S' in list_atoms and list_atoms.count('S')%2 == 1:
         has_S = True
         count_S = list_atoms.count('S')
 
 
-
-    
-
     print(list_atoms)
 
     list_output = []
     mass_copy = mass.copy()
     abundance_copy = abundance.copy()
     isotopes_copy = isotopes.copy()
 
@@ -204,31 +200,43 @@
 
 
                 #This for-loop runs over all isotope types of the atom type in pos 0 in list_atoms (input list)
 
                 index = isotopes.index(list_atoms[0])
                 new_mass = list_output[i][0] + mass_copy[index]
                 new_proba = list_output[i][1] * abundance_copy[index]
-                list_output_new.append([new_mass,new_proba])
+
+
+                #removes any molecule who's probability is below 0.0001
+
+                if render_imprecise_list: #only removes low-probability arrangements if render_imprecise_list arg is True
+                    if new_proba>0.0001:
+                        list_output_new.append([new_mass,new_proba])
+
+                else:
+                    list_output_new.append([new_mass,new_proba])
+
                 mass_copy.pop(index)
                 abundance_copy.pop(index)
                 isotopes_copy.pop(index)
                 
         list_output = list_output_new
         list_atoms.pop(0)
 
 
     #Conversion of list_output (which is a list of lists) to a combination of two lists (x_axis & y_axis)
 
     x_axis, y_axis = [],[]
     x_axis_final, y_axis_final = [],[]
     for j in range (len(list_output)):
-        x_axis.append(list_output[j][0])
-        y_axis.append(list_output[j][1])
-
+        '''x_axis.append(list_output[j][0])'''
+        x_axis.append(round(list_output[j][0],3)) # Adds rounded value (should help with Python-limitations that render a diff of magnitude 10^(-7) to combinatorics
+        
+        y_axis.append(list_output[j][1]) #Adds the true value
+        
 
     #Compression of lists x_axis & y_axis into x_axis_final & y_axis_final so that peaks corresponding to same mass will be represented together 
     
     for j in range (len(x_axis)):
             if x_axis.count(x_axis[j]) == 1:
                 x_axis_final.append(x_axis[j])
                 y_axis_final.append(y_axis[j])
@@ -254,16 +262,55 @@
     if has_N:
         x_axis_final.append(x_axis_final[index] - 0.006)  
         y_axis_final.append(0.0035*count_N*maximum)  
     
     if has_S:
         x_axis_final.append(x_axis_final[index]-0.004)  
         y_axis_final.append(0.008*count_S*maximum)  
+
     return x_axis_final, y_axis_final
 
+
+def list_sorter (x_in, y_in):
+
+    #---------------------------------------------------------------------------------------------#
+    '''
+    list_sorter (x_in, y_in)
+    
+    Input: two lists:
+    1. list of the masses (of individual molecules) of each possible combination of isotopes
+    2. list of the probabilities of apparation of each of the molecules 
+    (the mass in list 1 at index i is associated to the probability at index i in list 2)
+    
+    Output: two lists:
+    1. (x_out): sorted list
+    2. (y_out): sorted list
+
+    Functionality: sorts lists to have sorted list in x
+    '''
+    #---------------------------------------------------------------------------------------------#
+
+    x_out, y_out = [],[]
+    print(len(x_in))
+    while len(x_in)>0:
+        min_x = min(x_in)
+        index_min = x_in.index(min_x)
+        x_out.append(min_x)
+        y_out.append(y_in[index_min])
+        x_in.pop(index_min)
+        y_in.pop(index_min)
+    print(len(x_out))
+    return x_out, y_out
+    
+
+
+
+def peak_merger (x_axis_final, y_axis_final):
+    return
+
 def matplotlib_plotter(x_axis_final, y_axis_final):
 
     #---------------------------------------------------------------------------------------------#
     '''
     matplotlib_plotter(x_axis_final, y_axis_final)
     
     Input: two lists:
@@ -273,71 +320,76 @@
     
     Output: none
 
     Functionality: plots a graph made of dots with matplotlib
     '''
     #---------------------------------------------------------------------------------------------#
 
-    max_x = max(x_axis_final)
-    min_x = min(x_axis_final)
-    diff = (max_x-min_x)
-    x_axis_final_use = x_axis_final.copy()
-    y_axis_final_use = y_axis_final.copy()
-
-    for i in range(int(-(100*diff)/10),int(11*(100*diff)/10)):
-        x_axis_final_use.append(i/100 + min_x)
-        y_axis_final_use.append(0)
-    x_final_final = []
-    y_final_final = []
-    while len(x_axis_final_use)>1 :
-        minx = min(x_axis_final_use)
-        index = x_axis_final_use.index(minx)
-        x_final_final.append(minx)
-        y_final_final.append(y_axis_final_use[index])
-        x_axis_final_use.pop(index)
-        y_axis_final_use.pop(index)
-
+    x_axis, y_axis = [],[]
+    for i in range (len(x_axis_final)):
+        x_axis.append(x_axis_final[i]-0.0000003)
+        x_axis.append(x_axis_final[i])
+        x_axis.append(x_axis_final[i]+0.0000003)
+        y_axis.append(0)
+        y_axis.append(y_axis_final[i])
+        y_axis.append(0)
+        
 
     #plotting with matpotlib
-    plt.scatter(x_axis_final,y_axis_final)
-    plt.show()
-    return
+    plt.plot(x_axis,y_axis)
+    
+    return x_axis, y_axis
 
 def pyplot_plotter (x_axis_final, y_axis_final):
 
     #---------------------------------------------------------------------------------------------#
     '''
     pyplot_plotter (x_axis_final, y_axis_final)
     
     Input: two lists:
     1. list of the masses (of individual molecules) of each possible combination of isotopes
     2. list of the probabilities of apparation of each of the molecules 
     (the mass in list 1 at index i is associated to the probability at index i in list 2) 
     
-    Output: none
+    Output: p (plot of mass spectrum on bokeh)
 
-    Functionality: plots graph with plotly (html format)
+    Functionality: none
     '''
     #---------------------------------------------------------------------------------------------#
+    x_axis, y_axis = [min(x_axis_final)-1],[0]
+    max_x = max(x_axis_final)
+    for i in range (len(x_axis_final)):
+        x_axis.append(x_axis_final[i]-0.0000003)
+        x_axis.append(x_axis_final[i])
+        x_axis.append(x_axis_final[i]+0.0000003)
+        y_axis.append(0)
+        y_axis.append(y_axis_final[i])
+        y_axis.append(0)
+    x_axis.append(max_x+1)
+    y_axis.append(0)
 
-    x, y = x_axis_final, y_axis_final
+    x, y = x_axis, y_axis
     fig = go.Figure()
-    fig.add_trace(go.Scatter(x = x,y = y, mode = 'markers'))
+    fig.add_trace(go.Scatter(x = x,y = y, mode = 'lines'))
 
     fig.update_layout(xaxis=dict(rangeslider=dict(visible=True), 
                                 type="linear"),
-                                yaxis=dict(range=[min(y)-1, max(y)], 
+                                yaxis=dict(range=[min(y)-0.1, max(y)+0.1], 
                                 type="linear"),
                                 dragmode='zoom',
                                 )
 
 
     fig.show()
     return 
 
+
+def lorentzian(x, eps):
+    return 1.0 / (np.pi * eps * (1 + (x / eps) ** 2))
+
 def bokeh_plotter(x_axis_final, y_axis_final):
 
     #---------------------------------------------------------------------------------------------#
     '''
     bokeh_plotter(x_axis_final, y_axis_final)
     
     Input: two lists:
@@ -347,53 +399,62 @@
     
     Output: none
 
     Functionality: plots graph with bokeh (html format)
     '''
     #---------------------------------------------------------------------------------------------#
 
-    x = 0.004
+    eps = 10**(-4)
 
     mass_range = np.linspace(min(x_axis_final)-1, max(x_axis_final)+1, 1000)
 
     intensity = np.zeros_like(mass_range)
 
     for peak_position, peak_intensity in zip(x_axis_final, y_axis_final):
-
-        peak_shape = peak_intensity * np.exp(-((mass_range - peak_position) ** 2) / (2 * x ** 2))  # Gaussian example
+        peak_shape = peak_intensity * lorentzian(mass_range - peak_position, eps)  # Lorentzian example
 
         intensity += peak_shape
 
 
+
     ticked_peaks = []
     for i in range(len(x_axis_final)):
         if y_axis_final[i]>0.0001:
             ticked_peaks.append(round(x_axis_final[i],4))
 
-    print(ticked_peaks)
 
     # Create a new plot with a title and axis labels
-    p = figure(title="Simulated Mass Spectrum", x_axis_label='Mass [Th]', y_axis_label='Intensity [AU]')
+    p = figure(title="Simulated Mass Spectrum", x_axis_label='Mass [m/z]', y_axis_label='Intensity [AU]')
     p = figure(width=700 , title= f'Mass spectrum of molecule')
     p.height = 500
     p.xaxis.ticker = FixedTicker(ticks= ticked_peaks)
-    p.toolbar.autohide = True
+    p.toolbar.autohide = False
     p.add_tools(WheelPanTool(dimension="height"))
     p.add_tools(WheelZoomTool(dimensions="height"))
 
     # Add a line renderer with legend and line thickness
     p.line(mass_range, intensity, legend_label="Intensity", line_width=1)
 
     # Show the plot
-    show(p) 
-    return 
+    show(p)
+    print('')
+    return  (f'Computation complete.')
 
+print('')
 
+mol_smi = input('Enter SMILEs: ')
 
+start_time = time.time()
 
-mol_smi = input('Enter SMILEs: ')
 mol = SMILEs_interpreter(mol_smi)
 mass, abundance, isotopes = data_list_generator()
 list_atoms_pre = molecule_list_generator(mol) 
 list_atoms = ionisation_method(list_atoms_pre)
-xvalues, yvalues = main_function(list_atoms)
-print(bokeh_plotter(xvalues,yvalues))
+xvalues_pre, yvalues_pre = main_function(list_atoms, True)
+xvalues, yvalues = list_sorter(xvalues_pre, yvalues_pre)
+
+end_time = time.time()
+
+duration = end_time-start_time
+
+print(pyplot_plotter(xvalues,yvalues))
+print(f'Process took: {duration} s')
```

### Comparing `cheminterface_ppchem-1.0/Thomas/Copy_spectrometer.py` & `cheminterface_ppchem-2.0/Thomas/Copy_spectrometer.py`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-1.0/Thomas/Thomas_return.html` & `cheminterface_ppchem-2.0/Thomas/Thomas_return.html`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-1.0/Thomas/Thomas_return_pyplot.html` & `cheminterface_ppchem-2.0/Thomas/Thomas_return_pyplot.html`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-1.0/Thomas/Thomas_return_pyplot.py` & `cheminterface_ppchem-2.0/Thomas/Thomas_return_pyplot.py`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-1.0/Thomas/tests.py` & `cheminterface_ppchem-2.0/Thomas/tests.py`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-1.0/src/ChemInterface_ppchem/ChemInterface.py` & `cheminterface_ppchem-2.0/src/ChemInterface_ppchem/ChemInterface.py`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-1.0/LICENSE.txt` & `cheminterface_ppchem-2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cheminterface_ppchem-1.0/README.md` & `cheminterface_ppchem-2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-# - Cheminterface_alpha 2.3.07 package -
+# - ChemInterface package for applied mass spectrometry -
 #### Project in practical programming in chemistry course
+#### EPFL CH-200
 
-This repository provides the user a package which will display an interactive interface where the user will be able to input the SMILES of a molecule. The interface will be able to give specific information about the molecule such as its molecular mass, its organic functional groups or its degree of insaturation. The most important part of the package will provide a way to simulate the mass spectrometry of the given molecule. 
+This repository provides the user with a package which will display an interactive interface where the user will be able to input the SMILEs of a molecule. The interface will be able to give specific information about the molecule such as its molecular mass, its organic functional groups or its degree of insaturation. The most important part of the package will provide a way to simulate the mass spectrum of the given molecule. 
 
 Developpers:
 - Thomas Christianson, genius coder and CTO of SwissChemInfoTech, https://github.com/ThomasCsson
 - Igor Gonteri, brilliant back-end developper and founder of AppliedOrbitals.Org, https://github.com/igorgonteri
-- Arthur Humery, leading expert amongst the new generation of Computational Chemical Programmers and CEO of Plastogaz, https://github.com/Arthurhmy
+- Arthur Humery, leading expert amongst the new generation of Computational Chemical Programmers and CEO of the United Kingdom of Great Britain and Northern Ireland, https://github.com/Arthurhmy
 
 **What is mass spectrometry ?**
    - Mass spectrometry is an analytical technique used to identify and quantify chemical compounds in a sample by measuring the mass and sometimes the charge of molecules. It involves separating ions according to their mass-to-charge ratio (m/z), then detecting and analysing them. This method is widely used in chemistry, biochemistry, pharmacology and other fields to characterise substances and understand their structure and composition.
 
 Let us go through the steps required to make this package.
 
 #### Imported packages
 
-In order to run the package correctly, the following packages need to be installed using the following command
+In order to run the package correctly, the following packages need to be installed before running any pip-installed functions using the following command
 
 ```bash
 pip install matplotlib
 pip install bokeh
 pip install rdkit
 pip install numpy
 pip install pandas
```

### Comparing `cheminterface_ppchem-1.0/pyproject.toml` & `cheminterface_ppchem-2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,42 +1,33 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ChemInterface_ppchem"
-version = "1.0"
+version = "2.0"
 description = "..."
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
 keywords = ["unsaturation", "Mass spectroscopy"]
 authors = [
   { name = "Thomas Christianson", email = "thomas.christiansson@epfl.ch" },
   { name = "Igor Gonteri", email = "igor.gonteri@epfl.ch" },
   { name = "Arthur Humery", email = "arthur.humery@epfl.ch" }
 ]
 dependencies = [
-  "blas==1.0",
   "bzip2==1.0.8",
   "ca-certificates==2024.3.11",
-  "intel-openmp==2023.1.0",
   "libffi==3.4.4",
-  "mkl==2023.1.0",
-  "mkl-service==2.4.0",
-  "mkl_fft==1.3.8",
-  "mkl_random==1.2.4",
-  "numpy==1.26.4",
-  "numpy-base==1.26.4",
   "openssl==3.0.13",
   "pip==23.3.1",
   "python==3.10.12",
   "setuptools==68.2.2",
-  "sqlite==3.41.2",
-  "tbb==2021.8.0",
+  "sqlite==3.45.3",
   "tk==8.6.12",
   "vc==14.2",
   "vs2015_runtime==14.27.29016",
   "wheel==0.41.2",
   "xz==5.4.6",
   "zlib==1.2.13"
 ]
@@ -44,8 +35,8 @@
     "Development Status :: 4 - Beta",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 
 [project.urls]
-Homepage = "https://github.com/ThomasCsson/ppchem-project-Christiansson-Gonteri-Humery.git"
+Homepage = "https://github.com/ThomasCsson/ppchem-project-Christiansson-Gonteri-Humery.git"
```

### Comparing `cheminterface_ppchem-1.0/PKG-INFO` & `cheminterface_ppchem-2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,56 @@
 Metadata-Version: 2.3
 Name: ChemInterface_ppchem
-Version: 1.0
+Version: 2.0
 Summary: ...
 Project-URL: Homepage, https://github.com/ThomasCsson/ppchem-project-Christiansson-Gonteri-Humery.git
 Author-email: Thomas Christianson <thomas.christiansson@epfl.ch>, Igor Gonteri <igor.gonteri@epfl.ch>, Arthur Humery <arthur.humery@epfl.ch>
 License-Expression: MIT
 License-File: LICENSE.txt
 Keywords: Mass spectroscopy,unsaturation
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
-Requires-Dist: blas==1.0
 Requires-Dist: bzip2==1.0.8
 Requires-Dist: ca-certificates==2024.3.11
-Requires-Dist: intel-openmp==2023.1.0
 Requires-Dist: libffi==3.4.4
-Requires-Dist: mkl-fft==1.3.8
-Requires-Dist: mkl-random==1.2.4
-Requires-Dist: mkl-service==2.4.0
-Requires-Dist: mkl==2023.1.0
-Requires-Dist: numpy-base==1.26.4
-Requires-Dist: numpy==1.26.4
 Requires-Dist: openssl==3.0.13
 Requires-Dist: pip==23.3.1
 Requires-Dist: python==3.10.12
 Requires-Dist: setuptools==68.2.2
-Requires-Dist: sqlite==3.41.2
-Requires-Dist: tbb==2021.8.0
+Requires-Dist: sqlite==3.45.3
 Requires-Dist: tk==8.6.12
 Requires-Dist: vc==14.2
 Requires-Dist: vs2015-runtime==14.27.29016
 Requires-Dist: wheel==0.41.2
 Requires-Dist: xz==5.4.6
 Requires-Dist: zlib==1.2.13
 Description-Content-Type: text/markdown
 
-# - Cheminterface_alpha 2.3.07 package -
+# - ChemInterface package for applied mass spectrometry -
 #### Project in practical programming in chemistry course
+#### EPFL CH-200
 
-This repository provides the user a package which will display an interactive interface where the user will be able to input the SMILES of a molecule. The interface will be able to give specific information about the molecule such as its molecular mass, its organic functional groups or its degree of insaturation. The most important part of the package will provide a way to simulate the mass spectrometry of the given molecule. 
+This repository provides the user with a package which will display an interactive interface where the user will be able to input the SMILEs of a molecule. The interface will be able to give specific information about the molecule such as its molecular mass, its organic functional groups or its degree of insaturation. The most important part of the package will provide a way to simulate the mass spectrum of the given molecule. 
 
 Developpers:
 - Thomas Christianson, genius coder and CTO of SwissChemInfoTech, https://github.com/ThomasCsson
 - Igor Gonteri, brilliant back-end developper and founder of AppliedOrbitals.Org, https://github.com/igorgonteri
-- Arthur Humery, leading expert amongst the new generation of Computational Chemical Programmers and CEO of Plastogaz, https://github.com/Arthurhmy
+- Arthur Humery, leading expert amongst the new generation of Computational Chemical Programmers and CEO of the United Kingdom of Great Britain and Northern Ireland, https://github.com/Arthurhmy
 
 **What is mass spectrometry ?**
    - Mass spectrometry is an analytical technique used to identify and quantify chemical compounds in a sample by measuring the mass and sometimes the charge of molecules. It involves separating ions according to their mass-to-charge ratio (m/z), then detecting and analysing them. This method is widely used in chemistry, biochemistry, pharmacology and other fields to characterise substances and understand their structure and composition.
 
 Let us go through the steps required to make this package.
 
 #### Imported packages
 
-In order to run the package correctly, the following packages need to be installed using the following command
+In order to run the package correctly, the following packages need to be installed before running any pip-installed functions using the following command
 
 ```bash
 pip install matplotlib
 pip install bokeh
 pip install rdkit
 pip install numpy
 pip install pandas
```

