# Comparing `tmp/me_toolbox-0.0.8.tar.gz` & `tmp/me_toolbox-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "me_toolbox-0.0.8.tar", last modified: Tue Mar 26 21:23:25 2024, max compression
+gzip compressed data, was "me_toolbox-0.0.9.tar", last modified: Sat Mar 30 20:16:39 2024, max compression
```

## Comparing `me_toolbox-0.0.8.tar` & `me_toolbox-0.0.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 21:23:25.463849 me_toolbox-0.0.8/
--rw-rw-rw-   0        0        0     1091 2021-04-12 19:58:49.000000 me_toolbox-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       37 2021-04-13 10:57:43.000000 me_toolbox-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1900 2024-03-26 21:23:25.447635 me_toolbox-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1170 2024-03-26 21:07:14.000000 me_toolbox-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-03-26 21:23:25.102455 me_toolbox-0.0.8/me_toolbox/
--rw-rw-rw-   0        0        0        0 2024-03-09 18:44:50.000000 me_toolbox-0.0.8/me_toolbox/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-26 21:23:25.188593 me_toolbox-0.0.8/me_toolbox/fasteners/
--rw-rw-rw-   0        0        0      172 2022-09-30 10:32:14.000000 me_toolbox-0.0.8/me_toolbox/fasteners/__init__.py
--rw-rw-rw-   0        0        0     7208 2024-03-24 19:43:47.000000 me_toolbox-0.0.8/me_toolbox/fasteners/bolt.py
--rw-rw-rw-   0        0        0    16759 2024-03-24 20:09:15.000000 me_toolbox-0.0.8/me_toolbox/fasteners/bolt_pattern.py
--rw-rw-rw-   0        0        0     1831 2022-09-30 13:56:11.000000 me_toolbox-0.0.8/me_toolbox/fasteners/test_bolt.py
--rw-rw-rw-   0        0        0     4714 2022-09-30 13:53:33.000000 me_toolbox-0.0.8/me_toolbox/fasteners/test_threaded_fastener.py
--rw-rw-rw-   0        0        0     7625 2024-03-24 20:16:47.000000 me_toolbox-0.0.8/me_toolbox/fasteners/threaded_fastener.py
-drwxrwxrwx   0        0        0        0 2024-03-26 21:23:25.229098 me_toolbox-0.0.8/me_toolbox/fatigue/
--rw-rw-rw-   0        0        0      236 2024-03-18 19:46:59.000000 me_toolbox-0.0.8/me_toolbox/fatigue/__init__.py
--rw-rw-rw-   0        0        0     6301 2024-03-18 19:20:28.000000 me_toolbox-0.0.8/me_toolbox/fatigue/endurance_limit.py
--rw-rw-rw-   0        0        0     6113 2024-03-20 10:28:30.000000 me_toolbox-0.0.8/me_toolbox/fatigue/failure_criteria.py
--rw-rw-rw-   0        0        0    18335 2024-03-20 20:43:04.000000 me_toolbox-0.0.8/me_toolbox/fatigue/fatigue_analysis.py
--rw-rw-rw-   0        0        0     2104 2021-04-19 20:13:15.000000 me_toolbox-0.0.8/me_toolbox/fatigue/stress.py
-drwxrwxrwx   0        0        0        0 2024-03-26 21:23:25.309955 me_toolbox-0.0.8/me_toolbox/gears/
--rw-rw-rw-   0        0        0      215 2021-04-21 10:01:28.000000 me_toolbox-0.0.8/me_toolbox/gears/__init__.py
--rw-rw-rw-   0        0        0    13524 2021-04-21 10:09:11.000000 me_toolbox-0.0.8/me_toolbox/gears/gear.py
--rw-rw-rw-   0        0        0    20348 2021-04-21 08:37:31.000000 me_toolbox-0.0.8/me_toolbox/gears/helical_gear.py
--rw-rw-rw-   0        0        0    17310 2021-04-21 10:10:40.000000 me_toolbox-0.0.8/me_toolbox/gears/spur_gear.py
-drwxrwxrwx   0        0        0        0 2024-03-26 21:23:25.342345 me_toolbox-0.0.8/me_toolbox/gears/tables/
--rw-rw-rw-   0        0        0     1318 2021-03-01 22:05:44.000000 me_toolbox-0.0.8/me_toolbox/gears/tables/20deg - spur gear geometry factors.csv
--rw-rw-rw-   0        0        0     1596 2021-03-01 22:08:27.000000 me_toolbox-0.0.8/me_toolbox/gears/tables/25deg - spur gear geometry factors.csv
--rw-rw-rw-   0        0        0      100 2021-03-19 13:14:28.000000 me_toolbox-0.0.8/me_toolbox/gears/tables/J75 - helix gear geometry factors.csv
--rw-rw-rw-   0        0        0      112 2021-03-19 13:16:09.000000 me_toolbox-0.0.8/me_toolbox/gears/tables/JPrime - helix gear geometry factors.csv
--rw-rw-rw-   0        0        0    17121 2024-03-03 20:02:37.000000 me_toolbox-0.0.8/me_toolbox/gears/transmission.py
-drwxrwxrwx   0        0        0        0 2024-03-26 21:23:25.390957 me_toolbox-0.0.8/me_toolbox/springs/
--rw-rw-rw-   0        0        0      257 2021-04-13 08:40:42.000000 me_toolbox-0.0.8/me_toolbox/springs/__init__.py
--rw-rw-rw-   0        0        0    24038 2024-03-20 10:03:53.000000 me_toolbox-0.0.8/me_toolbox/springs/extension_spring.py
--rw-rw-rw-   0        0        0    24095 2024-03-20 10:03:53.000000 me_toolbox-0.0.8/me_toolbox/springs/helical_push_spring.py
--rw-rw-rw-   0        0        0    17375 2024-03-20 10:03:53.000000 me_toolbox-0.0.8/me_toolbox/springs/helical_torsion_spring.py
--rw-rw-rw-   0        0        0     7070 2021-04-24 12:06:44.000000 me_toolbox-0.0.8/me_toolbox/springs/spring.py
-drwxrwxrwx   0        0        0        0 2024-03-26 21:23:25.431627 me_toolbox-0.0.8/me_toolbox/tools/
--rw-rw-rw-   0        0        0      174 2021-04-13 13:52:24.000000 me_toolbox-0.0.8/me_toolbox/tools/__init__.py
--rw-rw-rw-   0        0        0     4248 2024-03-17 22:06:01.000000 me_toolbox-0.0.8/me_toolbox/tools/helpers.py
--rw-rw-rw-   0        0        0     3079 2021-04-19 20:13:15.000000 me_toolbox-0.0.8/me_toolbox/tools/table_interpolation.py
-drwxrwxrwx   0        0        0        0 2024-03-26 21:23:25.439630 me_toolbox-0.0.8/me_toolbox.egg-info/
--rw-rw-rw-   0        0        0     1900 2024-03-26 21:23:24.000000 me_toolbox-0.0.8/me_toolbox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1329 2024-03-26 21:23:25.000000 me_toolbox-0.0.8/me_toolbox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 21:23:24.000000 me_toolbox-0.0.8/me_toolbox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2024-03-26 21:23:24.000000 me_toolbox-0.0.8/me_toolbox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-03-26 21:23:24.000000 me_toolbox-0.0.8/me_toolbox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2021-04-12 20:05:38.000000 me_toolbox-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-26 21:23:25.463849 me_toolbox-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1059 2024-03-26 21:23:07.000000 me_toolbox-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-03-30 20:16:39.832514 me_toolbox-0.0.9/
+-rw-rw-rw-   0        0        0     1091 2021-04-12 19:58:49.000000 me_toolbox-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       37 2021-04-13 10:57:43.000000 me_toolbox-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     1902 2024-03-30 20:16:39.816892 me_toolbox-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1174 2024-03-30 20:14:19.000000 me_toolbox-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-03-30 20:16:39.488766 me_toolbox-0.0.9/me_toolbox/
+-rw-rw-rw-   0        0        0        0 2024-03-09 18:44:50.000000 me_toolbox-0.0.9/me_toolbox/__init__.py
+drwxrwxrwx   0        0        0        0 2024-03-30 20:16:39.582518 me_toolbox-0.0.9/me_toolbox/fasteners/
+-rw-rw-rw-   0        0        0      172 2022-09-30 10:32:14.000000 me_toolbox-0.0.9/me_toolbox/fasteners/__init__.py
+-rw-rw-rw-   0        0        0     7208 2024-03-24 19:43:47.000000 me_toolbox-0.0.9/me_toolbox/fasteners/bolt.py
+-rw-rw-rw-   0        0        0    16759 2024-03-24 20:09:15.000000 me_toolbox-0.0.9/me_toolbox/fasteners/bolt_pattern.py
+-rw-rw-rw-   0        0        0     1831 2022-09-30 13:56:11.000000 me_toolbox-0.0.9/me_toolbox/fasteners/test_bolt.py
+-rw-rw-rw-   0        0        0     4714 2022-09-30 13:53:33.000000 me_toolbox-0.0.9/me_toolbox/fasteners/test_threaded_fastener.py
+-rw-rw-rw-   0        0        0     7809 2024-03-30 19:46:37.000000 me_toolbox-0.0.9/me_toolbox/fasteners/threaded_fastener.py
+drwxrwxrwx   0        0        0        0 2024-03-30 20:16:39.629394 me_toolbox-0.0.9/me_toolbox/fatigue/
+-rw-rw-rw-   0        0        0      236 2024-03-18 19:46:59.000000 me_toolbox-0.0.9/me_toolbox/fatigue/__init__.py
+-rw-rw-rw-   0        0        0     6301 2024-03-18 19:20:28.000000 me_toolbox-0.0.9/me_toolbox/fatigue/endurance_limit.py
+-rw-rw-rw-   0        0        0     6113 2024-03-20 10:28:30.000000 me_toolbox-0.0.9/me_toolbox/fatigue/failure_criteria.py
+-rw-rw-rw-   0        0        0    18335 2024-03-20 20:43:04.000000 me_toolbox-0.0.9/me_toolbox/fatigue/fatigue_analysis.py
+-rw-rw-rw-   0        0        0     2104 2021-04-19 20:13:15.000000 me_toolbox-0.0.9/me_toolbox/fatigue/stress.py
+drwxrwxrwx   0        0        0        0 2024-03-30 20:16:39.676265 me_toolbox-0.0.9/me_toolbox/gears/
+-rw-rw-rw-   0        0        0      215 2021-04-21 10:01:28.000000 me_toolbox-0.0.9/me_toolbox/gears/__init__.py
+-rw-rw-rw-   0        0        0    13524 2021-04-21 10:09:11.000000 me_toolbox-0.0.9/me_toolbox/gears/gear.py
+-rw-rw-rw-   0        0        0    20348 2021-04-21 08:37:31.000000 me_toolbox-0.0.9/me_toolbox/gears/helical_gear.py
+-rw-rw-rw-   0        0        0    17310 2021-04-21 10:10:40.000000 me_toolbox-0.0.9/me_toolbox/gears/spur_gear.py
+drwxrwxrwx   0        0        0        0 2024-03-30 20:16:39.723142 me_toolbox-0.0.9/me_toolbox/gears/tables/
+-rw-rw-rw-   0        0        0     1318 2021-03-01 22:05:44.000000 me_toolbox-0.0.9/me_toolbox/gears/tables/20deg - spur gear geometry factors.csv
+-rw-rw-rw-   0        0        0     1596 2021-03-01 22:08:27.000000 me_toolbox-0.0.9/me_toolbox/gears/tables/25deg - spur gear geometry factors.csv
+-rw-rw-rw-   0        0        0      100 2021-03-19 13:14:28.000000 me_toolbox-0.0.9/me_toolbox/gears/tables/J75 - helix gear geometry factors.csv
+-rw-rw-rw-   0        0        0      112 2021-03-19 13:16:09.000000 me_toolbox-0.0.9/me_toolbox/gears/tables/JPrime - helix gear geometry factors.csv
+-rw-rw-rw-   0        0        0    17121 2024-03-03 20:02:37.000000 me_toolbox-0.0.9/me_toolbox/gears/transmission.py
+drwxrwxrwx   0        0        0        0 2024-03-30 20:16:39.785642 me_toolbox-0.0.9/me_toolbox/springs/
+-rw-rw-rw-   0        0        0      257 2021-04-13 08:40:42.000000 me_toolbox-0.0.9/me_toolbox/springs/__init__.py
+-rw-rw-rw-   0        0        0    24038 2024-03-20 10:03:53.000000 me_toolbox-0.0.9/me_toolbox/springs/extension_spring.py
+-rw-rw-rw-   0        0        0    24095 2024-03-20 10:03:53.000000 me_toolbox-0.0.9/me_toolbox/springs/helical_push_spring.py
+-rw-rw-rw-   0        0        0    17375 2024-03-20 10:03:53.000000 me_toolbox-0.0.9/me_toolbox/springs/helical_torsion_spring.py
+-rw-rw-rw-   0        0        0     7070 2021-04-24 12:06:44.000000 me_toolbox-0.0.9/me_toolbox/springs/spring.py
+drwxrwxrwx   0        0        0        0 2024-03-30 20:16:39.801265 me_toolbox-0.0.9/me_toolbox/tools/
+-rw-rw-rw-   0        0        0      174 2021-04-13 13:52:24.000000 me_toolbox-0.0.9/me_toolbox/tools/__init__.py
+-rw-rw-rw-   0        0        0     4248 2024-03-17 22:06:01.000000 me_toolbox-0.0.9/me_toolbox/tools/helpers.py
+-rw-rw-rw-   0        0        0     3079 2021-04-19 20:13:15.000000 me_toolbox-0.0.9/me_toolbox/tools/table_interpolation.py
+drwxrwxrwx   0        0        0        0 2024-03-30 20:16:39.816892 me_toolbox-0.0.9/me_toolbox.egg-info/
+-rw-rw-rw-   0        0        0     1902 2024-03-30 20:16:39.000000 me_toolbox-0.0.9/me_toolbox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1329 2024-03-30 20:16:39.000000 me_toolbox-0.0.9/me_toolbox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-03-30 20:16:39.000000 me_toolbox-0.0.9/me_toolbox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2024-03-30 20:16:39.000000 me_toolbox-0.0.9/me_toolbox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-03-30 20:16:39.000000 me_toolbox-0.0.9/me_toolbox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2021-04-12 20:05:38.000000 me_toolbox-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-03-30 20:16:39.832514 me_toolbox-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1059 2024-03-30 20:16:19.000000 me_toolbox-0.0.9/setup.py
```

### Comparing `me_toolbox-0.0.8/LICENSE` & `me_toolbox-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `me_toolbox-0.0.8/PKG-INFO` & `me_toolbox-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: me_toolbox
-Version: 0.0.8
+Version: 0.0.9
 Summary: Mechanical engineering design tools
 Home-page: https://github.com/OmriStein/MEtoolbox
 Author: Omri Stein
 Author-email: omri.stein@gmail.com
 Project-URL: Bug Tracker, https://github.com/OmriStein/MEtoolbox/issues
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Education
@@ -22,21 +22,22 @@
 # me_toolbox
 
 me_toolbox is a Python library meant to simplify the tedious
 calculations of mechanical design and help speed up the design process.<br>
 This library contains fatigue, gears, springs and fasteners analysis tools.<br>
 This library is for my own personal use, use it at your own discretion.
 
-<!--
+
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install me_toolbox.
 ```bash
  pip install me_toolbox 
 ```
+<!--
 --->
 
 ## Usage
 
 ```python
 import me_toolbox.springs as springs 
 import me_toolbox.gears as gears
```

### Comparing `me_toolbox-0.0.8/README.md` & `me_toolbox-0.0.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # me_toolbox
 
 me_toolbox is a Python library meant to simplify the tedious
 calculations of mechanical design and help speed up the design process.<br>
 This library contains fatigue, gears, springs and fasteners analysis tools.<br>
 This library is for my own personal use, use it at your own discretion.
 
-<!--
+
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install me_toolbox.
 ```bash
  pip install me_toolbox 
 ```
+<!--
 --->
 
 ## Usage
 
 ```python
 import me_toolbox.springs as springs 
 import me_toolbox.gears as gears
@@ -36,8 +37,8 @@
 pattern = fasteners.BoltPattern(fasteners, ...)
 ```
 
 For more detailed examples:
 https://github.com/OmriStein/me-toolbox/tree/master/examples
 
 ## License
-[MIT](https://choosealicense.com/licenses/mit/)
+[MIT](https://choosealicense.com/licenses/mit/)
```

### Comparing `me_toolbox-0.0.8/me_toolbox/fasteners/bolt.py` & `me_toolbox-0.0.9/me_toolbox/fasteners/bolt.py`

 * *Files identical despite different names*

### Comparing `me_toolbox-0.0.8/me_toolbox/fasteners/bolt_pattern.py` & `me_toolbox-0.0.9/me_toolbox/fasteners/bolt_pattern.py`

 * *Files identical despite different names*

### Comparing `me_toolbox-0.0.8/me_toolbox/fasteners/test_bolt.py` & `me_toolbox-0.0.9/me_toolbox/fasteners/test_bolt.py`

 * *Files identical despite different names*

### Comparing `me_toolbox-0.0.8/me_toolbox/fasteners/test_threaded_fastener.py` & `me_toolbox-0.0.9/me_toolbox/fasteners/test_threaded_fastener.py`

 * *Files identical despite different names*

### Comparing `me_toolbox-0.0.8/me_toolbox/fasteners/threaded_fastener.py` & `me_toolbox-0.0.9/me_toolbox/fasteners/threaded_fastener.py`

 * *Files 8% similar despite different names*

```diff
@@ -165,28 +165,29 @@
         """
         return self.bolt_stiffness / (self.member_stiffness + self.bolt_stiffness)
 
     def bolt_load(self, external_force):
         """The load on the bolt (Fb)"""
         return self.fastener_stiffness * external_force + self.preload
 
-    def member_load(self, bolt_load):
+    def member_load(self, external_force):
         """The load on the member (Fm)"""
-        return (1 - self.fastener_stiffness) * bolt_load - self.preload
+        return (1 - self.fastener_stiffness) * external_force - self.preload
 
-    @staticmethod
-    def bolt_stress(bolt_load, stress_area):
-        """Bolt stress from pure tension"""
-        return bolt_load/stress_area
-
-    def load_safety_factor(self, equivalent_stress):
-        """Safety factor for load (nL)"""
-        return (self.bolt.proof_load - self.preload) / (
-                (equivalent_stress * self.bolt.stress_area) - self.preload)
-
-    def separation_safety_factor(self, external_force):
-        """Safety factor against joint separation (n0)"""
-        return self.preload / (external_force * (1 - self.fastener_stiffness))
-
-    def proof_safety_factor(self, equivalent_stress):
-        """Safety factor for proof strength (np)"""
-        return self.bolt.proof_strength / equivalent_stress
+    def safety_factors(self, external_force):
+        """Safety factor for direct normal stress only
+        (not shear stress and not eccentric loading)
+        :param float external_force: The force acting on the fastener
+
+        :return: A dictionary with the static safety factors<br>
+                 n0 - Separation safety factor<br>
+                 nL - Load safety factor<br>
+                 np - Proof safety factor
+        :rtype: dict
+        """
+        bolt_load = self.bolt_load(external_force)
+        separation_safety_factor = self.preload / (external_force * (1 - self.fastener_stiffness))
+        load_safety_factor = (self.bolt.proof_load - self.preload) / (bolt_load - self.preload)
+        proof_safety_factor = self.bolt.proof_strength / bolt_load
+        return {'n0': separation_safety_factor,
+                'nL': load_safety_factor,
+                'np': proof_safety_factor}
```

### Comparing `me_toolbox-0.0.8/me_toolbox/fatigue/endurance_limit.py` & `me_toolbox-0.0.9/me_toolbox/fatigue/endurance_limit.py`

 * *Files identical despite different names*

### Comparing `me_toolbox-0.0.8/me_toolbox/fatigue/failure_criteria.py` & `me_toolbox-0.0.9/me_toolbox/fatigue/failure_criteria.py`

 * *Files identical despite different names*

### Comparing `me_toolbox-0.0.8/me_toolbox/fatigue/fatigue_analysis.py` & `me_toolbox-0.0.9/me_toolbox/fatigue/fatigue_analysis.py`

 * *Files identical despite different names*

### Comparing `me_toolbox-0.0.8/me_toolbox/fatigue/stress.py` & `me_toolbox-0.0.9/me_toolbox/fatigue/stress.py`

 * *Files identical despite different names*

### Comparing `me_toolbox-0.0.8/me_toolbox/gears/gear.py` & `me_toolbox-0.0.9/me_toolbox/gears/gear.py`

 * *Files identical despite different names*

### Comparing `me_toolbox-0.0.8/me_toolbox/gears/helical_gear.py` & `me_toolbox-0.0.9/me_toolbox/gears/helical_gear.py`

 * *Files identical despite different names*

### Comparing `me_toolbox-0.0.8/me_toolbox/gears/spur_gear.py` & `me_toolbox-0.0.9/me_toolbox/gears/spur_gear.py`

 * *Files identical despite different names*

### Comparing `me_toolbox-0.0.8/me_toolbox/gears/tables/20deg - spur gear geometry factors.csv` & `me_toolbox-0.0.9/me_toolbox/gears/tables/20deg - spur gear geometry factors.csv`

 * *Files identical despite different names*

### Comparing `me_toolbox-0.0.8/me_toolbox/gears/tables/25deg - spur gear geometry factors.csv` & `me_toolbox-0.0.9/me_toolbox/gears/tables/25deg - spur gear geometry factors.csv`

 * *Files identical despite different names*

### Comparing `me_toolbox-0.0.8/me_toolbox/gears/transmission.py` & `me_toolbox-0.0.9/me_toolbox/gears/transmission.py`

 * *Files identical despite different names*

### Comparing `me_toolbox-0.0.8/me_toolbox/springs/extension_spring.py` & `me_toolbox-0.0.9/me_toolbox/springs/extension_spring.py`

 * *Files identical despite different names*

### Comparing `me_toolbox-0.0.8/me_toolbox/springs/helical_push_spring.py` & `me_toolbox-0.0.9/me_toolbox/springs/helical_push_spring.py`

 * *Files identical despite different names*

### Comparing `me_toolbox-0.0.8/me_toolbox/springs/helical_torsion_spring.py` & `me_toolbox-0.0.9/me_toolbox/springs/helical_torsion_spring.py`

 * *Files identical despite different names*

### Comparing `me_toolbox-0.0.8/me_toolbox/springs/spring.py` & `me_toolbox-0.0.9/me_toolbox/springs/spring.py`

 * *Files identical despite different names*

### Comparing `me_toolbox-0.0.8/me_toolbox/tools/helpers.py` & `me_toolbox-0.0.9/me_toolbox/tools/helpers.py`

 * *Files identical despite different names*

### Comparing `me_toolbox-0.0.8/me_toolbox/tools/table_interpolation.py` & `me_toolbox-0.0.9/me_toolbox/tools/table_interpolation.py`

 * *Files identical despite different names*

### Comparing `me_toolbox-0.0.8/me_toolbox.egg-info/PKG-INFO` & `me_toolbox-0.0.9/me_toolbox.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: me_toolbox
-Version: 0.0.8
+Version: 0.0.9
 Summary: Mechanical engineering design tools
 Home-page: https://github.com/OmriStein/MEtoolbox
 Author: Omri Stein
 Author-email: omri.stein@gmail.com
 Project-URL: Bug Tracker, https://github.com/OmriStein/MEtoolbox/issues
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Education
@@ -22,21 +22,22 @@
 # me_toolbox
 
 me_toolbox is a Python library meant to simplify the tedious
 calculations of mechanical design and help speed up the design process.<br>
 This library contains fatigue, gears, springs and fasteners analysis tools.<br>
 This library is for my own personal use, use it at your own discretion.
 
-<!--
+
 ## Installation
 
 Use the package manager [pip](https://pip.pypa.io/en/stable/) to install me_toolbox.
 ```bash
  pip install me_toolbox 
 ```
+<!--
 --->
 
 ## Usage
 
 ```python
 import me_toolbox.springs as springs 
 import me_toolbox.gears as gears
```

### Comparing `me_toolbox-0.0.8/me_toolbox.egg-info/SOURCES.txt` & `me_toolbox-0.0.9/me_toolbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `me_toolbox-0.0.8/setup.py` & `me_toolbox-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="me_toolbox",
-    version="0.0.8",
+    version="0.0.9",
     author="Omri Stein",
     author_email="omri.stein@gmail.com",
     description="Mechanical engineering design tools",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OmriStein/MEtoolbox",
     project_urls={
```

