# Comparing `tmp/suql-1.1.6.tar.gz` & `tmp/suql-1.1.7a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suql-1.1.6.tar", last modified: Tue Apr 30 04:29:06 2024, max compression
+gzip compressed data, was "suql-1.1.7a0.tar", last modified: Thu May  2 05:38:24 2024, max compression
```

## Comparing `suql-1.1.6.tar` & `suql-1.1.7a0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwx------   0 oval      (1000) users      (100)        0 2024-04-30 04:29:06.602478 suql-1.1.6/
--rw-------   0 oval      (1000) users      (100)    11356 2024-04-03 06:02:28.000000 suql-1.1.6/LICENSE
--rw-------   0 oval      (1000) users      (100)     5019 2024-04-30 04:29:06.602478 suql-1.1.6/PKG-INFO
--rw-------   0 oval      (1000) users      (100)     4415 2024-04-30 04:28:53.000000 suql-1.1.6/README.md
--rw-------   0 oval      (1000) users      (100)       38 2024-04-30 04:29:06.602478 suql-1.1.6/setup.cfg
--rw-------   0 oval      (1000) users      (100)     1539 2024-04-30 04:28:53.000000 suql-1.1.6/setup.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-30 04:29:06.598478 suql-1.1.6/src/
-drwx------   0 oval      (1000) users      (100)        0 2024-04-30 04:29:06.598478 suql-1.1.6/src/suql/
--rw-------   0 oval      (1000) users      (100)       73 2024-04-03 06:02:28.000000 suql-1.1.6/src/suql/__init__.py
--rw-------   0 oval      (1000) users      (100)    17393 2024-04-25 17:52:02.000000 suql-1.1.6/src/suql/agent.py
--rw-------   0 oval      (1000) users      (100)    20797 2024-04-30 04:28:53.000000 suql-1.1.6/src/suql/faiss_embedding.py
--rw-------   0 oval      (1000) users      (100)     8792 2024-04-17 07:27:02.000000 suql-1.1.6/src/suql/free_text_fcns_server.py
--rw-------   0 oval      (1000) users      (100)     3563 2024-04-25 17:52:02.000000 suql-1.1.6/src/suql/postgresql_connection.py
--rw-------   0 oval      (1000) users      (100)     9612 2024-04-17 08:33:05.000000 suql-1.1.6/src/suql/prompt_continuation.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-30 04:29:06.602478 suql-1.1.6/src/suql/prompts/
--rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:18.000000 suql-1.1.6/src/suql/prompts/__init__.py
--rw-------   0 oval      (1000) users      (100)      169 2024-04-03 06:02:28.000000 suql-1.1.6/src/suql/prompts/answer_qa.prompt
--rw-------   0 oval      (1000) users      (100)      451 2024-04-03 06:02:28.000000 suql-1.1.6/src/suql/prompts/field_classification.prompt
--rw-------   0 oval      (1000) users      (100)     2945 2024-04-03 06:02:28.000000 suql-1.1.6/src/suql/prompts/if_db_classification.prompt
--rw-------   0 oval      (1000) users      (100)     1305 2024-04-03 06:02:28.000000 suql-1.1.6/src/suql/prompts/opening_hours.prompt
--rw-------   0 oval      (1000) users      (100)     5574 2024-04-03 06:02:28.000000 suql-1.1.6/src/suql/prompts/parser_suql.prompt
--rw-------   0 oval      (1000) users      (100)      227 2024-04-03 06:02:28.000000 suql-1.1.6/src/suql/prompts/verification.prompt
--rw-------   0 oval      (1000) users      (100)     2983 2024-04-03 06:02:28.000000 suql-1.1.6/src/suql/prompts/yelp_response_SQL.prompt
--rw-------   0 oval      (1000) users      (100)     1454 2024-04-03 06:02:28.000000 suql-1.1.6/src/suql/prompts/yelp_response_no_results.prompt
-drwx------   0 oval      (1000) users      (100)        0 2024-04-30 04:29:06.602478 suql-1.1.6/src/suql/sql_free_text_support/
--rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:11.000000 suql-1.1.6/src/suql/sql_free_text_support/__init__.py
--rw-------   0 oval      (1000) users      (100)    66566 2024-04-25 17:52:02.000000 suql-1.1.6/src/suql/sql_free_text_support/execute_free_text_sql.py
--rw-------   0 oval      (1000) users      (100)     6455 2024-04-03 06:02:28.000000 suql-1.1.6/src/suql/utils.py
-drwx------   0 oval      (1000) users      (100)        0 2024-04-30 04:29:06.602478 suql-1.1.6/src/suql.egg-info/
--rw-r--r--   0 oval      (1000) users      (100)     5019 2024-04-30 04:29:06.000000 suql-1.1.6/src/suql.egg-info/PKG-INFO
--rw-------   0 oval      (1000) users      (100)      824 2024-04-30 04:29:06.000000 suql-1.1.6/src/suql.egg-info/SOURCES.txt
--rw-------   0 oval      (1000) users      (100)        1 2024-04-30 04:29:06.000000 suql-1.1.6/src/suql.egg-info/dependency_links.txt
--rw-------   0 oval      (1000) users      (100)      206 2024-04-30 04:29:06.000000 suql-1.1.6/src/suql.egg-info/requires.txt
--rw-------   0 oval      (1000) users      (100)        5 2024-04-30 04:29:06.000000 suql-1.1.6/src/suql.egg-info/top_level.txt
+drwx------   0 oval      (1000) users      (100)        0 2024-05-02 05:38:24.807002 suql-1.1.7a0/
+-rw-------   0 oval      (1000) users      (100)    11356 2024-04-03 06:02:28.000000 suql-1.1.7a0/LICENSE
+-rw-------   0 oval      (1000) users      (100)     5021 2024-05-02 05:38:24.807002 suql-1.1.7a0/PKG-INFO
+-rw-------   0 oval      (1000) users      (100)     4415 2024-04-30 04:28:53.000000 suql-1.1.7a0/README.md
+-rw-------   0 oval      (1000) users      (100)       38 2024-05-02 05:38:24.807002 suql-1.1.7a0/setup.cfg
+-rw-------   0 oval      (1000) users      (100)     1540 2024-05-02 05:36:07.000000 suql-1.1.7a0/setup.py
+drwx------   0 oval      (1000) users      (100)        0 2024-05-02 05:38:24.807002 suql-1.1.7a0/src/
+drwx------   0 oval      (1000) users      (100)        0 2024-05-02 05:38:24.807002 suql-1.1.7a0/src/suql/
+-rw-------   0 oval      (1000) users      (100)       73 2024-04-03 06:02:28.000000 suql-1.1.7a0/src/suql/__init__.py
+-rw-------   0 oval      (1000) users      (100)    17393 2024-04-25 17:52:02.000000 suql-1.1.7a0/src/suql/agent.py
+-rw-------   0 oval      (1000) users      (100)    20797 2024-05-02 02:56:05.000000 suql-1.1.7a0/src/suql/faiss_embedding.py
+-rw-------   0 oval      (1000) users      (100)     8792 2024-04-17 07:27:02.000000 suql-1.1.7a0/src/suql/free_text_fcns_server.py
+-rw-------   0 oval      (1000) users      (100)     3563 2024-04-25 17:52:02.000000 suql-1.1.7a0/src/suql/postgresql_connection.py
+-rw-------   0 oval      (1000) users      (100)     9612 2024-04-17 08:33:05.000000 suql-1.1.7a0/src/suql/prompt_continuation.py
+drwx------   0 oval      (1000) users      (100)        0 2024-05-02 05:38:24.807002 suql-1.1.7a0/src/suql/prompts/
+-rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:18.000000 suql-1.1.7a0/src/suql/prompts/__init__.py
+-rw-------   0 oval      (1000) users      (100)      169 2024-04-03 06:02:28.000000 suql-1.1.7a0/src/suql/prompts/answer_qa.prompt
+-rw-------   0 oval      (1000) users      (100)      451 2024-04-03 06:02:28.000000 suql-1.1.7a0/src/suql/prompts/field_classification.prompt
+-rw-------   0 oval      (1000) users      (100)     2945 2024-04-03 06:02:28.000000 suql-1.1.7a0/src/suql/prompts/if_db_classification.prompt
+-rw-------   0 oval      (1000) users      (100)     1305 2024-04-03 06:02:28.000000 suql-1.1.7a0/src/suql/prompts/opening_hours.prompt
+-rw-------   0 oval      (1000) users      (100)     5574 2024-04-03 06:02:28.000000 suql-1.1.7a0/src/suql/prompts/parser_suql.prompt
+-rw-------   0 oval      (1000) users      (100)      227 2024-04-03 06:02:28.000000 suql-1.1.7a0/src/suql/prompts/verification.prompt
+-rw-------   0 oval      (1000) users      (100)     2983 2024-04-03 06:02:28.000000 suql-1.1.7a0/src/suql/prompts/yelp_response_SQL.prompt
+-rw-------   0 oval      (1000) users      (100)     1454 2024-04-03 06:02:28.000000 suql-1.1.7a0/src/suql/prompts/yelp_response_no_results.prompt
+drwx------   0 oval      (1000) users      (100)        0 2024-05-02 05:38:24.807002 suql-1.1.7a0/src/suql/sql_free_text_support/
+-rw-------   0 oval      (1000) users      (100)        0 2024-04-04 04:29:11.000000 suql-1.1.7a0/src/suql/sql_free_text_support/__init__.py
+-rw-------   0 oval      (1000) users      (100)    70712 2024-05-02 05:34:16.000000 suql-1.1.7a0/src/suql/sql_free_text_support/execute_free_text_sql.py
+-rw-------   0 oval      (1000) users      (100)     6455 2024-04-03 06:02:28.000000 suql-1.1.7a0/src/suql/utils.py
+drwx------   0 oval      (1000) users      (100)        0 2024-05-02 05:38:24.807002 suql-1.1.7a0/src/suql.egg-info/
+-rw-r--r--   0 oval      (1000) users      (100)     5021 2024-05-02 05:38:24.000000 suql-1.1.7a0/src/suql.egg-info/PKG-INFO
+-rw-------   0 oval      (1000) users      (100)      824 2024-05-02 05:38:24.000000 suql-1.1.7a0/src/suql.egg-info/SOURCES.txt
+-rw-------   0 oval      (1000) users      (100)        1 2024-05-02 05:38:24.000000 suql-1.1.7a0/src/suql.egg-info/dependency_links.txt
+-rw-------   0 oval      (1000) users      (100)      206 2024-05-02 05:38:24.000000 suql-1.1.7a0/src/suql.egg-info/requires.txt
+-rw-------   0 oval      (1000) users      (100)        5 2024-05-02 05:38:24.000000 suql-1.1.7a0/src/suql.egg-info/top_level.txt
```

### Comparing `suql-1.1.6/LICENSE` & `suql-1.1.7a0/LICENSE`

 * *Files identical despite different names*

### Comparing `suql-1.1.6/PKG-INFO` & `suql-1.1.7a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suql
-Version: 1.1.6
+Version: 1.1.7a0
 Summary: Structured and Unstructured Query Language (SUQL) Python API
 Home-page: https://github.com/stanford-oval/suql
 Author: Shicheng Liu
 Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: suql Version: 1.1.6 Summary: Structured and
+Metadata-Version: 2.1 Name: suql Version: 1.1.7a0 Summary: Structured and
 Unstructured Query Language (SUQL) Python API Home-page: https://github.com/
 stanford-oval/suql Author: Shicheng Liu Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `suql-1.1.6/README.md` & `suql-1.1.7a0/README.md`

 * *Files identical despite different names*

### Comparing `suql-1.1.6/setup.py` & `suql-1.1.7a0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 # Package metadata
 name = "suql"
-version = "1.1.6"
+version = "1.1.7a"
 description = "Structured and Unstructured Query Language (SUQL) Python API"
 author = "Shicheng Liu"
 author_email = "shicheng@cs.stanford.edu"
 url = "https://github.com/stanford-oval/suql"
 
 # Specify the packages to include. You can use `find_packages` to automatically discover them.
 packages = find_packages(where="src")
```

### Comparing `suql-1.1.6/src/suql/agent.py` & `suql-1.1.7a0/src/suql/agent.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.6/src/suql/faiss_embedding.py` & `suql-1.1.7a0/src/suql/faiss_embedding.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.6/src/suql/free_text_fcns_server.py` & `suql-1.1.7a0/src/suql/free_text_fcns_server.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.6/src/suql/postgresql_connection.py` & `suql-1.1.7a0/src/suql/postgresql_connection.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.6/src/suql/prompt_continuation.py` & `suql-1.1.7a0/src/suql/prompt_continuation.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.6/src/suql/prompts/if_db_classification.prompt` & `suql-1.1.7a0/src/suql/prompts/if_db_classification.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.6/src/suql/prompts/opening_hours.prompt` & `suql-1.1.7a0/src/suql/prompts/opening_hours.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.6/src/suql/prompts/parser_suql.prompt` & `suql-1.1.7a0/src/suql/prompts/parser_suql.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.6/src/suql/prompts/yelp_response_SQL.prompt` & `suql-1.1.7a0/src/suql/prompts/yelp_response_SQL.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.6/src/suql/prompts/yelp_response_no_results.prompt` & `suql-1.1.7a0/src/suql/prompts/yelp_response_no_results.prompt`

 * *Files identical despite different names*

### Comparing `suql-1.1.6/src/suql/sql_free_text_support/execute_free_text_sql.py` & `suql-1.1.7a0/src/suql/sql_free_text_support/execute_free_text_sql.py`

 * *Files 3% similar despite different names*

```diff
@@ -1634,14 +1634,114 @@
     if source not in source_file_mapping:
         return None
     
     with open(source_file_mapping[source], "r") as fd:
         source_content = fd.read()
     
     return _answer(source_content, query)
+
+def _check_predicate_exist(a_expr: A_Expr, field_name: str):
+    if isinstance(a_expr.lexpr, ColumnRef):
+        for i in a_expr.lexpr.fields:
+            if isinstance(i, String) and i.sval == field_name:
+                return True
+        
+    if isinstance(a_expr.rexpr, ColumnRef):
+        for i in a_expr.rexpr.fields:
+            if isinstance(i, String) and i.sval == field_name:
+                return True
+    
+    return False
+
+
+class _RequiredParamMappingVisitor(Visitor):
+    def __init__(
+        self,
+        required_params_mapping
+    ) -> None:
+        super().__init__()
+        self.required_params_mapping = required_params_mapping
+        self.missing_params = defaultdict(set)        
+     
+    def visit_SelectStmt(self, ancestors, node: SelectStmt):
+
+        def check_a_expr_or_and_expr(_dnf_predicate, _field):
+            if isinstance(_dnf_predicate, A_Expr):
+                return _check_predicate_exist(_dnf_predicate, _field)
+            elif (
+                isinstance(_dnf_predicate, BoolExpr)
+                and _dnf_predicate.boolop == BoolExprType.AND_EXPR
+            ):
+                found = False
+                for i in _dnf_predicate.args:
+                    # there could also be NOT clauses
+                    if isinstance(i, A_Expr):
+                        if _check_predicate_exist(i, _field):
+                            found = True
+                            break
+                        
+                return found
+            
+            return False
+        
+        
+        for table in node.fromClause:
+            if isinstance(table, RangeVar) and table.relname in self.required_params_mapping:
+                assert type(self.required_params_mapping[table.relname]) == list
+                
+                if not node.whereClause:
+                    self.missing_params[table.relname].update(self.required_params_mapping[table.relname])
+                    continue
+                
+                dnf_predicate = _convert2dnf(node.whereClause)
+
+                if (
+                    isinstance(dnf_predicate, BoolExpr)
+                    and dnf_predicate.boolop == BoolExprType.OR_EXPR
+                ):
+                    for field in self.required_params_mapping[table.relname]:
+                        if not all(check_a_expr_or_and_expr(i, field) for i in dnf_predicate.args):
+                            self.missing_params[table.relname].add(field)
+                else:
+                    # target condition:
+                    # if isinstance(dnf_predicate, A_Expr) or (
+                    #     isinstance(dnf_predicate, BoolExpr)
+                    #     and dnf_predicate.boolop == BoolExprType.AND_EXPR
+                    # ):
+                    # and if it is a NOT, in which case we just return False
+                    for field in self.required_params_mapping[table.relname]:
+                        if not check_a_expr_or_and_expr(dnf_predicate, field):
+                            self.missing_params[table.relname].add(field)
+                    
+
+def _check_required_params(suql, required_params_mapping):
+    """
+    Check whether all required parameters exist in the `suql`.
+    
+    # Parameters:
+    `suql` (str): The to-be-executed suql query.
+    
+    `required_params_mapping` (Dict(str -> List[str]), optional): *Experimental feature*: a dictionary mapping
+    from table names to a list of "required" parameters for the tables. The SUQL compiler will check whether the
+    SUQL query contains all required parameters (i.e., whether for each such table there exists a `WHERE` clause
+    with the required parameter).
+    
+    # Returns:
+    `if_all_exist` (bool): whether all required parameters exist.
+    
+    `missing_params` (Dict(str -> List[str]): a mapping from table names to a list of required missing parameters.
+    """
+    root = parse_sql(suql)
+    visitor = _RequiredParamMappingVisitor(required_params_mapping)
+    visitor(root)
+    
+    if visitor.missing_params:
+        return False, {key: list(value) for key, value in visitor.missing_params.items()}
+    else:
+        return True, {}
     
 
 def suql_execute(
     suql,
     table_w_ids,
     database,
     fts_fields=[],
@@ -1692,19 +1792,19 @@
     
     `select_userpswd` (str, optional): above user's password with select privilege in db. Defaults to "select_user".
     
     `create_username` (str, optional): user name with create privilege in db. Defaults to "creator_role".
     
     `create_userpswd` (str, optional): above user's password with create privilege in db. Defaults to "creator_role".
 
-    `source_file_mapping` (Dict(str -> str), optional): Experimental feature - a dictionary mapping from variable
+    `source_file_mapping` (Dict(str -> str), optional): *Experimental feature*: a dictionary mapping from variable
     names to the file locations. This would support queries that only need a free text source, e.g.,
     `suql = answer(yelp_general_info, 'what is your cancellation policy?')`. In this case, you can specify
     `source_file_mapping = {"yelp_general_info": "PATH TO FILE"}` to inform the SUQL compiler where to find
-    `yelp_general_info`.
+    `yelp_general_info`. Defaults to `{}`.
 
     # Returns:
     `results` (List[[*]]): A list of returned database results. Each inner list stores a row of returned result.
     
     `column_names` (List[str]): A list of database column names in the same order as `results`.
     
     `cache` (Dict()): Debugging information from the SUQL compiler.
```

### Comparing `suql-1.1.6/src/suql/utils.py` & `suql-1.1.7a0/src/suql/utils.py`

 * *Files identical despite different names*

### Comparing `suql-1.1.6/src/suql.egg-info/PKG-INFO` & `suql-1.1.7a0/src/suql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suql
-Version: 1.1.6
+Version: 1.1.7a0
 Summary: Structured and Unstructured Query Language (SUQL) Python API
 Home-page: https://github.com/stanford-oval/suql
 Author: Shicheng Liu
 Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: suql Version: 1.1.6 Summary: Structured and
+Metadata-Version: 2.1 Name: suql Version: 1.1.7a0 Summary: Structured and
 Unstructured Query Language (SUQL) Python API Home-page: https://github.com/
 stanford-oval/suql Author: Shicheng Liu Author-email: shicheng@cs.stanford.edu
 Classifier: License :: OSI Approved :: Apache Software License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `suql-1.1.6/src/suql.egg-info/SOURCES.txt` & `suql-1.1.7a0/src/suql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

