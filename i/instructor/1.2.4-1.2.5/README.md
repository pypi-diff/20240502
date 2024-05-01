# Comparing `tmp/instructor-1.2.4.tar.gz` & `tmp/instructor-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "instructor-1.2.4.tar", max compression
+gzip compressed data, was "instructor-1.2.5.tar", max compression
```

## Comparing `instructor-1.2.4.tar` & `instructor-1.2.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     1066 2024-04-29 18:30:51.796761 instructor-1.2.4/LICENSE
--rw-r--r--   0        0        0     9716 2024-04-29 18:30:51.796761 instructor-1.2.4/README.md
--rw-r--r--   0        0        0     1445 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/__init__.py
--rw-r--r--   0        0        0        0 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/_types/__init__.py
--rw-r--r--   0        0        0      654 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/_types/_alias.py
--rw-r--r--   0        0        0        0 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/cli/__init__.py
--rw-r--r--   0        0        0      807 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/cli/cli.py
--rw-r--r--   0        0        0     3792 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/cli/files.py
--rw-r--r--   0        0        0     5348 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/cli/hub.py
--rw-r--r--   0        0        0     8255 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/cli/jobs.py
--rw-r--r--   0        0        0     6476 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/cli/usage.py
--rw-r--r--   0        0        0    10324 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/client.py
--rw-r--r--   0        0        0     2453 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/client_anthropic.py
--rw-r--r--   0        0        0     2348 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/client_cohere.py
--rw-r--r--   0        0        0     1379 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/client_groq.py
--rw-r--r--   0        0        0     1709 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/client_mistral.py
--rw-r--r--   0        0        0     8968 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/distil.py
--rw-r--r--   0        0        0      424 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/dsl/__init__.py
--rw-r--r--   0        0        0     2985 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/dsl/citation.py
--rw-r--r--   0        0        0     7929 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/dsl/iterable.py
--rw-r--r--   0        0        0     2165 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/dsl/maybe.py
--rw-r--r--   0        0        0     2580 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/dsl/parallel.py
--rw-r--r--   0        0        0    11052 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/dsl/partial.py
--rw-r--r--   0        0        0     1733 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/dsl/simple_type.py
--rw-r--r--   0        0        0     4381 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/dsl/validators.py
--rw-r--r--   0        0        0      346 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/exceptions.py
--rw-r--r--   0        0        0     8020 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/function_calls.py
--rw-r--r--   0        0        0      852 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/mode.py
--rw-r--r--   0        0        0     4989 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/patch.py
--rw-r--r--   0        0        0    13509 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/process_response.py
--rw-r--r--   0        0        0        1 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/py.typed
--rw-r--r--   0        0        0     9532 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/retry.py
--rw-r--r--   0        0        0     5505 2024-04-29 18:30:51.864761 instructor-1.2.4/instructor/utils.py
--rw-r--r--   0        0        0     2364 2024-04-29 18:30:51.868761 instructor-1.2.4/pyproject.toml
--rw-r--r--   0        0        0    11658 1970-01-01 00:00:00.000000 instructor-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-05-01 22:11:43.174889 instructor-1.2.5/LICENSE
+-rw-r--r--   0        0        0     9716 2024-05-01 22:11:43.174889 instructor-1.2.5/README.md
+-rw-r--r--   0        0        0     1450 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/_types/__init__.py
+-rw-r--r--   0        0        0      654 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/_types/_alias.py
+-rw-r--r--   0        0        0        0 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/cli/__init__.py
+-rw-r--r--   0        0        0      807 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/cli/cli.py
+-rw-r--r--   0        0        0     3865 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/cli/files.py
+-rw-r--r--   0        0        0     5441 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/cli/hub.py
+-rw-r--r--   0        0        0     8314 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/cli/jobs.py
+-rw-r--r--   0        0        0     6441 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/cli/usage.py
+-rw-r--r--   0        0        0    13256 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/client.py
+-rw-r--r--   0        0        0     2573 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/client_anthropic.py
+-rw-r--r--   0        0        0     2419 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/client_cohere.py
+-rw-r--r--   0        0        0     1391 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/client_groq.py
+-rw-r--r--   0        0        0     1727 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/client_mistral.py
+-rw-r--r--   0        0        0     9579 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/distil.py
+-rw-r--r--   0        0        0      424 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/dsl/__init__.py
+-rw-r--r--   0        0        0     2927 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/dsl/citation.py
+-rw-r--r--   0        0        0     8079 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/dsl/iterable.py
+-rw-r--r--   0        0        0     2169 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/dsl/maybe.py
+-rw-r--r--   0        0        0     2562 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/dsl/parallel.py
+-rw-r--r--   0        0        0    10922 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/dsl/partial.py
+-rw-r--r--   0        0        0     1879 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/dsl/simple_type.py
+-rw-r--r--   0        0        0     4360 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/dsl/validators.py
+-rw-r--r--   0        0        0      346 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/exceptions.py
+-rw-r--r--   0        0        0     8724 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/function_calls.py
+-rw-r--r--   0        0        0      852 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/mode.py
+-rw-r--r--   0        0        0     4969 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/patch.py
+-rw-r--r--   0        0        0    13501 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/process_response.py
+-rw-r--r--   0        0        0        1 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/py.typed
+-rw-r--r--   0        0        0     9502 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/retry.py
+-rw-r--r--   0        0        0     6668 2024-05-01 22:11:43.246888 instructor-1.2.5/instructor/utils.py
+-rw-r--r--   0        0        0     2799 2024-05-01 22:11:43.246888 instructor-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0    11713 1970-01-01 00:00:00.000000 instructor-1.2.5/PKG-INFO
```

### Comparing `instructor-1.2.4/LICENSE` & `instructor-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `instructor-1.2.4/README.md` & `instructor-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `instructor-1.2.4/instructor/__init__.py` & `instructor-1.2.5/instructor/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import importlib
+import importlib.util
 
 from .mode import Mode
 from .process_response import handle_response_model
 from .distil import FinetuneFormat, Instructions
 from .dsl import (
     CitationMixin,
     Maybe,
```

### Comparing `instructor-1.2.4/instructor/_types/_alias.py` & `instructor-1.2.5/instructor/_types/_alias.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.4/instructor/cli/cli.py` & `instructor-1.2.5/instructor/cli/cli.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.4/instructor/cli/files.py` & `instructor-1.2.5/instructor/cli/files.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
+# type: ignore - stub mismatched
+
 import time
 from datetime import datetime
-from typing import List
+from typing import Literal, cast
 
 import openai
 import typer
 from openai import OpenAI
 from rich.console import Console
 from rich.table import Table
 
 client = OpenAI()
 app = typer.Typer()
 console = Console()
 
 
 # Sample response data
-def generate_file_table(files: List[openai.types.FileObject]) -> Table:
+def generate_file_table(files: list[openai.types.FileObject]) -> Table:
     table = Table(
         title="OpenAI Files",
     )
     table.add_column("File ID", style="dim")
     table.add_column("Size (bytes)", justify="right")
     table.add_column("Creation Time")
     table.add_column("Filename")
@@ -32,88 +34,90 @@
             file["filename"],
             file["purpose"],
         )
 
     return table
 
 
-def get_files() -> List[openai.types.FileObject]:
+def get_files() -> list[openai.types.FileObject]:
     files = client.files.list()
     files = files.data
     files = sorted(files, key=lambda x: x.created_at, reverse=True)
     return files
 
 
 def get_file_status(file_id: str) -> str:
     response = client.files.retrieve(file_id)
     return response.status
 
 
 @app.command(
     help="Upload a file to OpenAI's servers, will monitor the upload status until it is processed",
-)  # type: ignore[misc]
+)
 def upload(
-    filepath: str = typer.Argument(..., help="Path to the file to upload"),
+    filepath: str = typer.Argument(help="Path to the file to upload"),
     purpose: str = typer.Option("fine-tune", help="Purpose of the file"),
     poll: int = typer.Option(5, help="Polling interval in seconds"),
 ) -> None:
+    # Literals aren't supported by Typer yet.
+    file_purpose = cast(Literal["fine-tune", "assistants"], purpose)
     with open(filepath, "rb") as file:
-        response = client.files.create(file=file, purpose=purpose)
-    file_id = response["id"]
+        response = client.files.create(file=file, purpose=file_purpose)
+    file_id = response["id"]  # type: ignore - types might be out of date
     with console.status(f"Monitoring upload: {file_id}...") as status:
         status.spinner_style = "dots"
         while True:
             file_status = get_file_status(file_id)
             if file_status == "processed":
                 console.log(f"[bold green]File {file_id} uploaded successfully!")
                 break
             time.sleep(poll)
 
 
 @app.command(
     help="Download a file from OpenAI's servers",
-)  # type: ignore[misc]
+)
 def download(
-    file_id: str = typer.Argument(..., help="ID of the file to download"),
-    output: str = typer.Argument(..., help="Output path for the downloaded file"),
+    file_id: str = typer.Argument(help="ID of the file to download"),
+    output: str = typer.Argument(help="Output path for the downloaded file"),
 ) -> None:
     with console.status(f"[bold green]Downloading file {file_id}...", spinner="dots"):
         content = client.files.download(file_id)
         with open(output, "wb") as file:
             file.write(content)
         console.log(f"[bold green]File {file_id} downloaded successfully!")
 
 
 @app.command(
     help="Delete a file from OpenAI's servers",
-)  # type: ignore[misc]
-def delete(file_id: str = typer.Argument(..., help="ID of the file to delete")) -> None:
+)
+def delete(file_id: str = typer.Argument(help="ID of the file to delete")) -> None:
     with console.status(f"[bold red]Deleting file {file_id}...", spinner="dots"):
         try:
             client.files.delete(file_id)
             console.log(f"[bold red]File {file_id} deleted successfully!")
         except Exception as e:
             console.log(f"[bold red]Error deleting file {file_id}: {e}")
             return
 
 
 @app.command(
     help="Monitor the status of a file on OpenAI's servers",
-)  # type: ignore[misc]
+)
 def status(
-    file_id: str = typer.Argument(..., help="ID of the file to check the status of"),
+    file_id: str = typer.Argument(help="ID of the file to check the status of"),
 ) -> None:
     with console.status(f"Monitoring status of file {file_id}...") as status:
         while True:
             file_status = get_file_status(file_id)
             status.update(f"File status: {file_status}")
             if file_status in ["pending", "processed"]:
                 break
             time.sleep(5)
 
 
 @app.command(
     help="List the files on OpenAI's servers",
-)  # type: ignore[misc]
+)
 def list() -> None:
     files = get_files()
     console.log(generate_file_table(files))
```

### Comparing `instructor-1.2.4/instructor/cli/hub.py` & `instructor-1.2.5/instructor/cli/hub.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,38 +54,38 @@
             pages = [HubPage(**page) for page in response.json()]
             if sort:
                 return sorted(pages, key=lambda x: x.count, reverse=True)
             return pages
         else:
             raise Exception(f"Failed to fetch cookbooks: {response.status_code}")
 
-    def get_content_markdown(self, branch, slug):
+    def get_content_markdown(self, branch: str, slug: str) -> str:
         """Get markdown content."""
         url = f"{self.base_url}/api/{branch}/items/{slug}/md/"
         response = httpx.get(url)
         if response.status_code == 200:
             return response.text
         else:
             raise Exception(f"Failed to fetch markdown content: {response.status_code}")
 
-    def get_content_python(self, branch, slug):
+    def get_content_python(self, branch: str, slug: str) -> str:
         """Get Python code blocks from content."""
         url = f"{self.base_url}/api/{branch}/items/{slug}/py/"
         response = httpx.get(url)
         if response.status_code == 200:
             return response.text
         else:
             raise Exception(f"Failed to fetch Python content: {response.status_code}")
 
-    def get_cookbook_id(self, id: int, branch: str = "main") -> HubPage:
+    def get_cookbook_id(self, id: int, branch: str = "main") -> Optional[HubPage]:
         for cookbook in self.get_cookbooks(branch):
             if cookbook.id == id:
                 return cookbook
 
-    def get_cookbook_slug(self, slug: str, branch: str = "main") -> HubPage:
+    def get_cookbook_slug(self, slug: str, branch: str = "main") -> Optional[HubPage]:
         for cookbook in self.get_cookbooks(branch):
             if cookbook.slug == slug:
                 return cookbook
 
 
 @app.command(
     "list",
@@ -151,15 +151,15 @@
         client.get_content_python(branch, cookbook.slug)
         if py
         else Markdown(client.get_content_markdown(branch, cookbook.slug))
     )
 
     if file:
         with open(file, "w") as f:
-            f.write(output)
+            f.write(output)  # type: ignore - markdown is writable
             return
 
     if page:
         with console.pager(styles=True):
             console.print(output)
     elif py:
         print(output)
```

### Comparing `instructor-1.2.4/instructor/cli/jobs.py` & `instructor-1.2.5/instructor/cli/jobs.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,33 @@
-from typing import Dict, List, Union
+from typing import Optional, TypedDict
 from openai import OpenAI
 
+from openai.types.fine_tuning.job_create_params import Hyperparameters
 import typer
 import time
 from rich.live import Live
 from rich.table import Table
 from rich.console import Console
 from datetime import datetime
-from typing import cast
 from openai.types.fine_tuning import FineTuningJob
 
 client = OpenAI()
 app = typer.Typer()
 console = Console()
 
 
-def generate_table(jobs: List[FineTuningJob]) -> Table:
+class FuneTuningParams(TypedDict, total=False):
+    hyperparameters: Hyperparameters
+    validation_file: Optional[str]
+    suffix: Optional[str]
+
+
+def generate_table(jobs: list[FineTuningJob]) -> Table:
     # Sorting the jobs by creation time
-    jobs = sorted(jobs, key=lambda x: (cast(FineTuningJob, x)).created_at, reverse=True)
-    jobs = cast(List[FineTuningJob], jobs)
+    jobs = sorted(jobs, key=lambda x: x.created_at, reverse=True)
 
     table = Table(
         title="OpenAI Fine Tuning Job Monitoring",
         caption="Automatically refreshes every 5 seconds, press Ctrl+C to exit",
     )
 
     table.add_column("Job ID", style="dim")
@@ -62,27 +67,27 @@
 
 def status_color(status: str) -> str:
     return {"running": "yellow", "succeeded": "green", "failed": "red"}.get(
         status, "white"
     )
 
 
-def get_jobs(limit: int = 5) -> List[FineTuningJob]:
+def get_jobs(limit: int = 5) -> list[FineTuningJob]:
     return client.fine_tuning.jobs.list(limit=limit).data
 
 
 def get_file_status(file_id: str) -> str:
     response = client.files.retrieve(file_id)
     return response.status
 
 
 @app.command(
     name="list",
     help="Monitor the status of the most recent fine-tuning jobs.",
-)  # type: ignore[misc]
+)
 def watch(
     limit: int = typer.Option(5, help="Limit the number of jobs to monitor"),
     poll: int = typer.Option(5, help="Polling interval in seconds"),
     screen: bool = typer.Option(False, help="Enable or disable screen output"),
 ) -> None:
     """
     Monitor the status of the most recent fine-tuning jobs.
@@ -93,72 +98,76 @@
             jobs = get_jobs(limit=limit)
             live_table.update(generate_table(jobs))
             time.sleep(poll)
 
 
 @app.command(
     help="Create a fine-tuning job from an existing ID.",
-)  # type: ignore[misc]
+)
 def create_from_id(
-    id: str = typer.Argument(..., help="ID of the existing fine-tuning job"),
+    id: str = typer.Argument(help="ID of the existing fine-tuning job"),
     model: str = typer.Option("gpt-3.5-turbo", help="Model to use for fine-tuning"),
-    n_epochs: int = typer.Option(
+    n_epochs: Optional[int] = typer.Option(
         None, help="Number of epochs for fine-tuning", show_default=False
     ),
-    batch_size: int = typer.Option(
+    batch_size: Optional[int] = typer.Option(
         None, help="Batch size for fine-tuning", show_default=False
     ),
-    learning_rate_multiplier: float = typer.Option(
+    learning_rate_multiplier: Optional[float] = typer.Option(
         None, help="Learning rate multiplier for fine-tuning", show_default=False
     ),
-    validation_file_id: str = typer.Option(
+    validation_file_id: Optional[str] = typer.Option(
         None, help="ID of the uploaded validation file"
     ),
 ) -> None:
-    hyperparameters_dict: Dict[str, Union[int, float, str]] = {}
+    hyperparameters_dict: Hyperparameters = {}
     if n_epochs is not None:
         hyperparameters_dict["n_epochs"] = n_epochs
     if batch_size is not None:
         hyperparameters_dict["batch_size"] = batch_size
     if learning_rate_multiplier is not None:
         hyperparameters_dict["learning_rate_multiplier"] = learning_rate_multiplier
 
     with console.status(
         f"[bold green]Creating fine-tuning job from ID {id}...", spinner="dots"
     ):
         job = client.fine_tuning.jobs.create(
             training_file=id,
             model=model,
-            hyperparameters=hyperparameters_dict if hyperparameters_dict else None,
+            hyperparameters=hyperparameters_dict,
             validation_file=validation_file_id if validation_file_id else None,
         )
         console.log(f"[bold green]Fine-tuning job created with ID: {job.id}")
     watch(limit=5, poll=2, screen=False)
 
 
 @app.command(
     help="Create a fine-tuning job from a file.",
-)  # type: ignore[misc]
+)
 def create_from_file(
-    file: str = typer.Argument(..., help="Path to the file for fine-tuning"),
+    file: str = typer.Argument(help="Path to the file for fine-tuning"),
     model: str = typer.Option("gpt-3.5-turbo", help="Model to use for fine-tuning"),
     poll: int = typer.Option(2, help="Polling interval in seconds"),
-    n_epochs: int = typer.Option(
+    n_epochs: Optional[int] = typer.Option(
         None, help="Number of epochs for fine-tuning", show_default=False
     ),
-    batch_size: int = typer.Option(
+    batch_size: Optional[int] = typer.Option(
         None, help="Batch size for fine-tuning", show_default=False
     ),
-    learning_rate_multiplier: float = typer.Option(
+    learning_rate_multiplier: Optional[float] = typer.Option(
         None, help="Learning rate multiplier for fine-tuning", show_default=False
     ),
-    validation_file: str = typer.Option(None, help="Path to the validation file"),
-    model_suffix: str = typer.Option(None, help="Suffix to identify the model"),
+    validation_file: Optional[str] = typer.Option(
+        None, help="Path to the validation file"
+    ),
+    model_suffix: Optional[str] = typer.Option(
+        None, help="Suffix to identify the model"
+    ),
 ) -> None:
-    hyperparameters_dict: Dict[str, Union[int, float, str]] = {}
+    hyperparameters_dict: Hyperparameters = {}
     if n_epochs is not None:
         hyperparameters_dict["n_epochs"] = n_epochs
     if batch_size is not None:
         hyperparameters_dict["batch_size"] = batch_size
     if learning_rate_multiplier is not None:
         hyperparameters_dict["learning_rate_multiplier"] = learning_rate_multiplier
 
@@ -173,30 +182,31 @@
             val_response = client.files.create(file=val_file, purpose="fine-tune")
         validation_file_id = val_response.id
 
     with console.status(f"Monitoring upload: {file_id} before finetuning...") as status:
         status.spinner_style = "dots"
         while True:
             file_status = get_file_status(file_id)
-            if validation_file_id:
-                validation_file_status = get_file_status(validation_file_id)
+            validation_file_status = (
+                get_file_status(validation_file_id) if validation_file_id else ""
+            )
 
             if file_status == "processed" and (
                 not validation_file_id or validation_file_status == "processed"
             ):
                 console.log(f"[bold green]File {file_id} uploaded successfully!")
                 if validation_file_id:
                     console.log(
                         f"[bold green]Validation file {validation_file_id} uploaded successfully!"
                     )
                 break
 
             time.sleep(poll)
 
-    additional_params: Dict[str, Union[str, Dict[str, Union[int, float, str]]]] = {}
+    additional_params: FuneTuningParams = {}
     if hyperparameters_dict:
         additional_params["hyperparameters"] = hyperparameters_dict
     if validation_file:
         additional_params["validation_file"] = validation_file
     if model_suffix:
         additional_params["suffix"] = model_suffix
 
@@ -214,17 +224,17 @@
             f"[bold green]Fine-tuning job created with ID: {job.id} from file ID: {file_id}"
         )
     watch(limit=5, poll=poll, screen=False)
 
 
 @app.command(
     help="Cancel a fine-tuning job.",
-)  # type: ignore[misc]
+)
 def cancel(
-    id: str = typer.Argument(..., help="ID of the fine-tuning job to cancel"),
+    id: str = typer.Argument(help="ID of the fine-tuning job to cancel"),
 ) -> None:
     with console.status(f"[bold red]Cancelling job {id}...", spinner="dots"):
         try:
             client.fine_tuning.jobs.cancel(id)
             console.log(f"[bold red]Job {id} cancelled successfully!")
         except Exception as e:
             console.log(f"[bold red]Error cancelling job {id}: {e}")
```

### Comparing `instructor-1.2.4/instructor/cli/usage.py` & `instructor-1.2.5/instructor/cli/usage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-from typing import List, Dict, Any, Union, DefaultDict
+from typing import Any, Union
+from collections.abc import Awaitable
 from datetime import datetime, timedelta
 import typer
 import os
 import aiohttp
 import asyncio
+from builtins import list as List
 from collections import defaultdict
 from rich.console import Console
 from rich.table import Table
 from rich.progress import Progress
 
 from instructor._types._alias import ModelNames
 
 
 app = typer.Typer()
 console = Console()
 
 api_key = os.environ.get("OPENAI_API_KEY")
 
 
-async def fetch_usage(date: str) -> Dict[str, Any]:
+async def fetch_usage(date: str) -> dict[str, Any]:
     headers = {"Authorization": f"Bearer {api_key}"}
     url = f"https://api.openai.com/v1/usage?date={date}"
     async with aiohttp.ClientSession() as session:
         async with session.get(url, headers=headers) as resp:
             return await resp.json()
 
 
-async def get_usage_for_past_n_days(n_days: int) -> List[Dict[str, Any]]:
-    tasks = []
-    all_data = []
+async def get_usage_for_past_n_days(n_days: int) -> list[dict[str, Any]]:
+    tasks: List[Awaitable[dict[str, Any]]] = []  # noqa: UP006 - conflicting with the fn name
+    all_data: List[dict[str, Any]] = []  # noqa: UP006 - conflicting with the fn name
     with Progress() as progress:
         if n_days > 1:
             task = progress.add_task("[green]Fetching usage data...", total=n_days)
             for i in range(n_days):
                 date = (datetime.now() - timedelta(days=i)).strftime("%Y-%m-%d")
                 tasks.append(fetch_usage(date))
                 progress.update(task, advance=1)
@@ -42,21 +44,15 @@
         fetched_data = await asyncio.gather(*tasks)
         for data in fetched_data:
             all_data.extend(data.get("data", []))
     return all_data
 
 
 # Define the cost per unit for each model
-# Add temporary body type hint here because mypy may infer the dict type
-# from the first few items (?) in the dict, which may not be representative of
-# the entire dict.
-MODEL_COSTS: Dict[
-    ModelNames,
-    Union[Dict[str, float], float],
-] = {
+MODEL_COSTS = {
     "gpt-4-0125-preview": {"prompt": 0.01 / 1000, "completion": 0.03 / 1000},
     "gpt-4-turbo-preview": {"prompt": 0.01 / 1000, "completion": 0.03 / 1000},
     "gpt-4-1106-preview": {"prompt": 0.01 / 1000, "completion": 0.03 / 1000},
     "gpt-4-vision-preview": {"prompt": 0.01 / 1000, "completion": 0.03 / 1000},
     "gpt-4": {"prompt": 0.03 / 1000, "completion": 0.06 / 1000},
     "gpt-4-0314": {"prompt": 0.03 / 1000, "completion": 0.06 / 1000},
     "gpt-4-0613": {"prompt": 0.03 / 1000, "completion": 0.06 / 1000},
@@ -75,15 +71,15 @@
     "text-embedding-3-large": 0.00013 / 1000,
     "text-embedding-ada-002": 0.00010 / 1000,
 }
 
 
 def get_model_cost(
     model: ModelNames,
-) -> Union[Dict[str, float], float]:
+) -> Union[dict[str, float], float]:
     """Get the cost details for a given model."""
     if model in MODEL_COSTS:
         return MODEL_COSTS[model]
 
     if model.startswith("gpt-3.5-turbo-16k"):
         return MODEL_COSTS["gpt-3.5-turbo-16k"]
     elif model.startswith("gpt-3.5-turbo"):
@@ -100,29 +96,29 @@
     snapshot_id: ModelNames,
     n_context_tokens: int,
     n_generated_tokens: int,
 ) -> float:
     """Calculate the cost based on the snapshot ID and number of tokens."""
     cost = get_model_cost(snapshot_id)
 
-    if isinstance(cost, float):
+    if isinstance(cost, (float, int)):
         return cost * (n_context_tokens + n_generated_tokens)
 
     prompt_cost = cost["prompt"] * n_context_tokens
     completion_cost = cost["completion"] * n_generated_tokens
     return prompt_cost + completion_cost
 
 
-def group_and_sum_by_date_and_snapshot(usage_data: List[Dict[str, Any]]) -> Table:
+def group_and_sum_by_date_and_snapshot(usage_data: list[dict[str, Any]]) -> Table:
     """Group and sum the usage data by date and snapshot, including costs."""
-    summary: DefaultDict[
-        str, DefaultDict[str, Dict[str, Union[int, float]]]
-    ] = defaultdict(
-        lambda: defaultdict(
-            lambda: {"total_requests": 0, "total_tokens": 0, "total_cost": 0.0}
+    summary: defaultdict[str, defaultdict[str, dict[str, Union[int, float]]]] = (
+        defaultdict(
+            lambda: defaultdict(
+                lambda: {"total_requests": 0, "total_tokens": 0, "total_cost": 0.0}
+            )
         )
     )
 
     for usage in usage_data:
         snapshot_id = usage["snapshot_id"]
         date = datetime.fromtimestamp(usage["aggregation_timestamp"]).strftime(
             "%Y-%m-%d"
@@ -156,15 +152,15 @@
                 str(data["total_requests"]),
                 "{:.2f}".format(data["total_cost"]),
             )
 
     return table
 
 
-@app.command(help="Displays OpenAI API usage data for the past N days.")  # type: ignore[misc]
+@app.command(help="Displays OpenAI API usage data for the past N days.")
 def list(
     n: int = typer.Option(0, help="Number of days."),
 ) -> None:
     all_data = asyncio.run(get_usage_for_past_n_days(n))
     table = group_and_sum_by_date_and_snapshot(all_data)
     console.print(table)
```

### Comparing `instructor-1.2.4/instructor/client.py` & `instructor-1.2.5/instructor/client.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,50 +1,44 @@
 from __future__ import annotations
 
 import openai
 import inspect
 import instructor
 from .utils import Provider, get_provider
-from openai.types.chat import ChatCompletion, ChatCompletionMessageParam
+from openai.types.chat import ChatCompletionMessageParam
 from typing import (
-    Type,
     TypeVar,
-    Generator,
-    Iterable,
-    Tuple,
     Callable,
-    List,
     overload,
     Union,
-    Awaitable,
-    AsyncGenerator,
     Any,
 )
+from collections.abc import Generator, Iterable, Awaitable, AsyncGenerator
 from typing_extensions import Self
 from pydantic import BaseModel
 from instructor.dsl.partial import Partial
 
 
-T = TypeVar("T", bound=Union[BaseModel, Iterable, Partial])
+T = TypeVar("T", bound=Union[BaseModel, "Iterable[Any]", "Partial[Any]"])
 
 
 class Instructor:
     client: Any | None
-    create_fn: Any
+    create_fn: Callable[..., Any]
     mode: instructor.Mode
     default_model: str | None = None
     provider: Provider
 
     def __init__(
         self,
         client: Any | None,
-        create: Callable,
+        create: Callable[..., Any],
         mode: instructor.Mode = instructor.Mode.TOOLS,
         provider: Provider = Provider.OPENAI,
-        **kwargs,
+        **kwargs: Any,
     ):
         self.client = client
         self.create_fn = create
         self.mode = mode
         self.kwargs = kwargs
         self.provider = provider
 
@@ -56,44 +50,88 @@
     def completions(self) -> Self:
         return self
 
     @property
     def messages(self) -> Self:
         return self
 
+    @overload
+    def create(
+        self: AsyncInstructor,
+        response_model: type[T],
+        messages: list[ChatCompletionMessageParam],
+        max_retries: int = 3,
+        validation_context: dict[str, Any] | None = None,
+        strict: bool = True,
+        **kwargs: Any,
+    ) -> Awaitable[T]: ...
+
+    @overload
+    def create(
+        self: Self,
+        response_model: type[T],
+        messages: list[ChatCompletionMessageParam],
+        max_retries: int = 3,
+        validation_context: dict[str, Any] | None = None,
+        strict: bool = True,
+        **kwargs: Any,
+    ) -> T: ...
+
     # TODO: we should overload a case where response_model is None
     def create(
         self,
-        response_model: Type[T],
-        messages: List[ChatCompletionMessageParam],
+        response_model: type[T],
+        messages: list[ChatCompletionMessageParam],
         max_retries: int = 3,
-        validation_context: dict | None = None,
+        validation_context: dict[str, Any] | None = None,
         strict: bool = True,
-        **kwargs,
-    ) -> T:
+        **kwargs: Any,
+    ) -> T | Awaitable[T]:
         kwargs = self.handle_kwargs(kwargs)
 
         return self.create_fn(
             response_model=response_model,
             messages=messages,
             max_retries=max_retries,
             validation_context=validation_context,
             strict=strict,
             **kwargs,
         )
 
+    @overload
+    def create_partial(
+        self: AsyncInstructor,
+        response_model: type[T],
+        messages: list[ChatCompletionMessageParam],
+        max_retries: int = 3,
+        validation_context: dict[str, Any] | None = None,
+        strict: bool = True,
+        **kwargs: Any,
+    ) -> AsyncGenerator[T, None]: ...
+
+    @overload
+    def create_partial(
+        self: Self,
+        response_model: type[T],
+        messages: list[ChatCompletionMessageParam],
+        max_retries: int = 3,
+        validation_context: dict[str, Any] | None = None,
+        strict: bool = True,
+        **kwargs: Any,
+    ) -> Generator[T, None, None]: ...
+
     def create_partial(
         self,
-        response_model: Type[T],
-        messages: List[ChatCompletionMessageParam],
+        response_model: type[T],
+        messages: list[ChatCompletionMessageParam],
         max_retries: int = 3,
-        validation_context: dict | None = None,
+        validation_context: dict[str, Any] | None = None,
         strict: bool = True,
-        **kwargs,
-    ) -> Generator[T, None, None]:
+        **kwargs: Any,
+    ) -> Generator[T, None, None] | AsyncGenerator[T, None]:
         assert self.provider != Provider.ANTHROPIC, "Anthropic doesn't support partial"
 
         kwargs["stream"] = True
 
         kwargs = self.handle_kwargs(kwargs)
 
         response_model = instructor.Partial[response_model]  # type: ignore
@@ -102,23 +140,45 @@
             response_model=response_model,
             max_retries=max_retries,
             validation_context=validation_context,
             strict=strict,
             **kwargs,
         )
 
+    @overload
+    def create_iterable(
+        self: AsyncInstructor,
+        messages: list[ChatCompletionMessageParam],
+        response_model: type[T],
+        max_retries: int = 3,
+        validation_context: dict[str, Any] | None = None,
+        strict: bool = True,
+        **kwargs: Any,
+    ) -> AsyncGenerator[T, None]: ...
+
+    @overload
+    def create_iterable(
+        self: Self,
+        messages: list[ChatCompletionMessageParam],
+        response_model: type[T],
+        max_retries: int = 3,
+        validation_context: dict[str, Any] | None = None,
+        strict: bool = True,
+        **kwargs: Any,
+    ) -> Generator[T, None, None]: ...
+
     def create_iterable(
         self,
-        messages: List[ChatCompletionMessageParam],
-        response_model: Type[T],
+        messages: list[ChatCompletionMessageParam],
+        response_model: type[T],
         max_retries: int = 3,
-        validation_context: dict | None = None,
+        validation_context: dict[str, Any] | None = None,
         strict: bool = True,
-        **kwargs,
-    ) -> Iterable[T]:
+        **kwargs: Any,
+    ) -> Generator[T, None, None] | AsyncGenerator[T, None]:
         assert self.provider != Provider.ANTHROPIC, "Anthropic doesn't support iterable"
 
         kwargs["stream"] = True
         kwargs = self.handle_kwargs(kwargs)
 
         response_model = Iterable[response_model]  # type: ignore
         return self.create_fn(
@@ -126,89 +186,111 @@
             response_model=response_model,
             max_retries=max_retries,
             validation_context=validation_context,
             strict=strict,
             **kwargs,
         )
 
+    @overload
+    def create_with_completion(
+        self: AsyncInstructor,
+        messages: list[ChatCompletionMessageParam],
+        response_model: type[T],
+        max_retries: int = 3,
+        validation_context: dict[str, Any] | None = None,
+        strict: bool = True,
+        **kwargs: Any,
+    ) -> Awaitable[tuple[T, Any]]: ...
+
+    @overload
+    def create_with_completion(
+        self: Self,
+        messages: list[ChatCompletionMessageParam],
+        response_model: type[T],
+        max_retries: int = 3,
+        validation_context: dict[str, Any] | None = None,
+        strict: bool = True,
+        **kwargs: Any,
+    ) -> tuple[T, Any]: ...
+
     def create_with_completion(
         self,
-        messages: List[ChatCompletionMessageParam],
-        response_model: Type[T],
+        messages: list[ChatCompletionMessageParam],
+        response_model: type[T],
         max_retries: int = 3,
-        validation_context: dict | None = None,
+        validation_context: dict[str, Any] | None = None,
         strict: bool = True,
-        **kwargs,
-    ) -> Tuple[T, ChatCompletion | Any]:
+        **kwargs: Any,
+    ) -> tuple[T, Any] | Awaitable[tuple[T, Any]]:
         kwargs = self.handle_kwargs(kwargs)
         model = self.create_fn(
             messages=messages,
             response_model=response_model,
             max_retries=max_retries,
             validation_context=validation_context,
             strict=strict,
             **kwargs,
         )
         return model, model._raw_response
 
-    def handle_kwargs(self, kwargs: dict):
+    def handle_kwargs(self, kwargs: dict[str, Any]) -> dict[str, Any]:
         for key, value in self.kwargs.items():
             if key not in kwargs:
                 kwargs[key] = value
         return kwargs
 
 
 class AsyncInstructor(Instructor):
     client: Any | None
-    create_fn: Any
+    create_fn: Callable[..., Any]
     mode: instructor.Mode
     default_model: str | None = None
     provider: Provider
 
     def __init__(
         self,
         client: Any | None,
-        create: Callable,
+        create: Callable[..., Any],
         mode: instructor.Mode = instructor.Mode.TOOLS,
         provider: Provider = Provider.OPENAI,
-        **kwargs,
+        **kwargs: Any,
     ):
         self.client = client
         self.create_fn = create
         self.mode = mode
         self.kwargs = kwargs
         self.provider = provider
 
     async def create(
         self,
-        messages: List[ChatCompletionMessageParam],
-        response_model: Type[T],
-        validation_context: dict | None = None,
+        response_model: type[T],
+        messages: list[ChatCompletionMessageParam],
         max_retries: int = 3,
+        validation_context: dict[str, Any] | None = None,
         strict: bool = True,
-        **kwargs,
+        **kwargs: Any,
     ) -> T:
         kwargs = self.handle_kwargs(kwargs)
         return await self.create_fn(
             response_model=response_model,
             validation_context=validation_context,
             max_retries=max_retries,
             messages=messages,
             strict=strict,
             **kwargs,
         )
 
     async def create_partial(
         self,
-        response_model: Type[T],
-        messages: List[ChatCompletionMessageParam],
-        validation_context: dict | None = None,
+        response_model: type[T],
+        messages: list[ChatCompletionMessageParam],
         max_retries: int = 3,
+        validation_context: dict[str, Any] | None = None,
         strict: bool = True,
-        **kwargs,
+        **kwargs: Any,
     ) -> AsyncGenerator[T, None]:
         assert self.provider != Provider.ANTHROPIC, "Anthropic doesn't support partial"
 
         kwargs = self.handle_kwargs(kwargs)
         kwargs["stream"] = True
         async for item in await self.create_fn(
             response_model=instructor.Partial[response_model],  # type: ignore
@@ -218,20 +300,20 @@
             strict=strict,
             **kwargs,
         ):
             yield item
 
     async def create_iterable(
         self,
-        response_model: Type[T],
-        messages: List[ChatCompletionMessageParam],
-        validation_context: dict | None = None,
+        messages: list[ChatCompletionMessageParam],
+        response_model: type[T],
         max_retries: int = 3,
+        validation_context: dict[str, Any] | None = None,
         strict: bool = True,
-        **kwargs,
+        **kwargs: Any,
     ) -> AsyncGenerator[T, None]:
         assert self.provider != Provider.ANTHROPIC, "Anthropic doesn't support iterable"
 
         kwargs = self.handle_kwargs(kwargs)
         kwargs["stream"] = True
         async for item in await self.create_fn(
             response_model=Iterable[response_model],
@@ -241,65 +323,67 @@
             strict=strict,
             **kwargs,
         ):
             yield item
 
     async def create_with_completion(
         self,
-        response_model: Type[T],
-        messages: List[ChatCompletionMessageParam],
-        validation_context: dict | None = None,
+        messages: list[ChatCompletionMessageParam],
+        response_model: type[T],
         max_retries: int = 3,
+        validation_context: dict[str, Any] | None = None,
         strict: bool = True,
-        **kwargs,
-    ) -> Tuple[T, dict]:
+        **kwargs: Any,
+    ) -> tuple[T, Any]:
         kwargs = self.handle_kwargs(kwargs)
         response = await self.create_fn(
             response_model=response_model,
             validation_context=validation_context,
             max_retries=max_retries,
             messages=messages,
             strict=strict,
             **kwargs,
         )
         return response, response._raw_response
 
 
 @overload
 def from_openai(
-    client: openai.OpenAI, mode: instructor.Mode = instructor.Mode.TOOLS, **kwargs
+    client: openai.OpenAI,
+    mode: instructor.Mode = instructor.Mode.TOOLS,
+    **kwargs: Any,
 ) -> Instructor:
     pass
 
 
 @overload
 def from_openai(
     client: openai.AsyncOpenAI,
     mode: instructor.Mode = instructor.Mode.TOOLS,
-    **kwargs,
+    **kwargs: Any,
 ) -> AsyncInstructor:
     pass
 
 
 def from_openai(
-    client: Union[openai.OpenAI, openai.AsyncOpenAI],
+    client: openai.OpenAI | openai.AsyncOpenAI,
     mode: instructor.Mode = instructor.Mode.TOOLS,
-    **kwargs,
+    **kwargs: Any,
 ) -> Instructor | AsyncInstructor:
     if hasattr(client, "base_url"):
         provider = get_provider(str(client.base_url))
     else:
         provider = Provider.OPENAI
 
     if not isinstance(client, (openai.OpenAI, openai.AsyncOpenAI)):
         import warnings
 
         warnings.warn(
-            "Client should be an instance of openai.OpenAI or openai.AsyncOpenAI. "
-            "Unexpected behavior may occur with other client types."
+            "Client should be an instance of openai.OpenAI or openai.AsyncOpenAI. Unexpected behavior may occur with other client types.",
+            stacklevel=2,
         )
 
     if provider in {Provider.ANYSCALE, Provider.TOGETHER}:
         assert mode in {
             instructor.Mode.TOOLS,
             instructor.Mode.JSON,
             instructor.Mode.JSON_SCHEMA,
@@ -332,33 +416,33 @@
             provider=provider,
             **kwargs,
         )
 
 
 @overload
 def from_litellm(
-    completion: Callable,
+    completion: Callable[..., Any],
     mode: instructor.Mode = instructor.Mode.TOOLS,
-    **kwargs,
+    **kwargs: Any,
 ) -> Instructor: ...
 
 
 @overload
 def from_litellm(
-    completion: Awaitable,
+    completion: Awaitable[Any],
     mode: instructor.Mode = instructor.Mode.TOOLS,
-    **kwargs,
+    **kwargs: Any,
 ) -> AsyncInstructor:
     pass
 
 
 def from_litellm(
-    completion: Callable | Awaitable,
+    completion: Callable[..., Any] | Awaitable[Any],
     mode: instructor.Mode = instructor.Mode.TOOLS,
-    **kwargs,
+    **kwargs: Any,
 ) -> Instructor | AsyncInstructor:
     is_async = inspect.isawaitable(completion)
 
     if not is_async:
         return Instructor(
             client=None,
             create=instructor.patch(create=completion, mode=mode),
```

### Comparing `instructor-1.2.4/instructor/client_anthropic.py` & `instructor-1.2.5/instructor/client_anthropic.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 from __future__ import annotations
 
 import anthropic
 import instructor
 
-from typing import overload
+from typing import overload, Any
 
 
 @overload
 def from_anthropic(
-    client: anthropic.Anthropic
-    | anthropic.AnthropicBedrock
-    | anthropic.AnthropicVertex,
+    client: (
+        anthropic.Anthropic | anthropic.AnthropicBedrock | anthropic.AnthropicVertex
+    ),
     mode: instructor.Mode = instructor.Mode.ANTHROPIC_JSON,
-    **kwargs,
-) -> instructor.Instructor:
-    ...
+    **kwargs: Any,
+) -> instructor.Instructor: ...
 
 
 @overload
 def from_anthropic(
-    client: anthropic.AsyncAnthropic
-    | anthropic.AsyncAnthropicBedrock
-    | anthropic.AsyncAnthropicVertex,
+    client: (
+        anthropic.AsyncAnthropic
+        | anthropic.AsyncAnthropicBedrock
+        | anthropic.AsyncAnthropicVertex
+    ),
     mode: instructor.Mode = instructor.Mode.ANTHROPIC_JSON,
-    **kwargs,
-) -> instructor.Instructor:
-    ...
+    **kwargs: Any,
+) -> instructor.AsyncInstructor: ...
 
 
 def from_anthropic(
     client: (
         anthropic.Anthropic
         | anthropic.AsyncAnthropic
         | anthropic.AnthropicBedrock
         | anthropic.AsyncAnthropicBedrock
         | anthropic.AsyncAnthropicVertex
+        | anthropic.AnthropicVertex
     ),
     mode: instructor.Mode = instructor.Mode.ANTHROPIC_JSON,
-    **kwargs,
+    **kwargs: Any,
 ) -> instructor.Instructor | instructor.AsyncInstructor:
     assert (
         mode
         in {
             instructor.Mode.ANTHROPIC_JSON,
             instructor.Mode.ANTHROPIC_TOOLS,
         }
@@ -56,15 +57,15 @@
             anthropic.AnthropicVertex,
             anthropic.AsyncAnthropicBedrock,
             anthropic.AsyncAnthropicVertex,
         ),
     ), "Client must be an instance of {anthropic.Anthropic, anthropic.AsyncAnthropic, anthropic.AnthropicBedrock, anthropic.AsyncAnthropicBedrock,  anthropic.AnthropicVertex, anthropic.AsyncAnthropicVertex}"
 
     if mode == instructor.Mode.ANTHROPIC_TOOLS:
-        create = client.beta.tools.messages.create
+        create = client.beta.tools.messages.create  # type: ignore - unknown in stubs
     else:
         create = client.messages.create
 
     if isinstance(
         client,
         (anthropic.Anthropic, anthropic.AnthropicBedrock, anthropic.AnthropicVertex),
     ):
```

### Comparing `instructor-1.2.4/instructor/client_cohere.py` & `instructor-1.2.5/instructor/client_cohere.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 from __future__ import annotations
 
 import cohere
 import instructor
 from functools import wraps
 from typing import (
-    Type,
     TypeVar,
     overload,
 )
+from typing import Any
 from typing_extensions import ParamSpec
 from pydantic import BaseModel
 from instructor.process_response import handle_response_model
 from instructor.retry import retry_async
 
 
 T_Model = TypeVar("T_Model", bound=BaseModel)
 T_ParamSpec = ParamSpec("T_ParamSpec")
 
 
 @overload
 def from_cohere(
     client: cohere.Client,
     mode: instructor.Mode = instructor.Mode.COHERE_TOOLS,
-    **kwargs,
-) -> instructor.Instructor:
-    ...
+    **kwargs: Any,
+) -> instructor.Instructor: ...
 
 
 @overload
 def from_cohere(
     client: cohere.AsyncClient,
     mode: instructor.Mode = instructor.Mode.COHERE_TOOLS,
-    **kwargs,
-) -> instructor.AsyncInstructor:
-    ...
+    **kwargs: Any,
+) -> instructor.AsyncInstructor: ...
 
 
 def from_cohere(
     client: cohere.Client | cohere.AsyncClient,
     mode: instructor.Mode = instructor.Mode.COHERE_TOOLS,
-    **kwargs,
+    **kwargs: Any,
 ):
     assert mode in {
         instructor.Mode.COHERE_TOOLS,
     }, "Mode be one of {instructor.Mode.COHERE_TOOLS}"
 
     assert isinstance(
         client, (cohere.Client, cohere.AsyncClient)
@@ -56,32 +54,34 @@
             provider=instructor.Provider.COHERE,
             mode=mode,
             **kwargs,
         )
 
     @wraps(client.chat)
     async def new_create_async(
-        response_model: Type[T_Model] = None,
-        validation_context: dict = None,
+        response_model: type[T_Model] | None = None,
+        validation_context: dict[str, Any] | None = None,
         max_retries: int = 1,
         *args: T_ParamSpec.args,
         **kwargs: T_ParamSpec.kwargs,
     ) -> T_Model:
-        response_model, new_kwargs = handle_response_model(
-            response_model=response_model, mode=mode, **kwargs
+        prepared_response_model, new_kwargs = handle_response_model(
+            response_model=response_model,
+            mode=mode,
+            **kwargs,
         )
         response = await retry_async(
             func=client.chat,
-            response_model=response_model,
+            response_model=prepared_response_model,
             validation_context=validation_context,
             max_retries=max_retries,
             args=args,
             kwargs=new_kwargs,
             mode=mode,
-        )  # type: ignore
+        )
         return response
 
     return instructor.AsyncInstructor(
         client=client,
         create=new_create_async,
         provider=instructor.Provider.COHERE,
         mode=mode,
```

### Comparing `instructor-1.2.4/instructor/client_groq.py` & `instructor-1.2.5/instructor/client_groq.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 from __future__ import annotations
 
-from typing import overload
+from typing import overload, Any
 
 import groq
 import instructor
 
 
 @overload
 def from_groq(
     client: groq.Groq,
     mode: instructor.Mode = instructor.Mode.TOOLS,
-    **kwargs,
-) -> instructor.Instructor:
-    ...
+    **kwargs: Any,
+) -> instructor.Instructor: ...
 
 
 @overload
 def from_groq(
     client: groq.AsyncGroq,
     mode: instructor.Mode = instructor.Mode.TOOLS,
-    **kwargs,
-) -> instructor.Instructor:
-    ...
+    **kwargs: Any,
+) -> instructor.Instructor: ...
 
 
 def from_groq(
     client: groq.Groq | groq.AsyncGroq,
     mode: instructor.Mode = instructor.Mode.TOOLS,
-    **kwargs,
+    **kwargs: Any,
 ) -> instructor.Instructor:
     assert mode in {
         instructor.Mode.JSON,
         instructor.Mode.TOOLS,
     }, "Mode be one of {instructor.Mode.JSON, instructor.Mode.TOOLS}"
 
     assert isinstance(
```

### Comparing `instructor-1.2.4/instructor/client_mistral.py` & `instructor-1.2.5/instructor/client_mistral.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,55 @@
 # Future imports to ensure compatibility with Python 3.9
 from __future__ import annotations
 
 import mistralai.client
 import mistralai.async_client as mistralaiasynccli
 import instructor
-from typing import overload
+from typing import overload, Any
 
 
 @overload
 def from_mistral(
     client: mistralai.client.MistralClient,
     mode: instructor.Mode = instructor.Mode.MISTRAL_TOOLS,
-    **kwargs,
+    **kwargs: Any,
 ) -> instructor.Instructor: ...
 
 
 @overload
 def from_mistral(
     client: mistralaiasynccli.MistralAsyncClient,
     mode: instructor.Mode = instructor.Mode.MISTRAL_TOOLS,
-    **kwargs,
+    **kwargs: Any,
 ) -> instructor.AsyncInstructor: ...
 
 
 def from_mistral(
     client: mistralai.client.MistralClient | mistralaiasynccli.MistralAsyncClient,
     mode: instructor.Mode = instructor.Mode.MISTRAL_TOOLS,
-    **kwargs,
+    **kwargs: Any,
 ) -> instructor.Instructor | instructor.AsyncInstructor:
     assert mode in {
         instructor.Mode.MISTRAL_TOOLS,
     }, "Mode be one of {instructor.Mode.MISTRAL_TOOLS}"
 
     assert isinstance(
         client, (mistralai.client.MistralClient, mistralaiasynccli.MistralAsyncClient)
     ), "Client must be an instance of mistralai.client.MistralClient or mistralai.async_cli.MistralAsyncClient"
 
     if isinstance(client, mistralai.client.MistralClient):
-
         return instructor.Instructor(
             client=client,
             create=instructor.patch(create=client.chat, mode=mode),
             provider=instructor.Provider.MISTRAL,
             mode=mode,
             **kwargs,
         )
 
     else:
-
         return instructor.AsyncInstructor(
             client=client,
             create=instructor.patch(create=client.chat, mode=mode),
             provider=instructor.Provider.MISTRAL,
             mode=mode,
             **kwargs,
         )
```

### Comparing `instructor-1.2.4/instructor/distil.py` & `instructor-1.2.5/instructor/distil.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,44 @@
 import enum
 import json
 import uuid
 import logging
 import inspect
 import functools
 
-from typing import Any, Callable, Dict, List, Optional, Tuple, Type, TypeVar
+from typing import (
+    Any,
+    Callable,
+    Optional,
+    TypeVar,
+    TypedDict,
+    Literal,
+    Union,
+)
+from typing_extensions import ParamSpec, NotRequired
+from openai.types.chat.chat_completion import ChatCompletion
+from openai.types.chat.chat_completion_message_param import ChatCompletionMessageParam
 from pydantic import BaseModel, validate_call
 
 from openai import OpenAI
 from instructor.function_calls import openai_schema
 
 
-T_Retval = TypeVar("T_Retval")
+P = ParamSpec("P")
+T_Retval = TypeVar("T_Retval", bound=BaseModel)
+
+
+class OpenAIChatKwargs(TypedDict):
+    messages: list[ChatCompletionMessageParam]
+    functions: NotRequired[list[dict[str, Any]]]
 
 
 class FinetuneFormat(enum.Enum):
-    MESSAGES: str = "messages"
-    RAW: str = "raw"
+    MESSAGES = "messages"
+    RAW = "raw"
 
 
 def get_signature_from_fn(fn: Callable[..., Any]) -> str:
     """
     Get the function signature as a string.
 
     :Example:
@@ -41,15 +58,15 @@
     if docstring:
         formatted_docstring = f'"""\n{docstring}\n"""'
     else:
         formatted_docstring = ""
     return f"{lines}\n{formatted_docstring}"
 
 
-@functools.lru_cache()
+@functools.lru_cache
 def format_function(func: Callable[..., Any]) -> str:
     """
     Format a function as a string with docstring and body.
     """
     source_lines = inspect.getsourcelines(func)
     definition = " ".join(source_lines[0]).strip()
 
@@ -80,15 +97,15 @@
 
 
 class Instructions:
     def __init__(
         self,
         name: Optional[str] = None,
         id: Optional[str] = None,
-        log_handlers: Optional[List[logging.Handler]] = None,
+        log_handlers: Optional[list[logging.Handler]] = None,
         finetune_format: FinetuneFormat = FinetuneFormat.MESSAGES,
         indent: int = 2,
         include_code_body: bool = False,
         openai_client: Optional[OpenAI] = None,
     ) -> None:
         """
         Instructions for distillation and dispatch.
@@ -112,20 +129,20 @@
         for handler in log_handlers or []:
             self.logger.addHandler(handler)
 
     def distil(
         self,
         *args: Any,
         name: Optional[str] = None,
-        mode: str = "distil",
+        mode: Literal["distil", "dispatch"] = "distil",
         model: str = "gpt-3.5-turbo",
         fine_tune_format: Optional[FinetuneFormat] = None,
-    ) -> Callable[
-        [Callable[..., Any]],
-        Callable[[Callable[..., T_Retval]], Callable[..., T_Retval]],
+    ) -> Union[
+        Callable[P, Union[T_Retval, ChatCompletion]],
+        Callable[[Callable[P, T_Retval]], Callable[P, Union[T_Retval, ChatCompletion]]],
     ]:
         """
         Decorator to track the function call and response, supports distillation and dispatch modes.
 
         If used without arguments, it must be used as a decorator.
 
         :Example:
@@ -145,56 +162,61 @@
         allowed_modes = {"distil", "dispatch"}
         assert mode in allowed_modes, f"Must be in {allowed_modes}"
 
         if fine_tune_format is None:
             fine_tune_format = self.finetune_format
 
         def _wrap_distil(
-            fn: Callable[..., Any],
-        ) -> Callable[[Callable[..., T_Retval]], Callable[..., T_Retval]]:
+            fn: Callable[P, T_Retval],
+        ) -> Callable[P, Union[T_Retval, ChatCompletion]]:
             msg = f"Return type hint for {fn} must subclass `pydantic.BaseModel'"
             assert is_return_type_base_model_or_instance(fn), msg
             return_base_model = inspect.signature(fn).return_annotation
 
             @functools.wraps(fn)
-            def _dispatch(*args: Any, **kwargs: Any) -> Callable[..., T_Retval]:
-                name = name if name else fn.__name__
+            def _dispatch(*args: P.args, **kwargs: P.kwargs) -> ChatCompletion:
                 openai_kwargs = self.openai_kwargs(
-                    name=name,
+                    name=name if name else fn.__name__,
                     fn=fn,
                     args=args,
                     kwargs=kwargs,
                     base_model=return_base_model,
                 )
                 return self.client.chat.completions.create(
-                    **openai_kwargs, model=model, response_model=return_base_model
+                    **openai_kwargs,
+                    model=model,
+                    response_model=return_base_model,  # type: ignore - TODO figure out why `response_model` is not recognized
                 )
 
             @functools.wraps(fn)
-            def _distil(*args: Any, **kwargs: Any) -> Callable[..., T_Retval]:
+            def _distil(*args: P.args, **kwargs: P.kwargs) -> T_Retval:
                 resp = fn(*args, **kwargs)
                 self.track(
-                    fn, args, kwargs, resp, name=name, finetune_format=fine_tune_format
+                    fn,
+                    args,
+                    kwargs,
+                    resp,
+                    name=name,
+                    finetune_format=fine_tune_format,
                 )
-
                 return resp
 
             return _dispatch if mode == "dispatch" else _distil
 
         if len(args) == 1 and callable(args[0]):
             return _wrap_distil(args[0])
 
         return _wrap_distil
 
-    @validate_call  # type: ignore[misc]
+    @validate_call
     def track(
         self,
         fn: Callable[..., Any],
-        args: Tuple[Any, ...],
-        kwargs: Dict[str, Any],
+        args: tuple[Any, ...],
+        kwargs: dict[str, Any],
         resp: BaseModel,
         name: Optional[str] = None,
         finetune_format: FinetuneFormat = FinetuneFormat.MESSAGES,
     ) -> None:
         """
         Track the function call and response in a log file, later used for finetuning.
 
@@ -202,15 +224,15 @@
         :param args: Arguments passed to the function.
         :param kwargs: Keyword arguments passed to the function.
         :param resp: Response returned by the function.
         :param name: Name of the function to track. Defaults to the function name.
         :param finetune_format: Format to use for finetuning. Defaults to "raw".
         """
         name = name if name else fn.__name__
-        base_model: BaseModel = type(resp)
+        base_model = type(resp)
 
         if finetune_format == FinetuneFormat.MESSAGES:
             openai_function_call = openai_schema(base_model).openai_schema
             openai_kwargs = self.openai_kwargs(name, fn, args, kwargs, base_model)
             openai_kwargs["messages"].append(
                 {
                     "role": "assistant",
@@ -234,30 +256,30 @@
             )
             self.logger.info(json.dumps(function_body))
 
     def openai_kwargs(
         self,
         name: str,
         fn: Callable[..., Any],
-        args: Tuple[Any, ...],
-        kwargs: Dict[str, Any],
-        base_model: Type[BaseModel],
-    ) -> Dict[str, Any]:
+        args: tuple[Any, ...],
+        kwargs: dict[str, Any],
+        base_model: type[BaseModel],
+    ) -> OpenAIChatKwargs:
         if self.include_code_body:
             func_def = format_function(fn)
         else:
             func_def = get_signature_from_fn(fn)
 
         str_args = ", ".join(map(str, args))
         str_kwargs = (
             ", ".join(f"{k}={json.dumps(v)}" for k, v in kwargs.items()) or None
         )
         call_args = ", ".join(filter(None, [str_args, str_kwargs]))
 
-        function_body = {
+        function_body: OpenAIChatKwargs = {
             "messages": [
                 {
                     "role": "system",
                     "content": f"Predict the results of this function:\n\n{func_def}",
                 },
                 {
                     "role": "user",
```

### Comparing `instructor-1.2.4/instructor/dsl/citation.py` & `instructor-1.2.5/instructor/dsl/citation.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pydantic import BaseModel, Field, model_validator, ValidationInfo
-from typing import Generator, List, Tuple
+from collections.abc import Generator
 
 
-class CitationMixin(BaseModel):  # type: ignore[misc]
+class CitationMixin(BaseModel):
     """
     Helpful mixing that can use `validation_context={"context": context}` in `from_response` to find the span of the substring_phrase in the context.
 
     ## Usage
 
     ```python
     from pydantic import BaseModel, Field
@@ -49,15 +49,15 @@
             "Jason is 20 years old",
         ]
     }
     ```
 
     """
 
-    substring_quotes: List[str] = Field(
+    substring_quotes: list[str] = Field(
         description="List of unique and specific substrings of the quote that was used to answer the question.",
     )
 
     @model_validator(mode="after")  # type: ignore[misc]
     def validate_sources(self, info: ValidationInfo) -> "CitationMixin":
         """
         For each substring_phrase, find the span of the substring_phrase in the context.
@@ -73,25 +73,25 @@
         spans = list(self.get_spans(text_chunks))
         # Replace the substring_phrase with the actual substring
         self.substring_quotes = [text_chunks[span[0] : span[1]] for span in spans]
         return self
 
     def _get_span(
         self, quote: str, context: str, errs: int = 5
-    ) -> Generator[Tuple[int, int], None, None]:
-        import regex  # type: ignore[import-untyped]
+    ) -> Generator[tuple[int, int], None, None]:
+        import regex
 
         minor = quote
         major = context
 
         errs_ = 0
         s = regex.search(f"({minor}){{e<={errs_}}}", major)
         while s is None and errs_ <= errs:
             errs_ += 1
             s = regex.search(f"({minor}){{e<={errs_}}}", major)
 
         if s is not None:
             yield from s.spans()
 
-    def get_spans(self, context: str) -> Generator[Tuple[int, int], None, None]:
+    def get_spans(self, context: str) -> Generator[tuple[int, int], None, None]:
         for quote in self.substring_quotes:
             yield from self._get_span(quote, context)
```

### Comparing `instructor-1.2.4/instructor/dsl/iterable.py` & `instructor-1.2.5/instructor/dsl/iterable.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from typing import Any, AsyncGenerator, Generator, Iterable, List, Optional, Tuple, Type
+from typing import Any, Optional, cast, ClassVar
+from collections.abc import AsyncGenerator, Generator, Iterable
 
-from pydantic import BaseModel, Field, create_model
+from pydantic import BaseModel, Field, create_model  # type: ignore - remove once Pydantic is updated
 
 from instructor.function_calls import OpenAISchema
 from instructor.mode import Mode
 from instructor.utils import extract_json_from_stream, extract_json_from_stream_async
 
 
 class IterableBase:
-    task_type = None  # type: ignore[var-annotated]
+    task_type: ClassVar[Optional[type[BaseModel]]] = None
 
     @classmethod
     def from_streaming_response(
         cls, completion: Iterable[Any], mode: Mode, **kwargs: Any
     ) -> Generator[BaseModel, None, None]:  # noqa: ARG003
         json_chunks = cls.extract_json(completion, mode)
 
@@ -115,31 +116,31 @@
                         raise NotImplementedError(
                             f"Mode {mode} is not supported for MultiTask streaming"
                         )
             except AttributeError:
                 pass
 
     @staticmethod
-    def get_object(s: str, stack: int) -> Tuple[Optional[str], str]:
+    def get_object(s: str, stack: int) -> tuple[Optional[str], str]:
         start_index = s.find("{")
         for i, c in enumerate(s):
             if c == "{":
                 stack += 1
             if c == "}":
                 stack -= 1
                 if stack == 0:
                     return s[start_index : i + 1], s[i + 2 :]
         return None, s
 
 
 def IterableModel(
-    subtask_class: Type[BaseModel],
+    subtask_class: type[BaseModel],
     name: Optional[str] = None,
     description: Optional[str] = None,
-) -> Type[BaseModel]:
+) -> type[BaseModel]:
     """
     Dynamically create a IterableModel OpenAISchema that can be used to segment multiple
     tasks given a base class. This creates class that can be used to create a toolkit
     for a specific task, names and descriptions are automatically generated. However
     they can be overridden.
 
     ## Usage
@@ -187,27 +188,30 @@
         schema (OpenAISchema): A new class that can be used to segment multiple tasks
     """
     task_name = subtask_class.__name__ if name is None else name
 
     name = f"Iterable{task_name}"
 
     list_tasks = (
-        List[subtask_class],  # type: ignore[valid-type]
+        list[subtask_class],
         Field(
             default_factory=list,
             repr=False,
             description=f"Correctly segmented list of `{task_name}` tasks",
         ),
     )
 
+    base_models = cast(tuple[type[BaseModel], ...], (OpenAISchema, IterableBase))
     new_cls = create_model(
         name,
         tasks=list_tasks,
-        __base__=(OpenAISchema, IterableBase),  # type: ignore
+        __base__=base_models,
     )
+    new_cls = cast(type[IterableBase], new_cls)
+
     # set the class constructor BaseModel
     new_cls.task_type = subtask_class
 
     new_cls.__doc__ = (
         f"Correct segmentation of `{task_name}` tasks"
         if description is None
         else description
```

### Comparing `instructor-1.2.4/instructor/dsl/maybe.py` & `instructor-1.2.5/instructor/dsl/maybe.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from pydantic import BaseModel, Field, create_model
-from typing import Generic, Optional, Type, TypeVar
+from pydantic import BaseModel, Field, create_model  # type: ignore - remove once Pydantic is updated
+from typing import Generic, Optional, TypeVar
 
 T = TypeVar("T", bound=BaseModel)
 
 
-class MaybeBase(BaseModel, Generic[T]):  # type: ignore[misc]
+class MaybeBase(BaseModel, Generic[T]):
     """
     Extract a result from a model, if any, otherwise set the error and message fields.
     """
 
     result: Optional[T]
     error: bool = Field(default=False)
     message: Optional[str]
 
     def __bool__(self) -> bool:
         return self.result is not None
 
 
-def Maybe(model: Type[T]) -> Type[MaybeBase[T]]:
+def Maybe(model: type[T]) -> type[MaybeBase[T]]:
     """
     Create a Maybe model for a given Pydantic model. This allows you to return a model that includes fields for `result`, `error`, and `message` for sitatations where the data may not be present in the context.
 
     ## Usage
 
     ```python
     from pydantic import BaseModel, Field
@@ -49,27 +49,26 @@
 
     Parameters:
         model (Type[BaseModel]): The Pydantic model to wrap with Maybe.
 
     Returns:
         MaybeModel (Type[BaseModel]): A new Pydantic model that includes fields for `result`, `error`, and `message`.
     """
-
-    fields = {
-        "result": (
+    return create_model(
+        f"Maybe{model.__name__}",
+        __base__=MaybeBase,
+        reuslts=(
             Optional[model],
             Field(
                 default=None,
                 description="Correctly extracted result from the model, if any, otherwise None",
             ),
         ),
-        "error": (bool, Field(default=False)),
-        "message": (
+        error=(bool, Field(default=False)),
+        message=(
             Optional[str],
             Field(
                 default=None,
                 description="Error message if no result was found, should be short and concise",
             ),
         ),
-    }
-
-    return create_model(f"Maybe{model.__name__}", __base__=MaybeBase, **fields)
+    )
```

### Comparing `instructor-1.2.4/instructor/dsl/parallel.py` & `instructor-1.2.5/instructor/dsl/parallel.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 from typing import (
     Any,
-    Dict,
-    Generator,
-    List,
     Optional,
-    Tuple,
-    Type,
     TypeVar,
     Union,
     get_args,
     get_origin,
 )
+from collections.abc import Generator
 from pydantic import BaseModel
 from instructor.function_calls import OpenAISchema, openai_schema
 from collections.abc import Iterable
 
 from instructor.mode import Mode
 
 T = TypeVar("T", bound=OpenAISchema)
 
 
 class ParallelBase:
-    def __init__(self, *models: Type[OpenAISchema]):
+    def __init__(self, *models: type[OpenAISchema]):
         # Note that for everything else we've created a class, but for parallel base it is an instance
         assert len(models) > 0, "At least one model is required"
         self.models = models
         self.registry = {
             model.__name__ if hasattr(model, "__name__") else str(model): model
             for model in models
         }
@@ -44,15 +40,15 @@
             name = tool_call.function.name
             arguments = tool_call.function.arguments
             yield self.registry[name].model_validate_json(
                 arguments, context=validation_context, strict=strict
             )
 
 
-def get_types_array(typehint: Type[Iterable[T]]) -> Tuple[Type[T], ...]:
+def get_types_array(typehint: type[Iterable[T]]) -> tuple[type[T], ...]:
     should_be_iterable = get_origin(typehint)
     if should_be_iterable is not Iterable:
         raise TypeError(f"Model should be with Iterable instead if {typehint}")
 
     if get_origin(get_args(typehint)[0]) is Union:
         # works for Iterable[Union[int, str]]
         the_types = get_args(get_args(typehint)[0])
@@ -63,18 +59,18 @@
         the_types = get_args(get_args(typehint)[0])
         return the_types
 
     # works for Iterable[int]
     return get_args(typehint)
 
 
-def handle_parallel_model(typehint: Type[Iterable[T]]) -> List[Dict[str, Any]]:
+def handle_parallel_model(typehint: type[Iterable[T]]) -> list[dict[str, Any]]:
     the_types = get_types_array(typehint)
     return [
         {"type": "function", "function": openai_schema(model).openai_schema}
         for model in the_types
     ]
 
 
-def ParallelModel(typehint: Type[Iterable[T]]) -> ParallelBase:
+def ParallelModel(typehint: type[Iterable[T]]) -> ParallelBase:
     the_types = get_types_array(typehint)
     return ParallelBase(*[model for model in the_types])
```

### Comparing `instructor-1.2.4/instructor/dsl/partial.py` & `instructor-1.2.5/instructor/dsl/partial.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,44 +5,42 @@
 # This code is used in accordance with the repository's license, and this reference
 # serves as an acknowledgment of the original author's contribution to this project.
 # --------------------------------------------------------------------------------
 
 from __future__ import annotations
 
 import pydantic_core
-from pydantic import BaseModel, create_model
+from pydantic import BaseModel, create_model  # type: ignore - remove once Pydantic is updated
 from pydantic.fields import FieldInfo
 from typing import (
     Any,
-    AsyncGenerator,
-    Generator,
     Generic,
     get_args,
     get_origin,
-    Iterable,
     NoReturn,
     Optional,
     TypeVar,
 )
+from collections.abc import AsyncGenerator, Generator, Iterable
 from copy import deepcopy
-from functools import lru_cache
+from functools import cache
 
 from instructor.mode import Mode
 from instructor.utils import extract_json_from_stream, extract_json_from_stream_async
 
 T_Model = TypeVar("T_Model", bound=BaseModel)
 
 
 class MakeFieldsOptional:
     pass
 
 
 def _make_field_optional(
     field: FieldInfo,
-) -> tuple[object, FieldInfo]:
+) -> tuple[Any, FieldInfo]:
     tmp_field = deepcopy(field)
 
     annotation = field.annotation
 
     # Handle generics (like List, Dict, etc.)
     if get_origin(annotation) is not None:
         # Get the generic base (like List, Dict) and its arguments (like User in List[User])
@@ -68,20 +66,21 @@
     # attributes to optionals.
     elif isinstance(annotation, type) and issubclass(annotation, BaseModel):
         tmp_field.annotation = Optional[Partial[annotation, MakeFieldsOptional]]  # type: ignore[assignment, valid-type]
         tmp_field.default = {}
     else:
         tmp_field.annotation = Optional[field.annotation]  # type: ignore[assignment]
         tmp_field.default = None
-    return tmp_field.annotation, tmp_field
+
+    return tmp_field.annotation, tmp_field  # type: ignore
 
 
 class PartialBase(Generic[T_Model]):
     @classmethod
-    @lru_cache(maxsize=None)
+    @cache
     def get_partial_model(cls) -> type[T_Model]:
         """Return a partial model we can use to validate partial results."""
         assert issubclass(
             cls, BaseModel
         ), f"{cls.__name__} must be a subclass of BaseModel"
 
         return create_model(
@@ -120,30 +119,28 @@
 
         return cls.model_from_chunks_async(json_chunks, **kwargs)
 
     @classmethod
     def model_from_chunks(
         cls, json_chunks: Iterable[Any], **kwargs: Any
     ) -> Generator[T_Model, None, None]:
-        prev_obj = None
         potential_object = ""
         partial_model = cls.get_partial_model()
         for chunk in json_chunks:
             potential_object += chunk
 
             obj = pydantic_core.from_json(potential_object or "{}", allow_partial=True)
-            obj = partial_model.model_validate(obj, strict=None, **kwargs)  # type: ignore[attr-defined]
+            obj = partial_model.model_validate(obj, strict=None, **kwargs)
             yield obj
 
     @classmethod
     async def model_from_chunks_async(
         cls, json_chunks: AsyncGenerator[str, None], **kwargs: Any
     ) -> AsyncGenerator[T_Model, None]:
         potential_object = ""
-        prev_obj = None
         partial_model = cls.get_partial_model()
         async for chunk in json_chunks:
             potential_object += chunk
             obj = pydantic_core.from_json(potential_object or "{}", allow_partial=True)
             obj = partial_model.model_validate(obj, strict=None, **kwargs)
             yield obj
 
@@ -204,15 +201,15 @@
         Partial[SomeModel]
     """
 
     def __new__(
         cls,
         *args: object,  # noqa :ARG003
         **kwargs: object,  # noqa :ARG003
-    ) -> "Partial[T_Model]":
+    ) -> Partial[T_Model]:
         """Cannot instantiate.
 
         Raises:
             TypeError: Direct instantiation not allowed.
         """
         raise TypeError("Cannot instantiate abstract Partial class.")
 
@@ -222,17 +219,17 @@
         **kwargs: object,
     ) -> NoReturn:
         """Cannot subclass.
 
         Raises:
            TypeError: Subclassing not allowed.
         """
-        raise TypeError("Cannot subclass {}.Partial".format(cls.__module__))
+        raise TypeError(f"Cannot subclass {cls.__module__}.Partial")
 
-    def __class_getitem__(  # type: ignore[override]
+    def __class_getitem__(
         cls,
         wrapped_class: type[T_Model] | tuple[type[T_Model], type[MakeFieldsOptional]],
     ) -> type[T_Model]:
         """Convert model to one that inherits from PartialBase.
 
         We don't make the fields optional at this point, we just wrap them with `Partial` so the names of the nested models will be
         `Partial{ModelName}`. We want the output of `model_json_schema()` to
@@ -256,29 +253,29 @@
                 # Get the generic base (like List, Dict) and its arguments (like User in List[User])
                 generic_base = get_origin(annotation)
                 generic_args = get_args(annotation)
 
                 # Recursively apply Partial to each of the generic arguments
                 modified_args = tuple(
                     (
-                        Partial[arg]  # type: ignore[valid-type]
+                        Partial[arg]
                         if isinstance(arg, type) and issubclass(arg, BaseModel)
                         else arg
                     )
                     for arg in generic_args
                 )
 
                 # Reconstruct the generic type with modified arguments
                 tmp_field.annotation = (
                     generic_base[modified_args] if generic_base else None
                 )
             # If the field is a BaseModel, then recursively convert it's
             # attributes to optionals.
             elif isinstance(annotation, type) and issubclass(annotation, BaseModel):
-                tmp_field.annotation = Partial[annotation]  # type: ignore[assignment, valid-type]
+                tmp_field.annotation = Partial[annotation]
             return tmp_field.annotation, tmp_field
 
         return create_model(
             __model_name=(
                 wrapped_class.__name__
                 if wrapped_class.__name__.startswith("Partial")
                 else f"Partial{wrapped_class.__name__}"
@@ -289,8 +286,8 @@
                 field_name: (
                     _make_field_optional(field_info)
                     if make_fields_optional is not None
                     else _wrap_models(field_info)
                 )
                 for field_name, field_info in wrapped_class.model_fields.items()
             },
-        )  # type: ignore[all]
+        )  # type: ignore
```

### Comparing `instructor-1.2.4/instructor/dsl/simple_type.py` & `instructor-1.2.5/instructor/dsl/simple_type.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
+from __future__ import annotations
 from inspect import isclass
 import typing
-from pydantic import BaseModel, create_model
+from pydantic import BaseModel, create_model  # type: ignore - remove once Pydantic is updated
 from enum import Enum
 
 
 from instructor.dsl.partial import Partial
 from instructor.function_calls import OpenAISchema
 
 
@@ -16,26 +17,28 @@
 
 
 class ModelAdapter(typing.Generic[T]):
     """
     Accepts a response model and returns a BaseModel with the response model as the content.
     """
 
-    def __class_getitem__(cls, response_model) -> typing.Type[BaseModel]:
+    def __class_getitem__(cls, response_model: type[BaseModel]) -> type[BaseModel]:
         assert is_simple_type(response_model), "Only simple types are supported"
         tmp = create_model(
             "Response",
             content=(response_model, ...),
             __doc__="Correctly Formated and Extracted Response.",
             __base__=(AdapterBase, OpenAISchema),
         )
         return tmp
 
 
-def is_simple_type(response_model) -> bool:
+def is_simple_type(
+    response_model: type[BaseModel] | str | int | float | bool,
+) -> bool:
     # ! we're getting mixes between classes and instances due to how we handle some
     # ! response model types, we should fix this in later PRs
     if isclass(response_model) and issubclass(response_model, BaseModel):
         return False
 
     if typing.get_origin(response_model) in {typing.Iterable, Partial}:
         # These are reserved for streaming types, would be nice to
```

### Comparing `instructor-1.2.4/instructor/dsl/validators.py` & `instructor-1.2.5/instructor/dsl/validators.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,15 @@
                 {
                     "role": "user",
                     "content": f"Does `{v}` follow the rules: {statement}",
                 },
             ],
             model=model,
             temperature=temperature,
-        )  # type: ignore[all]
+        )
 
         # If the response is  not valid, return the reason, this could be used in
         # the future to generate a better response, via reasking mechanism.
         assert resp.is_valid, resp.reason
 
         if allow_override and not resp.is_valid and resp.fixed_value is not None:
             # If the value is not valid, but we allow override, return the fixed value
```

### Comparing `instructor-1.2.4/instructor/function_calls.py` & `instructor-1.2.5/instructor/function_calls.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,37 @@
+import json
 import logging
 from functools import wraps
-from typing import Annotated, Any, Dict, Optional, Type, TypeVar
+from typing import Annotated, Any, Optional, TypeVar, cast
 
 from docstring_parser import parse
 from openai.types.chat import ChatCompletion
-from pydantic import BaseModel, Field, TypeAdapter, create_model
+from pydantic import (  # type: ignore - remove once Pydantic is updated
+    BaseModel,
+    ConfigDict,
+    Field,
+    TypeAdapter,
+    create_model,
+)
 
 from instructor.exceptions import IncompleteOutputException
 from instructor.mode import Mode
-from instructor.utils import extract_json_from_codeblock
+from instructor.utils import classproperty, extract_json_from_codeblock
 
 T = TypeVar("T")
 
 logger = logging.getLogger("instructor")
 
 
-class OpenAISchema(BaseModel):  # type: ignore[misc]
-    @classmethod  # type: ignore[misc]
-    @property
-    def openai_schema(cls) -> Dict[str, Any]:
+class OpenAISchema(BaseModel):
+    # Ignore classproperty, since Pydantic doesn't understand it like it would a normal property.
+    model_config = ConfigDict(ignored_types=(classproperty,))
+
+    @classproperty
+    def openai_schema(cls) -> dict[str, Any]:
         """
         Return the schema in the format of OpenAI's schema as jsonschema
 
         Note:
             Its important to add a docstring to describe how to best use this class, it will be included in the description attribute and be part of the prompt.
 
         Returns:
@@ -55,28 +64,27 @@
 
         return {
             "name": schema["title"],
             "description": schema["description"],
             "parameters": parameters,
         }
 
-    @classmethod
-    @property
-    def anthropic_schema(cls) -> Dict[str, Any]:
+    @classproperty
+    def anthropic_schema(cls) -> dict[str, Any]:
         return {
             "name": cls.openai_schema["name"],
             "description": cls.openai_schema["description"],
             "input_schema": cls.model_json_schema(),
         }
 
     @classmethod
     def from_response(
         cls,
         completion: ChatCompletion,
-        validation_context: Optional[Dict[str, Any]] = None,
+        validation_context: Optional[dict[str, Any]] = None,
         strict: Optional[bool] = None,
         mode: Mode = Mode.TOOLS,
     ) -> BaseModel:
         """Execute the function from the response of an openai chat completion
 
         Parameters:
             completion (openai.ChatCompletion): The response from an openai chat completion
@@ -109,116 +117,124 @@
         if mode in {Mode.JSON, Mode.JSON_SCHEMA, Mode.MD_JSON}:
             return cls.parse_json(completion, validation_context, strict)
 
         raise ValueError(f"Invalid patch mode: {mode}")
 
     @classmethod
     def parse_anthropic_tools(
-        cls: Type[BaseModel],
+        cls: type[BaseModel],
         completion: ChatCompletion,
-        validation_context: Optional[Dict[str, Any]] = None,
+        validation_context: Optional[dict[str, Any]] = None,
         strict: Optional[bool] = None,
     ) -> BaseModel:
-        tool_calls = [c.input for c in completion.content if c.type == "tool_use"]
+        tool_calls = [c.input for c in completion.content if c.type == "tool_use"]  # type: ignore - TODO update with anthropic specific types
 
         tool_calls_validator = TypeAdapter(
-            Annotated[list, Field(min_length=1, max_length=1)]
+            Annotated[list[Any], Field(min_length=1, max_length=1)]
         )
         tool_call = tool_calls_validator.validate_python(tool_calls)[0]
 
-        return cls.model_validate(tool_call, context=validation_context, strict=strict)  # type:ignore
+        return cls.model_validate(tool_call, context=validation_context, strict=strict)
 
     @classmethod
     def parse_anthropic_json(
-        cls: Type[BaseModel],
-        completion,
-        validation_context: Optional[Dict[str, Any]] = None,
+        cls: type[BaseModel],
+        completion: ChatCompletion,
+        validation_context: Optional[dict[str, Any]] = None,
         strict: Optional[bool] = None,
     ) -> BaseModel:
         from anthropic.types import Message
 
         assert isinstance(completion, Message)
 
         text = completion.content[0].text
         extra_text = extract_json_from_codeblock(text)
-        return cls.model_validate_json(
-            extra_text, context=validation_context, strict=strict
-        )
+
+        if strict:
+            return cls.model_validate_json(
+                extra_text, context=validation_context, strict=True
+            )
+        else:
+            # Allow control characters.
+            parsed = json.loads(extra_text, strict=False)
+            # Pydantic non-strict: https://docs.pydantic.dev/latest/concepts/strict_mode/
+            return cls.model_validate(parsed, context=validation_context, strict=False)
 
     @classmethod
     def parse_cohere_tools(
-        cls: Type[BaseModel],
-        completion,
-        validation_context: Optional[Dict[str, Any]] = None,
+        cls: type[BaseModel],
+        completion: ChatCompletion,
+        validation_context: Optional[dict[str, Any]] = None,
         strict: Optional[bool] = None,
     ) -> BaseModel:
-        text = completion.text
+        text = cast(str, completion.text)  # type: ignore - TODO update with cohere specific types
         extra_text = extract_json_from_codeblock(text)
         return cls.model_validate_json(
             extra_text, context=validation_context, strict=strict
         )
 
     @classmethod
     def parse_functions(
-        cls: Type[BaseModel],
+        cls: type[BaseModel],
         completion: ChatCompletion,
-        validation_context: Optional[Dict[str, Any]] = None,
+        validation_context: Optional[dict[str, Any]] = None,
         strict: Optional[bool] = None,
     ) -> BaseModel:
         message = completion.choices[0].message
         assert (
             message.function_call.name == cls.openai_schema["name"]  # type: ignore[index]
         ), "Function name does not match"
         return cls.model_validate_json(
             message.function_call.arguments,  # type: ignore[attr-defined]
             context=validation_context,
             strict=strict,
         )
 
     @classmethod
     def parse_tools(
-        cls: Type[BaseModel],
+        cls: type[BaseModel],
         completion: ChatCompletion,
-        validation_context: Optional[Dict[str, Any]] = None,
+        validation_context: Optional[dict[str, Any]] = None,
         strict: Optional[bool] = None,
     ) -> BaseModel:
         message = completion.choices[0].message
         assert (
             len(message.tool_calls or []) == 1
         ), "Instructor does not support multiple tool calls, use List[Model] instead."
         tool_call = message.tool_calls[0]  # type: ignore
         assert (
             tool_call.function.name == cls.openai_schema["name"]  # type: ignore[index]
         ), "Tool name does not match"
         return cls.model_validate_json(
-            tool_call.function.arguments,
+            tool_call.function.arguments,  # type: ignore
             context=validation_context,
             strict=strict,
         )
 
     @classmethod
     def parse_json(
-        cls: Type[BaseModel],
+        cls: type[BaseModel],
         completion: ChatCompletion,
-        validation_context: Optional[Dict[str, Any]] = None,
+        validation_context: Optional[dict[str, Any]] = None,
         strict: Optional[bool] = None,
     ) -> BaseModel:
         message = completion.choices[0].message.content or ""
         message = extract_json_from_codeblock(message)
 
         return cls.model_validate_json(
             message,
             context=validation_context,
             strict=strict,
         )
 
 
-def openai_schema(cls: Type[BaseModel]) -> OpenAISchema:
+def openai_schema(cls: type[BaseModel]) -> OpenAISchema:
     if not issubclass(cls, BaseModel):
         raise TypeError("Class must be a subclass of pydantic.BaseModel")
 
-    return wraps(cls, updated=())(
+    shema = wraps(cls, updated=())(
         create_model(
             cls.__name__ if hasattr(cls, "__name__") else str(cls),
             __base__=(cls, OpenAISchema),
         )
-    )  # type: ignore[all]
+    )
+    return cast(OpenAISchema, shema)
```

### Comparing `instructor-1.2.4/instructor/mode.py` & `instructor-1.2.5/instructor/mode.py`

 * *Files identical despite different names*

### Comparing `instructor-1.2.4/instructor/patch.py` & `instructor-1.2.5/instructor/patch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # type: ignore[all]
 from functools import wraps
 from typing import (
     Callable,
     Protocol,
-    Type,
     TypeVar,
     Union,
     overload,
-    Awaitable,
 )
+from collections.abc import Awaitable
 from typing_extensions import ParamSpec
 
 from openai import AsyncOpenAI, OpenAI
 from pydantic import BaseModel
 
 from instructor.process_response import handle_response_model
 from instructor.retry import retry_async, retry_sync
@@ -27,65 +26,59 @@
 T_Retval = TypeVar("T_Retval")
 T_ParamSpec = ParamSpec("T_ParamSpec")
 
 
 class InstructorChatCompletionCreate(Protocol):
     def __call__(
         self,
-        response_model: Type[T_Model] = None,
+        response_model: type[T_Model] = None,
         validation_context: dict = None,
         max_retries: int = 1,
         *args: T_ParamSpec.args,
         **kwargs: T_ParamSpec.kwargs,
-    ) -> T_Model:
-        ...
+    ) -> T_Model: ...
 
 
 class AsyncInstructorChatCompletionCreate(Protocol):
     async def __call__(
         self,
-        response_model: Type[T_Model] = None,
+        response_model: type[T_Model] = None,
         validation_context: dict = None,
         max_retries: int = 1,
         *args: T_ParamSpec.args,
         **kwargs: T_ParamSpec.kwargs,
-    ) -> T_Model:
-        ...
+    ) -> T_Model: ...
 
 
 @overload
 def patch(
     client: OpenAI,
     mode: Mode = Mode.TOOLS,
-) -> OpenAI:
-    ...
+) -> OpenAI: ...
 
 
 @overload
 def patch(
     client: AsyncOpenAI,
     mode: Mode = Mode.TOOLS,
-) -> AsyncOpenAI:
-    ...
+) -> AsyncOpenAI: ...
 
 
 @overload
 def patch(
     create: Callable[T_ParamSpec, T_Retval],
     mode: Mode = Mode.TOOLS,
-) -> InstructorChatCompletionCreate:
-    ...
+) -> InstructorChatCompletionCreate: ...
 
 
 @overload
 def patch(
     create: Awaitable[T_Retval],
     mode: Mode = Mode.TOOLS,
-) -> InstructorChatCompletionCreate:
-    ...
+) -> InstructorChatCompletionCreate: ...
 
 
 def patch(
     client: Union[OpenAI, AsyncOpenAI] = None,
     create: Callable[T_ParamSpec, T_Retval] = None,
     mode: Mode = Mode.TOOLS,
 ) -> Union[OpenAI, AsyncOpenAI]:
@@ -109,15 +102,15 @@
     else:
         raise ValueError("Either client or create must be provided")
 
     func_is_async = is_async(func)
 
     @wraps(func)
     async def new_create_async(
-        response_model: Type[T_Model] = None,
+        response_model: type[T_Model] = None,
         validation_context: dict = None,
         max_retries: int = 1,
         strict: bool = True,
         *args: T_ParamSpec.args,
         **kwargs: T_ParamSpec.kwargs,
     ) -> T_Model:
         response_model, new_kwargs = handle_response_model(
@@ -128,20 +121,20 @@
             response_model=response_model,
             validation_context=validation_context,
             max_retries=max_retries,
             args=args,
             kwargs=new_kwargs,
             strict=strict,
             mode=mode,
-        )  # type: ignore
+        )
         return response
 
     @wraps(func)
     def new_create_sync(
-        response_model: Type[T_Model] = None,
+        response_model: type[T_Model] = None,
         validation_context: dict = None,
         max_retries: int = 1,
         strict: bool = True,
         *args: T_ParamSpec.args,
         **kwargs: T_ParamSpec.kwargs,
     ) -> T_Model:
         response_model, new_kwargs = handle_response_model(
@@ -164,15 +157,15 @@
     if client is not None:
         client.chat.completions.create = new_create
         return client
     else:
         return new_create
 
 
-def apatch(client: AsyncOpenAI, mode: Mode = Mode.TOOLS):
+def apatch(client: AsyncOpenAI, mode: Mode = Mode.TOOLS) -> AsyncOpenAI:
     """
     No longer necessary, use `patch` instead.
 
     Patch the `client.chat.completions.create` method
 
     Enables the following features:
```

### Comparing `instructor-1.2.4/instructor/process_response.py` & `instructor-1.2.5/instructor/process_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # type: ignore[all]
-
 from __future__ import annotations
 
 from collections.abc import Iterable
 from textwrap import dedent
 from instructor.dsl.iterable import IterableBase, IterableModel
 from instructor.dsl.parallel import ParallelBase, ParallelModel, handle_parallel_model
 from instructor.dsl.partial import PartialBase
@@ -13,24 +12,20 @@
 from openai.types.chat import ChatCompletion
 from pydantic import BaseModel
 
 import json
 import inspect
 import logging
 from typing import (
-    Generator,
-    Optional,
-    Type,
-    Tuple,
     get_args,
     get_origin,
     TypeVar,
     Any,
-    Dict,
 )
+from collections.abc import Generator
 from typing_extensions import ParamSpec
 
 from instructor.mode import Mode
 
 logger = logging.getLogger("instructor")
 
 T_Model = TypeVar("T_Model", bound=BaseModel)
@@ -38,18 +33,18 @@
 T_ParamSpec = ParamSpec("T_ParamSpec")
 T = TypeVar("T")
 
 
 async def process_response_async(
     response: ChatCompletion,
     *,
-    response_model: Type[T_Model | OpenAISchema | BaseModel],
+    response_model: type[T_Model | OpenAISchema | BaseModel] | None,
     stream: bool = False,
-    validation_context: Optional[dict] = None,
-    strict: Optional[bool] = None,
+    validation_context: dict[str, Any] | None = None,
+    strict: bool | None = None,
     mode: Mode = Mode.TOOLS,
 ) -> T_Model | ChatCompletion:
     """Processes a OpenAI response with the response model, if available.
     It can use `validation_context` and `strict` to validate the response
     via the pydantic model
 
     Args:
@@ -101,17 +96,17 @@
     model._raw_response = response
     return model
 
 
 def process_response(
     response: T_Model,
     *,
-    response_model: Type[OpenAISchema | BaseModel],
+    response_model: type[OpenAISchema | BaseModel],
     stream: bool,
-    validation_context: Optional[dict] = None,
+    validation_context: dict | None = None,
     strict=None,
     mode: Mode = Mode.TOOLS,
 ) -> T_Model | Generator[T_Model, None, None] | ChatCompletion:
     """Processes a OpenAI response with the response model, if available.
 
     Args:
         response (T): The response from OpenAI's API
@@ -166,16 +161,16 @@
         return model.content
 
     model._raw_response = response
     return model
 
 
 def handle_response_model(
-    response_model: T, mode: Mode = Mode.TOOLS, **kwargs
-) -> Tuple[Type[OpenAISchema], Dict[str, Any]]:
+    response_model: type[T] | None, mode: Mode = Mode.TOOLS, **kwargs: Any
+) -> tuple[type[T], dict[str, Any]]:
     """Prepare the response model type hint, and returns the response_model
     along with the new modified kwargs needed to be able to use the response_model
     parameter with the patch function.
 
 
     Args:
         response_model (T): The response model to use for parsing the response
```

### Comparing `instructor-1.2.4/instructor/retry.py` & `instructor-1.2.5/instructor/retry.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from openai.types.completion_usage import CompletionUsage
 from pydantic import ValidationError
 from tenacity import AsyncRetrying, RetryError, Retrying, stop_after_attempt
 
 
 from json import JSONDecodeError
 from pydantic import BaseModel
-from typing import Callable, Optional, Type, TypeVar
+from typing import Callable, TypeVar, Any
 from typing_extensions import ParamSpec
 
 logger = logging.getLogger("instructor")
 
 T_Model = TypeVar("T_Model", bound=BaseModel)
 T_Retval = TypeVar("T_Retval")
 T_ParamSpec = ParamSpec("T_ParamSpec")
@@ -99,15 +99,15 @@
             "content": f"Validation Error found:\n{exception}\nRecall the function correctly, fix the errors",
         }
         return
 
     yield dump_message(response.choices[0].message)
     # TODO: Give users more control on configuration
     if mode == Mode.TOOLS:
-        for tool_call in response.choices[0].message.tool_calls:  # type: ignore
+        for tool_call in response.choices[0].message.tool_calls:
             yield {
                 "role": "tool",
                 "tool_call_id": tool_call.id,
                 "name": tool_call.function.name,
                 "content": f"Validation Error found:\n{exception}\nRecall the function correctly, fix the errors",
             }
     elif mode == Mode.MD_JSON:
@@ -120,20 +120,20 @@
             "role": "user",
             "content": f"Recall the function correctly, fix the errors, exceptions found\n{exception}",
         }
 
 
 def retry_sync(
     func: Callable[T_ParamSpec, T_Retval],
-    response_model: Type[T_Model],
+    response_model: type[T_Model],
     validation_context: dict,
     args,
     kwargs,
     max_retries: int | Retrying = 1,
-    strict: Optional[bool] = None,
+    strict: bool | None = None,
     mode: Mode = Mode.TOOLS,
 ) -> T_Model:
     total_usage = CompletionUsage(completion_tokens=0, prompt_tokens=0, total_tokens=0)
     if mode in {Mode.ANTHROPIC_TOOLS, Mode.ANTHROPIC_JSON}:
         from anthropic.types import Usage as AnthropicUsage
 
         total_usage = AnthropicUsage(input_tokens=0, output_tokens=0)
@@ -185,20 +185,20 @@
             messages=kwargs["messages"],
             total_usage=total_usage,
         ) from e
 
 
 async def retry_async(
     func: Callable[T_ParamSpec, T_Retval],
-    response_model: Type[T],
-    validation_context,
-    args,
-    kwargs,
+    response_model: type[T] | None,
+    validation_context: dict[str, Any] | None,
+    args: Any,
+    kwargs: Any,
     max_retries: int | AsyncRetrying = 1,
-    strict: Optional[bool] = None,
+    strict: bool | None = None,
     mode: Mode = Mode.TOOLS,
 ) -> T:
     total_usage = CompletionUsage(completion_tokens=0, prompt_tokens=0, total_tokens=0)
     if mode in {Mode.ANTHROPIC_TOOLS, Mode.ANTHROPIC_JSON}:
         from anthropic.types import Usage as AnthropicUsage
 
         total_usage = AnthropicUsage(input_tokens=0, output_tokens=0)
@@ -216,25 +216,25 @@
         )
 
     try:
         async for attempt in max_retries:
             logger.debug(f"Retrying, attempt: {attempt}")
             with attempt:
                 try:
-                    response: ChatCompletion = await func(*args, **kwargs)  # type: ignore
+                    response: ChatCompletion = await func(*args, **kwargs)
                     stream = kwargs.get("stream", False)
                     response = update_total_usage(response, total_usage)
                     return await process_response_async(
                         response,
                         response_model=response_model,
                         stream=stream,
                         validation_context=validation_context,
                         strict=strict,
                         mode=mode,
-                    )  # type: ignore[all]
+                    )
                 except (ValidationError, JSONDecodeError) as e:
                     logger.debug(f"Error response: {response}", e)
                     kwargs["messages"].extend(reask_messages(response, mode, e))
                     if mode in {Mode.ANTHROPIC_TOOLS, Mode.ANTHROPIC_JSON}:
                         kwargs["messages"] = merge_consecutive_messages(
                             kwargs["messages"]
                         )
```

### Comparing `instructor-1.2.4/instructor/utils.py` & `instructor-1.2.5/instructor/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,42 @@
 from __future__ import annotations
 
 import inspect
 import json
 import logging
-from typing import Callable, Generator, Iterable, AsyncGenerator, TypeVar
-
-from pydantic import BaseModel
+from typing import (
+    Callable,
+    Generic,
+    Protocol,
+    TypeVar,
+)
+from collections.abc import Generator, Iterable, AsyncGenerator
+from typing import Callable, Protocol, TypeVar
+from collections.abc import Generator, Iterable, AsyncGenerator
+from openai.types.completion_usage import CompletionUsage
+from anthropic.types import Usage as AnthropicUsage
+from typing import Any
 from openai.types import CompletionUsage as OpenAIUsage
 from openai.types.chat import (
     ChatCompletion,
     ChatCompletionMessage,
     ChatCompletionMessageParam,
 )
 
 logger = logging.getLogger("instructor")
-T_Model = TypeVar("T_Model", bound=BaseModel)
+R_co = TypeVar("R_co", covariant=True)
+T_Model = TypeVar("T_Model", bound="Response")
 
 from enum import Enum
 
 
+class Response(Protocol):
+    usage: OpenAIUsage | AnthropicUsage
+
+
 class Provider(Enum):
     OPENAI = "openai"
     ANTHROPIC = "anthropic"
     ANYSCALE = "anyscale"
     TOGETHER = "together"
     GROQ = "groq"
     MISTRAL = "mistral"
@@ -90,28 +104,35 @@
                 if brace_count == 0:
                     capturing = False
                     break  # Cease yielding upon closing the current JSON object
             elif capturing:
                 yield char
 
 
-def update_total_usage(response: T_Model, total_usage) -> T_Model | ChatCompletion:
+def update_total_usage(
+    response: T_Model,
+    total_usage: CompletionUsage | AnthropicUsage,
+) -> T_Model | ChatCompletion:
     response_usage = getattr(response, "usage", None)
-    if isinstance(response_usage, OpenAIUsage):
+    if isinstance(response_usage, OpenAIUsage) and isinstance(
+        total_usage, CompletionUsage
+    ):
         total_usage.completion_tokens += response_usage.completion_tokens or 0
         total_usage.prompt_tokens += response_usage.prompt_tokens or 0
         total_usage.total_tokens += response_usage.total_tokens or 0
         response.usage = total_usage  # Replace each response usage with the total usage
         return response
 
-    # Anthropic usage
+    # Anthropic usage.
     try:
         from anthropic.types import Usage as AnthropicUsage
 
-        if isinstance(response_usage, AnthropicUsage):
+        if isinstance(response_usage, AnthropicUsage) and isinstance(
+            total_usage, AnthropicUsage
+        ):
             total_usage.input_tokens += response_usage.input_tokens or 0
             total_usage.output_tokens += response_usage.output_tokens or 0
             response.usage = total_usage
             return response
     except ImportError:
         pass
 
@@ -135,26 +156,26 @@
         and message.function_call is not None
         and ret["content"]
     ):
         ret["content"] += json.dumps(message.model_dump()["function_call"])
     return ret
 
 
-def is_async(func: Callable) -> bool:
+def is_async(func: Callable[..., Any]) -> bool:
     """Returns true if the callable is async, accounting for wrapped callables"""
     is_coroutine = inspect.iscoroutinefunction(func)
     while hasattr(func, "__wrapped__"):
-        func = func.__wrapped__
+        func = func.__wrapped__  # type: ignore - dynamic
         is_coroutine = is_coroutine or inspect.iscoroutinefunction(func)
     return is_coroutine
 
 
-def merge_consecutive_messages(messages: list[dict]) -> list[dict]:
+def merge_consecutive_messages(messages: list[dict[str, Any]]) -> list[dict[str, Any]]:
     # merge all consecutive user messages into a single message
-    new_messages = []
+    new_messages: list[dict[str, Any]] = []
     for message in messages:
         new_content = message["content"]
         if isinstance(new_content, str):
             new_content = [{"type": "text", "text": new_content}]
 
         if len(new_messages) > 0 and message["role"] == new_messages[-1]["role"]:
             new_messages[-1]["content"].extend(new_content)
@@ -163,7 +184,28 @@
                 {
                     "role": message["role"],
                     "content": new_content,
                 }
             )
 
     return new_messages
+
+
+class classproperty(Generic[R_co]):
+    """Descriptor for class-level properties.
+
+    Examples:
+        >>> from instructor.utils import classproperty
+
+        >>> class MyClass:
+        ...     @classproperty
+        ...     def my_property(cls):
+        ...         return cls
+
+        >>> assert MyClass.my_property
+    """
+
+    def __init__(self, method: Callable[[Any], R_co]) -> None:
+        self.cproperty = method
+
+    def __get__(self, instance: object, cls: type[Any]) -> R_co:
+        return self.cproperty(cls)
```

### Comparing `instructor-1.2.4/pyproject.toml` & `instructor-1.2.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,57 +1,58 @@
 [tool.poetry]
 name = "instructor"
-version = "1.2.4"
+version = "1.2.5"
 description = "structured outputs for llm"
 authors = ["Jason Liu <jason@jxnl.co>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "instructor"}]
 repository = "https://github.com/jxnl/instructor"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 openai = "^1.1.0"
-pydantic = "2.7.0"
+pydantic = "^2.7.0"
 docstring-parser = "^0.16"
 typer = ">=0.9.0,<1.0.0"
 rich = "^13.7.0"
 aiohttp = "^3.9.1"
 tenacity = "^8.2.3"
 pydantic-core = "^2.18.0"
 
 # dependency versions for extras
 fastapi = { version = "^0.109.2", optional = true }
 redis = { version = "^5.0.1", optional = true }
 diskcache = { version = "^5.6.3", optional = true }
 pandas = { version = "^2.2.0", optional = true }
 tabulate = { version = "^0.9.0", optional = true }
 pydantic_extra_types = { version = "^2.6.0", optional = true }
-litellm = { version = "^1.0.0", optional = true }
+litellm = { version = "^1.35.31", optional = true }
 anthropic = { version = "^0.23.1", optional = true }
 xmltodict = { version = "^0.13.0", optional = true }
 groq = { version = "^0.4.2", optional = true }
 cohere = { version = "^5.1.8", optional = true }
 mistralai = { version = "^0.1.8", optional = true }
 
 [tool.poetry.extras]
 anthropic = ["anthropic", "xmltodict"]
 groq = ["groq"]
 cohere = ["cohere"]
 test-docs = ["fastapi", "redis", "diskcache", "pandas", "tabulate", "pydantic_extra_types", "litellm", "anthropic", "groq", "cohere", "mistralai"]
 mistralai = ["mistralai"]
+litellm = ["litellm"]
 
 [tool.poetry.scripts]
 instructor = "instructor.cli.cli:app"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.0"
 pytest-asyncio = "^0.21.1"
 coverage = "^7.3.2"
-mypy = "^1.7.1"
+pyright = "^1.1.360"
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.4.3"
 mkdocs-material = {extras = ["imaging"], version = "^9.5.9"}
 mkdocstrings = "^0.22.0"
 mkdocstrings-python = "^1.1.2"
 pytest-examples = "^0.0.10"
@@ -66,18 +67,36 @@
 [tool.poetry.group.test-docs.dependencies]
 fastapi = "^0.109.2"
 redis = "^5.0.1"
 diskcache = "^5.6.3"
 pandas = "^2.2.0"
 tabulate = "^0.9.0"
 pydantic_extra_types = "^2.6.0"
-litellm = "^1.0.0"
+litellm = "^1.35.31"
 anthropic = "^0.23.1"
 xmltodict = "^0.13.0"
 groq = "^0.4.2"
 phonenumbers = "^8.13.33"
 cohere = "^5.1.8"
 mistralai = "^0.1.8"
 
+[tool.poetry.group.litellm.dependencies]
+litellm = "^1.35.31"
+
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
+
+[tool.pyright]
+include = ["instructor"]
+exclude = [
+    "**/node_modules",
+    "**/__pycache__",
+    "src/experimental",
+    "src/typestubs",
+    "**/tests/**",
+]
+pythonVersion = "3.9"
+typeCheckingMode = "strict"
+# Allow "redundant" runtime type-checking.
+reportUnnecessaryIsInstance = "none"
+reportUnnecessaryTypeIgnoreComment = "error"
```

### Comparing `instructor-1.2.4/PKG-INFO` & `instructor-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: instructor
-Version: 1.2.4
+Version: 1.2.5
 Summary: structured outputs for llm
 Home-page: https://github.com/jxnl/instructor
 License: MIT
 Author: Jason Liu
 Author-email: jason@jxnl.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -12,28 +12,29 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: anthropic
 Provides-Extra: cohere
 Provides-Extra: groq
+Provides-Extra: litellm
 Provides-Extra: mistralai
 Provides-Extra: test-docs
 Requires-Dist: aiohttp (>=3.9.1,<4.0.0)
 Requires-Dist: anthropic (>=0.23.1,<0.24.0) ; extra == "anthropic" or extra == "test-docs"
 Requires-Dist: cohere (>=5.1.8,<6.0.0) ; extra == "cohere" or extra == "test-docs"
 Requires-Dist: diskcache (>=5.6.3,<6.0.0) ; extra == "test-docs"
 Requires-Dist: docstring-parser (>=0.16,<0.17)
 Requires-Dist: fastapi (>=0.109.2,<0.110.0) ; extra == "test-docs"
 Requires-Dist: groq (>=0.4.2,<0.5.0) ; extra == "groq" or extra == "test-docs"
-Requires-Dist: litellm (>=1.0.0,<2.0.0) ; extra == "test-docs"
+Requires-Dist: litellm (>=1.35.31,<2.0.0) ; extra == "test-docs" or extra == "litellm"
 Requires-Dist: mistralai (>=0.1.8,<0.2.0) ; extra == "test-docs" or extra == "mistralai"
 Requires-Dist: openai (>=1.1.0,<2.0.0)
 Requires-Dist: pandas (>=2.2.0,<3.0.0) ; extra == "test-docs"
-Requires-Dist: pydantic (==2.7.0)
+Requires-Dist: pydantic (>=2.7.0,<3.0.0)
 Requires-Dist: pydantic-core (>=2.18.0,<3.0.0)
 Requires-Dist: pydantic_extra_types (>=2.6.0,<3.0.0) ; extra == "test-docs"
 Requires-Dist: redis (>=5.0.1,<6.0.0) ; extra == "test-docs"
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0) ; extra == "test-docs"
 Requires-Dist: tenacity (>=8.2.3,<9.0.0)
 Requires-Dist: typer (>=0.9.0,<1.0.0)
```

