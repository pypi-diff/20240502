# Comparing `tmp/cc512_evolution-0.1.1.tar.gz` & `tmp/cc512_evolution-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cc512_evolution-0.1.1.tar", max compression
+gzip compressed data, was "cc512_evolution-1.0.0.tar", max compression
```

## Comparing `cc512_evolution-0.1.1.tar` & `cc512_evolution-1.0.0.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0        0 2024-04-20 16:48:16.722884 cc512_evolution-0.1.1/README.md
--rw-r--r--   0        0        0      414 2024-05-02 01:37:20.373243 cc512_evolution-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       80 2024-05-01 15:27:09.336087 cc512_evolution-0.1.1/src/evolution/__init__.py
--rw-r--r--   0        0        0      354 2024-05-01 10:53:16.697215 cc512_evolution-0.1.1/src/evolution/encoding/__init__.py
--rw-r--r--   0        0        0     2775 2024-05-01 19:22:53.755082 cc512_evolution-0.1.1/src/evolution/encoding/base.py
--rw-r--r--   0        0        0     2421 2024-05-01 17:43:12.613572 cc512_evolution-0.1.1/src/evolution/encoding/binary.py
--rw-r--r--   0        0        0     2034 2024-05-01 12:32:18.671279 cc512_evolution-0.1.1/src/evolution/encoding/gray.py
--rw-r--r--   0        0        0     1506 2024-04-20 12:41:59.068191 cc512_evolution-0.1.1/src/evolution/encoding/gray_code.py
--rw-r--r--   0        0        0     4772 2024-05-01 19:04:10.318473 cc512_evolution-0.1.1/src/evolution/encoding/interval.py
--rw-r--r--   0        0        0     7084 2024-05-02 00:31:10.955719 cc512_evolution-0.1.1/src/evolution/evolution.py
--rw-r--r--   0        0        0      382 2024-04-28 05:36:30.660588 cc512_evolution-0.1.1/src/evolution/fitness.py
--rw-r--r--   0        0        0     1091 2024-05-01 20:01:00.912595 cc512_evolution-0.1.1/src/evolution/population.py
--rw-r--r--   0        0        0      179 2024-05-01 23:44:32.151131 cc512_evolution-0.1.1/src/evolution/selection/__init__.py
--rw-r--r--   0        0        0      487 2024-05-01 15:28:52.057254 cc512_evolution-0.1.1/src/evolution/selection/base.py
--rw-r--r--   0        0        0      168 2024-05-01 20:27:18.061307 cc512_evolution-0.1.1/src/evolution/selection/misc.py
--rw-r--r--   0        0        0      762 2024-05-01 19:07:59.046499 cc512_evolution-0.1.1/src/evolution/selection/proportional2fitness.py
--rw-r--r--   0        0        0      802 2024-05-01 23:43:39.304984 cc512_evolution-0.1.1/src/evolution/selection/proportional2inversefitness.py
--rw-r--r--   0        0        0     1657 2024-04-28 06:27:18.505872 cc512_evolution-0.1.1/src/evolution/selection/rank_based_exponential_classification.py
--rw-r--r--   0        0        0     1547 2024-04-28 06:28:09.901230 cc512_evolution-0.1.1/src/evolution/selection/rank_based_linear_classification.py
--rw-r--r--   0        0        0     2011 2024-04-28 06:51:23.729483 cc512_evolution-0.1.1/src/evolution/selection/roulette.py
--rw-r--r--   0        0        0     2409 2024-04-28 06:45:40.145945 cc512_evolution-0.1.1/src/evolution/selection/tournament.py
--rw-r--r--   0        0        0      862 2024-04-28 06:49:12.924329 cc512_evolution-0.1.1/src/evolution/selection/uniform.py
--rw-r--r--   0        0        0        0 2024-05-01 14:45:46.565897 cc512_evolution-0.1.1/src/evolution/variation/__init__.py
--rw-r--r--   0        0        0      159 2024-05-01 14:47:11.100554 cc512_evolution-0.1.1/src/evolution/variation/crossover/__init__.py
--rw-r--r--   0        0        0      315 2024-05-01 17:07:45.009487 cc512_evolution-0.1.1/src/evolution/variation/crossover/base.py
--rw-r--r--   0        0        0     1478 2024-05-01 19:59:49.362851 cc512_evolution-0.1.1/src/evolution/variation/crossover/bit.py
--rw-r--r--   0        0        0      553 2024-04-20 13:27:30.081869 cc512_evolution-0.1.1/src/evolution/variation/crossover/cross_gen.py
--rw-r--r--   0        0        0      157 2024-05-01 14:49:17.034398 cc512_evolution-0.1.1/src/evolution/variation/mutation/__init__.py
--rw-r--r--   0        0        0      255 2024-05-01 15:33:04.707998 cc512_evolution-0.1.1/src/evolution/variation/mutation/base.py
--rw-r--r--   0        0        0      864 2024-05-01 19:54:38.030414 cc512_evolution-0.1.1/src/evolution/variation/mutation/bit.py
--rw-r--r--   0        0        0      443 1970-01-01 00:00:00.000000 cc512_evolution-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-20 16:48:16.722884 cc512_evolution-1.0.0/README.md
+-rw-r--r--   0        0        0      413 2024-05-02 01:49:23.420787 cc512_evolution-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0       80 2024-05-01 15:27:09.336087 cc512_evolution-1.0.0/src/evolution/__init__.py
+-rw-r--r--   0        0        0      354 2024-05-01 10:53:16.697215 cc512_evolution-1.0.0/src/evolution/encoding/__init__.py
+-rw-r--r--   0        0        0     2775 2024-05-01 19:22:53.755082 cc512_evolution-1.0.0/src/evolution/encoding/base.py
+-rw-r--r--   0        0        0     2421 2024-05-01 17:43:12.613572 cc512_evolution-1.0.0/src/evolution/encoding/binary.py
+-rw-r--r--   0        0        0     2034 2024-05-01 12:32:18.671279 cc512_evolution-1.0.0/src/evolution/encoding/gray.py
+-rw-r--r--   0        0        0     1506 2024-04-20 12:41:59.068191 cc512_evolution-1.0.0/src/evolution/encoding/gray_code.py
+-rw-r--r--   0        0        0     4772 2024-05-01 19:04:10.318473 cc512_evolution-1.0.0/src/evolution/encoding/interval.py
+-rw-r--r--   0        0        0     7826 2024-05-02 01:42:56.137791 cc512_evolution-1.0.0/src/evolution/evolution.py
+-rw-r--r--   0        0        0      382 2024-04-28 05:36:30.660588 cc512_evolution-1.0.0/src/evolution/fitness.py
+-rw-r--r--   0        0        0     1091 2024-05-01 20:01:00.912595 cc512_evolution-1.0.0/src/evolution/population.py
+-rw-r--r--   0        0        0      179 2024-05-01 23:44:32.151131 cc512_evolution-1.0.0/src/evolution/selection/__init__.py
+-rw-r--r--   0        0        0      487 2024-05-01 15:28:52.057254 cc512_evolution-1.0.0/src/evolution/selection/base.py
+-rw-r--r--   0        0        0      168 2024-05-01 20:27:18.061307 cc512_evolution-1.0.0/src/evolution/selection/misc.py
+-rw-r--r--   0        0        0      762 2024-05-01 19:07:59.046499 cc512_evolution-1.0.0/src/evolution/selection/proportional2fitness.py
+-rw-r--r--   0        0        0      802 2024-05-01 23:43:39.304984 cc512_evolution-1.0.0/src/evolution/selection/proportional2inversefitness.py
+-rw-r--r--   0        0        0     1657 2024-04-28 06:27:18.505872 cc512_evolution-1.0.0/src/evolution/selection/rank_based_exponential_classification.py
+-rw-r--r--   0        0        0     1547 2024-04-28 06:28:09.901230 cc512_evolution-1.0.0/src/evolution/selection/rank_based_linear_classification.py
+-rw-r--r--   0        0        0     2011 2024-04-28 06:51:23.729483 cc512_evolution-1.0.0/src/evolution/selection/roulette.py
+-rw-r--r--   0        0        0     2409 2024-04-28 06:45:40.145945 cc512_evolution-1.0.0/src/evolution/selection/tournament.py
+-rw-r--r--   0        0        0      862 2024-04-28 06:49:12.924329 cc512_evolution-1.0.0/src/evolution/selection/uniform.py
+-rw-r--r--   0        0        0        0 2024-05-01 14:45:46.565897 cc512_evolution-1.0.0/src/evolution/variation/__init__.py
+-rw-r--r--   0        0        0      159 2024-05-01 14:47:11.100554 cc512_evolution-1.0.0/src/evolution/variation/crossover/__init__.py
+-rw-r--r--   0        0        0      315 2024-05-01 17:07:45.009487 cc512_evolution-1.0.0/src/evolution/variation/crossover/base.py
+-rw-r--r--   0        0        0     1478 2024-05-01 19:59:49.362851 cc512_evolution-1.0.0/src/evolution/variation/crossover/bit.py
+-rw-r--r--   0        0        0      553 2024-04-20 13:27:30.081869 cc512_evolution-1.0.0/src/evolution/variation/crossover/cross_gen.py
+-rw-r--r--   0        0        0      157 2024-05-01 14:49:17.034398 cc512_evolution-1.0.0/src/evolution/variation/mutation/__init__.py
+-rw-r--r--   0        0        0      255 2024-05-01 15:33:04.707998 cc512_evolution-1.0.0/src/evolution/variation/mutation/base.py
+-rw-r--r--   0        0        0      864 2024-05-01 19:54:38.030414 cc512_evolution-1.0.0/src/evolution/variation/mutation/bit.py
+-rw-r--r--   0        0        0      543 1970-01-01 00:00:00.000000 cc512_evolution-1.0.0/PKG-INFO
```

### Comparing `cc512_evolution-0.1.1/src/evolution/encoding/base.py` & `cc512_evolution-1.0.0/src/evolution/encoding/base.py`

 * *Files identical despite different names*

### Comparing `cc512_evolution-0.1.1/src/evolution/encoding/binary.py` & `cc512_evolution-1.0.0/src/evolution/encoding/binary.py`

 * *Files identical despite different names*

### Comparing `cc512_evolution-0.1.1/src/evolution/encoding/gray.py` & `cc512_evolution-1.0.0/src/evolution/encoding/gray.py`

 * *Files identical despite different names*

### Comparing `cc512_evolution-0.1.1/src/evolution/encoding/gray_code.py` & `cc512_evolution-1.0.0/src/evolution/encoding/gray_code.py`

 * *Files identical despite different names*

### Comparing `cc512_evolution-0.1.1/src/evolution/encoding/interval.py` & `cc512_evolution-1.0.0/src/evolution/encoding/interval.py`

 * *Files identical despite different names*

### Comparing `cc512_evolution-0.1.1/src/evolution/evolution.py` & `cc512_evolution-1.0.0/src/evolution/evolution.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,14 +106,32 @@
                     }
                 }
 
     def population_fitness(self) -> List[float]:
         """Compute the fitness of the current population"""
         return [self.fitness_func(individual) for individual in self.population]
 
+    def _evolve(self, max_generations: int, 
+                  selection: int, descendents: int, *args, **kwargs) -> Population:
+        """
+        perform the evolution of initial population using multiple variation operations
+        this method quits when max number of iteratons were done or the convergence condition was met
+
+        Inputs
+        =======
+        max_generations: maximun number of iterations (or generations - evolutions)
+        selection: number of parents selected fom current population (for generate next generation)
+        descendents: number of descendents to generate using variation operation over selected individuals
+
+        Output
+        ======
+        evolved population
+        """
+        pass
+    
 
     def evolve(self, max_generations: int, 
                   selection: int, descendents: int, *args, **kwargs) -> Population:
         """
         perform the evolution of initial population using multiple variation operations
         this method quits when max number of iteratons were done or the convergence condition was met
```

### Comparing `cc512_evolution-0.1.1/src/evolution/population.py` & `cc512_evolution-1.0.0/src/evolution/population.py`

 * *Files identical despite different names*

### Comparing `cc512_evolution-0.1.1/src/evolution/selection/proportional2fitness.py` & `cc512_evolution-1.0.0/src/evolution/selection/proportional2fitness.py`

 * *Files identical despite different names*

### Comparing `cc512_evolution-0.1.1/src/evolution/selection/proportional2inversefitness.py` & `cc512_evolution-1.0.0/src/evolution/selection/proportional2inversefitness.py`

 * *Files identical despite different names*

### Comparing `cc512_evolution-0.1.1/src/evolution/selection/rank_based_exponential_classification.py` & `cc512_evolution-1.0.0/src/evolution/selection/rank_based_exponential_classification.py`

 * *Files identical despite different names*

### Comparing `cc512_evolution-0.1.1/src/evolution/selection/rank_based_linear_classification.py` & `cc512_evolution-1.0.0/src/evolution/selection/rank_based_linear_classification.py`

 * *Files identical despite different names*

### Comparing `cc512_evolution-0.1.1/src/evolution/selection/roulette.py` & `cc512_evolution-1.0.0/src/evolution/selection/roulette.py`

 * *Files identical despite different names*

### Comparing `cc512_evolution-0.1.1/src/evolution/selection/tournament.py` & `cc512_evolution-1.0.0/src/evolution/selection/tournament.py`

 * *Files identical despite different names*

### Comparing `cc512_evolution-0.1.1/src/evolution/selection/uniform.py` & `cc512_evolution-1.0.0/src/evolution/selection/uniform.py`

 * *Files identical despite different names*

### Comparing `cc512_evolution-0.1.1/src/evolution/variation/crossover/bit.py` & `cc512_evolution-1.0.0/src/evolution/variation/crossover/bit.py`

 * *Files identical despite different names*

### Comparing `cc512_evolution-0.1.1/src/evolution/variation/crossover/cross_gen.py` & `cc512_evolution-1.0.0/src/evolution/variation/crossover/cross_gen.py`

 * *Files identical despite different names*

### Comparing `cc512_evolution-0.1.1/src/evolution/variation/mutation/bit.py` & `cc512_evolution-1.0.0/src/evolution/variation/mutation/bit.py`

 * *Files identical despite different names*

