# Comparing `tmp/Quanthon-0.3.4.1.tar.gz` & `tmp/Quanthon-0.3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Quanthon-0.3.4.1.tar", last modified: Wed Apr  3 13:33:00 2024, max compression
+gzip compressed data, was "Quanthon-0.3.4.2.tar", last modified: Wed Apr  3 18:39:45 2024, max compression
```

## Comparing `Quanthon-0.3.4.1.tar` & `Quanthon-0.3.4.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-03 13:33:00.479809 Quanthon-0.3.4.1/
--rw-r--r--   0 bukser     (501) staff       (20)        0 2023-09-14 17:15:45.000000 Quanthon-0.3.4.1/LICENSE
--rw-r--r--   0 bukser     (501) staff       (20)     2546 2024-04-03 13:33:00.479593 Quanthon-0.3.4.1/PKG-INFO
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-03 13:33:00.475955 Quanthon-0.3.4.1/Quanthon/
--rw-r--r--   0 bukser     (501) staff       (20)     3709 2024-03-04 09:48:46.000000 Quanthon-0.3.4.1/Quanthon/Models.py
--rw-r--r--   0 bukser     (501) staff       (20)      327 2024-03-19 15:53:35.000000 Quanthon-0.3.4.1/Quanthon/__init__.py
--rw-r--r--   0 bukser     (501) staff       (20)     3181 2024-03-19 14:55:03.000000 Quanthon-0.3.4.1/Quanthon/algorithms.py
--rw-r--r--   0 bukser     (501) staff       (20)     6268 2024-04-03 13:32:46.000000 Quanthon-0.3.4.1/Quanthon/algorithms_new.py
--rw-r--r--   0 bukser     (501) staff       (20)     4391 2024-04-02 14:29:33.000000 Quanthon-0.3.4.1/Quanthon/ansatzs.py
--rw-r--r--   0 bukser     (501) staff       (20)    11984 2024-03-21 12:14:41.000000 Quanthon-0.3.4.1/Quanthon/base.py
--rw-r--r--   0 bukser     (501) staff       (20)     5970 2024-03-21 11:59:47.000000 Quanthon-0.3.4.1/Quanthon/expectation.py
--rw-r--r--   0 bukser     (501) staff       (20)     9854 2024-03-19 15:01:41.000000 Quanthon-0.3.4.1/Quanthon/mappers.py
--rw-r--r--   0 bukser     (501) staff       (20)    12329 2024-04-02 13:21:56.000000 Quanthon-0.3.4.1/Quanthon/new_base.py
--rw-r--r--   0 bukser     (501) staff       (20)      452 2024-03-21 16:13:36.000000 Quanthon-0.3.4.1/Quanthon/physics.py
--rw-r--r--   0 bukser     (501) staff       (20)     2302 2024-03-13 12:44:21.000000 Quanthon-0.3.4.1/Quanthon/ut_pyscf_mel.py
--rw-r--r--   0 bukser     (501) staff       (20)     1714 2024-03-18 22:32:17.000000 Quanthon-0.3.4.1/Quanthon/ut_qiskit_hamiltonian.py
--rw-r--r--   0 bukser     (501) staff       (20)     5299 2024-03-21 16:15:37.000000 Quanthon-0.3.4.1/Quanthon/ut_test_jw.py
--rw-r--r--   0 bukser     (501) staff       (20)     4804 2024-04-02 12:23:12.000000 Quanthon-0.3.4.1/Quanthon/utils.py
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-03 13:33:00.479231 Quanthon-0.3.4.1/Quanthon.egg-info/
--rw-r--r--   0 bukser     (501) staff       (20)     2546 2024-04-03 13:33:00.000000 Quanthon-0.3.4.1/Quanthon.egg-info/PKG-INFO
--rw-r--r--   0 bukser     (501) staff       (20)      541 2024-04-03 13:33:00.000000 Quanthon-0.3.4.1/Quanthon.egg-info/SOURCES.txt
--rw-r--r--   0 bukser     (501) staff       (20)        1 2024-04-03 13:33:00.000000 Quanthon-0.3.4.1/Quanthon.egg-info/dependency_links.txt
--rw-r--r--   0 bukser     (501) staff       (20)        6 2024-04-03 13:33:00.000000 Quanthon-0.3.4.1/Quanthon.egg-info/requires.txt
--rw-r--r--   0 bukser     (501) staff       (20)        9 2024-04-03 13:33:00.000000 Quanthon-0.3.4.1/Quanthon.egg-info/top_level.txt
--rw-r--r--   0 bukser     (501) staff       (20)     1681 2024-03-04 14:05:24.000000 Quanthon-0.3.4.1/README.md
--rw-r--r--   0 bukser     (501) staff       (20)       38 2024-04-03 13:33:00.483545 Quanthon-0.3.4.1/setup.cfg
--rw-r--r--   0 bukser     (501) staff       (20)     1511 2024-04-03 13:32:53.000000 Quanthon-0.3.4.1/setup.py
-drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-03 13:33:00.477363 Quanthon-0.3.4.1/tests/
--rw-r--r--   0 bukser     (501) staff       (20)     6073 2024-04-03 12:26:28.000000 Quanthon-0.3.4.1/tests/test_adapt.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-03 18:39:45.678838 Quanthon-0.3.4.2/
+-rw-r--r--   0 bukser     (501) staff       (20)        0 2023-09-14 17:15:45.000000 Quanthon-0.3.4.2/LICENSE
+-rw-r--r--   0 bukser     (501) staff       (20)     2546 2024-04-03 18:39:45.678639 Quanthon-0.3.4.2/PKG-INFO
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-03 18:39:45.677352 Quanthon-0.3.4.2/Quanthon/
+-rw-r--r--   0 bukser     (501) staff       (20)     3709 2024-03-04 09:48:46.000000 Quanthon-0.3.4.2/Quanthon/Models.py
+-rw-r--r--   0 bukser     (501) staff       (20)      327 2024-03-19 15:53:35.000000 Quanthon-0.3.4.2/Quanthon/__init__.py
+-rw-r--r--   0 bukser     (501) staff       (20)     3181 2024-03-19 14:55:03.000000 Quanthon-0.3.4.2/Quanthon/algorithms.py
+-rw-r--r--   0 bukser     (501) staff       (20)     6270 2024-04-03 18:01:53.000000 Quanthon-0.3.4.2/Quanthon/algorithms_new.py
+-rw-r--r--   0 bukser     (501) staff       (20)     4403 2024-04-03 18:20:37.000000 Quanthon-0.3.4.2/Quanthon/ansatzs.py
+-rw-r--r--   0 bukser     (501) staff       (20)    11984 2024-03-21 12:14:41.000000 Quanthon-0.3.4.2/Quanthon/base.py
+-rw-r--r--   0 bukser     (501) staff       (20)     5974 2024-04-03 18:36:12.000000 Quanthon-0.3.4.2/Quanthon/expectation.py
+-rw-r--r--   0 bukser     (501) staff       (20)     9854 2024-03-19 15:01:41.000000 Quanthon-0.3.4.2/Quanthon/mappers.py
+-rw-r--r--   0 bukser     (501) staff       (20)    12029 2024-04-03 18:33:51.000000 Quanthon-0.3.4.2/Quanthon/new_base.py
+-rw-r--r--   0 bukser     (501) staff       (20)      452 2024-03-21 16:13:36.000000 Quanthon-0.3.4.2/Quanthon/physics.py
+-rw-r--r--   0 bukser     (501) staff       (20)     2302 2024-03-13 12:44:21.000000 Quanthon-0.3.4.2/Quanthon/ut_pyscf_mel.py
+-rw-r--r--   0 bukser     (501) staff       (20)     1714 2024-03-18 22:32:17.000000 Quanthon-0.3.4.2/Quanthon/ut_qiskit_hamiltonian.py
+-rw-r--r--   0 bukser     (501) staff       (20)     5299 2024-03-21 16:15:37.000000 Quanthon-0.3.4.2/Quanthon/ut_test_jw.py
+-rw-r--r--   0 bukser     (501) staff       (20)     4804 2024-04-03 18:16:14.000000 Quanthon-0.3.4.2/Quanthon/utils.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-03 18:39:45.678425 Quanthon-0.3.4.2/Quanthon.egg-info/
+-rw-r--r--   0 bukser     (501) staff       (20)     2546 2024-04-03 18:39:45.000000 Quanthon-0.3.4.2/Quanthon.egg-info/PKG-INFO
+-rw-r--r--   0 bukser     (501) staff       (20)      540 2024-04-03 18:39:45.000000 Quanthon-0.3.4.2/Quanthon.egg-info/SOURCES.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        1 2024-04-03 18:39:45.000000 Quanthon-0.3.4.2/Quanthon.egg-info/dependency_links.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        6 2024-04-03 18:39:45.000000 Quanthon-0.3.4.2/Quanthon.egg-info/requires.txt
+-rw-r--r--   0 bukser     (501) staff       (20)        9 2024-04-03 18:39:45.000000 Quanthon-0.3.4.2/Quanthon.egg-info/top_level.txt
+-rw-r--r--   0 bukser     (501) staff       (20)     1681 2024-03-04 14:05:24.000000 Quanthon-0.3.4.2/README.md
+-rw-r--r--   0 bukser     (501) staff       (20)       38 2024-04-03 18:39:45.678887 Quanthon-0.3.4.2/setup.cfg
+-rw-r--r--   0 bukser     (501) staff       (20)     1511 2024-04-03 18:39:16.000000 Quanthon-0.3.4.2/setup.py
+drwxr-xr-x   0 bukser     (501) staff       (20)        0 2024-04-03 18:39:45.678258 Quanthon-0.3.4.2/tests/
+-rw-r--r--   0 bukser     (501) staff       (20)     5905 2024-04-03 18:39:02.000000 Quanthon-0.3.4.2/tests/test_vqes.py
```

### Comparing `Quanthon-0.3.4.1/PKG-INFO` & `Quanthon-0.3.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quanthon
-Version: 0.3.4.1
+Version: 0.3.4.2
 Summary: A quantum computing library
 Home-page: https://quanthon.readthedocs.io/
 Author: Keran Chen
 Author-email: keranc@uio.no
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Quanthon-0.3.4.1/Quanthon/Models.py` & `Quanthon-0.3.4.2/Quanthon/Models.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4.1/Quanthon/algorithms.py` & `Quanthon-0.3.4.2/Quanthon/algorithms.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4.1/Quanthon/algorithms_new.py` & `Quanthon-0.3.4.2/Quanthon/algorithms_new.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
         # print(op_cand)
         
         for op in self.ansatz.pool:
             op_mat = pauli_sum([(op.strip('i'), 1j)])
             op_grad = self.gradient(op_mat)
             abs_grad = np.abs(op_grad)
             
-            print(f"op: {op}, grad: {op_grad}")
+            # print(f"op: {op}, grad: {op_grad}")
 
             if abs_grad > max_abs_grad:
                 op_cand = op
                 max_abs_grad = abs_grad
         
         if max_abs_grad < eps:
             print(f"end of adapt, grad = {max_abs_grad}")
```

### Comparing `Quanthon-0.3.4.1/Quanthon/ansatzs.py` & `Quanthon-0.3.4.2/Quanthon/ansatzs.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
         
         reshaped_params = init_params.reshape(self.reps, 2*self.n_qubits)
         
         for r in range(self.reps):
             for i in range(self.n_qubits):
                 self.qubits.Rx(reshaped_params[r, i], i)
                 self.qubits.Ry(reshaped_params[r, i + self.n_qubits], i)
-                if i % 2 == 0:
+                if i != self.n_qubits - 1:
                     self.qubits.CNOT(i, i+1)
         
 
         
 
     def run(self):
         self.qubits.run()
```

### Comparing `Quanthon-0.3.4.1/Quanthon/base.py` & `Quanthon-0.3.4.2/Quanthon/base.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4.1/Quanthon/expectation.py` & `Quanthon-0.3.4.2/Quanthon/expectation.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,15 @@
 		qc: the circuit to be measured in
 	'''
 
 	expectation = 0
 	for pauli_str, coeff in pauli_ops:
 
 		
-		if pauli_str == 'IIII':
+		if set(pauli_str) == {'I'}:
 			expectation += coeff
 			continue
 		# print(pauli_str, coeff)
 		state_eigval = np.ones(len(qc.state))
 		state_eigval[int(0.5*len(qc.state)):] *= -1 # first half of state has eigenvalue 1 and the second half -1
 		# print(state_eigval)
 		qc_copy = qc.copy()
```

### Comparing `Quanthon-0.3.4.1/Quanthon/mappers.py` & `Quanthon-0.3.4.2/Quanthon/mappers.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4.1/Quanthon/new_base.py` & `Quanthon-0.3.4.2/Quanthon/new_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -180,22 +180,14 @@
         self._update_gate_history('Z', i)
     
     def Sdag(self,i):
         # self.operate(self.s.conj(), i)
         matrix = self._make_op_mat(self.s.conj(), i)
         self.circuit.append(Gate('Sdag', matrix, self.n_qubit))
         self._update_gate_history('Sdag', i)
-    
-    # def param_rx(self, theta, i):
-    #     matrix = lambda theta: np.cos(theta/2) * self.I - 1j * np.sin(theta/2) * self.x
-    #     self.circuit.append(Gate('Rx', matrix, self.n_qubit, theta))
-    #     self._update_gate_history(r'Rx_\theta', i)
-
-    # def param_ry(self,i):
-    #     pass
 
     def Rx(self, theta, i):
 
         rx = np.cos(theta/2) * self.I - 1j * np.sin(theta/2) * self.x
         # self.operate(Rx, i) 
         matrix = self._make_op_mat(rx, i)
         self.circuit.append(Gate('Rx', matrix, self.n_qubit))
@@ -232,15 +224,14 @@
 
     def SWAP(self, qubit1, qubit2):
         if self.n_qubit == 1:
             raise ValueError("The SWAP gate can not be applied to a single qubit.")
         
 
         matrix = np.zeros((self.opeartor_size, self.opeartor_size))
-
         for i in range(self.opeartor_size):
             j = swap_bits(i, self.n_qubit - qubit1 - 1, self.n_qubit - qubit2 - 1)
             matrix[i, j] = 1
             matrix[j, i] = 1
 
         # self.state = matrix @ self.state
         self.circuit.append(Gate('SWAP', matrix, self.n_qubit))
```

### Comparing `Quanthon-0.3.4.1/Quanthon/ut_pyscf_mel.py` & `Quanthon-0.3.4.2/Quanthon/ut_pyscf_mel.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4.1/Quanthon/ut_qiskit_hamiltonian.py` & `Quanthon-0.3.4.2/Quanthon/ut_qiskit_hamiltonian.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4.1/Quanthon/ut_test_jw.py` & `Quanthon-0.3.4.2/Quanthon/ut_test_jw.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4.1/Quanthon/utils.py` & `Quanthon-0.3.4.2/Quanthon/utils.py`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4.1/Quanthon.egg-info/PKG-INFO` & `Quanthon-0.3.4.2/Quanthon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Quanthon
-Version: 0.3.4.1
+Version: 0.3.4.2
 Summary: A quantum computing library
 Home-page: https://quanthon.readthedocs.io/
 Author: Keran Chen
 Author-email: keranc@uio.no
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Quanthon-0.3.4.1/Quanthon.egg-info/SOURCES.txt` & `Quanthon-0.3.4.2/Quanthon.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 Quanthon/ut_test_jw.py
 Quanthon/utils.py
 Quanthon.egg-info/PKG-INFO
 Quanthon.egg-info/SOURCES.txt
 Quanthon.egg-info/dependency_links.txt
 Quanthon.egg-info/requires.txt
 Quanthon.egg-info/top_level.txt
-tests/test_adapt.py
+tests/test_vqes.py
```

### Comparing `Quanthon-0.3.4.1/README.md` & `Quanthon-0.3.4.2/README.md`

 * *Files identical despite different names*

### Comparing `Quanthon-0.3.4.1/setup.py` & `Quanthon-0.3.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
     
 #### VERSION HERE #####
-version = "0.3.4.1" #####
+version = "0.3.4.2" #####
 #######################    
 
 setup(
     name="Quanthon",
     version=version,
     description="A quantum computing library",
     long_description=long_description,
```

### Comparing `Quanthon-0.3.4.1/tests/test_adapt.py` & `Quanthon-0.3.4.2/tests/test_vqes.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,28 +18,20 @@
 import warnings
 
 from Quanthon import VQE, AdaptVQE, jordan_wigner, Hamiltonian, QubitAdaptAnsatz, HardwareEfficietnAnsatz, pauli_sum
 
 
 class AlgorithmTest(unittest.TestCase):
 
-    def _qiskit_hardware(self):
+    def _qiskit_hardware(self, op):
         
         warnings.filterwarnings("ignore")
 
         estimator = Estimator()
-        H2_op = SparsePauliOp.from_list(
-        [
-            ("II", -1.052373245772859),
-            ("IZ", 0.39793742484318045),
-            ("ZI", -0.39793742484318045),
-            ("ZZ", -0.01128010425623538),
-            ("XX", 0.18093119978423156),
-        ]
-        )
+        qubit_op = SparsePauliOp.from_list(op)
 
         # we will iterate over these different optimizers
         optimizers = [COBYLA(maxiter=80), L_BFGS_B(maxiter=60), SLSQP(maxiter=60)]
         converge_counts = np.empty([len(optimizers)], dtype=object)
         converge_vals = np.empty([len(optimizers)], dtype=object)
 
         for i, optimizer in enumerate(optimizers):
@@ -51,15 +43,15 @@
             values = []
 
             def store_intermediate_result(eval_count, parameters, mean, std):
                 counts.append(eval_count)
                 values.append(mean)
 
             vqe = qk_VQE(estimator, ansatz, optimizer, callback=store_intermediate_result)
-            result = vqe.compute_minimum_eigenvalue(operator=H2_op)
+            result = vqe.compute_minimum_eigenvalue(operator=qubit_op)
             converge_counts[i] = np.asarray(counts)
             converge_vals[i] = np.asarray(values)
         
         return result
     
     def _qiskit_adapt(self):
         
@@ -88,38 +80,40 @@
         adapt_vqe = AdaptVQE(vqe)
         eigenvalue, _ = adapt_vqe.compute_minimum_eigenvalue(qubit_op)
         print(eigenvalue)
 
         return eigenvalue
 
     
-    def _test_vqe(self):
+    def test_vqe(self):
 
-        qubit_op =[("II", -1.052373245772859),
+        op_str =[("II", -1.052373245772859),
                     ("IZ", 0.39793742484318045),
                     ("ZI", -0.39793742484318045),
                     ("ZZ", -0.01128010425623538),
                     ("XX", 0.18093119978423156),
                 ]
+        
         ansatz = HardwareEfficietnAnsatz(2, reps=2)
 
         rng = np.random.default_rng(826)
         n_params = ansatz.n_params
 
         init_points = rng.random(n_params) * 2 * np.pi - np.pi 
         vqe = VQE(ansatz, init_points)
-        min_params, min_energy = vqe.minimise_eigenvalue(qubit_op, 1000)
+        min_params, min_energy = vqe.minimise_eigenvalue(op_str, 1000)
         print(min_energy)
 
         # with qiskit
 
-        result = self._qiskit_hardware()
+        result = self._qiskit_hardware(op_str)
+        # print("diff from qiskit")
         print(result.eigenvalue)
     
-    def test_adapt_vqe(self):
+    def _test_adapt_vqe(self):
 
         qubit_op =[("II", -1.052373245772859),
                     ("IZ", 0.39793742484318045),
                     ("ZI", -0.39793742484318045),
                     ("ZZ", -0.01128010425623538),
                     ("XX", 0.18093119978423156),
                 ]
@@ -134,15 +128,15 @@
 
         vqe = AdaptVQE(ansatz)
         ansatz, min_energy = vqe.run_adapt_circuit(qubit_op, 10000, max_iter=10)
         print(min_energy)
 
         # with qiskit
 
-        result = self._qiskit_hardware()
+        result = self._qiskit_hardware(qubit_op)
         print(result.eigenvalue)
 
  
 
 def matrix_to_fermionic_op(one_body_matrix, two_body_matrix):
     # Get the size of the one-body matrix
     n = one_body_matrix.shape[0]
```

