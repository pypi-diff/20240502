# Comparing `tmp/ipyslides-3.7.3.tar.gz` & `tmp/ipyslides-3.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipyslides-3.7.3.tar", last modified: Thu Mar 14 13:31:40 2024, max compression
+gzip compressed data, was "ipyslides-3.7.4.tar", last modified: Thu May  2 19:50:55 2024, max compression
```

## Comparing `ipyslides-3.7.3.tar` & `ipyslides-3.7.4.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-03-14 13:31:40.286661 ipyslides-3.7.3/
--rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.7.3/LICENSE
--rw-rw-rw-   0        0        0     5382 2024-03-14 13:31:40.283742 ipyslides-3.7.3/PKG-INFO
--rw-rw-rw-   0        0        0     4493 2024-02-21 04:16:19.000000 ipyslides-3.7.3/README.md
-drwxrwxrwx   0        0        0        0 2024-03-14 13:31:40.156335 ipyslides-3.7.3/ipyslides/
--rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.7.3/ipyslides/__init__.py
--rw-rw-rw-   0        0        0       25 2024-03-14 11:35:18.000000 ipyslides-3.7.3/ipyslides/__version__.py
-drwxrwxrwx   0        0        0        0 2024-03-14 13:31:40.274388 ipyslides-3.7.3/ipyslides/_base/
--rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.7.3/ipyslides/_base/__init__.py
--rw-rw-rw-   0        0        0    39921 2024-03-14 11:15:42.000000 ipyslides-3.7.3/ipyslides/_base/_layout_css.py
--rw-rw-rw-   0        0        0     5120 2024-02-21 00:47:59.000000 ipyslides-3.7.3/ipyslides/_base/_widgets.py
--rw-rw-rw-   0        0        0    32753 2024-03-14 12:26:14.000000 ipyslides-3.7.3/ipyslides/_base/base.py
--rw-rw-rw-   0        0        0     7567 2024-02-21 03:26:19.000000 ipyslides-3.7.3/ipyslides/_base/export_html.py
--rw-rw-rw-   0        0        0     6572 2024-02-21 00:10:04.000000 ipyslides-3.7.3/ipyslides/_base/export_template.py
--rw-rw-rw-   0        0        0    10773 2024-01-12 15:19:53.000000 ipyslides-3.7.3/ipyslides/_base/icons.py
--rw-rw-rw-   0        0        0    12233 2024-03-14 11:51:45.000000 ipyslides-3.7.3/ipyslides/_base/intro.py
-drwxrwxrwx   0        0        0        0 2024-03-14 13:31:40.280379 ipyslides-3.7.3/ipyslides/_base/js/
--rw-rw-rw-   0        0        0    12146 2024-02-21 00:47:42.000000 ipyslides-3.7.3/ipyslides/_base/js/interaction.js
--rw-rw-rw-   0        0        0     1483 2023-12-18 19:56:12.000000 ipyslides-3.7.3/ipyslides/_base/js/notes.js
--rw-rw-rw-   0        0        0     3737 2024-01-23 22:26:12.000000 ipyslides-3.7.3/ipyslides/_base/navigation.py
--rw-rw-rw-   0        0        0     2464 2023-11-26 19:40:40.000000 ipyslides-3.7.3/ipyslides/_base/notes.py
--rw-rw-rw-   0        0        0    13157 2024-01-19 17:58:40.000000 ipyslides-3.7.3/ipyslides/_base/screenshot.py
--rw-rw-rw-   0        0        0    23399 2024-02-24 17:42:30.000000 ipyslides-3.7.3/ipyslides/_base/settings.py
--rw-rw-rw-   0        0        0    28788 2024-03-08 17:11:40.000000 ipyslides-3.7.3/ipyslides/_base/slide.py
--rw-rw-rw-   0        0        0    28254 2024-03-06 23:50:13.000000 ipyslides-3.7.3/ipyslides/_base/styles.py
--rw-rw-rw-   0        0        0    15380 2024-03-14 11:53:55.000000 ipyslides-3.7.3/ipyslides/_base/widgets.py
--rw-rw-rw-   0        0        0    15373 2024-03-14 11:51:27.000000 ipyslides-3.7.3/ipyslides/_demo.py
--rw-rw-rw-   0        0        0    49517 2024-03-14 12:36:15.000000 ipyslides-3.7.3/ipyslides/core.py
--rw-rw-rw-   0        0        0    17494 2024-02-24 17:41:41.000000 ipyslides-3.7.3/ipyslides/formatters.py
--rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.7.3/ipyslides/source.py
--rw-rw-rw-   0        0        0    29143 2024-03-08 03:23:55.000000 ipyslides-3.7.3/ipyslides/utils.py
--rw-rw-rw-   0        0        0    13884 2024-03-09 15:23:53.000000 ipyslides-3.7.3/ipyslides/writer.py
--rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.7.3/ipyslides/xmd.py
-drwxrwxrwx   0        0        0        0 2024-03-14 13:31:40.219869 ipyslides-3.7.3/ipyslides.egg-info/
--rw-rw-rw-   0        0        0     5382 2024-03-14 13:31:39.000000 ipyslides-3.7.3/ipyslides.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      854 2024-03-14 13:31:39.000000 ipyslides-3.7.3/ipyslides.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-14 13:31:39.000000 ipyslides-3.7.3/ipyslides.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      134 2024-03-14 13:31:39.000000 ipyslides-3.7.3/ipyslides.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-14 13:31:39.000000 ipyslides-3.7.3/ipyslides.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-14 13:31:40.287654 ipyslides-3.7.3/setup.cfg
--rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.7.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 19:50:55.851592 ipyslides-3.7.4/
+-rw-rw-rw-   0        0        0     1090 2023-02-22 21:18:51.000000 ipyslides-3.7.4/LICENSE
+-rw-rw-rw-   0        0        0     5382 2024-05-02 19:50:55.850591 ipyslides-3.7.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4493 2024-02-21 04:16:19.000000 ipyslides-3.7.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 19:50:55.811317 ipyslides-3.7.4/ipyslides/
+-rw-rw-rw-   0        0        0      394 2024-03-14 11:52:17.000000 ipyslides-3.7.4/ipyslides/__init__.py
+-rw-rw-rw-   0        0        0       25 2024-05-02 18:51:45.000000 ipyslides-3.7.4/ipyslides/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 19:50:55.844320 ipyslides-3.7.4/ipyslides/_base/
+-rw-rw-rw-   0        0        0      283 2023-02-22 21:18:52.000000 ipyslides-3.7.4/ipyslides/_base/__init__.py
+-rw-rw-rw-   0        0        0    40549 2024-05-02 17:36:10.000000 ipyslides-3.7.4/ipyslides/_base/_layout_css.py
+-rw-rw-rw-   0        0        0     5191 2024-05-02 17:09:40.000000 ipyslides-3.7.4/ipyslides/_base/_widgets.py
+-rw-rw-rw-   0        0        0    32956 2024-05-02 18:42:52.000000 ipyslides-3.7.4/ipyslides/_base/base.py
+-rw-rw-rw-   0        0        0     7547 2024-04-30 19:43:44.000000 ipyslides-3.7.4/ipyslides/_base/export_html.py
+-rw-rw-rw-   0        0        0     6572 2024-02-21 00:10:04.000000 ipyslides-3.7.4/ipyslides/_base/export_template.py
+-rw-rw-rw-   0        0        0    11523 2024-05-02 17:07:46.000000 ipyslides-3.7.4/ipyslides/_base/icons.py
+-rw-rw-rw-   0        0        0    12178 2024-05-02 17:12:13.000000 ipyslides-3.7.4/ipyslides/_base/intro.py
+drwxrwxrwx   0        0        0        0 2024-05-02 19:50:55.844320 ipyslides-3.7.4/ipyslides/_base/js/
+-rw-rw-rw-   0        0        0    12184 2024-05-02 17:09:03.000000 ipyslides-3.7.4/ipyslides/_base/js/interaction.js
+-rw-rw-rw-   0        0        0     1483 2023-12-18 19:56:12.000000 ipyslides-3.7.4/ipyslides/_base/js/notes.js
+-rw-rw-rw-   0        0        0     3737 2024-01-23 22:26:12.000000 ipyslides-3.7.4/ipyslides/_base/navigation.py
+-rw-rw-rw-   0        0        0     2464 2023-11-26 19:40:40.000000 ipyslides-3.7.4/ipyslides/_base/notes.py
+-rw-rw-rw-   0        0        0    13157 2024-05-02 15:59:52.000000 ipyslides-3.7.4/ipyslides/_base/screenshot.py
+-rw-rw-rw-   0        0        0    22978 2024-05-02 19:12:44.000000 ipyslides-3.7.4/ipyslides/_base/settings.py
+-rw-rw-rw-   0        0        0    28848 2024-05-02 18:42:52.000000 ipyslides-3.7.4/ipyslides/_base/slide.py
+-rw-rw-rw-   0        0        0    28254 2024-03-06 23:50:13.000000 ipyslides-3.7.4/ipyslides/_base/styles.py
+-rw-rw-rw-   0        0        0    15531 2024-05-02 19:13:37.000000 ipyslides-3.7.4/ipyslides/_base/widgets.py
+-rw-rw-rw-   0        0        0    15373 2024-05-02 19:35:56.000000 ipyslides-3.7.4/ipyslides/_demo.py
+-rw-rw-rw-   0        0        0    49800 2024-05-02 19:49:43.000000 ipyslides-3.7.4/ipyslides/core.py
+-rw-rw-rw-   0        0        0    17494 2024-02-24 17:41:41.000000 ipyslides-3.7.4/ipyslides/formatters.py
+-rw-rw-rw-   0        0        0     9073 2024-02-24 17:26:11.000000 ipyslides-3.7.4/ipyslides/source.py
+-rw-rw-rw-   0        0        0    29143 2024-03-08 03:23:55.000000 ipyslides-3.7.4/ipyslides/utils.py
+-rw-rw-rw-   0        0        0    13884 2024-03-09 15:23:53.000000 ipyslides-3.7.4/ipyslides/writer.py
+-rw-rw-rw-   0        0        0    28883 2024-03-14 13:18:35.000000 ipyslides-3.7.4/ipyslides/xmd.py
+drwxrwxrwx   0        0        0        0 2024-05-02 19:50:55.832824 ipyslides-3.7.4/ipyslides.egg-info/
+-rw-rw-rw-   0        0        0     5382 2024-05-02 19:50:55.000000 ipyslides-3.7.4/ipyslides.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      854 2024-05-02 19:50:55.000000 ipyslides-3.7.4/ipyslides.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 19:50:55.000000 ipyslides-3.7.4/ipyslides.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      134 2024-05-02 19:50:55.000000 ipyslides-3.7.4/ipyslides.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-02 19:50:55.000000 ipyslides-3.7.4/ipyslides.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 19:50:55.851592 ipyslides-3.7.4/setup.cfg
+-rw-rw-rw-   0        0        0     3730 2023-12-09 17:54:29.000000 ipyslides-3.7.4/setup.py
```

### Comparing `ipyslides-3.7.3/LICENSE` & `ipyslides-3.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.3/PKG-INFO` & `ipyslides-3.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.7.3
+Version: 3.7.4
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.7.3/README.md` & `ipyslides-3.7.4/README.md`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.3/ipyslides/_base/_layout_css.py` & `ipyslides-3.7.4/ipyslides/_base/_layout_css.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
                     },  # Hide in screenshot
                     ".Menu-Box" : {"display": "none !important",},
                 },
                 "^.PresentMode .SlideBox .SlideArea .ProxyPasteBtns": {
                     "display": "none !important"
                 },  # Hide in presentation mode
                 "^.FullWindow, ^.FullScreen": {
-                    ".Width-Slider": {"display": "none !important"},
+                    ".Width-Slider, .Source-Btn": {"display": "none !important"},
                 },
                 "^.FullScreen": {
                     ".FullWindow-Btn": {"display": "none !important"},
                 },
                 "@keyframes heart-beat": {
                     "from": {
                         "transform": "translateX(-16px)",
@@ -333,15 +333,15 @@
                     ".Menu-Box": {
                         "width": "0 !important",
                         "transition": "width 400ms ease-in-out", # transition on exit
                         "overflow": "hidden !important", # needs to not jump on chnage of width
                     },
                     "^:hover, ^:focus, ^:active, ^.mod-active, ^.Active-Start" : {
                         ".Menu-Box" : {
-                            "width": "104px !important", # 3*28 + margin + paddings
+                            "width": "132px !important", # 4*28 + margin + paddings
                             "transition": "width 400ms ease-in-out", # transition on enter hover
                              "overflow": "hidden !important", # avoid jump on hover too
                         },
                     },
                     ".Toc-Btn, .Menu-Btn, .Screenshot-Btn": {
                         "min-width": "28px",
                         "width": "28px", # need this too
@@ -657,14 +657,28 @@
                 ".fa.fa-plus": Icon(
                     "dots", color=accent_color, size=_icons_size
                 ).css,
                 ".fa.fa-minus": Icon(
                     "close", color=accent_color, size=_icons_size
                 ).css,
             },
+            ".Source-Btn": {
+                ".fa.fa-plus": Icon(
+                    "code", color=accent_color, size=_icons_size
+                ).css,
+            },
+            "<.Scroll-Btn": { # top level
+                "color": "var(--jp-brand-color1,skyblue) !important",
+                "background": "transparent !important",
+                "^:hover": {"font-weight": "bold !important",},
+                "^:hover, ^:focus, ^:active, ^.mod-active" : {
+                    "box-shadow": "none !important",
+                    "outline": "none !important",
+                },
+            },
             "@media print": { # Needs modification
                 ".SlidesWrapper": {
                     "^, ^.FullWindow": {
                         "height": "auto !important",
                     },
                 },
                 ".Controls, .NavWrapper button, div.LaserPointer": {
```

### Comparing `ipyslides-3.7.3/ipyslides/_base/_widgets.py` & `ipyslides-3.7.4/ipyslides/_base/_widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,16 @@
             self._toggles.laser.value = not self._toggles.laser.value
         elif msg == 'ZOOM':
             self._toggles.zoom.value = not self._toggles.zoom.value
         elif msg == 'TPAN':
             self._buttons.setting.click()
         elif msg == 'SCAP':
             self._buttons.capture.click()
+        elif msg == 'EDIT':
+            self._buttons.source.click()
         elif msg == 'TVP' and not self._toggles.window.disabled:
             self._toggles.window.value = not self._toggles.window.value
         elif msg == 'NOVP': # Other than voila, no viewport button
             self._toggles.window.disabled = True
             self._toggles.window.layout.display = 'none'
         elif msg == 'LOADED':
             if self._checks.notes.value: # Notes window already there
```

### Comparing `ipyslides-3.7.3/ipyslides/_base/base.py` & `ipyslides-3.7.4/ipyslides/_base/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -314,23 +314,26 @@
                     ' Verify code is safe and try again with argument `trusted = True`.'
                     ' Never run files that you did not create yourself or not verified by you.')
         
         chunks = _parse_markdown_text(content)
             
         handles = self.create(*range(start, start + len(chunks))) # create slides faster or return older
 
-        with self.skip_post_run_cell():
-            for i,chunk in enumerate(chunks):
-                # Must run under this function to create frames with two dashes (--) and update only if things/variables change
-                checks = (str(chunk) != getattr(handles[i],'_mdff',''), re.findall(r"\`\{(.*?)\}\`", chunk, flags=re.DOTALL), 'Out-Sync' in handles[i].dom_classes,)
-                if  any(checks):
-                    with self._loading_private(self.widgets.buttons.refresh): # Hold and disable other refresh button while doing it
-                        self._slide(f'{i + start} -m', chunk)
+        for i,chunk in enumerate(chunks):
+            # Must run under this function to create frames with two dashes (--) and update only if things/variables change
+            checks = (str(chunk) != getattr(handles[i],'_mdff',''), re.findall(r"\`\{(.*?)\}\`", chunk, flags=re.DOTALL), 'Out-Sync' in handles[i].dom_classes,)
+            if any(checks):
+                with self._loading_private(self.widgets.buttons.refresh): # Hold and disable other refresh button while doing it
+                    self._slide(f'{i + start} -m', chunk)
+            else: # when slide is not built, scroll buttons still need an update to point to correct button
+                self._slides_per_cell.append(handles[i])
+                for frame in handles[i].frames:
+                    self._slides_per_cell.append(frame)
 
-                handles[i]._mdff = str(chunk) # This is need for update while editing, chunk could be ns_str, avoid that
+            handles[i]._mdff = str(chunk) # This is need for update while editing, chunk could be ns_str, avoid that
         
         # Return refrence to slides for quick update, frames should be accessed by slide.frames
         return handles
     
     def sync_with_file(self, start, path, trusted = False, interval=500):
         """Auto update slides when content of markdown file changes. You can stop syncing using `Slides.unsync` function.
         interval is in milliseconds, 500 ms default. Read `Slides.from_markdown` docs about content of file.
```

### Comparing `ipyslides-3.7.3/ipyslides/_base/export_html.py` & `ipyslides-3.7.4/ipyslides/_base/export_html.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     # Should be used inside Slides class only.
     def __init__(self, _instance_BaseSlides):
         self.main = _instance_BaseSlides
         self.main.widgets.buttons.export.on_click(self._export) # Export button
         
     def _htmlize(self, **kwargs):
         "page_size, slide_number are in kwargs"
-        navui_class = 'NavHidden' if self.main.widgets.checks.navgui.value else '' # it hides when True
+        navui_class = '' if self.main.widgets.checks.navgui.value else 'NavHidden' 
         content = ''
         for item in self.main:
             _html = '' 
             for out in item.contents:
                 _html += f'<div style="width: 100%; box-sizing:border-box;">{_fmt_html(out)}</div>' # Important to have each content in a div, so that it can be same as notebook content
             
             if hasattr(item,'_refs'):
```

### Comparing `ipyslides-3.7.3/ipyslides/_base/export_template.py` & `ipyslides-3.7.4/ipyslides/_base/export_template.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.3/ipyslides/_base/icons.py` & `ipyslides-3.7.4/ipyslides/_base/icons.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,14 +103,25 @@
         </svg>''',
     'zoom-out': '''
         <svg height="{size}" viewBox="0 0 25 25" xmlns="http://www.w3.org/2000/svg" stroke-width="2" stroke-linecap="round" transform="rotate({rotation})">
             <circle cx="9" cy="9" r="8" fill="none" stroke="{color}"/>
             <line x1="17" y1="17" x2="21" y2="21" stroke="{color}" stroke-width="4"/>
             <line x1="6" y1="9" x2="12" y2="9" stroke="{color}"/>
         </svg>''',
+    'search': '''
+        <svg height="{size}" viewBox="0 0 25 25" xmlns="http://www.w3.org/2000/svg" stroke-width="2" stroke-linecap="round" transform="rotate({rotation})">
+            <circle cx="9" cy="9" r="8" fill="none" stroke="{color}"/>
+            <line x1="17" y1="17" x2="21" y2="21" stroke="{color}" stroke-width="4"/>
+        </svg>''',
+    'code': '''
+        <svg height="{size}" viewBox="0 0 25 25" xmlns="http://www.w3.org/2000/svg" fill="none" stroke="{color}" stroke-width="2.5" stroke-linecap="round" stroke-linejoin="round">
+            <polyline points="7 8 2 13 7 18"></polyline>
+            <polyline points="18 8 23 13 18 18"></polyline>
+            <line x1="15" y1="4" x2="11" y2="21"></line>
+        </svg>''',
     'win-maximize': '''
         <svg height="{size}" viewBox="0 0 25 25" xmlns="http://www.w3.org/2000/svg" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
             <polygon points="2 4,23 4,23 21,2 21,2 4" fill="none" stroke="{color}"></polygon>
             <polygon points="2 4,23 4,23 8,2 8,2 4" fill="{color}" stroke="{color}"></polygon>
         </svg>''',
     'win-restore': '''
         <svg height="{size}" viewBox="0 0 25 25" xmlns="http://www.w3.org/2000/svg" stroke-width="2" stroke-linecap="round" stroke-linejoin="round">
```

### Comparing `ipyslides-3.7.3/ipyslides/_base/intro.py` & `ipyslides-3.7.4/ipyslides/_base/intro.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,14 @@
     ::: text-box
         sup`1`My University is somewhere in the middle of nowhere
         sup`2`Their University is somewhere in the middle of nowhere
 
 ::: note-warning
     Python 3.8+, ipywidgets 8+, IPython 8.7+ are required. Previous version 2.x.x will still be supported for bug fixes.
 
-::: note-info
-    Slides are shown after each run of cell (where a slide is present) by default to make user experience better (get output where you run). You can disable this by calling `Slides.settings.show_always(False)`.
-
 **After you initialize `slides = ipyslides.Slides()`**
 
 - `%%slide integer` on cell top auto picks slide and `%%title` auto picks title page.
 - `%%slide integer -m` can be used to create slide from full markdown (extended one).
 - You can use context managers like `with slides.slide(): ...` and `with slides.title(): ...` in place of `%%slide` and `%%title` respectively.
 - Inside python script, you can use auto numbering with `slides.AutoSlides().[get_next_number|title|slide|frames|from_markdown]`.
 
@@ -135,14 +132,15 @@
     "S": "Take screenshot",
     "P": "Print PDF of current slide",
     "F": "Toggle fullscreen",
     "Esc": "Exit fullscreen",
     "V": "Toggle fit to viewport [voila only]",
     "G": "Toggle settings panel",
     "L": "Toggle LASER pointer",
+    "E": "Edit Source Cell of Current Slide", 
     "K": "Show keyboard shortcuts",
 }
 
 key_combs = f"""
 | Shortcut                                    | Button                                            | Action                 | 
 |---------------------------------------------|---------------------------------------------------|------------------------|
 | {_key('&#9141;')}/{_key('▸')}               | {_icons["R"]}, {_icons["D"]}                      | Move to next slide     |
@@ -151,14 +149,15 @@
 | {_key('Ctrl')} + {_key('[1-9]')}/{_key('[1-9]')} |                                       | Shift [1-9] slides left/right |
 | {_key('Z')}                                 | {_icons["zoom-in"]}, {_icons["zoom-out"]}         | {key_maps["Z"]}        |
 | {_key('S')}                                 | {_icons["camera"]}                                | {key_maps["S"]}        |
 | {_key('F')}                                 | {_icons["expand"]}, {_icons["compress"]}          | {key_maps["F"]}        |
 | {_key('Esc')}                               |                                                   | {key_maps["Esc"]}      |
 | {_key('V')}                                 | {_icons["win-maximize"]}, {_icons["win-restore"]} | {key_maps["V"]}        |
 | {_key('G')}                                 | {_icons["settings"]}, {_icons["close"]}           | {key_maps["G"]}        |
+| {_key('E')}                                 | {_icons["code"]}                                  | {key_maps["E"]}        |
 | {_key('L')}                                 | {_icons["laser"]}, {_icons["circle"]}             | {key_maps["L"]}        |
 | {_key('K')}                                 |                                                   | {key_maps["K"]}        |
 """ 
 
 more_instructions = f"""{get_logo('2em', 'IPySlides')}
 ::: note-tip
     In JupyterLab, right click on the slides and select `Create New View for Output` and follow next there to optimize display.
```

### Comparing `ipyslides-3.7.3/ipyslides/_base/js/interaction.js` & `ipyslides-3.7.4/ipyslides/_base/js/interaction.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -58,14 +58,15 @@
     's': 'SCAP', // Screenshot
     'f': 'TFS', // Toggle Fullscreen with F but with click from button
     'z': 'ZOOM', // Enable zooming items
     'g': 'TPAN', // Setting panel
     'k': 'KSC', // keyboard shortcuts
     'l': 'TLSR', // L toggle laser
     'v': 'TVP', // V for toggle viewport, only in voila and LinkedOutputView
+    'e': 'EDIT', // Edit source cell
 }
 
 
 function keyboardEvents(box, model) {
     function keyOnSlides(e) {
         e.preventDefault();
         let key = e.key; // True unicode key
```

### Comparing `ipyslides-3.7.3/ipyslides/_base/js/notes.js` & `ipyslides-3.7.4/ipyslides/_base/js/notes.js`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.3/ipyslides/_base/navigation.py` & `ipyslides-3.7.4/ipyslides/_base/navigation.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.3/ipyslides/_base/notes.py` & `ipyslides-3.7.4/ipyslides/_base/notes.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.3/ipyslides/_base/screenshot.py` & `ipyslides-3.7.4/ipyslides/_base/screenshot.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.3/ipyslides/_base/settings.py` & `ipyslides-3.7.4/ipyslides/_base/settings.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,38 +46,35 @@
         self.btn_laser = self.widgets.toggles.laser
         self.btn_draw = self.widgets.toggles.draw
         self.btn_menu = self.widgets.toggles.menu
         self.box = self.widgets.panelbox
 
         self.widgets.buttons.toc.on_click(self._toggle_tocbox)
         self.widgets.buttons.info.on_click(self._show_info)
-        self.widgets.buttons._inview.on_click(self.__block_post_run)
+        self.widgets.buttons._inview.on_click(self.__keep_new_output_only)
         self.widgets.htmls.toast.observe(self._toast_on_value_change, names=["value"])
         self.theme_dd.observe(self._update_theme, names=["value"])
         self.fontsize_slider.observe(self._update_theme, names=["value"])
         self.width_slider.observe(self._update_size, names=["value"])
         self.btn_window.observe(self._toggle_viewport, names=["value"])
         self.btn_fscreen.observe(self._toggle_fullscreen, names=["value"])
         self.btn_fscreen.observe(self._on_icon_change, names=["icon"])
         self.btn_zoom.observe(self._push_zoom, names=["value"])
         self.btn_laser.observe(self._toggle_laser, names=["value"])
         self.reflow_check.observe(self._update_theme, names=["value"])
         self.btn_draw.observe(self._toggle_overlay, names=["value"])
         self.btn_menu.observe(self._toggle_menu, names = ["value"])
-        self.widgets.checks.postrun.observe(self._set_show_always, names=["value"])
         self.widgets.checks.navgui.observe(self._toggle_nav_gui, names=["value"])
         self.widgets.checks.proxy.observe(self._toggle_proxy_buttons, names=["value"])
         self._update_theme()  # Trigger Theme and Javascript in it
         self.set_code_theme()  # Trigger CSS in it, must
         self.set_layout(center=True)  # Trigger this as well
         self._update_size(change=None)  # Trigger this as well
 
-    def __block_post_run(self, btn):
-        self.widgets.checks.postrun.value = False  # Uncheck it
-        self.widgets.checks.postrun.disabled = True  # Disable it
+    def __keep_new_output_only(self, btn):
         self.widgets.navbox.children = [
             w for w in self.widgets.navbox.children if w is not btn
         ]
         dh = getattr(self._slides._display_box, "_DH", None)  # Get display handler
         self._slides._display_box = self._slides.alert("Slides → Linked Output View").as_widget()  # Swap display box by info, still widget to be closable
         if dh is not None:
             dh.update(self._slides._display_box) 
@@ -132,46 +129,47 @@
                     if key not in param_keys:
                         raise ValueError(f"function '{k}' -> 'set_{k}' expects these parameters: {str(sig)}")
                     
             func(**v) if isinstance(v, dict) else func(
                 *v
             )  # Call function with arguments
 
-    def show_always(self, b: bool = True):
-        """If True (default), slides are shown after each cell execution where a slide constructor is present (other view will be closed).
-        Otherwise only when `slides.show()` is called or `slides` is the last line in a cell.
-        :::note
-            In JupyterLab, right click on the slides and select `Create New View for Output` and follow next step there to optimize display.
-        """
-        if not isinstance(b, bool):
-            raise TypeError(f"Expected bool, got {b!r}")
-        self._slides._post_run_enabled = (
-            True if b else False
-        )  # Do not rely on user if they really give bool or not
-
-    def _set_show_always(self, change):
-        if change["new"]:
-            self.show_always(True)
-            self._slides.notify("Post run cell enabled!")
-        else:
-            self.show_always(False)
-            self._slides.notify("Post run cell disabled!")
-
     def _toggle_nav_gui(self, change):
         if change["new"]:  # It's checked then hide
-            self.set_nav_gui(False)
+            self.show_nav_gui(True)
         else:
-            self.set_nav_gui(True)
+            self.show_nav_gui(False)
 
     def _toggle_proxy_buttons(self, change):
         if change["new"]:
             self.widgets.mainbox.remove_class("PresentMode")  # Show if checked
         else:
             self.widgets.mainbox.add_class("PresentMode")
 
+    
+    def set_toggles(self,
+        nav_gui = True,
+        reflow_content = False, 
+        notes = False, 
+        notifications = True, 
+        proxy_buttons = True,
+        auto_focus = True,
+        ):
+        for name, value in ({
+            'navgui': nav_gui,
+            'reflow': reflow_content,
+            'notes': notes,
+            'toast': notifications,
+            'proxy': proxy_buttons,
+            'scroll': scroll_buttons,
+            'focus': auto_focus,
+        }).items():
+            if (widget := getattr(self.widgets.checks,name, None)):
+                widget.value = value # if condition for future additions check
+
     def set_animation(self, main="slide_h", frame="appear"):
         "Set animation for slides and frames."
         if len(self._slides[:]) >= 1:
             self._slides[0]._set_overall_animation(main=main, frame=frame)
         else:
             raise RuntimeError("No slides yet to set animation.")
 
@@ -179,15 +177,15 @@
     def set_theme_colors(self, colors={}):
         """Set theme colors. Only take effect when using custom theme.
         colors must be a dictionary with exactly like this:
         ```python
         Slides.settings.set_theme_colors({colors})
         ```
         """
-        styles._validate_colors(self._custom_colors)  # Validate colors before using
+        styles._validate_colors(colors)  # Validate colors before using and setting
         self._custom_colors = colors
         self.theme_dd.value = "Custom"  # Trigger theme update
         self._update_theme({'owner':self.theme_dd}) # This chnage is important to update layout theme as well
 
     @_sub_doc(css_docstring=_css_docstring)
     def set_css(self, css_dict={}):
         """Set CSS for all slides. This loads on slides navigation, so you can include keyframes animations as well.
@@ -334,21 +332,23 @@
         if (not isinstance(width, int)) or (width not in range(101)):
             raise ValueError("width should be int in range [0,100]")
         if not isinstance(aspect, (int,float)):
             raise TypeError("aspect should be int/float of ratio width/height.")
         self._layout = {'cwidth':width, 'scroll': scroll, 'centered': center, 'aspect': aspect, 'ncol_refs': ncol_refs}
         self._update_size(change = None) # will reset theme and send RESCALE message
 
-    def set_nav_gui(self, visible = True):
+    def show_nav_gui(self, visible = True):
         """Show/Hide navigation GUI, keyboard or touch still work. Hover on left-bottom corner to acess settings."""
         self.widgets.controls.layout.visibility = "visible" if visible else "hidden"
+        self.widgets.checks.navgui.value = True if visible else False
         self.widgets.iw.msg_tojs = 'RESCALE' # sets padding etc
 
         if not visible:
             self._slides.notify("Navigation controls hidden. But keyboard and touch gestures are working!")
+        
 
     def _update_size(self, change):
         self.widgets.mainbox.layout.height = "{}vw".format(
             int(self.width_slider.value / self._layout["aspect"])
         )
         self.widgets.mainbox.layout.width = "{}vw".format(self.width_slider.value)
         self._update_theme(
```

### Comparing `ipyslides-3.7.3/ipyslides/_base/slide.py` & `ipyslides-3.7.4/ipyslides/_base/slide.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Slide Object, should not be instantiated directly"""
 
 import sys, time
-from contextlib import contextmanager
+from contextlib import contextmanager, suppress
 from ipywidgets import Layout, Button, HBox, VBox, Label
 
 from IPython.display import display
 from IPython.core.ultratb import FormattedTB
 
 
 from . import styles
@@ -349,44 +349,46 @@
     def __repr__(self):
         return f'Slide(number = {self._number}, label = {self.label!r}, index = {self._index})'
     
     @contextmanager
     def _capture(self):
         "Capture output to this slide."
         self._app._next_number = int(self._number) + 1
+        self._app._slides_per_cell.append(self) # will be flushed at end of cell by post_run_cell event
         self._notes = '' # Reset notes
         self._citations = {} # Reset citations
         self._section = None # Reset sec_key
         self._proxies = {} # Reset placeholders
         self._dproxies = {} # Reset dynamic placeholders
         self._columns = {} # Reset columns
         self._exportables = {} # Reset exportables
     
         if hasattr(self,'_on_load'):
             del self._on_load # Remove on_load function
         if hasattr(self,'_target_id'):
             del self._target_id # Remove target_id
+
+        with suppress(Exception): # register only in slides building, not other cells
+            self._app._register_postrun_cell()
         
         with self._app._set_running(self):
-            self._app._remove_post_run_callback() # Remove before capturing
             with capture_content() as captured:
                 yield captured
 
             if captured.stderr:
                 if 'warning' in captured.stderr.lower():
                     self._app._warnings.append(captured.stderr)
                 else:
                     raise RuntimeError(f'Error in building {self}: {captured.stderr}')
-                
-            # If no error, then add callback keeping the user preference
-            if self._app._post_run_enabled:
-                self._app.shell.events.register('post_run_cell', self._app._post_run_cell)
 
             self._contents = _expand_objs(captured.outputs, self) # Expand columns  
             self.set_dom_classes(remove = 'Out-Sync') # Now synced
+
+            if self._app.widgets.checks.focus.value: # User preference
+                self._app._box.focus()
         
         if self._app._warnings:
             print(*self._app._warnings, sep='\n\n')
             self._app._warnings = [] # Reset warnings
         
         
     def update_display(self, go_there = True):
```

### Comparing `ipyslides-3.7.3/ipyslides/_base/styles.py` & `ipyslides-3.7.4/ipyslides/_base/styles.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.3/ipyslides/_base/widgets.py` & `ipyslides-3.7.4/ipyslides/_base/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,15 @@
     Instantiate under `Widgets` class only.
     """
     prev    =  Button(icon='chevron-left',layout= Layout(width='auto',height='auto'),tooltip='Previous Slide [<, Shift + Space]').add_class('Arrows').add_class('Prev-Btn')
     next    =  Button(icon='chevron-right',layout= Layout(width='auto',height='auto'),tooltip='Next Slide [>, Space]').add_class('Arrows').add_class('Next-Btn')
     setting =  Button(icon= 'plus',layout= Layout(width='auto',height='auto'), tooltip='Open Settings [G]').add_class('Menu-Item').add_class('Settings-Btn')
     toc     =  Button(icon= 'plus',layout= Layout(width='auto',height='auto'), tooltip='Toggle Table of Contents').add_class('Menu-Item').add_class('Toc-Btn')
     refresh =  Button(icon= 'plus',layout= Layout(width='auto',height='auto'),tooltip='Refresh Dynamic Content').add_class('Menu-Item').add_class('Refresh-Btn')
+    source  =  Button(icon= 'plus',layout= Layout(width='auto',height='auto'), tooltip='Edit Source Cell [E]').add_class('Menu-Item').add_class('Source-Btn')
     home    =  Button(description= '⇤',layout= Layout(width='auto',height='auto'), tooltip='Go to Title Page').add_class('Menu-Item')
     end     =  Button(description= '⇥',layout= Layout(width='auto',height='auto'), tooltip='Go To End of Slides').add_class('Menu-Item')
     info    =  Button(description= 'ℹ️',layout= Layout(width='auto',height='auto'), tooltip='Information').add_class('Menu-Item')
     capture =  Button(icon='camera',layout= Layout(width='auto',height='auto'),
                 tooltip='Take Screen short in full screen. Order of multiple shots in a slide is preserved! [S]',
                 ).add_class('Screenshot-Btn').add_class('Menu-Item')
     pdf     = Button(description='Save PDF',layout= Layout(width='auto',height='auto'))
@@ -108,17 +109,17 @@
 class _Checks:
     """
     Instantiate under `Widgets` class only.
     """
     reflow  = ipw.Checkbox(indent = False, value=False,description='Reflow Content',layout=auto_layout)
     notes   = ipw.Checkbox(indent = False, value=False,description='Notes',layout=auto_layout) # do not observe, just keep track when slides work
     toast   = ipw.Checkbox(indent = False, value = True, description='Notifications',layout=auto_layout)
-    postrun = ipw.Checkbox(indent = False, value = True, description='Display Per Cell',layout=auto_layout)
+    focus   = ipw.Checkbox(indent = False, value = True, description='Auto Focus',layout=auto_layout)
     proxy   = ipw.Checkbox(indent = False, value = True, description='Proxy Buttons',layout=auto_layout)
-    navgui  = ipw.Checkbox(indent = False, value = False, description='Hide Nav. GUI',layout=auto_layout)
+    navgui  = ipw.Checkbox(indent = False, value = True, description='Show Nav. GUI',layout=auto_layout)
 
 @dataclass(frozen=True)
 class _Sliders:
     """
     Instantiate under `Widgets` class only.
     """
     progress = ipw.SelectionSlider(options=[('0',0)], value=0, continuous_update=False,readout=True)
@@ -174,15 +175,16 @@
         ]).add_class('Controls') 
 
         
         self.footerbox = HBox([
             HBox([
                 self.toggles.menu,
                 self.buttons.capture,
-                self.buttons.toc,
+                self.buttons.toc, 
+                self.buttons.source,  
             ]).add_class('Menu-Box'),
             HBox([self.htmls.footer]), # should be in Box to avoid overflow
         ],layout=Layout(height='28px')).add_class('NavBox')
         
         self.navbox = VBox([
             self.buttons._inview,
             self.footerbox,
@@ -193,23 +195,22 @@
         self.panelbox = VBox([
             self.htmls.glass,
             HBox(_many_btns).add_class('TopBar').add_class('Inside'),
             VBox([
                 self.sliders.fontsize,
                 self.sliders.width,
                 self.ddowns.theme,
-                HTML('<hr/>'),
                 Box([GridBox([
-                    self.buttons.export, self.buttons.info, HTML(), # one empty button place
+                    self.buttons.export, self.buttons.info, HTML(), # empty space
                     self.checks.notes,self.checks.toast,self.checks.reflow,
-                    self.checks.proxy,self.checks.navgui,self.checks.postrun,
+                    self.checks.proxy,self.checks.navgui,self.checks.focus,
                     self.buttons.cap_all,self.buttons.pdf,self.buttons.png,
                 ],layout=Layout(width='auto',overflow_x='scroll',
                                 grid_template_columns='1fr 1fr 1fr',grid_gap='4px',
-                                padding='4px',margin='auto')
+                                padding='4px',margin='8px auto')
                 )],layout=Layout(min_height='120px')),# This ensures no collapse and scrollable Grid
                 self.ddowns.clear,
                 HTML('<span style="font-size:14px;">Set screenshot bounding box (if slides not fullscreen)</span>'),
                 self.inputs.bbox,
                 self._tmp_out,
                 self.notes, # Just to be there for acting on a popup window
             ],layout=Layout(width='auto',height='auto',overflow_y='scroll',padding='12px',margin='0')),
@@ -248,15 +249,15 @@
             self.htmls.zoom,
             HBox([ #Slide_box must be in a box to have animations work
                 self.tocbox, # Should be on left of slides
                 self.slidebox , 
             ],layout= Layout(width='100%',max_width='100%',height='100%',overflow='hidden')), #should be hidden for animation purpose
             self.controls, # Importnat for unique display
             self.drawer, 
-            self.navbox, 
+            self.navbox,
             self._snum,
             self._progbar # progressbar should come last
             ],layout= Layout(width=f'{self.sliders.width.value}vw', height=f'{int(self.sliders.width.value*9/16)}vw',margin='auto') # 9/16 is default, will change by setting
         ).add_class('SlidesWrapper')  #Very Important to add this class
 
         for child in self.mainbox.children:
             if isinstance(child, (HTML, HtmlWidget)):
```

### Comparing `ipyslides-3.7.3/ipyslides/_demo.py` & `ipyslides-3.7.4/ipyslides/_demo.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.3/ipyslides/core.py` & `ipyslides-3.7.4/ipyslides/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,16 +87,14 @@
         self.code = Code  # Code source
         self.icon = _Icon  # Icon is useful to add many places
         self.write = write
         self.parse = parse  # Parse extended markdown
         self.fmt = fmt # So important for flexibility
         self.serializer = serializer  # Serialize IPython objects to HTML
 
-        self._remove_post_run_callback()  # Remove post_run_cell callback before this and at end
-        self._post_run_enabled = True  # Enable post_run_cell event than can be hold by skip_post_run_cell context manager
         with suppress(Exception):  # Avoid error when using setuptools to install
             self.shell.register_magic_function(
                 self._slide, magic_kind="cell", magic_name="slide"
             )
             self.shell.register_magic_function(
                 self.__title, magic_kind="cell", magic_name="title"
             )
@@ -116,31 +114,32 @@
         self._running_slide = (
             None  # For Notes, citations etc in markdown, controlled in Slide class
         )
         self._next_number = (
             0  # Auto numbering of slides should be only in python scripts
         )
         self._citations = {}  # Initialize citations dictionary
+        self._slides_per_cell = [] # all buidling slides in a cell will be added while capture, and removed with post run cell
 
         with self.set_dir(self._assets_dir):  # Set assets directory
             self._set_citations_from_file(
                 "citations.json"
             )  # Load citations from file if exists
 
         self.progress_slider = self.widgets.sliders.progress
         self.progress_slider.label = "0"  # Set inital value, otherwise it does not capture screenshot if title only
         self.progress_slider.observe(self._update_content, names=["index"])
         self.widgets.buttons.refresh.on_click(self._update_dynamic_content)
+        self.widgets.buttons.source.on_click(self._jump_to_source_cell)
 
         # All Box of Slides
         self._box = self.widgets.mainbox.add_class(self.uid)
         self._setup()  # Load some initial data and fixing
         self._display_box = None  # Initialize
-        self._remove_post_run_callback()  # Remove post_run_cell callback at end of init, otherwise it appears during import
-
+        
     @contextmanager
     def _set_running(self, slide):
         "Context manager to set running slide and turns back to previous."
         if slide and not isinstance(
             slide, Slide
         ):  # None is acceptable to hold running slide in other function
             raise TypeError(f"slide must be None or Slide, got {type(slide)}")
@@ -154,41 +153,49 @@
 
     @contextmanager
     def _hold_running(self):
         "Context manager to pause running slide and restore it after"
         with self._set_running(None):
             yield
 
-    @contextmanager
-    def skip_post_run_cell(self, force = False):
-        """Context manager to skip post_run_cell event."""
-        self._remove_post_run_callback()
-        old = self._post_run_enabled
-        self._post_run_enabled = False
-        try:
-            yield
-        finally:
-            self._post_run_enabled = old  # Restore user prefrence, will be registered in slides start
-
-    def _remove_post_run_callback(self):
-        with suppress(Exception):
-            self.shell.events.unregister("post_run_cell", self._post_run_cell)
-
     def run_cell(self, cell, **kwargs):
-        """Run cell and return result. This is used to run cell without post_run_cell event."""
-        with self.skip_post_run_cell():
-            return self.shell.run_cell(cell, **kwargs)
-
+        """Run cell and return result. Use this instead of IPython's run_cell for extra controls."""
+        self._unregister_postrun_cell() # important to avoid putting contnet on slides
+        output = self.shell.run_cell(cell, **kwargs)
+        if self.running: # there was post_run_cell under building slides
+            self._register_postrun_cell() # should be back
+        return output
+    
     def _post_run_cell(self, result):
+        self._unregister_postrun_cell() # it will be initialized from next building slides
         if result.error_before_exec or result.error_in_exec:
             return  # Do not display if there is an error
-        if self._post_run_enabled:
-            return (
-                self._ipython_display_()
-            )  # Display after cell is executed only when enabled, don call show here, make issues
+
+        scroll_btn = ipw.Button(description= 'Scroll to Slides', icon= 'scroll').add_class('Scroll-Btn')
+        
+        for slide in self._slides_per_cell:
+            slide._scroll_btn = scroll_btn
+        
+        self._slides_per_cell.clear() # empty it
+        scroll_btn.on_click(lambda btn: self._box.focus()) # only need to go there, no slide switching 
+        display(scroll_btn)
+    
+    def _unregister_postrun_cell(self):
+        with suppress(Exception): 
+            self.shell.events.unregister("post_run_cell", self._post_run_cell)
+    
+    def _register_postrun_cell(self):
+        with suppress(Exception): 
+            self.shell.events.register("post_run_cell", self._post_run_cell)
+        
+    def _jump_to_source_cell(self, btn):
+        if hasattr(self.current, '_scroll_btn'):
+            self.current._scroll_btn.focus()
+        else:
+            self.notify('No source cell found!')
 
     def _setup(self):
         # Only in Jupyter Notebook
         if self.shell and self.shell.__class__.__name__ != "TerminalInteractiveShell":
             if self._max_index == 0:  # prevent overwrite
                 self._add_clean_title()
 
@@ -292,17 +299,15 @@
         "Verify if slide is being built, otherwise raise error."
         if self.running is None:
             raise RuntimeError(
                 error_msg or "This operation is only allowed under slide constructor."
             )
 
     def _add_clean_title(self):
-        with suppress(
-            BaseException
-        ), self.skip_post_run_cell():  # Otherwise it will trigger cell events during __init__
+        with suppress(BaseException):  # need to avoid any errors
             with _build_slide(self, "0") as s:
                 self.parse(
                     f"""
                     # Title Page 
                     ::: align-center
                         color[teal]`Author: Abdul Saboor`
 
@@ -313,14 +318,15 @@
                     returns = False,
                 )
                 self.details(
                     self.parse(key_combs, returns = True),
                     "Keyboard Shortcuts",
                 ).display()
 
+        self._unregister_postrun_cell() # no need in initialization functions 
         self.refresh()  # cleans up initialization setup and tocs/other things
 
     def clear(self):
         "Clear all slides. This will also clear resources including citations, sections."
         self._slides_dict = {}  # Clear slides
         _ = [
             self.__dict__.pop(s, None) for s in getattr(self, "_links_dict", {})
@@ -526,15 +532,15 @@
         return self._ipython_display_()
 
     def _ipython_display_(self):
         "Auto display when self is on last line of a cell"
         if not self.is_jupyter_session():
             raise Exception("Python/IPython REPL cannot show slides. Use IPython notebook instead.")
 
-        self._remove_post_run_callback()  # Avoid duplicate display
+        self._unregister_postrun_cell() # no need to scroll button where showing itself
         self._update_toc()  # Update toc before displaying app to include all sections
         self._update_dynamic_content()  # Update dynamic content before displaying app
         self.close_view()  # Close previous views
         self.__reset_navbox()  # Important to add inview button for each new view
         self._display_box = ipw.VBox(children=[self._box]).add_class(
             "DisplayBox"
         )  # Initialize display box again
@@ -547,15 +553,14 @@
         "Close slides/cell view, but keep slides in memory than can be shown again."
         if hasattr(self, "_display_box") and self._display_box is not None:
             self._display_box.close()  # Clear display that removes CSS things there
             self.__reset_navbox()  # Important to add inview button for next view
 
     def __reset_navbox(self):
         "Reset navbox to add inview button for Jupyter Lab"
-        self.widgets.checks.postrun.disabled = False  # Enable it
         others = [
             w
             for w in self.widgets.navbox.children
             if w is not self.widgets.buttons._inview
         ]
         self.widgets.navbox.children = [self.widgets.buttons._inview, *others]
 
@@ -1108,15 +1113,15 @@
     def instance(cls):
         "Access current instnace without changing the settings."
         return _private_instance
 
     def __new__(
         cls,
         extensions=[],
-        show_always=True,
+        auto_focus = True, 
         layout = dict(center=True, scroll=True, width=100, aspect=16/9, ncol_refs = 2),
         footer = dict(
             text='IPySlides | <a style="color:blue;" href="https://github.com/massgh/ipyslides">github-link</a>',
             numbering = True, 
             date="today",
         ),
         logo = dict(src=get_logo(), width=60),
@@ -1125,22 +1130,22 @@
         animation = dict(main="slide_h", frame = "appear"),
         **kwargs
     ):
         "Returns Same instance each time after applying given settings. Encapsulation."
         instance = cls.instance()
         instance.__doc__ = cls.__doc__  # copy docstring
         instance.extender.extend(extensions)
-        instance.settings.show_always(show_always)
         instance.settings.set(
-            layout = layout, # Defaults are kept by set_layout
+            layout = layout,
             footer = footer,
             logo = logo,
             font_family = font_family,
             code_theme = code_theme,
             **kwargs
         )
+        instance.widgets.checks.focus.value = auto_focus # after other settings
 
         with suppress(BaseException):  # Avoid error if no slides exist
             instance.settings.set_animation(**animation)
         return instance
 
     # No need to define __init__, __new__ is enough to show signature and docs
```

### Comparing `ipyslides-3.7.3/ipyslides/formatters.py` & `ipyslides-3.7.4/ipyslides/formatters.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.3/ipyslides/source.py` & `ipyslides-3.7.4/ipyslides/source.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.3/ipyslides/utils.py` & `ipyslides-3.7.4/ipyslides/utils.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.3/ipyslides/writer.py` & `ipyslides-3.7.4/ipyslides/writer.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.3/ipyslides/xmd.py` & `ipyslides-3.7.4/ipyslides/xmd.py`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.3/ipyslides.egg-info/PKG-INFO` & `ipyslides-3.7.4/ipyslides.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyslides
-Version: 3.7.3
+Version: 3.7.4
 Summary: Live rich content slides in jupyter notebook
 Home-page: https://github.com/massgh/ipyslides
 Author: Abdul Saboor
 Author-email: mass_qau@outlook.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/massgh/ipyslides/issues
 Keywords: Jupyter,Widgets,IPython
```

### Comparing `ipyslides-3.7.3/ipyslides.egg-info/SOURCES.txt` & `ipyslides-3.7.4/ipyslides.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ipyslides-3.7.3/setup.py` & `ipyslides-3.7.4/setup.py`

 * *Files identical despite different names*

