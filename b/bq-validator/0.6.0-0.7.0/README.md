# Comparing `tmp/bq_validator-0.6.0.tar.gz` & `tmp/bq_validator-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bq_validator-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "bq_validator-0.7.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `bq_validator-0.6.0.tar` & `bq_validator-0.7.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0      804 2023-06-27 01:35:06.444168 bq_validator-0.6.0/.github/CODEOWNERS
--rw-r--r--   0        0        0      981 2023-06-27 01:35:06.444168 bq_validator-0.6.0/.github/workflows/publish.yml
--rw-r--r--   0        0        0      986 2023-06-27 01:35:06.448168 bq_validator-0.6.0/.github/workflows/test-publish.yml
--rw-r--r--   0        0        0      980 2023-06-27 01:35:06.448168 bq_validator-0.6.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1799 2023-06-27 01:35:06.448168 bq_validator-0.6.0/.gitignore
--rw-r--r--   0        0        0      648 2023-06-27 01:35:06.448168 bq_validator-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0    13990 2023-06-27 01:35:06.448168 bq_validator-0.6.0/.pylintrc
--rw-r--r--   0        0        0      150 2023-06-27 01:35:06.448168 bq_validator-0.6.0/.pypirc
--rw-r--r--   0        0        0       32 2023-06-27 01:35:06.448168 bq_validator-0.6.0/.style.yapf
--rw-r--r--   0        0        0    11357 2023-06-27 01:35:06.448168 bq_validator-0.6.0/LICENSE
--rw-r--r--   0        0        0      100 2023-06-27 01:35:06.448168 bq_validator-0.6.0/MANIFEST.in
--rw-r--r--   0        0        0      967 2023-06-27 01:35:06.448168 bq_validator-0.6.0/Makefile
--rw-r--r--   0        0        0     1788 2023-06-27 01:35:06.448168 bq_validator-0.6.0/README.md
--rw-r--r--   0        0        0      890 2023-06-27 01:35:06.448168 bq_validator-0.6.0/bq_validator/__init__.py
--rw-r--r--   0        0        0     4456 2023-06-27 01:35:06.448168 bq_validator-0.6.0/bq_validator/bigquery.py
--rw-r--r--   0        0        0     2891 2023-06-27 01:35:06.448168 bq_validator-0.6.0/bq_validator/cli.py
--rw-r--r--   0        0        0     1444 2023-06-27 01:35:06.448168 bq_validator-0.6.0/bq_validator/utils.py
--rwxr-xr-x   0        0        0     1121 2023-06-27 01:35:06.448168 bq_validator-0.6.0/dev/clean.sh
--rwxr-xr-x   0        0        0     1013 2023-06-27 01:35:06.448168 bq_validator-0.6.0/dev/format_python.sh
--rw-r--r--   0        0        0      970 2023-06-27 01:35:06.448168 bq_validator-0.6.0/dev/lint_python.sh
--rwxr-xr-x   0        0        0     1394 2023-06-27 01:35:06.448168 bq_validator-0.6.0/dev/publish.sh
--rwxr-xr-x   0        0        0     1023 2023-06-27 01:35:06.448168 bq_validator-0.6.0/dev/setup.sh
--rw-r--r--   0        0        0      921 2023-06-27 01:35:06.448168 bq_validator-0.6.0/dev/test_entry_point.sh
--rwxr-xr-x   0        0        0      958 2023-06-27 01:35:06.448168 bq_validator-0.6.0/dev/test_python.sh
--rw-r--r--   0        0        0    14273 2023-06-27 01:35:06.448168 bq_validator-0.6.0/pylintrc
--rw-r--r--   0        0        0     2002 2023-06-27 01:35:06.448168 bq_validator-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      830 2023-06-27 01:35:06.448168 bq_validator-0.6.0/setup.py
--rw-r--r--   0        0        0      792 2023-06-27 01:35:06.448168 bq_validator-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0     1160 2023-06-27 01:35:06.448168 bq_validator-0.6.0/tests/resources/target/compiled/jaffle_shop/models/orders.sql
--rw-r--r--   0        0        0      218 2023-06-27 01:35:06.448168 bq_validator-0.6.0/tests/resources/target/compiled/jaffle_shop/models/staging/stg_customers.sql
--rw-r--r--   0        0        0      241 2023-06-27 01:35:06.448168 bq_validator-0.6.0/tests/resources/target/compiled/jaffle_shop/models/staging/stg_orders.sql
--rw-r--r--   0        0        0      330 2023-06-27 01:35:06.448168 bq_validator-0.6.0/tests/resources/target/compiled/jaffle_shop/models/staging/stg_payments.sql
--rw-r--r--   0        0        0      167 2023-06-27 01:35:06.448168 bq_validator-0.6.0/tests/resources/target/compiled/jaffle_shop/models/test_insert_overwrite.sql
--rw-r--r--   0        0        0      167 2023-06-27 01:35:06.448168 bq_validator-0.6.0/tests/resources/target/compiled/jaffle_shop/models/test_merge.sql
--rw-r--r--   0        0        0     1442 2023-06-27 01:35:06.448168 bq_validator-0.6.0/tests/test_utils.py
--rw-r--r--   0        0        0     3581 1970-01-01 00:00:00.000000 bq_validator-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0      804 2024-05-02 00:44:13.999086 bq_validator-0.7.0/.github/CODEOWNERS
+-rw-r--r--   0        0        0      981 2024-05-02 00:44:13.999086 bq_validator-0.7.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      986 2024-05-02 00:44:13.999086 bq_validator-0.7.0/.github/workflows/test-publish.yml
+-rw-r--r--   0        0        0      980 2024-05-02 00:44:13.999086 bq_validator-0.7.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1799 2024-05-02 00:44:13.999086 bq_validator-0.7.0/.gitignore
+-rw-r--r--   0        0        0      648 2024-05-02 00:44:13.999086 bq_validator-0.7.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    13990 2024-05-02 00:44:13.999086 bq_validator-0.7.0/.pylintrc
+-rw-r--r--   0        0        0      150 2024-05-02 00:44:13.999086 bq_validator-0.7.0/.pypirc
+-rw-r--r--   0        0        0       32 2024-05-02 00:44:13.999086 bq_validator-0.7.0/.style.yapf
+-rw-r--r--   0        0        0    11357 2024-05-02 00:44:13.999086 bq_validator-0.7.0/LICENSE
+-rw-r--r--   0        0        0      100 2024-05-02 00:44:13.999086 bq_validator-0.7.0/MANIFEST.in
+-rw-r--r--   0        0        0      967 2024-05-02 00:44:13.999086 bq_validator-0.7.0/Makefile
+-rw-r--r--   0        0        0     1788 2024-05-02 00:44:13.999086 bq_validator-0.7.0/README.md
+-rw-r--r--   0        0        0      890 2024-05-02 00:44:13.999086 bq_validator-0.7.0/bq_validator/__init__.py
+-rw-r--r--   0        0        0     4456 2024-05-02 00:44:13.999086 bq_validator-0.7.0/bq_validator/bigquery.py
+-rw-r--r--   0        0        0     3716 2024-05-02 00:44:13.999086 bq_validator-0.7.0/bq_validator/cli.py
+-rw-r--r--   0        0        0     1444 2024-05-02 00:44:13.999086 bq_validator-0.7.0/bq_validator/utils.py
+-rwxr-xr-x   0        0        0     1121 2024-05-02 00:44:13.999086 bq_validator-0.7.0/dev/clean.sh
+-rwxr-xr-x   0        0        0     1013 2024-05-02 00:44:13.999086 bq_validator-0.7.0/dev/format_python.sh
+-rw-r--r--   0        0        0      970 2024-05-02 00:44:13.999086 bq_validator-0.7.0/dev/lint_python.sh
+-rwxr-xr-x   0        0        0     1394 2024-05-02 00:44:13.999086 bq_validator-0.7.0/dev/publish.sh
+-rwxr-xr-x   0        0        0     1023 2024-05-02 00:44:13.999086 bq_validator-0.7.0/dev/setup.sh
+-rw-r--r--   0        0        0      921 2024-05-02 00:44:13.999086 bq_validator-0.7.0/dev/test_entry_point.sh
+-rwxr-xr-x   0        0        0      958 2024-05-02 00:44:13.999086 bq_validator-0.7.0/dev/test_python.sh
+-rw-r--r--   0        0        0    14273 2024-05-02 00:44:14.003085 bq_validator-0.7.0/pylintrc
+-rw-r--r--   0        0        0     2002 2024-05-02 00:44:14.003085 bq_validator-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      830 2024-05-02 00:44:14.003085 bq_validator-0.7.0/setup.py
+-rw-r--r--   0        0        0      792 2024-05-02 00:44:14.003085 bq_validator-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0     1160 2024-05-02 00:44:14.003085 bq_validator-0.7.0/tests/resources/target/compiled/jaffle_shop/models/orders.sql
+-rw-r--r--   0        0        0      218 2024-05-02 00:44:14.003085 bq_validator-0.7.0/tests/resources/target/compiled/jaffle_shop/models/staging/stg_customers.sql
+-rw-r--r--   0        0        0      241 2024-05-02 00:44:14.003085 bq_validator-0.7.0/tests/resources/target/compiled/jaffle_shop/models/staging/stg_orders.sql
+-rw-r--r--   0        0        0      330 2024-05-02 00:44:14.003085 bq_validator-0.7.0/tests/resources/target/compiled/jaffle_shop/models/staging/stg_payments.sql
+-rw-r--r--   0        0        0      167 2024-05-02 00:44:14.003085 bq_validator-0.7.0/tests/resources/target/compiled/jaffle_shop/models/test_insert_overwrite.sql
+-rw-r--r--   0        0        0      167 2024-05-02 00:44:14.003085 bq_validator-0.7.0/tests/resources/target/compiled/jaffle_shop/models/test_merge.sql
+-rw-r--r--   0        0        0     1442 2024-05-02 00:44:14.003085 bq_validator-0.7.0/tests/test_utils.py
+-rw-r--r--   0        0        0     3581 1970-01-01 00:00:00.000000 bq_validator-0.7.0/PKG-INFO
```

### Comparing `bq_validator-0.6.0/.github/CODEOWNERS` & `bq_validator-0.7.0/.github/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `bq_validator-0.6.0/.github/workflows/publish.yml` & `bq_validator-0.7.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `bq_validator-0.6.0/.github/workflows/test-publish.yml` & `bq_validator-0.7.0/.github/workflows/test-publish.yml`

 * *Files identical despite different names*

### Comparing `bq_validator-0.6.0/.github/workflows/test.yml` & `bq_validator-0.7.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `bq_validator-0.6.0/.gitignore` & `bq_validator-0.7.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bq_validator-0.6.0/.pre-commit-config.yaml` & `bq_validator-0.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bq_validator-0.6.0/.pylintrc` & `bq_validator-0.7.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `bq_validator-0.6.0/LICENSE` & `bq_validator-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bq_validator-0.6.0/Makefile` & `bq_validator-0.7.0/Makefile`

 * *Files identical despite different names*

### Comparing `bq_validator-0.6.0/README.md` & `bq_validator-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `bq_validator-0.6.0/bq_validator/__init__.py` & `bq_validator-0.7.0/bq_validator/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 """
 The `bq-validator` command enables us to validate BigQuery queries.
 """
-__version__ = "0.6.0"
+__version__ = "0.7.0"
```

### Comparing `bq_validator-0.6.0/bq_validator/bigquery.py` & `bq_validator-0.7.0/bq_validator/bigquery.py`

 * *Files identical despite different names*

### Comparing `bq_validator-0.6.0/bq_validator/cli.py` & `bq_validator-0.7.0/bq_validator/cli.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,70 +8,98 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
+import concurrent.futures
 import json
-import sys
 from typing import Optional
 
 import click
 import click_completion
 
 import bq_validator
 from bq_validator.bigquery import create_bigquery_client, validate_query
 from bq_validator.utils import get_sql_files, read_file
 
 # Initialize click-completion
 click_completion.init()
 
 
 @click.command()
-@click.argument('path', type=click.Path(exists=True))
-@click.option("--quota_project",
-              type=str,
-              required=False,
-              help="BigQuery client project ID")
-@click.option("--client_project",
-              type=str,
-              required=False,
-              help="BigQuery client project ID")
-@click.option("--client_location",
-              type=str,
-              required=False,
-              help="BigQuery client location")
-@click.option("--impersonate_service_account",
-              type=str,
-              required=False,
-              help="Impersonate service account email")
+@click.argument("path", type=click.Path(exists=True))
+@click.option(
+    "--quota_project", type=str, required=False, help="BigQuery client project ID"
+)
+@click.option(
+    "--client_project", type=str, required=False, help="BigQuery client project ID"
+)
+@click.option(
+    "--client_location", type=str, required=False, help="BigQuery client location"
+)
+@click.option(
+    "--impersonate_service_account",
+    type=str,
+    required=False,
+    help="Impersonate service account email",
+)
+@click.option(
+    "--num_parallels",
+    type=int,
+    required=False,
+    default=1,
+    help="Number of parallel query validations",
+)
+@click.option("--verbose", is_flag=True, help="Enable verbose output")
 @click.version_option(version=bq_validator.__version__)
-def main(path: str, quota_project: Optional[str], client_project: Optional[str],
-         client_location: Optional[str],
-         impersonate_service_account: Optional[str]):
+def main(
+    path: str,
+    quota_project: Optional[str],
+    client_project: Optional[str],
+    client_location: Optional[str],
+    impersonate_service_account: Optional[str],
+    num_parallels: Optional[int] = 1,
+    verbose: Optional[bool] = False,
+):
     """Validate BigQuery queries
 
     PATH is either of a SQL file path or a directory.
     When it is a directory, the command recursively validates all SQL files in the directory.
     """
     # Create a BigQuery client
     client = create_bigquery_client(
         client_project_id=client_project,
         quota_project_id=quota_project,
         location=client_location,
-        impersonate_service_account=impersonate_service_account)
-    # Validate queries
+        impersonate_service_account=impersonate_service_account,
+    )
+    # Validate queries in parallel
     sql_files = get_sql_files(path=path)
     errors = {}
-    for query_file in sql_files:
-        query = read_file(path=query_file)
-        is_valid, error_message = validate_query(client=client, query=query)
-        if is_valid is False:
-            errors[query_file] = {
-                "query": query,
-                "error": error_message,
-            }
+    with concurrent.futures.ThreadPoolExecutor(max_workers=num_parallels) as executor:
+        futures = {
+            executor.submit(validate_and_collect_errors, client, sql_files, verbose)
+            for sql_files in sql_files
+        }
+        for future in concurrent.futures.as_completed(futures):
+            result = future.result()
+            if result:
+                query_file, error_details = result
+                errors[query_file] = error_details
     # Show errors
     if len(errors) > 0:
         click.echo(json.dumps(errors, indent=2))
-        sys.exit(1)
+
+
+def validate_and_collect_errors(client, query_file, verbose: Optional[bool] = False):
+    """Validate a query and collect errors if any"""
+    if verbose:
+        click.echo(f"Validating {query_file}")
+    query = read_file(path=query_file)
+    is_valid, error_message = validate_query(client=client, query=query)
+    if not is_valid:
+        if verbose:
+            click.echo(f"Error: {error_message}")
+        return query_file, {"query": query, "error": error_message}
+    return None
```

### Comparing `bq_validator-0.6.0/bq_validator/utils.py` & `bq_validator-0.7.0/bq_validator/utils.py`

 * *Files identical despite different names*

### Comparing `bq_validator-0.6.0/dev/clean.sh` & `bq_validator-0.7.0/dev/clean.sh`

 * *Files identical despite different names*

### Comparing `bq_validator-0.6.0/dev/format_python.sh` & `bq_validator-0.7.0/dev/format_python.sh`

 * *Files identical despite different names*

### Comparing `bq_validator-0.6.0/dev/lint_python.sh` & `bq_validator-0.7.0/dev/lint_python.sh`

 * *Files identical despite different names*

### Comparing `bq_validator-0.6.0/dev/publish.sh` & `bq_validator-0.7.0/dev/publish.sh`

 * *Files identical despite different names*

### Comparing `bq_validator-0.6.0/dev/setup.sh` & `bq_validator-0.7.0/dev/setup.sh`

 * *Files identical despite different names*

### Comparing `bq_validator-0.6.0/dev/test_entry_point.sh` & `bq_validator-0.7.0/dev/test_entry_point.sh`

 * *Files identical despite different names*

### Comparing `bq_validator-0.6.0/dev/test_python.sh` & `bq_validator-0.7.0/dev/test_python.sh`

 * *Files identical despite different names*

### Comparing `bq_validator-0.6.0/pylintrc` & `bq_validator-0.7.0/pylintrc`

 * *Files identical despite different names*

### Comparing `bq_validator-0.6.0/pyproject.toml` & `bq_validator-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bq_validator-0.6.0/setup.py` & `bq_validator-0.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `bq_validator-0.6.0/tests/__init__.py` & `bq_validator-0.7.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `bq_validator-0.6.0/tests/resources/target/compiled/jaffle_shop/models/orders.sql` & `bq_validator-0.7.0/tests/resources/target/compiled/jaffle_shop/models/orders.sql`

 * *Files identical despite different names*

### Comparing `bq_validator-0.6.0/tests/test_utils.py` & `bq_validator-0.7.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `bq_validator-0.6.0/PKG-INFO` & `bq_validator-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bq-validator
-Version: 0.6.0
+Version: 0.7.0
 Summary: The `bq-validator` command enables us to validate BigQuery queries.
 Author: yu-iskw
 Requires-Python: >=3.6.1
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: bq-validator Version: 0.6.0 Summary: The `bq-
+Metadata-Version: 2.1 Name: bq-validator Version: 0.7.0 Summary: The `bq-
 validator` command enables us to validate BigQuery queries. Author: yu-iskw
 Requires-Python: >=3.6.1 Description-Content-Type: text/markdown Classifier:
 Intended Audience :: Information Technology Classifier: Intended Audience ::
 System Administrators Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

