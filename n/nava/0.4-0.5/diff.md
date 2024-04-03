# Comparing `tmp/nava-0.4.tar.gz` & `tmp/nava-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nava-0.4.tar", last modified: Mon Feb 19 07:32:43 2024, max compression
+gzip compressed data, was "nava-0.5.tar", last modified: Wed Apr  3 04:19:51 2024, max compression
```

## Comparing `nava-0.4.tar` & `nava-0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 07:32:43.053949 nava-0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-02-19 07:32:33.000000 nava-0.4/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-02-19 07:32:33.000000 nava-0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-02-19 07:32:43.053949 nava-0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-02-19 07:32:33.000000 nava-0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 07:32:43.053949 nava-0.4/nava/
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-02-19 07:32:33.000000 nava-0.4/nava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-02-19 07:32:33.000000 nava-0.4/nava/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-02-19 07:32:33.000000 nava-0.4/nava/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-02-19 07:32:33.000000 nava-0.4/nava/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-02-19 07:32:33.000000 nava-0.4/nava/params.py
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-02-19 07:32:33.000000 nava-0.4/nava/thread.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-19 07:32:43.053949 nava-0.4/nava.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9961 2024-02-19 07:32:43.000000 nava-0.4/nava.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-02-19 07:32:43.000000 nava-0.4/nava.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-19 07:32:43.000000 nava-0.4/nava.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-02-19 07:32:43.000000 nava-0.4/nava.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-02-19 07:32:43.000000 nava-0.4/nava.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-19 07:32:43.000000 nava-0.4/nava.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-19 07:32:43.053949 nava-0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-02-19 07:32:33.000000 nava-0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:19:51.755582 nava-0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-04-03 04:19:43.000000 nava-0.5/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-03 04:19:43.000000 nava-0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9744 2024-04-03 04:19:51.755582 nava-0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-04-03 04:19:43.000000 nava-0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:19:51.755582 nava-0.5/nava/
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-03 04:19:43.000000 nava-0.5/nava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-03 04:19:43.000000 nava-0.5/nava/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 04:19:43.000000 nava-0.5/nava/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7285 2024-04-03 04:19:43.000000 nava-0.5/nava/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-03 04:19:43.000000 nava-0.5/nava/params.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-03 04:19:43.000000 nava-0.5/nava/thread.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:19:51.755582 nava-0.5/nava.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9744 2024-04-03 04:19:51.000000 nava-0.5/nava.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-03 04:19:51.000000 nava-0.5/nava.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 04:19:51.000000 nava-0.5/nava.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 04:19:51.000000 nava-0.5/nava.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 04:19:51.000000 nava-0.5/nava.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-04-03 04:19:51.000000 nava-0.5/nava.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 04:19:51.755582 nava-0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-04-03 04:19:43.000000 nava-0.5/setup.py
```

### Comparing `nava-0.4/AUTHORS.md` & `nava-0.5/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `nava-0.4/LICENSE` & `nava-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nava-0.4/PKG-INFO` & `nava-0.5/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: nava
-Version: 0.4
+Version: 0.5
 Summary: A Python library for playing sound everywhere natively and securely.
 Home-page: https://github.com/openscilab/nava
-Download-URL: https://github.com/openscilab/nava/tarball/v0.4
+Download-URL: https://github.com/openscilab/nava/tarball/v0.5
 Author: OpenSciLab Development Team
 Author-email: info@openscilab.com
 License: MIT
 Project-URL: Webpage, https://openscilab.com/
 Project-URL: Source, https://github.com/openscilab/nava
 Project-URL: Discord, https://discord.gg/MCbPKCFBs3
 Keywords: sound wav music mp3 player audio
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -43,35 +43,25 @@
     <br/>
     <a href="https://www.python.org/">
         <img src="https://img.shields.io/badge/built%20with-Python3-green.svg" alt="built with Python3"/>
     </a>
     <a href="https://badge.fury.io/py/nava">
         <img src="https://badge.fury.io/py/nava.svg" alt="PyPI version" height="18">
     </a>
-	<a href="https://codecov.io/gh/openscilab/nava">
-		<img src="https://codecov.io/gh/openscilab/nava/branch/main/graph/badge.svg" alt="Codecov">
-	</a>
+    <a href="https://anaconda.org/openscilab/nava">
+	<img src="https://anaconda.org/openscilab/nava/badges/version.svg">
+    </a>
+    <a href="https://codecov.io/gh/openscilab/nava">
+        <img src="https://codecov.io/gh/openscilab/nava/branch/main/graph/badge.svg" alt="Codecov">
+    </a>
     <a href="https://discord.gg/MCbPKCFBs3">
         <img src="https://img.shields.io/discord/1064533716615049236.svg" alt="Discord Channel">
     </a>
 </div>
 
-## Table of contents
-   * [Overview](https://github.com/openscilab/nava#overview)
-   * [Installation](https://github.com/openscilab/nava#installation)
-   * [Usage](https://github.com/openscilab/nava#usage)
-   * [Engine](https://github.com/openscilab/nava#engine)
-   * [Issues & Bug Reports](https://github.com/openscilab/nava#issues--bug-reports)
-   * [Contribution](https://github.com/openscilab/nava/blob/main/.github/CONTRIBUTING.md)
-   * [Authors](https://github.com/openscilab/nava/blob/main/AUTHORS.md)
-   * [License](https://github.com/openscilab/nava/blob/main/LICENSE)
-   * [Show Your Support](https://github.com/openscilab/nava#show-your-support)
-   * [Changelog](https://github.com/openscilab/nava/blob/main/CHANGELOG.md)
-   * [Code of Conduct](https://github.com/openscilab/nava/blob/main/.github/CODE_OF_CONDUCT.md)
-
 ## Overview
 
 <p align="justify">
 Nava is a Python library that allows users to play sound in Python without any dependencies or platform restrictions. It is a cross-platform solution that runs on any operating system, including Windows, macOS, and Linux. Its lightweight and easy-to-use design makes Nava an ideal choice for developers looking to add sound functionality to their Python programs.
 </p>
 
 <table>
@@ -128,18 +118,18 @@
 </table>
 
 ## Installation
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)     
-- Run `pip install nava==0.4`
+- Run `pip install nava==0.5`
 
 ### Source code
-- Download [Version 0.4](https://github.com/openscilab/nava/archive/v0.4.zip) or [Latest Source](https://github.com/openscilab/nava/archive/dev.zip)
+- Download [Version 0.5](https://github.com/openscilab/nava/archive/v0.5.zip) or [Latest Source](https://github.com/openscilab/nava/archive/dev.zip)
 - Run `pip install .`
 
 ### Conda
 
 - Check [Conda Managing Package](https://conda.io/)
 - Update Conda using `conda update conda`
 - Run `conda install -c openscilab nava`
@@ -161,14 +151,26 @@
 import time
 from nava import play, stop
 sound_id = play("alarm.wav", async_mode=True)
 time.sleep(4)
 stop(sound_id)
 ```
 
+### Loop mode
+
+⚠️ The `loop` parameter has a default value of `False`
+⚠️ You should always set `async_mode` flag when you are using `loop`
+
+```python
+from nava import play, stop
+sound_id = play("alarm.wav", async_mode=True, loop=True)
+time.sleep(100)
+stop(sound_id)
+```
+
 ### Error
 
 ```python
 from nava import play, NavaBaseError
 
 try:
     play("alarm.wav")
@@ -231,14 +233,19 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [0.5] - 2024-04-03
+### Changed
+- `loop` parameter added to `play` function
+- `NavaThread` class modified
+- `README.md` modified
 ## [0.4] - 2024-02-19
 ### Added
 - `feature_request.yml` template
 - `config.yml` for issue template
 ### Changed
 - Bug report template modified
 - `NavaThread.stop` method bug fixed
@@ -270,12 +277,13 @@
 - `__play_linux` function
 - `__play_mac` function
 - `quote` function
 - `path_check` function
 - `play` function
 
 
-[Unreleased]: https://github.com/openscilab/nava/compare/v0.4...dev
+[Unreleased]: https://github.com/openscilab/nava/compare/v0.5...dev
+[0.5]: https://github.com/openscilab/nava/compare/v0.4...v0.5
 [0.4]: https://github.com/openscilab/nava/compare/v0.3...v0.4
 [0.3]: https://github.com/openscilab/nava/compare/v0.2...v0.3
 [0.2]: https://github.com/openscilab/nava/compare/v0.1...v0.2
 [0.1]: https://github.com/openscilab/nava/compare/bd789cc...v0.1
```

#### html2text {}

```diff
@@ -1,43 +1,34 @@
-Metadata-Version: 2.1 Name: nava Version: 0.4 Summary: A Python library for
+Metadata-Version: 2.1 Name: nava Version: 0.5 Summary: A Python library for
 playing sound everywhere natively and securely. Home-page: https://github.com/
-openscilab/nava Download-URL: https://github.com/openscilab/nava/tarball/v0.4
+openscilab/nava Download-URL: https://github.com/openscilab/nava/tarball/v0.5
 Author: OpenSciLab Development Team Author-email: info@openscilab.com License:
 MIT Project-URL: Webpage, https://openscilab.com/ Project-URL: Source, https://
 github.com/openscilab/nava Project-URL: Discord, https://discord.gg/MCbPKCFBs3
-Keywords: sound wav music mp3 player audio Classifier: Development Status :: 3
-- Alpha Classifier: Intended Audience :: Developers Classifier: Natural
-Language :: English Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Keywords: sound wav music mp3 player audio Classifier: Development Status :: 4
+- Beta Classifier: Intended Audience :: Developers Classifier: Natural Language
+:: English Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: End Users/Desktop Classifier: Intended Audience :: Manufacturing
 Classifier: Topic :: Multimedia Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players Classifier: Topic ::
 Multimedia :: Sound/Audio :: Players :: MP3 Requires-Python: >=3.6 Description-
 Content-Type: text/markdown License-File: LICENSE License-File: AUTHORS.md
 Requires-Dist: art>=1.8
          [https://github.com/openscilab/nava/raw/main/others/logo.png]
                               ************ NNaavvaa ************
 
-         _[_b_u_i_l_t_ _w_i_t_h_ _P_y_t_h_o_n_3_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_C_o_d_e_c_o_v_]_[_D_i_s_c_o_r_d_ _C_h_a_n_n_e_l_]
-## Table of contents * [Overview](https://github.com/openscilab/nava#overview)
-* [Installation](https://github.com/openscilab/nava#installation) * [Usage]
-(https://github.com/openscilab/nava#usage) * [Engine](https://github.com/
-openscilab/nava#engine) * [Issues & Bug Reports](https://github.com/openscilab/
-nava#issues--bug-reports) * [Contribution](https://github.com/openscilab/nava/
-blob/main/.github/CONTRIBUTING.md) * [Authors](https://github.com/openscilab/
-nava/blob/main/AUTHORS.md) * [License](https://github.com/openscilab/nava/blob/
-main/LICENSE) * [Show Your Support](https://github.com/openscilab/nava#show-
-your-support) * [Changelog](https://github.com/openscilab/nava/blob/main/
-CHANGELOG.md) * [Code of Conduct](https://github.com/openscilab/nava/blob/
-main/.github/CODE_OF_CONDUCT.md) ## Overview
+_[_b_u_i_l_t_ _w_i_t_h_ _P_y_t_h_o_n_3_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_h_t_t_p_s_:_/_/_a_n_a_c_o_n_d_a_._o_r_g_/_o_p_e_n_s_c_i_l_a_b_/_n_a_v_a_/_b_a_d_g_e_s_/
+                    _v_e_r_s_i_o_n_._s_v_g_]_[_C_o_d_e_c_o_v_]_[_D_i_s_c_o_r_d_ _C_h_a_n_n_e_l_]
+## Overview
 Nava is a Python library that allows users to play sound in Python without any
 dependencies or platform restrictions. It is a cross-platform solution that
 runs on any operating system, including Windows, macOS, and Linux. Its
 lightweight and easy-to-use design makes Nava an ideal choice for developers
 looking to add sound functionality to their Python programs.
 PyPI Counter               _[_h_t_t_p_:_/_/_p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_n_a_v_a_]
 Github Stars _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_o_p_e_n_s_c_i_l_a_b_/
@@ -55,26 +46,30 @@
  macOS CI      nava/actions/workflows/      actions/workflows/macOS_test.yml/
                    macOS_test.yml/                badge.svg?branch=dev]
                badge.svg?branch=main]
              _[_h_t_t_p_s_:_/_/_a_p_p_._c_o_d_a_c_y_._c_o_m_/_p_r_o_j_e_c_t_/
 Code Quality           _b_a_d_g_e_/_G_r_a_d_e_/            _[_C_o_d_e_F_a_c_t_o_r_] _[_c_o_d_e_b_e_a_t_ _b_a_d_g_e_]
              _9_c_3_8_4_b_4_e_4_0_0_3_4_0_a_e_9_4_7_7_2_c_1_d_7_e_1_8_4_2_d_0_]
 ## Installation ### PyPI - Check [Python Packaging User Guide](https://
-packaging.python.org/installing/) - Run `pip install nava==0.4` ### Source code
-- Download [Version 0.4](https://github.com/openscilab/nava/archive/v0.4.zip)
+packaging.python.org/installing/) - Run `pip install nava==0.5` ### Source code
+- Download [Version 0.5](https://github.com/openscilab/nava/archive/v0.5.zip)
 or [Latest Source](https://github.com/openscilab/nava/archive/dev.zip) - Run
 `pip install .` ### Conda - Check [Conda Managing Package](https://conda.io/) -
 Update Conda using `conda update conda` - Run `conda install -c openscilab
 nava` ## Usage ### Basic ```python from nava import play play("alarm.wav") ```
 ### Async mode â ï¸ The `async_mode` parameter has a default value of `False`
 ```python import time from nava import play, stop sound_id = play("alarm.wav",
-async_mode=True) time.sleep(4) stop(sound_id) ``` ### Error ```python from nava
-import play, NavaBaseError try: play("alarm.wav") except NavaBaseError as e:
-print(str(e)) ``` ## Engine List of different platforms and the corresponding
-engines that are used for sound playing.
+async_mode=True) time.sleep(4) stop(sound_id) ``` ### Loop mode â ï¸ The
+`loop` parameter has a default value of `False` â ï¸ You should always set
+`async_mode` flag when you are using `loop` ```python from nava import play,
+stop sound_id = play("alarm.wav", async_mode=True, loop=True) time.sleep(100)
+stop(sound_id) ``` ### Error ```python from nava import play, NavaBaseError
+try: play("alarm.wav") except NavaBaseError as e: print(str(e)) ``` ## Engine
+List of different platforms and the corresponding engines that are used for
+sound playing.
 PPllaattffoorrmm                     EEnnggiinnee        SSuuppppoorrtteedd FFoorrmmaattss
   Linux  _A_d_v_a_n_c_e_d_ _L_i_n_u_x_ _S_o_u_n_d_ _A_r_c_h_i_t_e_c_t_u_r_e          .wav
 Windows                    _W_i_n_s_o_u_n_d                 .wav
   macOS               _A_u_d_i_o_ _F_i_l_e_ _P_l_a_y            .wav,.mp3
 ## Issues & bug reports Just fill an issue and describe it. We'll check it
 ASAP! or send an email to [info@openscilab.com](mailto:info@openscilab.com
 "info@openscilab.com"). - Please complete the issue template You can also join
@@ -84,24 +79,26 @@
 ******** DDoonnaattee ttoo oouurr pprroojjeecctt ********
 If you do like our project and we hope that you do, can you please support us?
 Our project is not and is never going to be working for profit. We need the
 money just so we can continue doing what we do ;-) . _[_N_a_v_a_ _D_o_n_a_t_i_o_n_]# Changelog
 All notable changes to this project will be documented in this file. The format
 is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/) and this
 project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
-## [Unreleased] ## [0.4] - 2024-02-19 ### Added - `feature_request.yml`
-template - `config.yml` for issue template ### Changed - Bug report template
-modified - `NavaThread.stop` method bug fixed - Test system modified -
-`README.md` modified ## [0.3] - 2024-01-31 ### Added - `NavaThread` class -
-`stop` function - `stop_all` function ### Changed - `async_mode` parameter
-added to `play` function - Test system modified - `README.md` modified -
-`Python 3.12` added to `linux_test.yml`, `macOS_test.yml` and
-`windows_test.yml` ## [0.2] - 2023-07-10 ### Added - Logo - Anaconda package
-### Changed - `quote` decorator bug fixed - `path_check` decorator bug fixed -
-Test system modified - `README.md` modified ## [0.1] - 2023-06-10 ### Added -
-`README.md` - `__play_win` function - `__play_linux` function - `__play_mac`
-function - `quote` function - `path_check` function - `play` function
-[Unreleased]: https://github.com/openscilab/nava/compare/v0.4...dev [0.4]:
+## [Unreleased] ## [0.5] - 2024-04-03 ### Changed - `loop` parameter added to
+`play` function - `NavaThread` class modified - `README.md` modified ## [0.4] -
+2024-02-19 ### Added - `feature_request.yml` template - `config.yml` for issue
+template ### Changed - Bug report template modified - `NavaThread.stop` method
+bug fixed - Test system modified - `README.md` modified ## [0.3] - 2024-01-31
+### Added - `NavaThread` class - `stop` function - `stop_all` function ###
+Changed - `async_mode` parameter added to `play` function - Test system
+modified - `README.md` modified - `Python 3.12` added to `linux_test.yml`,
+`macOS_test.yml` and `windows_test.yml` ## [0.2] - 2023-07-10 ### Added - Logo
+- Anaconda package ### Changed - `quote` decorator bug fixed - `path_check`
+decorator bug fixed - Test system modified - `README.md` modified ## [0.1] -
+2023-06-10 ### Added - `README.md` - `__play_win` function - `__play_linux`
+function - `__play_mac` function - `quote` function - `path_check` function -
+`play` function [Unreleased]: https://github.com/openscilab/nava/compare/
+v0.5...dev [0.5]: https://github.com/openscilab/nava/compare/v0.4...v0.5 [0.4]:
 https://github.com/openscilab/nava/compare/v0.3...v0.4 [0.3]: https://
 github.com/openscilab/nava/compare/v0.2...v0.3 [0.2]: https://github.com/
 openscilab/nava/compare/v0.1...v0.2 [0.1]: https://github.com/openscilab/nava/
 compare/bd789cc...v0.1
```

### Comparing `nava-0.4/README.md` & `nava-0.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -4,35 +4,25 @@
     <br/>
     <a href="https://www.python.org/">
         <img src="https://img.shields.io/badge/built%20with-Python3-green.svg" alt="built with Python3"/>
     </a>
     <a href="https://badge.fury.io/py/nava">
         <img src="https://badge.fury.io/py/nava.svg" alt="PyPI version" height="18">
     </a>
-	<a href="https://codecov.io/gh/openscilab/nava">
-		<img src="https://codecov.io/gh/openscilab/nava/branch/main/graph/badge.svg" alt="Codecov">
-	</a>
+    <a href="https://anaconda.org/openscilab/nava">
+	<img src="https://anaconda.org/openscilab/nava/badges/version.svg">
+    </a>
+    <a href="https://codecov.io/gh/openscilab/nava">
+        <img src="https://codecov.io/gh/openscilab/nava/branch/main/graph/badge.svg" alt="Codecov">
+    </a>
     <a href="https://discord.gg/MCbPKCFBs3">
         <img src="https://img.shields.io/discord/1064533716615049236.svg" alt="Discord Channel">
     </a>
 </div>
 
-## Table of contents
-   * [Overview](https://github.com/openscilab/nava#overview)
-   * [Installation](https://github.com/openscilab/nava#installation)
-   * [Usage](https://github.com/openscilab/nava#usage)
-   * [Engine](https://github.com/openscilab/nava#engine)
-   * [Issues & Bug Reports](https://github.com/openscilab/nava#issues--bug-reports)
-   * [Contribution](https://github.com/openscilab/nava/blob/main/.github/CONTRIBUTING.md)
-   * [Authors](https://github.com/openscilab/nava/blob/main/AUTHORS.md)
-   * [License](https://github.com/openscilab/nava/blob/main/LICENSE)
-   * [Show Your Support](https://github.com/openscilab/nava#show-your-support)
-   * [Changelog](https://github.com/openscilab/nava/blob/main/CHANGELOG.md)
-   * [Code of Conduct](https://github.com/openscilab/nava/blob/main/.github/CODE_OF_CONDUCT.md)
-
 ## Overview
 
 <p align="justify">
 Nava is a Python library that allows users to play sound in Python without any dependencies or platform restrictions. It is a cross-platform solution that runs on any operating system, including Windows, macOS, and Linux. Its lightweight and easy-to-use design makes Nava an ideal choice for developers looking to add sound functionality to their Python programs.
 </p>
 
 <table>
@@ -89,18 +79,18 @@
 </table>
 
 ## Installation
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)     
-- Run `pip install nava==0.4`
+- Run `pip install nava==0.5`
 
 ### Source code
-- Download [Version 0.4](https://github.com/openscilab/nava/archive/v0.4.zip) or [Latest Source](https://github.com/openscilab/nava/archive/dev.zip)
+- Download [Version 0.5](https://github.com/openscilab/nava/archive/v0.5.zip) or [Latest Source](https://github.com/openscilab/nava/archive/dev.zip)
 - Run `pip install .`
 
 ### Conda
 
 - Check [Conda Managing Package](https://conda.io/)
 - Update Conda using `conda update conda`
 - Run `conda install -c openscilab nava`
@@ -122,14 +112,26 @@
 import time
 from nava import play, stop
 sound_id = play("alarm.wav", async_mode=True)
 time.sleep(4)
 stop(sound_id)
 ```
 
+### Loop mode
+
+⚠️ The `loop` parameter has a default value of `False`
+⚠️ You should always set `async_mode` flag when you are using `loop`
+
+```python
+from nava import play, stop
+sound_id = play("alarm.wav", async_mode=True, loop=True)
+time.sleep(100)
+stop(sound_id)
+```
+
 ### Error
 
 ```python
 from nava import play, NavaBaseError
 
 try:
     play("alarm.wav")
```

#### html2text {}

```diff
@@ -1,22 +1,13 @@
          [https://github.com/openscilab/nava/raw/main/others/logo.png]
                               ************ NNaavvaa ************
 
-         _[_b_u_i_l_t_ _w_i_t_h_ _P_y_t_h_o_n_3_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_C_o_d_e_c_o_v_]_[_D_i_s_c_o_r_d_ _C_h_a_n_n_e_l_]
-## Table of contents * [Overview](https://github.com/openscilab/nava#overview)
-* [Installation](https://github.com/openscilab/nava#installation) * [Usage]
-(https://github.com/openscilab/nava#usage) * [Engine](https://github.com/
-openscilab/nava#engine) * [Issues & Bug Reports](https://github.com/openscilab/
-nava#issues--bug-reports) * [Contribution](https://github.com/openscilab/nava/
-blob/main/.github/CONTRIBUTING.md) * [Authors](https://github.com/openscilab/
-nava/blob/main/AUTHORS.md) * [License](https://github.com/openscilab/nava/blob/
-main/LICENSE) * [Show Your Support](https://github.com/openscilab/nava#show-
-your-support) * [Changelog](https://github.com/openscilab/nava/blob/main/
-CHANGELOG.md) * [Code of Conduct](https://github.com/openscilab/nava/blob/
-main/.github/CODE_OF_CONDUCT.md) ## Overview
+_[_b_u_i_l_t_ _w_i_t_h_ _P_y_t_h_o_n_3_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_h_t_t_p_s_:_/_/_a_n_a_c_o_n_d_a_._o_r_g_/_o_p_e_n_s_c_i_l_a_b_/_n_a_v_a_/_b_a_d_g_e_s_/
+                    _v_e_r_s_i_o_n_._s_v_g_]_[_C_o_d_e_c_o_v_]_[_D_i_s_c_o_r_d_ _C_h_a_n_n_e_l_]
+## Overview
 Nava is a Python library that allows users to play sound in Python without any
 dependencies or platform restrictions. It is a cross-platform solution that
 runs on any operating system, including Windows, macOS, and Linux. Its
 lightweight and easy-to-use design makes Nava an ideal choice for developers
 looking to add sound functionality to their Python programs.
 PyPI Counter               _[_h_t_t_p_:_/_/_p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_n_a_v_a_]
 Github Stars _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_o_p_e_n_s_c_i_l_a_b_/
@@ -34,26 +25,30 @@
  macOS CI      nava/actions/workflows/      actions/workflows/macOS_test.yml/
                    macOS_test.yml/                badge.svg?branch=dev]
                badge.svg?branch=main]
              _[_h_t_t_p_s_:_/_/_a_p_p_._c_o_d_a_c_y_._c_o_m_/_p_r_o_j_e_c_t_/
 Code Quality           _b_a_d_g_e_/_G_r_a_d_e_/            _[_C_o_d_e_F_a_c_t_o_r_] _[_c_o_d_e_b_e_a_t_ _b_a_d_g_e_]
              _9_c_3_8_4_b_4_e_4_0_0_3_4_0_a_e_9_4_7_7_2_c_1_d_7_e_1_8_4_2_d_0_]
 ## Installation ### PyPI - Check [Python Packaging User Guide](https://
-packaging.python.org/installing/) - Run `pip install nava==0.4` ### Source code
-- Download [Version 0.4](https://github.com/openscilab/nava/archive/v0.4.zip)
+packaging.python.org/installing/) - Run `pip install nava==0.5` ### Source code
+- Download [Version 0.5](https://github.com/openscilab/nava/archive/v0.5.zip)
 or [Latest Source](https://github.com/openscilab/nava/archive/dev.zip) - Run
 `pip install .` ### Conda - Check [Conda Managing Package](https://conda.io/) -
 Update Conda using `conda update conda` - Run `conda install -c openscilab
 nava` ## Usage ### Basic ```python from nava import play play("alarm.wav") ```
 ### Async mode â ï¸ The `async_mode` parameter has a default value of `False`
 ```python import time from nava import play, stop sound_id = play("alarm.wav",
-async_mode=True) time.sleep(4) stop(sound_id) ``` ### Error ```python from nava
-import play, NavaBaseError try: play("alarm.wav") except NavaBaseError as e:
-print(str(e)) ``` ## Engine List of different platforms and the corresponding
-engines that are used for sound playing.
+async_mode=True) time.sleep(4) stop(sound_id) ``` ### Loop mode â ï¸ The
+`loop` parameter has a default value of `False` â ï¸ You should always set
+`async_mode` flag when you are using `loop` ```python from nava import play,
+stop sound_id = play("alarm.wav", async_mode=True, loop=True) time.sleep(100)
+stop(sound_id) ``` ### Error ```python from nava import play, NavaBaseError
+try: play("alarm.wav") except NavaBaseError as e: print(str(e)) ``` ## Engine
+List of different platforms and the corresponding engines that are used for
+sound playing.
 PPllaattffoorrmm                     EEnnggiinnee        SSuuppppoorrtteedd FFoorrmmaattss
   Linux  _A_d_v_a_n_c_e_d_ _L_i_n_u_x_ _S_o_u_n_d_ _A_r_c_h_i_t_e_c_t_u_r_e          .wav
 Windows                    _W_i_n_s_o_u_n_d                 .wav
   macOS               _A_u_d_i_o_ _F_i_l_e_ _P_l_a_y            .wav,.mp3
 ## Issues & bug reports Just fill an issue and describe it. We'll check it
 ASAP! or send an email to [info@openscilab.com](mailto:info@openscilab.com
 "info@openscilab.com"). - Please complete the issue template You can also join
```

### Comparing `nava-0.4/nava/functions.py` & `nava-0.5/nava/functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import subprocess
 import os
 import shlex
 from functools import wraps
 from .thread import NavaThread
 from .params import OVERVIEW
 from .params import SOUND_FILE_PLAY_ERROR, SOUND_FILE_EXIST_ERROR
-from .params import SOUND_FILE_PATH_TYPE_ERROR, SOUND_ID_EXIST_ERROR
+from .params import SOUND_FILE_PATH_TYPE_ERROR, SOUND_ID_EXIST_ERROR, LOOP_ASYNC_ERROR
 from .errors import NavaBaseError
 from . import params
 
 
 def stop(sound_id):
     """
     Stop sound.
@@ -78,36 +78,44 @@
         :return: modified function result
         """
         sound_path = shlex.quote(sound_path)
         return func(sound_path, *args, **kwargs)
     return quoter
 
 
-def __play_win(sound_path, async_mode=False):
+def __play_win(sound_path, async_mode=False, loop=False):
     """
     Play sound in Windows.
 
     :param sound_path: sound path
     :type sound_path: str
     :param async_mode: async mode flag
     :type async_mode: bool
+    :param loop: sound loop flag
+    :type loop: bool
     :return: None or sound id
     """
     import winsound
-    play_flags = winsound.SND_FILENAME | (async_mode & winsound.SND_ASYNC)
+    play_flags = \
+        winsound.SND_FILENAME | \
+        (async_mode & winsound.SND_ASYNC)
+    if loop:
+        play_flags = play_flags | winsound.SND_LOOP
 
     if async_mode:
-        sound_thread = NavaThread(target=__play_win_flags,
-                                  args=(sound_path, play_flags), daemon=True)
+        sound_thread = NavaThread(loop,
+                                  target=__play_win_flags,
+                                  args=(sound_path, play_flags),
+                                  daemon=True)
         sound_thread.start()
         sound_id = sound_id_gen()
         params._play_threads_map[sound_id] = sound_thread
         return sound_id
     else:
-        winsound.PlaySound(sound_path, play_flags)
+        __play_win_flags(sound_path, play_flags)
 
 
 def __play_win_flags(sound_path, flags):
     """
     Play sound in Windows using different flags.
 
     :param sound_path: sound path
@@ -117,35 +125,41 @@
     :return: None
     """
     import winsound
     winsound.PlaySound(sound_path, flags)
 
 
 @quote
-def __play_linux(sound_path, async_mode=False):
+def __play_linux(sound_path, async_mode=False, loop=False):
     """
     Play sound in Linux.
 
     :param sound_path: sound path to be played
     :type sound_path: str
     :param async_mode: async mode flag
     :type async_mode: bool
+    :param loop: sound loop flag
+    :type loop: bool
     :return: None or sound id
     """
     if async_mode:
-        sound_thread = NavaThread(target=__play_proc_linux,
+        sound_thread = NavaThread(loop,
+                                  target=__play_proc_linux,
                                   args=(sound_path,),
                                   daemon=True)
         sound_thread.start()
         sound_id = sound_id_gen()
         params._play_threads_map[sound_id] = sound_thread
         return sound_id
     else:
-        proc = __play_proc_linux(sound_path)
-        proc.wait()
+        while True:
+            proc = __play_proc_linux(sound_path)
+            proc.wait()
+            if not loop:
+                break
 
 
 def __play_proc_linux(sound_path):
     """
     Create sound playing process in Linux.
 
     :param sound_path: sound path to be played
@@ -158,35 +172,41 @@
                             stderr=subprocess.PIPE,
                             stdin=subprocess.PIPE,
                             stdout=subprocess.PIPE)
     return proc
 
 
 @quote
-def __play_mac(sound_path, async_mode=False):
+def __play_mac(sound_path, async_mode=False, loop=False):
     """
     Play sound in macOS.
 
     :param sound_path: sound path
     :type sound_path: str
     :param async_mode: async mode flag
     :type async_mode: bool
+    :param loop: sound loop flag
+    :type loop: bool
     :return: None or sound id
     """
     if async_mode:
-        sound_thread = NavaThread(target=__play_proc_mac,
+        sound_thread = NavaThread(loop,
+                                  target=__play_proc_mac,
                                   args=(sound_path,),
                                   daemon=True)
         sound_thread.start()
         sound_id = sound_id_gen()
         params._play_threads_map[sound_id] = sound_thread
         return sound_id
     else:
-        proc = __play_proc_mac(sound_path)
-        proc.wait()
+        while True:
+            proc = __play_proc_mac(sound_path)
+            proc.wait()
+            if not loop:
+                break
 
 
 def __play_proc_mac(sound_path):
     """
     Create sound playing process in macOS.
 
     :param sound_path: sound path to be played
@@ -227,27 +247,31 @@
         if not os.path.isfile(sound_path):
             raise NavaBaseError(SOUND_FILE_EXIST_ERROR)
         return func(sound_path, *args, **kwargs)
     return path_checker
 
 
 @path_check
-def play(sound_path, async_mode=False):
+def play(sound_path, async_mode=False, loop=False):
     """
     Play sound.
 
     :param sound_path: sound path
     :type sound_path: str
     :param async_mode: async mode flag
     :type async_mode: bool
+    :param loop: sound loop flag
+    :type loop: bool
     :return: None or sound id
     """
+    if loop and not async_mode:
+        raise NavaBaseError(LOOP_ASYNC_ERROR)
     try:
         sys_platform = sys.platform
         if sys_platform == "win32":
-            return __play_win(sound_path, async_mode)
+            return __play_win(sound_path, async_mode, loop)
         elif sys_platform == "darwin":
-            return __play_mac(sound_path, async_mode)
+            return __play_mac(sound_path, async_mode, loop)
         else:
-            return __play_linux(sound_path, async_mode)
+            return __play_linux(sound_path, async_mode, loop)
     except Exception:  # pragma: no cover
         raise NavaBaseError(SOUND_FILE_PLAY_ERROR)
```

### Comparing `nava-0.4/nava.egg-info/PKG-INFO` & `nava-0.5/nava.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: nava
-Version: 0.4
+Version: 0.5
 Summary: A Python library for playing sound everywhere natively and securely.
 Home-page: https://github.com/openscilab/nava
-Download-URL: https://github.com/openscilab/nava/tarball/v0.4
+Download-URL: https://github.com/openscilab/nava/tarball/v0.5
 Author: OpenSciLab Development Team
 Author-email: info@openscilab.com
 License: MIT
 Project-URL: Webpage, https://openscilab.com/
 Project-URL: Source, https://github.com/openscilab/nava
 Project-URL: Discord, https://discord.gg/MCbPKCFBs3
 Keywords: sound wav music mp3 player audio
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -43,35 +43,25 @@
     <br/>
     <a href="https://www.python.org/">
         <img src="https://img.shields.io/badge/built%20with-Python3-green.svg" alt="built with Python3"/>
     </a>
     <a href="https://badge.fury.io/py/nava">
         <img src="https://badge.fury.io/py/nava.svg" alt="PyPI version" height="18">
     </a>
-	<a href="https://codecov.io/gh/openscilab/nava">
-		<img src="https://codecov.io/gh/openscilab/nava/branch/main/graph/badge.svg" alt="Codecov">
-	</a>
+    <a href="https://anaconda.org/openscilab/nava">
+	<img src="https://anaconda.org/openscilab/nava/badges/version.svg">
+    </a>
+    <a href="https://codecov.io/gh/openscilab/nava">
+        <img src="https://codecov.io/gh/openscilab/nava/branch/main/graph/badge.svg" alt="Codecov">
+    </a>
     <a href="https://discord.gg/MCbPKCFBs3">
         <img src="https://img.shields.io/discord/1064533716615049236.svg" alt="Discord Channel">
     </a>
 </div>
 
-## Table of contents
-   * [Overview](https://github.com/openscilab/nava#overview)
-   * [Installation](https://github.com/openscilab/nava#installation)
-   * [Usage](https://github.com/openscilab/nava#usage)
-   * [Engine](https://github.com/openscilab/nava#engine)
-   * [Issues & Bug Reports](https://github.com/openscilab/nava#issues--bug-reports)
-   * [Contribution](https://github.com/openscilab/nava/blob/main/.github/CONTRIBUTING.md)
-   * [Authors](https://github.com/openscilab/nava/blob/main/AUTHORS.md)
-   * [License](https://github.com/openscilab/nava/blob/main/LICENSE)
-   * [Show Your Support](https://github.com/openscilab/nava#show-your-support)
-   * [Changelog](https://github.com/openscilab/nava/blob/main/CHANGELOG.md)
-   * [Code of Conduct](https://github.com/openscilab/nava/blob/main/.github/CODE_OF_CONDUCT.md)
-
 ## Overview
 
 <p align="justify">
 Nava is a Python library that allows users to play sound in Python without any dependencies or platform restrictions. It is a cross-platform solution that runs on any operating system, including Windows, macOS, and Linux. Its lightweight and easy-to-use design makes Nava an ideal choice for developers looking to add sound functionality to their Python programs.
 </p>
 
 <table>
@@ -128,18 +118,18 @@
 </table>
 
 ## Installation
 
 ### PyPI
 
 - Check [Python Packaging User Guide](https://packaging.python.org/installing/)     
-- Run `pip install nava==0.4`
+- Run `pip install nava==0.5`
 
 ### Source code
-- Download [Version 0.4](https://github.com/openscilab/nava/archive/v0.4.zip) or [Latest Source](https://github.com/openscilab/nava/archive/dev.zip)
+- Download [Version 0.5](https://github.com/openscilab/nava/archive/v0.5.zip) or [Latest Source](https://github.com/openscilab/nava/archive/dev.zip)
 - Run `pip install .`
 
 ### Conda
 
 - Check [Conda Managing Package](https://conda.io/)
 - Update Conda using `conda update conda`
 - Run `conda install -c openscilab nava`
@@ -161,14 +151,26 @@
 import time
 from nava import play, stop
 sound_id = play("alarm.wav", async_mode=True)
 time.sleep(4)
 stop(sound_id)
 ```
 
+### Loop mode
+
+⚠️ The `loop` parameter has a default value of `False`
+⚠️ You should always set `async_mode` flag when you are using `loop`
+
+```python
+from nava import play, stop
+sound_id = play("alarm.wav", async_mode=True, loop=True)
+time.sleep(100)
+stop(sound_id)
+```
+
 ### Error
 
 ```python
 from nava import play, NavaBaseError
 
 try:
     play("alarm.wav")
@@ -231,14 +233,19 @@
 # Changelog
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/)
 and this project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
+## [0.5] - 2024-04-03
+### Changed
+- `loop` parameter added to `play` function
+- `NavaThread` class modified
+- `README.md` modified
 ## [0.4] - 2024-02-19
 ### Added
 - `feature_request.yml` template
 - `config.yml` for issue template
 ### Changed
 - Bug report template modified
 - `NavaThread.stop` method bug fixed
@@ -270,12 +277,13 @@
 - `__play_linux` function
 - `__play_mac` function
 - `quote` function
 - `path_check` function
 - `play` function
 
 
-[Unreleased]: https://github.com/openscilab/nava/compare/v0.4...dev
+[Unreleased]: https://github.com/openscilab/nava/compare/v0.5...dev
+[0.5]: https://github.com/openscilab/nava/compare/v0.4...v0.5
 [0.4]: https://github.com/openscilab/nava/compare/v0.3...v0.4
 [0.3]: https://github.com/openscilab/nava/compare/v0.2...v0.3
 [0.2]: https://github.com/openscilab/nava/compare/v0.1...v0.2
 [0.1]: https://github.com/openscilab/nava/compare/bd789cc...v0.1
```

#### html2text {}

```diff
@@ -1,43 +1,34 @@
-Metadata-Version: 2.1 Name: nava Version: 0.4 Summary: A Python library for
+Metadata-Version: 2.1 Name: nava Version: 0.5 Summary: A Python library for
 playing sound everywhere natively and securely. Home-page: https://github.com/
-openscilab/nava Download-URL: https://github.com/openscilab/nava/tarball/v0.4
+openscilab/nava Download-URL: https://github.com/openscilab/nava/tarball/v0.5
 Author: OpenSciLab Development Team Author-email: info@openscilab.com License:
 MIT Project-URL: Webpage, https://openscilab.com/ Project-URL: Source, https://
 github.com/openscilab/nava Project-URL: Discord, https://discord.gg/MCbPKCFBs3
-Keywords: sound wav music mp3 player audio Classifier: Development Status :: 3
-- Alpha Classifier: Intended Audience :: Developers Classifier: Natural
-Language :: English Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Classifier: Programming Language
-:: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
+Keywords: sound wav music mp3 player audio Classifier: Development Status :: 4
+- Beta Classifier: Intended Audience :: Developers Classifier: Natural Language
+:: English Classifier: License :: OSI Approved :: MIT License Classifier:
+Operating System :: OS Independent Classifier: Programming Language :: Python
+:: 3.6 Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Classifier: Intended Audience :: Developers Classifier: Intended
 Audience :: End Users/Desktop Classifier: Intended Audience :: Manufacturing
 Classifier: Topic :: Multimedia Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Sound/Audio :: Players Classifier: Topic ::
 Multimedia :: Sound/Audio :: Players :: MP3 Requires-Python: >=3.6 Description-
 Content-Type: text/markdown License-File: LICENSE License-File: AUTHORS.md
 Requires-Dist: art>=1.8
          [https://github.com/openscilab/nava/raw/main/others/logo.png]
                               ************ NNaavvaa ************
 
-         _[_b_u_i_l_t_ _w_i_t_h_ _P_y_t_h_o_n_3_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_C_o_d_e_c_o_v_]_[_D_i_s_c_o_r_d_ _C_h_a_n_n_e_l_]
-## Table of contents * [Overview](https://github.com/openscilab/nava#overview)
-* [Installation](https://github.com/openscilab/nava#installation) * [Usage]
-(https://github.com/openscilab/nava#usage) * [Engine](https://github.com/
-openscilab/nava#engine) * [Issues & Bug Reports](https://github.com/openscilab/
-nava#issues--bug-reports) * [Contribution](https://github.com/openscilab/nava/
-blob/main/.github/CONTRIBUTING.md) * [Authors](https://github.com/openscilab/
-nava/blob/main/AUTHORS.md) * [License](https://github.com/openscilab/nava/blob/
-main/LICENSE) * [Show Your Support](https://github.com/openscilab/nava#show-
-your-support) * [Changelog](https://github.com/openscilab/nava/blob/main/
-CHANGELOG.md) * [Code of Conduct](https://github.com/openscilab/nava/blob/
-main/.github/CODE_OF_CONDUCT.md) ## Overview
+_[_b_u_i_l_t_ _w_i_t_h_ _P_y_t_h_o_n_3_]_[_P_y_P_I_ _v_e_r_s_i_o_n_]_[_h_t_t_p_s_:_/_/_a_n_a_c_o_n_d_a_._o_r_g_/_o_p_e_n_s_c_i_l_a_b_/_n_a_v_a_/_b_a_d_g_e_s_/
+                    _v_e_r_s_i_o_n_._s_v_g_]_[_C_o_d_e_c_o_v_]_[_D_i_s_c_o_r_d_ _C_h_a_n_n_e_l_]
+## Overview
 Nava is a Python library that allows users to play sound in Python without any
 dependencies or platform restrictions. It is a cross-platform solution that
 runs on any operating system, including Windows, macOS, and Linux. Its
 lightweight and easy-to-use design makes Nava an ideal choice for developers
 looking to add sound functionality to their Python programs.
 PyPI Counter               _[_h_t_t_p_:_/_/_p_e_p_y_._t_e_c_h_/_b_a_d_g_e_/_n_a_v_a_]
 Github Stars _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_s_t_a_r_s_/_o_p_e_n_s_c_i_l_a_b_/
@@ -55,26 +46,30 @@
  macOS CI      nava/actions/workflows/      actions/workflows/macOS_test.yml/
                    macOS_test.yml/                badge.svg?branch=dev]
                badge.svg?branch=main]
              _[_h_t_t_p_s_:_/_/_a_p_p_._c_o_d_a_c_y_._c_o_m_/_p_r_o_j_e_c_t_/
 Code Quality           _b_a_d_g_e_/_G_r_a_d_e_/            _[_C_o_d_e_F_a_c_t_o_r_] _[_c_o_d_e_b_e_a_t_ _b_a_d_g_e_]
              _9_c_3_8_4_b_4_e_4_0_0_3_4_0_a_e_9_4_7_7_2_c_1_d_7_e_1_8_4_2_d_0_]
 ## Installation ### PyPI - Check [Python Packaging User Guide](https://
-packaging.python.org/installing/) - Run `pip install nava==0.4` ### Source code
-- Download [Version 0.4](https://github.com/openscilab/nava/archive/v0.4.zip)
+packaging.python.org/installing/) - Run `pip install nava==0.5` ### Source code
+- Download [Version 0.5](https://github.com/openscilab/nava/archive/v0.5.zip)
 or [Latest Source](https://github.com/openscilab/nava/archive/dev.zip) - Run
 `pip install .` ### Conda - Check [Conda Managing Package](https://conda.io/) -
 Update Conda using `conda update conda` - Run `conda install -c openscilab
 nava` ## Usage ### Basic ```python from nava import play play("alarm.wav") ```
 ### Async mode â ï¸ The `async_mode` parameter has a default value of `False`
 ```python import time from nava import play, stop sound_id = play("alarm.wav",
-async_mode=True) time.sleep(4) stop(sound_id) ``` ### Error ```python from nava
-import play, NavaBaseError try: play("alarm.wav") except NavaBaseError as e:
-print(str(e)) ``` ## Engine List of different platforms and the corresponding
-engines that are used for sound playing.
+async_mode=True) time.sleep(4) stop(sound_id) ``` ### Loop mode â ï¸ The
+`loop` parameter has a default value of `False` â ï¸ You should always set
+`async_mode` flag when you are using `loop` ```python from nava import play,
+stop sound_id = play("alarm.wav", async_mode=True, loop=True) time.sleep(100)
+stop(sound_id) ``` ### Error ```python from nava import play, NavaBaseError
+try: play("alarm.wav") except NavaBaseError as e: print(str(e)) ``` ## Engine
+List of different platforms and the corresponding engines that are used for
+sound playing.
 PPllaattffoorrmm                     EEnnggiinnee        SSuuppppoorrtteedd FFoorrmmaattss
   Linux  _A_d_v_a_n_c_e_d_ _L_i_n_u_x_ _S_o_u_n_d_ _A_r_c_h_i_t_e_c_t_u_r_e          .wav
 Windows                    _W_i_n_s_o_u_n_d                 .wav
   macOS               _A_u_d_i_o_ _F_i_l_e_ _P_l_a_y            .wav,.mp3
 ## Issues & bug reports Just fill an issue and describe it. We'll check it
 ASAP! or send an email to [info@openscilab.com](mailto:info@openscilab.com
 "info@openscilab.com"). - Please complete the issue template You can also join
@@ -84,24 +79,26 @@
 ******** DDoonnaattee ttoo oouurr pprroojjeecctt ********
 If you do like our project and we hope that you do, can you please support us?
 Our project is not and is never going to be working for profit. We need the
 money just so we can continue doing what we do ;-) . _[_N_a_v_a_ _D_o_n_a_t_i_o_n_]# Changelog
 All notable changes to this project will be documented in this file. The format
 is based on [Keep a Changelog](http://keepachangelog.com/en/1.0.0/) and this
 project adheres to [Semantic Versioning](http://semver.org/spec/v2.0.0.html).
-## [Unreleased] ## [0.4] - 2024-02-19 ### Added - `feature_request.yml`
-template - `config.yml` for issue template ### Changed - Bug report template
-modified - `NavaThread.stop` method bug fixed - Test system modified -
-`README.md` modified ## [0.3] - 2024-01-31 ### Added - `NavaThread` class -
-`stop` function - `stop_all` function ### Changed - `async_mode` parameter
-added to `play` function - Test system modified - `README.md` modified -
-`Python 3.12` added to `linux_test.yml`, `macOS_test.yml` and
-`windows_test.yml` ## [0.2] - 2023-07-10 ### Added - Logo - Anaconda package
-### Changed - `quote` decorator bug fixed - `path_check` decorator bug fixed -
-Test system modified - `README.md` modified ## [0.1] - 2023-06-10 ### Added -
-`README.md` - `__play_win` function - `__play_linux` function - `__play_mac`
-function - `quote` function - `path_check` function - `play` function
-[Unreleased]: https://github.com/openscilab/nava/compare/v0.4...dev [0.4]:
+## [Unreleased] ## [0.5] - 2024-04-03 ### Changed - `loop` parameter added to
+`play` function - `NavaThread` class modified - `README.md` modified ## [0.4] -
+2024-02-19 ### Added - `feature_request.yml` template - `config.yml` for issue
+template ### Changed - Bug report template modified - `NavaThread.stop` method
+bug fixed - Test system modified - `README.md` modified ## [0.3] - 2024-01-31
+### Added - `NavaThread` class - `stop` function - `stop_all` function ###
+Changed - `async_mode` parameter added to `play` function - Test system
+modified - `README.md` modified - `Python 3.12` added to `linux_test.yml`,
+`macOS_test.yml` and `windows_test.yml` ## [0.2] - 2023-07-10 ### Added - Logo
+- Anaconda package ### Changed - `quote` decorator bug fixed - `path_check`
+decorator bug fixed - Test system modified - `README.md` modified ## [0.1] -
+2023-06-10 ### Added - `README.md` - `__play_win` function - `__play_linux`
+function - `__play_mac` function - `quote` function - `path_check` function -
+`play` function [Unreleased]: https://github.com/openscilab/nava/compare/
+v0.5...dev [0.5]: https://github.com/openscilab/nava/compare/v0.4...v0.5 [0.4]:
 https://github.com/openscilab/nava/compare/v0.3...v0.4 [0.3]: https://
 github.com/openscilab/nava/compare/v0.2...v0.3 [0.2]: https://github.com/
 openscilab/nava/compare/v0.1...v0.2 [0.1]: https://github.com/openscilab/nava/
 compare/bd789cc...v0.1
```

### Comparing `nava-0.4/setup.py` & `nava-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,32 +28,32 @@
    It is a cross-platform solution that runs on any operating system, including Windows, macOS, and Linux.
    Its lightweight and easy-to-use design makes Nava an ideal choice for developers looking to add sound functionality to their Python programs.'''
 
 
 setup(
     name='nava',
     packages=['nava'],
-    version='0.4',
+    version='0.5',
     description='A Python library for playing sound everywhere natively and securely.',
     long_description=read_description(),
     long_description_content_type='text/markdown',
     author='OpenSciLab Development Team',
     author_email='info@openscilab.com',
     url='https://github.com/openscilab/nava',
-    download_url='https://github.com/openscilab/nava/tarball/v0.4',
+    download_url='https://github.com/openscilab/nava/tarball/v0.5',
     keywords="sound wav music mp3 player audio",
     project_urls={
         'Webpage': 'https://openscilab.com/',
         'Source': 'https://github.com/openscilab/nava',
         'Discord': 'https://discord.gg/MCbPKCFBs3',
     },
     install_requires=get_requires(),
     python_requires='>=3.6',
     classifiers=[
-        'Development Status :: 3 - Alpha',
+        'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Natural Language :: English',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
```

