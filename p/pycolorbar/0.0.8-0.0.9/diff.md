# Comparing `tmp/pycolorbar-0.0.8.tar.gz` & `tmp/pycolorbar-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycolorbar-0.0.8.tar", last modified: Tue Mar 12 17:08:16 2024, max compression
+gzip compressed data, was "pycolorbar-0.0.9.tar", last modified: Wed Mar 13 17:18:15 2024, max compression
```

## Comparing `pycolorbar-0.0.8.tar` & `pycolorbar-0.0.9.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:08:16.524335 pycolorbar-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    21340 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10208 2024-03-12 17:08:16.524335 pycolorbar-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/Untitled.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:08:16.516334 pycolorbar-0.0.8/pycolorbar/
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/pycolorbar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-12 17:08:16.000000 pycolorbar-0.0.8/pycolorbar/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:08:16.516334 pycolorbar-0.0.8/pycolorbar/colors/
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/pycolorbar/colors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24441 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/pycolorbar/colors/colors_io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:08:16.512334 pycolorbar-0.0.8/pycolorbar/etc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:08:16.516334 pycolorbar-0.0.8/pycolorbar/etc/colorbars/
--rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/pycolorbar/etc/colorbars/example_colorbar_configurations.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:08:16.512334 pycolorbar-0.0.8/pycolorbar/etc/colormaps/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:08:16.520335 pycolorbar-0.0.8/pycolorbar/etc/colormaps/precipitation/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/pycolorbar/etc/colormaps/precipitation/IMERG_Liquid.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/pycolorbar/etc/colormaps/precipitation/IMERG_Solid.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/pycolorbar/etc/colormaps/precipitation/STEPS-BE.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/pycolorbar/etc/colormaps/precipitation/STEPS-BOM-RF3.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/pycolorbar/etc/colormaps/precipitation/STEPS-MCH.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/pycolorbar/etc/colormaps/precipitation/STEPS-NL.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:08:16.520335 pycolorbar-0.0.8/pycolorbar/settings/
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/pycolorbar/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/pycolorbar/settings/colorbar_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    19864 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/pycolorbar/settings/colorbar_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    27217 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/pycolorbar/settings/colorbar_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/pycolorbar/settings/colorbar_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/pycolorbar/settings/colormap_io.py
--rw-r--r--   0 runner    (1001) docker     (127)    21414 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/pycolorbar/settings/colormap_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/pycolorbar/settings/colormap_utility.py
--rw-r--r--   0 runner    (1001) docker     (127)    12474 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/pycolorbar/settings/colormap_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/pycolorbar/settings/colormap_visualization.py
--rw-r--r--   0 runner    (1001) docker     (127)    20278 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/pycolorbar/settings/matplotlib_kwargs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/pycolorbar/settings/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:08:16.520335 pycolorbar-0.0.8/pycolorbar/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/pycolorbar/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/pycolorbar/utils/directories.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/pycolorbar/utils/mpl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/pycolorbar/utils/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 17:08:16.520335 pycolorbar-0.0.8/pycolorbar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10208 2024-03-12 17:08:16.000000 pycolorbar-0.0.8/pycolorbar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-03-12 17:08:16.000000 pycolorbar-0.0.8/pycolorbar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 17:08:16.000000 pycolorbar-0.0.8/pycolorbar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-12 17:08:16.000000 pycolorbar-0.0.8/pycolorbar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-12 17:08:16.000000 pycolorbar-0.0.8/pycolorbar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 17:08:16.524335 pycolorbar-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-12 17:08:10.000000 pycolorbar-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:18:15.529718 pycolorbar-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)     2223 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5498 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    21340 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    10246 2024-03-13 17:18:15.529718 pycolorbar-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7077 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:18:15.525718 pycolorbar-0.0.9/pycolorbar/
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/pycolorbar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-13 17:18:15.000000 pycolorbar-0.0.9/pycolorbar/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:18:15.525718 pycolorbar-0.0.9/pycolorbar/colors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/pycolorbar/colors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24441 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/pycolorbar/colors/colors_io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:18:15.521718 pycolorbar-0.0.9/pycolorbar/etc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:18:15.525718 pycolorbar-0.0.9/pycolorbar/etc/colorbars/
+-rw-r--r--   0 runner    (1001) docker     (127)     2004 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/pycolorbar/etc/colorbars/example_colorbar_configurations.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:18:15.521718 pycolorbar-0.0.9/pycolorbar/etc/colormaps/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:18:15.525718 pycolorbar-0.0.9/pycolorbar/etc/colormaps/precipitation/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/pycolorbar/etc/colormaps/precipitation/IMERG_Liquid.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/pycolorbar/etc/colormaps/precipitation/IMERG_Solid.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/pycolorbar/etc/colormaps/precipitation/STEPS-BE.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/pycolorbar/etc/colormaps/precipitation/STEPS-BOM-RF3.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/pycolorbar/etc/colormaps/precipitation/STEPS-MCH.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/pycolorbar/etc/colormaps/precipitation/STEPS-NL.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:18:15.529718 pycolorbar-0.0.9/pycolorbar/settings/
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/pycolorbar/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/pycolorbar/settings/colorbar_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19872 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/pycolorbar/settings/colorbar_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27217 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/pycolorbar/settings/colorbar_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3919 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/pycolorbar/settings/colorbar_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/pycolorbar/settings/colormap_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21414 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/pycolorbar/settings/colormap_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/pycolorbar/settings/colormap_utility.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12474 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/pycolorbar/settings/colormap_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/pycolorbar/settings/colormap_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20435 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/pycolorbar/settings/matplotlib_kwargs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/pycolorbar/settings/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:18:15.529718 pycolorbar-0.0.9/pycolorbar/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/pycolorbar/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2676 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/pycolorbar/utils/directories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/pycolorbar/utils/mpl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2173 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/pycolorbar/utils/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-13 17:18:15.529718 pycolorbar-0.0.9/pycolorbar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10246 2024-03-13 17:18:15.000000 pycolorbar-0.0.9/pycolorbar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-03-13 17:18:15.000000 pycolorbar-0.0.9/pycolorbar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-13 17:18:15.000000 pycolorbar-0.0.9/pycolorbar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-13 17:18:15.000000 pycolorbar-0.0.9/pycolorbar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-13 17:18:15.000000 pycolorbar-0.0.9/pycolorbar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-13 17:18:15.529718 pycolorbar-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-13 17:18:11.000000 pycolorbar-0.0.9/setup.py
```

### Comparing `pycolorbar-0.0.8/.gitignore` & `pycolorbar-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `pycolorbar-0.0.8/.pre-commit-config.yaml` & `pycolorbar-0.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pycolorbar-0.0.8/.readthedocs.yml` & `pycolorbar-0.0.9/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `pycolorbar-0.0.8/AUTHORS.md` & `pycolorbar-0.0.9/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `pycolorbar-0.0.8/CODE_OF_CONDUCT.md` & `pycolorbar-0.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pycolorbar-0.0.8/CONTRIBUTING.rst` & `pycolorbar-0.0.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pycolorbar-0.0.8/LICENSE` & `pycolorbar-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pycolorbar-0.0.8/PKG-INFO` & `pycolorbar-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycolorbar
-Version: 0.0.8
+Version: 0.0.9
 Summary: YAML-based colormap & colorbar settings for matplotlib and xarray
 Author-email: Gionata Ghiggi <gionata.ghiggi@epfl.ch>
 License: MIT License
         
         Copyright (c) 2023 Gionata Ghiggi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -53,14 +53,15 @@
 License-File: LICENSE
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pydantic>=2.0.0
 Requires-Dist: PyYAML
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: loghub; extra == "dev"
 Requires-Dist: deepdiff; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-mock; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
```

### Comparing `pycolorbar-0.0.8/README.md` & `pycolorbar-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pycolorbar-0.0.8/SECURITY.md` & `pycolorbar-0.0.9/SECURITY.md`

 * *Files identical despite different names*

### Comparing `pycolorbar-0.0.8/pycolorbar/__init__.py` & `pycolorbar-0.0.9/pycolorbar/__init__.py`

 * *Files identical despite different names*

### Comparing `pycolorbar-0.0.8/pycolorbar/colors/__init__.py` & `pycolorbar-0.0.9/pycolorbar/colors/__init__.py`

 * *Files identical despite different names*

### Comparing `pycolorbar-0.0.8/pycolorbar/colors/colors_io.py` & `pycolorbar-0.0.9/pycolorbar/colors/colors_io.py`

 * *Files identical despite different names*

### Comparing `pycolorbar-0.0.8/pycolorbar/etc/colorbars/example_colorbar_configurations.yaml` & `pycolorbar-0.0.9/pycolorbar/etc/colorbars/example_colorbar_configurations.yaml`

 * *Files identical despite different names*

### Comparing `pycolorbar-0.0.8/pycolorbar/settings/__init__.py` & `pycolorbar-0.0.9/pycolorbar/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `pycolorbar-0.0.8/pycolorbar/settings/colorbar_io.py` & `pycolorbar-0.0.9/pycolorbar/settings/colorbar_io.py`

 * *Files identical despite different names*

### Comparing `pycolorbar-0.0.8/pycolorbar/settings/colorbar_registry.py` & `pycolorbar-0.0.9/pycolorbar/settings/colorbar_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,15 +338,15 @@
             self.show_colorbar(name=names[0])
             return None
 
         # Display colorbars
         list_args = [[name] + list(self.get_plot_kwargs(name=name)) for name in names]
         plot_colorbars(list_args, subplot_size=subplot_size)
 
-    def get_plot_kwargs(self, name=None, user_plot_kwargs={}, user_cbar_kwargs={}):
+    def get_plot_kwargs(self, name=None, user_plot_kwargs=None, user_cbar_kwargs=None):
         """Get pycolorbar plot kwargs (updated with optional user arguments)."""
         from pycolorbar.settings.matplotlib_kwargs import (
             get_plot_cbar_kwargs,
             update_plot_cbar_kwargs,
         )
 
         if not isinstance(name, (str, type(None))):
@@ -450,15 +450,15 @@
         The validated colorbar dictionary.
 
     """
     colorbars = ColorbarRegistry.get_instance()
     return colorbars.get_cbar_dict(name, resolve_reference=resolve_reference)
 
 
-def get_plot_kwargs(name=None, user_plot_kwargs={}, user_cbar_kwargs={}):
+def get_plot_kwargs(name=None, user_plot_kwargs=None, user_cbar_kwargs=None):
     """
     Get matplotlib, xarray and geopandas compatible plot and colorbar kwargs.
 
     Parameters
     ----------
     name : str, optional
         Name of the registered colorbar settings.
```

### Comparing `pycolorbar-0.0.8/pycolorbar/settings/colorbar_validator.py` & `pycolorbar-0.0.9/pycolorbar/settings/colorbar_validator.py`

 * *Files identical despite different names*

### Comparing `pycolorbar-0.0.8/pycolorbar/settings/colorbar_visualization.py` & `pycolorbar-0.0.9/pycolorbar/settings/colorbar_visualization.py`

 * *Files identical despite different names*

### Comparing `pycolorbar-0.0.8/pycolorbar/settings/colormap_io.py` & `pycolorbar-0.0.9/pycolorbar/settings/colormap_io.py`

 * *Files identical despite different names*

### Comparing `pycolorbar-0.0.8/pycolorbar/settings/colormap_registry.py` & `pycolorbar-0.0.9/pycolorbar/settings/colormap_registry.py`

 * *Files identical despite different names*

### Comparing `pycolorbar-0.0.8/pycolorbar/settings/colormap_utility.py` & `pycolorbar-0.0.9/pycolorbar/settings/colormap_utility.py`

 * *Files identical despite different names*

### Comparing `pycolorbar-0.0.8/pycolorbar/settings/colormap_validator.py` & `pycolorbar-0.0.9/pycolorbar/settings/colormap_validator.py`

 * *Files identical despite different names*

### Comparing `pycolorbar-0.0.8/pycolorbar/settings/colormap_visualization.py` & `pycolorbar-0.0.9/pycolorbar/settings/colormap_visualization.py`

 * *Files identical despite different names*

### Comparing `pycolorbar-0.0.8/pycolorbar/settings/matplotlib_kwargs.py` & `pycolorbar-0.0.9/pycolorbar/settings/matplotlib_kwargs.py`

 * *Files 2% similar despite different names*

```diff
@@ -267,16 +267,19 @@
     return ticks, ticklabels
 
 
 ####--------------------------------------------------------------------------------------------.
 #### Update pycolorbar settings based on user arguments
 
 
-def update_plot_cbar_kwargs(default_plot_kwargs, default_cbar_kwargs, user_plot_kwargs={}, user_cbar_kwargs={}):
+def update_plot_cbar_kwargs(default_plot_kwargs, default_cbar_kwargs, user_plot_kwargs=None, user_cbar_kwargs=None):
+
     # If no user kwargs, return default kwargs
+    user_plot_kwargs = {} if user_plot_kwargs is None else user_plot_kwargs
+    user_cbar_kwargs = {} if user_cbar_kwargs is None else user_cbar_kwargs
     if user_plot_kwargs == {} and user_cbar_kwargs == {}:
         return default_plot_kwargs, default_cbar_kwargs
 
     # If user cmap
     # - is a string, retrieve colormap
     # - is None --> delete the argument
     _parse_user_cmap(user_plot_kwargs=user_plot_kwargs)
```

### Comparing `pycolorbar-0.0.8/pycolorbar/settings/utils.py` & `pycolorbar-0.0.9/pycolorbar/settings/utils.py`

 * *Files identical despite different names*

### Comparing `pycolorbar-0.0.8/pycolorbar/utils/directories.py` & `pycolorbar-0.0.9/pycolorbar/utils/directories.py`

 * *Files identical despite different names*

### Comparing `pycolorbar-0.0.8/pycolorbar/utils/mpl.py` & `pycolorbar-0.0.9/pycolorbar/utils/mpl.py`

 * *Files identical despite different names*

### Comparing `pycolorbar-0.0.8/pycolorbar/utils/yaml.py` & `pycolorbar-0.0.9/pycolorbar/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `pycolorbar-0.0.8/pycolorbar.egg-info/PKG-INFO` & `pycolorbar-0.0.9/pycolorbar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycolorbar
-Version: 0.0.8
+Version: 0.0.9
 Summary: YAML-based colormap & colorbar settings for matplotlib and xarray
 Author-email: Gionata Ghiggi <gionata.ghiggi@epfl.ch>
 License: MIT License
         
         Copyright (c) 2023 Gionata Ghiggi
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -53,14 +53,15 @@
 License-File: LICENSE
 Requires-Dist: matplotlib
 Requires-Dist: numpy
 Requires-Dist: pydantic>=2.0.0
 Requires-Dist: PyYAML
 Provides-Extra: dev
 Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: loghub; extra == "dev"
 Requires-Dist: deepdiff; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-mock; extra == "dev"
 Requires-Dist: setuptools; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
```

### Comparing `pycolorbar-0.0.8/pycolorbar.egg-info/SOURCES.txt` & `pycolorbar-0.0.9/pycolorbar.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -4,17 +4,17 @@
 .readthedocs.yml
 AUTHORS.md
 CHANGELOG.md
 CODE_OF_CONDUCT.md
 CONTRIBUTING.rst
 LICENSE
 MANIFEST.in
+Makefile
 README.md
 SECURITY.md
-Untitled.ipynb
 pyproject.toml
 setup.py
 pycolorbar/__init__.py
 pycolorbar/_version.py
 pycolorbar.egg-info/PKG-INFO
 pycolorbar.egg-info/SOURCES.txt
 pycolorbar.egg-info/dependency_links.txt
```

### Comparing `pycolorbar-0.0.8/pyproject.toml` & `pycolorbar-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "pydantic>=2.0.0",
     "PyYAML",
 ]
 requires-python = ">=3.9"
 dynamic = ["version"]
 
 [project.optional-dependencies]
-dev = ["pre-commit",
+dev = ["pre-commit", "loghub",
        "deepdiff",
        "pytest", "pytest-cov", "pytest-mock",
        "setuptools",
        "build", "twine",
 ]
 
 [project.urls]
```

