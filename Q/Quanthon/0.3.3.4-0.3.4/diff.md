# Comparing `tmp/Quanthon-0.3.3.4.tar.gz` & `tmp/Quanthon-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Quanthon-0.3.3.4.tar", last modified: Tue Mar  5 16:41:30 2024, max compression
+gzip compressed data, was "Quanthon-0.3.4.tar", last modified: Wed Apr  3 12:44:56 2024, max compression
```

## Comparing `Quanthon-0.3.3.4.tar` & `Quanthon-0.3.4.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-03-05 16:41:30.372958 Quanthon-0.3.3.4/
--rw-r--r--   0 bukser     (501) staff       (20)        0 2023-09-14 17:15:45.000000 Quanthon-0.3.3.4/LICENSE
--rw-r--r--   0 bukser     (501) staff       (20)     2495 2024-03-05 16:41:30.372729 Quanthon-0.3.3.4/PKG-INFO
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-03-05 16:41:30.371193 Quanthon-0.3.3.4/Quanthon/
--rw-r--r--   0 bukser     (501) staff       (20)     2523 2024-03-04 14:02:06.000000 Quanthon-0.3.3.4/Quanthon/Ansatz.py
--rw-r--r--   0 bukser     (501) staff       (20)     7000 2024-03-05 16:30:39.000000 Quanthon-0.3.3.4/Quanthon/Expectation.py
--rw-r--r--   0 bukser     (501) staff       (20)     9311 2024-03-04 13:58:26.000000 Quanthon-0.3.3.4/Quanthon/Mapper.py
--rw-r--r--   0 bukser     (501) staff       (20)     3709 2024-03-04 09:48:46.000000 Quanthon-0.3.3.4/Quanthon/Models.py
--rw-r--r--   0 bukser     (501) staff       (20)      213 2024-03-04 18:24:15.000000 Quanthon-0.3.3.4/Quanthon/__init__.py
--rw-r--r--   0 bukser     (501) staff       (20)     3208 2024-03-04 14:02:03.000000 Quanthon-0.3.3.4/Quanthon/algorithms.py
--rw-r--r--   0 bukser     (501) staff       (20)     3586 2024-03-04 13:59:56.000000 Quanthon-0.3.3.4/Quanthon/algorithms_new.py
--rw-r--r--   0 bukser     (501) staff       (20)    11847 2024-02-15 14:43:17.000000 Quanthon-0.3.3.4/Quanthon/base.py
--rw-r--r--   0 bukser     (501) staff       (20)    11751 2024-03-05 10:38:50.000000 Quanthon-0.3.3.4/Quanthon/new_base.py
--rw-r--r--   0 bukser     (501) staff       (20)        0 2023-09-14 16:48:42.000000 Quanthon-0.3.3.4/Quanthon/operators.py
--rw-r--r--   0 bukser     (501) staff       (20)        0 2024-02-19 13:39:55.000000 Quanthon-0.3.3.4/Quanthon/test_new_base.py
--rw-r--r--   0 bukser     (501) staff       (20)     4804 2024-03-05 10:40:50.000000 Quanthon-0.3.3.4/Quanthon/utils.py
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-03-05 16:41:30.372484 Quanthon-0.3.3.4/Quanthon.egg-info/
--rw-r--r--   0 bukser     (501) staff       (20)     2495 2024-03-05 16:41:30.000000 Quanthon-0.3.3.4/Quanthon.egg-info/PKG-INFO
--rw-r--r--   0 bukser     (501) staff       (20)      441 2024-03-05 16:41:30.000000 Quanthon-0.3.3.4/Quanthon.egg-info/SOURCES.txt
--rw-r--r--   0 bukser     (501) staff       (20)        1 2024-03-05 16:41:30.000000 Quanthon-0.3.3.4/Quanthon.egg-info/dependency_links.txt
--rw-r--r--   0 bukser     (501) staff       (20)        6 2024-03-05 16:41:30.000000 Quanthon-0.3.3.4/Quanthon.egg-info/requires.txt
--rw-r--r--   0 bukser     (501) staff       (20)        9 2024-03-05 16:41:30.000000 Quanthon-0.3.3.4/Quanthon.egg-info/top_level.txt
--rw-r--r--   0 bukser     (501) staff       (20)     1681 2024-03-04 14:05:24.000000 Quanthon-0.3.3.4/README.md
--rw-r--r--   0 bukser     (501) staff       (20)       38 2024-03-05 16:41:30.373005 Quanthon-0.3.3.4/setup.cfg
--rw-r--r--   0 bukser     (501) staff       (20)     1461 2024-03-05 16:41:06.000000 Quanthon-0.3.3.4/setup.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-03 12:44:56.137905 Quanthon-0.3.4/
+-rw-r--r--   0 bukser     (501) staff       (20)        0 2023-09-14 17:15:45.000000 Quanthon-0.3.4/LICENSE
+-rw-r--r--   0 bukser     (501) staff       (20)     2544 2024-04-03 12:44:56.137620 Quanthon-0.3.4/PKG-INFO
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-03 12:44:56.134547 Quanthon-0.3.4/Quanthon/
+-rw-r--r--   0 bukser     (501) staff       (20)     3709 2024-03-04 09:48:46.000000 Quanthon-0.3.4/Quanthon/Models.py
+-rw-r--r--   0 bukser     (501) staff       (20)      327 2024-03-19 15:53:35.000000 Quanthon-0.3.4/Quanthon/__init__.py
+-rw-r--r--   0 bukser     (501) staff       (20)     3181 2024-03-19 14:55:03.000000 Quanthon-0.3.4/Quanthon/algorithms.py
+-rw-r--r--   0 bukser     (501) staff       (20)     6268 2024-04-03 12:38:02.000000 Quanthon-0.3.4/Quanthon/algorithms_new.py
+-rw-r--r--   0 bukser     (501) staff       (20)     4391 2024-04-02 14:29:33.000000 Quanthon-0.3.4/Quanthon/ansatzs.py
+-rw-r--r--   0 bukser     (501) staff       (20)    11984 2024-03-21 12:14:41.000000 Quanthon-0.3.4/Quanthon/base.py
+-rw-r--r--   0 bukser     (501) staff       (20)     5970 2024-03-21 11:59:47.000000 Quanthon-0.3.4/Quanthon/expectation.py
+-rw-r--r--   0 bukser     (501) staff       (20)     9854 2024-03-19 15:01:41.000000 Quanthon-0.3.4/Quanthon/mappers.py
+-rw-r--r--   0 bukser     (501) staff       (20)    12329 2024-04-02 13:21:56.000000 Quanthon-0.3.4/Quanthon/new_base.py
+-rw-r--r--   0 bukser     (501) staff       (20)      452 2024-03-21 16:13:36.000000 Quanthon-0.3.4/Quanthon/physics.py
+-rw-r--r--   0 bukser     (501) staff       (20)     2302 2024-03-13 12:44:21.000000 Quanthon-0.3.4/Quanthon/ut_pyscf_mel.py
+-rw-r--r--   0 bukser     (501) staff       (20)     1714 2024-03-18 22:32:17.000000 Quanthon-0.3.4/Quanthon/ut_qiskit_hamiltonian.py
+-rw-r--r--   0 bukser     (501) staff       (20)     5299 2024-03-21 16:15:37.000000 Quanthon-0.3.4/Quanthon/ut_test_jw.py
+-rw-r--r--   0 bukser     (501) staff       (20)     4804 2024-04-02 12:23:12.000000 Quanthon-0.3.4/Quanthon/utils.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-03 12:44:56.137307 Quanthon-0.3.4/Quanthon.egg-info/
+-rw-r--r--   0 bukser     (501) staff       (20)     2544 2024-04-03 12:44:56.000000 Quanthon-0.3.4/Quanthon.egg-info/PKG-INFO
+-rw-r--r--   0 bukser     (501) staff       (20)      541 2024-04-03 12:44:56.000000 Quanthon-0.3.4/Quanthon.egg-info/SOURCES.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        1 2024-04-03 12:44:56.000000 Quanthon-0.3.4/Quanthon.egg-info/dependency_links.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        6 2024-04-03 12:44:56.000000 Quanthon-0.3.4/Quanthon.egg-info/requires.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        9 2024-04-03 12:44:56.000000 Quanthon-0.3.4/Quanthon.egg-info/top_level.txt
+-rw-r--r--   0 bukser     (501) staff       (20)     1681 2024-03-04 14:05:24.000000 Quanthon-0.3.4/README.md
+-rw-r--r--   0 bukser     (501) staff       (20)       38 2024-04-03 12:44:56.137951 Quanthon-0.3.4/setup.cfg
+-rw-r--r--   0 bukser     (501) staff       (20)     1509 2024-04-03 12:41:08.000000 Quanthon-0.3.4/setup.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-03 12:44:56.136341 Quanthon-0.3.4/tests/
+-rw-r--r--   0 bukser     (501) staff       (20)     6073 2024-04-03 12:26:28.000000 Quanthon-0.3.4/tests/test_adapt.py
```

### Comparing `Quanthon-0.3.3.4/PKG-INFO` & `Quanthon-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quanthon
-Version: 0.3.3.4
+Version: 0.3.4
 Summary: A quantum computing library
 Home-page: https://quanthon.readthedocs.io/
 Author: Keran Chen
 Author-email: keranc@uio.no
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 
 # Quanthon
```

### Comparing `Quanthon-0.3.3.4/Quanthon/Models.py` & `Quanthon-0.3.4/Quanthon/Models.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.3.4/Quanthon/algorithms.py` & `Quanthon-0.3.4/Quanthon/algorithms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 '''Doc:
     VQEs
 '''
 
 from scipy.optimize import minimize
 import numpy as np
 import warnings
-from .Ansatz import Ansatz
 
 class VQE():
         def __init__(self, ansatz, init_points, expectation=None, optimiser=None):
             '''ansatz: a parametriced circuit that takes parmas: theta and phi
                 init_points: a list of initial points, must match the number of the parameters in the ansatz
                 expectation: the function that calculates the expectation value of the ansatz'''
             self.ansatz = ansatz
```

### Comparing `Quanthon-0.3.3.4/Quanthon/base.py` & `Quanthon-0.3.4/Quanthon/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import numpy as np
 from collections import Counter
 
 # Constants
 rng = np.random.default_rng()
 rangle = '\u27E9'
 
+PendingDeprecationWarning("This module is deprecated and will be removed in the next release. Please use the new_base module instead.")
+
 class Gate:
 
     def __init__(self, name, matrix, n_qubits, params=None):
         self.name = name
         self.matrix = matrix
         self.n_qubits = n_qubits
         self.params = params
```

### Comparing `Quanthon-0.3.3.4/Quanthon/new_base.py` & `Quanthon-0.3.4/Quanthon/new_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,44 +1,48 @@
+'''The basic classes for quantum computing. Replaced base.py, which was discontinued after Quanthon 0.3.0'''
+
+# TODO: Add n dimension rotation 
+
 import numpy as np
 from collections import Counter
 from .utils import one_fixed_bit, flip_bit, swap_bits
 
 # Constants
 rng = np.random.default_rng()
 rangle = '\u27E9'
 
 class Gate:
 
-    def __init__(self, name, matrix, n_qubits, params=None):
+    def __init__(self, name, matrix, n_qubits):
         '''
         args:
             name: string, the name of the gate;
             matrix: operator matrix or a function which takes params is an argument and returns the matrix of the correct size;
             n_qubits: int, the number of qubits the gate acts on;
-            params: a parameter of the gate, if any.
             '''
         self.name = name
         self.matrix = matrix
 
         self.n_qubits = n_qubits
-        self.params = params
-
-        if params:
-            try:
-                self.matrix(params)
-            except:
-                raise ValueError(f"Invalid matrix function or parameters.")
+        # self.params = params
 
 
     def __repr__(self):
         return f"Gate: {self.name} \n Matrix: \n {self.matrix} \n"
     
-    def act(self, state):
-        if self.params is not None:
-            return self.matrix(self.params) @ state
+    def _check_is_unitary(self, matrix):
+
+        if not np.allclose(matrix @ matrix.conj().T, np.eye(matrix.shape[0])):
+            raise ValueError(f"{self.name} is not unitary.")
+    
+    def act(self, state, param=None):
+        if param is not None:
+            self._check_is_unitary(self.matrix(param))
+            return self.matrix(param) @ state
+        self._check_is_unitary(self.matrix)
         return self.matrix @ state
 
     
 class Qubits:
 
     def __init__(self,n):
         self.state = np.zeros(2**n, dtype=np.complex_)
@@ -94,20 +98,23 @@
             else:
                 if j != i:
                     self.gate_history[f'{j}'].append('I')
 
 
     def set_state(self, state):
         assert len(state) == 2**self.n_qubit, f"Invalid state: must have length {2**self.n_qubit}"
-        assert np.linalg.norm(state) == 1, "Invalid state: must be normalised"
+        assert np.isclose(np.linalg.norm(state), 1), "Invalid state: must be normalised."
         self.state = state
 
-    def reinit_state(self):
+    def reset_state(self):
         self.state = np.zeros(2**self.n_qubit, dtype=np.complex_)
         self.state[0] = 1
+    
+    def reset_circuit(self):
+        self.circuit = []
 
     def copy(self):
         new_qubits = Qubits(self.n_qubit)
         new_qubits.state = self.state.copy()
         return new_qubits
 
 
@@ -168,38 +175,40 @@
 
     def Z(self,i):
         # self.operate(self.z, i)
         matrix = self._make_op_mat(self.z, i)
         self.circuit.append(Gate('Z', matrix, self.n_qubit))
         self._update_gate_history('Z', i)
     
-    def sdag(self,i):
+    def Sdag(self,i):
         # self.operate(self.s.conj(), i)
         matrix = self._make_op_mat(self.s.conj(), i)
         self.circuit.append(Gate('Sdag', matrix, self.n_qubit))
         self._update_gate_history('Sdag', i)
     
     # def param_rx(self, theta, i):
     #     matrix = lambda theta: np.cos(theta/2) * self.I - 1j * np.sin(theta/2) * self.x
     #     self.circuit.append(Gate('Rx', matrix, self.n_qubit, theta))
     #     self._update_gate_history(r'Rx_\theta', i)
 
     # def param_ry(self,i):
     #     pass
 
-    def rx(self, theta, i):
+    def Rx(self, theta, i):
 
-        matrix = np.cos(theta/2) * self.I - 1j * np.sin(theta/2) * self.x
+        rx = np.cos(theta/2) * self.I - 1j * np.sin(theta/2) * self.x
         # self.operate(Rx, i) 
+        matrix = self._make_op_mat(rx, i)
         self.circuit.append(Gate('Rx', matrix, self.n_qubit))
         self._update_gate_history(f'Rx_{theta}', i)
 
-    def ry(self, phi, i):
-        matrix = np.cos(phi/2) * self.I - 1j * np.sin(phi/2) * self.y
+    def Ry(self, phi, i):
+        ry = np.cos(phi/2) * self.I - 1j * np.sin(phi/2) * self.y
         # self.operate(Ry, i)
+        matrix = self._make_op_mat(ry, i)
         self.circuit.append(Gate('Ry', matrix, self.n_qubit))
         self._update_gate_history(f'Ry_{phi}', i)
 
     def CNOT(self, control, target):
 
         if self.n_qubit == 1:
             raise ValueError("The CNOT gate can not be applied to a single qubit.")
@@ -235,20 +244,24 @@
 
         # self.state = matrix @ self.state
         self.circuit.append(Gate('SWAP', matrix, self.n_qubit))
         self._update_gate_history("SWAP", (qubit1, qubit2))
     
     def run(self):
         
-        '''Execute the circuit.'''
+        '''Execute the circuit. Return the result.'''
         for gate in self.circuit:
             self.state = gate.act(self.state)
         
-        self.circuit = [] # DO I DO THIS?
-        
+    def run_and_reset(self):
+        '''Execute the circuit and reset the circuit. Return the result.'''
+        self.run()
+        state = self.state
+        self.reset_circuit()
+        return state
 
     def prob(self):
         prob = np.abs(self.state**2)
         return prob
 
     def measure(self, n_shots=1):
         ''' n: number of shots 
@@ -290,14 +303,15 @@
                 'Rx': lambda angle: '\\gate{R_x(' + f"{angle}" + ')}',
                 'Ry': lambda angle: '\\gate{R_y(' + f"{angle}" + ')}',
                 'Sdag': '\\gate{S^\\dagger}',
                 'CNOTctrl': lambda dist: "\\ctrl{" + f"{dist}" + '}',
                 'CNOTtrgt': '\\targ{}',
                 'SWAP1': lambda dist: "\\swap{" + f"{dist}" + '}',
                 'SWAP2': '\\targX{}',
+                # 'exp': lambda axis, theta: f'\\gate{R_{axis}}'
             }
 
             max_gate_length = max(len(gates) for gates in self.gate_history.values())
             
             quantikz_str = "\\begin{quantikz}\n"
             
             for qubit in range(self.n_qubit):
```

### Comparing `Quanthon-0.3.3.4/Quanthon/utils.py` & `Quanthon-0.3.4/Quanthon/utils.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.3.4/Quanthon.egg-info/PKG-INFO` & `Quanthon-0.3.4/Quanthon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quanthon
-Version: 0.3.3.4
+Version: 0.3.4
 Summary: A quantum computing library
 Home-page: https://quanthon.readthedocs.io/
 Author: Keran Chen
 Author-email: keranc@uio.no
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -12,14 +12,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 
 # Quanthon
```

### Comparing `Quanthon-0.3.3.4/README.md` & `Quanthon-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.3.4/setup.py` & `Quanthon-0.3.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
     
 #### VERSION HERE #####
-version = "0.3.3.4" #####
+version = "0.3.4" #####
 #######################    
 
 setup(
     name="Quanthon",
     version=version,
     description="A quantum computing library",
     long_description=long_description,
@@ -35,13 +35,14 @@
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Operating System :: OS Independent"
     ],
     packages=["Quanthon"],
     include_package_data=True,
     install_requires=["numpy"]
 )
```

