# Comparing `tmp/tantri-1.0.1.tar.gz` & `tmp/tantri-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tantri-1.0.1.tar", max compression
+gzip compressed data, was "tantri-1.1.0.tar", max compression
```

## Comparing `tantri-1.0.1.tar` & `tantri-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,31 @@
--rwxr-xr-x   0        0        0      333 2024-04-22 20:18:56.172965 tantri-1.0.1/README.md
--rwxr-xr-x   0        0        0     1033 2024-04-22 20:18:56.176965 tantri-1.0.1/pyproject.toml
--rwxr-xr-x   0        0        0      295 2024-04-22 20:18:56.176965 tantri-1.0.1/tantri/__init__.py
--rwxr-xr-x   0        0        0     5467 2024-04-22 20:18:56.176965 tantri-1.0.1/tantri/cli/__init__.py
--rw-r--r--   0        0        0     5504 2024-04-22 20:19:18.782079 tantri-1.0.1/tantri/cli/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     1202 2024-04-22 20:19:18.898085 tantri-1.0.1/tantri/cli/__pycache__/file_importer.cpython-39.pyc
--rwxr-xr-x   0        0        0      904 2024-04-22 20:18:56.176965 tantri-1.0.1/tantri/cli/file_importer.py
--rwxr-xr-x   0        0        0      174 2024-04-22 20:18:56.176965 tantri-1.0.1/tantri/cli/input_files/__init__.py
--rw-r--r--   0        0        0      359 2024-04-22 20:19:18.886084 tantri-1.0.1/tantri/cli/input_files/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      967 2024-04-22 20:19:18.894085 tantri-1.0.1/tantri/cli/input_files/__pycache__/read_dipoles.cpython-39.pyc
--rw-r--r--   0        0        0      944 2024-04-22 20:19:18.886084 tantri-1.0.1/tantri/cli/input_files/__pycache__/read_dots.cpython-39.pyc
--rw-r--r--   0        0        0      715 2024-04-22 20:19:18.898085 tantri-1.0.1/tantri/cli/input_files/__pycache__/write_dipoles.cpython-39.pyc
--rwxr-xr-x   0        0        0      573 2024-04-22 20:18:56.176965 tantri-1.0.1/tantri/cli/input_files/read_dipoles.py
--rwxr-xr-x   0        0        0      511 2024-04-22 20:18:56.176965 tantri-1.0.1/tantri/cli/input_files/read_dots.py
--rwxr-xr-x   0        0        0      301 2024-04-22 20:18:56.176965 tantri-1.0.1/tantri/cli/input_files/write_dipoles.py
--rwxr-xr-x   0        0        0     3824 2024-04-22 20:18:56.176965 tantri-1.0.1/tantri/dipoles/__init__.py
--rw-r--r--   0        0        0     4360 2024-04-22 20:19:18.890084 tantri-1.0.1/tantri/dipoles/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      638 2024-04-22 20:19:18.890084 tantri-1.0.1/tantri/dipoles/__pycache__/types.cpython-39.pyc
--rwxr-xr-x   0        0        0     2724 2024-04-22 20:18:56.176965 tantri-1.0.1/tantri/dipoles/generation/__init__.py
--rw-r--r--   0        0        0     2534 2024-04-22 20:19:18.902085 tantri-1.0.1/tantri/dipoles/generation/__pycache__/__init__.cpython-39.pyc
--rwxr-xr-x   0        0        0      374 2024-04-22 20:18:56.176965 tantri-1.0.1/tantri/dipoles/types.py
--rwxr-xr-x   0        0        0       72 2024-04-22 20:18:56.176965 tantri-1.0.1/tantri/meta.py
--rwxr-xr-x   0        0        0      675 2024-04-22 20:18:56.176965 tantri-1.0.1/tantri/simple_telegraph/__init__.py
--rw-r--r--   0        0        0     1043 2024-04-22 20:19:18.426061 tantri-1.0.1/tantri/simple_telegraph/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0      902 1970-01-01 00:00:00.000000 tantri-1.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1306 2024-05-02 19:26:03.872458 tantri-1.1.0/README.md
+-rwxr-xr-x   0        0        0     1016 2024-05-02 19:26:03.872458 tantri-1.1.0/pyproject.toml
+-rwxr-xr-x   0        0        0      295 2024-05-02 19:26:03.872458 tantri-1.1.0/tantri/__init__.py
+-rwxr-xr-x   0        0        0     5944 2024-05-02 19:26:03.872458 tantri-1.1.0/tantri/cli/__init__.py
+-rw-r--r--   0        0        0     5881 2024-05-02 19:26:27.341693 tantri-1.1.0/tantri/cli/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1202 2024-05-02 19:26:27.437698 tantri-1.1.0/tantri/cli/__pycache__/file_importer.cpython-39.pyc
+-rwxr-xr-x   0        0        0      904 2024-05-02 19:26:03.872458 tantri-1.1.0/tantri/cli/file_importer.py
+-rwxr-xr-x   0        0        0      174 2024-05-02 19:26:03.872458 tantri-1.1.0/tantri/cli/input_files/__init__.py
+-rw-r--r--   0        0        0      359 2024-05-02 19:26:27.421697 tantri-1.1.0/tantri/cli/input_files/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      967 2024-05-02 19:26:27.437698 tantri-1.1.0/tantri/cli/input_files/__pycache__/read_dipoles.cpython-39.pyc
+-rw-r--r--   0        0        0      944 2024-05-02 19:26:27.421697 tantri-1.1.0/tantri/cli/input_files/__pycache__/read_dots.cpython-39.pyc
+-rw-r--r--   0        0        0      715 2024-05-02 19:26:27.437698 tantri-1.1.0/tantri/cli/input_files/__pycache__/write_dipoles.cpython-39.pyc
+-rwxr-xr-x   0        0        0      573 2024-05-02 19:26:03.872458 tantri-1.1.0/tantri/cli/input_files/read_dipoles.py
+-rwxr-xr-x   0        0        0      511 2024-05-02 19:26:03.872458 tantri-1.1.0/tantri/cli/input_files/read_dots.py
+-rwxr-xr-x   0        0        0      301 2024-05-02 19:26:03.872458 tantri-1.1.0/tantri/cli/input_files/write_dipoles.py
+-rwxr-xr-x   0        0        0      386 2024-05-02 19:26:03.872458 tantri-1.1.0/tantri/dipoles/__init__.py
+-rw-r--r--   0        0        0      523 2024-05-02 19:26:27.421697 tantri-1.1.0/tantri/dipoles/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0      986 2024-05-02 19:26:27.429698 tantri-1.1.0/tantri/dipoles/__pycache__/supersample.cpython-39.pyc
+-rw-r--r--   0        0        0     4597 2024-05-02 19:26:27.429698 tantri-1.1.0/tantri/dipoles/__pycache__/time_series.cpython-39.pyc
+-rw-r--r--   0        0        0     2047 2024-05-02 19:26:27.425698 tantri-1.1.0/tantri/dipoles/__pycache__/types.cpython-39.pyc
+-rwxr-xr-x   0        0        0      106 2024-05-02 19:26:03.872458 tantri-1.1.0/tantri/dipoles/generation/__init__.py
+-rw-r--r--   0        0        0      294 2024-05-02 19:26:27.433698 tantri-1.1.0/tantri/dipoles/generation/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1566 2024-05-02 19:26:27.433698 tantri-1.1.0/tantri/dipoles/generation/__pycache__/generate_dipole_config.cpython-39.pyc
+-rw-r--r--   0        0        0     1620 2024-05-02 19:26:03.872458 tantri-1.1.0/tantri/dipoles/generation/generate_dipole_config.py
+-rw-r--r--   0        0        0     1196 2024-05-02 19:26:03.872458 tantri-1.1.0/tantri/dipoles/supersample.py
+-rw-r--r--   0        0        0     4024 2024-05-02 19:26:03.872458 tantri-1.1.0/tantri/dipoles/time_series.py
+-rwxr-xr-x   0        0        0     1647 2024-05-02 19:26:03.872458 tantri-1.1.0/tantri/dipoles/types.py
+-rwxr-xr-x   0        0        0       72 2024-05-02 19:26:03.872458 tantri-1.1.0/tantri/meta.py
+-rwxr-xr-x   0        0        0      675 2024-05-02 19:26:03.872458 tantri-1.1.0/tantri/simple_telegraph/__init__.py
+-rw-r--r--   0        0        0     1043 2024-05-02 19:26:27.057678 tantri-1.1.0/tantri/simple_telegraph/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0     1837 1970-01-01 00:00:00.000000 tantri-1.1.0/PKG-INFO
```

### Comparing `tantri-1.0.1/pyproject.toml` & `tantri-1.1.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 [tool.poetry]
 name = "tantri"
-version = "1.0.1"
+version = "1.1.0"
 description = "Python dipole model evaluator"
 authors = ["Deepak <dmallubhotla+github@gmail.com>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.10"
 numpy = "^1.22.3"
 scipy = "~1.10"
 click = "^8.1.7"
-tqdm = "^4.66.2"
 
 [tool.poetry.dev-dependencies]
 pytest = ">=6"
 flake8 = "^4.0.0"
 pytest-cov = "^4.1.0"
 mypy = "^0.961"
 black = "^22.3.0"
```

### Comparing `tantri-1.0.1/tantri/cli/__init__.py` & `tantri-1.1.0/tantri/cli/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import click
 import logging
 import tantri
 import numpy
 import tantri.cli.input_files.write_dipoles
 import tantri.cli.file_importer
-import tantri.dipoles
 import json
-import tantri.dipoles.generation
+import tantri.dipoles
 import pathlib
-import tqdm  # type: ignore
+
 
 _logger = logging.getLogger(__name__)
 
 LOG_PATTERN = "%(asctime)s | %(levelname)-7s | %(name)s | %(message)s"
 
 
 POTENTIAL = "electric-potential"
@@ -89,15 +88,15 @@
 	type=int,
 	default=None,
 	help="A seed to use to create an override default rng. You should set this.",
 )
 @click.option(
 	"output_file",
 	"-o",
-	type=click.File("w"),
+	type=click.Path(path_type=pathlib.Path),
 	help="The output file to write, in csv format",
 	required=True,
 )
 @click.option("--header-row/--no-header-row", default=False, help="Write a header row")
 def write_time_series(
 	dipoles_file,
 	dots_file,
@@ -107,14 +106,36 @@
 	time_series_rng_seed,
 	output_file,
 	header_row,
 ):
 	"""
 	Generate a time series for the passed in parameters.
 	"""
+	_write_time_series(
+		dipoles_file,
+		dots_file,
+		measurement_type,
+		delta_t,
+		num_iterations,
+		time_series_rng_seed,
+		output_file,
+		header_row,
+	)
+
+
+def _write_time_series(
+	dipoles_file,
+	dots_file,
+	measurement_type,
+	delta_t,
+	num_iterations,
+	time_series_rng_seed,
+	output_file,
+	header_row,
+):
 	_logger.debug(
 		f"Received parameters [dipoles_file: {dipoles_file}] and [dots_file: {dots_file}]"
 	)
 	dipoles = tantri.cli.file_importer.read_dipoles_json_file(dipoles_file)
 	dots = tantri.cli.file_importer.read_dots_json_file(dots_file)
 
 	if measurement_type == POTENTIAL:
@@ -122,74 +143,80 @@
 		value_name = "V"
 	elif measurement_type == X_ELECTRIC_FIELD:
 		measurement_enum = tantri.dipoles.DipoleMeasurementType.X_ELECTRIC_FIELD
 		value_name = "Ex"
 
 	_logger.debug(f"Using measurement {measurement_enum.name}")
 	labels = [dot.label for dot in dots]
-	if header_row:
-		value_labels = ", ".join([f"{value_name}_{label}" for label in labels])
-		output_file.write(f"t (s), {value_labels}\n")
+	with output_file.open("w") as out:
+		if header_row:
+			value_labels = ", ".join([f"{value_name}_{label}" for label in labels])
+			out.write(f"t (s), {value_labels}\n")
 
-	_logger.debug(
-		f"Going to simulate {num_iterations} iterations with a delta t of {delta_t}"
-	)
-
-	_logger.debug(f"Got seed {time_series_rng_seed}")
-	if time_series_rng_seed is None:
-		time_series = tantri.dipoles.DipoleTimeSeries(
-			dipoles, dots, measurement_enum, delta_t
-		)
-	else:
-		rng = numpy.random.default_rng(time_series_rng_seed)
-		time_series = tantri.dipoles.DipoleTimeSeries(
-			dipoles, dots, measurement_enum, delta_t, rng
+		_logger.debug(
+			f"Going to simulate {num_iterations} iterations with a delta t of {delta_t}"
 		)
 
-	for i in tqdm.trange(num_iterations):
-		transition = time_series.transition()
-		transition_values = ", ".join(str(transition[label]) for label in labels)
-		output_file.write(f"{i * delta_t}, {transition_values}\n")
+		_logger.debug(f"Got seed {time_series_rng_seed}")
+		if time_series_rng_seed is None:
+			time_series = tantri.dipoles.DipoleTimeSeries(
+				dipoles, dots, measurement_enum, delta_t
+			)
+		else:
+			rng = numpy.random.default_rng(time_series_rng_seed)
+			time_series = tantri.dipoles.DipoleTimeSeries(
+				dipoles, dots, measurement_enum, delta_t, rng
+			)
+
+		for i in range(num_iterations):
+			transition = time_series.transition()
+			transition_values = ", ".join(str(transition[label]) for label in labels)
+			out.write(f"{i * delta_t}, {transition_values}\n")
 
 
 @cli.command()
 @click.argument(
 	"generation_config",
 	type=click.Path(exists=True, path_type=pathlib.Path),
 )
 @click.argument(
 	"output_file",
-	type=click.File("w"),
+	type=click.Path(path_type=pathlib.Path),
 )
 @click.option(
 	"--override-rng-seed", type=int, help="Seed to override the generation config spec."
 )
 def generate_dipoles(generation_config, output_file, override_rng_seed):
+	_generate_dipoles(generation_config, output_file, override_rng_seed)
+
+
+def _generate_dipoles(generation_config, output_file, override_rng_seed):
 	"""Generate random dipoles as described by GENERATION_CONFIG and output to OUTPUT_FILE.
 
 	GENERATION_CONFIG should be a JSON file that matches the appropriate spec, and OUTPUT_FILE will contain JSON formatted contents.
 	OUTPUT_FILE will be overwritten, if it exists.
 
 	If the --override-rng-seed is set, it's better to keep logs of the generation!
 	"""
 	_logger.debug(
 		f"generate_dipoles was called, with config file {click.format_filename(generation_config)}"
 	)
 	_logger.debug(f"override_rng_seed: [{override_rng_seed}]")
 
 	with open(generation_config, "r") as config_file:
 		data = json.load(config_file)
-	config = tantri.dipoles.generation.DipoleGenerationConfig(**data)
+	config = tantri.dipoles.DipoleGenerationConfig(**data)
 
 	override_rng = None
 	if override_rng_seed is not None:
 		_logger.info(f"Overriding the rng with a new one with seed {override_rng_seed}")
 		override_rng = numpy.random.default_rng(override_rng_seed)
 	_logger.debug(f"generating dipoles with config {config}...")
-	generated = tantri.dipoles.generation.make_dipoles(config, override_rng)
+	generated = tantri.dipoles.make_dipoles(config, override_rng)
 
-	output_file.write(
-		json.dumps(
-			[g.as_dict() for g in generated],
-			cls=tantri.cli.input_files.write_dipoles.NumpyEncoder,
+	with output_file.open("w") as out:
+		out.write(
+			json.dumps(
+				[g.as_dict() for g in generated],
+				cls=tantri.cli.input_files.write_dipoles.NumpyEncoder,
+			)
 		)
-	)
```

### Comparing `tantri-1.0.1/tantri/cli/__pycache__/__init__.cpython-39.pyc` & `tantri-1.1.0/tantri/cli/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 22 20:18:56 2024 UTC, .py size: 5467 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,344 +1,368 @@
-00000000: 610d 0d0a 0000 0000 30c6 2666 5b15 0000  a.......0.&f[...
+00000000: 610d 0d0a 0000 0000 cbe8 3366 3817 0000  a.........3f8...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 000e 0000 0040 0000 0073 de01 0000 6400  .....@...s....d.
+00000020: 000e 0000 0040 0000 0073 e601 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a03 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6401 6c04 5a02 6400 6401 6c05 5a02 6400  d.l.Z.d.d.l.Z.d.
-00000060: 6401 6c06 5a02 6400 6401 6c07 5a07 6400  d.l.Z.d.d.l.Z.d.
-00000070: 6401 6c08 5a02 6400 6401 6c09 5a09 6400  d.l.Z.d.d.l.Z.d.
-00000080: 6401 6c0a 5a0a 6501 a00b 650c a101 5a0d  d.l.Z.e...e...Z.
-00000090: 6402 5a0e 6403 5a0f 6404 5a10 6405 6406  d.Z.d.Z.d.Z.d.d.
-000000a0: 8400 5a11 6500 a012 a100 6500 6a13 6407  ..Z.e.....e.j.d.
-000000b0: 6408 6409 640a 640b 8d04 6500 6a13 640c  d.d.d.d...e.j.d.
-000000c0: 640d 640e 8d02 6500 a014 6502 a015 a100  d.d...e...e.....
-000000d0: a101 640f 6410 8400 8301 8301 8301 8301  ..d.d...........
-000000e0: 5a16 6516 a017 a100 6500 6a13 6411 6412  Z.e.....e.j.d.d.
-000000f0: 6409 6500 6a18 6409 6509 6a18 6413 8d02  d.e.j.d.e.j.d...
-00000100: 6414 6415 8d05 6500 6a13 6416 6417 6409  d.d...e.j.d.d.d.
-00000110: 6500 6a18 6409 6509 6a18 6413 8d02 6418  e.j.d.e.j.d...d.
-00000120: 6415 8d05 6500 6a13 6419 6500 a019 650f  d...e.j.d.e...e.
-00000130: 6510 6702 a101 650f 641a 6409 641b 8d05  e.g...e.d.d.d...
-00000140: 6500 6a13 641c 641d 651a 641e 641f 6409  e.j.d.d.e.d.d.d.
-00000150: 641b 8d06 6500 6a13 6420 6421 651b 6422  d...e.j.d d!e.d"
-00000160: 6423 6409 641b 8d06 6500 6a13 6424 6425  d#d.d...e.j.d$d%
-00000170: 651b 6401 6426 6427 8d05 6500 6a13 6428  e.d.d&d'..e.j.d(
-00000180: 6429 6500 a01c 642a a101 642b 6409 642c  d)e...d*..d+d.d,
-00000190: 8d05 6500 6a13 642d 640a 642e 642f 8d03  ..e.j.d-d.d.d/..
-000001a0: 6430 6431 8400 8301 8301 8301 8301 8301  d0d1............
-000001b0: 8301 8301 8301 8301 5a1d 6516 a017 a100  ........Z.e.....
-000001c0: 6500 6a1e 6432 6500 6a18 6409 6509 6a18  e.j.d2e.j.d.e.j.
-000001d0: 6413 8d02 6433 8d02 6500 6a1e 6428 6500  d...d3..e.j.d(e.
-000001e0: a01c 642a a101 6433 8d02 6500 6a13 6434  ..d*..d3..e.j.d4
-000001f0: 651b 6435 6436 8d03 6437 6438 8400 8301  e.d5d6..d7d8....
-00000200: 8301 8301 8301 5a1f 6401 5300 2939 e900  ......Z.d.S.)9..
-00000210: 0000 004e 7a36 2528 6173 6374 696d 6529  ...Nz6%(asctime)
-00000220: 7320 7c20 2528 6c65 7665 6c6e 616d 6529  s | %(levelname)
-00000230: 2d37 7320 7c20 2528 6e61 6d65 2973 207c  -7s | %(name)s |
-00000240: 2025 286d 6573 7361 6765 2973 7a12 656c   %(message)sz.el
-00000250: 6563 7472 6963 2d70 6f74 656e 7469 616c  ectric-potential
-00000260: 7a10 782d 656c 6563 7472 6963 2d66 6965  z.x-electric-fie
-00000270: 6c64 6301 0000 0000 0000 0000 0000 0002  ldc.............
-00000280: 0000 0005 0000 0043 0000 0073 5400 0000  .......C...sT...
-00000290: 7400 a001 a100 6701 7d01 7c00 6400 7501  t.....g.}.|.d.u.
-000002a0: 7222 7c01 a002 7400 a003 7c00 a101 a101  r"|...t...|.....
-000002b0: 0100 7400 6a04 7400 6a05 7406 7c01 6401  ..t.j.t.j.t.|.d.
-000002c0: 8d03 0100 7400 a007 6402 a101 a008 7400  ....t...d.....t.
-000002d0: 6a09 a101 0100 7400 a00a 6403 a101 0100  j.....t...d.....
-000002e0: 6400 5300 2904 4e29 03da 056c 6576 656c  d.S.).N)...level
-000002f0: da06 666f 726d 6174 da08 6861 6e64 6c65  ..format..handle
-00000300: 7273 5a04 7064 6d65 5429 0bda 076c 6f67  rsZ.pdmeT)...log
-00000310: 6769 6e67 da0d 5374 7265 616d 4861 6e64  ging..StreamHand
-00000320: 6c65 72da 0661 7070 656e 64da 0b46 696c  ler..append..Fil
-00000330: 6548 616e 646c 6572 da0b 6261 7369 6343  eHandler..basicC
-00000340: 6f6e 6669 67da 0544 4542 5547 da0b 4c4f  onfig..DEBUG..LO
-00000350: 475f 5041 5454 4552 4eda 0967 6574 4c6f  G_PATTERN..getLo
-00000360: 6767 6572 da08 7365 744c 6576 656c da04  gger..setLevel..
-00000370: 494e 464f da0f 6361 7074 7572 6557 6172  INFO..captureWar
-00000380: 6e69 6e67 7329 02da 0866 696c 656e 616d  nings)...filenam
-00000390: 6572 0400 0000 a900 7211 0000 00fa 4f2f  er......r.....O/
-000003a0: 686f 6d65 2f6a 656e 6b69 6e73 2f61 6765  home/jenkins/age
-000003b0: 6e74 2f77 6f72 6b73 7061 6365 2f67 6974  nt/workspace/git
-000003c0: 6561 2d70 6879 7369 6373 5f74 616e 7472  ea-physics_tantr
-000003d0: 695f 312e 302e 312f 7461 6e74 7269 2f63  i_1.0.1/tantri/c
-000003e0: 6c69 2f5f 5f69 6e69 745f 5f2e 7079 da0f  li/__init__.py..
-000003f0: 5f73 6574 5f75 705f 6c6f 6767 696e 6716  _set_up_logging.
-00000400: 0000 0073 1400 0000 0001 0a01 0801 1001  ...s............
-00000410: 0401 0401 0201 02fd 0605 1201 7213 0000  ............r...
-00000420: 007a 052d 2d6c 6f67 7a1d 456e 6162 6c65  .z.--logz.Enable
-00000430: 206c 6f67 6769 6e67 2074 6f20 7374 7265   logging to stre
-00000440: 616d 206f 6e6c 7954 4629 03da 0468 656c  am onlyTF)...hel
-00000450: 705a 0769 735f 666c 6167 da07 6465 6661  pZ.is_flag..defa
-00000460: 756c 747a 0a2d 2d6c 6f67 2d66 696c 657a  ultz.--log-filez
-00000470: 2d41 2066 696c 656e 616d 6520 746f 2075  -A filename to u
-00000480: 7365 2066 6f72 206c 6f67 6769 6e67 2028  se for logging (
-00000490: 696d 706c 6965 7320 2d2d 6c6f 6729 2901  implies --log)).
-000004a0: 7214 0000 0063 0200 0000 0000 0000 0000  r....c..........
-000004b0: 0000 0200 0000 0200 0000 4300 0000 7318  ..........C...s.
-000004c0: 0000 007c 0073 0c7c 0164 0175 0172 1474  ...|.s.|.d.u.r.t
-000004d0: 007c 0183 0101 0064 0153 0029 027a 3855  .|.....d.S.).z8U
-000004e0: 7469 6c69 7469 6573 2066 6f72 2067 656e  tilities for gen
-000004f0: 6572 6174 696e 6720 7369 6d75 6c61 7465  erating simulate
-00000500: 6420 544c 5320 7469 6d65 2073 6572 6965  d TLS time serie
-00000510: 7320 6461 7461 2e4e 2901 7213 0000 0029  s data.N).r....)
-00000520: 02da 036c 6f67 da08 6c6f 675f 6669 6c65  ...log..log_file
-00000530: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
-00000540: 0363 6c69 2300 0000 7304 0000 0000 080c  .cli#...s.......
-00000550: 0272 1800 0000 7a0e 2d2d 6469 706f 6c65  .r....z.--dipole
-00000560: 732d 6669 6c65 7a0c 6469 706f 6c65 732e  s-filez.dipoles.
-00000570: 6a73 6f6e 2902 da06 6578 6973 7473 da09  json)...exists..
-00000580: 7061 7468 5f74 7970 657a 1f46 696c 6520  path_typez.File 
-00000590: 7769 7468 206a 736f 6e20 6172 7261 7920  with json array 
-000005a0: 6f66 2064 6970 6f6c 6573 2904 7215 0000  of dipoles).r...
-000005b0: 00da 0c73 686f 775f 6465 6661 756c 74da  ...show_default.
-000005c0: 0474 7970 6572 1400 0000 7a0b 2d2d 646f  .typer....z.--do
-000005d0: 7473 2d66 696c 657a 0964 6f74 732e 6a73  ts-filez.dots.js
-000005e0: 6f6e 7a1c 4669 6c65 2077 6974 6820 6a73  onz.File with js
-000005f0: 6f6e 2061 7272 6179 206f 6620 646f 7473  on array of dots
-00000600: 7a12 2d2d 6d65 6173 7572 656d 656e 742d  z.--measurement-
-00000610: 7479 7065 7a23 5468 6520 7479 7065 206f  typez#The type o
-00000620: 6620 6d65 6173 7572 656d 656e 7420 746f  f measurement to
-00000630: 2073 696d 756c 6174 6529 0472 1c00 0000   simulate).r....
-00000640: 7215 0000 0072 1400 0000 721b 0000 007a  r....r....r....z
-00000650: 092d 2d64 656c 7461 2d74 7a02 2d74 e901  .--delta-tz.-t..
-00000660: 0000 007a 2b54 6865 2064 656c 7461 2074  ...z+The delta t
-00000670: 2062 6574 7765 656e 2074 696d 6520 7365   between time se
-00000680: 7269 6573 2069 7465 7261 7469 6f6e 732e  ries iterations.
-00000690: 7a10 2d2d 6e75 6d2d 6974 6572 6174 696f  z.--num-iteratio
-000006a0: 6e73 7a02 2d6e e90a 0000 007a 1954 6865  nsz.-n.....z.The
-000006b0: 206e 756d 6265 7220 6f66 2069 7465 7261   number of itera
-000006c0: 7469 6f6e 732e 7a16 2d2d 7469 6d65 2d73  tions.z.--time-s
-000006d0: 6572 6965 732d 726e 672d 7365 6564 7a02  eries-rng-seedz.
-000006e0: 2d73 7a45 4120 7365 6564 2074 6f20 7573  -szEA seed to us
-000006f0: 6520 746f 2063 7265 6174 6520 616e 206f  e to create an o
-00000700: 7665 7272 6964 6520 6465 6661 756c 7420  verride default 
-00000710: 726e 672e 2059 6f75 2073 686f 756c 6420  rng. You should 
-00000720: 7365 7420 7468 6973 2e29 0372 1c00 0000  set this.).r....
-00000730: 7215 0000 0072 1400 0000 da0b 6f75 7470  r....r......outp
-00000740: 7574 5f66 696c 657a 022d 6fda 0177 7a27  ut_filez.-o..wz'
-00000750: 5468 6520 6f75 7470 7574 2066 696c 6520  The output file 
-00000760: 746f 2077 7269 7465 2c20 696e 2063 7376  to write, in csv
-00000770: 2066 6f72 6d61 7429 0372 1c00 0000 7214   format).r....r.
-00000780: 0000 00da 0872 6571 7569 7265 647a 1c2d  .....requiredz.-
-00000790: 2d68 6561 6465 722d 726f 772f 2d2d 6e6f  -header-row/--no
-000007a0: 2d68 6561 6465 722d 726f 777a 1257 7269  -header-rowz.Wri
-000007b0: 7465 2061 2068 6561 6465 7220 726f 7729  te a header row)
-000007c0: 0272 1500 0000 7214 0000 0063 0800 0000  .r....r....c....
-000007d0: 0000 0000 0000 0000 1100 0000 0700 0000  ................
-000007e0: 0300 0000 7362 0100 0074 00a0 0164 017c  ....sb...t...d.|
-000007f0: 009b 0064 027c 019b 0064 039d 05a1 0101  ...d.|...d......
-00000800: 0074 026a 036a 04a0 057c 00a1 017d 0874  .t.j.j...|...}.t
-00000810: 026a 036a 04a0 067c 01a1 017d 097c 0274  .j.j...|...}.|.t
-00000820: 076b 0272 4c74 026a 086a 096a 0a7d 0a64  .k.rLt.j.j.j.}.d
-00000830: 0489 016e 167c 0274 0b6b 0272 6274 026a  ...n.|.t.k.rbt.j
-00000840: 086a 096a 0b7d 0a64 0589 0174 00a0 0164  .j.j.}.d...t...d
-00000850: 067c 0a6a 0c9b 009d 02a1 0101 0064 0764  .|.j.........d.d
-00000860: 0884 007c 0944 0083 017d 0b7c 0772 b064  ...|.D...}.|.r.d
-00000870: 09a0 0d87 0166 0164 0a64 0884 087c 0b44  .....f.d.d...|.D
-00000880: 0083 01a1 017d 0c7c 06a0 0e64 0b7c 0c9b  .....}.|...d.|..
-00000890: 0064 0c9d 03a1 0101 0074 00a0 0164 0d7c  .d.......t...d.|
-000008a0: 049b 0064 0e7c 039b 009d 04a1 0101 0074  ...d.|.........t
-000008b0: 00a0 0164 0f7c 059b 009d 02a1 0101 007c  ...d.|.........|
-000008c0: 0564 1075 0072 f274 026a 08a0 0f7c 087c  .d.u.r.t.j...|.|
-000008d0: 097c 0a7c 03a1 047d 0d6e 2074 106a 11a0  .|.|...}.n t.j..
-000008e0: 127c 05a1 017d 0e74 026a 08a0 0f7c 087c  .|...}.t.j...|.|
-000008f0: 097c 0a7c 037c 0ea1 057d 0d74 13a0 147c  .|.|.|...}.t...|
-00000900: 04a1 0144 005d 407d 0f7c 0da0 15a1 0089  ...D.]@}.|......
-00000910: 0064 09a0 0d87 0066 0164 1164 1284 087c  .d.....f.d.d...|
-00000920: 0b44 0083 01a1 017d 107c 06a0 0e7c 0f7c  .D.....}.|...|.|
-00000930: 0314 009b 0064 097c 109b 0064 0c9d 04a1  .....d.|...d....
-00000940: 0101 0090 0171 1c64 1053 0029 137a 380a  .....q.d.S.).z8.
-00000950: 0947 656e 6572 6174 6520 6120 7469 6d65  .Generate a time
-00000960: 2073 6572 6965 7320 666f 7220 7468 6520   series for the 
-00000970: 7061 7373 6564 2069 6e20 7061 7261 6d65  passed in parame
-00000980: 7465 7273 2e0a 097a 2352 6563 6569 7665  ters...z#Receive
-00000990: 6420 7061 7261 6d65 7465 7273 205b 6469  d parameters [di
-000009a0: 706f 6c65 735f 6669 6c65 3a20 7a12 5d20  poles_file: z.] 
-000009b0: 616e 6420 5b64 6f74 735f 6669 6c65 3a20  and [dots_file: 
-000009c0: da01 5dda 0156 5a02 4578 7a12 5573 696e  ..]..VZ.Exz.Usin
-000009d0: 6720 6d65 6173 7572 656d 656e 7420 6301  g measurement c.
-000009e0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
-000009f0: 0000 0053 0000 0073 1200 0000 6700 7c00  ...S...s....g.|.
-00000a00: 5d0a 7d01 7c01 6a00 9102 7104 5300 7211  ].}.|.j...q.S.r.
-00000a10: 0000 0029 01da 056c 6162 656c 2902 da02  ...)...label)...
-00000a20: 2e30 da03 646f 7472 1100 0000 7211 0000  .0..dotr....r...
-00000a30: 0072 1200 0000 da0a 3c6c 6973 7463 6f6d  .r......<listcom
-00000a40: 703e 8000 0000 f300 0000 007a 2577 7269  p>.........z%wri
-00000a50: 7465 5f74 696d 655f 7365 7269 6573 2e3c  te_time_series.<
-00000a60: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
-00000a70: 703e 7a02 2c20 6301 0000 0000 0000 0000  p>z., c.........
-00000a80: 0000 0002 0000 0005 0000 0013 0000 0073  ...............s
-00000a90: 1a00 0000 6700 7c00 5d12 7d01 8800 9b00  ....g.|.].}.....
-00000aa0: 6400 7c01 9b00 9d03 9102 7104 5300 2901  d.|.......q.S.).
-00000ab0: da01 5f72 1100 0000 a902 7225 0000 0072  .._r......r%...r
-00000ac0: 2400 0000 2901 da0a 7661 6c75 655f 6e61  $...)...value_na
-00000ad0: 6d65 7211 0000 0072 1200 0000 7227 0000  mer....r....r'..
-00000ae0: 0082 0000 0072 2800 0000 7a07 7420 2873  .....r(...z.t (s
-00000af0: 292c 20da 010a 7a12 476f 696e 6720 746f  ), ...z.Going to
-00000b00: 2073 696d 756c 6174 6520 7a1e 2069 7465   simulate z. ite
-00000b10: 7261 7469 6f6e 7320 7769 7468 2061 2064  rations with a d
-00000b20: 656c 7461 2074 206f 6620 7a09 476f 7420  elta t of z.Got 
-00000b30: 7365 6564 204e 6301 0000 0000 0000 0000  seed Nc.........
-00000b40: 0000 0002 0000 0004 0000 0033 0000 0073  ...........3...s
-00000b50: 1a00 0000 7c00 5d12 7d01 7400 8800 7c01  ....|.].}.t...|.
-00000b60: 1900 8301 5600 0100 7102 6400 5300 2901  ....V...q.d.S.).
-00000b70: 4e29 01da 0373 7472 722a 0000 0029 01da  N)...strr*...)..
-00000b80: 0a74 7261 6e73 6974 696f 6e72 1100 0000  .transitionr....
-00000b90: 7212 0000 00da 093c 6765 6e65 7870 723e  r......<genexpr>
-00000ba0: 9600 0000 7228 0000 007a 2477 7269 7465  ....r(...z$write
-00000bb0: 5f74 696d 655f 7365 7269 6573 2e3c 6c6f  _time_series.<lo
-00000bc0: 6361 6c73 3e2e 3c67 656e 6578 7072 3e29  cals>.<genexpr>)
-00000bd0: 16da 075f 6c6f 6767 6572 da05 6465 6275  ..._logger..debu
-00000be0: 67da 0674 616e 7472 6972 1800 0000 5a0d  g..tantrir....Z.
-00000bf0: 6669 6c65 5f69 6d70 6f72 7465 725a 1672  file_importerZ.r
-00000c00: 6561 645f 6469 706f 6c65 735f 6a73 6f6e  ead_dipoles_json
-00000c10: 5f66 696c 655a 1372 6561 645f 646f 7473  _fileZ.read_dots
-00000c20: 5f6a 736f 6e5f 6669 6c65 da09 504f 5445  _json_file..POTE
-00000c30: 4e54 4941 4cda 0764 6970 6f6c 6573 5a15  NTIAL..dipolesZ.
-00000c40: 4469 706f 6c65 4d65 6173 7572 656d 656e  DipoleMeasuremen
-00000c50: 7454 7970 655a 1245 4c45 4354 5249 435f  tTypeZ.ELECTRIC_
-00000c60: 504f 5445 4e54 4941 4cda 1058 5f45 4c45  POTENTIAL..X_ELE
-00000c70: 4354 5249 435f 4649 454c 44da 046e 616d  CTRIC_FIELD..nam
-00000c80: 65da 046a 6f69 6eda 0577 7269 7465 5a10  e..join..writeZ.
-00000c90: 4469 706f 6c65 5469 6d65 5365 7269 6573  DipoleTimeSeries
-00000ca0: da05 6e75 6d70 79da 0672 616e 646f 6dda  ..numpy..random.
-00000cb0: 0b64 6566 6175 6c74 5f72 6e67 da04 7471  .default_rng..tq
-00000cc0: 646d 5a06 7472 616e 6765 722e 0000 0029  dmZ.tranger....)
-00000cd0: 115a 0c64 6970 6f6c 6573 5f66 696c 655a  .Z.dipoles_fileZ
-00000ce0: 0964 6f74 735f 6669 6c65 5a10 6d65 6173  .dots_fileZ.meas
-00000cf0: 7572 656d 656e 745f 7479 7065 5a07 6465  urement_typeZ.de
-00000d00: 6c74 615f 745a 0e6e 756d 5f69 7465 7261  lta_tZ.num_itera
-00000d10: 7469 6f6e 735a 1474 696d 655f 7365 7269  tionsZ.time_seri
-00000d20: 6573 5f72 6e67 5f73 6565 6472 1f00 0000  es_rng_seedr....
-00000d30: da0a 6865 6164 6572 5f72 6f77 7234 0000  ..header_rowr4..
-00000d40: 00da 0464 6f74 735a 106d 6561 7375 7265  ...dotsZ.measure
-00000d50: 6d65 6e74 5f65 6e75 6dda 066c 6162 656c  ment_enum..label
-00000d60: 735a 0c76 616c 7565 5f6c 6162 656c 735a  sZ.value_labelsZ
-00000d70: 0b74 696d 655f 7365 7269 6573 da03 726e  .time_series..rn
-00000d80: 67da 0169 5a11 7472 616e 7369 7469 6f6e  g..iZ.transition
-00000d90: 5f76 616c 7565 7372 1100 0000 2902 722e  _valuesr....).r.
-00000da0: 0000 0072 2b00 0000 7212 0000 00da 1177  ...r+...r......w
-00000db0: 7269 7465 5f74 696d 655f 7365 7269 6573  rite_time_series
-00000dc0: 3000 0000 7340 0000 0000 4204 0110 ff04  0...s@....B.....
-00000dd0: 030e 010e 0208 010a 0106 0108 010a 0104  ................
-00000de0: 0212 010e 0104 0118 0112 0204 010e ff04  ................
-00000df0: 0410 0108 0106 0108 ff06 040c 0106 010a  ................
-00000e00: ff04 040e 0108 0118 0172 4200 0000 da11  .........rB.....
-00000e10: 6765 6e65 7261 7469 6f6e 5f63 6f6e 6669  generation_confi
-00000e20: 6729 0172 1c00 0000 7a13 2d2d 6f76 6572  g).r....z.--over
-00000e30: 7269 6465 2d72 6e67 2d73 6565 647a 2c53  ride-rng-seedz,S
-00000e40: 6565 6420 746f 206f 7665 7272 6964 6520  eed to override 
-00000e50: 7468 6520 6765 6e65 7261 7469 6f6e 2063  the generation c
-00000e60: 6f6e 6669 6720 7370 6563 2e29 0272 1c00  onfig spec.).r..
-00000e70: 0000 7214 0000 0063 0300 0000 0000 0000  ..r....c........
-00000e80: 0000 0000 0800 0000 0800 0000 4300 0000  ............C...
-00000e90: 73e4 0000 0074 00a0 0164 0174 02a0 037c  s....t...d.t...|
-00000ea0: 00a1 019b 009d 02a1 0101 0074 00a0 0164  ...........t...d
-00000eb0: 027c 029b 0064 039d 03a1 0101 0074 047c  .|...d.......t.|
-00000ec0: 0064 0483 028f 1a7d 0374 05a0 067c 03a1  .d.....}.t...|..
-00000ed0: 017d 0457 0064 0504 0004 0083 0301 006e  .}.W.d.........n
-00000ee0: 1031 0073 5230 0001 0001 0001 0059 0001  .1.sR0.......Y..
-00000ef0: 0074 076a 086a 096a 0a66 0069 007c 04a4  .t.j.j.j.f.i.|..
-00000f00: 018e 017d 0564 057d 067c 0264 0575 0172  ...}.d.}.|.d.u.r
-00000f10: 9874 00a0 0b64 067c 029b 009d 02a1 0101  .t...d.|........
-00000f20: 0074 0c6a 0da0 0e7c 02a1 017d 0674 00a0  .t.j...|...}.t..
-00000f30: 0164 077c 059b 0064 089d 03a1 0101 0074  .d.|...d.......t
-00000f40: 076a 086a 09a0 0f7c 057c 06a1 027d 077c  .j.j...|.|...}.|
-00000f50: 01a0 1074 056a 1164 0964 0a84 007c 0744  ...t.j.d.d...|.D
-00000f60: 0083 0174 076a 126a 136a 146a 1564 0b8d  ...t.j.j.j.j.d..
-00000f70: 02a1 0101 0064 0553 0029 0c61 5a01 0000  .....d.S.).aZ...
-00000f80: 4765 6e65 7261 7465 2072 616e 646f 6d20  Generate random 
-00000f90: 6469 706f 6c65 7320 6173 2064 6573 6372  dipoles as descr
-00000fa0: 6962 6564 2062 7920 4745 4e45 5241 5449  ibed by GENERATI
-00000fb0: 4f4e 5f43 4f4e 4649 4720 616e 6420 6f75  ON_CONFIG and ou
-00000fc0: 7470 7574 2074 6f20 4f55 5450 5554 5f46  tput to OUTPUT_F
-00000fd0: 494c 452e 0a0a 0947 454e 4552 4154 494f  ILE....GENERATIO
-00000fe0: 4e5f 434f 4e46 4947 2073 686f 756c 6420  N_CONFIG should 
-00000ff0: 6265 2061 204a 534f 4e20 6669 6c65 2074  be a JSON file t
-00001000: 6861 7420 6d61 7463 6865 7320 7468 6520  hat matches the 
-00001010: 6170 7072 6f70 7269 6174 6520 7370 6563  appropriate spec
-00001020: 2c20 616e 6420 4f55 5450 5554 5f46 494c  , and OUTPUT_FIL
-00001030: 4520 7769 6c6c 2063 6f6e 7461 696e 204a  E will contain J
-00001040: 534f 4e20 666f 726d 6174 7465 6420 636f  SON formatted co
-00001050: 6e74 656e 7473 2e0a 094f 5554 5055 545f  ntents...OUTPUT_
-00001060: 4649 4c45 2077 696c 6c20 6265 206f 7665  FILE will be ove
-00001070: 7277 7269 7474 656e 2c20 6966 2069 7420  rwritten, if it 
-00001080: 6578 6973 7473 2e0a 0a09 4966 2074 6865  exists....If the
-00001090: 202d 2d6f 7665 7272 6964 652d 726e 672d   --override-rng-
-000010a0: 7365 6564 2069 7320 7365 742c 2069 7427  seed is set, it'
-000010b0: 7320 6265 7474 6572 2074 6f20 6b65 6570  s better to keep
-000010c0: 206c 6f67 7320 6f66 2074 6865 2067 656e   logs of the gen
-000010d0: 6572 6174 696f 6e21 0a09 7a2e 6765 6e65  eration!..z.gene
-000010e0: 7261 7465 5f64 6970 6f6c 6573 2077 6173  rate_dipoles was
-000010f0: 2063 616c 6c65 642c 2077 6974 6820 636f   called, with co
-00001100: 6e66 6967 2066 696c 6520 7a14 6f76 6572  nfig file z.over
-00001110: 7269 6465 5f72 6e67 5f73 6565 643a 205b  ride_rng_seed: [
-00001120: 7222 0000 00da 0172 4e7a 2c4f 7665 7272  r".....rNz,Overr
-00001130: 6964 696e 6720 7468 6520 726e 6720 7769  iding the rng wi
-00001140: 7468 2061 206e 6577 206f 6e65 2077 6974  th a new one wit
-00001150: 6820 7365 6564 207a 1f67 656e 6572 6174  h seed z.generat
-00001160: 696e 6720 6469 706f 6c65 7320 7769 7468  ing dipoles with
-00001170: 2063 6f6e 6669 6720 7a03 2e2e 2e63 0100   config z....c..
-00001180: 0000 0000 0000 0000 0000 0200 0000 0400  ................
-00001190: 0000 5300 0000 7314 0000 0067 007c 005d  ..S...s....g.|.]
-000011a0: 0c7d 017c 01a0 00a1 0091 0271 0453 0072  .}.|.......q.S.r
-000011b0: 1100 0000 2901 5a07 6173 5f64 6963 7429  ....).Z.as_dict)
-000011c0: 0272 2500 0000 da01 6772 1100 0000 7211  .r%.....gr....r.
-000011d0: 0000 0072 1200 0000 7227 0000 00c0 0000  ...r....r'......
-000011e0: 0072 2800 0000 7a24 6765 6e65 7261 7465  .r(...z$generate
-000011f0: 5f64 6970 6f6c 6573 2e3c 6c6f 6361 6c73  _dipoles.<locals
-00001200: 3e2e 3c6c 6973 7463 6f6d 703e 2901 da03  >.<listcomp>)...
-00001210: 636c 7329 1672 3000 0000 7231 0000 00da  cls).r0...r1....
-00001220: 0563 6c69 636b 5a0f 666f 726d 6174 5f66  .clickZ.format_f
-00001230: 696c 656e 616d 65da 046f 7065 6eda 046a  ilename..open..j
-00001240: 736f 6eda 046c 6f61 6472 3200 0000 7234  son..loadr2...r4
-00001250: 0000 005a 0a67 656e 6572 6174 696f 6e5a  ...Z.generationZ
-00001260: 1644 6970 6f6c 6547 656e 6572 6174 696f  .DipoleGeneratio
-00001270: 6e43 6f6e 6669 67da 0469 6e66 6f72 3900  nConfig..infor9.
-00001280: 0000 723a 0000 0072 3b00 0000 5a0c 6d61  ..r:...r;...Z.ma
-00001290: 6b65 5f64 6970 6f6c 6573 7238 0000 00da  ke_dipolesr8....
-000012a0: 0564 756d 7073 7218 0000 00da 0b69 6e70  .dumpsr......inp
-000012b0: 7574 5f66 696c 6573 5a0d 7772 6974 655f  ut_filesZ.write_
-000012c0: 6469 706f 6c65 735a 0c4e 756d 7079 456e  dipolesZ.NumpyEn
-000012d0: 636f 6465 7229 0872 4300 0000 721f 0000  coder).rC...r...
-000012e0: 005a 116f 7665 7272 6964 655f 726e 675f  .Z.override_rng_
-000012f0: 7365 6564 da0b 636f 6e66 6967 5f66 696c  seed..config_fil
-00001300: 65da 0464 6174 61da 0663 6f6e 6669 675a  e..data..configZ
-00001310: 0c6f 7665 7272 6964 655f 726e 675a 0967  .override_rngZ.g
-00001320: 656e 6572 6174 6564 7211 0000 0072 1100  eneratedr....r..
-00001330: 0000 7212 0000 00da 1067 656e 6572 6174  ..r......generat
-00001340: 655f 6469 706f 6c65 739a 0000 0073 2600  e_dipoles....s&.
-00001350: 0000 0014 0401 0eff 0403 1202 0c01 2801  ..............(.
-00001360: 1402 0401 0801 1001 0c01 1201 1002 0401  ................
-00001370: 0401 0c01 0afe 04ff 7251 0000 0029 2072  ........rQ...) r
-00001380: 4700 0000 7205 0000 0072 3200 0000 7239  G...r....r2...r9
-00001390: 0000 005a 2474 616e 7472 692e 636c 692e  ...Z$tantri.cli.
-000013a0: 696e 7075 745f 6669 6c65 732e 7772 6974  input_files.writ
-000013b0: 655f 6469 706f 6c65 735a 1874 616e 7472  e_dipolesZ.tantr
-000013c0: 692e 636c 692e 6669 6c65 5f69 6d70 6f72  i.cli.file_impor
-000013d0: 7465 725a 0e74 616e 7472 692e 6469 706f  terZ.tantri.dipo
-000013e0: 6c65 7372 4900 0000 5a19 7461 6e74 7269  lesrI...Z.tantri
-000013f0: 2e64 6970 6f6c 6573 2e67 656e 6572 6174  .dipoles.generat
-00001400: 696f 6eda 0770 6174 686c 6962 723c 0000  ion..pathlibr<..
-00001410: 0072 0c00 0000 da08 5f5f 6e61 6d65 5f5f  .r......__name__
-00001420: 7230 0000 0072 0b00 0000 7233 0000 0072  r0...r....r3...r
-00001430: 3500 0000 7213 0000 00da 0567 726f 7570  5...r......group
-00001440: da06 6f70 7469 6f6e 5a0e 7665 7273 696f  ..optionZ.versio
-00001450: 6e5f 6f70 7469 6f6e da0b 6765 745f 7665  n_option..get_ve
-00001460: 7273 696f 6e72 1800 0000 da07 636f 6d6d  rsionr......comm
-00001470: 616e 64da 0450 6174 685a 0643 686f 6963  and..PathZ.Choic
-00001480: 65da 0566 6c6f 6174 da03 696e 74da 0446  e..float..int..F
-00001490: 696c 6572 4200 0000 da08 6172 6775 6d65  ilerB.....argume
-000014a0: 6e74 7251 0000 0072 1100 0000 7211 0000  ntrQ...r....r...
-000014b0: 0072 1100 0000 7212 0000 00da 083c 6d6f  .r....r......<mo
-000014c0: 6475 6c65 3e01 0000 0073 b200 0000 0801  dule>....s......
-000014d0: 0801 0801 0801 0801 0801 0801 0801 0801  ................
-000014e0: 0801 0802 0a02 0403 0401 0403 080d 0601  ................
-000014f0: 0401 08ff 0403 0c01 0c01 1007 0601 0401  ................
-00001500: 0201 0201 0201 0e01 02fb 0407 0401 0201  ................
-00001510: 0201 0201 0e01 02fb 0407 0401 0201 0c01  ................
-00001520: 0201 0201 02fb 0407 0401 0201 0201 0201  ................
-00001530: 0201 0201 02fa 0408 0401 0201 0201 0201  ................
-00001540: 0201 0201 02fa 0408 0401 0201 0201 0201  ................
-00001550: 0201 02fb 0407 0401 0201 0201 0801 0201  ................
-00001560: 02fb 0407 0e01 1a35 0601 0401 0201 0efe  .......5........
-00001570: 0404 0401 0201 08fe 0404 0401 06ff 0403  ................
+00000060: 6401 6c06 5a06 6400 6401 6c07 5a02 6400  d.l.Z.d.d.l.Z.d.
+00000070: 6401 6c08 5a08 6501 a009 650a a101 5a0b  d.l.Z.e...e...Z.
+00000080: 6402 5a0c 6403 5a0d 6404 5a0e 6405 6406  d.Z.d.Z.d.Z.d.d.
+00000090: 8400 5a0f 6500 a010 a100 6500 6a11 6407  ..Z.e.....e.j.d.
+000000a0: 6408 6409 640a 640b 8d04 6500 6a11 640c  d.d.d.d...e.j.d.
+000000b0: 640d 640e 8d02 6500 a012 6502 a013 a100  d.d...e...e.....
+000000c0: a101 640f 6410 8400 8301 8301 8301 8301  ..d.d...........
+000000d0: 5a14 6514 a015 a100 6500 6a11 6411 6412  Z.e.....e.j.d.d.
+000000e0: 6409 6500 6a16 6409 6508 6a16 6413 8d02  d.e.j.d.e.j.d...
+000000f0: 6414 6415 8d05 6500 6a11 6416 6417 6409  d.d...e.j.d.d.d.
+00000100: 6500 6a16 6409 6508 6a16 6413 8d02 6418  e.j.d.e.j.d...d.
+00000110: 6415 8d05 6500 6a11 6419 6500 a017 650d  d...e.j.d.e...e.
+00000120: 650e 6702 a101 650d 641a 6409 641b 8d05  e.g...e.d.d.d...
+00000130: 6500 6a11 641c 641d 6518 641e 641f 6409  e.j.d.d.e.d.d.d.
+00000140: 641b 8d06 6500 6a11 6420 6421 6519 6422  d...e.j.d d!e.d"
+00000150: 6423 6409 641b 8d06 6500 6a11 6424 6425  d#d.d...e.j.d$d%
+00000160: 6519 6401 6426 6427 8d05 6500 6a11 6428  e.d.d&d'..e.j.d(
+00000170: 6429 6500 6a16 6508 6a16 642a 8d01 642b  d)e.j.e.j.d*..d+
+00000180: 6409 642c 8d05 6500 6a11 642d 640a 642e  d.d,..e.j.d-d.d.
+00000190: 642f 8d03 6430 6431 8400 8301 8301 8301  d/..d0d1........
+000001a0: 8301 8301 8301 8301 8301 8301 5a1a 6432  ............Z.d2
+000001b0: 6433 8400 5a1b 6514 a015 a100 6500 6a1c  d3..Z.e.....e.j.
+000001c0: 6434 6500 6a16 6409 6508 6a16 6413 8d02  d4e.j.d.e.j.d...
+000001d0: 6435 8d02 6500 6a1c 6428 6500 6a16 6508  d5..e.j.d(e.j.e.
+000001e0: 6a16 642a 8d01 6435 8d02 6500 6a11 6436  j.d*..d5..e.j.d6
+000001f0: 6519 6437 6438 8d03 6439 643a 8400 8301  e.d7d8..d9d:....
+00000200: 8301 8301 8301 5a1d 643b 643c 8400 5a1e  ......Z.d;d<..Z.
+00000210: 6401 5300 293d e900 0000 004e 7a36 2528  d.S.)=.....Nz6%(
+00000220: 6173 6374 696d 6529 7320 7c20 2528 6c65  asctime)s | %(le
+00000230: 7665 6c6e 616d 6529 2d37 7320 7c20 2528  velname)-7s | %(
+00000240: 6e61 6d65 2973 207c 2025 286d 6573 7361  name)s | %(messa
+00000250: 6765 2973 7a12 656c 6563 7472 6963 2d70  ge)sz.electric-p
+00000260: 6f74 656e 7469 616c 7a10 782d 656c 6563  otentialz.x-elec
+00000270: 7472 6963 2d66 6965 6c64 6301 0000 0000  tric-fieldc.....
+00000280: 0000 0000 0000 0002 0000 0005 0000 0043  ...............C
+00000290: 0000 0073 5400 0000 7400 a001 a100 6701  ...sT...t.....g.
+000002a0: 7d01 7c00 6400 7501 7222 7c01 a002 7400  }.|.d.u.r"|...t.
+000002b0: a003 7c00 a101 a101 0100 7400 6a04 7400  ..|.......t.j.t.
+000002c0: 6a05 7406 7c01 6401 8d03 0100 7400 a007  j.t.|.d.....t...
+000002d0: 6402 a101 a008 7400 6a09 a101 0100 7400  d.....t.j.....t.
+000002e0: a00a 6403 a101 0100 6400 5300 2904 4e29  ..d.....d.S.).N)
+000002f0: 03da 056c 6576 656c da06 666f 726d 6174  ...level..format
+00000300: da08 6861 6e64 6c65 7273 5a04 7064 6d65  ..handlersZ.pdme
+00000310: 5429 0bda 076c 6f67 6769 6e67 da0d 5374  T)...logging..St
+00000320: 7265 616d 4861 6e64 6c65 72da 0661 7070  reamHandler..app
+00000330: 656e 64da 0b46 696c 6548 616e 646c 6572  end..FileHandler
+00000340: da0b 6261 7369 6343 6f6e 6669 67da 0544  ..basicConfig..D
+00000350: 4542 5547 da0b 4c4f 475f 5041 5454 4552  EBUG..LOG_PATTER
+00000360: 4eda 0967 6574 4c6f 6767 6572 da08 7365  N..getLogger..se
+00000370: 744c 6576 656c da04 494e 464f da0f 6361  tLevel..INFO..ca
+00000380: 7074 7572 6557 6172 6e69 6e67 7329 02da  ptureWarnings)..
+00000390: 0866 696c 656e 616d 6572 0400 0000 a900  .filenamer......
+000003a0: 7211 0000 00fa 4f2f 686f 6d65 2f6a 656e  r.....O/home/jen
+000003b0: 6b69 6e73 2f61 6765 6e74 2f77 6f72 6b73  kins/agent/works
+000003c0: 7061 6365 2f67 6974 6561 2d70 6879 7369  pace/gitea-physi
+000003d0: 6373 5f74 616e 7472 695f 312e 312e 302f  cs_tantri_1.1.0/
+000003e0: 7461 6e74 7269 2f63 6c69 2f5f 5f69 6e69  tantri/cli/__ini
+000003f0: 745f 5f2e 7079 da0f 5f73 6574 5f75 705f  t__.py.._set_up_
+00000400: 6c6f 6767 696e 6715 0000 0073 1400 0000  logging....s....
+00000410: 0001 0a01 0801 1001 0401 0401 0201 02fd  ................
+00000420: 0605 1201 7213 0000 007a 052d 2d6c 6f67  ....r....z.--log
+00000430: 7a1d 456e 6162 6c65 206c 6f67 6769 6e67  z.Enable logging
+00000440: 2074 6f20 7374 7265 616d 206f 6e6c 7954   to stream onlyT
+00000450: 4629 03da 0468 656c 705a 0769 735f 666c  F)...helpZ.is_fl
+00000460: 6167 da07 6465 6661 756c 747a 0a2d 2d6c  ag..defaultz.--l
+00000470: 6f67 2d66 696c 657a 2d41 2066 696c 656e  og-filez-A filen
+00000480: 616d 6520 746f 2075 7365 2066 6f72 206c  ame to use for l
+00000490: 6f67 6769 6e67 2028 696d 706c 6965 7320  ogging (implies 
+000004a0: 2d2d 6c6f 6729 2901 7214 0000 0063 0200  --log)).r....c..
+000004b0: 0000 0000 0000 0000 0000 0200 0000 0200  ................
+000004c0: 0000 4300 0000 7318 0000 007c 0073 0c7c  ..C...s....|.s.|
+000004d0: 0164 0175 0172 1474 007c 0183 0101 0064  .d.u.r.t.|.....d
+000004e0: 0153 0029 027a 3855 7469 6c69 7469 6573  .S.).z8Utilities
+000004f0: 2066 6f72 2067 656e 6572 6174 696e 6720   for generating 
+00000500: 7369 6d75 6c61 7465 6420 544c 5320 7469  simulated TLS ti
+00000510: 6d65 2073 6572 6965 7320 6461 7461 2e4e  me series data.N
+00000520: 2901 7213 0000 0029 02da 036c 6f67 da08  ).r....)...log..
+00000530: 6c6f 675f 6669 6c65 7211 0000 0072 1100  log_filer....r..
+00000540: 0000 7212 0000 00da 0363 6c69 2200 0000  ..r......cli"...
+00000550: 7304 0000 0000 080c 0272 1800 0000 7a0e  s........r....z.
+00000560: 2d2d 6469 706f 6c65 732d 6669 6c65 7a0c  --dipoles-filez.
+00000570: 6469 706f 6c65 732e 6a73 6f6e 2902 da06  dipoles.json)...
+00000580: 6578 6973 7473 da09 7061 7468 5f74 7970  exists..path_typ
+00000590: 657a 1f46 696c 6520 7769 7468 206a 736f  ez.File with jso
+000005a0: 6e20 6172 7261 7920 6f66 2064 6970 6f6c  n array of dipol
+000005b0: 6573 2904 7215 0000 00da 0c73 686f 775f  es).r......show_
+000005c0: 6465 6661 756c 74da 0474 7970 6572 1400  default..typer..
+000005d0: 0000 7a0b 2d2d 646f 7473 2d66 696c 657a  ..z.--dots-filez
+000005e0: 0964 6f74 732e 6a73 6f6e 7a1c 4669 6c65  .dots.jsonz.File
+000005f0: 2077 6974 6820 6a73 6f6e 2061 7272 6179   with json array
+00000600: 206f 6620 646f 7473 7a12 2d2d 6d65 6173   of dotsz.--meas
+00000610: 7572 656d 656e 742d 7479 7065 7a23 5468  urement-typez#Th
+00000620: 6520 7479 7065 206f 6620 6d65 6173 7572  e type of measur
+00000630: 656d 656e 7420 746f 2073 696d 756c 6174  ement to simulat
+00000640: 6529 0472 1c00 0000 7215 0000 0072 1400  e).r....r....r..
+00000650: 0000 721b 0000 007a 092d 2d64 656c 7461  ..r....z.--delta
+00000660: 2d74 7a02 2d74 e901 0000 007a 2b54 6865  -tz.-t.....z+The
+00000670: 2064 656c 7461 2074 2062 6574 7765 656e   delta t between
+00000680: 2074 696d 6520 7365 7269 6573 2069 7465   time series ite
+00000690: 7261 7469 6f6e 732e 7a10 2d2d 6e75 6d2d  rations.z.--num-
+000006a0: 6974 6572 6174 696f 6e73 7a02 2d6e e90a  iterationsz.-n..
+000006b0: 0000 007a 1954 6865 206e 756d 6265 7220  ...z.The number 
+000006c0: 6f66 2069 7465 7261 7469 6f6e 732e 7a16  of iterations.z.
+000006d0: 2d2d 7469 6d65 2d73 6572 6965 732d 726e  --time-series-rn
+000006e0: 672d 7365 6564 7a02 2d73 7a45 4120 7365  g-seedz.-szEA se
+000006f0: 6564 2074 6f20 7573 6520 746f 2063 7265  ed to use to cre
+00000700: 6174 6520 616e 206f 7665 7272 6964 6520  ate an override 
+00000710: 6465 6661 756c 7420 726e 672e 2059 6f75  default rng. You
+00000720: 2073 686f 756c 6420 7365 7420 7468 6973   should set this
+00000730: 2e29 0372 1c00 0000 7215 0000 0072 1400  .).r....r....r..
+00000740: 0000 da0b 6f75 7470 7574 5f66 696c 657a  ....output_filez
+00000750: 022d 6f29 0172 1a00 0000 7a27 5468 6520  .-o).r....z'The 
+00000760: 6f75 7470 7574 2066 696c 6520 746f 2077  output file to w
+00000770: 7269 7465 2c20 696e 2063 7376 2066 6f72  rite, in csv for
+00000780: 6d61 7429 0372 1c00 0000 7214 0000 00da  mat).r....r.....
+00000790: 0872 6571 7569 7265 647a 1c2d 2d68 6561  .requiredz.--hea
+000007a0: 6465 722d 726f 772f 2d2d 6e6f 2d68 6561  der-row/--no-hea
+000007b0: 6465 722d 726f 777a 1257 7269 7465 2061  der-rowz.Write a
+000007c0: 2068 6561 6465 7220 726f 7729 0272 1500   header row).r..
+000007d0: 0000 7214 0000 0063 0800 0000 0000 0000  ..r....c........
+000007e0: 0000 0000 0800 0000 0900 0000 4300 0000  ............C...
+000007f0: 731a 0000 0074 007c 007c 017c 027c 037c  s....t.|.|.|.|.|
+00000800: 047c 057c 067c 0783 0801 0064 0153 0029  .|.|.|.....d.S.)
+00000810: 027a 380a 0947 656e 6572 6174 6520 6120  .z8..Generate a 
+00000820: 7469 6d65 2073 6572 6965 7320 666f 7220  time series for 
+00000830: 7468 6520 7061 7373 6564 2069 6e20 7061  the passed in pa
+00000840: 7261 6d65 7465 7273 2e0a 094e 2901 da12  rameters...N)...
+00000850: 5f77 7269 7465 5f74 696d 655f 7365 7269  _write_time_seri
+00000860: 6573 2908 da0c 6469 706f 6c65 735f 6669  es)...dipoles_fi
+00000870: 6c65 da09 646f 7473 5f66 696c 65da 106d  le..dots_file..m
+00000880: 6561 7375 7265 6d65 6e74 5f74 7970 65da  easurement_type.
+00000890: 0764 656c 7461 5f74 da0e 6e75 6d5f 6974  .delta_t..num_it
+000008a0: 6572 6174 696f 6e73 da14 7469 6d65 5f73  erations..time_s
+000008b0: 6572 6965 735f 726e 675f 7365 6564 721f  eries_rng_seedr.
+000008c0: 0000 00da 0a68 6561 6465 725f 726f 7772  .....header_rowr
+000008d0: 1100 0000 7211 0000 0072 1200 0000 da11  ....r....r......
+000008e0: 7772 6974 655f 7469 6d65 5f73 6572 6965  write_time_serie
+000008f0: 732f 0000 0073 1400 0000 0042 0201 0201  s/...s.....B....
+00000900: 0201 0201 0201 0201 0201 0201 02f8 7229  ..............r)
+00000910: 0000 0063 0800 0000 0000 0000 0000 0000  ...c............
+00000920: 1200 0000 0800 0000 0300 0000 738c 0100  ............s...
+00000930: 0074 00a0 0164 017c 009b 0064 027c 019b  .t...d.|...d.|..
+00000940: 0064 039d 05a1 0101 0074 026a 036a 04a0  .d.......t.j.j..
+00000950: 057c 00a1 017d 0874 026a 036a 04a0 067c  .|...}.t.j.j...|
+00000960: 01a1 017d 097c 0274 076b 0272 4c74 026a  ...}.|.t.k.rLt.j
+00000970: 086a 096a 0a7d 0a64 0489 016e 167c 0274  .j.j.}.d...n.|.t
+00000980: 0b6b 0272 6274 026a 086a 096a 0b7d 0a64  .k.rbt.j.j.j.}.d
+00000990: 0589 0174 00a0 0164 067c 0a6a 0c9b 009d  ...t...d.|.j....
+000009a0: 02a1 0101 0064 0764 0884 007c 0944 0083  .....d.d...|.D..
+000009b0: 017d 0b7c 06a0 0d64 09a1 018f ea7d 0c7c  .}.|...d.....}.|
+000009c0: 0772 bc64 0aa0 0e87 0166 0164 0b64 0884  .r.d.....f.d.d..
+000009d0: 087c 0b44 0083 01a1 017d 0d7c 0ca0 0f64  .|.D.....}.|...d
+000009e0: 0c7c 0d9b 0064 0d9d 03a1 0101 0074 00a0  .|...d.......t..
+000009f0: 0164 0e7c 049b 0064 0f7c 039b 009d 04a1  .d.|...d.|......
+00000a00: 0101 0074 00a0 0164 107c 059b 009d 02a1  ...t...d.|......
+00000a10: 0101 007c 0564 0075 0072 fe74 026a 08a0  ...|.d.u.r.t.j..
+00000a20: 107c 087c 097c 0a7c 03a1 047d 0e6e 2074  .|.|.|.|...}.n t
+00000a30: 116a 12a0 137c 05a1 017d 0f74 026a 08a0  .j...|...}.t.j..
+00000a40: 107c 087c 097c 0a7c 037c 0fa1 057d 0e74  .|.|.|.|.|...}.t
+00000a50: 147c 0483 0144 005d 407d 107c 0ea0 15a1  .|...D.]@}.|....
+00000a60: 0089 0064 0aa0 0e87 0066 0164 1164 1284  ...d.....f.d.d..
+00000a70: 087c 0b44 0083 01a1 017d 117c 0ca0 0f7c  .|.D.....}.|...|
+00000a80: 107c 0314 009b 0064 0a7c 119b 0064 0d9d  .|.....d.|...d..
+00000a90: 04a1 0101 0090 0171 2657 0064 0004 0004  .......q&W.d....
+00000aa0: 0083 0301 006e 1231 0090 0173 7e30 0001  .....n.1...s~0..
+00000ab0: 0001 0001 0059 0001 0064 0053 0029 134e  .....Y...d.S.).N
+00000ac0: 7a23 5265 6365 6976 6564 2070 6172 616d  z#Received param
+00000ad0: 6574 6572 7320 5b64 6970 6f6c 6573 5f66  eters [dipoles_f
+00000ae0: 696c 653a 207a 125d 2061 6e64 205b 646f  ile: z.] and [do
+00000af0: 7473 5f66 696c 653a 20da 015d da01 565a  ts_file: ..]..VZ
+00000b00: 0245 787a 1255 7369 6e67 206d 6561 7375  .Exz.Using measu
+00000b10: 7265 6d65 6e74 2063 0100 0000 0000 0000  rement c........
+00000b20: 0000 0000 0200 0000 0300 0000 5300 0000  ............S...
+00000b30: 7312 0000 0067 007c 005d 0a7d 017c 016a  s....g.|.].}.|.j
+00000b40: 0091 0271 0453 0072 1100 0000 2901 da05  ...q.S.r....)...
+00000b50: 6c61 6265 6c29 02da 022e 30da 0364 6f74  label)....0..dot
+00000b60: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
+00000b70: 0a3c 6c69 7374 636f 6d70 3e95 0000 00f3  .<listcomp>.....
+00000b80: 0000 0000 7a26 5f77 7269 7465 5f74 696d  ....z&_write_tim
+00000b90: 655f 7365 7269 6573 2e3c 6c6f 6361 6c73  e_series.<locals
+00000ba0: 3e2e 3c6c 6973 7463 6f6d 703e da01 777a  >.<listcomp>..wz
+00000bb0: 022c 2063 0100 0000 0000 0000 0000 0000  ., c............
+00000bc0: 0200 0000 0500 0000 1300 0000 731a 0000  ............s...
+00000bd0: 0067 007c 005d 127d 0188 009b 0064 007c  .g.|.].}.....d.|
+00000be0: 019b 009d 0391 0271 0453 0029 01da 015f  .......q.S.)..._
+00000bf0: 7211 0000 00a9 0272 2d00 0000 722c 0000  r......r-...r,..
+00000c00: 0029 01da 0a76 616c 7565 5f6e 616d 6572  .)...value_namer
+00000c10: 1100 0000 7212 0000 0072 2f00 0000 9800  ....r....r/.....
+00000c20: 0000 7230 0000 007a 0774 2028 7329 2c20  ..r0...z.t (s), 
+00000c30: da01 0a7a 1247 6f69 6e67 2074 6f20 7369  ...z.Going to si
+00000c40: 6d75 6c61 7465 207a 1e20 6974 6572 6174  mulate z. iterat
+00000c50: 696f 6e73 2077 6974 6820 6120 6465 6c74  ions with a delt
+00000c60: 6120 7420 6f66 207a 0947 6f74 2073 6565  a t of z.Got see
+00000c70: 6420 6301 0000 0000 0000 0000 0000 0002  d c.............
+00000c80: 0000 0004 0000 0033 0000 0073 1a00 0000  .......3...s....
+00000c90: 7c00 5d12 7d01 7400 8800 7c01 1900 8301  |.].}.t...|.....
+00000ca0: 5600 0100 7102 6400 5300 a901 4e29 01da  V...q.d.S...N)..
+00000cb0: 0373 7472 7233 0000 0029 01da 0a74 7261  .strr3...)...tra
+00000cc0: 6e73 6974 696f 6e72 1100 0000 7212 0000  nsitionr....r...
+00000cd0: 00da 093c 6765 6e65 7870 723e ac00 0000  ...<genexpr>....
+00000ce0: 7230 0000 007a 255f 7772 6974 655f 7469  r0...z%_write_ti
+00000cf0: 6d65 5f73 6572 6965 732e 3c6c 6f63 616c  me_series.<local
+00000d00: 733e 2e3c 6765 6e65 7870 723e 2916 da07  s>.<genexpr>)...
+00000d10: 5f6c 6f67 6765 72da 0564 6562 7567 da06  _logger..debug..
+00000d20: 7461 6e74 7269 7218 0000 005a 0d66 696c  tantrir....Z.fil
+00000d30: 655f 696d 706f 7274 6572 5a16 7265 6164  e_importerZ.read
+00000d40: 5f64 6970 6f6c 6573 5f6a 736f 6e5f 6669  _dipoles_json_fi
+00000d50: 6c65 5a13 7265 6164 5f64 6f74 735f 6a73  leZ.read_dots_js
+00000d60: 6f6e 5f66 696c 65da 0950 4f54 454e 5449  on_file..POTENTI
+00000d70: 414c da07 6469 706f 6c65 735a 1544 6970  AL..dipolesZ.Dip
+00000d80: 6f6c 654d 6561 7375 7265 6d65 6e74 5479  oleMeasurementTy
+00000d90: 7065 5a12 454c 4543 5452 4943 5f50 4f54  peZ.ELECTRIC_POT
+00000da0: 454e 5449 414c da10 585f 454c 4543 5452  ENTIAL..X_ELECTR
+00000db0: 4943 5f46 4945 4c44 da04 6e61 6d65 da04  IC_FIELD..name..
+00000dc0: 6f70 656e da04 6a6f 696e da05 7772 6974  open..join..writ
+00000dd0: 655a 1044 6970 6f6c 6554 696d 6553 6572  eZ.DipoleTimeSer
+00000de0: 6965 73da 056e 756d 7079 da06 7261 6e64  ies..numpy..rand
+00000df0: 6f6d da0b 6465 6661 756c 745f 726e 67da  om..default_rng.
+00000e00: 0572 616e 6765 7238 0000 0029 1272 2200  .ranger8...).r".
+00000e10: 0000 7223 0000 0072 2400 0000 7225 0000  ..r#...r$...r%..
+00000e20: 0072 2600 0000 7227 0000 0072 1f00 0000  .r&...r'...r....
+00000e30: 7228 0000 0072 3e00 0000 da04 646f 7473  r(...r>.....dots
+00000e40: 5a10 6d65 6173 7572 656d 656e 745f 656e  Z.measurement_en
+00000e50: 756d da06 6c61 6265 6c73 da03 6f75 745a  um..labels..outZ
+00000e60: 0c76 616c 7565 5f6c 6162 656c 735a 0b74  .value_labelsZ.t
+00000e70: 696d 655f 7365 7269 6573 da03 726e 67da  ime_series..rng.
+00000e80: 0169 5a11 7472 616e 7369 7469 6f6e 5f76  .iZ.transition_v
+00000e90: 616c 7565 7372 1100 0000 2902 7238 0000  aluesr....).r8..
+00000ea0: 0072 3400 0000 7212 0000 0072 2100 0000  .r4...r....r!...
+00000eb0: 7d00 0000 7342 0000 0000 0a04 0110 ff04  }...sB..........
+00000ec0: 030e 010e 0208 010a 0106 0108 010a 0104  ................
+00000ed0: 0212 010e 010c 0104 0118 0112 0204 010e  ................
+00000ee0: ff04 0410 0108 0106 0108 ff06 040c 0106  ................
+00000ef0: 010a ff04 040c 0108 0118 0172 2100 0000  ...........r!...
+00000f00: da11 6765 6e65 7261 7469 6f6e 5f63 6f6e  ..generation_con
+00000f10: 6669 6729 0172 1c00 0000 7a13 2d2d 6f76  fig).r....z.--ov
+00000f20: 6572 7269 6465 2d72 6e67 2d73 6565 647a  erride-rng-seedz
+00000f30: 2c53 6565 6420 746f 206f 7665 7272 6964  ,Seed to overrid
+00000f40: 6520 7468 6520 6765 6e65 7261 7469 6f6e  e the generation
+00000f50: 2063 6f6e 6669 6720 7370 6563 2e29 0272   config spec.).r
+00000f60: 1c00 0000 7214 0000 0063 0300 0000 0000  ....r....c......
+00000f70: 0000 0000 0000 0300 0000 0400 0000 4300  ..............C.
+00000f80: 0000 7310 0000 0074 007c 007c 017c 0283  ..s....t.|.|.|..
+00000f90: 0301 0064 0053 0072 3600 0000 2901 da11  ...d.S.r6...)...
+00000fa0: 5f67 656e 6572 6174 655f 6469 706f 6c65  _generate_dipole
+00000fb0: 7329 0372 4d00 0000 721f 0000 00da 116f  s).rM...r......o
+00000fc0: 7665 7272 6964 655f 726e 675f 7365 6564  verride_rng_seed
+00000fd0: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
+00000fe0: 1067 656e 6572 6174 655f 6469 706f 6c65  .generate_dipole
+00000ff0: 73b0 0000 0073 0200 0000 000d 7250 0000  s....s......rP..
+00001000: 0063 0300 0000 0000 0000 0000 0000 0900  .c..............
+00001010: 0000 0800 0000 4300 0000 730a 0100 0074  ......C...s....t
+00001020: 00a0 0164 0174 02a0 037c 00a1 019b 009d  ...d.t...|......
+00001030: 02a1 0101 0074 00a0 0164 027c 029b 0064  .....t...d.|...d
+00001040: 039d 03a1 0101 0074 047c 0064 0483 028f  .......t.|.d....
+00001050: 1a7d 0374 05a0 067c 03a1 017d 0457 0064  .}.t...|...}.W.d
+00001060: 0504 0004 0083 0301 006e 1031 0073 5230  .........n.1.sR0
+00001070: 0001 0001 0001 0059 0001 0074 076a 086a  .......Y...t.j.j
+00001080: 0966 0069 007c 04a4 018e 017d 0564 057d  .f.i.|.....}.d.}
+00001090: 067c 0264 0575 0172 9674 00a0 0a64 067c  .|.d.u.r.t...d.|
+000010a0: 029b 009d 02a1 0101 0074 0b6a 0ca0 0d7c  .........t.j...|
+000010b0: 02a1 017d 0674 00a0 0164 077c 059b 0064  ...}.t...d.|...d
+000010c0: 089d 03a1 0101 0074 076a 08a0 0e7c 057c  .......t.j...|.|
+000010d0: 06a1 027d 077c 01a0 0464 09a1 018f 367d  ...}.|...d....6}
+000010e0: 087c 08a0 0f74 056a 1064 0a64 0b84 007c  .|...t.j.d.d...|
+000010f0: 0744 0083 0174 076a 116a 126a 136a 1464  .D...t.j.j.j.j.d
+00001100: 0c8d 02a1 0101 0057 0064 0504 0004 0083  .......W.d......
+00001110: 0301 006e 1031 0073 fc30 0001 0001 0001  ...n.1.s.0......
+00001120: 0059 0001 0064 0553 0029 0d61 5a01 0000  .Y...d.S.).aZ...
+00001130: 4765 6e65 7261 7465 2072 616e 646f 6d20  Generate random 
+00001140: 6469 706f 6c65 7320 6173 2064 6573 6372  dipoles as descr
+00001150: 6962 6564 2062 7920 4745 4e45 5241 5449  ibed by GENERATI
+00001160: 4f4e 5f43 4f4e 4649 4720 616e 6420 6f75  ON_CONFIG and ou
+00001170: 7470 7574 2074 6f20 4f55 5450 5554 5f46  tput to OUTPUT_F
+00001180: 494c 452e 0a0a 0947 454e 4552 4154 494f  ILE....GENERATIO
+00001190: 4e5f 434f 4e46 4947 2073 686f 756c 6420  N_CONFIG should 
+000011a0: 6265 2061 204a 534f 4e20 6669 6c65 2074  be a JSON file t
+000011b0: 6861 7420 6d61 7463 6865 7320 7468 6520  hat matches the 
+000011c0: 6170 7072 6f70 7269 6174 6520 7370 6563  appropriate spec
+000011d0: 2c20 616e 6420 4f55 5450 5554 5f46 494c  , and OUTPUT_FIL
+000011e0: 4520 7769 6c6c 2063 6f6e 7461 696e 204a  E will contain J
+000011f0: 534f 4e20 666f 726d 6174 7465 6420 636f  SON formatted co
+00001200: 6e74 656e 7473 2e0a 094f 5554 5055 545f  ntents...OUTPUT_
+00001210: 4649 4c45 2077 696c 6c20 6265 206f 7665  FILE will be ove
+00001220: 7277 7269 7474 656e 2c20 6966 2069 7420  rwritten, if it 
+00001230: 6578 6973 7473 2e0a 0a09 4966 2074 6865  exists....If the
+00001240: 202d 2d6f 7665 7272 6964 652d 726e 672d   --override-rng-
+00001250: 7365 6564 2069 7320 7365 742c 2069 7427  seed is set, it'
+00001260: 7320 6265 7474 6572 2074 6f20 6b65 6570  s better to keep
+00001270: 206c 6f67 7320 6f66 2074 6865 2067 656e   logs of the gen
+00001280: 6572 6174 696f 6e21 0a09 7a2e 6765 6e65  eration!..z.gene
+00001290: 7261 7465 5f64 6970 6f6c 6573 2077 6173  rate_dipoles was
+000012a0: 2063 616c 6c65 642c 2077 6974 6820 636f   called, with co
+000012b0: 6e66 6967 2066 696c 6520 7a14 6f76 6572  nfig file z.over
+000012c0: 7269 6465 5f72 6e67 5f73 6565 643a 205b  ride_rng_seed: [
+000012d0: 722a 0000 00da 0172 4e7a 2c4f 7665 7272  r*.....rNz,Overr
+000012e0: 6964 696e 6720 7468 6520 726e 6720 7769  iding the rng wi
+000012f0: 7468 2061 206e 6577 206f 6e65 2077 6974  th a new one wit
+00001300: 6820 7365 6564 207a 1f67 656e 6572 6174  h seed z.generat
+00001310: 696e 6720 6469 706f 6c65 7320 7769 7468  ing dipoles with
+00001320: 2063 6f6e 6669 6720 7a03 2e2e 2e72 3100   config z....r1.
+00001330: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
+00001340: 0000 0004 0000 0053 0000 0073 1400 0000  .......S...s....
+00001350: 6700 7c00 5d0c 7d01 7c01 a000 a100 9102  g.|.].}.|.......
+00001360: 7104 5300 7211 0000 0029 015a 0761 735f  q.S.r....).Z.as_
+00001370: 6469 6374 2902 722d 0000 00da 0167 7211  dict).r-.....gr.
+00001380: 0000 0072 1100 0000 7212 0000 0072 2f00  ...r....r....r/.
+00001390: 0000 db00 0000 7230 0000 007a 255f 6765  ......r0...z%_ge
+000013a0: 6e65 7261 7465 5f64 6970 6f6c 6573 2e3c  nerate_dipoles.<
+000013b0: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+000013c0: 703e 2901 da03 636c 7329 1572 3a00 0000  p>)...cls).r:...
+000013d0: 723b 0000 00da 0563 6c69 636b 5a0f 666f  r;.....clickZ.fo
+000013e0: 726d 6174 5f66 696c 656e 616d 6572 4100  rmat_filenamerA.
+000013f0: 0000 da04 6a73 6f6e da04 6c6f 6164 723c  ....json..loadr<
+00001400: 0000 0072 3e00 0000 5a16 4469 706f 6c65  ...r>...Z.Dipole
+00001410: 4765 6e65 7261 7469 6f6e 436f 6e66 6967  GenerationConfig
+00001420: da04 696e 666f 7244 0000 0072 4500 0000  ..inforD...rE...
+00001430: 7246 0000 005a 0c6d 616b 655f 6469 706f  rF...Z.make_dipo
+00001440: 6c65 7372 4300 0000 da05 6475 6d70 7372  lesrC.....dumpsr
+00001450: 1800 0000 da0b 696e 7075 745f 6669 6c65  ......input_file
+00001460: 735a 0d77 7269 7465 5f64 6970 6f6c 6573  sZ.write_dipoles
+00001470: 5a0c 4e75 6d70 7945 6e63 6f64 6572 2909  Z.NumpyEncoder).
+00001480: 724d 0000 0072 1f00 0000 724f 0000 00da  rM...r....rO....
+00001490: 0b63 6f6e 6669 675f 6669 6c65 da04 6461  .config_file..da
+000014a0: 7461 da06 636f 6e66 6967 5a0c 6f76 6572  ta..configZ.over
+000014b0: 7269 6465 5f72 6e67 5a09 6765 6e65 7261  ride_rngZ.genera
+000014c0: 7465 6472 4a00 0000 7211 0000 0072 1100  tedrJ...r....r..
+000014d0: 0000 7212 0000 0072 4e00 0000 c000 0000  ..r....rN.......
+000014e0: 7328 0000 0000 0804 010e ff04 0312 020c  s(..............
+000014f0: 0128 0112 0204 0108 0110 010c 0112 010e  .(..............
+00001500: 020c 0104 0104 010c 010a fe04 ff72 4e00  .............rN.
+00001510: 0000 291f 7254 0000 0072 0500 0000 723c  ..).rT...r....r<
+00001520: 0000 0072 4400 0000 5a24 7461 6e74 7269  ...rD...Z$tantri
+00001530: 2e63 6c69 2e69 6e70 7574 5f66 696c 6573  .cli.input_files
+00001540: 2e77 7269 7465 5f64 6970 6f6c 6573 5a18  .write_dipolesZ.
+00001550: 7461 6e74 7269 2e63 6c69 2e66 696c 655f  tantri.cli.file_
+00001560: 696d 706f 7274 6572 7255 0000 005a 0e74  importerrU...Z.t
+00001570: 616e 7472 692e 6469 706f 6c65 73da 0770  antri.dipoles..p
+00001580: 6174 686c 6962 720c 0000 00da 085f 5f6e  athlibr......__n
+00001590: 616d 655f 5f72 3a00 0000 720b 0000 0072  ame__r:...r....r
+000015a0: 3d00 0000 723f 0000 0072 1300 0000 da05  =...r?...r......
+000015b0: 6772 6f75 70da 066f 7074 696f 6e5a 0e76  group..optionZ.v
+000015c0: 6572 7369 6f6e 5f6f 7074 696f 6eda 0b67  ersion_option..g
+000015d0: 6574 5f76 6572 7369 6f6e 7218 0000 00da  et_versionr.....
+000015e0: 0763 6f6d 6d61 6e64 da04 5061 7468 5a06  .command..PathZ.
+000015f0: 4368 6f69 6365 da05 666c 6f61 74da 0369  Choice..float..i
+00001600: 6e74 7229 0000 0072 2100 0000 da08 6172  ntr)...r!.....ar
+00001610: 6775 6d65 6e74 7250 0000 0072 4e00 0000  gumentrP...rN...
+00001620: 7211 0000 0072 1100 0000 7211 0000 0072  r....r....r....r
+00001630: 1200 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00001640: 0000 73b2 0000 0008 0108 0108 0108 0108  ..s.............
+00001650: 0108 0108 0108 0108 030a 0204 0304 0104  ................
+00001660: 0308 0d06 0104 0108 ff04 030c 010c 0110  ................
+00001670: 0706 0104 0102 0102 0102 010e 0102 fb04  ................
+00001680: 0704 0102 0102 0102 010e 0102 fb04 0704  ................
+00001690: 0102 010c 0102 0102 0102 fb04 0704 0102  ................
+000016a0: 0102 0102 0102 0102 0102 fa04 0804 0102  ................
+000016b0: 0102 0102 0102 0102 0102 fa04 0804 0102  ................
+000016c0: 0102 0102 0102 0102 fb04 0704 0102 0102  ................
+000016d0: 010c 0102 0102 fb04 070e 011a 1908 3306  ..............3.
+000016e0: 0104 0102 010e fe04 0404 0102 010c fe04  ................
+000016f0: 0404 0106 ff04 0310 04                   .........
```

### Comparing `tantri-1.0.1/tantri/cli/__pycache__/file_importer.cpython-39.pyc` & `tantri-1.1.0/tantri/cli/__pycache__/file_importer.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 22 20:18:56 2024 UTC, .py size: 904 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 30c6 2666 8803 0000  a.......0.&f....
+00000000: 610d 0d0a 0000 0000 cbe8 3366 8803 0000  a.........3f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 8600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a02 6400 6401 6c03 5a04 6400  d.l.Z.d.d.l.Z.d.
 00000050: 6402 6c05 6d06 5a06 0100 6400 6401 6c07  d.l.m.Z...d.d.l.
 00000060: 5a04 6502 a008 6509 a101 5a0a 6500 6a0b  Z.e...e...Z.e.j.
 00000070: 6403 9c01 6404 6405 8404 5a0c 6500 6a0b  d...d.d...Z.e.j.
@@ -28,15 +28,15 @@
 000001b0: 2906 da04 6f70 656e da04 6a73 6f6e da04  )...open..json..
 000001c0: 6c6f 6164 da09 4578 6365 7074 696f 6eda  load..Exception.
 000001d0: 075f 6c6f 6767 6572 da05 6572 726f 7229  ._logger..error)
 000001e0: 0372 0300 0000 da04 6669 6c65 da01 65a9  .r......file..e.
 000001f0: 0072 0e00 0000 fa54 2f68 6f6d 652f 6a65  .r.....T/home/je
 00000200: 6e6b 696e 732f 6167 656e 742f 776f 726b  nkins/agent/work
 00000210: 7370 6163 652f 6769 7465 612d 7068 7973  space/gitea-phys
-00000220: 6963 735f 7461 6e74 7269 5f31 2e30 2e31  ics_tantri_1.0.1
+00000220: 6963 735f 7461 6e74 7269 5f31 2e31 2e30  ics_tantri_1.1.0
 00000230: 2f74 616e 7472 692f 636c 692f 6669 6c65  /tantri/cli/file
 00000240: 5f69 6d70 6f72 7465 722e 7079 da17 7265  _importer.py..re
 00000250: 6164 5f64 6174 615f 6672 6f6d 5f66 696c  ad_data_from_fil
 00000260: 656e 616d 650f 0000 0073 0e00 0000 0001  ename....s......
 00000270: 0201 0c01 2e01 0e01 0401 0cff 7210 0000  ............r...
 00000280: 0029 0272 0300 0000 da06 7265 7475 726e  .).r......return
 00000290: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
```

### Comparing `tantri-1.0.1/tantri/cli/file_importer.py` & `tantri-1.1.0/tantri/cli/file_importer.py`

 * *Files identical despite different names*

### Comparing `tantri-1.0.1/tantri/cli/input_files/__pycache__/read_dipoles.cpython-39.pyc` & `tantri-1.1.0/tantri/cli/input_files/__pycache__/read_dipoles.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 22 20:18:56 2024 UTC, .py size: 573 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 30c6 2666 3d02 0000  a.......0.&f=...
+00000000: 610d 0d0a 0000 0000 cbe8 3366 3d02 0000  a.........3f=...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4400 0000 6400  .....@...sD...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6504 6503 6403 9c02 6404  m.Z...e.e.d...d.
 00000050: 6405 8404 5a05 6501 6504 1900 6501 6503  d...Z.e.e...e.e.
 00000060: 1900 6406 9c02 6407 6408 8404 5a06 6409  ..d...d.d...Z.d.
 00000070: 5300 290a e900 0000 0029 01da 0853 6571  S.)......)...Seq
@@ -25,15 +25,15 @@
 00000180: 7420 5bda 0177 2903 da03 6c65 6eda 0a56  t [..w)...len..V
 00000190: 616c 7565 4572 726f 7272 0300 0000 2904  alueErrorr....).
 000001a0: 7204 0000 0072 0600 0000 7208 0000 0072  r....r....r....r
 000001b0: 0900 0000 a900 720c 0000 00fa 5f2f 686f  ......r....._/ho
 000001c0: 6d65 2f6a 656e 6b69 6e73 2f61 6765 6e74  me/jenkins/agent
 000001d0: 2f77 6f72 6b73 7061 6365 2f67 6974 6561  /workspace/gitea
 000001e0: 2d70 6879 7369 6373 5f74 616e 7472 695f  -physics_tantri_
-000001f0: 312e 302e 312f 7461 6e74 7269 2f63 6c69  1.0.1/tantri/cli
+000001f0: 312e 312e 302f 7461 6e74 7269 2f63 6c69  1.1.0/tantri/cli
 00000200: 2f69 6e70 7574 5f66 696c 6573 2f72 6561  /input_files/rea
 00000210: 645f 6469 706f 6c65 732e 7079 da0d 726f  d_dipoles.py..ro
 00000220: 775f 746f 5f64 6970 6f6c 6505 0000 0073  w_to_dipole....s
 00000230: 1800 0000 0001 0801 0c01 0201 0aff 0403  ................
 00000240: 0801 0c01 0201 0aff 0403 0802 720e 0000  ............r...
 00000250: 0029 02da 0e64 6f74 5f64 6963 745f 6172  .)...dot_dict_ar
 00000260: 7261 7972 0500 0000 6301 0000 0000 0000  rayr....c.......
```

### Comparing `tantri-1.0.1/tantri/cli/input_files/__pycache__/read_dots.cpython-39.pyc` & `tantri-1.1.0/tantri/cli/input_files/__pycache__/read_dots.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 22 20:18:56 2024 UTC, .py size: 511 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 30c6 2666 ff01 0000  a.......0.&f....
+00000000: 610d 0d0a 0000 0000 cbe8 3366 ff01 0000  a.........3f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 5000 0000 6400  .....@...sP...d.
 00000030: 6401 6c00 5a01 6400 6401 6c02 5a02 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c03 6d04 5a04 0100 6505 6501 6a06  d.l.m.Z...e.e.j.
 00000050: 6a07 6403 9c02 6404 6405 8404 5a08 6504  j.d...d.d...Z.e.
 00000060: 6505 1900 6504 6501 6a06 6a07 1900 6406  e...e.e.j.j...d.
 00000070: 9c02 6407 6408 8404 5a09 6401 5300 2909  ..d.d...Z.d.S.).
@@ -23,15 +23,15 @@
 00000160: 6f72 da06 7461 6e74 7269 da07 6469 706f  or..tantri..dipo
 00000170: 6c65 73da 0b44 6f74 506f 7369 7469 6f6e  les..DotPosition
 00000180: da05 6e75 6d70 79da 0561 7272 6179 2903  ..numpy..array).
 00000190: 7203 0000 0072 0500 0000 7207 0000 00a9  r....r....r.....
 000001a0: 0072 0f00 0000 fa5c 2f68 6f6d 652f 6a65  .r.....\/home/je
 000001b0: 6e6b 696e 732f 6167 656e 742f 776f 726b  nkins/agent/work
 000001c0: 7370 6163 652f 6769 7465 612d 7068 7973  space/gitea-phys
-000001d0: 6963 735f 7461 6e74 7269 5f31 2e30 2e31  ics_tantri_1.0.1
+000001d0: 6963 735f 7461 6e74 7269 5f31 2e31 2e30  ics_tantri_1.1.0
 000001e0: 2f74 616e 7472 692f 636c 692f 696e 7075  /tantri/cli/inpu
 000001f0: 745f 6669 6c65 732f 7265 6164 5f64 6f74  t_files/read_dot
 00000200: 732e 7079 da0a 726f 775f 746f 5f64 6f74  s.py..row_to_dot
 00000210: 0600 0000 730e 0000 0000 0108 010c 0102  ....s...........
 00000220: 010a ff04 0308 0272 1100 0000 2902 da0e  .......r....)...
 00000230: 646f 745f 6469 6374 5f61 7272 6179 7204  dot_dict_arrayr.
 00000240: 0000 0063 0100 0000 0000 0000 0000 0000  ...c............
```

### Comparing `tantri-1.0.1/tantri/cli/input_files/__pycache__/write_dipoles.cpython-39.pyc` & `tantri-1.1.0/tantri/cli/input_files/__pycache__/write_dipoles.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 22 20:18:56 2024 UTC, .py size: 301 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 30c6 2666 2d01 0000  a.......0.&f-...
+00000000: 610d 0d0a 0000 0000 cbe8 3366 2d01 0000  a.........3f-...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 4700  d.l.Z.d.d.l.Z.G.
 00000040: 6402 6403 8400 6403 6501 6a02 8303 5a03  d.d...d.e.j...Z.
 00000050: 6401 5300 2904 e900 0000 004e 6300 0000  d.S.)......Nc...
 00000060: 0000 0000 0000 0000 0000 0000 0002 0000  ................
 00000070: 0040 0000 0073 1800 0000 6500 5a01 6400  .@...s....e.Z.d.
@@ -23,15 +23,15 @@
 00000160: 6461 7272 6179 da06 746f 6c69 7374 da04  darray..tolist..
 00000170: 6a73 6f6e da0b 4a53 4f4e 456e 636f 6465  json..JSONEncode
 00000180: 72da 0764 6566 6175 6c74 2902 da04 7365  r..default)...se
 00000190: 6c66 da03 6f62 6aa9 0072 0c00 0000 fa60  lf..obj..r.....`
 000001a0: 2f68 6f6d 652f 6a65 6e6b 696e 732f 6167  /home/jenkins/ag
 000001b0: 656e 742f 776f 726b 7370 6163 652f 6769  ent/workspace/gi
 000001c0: 7465 612d 7068 7973 6963 735f 7461 6e74  tea-physics_tant
-000001d0: 7269 5f31 2e30 2e31 2f74 616e 7472 692f  ri_1.0.1/tantri/
+000001d0: 7269 5f31 2e31 2e30 2f74 616e 7472 692f  ri_1.1.0/tantri/
 000001e0: 636c 692f 696e 7075 745f 6669 6c65 732f  cli/input_files/
 000001f0: 7772 6974 655f 6469 706f 6c65 732e 7079  write_dipoles.py
 00000200: 7209 0000 000a 0000 0073 0600 0000 0001  r........s......
 00000210: 0c01 0801 7a14 4e75 6d70 7945 6e63 6f64  ....z.NumpyEncod
 00000220: 6572 2e64 6566 6175 6c74 4e29 05da 085f  er.defaultN)..._
 00000230: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
 00000240: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
```

### Comparing `tantri-1.0.1/tantri/cli/input_files/read_dipoles.py` & `tantri-1.1.0/tantri/cli/input_files/read_dipoles.py`

 * *Files identical despite different names*

### Comparing `tantri-1.0.1/tantri/dipoles/__init__.py` & `tantri-1.1.0/tantri/dipoles/time_series.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,13 @@
 from dataclasses import dataclass
 import numpy
 import numpy.random
 import typing
-from enum import Enum
-from tantri.dipoles.types import DipoleTO
-
-import logging
-
-_logger = logging.getLogger(__name__)
-
-
-class DipoleMeasurementType(Enum):
-	ELECTRIC_POTENTIAL = 1
-	X_ELECTRIC_FIELD = 2
-
-
-@dataclass(frozen=True)
-class DotPosition:
-	# assume len 3
-	r: numpy.ndarray
-	label: str
+from tantri.dipoles.types import DipoleTO, DotPosition, DipoleMeasurementType
+import tantri.dipoles.supersample
 
 
 @dataclass
 class WrappedDipole:
 	# assumed len 3
 	p: numpy.ndarray
 	s: numpy.ndarray
@@ -124,27 +108,30 @@
 		if rng_to_use is None:
 			self.rng = numpy.random.default_rng()
 		else:
 			self.rng = rng_to_use
 
 		self.dipoles = get_wrapped_dipoles(dipoles, dots, measurement_type)
 		self.state = 0
-		self.dt = dt
 
-	def transition(self) -> typing.Dict[str, float]:
+		# we may need to supersample, because of how dumb this process is.
+		# let's find our highest frequency
+		max_frequency = max(d.w for d in self.dipoles)
+
+		super_sample = tantri.dipoles.supersample.get_supersample(max_frequency, dt)
+		self.dt = super_sample.super_dt
+		self.super_sample_ratio = super_sample.super_sample_ratio
+
+	def _sub_transition(self) -> typing.Dict[str, float]:
 		new_vals = [dipole.transition(self.dt, self.rng) for dipole in self.dipoles]
 
 		ret = {}
 		for transition in new_vals:
 			for k, v in transition.items():
 				if k not in ret:
 					ret[k] = v
 				else:
 					ret[k] += v
 		return ret
 
-
-__all__ = [
-	"WrappedDipole",
-	"DipoleTimeSeries",
-	"DipoleTO",
-]
+	def transition(self) -> typing.Dict[str, float]:
+		return [self._sub_transition() for i in range(self.super_sample_ratio)][-1]
```

### Comparing `tantri-1.0.1/tantri/dipoles/__pycache__/__init__.cpython-39.pyc` & `tantri-1.1.0/tantri/dipoles/__pycache__/time_series.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 22 20:18:56 2024 UTC, .py size: 3824 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,273 +1,288 @@
-00000000: 610d 0d0a 0000 0000 30c6 2666 f00e 0000  a.......0.&f....
+00000000: 610d 0d0a 0000 0000 cbe8 3366 b80f 0000  a.........3f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0005 0000 0040 0000 0073 c800 0000 6400  .....@...s....d.
+00000020: 0005 0000 0040 0000 0073 8a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a02 6400 6402 6c04  Z.d.d.l.Z.d.d.l.
-00000050: 5a04 6400 6403 6c05 6d06 5a06 0100 6400  Z.d.d.l.m.Z...d.
-00000060: 6404 6c07 6d08 5a08 0100 6400 6402 6c09  d.l.m.Z...d.d.l.
-00000070: 5a09 6509 a00a 650b a101 5a0c 4700 6405  Z.e...e...Z.G.d.
-00000080: 6406 8400 6406 6506 8303 5a0d 6501 6407  d...d.e...Z.e.d.
-00000090: 6408 8d01 4700 6409 640a 8400 640a 8302  d...G.d.d...d...
-000000a0: 8301 5a0e 6501 4700 640b 640c 8400 640c  ..Z.e.G.d.d...d.
-000000b0: 8302 8301 5a0f 6504 6a10 6508 1900 6504  ....Z.e.j.e...e.
-000000c0: 6a10 650e 1900 650d 6504 6a10 650f 1900  j.e...e.e.j.e...
-000000d0: 640d 9c04 640e 640f 8404 5a11 4700 6410  d...d.d...Z.G.d.
-000000e0: 6411 8400 6411 8302 5a12 6700 6412 a201  d...d...Z.g.d...
-000000f0: 5a13 6402 5300 2913 e900 0000 0029 01da  Z.d.S.)......)..
-00000100: 0964 6174 6163 6c61 7373 4e29 01da 0445  .dataclassN)...E
-00000110: 6e75 6d29 01da 0844 6970 6f6c 6554 4f63  num)...DipoleTOc
-00000120: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00000130: 0100 0000 4000 0000 7314 0000 0065 005a  ....@...s....e.Z
-00000140: 0164 005a 0264 015a 0364 025a 0464 0353  .d.Z.d.Z.d.Z.d.S
-00000150: 0029 04da 1544 6970 6f6c 654d 6561 7375  .)...DipoleMeasu
-00000160: 7265 6d65 6e74 5479 7065 e901 0000 00e9  rementType......
-00000170: 0200 0000 4e29 05da 085f 5f6e 616d 655f  ....N)...__name_
-00000180: 5fda 0a5f 5f6d 6f64 756c 655f 5fda 0c5f  _..__module__.._
-00000190: 5f71 7561 6c6e 616d 655f 5fda 1245 4c45  _qualname__..ELE
-000001a0: 4354 5249 435f 504f 5445 4e54 4941 4cda  CTRIC_POTENTIAL.
-000001b0: 1058 5f45 4c45 4354 5249 435f 4649 454c  .X_ELECTRIC_FIEL
-000001c0: 44a9 0072 0d00 0000 720d 0000 00fa 532f  D..r....r.....S/
-000001d0: 686f 6d65 2f6a 656e 6b69 6e73 2f61 6765  home/jenkins/age
-000001e0: 6e74 2f77 6f72 6b73 7061 6365 2f67 6974  nt/workspace/git
-000001f0: 6561 2d70 6879 7369 6373 5f74 616e 7472  ea-physics_tantr
-00000200: 695f 312e 302e 312f 7461 6e74 7269 2f64  i_1.0.1/tantri/d
-00000210: 6970 6f6c 6573 2f5f 5f69 6e69 745f 5f2e  ipoles/__init__.
-00000220: 7079 7205 0000 000d 0000 0073 0400 0000  pyr........s....
-00000230: 0801 0401 7205 0000 0054 2901 da06 6672  ....r....T)...fr
-00000240: 6f7a 656e 6300 0000 0000 0000 0000 0000  ozenc...........
-00000250: 0000 0000 0003 0000 0040 0000 0073 2000  .........@...s .
-00000260: 0000 6500 5a01 6400 5a02 5500 6503 6a04  ..e.Z.d.Z.U.e.j.
-00000270: 6505 6401 3c00 6506 6505 6402 3c00 6403  e.d.<.e.e.d.<.d.
-00000280: 5300 2904 da0b 446f 7450 6f73 6974 696f  S.)...DotPositio
-00000290: 6eda 0172 da05 6c61 6265 6c4e 2907 7208  n..r..labelN).r.
-000002a0: 0000 0072 0900 0000 720a 0000 00da 056e  ...r....r......n
-000002b0: 756d 7079 da07 6e64 6172 7261 79da 0f5f  umpy..ndarray.._
-000002c0: 5f61 6e6e 6f74 6174 696f 6e73 5f5f da03  _annotations__..
-000002d0: 7374 7272 0d00 0000 720d 0000 0072 0d00  strr....r....r..
-000002e0: 0000 720e 0000 0072 1000 0000 1200 0000  ..r....r........
-000002f0: 7304 0000 000a 030a 0172 1000 0000 6300  s........r....c.
-00000300: 0000 0000 0000 0000 0000 0000 0000 0006  ................
-00000310: 0000 0040 0000 0073 9e00 0000 6500 5a01  ...@...s....e.Z.
-00000320: 6400 5a02 5500 6503 6a04 6505 6401 3c00  d.Z.U.e.j.e.d.<.
-00000330: 6503 6a04 6505 6402 3c00 6506 6505 6403  e.j.e.d.<.e.e.d.
-00000340: 3c00 6507 6a08 6509 1900 6505 6404 3c00  <.e.j.e...e.d.<.
-00000350: 650a 6505 6405 3c00 6406 6407 9c01 6408  e.e.d.<.d.d...d.
-00000360: 6409 8404 5a0b 6509 6506 640a 9c02 640b  d...Z.e.e.d...d.
-00000370: 640c 8404 5a0c 6509 6506 640a 9c02 640d  d...Z.e.e.d...d.
-00000380: 640e 8404 5a0d 6414 6506 6507 6a0e 6503  d...Z.d.e.e.j.e.
-00000390: 6a0f 6a10 1900 6507 6a11 6512 6506 6602  j.j...e.j.e.e.f.
-000003a0: 1900 640f 9c03 6410 6411 8405 5a13 6412  ..d...d.d...Z.d.
-000003b0: 6413 8400 5a14 6406 5300 2915 da0d 5772  d...Z.d.S.)...Wr
-000003c0: 6170 7065 6444 6970 6f6c 65da 0170 da01  appedDipole..p..
-000003d0: 73da 0177 da0d 646f 745f 706f 7369 7469  s..w..dot_positi
-000003e0: 6f6e 73da 106d 6561 7375 7265 6d65 6e74  ons..measurement
-000003f0: 5f74 7970 654e a901 da06 7265 7475 726e  _typeN....return
-00000400: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
-00000410: 0004 0000 0043 0000 0073 7600 0000 7400  .....C...sv...t.
-00000420: a001 7c00 6a02 a101 7c00 5f02 7400 a001  ..|.j...|._.t...
-00000430: 7c00 6a03 a101 7c00 5f03 6401 7c00 5f04  |.j...|._.d.|._.
-00000440: 6900 7c00 5f05 7c00 6a06 4400 5d42 7d01  i.|._.|.j.D.]B}.
-00000450: 7c00 6a07 7408 6a09 7500 7252 7c00 a00a  |.j.t.j.u.rR|...
-00000460: 7c01 a101 7c00 6a05 7c01 6a0b 3c00 712e  |...|.j.|.j.<.q.
-00000470: 7c00 6a07 7408 6a0c 7500 722e 7c00 a00d  |.j.t.j.u.r.|...
-00000480: 7c01 a101 7c00 6a05 7c01 6a0b 3c00 712e  |...|.j.|.j.<.q.
-00000490: 6402 5300 2903 7a2a 0a09 0943 6f65 7263  d.S.).z*...Coerc
-000004a0: 6520 7468 6520 696e 7075 7473 2069 6e74  e the inputs int
-000004b0: 6f20 6e75 6d70 7920 6172 7261 7973 2e0a  o numpy arrays..
-000004c0: 0909 7206 0000 004e 290e 7213 0000 00da  ..r....N).r.....
-000004d0: 0561 7272 6179 7218 0000 0072 1900 0000  .arrayr....r....
-000004e0: da05 7374 6174 65da 0563 6163 6865 721b  ..state..cacher.
-000004f0: 0000 0072 1c00 0000 7205 0000 0072 0b00  ...r....r....r..
-00000500: 0000 da09 706f 7465 6e74 6961 6c72 1200  ....potentialr..
-00000510: 0000 720c 0000 00da 0965 5f66 6965 6c64  ..r......e_field
-00000520: 5f78 2902 da04 7365 6c66 da03 706f 7372  _x)...self..posr
-00000530: 0d00 0000 720d 0000 0072 0e00 0000 da0d  ....r....r......
-00000540: 5f5f 706f 7374 5f69 6e69 745f 5f2a 0000  __post_init__*..
-00000550: 0073 1200 0000 0004 0e01 0e02 0601 0601  .s..............
-00000560: 0a01 0c01 1401 0c01 7a1b 5772 6170 7065  ........z.Wrappe
-00000570: 6444 6970 6f6c 652e 5f5f 706f 7374 5f69  dDipole.__post_i
-00000580: 6e69 745f 5f29 02da 0364 6f74 721e 0000  nit__)...dotr...
-00000590: 0063 0200 0000 0000 0000 0000 0000 0300  .c..............
-000005a0: 0000 0400 0000 4300 0000 7328 0000 007c  ......C...s(...|
-000005b0: 006a 007c 016a 0118 007d 027c 006a 02a0  .j.|.j...}.|.j..
-000005c0: 037c 02a1 0174 046a 05a0 067c 02a1 0164  .|...t.j...|...d
-000005d0: 0113 001b 0053 0029 024e e903 0000 0029  .....S.).N.....)
-000005e0: 0772 1900 0000 7211 0000 0072 1800 0000  .r....r....r....
-000005f0: 7227 0000 0072 1300 0000 da06 6c69 6e61  r'...r......lina
-00000600: 6c67 da04 6e6f 726d 2903 7224 0000 0072  lg..norm).r$...r
-00000610: 2700 0000 da06 725f 6469 6666 720d 0000  '.....r_diffr...
-00000620: 0072 0d00 0000 720e 0000 0072 2200 0000  .r....r....r"...
-00000630: 3900 0000 7304 0000 0000 020c 017a 1757  9...s........z.W
-00000640: 7261 7070 6564 4469 706f 6c65 2e70 6f74  rappedDipole.pot
-00000650: 656e 7469 616c 6302 0000 0000 0000 0000  entialc.........
-00000660: 0000 0004 0000 0004 0000 0043 0000 0073  ...........C...s
-00000670: 4600 0000 7c00 6a00 7c01 6a01 1800 7d02  F...|.j.|.j...}.
-00000680: 7402 6a03 a004 7c02 a101 7d03 6401 7c00  t.j...|...}.d.|.
-00000690: 6a05 a006 7c02 a101 1400 7c02 1400 7c03  j...|.....|...|.
-000006a0: 6402 1300 1b00 7c00 6a05 1800 7c03 6401  d.....|.j...|.d.
-000006b0: 1300 1b00 6403 1900 5300 2904 4e72 2800  ....d...S.).Nr(.
-000006c0: 0000 7207 0000 0072 0100 0000 2907 7219  ..r....r....).r.
-000006d0: 0000 0072 1100 0000 7213 0000 0072 2900  ...r....r....r).
-000006e0: 0000 722a 0000 0072 1800 0000 7227 0000  ..r*...r....r'..
-000006f0: 0029 0472 2400 0000 7227 0000 0072 2b00  .).r$...r'...r+.
-00000700: 0000 722a 0000 0072 0d00 0000 720d 0000  ..r*...r....r...
-00000710: 0072 0e00 0000 7223 0000 003e 0000 0073  .r....r#...>...s
-00000720: 0a00 0000 0002 0c01 0c03 2801 02fe 7a17  ..........(...z.
-00000730: 5772 6170 7065 6444 6970 6f6c 652e 655f  WrappedDipole.e_
-00000740: 6669 656c 645f 7829 03da 0264 74da 0a72  field_x)...dt..r
-00000750: 6e67 5f74 6f5f 7573 6572 1e00 0000 6303  ng_to_user....c.
-00000760: 0000 0000 0000 0000 0000 0005 0000 0005  ................
-00000770: 0000 0003 0000 0073 7400 0000 7c02 6400  .......st...|.d.
-00000780: 7500 7214 7400 6a01 a002 a100 7d03 6e04  u.r.t.j.....}.n.
-00000790: 7c02 7d03 7c01 6401 1400 6402 8800 6a03  |.}.|.d...d...j.
-000007a0: 1b00 6b05 723e 7c03 6a04 6403 6402 6404  ..k.r>|.j.d.d.d.
-000007b0: 6405 8d03 8800 5f05 6e1e 7c01 8800 6a03  d....._.n.|...j.
-000007c0: 1400 7d04 7c03 a001 a100 7c04 6b00 725c  ..}.|.....|.k.r\
-000007d0: 8800 a006 a100 0100 8700 6601 6406 6407  ..........f.d.d.
-000007e0: 8408 8800 6a07 a008 a100 4400 8301 5300  ....j.....D...S.
-000007f0: 2908 4ee9 0a00 0000 7206 0000 0072 0100  ).N.....r....r..
-00000800: 0000 5429 01da 0865 6e64 706f 696e 7463  ..T)...endpointc
-00000810: 0100 0000 0000 0000 0000 0000 0300 0000  ................
-00000820: 0500 0000 1300 0000 731c 0000 0069 007c  ........s....i.|
-00000830: 005d 145c 027d 017d 027c 0188 006a 007c  .].\.}.}.|...j.|
-00000840: 0214 0093 0271 0453 0072 0d00 0000 a901  .....q.S.r......
-00000850: 7220 0000 0029 03da 022e 30da 016b da01  r ...)....0..k..
-00000860: 76a9 0172 2400 0000 720d 0000 0072 0e00  v..r$...r....r..
-00000870: 0000 da0a 3c64 6963 7463 6f6d 703e 5b00  ....<dictcomp>[.
-00000880: 0000 f300 0000 007a 2c57 7261 7070 6564  .......z,Wrapped
-00000890: 4469 706f 6c65 2e74 7261 6e73 6974 696f  Dipole.transitio
-000008a0: 6e2e 3c6c 6f63 616c 733e 2e3c 6469 6374  n.<locals>.<dict
-000008b0: 636f 6d70 3e29 0972 1300 0000 da06 7261  comp>).r......ra
-000008c0: 6e64 6f6d da0b 6465 6661 756c 745f 726e  ndom..default_rn
-000008d0: 6772 1a00 0000 da08 696e 7465 6765 7273  gr......integers
-000008e0: 7220 0000 00da 0a66 6c69 705f 7374 6174  r .....flip_stat
-000008f0: 6572 2100 0000 da05 6974 656d 7329 0572  er!.....items).r
-00000900: 2400 0000 722c 0000 0072 2d00 0000 da03  $...r,...r-.....
-00000910: 726e 675a 0470 726f 6272 0d00 0000 7234  rngZ.probr....r4
-00000920: 0000 0072 0e00 0000 da0a 7472 616e 7369  ...r......transi
-00000930: 7469 6f6e 4700 0000 7312 0000 0000 0408  tionG...s.......
-00000940: 010c 0204 0312 0414 020a 010c 0208 017a  ...............z
-00000950: 1857 7261 7070 6564 4469 706f 6c65 2e74  .WrappedDipole.t
-00000960: 7261 6e73 6974 696f 6e63 0100 0000 0000  ransitionc......
-00000970: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-00000980: 0000 7312 0000 007c 0004 006a 0064 0139  ..s....|...j.d.9
-00000990: 0002 005f 0064 0053 0029 024e e9ff ffff  ..._.d.S.).N....
-000009a0: ff72 3000 0000 7234 0000 0072 0d00 0000  .r0...r4...r....
-000009b0: 720d 0000 0072 0e00 0000 723a 0000 005d  r....r....r:...]
-000009c0: 0000 0073 0200 0000 0001 7a18 5772 6170  ...s......z.Wrap
-000009d0: 7065 6444 6970 6f6c 652e 666c 6970 5f73  pedDipole.flip_s
-000009e0: 7461 7465 2901 4e29 1572 0800 0000 7209  tate).N).r....r.
-000009f0: 0000 0072 0a00 0000 7213 0000 0072 1400  ...r....r....r..
-00000a00: 0000 7215 0000 00da 0566 6c6f 6174 da06  ..r......float..
-00000a10: 7479 7069 6e67 da08 5365 7175 656e 6365  typing..Sequence
-00000a20: 7210 0000 0072 0500 0000 7226 0000 0072  r....r....r&...r
-00000a30: 2200 0000 7223 0000 00da 084f 7074 696f  "...r#.....Optio
-00000a40: 6e61 6c72 3700 0000 da09 4765 6e65 7261  nalr7.....Genera
-00000a50: 746f 72da 0444 6963 7472 1600 0000 723d  tor..Dictr....r=
-00000a60: 0000 0072 3a00 0000 720d 0000 0072 0d00  ...r:...r....r..
-00000a70: 0000 720d 0000 0072 0e00 0000 7217 0000  ..r....r....r...
-00000a80: 0019 0000 0073 1c00 0000 0a03 0a01 0a03  .....s..........
-00000a90: 0806 0e02 0802 0e0f 1005 100a 00ff 0201  ................
-00000aa0: 0e01 0cfe 0c16 7217 0000 0029 04da 0a64  ......r....)...d
-00000ab0: 6970 6f6c 655f 746f 73da 0464 6f74 7372  ipole_tos..dotsr
-00000ac0: 1c00 0000 721e 0000 0063 0300 0000 0000  ....r....c......
-00000ad0: 0000 0000 0000 0300 0000 0300 0000 0300  ................
-00000ae0: 0000 7314 0000 0087 0087 0166 0264 0164  ..s........f.d.d
-00000af0: 0284 087c 0044 0083 0153 0029 034e 6301  ...|.D...S.).Nc.
-00000b00: 0000 0000 0000 0000 0000 0002 0000 0009  ................
-00000b10: 0000 0013 0000 0073 2400 0000 6700 7c00  .......s$...g.|.
-00000b20: 5d1c 7d01 7400 7c01 6a01 7c01 6a02 7c01  ].}.t.|.j.|.j.|.
-00000b30: 6a03 8800 8801 6400 8d05 9102 7104 5300  j.....d.....q.S.
-00000b40: 2901 2905 7218 0000 0072 1900 0000 721a  ).).r....r....r.
-00000b50: 0000 0072 1b00 0000 721c 0000 0029 0472  ...r....r....).r
-00000b60: 1700 0000 7218 0000 0072 1900 0000 721a  ....r....r....r.
-00000b70: 0000 0029 0272 3100 0000 5a09 6469 706f  ...).r1...Z.dipo
-00000b80: 6c65 5f74 6fa9 0272 4600 0000 721c 0000  le_to..rF...r...
-00000b90: 0072 0d00 0000 720e 0000 00da 0a3c 6c69  .r....r......<li
-00000ba0: 7374 636f 6d70 3e66 0000 0073 1000 0000  stcomp>f...s....
-00000bb0: 0608 02f9 0201 0401 0401 0401 0201 02fb  ................
-00000bc0: 7a27 6765 745f 7772 6170 7065 645f 6469  z'get_wrapped_di
-00000bd0: 706f 6c65 732e 3c6c 6f63 616c 733e 2e3c  poles.<locals>.<
-00000be0: 6c69 7374 636f 6d70 3e72 0d00 0000 2903  listcomp>r....).
-00000bf0: 7245 0000 0072 4600 0000 721c 0000 0072  rE...rF...r....r
-00000c00: 0d00 0000 7247 0000 0072 0e00 0000 da13  ....rG...r......
-00000c10: 6765 745f 7772 6170 7065 645f 6469 706f  get_wrapped_dipo
-00000c20: 6c65 7361 0000 0073 0600 0000 0005 0c08  lesa...s........
-00000c30: 02f8 7249 0000 0063 0000 0000 0000 0000  ..rI...c........
-00000c40: 0000 0000 0000 0000 0700 0000 4000 0000  ............@...
-00000c50: 7352 0000 0065 005a 0164 005a 0264 0865  sR...e.Z.d.Z.d.e
-00000c60: 036a 0465 0519 0065 036a 0465 0619 0065  .j.e...e.j.e...e
-00000c70: 0765 0865 036a 0965 0a6a 0b6a 0c19 0064  .e.e.j.e.j.j...d
-00000c80: 029c 0564 0364 0484 055a 0d65 036a 0e65  ...d.d...Z.e.j.e
-00000c90: 0f65 0866 0219 0064 059c 0164 0664 0784  .e.f...d...d.d..
-00000ca0: 045a 1064 0153 0029 09da 1044 6970 6f6c  .Z.d.S.)...Dipol
-00000cb0: 6554 696d 6553 6572 6965 734e 2905 da07  eTimeSeriesN)...
-00000cc0: 6469 706f 6c65 7372 4600 0000 721c 0000  dipolesrF...r...
-00000cd0: 0072 2c00 0000 722d 0000 0063 0600 0000  .r,...r-...c....
-00000ce0: 0000 0000 0000 0000 0600 0000 0400 0000  ................
-00000cf0: 4300 0000 733e 0000 007c 0001 007c 0564  C...s>...|...|.d
-00000d00: 0075 0072 1a74 006a 01a0 02a1 007c 005f  .u.r.t.j.....|._
-00000d10: 036e 067c 057c 005f 0374 047c 017c 027c  .n.|.|._.t.|.|.|
-00000d20: 0383 037c 005f 0564 017c 005f 067c 047c  ...|._.d.|._.|.|
-00000d30: 005f 0764 0053 0029 024e 7201 0000 0029  ._.d.S.).Nr....)
-00000d40: 0872 1300 0000 7237 0000 0072 3800 0000  .r....r7...r8...
-00000d50: 723c 0000 0072 4900 0000 724b 0000 0072  r<...rI...rK...r
-00000d60: 2000 0000 722c 0000 0029 0672 2400 0000   ...r,...).r$...
-00000d70: 724b 0000 0072 4600 0000 721c 0000 0072  rK...rF...r....r
-00000d80: 2c00 0000 722d 0000 0072 0d00 0000 720d  ,...r-...r....r.
-00000d90: 0000 0072 0e00 0000 da08 5f5f 696e 6974  ...r......__init
-00000da0: 5f5f 7300 0000 730e 0000 0000 0804 0108  __s...s.........
-00000db0: 010e 0206 020e 0106 017a 1944 6970 6f6c  .........z.Dipol
-00000dc0: 6554 696d 6553 6572 6965 732e 5f5f 696e  eTimeSeries.__in
-00000dd0: 6974 5f5f 721d 0000 0063 0100 0000 0000  it__r....c......
-00000de0: 0000 0000 0000 0600 0000 0600 0000 0300  ................
-00000df0: 0000 735a 0000 0087 0066 0164 0164 0284  ..sZ.....f.d.d..
-00000e00: 0888 006a 0044 0083 017d 0169 007d 027c  ...j.D...}.i.}.|
-00000e10: 0144 005d 387d 037c 03a0 01a1 0044 005d  .D.]8}.|.....D.]
-00000e20: 2a5c 027d 047d 057c 047c 0276 0172 427c  *\.}.}.|.|.v.rB|
-00000e30: 057c 027c 043c 0071 287c 027c 0405 0019  .|.|.<.q(|.|....
-00000e40: 007c 0537 0003 003c 0071 2871 1c7c 0253  .|.7...<.q(q.|.S
-00000e50: 0029 034e 6301 0000 0000 0000 0000 0000  .).Nc...........
-00000e60: 0002 0000 0006 0000 0013 0000 0073 1c00  .............s..
-00000e70: 0000 6700 7c00 5d14 7d01 7c01 a000 8800  ..g.|.].}.|.....
-00000e80: 6a01 8800 6a02 a102 9102 7104 5300 720d  j...j.....q.S.r.
-00000e90: 0000 0029 0372 3d00 0000 722c 0000 0072  ...).r=...r,...r
-00000ea0: 3c00 0000 2902 7231 0000 005a 0664 6970  <...).r1...Z.dip
-00000eb0: 6f6c 6572 3400 0000 720d 0000 0072 0e00  oler4...r....r..
-00000ec0: 0000 7248 0000 0086 0000 0072 3600 0000  ..rH.......r6...
-00000ed0: 7a2f 4469 706f 6c65 5469 6d65 5365 7269  z/DipoleTimeSeri
-00000ee0: 6573 2e74 7261 6e73 6974 696f 6e2e 3c6c  es.transition.<l
-00000ef0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
-00000f00: 3e29 0272 4b00 0000 723b 0000 0029 0672  >).rK...r;...).r
-00000f10: 2400 0000 5a08 6e65 775f 7661 6c73 da03  $...Z.new_vals..
-00000f20: 7265 7472 3d00 0000 7232 0000 0072 3300  retr=...r2...r3.
-00000f30: 0000 720d 0000 0072 3400 0000 720e 0000  ..r....r4...r...
-00000f40: 0072 3d00 0000 8500 0000 7310 0000 0000  .r=.......s.....
-00000f50: 0114 0204 0108 0110 0108 010a 0214 017a  ...............z
-00000f60: 1b44 6970 6f6c 6554 696d 6553 6572 6965  .DipoleTimeSerie
-00000f70: 732e 7472 616e 7369 7469 6f6e 2901 4e29  s.transition).N)
-00000f80: 1172 0800 0000 7209 0000 0072 0a00 0000  .r....r....r....
-00000f90: 7240 0000 0072 4100 0000 7204 0000 0072  r@...rA...r....r
-00000fa0: 1000 0000 7205 0000 0072 3f00 0000 7242  ....r....r?...rB
-00000fb0: 0000 0072 1300 0000 7237 0000 0072 4300  ...r....r7...rC.
-00000fc0: 0000 724c 0000 0072 4400 0000 7216 0000  ..rL...rD...r...
-00000fd0: 0072 3d00 0000 720d 0000 0072 0d00 0000  .r=...r....r....
-00000fe0: 720d 0000 0072 0e00 0000 724a 0000 0072  r....r....rJ...r
-00000ff0: 0000 0073 1200 0000 0807 00fa 0202 0801  ...s............
-00001000: 0801 0201 0201 0cfa 0c12 724a 0000 0029  ..........rJ...)
-00001010: 0372 1700 0000 724a 0000 0072 0400 0000  .r....rJ...r....
-00001020: 2914 da0b 6461 7461 636c 6173 7365 7372  )...dataclassesr
-00001030: 0200 0000 7213 0000 00da 0c6e 756d 7079  ....r......numpy
-00001040: 2e72 616e 646f 6d72 4000 0000 da04 656e  .randomr@.....en
-00001050: 756d 7203 0000 005a 1474 616e 7472 692e  umr....Z.tantri.
-00001060: 6469 706f 6c65 732e 7479 7065 7372 0400  dipoles.typesr..
-00001070: 0000 da07 6c6f 6767 696e 67da 0967 6574  ....logging..get
-00001080: 4c6f 6767 6572 7208 0000 00da 075f 6c6f  Loggerr......_lo
-00001090: 6767 6572 7205 0000 0072 1000 0000 7217  ggerr....r....r.
-000010a0: 0000 0072 4100 0000 7249 0000 0072 4a00  ...rA...rI...rJ.
-000010b0: 0000 da07 5f5f 616c 6c5f 5f72 0d00 0000  ....__all__r....
-000010c0: 720d 0000 0072 0d00 0000 720e 0000 00da  r....r....r.....
-000010d0: 083c 6d6f 6475 6c65 3e01 0000 0073 2600  .<module>....s&.
-000010e0: 0000 0c01 0801 0801 0801 0c01 0c02 0802  ................
-000010f0: 0a03 1005 0801 1006 0201 1048 0801 0801  ...........H....
-00001100: 0201 08fc 0c11 0e20                      ....... 
+00000050: 5a04 6400 6403 6c05 6d06 5a06 6d07 5a07  Z.d.d.l.m.Z.m.Z.
+00000060: 6d08 5a08 0100 6400 6402 6c09 5a0a 6501  m.Z...d.d.l.Z.e.
+00000070: 4700 6404 6405 8400 6405 8302 8301 5a0b  G.d.d...d.....Z.
+00000080: 6504 6a0c 6506 1900 6504 6a0c 6507 1900  e.j.e...e.j.e...
+00000090: 6508 6504 6a0c 650b 1900 6406 9c04 6407  e.e.j.e...d...d.
+000000a0: 6408 8404 5a0d 4700 6409 640a 8400 640a  d...Z.G.d.d...d.
+000000b0: 8302 5a0e 6402 5300 290b e900 0000 0029  ..Z.d.S.)......)
+000000c0: 01da 0964 6174 6163 6c61 7373 4e29 03da  ...dataclassN)..
+000000d0: 0844 6970 6f6c 6554 4fda 0b44 6f74 506f  .DipoleTO..DotPo
+000000e0: 7369 7469 6f6e da15 4469 706f 6c65 4d65  sition..DipoleMe
+000000f0: 6173 7572 656d 656e 7454 7970 6563 0000  asurementTypec..
+00000100: 0000 0000 0000 0000 0000 0000 0000 0600  ................
+00000110: 0000 4000 0000 739e 0000 0065 005a 0164  ..@...s....e.Z.d
+00000120: 005a 0255 0065 036a 0465 0564 013c 0065  .Z.U.e.j.e.d.<.e
+00000130: 036a 0465 0564 023c 0065 0665 0564 033c  .j.e.d.<.e.e.d.<
+00000140: 0065 076a 0865 0919 0065 0564 043c 0065  .e.j.e...e.d.<.e
+00000150: 0a65 0564 053c 0064 0664 079c 0164 0864  .e.d.<.d.d...d.d
+00000160: 0984 045a 0b65 0965 0664 0a9c 0264 0b64  ...Z.e.e.d...d.d
+00000170: 0c84 045a 0c65 0965 0664 0a9c 0264 0d64  ...Z.e.e.d...d.d
+00000180: 0e84 045a 0d64 1465 0665 076a 0e65 036a  ...Z.d.e.e.j.e.j
+00000190: 0f6a 1019 0065 076a 1165 1265 0666 0219  .j...e.j.e.e.f..
+000001a0: 0064 0f9c 0364 1064 1184 055a 1364 1264  .d...d.d...Z.d.d
+000001b0: 1384 005a 1464 0653 0029 15da 0d57 7261  ...Z.d.S.)...Wra
+000001c0: 7070 6564 4469 706f 6c65 da01 70da 0173  ppedDipole..p..s
+000001d0: da01 77da 0d64 6f74 5f70 6f73 6974 696f  ..w..dot_positio
+000001e0: 6e73 da10 6d65 6173 7572 656d 656e 745f  ns..measurement_
+000001f0: 7479 7065 4ea9 01da 0672 6574 7572 6e63  typeN....returnc
+00000200: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000210: 0400 0000 4300 0000 7376 0000 0074 00a0  ....C...sv...t..
+00000220: 017c 006a 02a1 017c 005f 0274 00a0 017c  .|.j...|._.t...|
+00000230: 006a 03a1 017c 005f 0364 017c 005f 0469  .j...|._.d.|._.i
+00000240: 007c 005f 057c 006a 0644 005d 427d 017c  .|._.|.j.D.]B}.|
+00000250: 006a 0774 086a 0975 0072 527c 00a0 0a7c  .j.t.j.u.rR|...|
+00000260: 01a1 017c 006a 057c 016a 0b3c 0071 2e7c  ...|.j.|.j.<.q.|
+00000270: 006a 0774 086a 0c75 0072 2e7c 00a0 0d7c  .j.t.j.u.r.|...|
+00000280: 01a1 017c 006a 057c 016a 0b3c 0071 2e64  ...|.j.|.j.<.q.d
+00000290: 0253 0029 037a 2a0a 0909 436f 6572 6365  .S.).z*...Coerce
+000002a0: 2074 6865 2069 6e70 7574 7320 696e 746f   the inputs into
+000002b0: 206e 756d 7079 2061 7272 6179 732e 0a09   numpy arrays...
+000002c0: 09e9 0100 0000 4e29 0eda 056e 756d 7079  ......N)...numpy
+000002d0: da05 6172 7261 7972 0700 0000 7208 0000  ..arrayr....r...
+000002e0: 00da 0573 7461 7465 da05 6361 6368 6572  ...state..cacher
+000002f0: 0a00 0000 720b 0000 0072 0500 0000 da12  ....r....r......
+00000300: 454c 4543 5452 4943 5f50 4f54 454e 5449  ELECTRIC_POTENTI
+00000310: 414c da09 706f 7465 6e74 6961 6cda 056c  AL..potential..l
+00000320: 6162 656c da10 585f 454c 4543 5452 4943  abel..X_ELECTRIC
+00000330: 5f46 4945 4c44 da09 655f 6669 656c 645f  _FIELD..e_field_
+00000340: 7829 02da 0473 656c 66da 0370 6f73 a900  x)...self..pos..
+00000350: 721a 0000 00fa 562f 686f 6d65 2f6a 656e  r.....V/home/jen
+00000360: 6b69 6e73 2f61 6765 6e74 2f77 6f72 6b73  kins/agent/works
+00000370: 7061 6365 2f67 6974 6561 2d70 6879 7369  pace/gitea-physi
+00000380: 6373 5f74 616e 7472 695f 312e 312e 302f  cs_tantri_1.1.0/
+00000390: 7461 6e74 7269 2f64 6970 6f6c 6573 2f74  tantri/dipoles/t
+000003a0: 696d 655f 7365 7269 6573 2e70 79da 0d5f  ime_series.py.._
+000003b0: 5f70 6f73 745f 696e 6974 5f5f 1a00 0000  _post_init__....
+000003c0: 7312 0000 0000 040e 010e 0206 0106 010a  s...............
+000003d0: 010c 0114 010c 017a 1b57 7261 7070 6564  .......z.Wrapped
+000003e0: 4469 706f 6c65 2e5f 5f70 6f73 745f 696e  Dipole.__post_in
+000003f0: 6974 5f5f 2902 da03 646f 7472 0d00 0000  it__)...dotr....
+00000400: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
+00000410: 0004 0000 0043 0000 0073 2800 0000 7c00  .....C...s(...|.
+00000420: 6a00 7c01 6a01 1800 7d02 7c00 6a02 a003  j.|.j...}.|.j...
+00000430: 7c02 a101 7404 6a05 a006 7c02 a101 6401  |...t.j...|...d.
+00000440: 1300 1b00 5300 2902 4ee9 0300 0000 2907  ....S.).N.....).
+00000450: 7208 0000 00da 0172 7207 0000 0072 1d00  r......rr....r..
+00000460: 0000 720f 0000 00da 066c 696e 616c 67da  ..r......linalg.
+00000470: 046e 6f72 6d29 0372 1800 0000 721d 0000  .norm).r....r...
+00000480: 00da 0672 5f64 6966 6672 1a00 0000 721a  ...r_diffr....r.
+00000490: 0000 0072 1b00 0000 7214 0000 0029 0000  ...r....r....)..
+000004a0: 0073 0400 0000 0002 0c01 7a17 5772 6170  .s........z.Wrap
+000004b0: 7065 6444 6970 6f6c 652e 706f 7465 6e74  pedDipole.potent
+000004c0: 6961 6c63 0200 0000 0000 0000 0000 0000  ialc............
+000004d0: 0400 0000 0400 0000 4300 0000 7346 0000  ........C...sF..
+000004e0: 007c 006a 007c 016a 0118 007d 0274 026a  .|.j.|.j...}.t.j
+000004f0: 03a0 047c 02a1 017d 0364 017c 006a 05a0  ...|...}.d.|.j..
+00000500: 067c 02a1 0114 007c 0214 007c 0364 0213  .|.....|...|.d..
+00000510: 001b 007c 006a 0518 007c 0364 0113 001b  ...|.j...|.d....
+00000520: 0064 0319 0053 0029 044e 721e 0000 00e9  .d...S.).Nr.....
+00000530: 0200 0000 7201 0000 0029 0772 0800 0000  ....r....).r....
+00000540: 721f 0000 0072 0f00 0000 7220 0000 0072  r....r....r ...r
+00000550: 2100 0000 7207 0000 0072 1d00 0000 2904  !...r....r....).
+00000560: 7218 0000 0072 1d00 0000 7222 0000 0072  r....r....r"...r
+00000570: 2100 0000 721a 0000 0072 1a00 0000 721b  !...r....r....r.
+00000580: 0000 0072 1700 0000 2e00 0000 730a 0000  ...r........s...
+00000590: 0000 020c 010c 0328 0102 fe7a 1757 7261  .......(...z.Wra
+000005a0: 7070 6564 4469 706f 6c65 2e65 5f66 6965  ppedDipole.e_fie
+000005b0: 6c64 5f78 2903 da02 6474 da0a 726e 675f  ld_x)...dt..rng_
+000005c0: 746f 5f75 7365 720d 0000 0063 0300 0000  to_user....c....
+000005d0: 0000 0000 0000 0000 0500 0000 0500 0000  ................
+000005e0: 0300 0000 7374 0000 007c 0264 0075 0072  ....st...|.d.u.r
+000005f0: 1474 006a 01a0 02a1 007d 036e 047c 027d  .t.j.....}.n.|.}
+00000600: 037c 0164 0114 0064 0288 006a 031b 006b  .|.d...d...j...k
+00000610: 0572 3e7c 036a 0464 0364 0264 0464 058d  .r>|.j.d.d.d.d..
+00000620: 0388 005f 056e 1e7c 0188 006a 0314 007d  ..._.n.|...j...}
+00000630: 047c 03a0 01a1 007c 046b 0072 5c88 00a0  .|.....|.k.r\...
+00000640: 06a1 0001 0087 0066 0164 0664 0784 0888  .......f.d.d....
+00000650: 006a 07a0 08a1 0044 0083 0153 0029 084e  .j.....D...S.).N
+00000660: e90a 0000 0072 0e00 0000 7201 0000 0054  .....r....r....T
+00000670: 2901 da08 656e 6470 6f69 6e74 6301 0000  )...endpointc...
+00000680: 0000 0000 0000 0000 0003 0000 0005 0000  ................
+00000690: 0013 0000 0073 1c00 0000 6900 7c00 5d14  .....s....i.|.].
+000006a0: 5c02 7d01 7d02 7c01 8800 6a00 7c02 1400  \.}.}.|...j.|...
+000006b0: 9302 7104 5300 721a 0000 00a9 0172 1100  ..q.S.r......r..
+000006c0: 0000 2903 da02 2e30 da01 6bda 0176 a901  ..)....0..k..v..
+000006d0: 7218 0000 0072 1a00 0000 721b 0000 00da  r....r....r.....
+000006e0: 0a3c 6469 6374 636f 6d70 3e4b 0000 00f3  .<dictcomp>K....
+000006f0: 0000 0000 7a2c 5772 6170 7065 6444 6970  ....z,WrappedDip
+00000700: 6f6c 652e 7472 616e 7369 7469 6f6e 2e3c  ole.transition.<
+00000710: 6c6f 6361 6c73 3e2e 3c64 6963 7463 6f6d  locals>.<dictcom
+00000720: 703e 2909 720f 0000 00da 0672 616e 646f  p>).r......rando
+00000730: 6dda 0b64 6566 6175 6c74 5f72 6e67 7209  m..default_rngr.
+00000740: 0000 00da 0869 6e74 6567 6572 7372 1100  .....integersr..
+00000750: 0000 da0a 666c 6970 5f73 7461 7465 7212  ....flip_stater.
+00000760: 0000 00da 0569 7465 6d73 2905 7218 0000  .....items).r...
+00000770: 0072 2400 0000 7225 0000 00da 0372 6e67  .r$...r%.....rng
+00000780: 5a04 7072 6f62 721a 0000 0072 2c00 0000  Z.probr....r,...
+00000790: 721b 0000 00da 0a74 7261 6e73 6974 696f  r......transitio
+000007a0: 6e37 0000 0073 1200 0000 0004 0801 0c02  n7...s..........
+000007b0: 0403 1204 1402 0a01 0c02 0801 7a18 5772  ............z.Wr
+000007c0: 6170 7065 6444 6970 6f6c 652e 7472 616e  appedDipole.tran
+000007d0: 7369 7469 6f6e 6301 0000 0000 0000 0000  sitionc.........
+000007e0: 0000 0001 0000 0003 0000 0043 0000 0073  ...........C...s
+000007f0: 1200 0000 7c00 0400 6a00 6401 3900 0200  ....|...j.d.9...
+00000800: 5f00 6400 5300 2902 4ee9 ffff ffff 7228  _.d.S.).N.....r(
+00000810: 0000 0072 2c00 0000 721a 0000 0072 1a00  ...r,...r....r..
+00000820: 0000 721b 0000 0072 3200 0000 4d00 0000  ..r....r2...M...
+00000830: 7302 0000 0000 017a 1857 7261 7070 6564  s......z.Wrapped
+00000840: 4469 706f 6c65 2e66 6c69 705f 7374 6174  Dipole.flip_stat
+00000850: 6529 014e 2915 da08 5f5f 6e61 6d65 5f5f  e).N)...__name__
+00000860: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000870: 7175 616c 6e61 6d65 5f5f 720f 0000 00da  qualname__r.....
+00000880: 076e 6461 7272 6179 da0f 5f5f 616e 6e6f  .ndarray..__anno
+00000890: 7461 7469 6f6e 735f 5fda 0566 6c6f 6174  tations__..float
+000008a0: da06 7479 7069 6e67 da08 5365 7175 656e  ..typing..Sequen
+000008b0: 6365 7204 0000 0072 0500 0000 721c 0000  cer....r....r...
+000008c0: 0072 1400 0000 7217 0000 00da 084f 7074  .r....r......Opt
+000008d0: 696f 6e61 6c72 2f00 0000 da09 4765 6e65  ionalr/.....Gene
+000008e0: 7261 746f 72da 0444 6963 74da 0373 7472  rator..Dict..str
+000008f0: 7235 0000 0072 3200 0000 721a 0000 0072  r5...r2...r....r
+00000900: 1a00 0000 721a 0000 0072 1b00 0000 7206  ....r....r....r.
+00000910: 0000 0009 0000 0073 1c00 0000 0a03 0a01  .......s........
+00000920: 0a03 0806 0e02 0802 0e0f 1005 100a 00ff  ................
+00000930: 0201 0e01 0cfe 0c16 7206 0000 0029 04da  ........r....)..
+00000940: 0a64 6970 6f6c 655f 746f 73da 0464 6f74  .dipole_tos..dot
+00000950: 7372 0b00 0000 720d 0000 0063 0300 0000  sr....r....c....
+00000960: 0000 0000 0000 0000 0300 0000 0300 0000  ................
+00000970: 0300 0000 7314 0000 0087 0087 0166 0264  ....s........f.d
+00000980: 0164 0284 087c 0044 0083 0153 0029 034e  .d...|.D...S.).N
+00000990: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+000009a0: 0009 0000 0013 0000 0073 2400 0000 6700  .........s$...g.
+000009b0: 7c00 5d1c 7d01 7400 7c01 6a01 7c01 6a02  |.].}.t.|.j.|.j.
+000009c0: 7c01 6a03 8800 8801 6400 8d05 9102 7104  |.j.....d.....q.
+000009d0: 5300 2901 2905 7207 0000 0072 0800 0000  S.).).r....r....
+000009e0: 7209 0000 0072 0a00 0000 720b 0000 0029  r....r....r....)
+000009f0: 0472 0600 0000 7207 0000 0072 0800 0000  .r....r....r....
+00000a00: 7209 0000 0029 0272 2900 0000 5a09 6469  r....).r)...Z.di
+00000a10: 706f 6c65 5f74 6fa9 0272 4400 0000 720b  pole_to..rD...r.
+00000a20: 0000 0072 1a00 0000 721b 0000 00da 0a3c  ...r....r......<
+00000a30: 6c69 7374 636f 6d70 3e56 0000 0073 1000  listcomp>V...s..
+00000a40: 0000 0608 02f9 0201 0401 0401 0401 0201  ................
+00000a50: 02fb 7a27 6765 745f 7772 6170 7065 645f  ..z'get_wrapped_
+00000a60: 6469 706f 6c65 732e 3c6c 6f63 616c 733e  dipoles.<locals>
+00000a70: 2e3c 6c69 7374 636f 6d70 3e72 1a00 0000  .<listcomp>r....
+00000a80: 2903 7243 0000 0072 4400 0000 720b 0000  ).rC...rD...r...
+00000a90: 0072 1a00 0000 7245 0000 0072 1b00 0000  .r....rE...r....
+00000aa0: da13 6765 745f 7772 6170 7065 645f 6469  ..get_wrapped_di
+00000ab0: 706f 6c65 7351 0000 0073 0600 0000 0005  polesQ...s......
+00000ac0: 0c08 02f8 7247 0000 0063 0000 0000 0000  ....rG...c......
+00000ad0: 0000 0000 0000 0000 0000 0700 0000 4000  ..............@.
+00000ae0: 0000 736a 0000 0065 005a 0164 005a 0264  ..sj...e.Z.d.Z.d
+00000af0: 0a65 036a 0465 0519 0065 036a 0465 0619  .e.j.e...e.j.e..
+00000b00: 0065 0765 0865 036a 0965 0a6a 0b6a 0c19  .e.e.e.j.e.j.j..
+00000b10: 0064 029c 0564 0364 0484 055a 0d65 036a  .d...d.d...Z.e.j
+00000b20: 0e65 0f65 0866 0219 0064 059c 0164 0664  .e.e.f...d...d.d
+00000b30: 0784 045a 1065 036a 0e65 0f65 0866 0219  ...Z.e.j.e.e.f..
+00000b40: 0064 059c 0164 0864 0984 045a 1164 0153  .d...d.d...Z.d.S
+00000b50: 0029 0bda 1044 6970 6f6c 6554 696d 6553  .)...DipoleTimeS
+00000b60: 6572 6965 734e 2905 da07 6469 706f 6c65  eriesN)...dipole
+00000b70: 7372 4400 0000 720b 0000 0072 2400 0000  srD...r....r$...
+00000b80: 7225 0000 0063 0600 0000 0000 0000 0000  r%...c..........
+00000b90: 0000 0800 0000 0400 0000 4300 0000 736c  ..........C...sl
+00000ba0: 0000 007c 0001 007c 0564 0075 0072 1a74  ...|...|.d.u.r.t
+00000bb0: 006a 01a0 02a1 007c 005f 036e 067c 057c  .j.....|._.n.|.|
+00000bc0: 005f 0374 047c 017c 027c 0383 037c 005f  ._.t.|.|.|...|._
+00000bd0: 0564 017c 005f 0674 0764 0264 0384 007c  .d.|._.t.d.d...|
+00000be0: 006a 0544 0083 0183 017d 0674 086a 056a  .j.D.....}.t.j.j
+00000bf0: 09a0 0a7c 067c 04a1 027d 077c 076a 0b7c  ...|.|...}.|.j.|
+00000c00: 005f 0c7c 076a 0d7c 005f 0d64 0053 0029  ._.|.j.|._.d.S.)
+00000c10: 044e 7201 0000 0063 0100 0000 0000 0000  .Nr....c........
+00000c20: 0000 0000 0200 0000 0200 0000 7300 0000  ............s...
+00000c30: 7314 0000 007c 005d 0c7d 017c 016a 0056  s....|.].}.|.j.V
+00000c40: 0001 0071 0264 0053 0029 014e 2901 7209  ...q.d.S.).N).r.
+00000c50: 0000 0029 0272 2900 0000 da01 6472 1a00  ...).r).....dr..
+00000c60: 0000 721a 0000 0072 1b00 0000 da09 3c67  ..r....r......<g
+00000c70: 656e 6578 7072 3e76 0000 0072 2e00 0000  enexpr>v...r....
+00000c80: 7a2c 4469 706f 6c65 5469 6d65 5365 7269  z,DipoleTimeSeri
+00000c90: 6573 2e5f 5f69 6e69 745f 5f2e 3c6c 6f63  es.__init__.<loc
+00000ca0: 616c 733e 2e3c 6765 6e65 7870 723e 290e  als>.<genexpr>).
+00000cb0: 720f 0000 0072 2f00 0000 7230 0000 0072  r....r/...r0...r
+00000cc0: 3400 0000 7247 0000 0072 4900 0000 7211  4...rG...rI...r.
+00000cd0: 0000 00da 036d 6178 da06 7461 6e74 7269  .....max..tantri
+00000ce0: 5a0b 7375 7065 7273 616d 706c 655a 0f67  Z.supersampleZ.g
+00000cf0: 6574 5f73 7570 6572 7361 6d70 6c65 5a08  et_supersampleZ.
+00000d00: 7375 7065 725f 6474 7224 0000 00da 1273  super_dtr$.....s
+00000d10: 7570 6572 5f73 616d 706c 655f 7261 7469  uper_sample_rati
+00000d20: 6f29 0872 1800 0000 7249 0000 0072 4400  o).r....rI...rD.
+00000d30: 0000 720b 0000 0072 2400 0000 7225 0000  ..r....r$...r%..
+00000d40: 005a 0d6d 6178 5f66 7265 7175 656e 6379  .Z.max_frequency
+00000d50: 5a0c 7375 7065 725f 7361 6d70 6c65 721a  Z.super_sampler.
+00000d60: 0000 0072 1a00 0000 721b 0000 00da 085f  ...r....r......_
+00000d70: 5f69 6e69 745f 5f63 0000 0073 1400 0000  _init__c...s....
+00000d80: 0008 0401 0801 0e02 0602 0e01 0604 1402  ................
+00000d90: 1001 0801 7a19 4469 706f 6c65 5469 6d65  ....z.DipoleTime
+00000da0: 5365 7269 6573 2e5f 5f69 6e69 745f 5f72  Series.__init__r
+00000db0: 0c00 0000 6301 0000 0000 0000 0000 0000  ....c...........
+00000dc0: 0006 0000 0006 0000 0003 0000 0073 5a00  .............sZ.
+00000dd0: 0000 8700 6601 6401 6402 8408 8800 6a00  ....f.d.d.....j.
+00000de0: 4400 8301 7d01 6900 7d02 7c01 4400 5d38  D...}.i.}.|.D.]8
+00000df0: 7d03 7c03 a001 a100 4400 5d2a 5c02 7d04  }.|.....D.]*\.}.
+00000e00: 7d05 7c04 7c02 7601 7242 7c05 7c02 7c04  }.|.|.v.rB|.|.|.
+00000e10: 3c00 7128 7c02 7c04 0500 1900 7c05 3700  <.q(|.|.....|.7.
+00000e20: 0300 3c00 7128 711c 7c02 5300 2903 4e63  ..<.q(q.|.S.).Nc
+00000e30: 0100 0000 0000 0000 0000 0000 0200 0000  ................
+00000e40: 0600 0000 1300 0000 731c 0000 0067 007c  ........s....g.|
+00000e50: 005d 147d 017c 01a0 0088 006a 0188 006a  .].}.|.....j...j
+00000e60: 02a1 0291 0271 0453 0072 1a00 0000 2903  .....q.S.r....).
+00000e70: 7235 0000 0072 2400 0000 7234 0000 0029  r5...r$...r4...)
+00000e80: 0272 2900 0000 5a06 6469 706f 6c65 722c  .r)...Z.dipoler,
+00000e90: 0000 0072 1a00 0000 721b 0000 0072 4600  ...r....r....rF.
+00000ea0: 0000 7d00 0000 722e 0000 007a 3444 6970  ..}...r....z4Dip
+00000eb0: 6f6c 6554 696d 6553 6572 6965 732e 5f73  oleTimeSeries._s
+00000ec0: 7562 5f74 7261 6e73 6974 696f 6e2e 3c6c  ub_transition.<l
+00000ed0: 6f63 616c 733e 2e3c 6c69 7374 636f 6d70  ocals>.<listcomp
+00000ee0: 3e29 0272 4900 0000 7233 0000 0029 0672  >).rI...r3...).r
+00000ef0: 1800 0000 5a08 6e65 775f 7661 6c73 da03  ....Z.new_vals..
+00000f00: 7265 7472 3500 0000 722a 0000 0072 2b00  retr5...r*...r+.
+00000f10: 0000 721a 0000 0072 2c00 0000 721b 0000  ..r....r,...r...
+00000f20: 00da 0f5f 7375 625f 7472 616e 7369 7469  ..._sub_transiti
+00000f30: 6f6e 7c00 0000 7310 0000 0000 0114 0204  on|...s.........
+00000f40: 0108 0110 0108 010a 0214 017a 2044 6970  ...........z Dip
+00000f50: 6f6c 6554 696d 6553 6572 6965 732e 5f73  oleTimeSeries._s
+00000f60: 7562 5f74 7261 6e73 6974 696f 6e63 0100  ub_transitionc..
+00000f70: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00000f80: 0000 0300 0000 731c 0000 0087 0066 0164  ......s......f.d
+00000f90: 0164 0284 0874 0088 006a 0183 0144 0083  .d...t...j...D..
+00000fa0: 0164 0319 0053 0029 044e 6301 0000 0000  .d...S.).Nc.....
+00000fb0: 0000 0000 0000 0002 0000 0004 0000 0013  ................
+00000fc0: 0000 0073 1400 0000 6700 7c00 5d0c 7d01  ...s....g.|.].}.
+00000fd0: 8800 a000 a100 9102 7104 5300 721a 0000  ........q.S.r...
+00000fe0: 0029 0172 5100 0000 2902 7229 0000 00da  .).rQ...).r)....
+00000ff0: 0169 722c 0000 0072 1a00 0000 721b 0000  .ir,...r....r...
+00001000: 0072 4600 0000 8900 0000 722e 0000 007a  .rF.......r....z
+00001010: 2f44 6970 6f6c 6554 696d 6553 6572 6965  /DipoleTimeSerie
+00001020: 732e 7472 616e 7369 7469 6f6e 2e3c 6c6f  s.transition.<lo
+00001030: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
+00001040: 7236 0000 0029 02da 0572 616e 6765 724e  r6...)...rangerN
+00001050: 0000 0072 2c00 0000 721a 0000 0072 2c00  ...r,...r....r,.
+00001060: 0000 721b 0000 0072 3500 0000 8800 0000  ..r....r5.......
+00001070: 7302 0000 0000 017a 1b44 6970 6f6c 6554  s......z.DipoleT
+00001080: 696d 6553 6572 6965 732e 7472 616e 7369  imeSeries.transi
+00001090: 7469 6f6e 2901 4e29 1272 3700 0000 7238  tion).N).r7...r8
+000010a0: 0000 0072 3900 0000 723d 0000 0072 3e00  ...r9...r=...r>.
+000010b0: 0000 7203 0000 0072 0400 0000 7205 0000  ..r....r....r...
+000010c0: 0072 3c00 0000 723f 0000 0072 0f00 0000  .r<...r?...r....
+000010d0: 722f 0000 0072 4000 0000 724f 0000 0072  r/...r@...rO...r
+000010e0: 4100 0000 7242 0000 0072 5100 0000 7235  A...rB...rQ...r5
+000010f0: 0000 0072 1a00 0000 721a 0000 0072 1a00  ...r....r....r..
+00001100: 0000 721b 0000 0072 4800 0000 6200 0000  ..r....rH...b...
+00001110: 7314 0000 0008 0700 fa02 0208 0108 0102  s...............
+00001120: 0102 010c fa0c 1918 0c72 4800 0000 290f  .........rH...).
+00001130: da0b 6461 7461 636c 6173 7365 7372 0200  ..dataclassesr..
+00001140: 0000 720f 0000 00da 0c6e 756d 7079 2e72  ..r......numpy.r
+00001150: 616e 646f 6d72 3d00 0000 da14 7461 6e74  andomr=.....tant
+00001160: 7269 2e64 6970 6f6c 6573 2e74 7970 6573  ri.dipoles.types
+00001170: 7203 0000 0072 0400 0000 7205 0000 005a  r....r....r....Z
+00001180: 1a74 616e 7472 692e 6469 706f 6c65 732e  .tantri.dipoles.
+00001190: 7375 7065 7273 616d 706c 6572 4d00 0000  supersamplerM...
+000011a0: 7206 0000 0072 3e00 0000 7247 0000 0072  r....r>...rG...r
+000011b0: 4800 0000 721a 0000 0072 1a00 0000 721a  H...r....r....r.
+000011c0: 0000 0072 1b00 0000 da08 3c6d 6f64 756c  ...r......<modul
+000011d0: 653e 0100 0000 731a 0000 000c 0108 0108  e>....s.........
+000011e0: 0108 0114 0108 0302 0110 4808 0108 0102  ..........H.....
+000011f0: 0108 fc0c 11                             .....
```

### Comparing `tantri-1.0.1/tantri/simple_telegraph/__init__.py` & `tantri-1.1.0/tantri/simple_telegraph/__init__.py`

 * *Files identical despite different names*

### Comparing `tantri-1.0.1/tantri/simple_telegraph/__pycache__/__init__.cpython-39.pyc` & `tantri-1.1.0/tantri/simple_telegraph/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 22 20:18:56 2024 UTC, .py size: 675 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 30c6 2666 a302 0000  a.......0.&f....
+00000000: 610d 0d0a 0000 0000 cbe8 3366 a302 0000  a.........3f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a01 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000040: 8302 5a02 6401 5300 2904 e900 0000 004e  ..Z.d.S.)......N
 00000050: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 00000060: 0003 0000 0040 0000 0073 2e00 0000 6500  .....@...s....e.
 00000070: 5a01 6400 5a02 6503 6a04 6a05 6506 6401  Z.d.Z.e.j.j.e.d.
@@ -28,15 +28,15 @@
 000001b0: 756d 7079 da06 7261 6e64 6f6d 5a0b 6465  umpy..randomZ.de
 000001c0: 6661 756c 745f 726e 67da 0372 6e67 da05  fault_rng..rng..
 000001d0: 7374 6174 6529 03da 0473 656c 6672 0300  state)...selfr..
 000001e0: 0000 7204 0000 00a9 0072 0c00 0000 fa5c  ..r......r.....\
 000001f0: 2f68 6f6d 652f 6a65 6e6b 696e 732f 6167  /home/jenkins/ag
 00000200: 656e 742f 776f 726b 7370 6163 652f 6769  ent/workspace/gi
 00000210: 7465 612d 7068 7973 6963 735f 7461 6e74  tea-physics_tant
-00000220: 7269 5f31 2e30 2e31 2f74 616e 7472 692f  ri_1.0.1/tantri/
+00000220: 7269 5f31 2e31 2e30 2f74 616e 7472 692f  ri_1.1.0/tantri/
 00000230: 7369 6d70 6c65 5f74 656c 6567 7261 7068  simple_telegraph
 00000240: 2f5f 5f69 6e69 745f 5f2e 7079 da08 5f5f  /__init__.py..__
 00000250: 696e 6974 5f5f 0500 0000 7314 0000 0000  init__....s.....
 00000260: 0310 0102 010a ff04 0306 0204 0108 010e  ................
 00000270: 0206 027a 2253 696d 706c 6554 656c 6567  ...z"SimpleTeleg
 00000280: 7261 7068 5469 6d65 5365 7269 6573 2e5f  raphTimeSeries._
 00000290: 5f69 6e69 745f 5f29 01da 0672 6574 7572  _init__)...retur
```

