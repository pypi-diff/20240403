# Comparing `tmp/paibox-1.0.0a7.tar.gz` & `tmp/paibox-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paibox-1.0.0a7.tar", max compression
+gzip compressed data, was "paibox-1.0.0b1.tar", max compression
```

## Comparing `paibox-1.0.0a7.tar` & `paibox-1.0.0b1.tar`

### file list

```diff
@@ -1,44 +1,45 @@
--rw-r--r--   0        0        0      806 2024-03-24 08:51:45.073101 paibox-1.0.0a7/CHANGELOG.md
--rw-r--r--   0        0        0    35149 2024-03-24 08:51:45.073101 paibox-1.0.0a7/LICENSE
--rw-r--r--   0        0        0     1004 2024-03-24 08:51:45.073101 paibox-1.0.0a7/README.md
--rw-r--r--   0        0        0    26412 2024-03-24 08:51:45.077101 paibox-1.0.0a7/docs/Guide-of-PAIBox.md
--rw-r--r--   0        0        0     2352 2024-03-24 08:51:45.077101 paibox-1.0.0a7/docs/Guide-of-Test.md
--rw-r--r--   0        0        0    19453 2024-03-24 08:51:45.077101 paibox-1.0.0a7/docs/images/Guide-基础网络搭建-全连接网络示例.png
--rw-r--r--   0        0        0     1545 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/__init__.py
--rw-r--r--   0        0        0      131 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/backend/__init__.py
--rw-r--r--   0        0        0      394 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/backend/checker.py
--rw-r--r--   0        0        0    12743 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/backend/conf_template.py
--rw-r--r--   0        0        0     2079 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/backend/constrs.py
--rw-r--r--   0        0        0     1672 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/backend/context.py
--rw-r--r--   0        0        0    17822 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/backend/graphs.py
--rw-r--r--   0        0        0     1044 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/backend/graphs_types.py
--rw-r--r--   0        0        0    18969 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/backend/mapper.py
--rw-r--r--   0        0        0    23898 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/backend/placement.py
--rw-r--r--   0        0        0    18234 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/backend/routing.py
--rw-r--r--   0        0        0    11780 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/backend/segment_utils.py
--rw-r--r--   0        0        0    10093 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/base.py
--rw-r--r--   0        0        0     5192 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/collector.py
--rw-r--r--   0        0        0     1826 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/context.py
--rw-r--r--   0        0        0     1094 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/exceptions.py
--rw-r--r--   0        0        0     7015 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/mixin.py
--rw-r--r--   0        0        0     1116 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/naming.py
--rw-r--r--   0        0        0    10079 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/network.py
--rw-r--r--   0        0        0      316 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/neuron/__init__.py
--rw-r--r--   0        0        0    19193 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/neuron/base.py
--rw-r--r--   0        0        0     5469 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/neuron/neurons.py
--rw-r--r--   0        0        0      894 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/node.py
--rw-r--r--   0        0        0     5204 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/projection.py
--rw-r--r--   0        0        0      244 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/simulator/__init__.py
--rw-r--r--   0        0        0     3699 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/simulator/encoder.py
--rw-r--r--   0        0        0     1097 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/simulator/probe.py
--rw-r--r--   0        0        0     6794 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/simulator/simulator.py
--rw-r--r--   0        0        0      348 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/synapses/__init__.py
--rw-r--r--   0        0        0     8044 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/synapses/base.py
--rw-r--r--   0        0        0     7165 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/synapses/conv_utils.py
--rw-r--r--   0        0        0     4274 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/synapses/synapses.py
--rw-r--r--   0        0        0     9735 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/synapses/transforms.py
--rw-r--r--   0        0        0      400 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/tools.py
--rw-r--r--   0        0        0     2125 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/types.py
--rw-r--r--   0        0        0     5195 2024-03-24 08:51:45.081102 paibox-1.0.0a7/paibox/utils.py
--rw-r--r--   0        0        0     1936 2024-03-24 08:51:45.081102 paibox-1.0.0a7/pyproject.toml
--rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 paibox-1.0.0a7/PKG-INFO
+-rw-r--r--   0        0        0     1065 2024-04-03 02:23:11.626351 paibox-1.0.0b1/CHANGELOG.md
+-rw-r--r--   0        0        0    35149 2024-04-03 02:23:11.626351 paibox-1.0.0b1/LICENSE
+-rw-r--r--   0        0        0     1004 2024-04-03 02:23:11.626351 paibox-1.0.0b1/README.md
+-rw-r--r--   0        0        0    26509 2024-04-03 02:23:11.626351 paibox-1.0.0b1/docs/Guide-of-PAIBox.md
+-rw-r--r--   0        0        0     2352 2024-04-03 02:23:11.626351 paibox-1.0.0b1/docs/Guide-of-Test.md
+-rw-r--r--   0        0        0    19453 2024-04-03 02:23:11.626351 paibox-1.0.0b1/docs/images/Guide-基础网络搭建-全连接网络示例.png
+-rw-r--r--   0        0        0     1545 2024-04-03 02:23:11.630351 paibox-1.0.0b1/paibox/__init__.py
+-rw-r--r--   0        0        0      131 2024-04-03 02:23:11.630351 paibox-1.0.0b1/paibox/backend/__init__.py
+-rw-r--r--   0        0        0      394 2024-04-03 02:23:11.630351 paibox-1.0.0b1/paibox/backend/checker.py
+-rw-r--r--   0        0        0    12743 2024-04-03 02:23:11.630351 paibox-1.0.0b1/paibox/backend/conf_template.py
+-rw-r--r--   0        0        0     2079 2024-04-03 02:23:11.630351 paibox-1.0.0b1/paibox/backend/constrs.py
+-rw-r--r--   0        0        0     1672 2024-04-03 02:23:11.630351 paibox-1.0.0b1/paibox/backend/context.py
+-rw-r--r--   0        0        0    17822 2024-04-03 02:23:11.630351 paibox-1.0.0b1/paibox/backend/graphs.py
+-rw-r--r--   0        0        0     1044 2024-04-03 02:23:11.630351 paibox-1.0.0b1/paibox/backend/graphs_types.py
+-rw-r--r--   0        0        0    19027 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/backend/mapper.py
+-rw-r--r--   0        0        0    23458 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/backend/placement.py
+-rw-r--r--   0        0        0    18234 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/backend/routing.py
+-rw-r--r--   0        0        0    11780 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/backend/segment_utils.py
+-rw-r--r--   0        0        0    10082 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/base.py
+-rw-r--r--   0        0        0     5192 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/collector.py
+-rw-r--r--   0        0        0     1826 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/context.py
+-rw-r--r--   0        0        0     1212 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/exceptions.py
+-rw-r--r--   0        0        0     7015 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/mixin.py
+-rw-r--r--   0        0        0     1116 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/naming.py
+-rw-r--r--   0        0        0    10079 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/network.py
+-rw-r--r--   0        0        0      316 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/neuron/__init__.py
+-rw-r--r--   0        0        0    18461 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/neuron/base.py
+-rw-r--r--   0        0        0     5469 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/neuron/neurons.py
+-rw-r--r--   0        0        0      775 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/neuron/utils.py
+-rw-r--r--   0        0        0      894 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/node.py
+-rw-r--r--   0        0        0     5204 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/projection.py
+-rw-r--r--   0        0        0      244 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/simulator/__init__.py
+-rw-r--r--   0        0        0     3699 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/simulator/encoder.py
+-rw-r--r--   0        0        0     1097 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/simulator/probe.py
+-rw-r--r--   0        0        0     6794 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/simulator/simulator.py
+-rw-r--r--   0        0        0      348 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/synapses/__init__.py
+-rw-r--r--   0        0        0     8069 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/synapses/base.py
+-rw-r--r--   0        0        0     7179 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/synapses/conv_utils.py
+-rw-r--r--   0        0        0     4274 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/synapses/synapses.py
+-rw-r--r--   0        0        0    11275 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/synapses/transforms.py
+-rw-r--r--   0        0        0      400 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/tools.py
+-rw-r--r--   0        0        0     2165 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/types.py
+-rw-r--r--   0        0        0     5195 2024-04-03 02:23:11.634351 paibox-1.0.0b1/paibox/utils.py
+-rw-r--r--   0        0        0     1936 2024-04-03 02:23:11.634351 paibox-1.0.0b1/pyproject.toml
+-rw-r--r--   0        0        0     2357 1970-01-01 00:00:00.000000 paibox-1.0.0b1/PKG-INFO
```

### Comparing `paibox-1.0.0a7/CHANGELOG.md` & `paibox-1.0.0b1/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -22,7 +22,14 @@
 ## v1.0.0a6
 
 - 新增 `Always1Neuron` 神经元，该神经元将在工作期间持续输出1，不得单独存在，需存在前向突触与其连接。
 
 ## v1.0.0a7
 
 - 支持全展开1D卷积算子构建与部署（`padding` 不支持）
+
+## v1.0.0a8
+
+- 提高 `numpy` 依赖版本至 `^1.24.0`
+- 修复神经元输入累加错误
+- 修复当权重为 `np.bool_` 且关闭权重精度优化选项( `weight_bit_optimization` )后，仍视为 `np.int8` 的错误
+- 支持混合精度权重的部署
```

### Comparing `paibox-1.0.0a7/LICENSE` & `paibox-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0a7/README.md` & `paibox-1.0.0b1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 </div>
 
 <p align="center">
     <a href="https://github.com/PAICookers/PAIBox/blob/master/pyproject.toml">
         <img src="https://img.shields.io/pypi/pyversions/paibox">
     </a>
-    <a href="https://github.com/PAICookers/PAIBox/releases/tag/v1.0.0a7">
+    <a href="https://github.com/PAICookers/PAIBox/releases/tag/v1.0.0b1">
         <img src="https://img.shields.io/github/v/release/PAICookers/PAIBox?include_prereleases&color=orange">
     </a>
     <a href="https://www.codefactor.io/repository/github/PAICookers/PAIBox">
       <img src="https://img.shields.io/codefactor/grade/github/PAICookers/PAIBox/master?color=red">
     </a>
     <a href="https://results.pre-commit.ci/latest/github/PAICookers/PAIBox/master">
 	   <img src="https://results.pre-commit.ci/badge/github/PAICookers/PAIBox/master.svg" alt="pre-commit.ci status">
```

### Comparing `paibox-1.0.0a7/docs/Guide-of-PAIBox.md` & `paibox-1.0.0b1/docs/Guide-of-PAIBox.md`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ```
 
 若使用conda等，则手动安装如下依赖至Python虚拟环境：
 
 ```toml
 python = "^3.8"
 pydantic = "^2.0"
-numpy = "^1.23.0"
+numpy = "^1.24.0"
 paicorelib = "0.0.13"
 ```
 
 通过pip安装PAIBox：
 
 ```bash
 pip install paibox
@@ -701,45 +701,45 @@
 
 # Clear all the results
 mapper.clear()
 ```
 
 其中，编译时有如下参数可指定：
 
-- `weight_bit_optimization`: 是否对权重精度进行优化处理。例如，将声明时为 INT8 的权重根据实际值当作更小的精度处理（当权重的值均在 [-8, 7] 之间，则可当作 INT4 进行处理）。默认由后端配置项内对应**编译选项**指定（默认开启）。
+- `weight_bit_optimization`: 是否对权重精度进行优化处理。这将使得声明时为 INT8 的权重根据实际值当作更小的精度处理（当权重的值均在 [-8, 7] 之间，则可当作 INT4 进行处理）。默认由后端配置项内对应**编译选项**指定（默认开启）。
 - `grouping_optim_target`：指定神经元分组的优化目标，可以为 `"latency"`，`"core"` 或 `"both"`，分别代表以延时/吞吐率、占用核资源为优化目标、或二者兼顾。默认由后端配置项内对应**编译选项**指定（默认为 `both`）。
 - 同时，该方法将返回字典形式的编译后网络的信息。
 
 导出时有如下参数可指定：
 
 - `write_to_file`: 是否将配置帧导出为文件。默认为 `True`。
 - `fp`：导出目录。若未指定，则默认为后端配置选项 `build_directory` 所设置的目录（当前工作目录）。
 - `format`：导出交换文件格式，可以为 `bin`、`npy` 或 `txt`。默认为 `bin`。
-- `split_by_coordinate`：是否将配置帧以每个核坐标进行分割，由此生成的配置帧文件命名为"config_core1"、"config_core2"等。默认为 `False`。
-- `local_chip_addr`：本地芯片地址，元组格式表示。默认为后端配置项 `local_chip_addr` 所设置的默认值。
+- `split_by_coordinate`：是否将配置帧以每个核坐标进行分割，由此生成的配置帧文件命名为"config_core1"、"config_core2"等。默认为 `False`，即最终导出为一个文件。
+- `local_chip_addr`：本地芯片坐标，元组格式表示。默认为后端配置项 `local_chip_addr` 所设置的默认值。
 - `export_core_params`: 是否导出实际使用核参数至json文件，以直观显示实际使用核的配置信息。默认为 `False`。
 
 同时，该方法将返回模型的配置项字典 `GraphInfo`，包括：
 
 - `input`：输入节点信息字典。
 - `output`：输出目的地信息字典。
 - `memebers`：中间层所在物理核的配置项字典。
 - `inherent_timestep`：网络模型的最长时间步。
 - `n_core_required`：网络模型需要的物理核数目。
-- `extras`：其他额外的网络信息字典，例如，编译后网络名称。
+- `extras`：其他额外的网络信息字典，例如，编译后的网络名称。
 
 ### 后端配置项
 
 与后端相关的配置项由 `BACKEND_CONFIG` 统一保存与访问，例如上述**编译选项**、`build_directory`、`local_chip_addr` 等。常用的配置项有如下：
 
 ```python
-BACKEND_CONFIG.local_chip_addr
+BACKEND_CONFIG.local_chip_addr # 本地芯片坐标
 >>> Coord(0, 0)
 
-BACKEND_CONFIG.test_chip_addr
+BACKEND_CONFIG.test_chip_addr # 测试芯片坐标（一般是FPGA）
 >>> Coord(1, 0)
 
 # Set output directory
 BACKEND_CONFIG.output_dir = "./output"
 
 # Set cflag for enabling weight precision optimization
 set_cflag(enable_wp_opt=True, cflag="This is a cflag.")
```

### Comparing `paibox-1.0.0a7/docs/Guide-of-Test.md` & `paibox-1.0.0b1/docs/Guide-of-Test.md`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0a7/docs/images/Guide-基础网络搭建-全连接网络示例.png` & `paibox-1.0.0b1/docs/images/Guide-基础网络搭建-全连接网络示例.png`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0a7/paibox/__init__.py` & `paibox-1.0.0b1/paibox/__init__.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0a7/paibox/backend/conf_template.py` & `paibox-1.0.0b1/paibox/backend/conf_template.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0a7/paibox/backend/constrs.py` & `paibox-1.0.0b1/paibox/backend/constrs.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0a7/paibox/backend/context.py` & `paibox-1.0.0b1/paibox/backend/context.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0a7/paibox/backend/graphs.py` & `paibox-1.0.0b1/paibox/backend/graphs.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0a7/paibox/backend/graphs_types.py` & `paibox-1.0.0b1/paibox/backend/graphs_types.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0a7/paibox/backend/mapper.py` & `paibox-1.0.0b1/paibox/backend/mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     CoordLike,
     CoordOffset,
     HwConfig,
     get_replication_id,
     to_coord,
 )
 
-from paibox.base import NeuDyn
+from paibox.base import NeuDyn, SynSys
 from paibox.exceptions import ResourceError
 from paibox.network import DynSysGroup
 
 from .conf_template import (
     CoreConfig,
     CorePlacementInfo,
     GraphInfo,
@@ -136,47 +136,44 @@
         """
         if weight_bit_optimization is not None:
             set_cflag(enable_wp_opt=weight_bit_optimization)
 
         if grouping_optim_target is not None:
             set_cflag(grouping_optim_target=grouping_optim_target)
 
-        """Backend compilation."""
+        """1. Check whether the PAIGraph has built."""
         self._build_check()
 
-        """1. Build core blocks."""
+        """2. Set global compilation flags."""
+        self._set_global_cflags()
+
+        """3. Build core blocks."""
         self.build_core_blocks()
 
-        """2. Adjust the LCN extension of each core block."""
+        """4. Adjust the LCN extension of each core block."""
         self.lcn_ex_adjustment()
 
-        """3. Core coordinate assignment."""
+        """5. Core coordinate assignment."""
         self.coord_assign()
 
-        """4. Allocate the core blocks to the `CorePlacement`."""
+        """6. Allocate the core blocks to the `CorePlacement`."""
         self.core_allocation()
 
-        """5. Export parameters."""
+        """7. Export parameters."""
         return self.config_export()
 
     def build_core_blocks(self) -> None:
         """Build core blocks based on grouped edges.
 
         Description: Group all edges & build `CoreBlock` based on the grouped edges.
         """
         grouped_edges = self.graph.group_edges()
 
         for syns in grouped_edges:
-            self.core_blocks.append(
-                CoreBlock.build(
-                    *syns,
-                    seed=0,
-                    enable_wp_opt=_BACKEND_CONTEXT.cflags["enable_wp_opt"],
-                )
-            )
+            self.core_blocks.append(CoreBlock.build(*syns, seed=0))
 
         for cb in self.core_blocks:
             succ_cbs = list(
                 filter(
                     lambda succ_cb: any(d for d in cb.dest if d in succ_cb.source),
                     self.core_blocks,
                 )
@@ -206,17 +203,16 @@
             else:
                 # Doesn't have following core blocks
                 cb.lcn_locked = True
 
     def coord_assign(self) -> None:
         """Assign the coordinate of each `CorePlacement`.
 
-        NOTE: The neurons in each core block must be grouped first  \
-            to determine the #N of cores required, and then the     \
-            routing coordinates can be assigned.
+        NOTE: The neurons in each core block must be grouped first to determine the #N of cores required,   \
+            and then the routing coordinates can be assigned.
         """
         for cb in self.core_blocks:
             # Group the neurons, get the #N of cores required.
             cb.group_neurons(
                 optim_target=_BACKEND_CONTEXT.cflags["grouping_optim_target"]
             )
 
@@ -270,14 +266,17 @@
             extras={"name": self.graph.graph_name_repr},
         )
 
         self.graph_info = _graph_info
 
         return _graph_info
 
+    def _set_global_cflags(self) -> None:
+        SynSys.CFLAG_ENABLE_WP_OPTIMIZATION = _BACKEND_CONTEXT.cflags["enable_wp_opt"]
+
     def _inpproj_config_export(self) -> InputNodeInfo:
         """Export the configuration of input projections.
 
         Json exchange file format for input nodes:
         {
             "inp1_1": { # as input node #1 without dest info
                 "addr_core_x": 0,
```

### Comparing `paibox-1.0.0a7/paibox/backend/placement.py` & `paibox-1.0.0b1/paibox/backend/placement.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     HwConfig,
     HwCore,
     MaxPoolingEnable,
 )
 from paicorelib import WeightPrecision as WP
 
 from paibox.base import NeuDyn, PAIBoxObject
-from paibox.exceptions import BuildError, NotSupportedError, ResourceError
+from paibox.exceptions import BuildError, ResourceError, TruncationWarning
 from paibox.synapses import SynSys
 from paibox.types import WeightType
 from paibox.utils import check_attr_same, count_unique_elem
 
 from .conf_template import CoreConfig, CorePlacementConfig, NeuronConfig
 from .context import _BACKEND_CONTEXT
 from .graphs_types import DestNodeType, SourceNodeType
@@ -43,50 +43,35 @@
     get_neu_segments,
 )
 
 WeightRamType: TypeAlias = NDArray[np.uint64]  # uint64 weights mapped in weight RAM
 
 
 class CoreAbstract(HwCore, PAIBoxObject):
-    SUPPORTED_WP: ClassVar[Tuple[WP, ...]] = (
-        WP.WEIGHT_WIDTH_1BIT,
-        WP.WEIGHT_WIDTH_2BIT,  # Not verified
-        WP.WEIGHT_WIDTH_4BIT,  # Not verified
-        WP.WEIGHT_WIDTH_8BIT,
-    )
-    """Supported weight precision."""
-
     SUPPORTED_MODE: ClassVar[Tuple[CoreMode, ...]] = (CoreMode.MODE_SNN,)
     """Supported core modes."""
 
 
 class CoreBlock(CoreAbstract):
     """Core Block for `MODE_SNN` ONLY."""
 
     RUNTIME_MODE: ClassVar[CoreMode] = CoreMode.MODE_SNN
 
-    def __init__(
-        self,
-        *parents: SynSys,
-        weight_precision: WP,
-        seed: int = 0,
-        name: Optional[str] = None,
-    ) -> None:
-        """
-        Arguments:
+    def __init__(self, *parents: SynSys, seed: int, name: Optional[str] = None) -> None:
+        """Core blocks in SNN mode.
+
+        Args:
             - parents: the parent synapses.
-            - weight_precision: the precision of weight matrix.
-            - seed: the random seed.
-            - name: the name of the core block. Optional.
+            - seed: random seed. Default value is 0.
+            - name: name of the core block. Optional.
         """
-
         super().__init__(name)
         self._parents = parents
-        self._lcn_ex = n_axon2lcn_ex(self.n_axon, self.n_fanin_max)
-        self.weight_precision = weight_precision
+        self._lcn_ex = self._n_axon2lcn_ex()
+        self._wp = WP.WEIGHT_WIDTH_8BIT  # Default value
 
         self.seed = seed
         """Random seed, legal integer, no more than uint64."""
 
         self.target_lcn = LCN_EX.LCN_1X
         """The target(destination core block) LCN."""
 
@@ -138,14 +123,36 @@
     def _get_syn_of(self, src: SourceNodeType, dest: DestNodeType) -> Optional[SynSys]:
         for syn in self.obj:
             if syn.source == src and syn.dest == dest:
                 return syn
 
         return None
 
+    def _n_axon2lcn_ex(self) -> LCN_EX:
+        """Convert #N(of axons) to `LCN_EX` & check.
+
+        NOTE: LCN_EX = log2[ceil(#N/fan-in per dendrite)], where `LCN_1X` = 0.
+        """
+        if self.n_axon < 1:
+            raise ValueError(
+                f"the number of axons must be positive, but got {self.n_axon}."
+            )
+
+        if (
+            lcn := ((self.n_axon - 1) // self.n_fanin_max).bit_length()
+        ) > LCN_EX.LCN_64X:
+            _max_n_axons = self.n_fanin_max * (1 << LCN_EX.LCN_64X)
+            raise ResourceError(
+                f"required LCN extension out of range {LCN_EX.LCN_64X} ({lcn}). "
+                f"The number of axons must be <= {_max_n_axons}. "
+                f"But synapses {self._obj_repr()} have a total of {self.n_axon} axons."
+            )
+
+        return LCN_EX(lcn)
+
     def copy(self):
         raise NotImplementedError
 
     """Interfaces"""
 
     @property
     def obj(self) -> Tuple[SynSys, ...]:
@@ -193,21 +200,24 @@
         )
 
     @property
     def n_core_required(self) -> int:
         return len(self.neuron_segs_of_cb)
 
     @property
+    def weight_precision(self) -> WP:
+        # Optimized in `s.weight_precision`.
+        return max(s.weight_precision for s in self.obj)
+
+    @property
     def n_dendrite_per_neuron(self) -> int:
-        """Multiple dendrites will be combined to achieve higher    \
-            precision weights.
+        """Multiple dendrites will be combined to achieve higher precision weights.
 
-        FIXME The limit on the number of dendrites in SNN/ANN modes \
-            is different, which affects the capacity of neurons in  \
-            physical core.
+        FIXME The limit on the number of dendrites in SNN/ANN modes is different, which affects \
+            the capacity of neurons in physical core.
         """
         return 1 << self.weight_precision
 
     @property
     def n_weight_bits(self) -> int:
         return self.n_dendrite_per_neuron
 
@@ -216,15 +226,15 @@
         return self._lcn_ex
 
     @lcn_ex.setter
     def lcn_ex(self, lcn_ex: LCN_EX) -> None:
         """Set or adjust the `lcn_ex` & lock."""
         if lcn_ex > LCN_EX.LCN_64X:
             raise ResourceError(
-                f"LCN extension required out of {LCN_EX.LCN_64X}: {lcn_ex}"
+                f"required LCN extension out of range {LCN_EX.LCN_64X} ({lcn_ex})."
             )
 
         self._lcn_ex = lcn_ex
         self.lcn_locked = True
 
     @property
     def n_timeslot(self) -> int:
@@ -333,38 +343,29 @@
 
     def __repr__(self) -> str:
         return f"<{self.name} at 0x{id(self):x} of target '{self.obj}'>"
 
     def __str__(self) -> str:
         return f"<{self.name} of target '{self.obj}'>"
 
-    @classmethod
-    def build(cls, *synapses: SynSys, seed: int = 0, enable_wp_opt: bool):
-        """Combine the SAME weight precision synapses and build the `CoreBlock`."""
-        SynSys.CFLAG_ENABLE_WP_OPTIMIZATION = enable_wp_opt  # TODO OK but ugly
-
-        wp0 = synapses[0].weight_precision
-        # Check wether weight precision of all synapses equal.
-        if not all(wp0 == s.weight_precision for s in synapses):
-            raise NotSupportedError("mixed weight precision is not supported yet.")
-
-        if wp0 > max(cls.SUPPORTED_WP):
-            raise NotSupportedError(f"{wp0.name} is not supported yet.")
-
-        elif wp0 not in cls.SUPPORTED_WP:
-            # Treat lower bit weights as 8-bit weights.
-            wp0 = cls.SUPPORTED_WP[-1]
+    def _obj_repr(self) -> str:
+        """The representation of the names of target objects."""
+        return ", ".join(n.name for n in self.obj)
 
+    @classmethod
+    def build(cls, *synapses: SynSys, seed: int = 0):
+        """Group synapses & build `CoreBlock`."""
         # FIXME where does the parameter check do?
         if seed > (1 << 64) - 1:
             warnings.warn(
-                f"random seed {seed} is too large, truncated into 64 bits.", UserWarning
+                f"random seed {seed} is too large, truncated into 64 bits.",
+                TruncationWarning,
             )
 
-        return cls(*synapses, weight_precision=wp0, seed=seed)
+        return cls(*synapses, seed=seed)
 
     @classmethod
     def export_core_plm_config(cls, cb: "CoreBlock") -> Dict[Coord, CoreConfig]:
         """Export the parameters of the core into a dictionary."""
         cb_config = dict()
 
         for coord, core_plm in cb.core_placements.items():
@@ -710,31 +711,14 @@
     def n_core_required(self):
         return 1
 
     def __len__(self) -> int:
         return self.n_core_required
 
 
-def n_axon2lcn_ex(n_axon: int, fan_in_max: int) -> LCN_EX:
-    """Convert #N(of axons) to `LCN_EX`.
-
-    Description:
-        LCN_EX = log2[ceil(#N/fan-in per dendrite)], where LCN_EX = 0 is `LCN_1X`.
-    """
-    if n_axon < 1:
-        raise ValueError(f"the number of axons must be positive, but got {n_axon}.")
-
-    if (lcn_bit := ((n_axon - 1) // fan_in_max).bit_length()) > LCN_EX.LCN_64X:
-        raise ResourceError(
-            f"LCN extension required out of range {LCN_EX.LCN_64X} ({lcn_bit})."
-        )
-
-    return LCN_EX(lcn_bit)
-
-
 def max_lcn_of_cb(cb: List[CoreBlock]) -> LCN_EX:
     """Find the max LCN extenion of previous grouped synapses"""
     return max(cb, key=lambda cb: cb.lcn_ex).lcn_ex
 
 
 def _neuron_repl_prop(nbits: int, ntimeslot: int) -> int:
     """Get the proportion of neuron replication.
```

### Comparing `paibox-1.0.0a7/paibox/backend/routing.py` & `paibox-1.0.0b1/paibox/backend/routing.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0a7/paibox/backend/segment_utils.py` & `paibox-1.0.0b1/paibox/backend/segment_utils.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0a7/paibox/base.py` & `paibox-1.0.0b1/paibox/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import sys
-from typing import Any, ClassVar, Dict, List, Literal, Optional, Set, Tuple, Union
+from typing import Any, ClassVar, Dict, List, Literal, Optional, Set, Tuple
 
 import numpy as np
-from numpy.typing import NDArray
 
 if sys.version_info >= (3, 10):
     from typing import TypeAlias
 else:
     from typing_extensions import TypeAlias
 
+from paicorelib import WeightPrecision as WP
+
 from .collector import Collector
 from .mixin import ReceiveInputProj, StatusMemory, TimeRelatedNode
 from .naming import get_unique_name, is_name_unique
 from .node import NodeDict, NodeList
 from .types import WeightType
 
 __all__ = []
@@ -319,19 +320,19 @@
     """Compilation flag for weight precision optimization."""
 
     @property
     def weights(self) -> WeightType:
         raise NotImplementedError
 
     @property
-    def weight_precision(self):
+    def weight_precision(self) -> WP:
         raise NotImplementedError
 
     @property
-    def connectivity(self) -> NDArray[Union[np.bool_, np.int8]]:
+    def connectivity(self) -> WeightType:
         raise NotImplementedError
 
     @property
     def n_axon_each(self) -> np.ndarray:
         return np.sum(self.connectivity, axis=0)
 
     @property
```

### Comparing `paibox-1.0.0a7/paibox/collector.py` & `paibox-1.0.0b1/paibox/collector.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0a7/paibox/context.py` & `paibox-1.0.0b1/paibox/context.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0a7/paibox/exceptions.py` & `paibox-1.0.0b1/paibox/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -58,7 +58,13 @@
     pass
 
 
 class TruncationWarning(PAIBoxWarning, UserWarning):
     """Value out of range & will be truncated."""
 
     pass
+
+
+class AutoOptimizationWarning(PAIBoxWarning):
+    """Parameters are optimized automatically by PAIBox."""
+
+    pass
```

### Comparing `paibox-1.0.0a7/paibox/mixin.py` & `paibox-1.0.0b1/paibox/mixin.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0a7/paibox/naming.py` & `paibox-1.0.0b1/paibox/naming.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0a7/paibox/network.py` & `paibox-1.0.0b1/paibox/network.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0a7/paibox/neuron/base.py` & `paibox-1.0.0b1/paibox/neuron/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,23 +10,22 @@
     RM,
     SIM,
     TM,
     HwConfig,
     MaxPoolingEnable,
     SpikeWidthFormat,
 )
-from typing_extensions import TypeAlias
 
 from paibox.base import NeuDyn
-from paibox.types import Shape, SpikeType
+from paibox.types import Shape, SpikeType, VoltageType
 from paibox.utils import as_shape, shape2num
 
-__all__ = ["Neuron"]
+from .utils import _vjt_overflow
 
-VoltageType: TypeAlias = NDArray[np.int32]
+__all__ = ["Neuron"]
 
 
 class MetaNeuron:
     """Meta neuron"""
 
     def __init__(
         self,
@@ -61,15 +60,14 @@
         self.neg_threshold: int = neg_threshold  # Unsigned 29-bit
         self.pos_threshold: int = pos_threshold  # Unsigned 29-bit
         self.leak_direction: LDM = leak_direction
         self.leak_integration_mode: LIM = leak_integration_mode
         self.leak_v: int = leak_v  # Signed 30-bit
         self.synaptic_integration_mode: SIM = synaptic_integration_mode
         self.bit_truncation: int = bit_truncation  # Unsigned 5-bit
-        self._vjt_init = 0  # Signed 30-bit. Fixed.
 
         # TODO These two config below are parameters of CORE.
         self._spike_width_format: SpikeWidthFormat
         self._pool_max_en: MaxPoolingEnable
 
         # Auxiliary attributes or variables.
         self._thres_mask: int = (1 << threshold_mask_bits) - 1
@@ -86,29 +84,28 @@
 
             If synaptic integration mode is deterministic, then
                 `vjt` = `vjt_pre` + \sum^{N-1}_{i=0} * x_i(t) * w_{i,j} (incoming_v)
             else (stochastic)
                 `vjt` = `vjt_pre` + `_rho_w_ij` * \sum^{N-1}_{i=0} * x_i(t) * w_{i,j}
         """
         _rho_w_ij = 1  # Random synaptic integration enable, 0/1
-        xt = self.init_param(0).astype(np.int32)
 
         if self.synaptic_integration_mode is SIM.MODE_STOCHASTIC:
             raise NotImplementedError(
                 f"mode {SIM.MODE_STOCHASTIC.name} is not implemented."
             )
         else:
             if incoming_v.ndim == 2:
                 _v = incoming_v.sum(axis=1).astype(np.int32)
             else:
                 _v = incoming_v
 
         v_charged = np.add(vjt_pre, _v).astype(np.int32)
 
-        return v_charged
+        return _vjt_overflow(v_charged)  # Handle with overflow here
 
     def _neuronal_leak(self, vjt: VoltageType) -> VoltageType:
         r"""2. Leak integration.
 
         2.1 Leak direction, forward or reversal.
             If leak direction is `MODE_FORWARD`, the `_ld` is 1, else is \sgn{`vjt`}.
 
@@ -352,15 +349,14 @@
     def bias(self) -> int:
         """Signed 30-bit. ANN mode only."""
         return self.leak_v
 
 
 class Neuron(MetaNeuron, NeuDyn):
     _excluded_vars = (
-        "_vjt_init",
         "vjt",
         "vj",
         "y",
         "threshold_mode",
         "spike",
         "v_th_rand",
         "_spike_width_format",
@@ -439,19 +435,20 @@
             synaptic_integration_mode,
             bit_truncation,
             keep_shape,
         )
         super(MetaNeuron, self).__init__(name)
 
         """Stateful attributes. Vector."""
-        self.set_memory("_vjt", self.init_param(self._vjt_init).astype(np.int32))
+        # Initial vjt is fixed at 0.
+        self.set_memory("_vjt", self.init_param(0).astype(np.int32))
         self.set_memory("_inner_spike", self.init_param(0).astype(np.bool_))
 
         # Not supported for attributes in ANN mode
-        self.set_memory("vj", self.init_param(self._vjt_init).astype(np.int32))
+        self.set_memory("vj", self.init_param(0).astype(np.int32))
         self.set_memory("y", self.init_param(0).astype(np.int32))
 
         """Auxiliary internal stateful attributes for debugging"""
         self.set_memory(
             "_debug_thres_mode", self.init_param(TM.NOT_EXCEEDED).astype(np.uint8)
         )
 
@@ -489,18 +486,16 @@
             self._inner_spike = self.init_param(0).astype(np.bool_)
             return None
 
         # The neuron is going to work.
         if x is None:
             x = self.sum_inputs()
 
-        incoming_v = _vjt_overflow(x)
-
         self._inner_spike, self._vjt, self._debug_thres_mode = super().update(
-            incoming_v, self._vjt
+            x, self._vjt
         )
 
         idx = (self.timestamp + self.delay_relative - 1) % HwConfig.N_TIMESLOT_MAX
         self.delay_registers[idx] = self._inner_spike.copy()
 
         return self._inner_spike
 
@@ -571,30 +566,7 @@
     @property
     def feature_map(self) -> SpikeType:
         return self._inner_spike.reshape(self.varshape)
 
     @property
     def voltage(self) -> VoltageType:
         return self._vjt.reshape(self.varshape)
-
-
-VJT_MAX_LIMIT: int = 2**29 - 1
-VJT_MIN_LIMIT: int = -(2**29)
-VJT_LIMIT: int = 2**30
-
-
-def _vjt_overflow(x: np.ndarray) -> VoltageType:
-    """Handle the overflow of the membrane potential.
-
-    NOTE: If the incoming membrane potential (30-bit signed) overflows, the chip\
-        will automatically handle it. This behavior needs to be implemented in  \
-        simulation.
-    """
-    return np.where(
-        x > VJT_MAX_LIMIT,
-        x - VJT_LIMIT,
-        np.where(
-            x < VJT_MIN_LIMIT,
-            x + VJT_LIMIT,
-            x,
-        ),
-    ).astype(np.int32)
```

### Comparing `paibox-1.0.0a7/paibox/neuron/neurons.py` & `paibox-1.0.0b1/paibox/neuron/neurons.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0a7/paibox/node.py` & `paibox-1.0.0b1/paibox/node.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0a7/paibox/projection.py` & `paibox-1.0.0b1/paibox/projection.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0a7/paibox/simulator/encoder.py` & `paibox-1.0.0b1/paibox/simulator/encoder.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0a7/paibox/simulator/probe.py` & `paibox-1.0.0b1/paibox/simulator/probe.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0a7/paibox/simulator/simulator.py` & `paibox-1.0.0b1/paibox/simulator/simulator.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0a7/paibox/synapses/base.py` & `paibox-1.0.0b1/paibox/synapses/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -117,16 +117,16 @@
         return self.comm.weights
 
     @property
     def weight_precision(self) -> WP:
         return self.comm._get_wp(self.CFLAG_ENABLE_WP_OPTIMIZATION)
 
     @property
-    def connectivity(self):
-        """The connectivity matrix in `np.ndarray` format."""
+    def connectivity(self) -> WeightType:
+        """The connectivity matrix in `np.bool_` or `np.int8` format."""
         return self.comm.connectivity
 
 
 class FullConnSyn(FullConnectedSyn):
     def __init__(
         self,
         source: Union[NeuDyn, InputProj],
```

### Comparing `paibox-1.0.0a7/paibox/synapses/conv_utils.py` & `paibox-1.0.0b1/paibox/synapses/conv_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
 def _conv1d_unroll(
     in_shape: Size1Type,
     out_shape: Size1Type,
     kernel: WeightType,
     stride: Size1Type,
     # padding: Size1Type,
-):
+) -> WeightType:
     """Unroll the convolution kernel of 1d convolution into a matrix."""
     cout, cin, kl = kernel.shape
     il = in_shape[0]
     ol = out_shape[0]
 
     w_unrolled = np.zeros((cin * il, cout * ol), dtype=kernel.dtype)
     zeros_image = np.zeros((cin * il, cout, ol), dtype=kernel.dtype)
```

### Comparing `paibox-1.0.0a7/paibox/synapses/synapses.py` & `paibox-1.0.0b1/paibox/synapses/synapses.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0a7/paibox/synapses/transforms.py` & `paibox-1.0.0b1/paibox/synapses/transforms.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,14 @@
+import warnings
 from enum import Enum, auto, unique
-from typing import Type, Union
 
 import numpy as np
-from numpy.typing import NDArray
 from paicorelib import WeightPrecision as WP
 
-from paibox.exceptions import ShapeError
+from paibox.exceptions import AutoOptimizationWarning, ShapeError
 from paibox.types import DataArrayType, IntScalarType, SynOutType, WeightType
 from paibox.utils import is_shape
 
 from .conv_utils import (
     Size1Type,
     Size2Type,
     _conv1d_faster,
@@ -58,59 +57,107 @@
     Identity = auto()
     """Identity connection with scaling factor."""
 
     All2All = auto()
     """All-to-all connection."""
 
 
-def _get_weight_precision(weight: np.ndarray, enable_wp_opt: bool) -> WP:
-    """Get the actual weight_precision of the weight."""
-    _max = np.max(weight, axis=None).astype(np.int32)
-    _min = np.min(weight, axis=None).astype(np.int32)
+def _set_coarse_dtype(raw_w: DataArrayType) -> WeightType:
+    """Convert raw weights to `np.ndarray` coarsely (without optimization).
+
+    Description:
+        - For weights of type `bool` or `np.bool_`, set `np.bool_` as the dtype.
+        - For integer scalar weight, set the dtype according to its value.
+        - For array weights, set the dtype according to its minimum & maximum values. For weights in the\
+            range of int8, the dtype when declared will be followed (i.e. not optimized).
+
+    NOTE: Only when the weight is input in integer scalar form, the weight precision will be optimized  \
+        automatically. 0/1 is treated as bool_ while others are treated as int8. The weights must not   \
+        exceed the range of int8.
+    """
+    if isinstance(raw_w, (bool, np.bool_, int, np.integer)):
+        if raw_w > MAX_INT8 or raw_w < MIN_INT8:
+            raise ValueError(f"weight out of range int8, got {raw_w}.")
+
+        if raw_w <= MAX_INT1 and raw_w >= MIN_INT1:
+            _dtype = np.bool_
+        else:
+            _dtype = np.int8
+
+        return np.asarray(raw_w, dtype=_dtype)
+
+    # Convert list or tuple to np.ndarray
+    _array = np.asarray(raw_w)
+    _max = np.max(_array, axis=None)
+    _min = np.min(_array, axis=None)
 
     if _max > MAX_INT8 or _min < MIN_INT8:
-        raise ValueError(f"weight precision out of range [{_min}, {_max}].")
+        raise ValueError(f"weight out of range int8, got [{_min}, {_max}].")
+
+    if _array.dtype > np.int8:
+        # XXX If it is automatically optimized to int8, it cannot be converted using the 'same_kind' rule.
+        # if _max <= MAX_INT1 and _min >= MIN_INT1:
+        #     warnings.warn(
+        #         f"dtype of weight is optimized automatically, {_array.dtype} -> bool.",
+        #         AutoOptimizationWarning,
+        #     )
+        #     _dtype = np.bool_
+        # else:
+        warnings.warn(
+            f"dtype of weight is optimized automatically, {_array.dtype} -> int8.",
+            AutoOptimizationWarning,
+        )
+        _dtype = np.int8
 
-    if _max <= MAX_INT1 and _min >= MIN_INT1:
-        return WP.WEIGHT_WIDTH_1BIT
-    elif enable_wp_opt:
-        if _max <= MAX_INT2 and _min >= MIN_INT2:
+    elif _array.dtype == np.bool_ or _array.dtype == np.int8:
+        _dtype = _array.dtype
+    else:
+        raise TypeError(f"weights must be bool or int8, but got {_array.dtype}.")
+
+    return _array.astype(_dtype, casting="same_kind")
+
+
+def _get_weight_precision(weight: WeightType, enable_wp_opt: bool) -> WP:
+    """Get the actual weight_precision of the weight."""
+    _max = np.max(weight, axis=None)
+    _min = np.min(weight, axis=None)
+
+    if enable_wp_opt:
+        if _max <= MAX_INT1 and _min >= MIN_INT1:
+            return WP.WEIGHT_WIDTH_1BIT
+        elif _max <= MAX_INT2 and _min >= MIN_INT2:
             return WP.WEIGHT_WIDTH_2BIT
         elif _max <= MAX_INT4 and _min >= MIN_INT4:
             return WP.WEIGHT_WIDTH_4BIT
         else:
             return WP.WEIGHT_WIDTH_8BIT
     else:
-        return WP.WEIGHT_WIDTH_8BIT
+        # If weight precision opt is disabled, return WP1 if dtype is np.bool_ else WP8.
+        if weight.dtype == np.bool_:
+            return WP.WEIGHT_WIDTH_1BIT
+        else:
+            return WP.WEIGHT_WIDTH_8BIT
 
 
 class Transform:
-    def __init__(self, weights: WeightType) -> None:
-        self.weights = weights
-        """The actual weights in synapse. Must stored in `np.int8` format."""
+    def __init__(self, weights: DataArrayType) -> None:
+        self.weights = _set_coarse_dtype(weights)
+
+        """The actual weights in synapses. Stored in `np.bool_` or `np.int8` format."""
         self.weights.setflags(write=False)
 
     def __call__(self, *args, **kwargs) -> SynOutType:
         """Ensure that in all subclasses, the output dimensions are (M,)."""
         raise NotImplementedError
 
     def _get_wp(self, enable_wp_opt: bool) -> WP:
-        """Precision of weights."""
         return _get_weight_precision(self.weights, enable_wp_opt)
 
     @property
-    def conn_dtype(self) -> Union[Type[np.bool_], Type[np.int8]]:
-        # The value of `enable_wp_opt` dosen't effect the dtype of `connectivity`.
-        if self._get_wp(enable_wp_opt=False) is WP.WEIGHT_WIDTH_1BIT:
-            return np.bool_
-        else:
-            return np.int8
-
-    @property
-    def connectivity(self) -> NDArray[Union[np.bool_, np.int8]]:
+    def connectivity(self) -> WeightType:
         """The connectivity matrix in `np.ndarray` format."""
         raise NotImplementedError
 
 
 class OneToOne(Transform):
     def __init__(self, num: int, weights: DataArrayType) -> None:
         """
@@ -128,34 +175,34 @@
                      [0, 0, z]]
         """
         self.num = num
 
         if isinstance(weights, np.ndarray) and not is_shape(weights, (num,)):
             raise ShapeError(f"expected shape is ({num},), but got {weights.shape}.")
 
-        # The ndim of weights = 0 or 1.
-        _w = np.asarray(weights, dtype=np.int8)
-
-        if _w.ndim not in (0, 1):
-            raise ShapeError(f"the ndim of weights must be 0 or 1, but got {_w.ndim}.")
+        super().__init__(weights)
 
-        super().__init__(_w)
+        # The ndim of weights = 0 or 1.
+        if self.weights.ndim not in (0, 1):
+            raise ShapeError(
+                f"the ndim of weights must be 0 or 1, but got {self.weights.ndim}."
+            )
 
     def __call__(self, x: np.ndarray, *args, **kwargs) -> SynOutType:
         # (N,) * (N,) -> (N,)
         output = x * self.weights.copy()
 
         return output.astype(np.int32)
 
     @property
     def connectivity(self):
         return (
-            (self.weights * np.eye(self.num, dtype=np.bool_)).astype(self.conn_dtype)
+            (self.weights * np.eye(self.num, dtype=np.bool_))
             if self.weights.ndim == 0
-            else np.diag(self.weights).astype(self.conn_dtype)
+            else np.diag(self.weights)
         )
 
 
 class Identity(OneToOne):
     def __init__(self, num: int, scaling_factor: IntScalarType = 1) -> None:
         """
         Arguments:
@@ -179,20 +226,20 @@
                      [g, h, i]]
         """
         self.conn_size = conn_size
 
         if isinstance(weights, np.ndarray) and not is_shape(weights, conn_size):
             raise ShapeError(f"expected shape is {conn_size}, but got {weights.shape}.")
 
-        _w = np.asarray(weights, dtype=np.int8)
-
-        if _w.ndim not in (0, 2):
-            raise ShapeError(f"the ndim of weights must be 0 or 2, but got {_w.ndim}.")
+        super().__init__(weights)
 
-        super().__init__(_w)
+        if self.weights.ndim not in (0, 2):
+            raise ShapeError(
+                f"the ndim of weights must be 0 or 2, but got {self.weights.ndim}."
+            )
 
     def __call__(self, x: np.ndarray, *args, **kwargs) -> SynOutType:
         """
         NOTE:
             - When weights is a scalar, the output is a scalar (sum * w) & repeated     \
                 `conn_size[1]` times.
             - When weights is a matrix, the output is the dot product of `x` & weights.
@@ -206,43 +253,36 @@
             output = x @ self.weights.copy().astype(np.int32)
 
         return output
 
     @property
     def connectivity(self):
         return (
-            self.weights.astype(self.conn_dtype)
+            self.weights
             if self.weights.ndim == 2
-            else (self.weights * np.ones(self.conn_size, dtype=np.bool_)).astype(
-                self.conn_dtype
-            )
+            else (self.weights * np.ones(self.conn_size, dtype=np.bool_))
         )
 
 
 class MaskedLinear(Transform):
-    def __init__(
-        self,
-        conn_size: Size2Type,
-        weights: np.ndarray,
-    ) -> None:
+    def __init__(self, conn_size: Size2Type, weights: np.ndarray) -> None:
         if not is_shape(weights, conn_size):
             raise ShapeError(f"expected shape is {conn_size}, but got {weights.shape}.")
 
-        _w = np.asarray(weights, dtype=np.int8)
-        super().__init__(_w)
+        super().__init__(weights)
 
     def __call__(self, x: np.ndarray, *args, **kwargs) -> SynOutType:
         # (N,) @ (N, M) -> (M,)
         output = x @ self.weights.copy().astype(np.int32)
 
         return output.astype(np.int32)
 
     @property
     def connectivity(self):
-        return self.weights.astype(self.conn_dtype)
+        return self.weights
 
 
 class Conv1dForward(Transform):
     def __init__(
         self,
         in_shape: Size1Type,
         out_shape: Size1Type,
@@ -253,16 +293,15 @@
     ) -> None:
         self.in_shape = in_shape
         self.out_shape = out_shape
         self.stride = stride
         self.padding = padding
         self.fm_order = fm_order
 
-        _w = kernel.astype(np.int8)
-        super().__init__(_w)
+        super().__init__(kernel)
 
     def __call__(self, x: np.ndarray, *args, **kwargs) -> SynOutType:
         cin = self.weights.shape[1]
 
         if self.fm_order == "LC":
             # (N,) -> (L, C) -> (C, L)
             _x = x.reshape(self.in_shape + (cin,)).T
@@ -277,17 +316,15 @@
             self.padding,
         )
 
         return o_conv1d.flatten()
 
     @property
     def connectivity(self):
-        return _conv1d_unroll(
-            self.in_shape, self.out_shape, self.weights, self.stride
-        ).astype(self.conn_dtype)
+        return _conv1d_unroll(self.in_shape, self.out_shape, self.weights, self.stride)
 
 
 class Conv2dForward(Transform):
     def __init__(
         self,
         in_shape: Size2Type,
         out_shape: Size2Type,
@@ -298,16 +335,15 @@
     ) -> None:
         self.in_shape = in_shape
         self.out_shape = out_shape
         self.stride = stride
         self.padding = padding
         self.fm_order = fm_order
 
-        _w = kernel.astype(np.int8)
-        super().__init__(_w)
+        super().__init__(kernel)
 
     def __call__(self, x: np.ndarray, *args, **kwargs) -> SynOutType:
         cin = self.weights.shape[1]
 
         if self.fm_order == "HWC":
             # (N,) -> (H, W, C) -> (C, H, W)
             _x = x.reshape(self.in_shape + (cin,)).transpose(2, 0, 1)
@@ -322,10 +358,8 @@
             self.padding,
         )
 
         return o_conv2d.flatten()
 
     @property
     def connectivity(self):
-        return _conv2d_unroll(
-            self.in_shape, self.out_shape, self.weights, self.stride
-        ).astype(self.conn_dtype)
+        return _conv2d_unroll(self.in_shape, self.out_shape, self.weights, self.stride)
```

### Comparing `paibox-1.0.0a7/paibox/types.py` & `paibox-1.0.0b1/paibox/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     Iterator,
     List,
     MutableSet,
     NoReturn,
     Optional,
     Tuple,
     TypeVar,
+    Union,
 )
 
 import numpy as np
 from numpy.typing import NDArray
 
 Shape = TypeVar("Shape", int, Tuple[int, ...], List[int])
 ArrayType = TypeVar("ArrayType", List[int], Tuple[int, ...], np.ndarray)
@@ -21,15 +22,16 @@
 IntScalarType = TypeVar("IntScalarType", int, np.bool_, np.integer)
 DataType = TypeVar("DataType", int, np.bool_, np.integer, np.ndarray)
 DataArrayType = TypeVar(
     "DataArrayType", int, np.bool_, np.integer, List[int], Tuple[int, ...], np.ndarray
 )
 SpikeType = NDArray[np.bool_]
 SynOutType = NDArray[np.int32]
-WeightType = NDArray[np.int8]  # raw int8 weights
+VoltageType = NDArray[np.int32]
+WeightType = NDArray[Union[np.bool_, np.int8]]
 
 _T = TypeVar("_T")
 
 
 class FrozenOrderedSet(AbstractSet, Generic[_T]):
     """A set that preserves insertion order and is hashable."""
```

### Comparing `paibox-1.0.0a7/paibox/utils.py` & `paibox-1.0.0b1/paibox/utils.py`

 * *Files identical despite different names*

### Comparing `paibox-1.0.0a7/pyproject.toml` & `paibox-1.0.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paibox"
-version = "1.0.0a7"
+version = "1.0.0b1"
 description = "New toolbox of PAICORE 2.0."
 authors = ["Ziru Pan <zrpan@stu.pku.edu.cn>"]
 maintainers = ["Ziru Pan <zrpan@stu.pku.edu.cn>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 repository = "https://github.com/PAICookers/PAIBox"
 homepage = "https://github.com/PAICookers/PAIBox"
@@ -30,15 +30,15 @@
 include = ["docs", "CHANGELOG.md"]
 # Excludes the experimental code
 exclude = ["paibox/experimental"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^2.0"
-numpy = "^1.23.0"
+numpy = "^1.24.0"
 paicorelib = "0.0.13"
 
 [tool.poetry.group.test]
 optional = true
 
 
 [tool.poetry.group.test.dependencies]
```

### Comparing `paibox-1.0.0a7/PKG-INFO` & `paibox-1.0.0b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paibox
-Version: 1.0.0a7
+Version: 1.0.0b1
 Summary: New toolbox of PAICORE 2.0.
 Home-page: https://github.com/PAICookers/PAIBox
 License: GPL-3.0-or-later
 Keywords: PAICORE 2.0,PAIBox,Toolbox
 Author: Ziru Pan
 Author-email: zrpan@stu.pku.edu.cn
 Maintainer: Ziru Pan
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries
-Requires-Dist: numpy (>=1.23.0,<2.0.0)
+Requires-Dist: numpy (>=1.24.0,<2.0.0)
 Requires-Dist: paicorelib (==0.0.13)
 Requires-Dist: pydantic (>=2.0,<3.0)
 Project-URL: Documentation, https://github.com/PAICookers/PAIBox#readme
 Project-URL: Repository, https://github.com/PAICookers/PAIBox
 Description-Content-Type: text/markdown
 
 <div align="center">
@@ -36,15 +36,15 @@
 
 </div>
 
 <p align="center">
     <a href="https://github.com/PAICookers/PAIBox/blob/master/pyproject.toml">
         <img src="https://img.shields.io/pypi/pyversions/paibox">
     </a>
-    <a href="https://github.com/PAICookers/PAIBox/releases/tag/v1.0.0a7">
+    <a href="https://github.com/PAICookers/PAIBox/releases/tag/v1.0.0b1">
         <img src="https://img.shields.io/github/v/release/PAICookers/PAIBox?include_prereleases&color=orange">
     </a>
     <a href="https://www.codefactor.io/repository/github/PAICookers/PAIBox">
       <img src="https://img.shields.io/codefactor/grade/github/PAICookers/PAIBox/master?color=red">
     </a>
     <a href="https://results.pre-commit.ci/latest/github/PAICookers/PAIBox/master">
 	   <img src="https://results.pre-commit.ci/badge/github/PAICookers/PAIBox/master.svg" alt="pre-commit.ci status">
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
-Metadata-Version: 2.1 Name: paibox Version: 1.0.0a7 Summary: New toolbox of
+Metadata-Version: 2.1 Name: paibox Version: 1.0.0b1 Summary: New toolbox of
 PAICORE 2.0. Home-page: https://github.com/PAICookers/PAIBox License: GPL-3.0-
 or-later Keywords: PAICORE 2.0,PAIBox,Toolbox Author: Ziru Pan Author-email:
 zrpan@stu.pku.edu.cn Maintainer: Ziru Pan Maintainer-email:
 zrpan@stu.pku.edu.cn Requires-Python: >=3.8,<4.0 Classifier: Intended Audience
 :: Science/Research Classifier: License :: OSI Approved :: GNU General Public
 License v3 or later (GPLv3+) Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only Classifier: Topic ::
 Scientific/Engineering :: Artificial Intelligence Classifier: Topic :: Software
 Development :: Build Tools Classifier: Topic :: Software Development ::
-Libraries Requires-Dist: numpy (>=1.23.0,<2.0.0) Requires-Dist: paicorelib
+Libraries Requires-Dist: numpy (>=1.24.0,<2.0.0) Requires-Dist: paicorelib
 (==0.0.13) Requires-Dist: pydantic (>=2.0,<3.0) Project-URL: Documentation,
 https://github.com/PAICookers/PAIBox#readme Project-URL: Repository, https://
 github.com/PAICookers/PAIBox Description-Content-Type: text/markdown
                                    # PAIBox
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_p_y_v_e_r_s_i_o_n_s_/_p_a_i_b_o_x_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/
     _v_/_r_e_l_e_a_s_e_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_B_o_x_?_i_n_c_l_u_d_e___p_r_e_r_e_l_e_a_s_e_s_&_c_o_l_o_r_=_o_r_a_n_g_e_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_c_o_d_e_f_a_c_t_o_r_/_g_r_a_d_e_/_g_i_t_h_u_b_/_P_A_I_C_o_o_k_e_r_s_/_P_A_I_B_o_x_/_m_a_s_t_e_r_?_c_o_l_o_r_=_r_e_d_]_[_p_r_e_-
```

