# Comparing `tmp/circuitree-0.9.8.tar.gz` & `tmp/circuitree-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitree-0.9.8.tar", max compression
+gzip compressed data, was "circuitree-0.9.9.tar", max compression
```

## Comparing `circuitree-0.9.8.tar` & `circuitree-0.9.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    35149 2023-08-08 23:12:20.534641 circuitree-0.9.8/LICENSE
--rw-r--r--   0        0        0     1011 2023-08-08 23:12:20.534641 circuitree-0.9.8/README.md
--rwxr-xr-x   0        0        0      118 2024-04-02 19:18:57.943202 circuitree-0.9.8/circuitree/__init__.py
--rwxr-xr-x   0        0        0    40695 2024-04-23 21:41:45.758026 circuitree-0.9.8/circuitree/circuitree.py
--rw-r--r--   0        0        0     1621 2023-10-23 22:25:37.646685 circuitree-0.9.8/circuitree/grammar.py
--rwxr-xr-x   0        0        0    32344 2024-04-17 22:29:27.655740 circuitree-0.9.8/circuitree/models.py
--rw-r--r--   0        0        0     3991 2023-08-29 19:51:25.141731 circuitree-0.9.8/circuitree/modularity.py
--rw-r--r--   0        0        0     6541 2023-11-14 01:41:12.991399 circuitree-0.9.8/circuitree/parallel.py
--rw-r--r--   0        0        0      758 2023-10-20 16:36:26.268282 circuitree-0.9.8/circuitree/utils.py
--rw-r--r--   0        0        0    18102 2024-04-23 20:34:18.519091 circuitree-0.9.8/circuitree/viz.py
--rw-r--r--   0        0        0     1285 2024-04-23 21:42:16.508016 circuitree-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     1871 1970-01-01 00:00:00.000000 circuitree-0.9.8/setup.py
--rw-r--r--   0        0        0     1678 1970-01-01 00:00:00.000000 circuitree-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-08 23:12:20.534641 circuitree-0.9.9/LICENSE
+-rw-r--r--   0        0        0     1011 2023-08-08 23:12:20.534641 circuitree-0.9.9/README.md
+-rwxr-xr-x   0        0        0      118 2024-04-02 19:18:57.943202 circuitree-0.9.9/circuitree/__init__.py
+-rwxr-xr-x   0        0        0    42015 2024-04-26 17:42:19.044777 circuitree-0.9.9/circuitree/circuitree.py
+-rw-r--r--   0        0        0     1621 2023-10-23 22:25:37.646685 circuitree-0.9.9/circuitree/grammar.py
+-rwxr-xr-x   0        0        0    32450 2024-04-26 17:42:19.374777 circuitree-0.9.9/circuitree/models.py
+-rw-r--r--   0        0        0     3991 2023-08-29 19:51:25.141731 circuitree-0.9.9/circuitree/modularity.py
+-rw-r--r--   0        0        0     6541 2023-11-14 01:41:12.991399 circuitree-0.9.9/circuitree/parallel.py
+-rw-r--r--   0        0        0      758 2023-10-20 16:36:26.268282 circuitree-0.9.9/circuitree/utils.py
+-rw-r--r--   0        0        0    19326 2024-04-26 18:15:31.504255 circuitree-0.9.9/circuitree/viz.py
+-rw-r--r--   0        0        0     1285 2024-04-26 18:19:42.744186 circuitree-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     1871 1970-01-01 00:00:00.000000 circuitree-0.9.9/setup.py
+-rw-r--r--   0        0        0     1678 1970-01-01 00:00:00.000000 circuitree-0.9.9/PKG-INFO
```

### Comparing `circuitree-0.9.8/LICENSE` & `circuitree-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `circuitree-0.9.8/README.md` & `circuitree-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `circuitree-0.9.8/circuitree/circuitree.py` & `circuitree-0.9.9/circuitree/circuitree.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         self,
         grammar: CircuitGrammar,
         root: str,
         exploration_constant: Optional[float] = None,
         seed: int = 2023,
         graph: Optional[nx.DiGraph] = None,
         tree_shape: Optional[Literal["tree", "dag"]] = None,
-        compute_symmetries: bool = True,
+        compute_unique: bool = True,
         **kwargs,
     ):
         self.rg = np.random.default_rng(seed)
         self.seed = self.rg.bit_generator._seed_seq.entropy
 
         self.root = root
         if graph is None:
@@ -60,15 +60,15 @@
             self.graph = graph
             if self.root not in self.graph:
                 raise ValueError(
                     f"Supplied graph does not contain the root node: {root}"
                 )
         self.graph.root = self.root
 
-        self.compute_symmetries = compute_symmetries
+        self.compute_symmetries = compute_unique
         if tree_shape is not None:
             if tree_shape not in ("tree", "dag"):
                 raise ValueError("Argument `tree_shape` must be `tree` or `dag`.")
             warnings.warn(
                 "The `tree_shape` argument is deprecated and will be removed in a "
                 "future version. Please use `compute_symmetries` instead."
             )
@@ -351,86 +351,116 @@
         run_kwargs = {} if run_kwargs is None else run_kwargs
         if callback is not None and callback_before_start:
             callback(self, -1, [None], None, None)
 
         for i in iterator:
             selection_path, reward, sim_node = self.traverse(**run_kwargs)
             if callback is not None and i % callback_every == 0:
-                _ = callback(self, i, selection_path, sim_node, reward)
+                callback(self, i, selection_path, sim_node, reward)
+
+        return
 
     def is_success(self, state: Hashable) -> bool:
         """Returns whether or not a state is successful. Used to infer which patterns
         lead to more successes (i.e. motif candidates)."""
         raise NotImplementedError
 
+    def copy_graph(self) -> nx.DiGraph:
+        """Return a shallow copy of the graph. Use copy.deepcopy() for a deep copy."""
+        return self.graph.copy()
+
+    def get_attributes(self, attrs_copy: Optional[Iterable[str]]) -> dict:
+        """Return a dictionary of the object's attributes. If `attrs_copy` is not
+        provided, all attributes are returned except those in the
+        `_non_serializable_attrs` list. If `attrs_copy` is provided, only the specified
+        attributes are returned. If any of the specified attributes are in
+        `_non_serializable_attrs`, a ValueError is raised.
+
+        If an attribute has a `to_dict()` method, it is called to get the attribute's
+        value. Otherwise, the attribute is copied as-is.
+        """
+
+        # Get the attributes to copy
+        if attrs_copy is None:
+            keys = set(self.__dict__.keys()) - set(self._non_serializable_attrs)
+        else:
+            keys = set(attrs_copy)
+            if non_serializable := (keys & set(self._non_serializable_attrs)):
+                repr_non_ser = ", ".join(non_serializable)
+                raise ValueError(
+                    f"Attempting to save non-serializable attributes: {repr_non_ser}."
+                )
+
+        # Copy the attributes
+        attrs_copy = {}
+        for k, v in self.__dict__.items():
+            if k not in keys:
+                continue
+            if hasattr(v, "to_dict"):
+                attrs_copy[k] = v.to_dict()
+            else:
+                attrs_copy[k] = v
+
+        return attrs_copy
+
     def to_file(
         self,
         gml_file: str | Path,
         json_file: Optional[str | Path] = None,
         save_attrs: Optional[Iterable[str]] = None,
         compress: bool = False,
         **kwargs,
     ):
+        """Save the CircuiTree object to a gml file and optionally a json file
+        containing the object's attributes. The `save_attrs` argument can be used to
+        specify which attributes to save. If `compress` is True, the gml file is
+        compressed with gzip.
+
+        A saved CircuiTree object can be loaded with the `from_file` class method.
+
+        The grammar is saved by calling its `to_dict()` method, which returns a
+        dictionary of the grammar's attributes and its class name string
+        `__grammar_cls__`. These attributes are saved in the JSON file and used to
+        create the grammar object upon loading."""
+
+        # Save the graph
         if compress:
             gml_target = Path(gml_file).with_suffix(".gml.gz")
         else:
             gml_target = Path(gml_file).with_suffix(".gml")
         nx.write_gml(self.graph, gml_target, **kwargs)
 
+        # Save the other attributes
         if json_file is not None:
-            if save_attrs is None:
-                keys = set(self.__dict__.keys()) - set(self._non_serializable_attrs)
-            else:
-                keys = set(save_attrs)
-                if non_serializable := (keys & set(self._non_serializable_attrs)):
-                    repr_non_ser = ", ".join(non_serializable)
-                    raise ValueError(
-                        f"Attempting to save non-serializable attributes: {repr_non_ser}."
-                    )
-
-            attrs = {}
-            for k, v in self.__dict__.items():
-                if k not in keys:
-                    continue
-                if hasattr(v, "to_dict"):
-                    attrs[k] = v.to_dict()
-                else:
-                    attrs[k] = v
-
+            attrs = self.get_attributes(save_attrs)
             json_target = Path(json_file).with_suffix(".json")
             with json_target.open("w") as f:
                 json.dump(attrs, f, indent=4)
-
             return gml_target, json_target
-
         else:
             return gml_target
 
     @classmethod
     def from_file(
         cls,
         graph_gml: str | Path | None,
         attrs_json: str | Path,
         grammar_cls: Optional[CircuitGrammar] = None,
         grammar_kwargs: Optional[dict] = None,
         **kwargs,
     ):
         """Load a CircuiTree from a gml file and a JSON file containing the object's
-        attributes.
+        attributes, typically saved with the `to_file` method.
 
         The grammar attribute is loaded by looking for a key "grammar" in the JSON file,
         whose value should be a dict `grammar_kwargs` used to create a grammar object.
         The grammar_cls keyword can be passed to specify the class constructor for the
         grammar object. Alternatively, if `grammar_kwargs` contains a key
         "__grammar_cls__" that specifies a class name string, that class will be found
         in globals() and used to construct the grammar object.
-
-        When dumping a CircuiTree to a JSON file, the grammar object is dumped using
-        the method `to_dict()`, which automatically creates the "__grammar_cls__"
-        key-value entry.
         """
         # Load the attributes from the json file
         with open(attrs_json, "r") as f:
             kwargs.update(json.load(f))
 
         # Make the grammar object
         # Get kwargs from the grammar_kwargs in this function and/or from the json
@@ -575,24 +605,24 @@
     ) -> list[Hashable]:
         """Sample a random successful state by first creating a new graph that contains
         all possible paths from the root to a successful terminal state. Then, sample
         paths by random traversal from the root."""
 
         # Check if is_success() is implemented
         try:
-            _ = self.grammar.is_success(next(self.terminal_states))
+            _ = self.is_success(self.root)
         except NotImplementedError:
             raise NotImplementedError(
                 "The CircuiTree subclass must implement the is_success() method to "
                 "use this function."
             )
 
         ## Create a graph with all possible paths to success
         successful_terminals = set(
-            s for s in self.terminal_states if self.grammar.is_success(s)
+            s for s in self.terminal_states if self.is_success(s)
         )
 
         # Generate the graph with all possible paths to success
         all_paths_to_success = self.grow_tree_from_leaves(successful_terminals)
 
         if nprocs == 1:
             samples = self._sample_leaves(
@@ -636,24 +666,24 @@
     ) -> list[Hashable]:
         """Sample a random successful state with rejection sampling. Starts from the
         root state, selects random actions until termination, and accepts the sample if
         it is successful."""
 
         # Check if is_success() is implemented
         try:
-            _ = self.grammar.is_success(next(self.terminal_states))
+            _ = self.is_success(self.root)
         except NotImplementedError:
             raise NotImplementedError(
                 "The CircuiTree subclass must implement the is_success() method to "
                 "use this function."
             )
 
         # Use rejection sampling to sample paths with the given pattern
         successful_terminals = set(
-            s for s in self.terminal_states if self.grammar.is_success(s)
+            s for s in self.terminal_states if self.is_success(s)
         )
         if progress:
             from tqdm import tqdm
 
             pbar = tqdm(desc="Sampling successful terminal circuits", total=n_samples)
         if nprocs == 1:
             samples = []
@@ -944,30 +974,30 @@
     ) -> nx.DiGraph:
         if isinstance(successes, Iterable):
             successful_children = set(successes)
         elif successes is True:
 
             # Check if is_success() is implemented
             try:
-                _ = self.grammar.is_success(next(self.terminal_states))
+                _ = self.is_success(self.root)
             except NotImplementedError:
                 raise NotImplementedError(
                     "If successes=True, the CircuiTree subclass must implement "
                     "the is_success() method."
                 )
 
             # Keep only the successful nodes
             successful_children = set(
-                c for c in self.terminal_states if self.grammar.is_success(c)
+                c for c in self.terminal_states if self.is_success(c)
             )
         elif successes is False:
             # keep all terminal nodes
             successful_children = set(self.terminal_states)
         else:
-            raise ValueError(f"Invalid value for successes: {successes}")
+            raise ValueError(f"Invalid value for `successes`: {successes}")
 
         # Store the attributes of the terminal states
         child_attrs: dict[Hashable, dict[str, Any]] = {}
         for child in successful_children:
             parents = [p for p, _ in self.graph.in_edges(child)]
             for p in parents:
                 child_attrs[(p, child)] = self.graph.edges[(p, child)]
```

### Comparing `circuitree-0.9.8/circuitree/grammar.py` & `circuitree-0.9.9/circuitree/grammar.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.9.8/circuitree/models.py` & `circuitree-0.9.9/circuitree/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,16 +28,18 @@
         self,
         components: Iterable[Iterable[str]],
         interactions: Iterable[str],
         max_interactions: Optional[int] = None,
         root: Optional[str] = None,
         cache_maxsize: int | None = 128,
         fixed_components: Optional[list[str]] = None,
+        *args,
+        **kwargs,
     ):
-        super().__init__()
+        super().__init__(*args, **kwargs)
 
         if len(set(c[0] for c in components)) < len(components):
             raise ValueError("First character of each component must be unique")
         if len(set(c[0] for c in interactions)) < len(interactions):
             raise ValueError("First character of each interaction must be unique")
 
         self.root = root
@@ -48,52 +50,53 @@
 
         if max_interactions is None:
             self.max_interactions = len(self.components) ** 2  # all possible edges
         else:
             self.max_interactions = max_interactions
 
         self.fixed_components = fixed_components or []
-        self.recolorable_components = [
-            c for c in self.components if c not in self.fixed_components
-        ]
 
         # Allow user to specify a cache size for the get_interaction_recolorings method.
         # This method is called frequently during search, and evaluation can become a
         # bottleneck for large spaces. Caching the results of this method can
         # significantly speed up search, but cache size is limited by system memory.
-        self._cache_maxsize = cache_maxsize
+        self.cache_maxsize = cache_maxsize
         self.get_interaction_recolorings: Callable[[str], list[str]] = lru_cache(
-            maxsize=self._cache_maxsize
+            maxsize=self.cache_maxsize
         )(self._get_interaction_recolorings)
 
         # Attributes that should not be serialized when saving the object to file
         self._non_serializable_attrs.extend(
             [
                 "component_map",
                 "interaction_map",
                 "edge_options",
                 "component_codes",
                 "_recolor",
                 "get_interaction_recolorings",
             ]
         )
 
+    @property
+    def recolorable_components(self) -> list[str]:
+        return [c for c in self.components if c not in self.fixed_components]
+
     def __getstate__(self):
         result = copy(self.__dict__)
 
         # We need to remove the lru_cache object because it is not serializable. We
         # will re-initialize it in the __setstate__ method.
         result["get_interaction_recolorings"] = NotImplemented
         return result
 
     def __setstate__(self, state):
         self.__dict__ = state
 
         # Re-initialize the lru_cache object
-        self.get_interaction_recolorings = lru_cache(maxsize=self._cache_maxsize)(
+        self.get_interaction_recolorings = lru_cache(maxsize=self.cache_maxsize)(
             self._get_interaction_recolorings
         )
 
     @cached_property
     def edge_options(self):
         return [
             [c1[0] + c2[0] + ixn[0] for ixn in self.interactions]
@@ -367,15 +370,15 @@
         super().__init__(
             grammar=grammar,
             root=root,
             exploration_constant=exploration_constant,
             seed=seed,
             graph=graph,
             tree_shape=tree_shape,
-            compute_symmetries=compute_symmetries,
+            compute_unique=compute_symmetries,
             **kwargs,
         )
 
 
 class DimersGrammar(CircuitGrammar):
     """A grammar class for circuits consisting of dimerizing molecules."""
 
@@ -384,16 +387,18 @@
         components: Iterable[str],
         regulators: Iterable[str],
         interactions: Iterable[str],
         max_interactions: Optional[int] = None,
         max_interactions_per_promoter: int = 2,
         root: Optional[str] = None,
         cache_maxsize: int | None = 128,
+        *args,
+        **kwargs,
     ):
-        super().__init__()
+        super().__init__(*args, **kwargs)
 
         if len(set(c[0] for c in components)) < len(components):
             raise ValueError("First character of each component must be unique")
         if len(set(c[0] for c in regulators)) < len(regulators):
             raise ValueError("First character of each component must be unique")
         if len(set(c[0] for c in interactions)) < len(interactions):
             raise ValueError("First character of each interaction must be unique")
@@ -807,10 +812,10 @@
         super().__init__(
             grammar=grammar,
             root=root,
             exploration_constant=exploration_constant,
             seed=seed,
             graph=graph,
             tree_shape=tree_shape,
-            compute_symmetries=compute_symmetries,
+            compute_unique=compute_symmetries,
             **kwargs,
         )
```

### Comparing `circuitree-0.9.8/circuitree/modularity.py` & `circuitree-0.9.9/circuitree/modularity.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.9.8/circuitree/parallel.py` & `circuitree-0.9.9/circuitree/parallel.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.9.8/circuitree/utils.py` & `circuitree-0.9.9/circuitree/utils.py`

 * *Files identical despite different names*

### Comparing `circuitree-0.9.8/circuitree/viz.py` & `circuitree-0.9.9/circuitree/viz.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,166 +51,178 @@
 
 ## Search graph visualization
 
 
 def complexity_layout(
     tree: CircuiTree,
     dy: float = 0.5,
-    aspect_ratio: float = 2.0,
+    aspect: float = 2.0,
 ) -> tuple[dict[str, int], dict[str, tuple[float, float]]]:
     """Returns the depth and xy coordinates of each node in the search graph when
     visualized based on complexity.
 
     In a complexity layout, a search graph is represented by a series of layers, where
     each layer contains nodes that have the same complexity, which is measured as the
     depth, or distance from the root node. Layers are separated in the y direction, and
     in the x direction, nodes in the same layer are sorted by the number of visits they
     have received. Terminal nodes are subsumed into their parent nonterminals.
     """
 
-    # Convert the the search graph as a "complexity graph" - subsumes terminal nodes
-    # into their parent nonterminals
-    G = tree.to_complexity_graph()
+    # Convert the search graph to a complexity graph, where terminal nodes are subsumed
+    # into their parent nonterminals.
+    G = tree.to_complexity_graph(successes=False)
 
     # Get the depth of each node (distance from the root)
     depth_of_node = {}
-    for i, layer in enumerate(nx.bfs_layers(G, source=tree.root)):
+    for i, layer in enumerate(nx.bfs_layers(tree.graph, sources=tree.root)):
         for n in layer:
-            depth_of_node[n] = i
+            if n in G.nodes:
+                depth_of_node[n] = i
 
-    layer_counter = Counter(depth_of_node)
-    max_layer_size = layer_counter.most_common(1)[0][1]
+    layer_counter = Counter(depth_of_node.values())
+    max_layer_size = max(layer_counter.values(), default=0)
 
-    # Sort nodes by depth, then by descending number of visits
-    node_visits_inv = -np.array([G.nodes[n]["visits"] for n in G.nodes])
-    node_depth = np.array([depth_of_node[n] for n in G.nodes])
-    node_order = np.lexsort((node_visits_inv, node_depth))
-    node_depth = node_depth[node_order]
-
-    # Get the min and max x values for each layer
-    yvals = dy * (node_depth.max() - node_depth)
-    y_max = yvals.max()
-    x_max = y_max * aspect_ratio
-    dx = x_max / max_layer_size
+    if max_layer_size == 0:
+        return np.array([], dtype=np.float64), {}
 
-    # Evenly space nodes in the x direction within each layer
+    # Get the complexity as the distance from the root to each node
+    nodes = np.array(list(G.nodes))
+    complexity = np.array([depth_of_node[n] for n in nodes])
+    visits = np.array([G.nodes[n]["visits"] for n in nodes])
+    order = np.lexsort((-visits, complexity))
+    nodes = nodes[order]
+    complexity = complexity[order]
+
+    # Get y coordinates for each node based on complexity
+    yvals = -dy * complexity
+    height = dy * complexity.max(initial=0) + dy / 2
+
+    # Evenly space nodes in the x direction within each layer. Sort nodes in the
+    # x-direction by the number of visits they have received.
+    width = height * aspect
+    dx = width / max_layer_size
     xvals = np.zeros_like(yvals)
-    for d, n_d in layer_counter.items():
-        xvals_d = np.arange(n_d) * dx
-        xvals_d = xvals_d - xvals_d.mean()
-        xvals[node_depth == d] = xvals_d
+    for c, n_c in layer_counter.items():
+        xvals_c = np.arange(n_c) * dx
+        xvals_c = xvals_c - xvals_c.mean()
+        xvals[complexity == c] = xvals_c
 
-    pos = {n: (x, y) for n, x, y in zip(G.nodes, xvals, yvals)}
-    return depth_of_node, pos
+    pos = {n: (x, y) for n, x, y in zip(nodes, xvals, yvals)}
+    return complexity, pos
 
 
 def plot_complexity(
     tree: CircuiTree,
-    depth_of_node: Optional[dict[str, int]] = None,
+    complexity: Optional[dict[str, int]] = None,
     pos: Optional[dict[str, tuple[float, float]]] = None,
-    vlim: tuple[int | float] = (10, None),
-    vscale: Literal["log", "lin", "flat"] = "log",
+    vlim: tuple[int | float] = (None, None),
+    vscale: Literal["log", "lin", "flat"] = "flat",
     figsize: tuple[float, float] = (6, 3),
-    alpha: float = 0.8,
+    alpha: float = 0.25,
     lw: float = 1.0,
+    complexity_labels: bool = True,
     plot_layers_as_blocks: bool = True,
-    block_height: float = 0.1,
-    block_clr: str = "gray",
+    block_height: float = 0.075,
+    block_clr: str = "lightsteelblue",
     marker_clr: str = "k",
     marker_size: float = 10,
     n_to_highlight: Optional[float] = None,
+    highlight_min_visits: int = 1,
     highlight_clr: str = "tab:orange",
     fig: Optional[plt.Figure] = None,
     ax: Optional[plt.Axes] = None,
+    **kwargs,
 ) -> None:
 
-    G = tree.to_complexity_graph()
-
-    if depth_of_node is None or pos is None:
-        print("Computing layout...")
-        depth_of_node, pos = complexity_layout(tree)
-
-    xvals, yvals = zip(*pos.values())
+    # Convert the search graph to a complexity graph, where terminal nodes are subsumed
+    # into their parent nonterminals.
+    G = tree.to_complexity_graph(successes=False)
+
+    if complexity is None or pos is None:
+        complexity, pos = complexity_layout(tree, **kwargs)
+
+    if len(pos) == 0:
+        xvals = []
+        yvals = []
+    else:
+        xvals, yvals = zip(*pos.values())
     xvals = np.array(xvals)
     yvals = np.array(yvals)
 
     # Get the limits for the number of visits - only show edges with visits in this range
+    visits = np.array([v for *e, v in G.edges(data="visits")])
     if vlim[0] is None:
-        vmin = min(v for *e, v in G.edges(data="visits"))
+        vmin = max(visits.min(initial=1), 1)  # ignore zero visits
     else:
         vmin = vlim[0]
     if vlim[1] is None:
-        vmax = max(v for *e, v in G.edges(data="visits"))
+        vmax = visits.max(initial=1)
     else:
         vmax = vlim[1]
 
-    total_visits_at_depth = Counter()
-    for n1, n2 in G.edges:
-        depth = depth_of_node[n1[0]]
-        total_visits_at_depth[depth] += G.edges[n1]["visits"]
-
     # Decide how to normalize the edge weights - on a log/linear scale or flat
     if vscale == "log":
         log_vmin = np.log10(vmin)
         log_vrange = np.log10(vmax) - log_vmin
-
-        def normalize(v):
-            return np.clip((np.log10(v) - log_vmin) / log_vrange, 0, 1)
-
+        weights = np.clip((np.log10(visits) - log_vmin) / log_vrange, 0, 1)
     elif vscale == "lin":
         vrange = vmax - vmin
-
-        def normalize(v):
-            return np.clip((v - vmin) / vrange, 0, 1)
-
+        weights = np.clip((visits - vmin) / vrange, 0, 1)
     elif vscale == "flat":
-
-        def normalize(v):
-            return 1
+        weights = (visits >= vmin).astype(float)
 
     else:
-        raise ValueError(f"Invalid vscale: {vscale}. Must be 'log' or 'lin'.")
+        raise ValueError(f"Invalid vscale: {vscale}. Must be 'flat', 'log', or 'lin'.")
 
-    # Compute weights for edges
-    weights = []
-    for n1, n2, v in G.edges(data="visits"):
-        depth = depth_of_node[n1]
-        weights.append(normalize(v))
-    weights = np.array(weights)
-
-    # # Black edges with alpha proportional to the weight
-    # edge_colors = np.zeros((len(weights), 4))
-    # edge_colors[:, 3] = alpha * weights
+    # Black edges with transparency (alpha) proportional to the weight
+    edge_colors = np.zeros((len(weights), 4))
+    edge_colors[:, 3] = alpha * weights
 
     if fig is None:
         fig = plt.figure(figsize=figsize)
     if ax is None:
         ax = fig.add_subplot(1, 1, 1)
 
+    # Turn of all axis spines
+    ax.spines["top"].set_visible(False)
+    ax.spines["right"].set_visible(False)
+    ax.spines["left"].set_visible(False)
+    ax.spines["bottom"].set_visible(False)
+
+    # Turn off x axis ticks
+    ax.set_xticks([])
+
+    if complexity_labels:
+        # Turn off y axis ticks but keep labels
+        ax.set_yticks(np.unique(yvals)[::-1])
+        ax.set_yticklabels([f"{d}" for d in np.unique(complexity)])
+        ax.yaxis.set_ticks_position("none")
+        ax.set_ylabel("Complexity")
+    else:
+        ax.set_yticks([])
+
     # set edge positions
     if plot_layers_as_blocks:
         ybias = 0.5 * block_height
     else:
         ybias = 0.0
     edge_pos = []
     for n1, n2 in G.edges:
-        x1, y1 = pos[n1[0]]
-        x2, y2 = pos[n2[0]]
+        x1, y1 = pos[n1]
+        x2, y2 = pos[n2]
         edge_pos.append(((x1, y1 - ybias), (x2, y2 + ybias)))
     edge_pos = np.array(edge_pos)
 
     # Draw edges
     edges = mpl_coll.LineCollection(
         edge_pos,
-        # colors=edge_colors,
-        colors=weights,
+        colors=edge_colors,
         linewidths=lw,
         antialiaseds=(1,),
         linestyle="-",
-        alpha=alpha,
     )
     edges.set_zorder(0)  # edges go behind nodes
     ax.add_collection(edges)
 
     # edges = nx.draw_networkx_edges(
     #     G,
     #     G_pos,
@@ -221,19 +233,19 @@
     #     node_size=0,
     # )
     # edges.set_zorder(0)
 
     if plot_layers_as_blocks:
         # Plot a gray horizontal rectangle to represent each layer of nodes
         rects = []
-        for d in np.unique(depth_of_node.values()):
-            d_mask = depth_of_node == d
-            xmin = xvals[d_mask].min()
-            xmax = xvals[d_mask].max()
-            yval = yvals[d_mask][0]
+        for c in np.unique(complexity):
+            c_mask = complexity == c
+            xmin = xvals[c_mask].min()
+            xmax = xvals[c_mask].max()
+            yval = yvals[c_mask][0]
             rect = Rectangle(
                 (xmin, yval - 0.5 * block_height),
                 width=xmax - xmin,
                 height=block_height,
                 color=block_clr,
                 zorder=1,
             )
@@ -247,37 +259,52 @@
             ax.scatter(x, y, color=marker_clr, s=marker_size, zorder=1)
 
     # for xmin_d, xmax_d, yval_d in zip(depth_xmins, depth_xmaxs, depth_yvals):
     #     plt.hlines(yval_d, xmin_d, xmax_d, color="gray", zorder=4, lw=1.0)
 
     if n_to_highlight is not None:
 
-        # Get locations of the top "N" oscillators
+        # Get the states with the highest mean reward among states that were
+        # visited at least "higlight_min_visits" times
+        states_to_consider = (
+            n
+            for n in tree.terminal_states
+            if tree.graph.nodes[n]["visits"] >= highlight_min_visits
+        )
         highlight_states = sorted(
-            tree.terminal_states, key=lambda n: -tree.graph.nodes[n]["visits"]
+            states_to_consider,
+            key=lambda n: (
+                tree.graph.nodes[n].get("reward", 0)
+                / tree.graph.nodes[n].get("visits", 1)
+            ),
+            reverse=True,
         )[:n_to_highlight]
+
+        # Get the coordinates for the top states
         top_states_pos = []
         for state in highlight_states:
             nonterm = state.lstrip("*")
             if nonterm in pos:
                 top_states_pos.append(pos[nonterm])
         top_states_pos = np.array(top_states_pos)
 
-        # Highlight the top N oscillators
+        # Plot a marker to highlight the top states
         if top_states_pos.size > 0:
             plt.scatter(
                 *top_states_pos.T,
                 color=highlight_clr,
                 s=15,
                 zorder=5,
                 edgecolors="k",
                 lw=0.3,
             )
 
-    ax.set_axis_off()
+    # axes_lims = xvals.min(), xvals.max(), yvals.min(), yvals.max()
+    # ax.axis(axes_lims)
+    ax.axis("equal")
 
     return fig, ax
 
 
 ## Plot a diagram of an N-component network (see models.SimpleNetworkTree)
```

### Comparing `circuitree-0.9.8/pyproject.toml` & `circuitree-0.9.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "circuitree"
-version = "0.9.8"
+version = "0.9.9"
 description = "Genetic circuit design using Monte Carlo tree search"
 authors = ["pranav-bhamidipati <pbhamidi@usc.edu>"]
 license = "GPLv3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `circuitree-0.9.8/setup.py` & `circuitree-0.9.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['networkx>=3.1,<4.0', 'numpy>=1.23.0,<2.0.0', 'pandas>=2.0.0,<3.0.0']
 
 extras_require = \
 {':python_version >= "3.10" and python_version < "3.13"': ['scipy>=1.11.3,<2.0.0']}
 
 setup_kwargs = {
     'name': 'circuitree',
-    'version': '0.9.8',
+    'version': '0.9.9',
     'description': 'Genetic circuit design using Monte Carlo tree search',
     'long_description': '# CircuiTree\nGenetic circuit design using Monte Carlo tree search\n\n## Installation\n\n### From a package repository\nTo install using `pip`:\n\n```pip install circuitree```\n\n### From the GitHub repository\n\nTo install and use `circuitree` from the GitHub source code, first clone the repo into a directory.\n\n```git clone https://github.com/pranav-bhamidipati/circuitree.git[ dir_name]```\n\nThen, you can build the environment using the command-line tool `poetry`. Instructions for installation can be [found here](https://python-poetry.org/). \n\nFrom the main project directory, run `poetry install` to install a virtual environment with `circuitree` installed. The easiest way to use this environment is to run it interactively with `poetry shell`. Alternatively, you can run a command in the virtual environment with `poetry run <command>`. For instance, to launch a Jupyter notebook with `circuitree` pre-loaded, run `poetry run jupyter notebook`. \n\n## Usage\n\nSee the [quick-start demo](examples/quick_start.ipynb).\n',
     'author': 'pranav-bhamidipati',
     'author_email': 'pbhamidi@usc.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `circuitree-0.9.8/PKG-INFO` & `circuitree-0.9.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: circuitree
-Version: 0.9.8
+Version: 0.9.9
 Summary: Genetic circuit design using Monte Carlo tree search
 License: GPLv3
 Author: pranav-bhamidipati
 Author-email: pbhamidi@usc.edu
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

