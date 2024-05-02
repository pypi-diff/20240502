# Comparing `tmp/dsse-1.0.3.tar.gz` & `tmp/dsse-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsse-1.0.3.tar", last modified: Thu Apr 25 20:11:00 2024, max compression
+gzip compressed data, was "dsse-1.1.1.tar", last modified: Thu May  2 00:39:27 2024, max compression
```

## Comparing `dsse-1.0.3.tar` & `dsse-1.1.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:11:00.980493 dsse-1.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:11:00.972493 dsse-1.0.3/DSSE/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:11:00.976493 dsse-1.0.3/DSSE/environment/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6333 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/coverage_env.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:11:00.976493 dsse-1.0.3/DSSE/environment/entities/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/entities/drone.py
--rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/entities/person.py
--rw-r--r--   0 runner    (1001) docker     (127)    12983 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/env.py
--rw-r--r--   0 runner    (1001) docker     (127)     9297 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/env_base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:11:00.976493 dsse-1.0.3/DSSE/environment/imgs/
--rw-r--r--   0 runner    (1001) docker     (127)    14774 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/imgs/drone.png
--rw-r--r--   0 runner    (1001) docker     (127)    13193 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/imgs/person-swimming.png
--rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/pygame_interface.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:11:00.976493 dsse-1.0.3/DSSE/environment/simulation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/simulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/simulation/dynamic_probability.py
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/simulation/particle_sim.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/environment/simulation/time_step.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:11:00.976493 dsse-1.0.3/DSSE/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/tests/drone_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    12849 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/tests/test_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/tests/test_env_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-25 20:10:46.000000 dsse-1.0.3/DSSE/tests/test_matrix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-25 20:11:00.976493 dsse-1.0.3/DSSE.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-04-25 20:11:00.000000 dsse-1.0.3/DSSE.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-04-25 20:11:00.000000 dsse-1.0.3/DSSE.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-25 20:11:00.000000 dsse-1.0.3/DSSE.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-25 20:11:00.000000 dsse-1.0.3/DSSE.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-25 20:11:00.000000 dsse-1.0.3/DSSE.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-25 20:10:46.000000 dsse-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-25 20:10:46.000000 dsse-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5453 2024-04-25 20:11:00.980493 dsse-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4650 2024-04-25 20:10:46.000000 dsse-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-25 20:11:00.980493 dsse-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-25 20:11:00.000000 dsse-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:39:27.152878 dsse-1.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:39:27.144878 dsse-1.1.1/DSSE/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:39:27.148878 dsse-1.1.1/DSSE/environment/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/environment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/environment/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7166 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/environment/coverage_env.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:39:27.148878 dsse-1.1.1/DSSE/environment/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/environment/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/environment/entities/drone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8070 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/environment/entities/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13639 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/environment/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8213 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/environment/env_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4765 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/environment/pygame_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:39:27.148878 dsse-1.1.1/DSSE/environment/simulation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/environment/simulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/environment/simulation/dynamic_probability.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6390 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/environment/simulation/particle_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/environment/simulation/time_step.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:39:27.148878 dsse-1.1.1/DSSE/environment/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1587 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/environment/wrappers/all_positions_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:39:27.148878 dsse-1.1.1/DSSE/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/tests/drone_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12849 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/tests/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6996 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/tests/test_env_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-05-02 00:39:16.000000 dsse-1.1.1/DSSE/tests/test_matrix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 00:39:27.148878 dsse-1.1.1/DSSE.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-02 00:39:27.000000 dsse-1.1.1/DSSE.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-02 00:39:27.000000 dsse-1.1.1/DSSE.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 00:39:27.000000 dsse-1.1.1/DSSE.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-02 00:39:27.000000 dsse-1.1.1/DSSE.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-02 00:39:27.000000 dsse-1.1.1/DSSE.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-05-02 00:39:16.000000 dsse-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 00:39:16.000000 dsse-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7438 2024-05-02 00:39:27.148878 dsse-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-05-02 00:39:16.000000 dsse-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2176 2024-05-02 00:39:16.000000 dsse-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 00:39:27.152878 dsse-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-02 00:39:25.000000 dsse-1.1.1/setup.py
```

### Comparing `dsse-1.0.3/DSSE/environment/coverage_env.py` & `dsse-1.1.1/DSSE/environment/coverage_env.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from gymnasium.spaces import Discrete
 from .env_base import DroneSwarmSearchBase
+from .simulation.particle_simulation import ParticleSimulation
 from .constants import Reward
 import numpy as np
 import functools
 
 
-# TODO: Match env_base to conv_env -> If using particle sim, redo __init__ and reset.
 class CoverageDroneSwarmSearch(DroneSwarmSearchBase):
     metadata = {
         "name": "DroneSwarmSearchCPP",
     }
     reward_scheme = Reward(
         default=0,
         leave_grid=-10,
@@ -17,43 +17,51 @@
         drones_collision=-10,
         search_cell=10,
         search_and_find=100,
     )
 
     def __init__(
         self,
-        grid_size=20,
         render_mode="ansi",
         render_grid=True,
         render_gradient=True,
-        vector=(1, 0.8),
-        dispersion_inc=0.1,
-        dispersion_start=0.5,
         timestep_limit=100,
-        disaster_position=(0, 0),
+        disaster_position=(-24.04, -46.17),
         drone_amount=1,
         drone_speed=10,
         drone_probability_of_detection=0.9,
         pre_render_time=10,
+        prob_matrix_path=None,
     ) -> None:
+
+        # Prob matrix
+        self.probability_matrix = ParticleSimulation(
+            disaster_lat=disaster_position[0],
+            disaster_long=disaster_position[1],
+            duration_hours=pre_render_time,
+        )
+        if prob_matrix_path is not None:
+            if not isinstance(prob_matrix_path, str):
+                raise ValueError("prob_matrix_path must be a string")
+            self.probability_matrix.load_state(prob_matrix_path)
+        else: 
+            self.probability_matrix.run_or_get_simulation()
+        grid_size = self.probability_matrix.get_map_size()
+
         super().__init__(
-            grid_size,
-            render_mode,
-            render_grid,
-            render_gradient,
-            vector,
-            dispersion_inc,
-            dispersion_start,
-            timestep_limit,
-            disaster_position,
-            drone_amount,
-            drone_speed,
-            drone_probability_of_detection,
-            pre_render_time,
+            grid_size=grid_size,
+            render_mode=render_mode,
+            render_grid=render_grid,
+            render_gradient=render_gradient,
+            timestep_limit=timestep_limit,
+            drone_amount=drone_amount,
+            drone_speed=drone_speed,
+            probability_of_detection=drone_probability_of_detection,
         )
+        self.disaster_position = disaster_position
         # Sets used to keep track of the seen and not seen states for reward calculation
         self.seen_states = None
         self.not_seen_states = None
         self.all_states = {
             (x, y) for x in range(self.grid_size) for y in range(self.grid_size)
         }
         self.repeated_coverage = 0
@@ -93,16 +101,15 @@
                 probability_matrix,
             )
             observations[agent] = observation
 
         return observations
 
     def pre_search_simulate(self):
-        for _ in range(self.pre_render_steps):
-            self.probability_matrix.step()
+        self.probability_matrix.run_or_get_simulation()
 
     def step(self, actions: dict[str, int]) -> tuple:
         if not self._was_reset:
             raise ValueError("Please reset the env before interacting with it")
 
         terminations = {a: False for a in self.agents}
         rewards = {a: self.reward_scheme.default for a in self.agents}
@@ -114,19 +121,24 @@
             if agent not in actions:
                 raise ValueError("Missing action for " + agent)
 
             drone_action = actions[agent]
             if drone_action not in self.action_space(agent):
                 raise ValueError("Invalid action for " + agent)
 
+
             if self.timestep >= self.timestep_limit:
                 rewards[agent] = self.reward_scheme.exceed_timestep
                 truncations[agent] = True
                 continue
 
+            # Action 8 is to stay in the same position, default reward.
+            if drone_action == 8:
+                continue
+        
             drone_x, drone_y = self.agents_positions[idx]
             new_position = self.move_drone((drone_x, drone_y), drone_action)
             if not self.is_valid_position(new_position):
                 rewards[agent] = self.reward_scheme.leave_grid
                 continue
 
             self.agents_positions[idx] = new_position
@@ -134,22 +146,24 @@
             if new_position in self.not_seen_states:
                 reward_poc = (1 / (self.timestep)) * prob_matrix[new_y, new_x] * 1_000
                 rewards[agent] = self.reward_scheme.search_cell + reward_poc
                 self.seen_states.add(new_position)
                 self.not_seen_states.remove(new_position)
                 # Probability of sucess (POS) = POC * POD
                 self.cumm_pos += prob_matrix[new_y, new_x] * self.drone.pod
+                # Remove the probability of the visited cell.
+                prob_matrix[new_y, new_x] = 0.0
             else:
                 self.repeated_coverage += 1
 
         # Get dummy infos
         is_completed = len(self.not_seen_states) == 0
         if self.render_mode == "human":
             self.render()
-        
+
         if is_completed:
             # TODO: Proper define reward for completing the search (R_done)
             rewards = {
                 drone: self.reward_scheme.search_and_find for drone in self.agents
             }
             terminations = {drone: True for drone in self.agents}
         infos = self.compute_infos(is_completed)
@@ -169,11 +183,14 @@
         infos = {
             "is_completed": is_completed,
             "coverage_rate": coverage_rate,
             "repeated_coverage": self.repeated_coverage / total_states,
             "acumulated_pos": self.cumm_pos,
         }
         return {drone: infos for drone in self.agents}
+    
+    def save_matrix(self, path: str):
+        self.probability_matrix.save_state(path)
 
     @functools.lru_cache(maxsize=None)
     def action_space(self, agent):
-        return Discrete(8)
+        return Discrete(9)
```

### Comparing `dsse-1.0.3/DSSE/environment/entities/drone.py` & `dsse-1.1.1/DSSE/environment/entities/drone.py`

 * *Files identical despite different names*

### Comparing `dsse-1.0.3/DSSE/environment/entities/person.py` & `dsse-1.1.1/DSSE/environment/entities/person.py`

 * *Files identical despite different names*

### Comparing `dsse-1.0.3/DSSE/environment/env.py` & `dsse-1.1.1/DSSE/environment/env.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from random import random, randint
 import functools
 import numpy as np
 from gymnasium.spaces import MultiDiscrete, Discrete, Box, Tuple
 from .constants import RED, GREEN, Actions, Reward
 from .entities.person import Person
 from .env_base import DroneSwarmSearchBase
+from .simulation.dynamic_probability import ProbabilityMatrix
 
 
 class DroneSwarmSearch(DroneSwarmSearchBase):
     """
     PettingZoo based environment for SAR missions using drones.
     """
 
@@ -48,25 +49,34 @@
         self.person_amount = person_amount
 
         super().__init__(
             grid_size=grid_size,
             render_mode=render_mode,
             render_grid=render_grid,
             render_gradient=render_gradient,
-            vector=vector,
-            dispersion_inc=dispersion_inc,
-            dispersion_start=dispersion_start,
             timestep_limit=timestep_limit,
-            disaster_position=person_initial_position,
             drone_amount=drone_amount,
             drone_speed=drone_speed,
             probability_of_detection=probability_of_detection,
-            pre_render_time=pre_render_time,
         )
 
+        self.pre_render_steps = round(
+            (pre_render_time * 60)
+            / (self.calculate_simulation_time_step(drone_speed, self.cell_size))
+        )
+        print(f"Pre render time: {pre_render_time} minutes")
+        print(f"Pre render steps: {self.pre_render_steps}")
+
+        # Prob matrix
+        self.probability_matrix = None
+        self.dispersion_inc = dispersion_inc
+        self.dispersion_start = dispersion_start
+        self.vector = vector
+        self.disaster_position = person_initial_position
+
         # Person initialization
         self.person_initial_position = person_initial_position
         self.persons_set = self.create_persons_set()
 
         # Initializing render
         self.rewards_sum = {a: 0 for a in self.possible_agents}
         self.rewards_sum["total"] = 0
@@ -132,25 +142,45 @@
         self.pygame_renderer.refresh_screen()
 
     def reset(
         self,
         seed=None,
         options=None,
     ):
+        vector = options.get("vector") if options else None
+        self.vector = vector if vector else self.vector
+
         self.persons_set = self.create_persons_set()
         for person in self.persons_set:
             person.reset_position()
             person.update_time_step_relation(self.time_step_relation, self.cell_size)
 
         pod_multiplier = options.get("person_pod_multipliers") if options else None
 
         if pod_multiplier is not None:
             self.raise_if_unvalid_mult(pod_multiplier)
             for person, mult in zip(self.persons_set, pod_multiplier):
                 person.set_mult(mult)
+            
+
+        self.probability_matrix = ProbabilityMatrix(
+            40,
+            self.dispersion_start,
+            self.dispersion_inc,
+            self.vector,
+            [
+                self.disaster_position[1],
+                self.disaster_position[0],
+            ],
+            self.grid_size,
+        )
+
+        self.probability_matrix.update_time_step_relation(
+            self.time_step_relation, self.cell_size
+        )
 
         observations, infos = super().reset(seed=seed, options=options)
         self.rewards_sum = {a: 0 for a in self.agents}
         self.rewards_sum["total"] = 0
         return observations, infos
 
     def raise_if_unvalid_mult(self, individual_multiplication: list[int]) -> bool:
@@ -206,15 +236,14 @@
 
             drone_action = actions[agent]
             if drone_action not in self.action_space(agent):
                 raise ValueError("Invalid action for " + agent)
 
             # Check truncation conditions (overwrites termination conditions)
             if self.timestep >= self.timestep_limit:
-                # TODO: Check if is really necessary to add rewards_sum into this reward
                 rewards[agent] = self.reward_scheme.exceed_timestep
                 if self.rewards_sum[agent] > 0:
                     rewards[agent] += self.rewards_sum[agent] // 2
                 truncations[agent] = True
                 terminations[agent] = True
                 continue
 
@@ -269,17 +298,14 @@
 
         self.timestep += 1
         # Get dummy infos
         infos = {drone: {"Found": person_found} for drone in self.agents}
 
         # CHECK COLISION - Drone
         self.compute_drone_collision(terminations, rewards)
-        # TODO: Check real usage of this, gives error when using w/ RL libs
-        # rewards["total_reward"] = sum(rewards.values())
-        # self.rewards_sum["total"] += rewards["total_reward"]
 
         self.render_step(any(terminations.values()), person_found)
 
         # Get observations
         observations = self.create_observations()
         # If terminated, reset the agents (pettingzoo parallel env requirement)
         if any(terminations.values()) or any(truncations.values()):
```

### Comparing `dsse-1.0.3/DSSE/environment/env_base.py` & `dsse-1.1.1/DSSE/environment/env_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,35 +13,25 @@
 class DroneSwarmSearchBase(ABC, ParallelEnv):
     def __init__(
         self,
         grid_size=7,
         render_mode="ansi",
         render_grid=False,
         render_gradient=True,
-        vector=(1, -0.5),
-        dispersion_inc=0.1,
-        dispersion_start=0.5,
         timestep_limit=100,
-        disaster_position=(0, 0),
         drone_amount=1,
         drone_speed=10,
         probability_of_detection=1,
-        pre_render_time=0,
     ) -> None:
         self.cell_size = 130  # in meters
         self.grid_size = grid_size
         self._was_reset = False
-        self.pre_render_steps = round(
-            (pre_render_time * 60)
-            / (self.calculate_simulation_time_step(drone_speed, self.cell_size))
-        )
-
-        print(f"Pre render time: {pre_render_time} minutes")
-        print(f"Pre render steps: {self.pre_render_steps}")
-
+        if not isinstance(drone_amount, int):
+            raise ValueError("Drone amount must be an integer")
+    
         self.drone = DroneData(
             amount=drone_amount,
             speed=drone_speed,
             pod=probability_of_detection,
         )
         self.probability_of_detection = probability_of_detection
 
@@ -55,27 +45,22 @@
             raise ValueError("Render mode not recognized")
 
         self.timestep = None
         self.timestep_limit = timestep_limit
         self.time_step_relation = self.calculate_simulation_time_step(
             self.drone.speed, self.cell_size
         )
-        self.dispersion_inc = dispersion_inc
-        self.dispersion_start = dispersion_start
-        self.vector = vector
-        self.disaster_position = disaster_position
 
         self.possible_agents = []
         self.agents_positions = [(None, None)] * self.drone.amount
         for i in range(self.drone.amount):
             agent_name = "drone" + str(i)
             self.possible_agents.append(agent_name)
 
         self.render_mode = render_mode
-        self.probability_matrix = None
 
         # Initializing render
         self.pygame_renderer = PygameInterface(
             self.grid_size, render_gradient, render_grid
         )
 
     def calculate_simulation_time_step(
@@ -102,41 +87,24 @@
     @abstractmethod
     def reset(
         self,
         seed=None,
         options=None,
     ):
         self._was_reset = True
-        vector = options.get("vector") if options else None
         drones_positions = options.get("drones_positions") if options else None
 
         if drones_positions is not None:
             if not self.is_valid_position_drones(drones_positions):
                 raise ValueError(
                     "You are trying to place the drone in a invalid position"
                 )
 
         self.agents = copy(self.possible_agents)
         self.timestep = 0
-        self.vector = vector if vector else self.vector
-        self.probability_matrix = ProbabilityMatrix(
-            40,
-            self.dispersion_start,
-            self.dispersion_inc,
-            self.vector,
-            [
-                self.disaster_position[1],
-                self.disaster_position[0],
-            ],
-            self.grid_size,
-        )
-
-        self.probability_matrix.update_time_step_relation(
-            self.time_step_relation, self.cell_size
-        )
 
         if drones_positions is None:
             self.default_drones_positions()
         else:
             self.required_drone_positions(drones_positions)
 
         if self.render_mode == "human":
```

### Comparing `dsse-1.0.3/DSSE/environment/pygame_interface.py` & `dsse-1.1.1/DSSE/environment/pygame_interface.py`

 * *Files identical despite different names*

### Comparing `dsse-1.0.3/DSSE/environment/simulation/dynamic_probability.py` & `dsse-1.1.1/DSSE/environment/simulation/dynamic_probability.py`

 * *Files identical despite different names*

### Comparing `dsse-1.0.3/DSSE/environment/simulation/time_step.py` & `dsse-1.1.1/DSSE/environment/simulation/time_step.py`

 * *Files identical despite different names*

### Comparing `dsse-1.0.3/DSSE/tests/drone_policy.py` & `dsse-1.1.1/DSSE/tests/drone_policy.py`

 * *Files identical despite different names*

### Comparing `dsse-1.0.3/DSSE/tests/test_env.py` & `dsse-1.1.1/DSSE/tests/test_env.py`

 * *Files identical despite different names*

### Comparing `dsse-1.0.3/DSSE/tests/test_matrix.py` & `dsse-1.1.1/DSSE/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `dsse-1.0.3/DSSE.egg-info/PKG-INFO` & `dsse-1.1.1/DSSE.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,90 @@
 Metadata-Version: 2.1
 Name: DSSE
-Version: 1.0.3
-Summary: An environment to train drones to search and find a shipwrecked person lost in the ocean using reinforcement learning.
-Home-page: https://github.com/pfeinsper/drone-swarm-search
-Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v1.0.3.tar.gz
-Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta, Jorás Oliveira, Ricardo Ribeiro Rodrigues, Renato Laffranchi Falcão, Pedro Henrique Britto Aragão Andrade, Fabricio Barth
-License: MIT
-Keywords: Reinforcement Learning,AI,SAR,Multi Agent
+Version: 1.1.1
+Summary: The Drone Swarm Search project provides an environment for SAR missions built on PettingZoo, where agents, represented by drones, are tasked with locating targets identified as shipwrecked individuals.
+Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v1.1.1.tar.gz
+Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta
+Author-email: Ricardo Ribeiro Rodrigues <ricardorr7@al.insper.edu.br>, Renato Laffranchi Falcão <renatolf1@al.insper.edu.br>, Pedro Henrique Britto Aragão Andrade <pedroa3@al.insper.edu.br>, Jorás Oliveira <jorascco@al.insper.edu.br>, Fabricio Barth <fabriciojb@insper.edu.br>
+License: MIT License
+Project-URL: Homepage, https://pfeinsper.github.io/drone-swarm-search/
+Project-URL: Repository, https://github.com/pfeinsper/drone-swarm-search/
+Project-URL: Documentation, https://pfeinsper.github.io/drone-swarm-search/
+Project-URL: Bug Report, https://github.com/pfeinsper/drone-swarm-search/issues/
+Keywords: Reinforcement Learning,AI,SAR,Multi Agent Reinforcement Learning
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.10.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: gymnasium
-Requires-Dist: pygame
-Requires-Dist: pettingzoo
-Requires-Dist: matplotlib
-Requires-Dist: numba
+Requires-Dist: numpy>=1.23.1
+Requires-Dist: gymnasium>=0.27.1
+Requires-Dist: pygame>=2.3.0
+Requires-Dist: pettingzoo>=1.22.3
+Requires-Dist: matplotlib>=3.7.0
+Requires-Dist: numba>=0.59.0
+Provides-Extra: all
+Requires-Dist: numpy>=1.23.1; extra == "all"
+Requires-Dist: gymnasium>=0.27.1; extra == "all"
+Requires-Dist: pygame>=2.3.0; extra == "all"
+Requires-Dist: pettingzoo>=1.22.3; extra == "all"
+Requires-Dist: matplotlib>=3.7.0; extra == "all"
+Requires-Dist: numba>=0.59.0; extra == "all"
+Requires-Dist: GDAL==3.4.1; extra == "all"
+Requires-Dist: opendrift; extra == "all"
+Provides-Extra: coverage
+Requires-Dist: GDAL==3.4.1; extra == "coverage"
+Requires-Dist: opendrift; extra == "coverage"
 
 [![Tests Status 🧪](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/env.yml/badge.svg)](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/env.yml)
 [![Docs Deployment 📝](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/deploy.yml/badge.svg?branch=vitepress_docs)](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/deploy.yml)
 [![PyPI Release 🚀](https://badge.fury.io/py/DSSE.svg)](https://badge.fury.io/py/DSSE)
 [![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg?style=flat)](https://github.com/pfeinsper/drone-swarm-search/blob/main/LICENSE)
 [![PettingZoo version dependency](https://img.shields.io/badge/PettingZoo-v1.22.3-blue)]()
 ![GitHub stars](https://img.shields.io/github/stars/pfeinsper/drone-swarm-search)
 
-## Documentation Links
+# <img src="https://github.com/pfeinsper/drone-swarm-search/blob/main/docs/public/pics/drone.svg" alt="DSSE Icon" width="45" height="25"> Drone Swarm Search Environment (DSSE)
+
+Welcome to the official GitHub repository for the Drone Swarm Search Environment (DSSE). This project is dedicated to providing a comprehensive simulation environment designed to develop, test, and refine drone swarm search strategies. Here, researchers and developers can access a versatile platform that supports a wide range of drone swarm simulations, enabling the exploration of complex behaviors and interactions within dynamic, real-world scenarios.
+
+
+## 📚 Documentation Links
 
 - **[Documentation Site](https://pfeinsper.github.io/drone-swarm-search/)**: Access comprehensive documentation including tutorials, and usage examples for the Drone Swarm Search Environment (DSSE). Ideal for users seeking detailed information about the project's capabilities and how to integrate them into their own applications.
 
 - **[Algorithm Details](https://github.com/pfeinsper/drone-swarm-search-algorithms)**: Explore in-depth discussions and source code for the algorithms powering the DSSE. This section is perfect for developers interested in the technical underpinnings and enhancements of the search algorithms.
 
 - **[PyPI Repository](https://pypi.org/project/DSSE/)**: Visit the PyPI page for DSSE to download the latest release, view release histories, and read additional installation instructions.
 
-## Visual Demonstrations
+## 🎥 Visual Demonstrations
 <p align="center">
     <img src="https://raw.github.com/PFE-Embraer/drone-swarm-search/env-cleanup/docs/gifs/render_with_grid_gradient.gif" width="400" height="400" align="center">
     <br>
     <em>Above: A simulation showing how drones adjust their search pattern over a grid.</em>
 </p>
 
-## Quick Start
+## ⚡Quick Start
 
-### Installation
+### ⚙️ Installation
 Install DSSE quickly with pip:
 ```bash
 pip install DSSE
 ````
 
-## Outcome
+## 🎯 Outcome
 
-| If drone is found            | If drone is not found  |
+| If target is found       | If target is not found   |
 :-------------------------:|:-------------------------:
-| ![](https://raw.githubusercontent.com/PFE-Embraer/drone-swarm-search/main/docs/pics/victory_render.png)     | ![](https://raw.github.com/PFE-Embraer/drone-swarm-search/main/docs/pics/fail_render.png) |
+| ![](https://raw.githubusercontent.com/PFE-Embraer/drone-swarm-search/main/docs/public/pics/victory_render.png)     | ![](https://raw.github.com/PFE-Embraer/drone-swarm-search/main/docs/public/pics/fail_render.png) |
 
 
-## Basic Env Usage
+## 🛠️ Basic Env Usage
 ```python
 from DSSE import DroneSwarmSearch
 
 env = DroneSwarmSearch(
     grid_size=40,
     render_mode="human",
     render_grid=True,
@@ -91,15 +118,15 @@
 done = False
 while not done:
     actions = random_policy(observations, env.get_agents())
     observations, rewards, terminations, truncations, infos = env.step(actions)
     done = any(terminations.values()) or any(truncations.values())
 ```
 
-## Basic Covarage Usage
+## 🛠️ Basic Coverage Usage
 ```python
 from DSSE import CoverageDroneSwarmSearch
 
 env = CoverageDroneSwarmSearch(
     grid_size=40,
     drone_amount=3,
     dispersion_inc=0.1,
@@ -117,26 +144,26 @@
     step += 1
     actions = {agent: env.action_space(agent).sample() for agent in env.agents}
     observations, rewards, terminations, truncations, infos = env.step(actions)
 
 print(infos["drone0"])
 ```
 
-## Support
+## 🆘 Support
 
 If you encounter any issues or have questions, please file an issue on our [GitHub issues page](https://github.com/pfeinsper/drone-swarm-search/issues).
 
-## How to cite this work
+## 📖 How to cite this work
 
 If you use this package, please consider citing it with this piece of BibTeX:
 
 ```
 @misc{castanares2023dsse,
       title={DSSE: a drone swarm search environment}, 
-      author={Jorás Oliveira, Pedro Andrade, Ricardo Rodrigues, Renato Laffranchi,Manuel Castanares, Luis F. S. Carrete, Enrico F. Damiani, Leonardo D. M. de Abreu, José Fernando B. Brancalion and Fabrício J. Barth},
+      author={Manuel Castanares, Luis F. S. Carrete, Enrico F. Damiani, Leonardo D. M. de Abreu, José Fernando B. Brancalion and Fabrício J. Barth},
       year={2024},
       eprint={2307.06240},
       archivePrefix={arXiv},
       primaryClass={cs.LG},
       doi={https://doi.org/10.48550/arXiv.2307.06240}
 }
 ```
```

### Comparing `dsse-1.0.3/DSSE.egg-info/SOURCES.txt` & `dsse-1.1.1/DSSE.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 setup.py
 DSSE/__init__.py
 DSSE.egg-info/PKG-INFO
 DSSE.egg-info/SOURCES.txt
 DSSE.egg-info/dependency_links.txt
 DSSE.egg-info/requires.txt
 DSSE.egg-info/top_level.txt
@@ -13,18 +14,17 @@
 DSSE/environment/coverage_env.py
 DSSE/environment/env.py
 DSSE/environment/env_base.py
 DSSE/environment/pygame_interface.py
 DSSE/environment/entities/__init__.py
 DSSE/environment/entities/drone.py
 DSSE/environment/entities/person.py
-DSSE/environment/imgs/drone.png
-DSSE/environment/imgs/person-swimming.png
 DSSE/environment/simulation/__init__.py
 DSSE/environment/simulation/dynamic_probability.py
-DSSE/environment/simulation/particle_sim.py
+DSSE/environment/simulation/particle_simulation.py
 DSSE/environment/simulation/time_step.py
+DSSE/environment/wrappers/all_positions_wrapper.py
 DSSE/tests/__init__.py
 DSSE/tests/drone_policy.py
 DSSE/tests/test_env.py
 DSSE/tests/test_env_coverage.py
 DSSE/tests/test_matrix.py
```

### Comparing `dsse-1.0.3/LICENSE` & `dsse-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dsse-1.0.3/PKG-INFO` & `dsse-1.1.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,90 @@
 Metadata-Version: 2.1
 Name: DSSE
-Version: 1.0.3
-Summary: An environment to train drones to search and find a shipwrecked person lost in the ocean using reinforcement learning.
-Home-page: https://github.com/pfeinsper/drone-swarm-search
-Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v1.0.3.tar.gz
-Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta, Jorás Oliveira, Ricardo Ribeiro Rodrigues, Renato Laffranchi Falcão, Pedro Henrique Britto Aragão Andrade, Fabricio Barth
-License: MIT
-Keywords: Reinforcement Learning,AI,SAR,Multi Agent
+Version: 1.1.1
+Summary: The Drone Swarm Search project provides an environment for SAR missions built on PettingZoo, where agents, represented by drones, are tasked with locating targets identified as shipwrecked individuals.
+Download-URL: https://github.com/pfeinsper/drone-swarm-search/archive/refs/tags/v1.1.1.tar.gz
+Author: Luis Filipe Carrete, Manuel Castanares, Enrico Damiani, Leonardo Malta
+Author-email: Ricardo Ribeiro Rodrigues <ricardorr7@al.insper.edu.br>, Renato Laffranchi Falcão <renatolf1@al.insper.edu.br>, Pedro Henrique Britto Aragão Andrade <pedroa3@al.insper.edu.br>, Jorás Oliveira <jorascco@al.insper.edu.br>, Fabricio Barth <fabriciojb@insper.edu.br>
+License: MIT License
+Project-URL: Homepage, https://pfeinsper.github.io/drone-swarm-search/
+Project-URL: Repository, https://github.com/pfeinsper/drone-swarm-search/
+Project-URL: Documentation, https://pfeinsper.github.io/drone-swarm-search/
+Project-URL: Bug Report, https://github.com/pfeinsper/drone-swarm-search/issues/
+Keywords: Reinforcement Learning,AI,SAR,Multi Agent Reinforcement Learning
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Python: >=3.10.5
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: gymnasium
-Requires-Dist: pygame
-Requires-Dist: pettingzoo
-Requires-Dist: matplotlib
-Requires-Dist: numba
+Requires-Dist: numpy>=1.23.1
+Requires-Dist: gymnasium>=0.27.1
+Requires-Dist: pygame>=2.3.0
+Requires-Dist: pettingzoo>=1.22.3
+Requires-Dist: matplotlib>=3.7.0
+Requires-Dist: numba>=0.59.0
+Provides-Extra: all
+Requires-Dist: numpy>=1.23.1; extra == "all"
+Requires-Dist: gymnasium>=0.27.1; extra == "all"
+Requires-Dist: pygame>=2.3.0; extra == "all"
+Requires-Dist: pettingzoo>=1.22.3; extra == "all"
+Requires-Dist: matplotlib>=3.7.0; extra == "all"
+Requires-Dist: numba>=0.59.0; extra == "all"
+Requires-Dist: GDAL==3.4.1; extra == "all"
+Requires-Dist: opendrift; extra == "all"
+Provides-Extra: coverage
+Requires-Dist: GDAL==3.4.1; extra == "coverage"
+Requires-Dist: opendrift; extra == "coverage"
 
 [![Tests Status 🧪](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/env.yml/badge.svg)](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/env.yml)
 [![Docs Deployment 📝](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/deploy.yml/badge.svg?branch=vitepress_docs)](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/deploy.yml)
 [![PyPI Release 🚀](https://badge.fury.io/py/DSSE.svg)](https://badge.fury.io/py/DSSE)
 [![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg?style=flat)](https://github.com/pfeinsper/drone-swarm-search/blob/main/LICENSE)
 [![PettingZoo version dependency](https://img.shields.io/badge/PettingZoo-v1.22.3-blue)]()
 ![GitHub stars](https://img.shields.io/github/stars/pfeinsper/drone-swarm-search)
 
-## Documentation Links
+# <img src="https://github.com/pfeinsper/drone-swarm-search/blob/main/docs/public/pics/drone.svg" alt="DSSE Icon" width="45" height="25"> Drone Swarm Search Environment (DSSE)
+
+Welcome to the official GitHub repository for the Drone Swarm Search Environment (DSSE). This project is dedicated to providing a comprehensive simulation environment designed to develop, test, and refine drone swarm search strategies. Here, researchers and developers can access a versatile platform that supports a wide range of drone swarm simulations, enabling the exploration of complex behaviors and interactions within dynamic, real-world scenarios.
+
+
+## 📚 Documentation Links
 
 - **[Documentation Site](https://pfeinsper.github.io/drone-swarm-search/)**: Access comprehensive documentation including tutorials, and usage examples for the Drone Swarm Search Environment (DSSE). Ideal for users seeking detailed information about the project's capabilities and how to integrate them into their own applications.
 
 - **[Algorithm Details](https://github.com/pfeinsper/drone-swarm-search-algorithms)**: Explore in-depth discussions and source code for the algorithms powering the DSSE. This section is perfect for developers interested in the technical underpinnings and enhancements of the search algorithms.
 
 - **[PyPI Repository](https://pypi.org/project/DSSE/)**: Visit the PyPI page for DSSE to download the latest release, view release histories, and read additional installation instructions.
 
-## Visual Demonstrations
+## 🎥 Visual Demonstrations
 <p align="center">
     <img src="https://raw.github.com/PFE-Embraer/drone-swarm-search/env-cleanup/docs/gifs/render_with_grid_gradient.gif" width="400" height="400" align="center">
     <br>
     <em>Above: A simulation showing how drones adjust their search pattern over a grid.</em>
 </p>
 
-## Quick Start
+## ⚡Quick Start
 
-### Installation
+### ⚙️ Installation
 Install DSSE quickly with pip:
 ```bash
 pip install DSSE
 ````
 
-## Outcome
+## 🎯 Outcome
 
-| If drone is found            | If drone is not found  |
+| If target is found       | If target is not found   |
 :-------------------------:|:-------------------------:
-| ![](https://raw.githubusercontent.com/PFE-Embraer/drone-swarm-search/main/docs/pics/victory_render.png)     | ![](https://raw.github.com/PFE-Embraer/drone-swarm-search/main/docs/pics/fail_render.png) |
+| ![](https://raw.githubusercontent.com/PFE-Embraer/drone-swarm-search/main/docs/public/pics/victory_render.png)     | ![](https://raw.github.com/PFE-Embraer/drone-swarm-search/main/docs/public/pics/fail_render.png) |
 
 
-## Basic Env Usage
+## 🛠️ Basic Env Usage
 ```python
 from DSSE import DroneSwarmSearch
 
 env = DroneSwarmSearch(
     grid_size=40,
     render_mode="human",
     render_grid=True,
@@ -91,15 +118,15 @@
 done = False
 while not done:
     actions = random_policy(observations, env.get_agents())
     observations, rewards, terminations, truncations, infos = env.step(actions)
     done = any(terminations.values()) or any(truncations.values())
 ```
 
-## Basic Covarage Usage
+## 🛠️ Basic Coverage Usage
 ```python
 from DSSE import CoverageDroneSwarmSearch
 
 env = CoverageDroneSwarmSearch(
     grid_size=40,
     drone_amount=3,
     dispersion_inc=0.1,
@@ -117,26 +144,26 @@
     step += 1
     actions = {agent: env.action_space(agent).sample() for agent in env.agents}
     observations, rewards, terminations, truncations, infos = env.step(actions)
 
 print(infos["drone0"])
 ```
 
-## Support
+## 🆘 Support
 
 If you encounter any issues or have questions, please file an issue on our [GitHub issues page](https://github.com/pfeinsper/drone-swarm-search/issues).
 
-## How to cite this work
+## 📖 How to cite this work
 
 If you use this package, please consider citing it with this piece of BibTeX:
 
 ```
 @misc{castanares2023dsse,
       title={DSSE: a drone swarm search environment}, 
-      author={Jorás Oliveira, Pedro Andrade, Ricardo Rodrigues, Renato Laffranchi,Manuel Castanares, Luis F. S. Carrete, Enrico F. Damiani, Leonardo D. M. de Abreu, José Fernando B. Brancalion and Fabrício J. Barth},
+      author={Manuel Castanares, Luis F. S. Carrete, Enrico F. Damiani, Leonardo D. M. de Abreu, José Fernando B. Brancalion and Fabrício J. Barth},
       year={2024},
       eprint={2307.06240},
       archivePrefix={arXiv},
       primaryClass={cs.LG},
       doi={https://doi.org/10.48550/arXiv.2307.06240}
 }
 ```
```

### Comparing `dsse-1.0.3/README.md` & `dsse-1.1.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,45 +1,50 @@
 [![Tests Status 🧪](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/env.yml/badge.svg)](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/env.yml)
 [![Docs Deployment 📝](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/deploy.yml/badge.svg?branch=vitepress_docs)](https://github.com/pfeinsper/drone-swarm-search/actions/workflows/deploy.yml)
 [![PyPI Release 🚀](https://badge.fury.io/py/DSSE.svg)](https://badge.fury.io/py/DSSE)
 [![License: MIT](https://img.shields.io/badge/License-MIT-brightgreen.svg?style=flat)](https://github.com/pfeinsper/drone-swarm-search/blob/main/LICENSE)
 [![PettingZoo version dependency](https://img.shields.io/badge/PettingZoo-v1.22.3-blue)]()
 ![GitHub stars](https://img.shields.io/github/stars/pfeinsper/drone-swarm-search)
 
-## Documentation Links
+# <img src="https://github.com/pfeinsper/drone-swarm-search/blob/main/docs/public/pics/drone.svg" alt="DSSE Icon" width="45" height="25"> Drone Swarm Search Environment (DSSE)
+
+Welcome to the official GitHub repository for the Drone Swarm Search Environment (DSSE). This project is dedicated to providing a comprehensive simulation environment designed to develop, test, and refine drone swarm search strategies. Here, researchers and developers can access a versatile platform that supports a wide range of drone swarm simulations, enabling the exploration of complex behaviors and interactions within dynamic, real-world scenarios.
+
+
+## 📚 Documentation Links
 
 - **[Documentation Site](https://pfeinsper.github.io/drone-swarm-search/)**: Access comprehensive documentation including tutorials, and usage examples for the Drone Swarm Search Environment (DSSE). Ideal for users seeking detailed information about the project's capabilities and how to integrate them into their own applications.
 
 - **[Algorithm Details](https://github.com/pfeinsper/drone-swarm-search-algorithms)**: Explore in-depth discussions and source code for the algorithms powering the DSSE. This section is perfect for developers interested in the technical underpinnings and enhancements of the search algorithms.
 
 - **[PyPI Repository](https://pypi.org/project/DSSE/)**: Visit the PyPI page for DSSE to download the latest release, view release histories, and read additional installation instructions.
 
-## Visual Demonstrations
+## 🎥 Visual Demonstrations
 <p align="center">
     <img src="https://raw.github.com/PFE-Embraer/drone-swarm-search/env-cleanup/docs/gifs/render_with_grid_gradient.gif" width="400" height="400" align="center">
     <br>
     <em>Above: A simulation showing how drones adjust their search pattern over a grid.</em>
 </p>
 
-## Quick Start
+## ⚡Quick Start
 
-### Installation
+### ⚙️ Installation
 Install DSSE quickly with pip:
 ```bash
 pip install DSSE
 ````
 
-## Outcome
+## 🎯 Outcome
 
-| If drone is found            | If drone is not found  |
+| If target is found       | If target is not found   |
 :-------------------------:|:-------------------------:
-| ![](https://raw.githubusercontent.com/PFE-Embraer/drone-swarm-search/main/docs/pics/victory_render.png)     | ![](https://raw.github.com/PFE-Embraer/drone-swarm-search/main/docs/pics/fail_render.png) |
+| ![](https://raw.githubusercontent.com/PFE-Embraer/drone-swarm-search/main/docs/public/pics/victory_render.png)     | ![](https://raw.github.com/PFE-Embraer/drone-swarm-search/main/docs/public/pics/fail_render.png) |
 
 
-## Basic Env Usage
+## 🛠️ Basic Env Usage
 ```python
 from DSSE import DroneSwarmSearch
 
 env = DroneSwarmSearch(
     grid_size=40,
     render_mode="human",
     render_grid=True,
@@ -73,15 +78,15 @@
 done = False
 while not done:
     actions = random_policy(observations, env.get_agents())
     observations, rewards, terminations, truncations, infos = env.step(actions)
     done = any(terminations.values()) or any(truncations.values())
 ```
 
-## Basic Covarage Usage
+## 🛠️ Basic Coverage Usage
 ```python
 from DSSE import CoverageDroneSwarmSearch
 
 env = CoverageDroneSwarmSearch(
     grid_size=40,
     drone_amount=3,
     dispersion_inc=0.1,
@@ -99,26 +104,26 @@
     step += 1
     actions = {agent: env.action_space(agent).sample() for agent in env.agents}
     observations, rewards, terminations, truncations, infos = env.step(actions)
 
 print(infos["drone0"])
 ```
 
-## Support
+## 🆘 Support
 
 If you encounter any issues or have questions, please file an issue on our [GitHub issues page](https://github.com/pfeinsper/drone-swarm-search/issues).
 
-## How to cite this work
+## 📖 How to cite this work
 
 If you use this package, please consider citing it with this piece of BibTeX:
 
 ```
 @misc{castanares2023dsse,
       title={DSSE: a drone swarm search environment}, 
-      author={Jorás Oliveira, Pedro Andrade, Ricardo Rodrigues, Renato Laffranchi,Manuel Castanares, Luis F. S. Carrete, Enrico F. Damiani, Leonardo D. M. de Abreu, José Fernando B. Brancalion and Fabrício J. Barth},
+      author={Manuel Castanares, Luis F. S. Carrete, Enrico F. Damiani, Leonardo D. M. de Abreu, José Fernando B. Brancalion and Fabrício J. Barth},
       year={2024},
       eprint={2307.06240},
       archivePrefix={arXiv},
       primaryClass={cs.LG},
       doi={https://doi.org/10.48550/arXiv.2307.06240}
 }
 ```
```

