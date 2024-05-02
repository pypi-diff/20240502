# Comparing `tmp/odoo_openupgrade_wizard-0.6.0.tar.gz` & `tmp/odoo_openupgrade_wizard-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odoo_openupgrade_wizard-0.6.0.tar", max compression
+gzip compressed data, was "odoo_openupgrade_wizard-0.7.0.tar", max compression
```

## Comparing `odoo_openupgrade_wizard-0.6.0.tar` & `odoo_openupgrade_wizard-0.7.0.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0    15464 2024-02-22 07:54:03.942560 odoo_openupgrade_wizard-0.6.0/README.md
--rw-r--r--   0        0        0      131 2023-11-09 12:08:57.560506 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/__init__.py
--rw-r--r--   0        0        0      142 2023-11-09 12:08:57.560506 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/__main__.py
--rw-r--r--   0        0        0     4652 2024-03-01 21:11:49.613201 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli.py
--rw-r--r--   0        0        0      546 2023-11-09 12:08:57.560506 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_copydb.py
--rw-r--r--   0        0        0     1824 2023-11-09 16:00:22.573825 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_docker_build.py
--rw-r--r--   0        0        0      373 2024-02-22 07:54:03.942560 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_dropdb.py
--rw-r--r--   0        0        0     3160 2023-11-09 12:08:57.560506 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_dumpdb.py
--rw-r--r--   0        0        0     2525 2023-11-09 12:08:57.560506 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_estimate_workload.py
--rw-r--r--   0        0        0      866 2023-11-09 12:08:57.560506 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_execute_script_python.py
--rw-r--r--   0        0        0      864 2023-11-09 12:08:57.560506 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_execute_script_sql.py
--rw-r--r--   0        0        0     4617 2023-11-09 16:00:22.573825 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_generate_module_analysis.py
--rw-r--r--   0        0        0      880 2023-11-09 12:08:57.560506 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_get_code.py
--rw-r--r--   0        0        0     5549 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_init.py
--rw-r--r--   0        0        0     2883 2024-03-03 08:25:45.633875 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_install_from_csv.py
--rw-r--r--   0        0        0     3279 2024-03-03 08:25:45.637875 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_options.py
--rw-r--r--   0        0        0      727 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_psql.py
--rw-r--r--   0        0        0     1900 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_pull_submodule.py
--rw-r--r--   0        0        0     2154 2024-03-02 23:00:00.880740 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_restoredb.py
--rw-r--r--   0        0        0     2271 2024-03-03 08:25:45.637875 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_run.py
--rw-r--r--   0        0        0     1369 2024-03-03 08:25:45.637875 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_upgrade.py
--rw-r--r--   0        0        0     8559 2024-03-01 15:12:57.400429 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/configuration_version_dependant.py
--rw-r--r--   0        0        0       14 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/templates/.gitignore.j2
--rw-r--r--   0        0        0     4978 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/templates/analysis.html.j2
--rw-r--r--   0        0        0     1538 2024-03-20 11:26:47.954759 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/templates/config.yml.j2
--rw-r--r--   0        0        0        0 2024-03-20 16:28:39.879440 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/templates/custom-postgres.conf.j2
--rw-r--r--   0        0        0       10 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/templates/modules.csv.j2
--rw-r--r--   0        0        0     1931 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/templates/odoo/11.0/Dockerfile
--rw-r--r--   0        0        0     1930 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/templates/odoo/12.0/Dockerfile
--rw-r--r--   0        0        0     1720 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/templates/odoo/13.0/Dockerfile
--rw-r--r--   0        0        0     1570 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/templates/odoo/14.0/Dockerfile
--rw-r--r--   0        0        0     1570 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/templates/odoo/15.0/Dockerfile
--rw-r--r--   0        0        0     1570 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/templates/odoo/16.0/Dockerfile
--rw-r--r--   0        0        0        0 2024-03-20 16:28:39.879440 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/templates/odoo/extra_debian_requirements.txt.j2
--rw-r--r--   0        0        0      355 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/templates/odoo/extra_python_requirements.txt.j2
--rw-r--r--   0        0        0      314 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/templates/odoo/odoo.conf.j2
--rw-r--r--   0        0        0     1303 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/templates/odoo/repos.yml.j2
--rw-r--r--   0        0        0      179 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/templates/scripts/post-migration.py.j2
--rw-r--r--   0        0        0        0 2024-03-20 16:28:39.879440 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/templates/scripts/pre-migration.sql.j2
--rw-r--r--   0        0        0     1326 2024-02-22 07:54:03.942560 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/tools/tools_click_odoo_contrib.py
--rw-r--r--   0        0        0     4391 2023-11-09 18:06:28.344693 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/tools/tools_docker.py
--rw-r--r--   0        0        0    12142 2024-03-01 15:12:57.400429 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/tools/tools_odoo.py
--rw-r--r--   0        0        0     4927 2023-11-09 16:00:22.577825 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/tools/tools_odoo_instance.py
--rw-r--r--   0        0        0    29695 2024-03-01 15:12:57.404429 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/tools/tools_odoo_module.py
--rw-r--r--   0        0        0     8065 2024-03-01 21:11:49.617201 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/tools/tools_postgres.py
--rw-r--r--   0        0        0     5128 2024-03-01 21:11:49.617201 odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/tools/tools_system.py
--rw-r--r--   0        0        0     1747 2024-03-20 11:26:47.954759 odoo_openupgrade_wizard-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    17061 1970-01-01 00:00:00.000000 odoo_openupgrade_wizard-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    15464 2024-02-22 07:54:03.942560 odoo_openupgrade_wizard-0.7.0/README.md
+-rw-r--r--   0        0        0      131 2023-11-09 12:08:57.560506 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/__init__.py
+-rw-r--r--   0        0        0      142 2023-11-09 12:08:57.560506 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/__main__.py
+-rw-r--r--   0        0        0     5471 2024-05-02 20:14:54.323424 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli.py
+-rw-r--r--   0        0        0      546 2023-11-09 12:08:57.560506 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_copydb.py
+-rw-r--r--   0        0        0     1818 2024-03-23 19:50:04.104055 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_docker_build.py
+-rw-r--r--   0        0        0      373 2024-02-22 07:54:03.942560 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_dropdb.py
+-rw-r--r--   0        0        0     3160 2023-11-09 12:08:57.560506 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_dumpdb.py
+-rw-r--r--   0        0        0     2525 2023-11-09 12:08:57.560506 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_estimate_workload.py
+-rw-r--r--   0        0        0      866 2023-11-09 12:08:57.560506 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_execute_script_python.py
+-rw-r--r--   0        0        0      864 2023-11-09 12:08:57.560506 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_execute_script_sql.py
+-rw-r--r--   0        0        0     4638 2024-04-30 13:13:00.572724 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_generate_module_analysis.py
+-rw-r--r--   0        0        0      880 2023-11-09 12:08:57.560506 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_get_code.py
+-rw-r--r--   0        0        0     5996 2024-03-23 20:59:26.155584 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_init.py
+-rw-r--r--   0        0        0     2868 2024-04-30 13:13:00.572724 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_install_from_csv.py
+-rw-r--r--   0        0        0     3263 2024-03-23 19:50:04.108055 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_options.py
+-rw-r--r--   0        0        0      727 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_psql.py
+-rw-r--r--   0        0        0     1900 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_pull_submodule.py
+-rw-r--r--   0        0        0     2154 2024-03-02 23:00:00.880740 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_restoredb.py
+-rw-r--r--   0        0        0     2295 2024-04-30 13:13:00.576725 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_run.py
+-rw-r--r--   0        0        0     1379 2024-04-30 13:13:00.576725 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_upgrade.py
+-rw-r--r--   0        0        0     8559 2024-03-01 15:12:57.400429 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/configuration_version_dependant.py
+-rw-r--r--   0        0        0       14 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/templates/.gitignore.j2
+-rw-r--r--   0        0        0     4978 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/templates/analysis.html.j2
+-rw-r--r--   0        0        0     1604 2024-03-22 21:50:05.607389 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/templates/config.yml.j2
+-rw-r--r--   0        0        0        0 2024-05-02 20:45:28.350244 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/templates/custom-postgres.conf.j2
+-rw-r--r--   0        0        0       10 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/templates/modules.csv.j2
+-rw-r--r--   0        0        0     1931 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/templates/odoo/11.0/Dockerfile
+-rw-r--r--   0        0        0     1930 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/templates/odoo/12.0/Dockerfile
+-rw-r--r--   0        0        0     1720 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/templates/odoo/13.0/Dockerfile
+-rw-r--r--   0        0        0     1570 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/templates/odoo/14.0/Dockerfile
+-rw-r--r--   0        0        0     1570 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/templates/odoo/15.0/Dockerfile
+-rw-r--r--   0        0        0     1570 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/templates/odoo/16.0/Dockerfile
+-rw-r--r--   0        0        0        0 2024-05-02 20:45:28.350244 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/templates/odoo/extra_debian_requirements.txt.j2
+-rw-r--r--   0        0        0      355 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/templates/odoo/extra_python_requirements.txt.j2
+-rw-r--r--   0        0        0      314 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/templates/odoo/odoo.conf.j2
+-rw-r--r--   0        0        0     1303 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/templates/odoo/repos.yml.j2
+-rw-r--r--   0        0        0      179 2023-11-09 12:08:57.564506 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/templates/scripts/post-migration.py.j2
+-rw-r--r--   0        0        0        0 2024-05-02 20:45:28.350244 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/templates/scripts/pre-migration.sql.j2
+-rw-r--r--   0        0        0     1196 2024-03-23 19:54:18.858719 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/tools/tools_click_odoo_contrib.py
+-rw-r--r--   0        0        0     4005 2024-04-30 13:13:00.576725 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/tools/tools_docker.py
+-rw-r--r--   0        0        0    11952 2024-04-30 13:13:00.576725 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/tools/tools_odoo.py
+-rw-r--r--   0        0        0     4373 2024-03-23 20:59:26.155584 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/tools/tools_odoo_instance.py
+-rw-r--r--   0        0        0    29234 2024-03-23 19:50:04.112055 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/tools/tools_odoo_module.py
+-rw-r--r--   0        0        0     8205 2024-05-02 20:14:54.323424 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/tools/tools_postgres.py
+-rw-r--r--   0        0        0     5113 2024-03-23 19:50:04.112055 odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/tools/tools_system.py
+-rw-r--r--   0        0        0     1749 2024-05-02 20:18:48.073687 odoo_openupgrade_wizard-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    17072 1970-01-01 00:00:00.000000 odoo_openupgrade_wizard-0.7.0/PKG-INFO
```

### Comparing `odoo_openupgrade_wizard-0.6.0/README.md` & `odoo_openupgrade_wizard-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli.py` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -29,14 +29,17 @@
 from odoo_openupgrade_wizard.cli.cli_psql import psql
 from odoo_openupgrade_wizard.cli.cli_pull_submodule import pull_submodule
 from odoo_openupgrade_wizard.cli.cli_restoredb import restoredb
 from odoo_openupgrade_wizard.cli.cli_run import run
 from odoo_openupgrade_wizard.cli.cli_upgrade import upgrade
 from odoo_openupgrade_wizard.tools.tools_system import ensure_folder_exists
 
+DEFAULT_CONFIG_FILE = "config.yml"
+DEFAULT_MODULES_FILE = "modules.csv"
+
 
 @click.group()
 @click.version_option(version=odoo_openupgrade_wizard.__version__)
 @click.option(
     "--env-folder",
     default="./",
     type=click.Path(
@@ -46,32 +49,57 @@
         resolve_path=True,
     ),
     help="Folder that will contains all the configuration of the wizard"
     " and all the Odoo code required to make the migrations. Let empty to"
     " use current folder (./).",
 )
 @click.option(
+    "-c",
+    "--config-file",
+    type=click.Path(
+        exists=True,
+        file_okay=True,
+    ),
+    help=(
+        f"Configuration file to use. By default, a file named "
+        f'"{DEFAULT_CONFIG_FILE}" in the environment folder will be used.'
+    ),
+)
+@click.option(
+    "--modules-file",
+    type=click.Path(
+        exists=True,
+        file_okay=True,
+    ),
+    help=(
+        f"Modules file to use. By default, a file named "
+        f'"{DEFAULT_MODULES_FILE}" in the environment folder will be used.'
+    ),
+)
+@click.option(
     "--filestore-folder",
     type=click.Path(
         exists=True, file_okay=False, writable=True, resolve_path=True
     ),
     help="Folder that contains the Odoo filestore of the database(s)"
     " to migrate. Let empty to use the subfolder 'filestore' of the"
     " environment folder.",
 )
 @click.option("-l", "--log-level", type=LogLevel(), default=logging.INFO)
 @click.pass_context
-def main(ctx, env_folder, filestore_folder, log_level):
+def main(
+    ctx, env_folder, config_file, modules_file, filestore_folder, log_level
+):
     """
     Provides a command set to perform odoo Community Edition migrations.
     """
     date_begin = datetime.datetime.now()
     logger.remove()
     logger.add(sys.stderr, level=log_level)
-    logger.debug("Beginning script '%s' ..." % (ctx.invoked_subcommand))
+    logger.debug(f"Beginning script '{ctx.invoked_subcommand}' ...")
     if not isinstance(ctx.obj, dict):
         ctx.obj = {}
 
     # Define all the folder required by the tools
     env_folder_path = Path(env_folder)
     src_folder_path = env_folder_path / Path("./src/")
     if filestore_folder:
@@ -88,16 +116,23 @@
     # Create log file
     log_prefix = "{}__{}".format(
         date_begin.strftime("%Y_%m_%d__%H_%M_%S"), ctx.invoked_subcommand
     )
     log_file_path = log_folder_path / Path(log_prefix + ".log")
     logger.add(log_file_path)
 
-    config_file_path = env_folder_path / Path("config.yml")
-    module_file_path = env_folder_path / Path("modules.csv")
+    if config_file:
+        config_file_path = Path(config_file)
+    else:
+        config_file_path = env_folder_path / Path(DEFAULT_CONFIG_FILE)
+
+    if modules_file:
+        module_file_path = Path(modules_file)
+    else:
+        module_file_path = env_folder_path / Path(DEFAULT_MODULES_FILE)
 
     # Add all global values in the context
     ctx.obj["env_folder_path"] = env_folder_path
     ctx.obj["src_folder_path"] = src_folder_path
     ctx.obj["filestore_folder_path"] = filestore_folder_path
     ctx.obj["script_folder_path"] = script_folder_path
     ctx.obj["log_folder_path"] = log_folder_path
```

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_copydb.py` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_copydb.py`

 * *Files identical despite different names*

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_docker_build.py` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_docker_build.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,16 +37,16 @@
                 "Have your run the get-code command ?",
                 odoo_version=odoo_version,
                 odoo_requirement_file_path=odoo_requirement_file_path,
             )
             continue
 
         logger.info(
-            "Building Odoo docker image for version '%s'. "
-            "This can take a while..." % (odoo_version)
+            f"Building Odoo docker image for version '{odoo_version}'."
+            " This can take a while..."
         )
         image = build_image(
             get_odoo_env_path(ctx, odoo_version),
             get_docker_image_tag(ctx, odoo_version),
             {"LOCAL_USER_ID": str(get_local_user_id())},
         )
-        logger.info("Docker Image build. '%s'" % image[0].tags[0])
+        logger.info(f"Docker Image build. '{image[0].tags[0]}'")
```

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_dumpdb.py` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_dumpdb.py`

 * *Files identical despite different names*

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_estimate_workload.py` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_estimate_workload.py`

 * *Files identical despite different names*

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_execute_script_python.py` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_execute_script_python.py`

 * *Files identical despite different names*

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_execute_script_sql.py` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_execute_script_sql.py`

 * *Files identical despite different names*

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_generate_module_analysis.py` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_generate_module_analysis.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,25 +37,24 @@
 
     initial_step = migration_steps[0].copy()
     final_step = migration_steps[1].copy()
 
     alternative_xml_rpc_port = ctx.obj["config"]["odoo_host_xmlrpc_port"] + 10
 
     if not database:
-        database = "%s__analysis__" % (
-            ctx.obj["config"]["project_name"].replace("-", "_"),
+        database = (
+            f"{ctx.obj['config']['project_name'].replace('-', '_')}"
+            "__analysis__"
         )
 
-    initial_database = "%s_%s" % (
-        database,
-        str(initial_step["version"]).replace(".", ""),
+    initial_database = (
+        f"{database}_{str(initial_step['version']).replace('.', '')}"
     )
-    final_database = "%s_%s" % (
-        database,
-        str(final_step["version"]).replace(".", ""),
+    final_database = (
+        f"{database}_{str(final_step['version']).replace('.', '')}"
     )
 
     modules = modules and modules.split(",") or []
 
     try:
         # INITIAL : Run odoo and install analysis module
         run_odoo(
@@ -71,14 +70,15 @@
         # INITIAL : Run odoo for odoorpc
         initial_container = run_odoo(
             ctx,
             initial_step,
             database=initial_database,
             execution_context="openupgrade",
             detached_container=True,
+            publish_ports=True,
         )
         # INITIAL : install modules to analyse and generate records
         initial_instance = OdooInstance(ctx, initial_database)
         initial_modules = (
             modules
             and modules
             or get_installable_odoo_modules(initial_instance, initial_step)
@@ -91,29 +91,29 @@
             ctx,
             final_step,
             database=final_database,
             detached_container=False,
             stop_after_init=True,
             init=get_upgrade_analysis_module(final_step),
             execution_context="openupgrade",
-            alternative_xml_rpc_port=alternative_xml_rpc_port,
         )
 
         # name of the first odoo instance inside the second odoo instance
         odoo_initial_host_name = "odoo_initial_instance"
 
         # FINAL : Run odoo for odoorpc and install modules to analyse
         run_odoo(
             ctx,
             final_step,
             database=final_database,
             detached_container=True,
             alternative_xml_rpc_port=alternative_xml_rpc_port,
             execution_context="openupgrade",
             links={initial_container.name: odoo_initial_host_name},
+            publish_ports=True,
         )
 
         # FINAL : install modules to analyse and generate records
         final_instance = OdooInstance(
             ctx,
             final_database,
             alternative_xml_rpc_port=alternative_xml_rpc_port,
@@ -139,9 +139,9 @@
             odoo_initial_host_name,
             initial_database,
         )
 
     except (KeyboardInterrupt, SystemExit):
         logger.info("Received Keyboard Interrupt or System Exiting...")
     finally:
-        kill_odoo(ctx, initial_step)
-        kill_odoo(ctx, final_step)
+        kill_odoo(ctx, initial_database, initial_step)
+        kill_odoo(ctx, final_database, final_step)
```

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_get_code.py` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_get_code.py`

 * *Files identical despite different names*

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_init.py` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_init.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,23 +33,37 @@
 @click.option(
     "--final-version",
     required=True,
     prompt=True,
     type=click.Choice(get_version_options("final")),
 )
 @click.option(
+    "--postgresql-version",
+    required=True,
+    help="The version of postgresql that will be used"
+    " to create the postgresql container.Ex : '9.1', '16', ..."
+    " The version should be available in docker hub."
+    " (https://hub.docker.com/_/postgres)"
+    " avoid the 'latest' version if you want a deterministic installation.",
+)
+@click.option(
     "--extra-repository",
     "extra_repository_list",
     # TODO, add a callback to check the quality of the argument
     help="Coma separated extra repositories to use in the odoo environment."
     "Ex: 'OCA/web,OCA/server-tools,GRAP/grap-odoo-incubator'",
 )
 @click.pass_context
 def init(
-    ctx, project_name, initial_version, final_version, extra_repository_list
+    ctx,
+    project_name,
+    initial_version,
+    final_version,
+    postgresql_version,
+    extra_repository_list,
 ):
     """Initialize OOW Environment based on the initial and
     the final version of Odoo you want to migrate.
     """
 
     # Handle arguments
     if extra_repository_list:
@@ -71,51 +85,54 @@
 
     # Create initial Regular step
     steps = [
         {
             "name": 1,
             "execution_context": "regular",
             "version": odoo_versions[0],
-            "complete_name": "step_01__regular__%s" % (odoo_versions[0]),
+            "complete_name": f"step_01__regular__{odoo_versions[0]}",
         }
     ]
     # Add all Openupgrade steps
     step_nbr = 2
     for odoo_version in odoo_versions[1:]:
         steps.append(
             {
                 "name": step_nbr,
                 "execution_context": "openupgrade",
                 "version": odoo_version,
-                "complete_name": "step_%s__openupgrade__%s"
-                % (str(step_nbr).rjust(2, "0"), odoo_version),
+                "complete_name": (
+                    f"step_{step_nbr:>02}__openupgrade__{odoo_version}"
+                ),
             }
         )
         step_nbr += 1
 
     # add final Regular step
     if len(odoo_versions) > 1:
         steps.append(
             {
                 "name": step_nbr,
                 "execution_context": "regular",
                 "version": odoo_versions[-1],
-                "complete_name": "step_%s__regular__%s"
-                % (str(step_nbr).rjust(2, "0"), odoo_versions[-1]),
+                "complete_name": (
+                    f"step_{step_nbr:>02}__regular__{odoo_versions[-1]}"
+                ),
             }
         )
 
     # Ensure src folder exists
     ensure_folder_exists(ctx.obj["src_folder_path"])
 
     # Ensure main configuration file exists
     ensure_file_exists_from_template(
         ctx.obj["config_file_path"],
         "config.yml.j2",
         project_name=project_name,
+        postgresql_version=postgresql_version,
         steps=steps,
         odoo_versions=odoo_versions,
     )
 
     # Ensure module list file exists
     ensure_file_exists_from_template(
         ctx.obj["module_file_path"],
```

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_install_from_csv.py` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_install_from_csv.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,26 +22,27 @@
 def install_from_csv(ctx, database, with_demo):
     migration_step = get_migration_step_from_options(ctx, 1)
     ensure_database(ctx, database, state="present")
 
     # Get modules list from the CSV file
     module_names = get_odoo_modules_from_csv(ctx.obj["module_file_path"])
     module_names.sort()
-    logger.info("Found %d modules." % (len(module_names)))
+    logger.info(f"Found {len(module_names)} modules.")
     logger.debug(module_names)
 
     try:
-        logger.info("Install 'base' module on %s database ..." % (database))
+        logger.info(f"Install 'base' module on {database} database ...")
         run_odoo(
             ctx,
             migration_step,
             database=database,
             detached_container=True,
             init="base",
             demo=with_demo,
+            publish_ports=True,
         )
         odoo_instance = OdooInstance(ctx, database)
         odoo_default_company = ctx.obj["config"].get(
             "odoo_default_company", False
         )
         if odoo_default_company:
             # Then, set correct country to the company of the current user
@@ -51,20 +52,18 @@
 
             countries = odoo_instance.browse_by_search(
                 "res.country",
                 [("code", "=", odoo_default_company["country_code"])],
             )
             if len(countries) != 1:
                 raise Exception(
-                    "Unable to find a country, based on the code %s."
-                    " countries found : %s "
-                    % (
-                        odoo_default_company["country_code"],
-                        ", ".join([x.name for x in countries]),
-                    )
+                    f"Unable to find a country, based on the"
+                    f" code {odoo_default_company['country_code']}."
+                    f" Countries found :"
+                    f" {', '.join([x.name for x in countries])}"
                 )
             vals = {
                 "country_id": countries[0].id,
                 "currency_id": countries[0].currency_id.id,
                 "phone": odoo_default_company.get("phone"),
                 "email": odoo_default_company.get("email"),
             }
@@ -77,8 +76,8 @@
 
         # Install modules
         odoo_instance.install_modules(module_names)
 
     except (KeyboardInterrupt, SystemExit):
         logger.info("Received Keyboard Interrupt or System Exiting...")
     finally:
-        kill_odoo(ctx, migration_step)
+        kill_odoo(ctx, database, migration_step)
```

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_options.py` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_options.py`

 * *Files 9% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
 def get_migration_step_from_options(ctx, step_arg):
     step = float(step_arg)
     for migration_step in ctx.obj["config"]["migration_steps"]:
         if migration_step["name"] == step:
             return migration_step
     raise ValueError(
-        "No migration step found in configuration for step %s" % step_arg
+        f"No migration step found in configuration for step {step_arg}"
     )
 
 
 def get_migration_steps_from_options(ctx, first_step_arg, last_step_arg):
     result = []
     if first_step_arg:
         first_step = int(first_step_arg)
@@ -110,11 +110,10 @@
     for migration_step in ctx.obj["config"]["migration_steps"]:
         if migration_step["name"] in list(range(first_step, last_step + 1)):
             result.append(migration_step.copy())
     if result:
         return result
 
     raise ValueError(
-        "Unable to define steps in configuration"
-        " from options. (first step %s ; last step %s)"
-        % (first_step_arg, last_step_arg)
+        "Unable to define steps in configuration from options."
+        f" (first step {first_step_arg} ; last step {last_step_arg})"
     )
```

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_psql.py` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_psql.py`

 * *Files identical despite different names*

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_pull_submodule.py` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_pull_submodule.py`

 * *Files identical despite different names*

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_restoredb.py` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_restoredb.py`

 * *Files identical despite different names*

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_run.py` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_run.py`

 * *Files 6% similar despite different names*

```diff
@@ -63,19 +63,19 @@
             database=database,
             detached_container=not stop_after_init,
             init=init_modules,
             update=update_modules,
             stop_after_init=stop_after_init,
             demo=with_demo,
             execution_context=execution_context,
+            publish_ports=True,
         )
         if not stop_after_init:
             logger.info(
-                "Odoo is available on your host at"
-                " http://localhost:%s"
-                % ctx.obj["config"]["odoo_host_xmlrpc_port"]
+                "Odoo is available on your host at http://localhost:"
+                f"{ctx.obj['config']['odoo_host_xmlrpc_port']}"
             )
             input("Press 'Enter' to kill the odoo container and exit ...")
     except (KeyboardInterrupt, SystemExit):
         logger.info("Received Keyboard Interrupt or System Exiting...")
     finally:
-        kill_odoo(ctx, migration_step)
+        kill_odoo(ctx, database, migration_step)
```

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/cli/cli_upgrade.py` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/cli/cli_upgrade.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,9 +39,9 @@
                 update="all",
                 stop_after_init=True,
                 demo=with_demo,
             )
         except (KeyboardInterrupt, SystemExit):
             logger.info("Received Keyboard Interrupt or System Exiting...")
         finally:
-            kill_odoo(ctx, migration_step)
+            kill_odoo(ctx, database, migration_step)
         execute_click_odoo_python_files(ctx, database, migration_step)
```

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/configuration_version_dependant.py` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/configuration_version_dependant.py`

 * *Files identical despite different names*

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/templates/analysis.html.j2` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/templates/analysis.html.j2`

 * *Files identical despite different names*

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/templates/config.yml.j2` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/templates/config.yml.j2`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 project_name: {{ project_name }}
 
 
-postgres_image_name: postgres:13
-postgres_container_name: {{project_name}}-container-postgres
-postgres_volume_name: {{project_name}}-volume-postgres
+postgres_image_name: postgres:{{postgresql_version}}
+postgres_container_name: {{project_name}}-container-postgres-{{postgresql_version}}
+postgres_volume_name: {{project_name}}-volume-postgres-{{postgresql_version}}
 postgres_extra_settings:
 
 
 odoo_rpc_timeout: 3600
 odoo_host_xmlrpc_port: 9069
 odoo_default_company:
   country_code: FR
```

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/templates/odoo/11.0/Dockerfile` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/templates/odoo/11.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/templates/odoo/12.0/Dockerfile` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/templates/odoo/12.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/templates/odoo/13.0/Dockerfile` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/templates/odoo/13.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/templates/odoo/14.0/Dockerfile` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/templates/odoo/14.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/templates/odoo/15.0/Dockerfile` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/templates/odoo/15.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/templates/odoo/16.0/Dockerfile` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/templates/odoo/16.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/templates/odoo/repos.yml.j2` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/templates/odoo/repos.yml.j2`

 * *Files identical despite different names*

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/tools/tools_click_odoo_contrib.py` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/tools/tools_click_odoo_contrib.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 import shutil
 
 from loguru import logger
 
-from odoo_openupgrade_wizard.tools.tools_postgres import (
-    ensure_database,
-    execute_sql_request,
-)
+from odoo_openupgrade_wizard.tools.tools_postgres import ensure_database
 
 
 def copydb(ctx, source, dest):
     # drop database if exist
     ensure_database(ctx, dest, state="absent")
 
     # Copy database
-    logger.info(f"Copy database {source} into {dest} ...")
-    request = f"CREATE DATABASE {dest} WITH TEMPLATE {source};"
-    execute_sql_request(ctx, request)
+    ensure_database(ctx, dest, state="present", template=source)
 
     main_path = ctx.obj["filestore_folder_path"] / "filestore"
     source_path = main_path / source
     dest_path = main_path / dest
     # Drop filestore if exist
     logger.info(f"Remove filestore of '{dest}' if exists.")
     shutil.rmtree(dest_path, ignore_errors=True)
```

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/tools/tools_docker.py` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/tools/tools_docker.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 def pull_image(image_name):
     client = get_docker_client()
     client.images.pull(image_name)
 
 
 def build_image(path, tag, buildargs={}):
     logger.debug(
-        "Building image named based on %s/Dockerfile."
-        " This can take a big while ..." % (path)
+        f"Building image named based on {path}/Dockerfile."
+        " This can take a big while ..."
     )
-    debug_docker_command = "docker build %s --tag %s" % (path, tag)
+    debug_docker_command = f"docker build {path} --tag {tag}"
     for arg_name, arg_value in buildargs.items():
         debug_docker_command += f"\\\n --build-arg {arg_name}={arg_value}"
 
-    logger.debug("DOCKER COMMAND:\n\n%s\n" % debug_docker_command)
+    logger.debug(f"DOCKER COMMAND:\n\n{debug_docker_command}\n")
     docker_client = get_docker_client()
     image = docker_client.images.build(
         path=str(path),
         tag=tag,
         buildargs=buildargs,
     )
     logger.debug("Image build.")
@@ -41,104 +41,90 @@
     links={},
     detach=False,
     auto_remove=False,
 ):
     client = get_docker_client()
     if not client.images.list(filters={"reference": image_name}):
         raise Exception(
-            "The image %s is not available on your system."
+            f"The image {image_name} is not available on your system."
             " Did you run 'odoo-openupgrade-wizard docker-build' ?"
-            % image_name
         )
 
-    logger.debug("Launching Docker container named %s ..." % (image_name))
-    debug_docker_command = "docker run --name %s\\\n" % (container_name)
+    logger.debug(f"Launching Docker container named {image_name} ...")
+    debug_docker_command = f"docker run --name {container_name}\\\n"
 
     for k, v in ports.items():
-        debug_docker_command += " --publish {k}:{v}\\\n".format(k=k, v=v)
+        debug_docker_command += f" --publish {k}:{v}\\\n"
     for k, v in volumes.items():
-        debug_docker_command += " --volume {k}:{v}\\\n".format(
-            k=str(k), v=str(v)
-        )
+        debug_docker_command += f" --volume {k}:{v}\\\n"
     for k, v in environments.items():
-        debug_docker_command += " --env {k}={v}\\\n".format(k=k, v=v)
+        debug_docker_command += f" --env {k}={v}\\\n"
     for k, v in links.items():
-        debug_docker_command += " --link {k}:{v}\\\n".format(k=k, v=v)
+        debug_docker_command += f" --link {k}:{v}\\\n"
     if auto_remove:
         debug_docker_command += " --rm"
     if detach:
         debug_docker_command += " --detach"
-    debug_docker_command += " %s" % (image_name)
+    debug_docker_command += f" {image_name}"
     if command:
-        debug_docker_command += " \\\n%s" % (command)
-    logger.debug("DOCKER COMMAND:\n%s" % debug_docker_command)
+        debug_docker_command += f" \\\n{command}"
+    logger.debug(f"DOCKER COMMAND:\n{debug_docker_command}")
 
     container = client.containers.run(
         image_name,
         name=container_name,
         command=command,
         ports={x: y for y, x in ports.items()},
         volumes=[str(k) + ":" + str(v) for k, v in volumes.items()],
         environment=environments,
         links=links,
         detach=detach,
         auto_remove=auto_remove,
     )
     if detach:
-        logger.debug("Container %s launched." % image_name)
+        logger.debug(f"Container {image_name} launched.")
     elif auto_remove:
         logger.debug("Container closed.")
 
     return container
 
 
 def exec_container(container, command):
-    debug_docker_command = "docker exec %s" % (container.name)
-    debug_docker_command += " \\\n%s" % (command)
-    logger.debug("DOCKER COMMAND:\n%s" % debug_docker_command)
+    debug_docker_command = f"docker exec {container.name}"
+    debug_docker_command += f" \\\n{command}"
+    logger.debug(f"DOCKER COMMAND:\n{debug_docker_command}")
     docker_result = container.exec_run(command)
     if docker_result.exit_code != 0:
         raise Exception(
-            "The command failed in the container %s.\n"
-            "- Command : %s\n"
-            "- Exit Code : %d\n"
-            "- Output: %s"
-            % (
-                container.name,
-                command,
-                docker_result.exit_code,
-                docker_result.output,
-            )
+            f"The command failed in the container {container.name}.\n"
+            f"- Command : {command}\n"
+            f"- Exit Code : {docker_result.exit_code}\n"
+            f"- Output: {docker_result.output}"
         )
     return docker_result
 
 
 def kill_container(container_name):
     client = get_docker_client()
 
     try:
         containers = client.containers.list(
             all=True,
             filters={"name": container_name},
             ignore_removed=True,
         )
     except docker.errors.NotFound as err:
-        logger.debug(f"Cannot kill container {container_name}: " + str(err))
+        logger.debug(f"Cannot kill container {container_name}: {err}")
         containers = []
 
     for container in containers:
         if container.status != "exited":
             logger.debug(
                 "Stop container %s, based on image '%s'."
                 % (container.name, ",".join(container.image.tags))
             )
             try:
                 container.stop()
+                container.wait()
+                container.remove()
             except docker.errors.NotFound as err:
-                logger.debug(
-                    f"Cannot kill container {container.name}: " + str(err)
-                )
-
-        # TODO, we should here filter by name
-        # but filters={"name": container_name}
-        # doesn't work...
-        client.containers.prune()
+                logger.debug(f"Cannot kill container {container.name}: {err}")
```

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/tools/tools_odoo.py` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/tools/tools_odoo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import configparser
 import csv
 import os
 import sys
 import traceback
 from pathlib import Path
 
-# import docker
 import yaml
 from loguru import logger
 
 from odoo_openupgrade_wizard.configuration_version_dependant import (
     get_base_module_folder,
     get_manifest_name,
     get_odoo_folder,
@@ -20,14 +19,16 @@
 from odoo_openupgrade_wizard.tools.tools_docker import (
     kill_container,
     run_container,
 )
 from odoo_openupgrade_wizard.tools.tools_postgres import get_postgres_container
 from odoo_openupgrade_wizard.tools.tools_system import get_script_folder
 
+DEFAULT_ODOO_HTTP_PORT = 8069
+
 
 def get_repo_file_path(ctx, odoo_version: float) -> Path:
     """return the relative path of the repos.yml file
     of a given odoo version"""
     repo_file = False
     # Check if submodule path exists
     version_cfg = (
@@ -104,21 +105,23 @@
     """Return a docker image tag, based on project name and odoo version"""
     return "odoo-openupgrade-wizard-image__%s__%s" % (
         ctx.obj["config"]["project_name"],
         str(odoo_version).rjust(4, "0"),
     )
 
 
-def get_docker_container_name(ctx, migration_step: dict) -> str:
-    """Return a docker container name, based on project name,
+def get_docker_container_name(ctx, database: str, migration_step: dict) -> str:
+    """Return a docker container name, based on project name, database name,
     odoo version and migration step"""
-    return "odoo-openupgrade-wizard-container__%s__%s__step-%s" % (
-        ctx.obj["config"]["project_name"],
-        str(migration_step["version"]).rjust(4, "0"),
-        str(migration_step["name"]).rjust(2, "0"),
+    return "oow-{project}-{database}-{version}-step-{step}".format(
+        project=ctx.obj["config"]["project_name"],
+        database=database,
+        # FIXME: version should be a string, but it is a float
+        version=str(migration_step["version"]).rjust(4, "0"),
+        step=str(migration_step["name"]).rjust(2, "0"),
     )
 
 
 def generate_odoo_command(
     ctx,
     migration_step: dict,
     execution_context: str,
@@ -212,14 +215,15 @@
     init: str = False,
     stop_after_init: bool = False,
     shell: bool = False,
     demo: bool = False,
     execution_context: str = False,
     alternative_xml_rpc_port: int = False,
     links: dict = {},
+    publish_ports: bool = False,
 ):
     # Ensure that Postgres container exist
     get_postgres_container(ctx)
     logger.info(
         "Launching Odoo Container (Version {version}) for {db_text}"
         " in {execution_context} mode. Demo Data is {demo_text}"
         " {stop_text} {init_text} {update_text}".format(
@@ -251,70 +255,62 @@
         migration_step,
         command,
         detached_container=detached_container,
         database=database,
         execution_context=execution_context,
         alternative_xml_rpc_port=alternative_xml_rpc_port,
         links=links,
+        publish_ports=publish_ports,
     )
 
 
 def run_container_odoo(
     ctx,
     migration_step: dict,
     command: str,
     detached_container: bool = False,
     database: str = False,
     alternative_xml_rpc_port: int = False,
     execution_context: str = False,
     links: dict = {},
+    publish_ports: bool = False,
 ):
     env_path = ctx.obj["env_folder_path"]
     odoo_env_path = get_odoo_env_path(ctx, migration_step["version"])
 
     host_xmlrpc_port = (
         alternative_xml_rpc_port
         and alternative_xml_rpc_port
         or ctx.obj["config"]["odoo_host_xmlrpc_port"]
     )
 
     links.update({ctx.obj["config"]["postgres_container_name"]: "db"})
 
-    # try:
+    if publish_ports:
+        ports = {host_xmlrpc_port: DEFAULT_ODOO_HTTP_PORT}
+    else:
+        ports = {}
+
     return run_container(
         get_docker_image_tag(ctx, migration_step["version"]),
-        get_docker_container_name(ctx, migration_step),
+        get_docker_container_name(ctx, database, migration_step),
         command=command,
-        ports={
-            host_xmlrpc_port: 8069,
-        },
+        ports=ports,
         volumes={
             env_path: "/env/",
             odoo_env_path: "/odoo_env/",
         },
         links=links,
         detach=detached_container,
         auto_remove=True,
     )
-    # except docker.errors.ContainerError as exception:
-    #     host_log_file_path = ctx.obj["log_folder_path"] / log_file_name
-    #     if host_log_file_path.exists():
-    #         with open(host_log_file_path) as _log_file:
-    #             logger.debug("*" * 50)
-    #             logger.debug("*" * 50)
-    #             logger.debug("*" * 50)
-    #             logger.debug(_log_file.read())
-    #             logger.debug("*" * 50)
-    #             logger.debug("*" * 50)
-    #             logger.debug("*" * 50)
-    #     raise exception
 
 
-def kill_odoo(ctx, migration_step: dict):
-    kill_container(get_docker_container_name(ctx, migration_step))
+def kill_odoo(ctx, database, migration_step: dict):
+    kill_container(get_docker_container_name(ctx, database, migration_step))
 
 
 def execute_click_odoo_python_files(
     ctx,
     database: str,
     migration_step: dict,
     python_files: list = [],
@@ -342,16 +338,16 @@
     for python_file in python_files:
         command = ("/bin/bash -c 'cat /env/{python_file} | {command}'").format(
             command=command,
             python_file=str(python_file),
         )
         try:
             logger.info(
-                "Executing script %s / %s"
-                % (migration_step["complete_name"], python_file)
+                f"Step {migration_step['complete_name']}."
+                f" Executing script {python_file} ..."
             )
             return run_container_odoo(
                 ctx,
                 migration_step,
                 command,
                 detached_container=False,
                 database=database,
@@ -361,19 +357,19 @@
             traceback.print_exc()
             logger.error(
                 "An error occured. Exiting. %s\n%s"
                 % (e, traceback.print_exception(*sys.exc_info()))
             )
             raise e
         finally:
-            kill_odoo(ctx, migration_step)
+            kill_odoo(ctx, database, migration_step)
 
 
 def get_odoo_modules_from_csv(module_file_path: Path) -> list:
-    logger.debug("Reading '%s' file ..." % module_file_path)
+    logger.debug(f"Reading '{module_file_path}' file ...")
     module_names = []
     csvfile = open(module_file_path, "r")
     spamreader = csv.reader(csvfile, delimiter=",", quotechar='"')
     for row in spamreader:
         # Try to guess that a line is not correct
         if not row:
             continue
```

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/tools/tools_odoo_instance.py` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/tools/tools_odoo_instance.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,16 +16,15 @@
     def __init__(self, ctx, database, alternative_xml_rpc_port=False):
         port = (
             alternative_xml_rpc_port
             and alternative_xml_rpc_port
             or ctx.obj["config"]["odoo_host_xmlrpc_port"]
         )
         logger.info(
-            "Connect to Odoo database %s via odoorpc (Port %s)... "
-            % (database, port)
+            f"Connect to database {database} via odoorpc (Port {port})..."
         )
 
         for x in range(1, _ODOO_RPC_MAX_TRY + 1):
             # Connection
             try:
                 rpc_connexion = odoorpc.ODOO(
                     _ODOO_RPC_URL,
@@ -34,41 +33,32 @@
                     timeout=ctx.obj["config"]["odoo_rpc_timeout"],
                 )
                 # connexion is OK
                 break
             except (socket.gaierror, socket.error) as e:
                 if x < _ODOO_RPC_MAX_TRY:
                     logger.debug(
-                        "%d/%d Unable to connect to the server."
-                        " Retrying in 1 second ..." % (x, _ODOO_RPC_MAX_TRY)
+                        f"{x}/{_ODOO_RPC_MAX_TRY}"
+                        " Unable to connect to the server."
+                        " Retrying in 1 second ..."
                     )
                     time.sleep(1)
                 else:
                     logger.critical(
-                        "%d/%d Unable to connect to the server."
-                        % (x, _ODOO_RPC_MAX_TRY)
+                        f"{x}/{_ODOO_RPC_MAX_TRY}"
+                        " Unable to connect to the server."
                     )
                     raise e
-
         # Login
         try:
-            rpc_connexion.login(
-                database,
-                "admin",
-                "admin",
-            )
+            rpc_connexion.login(database, "admin", "admin")
         except Exception as e:
             logger.error(
-                "Unable to connect to http://localhost:%s"
-                " with login %s and password %s"
-                % (
-                    port,
-                    "admin",
-                    "admin",
-                )
+                f"Unable to connect to http://localhost:{port}"
+                " with login 'admin' and password 'admin."
             )
             raise e
 
         self.env = rpc_connexion.env
         self.version = rpc_connexion.version
 
     def browse_by_search(
@@ -85,62 +75,49 @@
     def install_modules(self, module_names):
         if type(module_names) is str:
             module_names = [module_names]
         installed_modules = []
         i = 0
         for module_name in module_names:
             i += 1
-            prefix = str(i) + "/" + str(len(module_names))
+            log_prefix = f"{i}/{len(module_names)} - Module '{module_name}': "
             modules = self.browse_by_search(
                 "ir.module.module", [("name", "=", module_name)]
             )
             if not len(modules):
-                logger.error(
-                    "%s - Module '%s': Not found." % (prefix, module_name)
-                )
+                logger.error(f"{log_prefix}': Not found.")
                 continue
 
             module = modules[0]
             if module.state == "installed":
-                logger.info(
-                    "%s - Module %s still installed."
-                    " skipped." % (prefix, module_name)
-                )
+                logger.info(f"{log_prefix}': still installed. Skipped.")
             elif module.state == "uninstalled":
                 try_qty = 0
                 installed = False
                 while installed is False:
                     try_qty += 1
-                    logger.info(
-                        "%s - Module '%s': Installing ... %s"
-                        % (
-                            prefix,
-                            module_name,
-                            "(try #%d)" % try_qty if try_qty != 1 else "",
-                        )
-                    )
+                    try_qty_text = f" (try #{try_qty})" if try_qty != 1 else ""
+                    logger.info(f"{log_prefix}': Installing ...{try_qty_text}")
                     try:
                         module.button_immediate_install()
                         installed = True
                         installed_modules.append(module_name)
                         time.sleep(5)
                     except Exception as e:
                         if try_qty <= 5:
                             sleeping_time = 2 * try_qty * 60
                             logger.warning(
-                                "Error. Retrying in %d seconds.\n %s"
-                                % (sleeping_time, e)
+                                f"Error. Retrying in {sleeping_time} seconds."
+                                f"\n{e}"
                             )
                             time.sleep(sleeping_time)
                         else:
                             logger.critical(
-                                "Error after %d try. Exiting.\n %s"
-                                % (try_qty, e)
+                                f"Error after {try_qty} try. Exiting." f"\n{e}"
                             )
                             raise e
             else:
                 logger.error(
-                    "%s - Module '%s': In the %s state."
+                    f"{log_prefix}': In the {module.state} state."
                     " (Unable to install)"
-                    % (prefix, module_name, module.state)
                 )
         return installed_modules
```

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/tools/tools_odoo_module.py` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/tools/tools_odoo_module.py`

 * *Files 6% similar despite different names*

```diff
@@ -60,16 +60,16 @@
                     ]
                 if len(splited_line) == 3:
                     coverage_analysis[version][splited_line[0]] = (
                         splited_line[1] + " " + splited_line[2]
                     ).strip()
                 elif len(splited_line) > 3:
                     raise ValueError(
-                        "Incorrect value in openupgrade analysis file %s"
-                        " for line %s" % (coverage_path, line)
+                        "Incorrect value in openupgrade analysis"
+                        f" file {coverage_path} for line {line}"
                     )
 
         for odoo_module in filter(
             lambda x: x.module_type == "odoo", self.modules
         ):
             for module_version in list(odoo_module.module_versions.values()):
                 module_version.analyse_openupgrade_state(coverage_analysis)
@@ -107,38 +107,34 @@
     def estimate_workload(self, ctx):
         logger.info("Estimate workload ...")
         for odoo_module in self.modules:
             for module_version in odoo_module.module_versions.values():
                 module_version.estimate_workload(ctx)
 
     def _generate_module_version_first_version(self, ctx, module_list):
-        logger.info(
-            "Analyse version %s. (First version)" % self.initial_version
-        )
+        logger.info(f"Analyse version {self.initial_version}. (First version)")
 
         # Instanciate a new odoo_module
         for module_name in module_list:
             addon_path = OdooModule.get_addon_path(
                 ctx, module_name, self.initial_version
             )
             if addon_path:
                 repository_name = OdooModule.get_repository_name(addon_path)
-                if (
-                    "%s.%s" % (repository_name, module_name)
-                    not in self.modules
-                ):
+                if f"{repository_name}.{module_name}" not in self.modules:
                     logger.debug(
-                        "Discovering module '%s' in %s for version %s"
-                        % (module_name, repository_name, self.initial_version)
+                        f"Discovering module '{module_name}'"
+                        f" in {repository_name}"
+                        f" for version {self.initial_version}"
                     )
             else:
                 repository_name = False
                 logger.error(
-                    "Module %s not found for version %s."
-                    % (module_name, self.initial_version)
+                    f"Module {module_name} not found"
+                    f" for version {self.initial_version}."
                 )
             new_odoo_module = OdooModule(
                 ctx, self, module_name, repository_name
             )
             new_module_version = OdooModuleVersion(
                 self.initial_version, new_odoo_module, addon_path
             )
@@ -147,29 +143,28 @@
             )
             self.modules.append(new_odoo_module)
 
     def _generate_module_version_next_version(
         self, ctx, previous_version, current_version
     ):
         logger.info(
-            "Analyse change between %s and %s"
-            % (previous_version, current_version)
+            f"Analyse change between {previous_version} and {current_version}"
         )
         # Get changes between the two versions
         (
             apriori_module_name,
             apriori_relative_path,
         ) = get_apriori_file_relative_path(current_version)
         apriori_module_path = OdooModule.get_addon_path(
             ctx, apriori_module_name, current_version
         )
         if not apriori_module_path:
             raise ValueError(
-                "Unable to find the path of the module %s for the version %s"
-                % (apriori_module_name, current_version)
+                f"Unable to find the path of the module {apriori_module_name}"
+                f" for the version {current_version}."
             )
         apriori_absolute_path = (
             apriori_module_path
             / Path(apriori_module_name)
             / apriori_relative_path
         )
 
@@ -185,62 +180,49 @@
         for odoo_module in self.modules:
             state = False
             new_module_name = False
             if odoo_module.name in renamed_modules:
                 state = "renamed"
                 new_module_name = renamed_modules[odoo_module.name]
                 logger.debug(
-                    "%s -> %s : %s renamed into %s"
-                    % (
-                        previous_version,
-                        current_version,
-                        odoo_module.name,
-                        new_module_name,
-                    )
+                    f"{previous_version} -> {current_version} :"
+                    f" {odoo_module.name} renamed into {new_module_name}"
                 )
             elif odoo_module.name in merged_modules:
                 state = "merged"
                 new_module_name = merged_modules[odoo_module.name]
                 logger.debug(
-                    "%s -> %s : %s merged into %s"
-                    % (
-                        previous_version,
-                        current_version,
-                        odoo_module.name,
-                        new_module_name,
-                    )
+                    f"{previous_version} -> {current_version} :"
+                    f" {odoo_module.name} merged into {new_module_name}"
                 )
 
             # Handle new module
             if state and new_module_name != odoo_module.name:
                 # Ensure that the module exists in self.modules
                 new_addon_path = OdooModule.get_addon_path(
                     ctx, new_module_name, current_version
                 )
                 if not new_addon_path:
                     raise ValueError(
-                        "The module %s has not been found in the version %s."
+                        f"The module {new_module_name} has not been found"
+                        f" in the version {current_version}."
                         " Analyse can not be done."
-                        % (new_module_name, current_version)
                     )
                 else:
                     new_repository_name = OdooModule.get_repository_name(
                         new_addon_path
                     )
                     if (
                         "%s.%s" % (new_repository_name, new_module_name)
                         not in self.modules
                     ):
                         logger.debug(
-                            "Discovering module '%s' in %s for version %s"
-                            % (
-                                new_module_name,
-                                new_repository_name,
-                                current_version,
-                            )
+                            f"Discovering module '{new_module_name}'"
+                            f" in {new_repository_name}"
+                            f" for version {current_version}"
                         )
                         new_odoo_module = OdooModule(
                             ctx, self, new_module_name, new_repository_name
                         )
                         self.modules.append(new_odoo_module)
                         new_odoo_module.module_versions.update(
                             {
@@ -312,15 +294,15 @@
 
 @total_ordering
 class OdooModule(object):
     def __init__(self, ctx, analyse, module_name, repository_name):
         self.analyse = analyse
         self.name = module_name
         self.repository = repository_name
-        self.unique_name = "%s.%s" % (repository_name, module_name)
+        self.unique_name = f"{repository_name}.{module_name}"
         self.ignored = self.is_ignored(ctx, module_name)
         self.module_versions = {}
         if not repository_name:
             self.module_type = "not_found"
         elif repository_name == "odoo/odoo":
             self.module_type = "odoo"
         elif repository_name.startswith("oca"):
@@ -341,30 +323,30 @@
         return module_name in settings["ignored_module_list"]
 
     def get_module_version(self, current_version):
         res = self.module_versions.get(current_version, False)
         return res
 
     def get_odoo_apps_url(self):
-        logger.info("Searching %s in the Odoo appstore ..." % self.name)
+        logger.info(f"Searching {self.name} in the Odoo appstore ...")
         url = (
             f"https://apps.odoo.com/apps/modules/"
             f"{self.analyse.initial_version}/{self.name}/"
         )
         try:
             response = requests.get(url)
         except requests.exceptions.RequestException as err:
             logger.warning(f"Error when trying to get {url}: {err}")
             return False
         if response.status_code == 200:
             return url
         return False
 
     def get_odoo_code_search_url(self):
-        logger.info("Searching %s in Odoo-Code-Search ..." % self.name)
+        logger.info(f"Searching {self.name} in Odoo-Code-Search ...")
         url = (
             f"https://odoo-code-search.com/ocs/search?"
             f"q=name%3A%3D{self.name}+version%3A{self.analyse.initial_version}"
         )
         result = requests.get(url)
         if '<td class="code">404</td>' in result.text:
             return False
@@ -670,15 +652,15 @@
                     continue
                 elif line.startswith("---XML records in module"):
                     line_type = "xml"
                     continue
                 elif line.startswith("---nothing has changed in this module"):
                     continue
                 elif line.startswith("---"):
-                    raise Exception("comment %s not undestood" % line)
+                    raise Exception(f"comment {line} not understood")
 
                 if line_type == "model":
                     self.openupgrade_model_lines += 1
                 elif line_type == "field":
                     self.openupgrade_field_lines += 1
                 elif line_type == "xml":
                     self.openupgrade_xml_lines += 1
@@ -770,17 +752,17 @@
             ):
                 if self.openupgrade_state:
                     return self.openupgrade_state
                 else:
                     return "To analyse"
         else:
             if self.state == "merged":
-                return "Merged into %s" % self.target_module
+                return f"Merged into {self.target_module}"
             elif self.state == "renamed":
-                return "Renamed into %s" % self.target_module
+                return f"Renamed into {self.target_module}"
             elif self.state == "ignored":
                 return "Ignored"
             elif self.state == "normal_loss":
                 return ""
 
             if self.odoo_module.module_type == "odoo":
                 # A core module disappeared and has not been merged
@@ -789,8 +771,8 @@
             else:
                 last_existing_version = self.get_last_existing_version()
                 if not last_existing_version:
                     return "Unknown"
                 elif self.version != self.odoo_module.analyse.final_version:
                     return "Unported"
                 else:
-                    return "To port from %s" % last_existing_version.version
+                    return f"To port from {last_existing_version.version}"
```

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/tools/tools_postgres.py` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/tools/tools_postgres.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import shlex
 import time
 from pathlib import Path
 
 import docker
 from loguru import logger
 
 from odoo_openupgrade_wizard.tools.tools_docker import (
@@ -25,37 +26,37 @@
         filters={"name": container_name},
         ignore_removed=True,
     )
     if containers:
         container = containers[0]
         if container.status == "exited":
             logger.warning(
-                "Found container %s in a exited status. Removing it..."
-                % container_name
+                f"Found container {container_name} in a exited status."
+                " Removing it..."
             )
             container.remove()
         else:
             return container
 
     # Check if volume exists
     try:
         client.volumes.get(volume_name)
-        logger.debug("Recovering existing postgres volume: %s" % volume_name)
+        logger.debug(f"Recovering existing postgres volume: {volume_name}")
     except docker.errors.NotFound:
-        logger.info("Creating Postgres volume: %s" % volume_name)
+        logger.info(f"Creating Postgres volume: {volume_name}")
         client.volumes.create(volume_name)
 
     command = None
     postgres_extra_settings = ctx.obj["config"].get("postgres_extra_settings")
     if postgres_extra_settings:
         command = "postgres"
         for key, value in postgres_extra_settings.items():
             command += f" -c {key}={value}"
 
-    logger.info("Launching Postgres Container. (Image %s)" % image_name)
+    logger.info(f"Launching Postgres Container. (Image {image_name})")
     container = run_container(
         image_name,
         container_name,
         command=command,
         environments={
             "POSTGRES_USER": "odoo",
             "POSTGRES_PASSWORD": "odoo",
@@ -81,30 +82,29 @@
 def execute_sql_file(ctx, database, sql_file):
     container = get_postgres_container(ctx)
 
     # Recreate relative path to make posible to
     # call psql in the container
     if str(ctx.obj["env_folder_path"]) not in str(sql_file):
         raise Exception(
-            "The SQL file %s is not in the"
-            " main folder %s available"
+            f"The SQL file {sql_file} is not in the"
+            f" main folder {ctx.obj['env_folder_path']} available"
             " in the postgres container."
-            % (sql_file, ctx.obj["env_folder_path"])
         )
     relative_path = Path(
         str(sql_file).replace(str(ctx.obj["env_folder_path"]), ".")
     )
 
     container_path = Path("/env/") / relative_path
     command = (
         "psql --username=odoo --dbname={database} --file {file_path}"
     ).format(database=database, file_path=container_path)
     logger.info(
-        "Executing the script '%s' in postgres container"
-        " on database %s" % (relative_path, database)
+        f"Executing the script '{relative_path}' in postgres container"
+        f" on database {database}"
     )
     exec_container(container, command)
 
 
 def execute_sql_request(ctx, request, database="postgres"):
     psql_args = ("--tuples-only",)
     output = execute_psql_command(ctx, request, database, psql_args)
@@ -122,52 +122,56 @@
 ):
     """Execute psql request in postgres container with psql_args on database"""
     container = get_postgres_container(ctx)
     command = (
         "psql"
         " --username=odoo"
         f" --dbname={database or 'postgres'}"
-        f' --command "{request}"'
+        f" --command {shlex.quote(request)}"
         f" {' '.join(psql_args)}"
     )
     logger.debug(
-        "Executing the following command in postgres container\n"
-        "%s" % (command)
+        f"Executing the following command in postgres container\n{command}"
     )
     docker_result = exec_container(container, command)
     return docker_result.output.decode("utf-8")
 
 
-def ensure_database(ctx, database: str, state="present"):
+def ensure_database(ctx, database: str, state="present", template: str = ""):
     """
     - Connect to postgres container.
     - Check if the database exist.
     - if doesn't exists and state == 'present', create it.
     - if exists and state == 'absent', drop it.
     """
     request = "select datname FROM pg_database WHERE datistemplate = false;"
 
     result = execute_sql_request(ctx, request)
 
     if state == "present":
         if [database] in result:
             return
 
-        logger.info("Create database '%s' ..." % database)
-        request = "CREATE DATABASE {database} owner odoo;".format(
-            database=database
-        )
-        execute_sql_request(ctx, request)
+        if template:
+            logger.info(f'Copy database "{template}" into "{database}"...')
+            request = (
+                f'CREATE DATABASE "{database}" WITH TEMPLATE "{template}";'
+            )
+        else:
+            logger.info(f"Create database '{database}'...")
+            request = f'CREATE DATABASE "{database}" OWNER odoo;'
+        execute_psql_command(ctx, request)
+
     else:
         if [database] not in result:
             return
 
-        logger.info("Drop database '%s' ..." % database)
-        request = "DROP DATABASE {database};".format(database=database)
-        execute_sql_request(ctx, request)
+        logger.info(f'Drop database "{database}"...')
+        request = f'DROP DATABASE "{database}";'
+        execute_psql_command(ctx, request)
 
 
 def execute_sql_files_pre_migration(
     ctx, database: str, migration_step: dict, sql_files: list = []
 ):
     ensure_database(ctx, database, state="present")
     if not sql_files:
@@ -188,16 +192,15 @@
     """Chown a filepath in the postgres container to the local user"""
     container = get_postgres_container(ctx)
     user_uid = os.getuid()
     command = "chown -R {uid}:{uid} {filepath}".format(
         uid=user_uid, filepath=filepath
     )
     logger.debug(
-        "Executing the following command in postgres container: %s"
-        % (command,)
+        f"Executing the following command in postgres container:\n{command}"
     )
     chown_result = exec_container(container, command)
     return chown_result.output.decode("utf8")
 
 
 def execute_pg_dump(
     ctx,
@@ -225,16 +228,15 @@
     ).format(
         dumpformat=dumpformat,
         filepath=filepath,
         database=database,
         pg_dump_args=pg_dump_args,
     )
     logger.debug(
-        "Executing the following command in postgres container: %s"
-        % (command,)
+        f"Executing the following command in postgres container:\n{command}"
     )
     pg_dump_result = exec_container(container, command)
 
     chown_to_local_user(ctx, filepath)
     return pg_dump_result.output.decode("utf8")
```

### Comparing `odoo_openupgrade_wizard-0.6.0/odoo_openupgrade_wizard/tools/tools_system.py` & `odoo_openupgrade_wizard-0.7.0/odoo_openupgrade_wizard/tools/tools_system.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 
 def get_script_folder(ctx, migration_step: dict) -> Path:
     return ctx.obj["script_folder_path"] / migration_step["complete_name"]
 
 
 def ensure_folder_writable(folder_path: Path):
-    logger.info("Make writable the folder '%s'" % folder_path)
+    logger.info(f"Make writable the folder '{folder_path}'")
     try:
         chmod(["--silent", "--recursive", "o+w", str(folder_path)])
     except ProcessExecutionError:
         pass
 
 
 def ensure_folder_exists(
@@ -33,15 +33,15 @@
     - directory is created if it doesn't exist.
     - mode is applied if defined.
     - a log is done at INFO level.
     """
     if not folder_path.exists():
         cmd = ["--parents", folder_path]
         cmd = ["--mode", mode] + cmd
-        logger.info("Creating folder '%s' ..." % (folder_path))
+        logger.info(f"Creating folder '{folder_path}' ...")
         mkdir(cmd)
 
     if git_ignore_content:
         ensure_file_exists_from_template(
             folder_path / Path(".gitignore"),
             ".gitignore.j2",
         )
@@ -70,17 +70,17 @@
         # Check if content is different
         with open(file_path, "r") as file:
             data = file.read()
             file.close()
             if data == output:
                 return
 
-        log_text = "Updating file '%s' from template ..." % (file_path)
+        log_text = f"Updating file '{file_path}' from template ..."
     else:
-        log_text = "Creating file '%s' from template ..." % (file_path)
+        log_text = f"Creating file '{file_path}' from template ..."
 
     with open(file_path, "w") as f:
         logger.info(log_text)
         print(output, file=f)
 
 
 def git_aggregate(folder_path: Path, config_path: Path, jobs: int):
@@ -93,26 +93,26 @@
         expand_env=False,
         env_file=None,
         force=True,
     )
     with working_directory_keeper:
         os.chdir(folder_path)
         logger.info(
-            "Gitaggregate source code for %s. This can take a while ..."
-            % config_path
+            f"Gitaggregate source code for {config_path}."
+            " This can take a while ..."
         )
         gitaggregate_cmd.run(args)
 
 
 def get_local_user_id():
     return os.getuid()
 
 
 def execute_check_output(args_list, working_directory=False):
-    logger.debug("Execute %s" % " ".join(args_list))
+    logger.debug(f"Execute {' '.join(args_list)}")
     subprocess.check_output(args_list, cwd=working_directory)
 
 
 def dump_filestore(
     ctx,
     database: str,
     destpath: os.PathLike,
```

### Comparing `odoo_openupgrade_wizard-0.6.0/pyproject.toml` & `odoo_openupgrade_wizard-0.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "odoo-openupgrade-wizard"
-version = "0.6.0"
+version = "0.7.0"
 description = "CLI tool to manage Odoo Major Upgrades"
 authors = [
     "GRAP, Groupement Régional Alimentaire de Proximité",
 ]
 maintainers = [
     "Sylvain LE GAL",
 ]
@@ -24,27 +24,27 @@
 ]
 
 [tool.poetry.scripts]
 oow = "odoo_openupgrade_wizard.cli.cli:main"
 odoo-openupgrade-wizard = "odoo_openupgrade_wizard.cli.cli:main"
 
 [tool.poetry.dependencies]
-python = ">=3.6.3,<4.0.0"
+python = ">=3.9,<4.0.0"
 click = "^7.0"
 click-loglevel = "^0.4"
-docker = "^5.0"
+docker = "^7.0"
 importlib-resources = "^5.4"
 git-aggregator = "^2.1"
 GitPython = "^3.1"
 jinja2 = "^3.0"
 loguru = "^0.6"
-odoorpc = "^0.8"
+odoorpc = "^0.10.1"
 plumbum = "^1.7"
 pygount = "^1.4"
-pyyaml = "5.4.1"
+pyyaml = "^6.0.0"
 single-source = "^0.3"
 
 [tool.poetry.group.dev.dependencies]
 pytest = [
     {version = "<=6.1.2", python = "<3.10"},
     {version = ">=6.2.5", python = ">=3.10"}
 ]
```

### Comparing `odoo_openupgrade_wizard-0.6.0/PKG-INFO` & `odoo_openupgrade_wizard-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: odoo-openupgrade-wizard
-Version: 0.6.0
+Version: 0.7.0
 Summary: CLI tool to manage Odoo Major Upgrades
 Home-page: https://gitlab.com/odoo-openupgrade-wizard/odoo-openupgrade-wizard
 License: AGPLv3+
 Keywords: cli,odoo,openupgrade
 Author: GRAP, Groupement Régional Alimentaire de Proximité
 Maintainer: Sylvain LE GAL
-Requires-Python: >=3.6.3,<4.0.0
+Requires-Python: >=3.9,<4.0.0
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Odoo
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: GitPython (>=3.1,<4.0)
 Requires-Dist: click (>=7.0,<8.0)
 Requires-Dist: click-loglevel (>=0.4,<0.5)
-Requires-Dist: docker (>=5.0,<6.0)
+Requires-Dist: docker (>=7.0,<8.0)
 Requires-Dist: git-aggregator (>=2.1,<3.0)
 Requires-Dist: importlib-resources (>=5.4,<6.0)
 Requires-Dist: jinja2 (>=3.0,<4.0)
 Requires-Dist: loguru (>=0.6,<0.7)
-Requires-Dist: odoorpc (>=0.8,<0.9)
+Requires-Dist: odoorpc (>=0.10.1,<0.11.0)
 Requires-Dist: plumbum (>=1.7,<2.0)
 Requires-Dist: pygount (>=1.4,<2.0)
-Requires-Dist: pyyaml (==5.4.1)
+Requires-Dist: pyyaml (>=6.0.0,<7.0.0)
 Requires-Dist: single-source (>=0.3,<0.4)
 Project-URL: Repository, https://gitlab.com/odoo-openupgrade-wizard/odoo-openupgrade-wizard
 Description-Content-Type: text/markdown
 
 [![Gitlab CI](https://gitlab.com/odoo-openupgrade-wizard/odoo-openupgrade-wizard/badges/main/pipeline.svg)](https://gitlab.com/odoo-openupgrade-wizard/odoo-openupgrade-wizard/-/pipelines)
 [![codecov](https://gitlab.com/odoo-openupgrade-wizard/odoo-openupgrade-wizard/badges/main/coverage.svg)](https://gitlab.com/odoo-openupgrade-wizard/odoo-openupgrade-wizard/)
 [![License: AGPL v3](https://img.shields.io/badge/License-AGPL_v3-blue.svg)](https://www.gnu.org/licenses/agpl-3.0)
```

