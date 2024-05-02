# Comparing `tmp/cocoon_data-0.1.8.tar.gz` & `tmp/cocoon_data-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cocoon_data-0.1.8.tar", last modified: Tue Jan  2 19:07:37 2024, max compression
+gzip compressed data, was "cocoon_data-0.1.9.tar", last modified: Thu Jan  4 17:29:58 2024, max compression
```

## Comparing `cocoon_data-0.1.8.tar` & `cocoon_data-0.1.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 zh2408    (1024) zh2408    (1025)        0 2024-01-02 19:07:37.448747 cocoon_data-0.1.8/
--rw-r--r--   0 zh2408    (1024) zh2408    (1025)     1063 2023-12-03 21:26:43.000000 cocoon_data-0.1.8/LICENSE
--rw-r--r--   0 zh2408    (1024) zh2408    (1025)      331 2024-01-02 19:07:37.448747 cocoon_data-0.1.8/PKG-INFO
--rw-r--r--   0 zh2408    (1024) zh2408    (1025)     6567 2023-12-06 15:28:26.000000 cocoon_data-0.1.8/README.md
-drwxr-xr-x   0 zh2408    (1024) zh2408    (1025)        0 2024-01-02 19:07:37.448747 cocoon_data-0.1.8/cocoon_data/
--rw-r--r--   0 zh2408    (1024) zh2408    (1025)   450343 2024-01-02 19:07:24.000000 cocoon_data-0.1.8/cocoon_data/__init__.py
-drwxr-xr-x   0 zh2408    (1024) zh2408    (1025)        0 2024-01-02 19:07:37.448747 cocoon_data-0.1.8/cocoon_data.egg-info/
--rw-r--r--   0 zh2408    (1024) zh2408    (1025)      331 2024-01-02 19:07:37.000000 cocoon_data-0.1.8/cocoon_data.egg-info/PKG-INFO
--rw-r--r--   0 zh2408    (1024) zh2408    (1025)      224 2024-01-02 19:07:37.000000 cocoon_data-0.1.8/cocoon_data.egg-info/SOURCES.txt
--rw-r--r--   0 zh2408    (1024) zh2408    (1025)        1 2024-01-02 19:07:37.000000 cocoon_data-0.1.8/cocoon_data.egg-info/dependency_links.txt
--rw-r--r--   0 zh2408    (1024) zh2408    (1025)      217 2024-01-02 19:07:37.000000 cocoon_data-0.1.8/cocoon_data.egg-info/requires.txt
--rw-r--r--   0 zh2408    (1024) zh2408    (1025)       12 2024-01-02 19:07:37.000000 cocoon_data-0.1.8/cocoon_data.egg-info/top_level.txt
--rw-r--r--   0 zh2408    (1024) zh2408    (1025)       38 2024-01-02 19:07:37.448747 cocoon_data-0.1.8/setup.cfg
--rw-r--r--   0 zh2408    (1024) zh2408    (1025)      633 2024-01-02 19:07:32.000000 cocoon_data-0.1.8/setup.py
+drwxr-xr-x   0 zh2408    (1024) zh2408    (1025)        0 2024-01-04 17:29:58.288308 cocoon_data-0.1.9/
+-rw-r--r--   0 zh2408    (1024) zh2408    (1025)     1063 2023-12-03 21:26:43.000000 cocoon_data-0.1.9/LICENSE
+-rw-r--r--   0 zh2408    (1024) zh2408    (1025)      331 2024-01-04 17:29:58.288308 cocoon_data-0.1.9/PKG-INFO
+-rw-r--r--   0 zh2408    (1024) zh2408    (1025)     6567 2023-12-06 15:28:26.000000 cocoon_data-0.1.9/README.md
+drwxr-xr-x   0 zh2408    (1024) zh2408    (1025)        0 2024-01-04 17:29:58.284308 cocoon_data-0.1.9/cocoon_data/
+-rw-r--r--   0 zh2408    (1024) zh2408    (1025)   453257 2024-01-04 17:26:24.000000 cocoon_data-0.1.9/cocoon_data/__init__.py
+drwxr-xr-x   0 zh2408    (1024) zh2408    (1025)        0 2024-01-04 17:29:58.288308 cocoon_data-0.1.9/cocoon_data.egg-info/
+-rw-r--r--   0 zh2408    (1024) zh2408    (1025)      331 2024-01-04 17:29:58.000000 cocoon_data-0.1.9/cocoon_data.egg-info/PKG-INFO
+-rw-r--r--   0 zh2408    (1024) zh2408    (1025)      224 2024-01-04 17:29:58.000000 cocoon_data-0.1.9/cocoon_data.egg-info/SOURCES.txt
+-rw-r--r--   0 zh2408    (1024) zh2408    (1025)        1 2024-01-04 17:29:58.000000 cocoon_data-0.1.9/cocoon_data.egg-info/dependency_links.txt
+-rw-r--r--   0 zh2408    (1024) zh2408    (1025)      217 2024-01-04 17:29:58.000000 cocoon_data-0.1.9/cocoon_data.egg-info/requires.txt
+-rw-r--r--   0 zh2408    (1024) zh2408    (1025)       12 2024-01-04 17:29:58.000000 cocoon_data-0.1.9/cocoon_data.egg-info/top_level.txt
+-rw-r--r--   0 zh2408    (1024) zh2408    (1025)       38 2024-01-04 17:29:58.288308 cocoon_data-0.1.9/setup.cfg
+-rw-r--r--   0 zh2408    (1024) zh2408    (1025)      633 2024-01-04 17:26:10.000000 cocoon_data-0.1.9/setup.py
```

### Comparing `cocoon_data-0.1.8/LICENSE` & `cocoon_data-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cocoon_data-0.1.8/README.md` & `cocoon_data-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `cocoon_data-0.1.8/cocoon_data/__init__.py` & `cocoon_data-0.1.9/cocoon_data/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,17 +348,17 @@
     return overlap, only_set1, only_set2
 
 
 
 
 
 
-def create_column_selector(columns, callback):
+def create_column_selector(columns, callback, default=False):
     labels = [widgets.Label(column) for column in columns]
-    checkboxes = [widgets.Checkbox(value=False) for _ in columns]
+    checkboxes = [widgets.Checkbox(value=default) for _ in columns]
     widgets_list = [item for pair in zip(labels, checkboxes) for item in pair]
 
     grid = widgets.GridBox(widgets_list, layout=widgets.Layout(grid_template_columns="repeat(2, auto)"))
 
     def update_checkboxes(value):
         for checkbox in checkboxes:
             checkbox.value = value
@@ -379,14 +379,15 @@
 
     submit_button.on_click(on_submit)
 
     display(grid, buttons_box, submit_button, output)
 
 
 
+
 def find_duplicate_indices(df):
     if not isinstance(df, pd.DataFrame):
         raise ValueError("Input must be a pandas DataFrame")
 
     duplicates = df[df.duplicated(keep=False)]
     
     if duplicates.empty:
@@ -439,16 +440,15 @@
     return missing_column_indices
 
 def display_and_ask_removal(df, missing_column_indices):
     html_output = f"<p>🤔 There are {len(missing_column_indices)} columns <b>with all missing values</b>:</p>"
     display(HTML(html_output))
 
     df_sample = color_columns(df.head(), 'lightgreen', missing_column_indices)
-    display(HTML(wrap_in_scrollable_div(df_sample.to_html())))
-
+    display(HTML(wrap_in_scrollable_div(truncate_html_td(df_sample.to_html()))))
 
     display(HTML("<p>🧐 Select the columns you want to remove:</p>"))
 
 
 
 
 
@@ -478,30 +478,29 @@
 
 def display_duplicated_columns_html(df, duplicate_column_indices):
     html_output = f"<p>🤔 There are {len(duplicate_column_indices)} groups of duplicated column names.</p>"
 
 
     for group in duplicate_column_indices:
 
-        col_name = df_sample.columns[group[0]]
+        col_name = df.columns[group[0]]
         
-        new_column_names = df_sample.columns.tolist()
+        new_column_names = df.columns.tolist()
 
         for i, idx in enumerate(group):
-            new_column_names[idx] = f"{df_sample.columns[idx]} ({i+1})"
+            new_column_names[idx] = f"{df.columns[idx]} ({i+1})"
         
-        df_sample.columns = new_column_names
+        df.columns = new_column_names
 
     colors = generate_seaborn_palette(len(duplicate_column_indices))
 
     styled_df = color_columns_multiple(df.head(), colors, duplicate_column_indices)
 
     display(HTML(html_output))
-    display(HTML(wrap_in_scrollable_div(styled_df.to_html())))
-
+    display(HTML(wrap_in_scrollable_div(truncate_html_td(styled_df.to_html()))))
 
     display(HTML("<p>🧐 Select the columns you want to remove:</p>"))
 
 
 def find_duplicate_column_indices(df):
     if not isinstance(df, pd.DataFrame):
         raise ValueError("Input must be a pandas DataFrame")
@@ -560,29 +559,29 @@
 
 def display_xy_duplicated_columns_html(df, duplicate_column_indices):
     html_output = f"<p>🤔 There are {len(duplicate_column_indices)} groups of column names, duplicated likely by merge.</p>"
 
 
     for group in duplicate_column_indices:
 
-        col_name = df_sample.columns[group[0]]
+        col_name = df.columns[group[0]]
         
-        new_column_names = df_sample.columns.tolist()
+        new_column_names = df.columns.tolist()
 
         for i, idx in enumerate(group):
-            new_column_names[idx] = f"{df_sample.columns[idx]}"
+            new_column_names[idx] = f"{df.columns[idx]}"
         
-        df_sample.columns = new_column_names
+        df.columns = new_column_names
 
     colors = generate_seaborn_palette(len(duplicate_column_indices))
 
     styled_df = color_columns_multiple(df.head(), colors, duplicate_column_indices)
 
     display(HTML(html_output))
-    display(HTML(wrap_in_scrollable_div(styled_df.to_html())))
+    display(HTML(wrap_in_scrollable_div(truncate_html_td(styled_df.to_html()))))
 
     display(HTML("<p>🧐 Select the columns you want to remove:</p>"))
 
 
 
 
 def find_default_index_column(df):
@@ -602,15 +601,15 @@
     
 def display_index_and_ask_removal(df, missing_column_indices):
     html_output = f"<p>🤔 There are {len(missing_column_indices)} columns <b>for row id</b>:</p>"
 
     df_sample = color_columns(df.head(), 'lightgreen', missing_column_indices)
 
     display(HTML(html_output))
-    display(HTML(wrap_in_scrollable_div(df_sample.to_html())))
+    display(HTML(wrap_in_scrollable_div(truncate_html_td(df_sample.to_html()))))
 
     display(HTML("<p>🧐 Select the columns you want to remove:</p>"))
 
 
 
 
 
@@ -963,15 +962,15 @@
 
     plt.figure(figsize=(plot_width, 3), dpi=100)
     bar_plot = sns.barplot(x=missing_percent.index, y=missing_percent, color="lightgreen")
 
     for index, value in enumerate(missing_percent):
         bar_plot.text(index, value, f'{value:.2f}%', color='black', ha="center", fontsize=8)
 
-    plt.title('Missing Values %', fontsize=8)
+    plt.title('Missing % (for Columns with Missing Values)', fontsize=8)
     plt.ylabel('%', fontsize=10)
     plt.xticks(rotation=45, fontsize=6)
     plt.yticks(fontsize=8)
     plt.tight_layout()
 
     buffer = BytesIO()
     plt.savefig(buffer, format='png')
@@ -2339,14 +2338,15 @@
 
         self.rename_step_finished = False
         self.drop_duplicated_row_step_finished = False
         self.drop_duplicated_colulmn_step_finished = False
         self.drop_all_missing_columns_step_finished = False
         self.drop_x_y_columns_step_finished = False
         self.drop_index_column_step_finished = False
+        self.project_step_finished = False
 
     def get_summary(self):
         return self.document["table_summary"]["summary"]
 
     def transform(self):
         if not hasattr(self, 'cleaner'):
             self.cleaner = DataCleaning(self)
@@ -2433,15 +2433,15 @@
         else:
             next_step()
 
     
 
 
     def start_document(self, viewer=None):
-        next_step = self.check_duplicated_rows
+        next_step = self.decide_project
 
         self.viewer = viewer
         
         if self.viewer is  None:
             mode_selector = widgets.RadioButtons(
                 options=[
                     ('Table Viewer 👀: I’m not familiar with the table. Please provide your best guess.', 'Table Viewer'),
@@ -3322,14 +3322,33 @@
         accuracy_question, on_button_clicked = create_widgets_for_column_grouping()
 
         display(accuracy_question)
 
         if self.viewer:
             on_button_clicked(None)
 
+        
+    
+    def execute_project(self):
+        next_step = self.check_duplicated_rows
+
+        if self.project_step_finished:
+            next_step()
+
+        keep_column_indices = self.document["project"]
+        remove_column_indices = [i for i in range(len(self.df.columns)) if i not in keep_column_indices]
+
+        if len(remove_column_indices) > 0:
+            remove_columns_step = RemoveColumnsStep(sample_df = self.df[:2], col_indices = remove_column_indices, name="Project Columns")
+            self.pipeline.add_step_to_final(remove_columns_step)
+            self.df = self.pipeline.run_codes()
+        
+        self.project_step_finished = True
+        next_step()
+
     def execute_drop_x_y_columns(self):
         next_step = self.check_index_columns
 
         if self.drop_x_y_columns_step_finished:
             next_step()
 
         remove_column_indices = self.document["x_y_columns"]["remove_columns"]
@@ -3436,14 +3455,52 @@
 
 
         next_step()
 
     def generate_pipeline(self):
         return self.pipeline
 
+
+    def decide_project(self, overwrite=False, once=False):
+        
+        next_step = self.execute_project
+
+        if "project" not in self.document:
+            pass
+        else:
+            if not overwrite:
+                write_log("Warning: project already exists in the document.")
+                if not once:
+                    next_step()
+                return
+        
+        create_progress_bar_with_numbers(0, doc_steps)
+
+        df = self.df
+
+        df_sample = df.head()
+        display(HTML(wrap_in_scrollable_div(truncate_html_td(df_sample.to_html()))))
+
+        num_cols = len(df.columns)
+
+        display(HTML(f"<p>🧐 There are <b>{num_cols}</b> columns. Please select the columns that you want to keep.</p>"))
+
+        column_names = self.df.columns.to_list()
+
+        def callback_next(selected_indices):
+            clear_output(wait=True)
+            self.document["project"] = selected_indices
+            next_step()
+
+        create_column_selector(column_names, callback_next, default=True)
+
+        if self.viewer:
+            callback_next(list(range(num_cols)))
+            
+
     def check_duplicated_rows(self, overwrite=False, once=False):
 
         next_step = self.execute_deduplicated_rows
 
         if "duplicate_rows" not in self.document or \
            "duplicated_indices" not in self.document["duplicate_rows"] or\
             "remove_duplicates" not in self.document["duplicate_rows"]:
@@ -6468,54 +6525,60 @@
 
         explanation_label = widgets.Label('Task:')
         explanation_text = widgets.Textarea(
             value = self.explanation if self.explanation != "" else "Transform ... For example ...",
             layout=widgets.Layout(width='95%', height='200px')
         )
         submit_button = widgets.Button(description="Submit Task")
+        submit_spinner = widgets.HTML()
 
         def on_submit_clicked(b):
             print("Generating codes...")
+            submit_spinner.value = "<i class='fa fa-spinner fa-spin'></i>"
             self.generate_codes(explanation = explanation_text.value)
-
             codes_text.value = self.codes
             reason_label.value = self.reason
+            submit_spinner.value = ""
             print("Done")
 
         submit_button.on_click(on_submit_clicked)
+        submit_box = widgets.HBox([submit_button, submit_spinner])
 
         codes_label = widgets.Label('Codes:')
         codes_text = widgets.Textarea(
             value=self.codes,
             layout=widgets.Layout(width='95%', height='200px')
         )
         run_button = widgets.Button(description="Run Codes")
+        run_spinner = widgets.HTML()
+
         reason_label = widgets.Label(layout=Layout(width='100%', overflow='auto', white_space='pre-wrap'))
         output_label = widgets.Label()
 
         def on_run_clicked(b):
             print("Running codes...")
-
+            run_spinner.value = "<i class='fa fa-spinner fa-spin'></i>"
             output = self.run_codes(dfs = self.sample_df, codes = codes_text.value)
             if isinstance(output, str):
                 error_label.value = "<span style='color: red;'>" + output.replace("\n", "<br>") + "</span>"
                 output_df_widget.value = ""
             else:
                 error_label.value = ""
                 output_df_widget.value = output.to_html(border=0)
+            run_spinner.value = ""
             print("Done")
                 
-
         run_button.on_click(on_run_clicked)
+        run_box = widgets.HBox([run_button, run_spinner])
 
 
         panel_layout = Layout(width='400px')
 
-        left_panel = widgets.VBox([explanation_label, explanation_text, submit_button], layout=panel_layout)
-        right_panel = widgets.VBox([codes_label, codes_text, run_button, output_label], layout=panel_layout)
+        left_panel = widgets.VBox([explanation_label, explanation_text, submit_box], layout=panel_layout)
+        right_panel = widgets.VBox([codes_label, codes_text, run_box, output_label], layout=panel_layout)
         display(widgets.HBox([left_panel, right_panel]))
         display(reason_label)
 
         input_df_label = widgets.Label('Input Table:')
         display(input_df_label)
         display(HTML(self.sample_df.to_html(border=0)))
 
@@ -6602,34 +6665,37 @@
     def verify_input(self, df):
         if not set(self.agg_cols).issubset(df.columns):
             raise ValueError(f"Columns {self.agg_cols} are not in the input dataframe.")
 
     def postprocessing(self, df):
         if not isinstance(df, pd.DataFrame):
             raise ValueError("Output is not a pandas dataframe.")
+
+        if not set(self.agg_cols).issubset(df.columns):
+            raise ValueError(f"Columns {self.agg_cols} are not in the output dataframe.")
         
         if df.index.name is not None:
             df = df.reset_index()
         return df
 
     def generate_codes(self, explanation=None):
         if explanation is None:
             explanation = self.explanation
             
         template = f"""Transformation task: Given input df, write python codes that aggregate and ouput df.
 ===
 Input Df:
 {self.sample_df.df[:2].to_csv()}
 ===
-Transformation Requirement
-The final output df should group by {self.agg_cols}.
+Transformation Requirement:
+Aggregate {self.agg_cols}.
 {explanation}
 
 Do the following:
-1. First reason about how to transform
+1. First reason about how to transform. The final output df should group by only attributes: {self.agg_cols}
 2. Then fill in the python function, with detailed comments. 
 DONT change the function name, first line and the return clause.
 
 {{
     "reason": "To transform, we need to ...",
     "codes": "def transform(input_df):\\n    output_df = input_df.copy()\\n    ...\\n    return output_df"
 }}
@@ -8425,19 +8491,24 @@
         if col in columns_to_copy:
             new_df[col] = df[col].copy()
         else:
             new_df[col] = df[col]
 
     return new_df
 
+
+
 def plot_efficient_grid(df, x_col, y_col, value_col=None):
+
     if value_col:
         value_columns = [value_col]
     else:
-        value_columns = [col for col in df.columns if col not in [x_col, y_col]]
+        numeric_columns = df.select_dtypes(include=np.number).columns
+        value_columns = [col for col in numeric_columns if col not in [x_col, y_col]]
+        value_columns = value_columns[:5]
 
     n_rows = len(value_columns)
     fig, axs = plt.subplots(n_rows, 1, figsize=(6, 3 * n_rows))
 
     if n_rows == 1:
         axs = [axs]
 
@@ -9495,14 +9566,18 @@
             gdf_html = self.gdf.head(5).to_html()
             gdf_html = truncate_html_td(gdf_html)
             html += gdf_html
         elif hasattr(self, 'df'):
             df_html = self.df.head(5).to_html()
             df_html = truncate_html_td(df_html)
             html += df_html
+        elif hasattr(self, 'np_array'):
+            np_array = self.np_array
+            html += f"<br>NumPy arraay shape: {np_array.shape}<br>"
+            html += "<br>"
 
         html += self.display_html(value_att=value_att)
         return html
 
     def display(self, value_att=None):
         html_img = self.display_html(value_att=value_att)
         if hasattr(self, 'gdf'):
@@ -10244,23 +10319,25 @@
 
     display(radio_buttons, geo_transform_widgets, resolution_widget, button)
 
 
 
 
 def truncate_html_td(html, max_length=30):
-    pattern = r'(<td>)(.*?)(</td>)'
+    pattern = r'(<td[^>]*>)(.*?)(</td>)'
     
     def truncate_match(match):
-        content = match.group(2)
+        content = match.group(2).strip()
         if len(content) > max_length:
             content = content[:max_length] + '...'
         return match.group(1) + content + match.group(3)
 
-    return re.sub(pattern, truncate_match, html)
+    return re.sub(pattern, truncate_match, html, flags=re.DOTALL)
+
+
 
 def save_np_array_as_raster(np_array, output_path, meta):
     if np_array.ndim == 2:
         height, width = np_array.shape
         count = 1
     elif np_array.ndim == 3:
         count, height, width = np_array.shape
@@ -10346,15 +10423,15 @@
             
             to_df_button = widgets.Button(description="To DataFrame")
 
             to_df_button.on_click(on_to_df_clicked)
             box = widgets.VBox([to_df_button])
             boxes.append(box)
 
-        label = widgets.HTML(value=f"🎲 Want to perform an ad hoc transformation?")
+        label = widgets.HTML(value=f"🎲 Want to perform an ad hoc transformation?\n⚠️ Currently, ad hoc transformation can't change CRS or file type.")
 
         def on_ad_hoc_clicked(b):
             clear_output(wait=True)
             self.create_ad_hoc_step()
 
         adhoc_button = widgets.Button(description="Ad hoc")
         adhoc_button.on_click(on_ad_hoc_clicked)
@@ -10762,15 +10839,15 @@
             df = self.doc_dfs[i].df
             json_code = self.document["candidate_longitude_latitude"][id_str]
 
             column_indices = [[df.columns.get_loc(pair["longitude_name"]), df.columns.get_loc(pair["latitude_name"])] for pair in json_code]
 
             colors = generate_seaborn_palette(len(column_indices))
             styled_df = color_columns_multiple(df.head(), colors, column_indices)
-            display(HTML(wrap_in_scrollable_div(styled_df.to_html())))
+            display(HTML(wrap_in_scrollable_div(truncate_html_td(styled_df.to_html()))))
             
             
             def call_back(longitude, latitude):
                 self.document["decided_longitude_latitude"][id_str] = [longitude, latitude]
                 self.ask_for_attributes()
             
             display_longitude_latitude(json_code, list(df.columns), call_back)
```

### Comparing `cocoon_data-0.1.8/setup.py` & `cocoon_data-0.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='cocoon_data',
-    version='0.1.8',
+    version='0.1.9',
     packages=find_packages(),
     install_requires=open('requirements.txt').read().splitlines(),
     extras_require={
         'geo': [
             'geopandas==0.14.1', 
             'rasterio',  
             "pyproj",
```

