# Comparing `tmp/napari-deeplabcut-0.2.1.5.tar.gz` & `tmp/napari-deeplabcut-0.2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-deeplabcut-0.2.1.5.tar", last modified: Tue Mar  5 15:05:50 2024, max compression
+gzip compressed data, was "napari-deeplabcut-0.2.1.6.tar", last modified: Wed Apr  3 15:32:53 2024, max compression
```

## Comparing `napari-deeplabcut-0.2.1.5.tar` & `napari-deeplabcut-0.2.1.6.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:05:50.388939 napari-deeplabcut-0.2.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:05:50.372939 napari-deeplabcut-0.2.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:05:50.376939 napari-deeplabcut-0.2.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:05:50.376939 napari-deeplabcut-0.2.1.5/.napari/
--rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/.napari/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14330 2024-03-05 15:05:50.388939 napari-deeplabcut-0.2.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12495 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:05:50.376939 napari-deeplabcut-0.2.1.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-03-05 15:05:50.388939 napari-deeplabcut-0.2.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:05:50.372939 napari-deeplabcut-0.2.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:05:50.376939 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9032 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:05:50.380939 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/_tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/_tests/test_keypoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/_tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/_tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/_tests/test_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-03-05 15:05:50.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    51599 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/_widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:05:50.380939 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:05:50.384939 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/black/
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/black/Back.png
--rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/black/Customize.png
--rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/black/Forward.png
--rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/black/Home.png
--rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/black/Pan.png
--rw-r--r--   0 runner    (1001) docker     (127)    12383 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/black/Pan_checked.png
--rw-r--r--   0 runner    (1001) docker     (127)     7726 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/black/Save.png
--rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/black/Subplots.png
--rw-r--r--   0 runner    (1001) docker     (127)     8367 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/black/Zoom.png
--rw-r--r--   0 runner    (1001) docker     (127)    12884 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/black/Zoom_checked.png
--rw-r--r--   0 runner    (1001) docker     (127)   437416 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/napari_shortcuts.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:05:50.384939 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/white/
--rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/white/Back.png
--rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/white/Customize.png
--rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/white/Forward.png
--rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/white/Home.png
--rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/white/Pan.png
--rw-r--r--   0 runner    (1001) docker     (127)    11810 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/white/Pan_checked.png
--rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/white/Save.png
--rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/white/Subplots.png
--rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/white/Zoom.png
--rw-r--r--   0 runner    (1001) docker     (127)    12372 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/white/Zoom_checked.png
--rw-r--r--   0 runner    (1001) docker     (127)     6598 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/keypoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     7072 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:05:50.384939 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/styles/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/styles/dark.mplstyle
--rw-r--r--   0 runner    (1001) docker     (127)      371 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/styles/light.mplstyle
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 15:05:50.384939 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14330 2024-03-05 15:05:50.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-03-05 15:05:50.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 15:05:50.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-05 15:05:50.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-05 15:05:50.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-05 15:05:50.000000 napari-deeplabcut-0.2.1.5/src/napari_deeplabcut.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-05 15:05:38.000000 napari-deeplabcut-0.2.1.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:32:53.844672 napari-deeplabcut-0.2.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:32:53.828672 napari-deeplabcut-0.2.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:32:53.832672 napari-deeplabcut-0.2.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:32:53.832672 napari-deeplabcut-0.2.1.6/.napari/
+-rw-r--r--   0 runner    (1001) docker     (127)     4203 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/.napari/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3356 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7651 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14330 2024-04-03 15:32:53.844672 napari-deeplabcut-0.2.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12495 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:32:53.832672 napari-deeplabcut-0.2.1.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-03 15:32:53.844672 napari-deeplabcut-0.2.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:32:53.832672 napari-deeplabcut-0.2.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:32:53.836672 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9032 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:32:53.836672 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2555 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/_tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/_tests/test_keypoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/_tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3585 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/_tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/_tests/test_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-03 15:32:53.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57412 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:32:53.836672 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:32:53.840672 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/black/
+-rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/black/Back.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7245 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/black/Customize.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/black/Forward.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7414 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/black/Home.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7315 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/black/Pan.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12383 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/black/Pan_checked.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7726 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/black/Save.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/black/Subplots.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8367 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/black/Zoom.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12884 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/black/Zoom_checked.png
+-rw-r--r--   0 runner    (1001) docker     (127)   437416 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/napari_shortcuts.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:32:53.840672 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/white/
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/white/Back.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6951 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/white/Customize.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6535 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/white/Forward.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7143 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/white/Home.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7114 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/white/Pan.png
+-rw-r--r--   0 runner    (1001) docker     (127)    11810 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/white/Pan_checked.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7381 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/white/Save.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6739 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/white/Subplots.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8064 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/white/Zoom.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12372 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/white/Zoom_checked.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7011 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/keypoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7072 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:32:53.840672 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/styles/
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/styles/dark.mplstyle
+-rw-r--r--   0 runner    (1001) docker     (127)      371 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/styles/light.mplstyle
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 15:32:53.840672 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14330 2024-04-03 15:32:53.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-03 15:32:53.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 15:32:53.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-03 15:32:53.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-03 15:32:53.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-03 15:32:53.000000 napari-deeplabcut-0.2.1.6/src/napari_deeplabcut.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-03 15:32:35.000000 napari-deeplabcut-0.2.1.6/tox.ini
```

### Comparing `napari-deeplabcut-0.2.1.5/.github/workflows/test_and_deploy.yml` & `napari-deeplabcut-0.2.1.6/.github/workflows/test_and_deploy.yml`

 * *Files 20% similar despite different names*

```diff
@@ -11,29 +11,34 @@
     tags:
       - "v*" # Push events to matching v*, i.e. v1.0, v20.15.10
   pull_request:
     branches:
       - main
       - npe2
   workflow_dispatch:
+    inputs:
+      force_deploy:
+        description: 'Force deployment even if tests fail'
+        required: true
+        type: boolean
 
 jobs:
   test:
     name: ${{ matrix.platform }} py${{ matrix.python-version }}
     runs-on: ${{ matrix.platform }}
     strategy:
       matrix:
         platform: [ubuntu-latest, windows-latest, macos-latest]
         python-version: [3.9, "3.10"]
 
     steps:
       - uses: actions/checkout@v4
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
 
       # these libraries enable testing on Qt on linux
       - uses: tlambert03/setup-qt-libs@v1
 
       # strategy borrowed from vispy for installing opengl libs on windows
@@ -58,23 +63,26 @@
         uses: aganders3/headless-gui@v2
         with:
           run: python -m tox
         env:
           PLATFORM: ${{ matrix.platform }}
 
       - name: Coverage
-        uses: codecov/codecov-action@v2
+        uses: codecov/codecov-action@v4
 
   deploy:
     # this will run when you have tagged a commit, starting with "v*"
     # and requires that you have put your twine API key in your
     # github secrets (see readme for details)
     needs: [test]
     runs-on: ubuntu-latest
-    if: contains(github.ref, 'tags')
+    if: |
+      always() &&
+      inputs.force_deploy ||
+      (contains(github.ref, 'tags') && contains(needs.test.result, 'success'))
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python
         uses: actions/setup-python@v4
         with:
           python-version: "3.x"
       - name: Install dependencies
```

### Comparing `napari-deeplabcut-0.2.1.5/.gitignore` & `napari-deeplabcut-0.2.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/.napari/DESCRIPTION.md` & `napari-deeplabcut-0.2.1.6/.napari/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/.pre-commit-config.yaml` & `napari-deeplabcut-0.2.1.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/CODE_OF_CONDUCT.md` & `napari-deeplabcut-0.2.1.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/LICENSE` & `napari-deeplabcut-0.2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/PKG-INFO` & `napari-deeplabcut-0.2.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-deeplabcut
-Version: 0.2.1.5
+Version: 0.2.1.6
 Summary: napari + DeepLabCut annotation tool
 Home-page: https://github.com/DeepLabCut/napari-deeplabcut
 Author: Team DeepLabCut, Lead by Jessy Lauer
 Author-email: admin@deeplabcut.org
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/DeepLabCut/napari-deeplabcut/issues
 Project-URL: Documentation, https://github.com/DeepLabCut/napari-deeplabcut#README.md
```

### Comparing `napari-deeplabcut-0.2.1.5/README.md` & `napari-deeplabcut-0.2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/docs/index.md` & `napari-deeplabcut-0.2.1.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/setup.cfg` & `napari-deeplabcut-0.2.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/_reader.py` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/_reader.py`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/_tests/conftest.py` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/_tests/test_keypoints.py` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/_tests/test_keypoints.py`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/_tests/test_misc.py` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/_tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/_tests/test_reader.py` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/_tests/test_widgets.py` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/_tests/test_widgets.py`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/_widgets.py` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/_widgets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import os
 from collections import defaultdict, namedtuple
 from copy import deepcopy
 from datetime import datetime
 from functools import partial, cached_property
 from math import ceil, log10
 import matplotlib.pyplot as plt
@@ -50,51 +51,49 @@
 from napari_deeplabcut import keypoints
 from napari_deeplabcut._reader import _load_config
 from napari_deeplabcut._writer import _write_config, _write_image, _form_df
 from napari_deeplabcut.misc import (
     encode_categories,
     to_os_dir_sep,
     guarantee_multiindex_rows,
-    build_color_cycles
+    build_color_cycles,
 )
 
-
 Tip = namedtuple("Tip", ["msg", "pos"])
 
 
 class Shortcuts(QDialog):
+    """Opens a window displaying available napari-deeplabcut shortcuts"""
+
     def __init__(self, parent):
         super().__init__(parent=parent)
         self.setParent(parent)
         self.setWindowTitle("Shortcuts")
 
         image_path = str(Path(__file__).parent / "assets" / "napari_shortcuts.svg")
 
         vlayout = QVBoxLayout()
-        background_widget = QWidget()
-        background_widget.setStyleSheet("background-color: white;")
         svg_widget = QSvgWidget(image_path)
-        vlayout.addWidget(background_widget)
+        svg_widget.setStyleSheet("background-color: white;")
         vlayout.addWidget(svg_widget)
-        vlayout.setContentsMargins(0, 0, 0, 0)
         self.setLayout(vlayout)
 
 
 class Tutorial(QDialog):
     def __init__(self, parent):
         super().__init__(parent=parent)
         self.setParent(parent)
         self.setWindowTitle("Tutorial")
         self.setModal(True)
         self.setStyleSheet("background:#361AE5")
         self.setAttribute(Qt.WA_DeleteOnClose)
         self.setWindowOpacity(0.95)
-        self.setWindowFlags(self.windowFlags() | Qt.FramelessWindowHint)
+        self.setWindowFlags(self.windowFlags() | Qt.WindowCloseButtonHint)
 
-        self._current_tip = 0
+        self._current_tip = -1
         self._tips = [
             Tip(
                 "Load a folder of annotated data\n(and optionally a config file if labeling from scratch)\nfrom the menu File > Open File or Open Folder.\nAlternatively, files and folders of images can be dragged\nand dropped onto the main window.",
                 (0.35, 0.15),
             ),
             Tip(
                 "Data layers will be listed at the bottom left;\ntheir visibility can be toggled by clicking on the small eye icon.",
@@ -114,53 +113,68 @@
             ),
             Tip(
                 "Read more at <a href='https://github.com/DeepLabCut/napari-deeplabcut#usage'>napari-deeplabcut</a>",
                 (0.4, 0.4),
             ),
         ]
 
-        buttons = (
-            QDialogButtonBox.StandardButton.Ok | QDialogButtonBox.StandardButton.Abort
-        )
-        self.button_box = QDialogButtonBox(buttons)
-        self.button_box.accepted.connect(self.accept)
-        self.button_box.rejected.connect(self.reject)
-
         vlayout = QVBoxLayout()
         self.message = QLabel("💡\n\nLet's get started with a quick walkthrough!")
         self.message.setTextInteractionFlags(Qt.LinksAccessibleByMouse)
         self.message.setOpenExternalLinks(True)
         vlayout.addWidget(self.message)
+
+        nav_layout = QHBoxLayout()
+        self.prev_button = QPushButton("<")
+        self.prev_button.clicked.connect(self.prev_tip)
+        nav_layout.addWidget(self.prev_button)
+        self.next_button = QPushButton(">")
+        self.next_button.clicked.connect(self.next_tip)
+        nav_layout.addWidget(self.next_button)
+
+        self.update_nav_buttons()
+
         hlayout = QHBoxLayout()
         self.count = QLabel("")
         hlayout.addWidget(self.count)
-        hlayout.addWidget(self.button_box)
+        hlayout.addLayout(nav_layout)
         vlayout.addLayout(hlayout)
         self.setLayout(vlayout)
 
-    def accept(self):
-        if self._current_tip == 0 and "walkthrough" not in self.message.text():
-            self.reject()
+    def prev_tip(self):
+        self._current_tip = (self._current_tip - 1) % len(self._tips)
+        self.update_tip()
+        self.update_nav_buttons()
+
+    def next_tip(self):
+        self._current_tip = (self._current_tip + 1) % len(self._tips)
+        self.update_tip()
+        self.update_nav_buttons()
+
+    def update_tip(self):
         tip = self._tips[self._current_tip]
         msg = tip.msg
         if (
-            self._current_tip < 5
+            self._current_tip < len(self._tips) - 1
         ):  # No emoji in the last tip otherwise the hyperlink breaks
             msg = "💡\n\n" + msg
         self.message.setText(msg)
         self.count.setText(f"Tip {self._current_tip + 1}|{len(self._tips)}")
         self.adjustSize()
         xrel, yrel = tip.pos
         geom = self.parent().geometry()
         p = QPoint(
             int(geom.left() + geom.width() * xrel),
             int(geom.top() + geom.height() * yrel),
         )
         self.move(p)
-        self._current_tip = (self._current_tip + 1) % len(self._tips)
+
+    def update_nav_buttons(self):
+        self.prev_button.setEnabled(self._current_tip > 0)
+        self.next_button.setEnabled(self._current_tip < len(self._tips) - 1)
 
 
 def _get_and_try_preferred_reader(
     self,
     dialog,
     *args,
 ):
@@ -554,14 +568,15 @@
         welcome_widget = overlay.layout().itemAt(1).widget()
         welcome_widget.deleteLater()
         w = QtWelcomeWidget(None)
         overlay._overlay = w
         overlay.addWidget(w)
         overlay._overlay.sig_dropped.connect(overlay.sig_dropped)
 
+        self._color_mode = keypoints.ColorMode.default()
         self._label_mode = keypoints.LabelMode.default()
 
         # Hold references to the KeypointStores
         self._stores = {}
         # Intercept close event if data were not saved
         self.viewer.window._qt_window.closeEvent = partial(
             on_close,
@@ -573,21 +588,27 @@
         # These are updated anytime images are added to the Viewer
         # and passed on to the other layers upon creation.
         self._images_meta = dict()
 
         # Add some more controls
         self._layout = QVBoxLayout(self)
         self._menus = []
+        self._layer_to_menu = {}
+        self.viewer.layers.selection.events.active.connect(self.on_active_layer_change)
 
         self._video_group = self._form_video_action_menu()
         self.video_widget = self.viewer.window.add_dock_widget(
             self._video_group, name="video", area="right"
         )
         self.video_widget.setVisible(False)
 
+        # form helper display
+        help_buttons = self._form_help_buttons()
+        self._layout.addLayout(help_buttons)
+
         hlayout = QHBoxLayout()
         trail_label = QLabel("Show trails")
         self._trail_cb = QCheckBox()
         self._trail_cb.setToolTip("toggle trails visibility")
         self._trail_cb.setChecked(False)
         self._trail_cb.setEnabled(False)
         self._trail_cb.stateChanged.connect(self._show_trails)
@@ -606,16 +627,19 @@
         hlayout.addWidget(matplotlib_label)
         hlayout.addWidget(self._trail_cb)
         hlayout.addWidget(trail_label)
         hlayout.addWidget(self._view_scheme_cb)
 
         self._layout.addLayout(hlayout)
 
+        # form buttons for selection of annotation mode
         self._radio_group = self._form_mode_radio_buttons()
 
+        # form color scheme display + color mode selector
+        self._color_grp, self._color_mode_selector = self._form_color_mode_selector()
         self._display = ColorSchemeDisplay(parent=self)
         self._color_scheme_display = self._form_color_scheme_display(self.viewer)
         self._view_scheme_cb.toggled.connect(self._show_color_scheme)
         self._view_scheme_cb.toggle()
         self._display.added.connect(
             lambda w: w.part_label.clicked.connect(
                 self._matplotlib_canvas._toggle_line_visibility
@@ -717,14 +741,24 @@
         layout.addWidget(extract_button)
         crop_button = QPushButton("Store crop coordinates")
         crop_button.clicked.connect(self._store_crop_coordinates)
         layout.addWidget(crop_button)
         group_box.setLayout(layout)
         return group_box
 
+    def _form_help_buttons(self):
+        layout = QHBoxLayout()
+        show_shortcuts = QPushButton("View shortcuts")
+        show_shortcuts.clicked.connect(self.display_shortcuts)
+        layout.addWidget(show_shortcuts)
+        tutorial = QPushButton("Start tutorial")
+        tutorial.clicked.connect(self.start_tutorial)
+        layout.addWidget(tutorial)
+        return layout
+
     def _extract_single_frame(self, *args):
         image_layer = None
         points_layer = None
         for layer in self.viewer.layers:
             if isinstance(layer, Image):
                 image_layer = layer
             elif isinstance(layer, Points):
@@ -742,15 +776,15 @@
                 df = _form_df(
                     points_layer.data,
                     {
                         "metadata": points_layer.metadata,
                         "properties": points_layer.properties,
                     },
                 )
-                df = df.iloc[ind : ind + 1]
+                df = df.iloc[ind: ind + 1]
                 df.index = pd.MultiIndex.from_tuples([Path(output_path).parts[-3:]])
                 filepath = os.path.join(
                     image_layer.metadata["root"], "machinelabels-iter0.h5"
                 )
                 if Path(filepath).is_file():
                     df_prev = pd.read_hdf(filepath)
                     guarantee_multiindex_rows(df_prev)
@@ -786,14 +820,15 @@
         menu = KeypointsDropdownMenu(store)
         self.viewer.dims.events.current_step.connect(
             menu.smart_reset,
             position="last",
         )
         menu.smart_reset(event=None)
         self._menus.append(menu)
+        self._layer_to_menu[store.layer] = len(self._menus) - 1
         layout = QVBoxLayout()
         layout.addWidget(menu)
         self._layout.addLayout(layout)
 
     def _form_mode_radio_buttons(self):
         group_box = QGroupBox("Labeling mode")
         layout = QHBoxLayout()
@@ -809,37 +844,58 @@
 
         def _func():
             self.label_mode = group.checkedButton().text()
 
         group.buttonClicked.connect(_func)
         return group
 
+    def _form_color_mode_selector(self):
+        group_box = QGroupBox("Keypoint coloring mode")
+        layout = QHBoxLayout()
+        group = QButtonGroup(self)
+        for i, mode in enumerate(keypoints.ColorMode.__members__, start=1):
+            btn = QRadioButton(mode.lower())
+            group.addButton(btn, i)
+            layout.addWidget(btn)
+        group.button(1).setChecked(True)
+        group_box.setLayout(layout)
+        self._layout.addWidget(group_box)
+
+        def _func():
+            self.color_mode = group.checkedButton().text()
+
+        group.buttonClicked.connect(_func)
+        return group_box, group
+
     def _form_color_scheme_display(self, viewer):
         self.viewer.layers.events.inserted.connect(self._update_color_scheme)
         return viewer.window.add_dock_widget(
             self._display, name="Color scheme reference", area="left"
         )
 
     def _update_color_scheme(self):
         def to_hex(nparray):
             a = np.array(nparray * 255, dtype=int)
             rgb2hex = lambda r, g, b, _: f"#{r:02x}{g:02x}{b:02x}"
             res = rgb2hex(*a)
             return res
 
         self._display.reset()
+        mode = "label"
+        if self.color_mode == str(keypoints.ColorMode.INDIVIDUAL):
+            mode = "id"
+
         for layer in self.viewer.layers:
             if isinstance(layer, Points) and layer.metadata:
-                [
-                    self._display.add_entry(name, to_hex(color))
-                    for name, color in layer.metadata["face_color_cycles"][
-                        "label"
-                    ].items()
-                ]
-                break
+                self._display.update_color_scheme(
+                    {
+                        name: to_hex(color)
+                        for name, color in layer.metadata["face_color_cycles"][mode].items()
+                    }
+                )
 
     def _remap_frame_indices(self, layer):
         if not self._images_meta.get("paths"):
             return
 
         new_paths = [to_os_dir_sep(p) for p in self._images_meta["paths"]]
         paths = layer.metadata.get("paths")
@@ -870,14 +926,15 @@
             else:
                 data[:, 0] = np.vectorize(temp.get)(data[:, 0])
             layer.data = data
         layer.metadata.update(self._images_meta)
 
     def on_insert(self, event):
         layer = event.source[-1]
+        logging.debug(f"Inserting Layer {layer}")
         if isinstance(layer, Image):
             paths = layer.metadata.get("paths")
             if paths is None:  # Then it's a video file
                 self.video_widget.setVisible(True)
             # Store the metadata and pass them on to the other layers
             self._images_meta.update(
                 {
@@ -942,27 +999,28 @@
             self._stores[layer] = store
             # TODO Set default dir of the save file dialog
             if root := layer.metadata.get("root"):
                 update_save_history(root)
             layer.metadata["controls"] = self
             layer.text.visible = False
             layer.bind_key("M", self.cycle_through_label_modes)
+            layer.bind_key("F", self.cycle_through_color_modes)
             func = partial(_paste_data, store=store)
             layer._paste_data = MethodType(func, layer)
             layer.add = MethodType(keypoints._add, store)
             layer.events.add(query_next_frame=Event)
             layer.events.query_next_frame.connect(store._advance_step)
             layer.bind_key("Shift-Right", store._find_first_unlabeled_frame)
             layer.bind_key("Shift-Left", store._find_first_unlabeled_frame)
 
             layer.bind_key("Down", store.next_keypoint, overwrite=True)
             layer.bind_key("Up", store.prev_keypoint, overwrite=True)
             layer.face_color_mode = "cycle"
-            if not self._menus:
-                self._form_dropdown_menus(store)
+            self._form_dropdown_menus(store)
+
             self._images_meta.update(
                 {
                     "project": layer.metadata.get("project"),
                 }
             )
             self._trail_cb.setEnabled(True)
             self._matplotlib_cb.setEnabled(True)
@@ -995,45 +1053,73 @@
                 self._display.reset()
             self._stores.pop(layer, None)
             while self._menus:
                 menu = self._menus.pop()
                 self._layout.removeWidget(menu)
                 menu.deleteLater()
                 menu.destroy()
+            self._layer_to_menu = {}
             self._trail_cb.setEnabled(False)
             self._matplotlib_cb.setEnabled(False)
             self.last_saved_label.hide()
         elif isinstance(layer, Image):
             self._images_meta = dict()
             paths = layer.metadata.get("paths")
             if paths is None:
                 self.video_widget.setVisible(False)
         elif isinstance(layer, Tracks):
             self._trail_cb.setChecked(False)
             self._matplotlib_cb.setChecked(False)
             self._trails = None
 
+    def on_active_layer_change(self, event) -> None:
+        """Updates the GUI when the active layer changes
+            * Hides all KeypointsDropdownMenu that aren't for the selected layer
+            * Sets the visibility of the "Color mode" box to True if the selected layer
+                is a multi-animal one, or False otherwise
+        """
+        self._color_grp.setVisible(self._is_multianimal(event.value))
+        menu_idx = -1
+        if event.value is not None and isinstance(event.value, Points):
+            menu_idx = self._layer_to_menu.get(event.value, -1)
+
+        for idx, menu in enumerate(self._menus):
+            if idx == menu_idx:
+                menu.setHidden(False)
+            else:
+                menu.setHidden(True)
+
     def _update_colormap(self, colormap_name):
-        for layer in self.viewer.layers:
+        for layer in self.viewer.layers.selection:
             if isinstance(layer, Points) and layer.metadata:
                 face_color_cycle_maps = build_color_cycles(
                     layer.metadata["header"], colormap_name,
                 )
                 layer.metadata["face_color_cycles"] = face_color_cycle_maps
-                face_color_prop = layer._face.color_properties.name
+                face_color_prop = "label"
+                if self.color_mode == str(keypoints.ColorMode.INDIVIDUAL):
+                    face_color_prop = "id"
+
                 layer.face_color = face_color_prop
                 layer.face_color_cycle = face_color_cycle_maps[face_color_prop]
                 layer.events.face_color()
                 self._update_color_scheme()
-                break
 
     @register_points_action("Change labeling mode")
     def cycle_through_label_modes(self, *args):
         self.label_mode = next(keypoints.LabelMode)
 
+    @register_points_action("Change color mode")
+    def cycle_through_color_modes(self, *args):
+        if (
+            self._active_layer_is_multianimal()
+            or self.color_mode != str(keypoints.ColorMode.BODYPART)
+        ):
+            self.color_mode = next(keypoints.ColorMode)
+
     @property
     def label_mode(self):
         return str(self._label_mode)
 
     @label_mode.setter
     def label_mode(self, mode: Union[str, keypoints.LabelMode]):
         self._label_mode = keypoints.LabelMode(mode)
@@ -1046,24 +1132,60 @@
             for menu in self._menus:
                 menu._locked = False
         for btn in self._radio_group.buttons():
             if btn.text() == mode_:
                 btn.setChecked(True)
                 break
 
+    @property
+    def color_mode(self):
+        return str(self._color_mode)
 
-@Points.bind_key("F")
-def toggle_face_color(layer):
-    if layer._face.color_properties.name == "id":
-        layer.face_color = "label"
-        layer.face_color_cycle = layer.metadata["face_color_cycles"]["label"]
-    else:
-        layer.face_color = "id"
-        layer.face_color_cycle = layer.metadata["face_color_cycles"]["id"]
-    layer.events.face_color()
+    @color_mode.setter
+    def color_mode(self, mode: Union[str, keypoints.ColorMode]):
+        self._color_mode = keypoints.ColorMode(mode)
+        if self._color_mode == keypoints.ColorMode.BODYPART:
+            face_color_mode = "label"
+        else:
+            face_color_mode = "id"
+
+        for layer in self.viewer.layers:
+            if isinstance(layer, Points) and layer.metadata:
+                layer.face_color = face_color_mode
+                layer.face_color_cycle = layer.metadata["face_color_cycles"][
+                    face_color_mode]
+                layer.events.face_color()
+
+        for btn in self._color_mode_selector.buttons():
+            if btn.text() == str(mode):
+                btn.setChecked(True)
+                break
+
+        self._update_color_scheme()
+
+    def _is_multianimal(self, layer) -> bool:
+        is_multi = False
+        if layer is not None and isinstance(layer, Points):
+            try:
+                header = layer.metadata.get("header")
+                if header is not None:
+                    ids = header.individuals
+                    is_multi = len(ids) > 0 and ids[0] != ""
+            except AttributeError:
+                pass
+
+        return is_multi
+
+    def _active_layer_is_multianimal(self) -> bool:
+        """Returns: whether the active layer is a multi-animal points layer"""
+        for layer in self.viewer.layers.selection:
+            if self._is_multianimal(layer):
+                return True
+
+        return False
 
 
 @Points.bind_key("E")
 def toggle_edge_color(layer):
     # Trick to toggle between 0 and 2
     layer.edge_width = np.bitwise_xor(layer.edge_width, 2)
 
@@ -1410,13 +1532,42 @@
     def add_entry(self, name, color):
         self.scheme_dict.update({name: color})
 
         widget = LabelPair(color, name, self)
         self._layout.addWidget(widget, alignment=Qt.AlignmentFlag.AlignLeft)
         self.added.emit(widget)
 
+    def update_color_scheme(self, new_color_scheme) -> None:
+        logging.debug(f"Updating color scheme: {self._layout.count()} widgets")
+        self.scheme_dict = {name: color for name, color in new_color_scheme.items()}
+        names = list(new_color_scheme.keys())
+        existing_widgets = self._layout.count()
+        required_widgets = len(self.scheme_dict)
+
+        # update existing widgets
+        for idx in range(min(existing_widgets, required_widgets)):
+            logging.debug(f"  updating {idx}")
+            w = self._layout.itemAt(idx).widget()
+            w.setVisible(True)
+            w.part_name = names[idx]
+            w.color = self.scheme_dict[names[idx]]
+
+        # remove extra widgets
+        for i in range(max(existing_widgets - required_widgets, 0)):
+            logging.debug(f"  hiding {required_widgets + i}")
+            if w := self._layout.itemAt(required_widgets + i).widget():
+                logging.debug(f"  done!")
+                w.setVisible(False)
+
+        # add missing widgets
+        for i in range(max(required_widgets - existing_widgets, 0)):
+            logging.debug(f"  adding {existing_widgets + i}")
+            name = names[existing_widgets + i]
+            self.add_entry(name, self.scheme_dict[name])
+        logging.debug(f"  done!")
+
     def reset(self):
         self.scheme_dict = {}
-        for i in reversed(range(self._layout.count())):
+        for i in range(self._layout.count()):
             w = self._layout.itemAt(i).widget()
-            w.setParent(None)
-            self._layout.removeWidget(w)
+            logging.debug(f"making {w} invisible")
+            w.setVisible(False)
```

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/_writer.py` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/_writer.py`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/black/Back.png` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/black/Back.png`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/black/Customize.png` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/black/Customize.png`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/black/Forward.png` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/black/Forward.png`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/black/Home.png` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/black/Home.png`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/black/Pan.png` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/black/Pan.png`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/black/Pan_checked.png` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/black/Pan_checked.png`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/black/Save.png` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/black/Save.png`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/black/Subplots.png` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/black/Subplots.png`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/black/Zoom.png` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/black/Zoom.png`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/black/Zoom_checked.png` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/black/Zoom_checked.png`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/napari_shortcuts.svg` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/napari_shortcuts.svg`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/white/Back.png` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/white/Back.png`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/white/Customize.png` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/white/Customize.png`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/white/Forward.png` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/white/Forward.png`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/white/Home.png` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/white/Home.png`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/white/Pan.png` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/white/Pan.png`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/white/Pan_checked.png` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/white/Pan_checked.png`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/white/Save.png` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/white/Save.png`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/white/Subplots.png` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/white/Subplots.png`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/white/Zoom.png` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/white/Zoom.png`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/assets/white/Zoom_checked.png` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/assets/white/Zoom_checked.png`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/keypoints.py` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/keypoints.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,14 +30,30 @@
     self.layer.events.current_symbol()
 
 
 QtPointsControls.changeCurrentSize = _change_size
 QtPointsControls.changeCurrentSymbol = _change_symbol
 
 
+class ColorMode(CycleEnum):
+    """Modes in which keypoints can be colored
+
+    BODYPART: the keypoints are grouped by bodypart (all bodyparts have the same color)
+    INDIVIDUAL: the keypoints are grouped by individual (all keypoints for the same
+        individual have the same color)
+    """
+
+    BODYPART = auto()
+    INDIVIDUAL = auto()
+
+    @classmethod
+    def default(cls):
+        return cls.BODYPART
+
+
 class LabelMode(CycleEnum):
     """
     Labeling modes.
     SEQUENTIAL: points are placed in sequence, then frame after frame;
         clicking to add an already annotated point has no effect.
     QUICK: similar to SEQUENTIAL, but trying to add an already
         annotated point actually moves it to the cursor location.
```

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/misc.py` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/misc.py`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut/napari.yaml` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut.egg-info/PKG-INFO` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-deeplabcut
-Version: 0.2.1.5
+Version: 0.2.1.6
 Summary: napari + DeepLabCut annotation tool
 Home-page: https://github.com/DeepLabCut/napari-deeplabcut
 Author: Team DeepLabCut, Lead by Jessy Lauer
 Author-email: admin@deeplabcut.org
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/DeepLabCut/napari-deeplabcut/issues
 Project-URL: Documentation, https://github.com/DeepLabCut/napari-deeplabcut#README.md
```

### Comparing `napari-deeplabcut-0.2.1.5/src/napari_deeplabcut.egg-info/SOURCES.txt` & `napari-deeplabcut-0.2.1.6/src/napari_deeplabcut.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari-deeplabcut-0.2.1.5/tox.ini` & `napari-deeplabcut-0.2.1.6/tox.ini`

 * *Files identical despite different names*

