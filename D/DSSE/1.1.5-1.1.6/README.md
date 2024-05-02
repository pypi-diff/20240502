# Comparing `tmp/dsse-1.1.5.tar.gz` & `tmp/dsse-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsse-1.1.5.tar", last modified: Thu May  2 18:34:10 2024, max compression
+gzip compressed data, was "dsse-1.1.6.tar", last modified: Thu May  2 18:36:36 2024, max compression
```

## Comparing `dsse-1.1.5.tar` & `dsse-1.1.6.tar`

### file list

```diff
@@ -1,42 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:34:10.541565 dsse-1.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:34:10.533564 dsse-1.1.5/DSSE/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-02 18:33:59.000000 dsse-1.1.5/DSSE/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:34:10.537565 dsse-1.1.5/DSSE/environment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:33:59.000000 dsse-1.1.5/DSSE/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-02 18:33:59.000000 dsse-1.1.5/DSSE/environment/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-05-02 18:33:59.000000 dsse-1.1.5/DSSE/environment/coverage_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:34:10.537565 dsse-1.1.5/DSSE/environment/entities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:33:59.000000 dsse-1.1.5/DSSE/environment/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-02 18:33:59.000000 dsse-1.1.5/DSSE/environment/entities/drone.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-02 18:33:59.000000 dsse-1.1.5/DSSE/environment/entities/person.py
--rw-r--r--   0 runner    (1001) docker     (127)    13639 2024-05-02 18:33:59.000000 dsse-1.1.5/DSSE/environment/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-05-02 18:33:59.000000 dsse-1.1.5/DSSE/environment/env_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:34:10.537565 dsse-1.1.5/DSSE/environment/imgs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:33:59.000000 dsse-1.1.5/DSSE/environment/imgs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-02 18:33:59.000000 dsse-1.1.5/DSSE/environment/pygame_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:34:10.537565 dsse-1.1.5/DSSE/environment/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:33:59.000000 dsse-1.1.5/DSSE/environment/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-02 18:33:59.000000 dsse-1.1.5/DSSE/environment/simulation/dynamic_probability.py
--rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-05-02 18:33:59.000000 dsse-1.1.5/DSSE/environment/simulation/particle_simulation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-02 18:33:59.000000 dsse-1.1.5/DSSE/environment/simulation/time_step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:34:10.537565 dsse-1.1.5/DSSE/environment/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-02 18:33:59.000000 dsse-1.1.5/DSSE/environment/wrappers/all_positions_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:34:10.537565 dsse-1.1.5/DSSE/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 18:33:59.000000 dsse-1.1.5/DSSE/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-02 18:33:59.000000 dsse-1.1.5/DSSE/tests/drone_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    12849 2024-05-02 18:33:59.000000 dsse-1.1.5/DSSE/tests/test_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-02 18:33:59.000000 dsse-1.1.5/DSSE/tests/test_env_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-02 18:33:59.000000 dsse-1.1.5/DSSE/tests/test_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 18:34:10.537565 dsse-1.1.5/DSSE.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-02 18:34:10.000000 dsse-1.1.5/DSSE.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-05-02 18:34:10.000000 dsse-1.1.5/DSSE.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 18:34:10.000000 dsse-1.1.5/DSSE.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-02 18:34:10.000000 dsse-1.1.5/DSSE.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 18:34:10.000000 dsse-1.1.5/DSSE.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-02 18:33:59.000000 dsse-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-02 18:33:59.000000 dsse-1.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-02 18:34:10.541565 dsse-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-05-02 18:33:59.000000 dsse-1.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-02 18:33:59.000000 dsse-1.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 18:34:10.541565 dsse-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-02 18:34:08.000000 dsse-1.1.5/setup.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-02 18:36:36.104976 dsse-1.1.6/
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-02 18:36:36.100976 dsse-1.1.6/DSSE/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      322 2024-04-18 19:38:11.000000 dsse-1.1.6/DSSE/__init__.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-02 18:36:36.100976 dsse-1.1.6/DSSE/environment/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 14:40:14.000000 dsse-1.1.6/DSSE/environment/__init__.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      490 2024-04-18 19:38:11.000000 dsse-1.1.6/DSSE/environment/constants.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     7166 2024-05-02 18:19:41.000000 dsse-1.1.6/DSSE/environment/coverage_env.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-02 18:36:36.100976 dsse-1.1.6/DSSE/environment/entities/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-04-18 19:38:11.000000 dsse-1.1.6/DSSE/environment/entities/__init__.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      686 2024-04-18 19:38:11.000000 dsse-1.1.6/DSSE/environment/entities/drone.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     8070 2024-04-18 19:38:11.000000 dsse-1.1.6/DSSE/environment/entities/person.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    13639 2024-05-02 18:19:41.000000 dsse-1.1.6/DSSE/environment/env.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     8213 2024-05-02 18:19:41.000000 dsse-1.1.6/DSSE/environment/env_base.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-02 18:36:36.100976 dsse-1.1.6/DSSE/environment/imgs/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-05-02 18:19:41.000000 dsse-1.1.6/DSSE/environment/imgs/__init__.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    14774 2024-03-12 14:40:14.000000 dsse-1.1.6/DSSE/environment/imgs/drone.png
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    13193 2024-03-12 14:40:14.000000 dsse-1.1.6/DSSE/environment/imgs/person-swimming.png
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     4765 2024-04-18 19:38:11.000000 dsse-1.1.6/DSSE/environment/pygame_interface.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-02 18:36:36.104976 dsse-1.1.6/DSSE/environment/simulation/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-04-18 19:38:11.000000 dsse-1.1.6/DSSE/environment/simulation/__init__.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     4890 2024-04-18 19:38:11.000000 dsse-1.1.6/DSSE/environment/simulation/dynamic_probability.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     6390 2024-05-02 18:19:41.000000 dsse-1.1.6/DSSE/environment/simulation/particle_simulation.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1205 2024-04-18 19:38:11.000000 dsse-1.1.6/DSSE/environment/simulation/time_step.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-02 18:36:36.104976 dsse-1.1.6/DSSE/environment/wrappers/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1587 2024-04-18 19:38:11.000000 dsse-1.1.6/DSSE/environment/wrappers/all_positions_wrapper.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-02 18:36:36.104976 dsse-1.1.6/DSSE/tests/
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        0 2024-03-12 14:40:14.000000 dsse-1.1.6/DSSE/tests/__init__.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1488 2024-04-18 19:38:11.000000 dsse-1.1.6/DSSE/tests/drone_policy.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)    12849 2024-05-02 18:19:41.000000 dsse-1.1.6/DSSE/tests/test_env.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     6996 2024-05-02 18:19:41.000000 dsse-1.1.6/DSSE/tests/test_env_coverage.py
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      581 2024-04-18 19:38:11.000000 dsse-1.1.6/DSSE/tests/test_matrix.py
+drwxrwxr-x   0 ricardo   (1000) ricardo   (1000)        0 2024-05-02 18:36:36.104976 dsse-1.1.6/DSSE.egg-info/
+-rw-r--r--   0 ricardo   (1000) ricardo   (1000)     7438 2024-05-02 18:36:36.000000 dsse-1.1.6/DSSE.egg-info/PKG-INFO
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      973 2024-05-02 18:36:36.000000 dsse-1.1.6/DSSE.egg-info/SOURCES.txt
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        1 2024-05-02 18:36:36.000000 dsse-1.1.6/DSSE.egg-info/dependency_links.txt
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      257 2024-05-02 18:36:36.000000 dsse-1.1.6/DSSE.egg-info/requires.txt
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)        5 2024-05-02 18:36:36.000000 dsse-1.1.6/DSSE.egg-info/top_level.txt
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     1094 2024-04-18 19:38:11.000000 dsse-1.1.6/LICENSE
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       32 2024-05-02 18:21:55.000000 dsse-1.1.6/MANIFEST.in
+-rw-r--r--   0 ricardo   (1000) ricardo   (1000)     7438 2024-05-02 18:36:36.104976 dsse-1.1.6/PKG-INFO
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     5280 2024-05-02 18:19:41.000000 dsse-1.1.6/README.md
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)     2225 2024-05-02 18:19:41.000000 dsse-1.1.6/pyproject.toml
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)       38 2024-05-02 18:36:36.104976 dsse-1.1.6/setup.cfg
+-rw-rw-r--   0 ricardo   (1000) ricardo   (1000)      189 2024-05-02 18:31:18.000000 dsse-1.1.6/setup.py
```

### Comparing `dsse-1.1.5/DSSE/environment/coverage_env.py` & `dsse-1.1.6/DSSE/environment/coverage_env.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.5/DSSE/environment/entities/drone.py` & `dsse-1.1.6/DSSE/environment/entities/drone.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.5/DSSE/environment/entities/person.py` & `dsse-1.1.6/DSSE/environment/entities/person.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.5/DSSE/environment/env.py` & `dsse-1.1.6/DSSE/environment/env.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.5/DSSE/environment/env_base.py` & `dsse-1.1.6/DSSE/environment/env_base.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.5/DSSE/environment/pygame_interface.py` & `dsse-1.1.6/DSSE/environment/pygame_interface.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.5/DSSE/environment/simulation/dynamic_probability.py` & `dsse-1.1.6/DSSE/environment/simulation/dynamic_probability.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.5/DSSE/environment/simulation/particle_simulation.py` & `dsse-1.1.6/DSSE/environment/simulation/particle_simulation.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.5/DSSE/environment/simulation/time_step.py` & `dsse-1.1.6/DSSE/environment/simulation/time_step.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.5/DSSE/environment/wrappers/all_positions_wrapper.py` & `dsse-1.1.6/DSSE/environment/wrappers/all_positions_wrapper.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.5/DSSE/tests/drone_policy.py` & `dsse-1.1.6/DSSE/tests/drone_policy.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.5/DSSE/tests/test_env.py` & `dsse-1.1.6/DSSE/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.5/DSSE/tests/test_env_coverage.py` & `dsse-1.1.6/DSSE/tests/test_env_coverage.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.5/DSSE/tests/test_matrix.py` & `dsse-1.1.6/DSSE/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `dsse-1.1.5/DSSE.egg-info/PKG-INFO` & `dsse-1.1.6/DSSE.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: DSSE
-Version: 1.1.5
+Version: 1.1.6
 Summary: The Drone Swarm Search project provides an environment for SAR missions built on PettingZoo, where agents, represented by drones, are tasked with locating targets identified as shipwrecked individuals.
-Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v1.1.5.tar.gz
+Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v1.1.6.tar.gz
 Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta
 Author-email: Ricardo Ribeiro Rodrigues <ricardorr7@al.insper.edu.br>, Renato Laffranchi Falcão <renatolf1@al.insper.edu.br>, Pedro Henrique Britto Aragão Andrade <pedroa3@al.insper.edu.br>, Jorás Oliveira <jorascco@al.insper.edu.br>, Fabricio Barth <fabriciojb@insper.edu.br>
 License: MIT License
 Project-URL: Homepage, https://pfeinsper.github.io/drone-swarm-search/
 Project-URL: Repository, https://github.com/pfeinsper/drone-swarm-search/
 Project-URL: Documentation, https://pfeinsper.github.io/drone-swarm-search/
 Project-URL: Bug Report, https://github.com/pfeinsper/drone-swarm-search/issues/
```

### Comparing `dsse-1.1.5/DSSE.egg-info/SOURCES.txt` & `dsse-1.1.6/DSSE.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 DSSE/environment/env.py
 DSSE/environment/env_base.py
 DSSE/environment/pygame_interface.py
 DSSE/environment/entities/__init__.py
 DSSE/environment/entities/drone.py
 DSSE/environment/entities/person.py
 DSSE/environment/imgs/__init__.py
+DSSE/environment/imgs/drone.png
+DSSE/environment/imgs/person-swimming.png
 DSSE/environment/simulation/__init__.py
 DSSE/environment/simulation/dynamic_probability.py
 DSSE/environment/simulation/particle_simulation.py
 DSSE/environment/simulation/time_step.py
 DSSE/environment/wrappers/all_positions_wrapper.py
 DSSE/tests/__init__.py
 DSSE/tests/drone_policy.py
```

### Comparing `dsse-1.1.5/LICENSE` & `dsse-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dsse-1.1.5/PKG-INFO` & `dsse-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: DSSE
-Version: 1.1.5
+Version: 1.1.6
 Summary: The Drone Swarm Search project provides an environment for SAR missions built on PettingZoo, where agents, represented by drones, are tasked with locating targets identified as shipwrecked individuals.
-Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v1.1.5.tar.gz
+Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v1.1.6.tar.gz
 Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta
 Author-email: Ricardo Ribeiro Rodrigues <ricardorr7@al.insper.edu.br>, Renato Laffranchi Falcão <renatolf1@al.insper.edu.br>, Pedro Henrique Britto Aragão Andrade <pedroa3@al.insper.edu.br>, Jorás Oliveira <jorascco@al.insper.edu.br>, Fabricio Barth <fabriciojb@insper.edu.br>
 License: MIT License
 Project-URL: Homepage, https://pfeinsper.github.io/drone-swarm-search/
 Project-URL: Repository, https://github.com/pfeinsper/drone-swarm-search/
 Project-URL: Documentation, https://pfeinsper.github.io/drone-swarm-search/
 Project-URL: Bug Report, https://github.com/pfeinsper/drone-swarm-search/issues/
```

### Comparing `dsse-1.1.5/README.md` & `dsse-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `dsse-1.1.5/pyproject.toml` & `dsse-1.1.6/pyproject.toml`

 * *Files identical despite different names*

