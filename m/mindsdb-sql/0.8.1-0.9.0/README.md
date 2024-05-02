# Comparing `tmp/mindsdb_sql-0.8.1.tar.gz` & `tmp/mindsdb_sql-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mindsdb_sql-0.8.1.tar", last modified: Thu Dec  7 12:55:37 2023, max compression
+gzip compressed data, was "dist\mindsdb_sql-0.9.0.tar", last modified: Tue Dec 19 08:26:13 2023, max compression
```

## Comparing `mindsdb_sql-0.8.1.tar` & `mindsdb_sql-0.9.0.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxrwx   0        0        0        0 2023-12-07 12:55:37.000000 mindsdb_sql-0.8.1/
--rw-rw-rw-   0        0        0      535 2023-12-07 12:55:37.000000 mindsdb_sql-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     7227 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/README.md
-drwxrwxrwx   0        0        0        0 2023-12-07 12:55:37.000000 mindsdb_sql-0.8.1/mindsdb_sql/
--rw-rw-rw-   0        0        0      365 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/__about__.py
--rw-rw-rw-   0        0        0     1196 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/__init__.py
--rw-rw-rw-   0        0        0      170 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-12-07 12:55:37.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/
--rw-rw-rw-   0        0        0        0 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-07 12:55:37.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/
--rw-rw-rw-   0        0        0      537 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/__init__.py
--rw-rw-rw-   0        0        0      842 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/alter_table.py
--rw-rw-rw-   0        0        0     1539 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/base.py
--rw-rw-rw-   0        0        0      460 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/commit_transaction.py
--rw-rw-rw-   0        0        0     3032 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/create.py
--rw-rw-rw-   0        0        0      994 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/delete.py
--rw-rw-rw-   0        0        0      942 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/describe.py
--rw-rw-rw-   0        0        0     3056 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/drop.py
--rw-rw-rw-   0        0        0      659 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/explain.py
--rw-rw-rw-   0        0        0     3260 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/insert.py
--rw-rw-rw-   0        0        0      466 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/rollback_transaction.py
-drwxrwxrwx   0        0        0        0 2023-12-07 12:55:37.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/
--rw-rw-rw-   0        0        0      597 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/__init__.py
--rw-rw-rw-   0        0        0     1482 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/case.py
--rw-rw-rw-   0        0        0     1113 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/common_table_expression.py
--rw-rw-rw-   0        0        0     1952 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/constant.py
--rw-rw-rw-   0        0        0      503 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/data.py
--rw-rw-rw-   0        0        0     3196 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/identifier.py
--rw-rw-rw-   0        0        0     1381 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/join.py
--rw-rw-rw-   0        0        0      662 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/native_query.py
--rw-rw-rw-   0        0        0     5949 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/operation.py
--rw-rw-rw-   0        0        0      806 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/order_by.py
--rw-rw-rw-   0        0        0      464 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/parameter.py
--rw-rw-rw-   0        0        0     5904 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/select.py
--rw-rw-rw-   0        0        0      504 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/star.py
--rw-rw-rw-   0        0        0      648 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/tuple.py
--rw-rw-rw-   0        0        0      774 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/type_cast.py
--rw-rw-rw-   0        0        0     1178 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/union.py
--rw-rw-rw-   0        0        0     3296 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/set.py
--rw-rw-rw-   0        0        0     2979 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/show.py
--rw-rw-rw-   0        0        0      469 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/start_transaction.py
--rw-rw-rw-   0        0        0     3154 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/update.py
--rw-rw-rw-   0        0        0      639 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/use.py
-drwxrwxrwx   0        0        0        0 2023-12-07 12:55:37.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/
--rw-rw-rw-   0        0        0        0 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-07 12:55:37.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/
--rw-rw-rw-   0        0        0      999 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/__init__.py
--rw-rw-rw-   0        0        0     3254 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/agents.py
--rw-rw-rw-   0        0        0     2893 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/chatbot.py
--rw-rw-rw-   0        0        0     1794 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/create_database.py
--rw-rw-rw-   0        0        0      953 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/create_file.py
--rw-rw-rw-   0        0        0     2383 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/create_job.py
--rw-rw-rw-   0        0        0     1400 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py
--rw-rw-rw-   0        0        0     6029 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py
--rw-rw-rw-   0        0        0     1799 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/create_view.py
--rw-rw-rw-   0        0        0      873 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py
--rw-rw-rw-   0        0        0      882 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py
--rw-rw-rw-   0        0        0      861 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/drop_job.py
--rw-rw-rw-   0        0        0      877 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py
--rw-rw-rw-   0        0        0      906 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py
--rw-rw-rw-   0        0        0     1313 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/evaluate.py
--rw-rw-rw-   0        0        0      223 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/finetune_predictor.py
--rw-rw-rw-   0        0        0     3563 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/knowledge_base.py
--rw-rw-rw-   0        0        0      359 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/latest.py
--rw-rw-rw-   0        0        0     8673 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/lexer.py
--rw-rw-rw-   0        0        0    53190 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/parser.py
--rw-rw-rw-   0        0        0      311 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/retrain_predictor.py
--rw-rw-rw-   0        0        0     3221 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/skills.py
--rw-rw-rw-   0        0        0     2246 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/trigger.py
-drwxrwxrwx   0        0        0        0 2023-12-07 12:55:37.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mysql/
--rw-rw-rw-   0        0        0       67 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mysql/__init__.py
--rw-rw-rw-   0        0        0     1046 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mysql/lexer.py
--rw-rw-rw-   0        0        0    29491 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mysql/parser.py
--rw-rw-rw-   0        0        0      904 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mysql/show_index.py
--rw-rw-rw-   0        0        0      686 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mysql/variable.py
--rw-rw-rw-   0        0        0     6231 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/lexer.py
--rw-rw-rw-   0        0        0      751 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/logger.py
--rw-rw-rw-   0        0        0    21382 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/parser.py
--rw-rw-rw-   0        0        0     2497 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/parser/utils.py
-drwxrwxrwx   0        0        0        0 2023-12-07 12:55:37.000000 mindsdb_sql-0.8.1/mindsdb_sql/planner/
--rw-rw-rw-   0        0        0      150 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/planner/__init__.py
--rw-rw-rw-   0        0        0      878 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/planner/query_plan.py
--rw-rw-rw-   0        0        0    55929 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/planner/query_planner.py
--rw-rw-rw-   0        0        0    21398 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/planner/query_prepare.py
--rw-rw-rw-   0        0        0      536 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/planner/step_result.py
--rw-rw-rw-   0        0        0     8788 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/planner/steps.py
--rw-rw-rw-   0        0        0     2981 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/planner/ts_utils.py
--rw-rw-rw-   0        0        0    13797 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/planner/utils.py
-drwxrwxrwx   0        0        0        0 2023-12-07 12:55:37.000000 mindsdb_sql-0.8.1/mindsdb_sql/render/
--rw-rw-rw-   0        0        0        0 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/render/__init__.py
--rw-rw-rw-   0        0        0    21146 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/mindsdb_sql/render/sqlalchemy_render.py
-drwxrwxrwx   0        0        0        0 2023-12-07 12:55:37.000000 mindsdb_sql-0.8.1/mindsdb_sql.egg-info/
--rw-rw-rw-   0        0        0      535 2023-12-07 12:55:37.000000 mindsdb_sql-0.8.1/mindsdb_sql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3470 2023-12-07 12:55:37.000000 mindsdb_sql-0.8.1/mindsdb_sql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-07 12:55:37.000000 mindsdb_sql-0.8.1/mindsdb_sql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-12-07 12:55:37.000000 mindsdb_sql-0.8.1/mindsdb_sql.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-12-07 12:55:37.000000 mindsdb_sql-0.8.1/mindsdb_sql.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-07 12:55:37.000000 mindsdb_sql-0.8.1/setup.cfg
--rw-rw-rw-   0        0        0      862 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-07 12:55:37.000000 mindsdb_sql-0.8.1/sly/
--rw-rw-rw-   0        0        0      109 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/sly/__init__.py
--rw-rw-rw-   0        0        0      777 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/sly/ast.py
--rw-rw-rw-   0        0        0    16752 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/sly/lex.py
--rw-rw-rw-   0        0        0    89289 2023-12-07 12:55:09.000000 mindsdb_sql-0.8.1/sly/yacc.py
+drwxrwxrwx   0        0        0        0 2023-12-19 08:26:13.000000 mindsdb_sql-0.9.0/
+-rw-rw-rw-   0        0        0      535 2023-12-19 08:26:13.000000 mindsdb_sql-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     7227 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2023-12-19 08:26:13.000000 mindsdb_sql-0.9.0/mindsdb_sql/
+-rw-rw-rw-   0        0        0      365 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/__about__.py
+-rw-rw-rw-   0        0        0     1196 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/__init__.py
+-rw-rw-rw-   0        0        0      170 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-12-19 08:26:13.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/
+-rw-rw-rw-   0        0        0        0 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-19 08:26:13.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/
+-rw-rw-rw-   0        0        0      537 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/__init__.py
+-rw-rw-rw-   0        0        0      842 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/alter_table.py
+-rw-rw-rw-   0        0        0     1539 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/base.py
+-rw-rw-rw-   0        0        0      460 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/commit_transaction.py
+-rw-rw-rw-   0        0        0     3032 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/create.py
+-rw-rw-rw-   0        0        0      994 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/delete.py
+-rw-rw-rw-   0        0        0      942 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/describe.py
+-rw-rw-rw-   0        0        0     3056 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/drop.py
+-rw-rw-rw-   0        0        0      659 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/explain.py
+-rw-rw-rw-   0        0        0     3260 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/insert.py
+-rw-rw-rw-   0        0        0      466 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/rollback_transaction.py
+drwxrwxrwx   0        0        0        0 2023-12-19 08:26:13.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/
+-rw-rw-rw-   0        0        0      597 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/__init__.py
+-rw-rw-rw-   0        0        0     1482 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/case.py
+-rw-rw-rw-   0        0        0     1113 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/common_table_expression.py
+-rw-rw-rw-   0        0        0     1952 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/constant.py
+-rw-rw-rw-   0        0        0      503 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/data.py
+-rw-rw-rw-   0        0        0     3196 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/identifier.py
+-rw-rw-rw-   0        0        0     1381 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/join.py
+-rw-rw-rw-   0        0        0      662 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/native_query.py
+-rw-rw-rw-   0        0        0     5949 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/operation.py
+-rw-rw-rw-   0        0        0      806 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/order_by.py
+-rw-rw-rw-   0        0        0      464 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/parameter.py
+-rw-rw-rw-   0        0        0     5904 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/select.py
+-rw-rw-rw-   0        0        0      504 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/star.py
+-rw-rw-rw-   0        0        0      648 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/tuple.py
+-rw-rw-rw-   0        0        0      774 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/type_cast.py
+-rw-rw-rw-   0        0        0     1178 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/union.py
+-rw-rw-rw-   0        0        0     3296 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/set.py
+-rw-rw-rw-   0        0        0     2979 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/show.py
+-rw-rw-rw-   0        0        0      469 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/start_transaction.py
+-rw-rw-rw-   0        0        0     3154 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/update.py
+-rw-rw-rw-   0        0        0      639 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/use.py
+drwxrwxrwx   0        0        0        0 2023-12-19 08:26:13.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/
+-rw-rw-rw-   0        0        0        0 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-19 08:26:13.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/
+-rw-rw-rw-   0        0        0      999 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/__init__.py
+-rw-rw-rw-   0        0        0     3254 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/agents.py
+-rw-rw-rw-   0        0        0     2893 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/chatbot.py
+-rw-rw-rw-   0        0        0     1794 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/create_database.py
+-rw-rw-rw-   0        0        0      953 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/create_file.py
+-rw-rw-rw-   0        0        0     2383 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/create_job.py
+-rw-rw-rw-   0        0        0     1400 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py
+-rw-rw-rw-   0        0        0     6029 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py
+-rw-rw-rw-   0        0        0     1799 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/create_view.py
+-rw-rw-rw-   0        0        0      873 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py
+-rw-rw-rw-   0        0        0      882 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py
+-rw-rw-rw-   0        0        0      861 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/drop_job.py
+-rw-rw-rw-   0        0        0      877 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py
+-rw-rw-rw-   0        0        0      906 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py
+-rw-rw-rw-   0        0        0     1313 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/evaluate.py
+-rw-rw-rw-   0        0        0      223 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/finetune_predictor.py
+-rw-rw-rw-   0        0        0     3563 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/knowledge_base.py
+-rw-rw-rw-   0        0        0      356 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/latest.py
+-rw-rw-rw-   0        0        0     8673 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/lexer.py
+-rw-rw-rw-   0        0        0    53190 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/parser.py
+-rw-rw-rw-   0        0        0      311 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/retrain_predictor.py
+-rw-rw-rw-   0        0        0     3221 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/skills.py
+-rw-rw-rw-   0        0        0     2246 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/trigger.py
+drwxrwxrwx   0        0        0        0 2023-12-19 08:26:13.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mysql/
+-rw-rw-rw-   0        0        0       67 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mysql/__init__.py
+-rw-rw-rw-   0        0        0     1046 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mysql/lexer.py
+-rw-rw-rw-   0        0        0    29491 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mysql/parser.py
+-rw-rw-rw-   0        0        0      904 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mysql/show_index.py
+-rw-rw-rw-   0        0        0      686 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mysql/variable.py
+-rw-rw-rw-   0        0        0     6231 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/lexer.py
+-rw-rw-rw-   0        0        0      751 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/logger.py
+-rw-rw-rw-   0        0        0    21382 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/parser.py
+-rw-rw-rw-   0        0        0     2497 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/parser/utils.py
+drwxrwxrwx   0        0        0        0 2023-12-19 08:26:13.000000 mindsdb_sql-0.9.0/mindsdb_sql/planner/
+-rw-rw-rw-   0        0        0      150 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/planner/__init__.py
+-rw-rw-rw-   0        0        0      878 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/planner/query_plan.py
+-rw-rw-rw-   0        0        0    56561 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/planner/query_planner.py
+-rw-rw-rw-   0        0        0    21398 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/planner/query_prepare.py
+-rw-rw-rw-   0        0        0      536 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/planner/step_result.py
+-rw-rw-rw-   0        0        0     8788 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/planner/steps.py
+-rw-rw-rw-   0        0        0     2981 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/planner/ts_utils.py
+-rw-rw-rw-   0        0        0    13797 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/planner/utils.py
+drwxrwxrwx   0        0        0        0 2023-12-19 08:26:13.000000 mindsdb_sql-0.9.0/mindsdb_sql/render/
+-rw-rw-rw-   0        0        0        0 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/render/__init__.py
+-rw-rw-rw-   0        0        0    21146 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/mindsdb_sql/render/sqlalchemy_render.py
+drwxrwxrwx   0        0        0        0 2023-12-19 08:26:13.000000 mindsdb_sql-0.9.0/mindsdb_sql.egg-info/
+-rw-rw-rw-   0        0        0      535 2023-12-19 08:26:13.000000 mindsdb_sql-0.9.0/mindsdb_sql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3470 2023-12-19 08:26:13.000000 mindsdb_sql-0.9.0/mindsdb_sql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-19 08:26:13.000000 mindsdb_sql-0.9.0/mindsdb_sql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-12-19 08:26:13.000000 mindsdb_sql-0.9.0/mindsdb_sql.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-12-19 08:26:13.000000 mindsdb_sql-0.9.0/mindsdb_sql.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-12-19 08:26:13.000000 mindsdb_sql-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      862 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-12-19 08:26:13.000000 mindsdb_sql-0.9.0/sly/
+-rw-rw-rw-   0        0        0      109 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/sly/__init__.py
+-rw-rw-rw-   0        0        0      777 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/sly/ast.py
+-rw-rw-rw-   0        0        0    16752 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/sly/lex.py
+-rw-rw-rw-   0        0        0    89289 2023-12-19 08:25:55.000000 mindsdb_sql-0.9.0/sly/yacc.py
```

### Comparing `mindsdb_sql-0.8.1/PKG-INFO` & `mindsdb_sql-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mindsdb_sql
-Version: 0.8.1
+Version: 0.9.0
 Summary: Pure python SQL parser
 Home-page: https://github.com/mindsdb/mindsdb_sql
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb_sql
 Description: UNKNOWN
```

### Comparing `mindsdb_sql-0.8.1/README.md` & `mindsdb_sql-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/__init__.py` & `mindsdb_sql-0.9.0/mindsdb_sql/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/__init__.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/alter_table.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/alter_table.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/base.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/base.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/create.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/create.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/delete.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/delete.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/describe.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/describe.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/drop.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/drop.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/explain.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/explain.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/insert.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/insert.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/__init__.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/case.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/case.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/common_table_expression.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/common_table_expression.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/constant.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/constant.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/identifier.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/identifier.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/join.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/join.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/native_query.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/native_query.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/operation.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/operation.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/order_by.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/order_by.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/select.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/select.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/tuple.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/tuple.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/type_cast.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/type_cast.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/select/union.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/select/union.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/set.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/set.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/show.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/show.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/update.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/update.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/ast/use.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/ast/use.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/__init__.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/__init__.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/agents.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/agents.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/chatbot.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/chatbot.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/create_database.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/create_database.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/create_file.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/create_file.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/create_job.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/create_job.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/create_ml_engine.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/create_predictor.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/create_view.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/create_view.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/drop_dataset.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/drop_datasource.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/drop_job.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/drop_job.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/drop_ml_engine.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/drop_predictor.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/evaluate.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/evaluate.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/knowledge_base.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/knowledge_base.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/lexer.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/lexer.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/parser.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/parser.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/skills.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/skills.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mindsdb/trigger.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mindsdb/trigger.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mysql/lexer.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mysql/lexer.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mysql/parser.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mysql/parser.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mysql/show_index.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mysql/show_index.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/dialects/mysql/variable.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/dialects/mysql/variable.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/lexer.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/lexer.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/logger.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/logger.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/parser.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/parser.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/parser/utils.py` & `mindsdb_sql-0.9.0/mindsdb_sql/parser/utils.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/planner/query_plan.py` & `mindsdb_sql-0.9.0/mindsdb_sql/planner/query_plan.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/planner/query_planner.py` & `mindsdb_sql-0.9.0/mindsdb_sql/planner/query_planner.py`

 * *Files 2% similar despite different names*

```diff
@@ -572,23 +572,41 @@
                                         where=preparation_where,
                                         modifiers=query_modifiers,
                                         order_by=order_by,
                                         limit=Constant(predictor_window),
                                         )
             integration_select.where = find_and_remove_time_filter(integration_select.where, time_filter)
             integration_selects = [integration_select]
-        elif isinstance(time_filter, BinaryOperation) and time_filter.op == '=' and time_filter.args[1] == Latest():
+        elif isinstance(time_filter, BinaryOperation) and time_filter.op == '=':
             integration_select = Select(targets=[Star()],
                                         from_table=table,
                                         where=preparation_where,
                                         modifiers=query_modifiers,
                                         order_by=order_by,
                                         limit=Constant(predictor_window),
                                         )
-            integration_select.where = find_and_remove_time_filter(integration_select.where, time_filter)
+
+            if type(time_filter.args[1]) is Latest:
+                integration_select.where = find_and_remove_time_filter(integration_select.where, time_filter)
+            else:
+                time_filter_date = time_filter.args[1]
+                preparation_time_filter = BinaryOperation(
+                    '<=',
+                    args=[
+                        Identifier(predictor_time_column_name),
+                        time_filter_date
+                    ]
+                )
+                integration_select.where = add_order_not_null(
+                    replace_time_filter(
+                        preparation_where2, time_filter, preparation_time_filter
+                    )
+                )
+                time_filter.op = '>'
+
             integration_selects = [integration_select]
         elif isinstance(time_filter, BinaryOperation) and time_filter.op in ('>', '>='):
             time_filter_date = time_filter.args[1]
             preparation_time_filter_op = {'>': '<=', '>=': '<'}[time_filter.op]
 
             preparation_time_filter = BinaryOperation(preparation_time_filter_op, args=[Identifier(predictor_time_column_name), time_filter_date])
             preparation_where2 = replace_time_filter(preparation_where2, time_filter, preparation_time_filter)
```

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/planner/query_prepare.py` & `mindsdb_sql-0.9.0/mindsdb_sql/planner/query_prepare.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/planner/step_result.py` & `mindsdb_sql-0.9.0/mindsdb_sql/planner/step_result.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/planner/steps.py` & `mindsdb_sql-0.9.0/mindsdb_sql/planner/steps.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/planner/ts_utils.py` & `mindsdb_sql-0.9.0/mindsdb_sql/planner/ts_utils.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/planner/utils.py` & `mindsdb_sql-0.9.0/mindsdb_sql/planner/utils.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql/render/sqlalchemy_render.py` & `mindsdb_sql-0.9.0/mindsdb_sql/render/sqlalchemy_render.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql.egg-info/PKG-INFO` & `mindsdb_sql-0.9.0/mindsdb_sql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: mindsdb-sql
-Version: 0.8.1
+Version: 0.9.0
 Summary: Pure python SQL parser
 Home-page: https://github.com/mindsdb/mindsdb_sql
 Author: MindsDB Inc
 Author-email: jorge@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/mindsdb_sql
 Description: UNKNOWN
```

### Comparing `mindsdb_sql-0.8.1/mindsdb_sql.egg-info/SOURCES.txt` & `mindsdb_sql-0.9.0/mindsdb_sql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/setup.py` & `mindsdb_sql-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/sly/ast.py` & `mindsdb_sql-0.9.0/sly/ast.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/sly/lex.py` & `mindsdb_sql-0.9.0/sly/lex.py`

 * *Files identical despite different names*

### Comparing `mindsdb_sql-0.8.1/sly/yacc.py` & `mindsdb_sql-0.9.0/sly/yacc.py`

 * *Files identical despite different names*

