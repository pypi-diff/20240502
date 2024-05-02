# Comparing `tmp/cloudzero_uca_tools-0.7.8.tar.gz` & `tmp/cloudzero_uca_tools-0.7.9.tar.gz`

## Comparing `cloudzero_uca_tools-0.7.8.tar` & `cloudzero_uca_tools-0.7.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/__init__.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/__version__.py
--rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/constants.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/exceptions.py
--rwxr-xr-x   0        0        0    11510 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/main.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/commands/__init__.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/commands/convert.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/common/__init__.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/common/aws.py
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/common/cli.py
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/common/custom_types.py
--rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/common/files.py
--rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/common/formatters.py
--rw-r--r--   0        0        0     1600 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/common/standards.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/data/alb_configuration.json
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/data/configuration.json
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/data/csv_configuration.json
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/data/data.csv
--rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/data/example_alb_logs
--rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/data/sample_uca_data.json
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/data/test_configuration.json
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/data/test_data.csv
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/data/transform.jq
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/features/__init__.py
--rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/features/convert.py
--rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/features/generate.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/features/transform.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/features/transmit.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/interfaces/__init__.py
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/interfaces/uca_api.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/vendored/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/__init__.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/exceptions.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/interface.py
--rw-r--r--   0        0        0     5354 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/models.py
--rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/parser.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/util.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/aws/__init__.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/aws/client.py
--rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/aws/plugin.py
--rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/aws/s3.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/cli/__init__.py
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/cli/main.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/.gitignore
--rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/LICENSE
--rw-r--r--   0        0        0    14691 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/README.md
--rw-r--r--   0        0        0     2603 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/pyproject.toml
--rw-r--r--   0        0        0    15827 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.8/PKG-INFO
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/__init__.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/__version__.py
+-rw-r--r--   0        0        0     1373 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/constants.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/exceptions.py
+-rwxr-xr-x   0        0        0    10735 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/main.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/commands/__init__.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/commands/convert.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/common/__init__.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/common/aws.py
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/common/cli.py
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/common/custom_types.py
+-rw-r--r--   0        0        0     4979 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/common/files.py
+-rw-r--r--   0        0        0     2907 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/common/formatters.py
+-rw-r--r--   0        0        0     4126 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/common/standards.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/data/alb_configuration.json
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/data/configuration.json
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/data/csv_configuration.json
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/data/data.csv
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/data/example_alb_logs
+-rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/data/sample_uca_data.json
+-rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/data/test_configuration.json
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/data/test_data.csv
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/data/transform.jq
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/features/__init__.py
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/features/convert.py
+-rw-r--r--   0        0        0     6576 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/features/generate.py
+-rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/features/transform.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/features/transmit.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/interfaces/__init__.py
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/interfaces/uca_api.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/vendored/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/vendored/aws_log_parser/__init__.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/vendored/aws_log_parser/exceptions.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/vendored/aws_log_parser/interface.py
+-rw-r--r--   0        0        0     5354 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/vendored/aws_log_parser/models.py
+-rw-r--r--   0        0        0     2231 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/vendored/aws_log_parser/parser.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/vendored/aws_log_parser/util.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/vendored/aws_log_parser/aws/__init__.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/vendored/aws_log_parser/aws/client.py
+-rw-r--r--   0        0        0      701 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/vendored/aws_log_parser/aws/plugin.py
+-rw-r--r--   0        0        0     1384 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/vendored/aws_log_parser/aws/s3.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/vendored/aws_log_parser/cli/__init__.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/uca/vendored/aws_log_parser/cli/main.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/.gitignore
+-rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/LICENSE
+-rw-r--r--   0        0        0    14691 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/README.md
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/pyproject.toml
+-rw-r--r--   0        0        0    15827 2020-02-02 00:00:00.000000 cloudzero_uca_tools-0.7.9/PKG-INFO
```

### Comparing `cloudzero_uca_tools-0.7.8/uca/constants.py` & `cloudzero_uca_tools-0.7.9/uca/constants.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.8/uca/main.py` & `cloudzero_uca_tools-0.7.9/uca/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,19 @@
 import click
 import simplejson as json
 
 from uca.__version__ import __version__
 from uca.common.cli import eprint, print_uca_sample
 from uca.common.custom_types import TimeRange
 from uca.common.files import load_data_files, write_to_file
-from uca.common.standards import utc_datetime_from_anything
+from uca.common.standards import (
+    utc_datetime_from_anything,
+    valid_settings,
+    valid_template,
+)
 from uca.constants import FILE_FORMATS, DEFAULT_FILE_FORMAT
 from uca.exceptions import InvalidDate
 from uca.features.convert import convert
 from uca.features.generate import generate_uca
 from uca.features.transform import transform_data, load_transform_script
 from uca.features.transmit import transmit
 
@@ -108,25 +112,24 @@
 @click.option(
     "--today", is_flag=True, required=False, help="Generate events for the current day"
 )
 @click.option("--input", "-i", required=True, help="Input UCA data (CSV)")
 @click.option("--output", "-o", required=True, help="Output file")
 @pass_root_configuration
 def generate_uca_command(configuration, start, end, today, input, output):
-    if not configuration.settings:
+
+    if not configuration.settings or not configuration.template:
         eprint("Please specify a --configuration file")
         sys.exit()
 
     output = os.path.abspath(output)
     configuration.output_path = output
     configuration.destination = "File"
 
-    configuration.template.pop("metric-name", None)
-    configuration.template.pop("telemetry-stream", None)
-
+    # Process Date Range Inputs
     if today:
         today = datetime.today().replace(hour=0, minute=0, second=0, microsecond=0)
         range_requested = TimeRange(start=today, end=today + timedelta(days=1))
 
     elif all([start, end]):
         try:
             start_date = utc_datetime_from_anything(start)
@@ -139,73 +142,75 @@
             print(f"Invalid end date: {error}")
             sys.exit(-1)
         range_requested = TimeRange(start=start_date, end=end_date)
 
     else:
         range_requested = None
 
-    try:
-        generate_settings = configuration.settings["generate"]
-
-        if not isinstance(generate_settings, dict):
-            raise TypeError("generate_settings must be a dictionary")
-
-        required_generate_keys = ["mode"]
-        missing_keys = [
-            key for key in required_generate_keys if key not in generate_settings
-        ]
-        if missing_keys:
-            raise ValueError(
-                f"Missing required key(s) in 'generate' config: {', '.join(missing_keys)}"
-            )
-
-        print("CloudZero UCA Data Generator")
-        print("-" * 140)
-        print(f"   Date Range : {range_requested or 'data driven'}")
-
-        if "metric-name" not in configuration.template:
-            print(f"  Granularity : {configuration.template['granularity']}")
-
-        print(f"         Mode : {generate_settings['mode']}")
+    stream_type = configuration.settings.get("stream_type", None)
+    if stream_type not in ["allocation", "metric"]:
+        print(f"Invalid 'stream_type' in Settings: {stream_type}")
+        sys.exit(-1)
 
-        if generate_settings["mode"] == "jitter":
-            print(f"       Jitter : {generate_settings['jitter']}")
+    try:
+        if not valid_settings(configuration.settings):
+            sys.exit(-1)
 
-        elif generate_settings["mode"] == "allocation":
-            print(f"   Allocation : {generate_settings['allocation']}")
+        if not valid_template(configuration.template, stream_type):
+            sys.exit(-1)
 
-            if generate_settings.get("jitter"):
-                print(f"              : with Jitter {generate_settings['jitter']}")
+    except Exception as err:
+        print(err)
+        sys.exit(-1)
 
-        if generate_settings.get("precision"):
-            print(f"    Precision : {generate_settings['precision']}")
+    print("CloudZero UCA Data Generator")
+    print("-" * 140)
+    print(f"   Date Range : {range_requested or 'data driven'}")
 
-        print(f"Configuration : {configuration.configuration_path}")
-        print(f"   Input Data : {input}")
-        print(f"  Output File : {configuration.output_path}")
-        print("-" * 140)
+    generate_settings = configuration.settings["generate"]
 
-    except KeyError as error:
-        eprint(f"Missing configurations: {error}")
-        sys.exit(-1)
-    except TypeError:
-        eprint("'Generate' configuration must be a dictionary.")
-        sys.exit(-1)
-    except ValueError as error:
-        eprint(error)
-        sys.exit(-1)
+    mode = generate_settings.get("mode")
+    granularity = configuration.template.get("granularity")
+    stream_type = configuration.settings.get("stream_type")
+    jitter = generate_settings.get("jitter")
+    allocation = generate_settings.get("allocation")
+    precision = generate_settings.get("precision")
+
+    if stream_type == "allocation" and granularity:
+        print(f"  Granularity : {granularity}")
+
+    print(f"         Mode : {mode}")
+
+    if mode == "allocation":
+        print(f"   Allocation : {allocation}")
+        if jitter:
+            print(f"       Jitter : {jitter}")
+    elif mode == "jitter":
+        print(f"       Jitter : {jitter}")
+
+    if precision:
+        print(f"    Precision : {precision}")
+
+    print(f"Configuration : {configuration.configuration_path}")
+    print(f"   Input Data : {input}")
+    print(f"  Output File : {configuration.output_path}")
+    print("-" * 140)
 
     try:
         uca_data = load_data_files(input, "CSV")
+
     except Exception as error:
         eprint(f"Unable to read input file {input}, error: {error}")
         sys.exit(-1)
 
     uca_to_send = generate_uca(
-        range_requested, configuration.template, generate_settings, uca_data
+        range_requested,
+        configuration.template,
+        configuration.settings,
+        uca_data
     )
     if not uca_to_send:
         print(f" - Event Generation failed, {len(uca_to_send)} events created")
         sys.exit(-1)
 
     print(f" - Event Generation complete, {len(uca_to_send)} events created")
 
@@ -237,44 +242,35 @@
 )
 @pass_root_configuration
 def transmit_uca_command(configuration, data, output, transform):
     if output:
         configuration.output_path = output
         configuration.destination = "File"
 
-    if "telemetry-stream" in configuration.template:
-        stream_name = configuration.template["telemetry-stream"].lower()
-        stream_type = "allocation"
-
-    elif "metric-name" in configuration.template:
-        stream_name = configuration.template["metric-name"].lower()
-        stream_type = "metric"
+    try:
+        if not valid_settings(configuration.settings):
+            sys.exit(-1)
 
-    else:
-        print("Missing 'telemetry-stream' or 'metric-name' key in 'template' config")
+    except Exception as err:
+        print(err)
         sys.exit(-1)
 
+    stream_name = configuration.settings.get("stream_name")
+    stream_type = configuration.settings.get("stream_type")
+
     print(f"Transmitting UCA data from {data} to {configuration.destination}")
     print("-" * 140)
 
     records = load_data_files(data, file_format="JSON")
     transform_script = load_transform_script(transform)
     uca_to_send, transformed_records, filtered_records = transform_data(
         records, transform_script
     )
 
-    if "transmit_type" not in configuration.settings:
-        print("Missing 'transmit_type' key in 'settings' config")
-        sys.exit(-1)
-
-    transmit_type = configuration.settings["transmit_type"].lower()
-    if transmit_type not in ["sum", "replace", "delete", "update"]:
-        print(f"Invalid value, '{transmit_type}', for 'transmit_type' key in 'settings' config")
-        print("Valid values: 'sum', 'replace', 'delete'")
-        sys.exit(-1)
+    transmit_type = configuration.settings.get("transmit_type", "replace")
 
     if transmit_type == "delete":
         for record in uca_to_send:
             try:
                 del record["value"]
 
             except KeyError:
```

### Comparing `cloudzero_uca_tools-0.7.8/uca/commands/convert.py` & `cloudzero_uca_tools-0.7.9/uca/commands/convert.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.8/uca/common/aws.py` & `cloudzero_uca_tools-0.7.9/uca/common/aws.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.8/uca/common/cli.py` & `cloudzero_uca_tools-0.7.9/uca/common/cli.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.8/uca/common/custom_types.py` & `cloudzero_uca_tools-0.7.9/uca/common/custom_types.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.8/uca/common/files.py` & `cloudzero_uca_tools-0.7.9/uca/common/files.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.8/uca/common/formatters.py` & `cloudzero_uca_tools-0.7.9/uca/common/formatters.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.8/uca/data/alb_configuration.json` & `cloudzero_uca_tools-0.7.9/uca/data/alb_configuration.json`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.8/uca/data/example_alb_logs` & `cloudzero_uca_tools-0.7.9/uca/data/example_alb_logs`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.8/uca/data/sample_uca_data.json` & `cloudzero_uca_tools-0.7.9/uca/data/sample_uca_data.json`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.8/uca/features/convert.py` & `cloudzero_uca_tools-0.7.9/uca/features/convert.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.8/uca/features/generate.py` & `cloudzero_uca_tools-0.7.9/uca/features/generate.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,21 +12,21 @@
 
 import simplejson as json
 
 from uca.common.cli import eprint
 from uca.common.custom_types import TimeRange
 from uca.common.standards import datetime_chunks, utc_datetime_from_anything
 
-PRECISION = 10000
+PRECISION = 4
 
 
 def generate_uca(time_range: TimeRange, uca_template, settings, uca_data):
     expand_month = False
 
-    if "metric-name" in uca_template:
+    if settings.get("stream_type") == "metric":
         delta = timedelta(days=1)
 
     else:
         if uca_template['granularity'] == "HOURLY":
             delta = timedelta(hours=1)
         elif uca_template['granularity'] == "DAILY":
             delta = timedelta(days=1)
@@ -65,46 +65,51 @@
             uca_events = _render_uca_data(uca_data, settings, uca_template)
 
     return uca_events
 
 
 def _render_uca_data(uca_data, settings, uca_template, timestamp=None):
 
+    generate_settings = settings.get("generate")
     unit_value_header = uca_template['value'].replace('$', '')
     timestamp_header = uca_template['timestamp'].replace('$', '')
 
-    if settings.get("precision"):
-        precision = int("1" + "0" * settings.get("precision"))
+    try:
+        precision = int("1" + "0" * int(settings.get("precision", PRECISION)))
 
-    else:
-        precision = PRECISION
+    except TypeError:
+        print("precision is Settings must be an integer")
+        sys.exit(-1)
+    except ValueError:
+        print("precision is Settings must be an integer")
+        sys.exit(-1)
 
     uca_events = []
     # skipped = 0
     for row in uca_data:
         try:
             if not row[unit_value_header] or Decimal(row[unit_value_header]) <= 0:
                 continue
         except Exception as err:
             print(f"Error: {err}")
             print(f"{row[unit_value_header]}")
             sys.exit(-1)
 
-        if settings['mode'] == 'random':
+        if generate_settings.get('mode') == 'random':
             unit_value = preserve_precision(row[unit_value_header], precision)
             row[unit_value_header] = str(restore_precision(randint(0, unit_value), precision))
-        elif settings['mode'] == 'jitter':
-            jitter = int(settings['jitter'])
+        elif generate_settings.get('mode') == 'jitter':
+            jitter = int(generate_settings.get('jitter'))
             row[unit_value_header] = str(
                 round_decimal(max(Decimal(abs(Decimal(row[unit_value_header]) + randint(-jitter, jitter))), Decimal(1)),
                               precision))
-        elif settings['mode'] == 'allocation':
+        elif generate_settings.get('mode') == 'allocation':
             jitter = None
-            if settings.get('jitter'):
-                jitter = int(settings.get('jitter'))
+            if generate_settings.get('jitter'):
+                jitter = int(generate_settings.get('jitter'))
             try:
                 if jitter:
                     row[unit_value_header] = round_decimal((Decimal(settings['allocation']) *
                                                             Decimal(row['unit_allocation'])) + randint(0, jitter),
                                                            precision)
                 else:
                     row[unit_value_header] = round_decimal(
@@ -113,19 +118,19 @@
             except KeyError:
                 print('ERROR: Must add "unit_allocation" column to CSV')
                 sys.exit(-1)
             except Exception as error:
                 print(f'ERROR: {error}')
                 sys.exit(-1)
 
-        elif settings['mode'] == 'exact':
+        elif generate_settings.get('mode') == 'exact':
             row[unit_value_header] = str(round_decimal(Decimal(row[unit_value_header]), precision))
         else:
             eprint(
-                f"Unsupported UCA Mode '{settings['mode']}', please choose either 'exact', 'random', 'jitter' or 'allocation'")
+                f"Unsupported UCA Mode '{generate_settings.get('mode')}', please choose either 'exact', 'random', 'jitter' or 'allocation'")
             sys.exit(-1)
 
         try:
             template = Template(json.dumps(uca_template))
             if timestamp:
                 rendered_template = template.substitute({**row, timestamp_header: timestamp})
```

### Comparing `cloudzero_uca_tools-0.7.8/uca/features/transform.py` & `cloudzero_uca_tools-0.7.9/uca/features/transform.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.8/uca/features/transmit.py` & `cloudzero_uca_tools-0.7.9/uca/features/transmit.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.8/uca/interfaces/uca_api.py` & `cloudzero_uca_tools-0.7.9/uca/interfaces/uca_api.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/interface.py` & `cloudzero_uca_tools-0.7.9/uca/vendored/aws_log_parser/interface.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/models.py` & `cloudzero_uca_tools-0.7.9/uca/vendored/aws_log_parser/models.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/parser.py` & `cloudzero_uca_tools-0.7.9/uca/vendored/aws_log_parser/parser.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/aws/client.py` & `cloudzero_uca_tools-0.7.9/uca/vendored/aws_log_parser/aws/client.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/aws/plugin.py` & `cloudzero_uca_tools-0.7.9/uca/vendored/aws_log_parser/aws/plugin.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/aws/s3.py` & `cloudzero_uca_tools-0.7.9/uca/vendored/aws_log_parser/aws/s3.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.8/uca/vendored/aws_log_parser/cli/main.py` & `cloudzero_uca_tools-0.7.9/uca/vendored/aws_log_parser/cli/main.py`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.8/.gitignore` & `cloudzero_uca_tools-0.7.9/.gitignore`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.8/LICENSE` & `cloudzero_uca_tools-0.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.8/README.md` & `cloudzero_uca_tools-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `cloudzero_uca_tools-0.7.8/pyproject.toml` & `cloudzero_uca_tools-0.7.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -49,19 +49,14 @@
 
 [project.scripts]
 uca = "uca.main:cli"
 
 [project.urls]
 Homepage = "https://github.com/Cloudzero/cloudzero-uca-tools"
 
-[tool]
-rye = { dev-dependencies = [
-    "hatch>=1.9.4",
-] }
-
 [tool.hatch.version]
 path = "uca/__version__.py"
 
 [tool.hatch.build.targets.wheel]
 packages = ["uca"]
 [tool.hatch.build.targets.sdist]
 include = [
@@ -124,8 +119,8 @@
 [tool.hatch.envs.lint]
 detached = true
 dependencies = [
     "ruff>=0.0.243"
 ]
 [tool.hatch.envs.lint.scripts]
 fix = "ruff . --fix"
-check = "ruff ."
+check = "ruff ."
```

### Comparing `cloudzero_uca_tools-0.7.8/PKG-INFO` & `cloudzero_uca_tools-0.7.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudzero-uca-tools
-Version: 0.7.8
+Version: 0.7.9
 Summary: CloudZero UCA Toolkit
 Project-URL: Homepage, https://github.com/Cloudzero/cloudzero-uca-tools
 Author-email: CloudZero <support@cloudzero.com>
 License: Apache-2.0
 License-File: LICENSE
 Keywords: CloudZero,Toolkit,UCA,analysis,cost,economics,unit
 Classifier: Development Status :: 4 - Beta
```

