# Comparing `tmp/elphmod-0.8.tar.gz` & `tmp/elphmod-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elphmod-0.8.tar", last modified: Tue Nov  2 12:16:04 2021, max compression
+gzip compressed data, was "elphmod-0.9.tar", last modified: Thu Jan  6 17:56:02 2022, max compression
```

## Comparing `elphmod-0.8.tar` & `elphmod-0.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2021-11-02 12:16:04.172623 elphmod-0.8/
--rw-rw-r--   0 jan       (1000) jan       (1000)    35149 2021-01-17 10:15:03.000000 elphmod-0.8/LICENSE
--rw-rw-r--   0 jan       (1000) jan       (1000)       14 2021-11-02 10:01:24.000000 elphmod-0.8/MANIFEST.in
--rw-rw-r--   0 jan       (1000) jan       (1000)     3258 2021-11-02 12:16:04.172623 elphmod-0.8/PKG-INFO
--rw-rw-r--   0 jan       (1000) jan       (1000)     2784 2021-10-14 11:45:59.000000 elphmod-0.8/README.md
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2021-11-02 12:16:04.172623 elphmod-0.8/bin/
--rwxrwxr-x   0 jan       (1000) jan       (1000)      703 2021-10-14 11:45:59.000000 elphmod-0.8/bin/elphmodenv
--rwxrwxr-x   0 jan       (1000) jan       (1000)      549 2021-11-01 08:32:58.000000 elphmod-0.8/bin/kpoints
--rwxrwxr-x   0 jan       (1000) jan       (1000)      589 2021-10-14 11:45:59.000000 elphmod-0.8/bin/minimum
--rwxrwxr-x   0 jan       (1000) jan       (1000)      993 2021-02-18 08:22:47.000000 elphmod-0.8/bin/ph2epw
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2021-11-02 12:16:04.172623 elphmod-0.8/elphmod/
--rwxrwxr-x   0 jan       (1000) jan       (1000)     6263 2021-10-14 11:45:59.000000 elphmod-0.8/elphmod/MPI.py
--rwxrwxr-x   0 jan       (1000) jan       (1000)      471 2021-11-02 12:08:31.000000 elphmod-0.8/elphmod/__init__.py
--rwxrwxr-x   0 jan       (1000) jan       (1000)    73250 2021-10-14 11:45:59.000000 elphmod-0.8/elphmod/bravais.py
--rwxrwxr-x   0 jan       (1000) jan       (1000)    30011 2021-10-14 11:45:59.000000 elphmod-0.8/elphmod/diagrams.py
--rwxrwxr-x   0 jan       (1000) jan       (1000)    16581 2021-10-14 11:45:59.000000 elphmod-0.8/elphmod/dispersion.py
--rwxrwxr-x   0 jan       (1000) jan       (1000)    10513 2021-10-14 11:45:59.000000 elphmod-0.8/elphmod/dos.py
--rwxrwxr-x   0 jan       (1000) jan       (1000)    35042 2021-10-22 07:49:05.000000 elphmod-0.8/elphmod/el.py
--rwxrwxr-x   0 jan       (1000) jan       (1000)     6937 2021-10-14 11:45:59.000000 elphmod-0.8/elphmod/elel.py
--rwxrwxr-x   0 jan       (1000) jan       (1000)     2810 2021-10-14 11:45:59.000000 elphmod-0.8/elphmod/eliashberg.py
--rwxrwxr-x   0 jan       (1000) jan       (1000)    30542 2021-10-14 11:45:59.000000 elphmod-0.8/elphmod/elph.py
--rwxrwxr-x   0 jan       (1000) jan       (1000)     6303 2021-10-14 11:45:59.000000 elphmod-0.8/elphmod/misc.py
--rwxrwxr-x   0 jan       (1000) jan       (1000)     5212 2021-10-14 11:45:59.000000 elphmod-0.8/elphmod/occupations.py
--rwxrwxr-x   0 jan       (1000) jan       (1000)    34700 2021-10-22 07:49:05.000000 elphmod-0.8/elphmod/ph.py
--rwxrwxr-x   0 jan       (1000) jan       (1000)    26536 2021-10-14 11:45:59.000000 elphmod-0.8/elphmod/plot.py
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2021-11-02 12:16:04.172623 elphmod-0.8/elphmod.egg-info/
--rw-rw-r--   0 jan       (1000) jan       (1000)     3258 2021-11-02 12:16:04.000000 elphmod-0.8/elphmod.egg-info/PKG-INFO
--rw-rw-r--   0 jan       (1000) jan       (1000)      617 2021-11-02 12:16:04.000000 elphmod-0.8/elphmod.egg-info/SOURCES.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)        1 2021-11-02 12:16:04.000000 elphmod-0.8/elphmod.egg-info/dependency_links.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)        6 2021-11-02 12:16:04.000000 elphmod-0.8/elphmod.egg-info/requires.txt
--rw-rw-r--   0 jan       (1000) jan       (1000)        8 2021-11-02 12:16:04.000000 elphmod-0.8/elphmod.egg-info/top_level.txt
-drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2021-11-02 12:16:04.172623 elphmod-0.8/patches/
--rw-rw-r--   0 jan       (1000) jan       (1000)      472 2021-10-14 11:45:59.000000 elphmod-0.8/patches/README.md
--rw-rw-r--   0 jan       (1000) jan       (1000)     9150 2021-10-14 11:45:59.000000 elphmod-0.8/patches/qe-6.3-backports.patch
--rw-rw-r--   0 jan       (1000) jan       (1000)    13647 2021-10-14 14:33:40.000000 elphmod-0.8/patches/qe-6.7MaX-Release.patch
--rw-rw-r--   0 jan       (1000) jan       (1000)    13689 2021-10-14 14:33:23.000000 elphmod-0.8/patches/qe-6.8.patch
--rw-rw-r--   0 jan       (1000) jan       (1000)       98 2021-10-14 11:45:59.000000 elphmod-0.8/pyproject.toml
--rw-rw-r--   0 jan       (1000) jan       (1000)      610 2021-11-02 12:16:04.172623 elphmod-0.8/setup.cfg
--rwxrwxr-x   0 jan       (1000) jan       (1000)      178 2021-10-14 11:45:59.000000 elphmod-0.8/setup.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2022-01-06 17:56:02.937546 elphmod-0.9/
+-rw-rw-r--   0 jan       (1000) jan       (1000)    35149 2021-01-17 10:15:03.000000 elphmod-0.9/LICENSE
+-rw-rw-r--   0 jan       (1000) jan       (1000)       14 2021-11-02 10:01:24.000000 elphmod-0.9/MANIFEST.in
+-rw-rw-r--   0 jan       (1000) jan       (1000)     3258 2022-01-06 17:56:02.937546 elphmod-0.9/PKG-INFO
+-rw-rw-r--   0 jan       (1000) jan       (1000)     2784 2021-10-14 11:45:59.000000 elphmod-0.9/README.md
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2022-01-06 17:56:02.937546 elphmod-0.9/bin/
+-rwxrwxr-x   0 jan       (1000) jan       (1000)      703 2021-10-14 11:45:59.000000 elphmod-0.9/bin/elphmodenv
+-rwxrwxr-x   0 jan       (1000) jan       (1000)      549 2021-11-01 08:32:58.000000 elphmod-0.9/bin/kpoints
+-rwxrwxr-x   0 jan       (1000) jan       (1000)      589 2021-10-14 11:45:59.000000 elphmod-0.9/bin/minimum
+-rwxrwxr-x   0 jan       (1000) jan       (1000)      993 2021-02-18 08:22:47.000000 elphmod-0.9/bin/ph2epw
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2022-01-06 17:56:02.937546 elphmod-0.9/elphmod/
+-rwxrwxr-x   0 jan       (1000) jan       (1000)     7934 2022-01-06 17:38:48.000000 elphmod-0.9/elphmod/MPI.py
+-rwxrwxr-x   0 jan       (1000) jan       (1000)      476 2022-01-06 17:42:42.000000 elphmod-0.9/elphmod/__init__.py
+-rwxrwxr-x   0 jan       (1000) jan       (1000)    73268 2022-01-06 17:38:48.000000 elphmod-0.9/elphmod/bravais.py
+-rwxrwxr-x   0 jan       (1000) jan       (1000)    30016 2022-01-06 17:38:48.000000 elphmod-0.9/elphmod/diagrams.py
+-rwxrwxr-x   0 jan       (1000) jan       (1000)    16586 2022-01-06 17:38:48.000000 elphmod-0.9/elphmod/dispersion.py
+-rwxrwxr-x   0 jan       (1000) jan       (1000)    11671 2022-01-06 17:38:48.000000 elphmod-0.9/elphmod/dos.py
+-rwxrwxr-x   0 jan       (1000) jan       (1000)    37425 2022-01-06 17:38:48.000000 elphmod-0.9/elphmod/el.py
+-rwxrwxr-x   0 jan       (1000) jan       (1000)    11724 2022-01-06 17:38:48.000000 elphmod-0.9/elphmod/elel.py
+-rwxrwxr-x   0 jan       (1000) jan       (1000)     2815 2022-01-06 17:38:48.000000 elphmod-0.9/elphmod/eliashberg.py
+-rwxrwxr-x   0 jan       (1000) jan       (1000)    30991 2022-01-06 17:38:48.000000 elphmod-0.9/elphmod/elph.py
+-rwxrwxr-x   0 jan       (1000) jan       (1000)    10610 2022-01-06 17:38:48.000000 elphmod-0.9/elphmod/misc.py
+-rwxrwxr-x   0 jan       (1000) jan       (1000)     5217 2022-01-06 17:38:48.000000 elphmod-0.9/elphmod/occupations.py
+-rwxrwxr-x   0 jan       (1000) jan       (1000)    35326 2022-01-06 17:38:48.000000 elphmod-0.9/elphmod/ph.py
+-rwxrwxr-x   0 jan       (1000) jan       (1000)    26541 2022-01-06 17:38:48.000000 elphmod-0.9/elphmod/plot.py
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2022-01-06 17:56:02.937546 elphmod-0.9/elphmod.egg-info/
+-rw-rw-r--   0 jan       (1000) jan       (1000)     3258 2022-01-06 17:56:02.000000 elphmod-0.9/elphmod.egg-info/PKG-INFO
+-rw-rw-r--   0 jan       (1000) jan       (1000)      617 2022-01-06 17:56:02.000000 elphmod-0.9/elphmod.egg-info/SOURCES.txt
+-rw-rw-r--   0 jan       (1000) jan       (1000)        1 2022-01-06 17:56:02.000000 elphmod-0.9/elphmod.egg-info/dependency_links.txt
+-rw-rw-r--   0 jan       (1000) jan       (1000)        6 2022-01-06 17:56:02.000000 elphmod-0.9/elphmod.egg-info/requires.txt
+-rw-rw-r--   0 jan       (1000) jan       (1000)        8 2022-01-06 17:56:02.000000 elphmod-0.9/elphmod.egg-info/top_level.txt
+drwxrwxr-x   0 jan       (1000) jan       (1000)        0 2022-01-06 17:56:02.937546 elphmod-0.9/patches/
+-rw-rw-r--   0 jan       (1000) jan       (1000)      472 2021-10-14 11:45:59.000000 elphmod-0.9/patches/README.md
+-rw-rw-r--   0 jan       (1000) jan       (1000)     9150 2021-10-14 11:45:59.000000 elphmod-0.9/patches/qe-6.3-backports.patch
+-rw-rw-r--   0 jan       (1000) jan       (1000)    13647 2021-10-14 14:33:40.000000 elphmod-0.9/patches/qe-6.7MaX-Release.patch
+-rw-rw-r--   0 jan       (1000) jan       (1000)    13689 2021-10-14 14:33:23.000000 elphmod-0.9/patches/qe-6.8.patch
+-rw-rw-r--   0 jan       (1000) jan       (1000)       98 2021-10-14 11:45:59.000000 elphmod-0.9/pyproject.toml
+-rw-rw-r--   0 jan       (1000) jan       (1000)      610 2022-01-06 17:56:02.937546 elphmod-0.9/setup.cfg
+-rwxrwxr-x   0 jan       (1000) jan       (1000)      183 2022-01-06 17:38:48.000000 elphmod-0.9/setup.py
```

### Comparing `elphmod-0.8/LICENSE` & `elphmod-0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `elphmod-0.8/PKG-INFO` & `elphmod-0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elphmod
-Version: 0.8
+Version: 0.9
 Summary: Modules to handle electron-phonon models
 Home-page: https://github.com/janberges/elphmod
 Author: elphmod Developers
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `elphmod-0.8/README.md` & `elphmod-0.9/README.md`

 * *Files identical despite different names*

### Comparing `elphmod-0.8/bin/elphmodenv` & `elphmod-0.9/bin/elphmodenv`

 * *Files identical despite different names*

### Comparing `elphmod-0.8/bin/kpoints` & `elphmod-0.9/bin/kpoints`

 * *Files identical despite different names*

### Comparing `elphmod-0.8/bin/minimum` & `elphmod-0.9/bin/minimum`

 * *Files identical despite different names*

### Comparing `elphmod-0.8/bin/ph2epw` & `elphmod-0.9/bin/ph2epw`

 * *Files identical despite different names*

### Comparing `elphmod-0.8/elphmod/bravais.py` & `elphmod-0.9/elphmod/bravais.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (C) 2021 elphmod Developers
+# Copyright (C) 2017-2022 elphmod Developers
 # This program is free software under the terms of the GNU GPLv3 or later.
 
 from __future__ import division
 
 import numpy as np
 
 from . import misc, MPI
@@ -1649,15 +1649,15 @@
 
         if 'celldm' in struct:
             for i, celldm in enumerate(struct['celldm'], 1):
                 if celldm:
                     data.write('celldm(%d) = %.12g\n' % (i, celldm))
 
         for key in ['a', 'b', 'c', 'nat', 'ibrav', 'ntyp',
-                    'ecutwfc', 'ecutrho', 'degauss', 'nbnd']:
+                'ecutwfc', 'ecutrho', 'degauss', 'nbnd']:
             if key in struct:
                 data.write('%s = %.12g\n' % (key, struct[key]))
 
         for key in ['occupations', 'smearing', 'nosym']:
             if key in struct:
                 data.write('%s = %s\n' % (key, struct[key]))
 
@@ -2186,18 +2186,18 @@
     struct : dict
         Input data.
     """
     if comm.rank != 0:
         return
 
     with open(matdyn, 'w') as data:
-
         data.write('&INPUT\n')
 
-        for key in 'asr', 'flfrq', 'flfrc', 'q_in_band_form', 'q_in_cryst_coord':
+        for key in ['asr', 'flfrq', 'flfrc', 'q_in_band_form',
+                'q_in_cryst_coord']:
             if key in struct:
                 data.write('%s = %s\n' % (key, struct[key]))
 
         data.write('/\n')
         data.write('%d\n' % struct['nq'])
         for (kx, ky, kz, wk) in struct['q']:
             data.write('%.12g %.12g %.12g %.12g\n' % (kx, ky, kz, wk))
@@ -2371,33 +2371,33 @@
     """
     if comm.rank != 0:
         return
 
     with open(epw, 'w') as data:
 
         data.write('&INPUTEPW\n')
-        for key in ('prefix', 'outdir', 'dvscf_dir'):
+        for key in ['prefix', 'outdir', 'dvscf_dir']:
             if key in struct:
                 data.write('%s = %s\n' % (key, struct[key]))
 
         data.write('\n')
 
-        for key in ('wannierize', 'elph'):
+        for key in ['wannierize', 'elph']:
             if key in struct:
                 data.write('%s = %s\n' % (key, struct[key]))
 
         data.write('\n')
 
-        for key in ('epbwrite', 'epwwrite'):
+        for key in ['epbwrite', 'epwwrite']:
             if key in struct:
                 data.write('%s = %s\n' % (key, struct[key]))
 
         data.write('\n')
 
-        for key in ('epbread', 'epwread'):
+        for key in ['epbread', 'epwread']:
             if key in struct:
                 data.write('%s = %s\n' % (key, struct[key]))
 
         data.write('\n')
 
         for key in ['use_ws']:
             if key in struct:
```

### Comparing `elphmod-0.8/elphmod/diagrams.py` & `elphmod-0.9/elphmod/diagrams.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (C) 2021 elphmod Developers
+# Copyright (C) 2017-2022 elphmod Developers
 # This program is free software under the terms of the GNU GPLv3 or later.
 
 from __future__ import division
 
 import numpy as np
 
 from . import MPI, occupations
```

### Comparing `elphmod-0.8/elphmod/dispersion.py` & `elphmod-0.9/elphmod/dispersion.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (C) 2021 elphmod Developers
+# Copyright (C) 2017-2022 elphmod Developers
 # This program is free software under the terms of the GNU GPLv3 or later.
 
 import numpy as np
 
 from . import bravais, misc, MPI
 comm = MPI.comm
```

### Comparing `elphmod-0.8/elphmod/dos.py` & `elphmod-0.9/elphmod/dos.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,34 @@
 #!/usr/bin/env python3
 
-# Copyright (C) 2021 elphmod Developers
+# Copyright (C) 2017-2022 elphmod Developers
 # This program is free software under the terms of the GNU GPLv3 or later.
 
 import numpy as np
 
 from . import bravais, misc, MPI
 comm = MPI.comm
 
-def hexDOS(energies):
+def hexDOS(energies, minimum=None, maximum=None):
     r"""Calculate DOS from energies on triangular mesh (2D tetrahedron method).
 
+    Parameters
+    ----------
+    energies : ndarray
+        Energies on triangular mesh.
+    minimum, maximum : float, optional
+        Energy window of interest (for efficiency).
+
+    Returns
+    -------
+    function
+        Density of states as a function of energy.
+
+    Notes
+    -----
     Integration over all energies yields unity.
 
     Derivation: The density of states can be expressed as
 
     .. math::
 
         \rho(E) = \frac 1 V \int_{W(k) = E} \frac{\D k}{|\vec \nabla W(k)|},
@@ -56,17 +70,25 @@
             energies[(i + k) % N, (j + k) % N],
             energies[(i + 1) % N, j],
             energies[i, (j + 1) % N],
             ])
         for i in range(N)
         for j in range(N)
         for k in range(2)
-        if comm.rank == ((i * N + j) * 2 + k) % comm.size
         ]
 
+    if minimum is not None:
+        triangles = [v for v in triangles if v[2] >= minimum]
+
+    if maximum is not None:
+        triangles = [v for v in triangles if v[0] <= maximum]
+
+    triangles = [v for n, v in enumerate(triangles)
+        if comm.rank == n % comm.size]
+
     D = np.empty(len(triangles))
 
     def DOS(E):
         for n, (A, B, C) in enumerate(triangles):
             if A < E <= B:
                 if E == B == C:
                     D[n] = 0.5 / (E - A)
@@ -85,17 +107,33 @@
             else:
                 D[n] = 0.0
 
         return comm.allreduce(D.sum()) / N ** 2
 
     return np.vectorize(DOS)
 
-def hexa2F(energies, couplings):
+def hexa2F(energies, couplings, minimum=None, maximum=None):
     r"""Calculate :math:`\alpha^2 F` from energies and coupling.
 
+    Parameters
+    ----------
+    energies : ndarray
+        Energies on triangular mesh.
+    couplings : ndarray
+        Couplings on triangular mesh.
+    minimum, maximum : float, optional
+        Energy window of interest (for efficiency).
+
+    Returns
+    -------
+    function
+        :math:`\alpha^2 F` as a function of energy.
+
+    Notes
+    -----
     Integration over all energies yields the arithmetic mean of the coupling.
 
     Note that it may be more convenient to calculate the mass renormalization
 
     .. math::
         \lambda_n = \int_0^\infty \D \omega
             \frac{2 \omega \alpha^2 F(\omega)}
@@ -105,25 +143,33 @@
                 {\omega_{\vec q \nu}^2 + \omega_n^2}
 
     directly from energies and couplings, without integrating this function."""
 
     N, N = energies.shape
 
     triangles = [
-        tuple(zip(*sorted([
+        sorted([
             ((i + k) % N, (j + k) % N),
             ((i + 1) % N, j),
             (i, (j + 1) % N),
-            ], key=lambda x: energies[x])))
+            ], key=lambda x: energies[x])
         for i in range(N)
         for j in range(N)
         for k in range(2)
-        if comm.rank == ((i * N + j) * 2 + k) % comm.size
         ]
 
+    if minimum is not None:
+        triangles = [v for v in triangles if energies[v[2]] >= minimum]
+
+    if maximum is not None:
+        triangles = [v for v in triangles if energies[v[0]] <= maximum]
+
+    triangles = [tuple(zip(*v)) for n, v in enumerate(triangles)
+        if comm.rank == n % comm.size]
+
     triangles = [(energies[v], couplings[v]) for v in triangles]
 
     D = np.empty(len(triangles))
 
     def a2F(E):
         for n, ((A, B, C), (a, b, c)) in enumerate(triangles):
             if A < E <= B:
```

### Comparing `elphmod-0.8/elphmod/el.py` & `elphmod-0.9/elphmod/el.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (C) 2021 elphmod Developers
+# Copyright (C) 2017-2022 elphmod Developers
 # This program is free software under the terms of the GNU GPLv3 or later.
 
 import numpy as np
 
 from . import bravais, dispersion, misc, MPI, occupations
 comm = MPI.comm
 info = MPI.info
@@ -79,14 +79,24 @@
         # self.data[self.R == R - R', a, b] = <R' a|H|R b> = <R b|H|R' a>
 
         # Compare this convention [doi:10.26092/elib/250, Eq. 2.35a]:
         # t(R - R', a, b) = <R a|H|R' b> = <R' b|H|R a>
 
         return np.einsum('Rab,R->ab', self.data, np.exp(1j * self.R.dot(k)))
 
+    def t(self, R1=0, R2=0, R3=0):
+        """Get on-site or hopping energy for arbitrary lattice vector."""
+
+        index = misc.vector_index(self.R, (R1, R2, R3))
+
+        if index is None:
+            return np.zeros_like(self.data[0])
+        else:
+            return self.data[index]
+
     def __init__(self, seedname=None, divide_ndegen=True, read_xsf=False,
             normalize_wf=False, buffer_wf=False, check_ortho=False,
             shared_memory=False):
 
         if seedname is None:
             return
 
@@ -131,36 +141,28 @@
                 self.data = np.empty((count, self.size, self.size),
                     dtype=complex)
 
             comm.Bcast(self.R)
             comm.Bcast(self.data)
 
         if read_xsf:
-            r0, a, self.atom_order, self.tau, shape = misc.read_xsf(
-                '%s_%05d.xsf' % (seedname, 1), only_header=True)
-
-            self.dV = abs(np.dot(np.cross(a[0], a[1]), a[2])) / np.prod(shape)
-
             if buffer_wf:
                 self.W = MPI.load('%s_wf.npy' % seedname, shared_memory)
                 self.r = MPI.load('%s_xyz.npy' % seedname, shared_memory)
 
-            if not buffer_wf or self.W.size == 0 or self.r.size == 0:
-                node, images, self.r = MPI.shared_array(shape + (3,),
-                    shared_memory=shared_memory)
+            read_buffer = buffer_wf and self.W.size and self.r.size
 
-                if comm.rank == 0:
-                    axes = [np.linspace(0.0, 1.0, num) for num in shape]
-                    axes = np.meshgrid(*axes, indexing='ij')
-                    self.r[...] = r0 + np.einsum('nijk,nx->ijkx', axes, a)
+            r0, a, self.atom_order, self.tau, shape = misc.read_xsf(
+                '%s_head.xsf' % seedname if read_buffer else
+                '%s_%05d.xsf' % (seedname, 1), only_header=True)
 
-                if node.rank == 0:
-                    images.Bcast(self.r)
+            self.dV = abs(np.dot(np.cross(a[0], a[1]), a[2])) / np.prod(shape)
 
-                comm.Barrier()
+            if not read_buffer:
+                self.r = misc.real_space_grid(shape, r0, a, shared_memory)
 
                 sizes, bounds = MPI.distribute(self.size, bounds=True)
 
                 my_W = np.empty((sizes[comm.rank],) + shape)
                 node, images, self.W = MPI.shared_array((self.size,) + shape,
                     shared_memory=shared_memory)
 
@@ -177,14 +179,17 @@
 
                 if node.rank == 0:
                     images.Bcast(self.W)
 
                 comm.Barrier()
 
                 if buffer_wf and comm.rank == 0:
+                    misc.write_xsf('%s_head.xsf' % seedname, r0, a,
+                        self.atom_order, self.tau, shape, only_header=True)
+
                     np.save('%s_wf.npy' % seedname, self.W)
                     np.save('%s_xyz.npy' % seedname, self.r)
 
             if check_ortho:
                 info('Check if Wannier functions are orthogonal:')
                 for m in range(self.size):
                     for n in range(self.size):
@@ -371,27 +376,26 @@
 
         old_R = set(range(len(self.R)))
         new_R = []
         new_t = []
 
         for i in range(len(self.R)):
             R = self.R[i] + S
-            match = np.all(self.R == R, axis=1)
+            j = misc.vector_index(self.R, R)
 
-            if np.any(match):
-                j = np.argmax(match)
-                old_R.remove(j)
-                data[j, :, s] = self.data[i, :, s]
-                data[j, s, s] = self.data[j, s, s]
-            else:
+            if j is None:
                 t = np.zeros((self.size, self.size), dtype=complex)
                 t[:, s] = self.data[i, :, s]
                 t[s, s] = 0.0
                 new_R.append(R)
                 new_t.append(t)
+            else:
+                old_R.remove(j)
+                data[j, :, s] = self.data[i, :, s]
+                data[j, s, s] = self.data[j, s, s]
 
         for j in old_R:
             data[j, :, s] = 0.0
             data[j, s, s] = self.data[j, s, s]
 
         self.R = np.concatenate((self.R, new_R))
         self.data = np.concatenate((data, new_t))
@@ -1010,15 +1014,15 @@
 
         eig[int(bandI) - 1, int(kI) - 1] = np.real(eigI)
 
     f.close()
 
     return eig
 
-def eband_from_qe_pwo(pw_scf_out):
+def eband_from_qe_pwo(pw_scf_out, subset=None):
     """Calculate ``eband`` part of one-electron energy.
 
     The 'one-electron contribution' energy in the Quantum ESPRESSO PWscf output
     is a sum ``eband + deband``. Here, we can calculate the ``eband`` part.
 
     To compare it with the Quantum ESPRESSO result, you need to modify
     the ``SUBROUTINE print_energies ( printout )`` from *electrons.f90*.
@@ -1046,14 +1050,17 @@
 
     At some point, we should add the ``deband`` routine as well...
 
     Parameters
     ----------
     pw_scf_out : str
         The name of the output file (typically 'pw.out').
+    subset : list or array
+        List of indices to pick only a subset of the bands
+        for the integration
 
     Returns
     -------
     eband : float
         The band energy.
     """
     f = open(pw_scf_out, 'r')
@@ -1063,19 +1070,17 @@
     # read number of k points and smearing:
 
     for ii in np.arange(len(lines)):
         if lines[ii].find('     number of k points=') == 0:
 
             line_index = ii
 
-    (number, of, k, pointsequal, N_k, fermd, smearing_s, width, ryequal,
-        smearing) = lines[line_index].split()
-
-    N_k = int(N_k)
-    kT = float(smearing)
+    smearing_line = lines[line_index].split()
+    N_k = int(smearing_line[4])
+    kT = float(smearing_line[9])
 
     k_Points = np.empty([N_k, 4])
 
     for ii in np.arange(N_k):
         (kb, einsb, eq, bra, kx, ky, kz, wk_s, eq2,
             wk) = lines[line_index + 2 + ii].split()
 
@@ -1096,44 +1101,52 @@
         if lines[ii].find('     number of Kohn-Sham') == 0:
             KS_index = ii
 
     number, of, KS_s, states, N_states = lines[KS_index].split()
 
     N_states = int(N_states)
 
-    # read all Energies for all the different k points and Kohn-Sham States:
+    # read all energies for all the different k points and Kohn-Sham States:
 
     for ii in np.arange(len(lines)):
         if lines[ii].find('     End of') == 0:
-
             state_start_index = ii + 4
 
-    Energies = []
-    k_weights = []
+    energies = np.zeros((N_k, N_states))
 
-    print('Number of k Points: ', N_k)
+    # the states are written in columns of size 8
+    # with divmod we check how many rows we have
+    state_lines = divmod(N_states, 8)[0]
+    if divmod(N_states, 8)[1] != 0:
+        state_lines += 1
+
+    for ik in np.arange(N_k):
+        energies_per_k = []
+        for istate in range(state_lines):
+            energies_per_k.extend(lines[state_start_index
+                + istate + (state_lines + 3) * ik].split())
 
-    for jj in np.arange(N_k):
-        for ii in np.arange(3):
-
-            List = lines[jj * (3 + 3) + state_start_index + ii].split()
-
-            for ii in np.arange(len(List)):
-                Energies.append(float(List[ii]))
-                k_weights.append(k_Points[jj, 3])
+        energies[ik] = np.array(energies_per_k)
 
     kT *= misc.Ry
 
-    eF = read_Fermi_level(pw_scf_out)
+    mu = read_Fermi_level(pw_scf_out)
 
-    eband = np.zeros(len(Energies))
+    eband = np.zeros(energies.shape)
 
-    for ii in np.arange(len(Energies)):
-        eband[ii] = (Energies[ii] * k_weights[ii]
-            * occupations.fermi_dirac((Energies[ii] - eF) / kT))
+    if subset == None:
+        for ik in range(N_k):
+            for iband in range(N_states):
+                eband[ik, iband] = (energies[ik, iband] * k_Points[ik, 3]
+                    * occupations.fermi_dirac((energies[ik, iband] - mu) / kT))
+    else:
+        for ik in range(N_k):
+            for iband in subset:
+                eband[ik, iband] = (energies[ik, iband] * k_Points[ik, 3]
+                    * occupations.fermi_dirac((energies[ik, iband] - mu) / kT))
 
     eband = eband.sum() / misc.Ry
 
     return eband
 
 def read_decayH(file):
     """Read *decay.H* output from EPW.
@@ -1211,7 +1224,65 @@
             distance[xi, :] = el.R[ii][xi] * bravais_vectors[xi, :]
         distance = distance.sum(axis=0)
 
         R[ii] = np.linalg.norm(distance)
         H[ii] = np.max(abs(el.data[ii])) / misc.Ry
 
     return R, H
+
+def read_energy_contributions_scf_out(filename):
+    """Read energy contributions to the total energy
+    from Quantum ESPRESSO's scf output file.
+
+    Parameters
+    ----------
+    filename : str
+        scf output file name.
+
+    Returns
+    -------
+    dict
+        energy contributions.
+    """
+
+    if comm.rank == 0:
+        energies = dict()
+
+        with open(filename) as lines:
+            for line in lines:
+                words = [word
+                    for column in line.split()
+                    for word in column.split('=') if word]
+
+                if not words:
+                    continue
+
+                key = words[0].lower()
+
+                if key in 'sum bands':
+                    if words[0] == 'sum':
+                        energies['sum bands'] = words[2]
+                elif key in 'one-electron contribution':
+                    if words[0] == 'one-electron':
+                        energies[key] = words[2]
+                elif key in 'hartree contribution':
+                    if words[0] == 'hartree':
+                        energies[key] = words[2]
+                elif key in 'xc contribution':
+                    if words[0] == 'xc':
+                        energies[key] = words[2]
+                elif key in 'ewald contribution':
+                    if words[0] == 'ewald':
+                        energies[key] = words[2]
+                elif key in 'smearing contrib.':
+                    if words[0] == 'smearing':
+                        energies[key] = words[3]
+                elif key in '!':
+                    if words[0] == '!':
+                        energies['total'] = words[3]
+
+    else:
+        energies = None
+
+    energies = comm.bcast(energies)
+
+    return energies
```

### Comparing `elphmod-0.8/elphmod/eliashberg.py` & `elphmod-0.9/elphmod/eliashberg.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (C) 2021 elphmod Developers
+# Copyright (C) 2017-2022 elphmod Developers
 # This program is free software under the terms of the GNU GPLv3 or later.
 
 import numpy as np
 
 from . import bravais, dos, occupations
 
 def Tc(lamda, wlog, mustar=0.1):
```

### Comparing `elphmod-0.8/elphmod/elph.py` & `elphmod-0.9/elphmod/elph.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (C) 2021 elphmod Developers
+# Copyright (C) 2017-2022 elphmod Developers
 # This program is free software under the terms of the GNU GPLv3 or later.
 
 # Some routines in this file follow wan2bloch.f90 of EPW v5.3.1.
 # Copyright (C) 2010-2016 S. Ponce', R. Margine, C. Verdi, F. Giustino
 
 import numpy as np
 
@@ -155,14 +155,25 @@
                 g = np.einsum('xab,xu->uab', g, uq)
 
         if broadcast:
             comm.Bcast(g)
 
         return g
 
+    def gR(self, Rq1=0, Rq2=0, Rq3=0, Rk1=0, Rk2=0, Rk3=0):
+        """Get electron-phonon matrix elements for arbitrary lattice vectors."""
+
+        index_q = misc.vector_index(self.Rq, (Rq1, Rq2, Rq3))
+        index_k = misc.vector_index(self.Rk, (Rk1, Rk2, Rk3))
+
+        if index_q is None or index_k is None:
+            return np.zeros_like(self.data[0, :, 0, :, :])
+        else:
+            return self.data[index_q, :, index_k, :, :]
+
     def __init__(self, epmatwp=None, wigner=None, el=None, ph=None,
             old_ws=False, divide_mass=True, divide_ndegen=True,
             shared_memory=False):
 
         self.el = el
         self.ph = ph
         self.q = None
```

### Comparing `elphmod-0.8/elphmod/misc.py` & `elphmod-0.9/elphmod/misc.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (C) 2021 elphmod Developers
+# Copyright (C) 2017-2022 elphmod Developers
 # This program is free software under the terms of the GNU GPLv3 or later.
 
 import numpy as np
 import sys
 
 from . import __version__, MPI
 comm = MPI.comm
@@ -89,17 +89,41 @@
     for i in range(len(points)):
         for j in range(i + 1, len(points)):
             if np.all(np.absolute(points[j] - points[i]) < eps):
                 groups[np.where(groups == groups[j])] = groups[i]
 
     return [np.where(groups == group)[0] for group in set(groups)]
 
-def read_cube(cube):
-    """Read Gaussian cube file."""
+def read_cube(cube, only_header=False, comm=comm):
+    """Read Gaussian cube file.
 
+    Parameters
+    ----------
+    cube : str
+        Name of Gaussian cube file.
+    only_header : bool, default False
+        Skip reading data?
+
+    Returns
+    -------
+    r0 : ndarray
+        Origin of the data grid.
+    a : ndarray
+        Spanning vectors of the data grid.
+    X : list of str
+        Atomic numbers.
+    tau : ndarray
+        Cartesian atomic coordinates.
+    data : ndarray
+        Data-grid values or, if `only_header`, shape of data grid.
+
+    See Also
+    --------
+    read_xsf : Equivalent function for XCrySDen format.
+    """
     if comm.rank == 0:
         lines = open(cube)
 
         next(lines)
         next(lines)
 
         cols = next(lines).split()
@@ -107,33 +131,39 @@
         r0 = np.array(list(map(float, cols[1:4])))
     else:
         nat = None
 
     nat = comm.bcast(nat)
 
     n = np.empty(3, dtype=int)
+    r0 = np.empty(3, dtype=float)
     a = np.empty((3, 3), dtype=float)
     X = np.empty(nat, dtype=int)
-    r = np.empty((nat, 3), dtype=float)
+    tau = np.empty((nat, 3), dtype=float)
 
     if comm.rank == 0:
         for i in range(3):
             cols = next(lines).split()
             n[i] = int(cols[0])
             a[i] = list(map(float, cols[1:4]))
+            a[i] *= n[i]
 
         for i in range(nat):
             cols = next(lines).split()
             X[i] = int(cols[0])
-            r[i] = list(map(float, cols[1:4]))
+            tau[i] = list(map(float, cols[2:5]))
 
     comm.Bcast(n)
+    comm.Bcast(r0)
     comm.Bcast(a)
     comm.Bcast(X)
-    comm.Bcast(r)
+    comm.Bcast(tau)
+
+    if only_header:
+        return r0, a, X, tau, tuple(n)
 
     if comm.rank == 0:
         data = np.empty(np.prod(n))
 
         i = 0
         for line in lines:
             for number in line.split():
@@ -144,19 +174,44 @@
 
         lines.close()
     else:
         data = np.empty(n, dtype=float)
 
     comm.Bcast(data)
 
-    return a, X, r, data
+    return r0, a, X, tau, data
 
 def read_xsf(xsf, only_header=False, comm=comm):
-    """Read file in XCrySDen format."""
+    """Read file in XCrySDen format.
+
+    Parameters
+    ----------
+    xsf : str
+        Name of XCrySDen file.
+    only_header : bool, default False
+        Skip reading data?
 
+    Returns
+    -------
+    r0 : ndarray
+        Origin of the data grid.
+    a : ndarray
+        Spanning vectors of the data grid.
+    X : list of str
+        Atomic numbers or symbols.
+    tau : ndarray
+        Cartesian atomic coordinates.
+    data : ndarray
+        Data-grid values or, if `only_header`, shape of data grid.
+
+    See Also
+    --------
+    read_cube : Equivalent function for Gaussian cube format.
+    write_xsf : Write file in XCrySDen format.
+    """
     if comm.rank == 0:
         lines = open(xsf)
 
         while next(lines).strip() != 'PRIMCOORD':
             pass
 
         nat = int(next(lines).split()[0])
@@ -165,39 +220,39 @@
 
     nat = comm.bcast(nat)
 
     n = np.empty(3, dtype=int)
     r0 = np.empty(3, dtype=float)
     a = np.empty((3, 3), dtype=float)
     X = ['X'] * nat
-    r = np.empty((nat, 3), dtype=float)
+    tau = np.empty((nat, 3), dtype=float)
 
     if comm.rank == 0:
         for i in range(nat):
             cols = next(lines).split()
             X[i] = cols[0]
-            r[i] = list(map(float, cols[1:4]))
+            tau[i] = list(map(float, cols[1:4]))
 
         while next(lines).strip() != 'BEGIN_DATAGRID_3D_UNKNOWN':
             pass
 
         n[:] = list(map(int, next(lines).split()))
         r0[:] = list(map(float, next(lines).split()))
 
         for i in range(3):
             a[i] = list(map(float, next(lines).split()))
 
     comm.Bcast(n)
     comm.Bcast(r0)
     comm.Bcast(a)
     X = comm.bcast(X)
-    comm.Bcast(r)
+    comm.Bcast(tau)
 
     if only_header:
-        return r0, a, X, r, tuple(n)
+        return r0, a, X, tau, tuple(n)
 
     if comm.rank == 0:
         data = np.empty(np.prod(n))
 
         i = 0
         while i < data.size:
             for number in next(lines).split():
@@ -209,15 +264,103 @@
 
         lines.close()
     else:
         data = np.empty(n, dtype=float)
 
     comm.Bcast(data)
 
-    return r0, a, X, r, data
+    return r0, a, X, tau, data
+
+def write_xsf(xsf, r0, a, X, tau, data, only_header=False, comm=comm):
+    """Write file in XCrySDen format.
+
+    Parameters
+    ----------
+    xsf : str
+        Name of XCrySDen file.
+    r0 : ndarray
+        Origin of the data grid.
+    a : ndarray
+        Spanning vectors of the data grid.
+    X : list of str
+        Atomic numbers or symbols.
+    tau : ndarray
+        Cartesian atomic coordinates.
+    data : ndarray
+        Data-grid values or, if `only_header`, shape of data grid.
+    only_header : bool, default False
+        Skip writing data?
+
+    See Also
+    --------
+    read_xsf : Read file in XCrySDen format.
+    """
+    if comm.rank == 0:
+        n = tuple(data) if only_header else data.shape
+
+        with open(xsf, 'w') as text:
+            text.write('PRIMCOORD\n')
+            text.write('%6d  1\n' % len(X))
+
+            for i in range(len(X)):
+                text.write('%-5s' % X[i])
+                text.write(' %11.7f %11.7f %11.7f\n' % tuple(tau[i]))
+
+            text.write('BEGIN_BLOCK_DATAGRID_3D\n')
+            text.write('3D_field\n')
+            text.write('BEGIN_DATAGRID_3D_UNKNOWN\n')
+            text.write('%6d %5d %5d\n' % tuple(n))
+            text.write('%12.6f %11.6f %11.6f\n' % tuple(r0))
+
+            for i in range(3):
+                text.write('%12.7f %11.7f %11.7f\n' % tuple(a[i]))
+
+            if not only_header:
+                for i, value in enumerate(data.flat, 1):
+                    text.write('%13.5e' % value)
+
+                    if not i % 6 or i == data.size:
+                        text.write('\n')
+
+            text.write('END_DATAGRID_3D\n')
+            text.write('END_BLOCK_DATAGRID_3D\n')
+
+def real_space_grid(shape, r0, a, shared_memory=False):
+    """Sample real-space grid.
+
+    Parameters
+    ----------
+    shape : tuple of int
+        Shape of the 3D real-space grid.
+    r0 : ndarray
+        Origin of the real-space grid.
+    a : ndarray
+        Cartesian spanning vectors of the real-space grid.
+    shared_memory : bool, default False
+        Store real-space grid in shared memory?
+
+    Returns
+    -------
+    ndarray
+        Cartesian coordinates for all grid points.
+    """
+    node, images, r = MPI.shared_array(shape + (3,),
+        shared_memory=shared_memory)
+
+    if comm.rank == 0:
+        axes = [np.linspace(0.0, 1.0, num) for num in shape]
+        axes = np.meshgrid(*axes, indexing='ij')
+        r[...] = r0 + np.einsum('nijk,nx->ijkx', axes, a)
+
+    if node.rank == 0:
+        images.Bcast(r)
+
+    comm.Barrier()
+
+    return r
 
 def split(expr, sd=',', od='{', cd='}'):
     """Split expression with separators and brackets using distributive law.
 
     Parameters
     ----------
     expr : str
@@ -258,7 +401,29 @@
             for y in groups[int(match.group(2))].split(sd):
                 for z in factorize(match.group(1) + y.strip() + match.group(3)):
                     yield z
         else:
             yield x
 
     return factorize(expr)
+
+def vector_index(vectors, vector):
+    """Find index of vector in list of vectors.
+
+    Parameters
+    ----------
+    vectors : ndarray
+        List of vectors.
+    vector : ndarray
+        Vector.
+
+    Returns
+    -------
+    int
+        Index of vector in list of vectors.
+    """
+    match = np.all(vectors == vector, axis=1)
+
+    if np.any(match):
+        return np.argmax(match)
+    else:
+        return None
```

### Comparing `elphmod-0.8/elphmod/occupations.py` & `elphmod-0.9/elphmod/occupations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (C) 2021 elphmod Developers
+# Copyright (C) 2017-2022 elphmod Developers
 # This program is free software under the terms of the GNU GPLv3 or later.
 
 import math
 import numpy as np
 import sys
 
 xmax = 709.0 # approx. log([max. double] / 2 - 1)
```

### Comparing `elphmod-0.8/elphmod/ph.py` & `elphmod-0.9/elphmod/ph.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (C) 2021 elphmod Developers
+# Copyright (C) 2017-2022 elphmod Developers
 # This program is free software under the terms of the GNU GPLv3 or later.
 
 import numpy as np
 
 from . import bravais, misc, MPI
 comm = MPI.comm
 
@@ -100,14 +100,24 @@
         self.size = self.data.shape[1]
         self.nat = self.size // 3
 
         if apply_asr or apply_rsr:
             sum_rule_correction(self, asr=apply_asr, rsr=apply_rsr,
                 divide_mass=divide_mass)
 
+    def C(self, R1=0, R2=0, R3=0):
+        """Get interatomic force constants for arbitrary lattice vector."""
+
+        index = misc.vector_index(self.R, (R1, R2, R3))
+
+        if index is None:
+            return np.zeros_like(self.data[0])
+        else:
+            return self.data[index]
+
     def supercell(self, N1=1, N2=1, N3=1):
         """Map mass-spring model onto supercell.
 
         Parameters
         ----------
         N1, N2, N3 : tuple of int or int, default 1
             Supercell lattice vectors in units of primitive lattice vectors.
@@ -305,27 +315,26 @@
 
         old_R = set(range(len(self.R)))
         new_R = []
         new_C = []
 
         for i in range(len(self.R)):
             R = self.R[i] + S
-            match = np.all(self.R == R, axis=1)
+            j = misc.vector_index(self.R, R)
 
-            if np.any(match):
-                j = np.argmax(match)
-                old_R.remove(j)
-                data[j, s, :, :, :] = self.data[i, s, :, :, :]
-                data[j, s, :, s, :] = self.data[j, s, :, s, :]
-            else:
+            if j is None:
                 C = np.zeros((self.nat, 3, self.nat, 3))
                 C[s, :, :, :] = self.data[i, s, :, :, :]
                 C[s, :, s, :] = 0.0
                 new_R.append(R)
                 new_C.append(C)
+            else:
+                old_R.remove(j)
+                data[j, s, :, :, :] = self.data[i, s, :, :, :]
+                data[j, s, :, s, :] = self.data[j, s, :, s, :]
 
         for j in old_R:
             data[j, s, :, :, :] = 0.0
             data[j, s, :, s, :] = self.data[j, s, :, s, :]
 
         self.R = np.concatenate((self.R, new_R))
         self.data = np.concatenate((data, new_C))
@@ -856,15 +865,16 @@
                 L = T = (L + T) / 2
 
             mode[n, band, :] = [L, T, Z]
 
     return mode
 
 def q2r(ph, D_irr=None, q_irr=None, nq=None, D_full=None, angle=60,
-        apply_asr=False, apply_asr_simple=False, apply_rsr=False):
+        apply_asr=False, apply_asr_simple=False, apply_rsr=False,
+        divide_mass=True, divide_ndegen=True):
     """Interpolate dynamical matrices given for irreducible wedge of q points.
 
     This function replaces `interpolate_dynamical_matrices`, which depends on
     Quantum ESPRESSO. For 2D lattices, it is sufficient to provide dynamical
     matrices `D_irr` for the irreducible q points `q_irr`. Here, for the square
     lattice, the rotation symmetry (90 degrees) is currently disabled! In turn,
     for 1D and 2D lattices, dynamical matrices `D_full` on the complete uniform
@@ -889,14 +899,20 @@
     apply_asr : bool
         Enforce acoustic sum rule by overwriting self force constants?
     apply_asr_simple : bool
         Apply simple acoustic sum rule correction to force constants? This sets
         the self force constant to minus the sum of all other force constants.
     apply_rsr : bool
         Enforce rotation sum rule by overwriting self force constants?
+    divide_mass : bool
+        Divide force constants by atomic masses?
+    divide_ndegen : bool
+        Divide force constants by degeneracy of Wigner-Seitz point? Only
+        ``True`` yields correct phonons. ``False`` should only be used for
+        debugging.
     """
     if D_full is None:
         D_full = np.empty((nq, nq, ph.size, ph.size), dtype=complex)
 
         def rotation(phi, n=1):
             block = np.array([
                 [np.cos(phi), -np.sin(phi), 0],
@@ -967,15 +983,16 @@
     for na in range(ph.nat):
         phid[na, :] *= np.sqrt(ph.M[na])
         phid[:, na] *= np.sqrt(ph.M[na])
 
     if apply_asr_simple:
         asr(phid)
 
-    ph.R, ph.data = short_range_model(phid, ph.M, ph.a, ph.r)
+    ph.R, ph.data = short_range_model(phid, ph.M, ph.a, ph.r,
+        divide_mass=divide_mass, divide_ndegen=divide_ndegen)
 
     if apply_asr or apply_rsr:
         sum_rule_correction(ph, asr=apply_asr, rsr=apply_rsr)
 
 def interpolate_dynamical_matrices(D, q, nq, fildyn_template, fildyn, flfrc,
         angle=120, write_fildyn0=True, apply_asr=False, apply_asr_simple=False,
         apply_rsr=False, qe_prefix='', clean=False):
```

### Comparing `elphmod-0.8/elphmod/plot.py` & `elphmod-0.9/elphmod/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (C) 2021 elphmod Developers
+# Copyright (C) 2017-2022 elphmod Developers
 # This program is free software under the terms of the GNU GPLv3 or later.
 
 import numpy as np
 
 from . import bravais, MPI, misc
 comm = MPI.comm
```

### Comparing `elphmod-0.8/elphmod.egg-info/PKG-INFO` & `elphmod-0.9/elphmod.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elphmod
-Version: 0.8
+Version: 0.9
 Summary: Modules to handle electron-phonon models
 Home-page: https://github.com/janberges/elphmod
 Author: elphmod Developers
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
```

### Comparing `elphmod-0.8/elphmod.egg-info/SOURCES.txt` & `elphmod-0.9/elphmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elphmod-0.8/patches/qe-6.3-backports.patch` & `elphmod-0.9/patches/qe-6.3-backports.patch`

 * *Files identical despite different names*

### Comparing `elphmod-0.8/patches/qe-6.7MaX-Release.patch` & `elphmod-0.9/patches/qe-6.7MaX-Release.patch`

 * *Files identical despite different names*

### Comparing `elphmod-0.8/patches/qe-6.8.patch` & `elphmod-0.9/patches/qe-6.8.patch`

 * *Files identical despite different names*

### Comparing `elphmod-0.8/setup.cfg` & `elphmod-0.9/setup.cfg`

 * *Files identical despite different names*

