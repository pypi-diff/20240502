# Comparing `tmp/wgdtree-0.0.2.tar.gz` & `tmp/wgdtree-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/nick/Proj/wgd/wgdtree/dist/tmpl2l86_un/wgdtree-0.0.2.tar", last modified: Thu Dec 16 22:21:43 2021, max compression
+gzip compressed data, was "wgdtree-1.0.tar", last modified: Thu May  2 16:35:18 2024, max compression
```

## Comparing `wgdtree-0.0.2.tar` & `wgdtree-1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2021-12-16 22:21:43.000000 wgdtree-0.0.2/
--rw-r--r--   0 nick      (1000) nick      (1000)     1074 2021-06-05 17:45:21.000000 wgdtree-0.0.2/LICENSE
--rw-r--r--   0 nick      (1000) nick      (1000)     3559 2021-12-16 22:21:43.000000 wgdtree-0.0.2/PKG-INFO
--rw-r--r--   0 nick      (1000) nick      (1000)     2992 2021-11-10 00:27:00.000000 wgdtree-0.0.2/README.md
--rw-r--r--   0 nick      (1000) nick      (1000)      118 2021-06-12 21:33:45.000000 wgdtree-0.0.2/pyproject.toml
--rw-r--r--   0 nick      (1000) nick      (1000)      655 2021-12-16 22:21:43.000000 wgdtree-0.0.2/setup.cfg
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2021-12-16 22:21:43.000000 wgdtree-0.0.2/src/
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2021-12-16 22:21:43.000000 wgdtree-0.0.2/src/wgdtree/
--rw-r--r--   0 nick      (1000) nick      (1000)      230 2021-12-16 22:20:47.000000 wgdtree-0.0.2/src/wgdtree/__init__.py
--rw-r--r--   0 nick      (1000) nick      (1000)     1993 2021-12-16 22:13:09.000000 wgdtree-0.0.2/src/wgdtree/batch_run.py
--rw-r--r--   0 nick      (1000) nick      (1000)     4735 2021-11-20 18:29:10.000000 wgdtree-0.0.2/src/wgdtree/retention_rates.py
--rw-r--r--   0 nick      (1000) nick      (1000)     4265 2021-07-29 18:05:18.000000 wgdtree-0.0.2/src/wgdtree/rooting.py
--rw-r--r--   0 nick      (1000) nick      (1000)     4737 2021-09-21 20:03:34.000000 wgdtree-0.0.2/src/wgdtree/simulation.py
--rw-r--r--   0 nick      (1000) nick      (1000)      725 2021-07-13 19:05:58.000000 wgdtree-0.0.2/src/wgdtree/split.py
-drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2021-12-16 22:21:43.000000 wgdtree-0.0.2/src/wgdtree.egg-info/
--rw-r--r--   0 nick      (1000) nick      (1000)     3559 2021-12-16 22:21:43.000000 wgdtree-0.0.2/src/wgdtree.egg-info/PKG-INFO
--rw-r--r--   0 nick      (1000) nick      (1000)      332 2021-12-16 22:21:43.000000 wgdtree-0.0.2/src/wgdtree.egg-info/SOURCES.txt
--rw-r--r--   0 nick      (1000) nick      (1000)        1 2021-12-16 22:21:43.000000 wgdtree-0.0.2/src/wgdtree.egg-info/dependency_links.txt
--rw-r--r--   0 nick      (1000) nick      (1000)        8 2021-12-16 22:21:43.000000 wgdtree-0.0.2/src/wgdtree.egg-info/top_level.txt
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-02 16:35:18.608434 wgdtree-1.0/
+-rwxr-xr-x   0 nick      (1000) nick      (1000)     1074 2024-05-02 15:27:56.000000 wgdtree-1.0/LICENSE
+-rw-r--r--   0 nick      (1000) nick      (1000)     4309 2024-05-02 16:35:18.608434 wgdtree-1.0/PKG-INFO
+-rwxr-xr-x   0 nick      (1000) nick      (1000)     3781 2024-05-02 15:27:56.000000 wgdtree-1.0/README.md
+-rwxr-xr-x   0 nick      (1000) nick      (1000)      118 2024-05-02 15:27:56.000000 wgdtree-1.0/pyproject.toml
+-rwxr-xr-x   0 nick      (1000) nick      (1000)      653 2024-05-02 16:35:18.608434 wgdtree-1.0/setup.cfg
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-02 16:35:18.608434 wgdtree-1.0/src/
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-02 16:35:18.608434 wgdtree-1.0/src/wgdtree/
+-rwxr-xr-x   0 nick      (1000) nick      (1000)      230 2024-05-02 15:27:56.000000 wgdtree-1.0/src/wgdtree/__init__.py
+-rwxr-xr-x   0 nick      (1000) nick      (1000)     2109 2024-05-02 15:27:56.000000 wgdtree-1.0/src/wgdtree/batch_run.py
+-rwxr-xr-x   0 nick      (1000) nick      (1000)     4700 2024-05-02 15:27:56.000000 wgdtree-1.0/src/wgdtree/retention_rates.py
+-rwxr-xr-x   0 nick      (1000) nick      (1000)     4280 2024-05-02 15:27:56.000000 wgdtree-1.0/src/wgdtree/rooting.py
+-rwxr-xr-x   0 nick      (1000) nick      (1000)     4826 2024-05-02 15:27:56.000000 wgdtree-1.0/src/wgdtree/simulation.py
+-rwxr-xr-x   0 nick      (1000) nick      (1000)      706 2024-05-02 15:27:56.000000 wgdtree-1.0/src/wgdtree/split.py
+drwxr-xr-x   0 nick      (1000) nick      (1000)        0 2024-05-02 16:35:18.608434 wgdtree-1.0/src/wgdtree.egg-info/
+-rw-r--r--   0 nick      (1000) nick      (1000)     4309 2024-05-02 16:35:18.000000 wgdtree-1.0/src/wgdtree.egg-info/PKG-INFO
+-rwxr-xr-x   0 nick      (1000) nick      (1000)      332 2024-05-02 16:35:18.000000 wgdtree-1.0/src/wgdtree.egg-info/SOURCES.txt
+-rwxr-xr-x   0 nick      (1000) nick      (1000)        1 2024-05-02 16:35:18.000000 wgdtree-1.0/src/wgdtree.egg-info/dependency_links.txt
+-rwxr-xr-x   0 nick      (1000) nick      (1000)        8 2024-05-02 16:35:18.000000 wgdtree-1.0/src/wgdtree.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `wgdtree-0.0.2/LICENSE` & `wgdtree-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wgdtree-0.0.2/setup.cfg` & `wgdtree-1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = wgdtree
-version = 0.0.2
+version = 1.0
 author = Charles Henry
 author_email = Charlesnhenry@gmail.com
 description = A small package for simulating and analysing phylo-genetic trees.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/cnickh/wgdtree
 project_urls =
```

### Comparing `wgdtree-0.0.2/src/wgdtree/batch_run.py` & `wgdtree-1.0/src/wgdtree/batch_run.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,73 +1,82 @@
-from ete import Tree
+from ete3 import Tree
 from wgdtree.retention_rates import rrates, place_wgd
 
-
 def run(list_of_gene_trees, species_tree):
 
     results_dic = {}
+    paired_trees = []
+    pSpecies = []
 
     for l in species_tree.get_leaves():
-        resuls_dic[l] = []
-
+        results_dic[l.name] = []
 
     clean_tree = species_tree.copy()
-    
+
     for n in clean_tree.iter_descendants():
         if('WGD' in n.features):
-            n.remove_feature('WGD')
+            n.del_feature('WGD')
 
-    
-    paired_trees = []
-    
-    
+    i = 0
     for n in species_tree.traverse():
+
         if('WGD' in n.features and n.WGD == 'Y'):
-            
             for x in n.iter_descendants():
-                if('WGD' in n.features and n.WGD == 'Y'):
-                                        
+
+                if('WGD' in x.features and x.WGD == 'Y'):
+
                     tmp_tree = clean_tree.copy()
-                    
+
                     n1 = tmp_tree&n.name
-                    
+
                     n2 = tmp_tree&x.name
-                    
+
                     n1.add_feature('WGD', 'Y')
-                    
+
                     n2.add_feature('WGD', 'Y')
-                    
+
                     paired_trees.append(tmp_tree)
-                    
+
+                    i+=1
                     leaves = []
-                    
+
                     for l in x.get_leaves():
                         leaves.append(l.name.split('_')[0])
-                            
+
                     pSpecies.append(leaves)
 
-                    
     i=0
     for t in paired_trees:  #for each pair of events
         for s in pSpecies[i]: #for each species present for the pair
-                l_poss = 0
-                r_poss = 0
-                l = 0
-                r = 0
+            l_poss = 0
+            r_poss = 0
+            l = 0
+            r = 0
+            q = 0
+
             for g in list_of_gene_trees: #for each gene tree
-                tmp_gene = place_wgd(species_tree,g)
-                    
+                tmp_gene = g.copy()
+                place_wgd(t,tmp_gene)
+
                 results = rrates(tmp_gene,s)
 
-                l_poss += results
-                r_poss += results
-                l += results
-                r += results
-                
-            results_dic[s].append((l/l_poss,r/r_poss))
-            
-            
-            
+                q+=1
+                if(results != -1):
+                    l_poss += results[1][1]
+                    r_poss += results[0][1]
+                    l += results[1][0]
+                    r += results[0][0]
+
+            if(l_poss == 0 and r_poss == 0):
+                results_dic[s].append((0,0))
+            elif (l_poss == 0):
+                results_dic[s].append((0,r/r_poss))
+            elif (r_poss == 0):
+                results_dic[s].append((l/l_poss,0))
+            else:
+                results_dic[s].append((l/l_poss,r/r_poss))
+
+
+
         i+=1
-    
-    return resuls_dic
-    
+
+    return results_dic
```

### Comparing `wgdtree-0.0.2/src/wgdtree/retention_rates.py` & `wgdtree-1.0/src/wgdtree/retention_rates.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,35 +71,31 @@
                         place_wgd(children[0],gene_wgd,wgd_num+1)
                         place_wgd(children[1],gene_wgd,wgd_num+1)
                 
             elif len(leaves) > len(species):
                 place_wgd(species_root,gene_wgd.children[0],wgd_num)
                 place_wgd(species_root,gene_wgd.children[1],wgd_num)
                 
-                    
     else:
         if children:
             place_wgd(children[0],gene_wgd,wgd_num)
             place_wgd(children[1],gene_wgd,wgd_num)
     
-    
     return 0
 
-
 #count copies 
 def rrates(gene_tree,pSpecies):
     
     #initialize variables
     rcopies = 0
     lcopies = 0
     l_poss = 0
     r_poss = 0
     p = 0
     
-    
     for l in gene_tree.get_leaves():
         if pSpecies in l.name and "_LOST" not in l.name:
             p+=1
 
     if p!=0:
          
         for g in gene_tree.iter_descendants():
@@ -127,15 +123,12 @@
                 elif g.event0 == 'P':
                     rcopies += copies
                     r_poss += c_poss
 
     if r_poss == 0 and l_poss == 0:
         ret = -1
     elif rcopies == 0 and lcopies == 0 and p != 0:
-        ret = -2
+        ret = -1
     else:
         ret = ((rcopies,r_poss),(lcopies,l_poss),p)
     
     return ret
-
-
-
```

### Comparing `wgdtree-0.0.2/src/wgdtree/rooting.py` & `wgdtree-1.0/src/wgdtree/rooting.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,24 +153,24 @@
     
     print("Reconciliation failed! Maybe your tree isn't binary")
     exit()
 
     
 def root(gene_tree,species_tree):
         
-    dups = 999999
-
-    for root in gene_tree.get_children():
+    score = 999999
+    for root in gene_tree.iter_descendants():
+        
         tree = gene_tree.copy()
         tree.set_outgroup(tree&root.name)
         r_tree = reconcile(tree,species_tree)
-        temp = find_dups(r_tree) + find_loss(r_tree)
-        if(temp < dups):
+        temp = find_loss(r_tree) + find_dups(r_tree)
+        if(temp < score):
             best_root = root
-            dups = temp
+            score = temp
 
     gene_tree.set_outgroup(best_root)
     tree = reconcile(gene_tree,species_tree)
-    find_dups(tree)
     find_loss(tree)
+    find_dups(tree)
     return tree
```

### Comparing `wgdtree-0.0.2/src/wgdtree/simulation.py` & `wgdtree-1.0/src/wgdtree/simulation.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,18 @@
     if c > 1:
         rate_sum = loss_rate + ssd_rate
     else:
         rate_sum = ssd_rate
 
     #create specified wgd events
     if("WGD" in root.features and root.WGD == "Y"):
-        wgd_t = int(root.T)
+        if("T" in root.features):
+            wgd_t = int(root.T)
+        else:
+            wgd_t = int(root.dist)/2
     
     branch = root.dist
 
     while(branch > 0):
     
         #get time of next event
         nxt_event = expon.rvs()/(rate_sum*c)
```

### Comparing `wgdtree-0.0.2/src/wgdtree/split.py` & `wgdtree-1.0/src/wgdtree/split.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from ete3 import Tree
 
-
 def sortFunc(e):
     return e['len']
 
 #reduce tree size for processing 
 def break_up(tree,size=100):
     
     nw_trees =[]
@@ -18,15 +17,13 @@
                 poss_trees.append({'node': n, 'len': len(n.get_leaves())})
                 
         poss_trees.sort(key=sortFunc)
         _n = poss_trees.pop()['node']
         print("Removing: " + str(len(_n.get_leaves())) + " | Tree_total: " + str(len(tree.get_leaves())))
         nw_trees.append(_n.detach())
         
-        
-        
     nw_trees.append(tree)
     return nw_trees
```

