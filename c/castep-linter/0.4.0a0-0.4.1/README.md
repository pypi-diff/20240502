# Comparing `tmp/castep_linter-0.4.0a0.tar.gz` & `tmp/castep_linter-0.4.1.tar.gz`

## Comparing `castep_linter-0.4.0a0.tar` & `castep_linter-0.4.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/.github/workflows/python-app.yml
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/__init__.py
--rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/scan_files.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/error_logging/__init__.py
--rw-r--r--   0        0        0     4326 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/error_logging/error_types.py
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/error_logging/json_writer.py
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/error_logging/logger.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/error_logging/xml_writer.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/fortran/__init__.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/fortran/fortran_raw_types.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/fortran/identifier.py
--rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/fortran/node_factory.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/fortran/node_type_err.py
--rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/fortran/parser.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/fortran/fortran_nodes/__init__.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/fortran/fortran_nodes/argument_types.py
--rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/fortran/fortran_nodes/fortran_argument_list.py
--rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/fortran/fortran_nodes/fortran_call_expression_node.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/fortran/fortran_nodes/fortran_function_node.py
--rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/fortran/fortran_nodes/fortran_node.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/fortran/fortran_nodes/fortran_subroutine_node.py
--rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/fortran/fortran_nodes/fortran_var_decl_node.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/tests/__init__.py
--rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/tests/allocate_stat_checked.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/tests/castep_identifiers.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/tests/complex_has_dp.py
--rw-r--r--   0        0        0     3669 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/tests/has_trace_entry_exit.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/tests/number_literal_correct_kind.py
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/tests/real_declaration_has_dp.py
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/tree_sitter_fortran/gen.py
--rw-r--r--   0        0        0   266661 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/tree_sitter_fortran/src/grammar.json
--rw-r--r--   0        0        0   168007 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/tree_sitter_fortran/src/node-types.json
--rw-r--r--   0        0        0  6209252 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/tree_sitter_fortran/src/parser.c
--rw-r--r--   0        0        0    11112 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/tree_sitter_fortran/src/scanner.c
--rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/src/castep_linter/tree_sitter_fortran/src/tree_sitter/parser.h
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/tests/__init__.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/tests/conftest.py
--rw-r--r--   0        0        0     6040 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/tests/test_allocate_stat_checked.py
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/tests/test_complex_delc_has_dp.py
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/tests/test_complex_function_has_dp.py
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/tests/test_identifier.py
--rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/tests/test_integer_literal_has_correct_kind.py
--rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/tests/test_real_delc_has_dp.py
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/tests/test_real_literal_has_correct_kind.py
--rw-r--r--   0        0        0     7017 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/tests/test_trace_entry_exit.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/utils/flycheck-castep.el
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/.gitignore
--rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/LICENSE.txt
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/README.md
--rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/pyproject.toml
--rw-r--r--   0        0        0     1109 2020-02-02 00:00:00.000000 castep_linter-0.4.0a0/PKG-INFO
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 castep_linter-0.4.1/.github/workflows/python-app.yml
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 castep_linter-0.4.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/__init__.py
+-rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/scan_files.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/error_logging/__init__.py
+-rw-r--r--   0        0        0     4326 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/error_logging/error_types.py
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/error_logging/json_writer.py
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/error_logging/logger.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/error_logging/xml_writer.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/fortran/__init__.py
+-rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/fortran/fortran_raw_types.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/fortran/identifier.py
+-rw-r--r--   0        0        0     1008 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/fortran/node_factory.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/fortran/node_type_err.py
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/fortran/parser.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/fortran/fortran_nodes/__init__.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/fortran/fortran_nodes/argument_types.py
+-rw-r--r--   0        0        0     2168 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/fortran/fortran_nodes/fortran_argument_list.py
+-rw-r--r--   0        0        0     1485 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/fortran/fortran_nodes/fortran_call_expression_node.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/fortran/fortran_nodes/fortran_function_node.py
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/fortran/fortran_nodes/fortran_node.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/fortran/fortran_nodes/fortran_subroutine_node.py
+-rw-r--r--   0        0        0     3121 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/fortran/fortran_nodes/fortran_var_decl_node.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/tests/__init__.py
+-rw-r--r--   0        0        0     5105 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/tests/allocate_stat_checked.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/tests/castep_identifiers.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/tests/complex_has_dp.py
+-rw-r--r--   0        0        0     4057 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/tests/has_trace_entry_exit.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/tests/number_literal_correct_kind.py
+-rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/tests/real_declaration_has_dp.py
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/tree_sitter_fortran/gen.py
+-rw-r--r--   0        0        0   266661 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/tree_sitter_fortran/src/grammar.json
+-rw-r--r--   0        0        0   168007 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/tree_sitter_fortran/src/node-types.json
+-rw-r--r--   0        0        0  6209252 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/tree_sitter_fortran/src/parser.c
+-rw-r--r--   0        0        0    11112 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/tree_sitter_fortran/src/scanner.c
+-rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 castep_linter-0.4.1/src/castep_linter/tree_sitter_fortran/src/tree_sitter/parser.h
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 castep_linter-0.4.1/tests/__init__.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 castep_linter-0.4.1/tests/conftest.py
+-rw-r--r--   0        0        0     6040 2020-02-02 00:00:00.000000 castep_linter-0.4.1/tests/test_allocate_stat_checked.py
+-rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 castep_linter-0.4.1/tests/test_complex_delc_has_dp.py
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 castep_linter-0.4.1/tests/test_complex_function_has_dp.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 castep_linter-0.4.1/tests/test_identifier.py
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 castep_linter-0.4.1/tests/test_integer_literal_has_correct_kind.py
+-rw-r--r--   0        0        0     3291 2020-02-02 00:00:00.000000 castep_linter-0.4.1/tests/test_real_delc_has_dp.py
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 castep_linter-0.4.1/tests/test_real_literal_has_correct_kind.py
+-rw-r--r--   0        0        0     7829 2020-02-02 00:00:00.000000 castep_linter-0.4.1/tests/test_trace_entry_exit.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 castep_linter-0.4.1/utils/flycheck-castep.el
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 castep_linter-0.4.1/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 castep_linter-0.4.1/LICENSE.txt
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 castep_linter-0.4.1/README.md
+-rw-r--r--   0        0        0     3514 2020-02-02 00:00:00.000000 castep_linter-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 castep_linter-0.4.1/PKG-INFO
```

### Comparing `castep_linter-0.4.0a0/.github/workflows/python-app.yml` & `castep_linter-0.4.1/.github/workflows/python-app.yml`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/.github/workflows/python-publish.yml` & `castep_linter-0.4.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/src/castep_linter/scan_files.py` & `castep_linter-0.4.1/src/castep_linter/scan_files.py`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/src/castep_linter/error_logging/error_types.py` & `castep_linter-0.4.1/src/castep_linter/error_logging/error_types.py`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/src/castep_linter/error_logging/json_writer.py` & `castep_linter-0.4.1/src/castep_linter/error_logging/json_writer.py`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/src/castep_linter/error_logging/logger.py` & `castep_linter-0.4.1/src/castep_linter/error_logging/logger.py`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/src/castep_linter/error_logging/xml_writer.py` & `castep_linter-0.4.1/src/castep_linter/error_logging/xml_writer.py`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/src/castep_linter/fortran/fortran_raw_types.py` & `castep_linter-0.4.1/src/castep_linter/fortran/fortran_raw_types.py`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/src/castep_linter/fortran/identifier.py` & `castep_linter-0.4.1/src/castep_linter/fortran/identifier.py`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/src/castep_linter/fortran/node_factory.py` & `castep_linter-0.4.1/src/castep_linter/fortran/node_factory.py`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/src/castep_linter/fortran/parser.py` & `castep_linter-0.4.1/src/castep_linter/fortran/parser.py`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/src/castep_linter/fortran/fortran_nodes/__init__.py` & `castep_linter-0.4.1/src/castep_linter/fortran/fortran_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/src/castep_linter/fortran/fortran_nodes/fortran_argument_list.py` & `castep_linter-0.4.1/src/castep_linter/fortran/fortran_nodes/fortran_argument_list.py`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/src/castep_linter/fortran/fortran_nodes/fortran_call_expression_node.py` & `castep_linter-0.4.1/src/castep_linter/fortran/fortran_nodes/fortran_call_expression_node.py`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/src/castep_linter/fortran/fortran_nodes/fortran_node.py` & `castep_linter-0.4.1/src/castep_linter/fortran/fortran_nodes/fortran_node.py`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/src/castep_linter/fortran/fortran_nodes/fortran_var_decl_node.py` & `castep_linter-0.4.1/src/castep_linter/fortran/fortran_nodes/fortran_var_decl_node.py`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/src/castep_linter/tests/__init__.py` & `castep_linter-0.4.1/src/castep_linter/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/src/castep_linter/tests/allocate_stat_checked.py` & `castep_linter-0.4.1/src/castep_linter/tests/allocate_stat_checked.py`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/src/castep_linter/tests/castep_identifiers.py` & `castep_linter-0.4.1/src/castep_linter/tests/castep_identifiers.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,18 @@
 from castep_linter.fortran.identifier import Identifier
 
 # TRACE THINGS
 TRACE_ENTRY = Identifier("trace_entry")
 TRACE_EXIT = Identifier("trace_exit")
 TRACE_STRING = Identifier("string")
 
+# Exceptions for trace subroutine names
+CASTEP_TRACE = Identifier("castep")
+TRACE_NAME_EXCEPTIONS = [CASTEP_TRACE]
+
 
 CMPLX = Identifier("cmplx")
 
 # Parameters
 DP = Identifier("dp")
 DPREC = Identifier("dprec")
 DI_DP = Identifier("di_dp")
```

### Comparing `castep_linter-0.4.0a0/src/castep_linter/tests/complex_has_dp.py` & `castep_linter-0.4.1/src/castep_linter/tests/complex_has_dp.py`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/src/castep_linter/tests/has_trace_entry_exit.py` & `castep_linter-0.4.1/src/castep_linter/tests/has_trace_entry_exit.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,23 @@
 )
 from castep_linter.fortran.fortran_raw_types import Fortran, FType
 from castep_linter.fortran.identifier import Identifier
 from castep_linter.fortran.node_type_err import WrongNodeError
 from castep_linter.tests import castep_identifiers
 
 
+def correct_trace_name(trace_name: str, subroutine_name: Identifier):
+    """Checks whether a subroutine name given to trace is fine. Allows exceptions from the global list"""
+    trace_name = trace_name.lower()
+    if trace_name in castep_identifiers.TRACE_NAME_EXCEPTIONS:
+        return True
+    else:
+        return trace_name == subroutine_name
+
+
 def check_trace_entry_exit(node: FortranNode, error_log: ErrorLogger) -> None:
     """Test that a subroutine or function has a trace_entry and trace_exit with the correct name"""
 
     if node.is_type(Fortran.SUBROUTINE) or node.is_type(Fortran.FUNCTION):
         subroutine_name = node.get_context_identifier()
     else:
         err = "Wrong node type passed"
@@ -56,25 +65,25 @@
         except KeyError:
             err = f"Unparsable name passed to trace in {subroutine_name}"
             error_log.add_msg("Error", routine, err)
             continue
 
         if trace_node.is_type(Fortran.STRING_LITERAL):
             trace_string = trace_node.parse_string_literal().lower()
-            if trace_string != subroutine_name:
+            if not correct_trace_name(trace_string, subroutine_name):
                 err = f"Incorrect name passed to trace in {subroutine_name}"
                 error_log.add_msg("Error", trace_node, err)
 
         elif trace_node.is_type(Fortran.IDENTIFIER):
             trace_sub_text = Identifier.from_node(trace_node)
 
             if trace_sub_text in const_string_vars:
                 trace_string = const_string_vars[trace_sub_text]
 
-                if trace_string.lower() != subroutine_name:
+                if not correct_trace_name(trace_string, subroutine_name):
                     err = (
                         f"Incorrect name passed to trace in {subroutine_name} "
                         f'by variable {trace_sub_text}="{trace_string}"'
                     )
                     error_log.add_msg("Error", trace_node, err)
             else:
                 err = f"Unidentified variable {trace_sub_text} passed to trace in {subroutine_name}"
```

### Comparing `castep_linter-0.4.0a0/src/castep_linter/tests/number_literal_correct_kind.py` & `castep_linter-0.4.1/src/castep_linter/tests/number_literal_correct_kind.py`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/src/castep_linter/tests/real_declaration_has_dp.py` & `castep_linter-0.4.1/src/castep_linter/tests/real_declaration_has_dp.py`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/src/castep_linter/tree_sitter_fortran/src/grammar.json` & `castep_linter-0.4.1/src/castep_linter/tree_sitter_fortran/src/grammar.json`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/src/castep_linter/tree_sitter_fortran/src/node-types.json` & `castep_linter-0.4.1/src/castep_linter/tree_sitter_fortran/src/node-types.json`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/src/castep_linter/tree_sitter_fortran/src/parser.c` & `castep_linter-0.4.1/src/castep_linter/tree_sitter_fortran/src/parser.c`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/src/castep_linter/tree_sitter_fortran/src/scanner.c` & `castep_linter-0.4.1/src/castep_linter/tree_sitter_fortran/src/scanner.c`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/src/castep_linter/tree_sitter_fortran/src/tree_sitter/parser.h` & `castep_linter-0.4.1/src/castep_linter/tree_sitter_fortran/src/tree_sitter/parser.h`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/tests/conftest.py` & `castep_linter-0.4.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/tests/test_allocate_stat_checked.py` & `castep_linter-0.4.1/tests/test_allocate_stat_checked.py`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/tests/test_complex_delc_has_dp.py` & `castep_linter-0.4.1/tests/test_complex_delc_has_dp.py`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/tests/test_complex_function_has_dp.py` & `castep_linter-0.4.1/tests/test_complex_function_has_dp.py`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/tests/test_identifier.py` & `castep_linter-0.4.1/tests/test_identifier.py`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/tests/test_integer_literal_has_correct_kind.py` & `castep_linter-0.4.1/tests/test_integer_literal_has_correct_kind.py`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/tests/test_real_delc_has_dp.py` & `castep_linter-0.4.1/tests/test_real_delc_has_dp.py`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/tests/test_real_literal_has_correct_kind.py` & `castep_linter-0.4.1/tests/test_real_literal_has_correct_kind.py`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/tests/test_trace_entry_exit.py` & `castep_linter-0.4.1/tests/test_trace_entry_exit.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,14 +142,41 @@
     call trace_exit(sub_name, stat)
     """
     )
     error_log = run_tests_on_code(parse(code), test_list, "filename")
     assert len(error_log.errors) == 2
 
 
+def test_trace_entry_exit_wrong_name_exception(
+    parse: Parser, subroutine_wrapper: CodeWrapper, test_list: CheckFunctionDict
+):
+    code = subroutine_wrapper(
+        b"""
+    call trace_entry("castep", stat)
+    call trace_exit("castep", stat)
+    """
+    )
+    error_log = run_tests_on_code(parse(code), test_list, "filename")
+    assert len(error_log.errors) == 0
+
+
+def test_trace_entry_exit_wrong_name_by_param_exception(
+    parse: Parser, subroutine_wrapper: CodeWrapper, test_list: CheckFunctionDict
+):
+    code = subroutine_wrapper(
+        b"""
+    character(len=100), parameter :: sub_name = "castep"
+    call trace_entry(sub_name, stat)
+    call trace_exit(sub_name, stat)
+    """
+    )
+    error_log = run_tests_on_code(parse(code), test_list, "filename")
+    assert len(error_log.errors) == 0
+
+
 def test_trace_entry_exit_no_name(
     parse: Parser, subroutine_wrapper: CodeWrapper, test_list: CheckFunctionDict
 ):
     code = subroutine_wrapper(
         b"""
     call trace_entry()
     call trace_exit()
```

### Comparing `castep_linter-0.4.0a0/utils/flycheck-castep.el` & `castep_linter-0.4.1/utils/flycheck-castep.el`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/LICENSE.txt` & `castep_linter-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/pyproject.toml` & `castep_linter-0.4.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `castep_linter-0.4.0a0/PKG-INFO` & `castep_linter-0.4.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: castep-linter
-Version: 0.4.0a0
+Version: 0.4.1
 Project-URL: Documentation, https://github.com/byornski/castep-linter#readme
 Project-URL: Issues, https://github.com/byornski/castep-linter/issues
 Project-URL: Source, https://github.com/byornski/castep-linter
 Author-email: Peter Byrne <peter.byrne@york.ac.uk>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
```

