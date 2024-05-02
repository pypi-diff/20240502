# Comparing `tmp/rastless_cli-1.8.0.tar.gz` & `tmp/rastless_cli-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rastless_cli-1.8.0.tar", max compression
+gzip compressed data, was "rastless_cli-1.9.0.tar", max compression
```

## Comparing `rastless_cli-1.8.0.tar` & `rastless_cli-1.9.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     5747 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/README.md
--rw-r--r--   0        0        0     1102 2024-02-26 09:04:51.107331 rastless_cli-1.8.0/pyproject.toml
--rw-r--r--   0        0        0        1 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/rastless/__init__.py
--rw-r--r--   0        0        0        0 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/rastless/cli/__init__.py
--rw-r--r--   0        0        0     3529 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/rastless/cli/colormaps.py
--rw-r--r--   0        0        0     5408 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/rastless/cli/layers.py
--rw-r--r--   0        0        0      733 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/rastless/cli/management.py
--rw-r--r--   0        0        0     2746 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/rastless/cli/permissions.py
--rw-r--r--   0        0        0     1960 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/rastless/cli/validate.py
--rw-r--r--   0        0        0        0 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/rastless/commands/__init__.py
--rw-r--r--   0        0        0     1595 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/rastless/commands/colormaps.py
--rw-r--r--   0        0        0     1799 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/rastless/commands/layers.py
--rw-r--r--   0        0        0     1544 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/rastless/commands/permissions.py
--rw-r--r--   0        0        0      793 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/rastless/commands/validate.py
--rw-r--r--   0        0        0      780 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/rastless/config.py
--rw-r--r--   0        0        0        0 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/rastless/core/__init__.py
--rw-r--r--   0        0        0      764 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/rastless/core/aws_connection.py
--rw-r--r--   0        0        0     6644 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/rastless/core/cog.py
--rw-r--r--   0        0        0     2550 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/rastless/core/colormap.py
--rw-r--r--   0        0        0     1294 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/rastless/core/s3.py
--rw-r--r--   0        0        0       96 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/rastless/core/schemas.py
--rw-r--r--   0        0        0      209 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/rastless/core/utils.py
--rw-r--r--   0        0        0     1589 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/rastless/core/validate.py
--rw-r--r--   0        0        0      436 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/rastless/custom_exceptions.py
--rw-r--r--   0        0        0        0 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/rastless/db/__init__.py
--rw-r--r--   0        0        0      913 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/rastless/db/base.py
--rw-r--r--   0        0        0     6801 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/rastless/db/handler.py
--rw-r--r--   0        0        0     4240 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/rastless/db/models.py
--rw-r--r--   0        0        0     1344 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/rastless/main.py
--rw-r--r--   0        0        0      583 2024-02-26 09:04:30.006738 rastless_cli-1.8.0/rastless/settings.py
--rw-r--r--   0        0        0     6576 1970-01-01 00:00:00.000000 rastless_cli-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0     6428 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/README.md
+-rw-r--r--   0        0        0     1102 2024-05-02 10:17:03.045926 rastless_cli-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/rastless/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/rastless/cli/__init__.py
+-rw-r--r--   0        0        0     3546 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/rastless/cli/colormaps.py
+-rw-r--r--   0        0        0     6918 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/rastless/cli/layers.py
+-rw-r--r--   0        0        0      733 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/rastless/cli/management.py
+-rw-r--r--   0        0        0     2746 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/rastless/cli/permissions.py
+-rw-r--r--   0        0        0     1964 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/rastless/cli/validate.py
+-rw-r--r--   0        0        0        0 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/rastless/commands/__init__.py
+-rw-r--r--   0        0        0     1528 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/rastless/commands/colormaps.py
+-rw-r--r--   0        0        0     3490 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/rastless/commands/layers.py
+-rw-r--r--   0        0        0     1544 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/rastless/commands/permissions.py
+-rw-r--r--   0        0        0      743 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/rastless/commands/validate.py
+-rw-r--r--   0        0        0     1094 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/rastless/config.py
+-rw-r--r--   0        0        0        0 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/rastless/core/__init__.py
+-rw-r--r--   0        0        0      764 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/rastless/core/aws_connection.py
+-rw-r--r--   0        0        0     6391 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/rastless/core/cog.py
+-rw-r--r--   0        0        0     2602 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/rastless/core/colormap.py
+-rw-r--r--   0        0        0     1874 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/rastless/core/s3.py
+-rw-r--r--   0        0        0       96 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/rastless/core/schemas.py
+-rw-r--r--   0        0        0      207 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/rastless/core/utils.py
+-rw-r--r--   0        0        0     1607 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/rastless/core/validate.py
+-rw-r--r--   0        0        0      436 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/rastless/custom_exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/rastless/db/__init__.py
+-rw-r--r--   0        0        0      895 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/rastless/db/base.py
+-rw-r--r--   0        0        0     8509 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/rastless/db/handler.py
+-rw-r--r--   0        0        0     4245 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/rastless/db/models.py
+-rw-r--r--   0        0        0     1382 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/rastless/main.py
+-rw-r--r--   0        0        0      885 2024-05-02 10:16:49.161733 rastless_cli-1.9.0/rastless/settings.py
+-rw-r--r--   0        0        0     7257 1970-01-01 00:00:00.000000 rastless_cli-1.9.0/PKG-INFO
```

### Comparing `rastless_cli-1.8.0/README.md` & `rastless_cli-1.9.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -69,25 +69,31 @@
 
 # Example production
 $ rastless list-layers
 ```
 
 ## Commands Overview
 
-| Commands             |                                                     |
-|----------------------|-----------------------------------------------------|
-| add-colormap         | Add a SLD file                                      |
-| add-permission       | Add a role to one or multiple layers                |
-| check-aws-connection | Check if cli can connect to aws                     |
-| create-layer         | Create layer                                        |
-| create-timestep      | Create timestep entry and upload layer to S3 bucket |
-| delete-colormap      | Remove a SLD file                                   |
-| delete-layer         | Delete a layer with all timestep entries            |
-| delete-permission    | Delete one or multiple permissions                  |
-| list-layers          | List all layers                                     |
+| Commands              |                                                       |
+|-----------------------|-------------------------------------------------------|
+| add-mpl-colormap      | Add a custom colormap based on matplotlib colormaps   |
+| add-discrete-colormap | Add a discrete colormap based on matplotlib colormaps |
+| add-sld-colormap      | Add a SLD file                                        |
+| add-permission        | Add a role to one or multiple layers                  |
+| check-aws-connection  | Check if cli can connect to aws                       |
+| create-layer          | Create layer                                          |
+| create-timestep       | Create timestep entry and upload layer to S3 bucket   |
+| delete-colormap       | Remove a SLD file                                     |
+| delete-layer          | Delete a layer with all timestep entries              |
+| delete-permission     | Delete one or multiple permissions                    |
+| delete-layer-timestep | Delete one or multiple layer timesteps                |
+| delete-cache          | Deletes cache                                         |
+| list-layers           | List all layers                                       |
+| list-colormaps        | List all colormaps                                    |
+| layer-exists          | Check if layer id exists                              |
 
 ## Accomplishing a running system
 
 #### 1. Check if you have access to the system
 
 ```bash
 $ rastless check-aws-connection
@@ -148,14 +154,18 @@
 # Now: Override existing timestep. Flag: -o
 rastless create-timestep -f file1.tif -f file2.tif -d 2020-01-01T15:00:00 -s Sent2 -layer-id 1234 -t daily -p deflate -o
 
 # Now: Append file to existing timestep. Flag: -a
 rastless create-timestep -f file2.tif -d 2020-01-01T15:00:00 -layer-id 1234 -p deflate -a
 ```
 
+### Version 1.7.0
+- Add new endoints to delete layer cache in s3 bucket and dynamodb
+- List-layer now has filter options for region_id, client and product
+
 ## Publish and Release
 
 When releasing we use [semantic versioning](https://semver.org/) to define the new version tag.
 
 When pushing to master any commit message that includes #major, #minor, #patch will add a tag to the commit
 with the respective version bump. If #none is contained in the merge commit message, it will skip the version bump.
 When none of the above types is provided the default version bump (minor) is triggered. After the tagging a package
```

### Comparing `rastless_cli-1.8.0/pyproject.toml` & `rastless_cli-1.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rastless-cli"
-version = "v1.8.0"
+version = "v1.9.0"
 description = "A cli for managing data and user access for the cloud application rastless"
 authors = ["Marcel Siegmann <siegmann@eomap.de>"]
 readme = "README.md"
 packages = [
     { include = "rastless" }
 ]
```

### Comparing `rastless_cli-1.8.0/rastless/cli/colormaps.py` & `rastless_cli-1.9.0/rastless/cli/colormaps.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,65 +4,83 @@
 from rastless.cli.validate import parse_string_colors, parse_string_labels, parse_string_values
 from rastless.commands import colormaps
 from rastless.config import Cfg
 
 
 @click.command()
 @click.pass_obj
-@click.argument('sld_file', type=click.Path(exists=True))
+@click.argument("sld_file", type=click.Path(exists=True))
 @click.option("-n", "--name", help="Name of the colormap, otherwise take the filename")
 @click.option("-d", "--description", help="Add description")
 @click.option("-l", "--legend-image", help="Filepath to png legend image")
 def add_sld_colormap(cfg: Cfg, sld_file, name, description, legend_image):
     """Add a SLD file"""
     try:
-        colormaps.add_sld_colormap(cfg=cfg, sld_file=sld_file, name=name, description=description,
-                                   legend_image=legend_image)
+        colormaps.add_sld_colormap(
+            cfg=cfg, sld_file=sld_file, name=name, description=description, legend_image=legend_image
+        )
     except Exception as e:
         click.echo(f"SLD File could not be converted. Reason: {e}")
 
 
 @click.command()
 @click.pass_obj
 @click.option("-n", "--name", required=True, help="Name of the colormap")
 @click.option("-d", "--description", help="Add description")
 @click.option("-min", "--cm-min", required=True, help="Min colormap value")
 @click.option("-max", "--cm-max", required=True, help="Max colormap value")
 @click.option("-cm-name", "--mpl-cm-name", required=True, help="Matplotlib colormap name to be used")
-@click.option("-l", "--log", is_flag=True, help=("Boolean to indicate whether default scale should be logarithmic or "
-                                                 "not, default is false"))
+@click.option(
+    "-l",
+    "--log",
+    is_flag=True,
+    help=("Boolean to indicate whether default scale should be logarithmic or " "not, default is false"),
+)
 @click.option("-st", "--subtitle", help="Subtitle e.g unit written beneath the colormap")
 def add_mpl_colormap(cfg: Cfg, name, description, cm_min, cm_max, mpl_cm_name, log, subtitle):
     """Add a custom colormap based on matplotlib colormaps"""
     try:
-        colormaps.add_mpl_colormap(cfg=cfg, name=name, description=description, cm_min=cm_min, cm_max=cm_max,
-                                   mpl_name=mpl_cm_name, log=log, subtitle=subtitle)
+        colormaps.add_mpl_colormap(
+            cfg=cfg,
+            name=name,
+            description=description,
+            cm_min=cm_min,
+            cm_max=cm_max,
+            mpl_name=mpl_cm_name,
+            log=log,
+            subtitle=subtitle,
+        )
     except Exception as e:
-        click.echo(f'Error when adding colormap: {e}')
+        click.echo(f"Error when adding colormap: {e}")
 
 
 @click.command()
 @click.pass_obj
 @click.option("-n", "--name", required=True, help="Name of the colormap")
 @click.option("-d", "--description", help="Add description")
-@click.option("-c", "--colors", required=True,
-              help='colormap colors (rgba) as string list: "[[0,255,0,255],[255,0,0,''255]]". Byte values.')
+@click.option(
+    "-c",
+    "--colors",
+    required=True,
+    help='colormap colors (rgba) as string list: "[[0,255,0,255],[255,0,0,' '255]]". Byte values.',
+)
 @click.option("-v", "--values", required=True, help='colormap values as string list: "[1,2]". Integer values.')
 @click.option("-l", "--labels", required=True, help='colormap labels as string list: "[low, high]"')
 def add_discrete_colormap(cfg: Cfg, name, description, colors, values, labels):
     """Add a discrete colormap based on matplotlib colormaps"""
     colors = parse_string_colors(colors)
     values = parse_string_values(values)
     labels = parse_string_labels(labels)
 
     try:
-        colormaps.add_discrete_colormap(cfg=cfg, name=name, description=description, colors=colors, values=values,
-                                        labels=labels)
+        colormaps.add_discrete_colormap(
+            cfg=cfg, name=name, description=description, colors=colors, values=values, labels=labels
+        )
     except Exception as e:
-        click.echo(f'Error when adding colormap: {e}')
+        click.echo(f"Error when adding colormap: {e}")
 
 
 @click.command()
 @click.option("-n", "--name", help="Name of the colormap", required=True)
 @click.pass_obj
 def delete_colormap(cfg: Cfg, name):
     """Remove a SLD file"""
```

### Comparing `rastless_cli-1.8.0/rastless/cli/layers.py` & `rastless_cli-1.9.0/rastless/cli/layers.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,18 +16,23 @@
 @click.option("-t", "--title", required=True, type=str, help="Title which is displayed in the frontend")
 @click.option("-id", "--layer-id", default=str_uuid, type=str, help="Predefined uuid otherwise self generated")
 @click.option("-cm", "--colormap", type=str, help="colormap name")
 @click.option("-u", "--unit", type=str, help="Unit abbreviation e.g. m or FTU")
 @click.option("-b", "--background-id", type=str, help="Layer uuid of the background layer")
 @click.option("-d", "--description", type=str, help="Description to better identify the layer")
 @click.option("-r", "--region-id", default=1, type=int, help="Region ID of api-layer service")
-@click.option("-p", "--permissions", type=str, multiple=True,
-              help="Keycloak role permissions in the following form: User -> user#<unique username>"
-                   " e.g. user#siegmann@eomap.de, Role -> role#<keycloak client>:<client role>"
-                   " e.g. role#hypos:full-access")
+@click.option(
+    "-p",
+    "--permissions",
+    type=str,
+    multiple=True,
+    help="Keycloak role permissions in the following form: User -> user#<unique username>"
+         " e.g. user#siegmann@eomap.de, Role -> role#<keycloak client>:<client role>"
+         " e.g. role#hypos:full-access",
+)
 def create_layer(cfg: Cfg, permissions, **kwargs):
     """Create layer. This has to be done before adding timesteps"""
     try:
         layer_id = layers.create_layer(cfg, permissions, **kwargs)
         click.echo(f"Created layer with id: {layer_id}")
     except Exception as e:
         click.echo(f"Layer could not be created. Reason: {e}")
@@ -36,81 +41,120 @@
 @click.command()
 @click.pass_obj
 @click.option("-f", "--filenames", type=str, help="Filename paths ", multiple=True, required=True)
 @click.option("-d", "--datetime", required=True, type=str, help="Admission date")
 @click.option("-s", "--sensor", type=str, help="Sensor e.g. SENT2")
 @click.option("-l", "--layer-id", required=True, type=str, help="Created layer uuid")
 @click.option("-t", "--temporal-resolution", default="daily", type=str, help="Temporal resolution e.g. daily, monthly")
-@click.option("-p", "--profile", type=click.Choice([CompressionTypes.DEFLATE.value, CompressionTypes.WEBP.value]),
-              default=CompressionTypes.DEFLATE.value,
-              help="Compression of the GeoTiff")
+@click.option(
+    "-p",
+    "--profile",
+    type=click.Choice([CompressionTypes.DEFLATE.value, CompressionTypes.WEBP.value]),
+    default=CompressionTypes.DEFLATE.value,
+    help="Compression of the GeoTiff",
+)
 @click.option("-a", "--append", is_flag=True)
 @click.option("-o", "--override", is_flag=True)
-def create_timestep(cfg: Cfg, filenames, append, datetime, sensor, layer_id, temporal_resolution, profile,
-                    override):
+def create_timestep(cfg: Cfg, filenames, append, datetime, sensor, layer_id, temporal_resolution, profile, override):
     """Create timestep entry and upload layer to S3 bucket"""
     try:
-        layers.create_timestep(cfg, filenames, append, datetime, sensor, layer_id, temporal_resolution, profile,
-                               override)
+        layers.create_timestep(
+            cfg, filenames, append, datetime, sensor, layer_id, temporal_resolution, profile, override
+        )
     except FileExistsError as e:
         click.echo(str(e))
     except FileUploadError as e:
         click.echo(e)
     except LayerStepExistsError as e:
         click.echo(str(e))
-        click.confirm(abort=True)
-        layers.create_timestep(cfg, filenames, append, datetime, sensor, layer_id, temporal_resolution, profile,
-                               override=True)
+        click.confirm("Layer step already exist. Do you want to override it?", abort=True)
+        layers.create_timestep(
+            cfg, filenames, append, datetime, sensor, layer_id, temporal_resolution, profile, override=True
+        )
 
 
 @click.command()
 @click.option("-cl", "--client", type=str, help="Filter by client")
+@click.option("-r", "--region", type=str, help="Filter by region string")
+@click.option("-p", "--product", type=str, help="Filter by product string")
 @click.pass_obj
-def list_layers(cfg: Cfg, client):
-    """List all layers"""
-    filtered_layers = layers.list_layers(cfg, client)
+def list_layers(cfg: Cfg, client, region, product):
+    """List all layers with optional filters for client, region, and product."""
+    filtered_layers = layers.list_layers(cfg, client, region, product)
     click.echo(simplejson.dumps(filtered_layers, indent=4, sort_keys=True))
 
 
 @click.command()
 @click.pass_obj
 @click.option("-l", "--layer-id", required=True, type=str, help="Layer uuid")
-@click.option('--yes', is_flag=True)
+@click.option("--yes", is_flag=True)
 def delete_layer(cfg: Cfg, layer_id, yes):
     """Delete a layer with all timestep entries and permissions"""
     if not yes:
-        click.confirm(f'Do you really want to delete layer {layer_id}? All associated data will be deleted', abort=True)
+        click.confirm(f"Do you really want to delete layer {layer_id}? All associated data will be deleted", abort=True)
 
     layer_steps = cfg.db.get_layer_steps(layer_id)
 
     for layer_step in layer_steps:
         delete_layer_step_files(layer_step, cfg)
 
     cfg.db.delete_layer(layer_id=layer_id)
 
 
 @click.command()
 @click.pass_obj
 @click.option("-l", "--layer-id", required=True, type=str, help="Layer uuid")
 @click.option("-t", "--timestep", required=True, type=str, help="ISO timestep e.g 2022-01-01T15:00:00", multiple=True)
-@click.option('--yes', is_flag=True)
+@click.option("--yes", is_flag=True)
 def delete_layer_timestep(cfg: Cfg, layer_id, timestep, yes):
     """Delete one or multiple layer timesteps"""
     if not yes:
         click.confirm(
-            f'Do you really want to delete layer the layer step {timestep} for layer {layer_id}? '
-            f'All associated data will be deleted',
-            abort=True)
+            f"Do you really want to delete layer the layer step {timestep} for layer {layer_id}? "
+            f"All associated data will be deleted",
+            abort=True,
+        )
     layer_steps = [cfg.db.get_layer_step(step, layer_id) for step in timestep]
 
     for layer_step in layer_steps:
         delete_layer_step_files(layer_step, cfg)
         cfg.db.delete_layer_step(layer_step.datetime, layer_id)
 
 
 @click.command()
 @click.pass_obj
 @click.option("-l", "--layer-id", required=True, type=str, help="Layer uuid")
 def layer_exists(cfg: Cfg, layer_id):
     """Ask database if layer_id exists: returns a boolean"""
     response = cfg.db.get_layer("layer", f"layer#{layer_id}")
     click.echo(bool(response))
+
+
+@click.command()
+@click.pass_obj
+@click.option("-l", "--layer-id", type=str, help="Layer UUID for which cache needs to be deleted")
+@click.option(
+    "-d",
+    "--datetime",
+    type=str,
+    help="Specific timestep whose cache needs to be deleted. Must be used in combination with --layer-id.",
+)
+@click.option("--yes", is_flag=True, help="Confirm the deletion without prompts")
+def delete_cache(cfg: Cfg, layer_id, datetime, yes):
+    """Deletes cache from the S3 bucket based on the layer ID and/or datetime. Without options, deletes full cache."""
+    if datetime and not layer_id:
+        click.echo("'datetime' provided without 'layer_id'. Please provide both 'layer_id' and 'datetime'.")
+        return
+
+    if not yes:
+        if layer_id and datetime:
+            prompt_message = f"Do you really want to delete cache for layer {layer_id} at {datetime}?"
+        elif layer_id:
+            prompt_message = f"Do you really want to delete all cache for layer {layer_id}?"
+        else:
+            prompt_message = "Do you really want to delete all cache in the bucket?"
+
+        if not click.confirm(prompt_message, abort=True):
+            return
+
+    result_message = layers.delete_cache(cfg, layer_id, datetime)
+    click.echo(result_message)
```

### Comparing `rastless_cli-1.8.0/rastless/cli/management.py` & `rastless_cli-1.9.0/rastless/cli/management.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 if TYPE_CHECKING:
     from rastless.settings import Cfg
 
 
 @click.command()
 @click.pass_obj
-def check_aws_connection(cfg: 'Cfg'):
+def check_aws_connection(cfg: "Cfg"):
     """Check if cli can connect to aws"""
     has_bucket_access, bucket_error = aws_connection.check_bucket_connection(cfg.s3.bucket_name)
     has_db_access, db_error = aws_connection.check_dynamodb_table_connection(cfg.db.table_name)
 
     if all([has_bucket_access, has_db_access]):
         click.echo("You have access to aws resources!")
     else:
```

### Comparing `rastless_cli-1.8.0/rastless/cli/permissions.py` & `rastless_cli-1.9.0/rastless/cli/permissions.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,66 +2,77 @@
 import simplejson
 
 from rastless.commands import permissions as cmd_permissions
 from rastless.config import Cfg
 
 
 @click.command()
-@click.option('-p', '--permission', required=True, type=str,
-              help='Role e.g role#<client>:<client_role>, user#<username>')
-@click.option('-l', '--layer_ids', help='Layer id', required=True, type=str, multiple=True)
+@click.option(
+    "-p", "--permission", required=True, type=str, help="Role e.g role#<client>:<client_role>, user#<username>"
+)
+@click.option("-l", "--layer_ids", help="Layer id", required=True, type=str, multiple=True)
 @click.pass_obj
 def add_permission(cfg: Cfg, permission, layer_ids):
     """Add a role to one or multiple layers."""
     cmd_permissions.add_permission(cfg, permission, layer_ids)
     click.echo("Role was successfully added to layers")
 
 
 @click.command()
-@click.option('-p', '--permissions', help='Permission name e.g role#<client>:<client_role>, user#<username>',
-              required=True, type=str, multiple=True)
+@click.option(
+    "-p",
+    "--permissions",
+    help="Permission name e.g role#<client>:<client_role>, user#<username>",
+    required=True,
+    type=str,
+    multiple=True,
+)
 @click.pass_obj
 def delete_permission(cfg: Cfg, permissions):
     """Delete one or multiple permissions."""
     cmd_permissions.delete_permission_asdf(cfg, permissions)
     click.echo("Roles were successfully deleted")
 
 
 @click.command()
-@click.option("-p", "--permission", help='Permission name e.g role#<client>:<client_role>, user#<username>',
-              required=True, type=str)
-@click.option('-l', '--layer_ids', help='Layer ids', type=str, required=True, multiple=True)
+@click.option(
+    "-p",
+    "--permission",
+    help="Permission name e.g role#<client>:<client_role>, user#<username>",
+    required=True,
+    type=str,
+)
+@click.option("-l", "--layer_ids", help="Layer ids", type=str, required=True, multiple=True)
 @click.pass_obj
 def delete_layer_permission(cfg: Cfg, permission, layer_ids):
     """Delete one or multiple layer permissions."""
     cmd_permissions.delete_layer_permission(cfg, permission, layer_ids)
     click.echo("Layer permission was successfully deleted")
 
 
 @click.command()
-@click.option('-l', '--layer_id', help='Layer id', type=str)
-@click.option('-p', '--permission', type=str,
-              help='Role e.g role#<client>:<client_role>, user#<username>')
+@click.option("-l", "--layer_id", help="Layer id", type=str)
+@click.option("-p", "--permission", type=str, help="Role e.g role#<client>:<client_role>, user#<username>")
 @click.pass_obj
 def get_permissions(cfg: Cfg, layer_id, permission):
     """Get layer ids for a role or get all permissions for a layer id."""
     items = cmd_permissions.get_permissions(cfg, layer_id, permission)
 
     click.echo(simplejson.dumps(items, indent=4, sort_keys=True))
 
 
 @click.command()
-@click.option('-a', '--access_token', help='Access token', type=str)
-@click.option('-l', '--layer_ids', help='Layer ids', type=str, required=True, multiple=True)
+@click.option("-a", "--access_token", help="Access token", type=str)
+@click.option("-l", "--layer_ids", help="Layer ids", type=str, required=True, multiple=True)
 @click.pass_obj
 def add_access_token(cfg: Cfg, access_token, layer_ids):
     """Create access token for project eoapp"""
     access_token_id = cmd_permissions.create_access_token(cfg, layer_ids, access_token)
     click.echo(f"Access token: {access_token_id}")
 
 
 @click.command()
-@click.option('-a', '--access_token', help='Access token', type=str)
+@click.option("-a", "--access_token", help="Access token", type=str)
 @click.pass_obj
 def delete_access_token(cfg: Cfg, access_token: str):
     cmd_permissions.delete_access_token(cfg, access_token)
     click.echo(f"Access token {access_token} was successfully deleted")
```

### Comparing `rastless_cli-1.8.0/rastless/cli/validate.py` & `rastless_cli-1.9.0/rastless/cli/validate.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,44 +4,49 @@
 from rastless.custom_exceptions import ColorMapParseError
 
 
 def parse_string_colors(colors: str):
     try:
         parsed_list = ast.literal_eval(colors)
     except SyntaxError:
-        raise ColorMapParseError('colors list could not be parsed, needs to be in the following format: "[[int,'
-                                 'int,int,int]]"')
+        raise ColorMapParseError(
+            'colors list could not be parsed, needs to be in the following format: "[[int,' 'int,int,int]]"'
+        )
     for item in parsed_list:
         if not len(item) == 4:
-            raise ColorMapParseError(f'colors list could not be parsed, every item needs to be a list of 4 integers '
-                                     f'representing rgba, but instead one item had a length of {len(item)}')
+            raise ColorMapParseError(
+                f"colors list could not be parsed, every item needs to be a list of 4 integers "
+                f"representing rgba, but instead one item had a length of {len(item)}"
+            )
         for num in item:
             if not isinstance(num, int):
                 raise ColorMapParseError(
-                    f'colors list could not be parsed, every item needs to be a list of 4 integers '
-                    f'representing rgba, but instead one item was of type{type(item)}')
+                    f"colors list could not be parsed, every item needs to be a list of 4 integers "
+                    f"representing rgba, but instead one item was of type{type(item)}"
+                )
     return parsed_list
 
 
 def parse_string_values(values: str) -> List[int]:
     try:
         parsed_list = ast.literal_eval(values)
     except SyntaxError:
-        raise ColorMapParseError('values list could not be parsed, needs to be in the following format: "[int,'
-                                 'int]"')
+        raise ColorMapParseError('values list could not be parsed, needs to be in the following format: "[int,' 'int]"')
     for item in parsed_list:
         if not isinstance(item, int):
             raise ColorMapParseError('values list could not be parsed, all elements have to be integers: "[int,int]"')
     return parsed_list
 
 
 def parse_string_labels(labels):
     try:
         parsed_list = ast.literal_eval(labels)
     except SyntaxError:
         raise ColorMapParseError(
-            'labels list could not be parsed, needs to be in the following format: "["str","str"]"')
+            'labels list could not be parsed, needs to be in the following format: "["str","str"]"'
+        )
     for item in parsed_list:
         if not isinstance(item, str):
             raise ColorMapParseError(
-                'labels list could not be parsed, all elements have to be strings: "["str","str"]"')
+                'labels list could not be parsed, all elements have to be strings: "["str","str"]"'
+            )
     return parsed_list
```

### Comparing `rastless_cli-1.8.0/rastless/commands/colormaps.py` & `rastless_cli-1.9.0/rastless/commands/colormaps.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,29 +11,36 @@
 
     if not name:
         name = os.path.basename(sld_file.split(".")[0])
     color_map = create_sld_colormap(name, sld_file, description, legend_image)
     cfg.db.add_color_map(color_map)
 
 
-def add_mpl_colormap(cfg, name: str, description: str, cm_min: float, cm_max: float, mpl_name: str, log: bool,
-                     subtitle: str = None):
+def add_mpl_colormap(
+    cfg, name: str, description: str, cm_min: float, cm_max: float, mpl_name: str, log: bool, subtitle: str = None
+):
     if log and float(cm_min) == 0:
         raise ValueError("Min must be greater than 0, when log is True.")
 
     color_map = create_mpl_colormap(name, description, cm_min, cm_max, log, mpl_name, subtitle)
     cfg.db.add_color_map(color_map)
 
 
-def add_discrete_colormap(cfg, name: str, description: Optional[str], values: List[int],
-                          colors: List[tuple[int, int, int, int]],
-                          labels: List[str]):
+def add_discrete_colormap(
+    cfg,
+    name: str,
+    description: Optional[str],
+    values: List[int],
+    colors: List[tuple[int, int, int, int]],
+    labels: List[str],
+):
     validate_list_lengths(values, colors, labels)
-    color_map = create_discrete_colormap(name=name, description=description, values=values, colors=colors,
-                                         labels=labels)
+    color_map = create_discrete_colormap(
+        name=name, description=description, values=values, colors=colors, labels=labels
+    )
     cfg.db.add_color_map(color_map)
 
 
 def delete_colormap(cfg: Cfg, name):
     """Remove a SLD file"""
     cfg.db.delete_color_map(name)
```

### Comparing `rastless_cli-1.8.0/rastless/commands/permissions.py` & `rastless_cli-1.9.0/rastless/commands/permissions.py`

 * *Files identical despite different names*

### Comparing `rastless_cli-1.8.0/rastless/commands/validate.py` & `rastless_cli-1.9.0/rastless/commands/validate.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import List
 
 from rastless.config import Cfg
 from rastless.custom_exceptions import ColorMapDoesNotExistError, ColorMapParseError
 
 
-def validate_list_lengths(values: List[int],
-                          colors: List[tuple[int, int, int, int]],
-                          labels: List[str]):
+def validate_list_lengths(values: List[int], colors: List[tuple[int, int, int, int]], labels: List[str]):
     if not len(values) == len(colors) == len(labels):
-        raise ColorMapParseError('values, colors and labels list need to be of same length')
+        raise ColorMapParseError("values, colors and labels list need to be of same length")
 
 
 def validate_colormap_exists(cfg: Cfg, **kwargs):
     if kwargs.get("colormap"):
-        if not cfg.db.get_color_map(kwargs['colormap']):
-            raise ColorMapDoesNotExistError(f'Error when creating layer as colormap with name {kwargs["colormap"]} '
-                                            f'does not exist. Create colormap first.')
+        if not cfg.db.get_color_map(kwargs["colormap"]):
+            raise ColorMapDoesNotExistError(
+                f'Error when creating layer as colormap with name {kwargs["colormap"]} '
+                f'does not exist. Create colormap first.'
+            )
```

### Comparing `rastless_cli-1.8.0/rastless/config.py` & `rastless_cli-1.9.0/rastless/config.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from rastless import settings
 from rastless.core.s3 import S3Bucket
 from rastless.db.handler import Database
 
 
 class Cfg:
-    def __init__(self, table_name, bucket_name):
+    def __init__(self, table_name, bucket_name, cache_bucket_name=None):
         self.db = Database(table_name)
         self.s3 = S3Bucket(bucket_name)
         self.bucket_name = bucket_name
+        self.cache_s3 = S3Bucket(cache_bucket_name)
 
 
 def create_config(dev: bool = False, test: bool = False) -> Cfg:
     if dev:
         table_name = settings.RASTLESS_TABLE_NAME_DEV
         bucket_name = settings.RASTLESS_BUCKET_NAME_DEV
+        cache_bucket_name = settings.RASTLESS_BUCKET_NAME_CACHE_DEV
     elif test:
         table_name = settings.RASTLESS_TABLE_NAME_TEST
         bucket_name = settings.RASTLESS_BUCKET_NAME_TEST
+        cache_bucket_name = settings.RASTLESS_BUCKET_NAME_CACHE_TEST
     else:
         table_name = settings.RASTLESS_TABLE_NAME
         bucket_name = settings.RASTLESS_BUCKET_NAME
-    return Cfg(table_name=table_name, bucket_name=bucket_name)
+        cache_bucket_name = settings.RASTLESS_BUCKET_NAME_CACHE
+    return Cfg(table_name=table_name, bucket_name=bucket_name, cache_bucket_name=cache_bucket_name)
```

### Comparing `rastless_cli-1.8.0/rastless/core/cog.py` & `rastless_cli-1.9.0/rastless/core/cog.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,26 +38,27 @@
     maxzoom: int
 
 
 def create_s3_cog_info(bucket_name: str, layer_id: str, datetime: str, filepath: str) -> S3Cog:
     filename = os.path.basename(filepath)
     object_name = f"layer/{layer_id}/{datetime}/{filename}"
     s3_path = f"s3://{bucket_name}/{object_name}"
-    return S3Cog(s3_object_name=object_name, s3_path=s3_path, bucket_name=bucket_name, filename=filename,
-                 filepath=filepath)
+    return S3Cog(
+        s3_object_name=object_name, s3_path=s3_path, bucket_name=bucket_name, filename=filename, filepath=filepath
+    )
 
 
 def get_s3_cog_info_from_s3_path(s3_file_path: str) -> S3Cog:
     parts = s3_file_path.split("/")
     object_name = "/".join(parts[3:])
     return S3Cog(s3_object_name=object_name, s3_path=s3_file_path, bucket_name=parts[2], filename=parts[-1])
 
 
 def upload_cog_file(s3_cog: S3Cog) -> bool:
-    s3_client = boto3.client('s3')
+    s3_client = boto3.client("s3")
 
     try:
         s3_client.upload_file(s3_cog.filepath, s3_cog.bucket_name, s3_cog.s3_object_name)
     except Exception:
         return False
     return True
 
@@ -101,20 +102,34 @@
 def get_layer_info(filename: str) -> LayerInfo:
     result = cog_info(filename)
     geo_info = result["GEO"]
     bbox_wgs84 = transform_bbox(geo_info["BoundingBox"], geo_info["CRS"])
     bbox_wgs84 = tuple([round(x, 6) for x in bbox_wgs84])
     max_zoom = geo_info["MaxZoom"] + 2 if geo_info["MaxZoom"] < 21 else geo_info["MaxZoom"]
 
-    return LayerInfo(bbox_wgs84=bbox_wgs84, resolution=float(geo_info["Resolution"][0]),
-                     maxzoom=max_zoom, minzoom=geo_info["MinZoom"])
-
-
-def upload_files(cfg: 'Cfg', filenames: Set[str], layer_id: str, datetime: str, profile: str, cog_layers: dict,
-                 bboxes: List, resolutions: List, min_zoom: List, max_zoom: List) -> (Set[str], List[float], float):
+    return LayerInfo(
+        bbox_wgs84=bbox_wgs84,
+        resolution=float(geo_info["Resolution"][0]),
+        maxzoom=max_zoom,
+        minzoom=geo_info["MinZoom"],
+    )
+
+
+def upload_files(
+    cfg: "Cfg",
+    filenames: Set[str],
+    layer_id: str,
+    datetime: str,
+    profile: str,
+    cog_layers: dict,
+    bboxes: List,
+    resolutions: List,
+    min_zoom: List,
+    max_zoom: List,
+) -> (Set[str], List[float], float):
     for filename in filenames:
         s3_cog = create_s3_cog_info(cfg.s3.bucket_name, layer_id, datetime, filename)
         layer_info = get_layer_info(filename)
 
         if layer_is_valid_cog(filename):
             uploaded = upload_cog_file(s3_cog)
         else:
@@ -130,45 +145,69 @@
             raise FileUploadError(f"File {filename} could not be uploaded. Please try again.")
 
     bbox_extent = merge_bbox_extent(bboxes)
 
     return cog_layers, bbox_extent, min(resolutions), min(min_zoom), max(max_zoom)
 
 
-def create_new_timestep(cfg: 'Cfg', filenames: Set[str], layer_id: str, datetime: str, profile: str,
-                        temporal_resolution: str, sensor: str):
+def create_new_timestep(
+    cfg: "Cfg", filenames: Set[str], layer_id: str, datetime: str, profile: str, temporal_resolution: str, sensor: str
+):
     cog_layers = {}
     bboxes = []
     resolutions = []
     min_zoom = []
     max_zoom = []
 
-    cog_layers, bbox_extent, resolution, min_zoom, max_zoom = upload_files(cfg, filenames, layer_id, datetime, profile,
-                                                                           cog_layers, bboxes, resolutions, min_zoom,
-                                                                           max_zoom)
-
-    layer_step = LayerStepModel(layer_id=layer_id, cog_layers=cog_layers, datetime=datetime, sensor=sensor,
-                                temporal_resolution=temporal_resolution, maxzoom=22,
-                                minzoom=0,
-                                bbox=bbox_extent, resolution=round(resolution, 6))
+    cog_layers, bbox_extent, resolution, min_zoom, max_zoom = upload_files(
+        cfg, filenames, layer_id, datetime, profile, cog_layers, bboxes, resolutions, min_zoom, max_zoom
+    )
+
+    layer_step = LayerStepModel(
+        layer_id=layer_id,
+        cog_layers=cog_layers,
+        datetime=datetime,
+        sensor=sensor,
+        temporal_resolution=temporal_resolution,
+        maxzoom=22,
+        minzoom=0,
+        bbox=bbox_extent,
+        resolution=round(resolution, 6),
+    )
 
     cfg.db.add_layer_step(layer_step)
 
 
-def append_to_timestep(cfg: 'Cfg', layer_step: LayerStepModel, filenames: Set[str], profile: str):
+def append_to_timestep(cfg: "Cfg", layer_step: LayerStepModel, filenames: Set[str], profile: str):
     if layer_step.cog_filepath:
         raise ValueError("Appending to old format is not allowed")
 
     bboxes = [layer_step.bbox]
     resolutions = [layer_step.resolution]
     min_zoom = [layer_step.minzoom]
     max_zoom = [layer_step.maxzoom]
 
-    cog_layers, bbox_extent, resolution, min_zoom, max_zoom = upload_files(cfg, filenames, layer_step.layer_id,
-                                                                           layer_step.datetime,
-                                                                           profile, layer_step.cog_layers, bboxes,
-                                                                           resolutions, min_zoom, max_zoom)
-
-    layer_step = LayerStepModel(layer_id=layer_step.layer_id, cog_layers=cog_layers, datetime=layer_step.datetime,
-                                sensor=layer_step.sensor, temporal_resolution=layer_step.temporal_resolution,
-                                maxzoom=max_zoom, minzoom=min_zoom, bbox=bbox_extent, resolution=round(resolution, 6))
+    cog_layers, bbox_extent, resolution, min_zoom, max_zoom = upload_files(
+        cfg,
+        filenames,
+        layer_step.layer_id,
+        layer_step.datetime,
+        profile,
+        layer_step.cog_layers,
+        bboxes,
+        resolutions,
+        min_zoom,
+        max_zoom,
+    )
+
+    layer_step = LayerStepModel(
+        layer_id=layer_step.layer_id,
+        cog_layers=cog_layers,
+        datetime=layer_step.datetime,
+        sensor=layer_step.sensor,
+        temporal_resolution=layer_step.temporal_resolution,
+        maxzoom=max_zoom,
+        minzoom=min_zoom,
+        bbox=bbox_extent,
+        resolution=round(resolution, 6),
+    )
     cfg.db.add_layer_step(layer_step)
```

### Comparing `rastless_cli-1.8.0/rastless/core/colormap.py` & `rastless_cli-1.9.0/rastless/core/colormap.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,60 +6,79 @@
 
 from rastless.db.models import DiscreteColorMap, MplColorMap, SldColorMap
 
 
 class Sld:
     def __init__(self, filename):
         self.xml_doc = minidom.parse(filename)
-        self.items = self.xml_doc.getElementsByTagName('sld:ColorMapEntry')
+        self.items = self.xml_doc.getElementsByTagName("sld:ColorMapEntry")
 
     @staticmethod
     def _hex_to_rgb(hex_color) -> tuple:
-        hex_value = hex_color.lstrip('#')
-        return tuple(int(hex_value[i:i + 2], 16) for i in (0, 2, 4))
+        hex_value = hex_color.lstrip("#")
+        return tuple(int(hex_value[i : i + 2], 16) for i in (0, 2, 4))
 
     @property
     def hex_colors(self) -> np.array:
-        return np.array([entry.attributes["color"].value for entry in self.items if
-                         float(entry.attributes["opacity"].value) > 0])
+        return np.array(
+            [entry.attributes["color"].value for entry in self.items if float(entry.attributes["opacity"].value) > 0]
+        )
 
     @property
     def rgb_colors(self) -> np.array:
         return np.array([self._hex_to_rgb(hex_color) for hex_color in self.hex_colors])
 
     @property
     def values(self) -> np.array:
-        return np.array([float(entry.attributes["quantity"].value) for entry in self.items if
-                         float(entry.attributes["opacity"].value) > 0])
+        return np.array(
+            [
+                float(entry.attributes["quantity"].value)
+                for entry in self.items
+                if float(entry.attributes["opacity"].value) > 0
+            ]
+        )
 
     @property
     def no_data(self) -> List:
-        return [float(entry.attributes["quantity"].value) for entry in self.items if
-                float(entry.attributes["opacity"].value) == 0]
+        return [
+            float(entry.attributes["quantity"].value)
+            for entry in self.items
+            if float(entry.attributes["opacity"].value) == 0
+        ]
 
 
 def legend_png_to_base64(legend_filepath: str) -> bytes:
     with open(legend_filepath, "rb") as image_file:
         encoded_image = base64.b64encode(image_file.read())
     return encoded_image
 
 
-def create_sld_colormap(name: str, sld_filepath: str, description: str = None,
-                        legend_filepath: str = None) -> SldColorMap:
+def create_sld_colormap(
+    name: str, sld_filepath: str, description: str = None, legend_filepath: str = None
+) -> SldColorMap:
     legend_base64 = None
     if legend_filepath:
         legend_base64 = legend_png_to_base64(legend_filepath)
 
     sld = Sld(sld_filepath)
-    return SldColorMap(name=name, values=sld.values.tolist(), colors=sld.rgb_colors.tolist(),
-                       nodata=sld.no_data, description=description, legend_image=legend_base64)
-
-
-def create_mpl_colormap(name, description: str, cm_min: float, cm_max: float, log: bool, mpl_name: str,
-                        subtitle: str) -> MplColorMap:
-    return MplColorMap(name=name, description=description, min=cm_min, max=cm_max, log=log, cmap_name=mpl_name,
-                       subtitle=subtitle)
-
-
-def create_discrete_colormap(name: str, description: str, values: List[int], colors: List[tuple[int, int, int, int]],
-                             labels: List[str]) -> DiscreteColorMap:
+    return SldColorMap(
+        name=name,
+        values=sld.values.tolist(),
+        colors=sld.rgb_colors.tolist(),
+        nodata=sld.no_data,
+        description=description,
+        legend_image=legend_base64,
+    )
+
+
+def create_mpl_colormap(
+    name, description: str, cm_min: float, cm_max: float, log: bool, mpl_name: str, subtitle: str
+) -> MplColorMap:
+    return MplColorMap(
+        name=name, description=description, min=cm_min, max=cm_max, log=log, cmap_name=mpl_name, subtitle=subtitle
+    )
+
+
+def create_discrete_colormap(
+    name: str, description: str, values: List[int], colors: List[tuple[int, int, int, int]], labels: List[str]
+) -> DiscreteColorMap:
     return DiscreteColorMap(name=name, description=description, values=values, colors=colors, labels=labels)
```

### Comparing `rastless_cli-1.8.0/rastless/core/s3.py` & `rastless_cli-1.9.0/rastless/core/s3.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,30 +3,45 @@
 from rastless.core.cog import get_s3_cog_info_from_s3_path
 from rastless.db.models import LayerStepModel
 
 
 class S3Bucket:
     def __init__(self, bucket_name, region="eu-central-1"):
         self.bucket_name = bucket_name
-        self.s3 = boto3.resource('s3', region_name=region)
-        self.s3_client = boto3.client('s3')
+        self.s3 = boto3.resource("s3", region_name=region)
+        self.s3_client = boto3.client("s3")
         self.bucket = self.s3.Bucket(bucket_name)
 
     def list_bucket_entries(self, prefix=None):
         bucket = self.s3.Bucket(self.bucket_name)
         if prefix:
             files = bucket.objects.filter(Prefix=prefix)
         else:
             files = bucket.objects.all()
 
         return list(files)
 
+    def delete_cache(self, layer_id=None, datetime=None):
+        """Deletes objects based on layer ID and/or datetime, or all cache if no parameters are given."""
+        if layer_id and datetime:
+            prefix = f"{layer_id}/{datetime}/"
+        elif layer_id:
+            prefix = f"{layer_id}/"
+        else:
+            prefix = ""
+
+        cache_objects = self.bucket.objects.filter(Prefix=prefix)
+        delete_keys = {"Objects": [{"Key": obj.key} for obj in cache_objects]}
+
+        response = self.bucket.delete_objects(Delete=delete_keys)
+        return response
+
 
 def delete_object_by_s3_path(s3_path, region="eu-central-1"):
-    s3 = boto3.resource('s3', region_name=region)
+    s3 = boto3.resource("s3", region_name=region)
 
     s3_cog_info = get_s3_cog_info_from_s3_path(s3_path)
     s3.Object(s3_cog_info.bucket_name, s3_cog_info.s3_object_name).delete()
 
 
 def delete_layer_step_files(layer_step: LayerStepModel, cfg):
     if layer_step.cog_filepath and cfg.bucket_name in layer_step.cog_filepath:
```

### Comparing `rastless_cli-1.8.0/rastless/core/validate.py` & `rastless_cli-1.9.0/rastless/core/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,20 +24,22 @@
         raise FileExistsError(f"Filenames could not be found:\n{filename_errors_str}")
 
 
 def validate_layer_step_override(layer_step: LayerStepModel, append: bool, override: bool) -> bool:
     if layer_step and not append and not override:
         raise LayerStepExistsError(
             f"Layer step {layer_step.datetime} with layer id {layer_step.layer_id} already exists."
-            f" Do yo want to override the layer step and delete all associated data?")
+            f" Do yo want to override the layer step and delete all associated data?"
+        )
 
     if append and override:
         raise LayerStepAppendOverwriteError(
             "You can either append data to a layer step or override the complete layer step. "
-            "Existing filenames will be overridden automatically on append.")
+            "Existing filenames will be overridden automatically on append."
+        )
 
     if (not layer_step and append) or (not layer_step and override):
         click.echo(f"Layer step {layer_step.datetime} is not existing. Layer step will be created.")
 
     return override
```

### Comparing `rastless_cli-1.8.0/rastless/db/base.py` & `rastless_cli-1.9.0/rastless/db/base.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import uuid
 
 from pydantic import BaseModel, model_validator
 
 
 def camel_case(string: str) -> str:
-    return ''.join(word.capitalize() if i > 0 else word for i, word in enumerate(string.split('_')))
+    return "".join(word.capitalize() if i > 0 else word for i, word in enumerate(string.split("_")))
 
 
 def str_uuid():
     return str(uuid.uuid4())
 
 
 class DynamoBaseModel(BaseModel):
@@ -16,16 +16,15 @@
     _pk_value: str = None
     _sk_tag: str
     _sk_value: str = None
     pk: str = None
     sk: str = None
 
     def __eq__(self, other):
-        return (self.pk == other.pk and
-                self.sk == other.sk)
+        return self.pk == other.pk and self.sk == other.sk
 
     @model_validator(mode="after")
     def new(self):
         self.pk = self.create_tag(self._pk_tag, self._pk_value)
         self.sk = self.create_tag(self._sk_tag, self._sk_value)
         return self
```

### Comparing `rastless_cli-1.8.0/rastless/db/handler.py` & `rastless_cli-1.9.0/rastless/db/handler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,142 +1,143 @@
+import json
 from typing import List, Union
 
 import boto3
-from boto3.dynamodb.conditions import Key
+from boto3.dynamodb.conditions import Attr, Key
 from pydantic import TypeAdapter
 
 from rastless.db.models import AccessToken, BaseColorMap, LayerModel, LayerStepModel, PermissionModel
 
 
 class Database:
     def __init__(self, table_name, resource=None):
         if not resource:
-            resource = boto3.resource('dynamodb')
+            resource = boto3.resource("dynamodb")
 
         self.table_name = table_name
         self.resource = resource
         self.table = self.resource.Table(table_name)
 
     def scan_table(self, pk_startswith, sk_startswith=None):
         filter_expression = Key("pk").begins_with(pk_startswith)
         if sk_startswith:
             filter_expression &= Key("sk").begins_with(sk_startswith)
 
-        scan_kwargs = {
-            "FilterExpression": filter_expression
-        }
+        scan_kwargs = {"FilterExpression": filter_expression}
 
         items_list = []
 
         done = False
         start_key = None
 
         while not done:
             if start_key:
-                scan_kwargs['ExclusiveStartKey'] = start_key
+                scan_kwargs["ExclusiveStartKey"] = start_key
             response = self.table.scan(**scan_kwargs)
             if items := response.get("Items"):
                 items_list.extend(items)
-            start_key = response.get('LastEvaluatedKey', None)
+            start_key = response.get("LastEvaluatedKey", None)
             done = start_key is None
 
         return items_list
 
     def query(self, query_params: dict) -> List:
         response = self.table.query(**query_params)
         items = response.get("Items", [])
 
-        while 'LastEvaluatedKey' in response:
-            response = self.table.query(ExclusiveStartKey=response['LastEvaluatedKey'], **query_params)
-            items.extend(response['Items'])
+        while "LastEvaluatedKey" in response:
+            response = self.table.query(ExclusiveStartKey=response["LastEvaluatedKey"], **query_params)
+            items.extend(response["Items"])
 
         return items
 
     def get_item(self, pk, sk, gsi=None):
-        response = self.table.get_item(Key={
-            "pk": pk,
-            "sk": sk
-        })
+        response = self.table.get_item(Key={"pk": pk, "sk": sk})
         return response.get("Item")
 
-    def list_layers(self):
-        query_parameters = {
-            "KeyConditionExpression": Key('pk').eq("layer")
-        }
-        return self.query(query_parameters)
+    def list_layers(self, client=None, region=None, product=None):
+        query_params = {"KeyConditionExpression": Key("pk").eq("layer")}
+        filter_expressions = []
+
+        if client:
+            filter_expressions.append(Attr("client").eq(client))
+
+        if region:
+            try:
+                numeric_region = int(region)
+                filter_expressions.append(Attr("regionId").eq(numeric_region))
+            except ValueError:
+                return []
+
+        if product:
+            filter_expressions.append(Attr("product").eq(product))
+
+        if filter_expressions:
+            combined_filter_expression = filter_expressions[0]
+            for expr in filter_expressions[1:]:
+                combined_filter_expression &= expr
+
+            query_params["FilterExpression"] = combined_filter_expression
+
+        return self.query(query_params)
 
     def add_permissions(self, permissions: List[PermissionModel]):
         with self.table.batch_writer() as writer:
             for permission in permissions:
-                writer.put_item(
-                    Item=permission.model_dump(by_alias=True)
-                )
+                writer.put_item(Item=permission.model_dump(by_alias=True))
 
     def get_permission(self, permission, layer_id):
         return self.get_item(f"permission#{permission}", f"layer#{layer_id}")
 
     def get_layers_for_permission(self, permission):
         query_parameters = {
-            "KeyConditionExpression": Key('pk').eq(f"permission#{permission}") & Key('sk').begins_with("layer")
+            "KeyConditionExpression": Key("pk").eq(f"permission#{permission}") & Key("sk").begins_with("layer")
         }
         return self.query(query_parameters)
 
     def get_permission_for_layer_id(self, layer_id):
         query_parameters = {
             "IndexName": "gsi1",
-            "KeyConditionExpression": Key('sk').eq(f"layer#{layer_id}") & Key('pk').begins_with("permission")
+            "KeyConditionExpression": Key("sk").eq(f"layer#{layer_id}") & Key("pk").begins_with("permission"),
         }
         return self.query(query_parameters)
 
     def add_layer(self, layer: LayerModel):
-        self.table.put_item(
-            Item=layer.model_dump(by_alias=True, exclude_none=True)
-        )
+        self.table.put_item(Item=layer.model_dump(by_alias=True, exclude_none=True))
 
     def get_layer(self, pk, sk) -> Union[LayerModel, None]:
         if item := self.get_item(pk, sk):
             return LayerModel.model_validate(item)
 
         return None
 
     def get_layers(self, layer_ids: set):
         response = self.resource.batch_get_item(
             RequestItems={
-                self.table_name: {
-                    "Keys": [{"pk": "layer", "sk": f"layer#{layer_id}"} for layer_id in layer_ids]
-                }
+                self.table_name: {"Keys": [{"pk": "layer", "sk": f"layer#{layer_id}"} for layer_id in layer_ids]}
             }
         )
 
         return response["Responses"][self.table_name]
 
     def delete_layer(self, layer_id: str):
-        query_parameters = {
-            "IndexName": "gsi1",
-            "KeyConditionExpression": Key('sk').eq(f"layer#{layer_id}")
-        }
+        query_parameters = {"IndexName": "gsi1", "KeyConditionExpression": Key("sk").eq(f"layer#{layer_id}")}
         items = self.query(query_parameters)
 
         with self.table.batch_writer() as writer:
             for item in items:
-                writer.delete_item(
-                    Key={"sk": item["sk"], "pk": item["pk"]}
-                )
+                writer.delete_item(Key={"sk": item["sk"], "pk": item["pk"]})
 
     def delete_permission(self, permission: str):
-        query_parameters = {
-            "KeyConditionExpression": Key('pk').eq(f"permission#{permission}")
-        }
+        query_parameters = {"KeyConditionExpression": Key("pk").eq(f"permission#{permission}")}
         items = self.query(query_parameters)
 
         with self.table.batch_writer() as writer:
             for item in items:
-                writer.delete_item(
-                    Key={"pk": item["pk"], "sk": item["sk"]}
-                )
+                writer.delete_item(Key={"pk": item["pk"], "sk": item["sk"]})
 
     def delete_layer_from_layer_permission(self, permissions: List[PermissionModel]):
         with self.table.batch_writer() as writer:
             for permission in permissions:
                 writer.delete_item(
                     Key={"pk": f"permission#{permission.permission}", "sk": f"layer#{permission.layer_id}"}
                 )
@@ -145,54 +146,79 @@
         response = self.table.get_item(Key={"pk": f"step#{step}", "sk": f"layer#{layer_id}"})
         if item := response.get("Item"):
             return LayerStepModel.model_validate(item)
 
         return None
 
     def delete_layer_step(self, step: str, layer_id: str):
-        self.table.delete_item(
-            Key={"pk": f"step#{step}", "sk": f"layer#{layer_id}"}
-        )
+        self.table.delete_item(Key={"pk": f"step#{step}", "sk": f"layer#{layer_id}"})
 
     def get_layer_steps(self, layer_id: str) -> List[LayerStepModel]:
         query_params = {
             "IndexName": "gsi1",
-            "KeyConditionExpression": Key("sk").eq(f"layer#{layer_id}") & Key("pk").begins_with("step")
+            "KeyConditionExpression": Key("sk").eq(f"layer#{layer_id}") & Key("pk").begins_with("step"),
         }
         items = self.query(query_params)
         adapter = TypeAdapter(List[LayerStepModel])
         return adapter.validate_python(items)
 
     def add_layer_step(self, layer_step: LayerStepModel):
         self.table.put_item(Item=layer_step.model_dump(by_alias=True))
 
     def add_color_map(self, color_map: BaseColorMap):
-        self.table.put_item(
-            Item=color_map.model_dump(by_alias=True)
-        )
+        self.table.put_item(Item=color_map.model_dump(by_alias=True))
 
     def get_color_map(self, name: str) -> BaseColorMap:
         if item := self.get_item(pk="cm", sk=f"cm#{name}"):
             return BaseColorMap.colormap_factory(item)
 
     def get_color_maps(self):
         query_parameters = {
             "KeyConditionExpression": Key("pk").eq("cm"),
             "ProjectionExpression": "#name, description",
-            "ExpressionAttributeNames": {'#name': 'name'}
+            "ExpressionAttributeNames": {"#name": "name"},
         }
         return self.query(query_parameters)
 
     def delete_color_map(self, name: str):
-        self.table.delete_item(
-            Key={"pk": "cm", "sk": f"cm#{name}"}
-        )
+        self.table.delete_item(Key={"pk": "cm", "sk": f"cm#{name}"})
 
     def create_access_token(self, access_token: AccessToken):
-        self.table.put_item(
-            Item=access_token.model_dump(by_alias=True)
-        )
+        self.table.put_item(Item=access_token.model_dump(by_alias=True))
 
     def delete_access_token(self, access_token_id: str):
-        self.table.delete_item(
-            Key={"pk": f"token#{access_token_id}", "sk": "token"}
-        )
+        self.table.delete_item(Key={"pk": f"token#{access_token_id}", "sk": "token"})
+
+    def get_cached_statistics(self, cache_key_startswith: str) -> List:
+        query_params = {
+            "IndexName": "gsi1",
+            "KeyConditionExpression": Key("sk").eq("cache") & Key("pk").begins_with(cache_key_startswith),
+            "ProjectionExpression": "#1",
+            "ExpressionAttributeNames": {"#1": "data"},
+        }
+
+        items = self.query(query_params)
+
+        return [json.loads(item["data"]) for item in items]
+
+    def set_cached_statistic(self, cache_key: str, data, ttl: int):
+        self.table.put_item(Item={"pk": cache_key, "sk": "cache", "data": json.dumps(data), "ttl": ttl})
+
+    def delete_cached_statistics(self, layer_id: str = None, datetime: str = None):
+        key_condition_expression = Key("sk").eq("cache")
+        if layer_id:
+            key_condition_expression &= Key("pk").begins_with(f"cache#{layer_id}")
+
+        query_params = {
+            "IndexName": "gsi1",
+            "KeyConditionExpression": key_condition_expression,
+            "ProjectionExpression": "pk, sk",
+        }
+
+        items_to_delete = self.query(query_params)
+
+        if datetime:
+            items_to_delete = [item for item in items_to_delete if datetime in item["pk"]]
+
+        with self.table.batch_writer() as batch:
+            for item in items_to_delete:
+                batch.delete_item(Key={"pk": item["pk"], "sk": item["sk"]})
```

### Comparing `rastless_cli-1.8.0/rastless/db/models.py` & `rastless_cli-1.9.0/rastless/db/models.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from decimal import Decimal
 from typing import Annotated, List, Optional, Set
 
 from pydantic import BaseModel, Field, PlainSerializer, ValidationError, field_validator, model_validator
 
 from rastless.db.base import DynamoBaseModel, camel_case, str_uuid
 
-FloatDecimal = Annotated[Decimal, PlainSerializer(lambda x: float(x), return_type=float, when_used='json')]
+FloatDecimal = Annotated[Decimal, PlainSerializer(lambda x: float(x), return_type=float, when_used="json")]
 
 
 class LayerModel(DynamoBaseModel):
     layer_id: str = Field(default_factory=str_uuid)
     client: str
     product: str
     title: str
@@ -35,15 +35,15 @@
 
 
 class CogFile(BaseModel):
     s3_filepath: str
     bbox: tuple[Decimal, Decimal, Decimal, Decimal]
 
     @classmethod
-    @field_validator('bbox', mode="before")
+    @field_validator("bbox", mode="before")
     def to_decimal(cls, value):
         return [Decimal(str(item)) if not isinstance(item, Decimal) else item for item in value]
 
     class Config:
         populate_by_name = True
         alias_generator = camel_case
 
@@ -62,30 +62,29 @@
 
     _pk_tag = "step"
     _pk_value = "datetime"
     _sk_tag = "layer"
     _sk_value = "layer_id"
 
     @classmethod
-    @field_validator('bbox', mode="before")
+    @field_validator("bbox", mode="before")
     def to_decimal(cls, value):
         return [Decimal(str(item)) if not isinstance(item, Decimal) else item for item in value]
 
 
 class BaseColorMap(DynamoBaseModel):
     name: str
     description: Optional[str] = None
 
     _pk_tag = "cm"
     _sk_tag = "cm"
     _sk_value = "name"
 
     def __eq__(self, other):
-        return (super().__eq__(other) and self.name == other.name and
-                self.description == other.description)
+        return super().__eq__(other) and self.name == other.name and self.description == other.description
 
     @classmethod
     def colormap_factory(cls, item):
         cm_models = [MplColorMap, DiscreteColorMap, SldColorMap]
         for model in cm_models:
             try:
                 return model.model_validate(item)
@@ -101,52 +100,59 @@
     legend_image: Optional[str] = None
 
     _pk_tag = "cm"
     _sk_tag = "cm"
     _sk_value = "name"
 
     def __eq__(self, other):
-        return (super().__eq__(other) and
-                self.values == other.values and
-                self.colors == other.colors and
-                self.nodata == other.nodata and
-                self.legend_image == other.legend_image)
+        return (
+            super().__eq__(other)
+            and self.values == other.values
+            and self.colors == other.colors
+            and self.nodata == other.nodata
+            and self.legend_image == other.legend_image
+        )
 
 
 class DiscreteColorMap(BaseColorMap):
     values: List[int]
     colors: List[tuple[int, int, int, int]]
     labels: List[str]
 
-    @model_validator(mode='after')
+    @model_validator(mode="after")
     def validate_list_lengths(self):
         if len(self.values) != len(self.colors) != len(self.labels):
-            raise ValueError(f"Invalid colormap, cm#{self.sk} does not have same amount of colors, "
-                             f"labels and values")
+            raise ValueError(
+                f"Invalid colormap, cm#{self.sk} does not have same amount of colors, " f"labels and values"
+            )
         return self
 
     def __eq__(self, other):
-        return (super().__eq__(other) and
-                self.values == other.values and
-                self.colors == other.colors and
-                self.labels == other.labels)
+        return (
+            super().__eq__(other)
+            and self.values == other.values
+            and self.colors == other.colors
+            and self.labels == other.labels
+        )
 
 
 class MplColorMap(BaseColorMap):
     min: FloatDecimal
     max: FloatDecimal
     log: bool
     cmap_name: str
 
     def __eq__(self, other):
-        return (super().__eq__(other) and
-                self.min == other.min and
-                self.max == other.max and
-                self.log == other.log and
-                self.cmap_name == other.cmap_name)
+        return (
+            super().__eq__(other)
+            and self.min == other.min
+            and self.max == other.max
+            and self.log == other.log
+            and self.cmap_name == other.cmap_name
+        )
 
 
 class AccessToken(DynamoBaseModel):
     token: str
     layer_ids: Set[str]
 
     _pk_tag = "token"
```

### Comparing `rastless_cli-1.8.0/rastless/main.py` & `rastless_cli-1.9.0/rastless/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import click
 
 from rastless.cli import colormaps, layers, management, permissions
 from rastless.config import create_config
 
 
 @click.group()
-@click.option('--dev', is_flag=True)
-@click.option('--test', is_flag=True)
+@click.option("--dev", is_flag=True)
+@click.option("--test", is_flag=True)
 @click.version_option(package_name="rastless-cli")
 @click.pass_context
 def cli(ctx, dev, test):
     if dev and test:
-        raise click.UsageError('DEV and TEST can not both be true, choose one environment.')
+        raise click.UsageError("DEV and TEST can not both be true, choose one environment.")
     ctx.obj = create_config(dev, test)
 
 
 # Management
 cli.add_command(management.check_aws_connection)
 
 # Layers
 cli.add_command(layers.create_layer)
 cli.add_command(layers.create_timestep)
 cli.add_command(layers.list_layers)
 cli.add_command(layers.delete_layer)
 cli.add_command(layers.layer_exists)
 cli.add_command(layers.delete_layer_timestep)
+cli.add_command(layers.delete_cache)
 
 # Colormaps
 cli.add_command(colormaps.add_sld_colormap)
 cli.add_command(colormaps.add_mpl_colormap)
 cli.add_command(colormaps.add_discrete_colormap)
 cli.add_command(colormaps.delete_colormap)
 cli.add_command(colormaps.list_colormaps)
@@ -37,9 +38,10 @@
 cli.add_command(permissions.add_permission)
 cli.add_command(permissions.delete_permission)
 cli.add_command(permissions.delete_layer_permission)
 cli.add_command(permissions.get_permissions)
 cli.add_command(permissions.add_access_token)
 cli.add_command(permissions.delete_access_token)
 
-if __name__ == '__main__':
+
+if __name__ == "__main__":
     cli()
```

### Comparing `rastless_cli-1.8.0/rastless/settings.py` & `rastless_cli-1.9.0/rastless/settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,7 +6,11 @@
 RASTLESS_TABLE_NAME = os.getenv("RASTLESS_TABLE_NAME", "rastless-prod")
 RASTLESS_TABLE_NAME_DEV = os.getenv("RASTLESS_TABLE_NAME_DEV", "rastless-dev")
 RASTLESS_TABLE_NAME_TEST = os.getenv("RASTLESS_TABLE_NAME_TEST", "rastless-end2end-test")
 
 RASTLESS_BUCKET_NAME = os.getenv("RASTLESS_BUCKET_NAME", "rastless-prod")
 RASTLESS_BUCKET_NAME_DEV = os.getenv("RASTLESS_BUCKET_NAME_DEV", "rastless-dev")
 RASTLESS_BUCKET_NAME_TEST = os.getenv("RASTLESS_BUCKET_NAME_TEST", "rastless-end2end-test")
+
+RASTLESS_BUCKET_NAME_CACHE = os.getenv("RASTLESS_BUCKET_NAME_CACHE", "rastless-cache-prod")
+RASTLESS_BUCKET_NAME_CACHE_DEV = os.getenv("RASTLESS_BUCKET_NAME_CACHE_DEV", "rastless-cache-dev")
+RASTLESS_BUCKET_NAME_CACHE_TEST = os.getenv("RASTLESS_BUCKET_NAME_CACHE_TEST", "rastless-cache-end2end-test")
```

### Comparing `rastless_cli-1.8.0/PKG-INFO` & `rastless_cli-1.9.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rastless-cli
-Version: 1.8.0
+Version: 1.9.0
 Summary: A cli for managing data and user access for the cloud application rastless
 Author: Marcel Siegmann
 Author-email: siegmann@eomap.de
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -91,25 +91,31 @@
 
 # Example production
 $ rastless list-layers
 ```
 
 ## Commands Overview
 
-| Commands             |                                                     |
-|----------------------|-----------------------------------------------------|
-| add-colormap         | Add a SLD file                                      |
-| add-permission       | Add a role to one or multiple layers                |
-| check-aws-connection | Check if cli can connect to aws                     |
-| create-layer         | Create layer                                        |
-| create-timestep      | Create timestep entry and upload layer to S3 bucket |
-| delete-colormap      | Remove a SLD file                                   |
-| delete-layer         | Delete a layer with all timestep entries            |
-| delete-permission    | Delete one or multiple permissions                  |
-| list-layers          | List all layers                                     |
+| Commands              |                                                       |
+|-----------------------|-------------------------------------------------------|
+| add-mpl-colormap      | Add a custom colormap based on matplotlib colormaps   |
+| add-discrete-colormap | Add a discrete colormap based on matplotlib colormaps |
+| add-sld-colormap      | Add a SLD file                                        |
+| add-permission        | Add a role to one or multiple layers                  |
+| check-aws-connection  | Check if cli can connect to aws                       |
+| create-layer          | Create layer                                          |
+| create-timestep       | Create timestep entry and upload layer to S3 bucket   |
+| delete-colormap       | Remove a SLD file                                     |
+| delete-layer          | Delete a layer with all timestep entries              |
+| delete-permission     | Delete one or multiple permissions                    |
+| delete-layer-timestep | Delete one or multiple layer timesteps                |
+| delete-cache          | Deletes cache                                         |
+| list-layers           | List all layers                                       |
+| list-colormaps        | List all colormaps                                    |
+| layer-exists          | Check if layer id exists                              |
 
 ## Accomplishing a running system
 
 #### 1. Check if you have access to the system
 
 ```bash
 $ rastless check-aws-connection
@@ -170,14 +176,18 @@
 # Now: Override existing timestep. Flag: -o
 rastless create-timestep -f file1.tif -f file2.tif -d 2020-01-01T15:00:00 -s Sent2 -layer-id 1234 -t daily -p deflate -o
 
 # Now: Append file to existing timestep. Flag: -a
 rastless create-timestep -f file2.tif -d 2020-01-01T15:00:00 -layer-id 1234 -p deflate -a
 ```
 
+### Version 1.7.0
+- Add new endoints to delete layer cache in s3 bucket and dynamodb
+- List-layer now has filter options for region_id, client and product
+
 ## Publish and Release
 
 When releasing we use [semantic versioning](https://semver.org/) to define the new version tag.
 
 When pushing to master any commit message that includes #major, #minor, #patch will add a tag to the commit
 with the respective version bump. If #none is contained in the merge commit message, it will skip the version bump.
 When none of the above types is provided the default version bump (minor) is triggered. After the tagging a package
```

