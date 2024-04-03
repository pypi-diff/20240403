# Comparing `tmp/HSTI-0.0.98.tar.gz` & `tmp/HSTI-0.0.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HSTI-0.0.98.tar", last modified: Tue Mar 26 08:31:46 2024, max compression
+gzip compressed data, was "HSTI-0.0.99.tar", last modified: Tue Mar 26 08:35:02 2024, max compression
```

## Comparing `HSTI-0.0.98.tar` & `HSTI-0.0.99.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 madslarsen   (501) staff       (20)        0 2024-03-26 08:31:46.392019 HSTI-0.0.98/
--rw-r--r--   0 madslarsen   (501) staff       (20)     1023 2023-02-06 08:23:04.000000 HSTI-0.0.98/LICENSE
--rw-r--r--   0 madslarsen   (501) staff       (20)     6581 2024-03-26 08:31:46.391824 HSTI-0.0.98/PKG-INFO
--rw-r--r--   0 madslarsen   (501) staff       (20)     5615 2024-03-12 08:14:47.000000 HSTI-0.0.98/README.md
-drwxr-xr-x   0 madslarsen   (501) staff       (20)        0 2024-03-26 08:31:46.382014 HSTI-0.0.98/hsti-analysis/
-drwxr-xr-x   0 madslarsen   (501) staff       (20)        0 2024-03-26 08:31:46.390855 HSTI-0.0.98/hsti-analysis/HSTI/
--rw-r--r--   0 madslarsen   (501) staff       (20)     6538 2023-10-24 05:34:10.000000 HSTI-0.0.98/hsti-analysis/HSTI/FPI_TMM.py
--rw-r--r--   0 madslarsen   (501) staff       (20)     4534 2023-10-24 07:37:32.000000 HSTI-0.0.98/hsti-analysis/HSTI/FPI_class.py
--rw-r--r--   0 madslarsen   (501) staff       (20)     1864 2023-02-06 08:23:05.000000 HSTI-0.0.98/hsti-analysis/HSTI/PCA_class.py
--rw-r--r--   0 madslarsen   (501) staff       (20)    11157 2023-02-06 08:23:05.000000 HSTI-0.0.98/hsti-analysis/HSTI/TMM_class.py
--rw-r--r--   0 madslarsen   (501) staff       (20)     2622 2024-03-26 08:31:05.000000 HSTI-0.0.98/hsti-analysis/HSTI/__init__.py
--rw-r--r--   0 madslarsen   (501) staff       (20)     1652 2024-03-12 10:17:16.000000 HSTI-0.0.98/hsti-analysis/HSTI/animate_data_cube.py
--rw-r--r--   0 madslarsen   (501) staff       (20)    18489 2024-03-22 13:04:55.000000 HSTI-0.0.98/hsti-analysis/HSTI/basic_math.py
--rw-r--r--   0 madslarsen   (501) staff       (20)     3098 2023-04-25 08:43:22.000000 HSTI-0.0.98/hsti-analysis/HSTI/black_body_spectrum.py
--rw-r--r--   0 madslarsen   (501) staff       (20)      759 2023-07-27 09:53:30.000000 HSTI-0.0.98/hsti-analysis/HSTI/density_scatter_plot.py
--rw-r--r--   0 madslarsen   (501) staff       (20)     2570 2023-03-13 08:50:24.000000 HSTI-0.0.98/hsti-analysis/HSTI/dsc2numpy.py
--rw-r--r--   0 madslarsen   (501) staff       (20)     8617 2023-03-13 09:26:36.000000 HSTI-0.0.98/hsti-analysis/HSTI/dsc_class.py
--rw-r--r--   0 madslarsen   (501) staff       (20)     3173 2023-02-06 08:23:05.000000 HSTI-0.0.98/hsti-analysis/HSTI/fill_gaps.py
--rw-r--r--   0 madslarsen   (501) staff       (20)    14931 2024-01-09 13:35:27.000000 HSTI-0.0.98/hsti-analysis/HSTI/fpi_gmm.py
--rw-r--r--   0 madslarsen   (501) staff       (20)     2389 2023-02-06 08:23:05.000000 HSTI-0.0.98/hsti-analysis/HSTI/fpi_sim.py
--rw-r--r--   0 madslarsen   (501) staff       (20)     4780 2023-02-06 08:23:05.000000 HSTI-0.0.98/hsti-analysis/HSTI/fpi_sim_matrix.py
--rw-r--r--   0 madslarsen   (501) staff       (20)     7138 2023-02-06 08:23:05.000000 HSTI-0.0.98/hsti-analysis/HSTI/fpi_sim_matrix_angular.py
--rw-r--r--   0 madslarsen   (501) staff       (20)     3659 2023-02-06 08:23:05.000000 HSTI-0.0.98/hsti-analysis/HSTI/fpi_sim_matrix_no_broadening.py
--rw-r--r--   0 madslarsen   (501) staff       (20)     6635 2023-02-06 08:23:05.000000 HSTI-0.0.98/hsti-analysis/HSTI/graphene_sensor_TMM.py
--rw-r--r--   0 madslarsen   (501) staff       (20)     2373 2023-02-28 08:01:33.000000 HSTI-0.0.98/hsti-analysis/HSTI/hsti_export.py
--rw-r--r--   0 madslarsen   (501) staff       (20)     4456 2024-03-22 12:33:55.000000 HSTI-0.0.98/hsti-analysis/HSTI/hsti_import.py
--rw-r--r--   0 madslarsen   (501) staff       (20)     1057 2023-02-06 08:23:05.000000 HSTI-0.0.98/hsti-analysis/HSTI/import_camera_response.py
--rw-r--r--   0 madslarsen   (501) staff       (20)   141995 2024-03-25 13:27:29.000000 HSTI-0.0.98/hsti-analysis/HSTI/import_colormap.py
--rw-r--r--   0 madslarsen   (501) staff       (20)      265 2023-02-06 08:23:05.000000 HSTI-0.0.98/hsti-analysis/HSTI/import_mirror_sep.py
--rw-r--r--   0 madslarsen   (501) staff       (20)     1277 2023-04-25 08:45:08.000000 HSTI-0.0.98/hsti-analysis/HSTI/import_output.py
--rw-r--r--   0 madslarsen   (501) staff       (20)      643 2023-06-15 10:30:51.000000 HSTI-0.0.98/hsti-analysis/HSTI/import_pam.py
--rw-r--r--   0 madslarsen   (501) staff       (20)    15405 2023-02-06 08:23:05.000000 HSTI-0.0.98/hsti-analysis/HSTI/least_squares_methods.py
--rw-r--r--   0 madslarsen   (501) staff       (20)     5619 2023-02-06 08:23:05.000000 HSTI-0.0.98/hsti-analysis/HSTI/lossy_fpi_sim_matrix.py
--rw-r--r--   0 madslarsen   (501) staff       (20)     1753 2023-02-06 08:23:05.000000 HSTI-0.0.98/hsti-analysis/HSTI/mirror_sep2wavelength.py
--rw-r--r--   0 madslarsen   (501) staff       (20)      199 2023-02-06 08:23:05.000000 HSTI-0.0.98/hsti-analysis/HSTI/mse.py
--rw-r--r--   0 madslarsen   (501) staff       (20)      406 2023-02-06 08:23:05.000000 HSTI-0.0.98/hsti-analysis/HSTI/r_sq.py
--rwxr-xr-x   0 madslarsen   (501) staff       (20)    19979 2023-02-06 08:23:05.000000 HSTI-0.0.98/hsti-analysis/HSTI/remove_bad_px.py
--rw-r--r--   0 madslarsen   (501) staff       (20)     1032 2023-02-06 08:23:05.000000 HSTI-0.0.98/hsti-analysis/HSTI/remove_vignetting.py
--rw-r--r--   0 madslarsen   (501) staff       (20)    23310 2023-02-06 08:23:05.000000 HSTI-0.0.98/hsti-analysis/HSTI/repair_image_defects.py
--rw-r--r--   0 madslarsen   (501) staff       (20)      388 2023-07-27 09:53:30.000000 HSTI-0.0.98/hsti-analysis/HSTI/save_band.py
--rw-r--r--   0 madslarsen   (501) staff       (20)     2307 2023-02-06 08:23:05.000000 HSTI-0.0.98/hsti-analysis/HSTI/spectral_debending.py
--rw-r--r--   0 madslarsen   (501) staff       (20)     3133 2023-02-06 08:23:05.000000 HSTI-0.0.98/hsti-analysis/HSTI/voronoi_partitioning.py
-drwxr-xr-x   0 madslarsen   (501) staff       (20)        0 2024-03-26 08:31:46.391579 HSTI-0.0.98/hsti-analysis/HSTI.egg-info/
--rw-r--r--   0 madslarsen   (501) staff       (20)     6581 2024-03-26 08:31:46.000000 HSTI-0.0.98/hsti-analysis/HSTI.egg-info/PKG-INFO
--rw-r--r--   0 madslarsen   (501) staff       (20)     1575 2024-03-26 08:31:46.000000 HSTI-0.0.98/hsti-analysis/HSTI.egg-info/SOURCES.txt
--rw-r--r--   0 madslarsen   (501) staff       (20)        1 2024-03-26 08:31:46.000000 HSTI-0.0.98/hsti-analysis/HSTI.egg-info/dependency_links.txt
--rw-r--r--   0 madslarsen   (501) staff       (20)      264 2024-03-26 08:31:46.000000 HSTI-0.0.98/hsti-analysis/HSTI.egg-info/requires.txt
--rw-r--r--   0 madslarsen   (501) staff       (20)        5 2024-03-26 08:31:46.000000 HSTI-0.0.98/hsti-analysis/HSTI.egg-info/top_level.txt
--rw-r--r--   0 madslarsen   (501) staff       (20)      104 2023-02-06 08:23:05.000000 HSTI-0.0.98/pyproject.toml
--rw-r--r--   0 madslarsen   (501) staff       (20)       38 2024-03-26 08:31:46.392056 HSTI-0.0.98/setup.cfg
--rw-r--r--   0 madslarsen   (501) staff       (20)     2146 2024-03-26 08:31:29.000000 HSTI-0.0.98/setup.py
+drwxr-xr-x   0 madslarsen   (501) staff       (20)        0 2024-03-26 08:35:02.838646 HSTI-0.0.99/
+-rw-r--r--   0 madslarsen   (501) staff       (20)     1023 2023-02-06 08:23:04.000000 HSTI-0.0.99/LICENSE
+-rw-r--r--   0 madslarsen   (501) staff       (20)     6581 2024-03-26 08:35:02.838440 HSTI-0.0.99/PKG-INFO
+-rw-r--r--   0 madslarsen   (501) staff       (20)     5615 2024-03-12 08:14:47.000000 HSTI-0.0.99/README.md
+drwxr-xr-x   0 madslarsen   (501) staff       (20)        0 2024-03-26 08:35:02.832043 HSTI-0.0.99/hsti-analysis/
+drwxr-xr-x   0 madslarsen   (501) staff       (20)        0 2024-03-26 08:35:02.837364 HSTI-0.0.99/hsti-analysis/HSTI/
+-rw-r--r--   0 madslarsen   (501) staff       (20)     6538 2023-10-24 05:34:10.000000 HSTI-0.0.99/hsti-analysis/HSTI/FPI_TMM.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)     4534 2023-10-24 07:37:32.000000 HSTI-0.0.99/hsti-analysis/HSTI/FPI_class.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)     1864 2023-02-06 08:23:05.000000 HSTI-0.0.99/hsti-analysis/HSTI/PCA_class.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)    11157 2023-02-06 08:23:05.000000 HSTI-0.0.99/hsti-analysis/HSTI/TMM_class.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)     2622 2024-03-26 08:34:35.000000 HSTI-0.0.99/hsti-analysis/HSTI/__init__.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)     1652 2024-03-12 10:17:16.000000 HSTI-0.0.99/hsti-analysis/HSTI/animate_data_cube.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)    18489 2024-03-22 13:04:55.000000 HSTI-0.0.99/hsti-analysis/HSTI/basic_math.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)     3098 2023-04-25 08:43:22.000000 HSTI-0.0.99/hsti-analysis/HSTI/black_body_spectrum.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)      759 2023-07-27 09:53:30.000000 HSTI-0.0.99/hsti-analysis/HSTI/density_scatter_plot.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)     2570 2023-03-13 08:50:24.000000 HSTI-0.0.99/hsti-analysis/HSTI/dsc2numpy.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)     8617 2023-03-13 09:26:36.000000 HSTI-0.0.99/hsti-analysis/HSTI/dsc_class.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)     3173 2023-02-06 08:23:05.000000 HSTI-0.0.99/hsti-analysis/HSTI/fill_gaps.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)    14931 2024-01-09 13:35:27.000000 HSTI-0.0.99/hsti-analysis/HSTI/fpi_gmm.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)     2389 2023-02-06 08:23:05.000000 HSTI-0.0.99/hsti-analysis/HSTI/fpi_sim.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)     4780 2023-02-06 08:23:05.000000 HSTI-0.0.99/hsti-analysis/HSTI/fpi_sim_matrix.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)     7138 2023-02-06 08:23:05.000000 HSTI-0.0.99/hsti-analysis/HSTI/fpi_sim_matrix_angular.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)     3659 2023-02-06 08:23:05.000000 HSTI-0.0.99/hsti-analysis/HSTI/fpi_sim_matrix_no_broadening.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)     6635 2023-02-06 08:23:05.000000 HSTI-0.0.99/hsti-analysis/HSTI/graphene_sensor_TMM.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)     2373 2023-02-28 08:01:33.000000 HSTI-0.0.99/hsti-analysis/HSTI/hsti_export.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)     4456 2024-03-22 12:33:55.000000 HSTI-0.0.99/hsti-analysis/HSTI/hsti_import.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)     1057 2023-02-06 08:23:05.000000 HSTI-0.0.99/hsti-analysis/HSTI/import_camera_response.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)   141989 2024-03-26 08:34:09.000000 HSTI-0.0.99/hsti-analysis/HSTI/import_colormap.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)      265 2023-02-06 08:23:05.000000 HSTI-0.0.99/hsti-analysis/HSTI/import_mirror_sep.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)     1277 2023-04-25 08:45:08.000000 HSTI-0.0.99/hsti-analysis/HSTI/import_output.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)      643 2023-06-15 10:30:51.000000 HSTI-0.0.99/hsti-analysis/HSTI/import_pam.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)    15405 2023-02-06 08:23:05.000000 HSTI-0.0.99/hsti-analysis/HSTI/least_squares_methods.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)     5619 2023-02-06 08:23:05.000000 HSTI-0.0.99/hsti-analysis/HSTI/lossy_fpi_sim_matrix.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)     1753 2023-02-06 08:23:05.000000 HSTI-0.0.99/hsti-analysis/HSTI/mirror_sep2wavelength.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)      199 2023-02-06 08:23:05.000000 HSTI-0.0.99/hsti-analysis/HSTI/mse.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)      406 2023-02-06 08:23:05.000000 HSTI-0.0.99/hsti-analysis/HSTI/r_sq.py
+-rwxr-xr-x   0 madslarsen   (501) staff       (20)    19979 2023-02-06 08:23:05.000000 HSTI-0.0.99/hsti-analysis/HSTI/remove_bad_px.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)     1032 2023-02-06 08:23:05.000000 HSTI-0.0.99/hsti-analysis/HSTI/remove_vignetting.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)    23310 2023-02-06 08:23:05.000000 HSTI-0.0.99/hsti-analysis/HSTI/repair_image_defects.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)      388 2023-07-27 09:53:30.000000 HSTI-0.0.99/hsti-analysis/HSTI/save_band.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)     2307 2023-02-06 08:23:05.000000 HSTI-0.0.99/hsti-analysis/HSTI/spectral_debending.py
+-rw-r--r--   0 madslarsen   (501) staff       (20)     3133 2023-02-06 08:23:05.000000 HSTI-0.0.99/hsti-analysis/HSTI/voronoi_partitioning.py
+drwxr-xr-x   0 madslarsen   (501) staff       (20)        0 2024-03-26 08:35:02.838181 HSTI-0.0.99/hsti-analysis/HSTI.egg-info/
+-rw-r--r--   0 madslarsen   (501) staff       (20)     6581 2024-03-26 08:35:02.000000 HSTI-0.0.99/hsti-analysis/HSTI.egg-info/PKG-INFO
+-rw-r--r--   0 madslarsen   (501) staff       (20)     1575 2024-03-26 08:35:02.000000 HSTI-0.0.99/hsti-analysis/HSTI.egg-info/SOURCES.txt
+-rw-r--r--   0 madslarsen   (501) staff       (20)        1 2024-03-26 08:35:02.000000 HSTI-0.0.99/hsti-analysis/HSTI.egg-info/dependency_links.txt
+-rw-r--r--   0 madslarsen   (501) staff       (20)      264 2024-03-26 08:35:02.000000 HSTI-0.0.99/hsti-analysis/HSTI.egg-info/requires.txt
+-rw-r--r--   0 madslarsen   (501) staff       (20)        5 2024-03-26 08:35:02.000000 HSTI-0.0.99/hsti-analysis/HSTI.egg-info/top_level.txt
+-rw-r--r--   0 madslarsen   (501) staff       (20)      104 2023-02-06 08:23:05.000000 HSTI-0.0.99/pyproject.toml
+-rw-r--r--   0 madslarsen   (501) staff       (20)       38 2024-03-26 08:35:02.838684 HSTI-0.0.99/setup.cfg
+-rw-r--r--   0 madslarsen   (501) staff       (20)     2146 2024-03-26 08:34:44.000000 HSTI-0.0.99/setup.py
```

### Comparing `HSTI-0.0.98/LICENSE` & `HSTI-0.0.99/LICENSE`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/PKG-INFO` & `HSTI-0.0.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HSTI
-Version: 0.0.98
+Version: 0.0.99
 Summary: The NEWTEC HSTI package contains fundamental functions for the data analysis of hyperspectral thermal images (HSTI).
 Author: Mads Nibe et. al.
 Author-email: mani@newtec.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `HSTI-0.0.98/README.md` & `HSTI-0.0.99/README.md`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/FPI_TMM.py` & `HSTI-0.0.99/hsti-analysis/HSTI/FPI_TMM.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/FPI_class.py` & `HSTI-0.0.99/hsti-analysis/HSTI/FPI_class.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/PCA_class.py` & `HSTI-0.0.99/hsti-analysis/HSTI/PCA_class.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/TMM_class.py` & `HSTI-0.0.99/hsti-analysis/HSTI/TMM_class.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/__init__.py` & `HSTI-0.0.99/hsti-analysis/HSTI/__init__.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/animate_data_cube.py` & `HSTI-0.0.99/hsti-analysis/HSTI/animate_data_cube.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/basic_math.py` & `HSTI-0.0.99/hsti-analysis/HSTI/basic_math.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/black_body_spectrum.py` & `HSTI-0.0.99/hsti-analysis/HSTI/black_body_spectrum.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/density_scatter_plot.py` & `HSTI-0.0.99/hsti-analysis/HSTI/density_scatter_plot.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/dsc2numpy.py` & `HSTI-0.0.99/hsti-analysis/HSTI/dsc2numpy.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/dsc_class.py` & `HSTI-0.0.99/hsti-analysis/HSTI/dsc_class.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/fill_gaps.py` & `HSTI-0.0.99/hsti-analysis/HSTI/fill_gaps.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/fpi_gmm.py` & `HSTI-0.0.99/hsti-analysis/HSTI/fpi_gmm.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/fpi_sim.py` & `HSTI-0.0.99/hsti-analysis/HSTI/fpi_sim.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/fpi_sim_matrix.py` & `HSTI-0.0.99/hsti-analysis/HSTI/fpi_sim_matrix.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/fpi_sim_matrix_angular.py` & `HSTI-0.0.99/hsti-analysis/HSTI/fpi_sim_matrix_angular.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/fpi_sim_matrix_no_broadening.py` & `HSTI-0.0.99/hsti-analysis/HSTI/fpi_sim_matrix_no_broadening.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/graphene_sensor_TMM.py` & `HSTI-0.0.99/hsti-analysis/HSTI/graphene_sensor_TMM.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/hsti_export.py` & `HSTI-0.0.99/hsti-analysis/HSTI/hsti_export.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/hsti_import.py` & `HSTI-0.0.99/hsti-analysis/HSTI/hsti_import.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/import_camera_response.py` & `HSTI-0.0.99/hsti-analysis/HSTI/import_camera_response.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/import_colormap.py` & `HSTI-0.0.99/hsti-analysis/HSTI/import_colormap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from matplotlib.colors import ListedColormap
 
-def import_colormap(cmap_name = 'newtec'):
+def import_cm(cmap_name = 'newtec'):
     if cmap_name == 'newtec':
         cm_data = [[0.1607822 ,0.02174219,0.36553504],
                    [0.16179567,0.03348725,0.36219837],
                    [0.16299883,0.04464816,0.35933774],
                    [0.16432363,0.05438842,0.35670512],
                    [0.16575288,0.06300251,0.35425233],
                    [0.16728259,0.07077683,0.35198694],
```

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/import_output.py` & `HSTI-0.0.99/hsti-analysis/HSTI/import_output.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/import_pam.py` & `HSTI-0.0.99/hsti-analysis/HSTI/import_pam.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/least_squares_methods.py` & `HSTI-0.0.99/hsti-analysis/HSTI/least_squares_methods.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/lossy_fpi_sim_matrix.py` & `HSTI-0.0.99/hsti-analysis/HSTI/lossy_fpi_sim_matrix.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/mirror_sep2wavelength.py` & `HSTI-0.0.99/hsti-analysis/HSTI/mirror_sep2wavelength.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/remove_bad_px.py` & `HSTI-0.0.99/hsti-analysis/HSTI/remove_bad_px.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/remove_vignetting.py` & `HSTI-0.0.99/hsti-analysis/HSTI/remove_vignetting.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/repair_image_defects.py` & `HSTI-0.0.99/hsti-analysis/HSTI/repair_image_defects.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/spectral_debending.py` & `HSTI-0.0.99/hsti-analysis/HSTI/spectral_debending.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI/voronoi_partitioning.py` & `HSTI-0.0.99/hsti-analysis/HSTI/voronoi_partitioning.py`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI.egg-info/PKG-INFO` & `HSTI-0.0.99/hsti-analysis/HSTI.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HSTI
-Version: 0.0.98
+Version: 0.0.99
 Summary: The NEWTEC HSTI package contains fundamental functions for the data analysis of hyperspectral thermal images (HSTI).
 Author: Mads Nibe et. al.
 Author-email: mani@newtec.dk
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `HSTI-0.0.98/hsti-analysis/HSTI.egg-info/SOURCES.txt` & `HSTI-0.0.99/hsti-analysis/HSTI.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HSTI-0.0.98/setup.py` & `HSTI-0.0.99/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="HSTI",
-    version="0.0.98",
+    version="0.0.99",
     author="Mads Nibe et. al.",
     author_email="mani@newtec.dk",
     description="The NEWTEC HSTI package contains fundamental functions for the data analysis of hyperspectral thermal images (HSTI).",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

