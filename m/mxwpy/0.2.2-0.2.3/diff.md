# Comparing `tmp/mxwpy-0.2.2.tar.gz` & `tmp/mxwpy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxwpy-0.2.2.tar", last modified: Thu Mar 21 02:44:30 2024, max compression
+gzip compressed data, was "mxwpy-0.2.3.tar", last modified: Wed Apr  3 06:51:04 2024, max compression
```

## Comparing `mxwpy-0.2.2.tar` & `mxwpy-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 02:44:30.920524 mxwpy-0.2.2/
--rw-rw-rw-   0        0        0     2511 2024-03-21 02:44:30.919522 mxwpy-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0     1537 2024-03-13 13:23:19.000000 mxwpy-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-21 02:44:30.901605 mxwpy-0.2.2/mxwpy/
--rw-rw-rw-   0        0        0        0 2023-11-10 02:06:30.000000 mxwpy-0.2.2/mxwpy/__init__.py
--rw-rw-rw-   0        0        0     1755 2024-03-15 09:39:53.000000 mxwpy-0.2.2/mxwpy/linalg.py
--rw-rw-rw-   0        0        0    11705 2024-03-16 14:40:08.000000 mxwpy-0.2.2/mxwpy/npde.py
--rw-rw-rw-   0        0        0    13225 2024-03-20 14:05:20.000000 mxwpy-0.2.2/mxwpy/spectral.py
--rw-rw-rw-   0        0        0     6621 2024-03-20 02:37:42.000000 mxwpy-0.2.2/mxwpy/tools.py
-drwxrwxrwx   0        0        0        0 2024-03-21 02:44:30.918522 mxwpy-0.2.2/mxwpy.egg-info/
--rw-rw-rw-   0        0        0     2511 2024-03-21 02:44:30.000000 mxwpy-0.2.2/mxwpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      243 2024-03-21 02:44:30.000000 mxwpy-0.2.2/mxwpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 02:44:30.000000 mxwpy-0.2.2/mxwpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2024-03-21 02:44:30.000000 mxwpy-0.2.2/mxwpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-21 02:44:30.000000 mxwpy-0.2.2/mxwpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-21 02:44:30.920524 mxwpy-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0     1644 2024-03-21 02:44:18.000000 mxwpy-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:51:04.934108 mxwpy-0.2.3/
+-rw-rw-rw-   0        0        0     1091 2024-04-03 06:49:12.000000 mxwpy-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0     2651 2024-04-03 06:51:04.932686 mxwpy-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1654 2024-04-03 06:39:13.000000 mxwpy-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 06:51:04.921782 mxwpy-0.2.3/mxwpy/
+-rw-rw-rw-   0        0        0        0 2023-11-10 02:06:30.000000 mxwpy-0.2.3/mxwpy/__init__.py
+-rw-rw-rw-   0        0        0     1755 2024-03-15 09:39:53.000000 mxwpy-0.2.3/mxwpy/linalg.py
+-rw-rw-rw-   0        0        0    12133 2024-04-03 03:41:58.000000 mxwpy-0.2.3/mxwpy/npde.py
+-rw-rw-rw-   0        0        0    16254 2024-04-03 05:24:24.000000 mxwpy-0.2.3/mxwpy/spectral.py
+-rw-rw-rw-   0        0        0     6621 2024-03-20 02:37:42.000000 mxwpy-0.2.3/mxwpy/tools.py
+drwxrwxrwx   0        0        0        0 2024-04-03 06:51:04.932686 mxwpy-0.2.3/mxwpy.egg-info/
+-rw-rw-rw-   0        0        0     2651 2024-04-03 06:51:04.000000 mxwpy-0.2.3/mxwpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2024-04-03 06:51:04.000000 mxwpy-0.2.3/mxwpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 06:51:04.000000 mxwpy-0.2.3/mxwpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2024-04-03 06:51:04.000000 mxwpy-0.2.3/mxwpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-03 06:51:04.000000 mxwpy-0.2.3/mxwpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 06:51:04.934108 mxwpy-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0     1644 2024-04-03 06:50:54.000000 mxwpy-0.2.3/setup.py
```

### Comparing `mxwpy-0.2.2/PKG-INFO` & `mxwpy-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxwpy
-Version: 0.2.2
+Version: 0.2.3
 Summary: efficient numerical schemes
 Home-page: https://github.com/mxweng/mxwpy
 Author: MXWeng
 Author-email: 2431141461@qq.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,37 +14,40 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: GPUtil
 Requires-Dist: IPython
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: psutil
 Requires-Dist: scipy
 Requires-Dist: sympy
 
-# mxwpy
-mxwpy is an under development Python library that provides efficient numerical schemes and some useful tools. It consists of the following modules:
+# SpecNN4PDE
+SpecNN4PDE is an under development Python library for solving partial differential equations using spectral methods and neural networks. It consists of the following modules:
 
-- `spectral`: Provides functions for working with spectral methods, specifically for evaluating orthonormal Jacobi polynomials, as described in the book [Spectral Methods: Algorithms, Analysis and Applications](https://link.springer.com/book/10.1007/978-3-540-71041-7) by Shen, Tang, and Wang.
+- `spectral`: Provides functions for working with spectral methods as described in the book [Spectral Methods: Algorithms, Analysis and Applications](https://link.springer.com/book/10.1007/978-3-540-71041-7) by Shen, Tang, and Wang.
 - `linalg`: This module primarily focuses on numerical algebra methods.
-- `tools`: A collection of utility functions for system and package information retrieval, time measurement, and other potential functionalities to be added in the future.
-- `npde`: Hosts functions for handling numerical partial differential equations.
+- `tools`: A collection of utility functions for system and package information retrieval, time measurement, etc.
+- `npde`: Functions for solving partial differential equations, e.g., calculating the multivariate derivatives.
+
+This project is still in the early stages of development, and the API is subject to change. The library is designed to be used in research and educational settings.
 
 ## Dependencies
 
 When you install this library using pip, most dependencies will be automatically handled. However, please note that the `npde` module requires PyTorch, which needs to be installed separately.
 
 You can install PyTorch by following the instructions on the [official PyTorch website](https://pytorch.org/get-started/locally/). Please ensure that you select the correct installation command based on your operating system, package manager, Python version, and the specifications of your CUDA toolkit if you are planning to use PyTorch with GPU support.
 
 If you are not planning to use the `npde` module, you do not need to install PyTorch.
 
 ## Installation
 
 To install this library, you can use pip:
 
 ```bash
-pip install mxwpy
+pip install specnn4pde
```

### Comparing `mxwpy-0.2.2/README.md` & `mxwpy-0.2.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-# mxwpy
-mxwpy is an under development Python library that provides efficient numerical schemes and some useful tools. It consists of the following modules:
+# SpecNN4PDE
+SpecNN4PDE is an under development Python library for solving partial differential equations using spectral methods and neural networks. It consists of the following modules:
 
-- `spectral`: Provides functions for working with spectral methods, specifically for evaluating orthonormal Jacobi polynomials, as described in the book [Spectral Methods: Algorithms, Analysis and Applications](https://link.springer.com/book/10.1007/978-3-540-71041-7) by Shen, Tang, and Wang.
+- `spectral`: Provides functions for working with spectral methods as described in the book [Spectral Methods: Algorithms, Analysis and Applications](https://link.springer.com/book/10.1007/978-3-540-71041-7) by Shen, Tang, and Wang.
 - `linalg`: This module primarily focuses on numerical algebra methods.
-- `tools`: A collection of utility functions for system and package information retrieval, time measurement, and other potential functionalities to be added in the future.
-- `npde`: Hosts functions for handling numerical partial differential equations.
+- `tools`: A collection of utility functions for system and package information retrieval, time measurement, etc.
+- `npde`: Functions for solving partial differential equations, e.g., calculating the multivariate derivatives.
+
+This project is still in the early stages of development, and the API is subject to change. The library is designed to be used in research and educational settings.
 
 ## Dependencies
 
 When you install this library using pip, most dependencies will be automatically handled. However, please note that the `npde` module requires PyTorch, which needs to be installed separately.
 
 You can install PyTorch by following the instructions on the [official PyTorch website](https://pytorch.org/get-started/locally/). Please ensure that you select the correct installation command based on your operating system, package manager, Python version, and the specifications of your CUDA toolkit if you are planning to use PyTorch with GPU support.
 
 If you are not planning to use the `npde` module, you do not need to install PyTorch.
 
 ## Installation
 
 To install this library, you can use pip:
 
 ```bash
-pip install mxwpy
+pip install specnn4pde
```

### Comparing `mxwpy-0.2.2/mxwpy/linalg.py` & `mxwpy-0.2.3/mxwpy/linalg.py`

 * *Files identical despite different names*

### Comparing `mxwpy-0.2.2/mxwpy/npde.py` & `mxwpy-0.2.3/mxwpy/npde.py`

 * *Files 6% similar despite different names*

```diff
@@ -239,28 +239,33 @@
     Co = torch.meshgrid(*inputs, indexing=indexing)
     return torch.cat([c.reshape(-1,1) for c in Co], dim=1)
 
 
 def gen_collo(Domain, grids, temporal = False, corner = True):
     """
     Generate the collocation points for the PDE problem on regular domain.
+    If Domain and grids are provided, the uniform grids will be generated automatically as G.
+    If Domain and grids are not provided, G should be provided.
 
     Parameters
     ----------
-    Domain : list of list
+    Domain : list of list, optional
         The domain of the problem. eg. [[t_min, x1_min, x2_min, ...], [t_max, x1_max, x2_max, ...]]
-    grids : list
+    grids : list, optional
         The number of collocations in each dimension. eg. [N_t, N_x1, N_x2, ...]
     temporal : bool, optional
         If the problem is temporal. The default is False.
     corner : bool, optional
         If the collocation points include the corner points. The default is True.
+    G : list of tensor, optional
+        The tensors in the list are the collocation points in each dimension.
+        If Domain and grids are not provided, G should be provided.
     
     Returns
-    ----------
+    -------
     collo_rs : tensor
         The collocation points in the interior of the domain.
     collo_ic : tensor, optional
         If temporal is set as True. The collocation points on the initial condition.
     collo_bc : tensor
         The collocation points on the boundary condition.
 
@@ -283,22 +288,24 @@
              [2.0000, 0.0000, 1.0000],
              ......
              [1.0000, 1.0000, 4.0000],
              [1.0000, 2.0000, 1.0000],
              [1.0000, 2.0000, 4.0000]]))
     """
 
-    dim = len(Domain[0])
-    if len(grids) != dim:
-        if len(grids) == 1:
-            Warning("The number of grids is set as the same for all dimensions.")
-            grids = grids * dim
-        else:
-            raise ValueError("The length of grids should be equal to the dimension of the domain.")
-    G = [torch.linspace(l, r, n) for l, r, n in zip(*(Domain + [grids]))]
+    if G is None:
+        dim = len(Domain[0])
+        if len(grids) != dim:
+            if len(grids) == 1:
+                Warning("The number of grids is set as the same for all dimensions.")
+                grids = grids * dim
+            else:
+                raise ValueError("The length of grids should be equal to the dimension of the domain.")
+        G = [torch.linspace(l, r, n) for l, r, n in zip(*(Domain + [grids]))]
+    dim = len(G)
     if temporal:
         G_rs = [G[0][1:]] + [G[i][1:-1] for i in range(1, dim)]
         G_ic = [G[0][0]] + G[1:]
         collo_rs = meshgrid_to_matrix(G_rs)
         collo_ic = meshgrid_to_matrix(G_ic)
         collo_bc = []
         for i in range(1, dim):
```

### Comparing `mxwpy-0.2.2/mxwpy/spectral.py` & `mxwpy-0.2.3/mxwpy/spectral.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 __all__ = ['JacobiP', 'Jacobi_Gauss', 'Jacobi_Gauss_Lobatto', 
-           'HermiteP', 'HermiteF', 'Hermite_Gauss', 'mapped_Jacobi_Gauss'
+           'HermiteP', 'HermiteF', 'Hermite_Gauss', 'mapped_Jacobi_Gauss',
+           'glue1D', 'glue_pts_1D',
            ]
 
 """
 spectral.py
 
 This module provides functions for working with spectral methods.
 The implementation is mainly based on the book: 
     Shen, J., Tang, T. & Wang, L.-L. Spectral Methods: Algorithms, 
     Analysis and Applications. vol. 41 (Springer Science & Business 
     Media, 2011).
     https://link.springer.com/book/10.1007/978-3-540-71041-7
 """
 
 import numpy as np
-from scipy.special import roots_hermite
-from scipy.special import gamma
-from scipy.sparse import diags
-from scipy.linalg import eigh
+from scipy.special import roots_hermite, gamma
+from scipy.sparse import diags, eye, lil_matrix, csr_matrix
+from scipy.linalg import eigh, block_diag
 from sympy import symbols, sqrt, atanh, tanh, sinh, log, lambdify, diff
 
 def JacobiP(x, alpha, beta, N):
     """
     This function evaluates the orthonormal Jacobi polynomial of order 
     up to N with parameters alpha and beta at points x.
     
@@ -374,8 +374,91 @@
     map = lambdify((y, s), map_expr, "numpy")
     diff_map = lambdify((y, s), diff_map_expr, "numpy")
 
     D, r, w = Jacobi_Gauss(alpha, beta, N)
     omega = (1 - r)**alpha * (1 + r)**beta
     diff_g = diff_map(r, sf)
     D, r, w = D / diff_g[:, None], map(r, sf), w / omega * diff_g
-    return D, r, w
+    return D, r, w
+
+
+
+
+def glue1D(interval, Ncell, D, r, w, end_pts = False):
+    """
+    Glue the differential matrix D, Gauss points r, and quadrature weights w on each cell together.
+
+    Parameters
+    ----------
+    interval : list or tuple, length 2
+        The left and right edge of the domain.
+    Ncell : int
+        The number of cells.
+    D, r, w : ndarray
+        The differential matrix, Gauss points, and quadrature weights on the reference cell [-1, 1],
+        which can be generated by `spectral.Jacobi_Gauss`, `spectral.Jacobi_Gauss_Lobatto`.
+    end_pts : bool, optional
+        Whether the end points -1, 1 are included in r or not. The default is False.
+        E.g., if `spectral.Jacobi_Gauss_Lobatto` is used, the end points are included in r.
+
+    Returns
+    ----------
+    D, r, w : ndarray
+        The differential matrix D, Gauss points r, and quadrature weights w on the interval.
+        if end_pts is False, shape (Ncell * Np, Ncell * Np), (Ncell * Np,), (Ncell * Np,)
+        if end_pts is True, shape (Ncell * (Np - 1) + 1, Ncell * (Np - 1) + 1), (Ncell * (Np - 1) + 1,), (Ncell * (Np - 1) + 1,)
+    """
+
+    Np = len(r)
+    D, r, w = D.copy(), r.copy(), w.copy()
+    left, right = interval
+    Len = (right - left) / Ncell / 2
+    r = (r + 1) * Len + left
+    r = r[None, :].repeat(Ncell, axis=0)
+    r = r + np.arange(Ncell)[:, None] * Len * 2
+    D_blocks = [D / Len] * Ncell
+    D, r, w = block_diag(*D_blocks), r.reshape(-1), np.tile(w, Ncell) * Len
+    if end_pts:
+        Glue = lil_matrix(np.zeros((Ncell * (Np - 1) + 1, Ncell * Np)))
+        for j in range(Ncell):
+            rowStart, colStart = j * (Np - 1), j * Np
+            Glue[rowStart:rowStart+Np, colStart:colStart+Np] = eye(Np)
+        D, Glue = csr_matrix(D), Glue.tocsr()
+        D = (Glue @ D @ Glue.T).toarray()
+        r = np.delete(r, np.arange(Np-1, len(r)-1, Np))
+        w = Glue @ w
+    return D, r, w
+
+def glue_pts_1D(interval, Ncell, r, end_pts = False):
+    """
+    Glue the points r on each cell together.
+
+    Parameters
+    ----------
+    interval : list or tuple, length 2
+        The left and right edge of the domain.
+    Ncell : int
+        The number of cells.
+    r : ndarray
+        The collocation points on the reference cell [-1, 1],
+    end_pts : bool, optional
+        Whether the end points -1, 1 are included in r or not. The default is False.
+
+    Returns
+    ----------
+    r : ndarray
+        The collocation points r on the interval.
+        if end_pts is False, shape (Ncell * Np,)
+        if end_pts is True, shape (Ncell * (Np - 1) + 1,)
+    """
+
+    Np = len(r)
+    r = r.copy()
+    left, right = interval
+    Len = (right - left) / Ncell / 2
+    r = (r + 1) * Len + left
+    r = r[None, :].repeat(Ncell, axis=0)
+    r = r + np.arange(Ncell)[:, None] * Len * 2
+    r = r.reshape(-1)
+    if end_pts:
+        r = np.delete(r, np.arange(Np-1, len(r)-1, Np))
+    return r
```

### Comparing `mxwpy-0.2.2/mxwpy/tools.py` & `mxwpy-0.2.3/mxwpy/tools.py`

 * *Files identical despite different names*

### Comparing `mxwpy-0.2.2/mxwpy.egg-info/PKG-INFO` & `mxwpy-0.2.3/mxwpy.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxwpy
-Version: 0.2.2
+Version: 0.2.3
 Summary: efficient numerical schemes
 Home-page: https://github.com/mxweng/mxwpy
 Author: MXWeng
 Author-email: 2431141461@qq.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -14,37 +14,40 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: GPUtil
 Requires-Dist: IPython
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: psutil
 Requires-Dist: scipy
 Requires-Dist: sympy
 
-# mxwpy
-mxwpy is an under development Python library that provides efficient numerical schemes and some useful tools. It consists of the following modules:
+# SpecNN4PDE
+SpecNN4PDE is an under development Python library for solving partial differential equations using spectral methods and neural networks. It consists of the following modules:
 
-- `spectral`: Provides functions for working with spectral methods, specifically for evaluating orthonormal Jacobi polynomials, as described in the book [Spectral Methods: Algorithms, Analysis and Applications](https://link.springer.com/book/10.1007/978-3-540-71041-7) by Shen, Tang, and Wang.
+- `spectral`: Provides functions for working with spectral methods as described in the book [Spectral Methods: Algorithms, Analysis and Applications](https://link.springer.com/book/10.1007/978-3-540-71041-7) by Shen, Tang, and Wang.
 - `linalg`: This module primarily focuses on numerical algebra methods.
-- `tools`: A collection of utility functions for system and package information retrieval, time measurement, and other potential functionalities to be added in the future.
-- `npde`: Hosts functions for handling numerical partial differential equations.
+- `tools`: A collection of utility functions for system and package information retrieval, time measurement, etc.
+- `npde`: Functions for solving partial differential equations, e.g., calculating the multivariate derivatives.
+
+This project is still in the early stages of development, and the API is subject to change. The library is designed to be used in research and educational settings.
 
 ## Dependencies
 
 When you install this library using pip, most dependencies will be automatically handled. However, please note that the `npde` module requires PyTorch, which needs to be installed separately.
 
 You can install PyTorch by following the instructions on the [official PyTorch website](https://pytorch.org/get-started/locally/). Please ensure that you select the correct installation command based on your operating system, package manager, Python version, and the specifications of your CUDA toolkit if you are planning to use PyTorch with GPU support.
 
 If you are not planning to use the `npde` module, you do not need to install PyTorch.
 
 ## Installation
 
 To install this library, you can use pip:
 
 ```bash
-pip install mxwpy
+pip install specnn4pde
```

### Comparing `mxwpy-0.2.2/setup.py` & `mxwpy-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from distutils.command import install_data
 from setuptools import setup, find_packages
 
 setup(
     name='mxwpy',  # package name
-    version='0.2.2',  # version
+    version='0.2.3',  # version
     author='MXWeng',  # author name
     author_email='2431141461@qq.com',  # author email
     description='efficient numerical schemes',  # short description
     long_description=open('README.md').read(),  # long description, usually your README
     long_description_content_type='text/markdown',  # format of the long description, 'text/markdown' if it's Markdown
     url='https://github.com/mxweng/mxwpy',  # project homepage
     packages=find_packages(),  # automatically discover all packages
```

