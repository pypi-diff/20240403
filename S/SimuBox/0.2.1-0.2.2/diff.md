# Comparing `tmp/simubox-0.2.1.tar.gz` & `tmp/simubox-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simubox-0.2.1.tar", max compression
+gzip compressed data, was "simubox-0.2.2.tar", max compression
```

## Comparing `simubox-0.2.1.tar` & `simubox-0.2.2.tar`

### file list

```diff
@@ -1,60 +1,103 @@
--rw-r--r--   0        0        0     1093 2023-12-15 10:21:19.938760 simubox-0.2.1/LICENSE
--rw-r--r--   0        0        0     1265 2024-03-27 15:56:28.965480 simubox-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     1041 2024-03-31 14:56:23.293212 simubox-0.2.1/README.md
--rw-r--r--   0        0        0      121 2024-03-27 15:55:02.995962 simubox-0.2.1/SimuBox/__init__.py
--rw-r--r--   0        0        0      123 2023-12-15 06:14:16.190366 simubox-0.2.1/SimuBox/artist/__init__.py
--rw-r--r--   0        0        0    11867 2024-03-27 14:22:19.156738 simubox-0.2.1/SimuBox/artist/compare.py
--rw-r--r--   0        0        0     7517 2024-04-02 10:47:15.385421 simubox-0.2.1/SimuBox/artist/isosurface.py
--rw-r--r--   0        0        0     9899 2024-03-27 14:22:19.169690 simubox-0.2.1/SimuBox/artist/landscape.py
--rw-r--r--   0        0        0    20834 2024-03-27 14:22:19.147653 simubox-0.2.1/SimuBox/artist/phase.py
--rw-r--r--   0        0        0     3939 2024-03-27 06:33:49.453914 simubox-0.2.1/SimuBox/artist/plotter.py
--rw-r--r--   0        0        0       90 2023-12-15 06:14:16.182366 simubox-0.2.1/SimuBox/calculator/__init__.py
--rw-r--r--   0        0        0     4496 2024-03-27 16:21:22.586663 simubox-0.2.1/SimuBox/calculator/peak.py
--rw-r--r--   0        0        0     5485 2024-03-27 15:55:02.982758 simubox-0.2.1/SimuBox/calculator/scatter.py
--rw-r--r--   0        0        0    26322 2024-03-27 15:55:02.975777 simubox-0.2.1/SimuBox/calculator/topo.py
--rw-r--r--   0        0        0    11281 2024-03-27 15:55:02.985758 simubox-0.2.1/SimuBox/calculator/voronoi.py
--rw-r--r--   0        0        0       70 2024-03-27 15:35:53.922506 simubox-0.2.1/SimuBox/runner/__init__.py
--rw-r--r--   0        0        0      175 2023-11-28 10:41:26.055035 simubox-0.2.1/SimuBox/runner/Agents/__init__.py
--rw-r--r--   0        0        0     4272 2023-11-27 15:25:46.282729 simubox-0.2.1/SimuBox/runner/Agents/ABC.py
--rw-r--r--   0        0        0     5195 2024-03-31 14:54:06.173110 simubox-0.2.1/SimuBox/runner/Agents/ABC_ABC.py
--rw-r--r--   0        0        0     4651 2024-03-31 14:54:03.405665 simubox-0.2.1/SimuBox/runner/Agents/BABCB.py
--rw-r--r--   0        0        0     1115 2023-11-27 15:27:54.239348 simubox-0.2.1/SimuBox/runner/Agents/Mask_AB_A.py
--rw-r--r--   0        0        0     1226 2023-11-27 15:27:54.236347 simubox-0.2.1/SimuBox/runner/Agents/Mask_AB_AB.py
--rw-r--r--   0        0        0     2125 2024-03-27 15:38:30.318428 simubox-0.2.1/SimuBox/runner/Agents/MixinModel.py
--rw-r--r--   0        0        0     8023 2024-03-27 15:35:53.930084 simubox-0.2.1/SimuBox/runner/Manager.py
--rw-r--r--   0        0        0    14973 2023-08-31 09:07:40.697135 simubox-0.2.1/SimuBox/runner/Phases.py
--rw-r--r--   0        0        0       91 2024-03-27 06:33:49.409890 simubox-0.2.1/SimuBox/schema/__init__.py
--rw-r--r--   0        0        0      100 2024-03-27 15:28:15.928633 simubox-0.2.1/SimuBox/schema/enums/__init__.py
--rw-r--r--   0        0        0      955 2024-03-27 14:18:43.001269 simubox-0.2.1/SimuBox/schema/enums/MixinEnums.py
--rw-r--r--   0        0        0     1167 2024-03-27 15:27:06.701601 simubox-0.2.1/SimuBox/schema/enums/Modes.py
--rw-r--r--   0        0        0      560 2024-03-27 15:28:15.922643 simubox-0.2.1/SimuBox/schema/enums/OtherEnums.py
--rw-r--r--   0        0        0      525 2024-03-27 15:36:57.283600 simubox-0.2.1/SimuBox/schema/enums/SCFTEnums.py
--rw-r--r--   0        0        0     1787 2024-03-27 14:18:43.242800 simubox-0.2.1/SimuBox/schema/labels.py
--rw-r--r--   0        0        0      168 2024-03-27 15:36:35.497459 simubox-0.2.1/SimuBox/schema/structs/__init__.py
--rw-r--r--   0        0        0     1736 2024-03-27 13:56:42.637867 simubox-0.2.1/SimuBox/schema/structs/ChartElement.py
--rw-r--r--   0        0        0     1556 2024-03-27 13:56:42.621775 simubox-0.2.1/SimuBox/schema/structs/ComputedRes.py
--rw-r--r--   0        0        0     6653 2024-03-31 13:00:07.546755 simubox-0.2.1/SimuBox/schema/structs/DataFile.py
--rw-r--r--   0        0        0      539 2024-03-27 14:10:13.621470 simubox-0.2.1/SimuBox/schema/structs/MixinStructs.py
--rw-r--r--   0        0        0      701 2024-03-27 14:24:08.192720 simubox-0.2.1/SimuBox/schema/structs/OtherStructs.py
--rw-r--r--   0        0        0     1384 2024-03-27 15:33:02.256233 simubox-0.2.1/SimuBox/schema/structs/SCFTStructs.py
--rw-r--r--   0        0        0      349 2024-03-31 13:01:32.188816 simubox-0.2.1/SimuBox/schema/types.py
--rw-r--r--   0        0        0    10088 2024-03-27 16:07:33.010245 simubox-0.2.1/SimuBox/scripts/extractor.py
--rw-r--r--   0        0        0     7048 2023-11-27 14:34:10.698773 simubox-0.2.1/SimuBox/scripts/JSON/ABC_ABC.json
--rw-r--r--   0        0        0     5195 2023-08-31 09:07:40.762862 simubox-0.2.1/SimuBox/scripts/JSON/BABCB.json
--rw-r--r--   0        0        0      762 2024-03-27 15:45:09.773000 simubox-0.2.1/SimuBox/scripts/push_job.py
--rw-r--r--   0        0        0     1177 2024-03-27 16:07:33.006243 simubox-0.2.1/SimuBox/scripts/setenv.py
--rw-r--r--   0        0        0      721 2024-03-27 16:02:20.309904 simubox-0.2.1/SimuBox/scripts/web.py
--rw-r--r--   0        0        0       96 2024-03-30 13:53:03.208828 simubox-0.2.1/SimuBox/toolkits/__init__.py
--rw-r--r--   0        0        0     3090 2024-03-31 07:22:04.791841 simubox-0.2.1/SimuBox/toolkits/function.py
--rw-r--r--   0        0        0    11509 2024-04-02 10:36:17.641981 simubox-0.2.1/SimuBox/toolkits/reader.py
--rw-r--r--   0        0        0     2544 2024-03-31 14:52:59.828684 simubox-0.2.1/SimuBox/toolkits/vector.py
--rw-r--r--   0        0        0     5010 2024-03-31 12:57:09.821763 simubox-0.2.1/SimuBox/toolkits/xmltrans.py
--rw-r--r--   0        0        0     1702 2024-03-27 14:41:55.709897 simubox-0.2.1/SimuBox/web/Homepage.py
--rw-r--r--   0        0        0     7440 2024-03-31 14:46:11.631170 simubox-0.2.1/SimuBox/web/pages/1_Structure.py
--rw-r--r--   0        0        0     8275 2024-03-27 14:42:26.986772 simubox-0.2.1/SimuBox/web/pages/2_Scatter.py
--rw-r--r--   0        0        0     8964 2024-03-27 14:41:55.704414 simubox-0.2.1/SimuBox/web/pages/3_Voronoi.py
--rw-r--r--   0        0        0     6080 2024-03-27 14:41:55.694890 simubox-0.2.1/SimuBox/web/pages/4_Curve.py
--rw-r--r--   0        0        0     7409 2024-03-27 14:41:55.707413 simubox-0.2.1/SimuBox/web/pages/5_Peaks.py
--rw-r--r--   0        0        0     7029 2024-03-27 14:41:55.698889 simubox-0.2.1/SimuBox/web/pages/6_Topology.py
--rw-r--r--   0        0        0     4057 2024-03-27 14:41:55.701413 simubox-0.2.1/SimuBox/web/pages/7_Landscape.py
--rw-r--r--   0        0        0     2533 1970-01-01 00:00:00.000000 simubox-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-12-15 10:21:19.938760 simubox-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1306 2024-04-03 14:57:54.022478 simubox-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     1041 2024-03-31 14:56:23.293212 simubox-0.2.2/README.md
+-rw-r--r--   0        0        0      121 2024-03-27 15:55:02.995962 simubox-0.2.2/SimuBox/__init__.py
+-rw-r--r--   0        0        0      123 2023-12-15 06:14:16.190366 simubox-0.2.2/SimuBox/artist/__init__.py
+-rw-r--r--   0        0        0      349 2023-12-16 12:36:51.060186 simubox-0.2.2/SimuBox/artist/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    16341 2024-03-27 14:37:31.902620 simubox-0.2.2/SimuBox/artist/__pycache__/compare.cpython-311.pyc
+-rw-r--r--   0        0        0    11781 2024-04-03 13:22:01.628417 simubox-0.2.2/SimuBox/artist/__pycache__/isosurface.cpython-311.pyc
+-rw-r--r--   0        0        0    15122 2024-04-03 13:20:27.256228 simubox-0.2.2/SimuBox/artist/__pycache__/landscape.cpython-311.pyc
+-rw-r--r--   0        0        0    28412 2024-04-03 13:48:55.642974 simubox-0.2.2/SimuBox/artist/__pycache__/phase.cpython-311.pyc
+-rw-r--r--   0        0        0     7600 2024-03-27 07:18:20.947746 simubox-0.2.2/SimuBox/artist/__pycache__/plotter.cpython-311.pyc
+-rw-r--r--   0        0        0    11867 2024-03-27 14:22:19.156738 simubox-0.2.2/SimuBox/artist/compare.py
+-rw-r--r--   0        0        0     7517 2024-04-03 10:55:55.772588 simubox-0.2.2/SimuBox/artist/isosurface.py
+-rw-r--r--   0        0        0     9899 2024-04-03 10:55:55.760588 simubox-0.2.2/SimuBox/artist/landscape.py
+-rw-r--r--   0        0        0    23671 2024-04-03 13:48:54.363411 simubox-0.2.2/SimuBox/artist/phase.py
+-rw-r--r--   0        0        0     3939 2024-03-27 06:33:49.453914 simubox-0.2.2/SimuBox/artist/plotter.py
+-rw-r--r--   0        0        0       90 2023-12-15 06:14:16.182366 simubox-0.2.2/SimuBox/calculator/__init__.py
+-rw-r--r--   0        0        0      315 2023-12-16 12:36:50.973187 simubox-0.2.2/SimuBox/calculator/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     8682 2024-04-03 13:22:02.266551 simubox-0.2.2/SimuBox/calculator/__pycache__/peak.cpython-311.pyc
+-rw-r--r--   0        0        0     9168 2024-03-30 13:53:39.106115 simubox-0.2.2/SimuBox/calculator/__pycache__/scatter.cpython-311.pyc
+-rw-r--r--   0        0        0    37861 2024-03-30 13:53:40.051251 simubox-0.2.2/SimuBox/calculator/__pycache__/topo.cpython-311.pyc
+-rw-r--r--   0        0        0    17589 2024-03-30 13:53:37.025659 simubox-0.2.2/SimuBox/calculator/__pycache__/voronoi.cpython-311.pyc
+-rw-r--r--   0        0        0     4478 2024-04-03 10:55:55.752589 simubox-0.2.2/SimuBox/calculator/peak.py
+-rw-r--r--   0        0        0     5485 2024-03-27 15:55:02.982758 simubox-0.2.2/SimuBox/calculator/scatter.py
+-rw-r--r--   0        0        0    26322 2024-03-27 15:55:02.975777 simubox-0.2.2/SimuBox/calculator/topo.py
+-rw-r--r--   0        0        0    11281 2024-03-27 15:55:02.985758 simubox-0.2.2/SimuBox/calculator/voronoi.py
+-rw-r--r--   0        0        0       70 2024-04-03 10:11:34.170669 simubox-0.2.2/SimuBox/runner/__init__.py
+-rw-r--r--   0        0        0      286 2024-04-03 10:35:11.919414 simubox-0.2.2/SimuBox/runner/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    13355 2024-04-03 10:35:11.935246 simubox-0.2.2/SimuBox/runner/__pycache__/manager.cpython-311.pyc
+-rw-r--r--   0        0        0     5176 2024-04-03 10:35:11.926591 simubox-0.2.2/SimuBox/runner/__pycache__/phases.cpython-311.pyc
+-rw-r--r--   0        0        0      175 2023-11-28 10:41:26.055035 simubox-0.2.2/SimuBox/runner/agents/__init__.py
+-rw-r--r--   0        0        0      473 2023-12-16 12:36:53.403339 simubox-0.2.2/SimuBox/runner/agents/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4294 2023-12-16 12:36:53.405338 simubox-0.2.2/SimuBox/runner/agents/__pycache__/ABC.cpython-311.pyc
+-rw-r--r--   0        0        0     5690 2024-04-03 10:35:11.929260 simubox-0.2.2/SimuBox/runner/agents/__pycache__/ABC_ABC.cpython-311.pyc
+-rw-r--r--   0        0        0     4864 2024-04-03 10:35:11.931247 simubox-0.2.2/SimuBox/runner/agents/__pycache__/BABCB.cpython-311.pyc
+-rw-r--r--   0        0        0     1727 2023-12-16 12:36:53.420340 simubox-0.2.2/SimuBox/runner/agents/__pycache__/Mask_AB_A.cpython-311.pyc
+-rw-r--r--   0        0        0     1863 2023-12-16 12:36:53.421338 simubox-0.2.2/SimuBox/runner/agents/__pycache__/Mask_AB_AB.cpython-311.pyc
+-rw-r--r--   0        0        0     5531 2024-04-03 10:35:11.923591 simubox-0.2.2/SimuBox/runner/agents/__pycache__/MixinModel.cpython-311.pyc
+-rw-r--r--   0        0        0     4272 2023-11-27 15:25:46.282729 simubox-0.2.2/SimuBox/runner/agents/ABC.py
+-rw-r--r--   0        0        0     5250 2024-04-03 10:14:35.582991 simubox-0.2.2/SimuBox/runner/agents/ABC_ABC.py
+-rw-r--r--   0        0        0     4707 2024-04-03 10:15:02.275022 simubox-0.2.2/SimuBox/runner/agents/BABCB.py
+-rw-r--r--   0        0        0     1115 2023-11-27 15:27:54.239348 simubox-0.2.2/SimuBox/runner/agents/Mask_AB_A.py
+-rw-r--r--   0        0        0     1226 2023-11-27 15:27:54.236347 simubox-0.2.2/SimuBox/runner/agents/Mask_AB_AB.py
+-rw-r--r--   0        0        0     2125 2024-04-03 10:11:34.173663 simubox-0.2.2/SimuBox/runner/agents/MixinModel.py
+-rw-r--r--   0        0        0     8023 2024-03-27 15:35:53.930084 simubox-0.2.2/SimuBox/runner/manager.py
+-rw-r--r--   0        0        0    14973 2023-08-31 09:07:40.697135 simubox-0.2.2/SimuBox/runner/phases.py
+-rw-r--r--   0        0        0       91 2024-03-27 06:33:49.409890 simubox-0.2.2/SimuBox/schema/__init__.py
+-rw-r--r--   0        0        0      312 2024-03-27 07:17:01.284000 simubox-0.2.2/SimuBox/schema/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1641 2024-03-27 14:36:51.896843 simubox-0.2.2/SimuBox/schema/__pycache__/labels.cpython-311.pyc
+-rw-r--r--   0        0        0      797 2024-04-03 13:20:26.787918 simubox-0.2.2/SimuBox/schema/__pycache__/types.cpython-311.pyc
+-rw-r--r--   0        0        0      100 2024-03-27 15:28:15.928633 simubox-0.2.2/SimuBox/schema/enums/__init__.py
+-rw-r--r--   0        0        0      329 2024-03-27 15:35:54.898985 simubox-0.2.2/SimuBox/schema/enums/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2672 2024-03-27 14:36:51.220564 simubox-0.2.2/SimuBox/schema/enums/__pycache__/MixinEnums.cpython-311.pyc
+-rw-r--r--   0        0        0     2492 2024-03-27 15:35:54.901985 simubox-0.2.2/SimuBox/schema/enums/__pycache__/Modes.cpython-311.pyc
+-rw-r--r--   0        0        0     1503 2024-03-27 15:35:54.904985 simubox-0.2.2/SimuBox/schema/enums/__pycache__/OtherEnums.cpython-311.pyc
+-rw-r--r--   0        0        0     1374 2024-03-27 15:38:31.041914 simubox-0.2.2/SimuBox/schema/enums/__pycache__/SCFTEnums.cpython-311.pyc
+-rw-r--r--   0        0        0      955 2024-03-27 14:18:43.001269 simubox-0.2.2/SimuBox/schema/enums/MixinEnums.py
+-rw-r--r--   0        0        0     1167 2024-03-27 15:27:06.701601 simubox-0.2.2/SimuBox/schema/enums/Modes.py
+-rw-r--r--   0        0        0      560 2024-03-27 15:28:15.922643 simubox-0.2.2/SimuBox/schema/enums/OtherEnums.py
+-rw-r--r--   0        0        0      525 2024-03-27 15:36:57.283600 simubox-0.2.2/SimuBox/schema/enums/SCFTEnums.py
+-rw-r--r--   0        0        0     1787 2024-03-27 14:18:43.242800 simubox-0.2.2/SimuBox/schema/labels.py
+-rw-r--r--   0        0        0      168 2024-03-27 15:36:35.497459 simubox-0.2.2/SimuBox/schema/structs/__init__.py
+-rw-r--r--   0        0        0      407 2024-03-27 15:38:31.043914 simubox-0.2.2/SimuBox/schema/structs/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3863 2024-03-27 14:36:51.620609 simubox-0.2.2/SimuBox/schema/structs/__pycache__/ChartElement.cpython-311.pyc
+-rw-r--r--   0        0        0     4110 2024-03-27 14:36:51.628615 simubox-0.2.2/SimuBox/schema/structs/__pycache__/ComputedRes.cpython-311.pyc
+-rw-r--r--   0        0        0    11753 2024-03-31 13:25:05.993963 simubox-0.2.2/SimuBox/schema/structs/__pycache__/DataFile.cpython-311.pyc
+-rw-r--r--   0        0        0     1499 2024-03-27 14:36:51.229567 simubox-0.2.2/SimuBox/schema/structs/__pycache__/MixinStructs.cpython-311.pyc
+-rw-r--r--   0        0        0     1517 2024-04-03 13:53:57.781385 simubox-0.2.2/SimuBox/schema/structs/__pycache__/OtherStructs.cpython-311.pyc
+-rw-r--r--   0        0        0     2767 2024-03-27 15:35:57.965475 simubox-0.2.2/SimuBox/schema/structs/__pycache__/SCFTStructs.cpython-311.pyc
+-rw-r--r--   0        0        0     1736 2024-03-27 13:56:42.637867 simubox-0.2.2/SimuBox/schema/structs/ChartElement.py
+-rw-r--r--   0        0        0     1556 2024-03-27 13:56:42.621775 simubox-0.2.2/SimuBox/schema/structs/ComputedRes.py
+-rw-r--r--   0        0        0     6653 2024-03-31 13:00:07.546755 simubox-0.2.2/SimuBox/schema/structs/DataFile.py
+-rw-r--r--   0        0        0      539 2024-03-27 14:10:13.621470 simubox-0.2.2/SimuBox/schema/structs/MixinStructs.py
+-rw-r--r--   0        0        0      724 2024-04-03 13:53:56.680819 simubox-0.2.2/SimuBox/schema/structs/OtherStructs.py
+-rw-r--r--   0        0        0     1384 2024-03-27 15:33:02.256233 simubox-0.2.2/SimuBox/schema/structs/SCFTStructs.py
+-rw-r--r--   0        0        0      395 2024-04-03 11:46:43.830219 simubox-0.2.2/SimuBox/schema/types.py
+-rw-r--r--   0        0        0     1376 2024-03-30 13:54:41.972260 simubox-0.2.2/SimuBox/scripts/__pycache__/web.cpython-311.pyc
+-rw-r--r--   0        0        0    10088 2024-03-27 16:07:33.010245 simubox-0.2.2/SimuBox/scripts/extractor.py
+-rw-r--r--   0        0        0     7048 2023-11-27 14:34:10.698773 simubox-0.2.2/SimuBox/scripts/JSON/ABC_ABC.json
+-rw-r--r--   0        0        0     5195 2023-08-31 09:07:40.762862 simubox-0.2.2/SimuBox/scripts/JSON/BABCB.json
+-rw-r--r--   0        0        0      762 2024-03-27 15:45:09.773000 simubox-0.2.2/SimuBox/scripts/push_job.py
+-rw-r--r--   0        0        0     1177 2024-03-27 16:07:33.006243 simubox-0.2.2/SimuBox/scripts/setenv.py
+-rw-r--r--   0        0        0      721 2024-03-27 16:02:20.309904 simubox-0.2.2/SimuBox/scripts/web.py
+-rw-r--r--   0        0        0       96 2024-03-30 13:53:03.208828 simubox-0.2.2/SimuBox/toolkits/__init__.py
+-rw-r--r--   0        0        0      319 2024-03-30 13:53:34.064029 simubox-0.2.2/SimuBox/toolkits/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5824 2024-04-03 13:53:57.785384 simubox-0.2.2/SimuBox/toolkits/__pycache__/function.cpython-311.pyc
+-rw-r--r--   0        0        0    18649 2024-04-03 13:20:25.500768 simubox-0.2.2/SimuBox/toolkits/__pycache__/reader.cpython-311.pyc
+-rw-r--r--   0        0        0     3360 2024-03-31 14:54:12.302611 simubox-0.2.2/SimuBox/toolkits/__pycache__/vector.cpython-311.pyc
+-rw-r--r--   0        0        0     9742 2024-04-03 10:35:08.059803 simubox-0.2.2/SimuBox/toolkits/__pycache__/xmltrans.cpython-311.pyc
+-rw-r--r--   0        0        0     3786 2024-04-03 13:52:28.451854 simubox-0.2.2/SimuBox/toolkits/function.py
+-rw-r--r--   0        0        0    12058 2024-04-03 12:27:05.411475 simubox-0.2.2/SimuBox/toolkits/reader.py
+-rw-r--r--   0        0        0     2544 2024-03-31 14:52:59.828684 simubox-0.2.2/SimuBox/toolkits/vector.py
+-rw-r--r--   0        0        0     5008 2024-04-03 03:44:10.626375 simubox-0.2.2/SimuBox/toolkits/xmltrans.py
+-rw-r--r--   0        0        0    74833 2024-03-31 14:46:18.268516 simubox-0.2.2/SimuBox/web/cache/iso3d_NaCl_phin_0.svg
+-rw-r--r--   0        0        0     1702 2024-03-27 14:41:55.709897 simubox-0.2.2/SimuBox/web/Homepage.py
+-rw-r--r--   0        0        0     7440 2024-03-31 14:46:11.631170 simubox-0.2.2/SimuBox/web/pages/1_Structure.py
+-rw-r--r--   0        0        0     8275 2024-03-27 14:42:26.986772 simubox-0.2.2/SimuBox/web/pages/2_Scatter.py
+-rw-r--r--   0        0        0     8964 2024-03-27 14:41:55.704414 simubox-0.2.2/SimuBox/web/pages/3_Voronoi.py
+-rw-r--r--   0        0        0     6080 2024-03-27 14:41:55.694890 simubox-0.2.2/SimuBox/web/pages/4_Curve.py
+-rw-r--r--   0        0        0     7409 2024-03-27 14:41:55.707413 simubox-0.2.2/SimuBox/web/pages/5_Peaks.py
+-rw-r--r--   0        0        0     7029 2024-03-27 14:41:55.698889 simubox-0.2.2/SimuBox/web/pages/6_Topology.py
+-rw-r--r--   0        0        0     4057 2024-03-27 14:41:55.701413 simubox-0.2.2/SimuBox/web/pages/7_Landscape.py
+-rw-r--r--   0        0        0     2615 1970-01-01 00:00:00.000000 simubox-0.2.2/PKG-INFO
```

### Comparing `simubox-0.2.1/LICENSE` & `simubox-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/pyproject.toml` & `simubox-0.2.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "SimuBox"
-version = "0.2.01"
+version = "0.2.2"
 description = "Free python package to do some science calculation."
 authors = ["Alkaid Yuan <kryuan@qq.com>"]
 maintainers = ["Alkaid Yuan <kryuan@qq.com>"]
 license = "./LICENSE"
 readme = "./README.md"
 repository  = "https://github.com/KangruiYuan/SimuBox"
 homepage = "https://pypi.org/project/SimuBox/"
@@ -26,14 +26,16 @@
 sympy = "^1.12"
 poetry-plugin-export = "^1.6.0"
 streamlit-nested-layout = "^0.1.1"
 streamlit-extras = "^0.3.6"
 pydantic = "^2.5.2"
 opencv-python = "^4.8.1.78"
 opencv-python-headless = "^4.8.1.78"
+plotly = "^5.20.0"
+pyecharts = "^2.0.5"
 
 [tool.poetry.group.dev.dependencies]
 streamlit-echarts = "^0.4.0"
 plotly = "^5.18.0"
 openpyxl = "^3.1.2"
 
 [build-system]
```

### Comparing `simubox-0.2.1/README.md` & `simubox-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/artist/compare.py` & `simubox-0.2.2/SimuBox/artist/compare.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/artist/isosurface.py` & `simubox-0.2.2/SimuBox/artist/isosurface.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import matplotlib as mpl
 import matplotlib.pyplot as plt
 import numpy as np
 import pyvista as pv
 from skimage.measure import marching_cubes
 
 from .plotter import plot_savefig
-from ..schema import Density, Numeric, PathLike, DensityParseResult
+from ..schema import Density, RealNum, PathLike, DensityParseResult
 from ..toolkits import parse_density
 
 __all__ = ["iso2D", "iso3D"]
 
 def iso3D(
     density: Union[Density, DensityParseResult],
     target: Optional[Union[int, Iterable[int]]] = 0,
@@ -94,23 +94,23 @@
         ax.plot_trisurf(vert[:, 0], vert[:, 1], faces, vert[:, 2], lw=1)
         plt.show()
         return fig, ax
 
 
 def iso2D(
     density: Union[Density, DensityParseResult],
-    target: Optional[Union[int, Iterable[int]], str] = 0,
+    target: Optional[Union[int, Iterable[int], str]] = 0,
     permute: Optional[Iterable[int]] = None,
     slices: Optional[tuple[int, int]] = None,
     titles: Optional[Sequence[str]] = None,
     grid: Optional[Sequence[int]] = None,
-    figsize: Optional[Sequence[Numeric]] = None,
-    aspect: Optional[Numeric] = None,
-    norm: Union[Tuple[Numeric, Numeric], List[Tuple[Numeric, Numeric]]] = None,
-    scale: Union[Tuple[Numeric, Numeric], List[Tuple[Numeric, Numeric]]] = None,
+    figsize: Optional[Sequence[RealNum]] = None,
+    aspect: Optional[RealNum] = None,
+    norm: Union[Tuple[RealNum, RealNum], List[Tuple[RealNum, RealNum]]] = None,
+    scale: Union[Tuple[RealNum, RealNum], List[Tuple[RealNum, RealNum]]] = None,
     cmap: str = "jet",
     label: bool = True,
     colorbar: bool = False,
     interactive: bool = True,
     save: Union[PathLike, bool] = False,
     fontsize: int = 25,
     verbose: bool = False,
```

### Comparing `simubox-0.2.1/SimuBox/artist/landscape.py` & `simubox-0.2.2/SimuBox/artist/landscape.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from scipy.interpolate import griddata
 from shapely.geometry import Polygon
 
 from .plotter import plot_locators, plot_savefig
-from ..schema import LandscapeResult, PathLike, CommonLabels, Numeric, Vector, Contour
+from ..schema import LandscapeResult, PathLike, CommonLabels, RealNum, Vector, Contour
 from ..toolkits import read_csv, find_nearest_1d
 
 LAND_PLOT_CONFIG = {
     "font.family": "Times New Roman",
     "font.size": 16,
     "mathtext.fontset": "stix",
     "font.serif": ["SimSun"],
@@ -84,15 +84,15 @@
         x_axis: str = "ly",
         y_axis: str = "lz",
         target: str = "freeE",
         levels: Optional[Vector] = None,
         precision: int = -3,
         save: Optional[bool] = True,
         tick_num: Optional[int] = None,
-        aspect: Union[Literal["auto", "equal", "square"], Numeric] = 1,
+        aspect: Union[Literal["auto", "equal", "square"], RealNum] = 1,
         relative: bool = True,
         IQ: bool = True,
         interactive: bool = True,
         data: Optional[pd.DataFrame] = None,
         **kwargs,
     ):
         df: pd.DataFrame = self.data(**kwargs) if data is None else data.copy()
```

### Comparing `simubox-0.2.1/SimuBox/artist/phase.py` & `simubox-0.2.2/SimuBox/artist/phase.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,33 @@
 from collections import ChainMap
 from pathlib import Path
-from typing import Any, Optional, Union
+from typing import Any, Optional, Union, Sequence
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
+
 from numpy.polynomial import Chebyshev
 from scipy.io import loadmat
 
-from .plotter import plot_locators, plot_savefig, generate_colors
-from ..schema import DetectionMode, PhaseCompareResult, Point, CommonLabels, PathLike
+from .plotter import plot_locators, plot_savefig, plot_legend, generate_colors
+from ..schema import (
+    DetectionMode,
+    PhaseCompareResult,
+    Point,
+    CommonLabels,
+    PathLike,
+    Operation,
+    RealNum,
+    ColorMode,
+)
 from ..toolkits import read_csv
 
+__all__ = ["PHASE_PLOT_CONFIG", "PhaseDiagram"]
+
 PHASE_PLOT_CONFIG = {
     "font.family": "Times New Roman",
     "font.serif": ["SimSun"],
     "font.size": 16,
     "mathtext.fontset": "stix",
     "axes.unicode_minus": False,
     "xtick.direction": "in",
@@ -43,129 +55,166 @@
         self,
         path: PathLike,
         xlabel: str,
         ylabel: str,
         colors: Optional[dict] = None,
         labels: Optional[dict] = None,
     ) -> None:
+        """
+        初始化对象。
+
+        :param path: 存放一系列相图文件(.csv)的文件夹路径。
+        :param xlabel: 相图横轴数值对应的列名。
+        :param ylabel: 相图纵轴数值对应的列名。
+        :param colors: 各相结构在绘制时的颜色。
+        :param labels: 各标签的姓名映射，如{"tau": r"$\tau$"}，即在渲染时将tau渲染为τ
+        """
         self.path = Path(path)
         self.colors = colors if colors is not None else {}
         self.labels = (
             ChainMap(labels, CommonLabels) if labels is not None else CommonLabels
         )
         self.xlabel = xlabel
         self.ylabel = ylabel
 
-    def query_point(
+    def query(
         self,
-        data: pd.DataFrame,
-        xval: Optional[Union[float, str, int]] = None,
-        yval: Optional[Union[float, str, int]] = None,
+        data: Union[pd.DataFrame, PathLike],
+        x: Optional[Union[float, str, int]] = None,
+        y: Optional[Union[float, str, int]] = None,
         **kwargs,
     ):
-        res = data.copy()
+        """
+        对表格数据进行快速筛选
+
+        :param data:
+        :param x:
+        :param y:
+        :param kwargs:
+        :return:
+        """
+        if isinstance(data, pd.DataFrame):
+            res = data.copy()
+        else:
+            res = read_csv(data)
+        if x:
+            res = res[res[self.xlabel] == x]
+        if y:
+            res = res[res[self.ylabel] == y]
+
         columns = res.columns
-        if xval:
-            res = res[res[self.xlabel] == xval]
-        if yval:
-            res = res[res[self.ylabel] == yval]
         for key, val in kwargs.items():
             if key in columns:
                 res = res[res[key] == val]
         return res
 
     @staticmethod
-    def checkin(phase: list, candidates: list):
-        if len(phase) == 0:
+    def checkin(phases: Sequence, candidates: Sequence):
+        """
+        检查相结构是否属于备选结构。
+
+        :param phases:
+        :param candidates:
+        :return:
+        """
+        if len(phases) == 0:
             return False
-        for i in phase:
+        for i in phases:
             if i in candidates:
                 return True
         return False
 
     def compare(
         self,
-        name: Optional[str] = None,
-        path: Optional[Union[str, Path]] = None,
+        path: PathLike,
         plot: bool = True,
-        acc: int = 3,
+        accuracy: int = 3,
         xlabel: Optional[str] = None,
         ylabel: Optional[str] = None,
+        verbose: bool = True,
+        operation: Optional[Union[Operation, Sequence[Operation]]] = None,
+        subset: Optional[Union[str, Sequence[str]]] = ("phase", "freeE"),
+        figsize: Union[Sequence[int]] = (8, 6),
+        interactive: bool = True,
         **kwargs,
     ):
-        if path is None:
-            assert name is not None
-            path = (self.path / name).with_suffix(".csv")
-        else:
-            if not isinstance(path, Path):
-                path = Path(path)
+        if not isinstance(path, Path):
+            path = Path(path)
+        if not path.is_file():
+            path = self.path / path
+            if not path.is_file():
+                if path.with_suffix(".csv").is_file():
+                    path = path.with_suffix(".csv")
+                elif path.with_suffix(".xlsx").is_file():
+                    path = path.with_suffix(".xlsx")
+                else:
+                    raise ValueError(f"请输入正确的文件名或者路径信息。{str(path)}不存在")
 
-        df = read_csv(path=path, acc=acc, **kwargs)
-        print(f"Include phase: {set(df['phase'].values)}")
+        df = read_csv(
+            path=path, accuracy=accuracy, operation=operation, subset=subset, **kwargs
+        )
+        if verbose:
+            print(f"包括相结构: {set(df['phase'].values)}")
 
         phase_map = dict()
         xlabel = xlabel if xlabel is not None else self.xlabel
         ylabel = ylabel if ylabel is not None else self.ylabel
         y_set = np.sort(df[ylabel].unique())
         x_set = np.sort(df[xlabel].unique())
 
-        exclude = kwargs.get("exclude", [])
+        exclude = kwargs.get("exclude", ())
+        sqrt3 = np.around(np.sqrt(3), decimals=accuracy)
+        sqrt2 = np.around(np.sqrt(2), decimals=accuracy)
 
         mat = np.zeros((len(y_set), len(x_set)), dtype=Point)
         for i, y in enumerate(y_set):
             for j, x in enumerate(x_set):
                 phase = "unknown"
                 temp_data = df[(df[ylabel] == y) & (df[xlabel] == x)]
                 min_data = temp_data[temp_data["freeE"] == temp_data["freeE"].min()]
                 if len(min_data) == 0:
                     continue
                 freeE = min_data["freeE"].min()
                 min_label = min_data["phase"].unique()
                 lxly = min_data["lxly"].unique()
-                lylx = np.around(1 / lxly, acc)
+                lylx = np.around(1 / lxly, accuracy)
                 lylz = min_data["lylz"].unique()
-                lzly = np.around(1 / lylz, acc)
+                lzly = np.around(1 / lylz, accuracy)
 
-                if self.checkin(exclude, min_label):
+                if self.checkin(min_label, exclude):
                     phase = min_label[0]
                 elif "L" in min_label:
                     phase = "L"
-                elif self.checkin(["C4", "Crect"], min_label):
-                    if any(lylz == 1):
+                elif self.checkin(min_label, ["C4", "Crect"]):
+                    if any(lylz == 1) or any(lylx == 1):
                         phase = "C4"
                     else:
                         phase = "Crect"
                 elif len(min_label) == 1:
-                    if self.checkin(["C6", "C3"], min_label):
-                        if lylz == np.around(np.sqrt(3), acc) or lzly == np.around(
-                            1 / np.sqrt(3), acc
-                        ):
+                    if self.checkin(min_label, ["C6", "C3"]):
+                        if sqrt3 in [lylz, lzly, lxly, lylx]:
                             phase = min_label[0]
-                    elif self.checkin(["iHPa"], min_label):
-                        if lxly == np.around(np.sqrt(3), acc) or lylx == np.around(
-                            1 / np.sqrt(3), acc
-                        ):
+                    elif self.checkin(min_label, ["iHPa"]):
+                        if sqrt3 in [lylz, lzly, lxly, lylx]:
                             phase = "iHPa"
-                        elif lylz == np.around(np.sqrt(2), acc) or lxly == 1:
+                        elif sqrt2 in [lylz, lzly, lxly, lylx]:
                             phase = "SC"
                     elif "PL" in min_label:
-                        if lxly == np.around(np.sqrt(3), acc) or lylx == np.around(
-                            1 / np.sqrt(3), acc
-                        ):
+                        if sqrt3 in [lylz, lzly, lxly, lylx]:
                             phase = "PL"
-                    elif self.checkin(["L", "Disorder", "O70"], min_label):
+                    elif self.checkin(min_label, ["L", "Disorder", "O70"]):
                         phase = min_label[0]
                     elif self.checkin(
-                        ["SC", "SG", "DG", "BCC", "FCC", "sdgn"], min_label
+                        min_label, ["SC", "SG", "DG", "BCC", "FCC", "sdgn"]
                     ):
                         if lxly == 1 and lylz == 1:
                             phase = min_label[0]
                     else:
                         phase = "_".join([phase, min_label[0]])
-                mat[i][j] = Point(phase=phase, x=x, y=y, value=freeE)
+                mat[i][j] = Point(label=phase, x=x, y=y, value=freeE)
                 if phase in phase_map:
                     for attr, val in zip(
                         [xlabel, ylabel, "freeE", "lylz", "lxly"],
                         [x, y, freeE, lylz, lxly],
                     ):
                         phase_map[phase][attr].append(val)
                 else:
@@ -176,109 +225,170 @@
                         "lylz": [lylz],
                         "lxly": [lxly],
                     }
 
         comp_res = PhaseCompareResult(data=df, phase_map=phase_map, mat=mat)
 
         if plot:
-            fig, ax = plt.subplots(1, 1, figsize=(8, 6))
+            fig, ax = plt.subplots(1, 1, figsize=figsize)
             for key, value in phase_map.items():
                 if key not in self.colors:
-                    self.colors[key] = generate_colors(mode="HEX")[0]
+                    self.colors[key] = generate_colors(mode=ColorMode.HEX)[0]
                 ax.scatter(
                     value[xlabel],
                     value[ylabel],
                     c=self.colors[key],
                     label=key,
                 )
             ax.tick_params(top="on", right="on", which="both")
             ax.tick_params(which="both", width=2, length=4, direction="in")
             plot_locators(**kwargs)
-            ax.set_xlabel(
-                self.labels.get(xlabel, xlabel), fontdict={"size": 20}
-            )
-            ax.set_ylabel(
-                self.labels.get(ylabel, ylabel), fontdict={"size": 20}
+            ax.set_xlabel(self.labels.get(xlabel, xlabel), fontdict={"size": 20})
+            ax.set_ylabel(self.labels.get(ylabel, ylabel), fontdict={"size": 20})
+            plot_legend(
+                legend=kwargs.get(
+                    "legend",
+                    {
+                        "mode": "outside",
+                        "loc": "upper left",
+                        "bbox_to_anchor": (0.98, 0.8),
+                    },
+                )
             )
-            ax.legend(frameon=False, loc="upper left", bbox_to_anchor=(0.98, 0.8))
             fig.tight_layout()
             comp_res.fig = fig
             comp_res.ax = ax
+            if not interactive:
+                plt.show()
 
         return comp_res
 
     @staticmethod
-    def cross_point(x1, y1, x2, y2, x3, y3, x4, y4):
+    def cross_point(
+        x1: RealNum,
+        y1: RealNum,
+        x2: RealNum,
+        y2: RealNum,
+        x3: RealNum,
+        y3: RealNum,
+        x4: RealNum,
+        y4: RealNum,
+    ):
+        """
+        两点确定直线，计算两条直线之间的交点。
+        (x1, y1), (x2, y2)为第一条直线的两点。
+        (x3, y3), (x4, y4)为第二条直线的两点。
+        y一般对应自由能的数值。
+
+        :param x1:
+        :param y1:
+        :param x2:
+        :param y2:
+        :param x3:
+        :param y3:
+        :param x4:
+        :param y4:
+        :return:
+        """
         b1 = (y2 - y1) * x1 + (x1 - x2) * y1
         b2 = (y4 - y3) * x3 + (x3 - x4) * y3
         D = (x2 - x1) * (y4 - y3) - (x4 - x3) * (y2 - y1)
         D1 = b2 * (x2 - x1) - b1 * (x4 - x3)
         D2 = b2 * (y2 - y1) - b1 * (y4 - y3)
         return D1 / D, D2 / D
 
     @staticmethod
     def de_unknown(comp_res: PhaseCompareResult):
+        """
+        将相结构名称前缀中的unknown去掉。
+
+        :param comp_res:
+        :return:
+        """
         mat = comp_res.mat
         for i in range(mat.shape[0]):
             for j in range(mat.shape[1]):
                 try:
-                    mat[i][j].label = mat[i][j].label.lstrip("unknown_")
+                    new_label = mat[i][j].label.lstrip("unknown_")
+                    if new_label == "":
+                        mat[i][j] = 0
+                    else:
+                        mat[i][j].label = new_label
                 except AttributeError:
                     continue
         comp_res.mat = mat
         return comp_res
 
-    def scan(self, folder: Optional[Union[str, Path]] = None, **kwargs):
-        if folder is not None:
-            if isinstance(folder, str):
-                folder = Path(folder)
+    def scan(
+        self,
+        path: Optional[Union[str, Path]] = None,
+        filetype: Sequence[str] = (".csv"),
+        figsize: Union[Sequence[int]] = (8, 8),
+        skip: Sequence[str] = (),
+        extract: Sequence[str] = (),
+        inverse: Sequence[str] = (),
+        deunknown: Sequence[str] = (),
+        annotation: Optional[dict] = None,
+        verbose: bool = True,
+        **kwargs,
+    ):
+        if annotation is None:
+            annotation = {}
+
+        if path is not None:
+            if isinstance(path, str):
+                path = Path(path)
+                assert path.is_dir()
         else:
-            folder = self.path
+            path = self.path
 
-        filelist = list(folder.glob("*.csv"))
-        fig, ax = plt.subplots(figsize=kwargs.get("figsize", (8, 6)))
-        skip: list[str] = kwargs.get("skip", [])
-        extract: list[str] = kwargs.get("extract", [])
-        inverse_lst: list[str] = kwargs.get("inverse", [])
-        deunknown: list[str] = kwargs.get("deunknown", [])
-        ann_dict: dict[str, Any] = kwargs.get("annotation", {})
+        filelist = []
+        for ft in filetype:
+            filelist += list(path.glob("*" + ft))
 
+        fig, ax = plt.subplots(figsize=figsize)
         for filename in filelist:
             tmp_name = filename.stem
-            tmp_dict: dict = ann_dict.get(tmp_name, {})
-            print(tmp_name, end="\t")
+            tmp_dict: dict = annotation.get(tmp_name, {})
+            if verbose:
+                print(tmp_name, end="\t")
             if tmp_name in skip:
-                print("Skip...")
+                if verbose:
+                    print("Skip...")
                 continue
             else:
                 comp_res = self.compare(
-                    path=filename, plot=False, acc=tmp_dict.get("acc", 2)
+                    path=filename, plot=False, accuracy=tmp_dict.get("acc", 2)
                 )
 
             if tmp_name in deunknown or deunknown == "All":
                 comp_res = self.de_unknown(comp_res)
 
             if tmp_name in extract:
+                # print("Extracting.")
                 tmp_xys = self.extract_edge(comp_res.mat, **tmp_dict)
             else:
-                # tmp_xys = self.boundary(comp_res.df, comp_res.mat, mode=["hori", "ver"])
                 tmp_xys = self.boundary_detect(comp_res, **tmp_dict)
 
-            if tmp_name in inverse_lst:
-                tmp_xys = tmp_xys[np.argsort(tmp_xys[:, 1])]
-                self.draw_line(tmp_xys, ax=ax, annotation=tmp_dict, inverse=True)
-            else:
-                tmp_xys = tmp_xys[np.argsort(tmp_xys[:, 0])]
-                self.draw_line(tmp_xys, ax=ax, annotation=tmp_dict)
+            try:
+                if tmp_name in inverse:
+                    tmp_xys = tmp_xys[np.argsort(tmp_xys[:, 1])]
+                    self.draw_line(tmp_xys, ax=ax, annotation=tmp_dict, inverse=True)
+                else:
+                    tmp_xys = tmp_xys[np.argsort(tmp_xys[:, 0])]
+                    self.draw_line(tmp_xys, ax=ax, annotation=tmp_dict)
+            except IndexError as ie:
+                print(tmp_xys)
+                raise ie
 
-        if phase_name := ann_dict.get("phase_name", ()):
+        if phase_name := annotation.get("phase_name", ()):
             for name, _x, _y in phase_name:
                 ax.text(_x, _y, name, fontsize=20, color="k")
 
-        if phase_name_arrow := ann_dict.get("phase_name_arrow", ()):
+        if phase_name_arrow := annotation.get("phase_name_arrow", ()):
             for name, _x, _y, _text_x, _text_y in phase_name_arrow:
                 ax.annotate(
                     name,
                     xy=(_x, _y),
                     xycoords="data",
                     xytext=(_text_x, _text_y),
                     textcoords="data",
@@ -320,23 +430,23 @@
         point_other: Optional[Point] = None,
         ignore: Optional[Union[str, list[str]]] = None,
     ):
         if ignore is None:
             ignore = []
         if point_other is None:
             return (
-                    not isinstance(point, Point)
-                    or "unknown" in point.label
-                    or point.label in ignore
+                not isinstance(point, Point)
+                or "unknown" in point.label
+                or point.label in ignore
             )
         else:
             return (
-                    cls.check_phase(point=point, ignore=ignore)
-                    or cls.check_phase(point=point_other, ignore=ignore)
-                    or point.label == point_other.label
+                cls.check_phase(point=point, ignore=ignore)
+                or cls.check_phase(point=point_other, ignore=ignore)
+                or point.label == point_other.label
             )
 
     def boundary_detect(
         self,
         comp_res: PhaseCompareResult,
         mode: DetectionMode = DetectionMode.BOTH,
         ignore: Optional[Union[str, list[str]]] = None,
@@ -352,24 +462,24 @@
                 line = mat[idx]
                 line = line[line != 0]
                 for ele_idx in range(len(line) - 1):
                     ele_left_1: Point = line[ele_idx]
                     ele_right_1: Point = line[ele_idx + 1]
                     if self.check_phase(ele_left_1, ele_right_1, ignore):
                         continue
-                    ele_left_2: pd.DataFrame = self.query_point(
+                    ele_left_2: pd.DataFrame = self.query(
                         data=df,
-                        xval=ele_left_1.x,
-                        yval=ele_left_1.y,
+                        x=ele_left_1.x,
+                        y=ele_left_1.y,
                         phase=ele_right_1.label,
                     )
-                    ele_right_2: pd.DataFrame = self.query_point(
+                    ele_right_2: pd.DataFrame = self.query(
                         data=df,
-                        xval=ele_right_1.x,
-                        yval=ele_right_1.y,
+                        x=ele_right_1.x,
+                        y=ele_right_1.y,
                         phase=ele_left_1.label,
                     )
 
                     if len(ele_left_2) != 1 or len(ele_right_2) != 1:
                         continue
                     x0, _ = self.cross_point(
                         ele_left_1.x,
@@ -389,24 +499,24 @@
                 line = line[line != 0]
                 for ele_idx in range(len(line) - 1):
                     ele_left_1: Point = line[ele_idx]
                     ele_right_1: Point = line[ele_idx + 1]
                     if self.check_phase(ele_left_1, ele_right_1, ignore):
                         continue
 
-                    ele_left_2: pd.DataFrame = self.query_point(
+                    ele_left_2: pd.DataFrame = self.query(
                         data=df,
-                        xval=ele_left_1.x,
-                        yval=ele_left_1.y,
+                        x=ele_left_1.x,
+                        y=ele_left_1.y,
                         phase=ele_right_1.label,
                     )
-                    ele_right_2: pd.DataFrame = self.query_point(
+                    ele_right_2: pd.DataFrame = self.query(
                         data=df,
-                        xval=ele_right_1.x,
-                        yval=ele_right_1.y,
+                        x=ele_right_1.x,
+                        y=ele_right_1.y,
                         phase=ele_left_1.label,
                     )
 
                     if len(ele_left_2) != 1 or len(ele_right_2) != 1:
                         continue
 
                     y0, _ = self.cross_point(
```

### Comparing `simubox-0.2.1/SimuBox/artist/plotter.py` & `simubox-0.2.2/SimuBox/artist/plotter.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/calculator/peak.py` & `simubox-0.2.2/SimuBox/calculator/peak.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import numpy as np
 from scipy.optimize import curve_fit
 import matplotlib.pyplot as plt
 import matplotlib.cm as cm
 from typing import Iterable, Union, Callable, Sequence
-from ..schema import Numeric, Peak, PeakFitResult
+from ..schema import RealNum, Peak, PeakFitResult
 from ..artist import plot_legend, plot_savefig, plot_locators
 from sklearn.metrics import r2_score
 
 
 def gaussian_expansion(
-    array: Union[Iterable, Numeric],
-    amp: Numeric,
-    ctr: Numeric,
-    wid: Numeric,
+    array: Union[Iterable, RealNum],
+    amp: RealNum,
+    ctr: RealNum,
+    wid: RealNum,
 ):
     return amp * np.exp(-(((array - ctr) / wid) ** 2))
 
 
-def curve_function(x: Union[Iterable, Numeric], *params):
+def curve_function(x: Union[Iterable, RealNum], *params):
 
     assert len(params) % 3 == 1
 
     res = 0
     for i in range(0, len(params) - 1, 3):
         res += gaussian_expansion(x, params[i], params[i + 1], params[i + 2])
 
     return res + params[-1]
 
-def curve_split(x: Union[Iterable, Numeric], *params):
+def curve_split(x: Union[Iterable, RealNum], *params):
     assert len(params) % 3 == 1
     res = []
     for i in range(0, len(params) - 1, 3):
         res.append(
             gaussian_expansion(x, params[i], params[i + 1], params[i + 2]) + params[-1]
         )
 
@@ -78,15 +78,15 @@
         for j, f in enumerate(peaks[i].fix):
             if f:
                 lb.append(max(guess[3 * i + j] * lb_scale, 0))
                 ub.append(guess[3 * i + j] * ub_scale)
             else:
                 lb.append(0)
                 ub.append(np.inf)
-    # print(lb,ub)
+
     if fix_background:
         lb.append(max(guess[-1] * lb_scale, 0))
         ub.append(guess[-1] * ub_scale)
     else:
         lb.append(0)
         ub.append(np.inf)
```

### Comparing `simubox-0.2.1/SimuBox/calculator/scatter.py` & `simubox-0.2.2/SimuBox/calculator/scatter.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/calculator/topo.py` & `simubox-0.2.2/SimuBox/calculator/topo.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/calculator/voronoi.py` & `simubox-0.2.2/SimuBox/calculator/voronoi.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/runner/Agents/ABC.py` & `simubox-0.2.2/SimuBox/runner/agents/ABC.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/runner/Agents/ABC_ABC.py` & `simubox-0.2.2/SimuBox/runner/agents/ABC_ABC.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 from .MixinModel import *
 
 __all__ = ["ABC_ABC"]
 
 
 class ABC_ABC(MixinAgent):
-
-    chain2_len: float
+    def __init__(self, *args, **kwargs):
+       self.chain2_len: float = -1.0
 
     @classmethod
     def modify(cls, pn: str, pv: Any, input_dict: OrderedDict, options: Options):
         if pn == "fA1":
             fC1 = fA1 = round(pv, 6)
             fB1 = round(1 - fA1 - fC1, 6)
             for i, j in zip(range(3), [fA1, fB1, fC1]):
```

### Comparing `simubox-0.2.1/SimuBox/runner/Agents/BABCB.py` & `simubox-0.2.2/SimuBox/runner/agents/BABCB.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from .MixinModel import *
 
 __all__ = ["BABCB"]
 
 
 class BABCB(MixinAgent):
-
-    fB: float
+    def __init__(self, *args, **kwargs):
+        self.fB: float = -1.0
 
     @classmethod
     def modify(cls, pn: str, pv: Any, input_dict: OrderedDict, options: Options):
         if pn == "fA":
             fC = fA = pv
             cls.fB = round(1 - fA - fC, 6)
             input_dict["Block"][1]["ContourLength"] = fA
```

### Comparing `simubox-0.2.1/SimuBox/runner/Agents/Mask_AB_A.py` & `simubox-0.2.2/SimuBox/runner/agents/Mask_AB_A.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/runner/Agents/Mask_AB_AB.py` & `simubox-0.2.2/SimuBox/runner/agents/Mask_AB_AB.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/runner/Agents/MixinModel.py` & `simubox-0.2.2/SimuBox/runner/agents/MixinModel.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import abstractmethod
 from collections import OrderedDict
 from typing import Any
 
-from ..Phases import PhaseInit
+from ..phases import PhaseInit
 from ...schema import Cells, Options
 
 
 class MixinAgent:
     def __call__(self, *args, **kwargs):
         self.modify(*args, **kwargs)
```

### Comparing `simubox-0.2.1/SimuBox/runner/Manager.py` & `simubox-0.2.2/SimuBox/runner/manager.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/runner/Phases.py` & `simubox-0.2.2/SimuBox/runner/phases.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/schema/enums/MixinEnums.py` & `simubox-0.2.2/SimuBox/schema/enums/MixinEnums.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/schema/enums/Modes.py` & `simubox-0.2.2/SimuBox/schema/enums/Modes.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/schema/enums/OtherEnums.py` & `simubox-0.2.2/SimuBox/schema/enums/OtherEnums.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/schema/enums/SCFTEnums.py` & `simubox-0.2.2/SimuBox/schema/enums/SCFTEnums.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/schema/labels.py` & `simubox-0.2.2/SimuBox/schema/labels.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/schema/structs/ChartElement.py` & `simubox-0.2.2/SimuBox/schema/structs/ChartElement.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/schema/structs/ComputedRes.py` & `simubox-0.2.2/SimuBox/schema/structs/ComputedRes.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/schema/structs/DataFile.py` & `simubox-0.2.2/SimuBox/schema/structs/DataFile.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/schema/structs/MixinStructs.py` & `simubox-0.2.2/SimuBox/schema/structs/MixinStructs.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/schema/structs/OtherStructs.py` & `simubox-0.2.2/SimuBox/schema/structs/OtherStructs.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     """
 
     left: str
     right: Optional[str] = None
     factor: Optional[float] = None
     operator: Operator
     name: Optional[str] = None
+    accuracy: int = 3
 
     @property
     def _name(self):
         if self.name is not None:
             return self.name
         assert self.right is not None or self.factor is not None
         return (
```

### Comparing `simubox-0.2.1/SimuBox/schema/structs/SCFTStructs.py` & `simubox-0.2.2/SimuBox/schema/structs/SCFTStructs.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/scripts/extractor.py` & `simubox-0.2.2/SimuBox/scripts/extractor.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/scripts/JSON/ABC_ABC.json` & `simubox-0.2.2/SimuBox/scripts/JSON/ABC_ABC.json`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/scripts/JSON/BABCB.json` & `simubox-0.2.2/SimuBox/scripts/JSON/BABCB.json`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/scripts/push_job.py` & `simubox-0.2.2/SimuBox/scripts/push_job.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/scripts/setenv.py` & `simubox-0.2.2/SimuBox/scripts/setenv.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/scripts/web.py` & `simubox-0.2.2/SimuBox/scripts/web.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/toolkits/function.py` & `simubox-0.2.2/SimuBox/toolkits/function.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import re
 from pathlib import Path
-from typing import Optional, Union
+from typing import Optional, Union, Sequence
 
 import numpy as np
 import pandas as pd
 
-from ..schema import Numeric, Vector, PathLike, Operation, OPERATOR_FUNCTION_MAP
+from ..schema import RealNum, Vector, PathLike, Operation, OPERATOR_FUNCTION_MAP
 
 
 __all__ = [
     "arange",
     "find_nearest_1d",
     "replace_target",
     "match_target",
@@ -40,68 +40,99 @@
 
     res = np.around(asc + start, accuracy)
     if end not in res:
         res = np.append(res, end)
     return np.sort(res)
 
 
-def find_nearest_1d(array: Vector, value: Numeric) -> int:
+def find_nearest_1d(array: Vector, value: RealNum) -> int:
     """
     寻找序列（array）中与指定值（value）最接近的数值的索引。
 
     :param array: 任意向量
     :param value: 任意数值
     :return: 索引值（整型）
     """
     if not isinstance(array, np.ndarray):
         array = np.asarray(array)
     idx = (np.abs(array - value)).argmin()
     return idx
 
 
-def replace_target(path: PathLike, target: str, key: str = "phase") -> Optional[Path]:
+def replace_target(
+    path: PathLike, target: Union[str, RealNum], key: str = "phase"
+) -> Optional[Path]:
+    """
+    替换路径中的信息。
+
+    :param path: 原路径。
+    :param target: 需要替换的值。
+    :param key: 值对应的名称。
+    :return: 替换值之后的路径。
+    """
+
     path = str(path)
     pattern = re.compile(key + r"(\w+)_?")
+    target = str(target)
     match = pattern.search(path)
     # 如果找到匹配项，则进行替换
     if match:
         # 获取匹配的字符串
         matched_string = match.group(1)
         modified_string = path.replace(matched_string, target)
         return Path(modified_string)
     else:
         print(f"路径：{path} 修改失败。")
         return
 
 
-def match_target(candidates: list[str], **kwargs):
+def match_target(candidates: Sequence[PathLike], **kwargs):
+    """
+    按照指定的关键字匹配路径。
+
+    :param candidates: 等待匹配的对象。
+    :param kwargs:
+    :return: 匹配到的对象。
+    """
     criteria = [k + str(v) for k, v in kwargs.items()]
+    res = []
     for candidate in candidates:
         candidate = str(candidate)
         for c in criteria:
             if c not in candidate:
                 break
         else:
-            return Path(candidate)
-    print(f"{criteria}匹配失败。")
-    return
+            res.append(Path(candidate))
+    if len(res) == 0:
+        print(f"{criteria}匹配失败。")
+        return
+    else:
+        return res if len(res) > 1 else res[0]
 
 
-def process_dataframe(data: pd.DataFrame, operation: Operation, accuracy: int = 3):
+def process_dataframe(data: pd.DataFrame, operation: Operation):
+    """
+    对dataframe数据进行便捷的预处理。
+
+    :param data:
+    :param operation:
+    :param accuracy:
+    :return:
+    """
 
     if operation.left in data.columns:
         left = data[operation.left].values
         if operation.right in data.columns:
             right = data[operation.right].values
         elif operation.factor is not None:
             right = operation.factor
         else:
             raise KeyError(
                 f"right: {operation.right} 或 factor: {operation.factor} 应至少有一个有效"
             )
 
         data[operation.name] = np.around(
-            OPERATOR_FUNCTION_MAP[operation.operator](left, right), accuracy
+            OPERATOR_FUNCTION_MAP[operation.operator](left, right), operation.accuracy
         )
         return data
     else:
         raise KeyError(f"left: {operation.left}不是有效数据列")
```

### Comparing `simubox-0.2.1/SimuBox/toolkits/reader.py` & `simubox-0.2.2/SimuBox/toolkits/reader.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import os
 
 from ..schema import (
     Printout,
     Density,
     Fet,
     DensityParseResult,
-    Numeric,
+    RealNum,
     FileLike,
     PathLike,
     Operation,
     Operator,
 )
 from .function import process_dataframe
 
@@ -76,15 +76,15 @@
 
 
 def read_density(
     path: FileLike,
     parse_N: bool = True,
     parse_L: bool = False,
     filename: str = "phout.txt",
-    binary: Sequence[str] = (".bin"),
+    binary: bool = False,
     mode: str = "r",
     encoding: str = "utf-8",
     **kwargs,
 ) -> Density:
     """
 
     :param path: 文件路径或者文件所在的文件夹路径。
@@ -100,21 +100,33 @@
 
     if isinstance(path, bytes):
         bin_read_function = np.frombuffer
         content = path
         text = False
     elif isinstance(path, PathLike):
         path = check_filepath(path, filename)
-        if path.suffix == binary:
+        if binary or path.suffix in (".bin"):
             bin_read_function = np.fromfile
             content = path
             text = False
         else:
-            content = path.open(mode=mode, encoding=encoding).readlines()
-            text = True
+            try:
+                content = path.open(mode=mode, encoding=encoding).readlines()
+                text = True
+            except UnicodeDecodeError as ude:
+                return read_density(
+                    path,
+                    parse_N=True,
+                    parse_L=True,
+                    filename=filename,
+                    mode=mode,
+                    encoding=encoding,
+                    binary=True,
+                    **kwargs,
+                )
     else:
         raise ValueError(type(path))
 
     def _validate(vec: np.ndarray):
         return any(vec > 1000) or any(vec <= 0)
 
     skip = 0
@@ -160,14 +172,16 @@
                 return read_density(
                     path,
                     parse_N=True,
                     parse_L=True,
                     filename=filename,
                     mode=mode,
                     **kwargs,
+                    encoding=encoding,
+                    binary=binary,
                 )
             else:
                 raise pe
     else:
         if isinstance(content, PathLike):
             count = os.path.getsize(content)
         else:
@@ -185,14 +199,16 @@
             if not parse_L or not parse_N:
                 return read_density(
                     path,
                     parse_N=True,
                     parse_L=True,
                     filename=filename,
                     mode=mode,
+                    encoding=encoding,
+                    binary=binary,
                     **kwargs,
                 )
             else:
                 print(f"NxNyNz:{NxNyNz}, lxlylz:{lxlylz}, offset:{offset}")
                 raise ve
 
 
@@ -211,30 +227,30 @@
     )
 
 
 def read_csv(
     path: PathLike,
     skiprows: int = 0,
     accuracy: int = 3,
-    Operations: Optional[Union[Operation, Sequence[Operation]]] = None,
+    operation: Optional[Union[Operation, Sequence[Operation]]] = None,
     subset: Optional[Union[str, Sequence[str]]] = ("phase", "freeE"),
     **kwargs,
 ):
     assert path.is_file(), f"{path} 并非有效的文件路径。"
     if path.suffix == ".csv":
         data = pd.read_csv(path, skiprows=skiprows)
     else:
         data = pd.read_excel(path, skiprows=skiprows)
     if "freeE" in data.columns:
         data["freeE"] = np.around(data["freeE"], 8)
     if subset:
         data = data.drop_duplicates(subset=subset)
 
-    if Operations is None:
-        Operations = [
+    if operation is None:
+        operation = [
             Operation(
                 left="ly",
                 right="lz",
                 operator=Operator.div,
                 accuracy=accuracy,
                 name="lylz",
             ),
@@ -249,18 +265,18 @@
                 left=kwargs.get("var", "chiN"),
                 factor=kwargs.get("factor", 1),
                 operator=Operator.div,
                 accuracy=accuracy,
                 name=kwargs.get("var", "chiN"),
             ),
         ]
-    elif isinstance(Operations, Operation):
-        Operations = [Operations]
+    elif isinstance(operation, Operation):
+        operation = [operation]
 
-    for Opr in Operations:
+    for Opr in operation:
         try:
             data = process_dataframe(data, Opr)
         except KeyError:
             continue
 
     return data
 
@@ -322,15 +338,15 @@
 
 
 def parse_density(
     density: Density,
     target: Union[int, Iterable[int], str] = 0,
     permute: Optional[Iterable[int]] = None,
     slices: Optional[tuple[int, int]] = None,
-    expand: Union[Numeric, Sequence[Numeric]] = 1,
+    expand: Union[RealNum, Sequence[RealNum]] = 1,
     **kwargs,
 ) -> DensityParseResult:
     """
     对密度信息进行二次处理，如延拓、交换轴、切片等。
 
     :param density:
     :param target:
@@ -364,15 +380,15 @@
         target = list(density.data.columns)
     elif isinstance(target, int):
         target = [target]
     mats = [f_mat(density.data[t].values.reshape(shape)) for t in target]
     shape = f_vec(shape)
     lxlylz = f_vec(lxlylz)
 
-    if isinstance(expand, Numeric):
+    if isinstance(expand, RealNum):
         expand = np.array([max(expand, 1)] * len(shape))
     else:
         assert len(expand) == len(shape), f"当前矩阵维度为3，拓展信息长度为{len(expand)}, 不匹配"
         expand = np.array(expand)
         expand[expand < 1] = 1
 
     expand_for_pad = np.around((expand - 1) / 2 * shape).astype(int)
```

### Comparing `simubox-0.2.1/SimuBox/toolkits/vector.py` & `simubox-0.2.2/SimuBox/toolkits/vector.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/toolkits/xmltrans.py` & `simubox-0.2.2/SimuBox/toolkits/xmltrans.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,14 @@
         将xml记录的粒子信息，转化为自洽场的密度信息。
 
         :param xml:
         :param r_cut:
         :return:
         """
 
-
         xml = xml if xml is not None else cls.xml
         assert xml is not None
         phi = np.zeros([len(xml.atoms_type), *xml.NxNyNz])
 
         idx_lst = np.array(r_cut * 2 / xml.grid_spacing + 2, dtype=int)
 
         res = np.array(list(product(*[range(idx) for idx in idx_lst])), dtype=int)
```

### Comparing `simubox-0.2.1/SimuBox/web/Homepage.py` & `simubox-0.2.2/SimuBox/web/Homepage.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/web/pages/1_Structure.py` & `simubox-0.2.2/SimuBox/web/pages/1_Structure.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/web/pages/2_Scatter.py` & `simubox-0.2.2/SimuBox/web/pages/2_Scatter.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/web/pages/3_Voronoi.py` & `simubox-0.2.2/SimuBox/web/pages/3_Voronoi.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/web/pages/4_Curve.py` & `simubox-0.2.2/SimuBox/web/pages/4_Curve.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/web/pages/5_Peaks.py` & `simubox-0.2.2/SimuBox/web/pages/5_Peaks.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/web/pages/6_Topology.py` & `simubox-0.2.2/SimuBox/web/pages/6_Topology.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/SimuBox/web/pages/7_Landscape.py` & `simubox-0.2.2/SimuBox/web/pages/7_Landscape.py`

 * *Files identical despite different names*

### Comparing `simubox-0.2.1/PKG-INFO` & `simubox-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimuBox
-Version: 0.2.1
+Version: 0.2.2
 Summary: Free python package to do some science calculation.
 Home-page: https://pypi.org/project/SimuBox/
 License: ./LICENSE
 Author: Alkaid Yuan
 Author-email: kryuan@qq.com
 Maintainer: Alkaid Yuan
 Maintainer-email: kryuan@qq.com
@@ -15,16 +15,18 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: matplotlib (>=3.8.2,<4.0.0)
 Requires-Dist: numpy (>=1.26.2,<2.0.0)
 Requires-Dist: opencv-python (>=4.8.1.78,<5.0.0.0)
 Requires-Dist: opencv-python-headless (>=4.8.1.78,<5.0.0.0)
 Requires-Dist: pandas (>=2.1.4,<3.0.0)
+Requires-Dist: plotly (>=5.20.0,<6.0.0)
 Requires-Dist: poetry-plugin-export (>=1.6.0,<2.0.0)
 Requires-Dist: pydantic (>=2.5.2,<3.0.0)
+Requires-Dist: pyecharts (>=2.0.5,<3.0.0)
 Requires-Dist: pyvista (>=0.43.1,<0.44.0)
 Requires-Dist: scikit-image (>=0.22.0,<0.23.0)
 Requires-Dist: scikit-learn (>=1.3.2,<2.0.0)
 Requires-Dist: scipy (>=1.11.4,<2.0.0)
 Requires-Dist: shapely (>=2.0.2,<3.0.0)
 Requires-Dist: simplejson (>=3.19.2,<4.0.0)
 Requires-Dist: stpyvista (>=0.0.11,<0.0.12)
```

