# Comparing `tmp/dsse-1.1.2.tar.gz` & `tmp/dsse-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsse-1.1.2.tar", last modified: Thu May  2 01:13:32 2024, max compression
+gzip compressed data, was "dsse-1.1.3.tar", last modified: Thu May  2 13:49:11 2024, max compression
```

## Comparing `dsse-1.1.2.tar` & `dsse-1.1.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:32.607998 dsse-1.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:32.603998 dsse-1.1.2/DSSE/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:32.603998 dsse-1.1.2/DSSE/environment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/coverage_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:32.607998 dsse-1.1.2/DSSE/environment/entities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/entities/drone.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/entities/person.py
--rw-r--r--   0 runner    (1001) docker     (127)    13639 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/env_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:32.607998 dsse-1.1.2/DSSE/environment/imgs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/imgs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/pygame_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:32.607998 dsse-1.1.2/DSSE/environment/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/simulation/dynamic_probability.py
--rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/simulation/particle_simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/simulation/time_step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:32.607998 dsse-1.1.2/DSSE/environment/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/wrappers/all_positions_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:32.607998 dsse-1.1.2/DSSE/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/tests/drone_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    12849 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/tests/test_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/tests/test_env_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/tests/test_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:32.607998 dsse-1.1.2/DSSE.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-02 01:13:32.000000 dsse-1.1.2/DSSE.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-02 01:13:32.000000 dsse-1.1.2/DSSE.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 01:13:32.000000 dsse-1.1.2/DSSE.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-02 01:13:32.000000 dsse-1.1.2/DSSE.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 01:13:32.000000 dsse-1.1.2/DSSE.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-02 01:13:16.000000 dsse-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 01:13:16.000000 dsse-1.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-02 01:13:32.607998 dsse-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-05-02 01:13:16.000000 dsse-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-02 01:13:16.000000 dsse-1.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 01:13:32.607998 dsse-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-02 01:13:29.000000 dsse-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:11.768874 dsse-1.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:11.764874 dsse-1.1.3/DSSE/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-02 13:49:01.000000 dsse-1.1.3/DSSE/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:11.764874 dsse-1.1.3/DSSE/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:01.000000 dsse-1.1.3/DSSE/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-02 13:49:01.000000 dsse-1.1.3/DSSE/environment/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-05-02 13:49:01.000000 dsse-1.1.3/DSSE/environment/coverage_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:11.764874 dsse-1.1.3/DSSE/environment/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:01.000000 dsse-1.1.3/DSSE/environment/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-02 13:49:01.000000 dsse-1.1.3/DSSE/environment/entities/drone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-02 13:49:01.000000 dsse-1.1.3/DSSE/environment/entities/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13639 2024-05-02 13:49:01.000000 dsse-1.1.3/DSSE/environment/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-05-02 13:49:01.000000 dsse-1.1.3/DSSE/environment/env_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:11.764874 dsse-1.1.3/DSSE/environment/imgs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:01.000000 dsse-1.1.3/DSSE/environment/imgs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-02 13:49:01.000000 dsse-1.1.3/DSSE/environment/pygame_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:11.768874 dsse-1.1.3/DSSE/environment/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:01.000000 dsse-1.1.3/DSSE/environment/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-02 13:49:01.000000 dsse-1.1.3/DSSE/environment/simulation/dynamic_probability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-05-02 13:49:01.000000 dsse-1.1.3/DSSE/environment/simulation/particle_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-02 13:49:01.000000 dsse-1.1.3/DSSE/environment/simulation/time_step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:11.768874 dsse-1.1.3/DSSE/environment/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-02 13:49:01.000000 dsse-1.1.3/DSSE/environment/wrappers/all_positions_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:11.768874 dsse-1.1.3/DSSE/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:01.000000 dsse-1.1.3/DSSE/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-02 13:49:01.000000 dsse-1.1.3/DSSE/tests/drone_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12849 2024-05-02 13:49:01.000000 dsse-1.1.3/DSSE/tests/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-02 13:49:01.000000 dsse-1.1.3/DSSE/tests/test_env_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-02 13:49:01.000000 dsse-1.1.3/DSSE/tests/test_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:11.768874 dsse-1.1.3/DSSE.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-02 13:49:11.000000 dsse-1.1.3/DSSE.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-02 13:49:11.000000 dsse-1.1.3/DSSE.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:49:11.000000 dsse-1.1.3/DSSE.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-02 13:49:11.000000 dsse-1.1.3/DSSE.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 13:49:11.000000 dsse-1.1.3/DSSE.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-02 13:49:01.000000 dsse-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 13:49:01.000000 dsse-1.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-02 13:49:11.768874 dsse-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-05-02 13:49:01.000000 dsse-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-02 13:49:01.000000 dsse-1.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 13:49:11.768874 dsse-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-02 13:49:09.000000 dsse-1.1.3/setup.py
```

### Comparing `dsse-1.1.2/DSSE/environment/coverage_env.py` & `dsse-1.1.3/DSSE/environment/coverage_env.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.2/DSSE/environment/entities/drone.py` & `dsse-1.1.3/DSSE/environment/entities/drone.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.2/DSSE/environment/entities/person.py` & `dsse-1.1.3/DSSE/environment/entities/person.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.2/DSSE/environment/env.py` & `dsse-1.1.3/DSSE/environment/env.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.2/DSSE/environment/env_base.py` & `dsse-1.1.3/DSSE/environment/env_base.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.2/DSSE/environment/pygame_interface.py` & `dsse-1.1.3/DSSE/environment/pygame_interface.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.2/DSSE/environment/simulation/dynamic_probability.py` & `dsse-1.1.3/DSSE/environment/simulation/dynamic_probability.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.2/DSSE/environment/simulation/particle_simulation.py` & `dsse-1.1.3/DSSE/environment/simulation/particle_simulation.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.2/DSSE/environment/simulation/time_step.py` & `dsse-1.1.3/DSSE/environment/simulation/time_step.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.2/DSSE/environment/wrappers/all_positions_wrapper.py` & `dsse-1.1.3/DSSE/environment/wrappers/all_positions_wrapper.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.2/DSSE/tests/drone_policy.py` & `dsse-1.1.3/DSSE/tests/drone_policy.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.2/DSSE/tests/test_env.py` & `dsse-1.1.3/DSSE/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.2/DSSE/tests/test_env_coverage.py` & `dsse-1.1.3/DSSE/tests/test_env_coverage.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.2/DSSE/tests/test_matrix.py` & `dsse-1.1.3/DSSE/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.2/DSSE.egg-info/PKG-INFO` & `dsse-1.1.3/DSSE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: DSSE
-Version: 1.1.2
+Version: 1.1.3
 Summary: The Drone Swarm Search project provides an environment for SAR missions built on PettingZoo, where agents, represented by drones, are tasked with locating targets identified as shipwrecked individuals.
-Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v1.1.2.tar.gz
+Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v1.1.3.tar.gz
 Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta
 Author-email: Ricardo Ribeiro Rodrigues <ricardorr7@al.insper.edu.br>, Renato Laffranchi Falcão <renatolf1@al.insper.edu.br>, Pedro Henrique Britto Aragão Andrade <pedroa3@al.insper.edu.br>, Jorás Oliveira <jorascco@al.insper.edu.br>, Fabricio Barth <fabriciojb@insper.edu.br>
 License: MIT License
 Project-URL: Homepage, https://pfeinsper.github.io/drone-swarm-search/
 Project-URL: Repository, https://github.com/pfeinsper/drone-swarm-search/
 Project-URL: Documentation, https://pfeinsper.github.io/drone-swarm-search/
 Project-URL: Bug Report, https://github.com/pfeinsper/drone-swarm-search/issues/
```

### Comparing `dsse-1.1.2/DSSE.egg-info/SOURCES.txt` & `dsse-1.1.3/DSSE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dsse-1.1.2/LICENSE` & `dsse-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dsse-1.1.2/PKG-INFO` & `dsse-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: DSSE
-Version: 1.1.2
+Version: 1.1.3
 Summary: The Drone Swarm Search project provides an environment for SAR missions built on PettingZoo, where agents, represented by drones, are tasked with locating targets identified as shipwrecked individuals.
-Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v1.1.2.tar.gz
+Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v1.1.3.tar.gz
 Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta
 Author-email: Ricardo Ribeiro Rodrigues <ricardorr7@al.insper.edu.br>, Renato Laffranchi Falcão <renatolf1@al.insper.edu.br>, Pedro Henrique Britto Aragão Andrade <pedroa3@al.insper.edu.br>, Jorás Oliveira <jorascco@al.insper.edu.br>, Fabricio Barth <fabriciojb@insper.edu.br>
 License: MIT License
 Project-URL: Homepage, https://pfeinsper.github.io/drone-swarm-search/
 Project-URL: Repository, https://github.com/pfeinsper/drone-swarm-search/
 Project-URL: Documentation, https://pfeinsper.github.io/drone-swarm-search/
 Project-URL: Bug Report, https://github.com/pfeinsper/drone-swarm-search/issues/
```

### Comparing `dsse-1.1.2/README.md` & `dsse-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `dsse-1.1.2/pyproject.toml` & `dsse-1.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -58,9 +58,12 @@
 Repository = "https://github.com/pfeinsper/drone-swarm-search/"
 Documentation = "https://pfeinsper.github.io/drone-swarm-search/"
 "Bug Report" = "https://github.com/pfeinsper/drone-swarm-search/issues/"
 
 [tool.setuptools]
 include-package-data = true
 
+[tool.setuptools.package-data]
+DSSE = ["*.png"]
+
 [tool.setuptools.packages.find]
 include = ["DSSE", "DSSE.*"]
```

