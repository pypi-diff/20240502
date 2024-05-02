# Comparing `tmp/hqm-0.0.8.tar.gz` & `tmp/hqm-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hqm-0.0.8.tar", last modified: Thu Sep 14 12:35:50 2023, max compression
+gzip compressed data, was "hqm-0.0.9.tar", last modified: Fri Sep 15 09:46:21 2023, max compression
```

## Comparing `hqm-0.0.8.tar` & `hqm-0.0.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)        0 2023-09-14 12:35:50.060055 hqm-0.0.8/
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     1072 2023-09-13 12:45:37.000000 hqm-0.0.8/LICENSE
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     5829 2023-09-14 12:35:50.059678 hqm-0.0.8/PKG-INFO
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     3774 2023-09-14 11:34:41.000000 hqm-0.0.8/README.md
-drwxr-xr-x   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)        0 2023-09-14 12:35:50.039886 hqm-0.0.8/hqm/
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)      160 2023-09-13 12:45:37.000000 hqm-0.0.8/hqm/__init__.py
-drwxr-xr-x   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)        0 2023-09-14 12:35:50.050565 hqm-0.0.8/hqm/circuits/
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)       97 2023-09-13 12:45:37.000000 hqm-0.0.8/hqm/circuits/__init__.py
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     8880 2023-09-13 12:45:37.000000 hqm-0.0.8/hqm/circuits/amplitudeencoding.py
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     8793 2023-09-13 12:45:37.000000 hqm-0.0.8/hqm/circuits/angleencoding.py
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     1492 2023-09-13 12:45:37.000000 hqm-0.0.8/hqm/circuits/circuit.py
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     8353 2023-09-13 12:45:37.000000 hqm-0.0.8/hqm/circuits/customcircuits.py
-drwxr-xr-x   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)        0 2023-09-14 12:35:50.051825 hqm-0.0.8/hqm/classification/
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)       84 2023-09-13 12:45:37.000000 hqm-0.0.8/hqm/classification/__init__.py
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     3522 2023-09-13 14:26:00.000000 hqm-0.0.8/hqm/classification/hcnn.py
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     7425 2023-09-13 12:45:37.000000 hqm-0.0.8/hqm/classification/hmlp.py
-drwxr-xr-x   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)        0 2023-09-14 12:35:50.052662 hqm-0.0.8/hqm/encoding/
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)       39 2023-09-13 12:45:37.000000 hqm-0.0.8/hqm/encoding/__init__.py
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)    10246 2023-09-14 11:22:21.000000 hqm-0.0.8/hqm/encoding/autoencoders.py
-drwxr-xr-x   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)        0 2023-09-14 12:35:50.056274 hqm-0.0.8/hqm/layers/
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)       37 2023-09-13 12:45:37.000000 hqm-0.0.8/hqm/layers/__init__.py
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     1417 2023-09-13 12:45:37.000000 hqm-0.0.8/hqm/layers/basiclayer.py
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     4080 2023-09-13 13:42:38.000000 hqm-0.0.8/hqm/layers/quanvolution.py
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     5613 2023-09-13 12:45:37.000000 hqm-0.0.8/hqm/layers/recurrent.py
-drwxr-xr-x   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)        0 2023-09-14 12:35:50.057187 hqm-0.0.8/hqm/regression/
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)       60 2023-09-13 12:45:37.000000 hqm-0.0.8/hqm/regression/__init__.py
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     7202 2023-09-13 12:45:37.000000 hqm-0.0.8/hqm/regression/hmlp.py
-drwxr-xr-x   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)        0 2023-09-14 12:35:50.059262 hqm-0.0.8/hqm/utils/
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)       86 2023-09-13 12:45:37.000000 hqm-0.0.8/hqm/utils/__init__.py
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     1659 2023-09-13 12:45:37.000000 hqm-0.0.8/hqm/utils/aiinterface.py
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)      960 2023-09-13 12:45:37.000000 hqm-0.0.8/hqm/utils/printer.py
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)      813 2023-09-14 11:19:16.000000 hqm-0.0.8/hqm/utils/sizes.py
-drwxr-xr-x   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)        0 2023-09-14 12:35:50.048298 hqm-0.0.8/hqm.egg-info/
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     5829 2023-09-14 12:35:49.000000 hqm-0.0.8/hqm.egg-info/PKG-INFO
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)      710 2023-09-14 12:35:49.000000 hqm-0.0.8/hqm.egg-info/SOURCES.txt
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)        1 2023-09-14 12:35:49.000000 hqm-0.0.8/hqm.egg-info/dependency_links.txt
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)       32 2023-09-14 12:35:49.000000 hqm-0.0.8/hqm.egg-info/requires.txt
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)        4 2023-09-14 12:35:49.000000 hqm-0.0.8/hqm.egg-info/top_level.txt
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)      863 2023-09-14 12:34:40.000000 hqm-0.0.8/pyproject.toml
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)       38 2023-09-14 12:35:50.060108 hqm-0.0.8/setup.cfg
--rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     2309 2023-09-14 12:34:53.000000 hqm-0.0.8/setup.py
+drwxr-xr-x   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)        0 2023-09-15 09:46:21.438799 hqm-0.0.9/
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     1072 2023-09-13 12:45:37.000000 hqm-0.0.9/LICENSE
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     5829 2023-09-15 09:46:21.438462 hqm-0.0.9/PKG-INFO
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     3774 2023-09-14 11:34:41.000000 hqm-0.0.9/README.md
+drwxr-xr-x   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)        0 2023-09-15 09:46:21.424270 hqm-0.0.9/hqm/
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)      184 2023-09-15 09:44:06.000000 hqm-0.0.9/hqm/__init__.py
+drwxr-xr-x   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)        0 2023-09-15 09:46:21.429851 hqm-0.0.9/hqm/circuits/
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)       97 2023-09-13 12:45:37.000000 hqm-0.0.9/hqm/circuits/__init__.py
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     8900 2023-09-15 07:31:47.000000 hqm-0.0.9/hqm/circuits/amplitudeencoding.py
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     8812 2023-09-15 07:32:02.000000 hqm-0.0.9/hqm/circuits/angleencoding.py
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     1501 2023-09-15 07:32:06.000000 hqm-0.0.9/hqm/circuits/circuit.py
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     8354 2023-09-15 07:31:22.000000 hqm-0.0.9/hqm/circuits/customcircuits.py
+drwxr-xr-x   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)        0 2023-09-15 09:46:21.431219 hqm-0.0.9/hqm/classification/
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)       84 2023-09-13 12:45:37.000000 hqm-0.0.9/hqm/classification/__init__.py
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     3583 2023-09-15 09:05:13.000000 hqm-0.0.9/hqm/classification/hcnn.py
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     7436 2023-09-15 07:32:22.000000 hqm-0.0.9/hqm/classification/hmlp.py
+drwxr-xr-x   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)        0 2023-09-15 09:46:21.432470 hqm-0.0.9/hqm/encoding/
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)       66 2023-09-15 09:41:38.000000 hqm-0.0.9/hqm/encoding/__init__.py
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)    10246 2023-09-14 11:22:21.000000 hqm-0.0.9/hqm/encoding/autoencoders.py
+drwxr-xr-x   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)        0 2023-09-15 09:46:21.435095 hqm-0.0.9/hqm/layers/
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)      115 2023-09-15 09:42:18.000000 hqm-0.0.9/hqm/layers/__init__.py
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     1416 2023-09-15 07:32:47.000000 hqm-0.0.9/hqm/layers/basiclayer.py
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     4080 2023-09-15 07:32:56.000000 hqm-0.0.9/hqm/layers/quanvolution.py
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     5622 2023-09-15 07:33:04.000000 hqm-0.0.9/hqm/layers/recurrent.py
+drwxr-xr-x   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)        0 2023-09-15 09:46:21.436201 hqm-0.0.9/hqm/regression/
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)       60 2023-09-13 12:45:37.000000 hqm-0.0.9/hqm/regression/__init__.py
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     7215 2023-09-15 07:33:21.000000 hqm-0.0.9/hqm/regression/hmlp.py
+drwxr-xr-x   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)        0 2023-09-15 09:46:21.438019 hqm-0.0.9/hqm/utils/
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)      106 2023-09-15 09:42:31.000000 hqm-0.0.9/hqm/utils/__init__.py
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     1659 2023-09-13 12:45:37.000000 hqm-0.0.9/hqm/utils/aiinterface.py
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)      969 2023-09-15 07:33:31.000000 hqm-0.0.9/hqm/utils/printer.py
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)      813 2023-09-14 11:19:16.000000 hqm-0.0.9/hqm/utils/sizes.py
+drwxr-xr-x   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)        0 2023-09-15 09:46:21.426967 hqm-0.0.9/hqm.egg-info/
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     5829 2023-09-15 09:46:21.000000 hqm-0.0.9/hqm.egg-info/PKG-INFO
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)      710 2023-09-15 09:46:21.000000 hqm-0.0.9/hqm.egg-info/SOURCES.txt
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)        1 2023-09-15 09:46:21.000000 hqm-0.0.9/hqm.egg-info/dependency_links.txt
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)       32 2023-09-15 09:46:21.000000 hqm-0.0.9/hqm.egg-info/requires.txt
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)        4 2023-09-15 09:46:21.000000 hqm-0.0.9/hqm.egg-info/top_level.txt
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)      863 2023-09-15 09:46:07.000000 hqm-0.0.9/pyproject.toml
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)       38 2023-09-15 09:46:21.438859 hqm-0.0.9/setup.cfg
+-rw-r--r--   0 asebastianelli (1445502215) ESAAD\Domain Users (1276952531)     2309 2023-09-15 09:45:50.000000 hqm-0.0.9/setup.py
```

### Comparing `hqm-0.0.8/LICENSE` & `hqm-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hqm-0.0.8/PKG-INFO` & `hqm-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hqm
-Version: 0.0.8
+Version: 0.0.9
 Summary: Hybrid Quantum Models - HQM
 Home-page: https://github.com/alessandrosebastianelli/hybrid_quantum_models.git
 Author: Alessandro Sebastianelli
 Author-email: Alessandro Sebastianelli <alessandro.sebastianelli1995@gmail.com>
 License: Copyright (c) 2023-2023 Alessandro Sebastianelli
         
         Permission is hereby granted, free of charge, to any person
```

### Comparing `hqm-0.0.8/README.md` & `hqm-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `hqm-0.0.8/hqm/circuits/amplitudeencoding.py` & `hqm-0.0.9/hqm/circuits/amplitudeencoding.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
                 PennyLane device on wich run quantum operations (dafault : None). When None it will be set
                 to 'default.qubit'  
             
             Returns:  
             --------  
             Nothing, a BasicEntangledCircuit object will be created.  
         '''
+
         super().__init__(n_qubits=n_qubits, n_layers=n_layers, dev=dev)
                
         self.weight_shape = {"weights": (n_layers, n_qubits)}
         self.circuit      = self.circ(self.dev, self.n_qubits)
         
 
     @staticmethod
@@ -51,14 +52,15 @@
                 number of qubits for the quantum circuit  
 
             Returns:  
             --------  
             - qnode : qml.qnode  
                 the actual PennyLane circuit   
         '''
+
         @qml.qnode(dev)
         def qnode(inputs : np.ndarray, weights : np.ndarray) -> list:
             '''
                 PennyLane based quantum circuit composed of an angle embedding layer and a basic entangler
                 layer.  
 
                 Parameters:  
@@ -70,14 +72,15 @@
                     array depends on circuit's layers and qubits.   
                 
                 Returns:  
                 --------  
                 - measurements : list  
                     list of values measured from the quantum circuits  
             '''
+
             qml.AmplitudeEmbedding(features=inputs, wires=range(n_qubits), normalize=True)
             qml.BasicEntanglerLayers(weights, wires=range(n_qubits))
             measurements = [qml.expval(qml.PauliZ(wires=i)) for i in range(n_qubits)]
             return measurements
     
         return qnode
     
@@ -100,15 +103,16 @@
             - dev : qml.device  
                 PennyLane device on wich run quantum operations (dafault : None). When None it will be set
                 to 'default.qubit'  
             
             Returns:  
             --------  
             Nothing, a StronglyEntangledCircuit object will be created.  
-        '''        
+        '''       
+
         super().__init__(n_qubits=n_qubits, n_layers=n_layers, dev=dev)
         
         self.weight_shape = {"weights": (n_layers, n_qubits, 3)}
         self.circuit      = self.circ(self.dev, self.n_qubits)
         
     @staticmethod
     def circ(dev : qml.devices, n_qubits : int) -> FunctionType:
@@ -124,14 +128,15 @@
                 number of qubits for the quantum circuit  
 
             Returns:  
             --------  
             - qnode : qml.qnode  
                 the actual PennyLane circuit  
         '''
+
         @qml.qnode(dev)
         def qnode(inputs : np.ndarray, weights : np.ndarray) -> list:
             '''
                 PennyLane based quantum circuit composed of an angle embedding layer and a strongly entangler
                 layer.  
 
                 Parameters:  
@@ -143,14 +148,15 @@
                     array depends on circuit's layers and qubits.   
                 
                 Returns:  
                 --------  
                 - measurements : list   
                     list of values measured from the quantum circuits  
             '''
+
             qml.AmplitudeEmbedding(features=inputs, wires=range(n_qubits), normalize=True)
             qml.StronglyEntanglingLayers(weights, wires=range(n_qubits))
             measurements = [qml.expval(qml.PauliZ(wires=i)) for i in range(n_qubits)]
             return measurements
     
         return qnode
 
@@ -174,14 +180,15 @@
                 PennyLane device on wich run quantum operations (dafault : None). When None it will be set
                 to 'default.qubit'  
             
             Returns:  
             --------  
             Nothing, a RandomCircuit object will be created.  
         '''
+
         super().__init__(n_qubits=n_qubits, n_layers=n_layers, dev=dev)
                
         self.weight_shape = {"weights": (n_layers, n_qubits)}
         self.circuit      = self.circ(self.dev, self.n_qubits)
 
     @staticmethod
     def circ(dev : qml.devices, n_qubits : int) -> FunctionType:
@@ -197,14 +204,15 @@
                 number of qubits for the quantum circuit  
 
             Returns:  
             --------  
             - qnode : qml.qnode  
                 the actual PennyLane circuit   
         '''
+
         @qml.qnode(dev)
         def qnode(inputs : np.ndarray, weights : np.ndarray) -> list:
             '''
                 PennyLane based quantum circuit composed of an angle embedding layer and a basic entangler
                 layer.  
 
                 Parameters:  
@@ -216,13 +224,14 @@
                     array depends on circuit's layers and qubits.   
                 
                 Returns:  
                 --------  
                 - measurements : list  
                     list of values measured from the quantum circuits  
             '''
+            
             qml.AmplitudeEmbedding(features=inputs, wires=range(n_qubits), normalize=True)
             qml.RandomLayers(weights, wires=range(n_qubits))
             measurements = [qml.expval(qml.PauliZ(wires=i)) for i in range(n_qubits)]
             return measurements
     
         return qnode
```

### Comparing `hqm-0.0.8/hqm/circuits/angleencoding.py` & `hqm-0.0.9/hqm/circuits/angleencoding.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
                 PennyLane device on wich run quantum operations (dafault : None). When None it will be set
                 to 'default.qubit'  
             
             Returns:  
             --------  
             Nothing, a BasicEntangledCircuit object will be created.  
         '''
+
         super().__init__(n_qubits=n_qubits, n_layers=n_layers, dev=dev)
                
         self.weight_shape = {"weights": (n_layers, n_qubits)}
         self.circuit      = self.circ(self.dev, self.n_qubits)
         
 
     @staticmethod
@@ -51,14 +52,15 @@
                 number of qubits for the quantum circuit  
 
             Returns:  
             --------  
             - qnode : qml.qnode  
                 the actual PennyLane circuit   
         '''
+
         @qml.qnode(dev)
         def qnode(inputs : np.ndarray, weights : np.ndarray) -> list:
             '''
                 PennyLane based quantum circuit composed of an angle embedding layer and a basic entangler
                 layer.  
 
                 Parameters:  
@@ -101,14 +103,15 @@
                 PennyLane device on wich run quantum operations (dafault : None). When None it will be set
                 to 'default.qubit'  
             
             Returns:  
             --------  
             Nothing, a StronglyEntangledCircuit object will be created.  
         '''        
+
         super().__init__(n_qubits=n_qubits, n_layers=n_layers, dev=dev)
         
         self.weight_shape = {"weights": (n_layers, n_qubits, 3)}
         self.circuit      = self.circ(self.dev, self.n_qubits)
         
     @staticmethod
     def circ(dev : qml.devices, n_qubits : int) -> FunctionType:
@@ -143,14 +146,15 @@
                     array depends on circuit's layers and qubits.   
                 
                 Returns:  
                 --------  
                 - measurements : list   
                     list of values measured from the quantum circuits  
             '''
+
             qml.AngleEmbedding(inputs, wires=range(n_qubits))
             qml.StronglyEntanglingLayers(weights, wires=range(n_qubits))
             measurements = [qml.expval(qml.PauliZ(wires=i)) for i in range(n_qubits)]
             return measurements
     
         return qnode
 
@@ -174,14 +178,15 @@
                 PennyLane device on wich run quantum operations (dafault : None). When None it will be set
                 to 'default.qubit'  
             
             Returns:  
             --------  
             Nothing, a RandomCircuit object will be created.  
         '''
+
         super().__init__(n_qubits=n_qubits, n_layers=n_layers, dev=dev)
                
         self.weight_shape = {"weights": (n_layers, n_qubits)}
         self.circuit      = self.circ(self.dev, self.n_qubits)
 
     @staticmethod
     def circ(dev : qml.devices, n_qubits : int) -> FunctionType:
@@ -197,14 +202,15 @@
                 number of qubits for the quantum circuit  
 
             Returns:  
             --------  
             - qnode : qml.qnode  
                 the actual PennyLane circuit   
         '''
+
         @qml.qnode(dev)
         def qnode(inputs : np.ndarray, weights : np.ndarray) -> list:
             '''
                 PennyLane based quantum circuit composed of an angle embedding layer and a basic entangler
                 layer.  
 
                 Parameters:  
@@ -216,13 +222,14 @@
                     array depends on circuit's layers and qubits.   
                 
                 Returns:  
                 --------  
                 - measurements : list  
                     list of values measured from the quantum circuits  
             '''
+            
             qml.AngleEmbedding(inputs, wires=range(n_qubits))
             qml.RandomLayers(weights, wires=range(n_qubits))
             measurements = [qml.expval(qml.PauliZ(wires=i)) for i in range(n_qubits)]
             return measurements
     
         return qnode
```

### Comparing `hqm-0.0.8/hqm/circuits/circuit.py` & `hqm-0.0.9/hqm/circuits/circuit.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,14 +21,15 @@
                 PennyLane device on wich run quantum operations (dafault : None). When None it will be set
                 to 'default.qubit'  
             
             Returns:  
             --------  
             Nothing, a QuantumCircuit object will be created.  
         '''
+        
         # Checking for exceptions  
         if n_qubits < 1: raise Exception(f"Number of qubits must be greater or equal than 1, found {n_qubits}")
         if n_layers < 1: raise Exception(f"Number of layers must be greater or equal than 1, found {n_layers}")
 
         # Set dev to 'default.qubit' if dev is None  
         if dev is None: 
             dev = qml.device("default.qubit", wires=n_qubits)
```

### Comparing `hqm-0.0.8/hqm/circuits/customcircuits.py` & `hqm-0.0.9/hqm/circuits/customcircuits.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
             - encoding : str  
                 string representing the type of input data encoding in quantum circuit, can be 'angle' or 'amplitude'
             
             Returns:  
             --------  
             Nothing, a BellmanCircuit object will be created.  
         '''
+        
         super().__init__(n_qubits=n_qubits, n_layers=n_layers, dev=dev)
 
         if encoding not in ['angle', 'amplitude']: raise(f"encoding can be angle or amplitude, found {encoding}")
         
         self.encoding     = encoding
         self.weight_shape = {"weights": (n_layers, n_qubits, 3)}
         self.circuit      = self.circ(self.dev, self.n_qubits, self.n_layers, self.encoding)
@@ -81,14 +82,15 @@
                     array depends on circuit's layers and qubits.   
                 
                 Returns:  
                 --------  
                 - measurements : list  
                     list of values measured from the quantum circuits  
             '''
+
             if encoding == 'angle':     qml.AngleEmbedding(inputs, wires=range(n_qubits))
             if encoding == 'amplitude': qml.AmplitudeEmbedding(features=inputs, wires=range(n_qubits), normalize=True)
 
             for n in range(n_layers):
                 qml.Hadamard(wires=0)
                 
                 # CNOT gates
@@ -179,15 +181,14 @@
                 
                 Returns:  
                 --------  
                 - measurements : list  
                     list of values measured from the quantum circuits  
             '''
 
-        
             if encoding == 'angle':     qml.AngleEmbedding(inputs, wires=range(n_qubits))
             if encoding == 'amplitude': qml.AmplitudeEmbedding(features=inputs, wires=range(n_qubits), normalize=True)
 
             for q in range(n_qubits): qml.Hadamard(wires=q)
 
             for n in range(n_layers):
                 for q1 in range(0, n_qubits):
```

### Comparing `hqm-0.0.8/hqm/classification/hcnn.py` & `hqm-0.0.9/hqm/classification/hcnn.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,28 +18,29 @@
             HybridLeNet5 constructor.  
 
             Parameters:  
             -----------  
             - qlayer : hqm.layers.basilayer.BasicLayer  
                 hqm quantum layer to be stacked between two fully connected layers  
             - in_shape : tuple  
-                tuple representing the shape of the input image  
+                tuple representing the shape of the input image (channels, widht, height)  
             - ou_dim : int  
                 integer representing the output size of the hybrid model  
             
             Returns:  
             --------  
             Nothing, a HybridLeNet5 object will be created.    
         '''
+
         super().__init__()
 
-        if len(in_shape) != 3: raise Exception(f"The parameter in_shape must be a tuple of three elements, found {in_shape}")
+        if len(in_shape) != 3: raise Exception(f"The parameter in_shape must be a tuple of four elements (channels, widht, height), found {in_shape}")
         if ou_dim < 1: raise Exception(f"The parameter ou_dim must be greater than 1, found {ou_dim}")
         
-        w, h, c = in_shape
+        c, w, h = in_shape
         
         c1 = 6
         self.conv_1    = torch.nn.Conv2d(in_channels=c, out_channels=c1, kernel_size=5, padding=2, stride=1)
         w1 = size_conv_layer(w, kernel_size=5, padding=2, stride=1)
         h1 = size_conv_layer(h, kernel_size=5, padding=2, stride=1)
         
         self.max_pool1 = torch.nn.MaxPool2d(kernel_size = (2,2), stride=(2,2))
@@ -75,14 +76,15 @@
                 input for the torch model  
 
             Returns:  
             --------  
             - out : torch.Tensor  
                 output from the torch model  
         '''
+        
         x = self.max_pool1(self.relu(self.conv_1(x)))
         x = self.max_pool2(self.relu(self.conv_2(x)))
         x = x.view(-1, self.flatten_size)
         x = self.relu(self.fc_1(x))
         x = self.relu(self.fc_2(x))
         x = self.relu(self.qc_1(x))
         x = self.fc_3(x)
```

### Comparing `hqm-0.0.8/hqm/classification/hmlp.py` & `hqm-0.0.9/hqm/classification/hmlp.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,14 +82,15 @@
             - ou_dim : int  
                 integer representing the output size of the hybrid model  
             
             Returns:  
             --------  
             Nothing, a MultiHybridMLPClassifier object will be created.    
         '''
+
         super().__init__()
 
         if in_dim < 1: raise Exception(f"The parameter in_dim must be greater than 1, found {in_dim}")
         if ou_dim < 1: raise Exception(f"The parameter ou_dim must be greater than 1, found {ou_dim}")
         if len(qlayers) < 1: raise Exception(f"Size of qlayers must be greater than 1, found {len(qlayers)}")
 
         n_qubits_0   = qlayers[0].n_qubits
@@ -110,14 +111,15 @@
                 input for the torch model  
 
             Returns:  
             --------  
             - out : torch.Tensor   
                 output from the torch model  
         '''
+
         x = self.fc_1(x)
         x = self.tanh(x)
         for qc in self.qcs: 
             x = qc(x)
             x = self.tanh(x)
         x = self.fc_2(x)
         out = self.softmax(x)
@@ -143,14 +145,15 @@
             - ou_dim : list  
                 list of integers representing the output size for the i-th fully connected layer (last value should correspond to desired output size)  
             
             Returns:  
             --------  
             Nothing, a MultiHybridMultiMLPClassifier object will be created.    
         '''
+        
         super().__init__()
 
         if len(in_dims) < 1: raise Exception(f"Size in_dims must be greater than 1, found {len(in_dims)}")
         if ou_dim < 1: raise Exception(f"The parameter ou_dim must be greater than 1, found {ou_dim}")
         if len(qlayers) < 1: raise Exception(f"Size of qlayerss must be greater than 1, found {len(qlayers)}")
         if len(qlayers) != len(in_dims): raise Exception(f"qlayers and in_dims must have the same lenght, found {len(qlayers)} and {len(in_dims)}")
         for i, dim in enumerate(in_dims):
```

### Comparing `hqm-0.0.8/hqm/encoding/autoencoders.py` & `hqm-0.0.9/hqm/encoding/autoencoders.py`

 * *Files identical despite different names*

### Comparing `hqm-0.0.8/hqm/layers/basiclayer.py` & `hqm-0.0.9/hqm/layers/basiclayer.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 class BasicLayer:
     '''
         Basic Quantum Layer
     '''
 
     def __init__(self, qcircuit : QuantumCircuit, aiframework : str) -> None:
         '''
-
         BasicLayer constructor.  
 
         Parameters:  
         -----------  
         - qcircuit : hqm.circuits.circuit.QuantumCircuit  
             QuantumCircuit object to be embedded into the quantum layer
         - aiframework : str
```

### Comparing `hqm-0.0.8/hqm/layers/quanvolution.py` & `hqm-0.0.9/hqm/layers/quanvolution.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
             string representing the AI framework in use, can be 'torch' or 'keras'. This will create  
             a compatible trainable layer for the framework.
 
         Returns:    
         --------     
         Nothing, a Quanvolution2D object will be created.  
         '''
+
         super().__init__()
 
         if aiframework not in ['torch', 'keras']: raise Exception(f"Quanvolution2D curently supports only 'torch' as framework, found {aiframework}")
         if kernelsize < 1:                        raise Exception(f"kernelsize must be greater than 1, found {kernelsize}")
         if stride < 1:                            raise Exception(f"stride must be greater than 1, found {stride}")
         
         self.aiframework = aiframework
@@ -70,15 +71,14 @@
         
         Returns:
         --------
         - out : torch.Tensor
             quanvoluted input
         '''
 
-
         if len(x.shape) != 4: raise Exception(f"x must be a tensor of 4 elements (batch, channels, width, height), found {len(x.shape)}")
 
         # Calculates the image shape after the convolution
         bs, ch, h, w = x.shape
         
         h_out = int(((h-self.kernelsize) / self.stride) +1)
         w_out = int(((w-self.kernelsize) / self.stride) +1)
```

### Comparing `hqm-0.0.8/hqm/layers/recurrent.py` & `hqm-0.0.9/hqm/layers/recurrent.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,14 +37,15 @@
             string representing the AI framework in use, can be 'torch' or 'keras'. This will create  
             a compatible trainable layer for the framework.
 
         Returns:    
         --------     
         Nothing, a QGRU object will be created.  
         '''
+        
         super().__init__()
 
         if aiframework not in ['torch', 'keras']: raise Exception(f"Quanvolution2D curently supports only 'torch' as framework, found {aiframework}")
         if inputsize       < 1:                   raise Exception(f"inputsize must be greater than 1, found {inputsize}")
         if hiddensize      < 1:                   raise Exception(f"hiddensize must be greater than 1, found {hiddensize}")
         if len(qcircuits) != 3:                   raise Exception(f"qcircuits must contain 3 elements, one for reset gate, one for update gate and one for output gate, found {len(qcircuits)}")
```

### Comparing `hqm-0.0.8/hqm/regression/hmlp.py` & `hqm-0.0.9/hqm/regression/hmlp.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,15 @@
             - ou_dim : int  
                 integer representing the output size of the hybrid model  
             
             Returns:  
             --------  
             Nothing, a BasicHybridMLPRegressor object will be created.    
         '''
+
         super().__init__()
 
         if in_dim < 1: raise Exception(f"The parameter in_dim must be greater than 1, found {in_dim}")
         if ou_dim < 1: raise Exception(f"The parameter ou_dim must be greater than 1, found {ou_dim}")
 
         n_qubits  = qlayer.n_qubits
         self.fc_1 = torch.nn.Linear(in_dim, n_qubits)
@@ -50,14 +51,15 @@
                 input for the torch model  
 
             Returns:  
             --------  
             - out : torch.Tensor  
                 output from the torch model  
         '''
+
         x = self.fc_1(x)
         x = self.tanh(x)
         x = self.qc_1(x)
         x = self.tanh(x)
         x = self.fc_2(x)
         out = self.tanh(x)
         return out
@@ -82,14 +84,15 @@
             - ou_dim : int  
                 integer representing the output size of the hybrid model  
             
             Returns:  
             --------  
             Nothing, a MultiHybridMLPRegressor object will be created.    
         '''
+
         super().__init__()
 
         if in_dim < 1: raise Exception(f"The parameter in_dim must be greater than 1, found {in_dim}")
         if ou_dim < 1: raise Exception(f"The parameter ou_dim must be greater than 1, found {ou_dim}")
         if len(qlayers) < 1: raise Exception(f"Size of qlayers must be greater than 1, found {len(qlayers)}")
 
         n_qubits_0 = qlayers[0].n_qubits
@@ -109,14 +112,15 @@
                 input for the torch model  
 
             Returns:  
             --------  
             - out : torch.Tensor  
                 output from the torch model  
         '''
+
         x = self.fc_1(x)
         x = self.tanh(x)
         for qc in self.qcs: 
             x = qc(x)
             x = self.tanh(x)
         x = self.fc_2(x)
         out = self.tanh(x)
@@ -142,14 +146,15 @@
             - ou_dim : list  
                 list of integers representing the output size for the i-th fully connected layer (last value should correspond to desired output size)  
             
             Returns:  
             --------  
             Nothing, a MultiHybridMLPRegressor object will be created.    
         '''
+        
         super().__init__()
 
         if len(in_dims) < 1: raise Exception(f"Size in_dims must be greater than 1, found {len(in_dims)}")
         if ou_dim < 1: raise Exception(f"The parameter ou_dim must be greater than 1, found {ou_dim}")
         if len(qlayers) < 1: raise Exception(f"Size of qlayers must be greater than 1, found {len(qlayers)}")
         if len(qlayers) != len(in_dims): raise Exception(f"qlayers and in_dims must have the same lenght, found {len(qlayers)} and {len(in_dims)}")
         for i, dim in enumerate(in_dims):
```

### Comparing `hqm-0.0.8/hqm/utils/aiinterface.py` & `hqm-0.0.9/hqm/utils/aiinterface.py`

 * *Files identical despite different names*

### Comparing `hqm-0.0.8/hqm/utils/printer.py` & `hqm-0.0.9/hqm/utils/printer.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,12 +23,13 @@
             
             Return:  
             -------  
             - str_circ : str  
                 string containing circuit structure  
 
         '''
+        
         weights  = np.random.random(size=circuit.weight_shape['weights'])
         inputs   = np.random.random(size=(circuit.n_qubits))
         str_circ = qml.draw(circuit.circuit, expansion_strategy="device")(inputs, weights)
         print(str_circ)
         return str_circ
```

### Comparing `hqm-0.0.8/hqm/utils/sizes.py` & `hqm-0.0.9/hqm/utils/sizes.py`

 * *Files identical despite different names*

### Comparing `hqm-0.0.8/hqm.egg-info/PKG-INFO` & `hqm-0.0.9/hqm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hqm
-Version: 0.0.8
+Version: 0.0.9
 Summary: Hybrid Quantum Models - HQM
 Home-page: https://github.com/alessandrosebastianelli/hybrid_quantum_models.git
 Author: Alessandro Sebastianelli
 Author-email: Alessandro Sebastianelli <alessandro.sebastianelli1995@gmail.com>
 License: Copyright (c) 2023-2023 Alessandro Sebastianelli
         
         Permission is hereby granted, free of charge, to any person
```

### Comparing `hqm-0.0.8/hqm.egg-info/SOURCES.txt` & `hqm-0.0.9/hqm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hqm-0.0.8/pyproject.toml` & `hqm-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
             "numpy==1.23.5", 
             "pennylane==0.28.0"
             ]
 
 [project]
 name = "hqm"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Alessandro Sebastianelli", email="alessandro.sebastianelli1995@gmail.com" },
 ]
 description = "Hybrid Quantum Models - HQM"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.9.17"
```

### Comparing `hqm-0.0.8/setup.py` & `hqm-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
             return file.read()
     except IOError:
         return ""
 
 # Package 
 HERE = pathlib.Path(__file__).parent
 PACKAGE_NAME  = 'hqm'
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 AUTHOR = 'Alessandro Sebastianelli'
 AUTHOR_EMAIL = 'alessandro.sebastianelli1995@gmail.com'
 URL = 'https://github.com/alessandrosebastianelli/hybrid_quantum_models.git'
 
 LICENSE = 'MIT'
 DESCRIPTION = 'Hybrid Quantum Models - HQM'
 LONG_DESCRIPTION = readme()
```

