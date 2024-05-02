# Comparing `tmp/hacktegic-0.1.9.tar.gz` & `tmp/hacktegic-0.2.0.tar.gz`

## Comparing `hacktegic-0.1.9.tar` & `hacktegic-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,46 @@
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 hacktegic-0.1.9/requirements.txt
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/__main__.py
--rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/base_command.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/config.py
--rw-r--r--   0        0        0     2859 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/credentials.py
--rw-r--r--   0        0        0     4557 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/parser.py
--rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/assets/cidr/create.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/assets/cidr/delete.py
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/assets/cidr/describe.py
--rw-r--r--   0        0        0     1042 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/assets/cidr/list.py
--rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/assets/cidr/update.py
--rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/auth/login.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/auth/logout.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/auth/register.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/config/get.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/config/set.py
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/projects/create.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/projects/delete.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/projects/describe.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/projects/list.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/_internal/commands/projects/update.py
--rw-r--r--   0        0        0     3147 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/cloud/api_clients/assets_cidr.py
--rw-r--r--   0        0        0     2532 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/cloud/api_clients/projects.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/cloud/resources/assets_cidr.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 hacktegic-0.1.9/hacktegic/cloud/resources/projects.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 hacktegic-0.1.9/.gitignore
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hacktegic-0.1.9/LICENSE
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 hacktegic-0.1.9/README.md
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 hacktegic-0.1.9/pyproject.toml
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 hacktegic-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 hacktegic-0.2.0/requirements.txt
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/__main__.py
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/base_command.py
+-rw-r--r--   0        0        0     1492 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/config.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/credentials.py
+-rw-r--r--   0        0        0    10712 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/parser.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/commands/auth/login.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/commands/auth/logout.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/commands/auth/register.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/commands/config/get.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/commands/config/set.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/commands/networks/create.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/commands/networks/delete.py
+-rw-r--r--   0        0        0     1549 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/commands/networks/describe.py
+-rw-r--r--   0        0        0     1032 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/commands/networks/list.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/commands/networks/update.py
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/commands/projects/create.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/commands/projects/delete.py
+-rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/commands/projects/describe.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/commands/projects/list.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/commands/projects/update.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/commands/scanprofiles/create.py
+-rw-r--r--   0        0        0     1018 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/commands/scanprofiles/delete.py
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/commands/scanprofiles/describe.py
+-rw-r--r--   0        0        0     1216 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/commands/scanprofiles/list.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/commands/scanprofiles/networks_attach.py
+-rw-r--r--   0        0        0     1048 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/commands/scanprofiles/networks_detach.py
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/commands/scanprofiles/networks_list.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/commands/scanprofiles/portscans_run.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/commands/scanprofiles/update.py
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/commands/scans/delete.py
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/commands/scans/describe.py
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/_internal/commands/scans/list.py
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/cloud/api_clients/networks.py
+-rw-r--r--   0        0        0     2492 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/cloud/api_clients/projects.py
+-rw-r--r--   0        0        0     6736 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/cloud/api_clients/scanprofiles.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/cloud/api_clients/scans.py
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/cloud/resources/networks.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/cloud/resources/projects.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/cloud/resources/scanprofiles.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 hacktegic-0.2.0/hacktegic/cloud/resources/scans.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 hacktegic-0.2.0/.gitignore
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 hacktegic-0.2.0/LICENSE
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 hacktegic-0.2.0/README.md
+-rw-r--r--   0        0        0     1240 2020-02-02 00:00:00.000000 hacktegic-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      867 2020-02-02 00:00:00.000000 hacktegic-0.2.0/PKG-INFO
```

### Comparing `hacktegic-0.1.9/hacktegic/__main__.py` & `hacktegic-0.2.0/hacktegic/__main__.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.9/hacktegic/_internal/config.py` & `hacktegic-0.2.0/hacktegic/_internal/config.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,22 +17,30 @@
         }
         self.config = {}
 
     async def load(self) -> None:
         """
         Load the config.
         """
+        for key in self.__default_config:
+            env_key = f"HACKTEGIC_{key.upper()}"
+            if env_key in os.environ:
+                self.config[key] = os.environ[env_key]
+
         if os.path.exists(self.__config_path):
             async with aiofiles.open(self.__config_path, mode="r") as f:
                 doc = tomlkit.loads(await f.read())
-                self.config = doc["hacktegic"]
+                file_config = doc.get("hacktegic", {})
+                for key, value in file_config.items():
+                    if key not in self.config:
+                        self.config[key] = value
 
-        for k, v in self.__default_config.items():
-            if k not in self.config:
-                self.config[k] = v
+        for key, default_value in self.__default_config.items():
+            if key not in self.config:
+                self.config[key] = default_value
 
     async def save(self) -> None:
         """
         Save the config to file.
         """
         async with aiofiles.open(self.__config_path, mode="w") as f:
             await f.write(tomlkit.dumps({"hacktegic": self.config}))
```

### Comparing `hacktegic-0.1.9/hacktegic/_internal/credentials.py` & `hacktegic-0.2.0/hacktegic/_internal/credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
         from hacktegic._internal.config import ConfigManager
 
         config_manager = ConfigManager()
         await config_manager.load()
 
         async with aiohttp.ClientSession() as session:
-            url = f'{config_manager.config["api_base_url"]}v1/general/me'
+            url = f'{config_manager.config["api_base_url"]}v1/me'
             headers = {"Authorization": f"Bearer {self.__access_token}"}
 
             async with session.get(url, headers=headers) as response:
                 return response.status == 200
 
     async def refresh(self) -> None:
         pass
```

### Comparing `hacktegic-0.1.9/hacktegic/_internal/commands/assets/cidr/create.py` & `hacktegic-0.2.0/hacktegic/_internal/commands/scans/delete.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,36 +3,30 @@
 
 from rich.console import Console
 from rich.text import Text
 
 from hacktegic._internal.base_command import BaseCommand
 from hacktegic._internal.config import ConfigManager
 from hacktegic._internal.credentials import Credentials
-from hacktegic.cloud.api_clients.assets_cidr import AssetsCIDRAPIClient
+from hacktegic.cloud.api_clients.scans import ScansAPIClient
 
-
-class AssetsCIDRCreateCommand(BaseCommand):
+class ScansDeleteCommand(BaseCommand):
     @staticmethod
     async def run(tg: TaskGroup, args: Namespace) -> None:
         creds = Credentials()
         config_manager = ConfigManager()
         await creds.load()
         await config_manager.load()
 
-        client = AssetsCIDRAPIClient(creds, config_manager)
-
+        client = ScansAPIClient(creds, config_manager)
         console = Console()
 
-        asset = {"address": args.address}
-        if hasattr(args, "description"):
-            asset["description"] = args.description
-
-        result = await client.create(asset)
+        result = await client.delete(args.scan_id)
 
-        if result.id:
-            text = Text("Asset successfully created!")
+        if result:
+            text = Text("Scan successfully deleted!")
             text.stylize("green")
         else:
             text = Text("Something went wrong!")
             text.stylize("bold red")
 
-        console.print(text)
+        console.print(text)
```

### Comparing `hacktegic-0.1.9/hacktegic/_internal/commands/assets/cidr/delete.py` & `hacktegic-0.2.0/hacktegic/_internal/commands/networks/delete.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,30 +3,29 @@
 
 from rich.console import Console
 from rich.text import Text
 
 from hacktegic._internal.base_command import BaseCommand
 from hacktegic._internal.config import ConfigManager
 from hacktegic._internal.credentials import Credentials
-from hacktegic.cloud.api_clients.assets_cidr import AssetsCIDRAPIClient
+from hacktegic.cloud.api_clients.networks import NetworksAPIClient
 
-
-class AssetsCIDRDeleteCommand(BaseCommand):
+class NetworksDeleteCommand(BaseCommand):
     @staticmethod
     async def run(tg: TaskGroup, args: Namespace) -> None:
         creds = Credentials()
         config_manager = ConfigManager()
         await creds.load()
         await config_manager.load()
 
-        client = AssetsCIDRAPIClient(creds, config_manager)
+        client = NetworksAPIClient(creds, config_manager)
 
-        results = await client.delete(args.asset_id)
+        result = await client.delete(args.network_id)
 
-        if results:
-            text = Text("Project successfully deleted!")
+        if result:
+            text = Text("Network successfully deleted!")
             text.stylize("green")
         else:
             text = Text("Something went wrong!")
             text.stylize("bold red")
         console = Console()
         console.print(text)
```

### Comparing `hacktegic-0.1.9/hacktegic/_internal/commands/assets/cidr/describe.py` & `hacktegic-0.2.0/hacktegic/_internal/commands/projects/describe.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,37 +4,36 @@
 from rich.console import Console
 from rich.style import Style
 from rich.text import Text
 
 from hacktegic._internal.base_command import BaseCommand
 from hacktegic._internal.config import ConfigManager
 from hacktegic._internal.credentials import Credentials
-from hacktegic.cloud.api_clients.assets_cidr import AssetsCIDRAPIClient
+from hacktegic.cloud.api_clients.projects import ProjectsAPIClient
 
 
-class AssetsCIDRDescribeCommand(BaseCommand):
+class ProjectsDescribeCommand(BaseCommand):
     @staticmethod
     async def run(tg: TaskGroup, args: Namespace) -> None:
         creds = Credentials()
         config_manager = ConfigManager()
         await creds.load()
         await config_manager.load()
 
-        client = AssetsCIDRAPIClient(creds, config_manager)
+        client = ProjectsAPIClient(creds, config_manager)
 
-        result = await client.describe(args.asset_id)
+        result = await client.describe(args.project_id)
 
         console = Console()
 
         if result:
             result_info = [
                 ("UUID", result.id),
-                ("Address", result.address),
-                ("Description", result.description),
-                ("Project ID", result.project_id),
+                ("Name", result.name),
+                ("Owner", result.owner_id),
                 ("Created At", result.created_at),
                 ("Updated At", result.updated_at),
             ]
 
             text = Text()
             for label, value in result_info:
                 label_style = Style(color="magenta", bold=True)
```

### Comparing `hacktegic-0.1.9/hacktegic/_internal/commands/assets/cidr/list.py` & `hacktegic-0.2.0/hacktegic/_internal/commands/projects/list.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,30 +3,29 @@
 
 from rich.console import Console
 from rich.table import Table
 
 from hacktegic._internal.base_command import BaseCommand
 from hacktegic._internal.config import ConfigManager
 from hacktegic._internal.credentials import Credentials
-from hacktegic.cloud.api_clients.assets_cidr import AssetsCIDRAPIClient
+from hacktegic.cloud.api_clients.projects import ProjectsAPIClient
 
 
-class AssetsCIDRListCommand(BaseCommand):
+class ProjectsListCommand(BaseCommand):
     @staticmethod
     async def run(tg: TaskGroup, args: Namespace) -> None:
         creds = Credentials()
         config_manager = ConfigManager()
         await creds.load()
         await config_manager.load()
 
-        client = AssetsCIDRAPIClient(creds, config_manager)
+        client = ProjectsAPIClient(creds, config_manager)
 
         table = Table()
         table.add_column("UUID")
-        table.add_column("Address", style="magenta")
-        table.add_column("Description")
+        table.add_column("Name", style="magenta")
         table.add_column("Created At")
 
         for i in await client.list():
-            table.add_row(i.id, i.address, i.description, str(i.created_at))
+            table.add_row(i.id, i.name, str(i.created_at))
         console = Console()
         console.print(table)
```

### Comparing `hacktegic-0.1.9/hacktegic/_internal/commands/assets/cidr/update.py` & `hacktegic-0.2.0/hacktegic/_internal/commands/networks/create.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,37 +3,35 @@
 
 from rich.console import Console
 from rich.text import Text
 
 from hacktegic._internal.base_command import BaseCommand
 from hacktegic._internal.config import ConfigManager
 from hacktegic._internal.credentials import Credentials
-from hacktegic.cloud.api_clients.assets_cidr import AssetsCIDRAPIClient
+from hacktegic.cloud.api_clients.networks import NetworksAPIClient
 
 
-class AssetsCIDRUpdateCommand(BaseCommand):
-    @staticmethod
+class NetworksCreateCommand(BaseCommand):
     async def run(tg: TaskGroup, args: Namespace) -> None:
         creds = Credentials()
         config_manager = ConfigManager()
         await creds.load()
         await config_manager.load()
 
-        client = AssetsCIDRAPIClient(creds, config_manager)
+        client = NetworksAPIClient(creds, config_manager)
 
         console = Console()
 
-        asset = {}
-        if hasattr(args, "address") and args.address:
-            asset["address"] = args.address
+        network = {"address": args.address}
         if hasattr(args, "description"):
-            asset["description"] = args.description
+            network["description"] = args.description
 
-        result = await client.update(args.asset_id, asset)
+        result = await client.create(network)
 
-        if result:
-            text = Text("Asset successfully updated!")
+        if result.id:
+            text = Text("Network successfully created!")
             text.stylize("green")
         else:
             text = Text("Something went wrong!")
             text.stylize("bold red")
+
         console.print(text)
```

### Comparing `hacktegic-0.1.9/hacktegic/_internal/commands/auth/login.py` & `hacktegic-0.2.0/hacktegic/_internal/commands/auth/login.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.9/hacktegic/_internal/commands/auth/logout.py` & `hacktegic-0.2.0/hacktegic/_internal/commands/auth/logout.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.9/hacktegic/_internal/commands/auth/register.py` & `hacktegic-0.2.0/hacktegic/_internal/commands/auth/register.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.9/hacktegic/_internal/commands/config/get.py` & `hacktegic-0.2.0/hacktegic/_internal/commands/config/get.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.9/hacktegic/_internal/commands/config/set.py` & `hacktegic-0.2.0/hacktegic/_internal/commands/config/set.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.9/hacktegic/_internal/commands/projects/create.py` & `hacktegic-0.2.0/hacktegic/_internal/commands/projects/create.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.9/hacktegic/_internal/commands/projects/delete.py` & `hacktegic-0.2.0/hacktegic/_internal/commands/projects/delete.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.9/hacktegic/_internal/commands/projects/describe.py` & `hacktegic-0.2.0/hacktegic/_internal/commands/scans/describe.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 from argparse import Namespace
 from asyncio import TaskGroup
 
+from rich.text import Text
 from rich.console import Console
 from rich.style import Style
-from rich.text import Text
 
 from hacktegic._internal.base_command import BaseCommand
 from hacktegic._internal.config import ConfigManager
 from hacktegic._internal.credentials import Credentials
-from hacktegic.cloud.api_clients.projects import ProjectsAPIClient
+from hacktegic.cloud.api_clients.scans import ScansAPIClient
 
-
-class ProjectsDescribeCommand(BaseCommand):
+class ScansDescribeCommand(BaseCommand):
     @staticmethod
     async def run(tg: TaskGroup, args: Namespace) -> None:
         creds = Credentials()
         config_manager = ConfigManager()
         await creds.load()
         await config_manager.load()
 
-        client = ProjectsAPIClient(creds, config_manager)
+        client = ScansAPIClient(creds, config_manager)
 
-        result = await client.describe(args.project_id)
+        result = await client.describe(args.scan_id)
 
         console = Console()
 
         if result:
             result_info = [
                 ("UUID", result.id),
-                ("Name", result.name),
-                ("Owner", result.owner_id),
+                ("Status", result.status),
+                ("scan_profile_id", result.scan_profile_id),
                 ("Created At", result.created_at),
                 ("Updated At", result.updated_at),
+                ("Deleted At", result.deleted_at),
             ]
 
             text = Text()
             for label, value in result_info:
                 label_style = Style(color="magenta", bold=True)
 
                 text.append(Text(label + ": ", style=label_style))
                 text.append(Text(str(value)))
                 text.append("\n")
         else:
             text = Text("Something went wrong!")
             text.stylize("bold red")
-
         console.print(text)
```

### Comparing `hacktegic-0.1.9/hacktegic/_internal/commands/projects/list.py` & `hacktegic-0.2.0/hacktegic/_internal/commands/networks/list.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,29 +3,30 @@
 
 from rich.console import Console
 from rich.table import Table
 
 from hacktegic._internal.base_command import BaseCommand
 from hacktegic._internal.config import ConfigManager
 from hacktegic._internal.credentials import Credentials
-from hacktegic.cloud.api_clients.projects import ProjectsAPIClient
+from hacktegic.cloud.api_clients.networks import NetworksAPIClient
 
-
-class ProjectsListCommand(BaseCommand):
+class NetworksListCommand(BaseCommand):
     @staticmethod
     async def run(tg: TaskGroup, args: Namespace) -> None:
         creds = Credentials()
         config_manager = ConfigManager()
+
         await creds.load()
         await config_manager.load()
 
-        client = ProjectsAPIClient(creds, config_manager)
+        client = NetworksAPIClient(creds, config_manager)
 
         table = Table()
         table.add_column("UUID")
-        table.add_column("Name", style="magenta")
+        table.add_column("Address", style="magenta")
+        table.add_column("Description")
         table.add_column("Created At")
 
         for i in await client.list():
-            table.add_row(i.id, i.name, str(i.created_at))
+            table.add_row(i.id, i.address, i.description, str(i.created_at))
         console = Console()
-        console.print(table)
+        console.print(table)
```

### Comparing `hacktegic-0.1.9/hacktegic/_internal/commands/projects/update.py` & `hacktegic-0.2.0/hacktegic/_internal/commands/projects/update.py`

 * *Files identical despite different names*

### Comparing `hacktegic-0.1.9/hacktegic/cloud/api_clients/assets_cidr.py` & `hacktegic-0.2.0/hacktegic/cloud/api_clients/networks.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,56 +1,56 @@
 import aiohttp
 
 from hacktegic._internal.config import ConfigManager
 from hacktegic._internal.credentials import Credentials
-from hacktegic.cloud.resources.assets_cidr import AssetsCIDR
+from hacktegic.cloud.resources.networks import Networks
 
 
-class AssetsCIDRAPIClient:
+class NetworksAPIClient:
     def __init__(self, credentials: Credentials, config_manager: ConfigManager) -> None:
         self.credentials = credentials
         self.config_manager = config_manager
 
-    async def create(self, asset_cidr: dict) -> AssetsCIDR:
+    async def create(self, network: dict) -> Networks:
         async with aiohttp.ClientSession() as session:
             base_url = self.config_manager.config["api_base_url"]
             project_id = self.config_manager.config["project_id"]
-            url = f"{base_url}v1/general/projects/{project_id}/assets/cidr"
+            url = f"{base_url}v1/projects/{project_id}/networks"
             headers = {"Authorization": f"Bearer {self.credentials.access_token}"}
-            async with session.post(url, headers=headers, json=asset_cidr) as response:
-                return AssetsCIDR(**(await response.json()))
+            async with session.post(url, headers=headers, json=network) as response:
+                return Networks(**(await response.json()))
 
-    async def list(self) -> list[AssetsCIDR]:
+    async def list(self) -> list[Networks]:
         async with aiohttp.ClientSession() as session:
             base_url = self.config_manager.config["api_base_url"]
             project_id = self.config_manager.config["project_id"]
-            url = f"{base_url}v1/general/projects/{project_id}/assets/cidr"
+            url = f"{base_url}v1/projects/{project_id}/networks"
             headers = {"Authorization": f"Bearer {self.credentials.access_token}"}
             async with session.get(url, headers=headers) as response:
-                return [AssetsCIDR(**i) for i in (await response.json())]
+                return [Networks(**i) for i in (await response.json())]
 
-    async def describe(self, asset_cidr_id: str) -> AssetsCIDR:
+    async def describe(self, network_id: str) -> Networks:
         async with aiohttp.ClientSession() as session:
             base_url = self.config_manager.config["api_base_url"]
             project_id = self.config_manager.config["project_id"]
-            url = f"{base_url}v1/general/projects/{project_id}/assets/cidr/{asset_cidr_id}"
+            url = f"{base_url}v1/networks/{network_id}"
             headers = {"Authorization": f"Bearer {self.credentials.access_token}"}
             async with session.get(url, headers=headers) as response:
-                return AssetsCIDR(**(await response.json()))
+                return Networks(**(await response.json()))
 
-    async def update(self, asset_cidr_id: str, asset_cidr: dict) -> bool:
+    async def update(self, network_id: str, network: dict) -> bool:
         async with aiohttp.ClientSession() as session:
             base_url = self.config_manager.config["api_base_url"]
             project_id = self.config_manager.config["project_id"]
-            url = f"{base_url}v1/general/projects/{project_id}/assets/cidr/{asset_cidr_id}"
+            url = f"{base_url}v1/networks/{network_id}"
             headers = {"Authorization": f"Bearer {self.credentials.access_token}"}
-            async with session.put(url, headers=headers, json=asset_cidr) as response:
+            async with session.put(url, headers=headers, json=network) as response:
                 return response.status == 200
 
-    async def delete(self, asset_cidr_id: str) -> bool:
+    async def delete(self, network_id: str) -> bool:
         async with aiohttp.ClientSession() as session:
             base_url = self.config_manager.config["api_base_url"]
             project_id = self.config_manager.config["project_id"]
-            url = f"{base_url}v1/general/projects/{project_id}/assets/cidr/{asset_cidr_id}"
+            url = f"{base_url}v1/networks/{network_id}"
             headers = {"Authorization": f"Bearer {self.credentials.access_token}"}
             async with session.delete(url, headers=headers) as response:
                 return response.status == 200
```

### Comparing `hacktegic-0.1.9/hacktegic/cloud/api_clients/projects.py` & `hacktegic-0.2.0/hacktegic/cloud/api_clients/scans.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,47 @@
 import aiohttp
 
 from hacktegic._internal.config import ConfigManager
 from hacktegic._internal.credentials import Credentials
-from hacktegic.cloud.resources.projects import Project
+from hacktegic.cloud.resources.scans import Scans
 
 
-class ProjectsAPIClient:
+class ScansAPIClient:
     def __init__(self, credentials: Credentials, config_manager: ConfigManager) -> None:
         self.credentials = credentials
         self.config_manager = config_manager
 
-    async def create(self, name: str) -> Project:
+    async def list(self) -> list[Scans]:
         async with aiohttp.ClientSession() as session:
-            url = f'{self.config_manager.config["api_base_url"]}v1/general/projects'
-            headers = {"Authorization": f"Bearer {self.credentials.access_token}"}
-            data = {"name": name}
-            async with session.post(url, headers=headers, json=data) as response:
-                return Project(**(await response.json()))
-
-    async def list(self) -> list[Project]:
-        async with aiohttp.ClientSession() as session:
-            url = f'{self.config_manager.config["api_base_url"]}v1/general/projects'
+            base_url = self.config_manager.config["api_base_url"]
+            project_id = self.config_manager.config["project_id"]
+            url = f"{base_url}v1/projects/{project_id}/scans"
             headers = {"Authorization": f"Bearer {self.credentials.access_token}"}
             async with session.get(url, headers=headers) as response:
-                return [Project(**i) for i in (await response.json())]
+                return [Scans(**i) for i in (await response.json())]
 
-    async def describe(self, project_id: str) -> Project:
+    async def describe(self, scan_id: str) -> Scans:
         async with aiohttp.ClientSession() as session:
-            url = f'{self.config_manager.config["api_base_url"]}v1/general/projects/{project_id}'
+            base_url = self.config_manager.config["api_base_url"]
+            project_id = self.config_manager.config["project_id"]
+            url = f"{base_url}v1/scans/{scan_id}"
             headers = {"Authorization": f"Bearer {self.credentials.access_token}"}
             async with session.get(url, headers=headers) as response:
-                return Project(**(await response.json()))
+                return Scans(**(await response.json()))
 
-    async def update(self, project_id: str, name: str) -> bool:
+    async def delete(self, scan_id: str) -> bool:
         async with aiohttp.ClientSession() as session:
-            url = f'{self.config_manager.config["api_base_url"]}v1/general/projects/{project_id}'
+            base_url = self.config_manager.config["api_base_url"]
+            project_id = self.config_manager.config["project_id"]
+            url = f"{base_url}v1/scans/{scan_id}"
             headers = {"Authorization": f"Bearer {self.credentials.access_token}"}
-            data = {"name": name}
-            async with session.patch(url, headers=headers, json=data) as response:
-                return response.status == 200
 
-    async def delete(self, project_id: str) -> bool:
-        async with aiohttp.ClientSession() as session:
-            url = f'{self.config_manager.config["api_base_url"]}v1/general/projects/{project_id}'
-            headers = {"Authorization": f"Bearer {self.credentials.access_token}"}
-            async with session.delete(url, headers=headers) as response:
-                return response.status == 200
+            try:
+                async with session.delete(url, headers=headers) as response:
+                    response.raise_for_status()
+                    return response.status == 200
+            except aiohttp.ClientResponseError as cre:
+                print(f"HTTP error occurred: {cre.status}, message='{cre.message}', url={cre.request_info.url}")
+                return False
+            except Exception as e:
+                print(f"An error occurred: {e}")
+                return False
```

### Comparing `hacktegic-0.1.9/pyproject.toml` & `hacktegic-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "hacktegic"
 #dynamic = ["version"]
-version = "0.1.9"
+version = "0.2.0"
 authors = [
     { name = "Artiom Mocrenco", email = "artiomm@hacktegic.com" },
 ]
 description = "Hacktegic CLI"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
@@ -16,23 +16,24 @@
     "Topic :: Security",
 ]
 
 dependencies = [
     "aiohttp~=3.9.0b1",
     "rich>=13.6,<13.8",
     "requests~=2.31.0",
-    "platformdirs>=3.11,<4.2",
+    "platformdirs>=3.11,<4.3",
     "aiofiles~=23.2.1",
     "tomlkit~=0.12.2",
-    "pydantic~=2.5.0",
+    "pydantic>=2.5,<2.8",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/hacktegic/cli"
 "Bug Tracker" = "https://github.com/hacktegic/cli/issues"
+"Release Notes" = "https://github.com/hacktegic/cli/releases"
 
 [project.scripts]
 hacktegic = "hacktegic.__main__:main"
 
 #[tool.hatch.version]
 #version = "0.0.1"
 #source = "vcs"
```

### Comparing `hacktegic-0.1.9/PKG-INFO` & `hacktegic-0.2.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: hacktegic
-Version: 0.1.9
+Version: 0.2.0
 Summary: Hacktegic CLI
 Project-URL: Homepage, https://github.com/hacktegic/cli
 Project-URL: Bug Tracker, https://github.com/hacktegic/cli/issues
+Project-URL: Release Notes, https://github.com/hacktegic/cli/releases
 Author-email: Artiom Mocrenco <artiomm@hacktegic.com>
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Security
 Requires-Python: >=3.12
 Requires-Dist: aiofiles~=23.2.1
 Requires-Dist: aiohttp~=3.9.0b1
-Requires-Dist: platformdirs<4.2,>=3.11
-Requires-Dist: pydantic~=2.5.0
+Requires-Dist: platformdirs<4.3,>=3.11
+Requires-Dist: pydantic<2.8,>=2.5
 Requires-Dist: requests~=2.31.0
 Requires-Dist: rich<13.8,>=13.6
 Requires-Dist: tomlkit~=0.12.2
 Description-Content-Type: text/markdown
 
 # Hacktegic CLI
```

