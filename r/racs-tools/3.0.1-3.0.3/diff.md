# Comparing `tmp/racs_tools-3.0.1.tar.gz` & `tmp/racs_tools-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "racs_tools-3.0.1.tar", max compression
+gzip compressed data, was "racs_tools-3.0.3.tar", max compression
```

## Comparing `racs_tools-3.0.1.tar` & `racs_tools-3.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1520 2023-05-22 00:36:00.000000 racs_tools-3.0.1/LICENSE
--rw-r--r--   0        0        0     9172 2023-11-27 07:12:18.027959 racs_tools-3.0.1/README.md
--rw-r--r--   0        0        0      735 2023-11-27 07:12:39.787190 racs_tools-3.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-22 00:36:00.000000 racs_tools-3.0.1/racs_tools/__init__.py
--rw-r--r--   0        0        0     5027 2023-11-27 06:58:23.881529 racs_tools-3.0.1/racs_tools/au2.py
--rw-r--r--   0        0        0    24627 2023-11-27 03:47:50.431863 racs_tools-3.0.1/racs_tools/beamcon_2D.py
--rw-r--r--   0        0        0    46084 2023-11-27 06:58:23.881829 racs_tools-3.0.1/racs_tools/beamcon_3D.py
--rw-r--r--   0        0        0     5430 2023-11-27 06:58:23.882032 racs_tools-3.0.1/racs_tools/convolve_uv.py
--rw-r--r--   0        0        0     2709 2023-11-27 06:58:23.882143 racs_tools-3.0.1/racs_tools/gaussft.py
--rw-r--r--   0        0        0     8670 2023-11-27 06:58:23.882296 racs_tools-3.0.1/racs_tools/getnoise_list.py
--rw-r--r--   0        0        0     1038 2023-11-27 05:02:46.964605 racs_tools-3.0.1/racs_tools/logging.py
--rw-r--r--   0        0        0     9940 1970-01-01 00:00:00.000000 racs_tools-3.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1520 2024-04-03 04:50:23.671596 racs_tools-3.0.3/LICENSE
+-rw-r--r--   0        0        0     9351 2024-04-03 04:50:23.671596 racs_tools-3.0.3/README.md
+-rw-r--r--   0        0        0      735 2024-04-03 04:50:23.671596 racs_tools-3.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-03 04:50:23.671596 racs_tools-3.0.3/racs_tools/__init__.py
+-rw-r--r--   0        0        0     5027 2024-04-03 04:50:23.671596 racs_tools-3.0.3/racs_tools/au2.py
+-rw-r--r--   0        0        0    24627 2024-04-03 04:50:23.671596 racs_tools-3.0.3/racs_tools/beamcon_2D.py
+-rw-r--r--   0        0        0    46084 2024-04-03 04:50:23.671596 racs_tools-3.0.3/racs_tools/beamcon_3D.py
+-rw-r--r--   0        0        0     5430 2024-04-03 04:50:23.671596 racs_tools-3.0.3/racs_tools/convolve_uv.py
+-rw-r--r--   0        0        0     2709 2024-04-03 04:50:23.671596 racs_tools-3.0.3/racs_tools/gaussft.py
+-rw-r--r--   0        0        0     8670 2024-04-03 04:50:23.671596 racs_tools-3.0.3/racs_tools/getnoise_list.py
+-rw-r--r--   0        0        0     1038 2024-04-03 04:50:23.671596 racs_tools-3.0.3/racs_tools/logging.py
+-rw-r--r--   0        0        0    10170 1970-01-01 00:00:00.000000 racs_tools-3.0.3/PKG-INFO
```

### Comparing `racs_tools-3.0.1/LICENSE` & `racs_tools-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `racs_tools-3.0.1/README.md` & `racs_tools-3.0.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-[![Docker Build and Push](https://github.com/AlecThomson/RACS-tools/actions/workflows/docker.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/docker.yml) ![Tests](https://github.com/AlecThomson/RACS-tools/actions/workflows/pytest.yml/badge.svg) [![Python package](https://github.com/AlecThomson/RACS-tools/actions/workflows/python-package.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/python-package.yml) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Docker Build and Push](https://github.com/AlecThomson/RACS-tools/actions/workflows/docker.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/docker.yml) ![Tests](https://github.com/AlecThomson/RACS-tools/actions/workflows/pytest.yml/badge.svg) [![Python package](https://github.com/AlecThomson/RACS-tools/actions/workflows/python-package.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/python-package.yml) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/AlecThomson/RACS-tools/master.svg)](https://results.pre-commit.ci/latest/github/AlecThomson/RACS-tools/master)
+
 # RACS-tools
 Useful scripts for RACS
 
 ## Installation
 
 ### Conda
 The recommended way to install. First obtain `conda` from Anaconda or Miniconda. Clone this repo, build the environment, and activate:
```

### Comparing `racs_tools-3.0.1/pyproject.toml` & `racs_tools-3.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "racs-tools"
-version = "3.0.1"
+version = "3.0.3"
 description = "Useful scripts for RACS."
 authors = ["Alec Thomson"]
 license = "BSD"
 readme = "README.md"
 packages = [{include = "racs_tools"}]
 
 [tool.poetry.dependencies]
```

### Comparing `racs_tools-3.0.1/racs_tools/au2.py` & `racs_tools-3.0.3/racs_tools/au2.py`

 * *Files identical despite different names*

### Comparing `racs_tools-3.0.1/racs_tools/beamcon_2D.py` & `racs_tools-3.0.3/racs_tools/beamcon_2D.py`

 * *Files identical despite different names*

### Comparing `racs_tools-3.0.1/racs_tools/beamcon_3D.py` & `racs_tools-3.0.3/racs_tools/beamcon_3D.py`

 * *Files identical despite different names*

### Comparing `racs_tools-3.0.1/racs_tools/convolve_uv.py` & `racs_tools-3.0.3/racs_tools/convolve_uv.py`

 * *Files identical despite different names*

### Comparing `racs_tools-3.0.1/racs_tools/gaussft.py` & `racs_tools-3.0.3/racs_tools/gaussft.py`

 * *Files identical despite different names*

### Comparing `racs_tools-3.0.1/racs_tools/getnoise_list.py` & `racs_tools-3.0.3/racs_tools/getnoise_list.py`

 * *Files identical despite different names*

### Comparing `racs_tools-3.0.1/racs_tools/logging.py` & `racs_tools-3.0.3/racs_tools/logging.py`

 * *Files identical despite different names*

### Comparing `racs_tools-3.0.1/PKG-INFO` & `racs_tools-3.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 Metadata-Version: 2.1
 Name: racs-tools
-Version: 3.0.1
+Version: 3.0.3
 Summary: Useful scripts for RACS.
 License: BSD
 Author: Alec Thomson
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: mpi
 Requires-Dist: astropy (>=5,<6)
 Requires-Dist: mpi4py ; extra == "mpi"
 Requires-Dist: numba
 Requires-Dist: numpy (<2)
 Requires-Dist: radio_beam
 Requires-Dist: schwimmbad
 Requires-Dist: scipy
 Requires-Dist: spectral_cube (>=0.6.3,<0.7.0)
 Requires-Dist: tqdm
 Description-Content-Type: text/markdown
 
-[![Docker Build and Push](https://github.com/AlecThomson/RACS-tools/actions/workflows/docker.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/docker.yml) ![Tests](https://github.com/AlecThomson/RACS-tools/actions/workflows/pytest.yml/badge.svg) [![Python package](https://github.com/AlecThomson/RACS-tools/actions/workflows/python-package.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/python-package.yml) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Docker Build and Push](https://github.com/AlecThomson/RACS-tools/actions/workflows/docker.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/docker.yml) ![Tests](https://github.com/AlecThomson/RACS-tools/actions/workflows/pytest.yml/badge.svg) [![Python package](https://github.com/AlecThomson/RACS-tools/actions/workflows/python-package.yml/badge.svg)](https://github.com/AlecThomson/RACS-tools/actions/workflows/python-package.yml) [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/AlecThomson/RACS-tools/master.svg)](https://results.pre-commit.ci/latest/github/AlecThomson/RACS-tools/master)
+
 # RACS-tools
 Useful scripts for RACS
 
 ## Installation
 
 ### Conda
 The recommended way to install. First obtain `conda` from Anaconda or Miniconda. Clone this repo, build the environment, and activate:
```

