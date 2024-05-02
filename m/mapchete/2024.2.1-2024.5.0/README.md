# Comparing `tmp/mapchete-2024.2.1.tar.gz` & `tmp/mapchete-2024.5.0.tar.gz`

## Comparing `mapchete-2024.2.1.tar` & `mapchete-2024.5.0.tar`

### file list

```diff
@@ -1,114 +1,114 @@
--rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/__init__.py
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/enums.py
--rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/errors.py
--rw-r--r--   0        0        0    17651 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/index.py
--rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/log.py
--rw-r--r--   0        0        0    33243 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/path.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/pretty.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/protocols.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/registered.py
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/settings.py
--rw-r--r--   0        0        0    18489 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/stac.py
--rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/testing.py
--rw-r--r--   0        0        0    17586 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/tile.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/timer.py
--rw-r--r--   0        0        0    12670 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/types.py
--rw-r--r--   0        0        0     5314 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/validate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/cli/__init__.py
--rwxr-xr-x   0        0        0      307 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/cli/main.py
--rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/cli/mpath.py
--rw-r--r--   0        0        0    11242 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/cli/options.py
--rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/cli/progress_bar.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/cli/default/__init__.py
--rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/cli/default/convert.py
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/cli/default/cp.py
--rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/cli/default/create.py
--rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/cli/default/execute.py
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/cli/default/formats.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/cli/default/index.py
--rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/cli/default/processes.py
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/cli/default/rm.py
--rwxr-xr-x   0        0        0     5035 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/cli/default/serve.py
--rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/cli/default/stac.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/commands/__init__.py
--rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/commands/_convert.py
--rw-r--r--   0        0        0     8381 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/commands/_cp.py
--rw-r--r--   0        0        0     8347 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/commands/_execute.py
--rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/commands/_index.py
--rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/commands/_rm.py
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/commands/observer.py
--rw-r--r--   0        0        0     6797 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/commands/parser.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/commons/__init__.py
--rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/commons/clip.py
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/commons/contours.py
--rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/commons/hillshade.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/config/__init__.py
--rw-r--r--   0        0        0    33124 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/config/base.py
--rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/config/models.py
--rw-r--r--   0        0        0    14894 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/config/parse.py
--rw-r--r--   0        0        0     4345 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/config/process_func.py
--rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/executor/__init__.py
--rw-r--r--   0        0        0     6109 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/executor/base.py
--rw-r--r--   0        0        0     6037 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/executor/concurrent_futures.py
--rw-r--r--   0        0        0    10482 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/executor/dask.py
--rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/executor/future.py
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/executor/sequential.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/executor/types.py
--rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/formats/__init__.py
--rw-r--r--   0        0        0    21029 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/formats/base.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/formats/drivers.py
--rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/formats/loaders.py
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/formats/models.py
--rw-r--r--   0        0        0    12983 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/formats/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/formats/default/__init__.py
--rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/formats/default/_fiona_base.py
--rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/formats/default/flatgeobuf.py
--rw-r--r--   0        0        0     5072 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/formats/default/geobuf.py
--rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/formats/default/geojson.py
--rw-r--r--   0        0        0    22077 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/formats/default/gtiff.py
--rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/formats/default/mapchete_input.py
--rw-r--r--   0        0        0     6958 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/formats/default/png.py
--rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/formats/default/png_hillshade.py
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/formats/default/raster_file.py
--rw-r--r--   0        0        0    16775 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/formats/default/tile_directory.py
--rw-r--r--   0        0        0     9624 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/formats/default/vector_file.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/io/__init__.py
--rw-r--r--   0        0        0    12038 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/io/_geometry_operations.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/io/_json.py
--rw-r--r--   0        0        0     7330 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/io/_misc.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/io/_path.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/io/profiles.py
--rw-r--r--   0        0        0    22406 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/io/vector.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/io/raster/__init__.py
--rw-r--r--   0        0        0     9237 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/io/raster/array.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/io/raster/convert.py
--rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/io/raster/mosaic.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/io/raster/open.py
--rw-r--r--   0        0        0    17604 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/io/raster/read.py
--rw-r--r--   0        0        0     6620 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/io/raster/referenced_raster.py
--rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/io/raster/write.py
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/processes/__init__.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/processes/contours.py
--rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/processes/convert.py
--rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/processes/hillshade.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/processes/examples/__init__.py
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/processes/examples/example_process.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/processing/__init__.py
--rw-r--r--   0        0        0    29802 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/processing/base.py
--rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/processing/execute.py
--rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/processing/mp.py
--rw-r--r--   0        0        0    22831 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/processing/tasks.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/processing/types.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/processing/profilers/__init__.py
--rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/processing/profilers/memory.py
--rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/processing/profilers/requests.py
--rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/processing/profilers/time.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/static/__init__.py
--rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/static/index.html
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/static/mapchete_template.mapchete
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 mapchete-2024.2.1/mapchete/static/process_template.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 mapchete-2024.2.1/.gitignore
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 mapchete-2024.2.1/LICENSE
--rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 mapchete-2024.2.1/README.rst
--rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 mapchete-2024.2.1/pyproject.toml
--rw-r--r--   0        0        0     9470 2020-02-02 00:00:00.000000 mapchete-2024.2.1/PKG-INFO
+-rw-r--r--   0        0        0     3792 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/__init__.py
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/enums.py
+-rw-r--r--   0        0        0     1574 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/errors.py
+-rw-r--r--   0        0        0    17651 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/index.py
+-rw-r--r--   0        0        0     3179 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/log.py
+-rw-r--r--   0        0        0    33243 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/path.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/pretty.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/protocols.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/registered.py
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/settings.py
+-rw-r--r--   0        0        0    18489 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/stac.py
+-rw-r--r--   0        0        0     6115 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/testing.py
+-rw-r--r--   0        0        0    17586 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/tile.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/timer.py
+-rw-r--r--   0        0        0    12670 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/types.py
+-rw-r--r--   0        0        0     5314 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/validate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/__init__.py
+-rwxr-xr-x   0        0        0      307 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/main.py
+-rw-r--r--   0        0        0     5566 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/mpath.py
+-rw-r--r--   0        0        0    11242 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/options.py
+-rw-r--r--   0        0        0     2404 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/progress_bar.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/default/__init__.py
+-rw-r--r--   0        0        0     3748 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/default/convert.py
+-rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/default/cp.py
+-rw-r--r--   0        0        0     2963 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/default/create.py
+-rw-r--r--   0        0        0     2434 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/default/execute.py
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/default/formats.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/default/index.py
+-rw-r--r--   0        0        0      989 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/default/processes.py
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/default/rm.py
+-rwxr-xr-x   0        0        0     5035 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/default/serve.py
+-rw-r--r--   0        0        0     4279 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/cli/default/stac.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/commands/__init__.py
+-rw-r--r--   0        0        0     9346 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/commands/_convert.py
+-rw-r--r--   0        0        0     8381 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/commands/_cp.py
+-rw-r--r--   0        0        0     8384 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/commands/_execute.py
+-rw-r--r--   0        0        0     3482 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/commands/_index.py
+-rw-r--r--   0        0        0     4601 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/commands/_rm.py
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/commands/observer.py
+-rw-r--r--   0        0        0     6797 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/commands/parser.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/commons/__init__.py
+-rw-r--r--   0        0        0     2288 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/commons/clip.py
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/commons/contours.py
+-rw-r--r--   0        0        0     5030 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/commons/hillshade.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/config/__init__.py
+-rw-r--r--   0        0        0    33124 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/config/base.py
+-rw-r--r--   0        0        0     2626 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/config/models.py
+-rw-r--r--   0        0        0    14894 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/config/parse.py
+-rw-r--r--   0        0        0     4345 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/config/process_func.py
+-rw-r--r--   0        0        0     1381 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/executor/__init__.py
+-rw-r--r--   0        0        0     6109 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/executor/base.py
+-rw-r--r--   0        0        0     6037 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/executor/concurrent_futures.py
+-rw-r--r--   0        0        0    10482 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/executor/dask.py
+-rw-r--r--   0        0        0     8238 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/executor/future.py
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/executor/sequential.py
+-rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/executor/types.py
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/__init__.py
+-rw-r--r--   0        0        0    21029 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/base.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/drivers.py
+-rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/loaders.py
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/models.py
+-rw-r--r--   0        0        0    12983 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/default/__init__.py
+-rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/default/_fiona_base.py
+-rw-r--r--   0        0        0     2545 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/default/flatgeobuf.py
+-rw-r--r--   0        0        0     5072 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/default/geobuf.py
+-rw-r--r--   0        0        0     2144 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/default/geojson.py
+-rw-r--r--   0        0        0    22077 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/default/gtiff.py
+-rw-r--r--   0        0        0     2179 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/default/mapchete_input.py
+-rw-r--r--   0        0        0     6958 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/default/png.py
+-rw-r--r--   0        0        0     6381 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/default/png_hillshade.py
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/default/raster_file.py
+-rw-r--r--   0        0        0    16775 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/default/tile_directory.py
+-rw-r--r--   0        0        0     9624 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/formats/default/vector_file.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/__init__.py
+-rw-r--r--   0        0        0    12038 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/_geometry_operations.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/_json.py
+-rw-r--r--   0        0        0     7330 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/_misc.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/_path.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/profiles.py
+-rw-r--r--   0        0        0    22406 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/vector.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/raster/__init__.py
+-rw-r--r--   0        0        0     9237 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/raster/array.py
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/raster/convert.py
+-rw-r--r--   0        0        0     7961 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/raster/mosaic.py
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/raster/open.py
+-rw-r--r--   0        0        0    17604 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/raster/read.py
+-rw-r--r--   0        0        0     6620 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/raster/referenced_raster.py
+-rw-r--r--   0        0        0     6188 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/io/raster/write.py
+-rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processes/__init__.py
+-rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processes/contours.py
+-rw-r--r--   0        0        0     4896 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processes/convert.py
+-rw-r--r--   0        0        0     3481 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processes/hillshade.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processes/examples/__init__.py
+-rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processes/examples/example_process.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processing/__init__.py
+-rw-r--r--   0        0        0    29802 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processing/base.py
+-rw-r--r--   0        0        0     7107 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processing/execute.py
+-rw-r--r--   0        0        0     5183 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processing/mp.py
+-rw-r--r--   0        0        0    22831 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processing/tasks.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processing/types.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processing/profilers/__init__.py
+-rw-r--r--   0        0        0     4289 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processing/profilers/memory.py
+-rw-r--r--   0        0        0     1631 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processing/profilers/requests.py
+-rw-r--r--   0        0        0      924 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/processing/profilers/time.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/static/__init__.py
+-rw-r--r--   0        0        0     8416 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/static/index.html
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/static/mapchete_template.mapchete
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 mapchete-2024.5.0/mapchete/static/process_template.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 mapchete-2024.5.0/.gitignore
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 mapchete-2024.5.0/LICENSE
+-rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 mapchete-2024.5.0/README.rst
+-rw-r--r--   0        0        0     3744 2020-02-02 00:00:00.000000 mapchete-2024.5.0/pyproject.toml
+-rw-r--r--   0        0        0     9470 2020-02-02 00:00:00.000000 mapchete-2024.5.0/PKG-INFO
```

### Comparing `mapchete-2024.2.1/mapchete/__init__.py` & `mapchete-2024.5.0/mapchete/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "count_tiles",
     "Mapchete",
     "MapcheteProcess",
     "Timer",
     "Executor",
     "MFuture",
 ]
-__version__ = "2024.2.1"
+__version__ = "2024.5.0"
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 
 def open(
     some_input: Union[MPathLike, dict, MapcheteConfig],
```

### Comparing `mapchete-2024.2.1/mapchete/enums.py` & `mapchete-2024.5.0/mapchete/enums.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/errors.py` & `mapchete-2024.5.0/mapchete/errors.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/index.py` & `mapchete-2024.5.0/mapchete/index.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/log.py` & `mapchete-2024.5.0/mapchete/log.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/path.py` & `mapchete-2024.5.0/mapchete/path.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/pretty.py` & `mapchete-2024.5.0/mapchete/pretty.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/registered.py` & `mapchete-2024.5.0/mapchete/registered.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/settings.py` & `mapchete-2024.5.0/mapchete/settings.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/stac.py` & `mapchete-2024.5.0/mapchete/stac.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/testing.py` & `mapchete-2024.5.0/mapchete/testing.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/tile.py` & `mapchete-2024.5.0/mapchete/tile.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/timer.py` & `mapchete-2024.5.0/mapchete/timer.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/types.py` & `mapchete-2024.5.0/mapchete/types.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/validate.py` & `mapchete-2024.5.0/mapchete/validate.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/cli/mpath.py` & `mapchete-2024.5.0/mapchete/cli/mpath.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/cli/options.py` & `mapchete-2024.5.0/mapchete/cli/options.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/cli/progress_bar.py` & `mapchete-2024.5.0/mapchete/cli/progress_bar.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/cli/default/convert.py` & `mapchete-2024.5.0/mapchete/cli/default/convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/cli/default/cp.py` & `mapchete-2024.5.0/mapchete/cli/default/cp.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/cli/default/create.py` & `mapchete-2024.5.0/mapchete/cli/default/create.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/cli/default/execute.py` & `mapchete-2024.5.0/mapchete/cli/default/execute.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/cli/default/formats.py` & `mapchete-2024.5.0/mapchete/cli/default/formats.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/cli/default/index.py` & `mapchete-2024.5.0/mapchete/cli/default/index.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/cli/default/processes.py` & `mapchete-2024.5.0/mapchete/cli/default/processes.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/cli/default/rm.py` & `mapchete-2024.5.0/mapchete/cli/default/rm.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/cli/default/serve.py` & `mapchete-2024.5.0/mapchete/cli/default/serve.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/cli/default/stac.py` & `mapchete-2024.5.0/mapchete/cli/default/stac.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/commands/_convert.py` & `mapchete-2024.5.0/mapchete/commands/_convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/commands/_cp.py` & `mapchete-2024.5.0/mapchete/commands/_cp.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/commands/_execute.py` & `mapchete-2024.5.0/mapchete/commands/_execute.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Execute a process."""
+
 import logging
 from contextlib import AbstractContextManager
 from multiprocessing import cpu_count
 from typing import List, Optional, Tuple, Type, Union
 
 from rasterio.crs import CRS
 from shapely.geometry.base import BaseGeometry
@@ -141,40 +142,40 @@
                         status=Status.done, message="no tasks to process"
                     )
                     return
 
                 all_observers.notify(
                     message=f"processing {len(tasks)} tasks on {workers} worker(s)"
                 )
-
                 all_observers.notify(message="waiting for executor ...")
-                with executor_getter(
-                    concurrency=concurrency,
-                    dask_scheduler=dask_settings.scheduler,
-                    dask_client=dask_settings.client,
-                    multiprocessing_start_method=multiprocessing_start_method,
-                    max_workers=workers,
-                    preprocessing_tasks=tasks.preprocessing_tasks_count,
-                    tile_tasks=tasks.tile_tasks_count,
-                ) as executor:
-                    if profiling:
-                        for profiler in preconfigured_profilers:
-                            executor.add_profiler(profiler)
-                    else:
-                        executor.add_profiler(
-                            Profiler(name="time", decorator=measure_time)
+
+                try:
+                    with executor_getter(
+                        concurrency=concurrency,
+                        dask_scheduler=dask_settings.scheduler,
+                        dask_client=dask_settings.client,
+                        multiprocessing_start_method=multiprocessing_start_method,
+                        max_workers=workers,
+                        preprocessing_tasks=tasks.preprocessing_tasks_count,
+                        tile_tasks=tasks.tile_tasks_count,
+                    ) as executor:
+                        if profiling:
+                            for profiler in preconfigured_profilers:
+                                executor.add_profiler(profiler)
+                        else:
+                            executor.add_profiler(
+                                Profiler(name="time", decorator=measure_time)
+                            )
+                        all_observers.notify(
+                            status=Status.running,
+                            progress=Progress(total=len(tasks)),
+                            message=f"sending {len(tasks)} tasks to {executor} ...",
+                            executor=executor,
                         )
-                    all_observers.notify(
-                        status=Status.running,
-                        progress=Progress(total=len(tasks)),
-                        message=f"sending {len(tasks)} tasks to {executor} ...",
-                        executor=executor,
-                    )
-                    # TODO it would be nice to track the time it took sending tasks to the executor
-                    try:
+                        # TODO it would be nice to track the time it took sending tasks to the executor
                         for count, task_info in enumerate(
                             mp.execute(
                                 executor=executor,
                                 tasks=tasks,
                                 dask_settings=dask_settings,
                             ),
                             1,
@@ -182,25 +183,25 @@
                             all_observers.notify(
                                 progress=Progress(total=len(tasks), current=count),
                                 task_info=task_info,
                             )
                         all_observers.notify(status=Status.done)
                         return
 
-                    except cancel_on_exception:
-                        # special exception indicating job was cancelled from the outside
-                        all_observers.notify(status=Status.cancelled)
-                        return
+                except cancel_on_exception:
+                    # special exception indicating job was cancelled from the outside
+                    all_observers.notify(status=Status.cancelled)
+                    return
 
-                    except retry_on_exception as exception:
-                        if retries:
-                            retries -= 1
-                            all_observers.notify(
-                                status=Status.retrying,
-                                message=f"run failed due to {repr(exception)} (remaining retries: {retries})",
-                            )
-                        else:
-                            raise
+                except retry_on_exception as exception:
+                    if retries:
+                        retries -= 1
+                        all_observers.notify(
+                            status=Status.retrying,
+                            message=f"run failed due to {repr(exception)} (remaining retries: {retries})",
+                        )
+                    else:
+                        raise
 
     except Exception as exception:
         all_observers.notify(status=Status.failed, exception=exception)
         raise
```

### Comparing `mapchete-2024.2.1/mapchete/commands/_index.py` & `mapchete-2024.5.0/mapchete/commands/_index.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/commands/_rm.py` & `mapchete-2024.5.0/mapchete/commands/_rm.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/commands/parser.py` & `mapchete-2024.5.0/mapchete/commands/parser.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/commons/clip.py` & `mapchete-2024.5.0/mapchete/commons/clip.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/commons/contours.py` & `mapchete-2024.5.0/mapchete/commons/contours.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/commons/hillshade.py` & `mapchete-2024.5.0/mapchete/commons/hillshade.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/config/base.py` & `mapchete-2024.5.0/mapchete/config/base.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/config/models.py` & `mapchete-2024.5.0/mapchete/config/models.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/config/parse.py` & `mapchete-2024.5.0/mapchete/config/parse.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/config/process_func.py` & `mapchete-2024.5.0/mapchete/config/process_func.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/executor/__init__.py` & `mapchete-2024.5.0/mapchete/executor/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/executor/base.py` & `mapchete-2024.5.0/mapchete/executor/base.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/executor/concurrent_futures.py` & `mapchete-2024.5.0/mapchete/executor/concurrent_futures.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/executor/dask.py` & `mapchete-2024.5.0/mapchete/executor/dask.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/executor/future.py` & `mapchete-2024.5.0/mapchete/executor/future.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/executor/sequential.py` & `mapchete-2024.5.0/mapchete/executor/sequential.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/formats/__init__.py` & `mapchete-2024.5.0/mapchete/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/formats/base.py` & `mapchete-2024.5.0/mapchete/formats/base.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/formats/loaders.py` & `mapchete-2024.5.0/mapchete/formats/loaders.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/formats/tools.py` & `mapchete-2024.5.0/mapchete/formats/tools.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/formats/default/_fiona_base.py` & `mapchete-2024.5.0/mapchete/formats/default/_fiona_base.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/formats/default/flatgeobuf.py` & `mapchete-2024.5.0/mapchete/formats/default/flatgeobuf.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/formats/default/geobuf.py` & `mapchete-2024.5.0/mapchete/formats/default/geobuf.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/formats/default/geojson.py` & `mapchete-2024.5.0/mapchete/formats/default/geojson.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/formats/default/gtiff.py` & `mapchete-2024.5.0/mapchete/formats/default/gtiff.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/formats/default/mapchete_input.py` & `mapchete-2024.5.0/mapchete/formats/default/mapchete_input.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/formats/default/png.py` & `mapchete-2024.5.0/mapchete/formats/default/png.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/formats/default/png_hillshade.py` & `mapchete-2024.5.0/mapchete/formats/default/png_hillshade.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/formats/default/raster_file.py` & `mapchete-2024.5.0/mapchete/formats/default/raster_file.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/formats/default/tile_directory.py` & `mapchete-2024.5.0/mapchete/formats/default/tile_directory.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/formats/default/vector_file.py` & `mapchete-2024.5.0/mapchete/formats/default/vector_file.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/io/__init__.py` & `mapchete-2024.5.0/mapchete/io/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/io/_geometry_operations.py` & `mapchete-2024.5.0/mapchete/io/_geometry_operations.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/io/_misc.py` & `mapchete-2024.5.0/mapchete/io/_misc.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/io/profiles.py` & `mapchete-2024.5.0/mapchete/io/profiles.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/io/vector.py` & `mapchete-2024.5.0/mapchete/io/vector.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/io/raster/__init__.py` & `mapchete-2024.5.0/mapchete/io/raster/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/io/raster/array.py` & `mapchete-2024.5.0/mapchete/io/raster/array.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/io/raster/convert.py` & `mapchete-2024.5.0/mapchete/io/raster/convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/io/raster/mosaic.py` & `mapchete-2024.5.0/mapchete/io/raster/mosaic.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/io/raster/open.py` & `mapchete-2024.5.0/mapchete/io/raster/open.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/io/raster/read.py` & `mapchete-2024.5.0/mapchete/io/raster/read.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/io/raster/referenced_raster.py` & `mapchete-2024.5.0/mapchete/io/raster/referenced_raster.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/io/raster/write.py` & `mapchete-2024.5.0/mapchete/io/raster/write.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/processes/__init__.py` & `mapchete-2024.5.0/mapchete/processes/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/processes/contours.py` & `mapchete-2024.5.0/mapchete/processes/contours.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/processes/convert.py` & `mapchete-2024.5.0/mapchete/processes/convert.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/processes/hillshade.py` & `mapchete-2024.5.0/mapchete/processes/hillshade.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/processes/examples/example_process.py` & `mapchete-2024.5.0/mapchete/processes/examples/example_process.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/processing/base.py` & `mapchete-2024.5.0/mapchete/processing/base.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/processing/execute.py` & `mapchete-2024.5.0/mapchete/processing/execute.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/processing/mp.py` & `mapchete-2024.5.0/mapchete/processing/mp.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/processing/tasks.py` & `mapchete-2024.5.0/mapchete/processing/tasks.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/processing/types.py` & `mapchete-2024.5.0/mapchete/processing/types.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/processing/profilers/__init__.py` & `mapchete-2024.5.0/mapchete/processing/profilers/__init__.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/processing/profilers/memory.py` & `mapchete-2024.5.0/mapchete/processing/profilers/memory.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/processing/profilers/requests.py` & `mapchete-2024.5.0/mapchete/processing/profilers/requests.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/processing/profilers/time.py` & `mapchete-2024.5.0/mapchete/processing/profilers/time.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/static/index.html` & `mapchete-2024.5.0/mapchete/static/index.html`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/mapchete/static/process_template.py` & `mapchete-2024.5.0/mapchete/static/process_template.py`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/LICENSE` & `mapchete-2024.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/README.rst` & `mapchete-2024.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/pyproject.toml` & `mapchete-2024.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mapchete-2024.2.1/PKG-INFO` & `mapchete-2024.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: mapchete
-Version: 2024.2.1
+Version: 2024.5.0
 Summary: Tile-based geodata processing using rasterio & Fiona
 Project-URL: Homepage, https://github.com/ungarj/mapchete
 Author-email: Joachim Ungar <joachim.ungar@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

