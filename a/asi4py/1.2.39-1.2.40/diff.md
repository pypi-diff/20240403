# Comparing `tmp/asi4py-1.2.39.tar.gz` & `tmp/asi4py-1.2.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asi4py-1.2.39.tar", last modified: Tue Mar 26 11:49:11 2024, max compression
+gzip compressed data, was "asi4py-1.2.40.tar", last modified: Wed Apr  3 16:33:11 2024, max compression
```

## Comparing `asi4py-1.2.39.tar` & `asi4py-1.2.40.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 11:49:11.005306 asi4py-1.2.39/
--rw-rw-rw-   0 root         (0) root         (0)     1180 2023-04-16 18:02:20.000000 asi4py-1.2.39/LICENSE
--rw-r--r--   0 root         (0) root         (0)     4498 2024-03-26 11:49:11.001305 asi4py-1.2.39/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2558 2023-04-16 18:02:20.000000 asi4py-1.2.39/README.md
--rw-rw-rw-   0 root         (0) root         (0)      680 2024-03-26 11:11:34.000000 asi4py-1.2.39/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-26 11:49:11.005306 asi4py-1.2.39/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 11:49:11.001305 asi4py-1.2.39/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 11:49:11.001305 asi4py-1.2.39/src/asi4py/
--rw-rw-rw-   0 root         (0) root         (0)      178 2024-02-23 22:44:56.000000 asi4py-1.2.39/src/asi4py/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2568 2023-04-19 20:01:15.000000 asi4py-1.2.39/src/asi4py/asecalc.py
--rw-rw-rw-   0 root         (0) root         (0)    18413 2024-03-26 11:11:34.000000 asi4py-1.2.39/src/asi4py/pyasi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 11:49:11.001305 asi4py-1.2.39/src/asi4py.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4498 2024-03-26 11:49:10.000000 asi4py-1.2.39/src/asi4py.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      266 2024-03-26 11:49:10.000000 asi4py-1.2.39/src/asi4py.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 11:49:10.000000 asi4py-1.2.39/src/asi4py.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2024-03-26 11:49:10.000000 asi4py-1.2.39/src/asi4py.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2024-03-26 11:49:10.000000 asi4py-1.2.39/src/asi4py.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:33:11.510376 asi4py-1.2.40/
+-rw-rw-rw-   0 root         (0) root         (0)     1180 2022-07-19 20:58:13.000000 asi4py-1.2.40/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     4498 2024-04-03 16:33:11.509376 asi4py-1.2.40/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2558 2022-07-19 20:58:13.000000 asi4py-1.2.40/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      680 2024-04-03 16:32:37.000000 asi4py-1.2.40/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-03 16:33:11.510376 asi4py-1.2.40/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:33:11.507376 asi4py-1.2.40/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:33:11.508376 asi4py-1.2.40/src/asi4py/
+-rw-rw-rw-   0 root         (0) root         (0)      178 2024-02-23 22:51:32.000000 asi4py-1.2.40/src/asi4py/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2568 2023-04-19 19:59:38.000000 asi4py-1.2.40/src/asi4py/asecalc.py
+-rw-rw-rw-   0 root         (0) root         (0)    19321 2024-04-03 16:32:37.000000 asi4py-1.2.40/src/asi4py/pyasi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 16:33:11.509376 asi4py-1.2.40/src/asi4py.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4498 2024-04-03 16:33:11.000000 asi4py-1.2.40/src/asi4py.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      266 2024-04-03 16:33:11.000000 asi4py-1.2.40/src/asi4py.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 16:33:11.000000 asi4py-1.2.40/src/asi4py.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2024-04-03 16:33:11.000000 asi4py-1.2.40/src/asi4py.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2024-04-03 16:33:11.000000 asi4py-1.2.40/src/asi4py.egg-info/top_level.txt
```

### Comparing `asi4py-1.2.39/LICENSE` & `asi4py-1.2.40/LICENSE`

 * *Files identical despite different names*

### Comparing `asi4py-1.2.39/PKG-INFO` & `asi4py-1.2.40/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asi4py
-Version: 1.2.39
+Version: 1.2.40
 Summary: A Python wrapper for Atomic Simulation Interface API
 Author-email: Pavel Stishenko <pstishenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Pavel V Stishenko, Andrew Logsdail, Reinhard Maurer, 
         Volker Blum, Mariana Rossi, Ben Hourahine, Scott Woodley, Thomas Keal
```

### Comparing `asi4py-1.2.39/README.md` & `asi4py-1.2.40/README.md`

 * *Files identical despite different names*

### Comparing `asi4py-1.2.39/src/asi4py/asecalc.py` & `asi4py-1.2.40/src/asi4py/asecalc.py`

 * *Files identical despite different names*

### Comparing `asi4py-1.2.39/src/asi4py/pyasi.py` & `asi4py-1.2.40/src/asi4py/pyasi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from ctypes import cdll, CDLL, RTLD_GLOBAL
-from ctypes import POINTER, byref, c_int, c_int64, c_int32, c_bool, c_char_p, c_double, c_void_p, CFUNCTYPE, py_object, cast, byref
+from ctypes import POINTER, byref, c_int, c_int64, c_int32, c_bool, c_char_p, c_double, c_void_p, CFUNCTYPE, py_object, cast, byref, Structure
 import ctypes
 
 '''
 CDLL(MPI.__file__, mode=RTLD_GLOBAL) is a workaround for a few MPICH bugs, including 
 the bug with non-working MPI_IN_PLACE and 2-stage ELPA solver
 https://bitbucket.org/mpi4py/mpi4py/issues/162/mpi4py-initialization-breaks-fortran
 https://lists.mpich.org/pipermail/discuss/2020-July/006018.html
@@ -20,14 +20,29 @@
 import os, shutil
 from ase import units
 from scalapack4py import ScaLAPACK4py
 
 dmhs_callback = CFUNCTYPE(None, c_void_p, c_int, c_int, POINTER(c_int), POINTER(c_double))  # void(*)(void *aux_ptr, int iK, int iS, int *blacs_descr, void *blacs_data)
 esp_callback = CFUNCTYPE(None, c_void_p, c_int, POINTER(c_double), POINTER(c_double), POINTER(c_double))   # void(*)(void *aux_ptr, int n, const double *coords, double *potential, double *potential_grad)
 
+class ASI_basis_func_descr_generic(Structure):
+  '''
+     Generic basis function descriptior.
+     Use basis_func_descr_type field to find actual structure type
+     in basis_func_descr_ptr_types dict
+  '''
+  _fields_ = [("descr_size",c_int), ("basis_func_descr_type",c_int),]
+
+class ASI_basis_func_descr_generic_local(Structure):
+  _fields_ = [("descr_size",c_int), ("basis_func_descr_type",c_int), ("atom_index",c_int),]
+
+basis_func_descr_types = {101:ASI_basis_func_descr_generic_local}
+
+
+
 def ltriang2herm_inplace(X):
   i_upper = np.triu_indices(X.shape[0], 1)
   X[i_upper] = X.T[i_upper].conj()
 
 def HS_to_DM(H, S):
   '''
     Compute density matrix from Hamiltonian (H) and overlap (S) matrices
@@ -161,16 +176,17 @@
       self.lib.ASI_register_overlap_callback.argtypes = [dmhs_callback, c_void_p]
       self.lib.ASI_register_hamiltonian_callback.argtypes = [dmhs_callback, c_void_p]
       if hasattr(self.lib, "ASI_register_dm_init_callback"):
         self.lib.ASI_register_dm_init_callback.argtypes = [dmhs_callback, c_void_p]
       self.lib.ASI_register_external_potential.argtypes = [esp_callback, c_void_p];
       self.lib.ASI_is_hamiltonian_real.restype = c_bool
       self.lib.ASI_get_basis_size.restype = c_int
-      if hasattr(self.lib, "ASI_basis_atoms"):
-        self.lib.ASI_basis_atoms.restype = POINTER(c_int)
+      if hasattr(self.lib, "ASI_get_basis_func_descr"):
+        self.lib.ASI_get_basis_func_descr.restype = POINTER(ASI_basis_func_descr_generic)
+        self.lib.ASI_get_basis_func_descr.argtypes = [c_int,]
       self.lib.ASI_get_nspin.restype = c_int
       self.lib.ASI_get_nkpts.restype = c_int
       self.lib.ASI_get_n_local_ks.restype = c_int
       self.lib.ASI_get_local_ks.restype = c_int
       self.lib.ASI_get_local_ks.argtypes = [ndpointer(dtype=np.int32),]
       self.lib.ASI_is_hamiltonian_real.restype = c_bool
       
@@ -182,14 +198,17 @@
     finally:
       os.chdir(curdir)
   
   def close(self):
     '''
       Calls `ASI_finalize()`. No ASI calls are should be attempted after that function call.
     '''
+    if not hasattr(self, 'lib'):
+      return # allready closed
+
     curdir = os.getcwd()
     try:
       os.chdir(self.work_dir)
       self.lib.ASI_finalize()
       handle = self.lib._handle
       del self.lib
       if self.mpi_comm.Get_rank() == 0:
@@ -352,29 +371,31 @@
   def n_basis(self):
     """
       int: Number of basis functions
 
       Calls `ASI_get_basis_size()`
     """
     return self.lib.ASI_get_basis_size()
+  
+  def get_basis_func_descr(self, bf_index):
+    if not hasattr(self.lib, "ASI_get_basis_func_descr"):
+      raise NotImplementedError("ASI_get_basis_func_descr not implemented in {self.lib_file}")
+    
+    descr_ptr = self.lib.ASI_get_basis_func_descr(bf_index)
+    descr_ptr_specific = cast(descr_ptr, POINTER(basis_func_descr_types[descr_ptr.contents.basis_func_descr_type]))
+    return descr_ptr_specific.contents
 
   @property
   def basis_atoms(self):
     """
       int[n_basis]: Atomic indices for each basis function
 
-      Calls `ASI_basis_atoms()`
+      Calls `ASI_get_basis_func_descr()` and `ASI_get_basis_size()`
     """
-    if not hasattr(self.lib, "ASI_basis_atoms"):
-      raise NotImplementedError("ASI_basis_atoms not implemented in {self.lib_file}")
-    basis_atoms_ptr = self.lib.ASI_basis_atoms()
-    if basis_atoms_ptr:
-      return np.ctypeslib.as_array(basis_atoms_ptr, shape=(self.n_basis, ))
-    else:
-      return None
+    return np.array([self.get_basis_func_descr(i).atom_index for i in range(self.n_basis)])
 
   @property
   def n_spin(self):
     """
       int: Number of spin channels
 
       Calls `ASI_get_nspin()`
```

### Comparing `asi4py-1.2.39/src/asi4py.egg-info/PKG-INFO` & `asi4py-1.2.40/src/asi4py.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asi4py
-Version: 1.2.39
+Version: 1.2.40
 Summary: A Python wrapper for Atomic Simulation Interface API
 Author-email: Pavel Stishenko <pstishenko@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 Pavel V Stishenko, Andrew Logsdail, Reinhard Maurer, 
         Volker Blum, Mariana Rossi, Ben Hourahine, Scott Woodley, Thomas Keal
```

