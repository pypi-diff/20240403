# Comparing `tmp/upc_pymotion-0.1.3.tar.gz` & `tmp/upc_pymotion-0.1.4.tar.gz`

## Comparing `upc_pymotion-0.1.3.tar` & `upc_pymotion-0.1.4.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.3/pymotion/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.3/pymotion/io/__init__.py
--rw-r--r--   0        0        0    16589 2020-02-02 00:00:00.000000 upc_pymotion-0.1.3/pymotion/io/bvh.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.3/pymotion/ops/__init__.py
--rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 upc_pymotion-0.1.3/pymotion/ops/forward_kinematics.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 upc_pymotion-0.1.3/pymotion/ops/forward_kinematics_torch.py
--rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 upc_pymotion-0.1.3/pymotion/ops/skeleton.py
--rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 upc_pymotion-0.1.3/pymotion/ops/skeleton_torch.py
--rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 upc_pymotion-0.1.3/pymotion/ops/time.py
--rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 upc_pymotion-0.1.3/pymotion/ops/time_torch.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 upc_pymotion-0.1.3/pymotion/render/__init__.py
--rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 upc_pymotion-0.1.3/pymotion/render/blender.py
--rw-r--r--   0        0        0    19647 2020-02-02 00:00:00.000000 upc_pymotion-0.1.3/pymotion/render/viewer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.3/pymotion/rotations/__init__.py
--rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 upc_pymotion-0.1.3/pymotion/rotations/dual_quat.py
--rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 upc_pymotion-0.1.3/pymotion/rotations/dual_quat_torch.py
--rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 upc_pymotion-0.1.3/pymotion/rotations/ortho6d.py
--rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 upc_pymotion-0.1.3/pymotion/rotations/ortho6d_torch.py
--rw-r--r--   0        0        0    14671 2020-02-02 00:00:00.000000 upc_pymotion-0.1.3/pymotion/rotations/quat.py
--rw-r--r--   0        0        0    15673 2020-02-02 00:00:00.000000 upc_pymotion-0.1.3/pymotion/rotations/quat_torch.py
--rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 upc_pymotion-0.1.3/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 upc_pymotion-0.1.3/LICENSE
--rw-r--r--   0        0        0     8986 2020-02-02 00:00:00.000000 upc_pymotion-0.1.3/README.md
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 upc_pymotion-0.1.3/pyproject.toml
--rw-r--r--   0        0        0    11177 2020-02-02 00:00:00.000000 upc_pymotion-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.4/pymotion/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.4/pymotion/io/__init__.py
+-rw-r--r--   0        0        0    16589 2020-02-02 00:00:00.000000 upc_pymotion-0.1.4/pymotion/io/bvh.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.4/pymotion/ops/__init__.py
+-rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 upc_pymotion-0.1.4/pymotion/ops/center_of_mass.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 upc_pymotion-0.1.4/pymotion/ops/center_of_mass_torch.py
+-rw-r--r--   0        0        0     1826 2020-02-02 00:00:00.000000 upc_pymotion-0.1.4/pymotion/ops/forward_kinematics.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 upc_pymotion-0.1.4/pymotion/ops/forward_kinematics_torch.py
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 upc_pymotion-0.1.4/pymotion/ops/skeleton.py
+-rw-r--r--   0        0        0     3382 2020-02-02 00:00:00.000000 upc_pymotion-0.1.4/pymotion/ops/skeleton_torch.py
+-rw-r--r--   0        0        0     2289 2020-02-02 00:00:00.000000 upc_pymotion-0.1.4/pymotion/ops/time.py
+-rw-r--r--   0        0        0     2516 2020-02-02 00:00:00.000000 upc_pymotion-0.1.4/pymotion/ops/time_torch.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 upc_pymotion-0.1.4/pymotion/render/__init__.py
+-rw-r--r--   0        0        0     2537 2020-02-02 00:00:00.000000 upc_pymotion-0.1.4/pymotion/render/blender.py
+-rw-r--r--   0        0        0    19647 2020-02-02 00:00:00.000000 upc_pymotion-0.1.4/pymotion/render/viewer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 upc_pymotion-0.1.4/pymotion/rotations/__init__.py
+-rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 upc_pymotion-0.1.4/pymotion/rotations/dual_quat.py
+-rw-r--r--   0        0        0     5759 2020-02-02 00:00:00.000000 upc_pymotion-0.1.4/pymotion/rotations/dual_quat_torch.py
+-rw-r--r--   0        0        0     3006 2020-02-02 00:00:00.000000 upc_pymotion-0.1.4/pymotion/rotations/ortho6d.py
+-rw-r--r--   0        0        0     3095 2020-02-02 00:00:00.000000 upc_pymotion-0.1.4/pymotion/rotations/ortho6d_torch.py
+-rw-r--r--   0        0        0    14671 2020-02-02 00:00:00.000000 upc_pymotion-0.1.4/pymotion/rotations/quat.py
+-rw-r--r--   0        0        0    15451 2020-02-02 00:00:00.000000 upc_pymotion-0.1.4/pymotion/rotations/quat_torch.py
+-rw-r--r--   0        0        0     3787 2020-02-02 00:00:00.000000 upc_pymotion-0.1.4/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 upc_pymotion-0.1.4/LICENSE
+-rw-r--r--   0        0        0     8986 2020-02-02 00:00:00.000000 upc_pymotion-0.1.4/README.md
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 upc_pymotion-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0    11177 2020-02-02 00:00:00.000000 upc_pymotion-0.1.4/PKG-INFO
```

### Comparing `upc_pymotion-0.1.3/pymotion/io/bvh.py` & `upc_pymotion-0.1.4/pymotion/io/bvh.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.3/pymotion/ops/forward_kinematics.py` & `upc_pymotion-0.1.4/pymotion/ops/forward_kinematics.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.3/pymotion/ops/forward_kinematics_torch.py` & `upc_pymotion-0.1.4/pymotion/ops/forward_kinematics_torch.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.3/pymotion/ops/skeleton.py` & `upc_pymotion-0.1.4/pymotion/ops/skeleton.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.3/pymotion/ops/skeleton_torch.py` & `upc_pymotion-0.1.4/pymotion/ops/skeleton_torch.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.3/pymotion/ops/time.py` & `upc_pymotion-0.1.4/pymotion/ops/time.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.3/pymotion/ops/time_torch.py` & `upc_pymotion-0.1.4/pymotion/ops/time_torch.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.3/pymotion/render/__init__.py` & `upc_pymotion-0.1.4/pymotion/render/__init__.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.3/pymotion/render/blender.py` & `upc_pymotion-0.1.4/pymotion/render/blender.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.3/pymotion/render/viewer.py` & `upc_pymotion-0.1.4/pymotion/render/viewer.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.3/pymotion/rotations/dual_quat.py` & `upc_pymotion-0.1.4/pymotion/rotations/dual_quat.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.3/pymotion/rotations/dual_quat_torch.py` & `upc_pymotion-0.1.4/pymotion/rotations/dual_quat_torch.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.3/pymotion/rotations/ortho6d.py` & `upc_pymotion-0.1.4/pymotion/rotations/ortho6d.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.3/pymotion/rotations/ortho6d_torch.py` & `upc_pymotion-0.1.4/pymotion/rotations/ortho6d_torch.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.3/pymotion/rotations/quat.py` & `upc_pymotion-0.1.4/pymotion/rotations/quat.py`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.3/pymotion/rotations/quat_torch.py` & `upc_pymotion-0.1.4/pymotion/rotations/quat_torch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from __future__ import annotations
 import torch
 import torch.nn.functional as F
 import numpy as np
 
 
 def from_scaled_angle_axis(scaledaxis: torch.Tensor) -> torch.Tensor:
     """
@@ -64,29 +65,23 @@
     axis = {
         "x": np.array([1, 0, 0]),
         "y": np.array([0, 1, 0]),
         "z": np.array([0, 0, 1]),
     }
     q0 = from_angle_axis(
         euler[..., 0:1],
-        torch.from_numpy(
-            np.apply_along_axis(lambda x: axis[x.item()], -1, order[..., 0:1])
-        ).to(euler.device),
+        torch.from_numpy(np.apply_along_axis(lambda x: axis[x.item()], -1, order[..., 0:1])).to(euler.device),
     )
     q1 = from_angle_axis(
         euler[..., 1:2],
-        torch.from_numpy(
-            np.apply_along_axis(lambda x: axis[x.item()], -1, order[..., 1:2])
-        ).to(euler.device),
+        torch.from_numpy(np.apply_along_axis(lambda x: axis[x.item()], -1, order[..., 1:2])).to(euler.device),
     )
     q2 = from_angle_axis(
         euler[..., 2:3],
-        torch.from_numpy(
-            np.apply_along_axis(lambda x: axis[x.item()], -1, order[..., 2:3])
-        ).to(euler.device),
+        torch.from_numpy(np.apply_along_axis(lambda x: axis[x.item()], -1, order[..., 2:3])).to(euler.device),
     )
     return mul(q0, mul(q1, q2))
 
 
 def from_matrix(rotmats: torch.Tensor) -> torch.Tensor:
     """
     Convert rotation matrices to quaternions.
@@ -189,37 +184,25 @@
         "z": 2,
     }
 
     angle_first = 2
     angle_third = 0
 
     i = (
-        torch.from_numpy(
-            np.apply_along_axis(lambda x: aux[x.item()], -1, order[..., 2:3])[
-                ..., np.newaxis
-            ]
-        )
+        torch.from_numpy(np.apply_along_axis(lambda x: aux[x.item()], -1, order[..., 2:3])[..., np.newaxis])
         .to(quaternions.device)
         .type(torch.long)
     )
     j = (
-        torch.from_numpy(
-            np.apply_along_axis(lambda x: aux[x.item()], -1, order[..., 1:2])[
-                ..., np.newaxis
-            ]
-        )
+        torch.from_numpy(np.apply_along_axis(lambda x: aux[x.item()], -1, order[..., 1:2])[..., np.newaxis])
         .to(quaternions.device)
         .type(torch.long)
     )
     k = (
-        torch.from_numpy(
-            np.apply_along_axis(lambda x: aux[x.item()], -1, order[..., 0:1])[
-                ..., np.newaxis
-            ]
-        )
+        torch.from_numpy(np.apply_along_axis(lambda x: aux[x.item()], -1, order[..., 0:1])[..., np.newaxis])
         .to(quaternions.device)
         .type(torch.long)
     )
 
     # check if permutation is even or odd
     sign = (i - j) * (j - k) * (k - i) // 2
 
@@ -234,17 +217,15 @@
     )
     c = torch.take_along_dim(quaternions, j + 1, dim=-1) + quaternions[..., 0:1]
     d = torch.take_along_dim(quaternions, k + 1, dim=-1) * sign - torch.take_along_dim(
         quaternions, i + 1, dim=-1
     )
 
     # compute second angle
-    euler[..., 1:2] = (2 * torch.arctan2(torch.hypot(c, d), torch.hypot(a, b))) - (
-        torch.pi / 2
-    )
+    euler[..., 1:2] = (2 * torch.arctan2(torch.hypot(c, d), torch.hypot(a, b))) - (torch.pi / 2)
 
     # compute first and third angle
     half_sum = torch.arctan2(b, a)
     half_diff = torch.arctan2(d, c)
     euler[..., angle_first : angle_first + 1] = half_sum - half_diff
     euler[..., angle_third : angle_third + 1] = (half_sum + half_diff) * sign
 
@@ -482,17 +463,15 @@
         d1 = torch.sum(-r[i] * r[i - 1], dim=-1)
         # if the distance with the flipped quaternion is smaller, use it
         r[i][d0 < d1] = -r[i][d0 < d1]
     r = r.swapaxes(0, dim)
     return r
 
 
-def slerp(
-    q0: torch.Tensor, q1: torch.Tensor, t: float or torch.Tensor, shortest: bool = True
-) -> torch.Tensor:
+def slerp(q0: torch.Tensor, q1: torch.Tensor, t: float | torch.Tensor, shortest: bool = True) -> torch.Tensor:
     """
     Perform spherical linear interpolation (SLERP) between two unit quaternions.
 
     Parameters
     ----------
     q0 : torch.Tensor[..., [w,x,y,z]]
     q1 : torch.Tensor[..., [w,x,y,z]]
@@ -520,17 +499,15 @@
     dot = torch.clip(dot, -1, 1)
 
     # Compute the quaternion of the angle between the quaternions
     theta_0 = torch.arccos(dot)  # theta_0 = angle between input vectors
     theta = theta_0 * t  # theta = angle between q0 vector and result
 
     q2 = q1 - q0 * dot
-    q2 /= torch.linalg.norm(
-        q2 + 0.000001, dim=-1, keepdim=True
-    )  # {q0, q2} is now an orthonormal basis
+    q2 /= torch.linalg.norm(q2 + 0.000001, dim=-1, keepdim=True)  # {q0, q2} is now an orthonormal basis
 
     return torch.cos(theta) * q0 + torch.sin(theta) * q2
 
 
 def _fast_cross(a: torch.Tensor, b: torch.Tensor) -> torch.Tensor:
     """
     Fast cross of two vectors
```

### Comparing `upc_pymotion-0.1.3/.gitignore` & `upc_pymotion-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.3/LICENSE` & `upc_pymotion-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.3/README.md` & `upc_pymotion-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `upc_pymotion-0.1.3/pyproject.toml` & `upc_pymotion-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [tool.hatch.build]
 include = ["pymotion/*"]
 exclude = ["*test*"]
 
 [project]
 name = "upc-pymotion"
-version = "0.1.3"
+version = "0.1.4"
 description = "A Python library for working with motion data in NumPy or PyTorch."
 readme = "README.md"
 authors = [{ name = "Jose Luis Ponton", email = "jose.luis.ponton@upc.edu" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `upc_pymotion-0.1.3/PKG-INFO` & `upc_pymotion-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: upc-pymotion
-Version: 0.1.3
+Version: 0.1.4
 Summary: A Python library for working with motion data in NumPy or PyTorch.
 Project-URL: Homepage, https://github.com/UPC-ViRVIG/pymotion
 Author-email: Jose Luis Ponton <jose.luis.ponton@upc.edu>
 License: MIT License
         
         Copyright (c) 2024 Jose Luis Ponton
```

