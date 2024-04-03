# Comparing `tmp/yanhekt-2.2.0.tar.gz` & `tmp/yanhekt-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yanhekt-2.2.0.tar", last modified: Tue Apr  2 12:11:33 2024, max compression
+gzip compressed data, was "yanhekt-2.3.3.tar", last modified: Wed Apr  3 08:57:48 2024, max compression
```

## Comparing `yanhekt-2.2.0.tar` & `yanhekt-2.3.3.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 12:11:33.571871 yanhekt-2.2.0/
--rw-rw-rw-   0        0        0    17098 2023-04-01 15:42:28.000000 yanhekt-2.2.0/LICENSE
--rw-rw-rw-   0        0        0    26270 2024-04-02 12:11:33.570865 yanhekt-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      720 2024-04-02 12:11:28.000000 yanhekt-2.2.0/pyproject.toml
--rw-rw-rw-   0        0        0     5685 2024-04-02 12:08:41.000000 yanhekt-2.2.0/readme.md
--rw-rw-rw-   0        0        0       42 2024-04-02 12:11:33.571871 yanhekt-2.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-02 12:11:33.552585 yanhekt-2.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-02 12:11:33.560783 yanhekt-2.2.0/src/yanhekt/
--rw-rw-rw-   0        0        0      239 2024-04-02 12:11:06.000000 yanhekt-2.2.0/src/yanhekt/__init__.py
--rw-rw-rw-   0        0        0    11381 2024-04-02 08:31:00.000000 yanhekt-2.2.0/src/yanhekt/m3u8dl.py
--rw-rw-rw-   0        0        0     6013 2024-04-02 12:06:27.000000 yanhekt-2.2.0/src/yanhekt/main.py
-drwxrwxrwx   0        0        0        0 2024-04-02 12:11:33.569899 yanhekt-2.2.0/src/yanhekt.egg-info/
--rw-rw-rw-   0        0        0    26270 2024-04-02 12:11:33.000000 yanhekt-2.2.0/src/yanhekt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      310 2024-04-02 12:11:33.000000 yanhekt-2.2.0/src/yanhekt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 12:11:33.000000 yanhekt-2.2.0/src/yanhekt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       46 2024-04-02 12:11:33.000000 yanhekt-2.2.0/src/yanhekt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-04-02 12:11:33.000000 yanhekt-2.2.0/src/yanhekt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-02 12:11:33.000000 yanhekt-2.2.0/src/yanhekt.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 08:57:48.499495 yanhekt-2.3.3/
+-rw-rw-rw-   0        0        0    17098 2023-04-01 15:42:28.000000 yanhekt-2.3.3/LICENSE
+-rw-rw-rw-   0        0        0    27047 2024-04-03 08:57:48.497497 yanhekt-2.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      822 2024-04-03 08:55:36.000000 yanhekt-2.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0     6426 2024-04-03 08:53:29.000000 yanhekt-2.3.3/readme.md
+-rw-rw-rw-   0        0        0       42 2024-04-03 08:57:48.499495 yanhekt-2.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 08:57:48.476171 yanhekt-2.3.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 08:57:48.486742 yanhekt-2.3.3/src/yanhekt/
+-rw-rw-rw-   0        0        0      241 2024-04-03 08:12:49.000000 yanhekt-2.3.3/src/yanhekt/__init__.py
+-rw-rw-rw-   0        0        0     8028 2024-04-03 08:56:47.000000 yanhekt-2.3.3/src/yanhekt/gui.py
+-rw-rw-rw-   0        0        0    11603 2024-04-03 08:57:01.000000 yanhekt-2.3.3/src/yanhekt/m3u8dl.py
+-rw-rw-rw-   0        0        0     3468 2024-04-03 08:57:13.000000 yanhekt-2.3.3/src/yanhekt/main.py
+-rw-rw-rw-   0        0        0     4915 2024-04-03 08:57:19.000000 yanhekt-2.3.3/src/yanhekt/yanhekt.py
+drwxrwxrwx   0        0        0        0 2024-04-03 08:57:48.496495 yanhekt-2.3.3/src/yanhekt.egg-info/
+-rw-rw-rw-   0        0        0    27047 2024-04-03 08:57:48.000000 yanhekt-2.3.3/src/yanhekt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      352 2024-04-03 08:57:48.000000 yanhekt-2.3.3/src/yanhekt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 08:57:48.000000 yanhekt-2.3.3/src/yanhekt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      114 2024-04-03 08:57:48.000000 yanhekt-2.3.3/src/yanhekt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       29 2024-04-03 08:57:48.000000 yanhekt-2.3.3/src/yanhekt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-03 08:57:48.000000 yanhekt-2.3.3/src/yanhekt.egg-info/top_level.txt
```

### Comparing `yanhekt-2.2.0/LICENSE` & `yanhekt-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yanhekt-2.2.0/PKG-INFO` & `yanhekt-2.3.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yanhekt
-Version: 2.2.0
+Version: 2.3.3
 Summary: Download Videos on BIT YanHeKT
 Author-email: GDDG08 <ZZH-Fusion@outlook.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -381,23 +381,24 @@
 Project-URL: Issues, https://github.com/GDDG08/YanHeKT_Downloader/issues
 Keywords: yanhekt,bit
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
+Requires-Dist: PySimpleGUI<=4.55.1
 
 <!--
  * @Project      : 
  * @FilePath     : \PypiPkg\readme.md
  * @Descripttion : 
  * @Author       : GDDG08
- * @Date         : 2024-04-02 20:02:11
+ * @Date         : 2024-04-03 16:48:02
  * @LastEditors  : GDDG08
- * @LastEditTime : 2024-04-02 20:08:41
+ * @LastEditTime : 2024-04-03 16:53:20
 -->
 # 北理工延河课堂视频下载
 
 欢迎Star🌟！欢迎提Issue
 
 本项目在 网协2023“十行代码”比赛 荣获**特等奖**🎉 指路👉[Github](https://github.com/BITNP/poems-2023/)
 
@@ -423,14 +424,17 @@
    - 支持一次下载全部课时，感谢@ZJC-GH同学的建议和pr
    - 支持分别或同时下载VGA和Video
    - 支持增量下载，自动跳过已下载文件
    - 更改临时文件存储位置，放在`temp`中
    - 可以自定义输出文件夹位置
    - **详见 #食用方法**
    - 优化ffmpeg输出
+- 2024-4-3 (🌟🌟)添加了GUI交互界面
+   - 基于PySimpleGUI4，可以跨平台运行
+
 
 ## 使用前准备
 
 ### 方法一：现已通过Pypi发布（推荐）
 
 https://pypi.org/project/yanhekt/
 
@@ -460,18 +464,45 @@
 
    - 本仓库的release附带了ffmpeg(仅exe)
    - 相关安装请自行搜索
      - Windows简单的方法：下载后拷贝到代码文件夹内
 
    - 如果最终视频没有合并，说明ffmpeg环境存在问题
 
+## 食用方法（GUI）
+
+1. 开启方法
+
+   1. 若使用pip安装
+
+      ```shell
+      yanhekt-gui
+      yanhekt gui
+      ```
+
+   2. 若源码运行
+
+      ```shell
+      python main.py gui
+      ```
+
+2. 开箱即食
+
+   <img src="https://github.com/GDDG08/YanHeKT_Downloader/raw/dev/assets/image-20240403163924034.png" width="250px"/>
+
+   - 扔进链接或者courseID（可Ctrl-C V）
+   - 获取课程信息
+   - 随意选择课时（Ctrl、Shift、鼠标拖拽都可多选）
+   - 设置一些参数，比如要下载什么视频
+   - 开下！
+
 
-## 食用方法
+## 食用方法（命令行）
 
-***注意：如果使用[本地源代码](#方法二：使用源代码)安装，请将本节中的`yanhekt`替换为`python main.py`***
+***注意：如果使用[本地源代码](#方法二：使用源代码)安装，请将本节中的`yanhekt`或`yanhekt-cli`替换为`python main.py`***
 
 1. 获取课程ID
 
    在课程详情页，**注意不是视频播放页**，如`https://www.yanhekt.cn/course/11111`，
 
    从url中获得课程id，如`11111`
 
@@ -555,26 +586,27 @@
 
 
 ## 作为python包使用
 
 仍处于初期开发阶段，欢迎提功能需求和PR
 
 ```python
-from yanhekt import YHKTDown
+from yanhekt import YanHeKT
 
-YHKTDown(25555, _all=True, _dual=True, _skip=True, _dir='./')
+yanhekt = YanHeKT(25555, _all=True, _dual=True, _skip=True, _dir='./')
+yanhekt.download()
 ```
 
 
 
 ## Todo（画大饼）
 
 - ~~@ZJC-GH 同学添加了批量下载功能~~
    - ~~有需要的同学可以到[这个仓库](https://github.com/ZJC-GH/YanHeKT_Downloader) release中下载使用~~
    - ~~目前已合并到dev分支~~
 - ~~计划使用`argparse`完善命令行参数，优化下交互体验~~(2.2.0已实现)
-- （超大饼）在参数写完后整个简单的gui
+- ~~（超大饼）在参数写完后整个简单的gui~~
 
 
 ## 致谢
 
 - [M3u8Download](https://github.com/anwenzen/M3u8Download)
```

### Comparing `yanhekt-2.2.0/readme.md` & `yanhekt-2.3.3/readme.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 <!--
  * @Project      : 
  * @FilePath     : \PypiPkg\readme.md
  * @Descripttion : 
  * @Author       : GDDG08
- * @Date         : 2024-04-02 20:02:11
+ * @Date         : 2024-04-03 16:48:02
  * @LastEditors  : GDDG08
- * @LastEditTime : 2024-04-02 20:08:41
+ * @LastEditTime : 2024-04-03 16:53:20
 -->
 # 北理工延河课堂视频下载
 
 欢迎Star🌟！欢迎提Issue
 
 本项目在 网协2023“十行代码”比赛 荣获**特等奖**🎉 指路👉[Github](https://github.com/BITNP/poems-2023/)
 
@@ -35,14 +35,17 @@
    - 支持一次下载全部课时，感谢@ZJC-GH同学的建议和pr
    - 支持分别或同时下载VGA和Video
    - 支持增量下载，自动跳过已下载文件
    - 更改临时文件存储位置，放在`temp`中
    - 可以自定义输出文件夹位置
    - **详见 #食用方法**
    - 优化ffmpeg输出
+- 2024-4-3 (🌟🌟)添加了GUI交互界面
+   - 基于PySimpleGUI4，可以跨平台运行
+
 
 ## 使用前准备
 
 ### 方法一：现已通过Pypi发布（推荐）
 
 https://pypi.org/project/yanhekt/
 
@@ -72,18 +75,45 @@
 
    - 本仓库的release附带了ffmpeg(仅exe)
    - 相关安装请自行搜索
      - Windows简单的方法：下载后拷贝到代码文件夹内
 
    - 如果最终视频没有合并，说明ffmpeg环境存在问题
 
+## 食用方法（GUI）
+
+1. 开启方法
+
+   1. 若使用pip安装
+
+      ```shell
+      yanhekt-gui
+      yanhekt gui
+      ```
+
+   2. 若源码运行
+
+      ```shell
+      python main.py gui
+      ```
+
+2. 开箱即食
+
+   <img src="https://github.com/GDDG08/YanHeKT_Downloader/raw/dev/assets/image-20240403163924034.png" width="250px"/>
+
+   - 扔进链接或者courseID（可Ctrl-C V）
+   - 获取课程信息
+   - 随意选择课时（Ctrl、Shift、鼠标拖拽都可多选）
+   - 设置一些参数，比如要下载什么视频
+   - 开下！
+
 
-## 食用方法
+## 食用方法（命令行）
 
-***注意：如果使用[本地源代码](#方法二：使用源代码)安装，请将本节中的`yanhekt`替换为`python main.py`***
+***注意：如果使用[本地源代码](#方法二：使用源代码)安装，请将本节中的`yanhekt`或`yanhekt-cli`替换为`python main.py`***
 
 1. 获取课程ID
 
    在课程详情页，**注意不是视频播放页**，如`https://www.yanhekt.cn/course/11111`，
 
    从url中获得课程id，如`11111`
 
@@ -167,26 +197,27 @@
 
 
 ## 作为python包使用
 
 仍处于初期开发阶段，欢迎提功能需求和PR
 
 ```python
-from yanhekt import YHKTDown
+from yanhekt import YanHeKT
 
-YHKTDown(25555, _all=True, _dual=True, _skip=True, _dir='./')
+yanhekt = YanHeKT(25555, _all=True, _dual=True, _skip=True, _dir='./')
+yanhekt.download()
 ```
 
 
 
 ## Todo（画大饼）
 
 - ~~@ZJC-GH 同学添加了批量下载功能~~
    - ~~有需要的同学可以到[这个仓库](https://github.com/ZJC-GH/YanHeKT_Downloader) release中下载使用~~
    - ~~目前已合并到dev分支~~
 - ~~计划使用`argparse`完善命令行参数，优化下交互体验~~(2.2.0已实现)
-- （超大饼）在参数写完后整个简单的gui
+- ~~（超大饼）在参数写完后整个简单的gui~~
 
 
 ## 致谢
 
 - [M3u8Download](https://github.com/anwenzen/M3u8Download)
```

### Comparing `yanhekt-2.2.0/src/yanhekt/m3u8dl.py` & `yanhekt-2.3.3/src/yanhekt/m3u8dl.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 '''
 Project      :
 FilePath     : \OPENSOURCE\m3u8dl.py
 Descripttion :
 Author       : GDDG08
 Date         : 2022-11-07 12:09:26
 LastEditors  : GDDG08
-LastEditTime : 2024-04-02 16:30:46
+LastEditTime : 2024-04-03 15:39:46
 '''
 import os
 import re
 import sys
 import queue
 import base64
 import platform
@@ -43,15 +43,15 @@
     :param url: 完整的m3u8文件链接 如"https://www.bilibili.com/example/index.m3u8"
     :param name: 保存m3u8的文件名 如"index"
     :param max_workers: 多线程最大线程数
     :param num_retries: 重试次数
     :param base64_key: base64编码的字符串
     """
 
-    def __init__(self, url, workDir, name, max_workers=64, num_retries=16, base64_key=None):
+    def __init__(self, url, workDir, name, max_workers=64, num_retries=16, base64_key=None, callback_progress=None):
 
         self._url = url
         self._token = None
         self._name = name
         self._max_workers = max_workers
         self._num_retries = num_retries
         self._workDir = os.path.join(workDir, self._name)
@@ -61,14 +61,15 @@
         self._success_sum = 0
         self._ts_sum = 0
         self._key = base64.b64decode(base64_key.encode()) if base64_key else None
         self._headers = {'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/93.0.4577.82 Safari/537.36 Edg/93.0.961.52',
                          'Origin': 'https://www.yanhekt.cn',
                          'referer': 'https://www.yanhekt.cn',
                          }
+        self._callback_progress = callback_progress
 
         urllib3.disable_warnings()
 
         self.sign_prefix = "1tJrMwNq3h0yLgx86Rued2J1tFc"
         self._url = self.encryptURL(self._url)
         # self.refreshSignature()
 
@@ -196,17 +197,19 @@
                 with requests.get(ts_url, stream=True, timeout=(5, 60), verify=False, headers=self._headers) as res:
                     if res.status_code == 200:
                         with open(name, "wb") as ts:
                             for chunk in res.iter_content(chunk_size=1024):
                                 if chunk:
                                     ts.write(chunk)
                         self._success_sum += 1
-                        sys.stdout.write('\r[%-25s](%d/%d)' % ("*" * (100 * self._success_sum // self._ts_sum // 4),
-                                                               self._success_sum, self._ts_sum))
-                        sys.stdout.flush()
+                        # sys.stdout.write('\r[%-25s](%d/%d)' % ("*" * (100 * self._success_sum // self._ts_sum // 4),
+                        #                                        self._success_sum, self._ts_sum))
+                        # sys.stdout.flush()
+                        if self._callback_progress:
+                            self._callback_progress(self._success_sum, self._ts_sum)
                     else:
                         self.refreshSignature()
                         self.download_ts(ts_url, name, num_retries - 1)
             else:
                 self._success_sum += 1
         except Exception:
             if os.path.exists(name):
```

### Comparing `yanhekt-2.2.0/src/yanhekt.egg-info/PKG-INFO` & `yanhekt-2.3.3/src/yanhekt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yanhekt
-Version: 2.2.0
+Version: 2.3.3
 Summary: Download Videos on BIT YanHeKT
 Author-email: GDDG08 <ZZH-Fusion@outlook.com>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
         --------------
@@ -381,23 +381,24 @@
 Project-URL: Issues, https://github.com/GDDG08/YanHeKT_Downloader/issues
 Keywords: yanhekt,bit
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
+Requires-Dist: PySimpleGUI<=4.55.1
 
 <!--
  * @Project      : 
  * @FilePath     : \PypiPkg\readme.md
  * @Descripttion : 
  * @Author       : GDDG08
- * @Date         : 2024-04-02 20:02:11
+ * @Date         : 2024-04-03 16:48:02
  * @LastEditors  : GDDG08
- * @LastEditTime : 2024-04-02 20:08:41
+ * @LastEditTime : 2024-04-03 16:53:20
 -->
 # 北理工延河课堂视频下载
 
 欢迎Star🌟！欢迎提Issue
 
 本项目在 网协2023“十行代码”比赛 荣获**特等奖**🎉 指路👉[Github](https://github.com/BITNP/poems-2023/)
 
@@ -423,14 +424,17 @@
    - 支持一次下载全部课时，感谢@ZJC-GH同学的建议和pr
    - 支持分别或同时下载VGA和Video
    - 支持增量下载，自动跳过已下载文件
    - 更改临时文件存储位置，放在`temp`中
    - 可以自定义输出文件夹位置
    - **详见 #食用方法**
    - 优化ffmpeg输出
+- 2024-4-3 (🌟🌟)添加了GUI交互界面
+   - 基于PySimpleGUI4，可以跨平台运行
+
 
 ## 使用前准备
 
 ### 方法一：现已通过Pypi发布（推荐）
 
 https://pypi.org/project/yanhekt/
 
@@ -460,18 +464,45 @@
 
    - 本仓库的release附带了ffmpeg(仅exe)
    - 相关安装请自行搜索
      - Windows简单的方法：下载后拷贝到代码文件夹内
 
    - 如果最终视频没有合并，说明ffmpeg环境存在问题
 
+## 食用方法（GUI）
+
+1. 开启方法
+
+   1. 若使用pip安装
+
+      ```shell
+      yanhekt-gui
+      yanhekt gui
+      ```
+
+   2. 若源码运行
+
+      ```shell
+      python main.py gui
+      ```
+
+2. 开箱即食
+
+   <img src="https://github.com/GDDG08/YanHeKT_Downloader/raw/dev/assets/image-20240403163924034.png" width="250px"/>
+
+   - 扔进链接或者courseID（可Ctrl-C V）
+   - 获取课程信息
+   - 随意选择课时（Ctrl、Shift、鼠标拖拽都可多选）
+   - 设置一些参数，比如要下载什么视频
+   - 开下！
+
 
-## 食用方法
+## 食用方法（命令行）
 
-***注意：如果使用[本地源代码](#方法二：使用源代码)安装，请将本节中的`yanhekt`替换为`python main.py`***
+***注意：如果使用[本地源代码](#方法二：使用源代码)安装，请将本节中的`yanhekt`或`yanhekt-cli`替换为`python main.py`***
 
 1. 获取课程ID
 
    在课程详情页，**注意不是视频播放页**，如`https://www.yanhekt.cn/course/11111`，
 
    从url中获得课程id，如`11111`
 
@@ -555,26 +586,27 @@
 
 
 ## 作为python包使用
 
 仍处于初期开发阶段，欢迎提功能需求和PR
 
 ```python
-from yanhekt import YHKTDown
+from yanhekt import YanHeKT
 
-YHKTDown(25555, _all=True, _dual=True, _skip=True, _dir='./')
+yanhekt = YanHeKT(25555, _all=True, _dual=True, _skip=True, _dir='./')
+yanhekt.download()
 ```
 
 
 
 ## Todo（画大饼）
 
 - ~~@ZJC-GH 同学添加了批量下载功能~~
    - ~~有需要的同学可以到[这个仓库](https://github.com/ZJC-GH/YanHeKT_Downloader) release中下载使用~~
    - ~~目前已合并到dev分支~~
 - ~~计划使用`argparse`完善命令行参数，优化下交互体验~~(2.2.0已实现)
-- （超大饼）在参数写完后整个简单的gui
+- ~~（超大饼）在参数写完后整个简单的gui~~
 
 
 ## 致谢
 
 - [M3u8Download](https://github.com/anwenzen/M3u8Download)
```

