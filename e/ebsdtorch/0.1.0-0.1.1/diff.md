# Comparing `tmp/ebsdtorch-0.1.0.tar.gz` & `tmp/ebsdtorch-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebsdtorch-0.1.0.tar", max compression
+gzip compressed data, was "ebsdtorch-0.1.1.tar", max compression
```

## Comparing `ebsdtorch-0.1.0.tar` & `ebsdtorch-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1070 2024-01-30 12:57:55.423222 ebsdtorch-0.1.0/LICENSE
--rw-r--r--   0        0        0     1942 2024-01-30 12:57:13.263133 ebsdtorch-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-09-11 16:52:02.001783 ebsdtorch-0.1.0/ebsdtorch/__init__.py
--rw-r--r--   0        0        0      218 2024-01-30 12:02:28.600549 ebsdtorch-0.1.0/ebsdtorch/ebsd_dictionary_indexing/__init__.py
--rw-r--r--   0        0        0     4477 2024-01-30 12:01:26.602536 ebsdtorch-0.1.0/ebsdtorch/ebsd_dictionary_indexing/blur_master_pattern_direct.py
--rw-r--r--   0        0        0    10088 2024-01-30 11:41:52.900698 ebsdtorch-0.1.0/ebsdtorch/ebsd_dictionary_indexing/ebsd_di_one_pc_one_phase.py
--rw-r--r--   0        0        0    13737 2024-01-30 11:38:40.130001 ebsdtorch-0.1.0/ebsdtorch/ebsd_dictionary_indexing/ebsd_di_one_pc_one_phase_pca.py
--rw-r--r--   0        0        0     9160 2024-01-30 11:56:48.271540 ebsdtorch-0.1.0/ebsdtorch/ebsd_dictionary_indexing/ebsd_di_spherical_covmat.py
--rw-r--r--   0        0        0     5094 2024-01-09 17:16:06.400640 ebsdtorch-0.1.0/ebsdtorch/ebsd_dictionary_indexing/utils_covariance_matrix.py
--rw-r--r--   0        0        0     8685 2024-01-30 11:57:40.020559 ebsdtorch-0.1.0/ebsdtorch/ebsd_dictionary_indexing/utils_nearest_neighbors.py
--rw-r--r--   0        0        0     1206 2024-01-09 17:15:47.659296 ebsdtorch-0.1.0/ebsdtorch/ebsd_dictionary_indexing/utils_progress_bar.py
--rw-r--r--   0        0        0       42 2024-01-30 11:31:37.461005 ebsdtorch-0.1.0/ebsdtorch/ebsd_high_resolution/__init__.py
--rw-r--r--   0        0        0     6242 2024-01-30 11:57:57.682272 ebsdtorch-0.1.0/ebsdtorch/ebsd_high_resolution/hrebsd_project.py
--rw-r--r--   0        0        0        0 2023-09-08 10:49:41.283732 ebsdtorch-0.1.0/ebsdtorch/patterns/__init__.py
--rw-r--r--   0        0        0    15084 2024-01-05 04:09:20.262954 ebsdtorch-0.1.0/ebsdtorch/patterns/lie_algebra_se3.py
--rw-r--r--   0        0        0     3206 2023-12-21 19:35:49.252383 ebsdtorch-0.1.0/ebsdtorch/patterns/lie_algebra_sim3_with_stretch.py
--rw-r--r--   0        0        0     8235 2024-01-30 11:38:40.534040 ebsdtorch-0.1.0/ebsdtorch/patterns/pattern_projection.py
--rw-r--r--   0        0        0     6958 2024-01-05 04:09:20.322959 ebsdtorch-0.1.0/ebsdtorch/patterns/square_hemisphere_bijection.py
--rw-r--r--   0        0        0        0 2023-09-09 11:06:24.072730 ebsdtorch-0.1.0/ebsdtorch/s2_and_so3/__init__.py
--rw-r--r--   0        0        0    23064 2024-01-30 12:17:06.553703 ebsdtorch-0.1.0/ebsdtorch/s2_and_so3/laue.py
--rw-r--r--   0        0        0    49329 2024-01-05 16:09:49.263451 ebsdtorch-0.1.0/ebsdtorch/s2_and_so3/orientations.py
--rw-r--r--   0        0        0     5121 2024-01-30 12:19:32.831890 ebsdtorch-0.1.0/ebsdtorch/s2_and_so3/sampling.py
--rw-r--r--   0        0        0    12034 2024-01-09 17:51:45.634049 ebsdtorch-0.1.0/ebsdtorch/simulation/monte_carlo_simulation.py
--rw-r--r--   0        0        0     4430 2024-01-05 04:09:20.750990 ebsdtorch-0.1.0/ebsdtorch/spherical/extended_precision.py
--rw-r--r--   0        0        0     3358 2024-01-05 04:09:20.522973 ebsdtorch-0.1.0/ebsdtorch/spherical/spherical_harmonic_transform.py
--rw-r--r--   0        0        0     9100 2024-01-09 17:45:48.544442 ebsdtorch-0.1.0/ebsdtorch/spherical/test_ts2kit_wigner.py
--rw-r--r--   0        0        0    23579 2024-01-05 04:09:20.710986 ebsdtorch-0.1.0/ebsdtorch/spherical/wigner_d_coeff.py
--rw-r--r--   0        0        0    14234 2024-01-05 04:09:20.838996 ebsdtorch-0.1.0/ebsdtorch/spherical/wigner_d_coeff_Fukushima.py
--rw-r--r--   0        0        0     1036 2024-01-09 17:51:28.008785 ebsdtorch-0.1.0/ebsdtorch/spherical/wigner_d_coeff_spherical.py
--rw-r--r--   0        0        0    18734 2024-01-05 04:09:20.955004 ebsdtorch-0.1.0/ebsdtorch/spherical/wigner_d_coeffs_Lenthe.py
--rw-r--r--   0        0        0     2897 2023-12-21 04:36:35.474971 ebsdtorch-0.1.0/ebsdtorch/spherical/wigner_naive.py
--rw-r--r--   0        0        0      291 2023-12-21 02:31:23.880295 ebsdtorch-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2324 1970-01-01 00:00:00.000000 ebsdtorch-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-01-30 12:57:55.423222 ebsdtorch-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1942 2024-01-30 12:57:13.263133 ebsdtorch-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-09-11 16:52:02.001783 ebsdtorch-0.1.1/ebsdtorch/__init__.py
+-rw-r--r--   0        0        0      218 2024-01-30 12:02:28.600549 ebsdtorch-0.1.1/ebsdtorch/ebsd_dictionary_indexing/__init__.py
+-rw-r--r--   0        0        0     4495 2024-01-30 13:13:09.011836 ebsdtorch-0.1.1/ebsdtorch/ebsd_dictionary_indexing/blur_master_pattern_direct.py
+-rw-r--r--   0        0        0    10088 2024-01-30 11:41:52.900698 ebsdtorch-0.1.1/ebsdtorch/ebsd_dictionary_indexing/ebsd_di_one_pc_one_phase.py
+-rw-r--r--   0        0        0    13737 2024-01-30 11:38:40.130001 ebsdtorch-0.1.1/ebsdtorch/ebsd_dictionary_indexing/ebsd_di_one_pc_one_phase_pca.py
+-rw-r--r--   0        0        0     9160 2024-01-30 11:56:48.271540 ebsdtorch-0.1.1/ebsdtorch/ebsd_dictionary_indexing/ebsd_di_spherical_covmat.py
+-rw-r--r--   0        0        0     5094 2024-01-09 17:16:06.400640 ebsdtorch-0.1.1/ebsdtorch/ebsd_dictionary_indexing/utils_covariance_matrix.py
+-rw-r--r--   0        0        0     8685 2024-01-30 11:57:40.020559 ebsdtorch-0.1.1/ebsdtorch/ebsd_dictionary_indexing/utils_nearest_neighbors.py
+-rw-r--r--   0        0        0     1206 2024-01-09 17:15:47.659296 ebsdtorch-0.1.1/ebsdtorch/ebsd_dictionary_indexing/utils_progress_bar.py
+-rw-r--r--   0        0        0       42 2024-01-30 11:31:37.461005 ebsdtorch-0.1.1/ebsdtorch/ebsd_high_resolution/__init__.py
+-rw-r--r--   0        0        0     6242 2024-01-30 11:57:57.682272 ebsdtorch-0.1.1/ebsdtorch/ebsd_high_resolution/hrebsd_project.py
+-rw-r--r--   0        0        0        0 2023-09-08 10:49:41.283732 ebsdtorch-0.1.1/ebsdtorch/patterns/__init__.py
+-rw-r--r--   0        0        0    15084 2024-01-05 04:09:20.262954 ebsdtorch-0.1.1/ebsdtorch/patterns/lie_algebra_se3.py
+-rw-r--r--   0        0        0     3206 2023-12-21 19:35:49.252383 ebsdtorch-0.1.1/ebsdtorch/patterns/lie_algebra_sim3_with_stretch.py
+-rw-r--r--   0        0        0     8235 2024-01-30 11:38:40.534040 ebsdtorch-0.1.1/ebsdtorch/patterns/pattern_projection.py
+-rw-r--r--   0        0        0     6958 2024-01-05 04:09:20.322959 ebsdtorch-0.1.1/ebsdtorch/patterns/square_hemisphere_bijection.py
+-rw-r--r--   0        0        0        0 2023-09-09 11:06:24.072730 ebsdtorch-0.1.1/ebsdtorch/s2_and_so3/__init__.py
+-rw-r--r--   0        0        0    23064 2024-01-30 12:17:06.553703 ebsdtorch-0.1.1/ebsdtorch/s2_and_so3/laue.py
+-rw-r--r--   0        0        0    49329 2024-01-05 16:09:49.263451 ebsdtorch-0.1.1/ebsdtorch/s2_and_so3/orientations.py
+-rw-r--r--   0        0        0     5121 2024-01-30 12:19:32.831890 ebsdtorch-0.1.1/ebsdtorch/s2_and_so3/sampling.py
+-rw-r--r--   0        0        0    12034 2024-01-09 17:51:45.634049 ebsdtorch-0.1.1/ebsdtorch/simulation/monte_carlo_simulation.py
+-rw-r--r--   0        0        0     4430 2024-01-05 04:09:20.750990 ebsdtorch-0.1.1/ebsdtorch/spherical/extended_precision.py
+-rw-r--r--   0        0        0     3358 2024-01-05 04:09:20.522973 ebsdtorch-0.1.1/ebsdtorch/spherical/spherical_harmonic_transform.py
+-rw-r--r--   0        0        0     9100 2024-01-09 17:45:48.544442 ebsdtorch-0.1.1/ebsdtorch/spherical/test_ts2kit_wigner.py
+-rw-r--r--   0        0        0    23579 2024-01-05 04:09:20.710986 ebsdtorch-0.1.1/ebsdtorch/spherical/wigner_d_coeff.py
+-rw-r--r--   0        0        0    14234 2024-01-05 04:09:20.838996 ebsdtorch-0.1.1/ebsdtorch/spherical/wigner_d_coeff_Fukushima.py
+-rw-r--r--   0        0        0     1036 2024-01-09 17:51:28.008785 ebsdtorch-0.1.1/ebsdtorch/spherical/wigner_d_coeff_spherical.py
+-rw-r--r--   0        0        0    18734 2024-01-05 04:09:20.955004 ebsdtorch-0.1.1/ebsdtorch/spherical/wigner_d_coeffs_Lenthe.py
+-rw-r--r--   0        0        0     2897 2023-12-21 04:36:35.474971 ebsdtorch-0.1.1/ebsdtorch/spherical/wigner_naive.py
+-rw-r--r--   0        0        0      291 2024-01-30 13:15:43.558827 ebsdtorch-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2324 1970-01-01 00:00:00.000000 ebsdtorch-0.1.1/PKG-INFO
```

### Comparing `ebsdtorch-0.1.0/LICENSE` & `ebsdtorch-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ebsdtorch-0.1.0/README.md` & `ebsdtorch-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `ebsdtorch-0.1.0/ebsdtorch/ebsd_dictionary_indexing/blur_master_pattern_direct.py` & `ebsdtorch-0.1.1/ebsdtorch/ebsd_dictionary_indexing/blur_master_pattern_direct.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,17 @@
     Returns
     -------
     torch.Tensor
         Shape (n, n). The detector annulus convolved with the incoming signal on the sphere.
 
     """
     # sample points on the sphere used for integration - returned as (n, 3) xyz coordinates
-    s2_points = s2_fibonacci_lattice(n_s2_points).double().to(square_lambert_mp.device)
+    s2_points = s2_fibonacci_lattice(
+        n_s2_points, device=square_lambert_mp.device
+    ).double()
 
     # convert xyz coordinates to latitude and longitude
     theta_phi_pts = xyz_to_theta_phi(s2_points).double()
 
     # make an indicator for the points in the annulus
     annulus_mask = (theta_phi_pts[:, 0] > inner_opening_angle) & (
         theta_phi_pts[:, 0] < outer_opening_angle
```

### Comparing `ebsdtorch-0.1.0/ebsdtorch/ebsd_dictionary_indexing/ebsd_di_one_pc_one_phase.py` & `ebsdtorch-0.1.1/ebsdtorch/ebsd_dictionary_indexing/ebsd_di_one_pc_one_phase.py`

 * *Files identical despite different names*

### Comparing `ebsdtorch-0.1.0/ebsdtorch/ebsd_dictionary_indexing/ebsd_di_one_pc_one_phase_pca.py` & `ebsdtorch-0.1.1/ebsdtorch/ebsd_dictionary_indexing/ebsd_di_one_pc_one_phase_pca.py`

 * *Files identical despite different names*

### Comparing `ebsdtorch-0.1.0/ebsdtorch/ebsd_dictionary_indexing/ebsd_di_spherical_covmat.py` & `ebsdtorch-0.1.1/ebsdtorch/ebsd_dictionary_indexing/ebsd_di_spherical_covmat.py`

 * *Files identical despite different names*

### Comparing `ebsdtorch-0.1.0/ebsdtorch/ebsd_dictionary_indexing/utils_covariance_matrix.py` & `ebsdtorch-0.1.1/ebsdtorch/ebsd_dictionary_indexing/utils_covariance_matrix.py`

 * *Files identical despite different names*

### Comparing `ebsdtorch-0.1.0/ebsdtorch/ebsd_dictionary_indexing/utils_nearest_neighbors.py` & `ebsdtorch-0.1.1/ebsdtorch/ebsd_dictionary_indexing/utils_nearest_neighbors.py`

 * *Files identical despite different names*

### Comparing `ebsdtorch-0.1.0/ebsdtorch/ebsd_dictionary_indexing/utils_progress_bar.py` & `ebsdtorch-0.1.1/ebsdtorch/ebsd_dictionary_indexing/utils_progress_bar.py`

 * *Files identical despite different names*

### Comparing `ebsdtorch-0.1.0/ebsdtorch/ebsd_high_resolution/hrebsd_project.py` & `ebsdtorch-0.1.1/ebsdtorch/ebsd_high_resolution/hrebsd_project.py`

 * *Files identical despite different names*

### Comparing `ebsdtorch-0.1.0/ebsdtorch/patterns/lie_algebra_se3.py` & `ebsdtorch-0.1.1/ebsdtorch/patterns/lie_algebra_se3.py`

 * *Files identical despite different names*

### Comparing `ebsdtorch-0.1.0/ebsdtorch/patterns/lie_algebra_sim3_with_stretch.py` & `ebsdtorch-0.1.1/ebsdtorch/patterns/lie_algebra_sim3_with_stretch.py`

 * *Files identical despite different names*

### Comparing `ebsdtorch-0.1.0/ebsdtorch/patterns/pattern_projection.py` & `ebsdtorch-0.1.1/ebsdtorch/patterns/pattern_projection.py`

 * *Files identical despite different names*

### Comparing `ebsdtorch-0.1.0/ebsdtorch/patterns/square_hemisphere_bijection.py` & `ebsdtorch-0.1.1/ebsdtorch/patterns/square_hemisphere_bijection.py`

 * *Files identical despite different names*

### Comparing `ebsdtorch-0.1.0/ebsdtorch/s2_and_so3/laue.py` & `ebsdtorch-0.1.1/ebsdtorch/s2_and_so3/laue.py`

 * *Files identical despite different names*

### Comparing `ebsdtorch-0.1.0/ebsdtorch/s2_and_so3/orientations.py` & `ebsdtorch-0.1.1/ebsdtorch/s2_and_so3/orientations.py`

 * *Files identical despite different names*

### Comparing `ebsdtorch-0.1.0/ebsdtorch/s2_and_so3/sampling.py` & `ebsdtorch-0.1.1/ebsdtorch/s2_and_so3/sampling.py`

 * *Files identical despite different names*

### Comparing `ebsdtorch-0.1.0/ebsdtorch/simulation/monte_carlo_simulation.py` & `ebsdtorch-0.1.1/ebsdtorch/simulation/monte_carlo_simulation.py`

 * *Files identical despite different names*

### Comparing `ebsdtorch-0.1.0/ebsdtorch/spherical/extended_precision.py` & `ebsdtorch-0.1.1/ebsdtorch/spherical/extended_precision.py`

 * *Files identical despite different names*

### Comparing `ebsdtorch-0.1.0/ebsdtorch/spherical/spherical_harmonic_transform.py` & `ebsdtorch-0.1.1/ebsdtorch/spherical/spherical_harmonic_transform.py`

 * *Files identical despite different names*

### Comparing `ebsdtorch-0.1.0/ebsdtorch/spherical/test_ts2kit_wigner.py` & `ebsdtorch-0.1.1/ebsdtorch/spherical/test_ts2kit_wigner.py`

 * *Files identical despite different names*

### Comparing `ebsdtorch-0.1.0/ebsdtorch/spherical/wigner_d_coeff.py` & `ebsdtorch-0.1.1/ebsdtorch/spherical/wigner_d_coeff.py`

 * *Files identical despite different names*

### Comparing `ebsdtorch-0.1.0/ebsdtorch/spherical/wigner_d_coeff_Fukushima.py` & `ebsdtorch-0.1.1/ebsdtorch/spherical/wigner_d_coeff_Fukushima.py`

 * *Files identical despite different names*

### Comparing `ebsdtorch-0.1.0/ebsdtorch/spherical/wigner_d_coeff_spherical.py` & `ebsdtorch-0.1.1/ebsdtorch/spherical/wigner_d_coeff_spherical.py`

 * *Files identical despite different names*

### Comparing `ebsdtorch-0.1.0/ebsdtorch/spherical/wigner_d_coeffs_Lenthe.py` & `ebsdtorch-0.1.1/ebsdtorch/spherical/wigner_d_coeffs_Lenthe.py`

 * *Files identical despite different names*

### Comparing `ebsdtorch-0.1.0/ebsdtorch/spherical/wigner_naive.py` & `ebsdtorch-0.1.1/ebsdtorch/spherical/wigner_naive.py`

 * *Files identical despite different names*

### Comparing `ebsdtorch-0.1.0/PKG-INFO` & `ebsdtorch-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ebsdtorch
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 Author: Zachary Varley
 Author-email: zvarley@andrew.cmu.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

