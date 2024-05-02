# Comparing `tmp/maspy-ml-0.0.4.tar.gz` & `tmp/maspy-ml-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maspy-ml-0.0.4.tar", last modified: Tue Apr 30 22:14:41 2024, max compression
+gzip compressed data, was "maspy-ml-0.1.0.tar", last modified: Thu May  2 06:10:17 2024, max compression
```

## Comparing `maspy-ml-0.0.4.tar` & `maspy-ml-0.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 22:14:41.440203 maspy-ml-0.0.4/
--rw-rw-rw-   0        0        0      631 2024-04-30 22:14:41.440203 maspy-ml-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     5540 2024-04-29 17:06:13.000000 maspy-ml-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-04-30 22:14:41.385117 maspy-ml-0.0.4/maspy/
--rw-rw-rw-   0        0        0      407 2024-04-29 16:16:10.000000 maspy-ml-0.0.4/maspy/__init__.py
--rw-rw-rw-   0        0        0     4961 2024-04-30 21:50:28.000000 maspy-ml-0.0.4/maspy/admin.py
--rw-rw-rw-   0        0        0    26567 2024-04-30 21:49:49.000000 maspy-ml-0.0.4/maspy/agent.py
--rw-rw-rw-   0        0        0     4305 2024-04-29 16:50:14.000000 maspy-ml-0.0.4/maspy/communication.py
--rw-rw-rw-   0        0        0     7567 2024-04-30 21:59:25.000000 maspy-ml-0.0.4/maspy/environment.py
--rw-rw-rw-   0        0        0      249 2024-04-08 01:20:57.000000 maspy-ml-0.0.4/maspy/error.py
--rw-rw-rw-   0        0        0    28882 2024-03-06 19:42:41.000000 maspy-ml-0.0.4/maspy/learning.py
--rw-rw-rw-   0        0        0      792 2024-04-29 12:28:21.000000 maspy-ml-0.0.4/maspy/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-30 22:14:41.398055 maspy-ml-0.0.4/maspy_ml.egg-info/
--rw-rw-rw-   0        0        0      631 2024-04-30 22:14:41.000000 maspy-ml-0.0.4/maspy_ml.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      378 2024-04-30 22:14:41.000000 maspy-ml-0.0.4/maspy_ml.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 22:14:41.000000 maspy-ml-0.0.4/maspy_ml.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-30 22:14:41.000000 maspy-ml-0.0.4/maspy_ml.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-30 22:14:41.440203 maspy-ml-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      925 2024-04-30 22:03:57.000000 maspy-ml-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-30 22:14:41.439177 maspy-ml-0.0.4/tests/
--rw-rw-rw-   0        0        0        0 2024-04-09 03:42:49.000000 maspy-ml-0.0.4/tests/__init__.py
--rw-rw-rw-   0        0        0      154 2024-04-25 19:34:48.000000 maspy-ml-0.0.4/tests/test_agent.py
--rw-rw-rw-   0        0        0     1016 2024-04-24 20:26:45.000000 maspy-ml-0.0.4/tests/test_communication.py
--rw-rw-rw-   0        0        0     3256 2024-04-24 20:26:45.000000 maspy-ml-0.0.4/tests/test_environment.py
+drwxrwxrwx   0        0        0        0 2024-05-02 06:10:17.424980 maspy-ml-0.1.0/
+-rw-rw-rw-   0        0        0      631 2024-05-02 06:10:17.423982 maspy-ml-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5540 2024-04-29 17:06:13.000000 maspy-ml-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 06:10:17.382122 maspy-ml-0.1.0/maspy/
+-rw-rw-rw-   0        0        0      407 2024-05-02 06:09:27.000000 maspy-ml-0.1.0/maspy/__init__.py
+-rw-rw-rw-   0        0        0     6764 2024-05-02 06:09:27.000000 maspy-ml-0.1.0/maspy/admin.py
+-rw-rw-rw-   0        0        0    26985 2024-05-02 06:09:27.000000 maspy-ml-0.1.0/maspy/agent.py
+-rw-rw-rw-   0        0        0     4480 2024-05-02 06:09:27.000000 maspy-ml-0.1.0/maspy/communication.py
+-rw-rw-rw-   0        0        0     7420 2024-05-02 06:09:27.000000 maspy-ml-0.1.0/maspy/environment.py
+-rw-rw-rw-   0        0        0      249 2024-05-02 06:09:27.000000 maspy-ml-0.1.0/maspy/error.py
+-rw-rw-rw-   0        0        0    28882 2024-05-02 06:09:27.000000 maspy-ml-0.1.0/maspy/learning.py
+-rw-rw-rw-   0        0        0      792 2024-05-02 06:09:27.000000 maspy-ml-0.1.0/maspy/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-02 06:10:17.394061 maspy-ml-0.1.0/maspy_ml.egg-info/
+-rw-rw-rw-   0        0        0      631 2024-05-02 06:10:17.000000 maspy-ml-0.1.0/maspy_ml.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2024-05-02 06:10:17.000000 maspy-ml-0.1.0/maspy_ml.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 06:10:17.000000 maspy-ml-0.1.0/maspy_ml.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-02 06:10:17.000000 maspy-ml-0.1.0/maspy_ml.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 06:10:17.424980 maspy-ml-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      925 2024-05-02 06:10:05.000000 maspy-ml-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 06:10:17.422984 maspy-ml-0.1.0/tests/
+-rw-rw-rw-   0        0        0        0 2024-04-09 03:42:49.000000 maspy-ml-0.1.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      154 2024-04-25 19:34:48.000000 maspy-ml-0.1.0/tests/test_agent.py
+-rw-rw-rw-   0        0        0     1016 2024-04-24 20:26:45.000000 maspy-ml-0.1.0/tests/test_communication.py
+-rw-rw-rw-   0        0        0     3144 2024-05-02 00:13:06.000000 maspy-ml-0.1.0/tests/test_environment.py
```

### Comparing `maspy-ml-0.0.4/PKG-INFO` & `maspy-ml-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maspy-ml
-Version: 0.0.4
+Version: 0.1.0
 Summary: Multi-Agent Systems in Python with Machine Learning
 Author: Alexandre Mellado
 Author-email: <melladoallm@gamil.com>
 Keywords: python,autonomous agents,multi-agent system,machine learning
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `maspy-ml-0.0.4/README.md` & `maspy-ml-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `maspy-ml-0.0.4/maspy/admin.py` & `maspy-ml-0.1.0/maspy/admin.py`

 * *Files 22% similar despite different names*

```diff
@@ -19,18 +19,25 @@
         return cls._instances[cls]
 class Admin(metaclass=AdminMeta):
     def __init__(self) -> None:
         signal.signal(signal.SIGINT, self.stop_all_agents)
         self.end_of_execution = False
         self._name = f"# {type(self).__name__} #"
         print("Starting MASPY Program")
-        self._started_agents: List[Agent] = []
-        self._agent_list: Dict[str, str] = {}
-        self._num_agent = {}
-        self._agents: Dict[str, Agent] = {}
+        self.full_log = False
+        self.agt_full_log = False
+        self.agt_sh_cycle = False
+        self.ch_full_log = False
+        self.env_full_log = False
+        self._started_agents: List[Agent] = list()
+        self._agent_list: Dict[str, str] = dict()
+        self._num_agent: Dict[str, int] = dict()
+        self._agents: Dict[str, Agent] = dict()
+        self._channels: Dict[str, Channel] = dict()
+        self._environments: Dict[str, Environment] = dict()
         
     def print(self,*args, **kwargs):
         return print(f"{self._name}>",*args,**kwargs)
 
     def get_agents(self) -> Dict[str, str]:
         return self._agent_list
 
@@ -55,17 +62,19 @@
             self._num_agent[name] = 1
             agent.my_name = (name, 1)
         
         #agent.my_name = ("").join(str(x) for x in agent.name_tag)
         
         self._agent_list[agent.my_name] = type(agent).__name__
         self._agents[agent.my_name] = agent
+        agent.full_log = self.agt_full_log
+        agent.show_cycle = self.agt_sh_cycle
         self.print(
             f"Registering Agent {type(agent).__name__}:{agent.my_name}"
-        )
+        ) if self.full_log else ...
 
     def rm_agents(
         self, agents: Union[Iterable[Agent], Agent]
     ):
         try:
             for agent in agents:
                 self._rm_agent(agent)
@@ -74,16 +83,24 @@
 
     def _rm_agent(self, agent: Agent):
         if agent.my_name in self._agents:
             del self._agents[agent.my_name]
             del self._agent_list[agent.my_name]
         self.print(
             f"Removing agent {type(agent).__name__}:{agent.my_name} from List"
-        )
+        ) if self.full_log else ...
 
+    def _add_channel(self, channel: Channel):
+        self._channels[channel._my_name] = channel
+        channel.full_log = self.ch_full_log
+
+    def _add_environment(self, environment: Environment):
+        self._environments[environment._my_name] = environment
+        environment.full_log = self.env_full_log
+    
     def start_system(self):
         no_agents = True
         try:
             self.print(f"Starting Agents")
             for agent_name in self._agents:
                 no_agents = False
                 self._start_agent(agent_name)
@@ -130,18 +147,37 @@
     def stop_all_agents(self,sig,frame):
         self.print(f"[Closing System]")
         for agent in self._started_agents:
             if agent.running:
                 agent.stop_cycle()
         self.end_of_execution = True
     
-    def connect_to(self, agents: Iterable, targets: Iterable[Environment | Channel]):
+    def connect_to(self, agents: Iterable | Agent, targets: Iterable[Environment | Channel] | Environment | Channel):
+        if not isinstance(agents, Iterable): agents = [agents]
+        if not isinstance(targets, Iterable): targets = [targets]
         for agent in agents:
             for target in targets:
                 match target:
                     case Environment():
                         agent._environments[target._my_name] = target
                     case Channel():
                         agent._channels[target._my_name] = target
                 
                 target._add_agent(agent)
 
+    def set_logging(self, full_log: bool, show_cycle: bool=False, 
+                     set_admin=True,
+                     set_agents=True,
+                     set_channels=True,
+                     set_environments=True
+                    ):
+        self.full_log = True if full_log and set_admin else False
+        self.agt_full_log = True if full_log and set_agents else False
+        self.agt_sh_cycle = True if show_cycle and set_agents else False
+        self.ch_full_log = True if full_log and set_channels else False
+        self.env_full_log = True if full_log and set_environments else False
+        
+        print(self.full_log,self.agt_full_log,self.agt_sh_cycle,self.ch_full_log,self.env_full_log)
+
+    def slow_cycle_by(self, time: int | float):
+        for agent in self._agents.values():
+            agent.sleep = time
```

### Comparing `maspy-ml-0.0.4/maspy/agent.py` & `maspy-ml-0.1.0/maspy/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,20 +15,22 @@
 import inspect
 
 gain = TypeVar('gain')
 lose = TypeVar('lose')
 test = TypeVar('test')
 
 DEFAULT_SOURCE = "self"
+DEFAULT_CHANNEL = "default"
 
 @dataclass(eq=True, frozen=True)
 class Belief:
     key: str
     _args: tuple = field(default_factory=tuple)
     source: str = DEFAULT_SOURCE
+    adds_event: bool = True
 
     @property
     def args(self):
         if len(self._args) > 1:
             return self._args
         elif len(self._args) == 1:
             return self._args[0]
@@ -170,19 +172,16 @@
     
 @dataclass
 class Event:
     change: str # ( + or add, - or rm, ~ or test )
     data: Belief | Goal 
     intention: str = None # still don't understand how it works
     
-    def __init__(self,change,data,intention=None):
-        if type(change)==TypeVar: self.change = change.__name__ 
-        else: self.change = change
-        self.data = data
-        self.intention = intention
+    def __post_init__(self):
+        if type(self.change)==TypeVar: self.change = self.change.__name__ 
     
     def __str__(self) -> str:
         return f"Event{self.change,self.data,self.intention}"
     
 @dataclass
 class Plan:
     trigger: Event
@@ -232,41 +231,45 @@
 class Agent:
     def __init__(
         self,
         name: str = None,
         beliefs: Optional[Iterable[Belief] | Belief] = None,
         goals: Optional[Iterable[Goal] | Goal] = None,
         full_log = False,
+        show_cycle = False,
         log_type = "Default",
         instant_mail = False
     ):              
+        self.full_log = full_log
+        self.show_cycle = show_cycle
+        self.log_type = log_type
+        
         from maspy.admin import Admin
         self.my_name = name
         Admin().add_agents(self)
         
+        self.sleep = None
         self.stop_flag = None
         self.running = False
         self.thread = None
         self.saved_msgs = []
-        self.full_log = full_log
-        self.log_type = log_type
         
         self._name = f"Agent:{self.my_name}"
         
         self._environments: Dict[str, Environment] = dict()
         self._channels: Dict[str, Channel] = dict()
 
         self.__events: List[Event] = []
         self.__beliefs: Dict[str, Dict[str, Set[Belief]]] = dict()
         self.__goals: Dict[str, Dict[str, Set[Goal]]] = dict()
         if beliefs: self.add(beliefs)
         if goals: self.add(goals)
         
         self.instant_mail = instant_mail
-        self.connect_to(Channel(),"")
+        self.connect_to(Channel())
         self.paused_agent = False
         
         try: 
             self._plans
         except AttributeError:
             self._plans = []
          
@@ -339,17 +342,19 @@
 
     def rm_plan(self, plan: Plan):
         self._plans.pop(plan)
     
     def _new_event(self,change,data,intention=None):
         try:
             for dt in data:
+                if isinstance(dt,Belief) and not dt.adds_event: continue
                 self.print(f"New Event: {change}:{dt}")  if self.full_log else ...
                 self.__events.append(Event(change,dt,intention))
         except(TypeError):
+            if isinstance(data,Belief) and not data.adds_event: return
             self.print(f"New Event: {change}:{data}")  if self.full_log else ...
             self.__events.append(Event(change,data,intention))
     
     def _get_type_base(self, data_type):
         if data_type == Belief:
             return self.__beliefs
         elif data_type == Goal:
@@ -365,36 +370,36 @@
     def add(self, data_type: Belief | Goal | Iterable[Belief | Goal]):
         self.print(f"Adding {data_type}") if self.full_log else ...
         cleaned_data = self._clean(data_type)
         
         for type_data, data in cleaned_data.items():
             if len(data) == 0: continue
             type_base = self._get_type_base(type_data)
-            type_base = utils.merge_dicts(data,type_base)
+            utils.merge_dicts(data,type_base)
             
         self._new_event("gain",data_type)
                  
     def rm(self, data_type: Belief | Goal | Iterable[Belief | Goal]):
         self.print(f"Removing {data_type}") if self.full_log else ...
         
-        if type(data_type) != Iterable: data_type = [data_type]
+        if not isinstance(data_type, Iterable): data_type = [data_type]
             
         for typ in data_type:
             type_base = self._get_type_base(type(typ))
             type_base[typ.source][typ.key].remove(typ)
         
         self._new_event("lose",data_type)
 
     def has(self, data_type: Belief | Goal | Plan | Event):
         return self.get(data_type) != None
 
     def get(self, data_type: Belief | Goal | Plan | Event,
         search_with:  Belief | Goal | Plan | Event = None,
         all = False, ck_chng=True, ck_type=True, ck_args=True, ck_src=True
-    ) -> List[Belief | Goal | Plan | Event]:
+    ) -> List[Belief | Goal | Plan | Event] | Belief | Goal | Plan | Event:
         if type(data_type) is type: data_type = data_type(0,0,0)
         type_base = self._get_type_base(type(data_type))
         if search_with is None: search_with = data_type
 
         change, data = self._to_belief_goal(search_with)
         
         found_data = []
@@ -414,15 +419,15 @@
                     if change and ck_chng and chng != change:
                         continue
                     if self._compare_data(belf_goal,data,ck_type,ck_args,ck_src):
                         found_data.append(plan_event)
                         if not all: return plan_event
 
             case _: pass
-        return found_data
+        return found_data if found_data else None
 
     def _to_belief_goal(self, data_type: Belief | Goal | Plan | Event):
         change = None
         belief_goal:Belief | Goal = None
         match data_type:
             case Belief() | Goal():
                 belief_goal = data_type
@@ -477,15 +482,16 @@
             raise RunPlanError
 
     # TODO: implement stoping plan
     def _stop_plan(self, plan):
         self.print(f"Stoping {plan})")  if self.full_log else ...
         pass
     
-    def send(self, target: str | tuple | List, act: TypeVar, msg: MSG | str, channel: str = Channel()._my_name):  
+    def send(self, target: str | tuple | List, act: TypeVar, msg: MSG | str, channel: str = DEFAULT_CHANNEL):  
+        if type(target) == str: target = (target,1) 
         try:
             self._channels[channel]._send(self.my_name,target,act,msg)
         except KeyError:
             self.print(f"Not Connected to Selected Channel:{channel}")
     
     def save_msg(self, act, msg):
         if self.instant_mail: 
@@ -570,24 +576,25 @@
         self.print("Shutting Down...")
         self.stop_flag.set()
         self.paused_agent = True
         self.running = False
             
     def cycle(self, stop_flag):
         while not stop_flag.is_set():   
+            self.print(f"#### New cycle ####") if self.show_cycle else ...
             self._perception()   
             self._mail()  
             event = self._select_event()
-            self.print(f"Selected event: {event} in {self.__events}") if self.full_log else ...
+            self.print(f"Selected event: {event} in {self.__events}") if self.show_cycle else ...
             plans = self._retrieve_plans(event)
-            self.print(f"Selected plans: {plans} in {self._plans}") if self.full_log else ...
+            self.print(f"Selected plans: {plans} in {self._plans}") if self.show_cycle else ...
             chosen_plan, args = self._select_plan(plans,event)
-            self.print(f"Selected chosen_plan: {chosen_plan} with {args} arguments") if self.full_log else ...
+            self.print(f"Selected chosen_plan: {chosen_plan} with {args} arguments") if self.show_cycle else ...
             result = self._execute_plan(chosen_plan,event,args)
-            #sleep(1)
+            if self.sleep: sleep(self.sleep)
 
     def _perception(self):
         percept_dict = dict()
         for env_name in self._environments:
             self.print(f"Percepting '{env_name}'") if self.full_log else ...
             percept_dict.update(self._environments[env_name].perception())
         percept_dict = self._percepts_to_beliefs(percept_dict)
@@ -595,15 +602,15 @@
     
     def _percepts_to_beliefs(self,percepts: dict) -> dict:
         # TODO make use of percepts group
         for source, keys in percepts.copy().items():
             for key,percepts_set in keys.items():
                 belief_set = set()
                 for percept in percepts_set:
-                    belief_set.add(Belief(percept.key,percept.args,source))
+                    belief_set.add(Belief(percept.key,percept.args,source,percept.adds_event))
                 percepts[source][key] = belief_set
         return percepts
      
     def _revise_beliefs(self, percept_dict: dict):
         for source, keys in self.__beliefs.copy().items():
             if source == DEFAULT_SOURCE: continue
             if source in percept_dict:
@@ -643,15 +650,15 @@
         
         args = tuple()
         for plan in plans:
             for context in plan.context:
                 ctxt = self.get(context,ck_src=False)
                 if not ctxt:
                     break
-                for x in ctxt[0]._args:
+                for x in ctxt._args:
                     args += (x,)
             else:    
                 return plan, args
         self.print(f"Found no applicable plan for {event.change}:{event.data}") if self.full_log else ...
         return None, None
     
     def _execute_plan(self, chosen_plan:Plan, event: Event, args):
```

### Comparing `maspy-ml-0.0.4/maspy/communication.py` & `maspy-ml-0.1.0/maspy/communication.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,22 +28,27 @@
             if __my_name not in cls._instances:
                 instance = super().__call__(__my_name)
                 cls._instances[__my_name] = instance
         return cls._instances[__my_name]
 
 
 class Channel(metaclass=CommsMultiton):
-    def __init__(self, comm_name) -> None:
+    def __init__(self, comm_name):
+        self.full_log = False
+        
+        from maspy.admin import Admin
+        self._my_name = comm_name
+        Admin()._add_channel(self)
+        
         from maspy.agent import Belief, Goal, Ask, Plan
         self.data_types = {Belief,Goal,Ask,Plan}
         self._my_name = comm_name
         self.agent_list: Dict[Agt_cls, Dict[Agt_name, Agt_fullname]] = {}
         self._agents: Dict[Agt_fullname, Agt_inst] = {}
         self._name = f"{type(self).__name__}:{self._my_name}"
-        self.full_log = True
         
     def print(self,*args, **kwargs):
         return print(f"{self._name}>",*args,**kwargs)
     
     def add_agents(self, agents):
         try:
             for agent in agents:
@@ -59,15 +64,15 @@
             else:
                 self.agent_list[type(agent).__name__].update({agent.my_name[0] : {agent.my_name}})
                 self._agents[agent.my_name] = agent
         else:
             self.agent_list[type(agent).__name__] = {agent.my_name[0] : {agent.my_name}}
             self._agents[agent.my_name] = agent
         
-        self.print(f'Connecting agent {type(agent).__name__}:{agent.my_name}')
+        self.print(f'Connecting agent {type(agent).__name__}:{agent.my_name}') if self.full_log else ...
 
             
     def _rm_agents(self, agents):
         try:
             for agent in agents:
                 self._rm_agent(agent)
         except TypeError:
@@ -75,15 +80,15 @@
 
     def _rm_agent(self, agent):
         if agent.my_name in self._agents:
             del self._agents[agent.my_name]
             del self.agent_list[type(agent).__name__][agent.my_name[0]]
         self.print(
             f"Desconnecting agent {type(agent).__name__}:{agent.my_name}"
-        )
+        ) if self.full_log else ...
 
     def _send(self, sender, target, act, message):  
         if type(act) == TypeVar: act = act.__name__ 
         
         messages = []
         if type(message) == Iterable:
             for m in message:
```

### Comparing `maspy-ml-0.0.4/maspy/environment.py` & `maspy-ml-0.1.0/maspy/environment.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 DEFAULT_GROUP = "default"
 
 @dataclass
 class Percept:
     key: str
     _args: tuple = field(default_factory=tuple)
     group: str = DEFAULT_GROUP # Percept Type (still unsure)
+    adds_event: bool = True
     
     @property
     def args(self):
         if len(self._args) > 1:
             return self._args
         elif len(self._args) == 1:
             return self._args[0]
@@ -47,29 +48,33 @@
 
         return hash((self.key, args_hashable, self.group))
 
 class EnvironmentMultiton(type):
     _instances: Dict[str, "Environment"] = {}
     _lock: Lock = Lock()
 
-    def __call__(cls, env_name=None):
+    def __call__(cls, env_name=None,full_log=False):
         with cls._lock:
             _my_name = env_name if env_name else str(cls.__name__)
             if _my_name not in cls._instances:
-                if env_name:
-                    instance = super().__call__(_my_name)
-                else:
-                    instance = super().__call__()
+                vars = []
+                if env_name: vars.append(env_name)
+                if full_log: vars.append(full_log)
+                instance = super().__call__(*vars)
                 cls._instances[_my_name] = instance
         return cls._instances[_my_name]
 
 class Environment(metaclass=EnvironmentMultiton):
-    def __init__(self, env_name=None):
+    def __init__(self, env_name=None,full_log=False):
         self._my_name = env_name if env_name else type(self).__name__
-        self.full_log = False
+        self.full_log = full_log
+        
+        from maspy.admin import Admin
+        Admin()._add_channel(self)
+        
         self.agent_list = {}
         self._agents = {}
         self._name = f"Environment:{self._my_name}"
         self._percepts: Dict[str, Dict[str, Set[Percept]]] = dict()
     
     def print(self,*args, **kwargs):
         return print(f"{self._name}>",*args,**kwargs)
@@ -101,35 +106,36 @@
             else:
                 self.agent_list[type(agent).__name__].update({agent.my_name[0] : {agent.my_name}})
                 self._agents[agent.my_name] = agent
         else:
             self.agent_list[type(agent).__name__] = {agent.my_name[0] : {agent.my_name}}
             self._agents[agent.my_name] = agent
         
-        self.print(f'Connecting agent {type(agent).__name__}:{agent.my_name}')
+        self.print(f'Connecting agent {type(agent).__name__}:{agent.my_name}') if self.full_log else ...
     
-    def create_percept(self, 
+    def create(self, 
             percept: Iterable[Percept] | Percept
         ):
         percept_dict = self._clean(percept)
             
-        self._percepts = utils.merge_dicts(self._percepts,percept_dict)
-        self.print(f"Creating percept {percept_dict}") if self.full_log else ...
+        utils.merge_dicts(percept_dict, self._percepts)
+        self.print(f"Creating {percept}") if self.full_log else ...
 
-    def get(self, percept:Percept, all=False, ck_group=False, ck_args=True) -> List[Percept] | Percept:
+    def get(self, percept:Percept, all=False, ck_group=False, ck_args=True) -> List[Percept] | Percept | None:
         found_data = []
         for group, keys in self._percepts.items():
             for key, prcs in keys.items():
                 for prcpt in prcs:
                     if self._compare_data(prcpt,percept,ck_group,ck_args):
                         if not all:
                             return prcpt
                         else:
                             found_data.append(prcpt)
-        return found_data
+                            
+        return found_data if found_data else None
                     
     def _compare_data(self, data1: Percept, data2: Percept, ck_group,ck_args):
         #self.print(f"Comparing: \n\t{data1} and {data2}")
         if ck_group and data1.group != data2.group:
         #    self.print("Failed at group")
             return False
         if data1.key != data2.key:
@@ -150,29 +156,23 @@
             else:
         #        self.print(f"Failed at args {arg1} x {arg2}")
                 return False
         else:
         #    self.print("Data is Compatible")
             return True
     
-    def change_percept(self, key: str, old_args: Any = tuple(), new_args: Any = tuple(), group: Optional[str] = DEFAULT_GROUP):
-        if type(old_args) is not tuple: old_args = (old_args,) 
+    def change(self, old_percept:Percept, new_args:Percept.args):
         if type(new_args) is not tuple: new_args = (new_args,) 
-        for percept in self._percepts[group][key]:
-            if percept == Percept(key,old_args,group): 
-                self.print(f"Updating {percept} to", end="")
-                percept.args = new_args
-                print(f" {percept}") 
-                break   
+        old_percept._args = new_args
             
     def _percept_exists(self, key, args, group=DEFAULT_GROUP) -> bool:
         if type(args) is not tuple: args = (args,)
         return Percept(key,args,group) in self._percepts[group][key]
 
-    def delete_percept(self, 
+    def delete(self, 
             key: str, 
             args: Optional[Any] = tuple(), 
             group: Optional[str] = DEFAULT_GROUP,
         ):
         if type(args) is not tuple: args = (args,) 
         self._percepts[group][key].remove(Percept(key,args,group))
```

### Comparing `maspy-ml-0.0.4/maspy/learning.py` & `maspy-ml-0.1.0/maspy/learning.py`

 * *Files identical despite different names*

### Comparing `maspy-ml-0.0.4/maspy/utils.py` & `maspy-ml-0.1.0/maspy/utils.py`

 * *Files identical despite different names*

### Comparing `maspy-ml-0.0.4/maspy_ml.egg-info/PKG-INFO` & `maspy-ml-0.1.0/maspy_ml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maspy-ml
-Version: 0.0.4
+Version: 0.1.0
 Summary: Multi-Agent Systems in Python with Machine Learning
 Author: Alexandre Mellado
 Author-email: <melladoallm@gamil.com>
 Keywords: python,autonomous agents,multi-agent system,machine learning
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `maspy-ml-0.0.4/setup.py` & `maspy-ml-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4'
+VERSION = '0.1.0'
 DESCRIPTION = 'Multi-Agent Systems in Python with Machine Learning'
 LONG_DESCRIPTION = 'A library for the devolopment of multi-agent systems with components of machine learning'
 
 # Setting up
 setup(
     name="maspy-ml",
     version=VERSION,
```

### Comparing `maspy-ml-0.0.4/tests/test_communication.py` & `maspy-ml-0.1.0/tests/test_communication.py`

 * *Files identical despite different names*

### Comparing `maspy-ml-0.0.4/tests/test_environment.py` & `maspy-ml-0.1.0/tests/test_environment.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,48 +16,48 @@
                 Percept("KEY",(2,)),
                 Percept("KEY",(3,)),
                 Percept("NEW_KEY")])
 
 def test_percepts_are_Percept():
     env = Environment("test_env1")
     with pytest.raises(Exception):
-        env.create_percept()
+        env.create()
         
-    env.create_percept("KEY")
-    env.create_percept("KEY",5)
-    env.create_percept("KEY",(1,2,3),"Normal")
-    env.create_percept("KEY",group="Normal")
-    env.create_percept(percept=Percept("B"))
-    env.create_percept(percept=[Percept("C",group="Normal"), Percept("D",(2,))])
+    env.create("KEY")
+    env.create("KEY",5)
+    env.create("KEY",(1,2,3),"Normal")
+    env.create("KEY",group="Normal")
+    env.create(percept=Percept("B"))
+    env.create(percept=[Percept("C",group="Normal"), Percept("D",(2,))])
     for group, keys in env._percepts.items():
             for key, percept_set in keys.items():
                 for percept in percept_set:
                     assert (type(percept) is Percept and percept.key == key and percept.group == group)
                     
 def test_delete_percepts():
     env = Environment("test_env2")
-    env.create_percept("KEY",23,"Normal")
-    env.create_percept("KEY",(42,27))
+    env.create("KEY",23,"Normal")
+    env.create("KEY",(42,27))
     assert Percept("KEY",(23,),"Normal") in env._percepts["Normal"]["KEY"]
     assert Percept("KEY",(42,27)) in env._percepts[DEFAULT_GROUP]["KEY"]
-    env.delete_percept("KEY",23,"Normal")
-    env.delete_percept("KEY",(42,27))
+    env.delete("KEY",23,"Normal")
+    env.delete("KEY",(42,27))
     assert Percept("KEY",(23,),"Normal") not in env._percepts["Normal"]["KEY"]
     assert Percept("KEY",(42,27)) not in env._percepts[DEFAULT_GROUP]["KEY"]
     
 def test_change_percept():
     env = Environment("change")
-    env.create_percept("KEY",42)
-    env.change_percept("KEY",42,27)
+    env.create("KEY",42)
+    env.change("KEY",42,27)
     assert Percept("KEY",(42,)) not in env._percepts[DEFAULT_GROUP]["KEY"]
     assert Percept("KEY",(27,)) not in env._percepts[DEFAULT_GROUP]["KEY"]
 
 def test_percept_exists():
     env = Environment("test_env3")
-    env.create_percept("KEY",23)
+    env.create("KEY",23)
     assert Percept("KEY",(23,)) in env._percepts[DEFAULT_GROUP]["KEY"] and \
         env._percept_exists("KEY",23)
     env.print_percepts
 
 def test_perception():
     env = Environment("test_env1")
     perception_dict, perception_list = env.perception()
```

