# Comparing `tmp/w2rpy-0.1.2.tar.gz` & `tmp/w2rpy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "w2rpy-0.1.2.tar", last modified: Thu May  2 14:44:21 2024, max compression
+gzip compressed data, was "w2rpy-0.1.3.tar", last modified: Thu May  2 14:51:00 2024, max compression
```

## Comparing `w2rpy-0.1.2.tar` & `w2rpy-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 14:44:21.554791 w2rpy-0.1.2/
--rw-rw-rw-   0        0        0     1062 2024-05-01 20:18:19.000000 w2rpy-0.1.2/LICENSE
--rw-rw-rw-   0        0        0      416 2024-05-02 14:44:21.554791 w2rpy-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0        7 2024-05-01 21:03:28.000000 w2rpy-0.1.2/README.md
--rw-rw-rw-   0        0        0       86 2024-05-02 14:44:21.555512 w2rpy-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      702 2024-05-02 14:44:16.000000 w2rpy-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-02 14:44:21.550463 w2rpy-0.1.2/w2rpy/
--rw-rw-rw-   0        0        0      114 2024-05-01 21:04:56.000000 w2rpy-0.1.2/w2rpy/__init__.py
--rw-rw-rw-   0        0        0    26091 2024-05-02 02:33:12.000000 w2rpy-0.1.2/w2rpy/w2rpy.py
-drwxrwxrwx   0        0        0        0 2024-05-02 14:44:21.554069 w2rpy-0.1.2/w2rpy.egg-info/
--rw-rw-rw-   0        0        0      416 2024-05-02 14:44:21.000000 w2rpy-0.1.2/w2rpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2024-05-02 14:44:21.000000 w2rpy-0.1.2/w2rpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 14:44:21.000000 w2rpy-0.1.2/w2rpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       54 2024-05-02 14:44:21.000000 w2rpy-0.1.2/w2rpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-02 14:44:21.000000 w2rpy-0.1.2/w2rpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-02 14:51:00.294977 w2rpy-0.1.3/
+-rw-rw-rw-   0        0        0     1062 2024-05-01 20:18:19.000000 w2rpy-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0      416 2024-05-02 14:51:00.294977 w2rpy-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2024-05-01 21:03:28.000000 w2rpy-0.1.3/README.md
+-rw-rw-rw-   0        0        0       86 2024-05-02 14:51:00.295977 w2rpy-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      702 2024-05-02 14:50:47.000000 w2rpy-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 14:51:00.288977 w2rpy-0.1.3/w2rpy/
+-rw-rw-rw-   0        0        0      114 2024-05-01 21:04:56.000000 w2rpy-0.1.3/w2rpy/__init__.py
+-rw-rw-rw-   0        0        0    26140 2024-05-02 14:47:58.000000 w2rpy-0.1.3/w2rpy/w2rpy.py
+drwxrwxrwx   0        0        0        0 2024-05-02 14:51:00.294977 w2rpy-0.1.3/w2rpy.egg-info/
+-rw-rw-rw-   0        0        0      416 2024-05-02 14:51:00.000000 w2rpy-0.1.3/w2rpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2024-05-02 14:51:00.000000 w2rpy-0.1.3/w2rpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 14:51:00.000000 w2rpy-0.1.3/w2rpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2024-05-02 14:51:00.000000 w2rpy-0.1.3/w2rpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-05-02 14:51:00.000000 w2rpy-0.1.3/w2rpy.egg-info/top_level.txt
```

### Comparing `w2rpy-0.1.2/LICENSE` & `w2rpy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `w2rpy-0.1.2/setup.py` & `w2rpy-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 from distutils.core import setup
 
 setup(
   name = 'w2rpy',         
   packages = ['w2rpy'],   
-  version = '0.1.2',     
+  version = '0.1.3',     
   license='MIT',        
   description = 'Water Resource Functions For Fluvial Systems',   
   author = 'Luke Russell',                   
   author_email = 'lrussell@wolfwaterresources.com',      
   keywords = ['SOME', 'MEANINGFULL', 'KEYWORDS'],   
   install_requires=['pandas',
                     'numpy',
```

### Comparing `w2rpy-0.1.2/w2rpy/w2rpy.py` & `w2rpy-0.1.3/w2rpy/w2rpy.py`

 * *Files 2% similar despite different names*

```diff
@@ -686,18 +686,19 @@
         chan_ind = np.array([np.argmin(abs(station-bound)) for bound in breaks])
         chan_ind = np.delete(chan_ind,elevation[chan_ind]>wse)
         indices = np.sort(np.unique(np.concatenate([indices,chan_ind]).flatten()))
         
         sta = np.split(station, indices)
         sta = [s for s in sta if (elevation[np.searchsorted(station,s)]<wse).any()]
         sta = [np.append(s,station[np.argwhere(station==max(s))+1]) for s in sta]
+        end_sta = [np.argwhere(station==s[-1]) for s in sta]
         
         elev = np.split(elevation, indices)
         elev = [e for e in elev if (e<wse).any()]
-        elev = [np.append(e,max(elevation[np.argwhere(elevation==e[-1])+1])) for e in elev]
+        elev = [np.append(e,elevation[end_sta[i]]) for i,e in enumerate(elev)]
         
         channels = [np.array([sta[i],elev[i]]).astype(float) for i in range(len(sta))]
         channels = [chan for chan in channels if chan.size>0]
         
         aas = []
         ps = []
         rs = []
```

