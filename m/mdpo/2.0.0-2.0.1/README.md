# Comparing `tmp/mdpo-2.0.0.tar.gz` & `tmp/mdpo-2.0.1.tar.gz`

## Comparing `mdpo-2.0.0.tar` & `mdpo-2.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 mdpo-2.0.0/src/mdpo/__init__.py
--rw-r--r--   0        0        0    12227 2020-02-02 00:00:00.000000 mdpo-2.0.0/src/mdpo/cli.py
--rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 mdpo-2.0.0/src/mdpo/command.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 mdpo-2.0.0/src/mdpo/compat.py
--rw-r--r--   0        0        0     7357 2020-02-02 00:00:00.000000 mdpo-2.0.0/src/mdpo/event.py
--rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 mdpo-2.0.0/src/mdpo/io.py
--rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 mdpo-2.0.0/src/mdpo/md.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 mdpo-2.0.0/src/mdpo/md4c.py
--rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 mdpo-2.0.0/src/mdpo/po.py
--rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 mdpo-2.0.0/src/mdpo/polib.py
--rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 mdpo-2.0.0/src/mdpo/text.py
--rw-r--r--   0        0        0    46672 2020-02-02 00:00:00.000000 mdpo-2.0.0/src/mdpo/md2po/__init__.py
--rwxr-xr-x   0        0        0     8431 2020-02-02 00:00:00.000000 mdpo-2.0.0/src/mdpo/md2po/__main__.py
--rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 mdpo-2.0.0/src/mdpo/md2po2md/__init__.py
--rwxr-xr-x   0        0        0     5100 2020-02-02 00:00:00.000000 mdpo-2.0.0/src/mdpo/md2po2md/__main__.py
--rw-r--r--   0        0        0    18140 2020-02-02 00:00:00.000000 mdpo-2.0.0/src/mdpo/mdpo2html/__init__.py
--rwxr-xr-x   0        0        0     3542 2020-02-02 00:00:00.000000 mdpo-2.0.0/src/mdpo/mdpo2html/__main__.py
--rw-r--r--   0        0        0    39866 2020-02-02 00:00:00.000000 mdpo-2.0.0/src/mdpo/po2md/__init__.py
--rwxr-xr-x   0        0        0     4227 2020-02-02 00:00:00.000000 mdpo-2.0.0/src/mdpo/po2md/__main__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 mdpo-2.0.0/.gitignore
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 mdpo-2.0.0/LICENSE
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 mdpo-2.0.0/README.md
--rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 mdpo-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     3300 2020-02-02 00:00:00.000000 mdpo-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 mdpo-2.0.1/src/mdpo/__init__.py
+-rw-r--r--   0        0        0    12227 2020-02-02 00:00:00.000000 mdpo-2.0.1/src/mdpo/cli.py
+-rw-r--r--   0        0        0     2961 2020-02-02 00:00:00.000000 mdpo-2.0.1/src/mdpo/command.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 mdpo-2.0.1/src/mdpo/compat.py
+-rw-r--r--   0        0        0     7357 2020-02-02 00:00:00.000000 mdpo-2.0.1/src/mdpo/event.py
+-rw-r--r--   0        0        0     3958 2020-02-02 00:00:00.000000 mdpo-2.0.1/src/mdpo/io.py
+-rw-r--r--   0        0        0     5027 2020-02-02 00:00:00.000000 mdpo-2.0.1/src/mdpo/md.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 mdpo-2.0.1/src/mdpo/md4c.py
+-rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 mdpo-2.0.1/src/mdpo/po.py
+-rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 mdpo-2.0.1/src/mdpo/polib.py
+-rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 mdpo-2.0.1/src/mdpo/text.py
+-rw-r--r--   0        0        0    46771 2020-02-02 00:00:00.000000 mdpo-2.0.1/src/mdpo/md2po/__init__.py
+-rwxr-xr-x   0        0        0     8431 2020-02-02 00:00:00.000000 mdpo-2.0.1/src/mdpo/md2po/__main__.py
+-rw-r--r--   0        0        0     6913 2020-02-02 00:00:00.000000 mdpo-2.0.1/src/mdpo/md2po2md/__init__.py
+-rwxr-xr-x   0        0        0     5100 2020-02-02 00:00:00.000000 mdpo-2.0.1/src/mdpo/md2po2md/__main__.py
+-rw-r--r--   0        0        0    18140 2020-02-02 00:00:00.000000 mdpo-2.0.1/src/mdpo/mdpo2html/__init__.py
+-rwxr-xr-x   0        0        0     3542 2020-02-02 00:00:00.000000 mdpo-2.0.1/src/mdpo/mdpo2html/__main__.py
+-rw-r--r--   0        0        0    39752 2020-02-02 00:00:00.000000 mdpo-2.0.1/src/mdpo/po2md/__init__.py
+-rwxr-xr-x   0        0        0     4227 2020-02-02 00:00:00.000000 mdpo-2.0.1/src/mdpo/po2md/__main__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 mdpo-2.0.1/.gitignore
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 mdpo-2.0.1/LICENSE
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 mdpo-2.0.1/README.md
+-rw-r--r--   0        0        0     4994 2020-02-02 00:00:00.000000 mdpo-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 mdpo-2.0.1/PKG-INFO
```

### Comparing `mdpo-2.0.0/src/mdpo/__init__.py` & `mdpo-2.0.1/src/mdpo/__init__.py`

 * *Files identical despite different names*

### Comparing `mdpo-2.0.0/src/mdpo/cli.py` & `mdpo-2.0.1/src/mdpo/cli.py`

 * *Files identical despite different names*

### Comparing `mdpo-2.0.0/src/mdpo/command.py` & `mdpo-2.0.1/src/mdpo/command.py`

 * *Files identical despite different names*

### Comparing `mdpo-2.0.0/src/mdpo/event.py` & `mdpo-2.0.1/src/mdpo/event.py`

 * *Files identical despite different names*

### Comparing `mdpo-2.0.0/src/mdpo/io.py` & `mdpo-2.0.1/src/mdpo/io.py`

 * *Files identical despite different names*

### Comparing `mdpo-2.0.0/src/mdpo/md.py` & `mdpo-2.0.1/src/mdpo/md.py`

 * *Files identical despite different names*

### Comparing `mdpo-2.0.0/src/mdpo/md4c.py` & `mdpo-2.0.1/src/mdpo/md4c.py`

 * *Files identical despite different names*

### Comparing `mdpo-2.0.0/src/mdpo/po.py` & `mdpo-2.0.1/src/mdpo/po.py`

 * *Files identical despite different names*

### Comparing `mdpo-2.0.0/src/mdpo/polib.py` & `mdpo-2.0.1/src/mdpo/polib.py`

 * *Files identical despite different names*

### Comparing `mdpo-2.0.0/src/mdpo/text.py` & `mdpo-2.0.1/src/mdpo/text.py`

 * *Files identical despite different names*

### Comparing `mdpo-2.0.0/src/mdpo/md2po/__init__.py` & `mdpo-2.0.1/src/mdpo/md2po/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -866,18 +866,21 @@
                     if self._inside_codespan:
                         # fix backticks for codespan start and end to escape
                         # internal backticks
                         self._codespan_backticks = min_not_max_chars_in_a_row(
                             self.code_start_string,
                             text,
                         ) - 1
-                        self.current_msgid = '{}{}{}'.format(
-                            self.current_msgid[:self._codespan_start_index],
-                            self._codespan_backticks * self.code_start_string,
-                            self.current_msgid[self._codespan_start_index:],
+                        backticks = (
+                            self._codespan_backticks * self.code_start_string
+                        )
+                        self.current_msgid = (
+                            f'{self.current_msgid[:self._codespan_start_index]}'
+                            f'{backticks}'
+                            f'{self.current_msgid[self._codespan_start_index:]}'
                         )
                         if self._inside_aspan:
                             self._current_aspan_text += text
                             return
                     elif self._inside_aspan:
                         self._current_aspan_text += text
                         return
```

### Comparing `mdpo-2.0.0/src/mdpo/md2po/__main__.py` & `mdpo-2.0.1/src/mdpo/md2po/__main__.py`

 * *Files identical despite different names*

### Comparing `mdpo-2.0.0/src/mdpo/md2po2md/__init__.py` & `mdpo-2.0.1/src/mdpo/md2po2md/__init__.py`

 * *Files identical despite different names*

### Comparing `mdpo-2.0.0/src/mdpo/md2po2md/__main__.py` & `mdpo-2.0.1/src/mdpo/md2po2md/__main__.py`

 * *Files identical despite different names*

### Comparing `mdpo-2.0.0/src/mdpo/mdpo2html/__init__.py` & `mdpo-2.0.1/src/mdpo/mdpo2html/__init__.py`

 * *Files identical despite different names*

### Comparing `mdpo-2.0.0/src/mdpo/mdpo2html/__main__.py` & `mdpo-2.0.1/src/mdpo/mdpo2html/__main__.py`

 * *Files identical despite different names*

### Comparing `mdpo-2.0.0/src/mdpo/po2md/__init__.py` & `mdpo-2.0.1/src/mdpo/po2md/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -582,23 +582,20 @@
         if block is md4c.BlockType.P:
             self._save_current_msgid()
 
             if self._inside_liblock:
                 if self._inside_quoteblock:
                     indent = '   ' * len(self._current_list_type)
                     self.current_line = f'{indent}{self.current_line}'
-                    self._save_current_line()
                 elif self._inside_liblock_first_p:
                     self._inside_liblock_first_p = False
                 else:
                     indent = '   ' * len(self._current_list_type)
                     self.current_line = f'\n{indent}{self.current_line}'
-                    self._save_current_line()
-            else:
-                self._save_current_line()
+            self._save_current_line()
 
             self._inside_pblock = False
             if self._inside_quoteblock:
                 self.current_line = '>'
                 self._save_current_line()
 
         elif block is md4c.BlockType.CODE:
```

### Comparing `mdpo-2.0.0/src/mdpo/po2md/__main__.py` & `mdpo-2.0.1/src/mdpo/po2md/__main__.py`

 * *Files identical despite different names*

### Comparing `mdpo-2.0.0/LICENSE` & `mdpo-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mdpo-2.0.0/README.md` & `mdpo-2.0.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -18,18 +18,15 @@
 </p>
 
 <h2 align="center">
   <a href="https://mondeja.github.io/mdpo/">Documentation</a>
 </h2>
 
 <p align="center">
-Complies with <a href="https://spec.commonmark.org/">CommonMark Specification</a>
-<a href="https://spec.commonmark.org/0.29">v0.29</a> and
-<a href="https://spec.commonmark.org/0.30">v0.30</a>, supporting additional features.
-</p>
+Complies with the <a href="https://spec.commonmark.org/">CommonMark Specification</a>, supporting some additional features.</p>
 
 ## Status
 
 [![Documentation status][docs-image]][docs-link]
 [![Tests][tests-image]][tests-link]
 [![Coverage status][coverage-image]][coverage-link]
```

#### html2text {}

```diff
@@ -1,14 +1,14 @@
                                     _[_m_d_p_o_]
                ****** MMaarrkkddoowwnn ffiilleess ttrraannssllaattiioonn uussiinngg PPOO ffiilleess ******
                 _[_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/
   _m_d_p_o_?_l_o_g_o_=_p_y_t_h_o_n_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_&_l_a_b_e_l_C_o_l_o_r_=_3_3_3_3_3_3_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
           _p_y_p_i_/_l_/_m_d_p_o_?_c_o_l_o_r_=_l_i_g_h_t_-_g_r_e_e_n_&_l_o_g_o_=_f_r_e_e_b_s_d_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_]
                            ********** _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn **********
- Complies with _C_o_m_m_o_n_M_a_r_k_ _S_p_e_c_i_f_i_c_a_t_i_o_n _v_0_._2_9 and _v_0_._3_0, supporting additional
+    Complies with the _C_o_m_m_o_n_M_a_r_k_ _S_p_e_c_i_f_i_c_a_t_i_o_n, supporting some additional
                                    features.
 ## Status [![Documentation status][docs-image]][docs-link] [![Tests][tests-
 image]][tests-link] [![Coverage status][coverage-image]][coverage-link] ##
 Installation ```bash pip install mdpo ``` [tests-image]: https://
 img.shields.io/github/actions/workflow/status/mondeja/mdpo/
 ci.yml?logo=github&label=tests&branch=master [tests-link]: https://github.com/
 mondeja/mdpo/actions?query=workflow%3ACI [coverage-image]: https://
```

### Comparing `mdpo-2.0.0/pyproject.toml` & `mdpo-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mdpo"
-version = "2.0.0"
+version = "2.0.1"
 description = "Markdown files translation using PO files."
 readme = "README.md"
 license = "BSD-3-Clause"
 authors = [{ name = "Álvaro Mondéjar Rubio", email = "mondejar1994@gmail.com" }]
 requires-python = ">=3.8,<3.13"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
```

### Comparing `mdpo-2.0.0/PKG-INFO` & `mdpo-2.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: mdpo
-Version: 2.0.0
+Version: 2.0.1
 Summary: Markdown files translation using PO files.
 Project-URL: Source, https://github.com/mondeja/mdpo
 Project-URL: Documentation, https://mondeja.github.io/mdpo
 Project-URL: Bug tracker, https://github.com/mondeja/mdpo/issues
 Project-URL: Changelog, https://github.com/mondeja/mdpo/releases
 Author-email: Álvaro Mondéjar Rubio <mondejar1994@gmail.com>
 License-Expression: BSD-3-Clause
@@ -52,18 +52,15 @@
 </p>
 
 <h2 align="center">
   <a href="https://mondeja.github.io/mdpo/">Documentation</a>
 </h2>
 
 <p align="center">
-Complies with <a href="https://spec.commonmark.org/">CommonMark Specification</a>
-<a href="https://spec.commonmark.org/0.29">v0.29</a> and
-<a href="https://spec.commonmark.org/0.30">v0.30</a>, supporting additional features.
-</p>
+Complies with the <a href="https://spec.commonmark.org/">CommonMark Specification</a>, supporting some additional features.</p>
 
 ## Status
 
 [![Documentation status][docs-image]][docs-link]
 [![Tests][tests-image]][tests-link]
 [![Coverage status][coverage-image]][coverage-link]
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mdpo Version: 2.0.0 Summary: Markdown files
+Metadata-Version: 2.3 Name: mdpo Version: 2.0.1 Summary: Markdown files
 translation using PO files. Project-URL: Source, https://github.com/mondeja/
 mdpo Project-URL: Documentation, https://mondeja.github.io/mdpo Project-URL:
 Bug tracker, https://github.com/mondeja/mdpo/issues Project-URL: Changelog,
 https://github.com/mondeja/mdpo/releases Author-email: Ãlvaro MondÃ©jar Rubio
 gmail.com> License-Expression: BSD-3-Clause License-File: LICENSE Keywords:
 html,i18n,markdown,po,pofile,translation Classifier: Development Status :: 5 -
 Production/Stable Classifier: Environment :: Console Classifier: Intended
@@ -20,15 +20,15 @@
 markdown
                                     _[_m_d_p_o_]
                ****** MMaarrkkddoowwnn ffiilleess ttrraannssllaattiioonn uussiinngg PPOO ffiilleess ******
                 _[_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/
   _m_d_p_o_?_l_o_g_o_=_p_y_t_h_o_n_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_&_l_a_b_e_l_C_o_l_o_r_=_3_3_3_3_3_3_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/
           _p_y_p_i_/_l_/_m_d_p_o_?_c_o_l_o_r_=_l_i_g_h_t_-_g_r_e_e_n_&_l_o_g_o_=_f_r_e_e_b_s_d_&_l_o_g_o_C_o_l_o_r_=_w_h_i_t_e_]
                            ********** _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn **********
- Complies with _C_o_m_m_o_n_M_a_r_k_ _S_p_e_c_i_f_i_c_a_t_i_o_n _v_0_._2_9 and _v_0_._3_0, supporting additional
+    Complies with the _C_o_m_m_o_n_M_a_r_k_ _S_p_e_c_i_f_i_c_a_t_i_o_n, supporting some additional
                                    features.
 ## Status [![Documentation status][docs-image]][docs-link] [![Tests][tests-
 image]][tests-link] [![Coverage status][coverage-image]][coverage-link] ##
 Installation ```bash pip install mdpo ``` [tests-image]: https://
 img.shields.io/github/actions/workflow/status/mondeja/mdpo/
 ci.yml?logo=github&label=tests&branch=master [tests-link]: https://github.com/
 mondeja/mdpo/actions?query=workflow%3ACI [coverage-image]: https://
```

