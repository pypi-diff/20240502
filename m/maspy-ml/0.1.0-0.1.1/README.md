# Comparing `tmp/maspy-ml-0.1.0.tar.gz` & `tmp/maspy-ml-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maspy-ml-0.1.0.tar", last modified: Thu May  2 06:10:17 2024, max compression
+gzip compressed data, was "maspy-ml-0.1.1.tar", last modified: Thu May  2 21:20:18 2024, max compression
```

## Comparing `maspy-ml-0.1.0.tar` & `maspy-ml-0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 06:10:17.424980 maspy-ml-0.1.0/
--rw-rw-rw-   0        0        0      631 2024-05-02 06:10:17.423982 maspy-ml-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     5540 2024-04-29 17:06:13.000000 maspy-ml-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-02 06:10:17.382122 maspy-ml-0.1.0/maspy/
--rw-rw-rw-   0        0        0      407 2024-05-02 06:09:27.000000 maspy-ml-0.1.0/maspy/__init__.py
--rw-rw-rw-   0        0        0     6764 2024-05-02 06:09:27.000000 maspy-ml-0.1.0/maspy/admin.py
--rw-rw-rw-   0        0        0    26985 2024-05-02 06:09:27.000000 maspy-ml-0.1.0/maspy/agent.py
--rw-rw-rw-   0        0        0     4480 2024-05-02 06:09:27.000000 maspy-ml-0.1.0/maspy/communication.py
--rw-rw-rw-   0        0        0     7420 2024-05-02 06:09:27.000000 maspy-ml-0.1.0/maspy/environment.py
--rw-rw-rw-   0        0        0      249 2024-05-02 06:09:27.000000 maspy-ml-0.1.0/maspy/error.py
--rw-rw-rw-   0        0        0    28882 2024-05-02 06:09:27.000000 maspy-ml-0.1.0/maspy/learning.py
--rw-rw-rw-   0        0        0      792 2024-05-02 06:09:27.000000 maspy-ml-0.1.0/maspy/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-02 06:10:17.394061 maspy-ml-0.1.0/maspy_ml.egg-info/
--rw-rw-rw-   0        0        0      631 2024-05-02 06:10:17.000000 maspy-ml-0.1.0/maspy_ml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      378 2024-05-02 06:10:17.000000 maspy-ml-0.1.0/maspy_ml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 06:10:17.000000 maspy-ml-0.1.0/maspy_ml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-02 06:10:17.000000 maspy-ml-0.1.0/maspy_ml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 06:10:17.424980 maspy-ml-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      925 2024-05-02 06:10:05.000000 maspy-ml-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-02 06:10:17.422984 maspy-ml-0.1.0/tests/
--rw-rw-rw-   0        0        0        0 2024-04-09 03:42:49.000000 maspy-ml-0.1.0/tests/__init__.py
--rw-rw-rw-   0        0        0      154 2024-04-25 19:34:48.000000 maspy-ml-0.1.0/tests/test_agent.py
--rw-rw-rw-   0        0        0     1016 2024-04-24 20:26:45.000000 maspy-ml-0.1.0/tests/test_communication.py
--rw-rw-rw-   0        0        0     3144 2024-05-02 00:13:06.000000 maspy-ml-0.1.0/tests/test_environment.py
+drwxrwxrwx   0        0        0        0 2024-05-02 21:20:18.615382 maspy-ml-0.1.1/
+-rw-rw-rw-   0        0        0      631 2024-05-02 21:20:18.614384 maspy-ml-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5540 2024-04-29 17:06:13.000000 maspy-ml-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 21:20:18.581471 maspy-ml-0.1.1/maspy/
+-rw-rw-rw-   0        0        0      407 2024-05-02 06:09:27.000000 maspy-ml-0.1.1/maspy/__init__.py
+-rw-rw-rw-   0        0        0     7301 2024-05-02 21:13:32.000000 maspy-ml-0.1.1/maspy/admin.py
+-rw-rw-rw-   0        0        0    28014 2024-05-02 21:09:07.000000 maspy-ml-0.1.1/maspy/agent.py
+-rw-rw-rw-   0        0        0     4480 2024-05-02 06:09:27.000000 maspy-ml-0.1.1/maspy/communication.py
+-rw-rw-rw-   0        0        0     7424 2024-05-02 20:29:16.000000 maspy-ml-0.1.1/maspy/environment.py
+-rw-rw-rw-   0        0        0      249 2024-05-02 06:09:27.000000 maspy-ml-0.1.1/maspy/error.py
+-rw-rw-rw-   0        0        0    28882 2024-05-02 06:09:27.000000 maspy-ml-0.1.1/maspy/learning.py
+-rw-rw-rw-   0        0        0      792 2024-05-02 06:09:27.000000 maspy-ml-0.1.1/maspy/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-02 21:20:18.593439 maspy-ml-0.1.1/maspy_ml.egg-info/
+-rw-rw-rw-   0        0        0      631 2024-05-02 21:20:18.000000 maspy-ml-0.1.1/maspy_ml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2024-05-02 21:20:18.000000 maspy-ml-0.1.1/maspy_ml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 21:20:18.000000 maspy-ml-0.1.1/maspy_ml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-02 21:20:18.000000 maspy-ml-0.1.1/maspy_ml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 21:20:18.615382 maspy-ml-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      925 2024-05-02 21:18:01.000000 maspy-ml-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 21:20:18.613386 maspy-ml-0.1.1/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-09 03:42:49.000000 maspy-ml-0.1.1/tests/__init__.py
+-rw-rw-rw-   0        0        0      154 2024-04-25 19:34:48.000000 maspy-ml-0.1.1/tests/test_agent.py
+-rw-rw-rw-   0        0        0     1016 2024-04-24 20:26:45.000000 maspy-ml-0.1.1/tests/test_communication.py
+-rw-rw-rw-   0        0        0     3144 2024-05-02 00:13:06.000000 maspy-ml-0.1.1/tests/test_environment.py
```

### Comparing `maspy-ml-0.1.0/PKG-INFO` & `maspy-ml-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maspy-ml
-Version: 0.1.0
+Version: 0.1.1
 Summary: Multi-Agent Systems in Python with Machine Learning
 Author: Alexandre Mellado
 Author-email: <melladoallm@gamil.com>
 Keywords: python,autonomous agents,multi-agent system,machine learning
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `maspy-ml-0.1.0/README.md` & `maspy-ml-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `maspy-ml-0.1.0/maspy/admin.py` & `maspy-ml-0.1.1/maspy/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,16 @@
         signal.signal(signal.SIGINT, self.stop_all_agents)
         self.end_of_execution = False
         self._name = f"# {type(self).__name__} #"
         print("Starting MASPY Program")
         self.full_log = False
         self.agt_full_log = False
         self.agt_sh_cycle = False
+        self.agt_sh_prct = False
+        self.agt_sh_slct = False
         self.ch_full_log = False
         self.env_full_log = False
         self._started_agents: List[Agent] = list()
         self._agent_list: Dict[str, str] = dict()
         self._num_agent: Dict[str, int] = dict()
         self._agents: Dict[str, Agent] = dict()
         self._channels: Dict[str, Channel] = dict()
@@ -64,14 +66,16 @@
         
         #agent.my_name = ("").join(str(x) for x in agent.name_tag)
         
         self._agent_list[agent.my_name] = type(agent).__name__
         self._agents[agent.my_name] = agent
         agent.full_log = self.agt_full_log
         agent.show_cycle = self.agt_sh_cycle
+        agent.show_prct = self.agt_sh_prct
+        agent.show_slct = self.agt_sh_slct
         self.print(
             f"Registering Agent {type(agent).__name__}:{agent.my_name}"
         ) if self.full_log else ...
 
     def rm_agents(
         self, agents: Union[Iterable[Agent], Agent]
     ):
@@ -88,18 +92,24 @@
         self.print(
             f"Removing agent {type(agent).__name__}:{agent.my_name} from List"
         ) if self.full_log else ...
 
     def _add_channel(self, channel: Channel):
         self._channels[channel._my_name] = channel
         channel.full_log = self.ch_full_log
+        self.print(
+            f"Registering {type(channel).__name__}:{channel._my_name}"
+        ) if self.full_log else ...
 
     def _add_environment(self, environment: Environment):
         self._environments[environment._my_name] = environment
         environment.full_log = self.env_full_log
+        self.print(
+            f"Registering Environment {type(environment).__name__}:{environment._my_name}"
+        ) if self.full_log else ...
     
     def start_system(self):
         no_agents = True
         try:
             self.print(f"Starting Agents")
             for agent_name in self._agents:
                 no_agents = False
@@ -160,24 +170,25 @@
                     case Environment():
                         agent._environments[target._my_name] = target
                     case Channel():
                         agent._channels[target._my_name] = target
                 
                 target._add_agent(agent)
 
-    def set_logging(self, full_log: bool, show_cycle: bool=False, 
+    def set_logging(self, full_log: bool, show_cycle: bool=False,
+                    show_prct: bool=False, show_slct: bool=False, 
                      set_admin=True,
                      set_agents=True,
                      set_channels=True,
                      set_environments=True
                     ):
         self.full_log = True if full_log and set_admin else False
         self.agt_full_log = True if full_log and set_agents else False
         self.agt_sh_cycle = True if show_cycle and set_agents else False
+        self.agt_sh_prct = True if show_prct and set_agents else False
+        self.agt_sh_slct  = True if show_slct and set_agents else False
         self.ch_full_log = True if full_log and set_channels else False
         self.env_full_log = True if full_log and set_environments else False
-        
-        print(self.full_log,self.agt_full_log,self.agt_sh_cycle,self.ch_full_log,self.env_full_log)
 
     def slow_cycle_by(self, time: int | float):
         for agent in self._agents.values():
             agent.sleep = time
```

### Comparing `maspy-ml-0.1.0/maspy/agent.py` & `maspy-ml-0.1.1/maspy/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -232,19 +232,23 @@
     def __init__(
         self,
         name: str = None,
         beliefs: Optional[Iterable[Belief] | Belief] = None,
         goals: Optional[Iterable[Goal] | Goal] = None,
         full_log = False,
         show_cycle = False,
+        show_prct = False,
+        show_slct = False,
         log_type = "Default",
         instant_mail = False
     ):              
         self.full_log = full_log
         self.show_cycle = show_cycle
+        self.show_prct = show_prct
+        self.show_slct = show_slct
         self.log_type = log_type
         
         from maspy.admin import Admin
         self.my_name = name
         Admin().add_agents(self)
         
         self.sleep = None
@@ -439,41 +443,41 @@
                 belief_goal = data_type.data
             case _: 
                 self.print(f"Error in _to_belief_goal: {type(data_type)}:{data_type}")
                 return None, None
         return change,belief_goal
     
     def _compare_data(self, data1, data2, ck_type,ck_args,ck_src):
-        #self.print(f"Comparing: \n\t{data1} and {data2}")
+        self.print(f"Comparing: \n\t{data1} and {data2}") if self.show_slct else ...
         if ck_type and type(data1) != type(data2):
-            #self.print("Failed at type")
+            self.print("Failed at type") if self.show_slct else ...
             return False
         if data1.key != data2.key:
-            #self.print("Failed at key")
+            self.print("Failed at key") if self.show_slct else ...
             return False
         if ck_src and data2.source != DEFAULT_SOURCE and data1.source != data2.source:
-            #self.print("Failed at source")
+            self.print("Failed at source") if self.show_slct else ...
             return False
         if not ck_args:
             return True
         if data1.args_len != data2.args_len:
-            #self.print("Failed at args_len")
+            self.print("Failed at args_len") if self.show_slct else ...
             return False
         for arg1,arg2 in zip(data1._args,data2._args):
             if isinstance(arg1,str) and (arg1[0].isupper()):
                 continue
             elif isinstance(arg2,str) and (arg2[0].isupper()):
                 continue
             elif arg1 == arg2:
                 continue
             else:
-                #self.print(f"Failed at args {arg1} x {arg2}")
+                self.print(f"Failed at args {arg1} x {arg2}") if self.show_slct else ...
                 return False
         else:
-            #self.print("Data is Compatible")
+            self.print("Data is Compatible") if self.show_slct else ...
             return True
                       
     def _run_plan(self, plan: Plan, trigger: Belief | Goal, args: tuple):
         self.print(f"Running {plan}")  if self.full_log else ...
         try:
             #self.print(f'running with {trigger._args} {args}')
             return plan.body(self, trigger.source, *trigger._args, *args)
@@ -591,15 +595,15 @@
             self.print(f"Selected chosen_plan: {chosen_plan} with {args} arguments") if self.show_cycle else ...
             result = self._execute_plan(chosen_plan,event,args)
             if self.sleep: sleep(self.sleep)
 
     def _perception(self):
         percept_dict = dict()
         for env_name in self._environments:
-            self.print(f"Percepting '{env_name}'") if self.full_log else ...
+            self.print(f"Percepting '{env_name}'") if self.show_cycle else ...
             percept_dict.update(self._environments[env_name].perception())
         percept_dict = self._percepts_to_beliefs(percept_dict)
         self._revise_beliefs(percept_dict)
     
     def _percepts_to_beliefs(self,percepts: dict) -> dict:
         # TODO make use of percepts group
         for source, keys in percepts.copy().items():
@@ -608,49 +612,58 @@
                 for percept in percepts_set:
                     belief_set.add(Belief(percept.key,percept.args,source,percept.adds_event))
                 percepts[source][key] = belief_set
         return percepts
      
     def _revise_beliefs(self, percept_dict: dict):
         for source, keys in self.__beliefs.copy().items():
-            if source == DEFAULT_SOURCE: continue
+            if source == DEFAULT_SOURCE: continue # Does not remove "self"
+            if type(source) == tuple: continue # Does not remove messages
             if source in percept_dict:
                 for key, beliefs in keys.copy().items():
                     if key in percept_dict[source]: 
                         new, gain, lose = utils.set_changes(beliefs,percept_dict[source][key])
                         self.__beliefs[source][key] = new
                         self._new_event("gain",gain) # Gained new specific belief
                         self._new_event("lose",lose) # Lost an old specific belief
                         del percept_dict[source][key]
+                        if self.show_prct:
+                            self.print(f"Beliefs gained in revision: {gain}")
+                            self.print(f"Beliefs lost in revision: {lose}") 
                     else:
                         self._new_event("lose",self.__beliefs[source][key]) # Lost whole key belief
+                        self.print(f"Beliefs lost in revision: {self.__beliefs[source][key]}") if self.show_prct else ...
                         del self.__beliefs[source][key]
                         
                 if percept_dict[source] == {}:
                     del percept_dict[source]
             else:
                 for beliefs in keys.values():
+                    self.print(f"Beliefs lost in revision: {beliefs}") if self.show_prct else ...
                     self._new_event("lose",beliefs) # Lost whole source of belief (env)
                 del self.__beliefs[source]
         
         for keys in percept_dict.values():
             for beliefs in keys.values():
+                self.print(f"Beliefs gained in revision: {beliefs}") if self.show_prct else ...
                 self._new_event("gain",beliefs) # Gained beliefs of new sources/keys
         self.__beliefs.update(percept_dict)
     
     def _select_event(self):
         if self.__events == []: return None
         return self.__events.pop(0)
     
     def _retrieve_plans(self, event):
         if event is None: return None
         return self.get(Plan,event,all=True,ck_src=False)
     
     def _select_plan(self, plans, event:Event):
-        if plans is None: return None, None
+        if plans is None:
+            self.print(f"No plans found for {event}") if self.show_cycle else ... 
+            return None, None
         
         args = tuple()
         for plan in plans:
             for context in plan.context:
                 ctxt = self.get(context,ck_src=False)
                 if not ctxt:
                     break
```

### Comparing `maspy-ml-0.1.0/maspy/communication.py` & `maspy-ml-0.1.1/maspy/communication.py`

 * *Files identical despite different names*

### Comparing `maspy-ml-0.1.0/maspy/environment.py` & `maspy-ml-0.1.1/maspy/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 class Environment(metaclass=EnvironmentMultiton):
     def __init__(self, env_name=None,full_log=False):
         self._my_name = env_name if env_name else type(self).__name__
         self.full_log = full_log
         
         from maspy.admin import Admin
-        Admin()._add_channel(self)
+        Admin()._add_environment(self)
         
         self.agent_list = {}
         self._agents = {}
         self._name = f"Environment:{self._my_name}"
         self._percepts: Dict[str, Dict[str, Set[Percept]]] = dict()
     
     def print(self,*args, **kwargs):
```

### Comparing `maspy-ml-0.1.0/maspy/learning.py` & `maspy-ml-0.1.1/maspy/learning.py`

 * *Files identical despite different names*

### Comparing `maspy-ml-0.1.0/maspy/utils.py` & `maspy-ml-0.1.1/maspy/utils.py`

 * *Files identical despite different names*

### Comparing `maspy-ml-0.1.0/maspy_ml.egg-info/PKG-INFO` & `maspy-ml-0.1.1/maspy_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maspy-ml
-Version: 0.1.0
+Version: 0.1.1
 Summary: Multi-Agent Systems in Python with Machine Learning
 Author: Alexandre Mellado
 Author-email: <melladoallm@gamil.com>
 Keywords: python,autonomous agents,multi-agent system,machine learning
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `maspy-ml-0.1.0/setup.py` & `maspy-ml-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'Multi-Agent Systems in Python with Machine Learning'
 LONG_DESCRIPTION = 'A library for the devolopment of multi-agent systems with components of machine learning'
 
 # Setting up
 setup(
     name="maspy-ml",
     version=VERSION,
```

### Comparing `maspy-ml-0.1.0/tests/test_communication.py` & `maspy-ml-0.1.1/tests/test_communication.py`

 * *Files identical despite different names*

### Comparing `maspy-ml-0.1.0/tests/test_environment.py` & `maspy-ml-0.1.1/tests/test_environment.py`

 * *Files identical despite different names*

