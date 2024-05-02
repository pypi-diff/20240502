# Comparing `tmp/dsse-1.1.1.tar.gz` & `tmp/dsse-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsse-1.1.1.tar", last modified: Thu May  2 00:39:27 2024, max compression
+gzip compressed data, was "dsse-1.1.2.tar", last modified: Thu May  2 01:13:32 2024, max compression
```

## Comparing `dsse-1.1.1.tar` & `dsse-1.1.2.tar`

### file list

```diff
@@ -1,40 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:39:27.152878 dsse-1.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:39:27.144878 dsse-1.1.1/DSSE/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:39:27.148878 dsse-1.1.1/DSSE/environment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/environment/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/environment/coverage_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:39:27.148878 dsse-1.1.1/DSSE/environment/entities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/environment/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/environment/entities/drone.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/environment/entities/person.py
--rw-r--r--   0 runner    (1001) docker     (127)    13639 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/environment/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/environment/env_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/environment/pygame_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:39:27.148878 dsse-1.1.1/DSSE/environment/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/environment/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/environment/simulation/dynamic_probability.py
--rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/environment/simulation/particle_simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/environment/simulation/time_step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:39:27.148878 dsse-1.1.1/DSSE/environment/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/environment/wrappers/all_positions_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:39:27.148878 dsse-1.1.1/DSSE/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/tests/drone_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    12849 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/tests/test_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/tests/test_env_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/tests/test_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:39:27.148878 dsse-1.1.1/DSSE.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-02 00:39:27.000000 dsse-1.1.1/DSSE.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-02 00:39:27.000000 dsse-1.1.1/DSSE.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 00:39:27.000000 dsse-1.1.1/DSSE.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-02 00:39:27.000000 dsse-1.1.1/DSSE.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 00:39:27.000000 dsse-1.1.1/DSSE.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-02 00:39:16.000000 dsse-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 00:39:16.000000 dsse-1.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-02 00:39:27.148878 dsse-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-05-02 00:39:16.000000 dsse-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-02 00:39:16.000000 dsse-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 00:39:27.152878 dsse-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-02 00:39:25.000000 dsse-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:32.607998 dsse-1.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:32.603998 dsse-1.1.2/DSSE/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:32.603998 dsse-1.1.2/DSSE/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/coverage_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:32.607998 dsse-1.1.2/DSSE/environment/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/entities/drone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/entities/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13639 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/env_base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:32.607998 dsse-1.1.2/DSSE/environment/imgs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/imgs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/pygame_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:32.607998 dsse-1.1.2/DSSE/environment/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/simulation/dynamic_probability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/simulation/particle_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/simulation/time_step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:32.607998 dsse-1.1.2/DSSE/environment/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/environment/wrappers/all_positions_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:32.607998 dsse-1.1.2/DSSE/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/tests/drone_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12849 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/tests/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/tests/test_env_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-02 01:13:16.000000 dsse-1.1.2/DSSE/tests/test_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 01:13:32.607998 dsse-1.1.2/DSSE.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-02 01:13:32.000000 dsse-1.1.2/DSSE.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-02 01:13:32.000000 dsse-1.1.2/DSSE.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 01:13:32.000000 dsse-1.1.2/DSSE.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-02 01:13:32.000000 dsse-1.1.2/DSSE.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 01:13:32.000000 dsse-1.1.2/DSSE.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-02 01:13:16.000000 dsse-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 01:13:16.000000 dsse-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-02 01:13:32.607998 dsse-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-05-02 01:13:16.000000 dsse-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-02 01:13:16.000000 dsse-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 01:13:32.607998 dsse-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-02 01:13:29.000000 dsse-1.1.2/setup.py
```

### Comparing `dsse-1.1.1/DSSE/environment/coverage_env.py` & `dsse-1.1.2/DSSE/environment/coverage_env.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.1/DSSE/environment/entities/drone.py` & `dsse-1.1.2/DSSE/environment/entities/drone.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.1/DSSE/environment/entities/person.py` & `dsse-1.1.2/DSSE/environment/entities/person.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.1/DSSE/environment/env.py` & `dsse-1.1.2/DSSE/environment/env.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.1/DSSE/environment/env_base.py` & `dsse-1.1.2/DSSE/environment/env_base.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.1/DSSE/environment/pygame_interface.py` & `dsse-1.1.2/DSSE/environment/pygame_interface.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.1/DSSE/environment/simulation/dynamic_probability.py` & `dsse-1.1.2/DSSE/environment/simulation/dynamic_probability.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.1/DSSE/environment/simulation/particle_simulation.py` & `dsse-1.1.2/DSSE/environment/simulation/particle_simulation.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.1/DSSE/environment/simulation/time_step.py` & `dsse-1.1.2/DSSE/environment/simulation/time_step.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.1/DSSE/environment/wrappers/all_positions_wrapper.py` & `dsse-1.1.2/DSSE/environment/wrappers/all_positions_wrapper.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.1/DSSE/tests/drone_policy.py` & `dsse-1.1.2/DSSE/tests/drone_policy.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.1/DSSE/tests/test_env.py` & `dsse-1.1.2/DSSE/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.1/DSSE/tests/test_env_coverage.py` & `dsse-1.1.2/DSSE/tests/test_env_coverage.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.1/DSSE/tests/test_matrix.py` & `dsse-1.1.2/DSSE/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.1/DSSE.egg-info/PKG-INFO` & `dsse-1.1.2/DSSE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: DSSE
-Version: 1.1.1
+Version: 1.1.2
 Summary: The Drone Swarm Search project provides an environment for SAR missions built on PettingZoo, where agents, represented by drones, are tasked with locating targets identified as shipwrecked individuals.
-Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v1.1.1.tar.gz
+Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v1.1.2.tar.gz
 Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta
 Author-email: Ricardo Ribeiro Rodrigues <ricardorr7@al.insper.edu.br>, Renato Laffranchi Falcão <renatolf1@al.insper.edu.br>, Pedro Henrique Britto Aragão Andrade <pedroa3@al.insper.edu.br>, Jorás Oliveira <jorascco@al.insper.edu.br>, Fabricio Barth <fabriciojb@insper.edu.br>
 License: MIT License
 Project-URL: Homepage, https://pfeinsper.github.io/drone-swarm-search/
 Project-URL: Repository, https://github.com/pfeinsper/drone-swarm-search/
 Project-URL: Documentation, https://pfeinsper.github.io/drone-swarm-search/
 Project-URL: Bug Report, https://github.com/pfeinsper/drone-swarm-search/issues/
```

### Comparing `dsse-1.1.1/DSSE.egg-info/SOURCES.txt` & `dsse-1.1.2/DSSE.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 DSSE/environment/coverage_env.py
 DSSE/environment/env.py
 DSSE/environment/env_base.py
 DSSE/environment/pygame_interface.py
 DSSE/environment/entities/__init__.py
 DSSE/environment/entities/drone.py
 DSSE/environment/entities/person.py
+DSSE/environment/imgs/__init__.py
 DSSE/environment/simulation/__init__.py
 DSSE/environment/simulation/dynamic_probability.py
 DSSE/environment/simulation/particle_simulation.py
 DSSE/environment/simulation/time_step.py
 DSSE/environment/wrappers/all_positions_wrapper.py
 DSSE/tests/__init__.py
 DSSE/tests/drone_policy.py
```

### Comparing `dsse-1.1.1/LICENSE` & `dsse-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dsse-1.1.1/PKG-INFO` & `dsse-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: DSSE
-Version: 1.1.1
+Version: 1.1.2
 Summary: The Drone Swarm Search project provides an environment for SAR missions built on PettingZoo, where agents, represented by drones, are tasked with locating targets identified as shipwrecked individuals.
-Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v1.1.1.tar.gz
+Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v1.1.2.tar.gz
 Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta
 Author-email: Ricardo Ribeiro Rodrigues <ricardorr7@al.insper.edu.br>, Renato Laffranchi Falcão <renatolf1@al.insper.edu.br>, Pedro Henrique Britto Aragão Andrade <pedroa3@al.insper.edu.br>, Jorás Oliveira <jorascco@al.insper.edu.br>, Fabricio Barth <fabriciojb@insper.edu.br>
 License: MIT License
 Project-URL: Homepage, https://pfeinsper.github.io/drone-swarm-search/
 Project-URL: Repository, https://github.com/pfeinsper/drone-swarm-search/
 Project-URL: Documentation, https://pfeinsper.github.io/drone-swarm-search/
 Project-URL: Bug Report, https://github.com/pfeinsper/drone-swarm-search/issues/
```

### Comparing `dsse-1.1.1/README.md` & `dsse-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dsse-1.1.1/pyproject.toml` & `dsse-1.1.2/pyproject.toml`

 * *Files identical despite different names*

