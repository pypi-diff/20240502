# Comparing `tmp/gcp-sphinx-docfx-yaml-3.1.0.tar.gz` & `tmp/gcp-sphinx-docfx-yaml-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gcp-sphinx-docfx-yaml-3.1.0.tar", last modified: Wed Apr  3 17:57:11 2024, max compression
+gzip compressed data, was "gcp-sphinx-docfx-yaml-3.2.0.tar", last modified: Thu May  2 07:11:59 2024, max compression
```

## Comparing `gcp-sphinx-docfx-yaml-3.1.0.tar` & `gcp-sphinx-docfx-yaml-3.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 17:57:11.227464 gcp-sphinx-docfx-yaml-3.1.0/
--rw-rw-r--   0 root         (0)     1003    11358 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/LICENSE
--rw-r--r--   0 root         (0)     1003      796 2024-04-03 17:57:11.227464 gcp-sphinx-docfx-yaml-3.1.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     2625 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 17:57:11.223463 gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/
--rw-rw-r--   0 root         (0)     1003      576 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/__init__.py
--rw-rw-r--   0 root         (0)     1003     1262 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/directives.py
--rw-rw-r--   0 root         (0)     1003    84402 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/extension.py
--rw-rw-r--   0 root         (0)     1003     5154 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/extract_nodes.py
--rw-rw-r--   0 root         (0)     1003    16722 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/markdown_utils.py
--rw-rw-r--   0 root         (0)     1003    20734 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/monkeypatch.py
--rw-rw-r--   0 root         (0)     1003      988 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/nodes.py
--rw-rw-r--   0 root         (0)     1003      727 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/settings.py
--rw-rw-r--   0 root         (0)     1003     1731 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/utils.py
--rw-rw-r--   0 root         (0)     1003    33366 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/writer.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 17:57:11.223463 gcp-sphinx-docfx-yaml-3.1.0/gcp_sphinx_docfx_yaml.egg-info/
--rw-r--r--   0 root         (0)     1003      796 2024-04-03 17:57:11.000000 gcp-sphinx-docfx-yaml-3.1.0/gcp_sphinx_docfx_yaml.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003      640 2024-04-03 17:57:11.000000 gcp-sphinx-docfx-yaml-3.1.0/gcp_sphinx_docfx_yaml.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-03 17:57:11.000000 gcp-sphinx-docfx-yaml-3.1.0/gcp_sphinx_docfx_yaml.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-04-03 17:57:11.000000 gcp-sphinx-docfx-yaml-3.1.0/gcp_sphinx_docfx_yaml.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      289 2024-04-03 17:57:11.000000 gcp-sphinx-docfx-yaml-3.1.0/gcp_sphinx_docfx_yaml.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003       11 2024-04-03 17:57:11.000000 gcp-sphinx-docfx-yaml-3.1.0/gcp_sphinx_docfx_yaml.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-04-03 17:57:11.227464 gcp-sphinx-docfx-yaml-3.1.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     1756 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-04-03 17:57:11.227464 gcp-sphinx-docfx-yaml-3.1.0/tests/
--rw-rw-r--   0 root         (0)     1003    15861 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/tests/test_helpers.py
--rw-rw-r--   0 root         (0)     1003     1588 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/tests/test_inspect.py
--rw-rw-r--   0 root         (0)     1003    11616 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/tests/test_markdown.py
--rw-rw-r--   0 root         (0)     1003    32326 2024-04-03 17:54:58.000000 gcp-sphinx-docfx-yaml-3.1.0/tests/test_unit.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-02 07:11:59.125235 gcp-sphinx-docfx-yaml-3.2.0/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/LICENSE
+-rw-r--r--   0 root         (0)     1003      796 2024-05-02 07:11:59.125235 gcp-sphinx-docfx-yaml-3.2.0/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     2625 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-02 07:11:59.121235 gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/
+-rw-rw-r--   0 root         (0)     1003      576 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1262 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/directives.py
+-rw-rw-r--   0 root         (0)     1003    85361 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/extension.py
+-rw-rw-r--   0 root         (0)     1003     5154 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/extract_nodes.py
+-rw-rw-r--   0 root         (0)     1003    16722 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/markdown_utils.py
+-rw-rw-r--   0 root         (0)     1003    20734 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/monkeypatch.py
+-rw-rw-r--   0 root         (0)     1003      988 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/nodes.py
+-rw-rw-r--   0 root         (0)     1003      727 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/settings.py
+-rw-rw-r--   0 root         (0)     1003     1731 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/utils.py
+-rw-rw-r--   0 root         (0)     1003    33366 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/writer.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-02 07:11:59.125235 gcp-sphinx-docfx-yaml-3.2.0/gcp_sphinx_docfx_yaml.egg-info/
+-rw-r--r--   0 root         (0)     1003      796 2024-05-02 07:11:59.000000 gcp-sphinx-docfx-yaml-3.2.0/gcp_sphinx_docfx_yaml.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003      640 2024-05-02 07:11:59.000000 gcp-sphinx-docfx-yaml-3.2.0/gcp_sphinx_docfx_yaml.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-02 07:11:59.000000 gcp-sphinx-docfx-yaml-3.2.0/gcp_sphinx_docfx_yaml.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-05-02 07:11:59.000000 gcp-sphinx-docfx-yaml-3.2.0/gcp_sphinx_docfx_yaml.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      289 2024-05-02 07:11:59.000000 gcp-sphinx-docfx-yaml-3.2.0/gcp_sphinx_docfx_yaml.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003       11 2024-05-02 07:11:59.000000 gcp-sphinx-docfx-yaml-3.2.0/gcp_sphinx_docfx_yaml.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-05-02 07:11:59.125235 gcp-sphinx-docfx-yaml-3.2.0/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     1756 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-05-02 07:11:59.125235 gcp-sphinx-docfx-yaml-3.2.0/tests/
+-rw-rw-r--   0 root         (0)     1003    15861 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/tests/test_helpers.py
+-rw-rw-r--   0 root         (0)     1003     1588 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/tests/test_inspect.py
+-rw-rw-r--   0 root         (0)     1003    11616 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/tests/test_markdown.py
+-rw-rw-r--   0 root         (0)     1003    32326 2024-05-02 07:09:47.000000 gcp-sphinx-docfx-yaml-3.2.0/tests/test_unit.py
```

### Comparing `gcp-sphinx-docfx-yaml-3.1.0/LICENSE` & `gcp-sphinx-docfx-yaml-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.1.0/PKG-INFO` & `gcp-sphinx-docfx-yaml-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp-sphinx-docfx-yaml
-Version: 3.1.0
+Version: 3.2.0
 Summary: Sphinx Python Domain to DocFX YAML Generator
 Home-page: https://github.com/googleapis/sphinx-docfx-yaml
 Author: Google LLC
 Author-email: dandhlee@google.com
 License: Apache 2.0
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `gcp-sphinx-docfx-yaml-3.1.0/README.rst` & `gcp-sphinx-docfx-yaml-3.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/__init__.py` & `gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/__init__.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/directives.py` & `gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/directives.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/extension.py` & `gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -396,14 +396,15 @@
     return "\n".join(parts)
 
 
 def _parse_docstring_summary(summary):
     summary_parts = []
     attributes = []
     attribute_type_token = ":type:"
+    enum_type_token = "Values:"
     keyword = name = description = var_type = ""
 
     notice_open_tag = '<aside class="{notice_tag}">\n<b>{notice_name}:</b>'
     notice_close_tag = '</aside>'
 
     # We need to separate in chunks, which is defined by 3 newline breaks.
     # Otherwise when parsing for code and blocks of stuff, we will not be able
@@ -482,15 +483,37 @@
                 summary_parts.append(notice_close_tag)
                 keyword = ""
             notice_body.append(part)
             continue
 
         # Parse keywords if found.
         # lstrip is added to parse code blocks that are not formatted well.
-        if part.lstrip('\n').startswith('..'):
+        if (potential_keyword := part.lstrip('\n')) and (
+            potential_keyword.startswith('..') or
+            potential_keyword.startswith(enum_type_token)
+        ):
+            if enum_type_token in potential_keyword:
+                # Handle the enum section starting with `Values:`
+                parts = [split_part for split_part in part.split("\n") if split_part][1:]
+                if not parts:
+                    continue
+                tab_space = len(parts[0]) - len(parts[0].lstrip(" "))
+                if tab_space == 0:
+                    raise ValueError("Content in the block should be indented."\
+                                     f"Please check the docstring: \n{summary}")
+                parts = "\n".join(
+                    [indent_code_left(part, tab_space) for part in parts]
+                )
+                summary_parts.append(
+                    "Enum values:\n\n```\n"
+                    f"{parts}"
+                    "\n```\n"
+                )
+                continue
+
             try:
                 keyword = extract_keyword(part.lstrip('\n'))
             except ValueError:
                 raise ValueError(f"Please check the docstring: \n{summary}")
             # Works for both code-block and code
             if keyword and keyword in [CODE, CODEBLOCK]:
                 # Retrieve the language found in the format of
@@ -562,30 +585,30 @@
     # Initialize known types needing further processing.
     var_types = {
         ':rtype:': 'returns',
         ':returns:': 'returns',
         ':type': 'variables',
         ':param': 'variables',
         ':raises': 'exceptions',
-        ':raises:': 'exceptions'
+        ':raises:': 'exceptions',
     }
-    
+
     initial_index = -1
     front_tag = '<xref'
     end_tag = '/xref>'
     end_len = len(end_tag)
-        
+
     # Prevent GoogleDocstring crashing on custom types and parse all xrefs to normal
     if front_tag in parsed_text:
         type_pairs = []
         # Constant length for end of xref tag
         initial_index = max(0, parsed_text.find(front_tag))
 
         summary_part = parsed_text[initial_index:]
-       
+
         # Remove all occurrences of "<xref uid="uid">text</xref>"
         while front_tag in summary_part:
 
             # Expecting format of "<xref uid="uid">text</xref>"
             if front_tag in summary_part:
                 # Retrieve the index for starting position of xref tag
                 initial_index += summary_part.find(front_tag)
@@ -607,20 +630,20 @@
             type_pairs.append([original_type, safe_type])
             summary_part = parsed_text[initial_index:]
 
         # Replace all the found occurrences
         for pairs in type_pairs:
             original_type, safe_type = pairs[0], pairs[1]
             parsed_text = parsed_text.replace(original_type, safe_type)
-        
+
     # Clean the string by cleaning newlines and backlashes, then split by white space.
     config = Config(napoleon_use_param=True, napoleon_use_rtype=True)
     # Convert Google style to reStructuredText
     parsed_text = str(GoogleDocstring(parsed_text, config))
-    
+
     # Trim the top summary but maintain its formatting.
     indexes = []
     for types in var_types:
         # Ensure that we look for exactly the string we want.
         # Adding the extra space for non-colon ending types
         # helps determine if we simply ran into desired occurrence
         # or if we ran into a similar looking syntax but shouldn't
@@ -662,15 +685,15 @@
     r_type, r_descr = '', ''
 
     # Using counter iteration to easily extract names rather than
     # coming up with more complicated stopping logic for each tags.
     while index <= len(parsed_text):
         word = parsed_text[index] if index < len(parsed_text) else ""
         # Check if we encountered specific words.
-        if word in var_types or index == len(parsed_text):               
+        if word in var_types or index == len(parsed_text):
             # Finish processing previous section.
             if cur_type:
                 if cur_type == ':type':
                     summary_info[var_types[cur_type]][arg_name]['var_type'] = " ".join(words)
                 elif cur_type == ':param':
                     summary_info[var_types[cur_type]][arg_name]['description'] = " ".join(words)
                 elif ":raises" in cur_type:
@@ -694,19 +717,19 @@
 
                 # If after we processed the top summary and get in this state,
                 # likely we encountered a type that's not covered above or the docstring
                 # was formatted badly. This will likely break docfx job later on, should not
                 # process further.
                 if word not in var_types:
                     raise ValueError(f"Encountered wrong formatting, please check docstring for {name}")
-   
+
             # Reached end of string, break after finishing processing
             if index == len(parsed_text):
                 break
-    
+
             # Start processing for new section
             cur_type = word
             if cur_type in [':type', ':param', ':raises', ':raises:']:
                 index += 1
                 # Exception that's not xref should be treated same as other names
                 if ':raises' not in cur_type or 'xref' not in parsed_text[index]:
                     arg_name = parsed_text[index][:-1]
```

### Comparing `gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/extract_nodes.py` & `gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/extract_nodes.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/markdown_utils.py` & `gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/markdown_utils.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/monkeypatch.py` & `gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/monkeypatch.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/nodes.py` & `gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/nodes.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/settings.py` & `gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/settings.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/utils.py` & `gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/utils.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.1.0/docfx_yaml/writer.py` & `gcp-sphinx-docfx-yaml-3.2.0/docfx_yaml/writer.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.1.0/gcp_sphinx_docfx_yaml.egg-info/PKG-INFO` & `gcp-sphinx-docfx-yaml-3.2.0/gcp_sphinx_docfx_yaml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gcp-sphinx-docfx-yaml
-Version: 3.1.0
+Version: 3.2.0
 Summary: Sphinx Python Domain to DocFX YAML Generator
 Home-page: https://github.com/googleapis/sphinx-docfx-yaml
 Author: Google LLC
 Author-email: dandhlee@google.com
 License: Apache 2.0
 Requires-Python: >=3.10
 License-File: LICENSE
```

### Comparing `gcp-sphinx-docfx-yaml-3.1.0/gcp_sphinx_docfx_yaml.egg-info/SOURCES.txt` & `gcp-sphinx-docfx-yaml-3.2.0/gcp_sphinx_docfx_yaml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.1.0/setup.py` & `gcp-sphinx-docfx-yaml-3.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # limitations under the License.
 
 import codecs
 import setuptools
 
 name = 'gcp-sphinx-docfx-yaml'
 description = 'Sphinx Python Domain to DocFX YAML Generator'
-version = '3.1.0'
+version = '3.2.0'
 dependencies = [
     'black',
     'gcp-docuploader',
     'PyYAML',
     'recommonmark',
     'sphinxcontrib-applehelp==1.0.4',
     'sphinxcontrib-devhelp==1.0.2',
```

### Comparing `gcp-sphinx-docfx-yaml-3.1.0/tests/test_helpers.py` & `gcp-sphinx-docfx-yaml-3.2.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.1.0/tests/test_inspect.py` & `gcp-sphinx-docfx-yaml-3.2.0/tests/test_inspect.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.1.0/tests/test_markdown.py` & `gcp-sphinx-docfx-yaml-3.2.0/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `gcp-sphinx-docfx-yaml-3.1.0/tests/test_unit.py` & `gcp-sphinx-docfx-yaml-3.2.0/tests/test_unit.py`

 * *Files identical despite different names*

