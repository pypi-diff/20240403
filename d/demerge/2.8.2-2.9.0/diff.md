# Comparing `tmp/demerge-2.8.2.tar.gz` & `tmp/demerge-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "demerge-2.8.2.tar", max compression
+gzip compressed data, was "demerge-2.9.0.tar", max compression
```

## Comparing `demerge-2.8.2.tar` & `demerge-2.9.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1074 2023-11-24 00:25:54.187724 demerge-2.8.2/LICENSE
--rw-r--r--   0        0        0    15094 2023-11-24 00:25:54.187724 demerge-2.8.2/README.md
--rw-r--r--   0        0        0      627 2023-11-24 00:25:54.187724 demerge-2.8.2/demerge/__init__.py
--rw-r--r--   0        0        0     2797 2023-11-24 00:25:54.187724 demerge-2.8.2/demerge/calc_resonance_params.py
--rwxr-xr-x   0        0        0  3059932 2023-11-24 00:25:54.203724 demerge-2.8.2/demerge/ddb_20231029.fits.gz
--rw-r--r--   0        0        0    39330 2023-11-24 00:25:54.203724 demerge-2.8.2/demerge/demerge.py
--rw-r--r--   0        0        0     1887 2023-11-24 00:25:54.203724 demerge-2.8.2/demerge/make_divided_data.py
--rw-r--r--   0        0        0    10327 2023-11-24 00:25:54.203724 demerge-2.8.2/demerge/make_reduced_fits.py
--rw-r--r--   0        0        0    10295 2023-11-24 00:25:54.203724 demerge-2.8.2/demerge/merge_function.py
--rw-r--r--   0        0        0    20864 2023-11-24 00:25:54.203724 demerge-2.8.2/demerge/merge_to_dems.py
--rw-r--r--   0        0        0     9655 2023-11-24 00:25:54.203724 demerge-2.8.2/demerge/plot.py
--rwxr-xr-x   0        0        0     6945 2023-11-24 00:25:54.203724 demerge-2.8.2/demerge/run.sh
--rw-r--r--   0        0        0     1173 2023-11-24 00:25:54.203724 demerge-2.8.2/pyproject.toml
--rw-r--r--   0        0        0    16117 1970-01-01 00:00:00.000000 demerge-2.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-11-24 02:31:15.098690 demerge-2.9.0/LICENSE
+-rw-r--r--   0        0        0    15094 2023-11-24 02:31:15.098690 demerge-2.9.0/README.md
+-rw-r--r--   0        0        0      627 2023-11-24 02:31:15.098690 demerge-2.9.0/demerge/__init__.py
+-rw-r--r--   0        0        0     2797 2023-11-24 02:31:15.098690 demerge-2.9.0/demerge/calc_resonance_params.py
+-rw-r--r--   0        0        0  9910516 2023-11-24 02:31:15.138690 demerge-2.9.0/demerge/ddb_20231123.fits.gz
+-rw-r--r--   0        0        0    39330 2023-11-24 02:31:15.138690 demerge-2.9.0/demerge/demerge.py
+-rw-r--r--   0        0        0     1887 2023-11-24 02:31:15.138690 demerge-2.9.0/demerge/make_divided_data.py
+-rw-r--r--   0        0        0    10327 2023-11-24 02:31:15.138690 demerge-2.9.0/demerge/make_reduced_fits.py
+-rw-r--r--   0        0        0    10295 2023-11-24 02:31:15.138690 demerge-2.9.0/demerge/merge_function.py
+-rw-r--r--   0        0        0    20864 2023-11-24 02:31:15.138690 demerge-2.9.0/demerge/merge_to_dems.py
+-rw-r--r--   0        0        0     9655 2023-11-24 02:31:15.138690 demerge-2.9.0/demerge/plot.py
+-rwxr-xr-x   0        0        0     6945 2023-11-24 02:31:15.138690 demerge-2.9.0/demerge/run.sh
+-rw-r--r--   0        0        0     1173 2023-11-24 02:31:15.138690 demerge-2.9.0/pyproject.toml
+-rw-r--r--   0        0        0    16117 1970-01-01 00:00:00.000000 demerge-2.9.0/PKG-INFO
```

### Comparing `demerge-2.8.2/LICENSE` & `demerge-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `demerge-2.8.2/README.md` & `demerge-2.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -9,40 +9,40 @@
 DESHIMA merge code for observed datasets
 
 MergeToDfits()クラスの代わりとなるmerge_to_dems()関数を実装し、DEMSオブジェクトを生成できるようにしました。今回の更新では、付属のPythonパッケージ`demerge`をPython環境にインストールすることで、同名のコマンド`demerge`が利用可能となります（`demerge/run.sh`のラッパースクリプトです）。これを実行するとmerge_to_dems()関数が実行され、解析結果がまとまったZarrファイルが生成されます。DEMSの構造については[deshima-dev/dems](https://github.com/deshima-dev/dems)をご覧ください。
 
 ## 動作環境
 
 - CPython: 3.9-3.12
-- Dependent packages: [pyproject.toml](https://github.com/deshima-dev/demerge/blob/v2.8.2/pyproject.toml)をご確認ください
+- Dependent packages: [pyproject.toml](https://github.com/deshima-dev/demerge/blob/v2.9.0/pyproject.toml)をご確認ください
 
 ## インストール
 
 ### 一般ユーザ
 
 pipで[PyPI](https://pypi.org)からインストールしてください。
 
 ```shell
-pip install demerge==2.8.2
+pip install demerge==2.9.0
 ```
 
 インストール後、`demerge`コマンドが利用可能になります。
 
 ### 開発者
 
 以下のコマンドで実行環境にダウンロード（クローン）してください。
 
 ```shell
 # テストデータを含める場合
 git clone --recursive https://github.com/deshima-dev/demerge.git
-cd demerge && git checkout v2.8.2
+cd demerge && git checkout v2.9.0
 
 # 最小構成でダウンロードする場合
 git clone --depth=1 https://github.com/deshima-dev/demerge.git
-cd demerge && git checkout v2.8.2
+cd demerge && git checkout v2.9.0
 ```
 
 続けて、`demerge`パッケージのPython環境へのインストールを行います。
 
 ```shell
 cd /path/to/demerge
 
@@ -80,15 +80,15 @@
 以下の引数を指定すると、データの取得ディレクトリや保存先などを変更することができます。
 
 引数 | 説明 | デフォルト
 --- | --- | ---
 `-d` | 観測データディレクトリの指定 | `data`
 `-c` | キャッシュディレクトリを指定 | `cache`
 `-g` | グラフディレクトリを指定 | `graph`
-`-b` | DDBファイルを指定 | `dmerge/ddb_20231029.fits.gz`（パッケージに同梱）
+`-b` | DDBファイルを指定 | `dmerge/ddb_20231123.fits.gz`（パッケージに同梱）
 `-o` | 出力データディレクトリを指定 | `cache`
 `-m` | マージオプションを指定（例：`-m "--coordinate radec"`） | なし
 
 ### 観測データの保存先の構造
 
 ```
 data
```

### Comparing `demerge-2.8.2/demerge/__init__.py` & `demerge-2.9.0/demerge/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "demerge",
     "make_divided_data",
     "make_reduced_fits",
     "merge_function",
     "merge_to_dems",
     "plot",
 ]
-__version__ = "2.8.2"
+__version__ = "2.9.0"
 
 
 # submodules
 from . import calc_resonance_params
 from . import demerge
 from . import make_divided_data
 from . import make_reduced_fits
```

### Comparing `demerge-2.8.2/demerge/calc_resonance_params.py` & `demerge-2.9.0/demerge/calc_resonance_params.py`

 * *Files identical despite different names*

### Comparing `demerge-2.8.2/demerge/demerge.py` & `demerge-2.9.0/demerge/demerge.py`

 * *Files identical despite different names*

### Comparing `demerge-2.8.2/demerge/make_divided_data.py` & `demerge-2.9.0/demerge/make_divided_data.py`

 * *Files identical despite different names*

### Comparing `demerge-2.8.2/demerge/make_reduced_fits.py` & `demerge-2.9.0/demerge/make_reduced_fits.py`

 * *Files identical despite different names*

### Comparing `demerge-2.8.2/demerge/merge_function.py` & `demerge-2.9.0/demerge/merge_function.py`

 * *Files identical despite different names*

### Comparing `demerge-2.8.2/demerge/merge_to_dems.py` & `demerge-2.9.0/demerge/merge_to_dems.py`

 * *Files identical despite different names*

### Comparing `demerge-2.8.2/demerge/plot.py` & `demerge-2.9.0/demerge/plot.py`

 * *Files identical despite different names*

### Comparing `demerge-2.8.2/demerge/run.sh` & `demerge-2.9.0/demerge/run.sh`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 #  -b DDBファイルの指定
 #  -o 出力データディレクトリの指定
 #  -m マージオプションの指定
 #  -p プロット実行オプションの指定
 #
 
 DEMERGE="$(cd "$(dirname "${BASH_SOURCE:-$0}")" && pwd)"
-DEFAULT_DDB="${DEMERGE}/ddb_20231029.fits.gz"
+DEFAULT_DDB="${DEMERGE}/ddb_20231123.fits.gz"
 NCPU=`python -c "import multiprocessing as m; print(m.cpu_count() - 1);"`
 
 # ==================
 # 指定可能オプション
 # ==================
 #  -c キャッシュディレクトリを指定
 #  -g グラフディレクトリを指定
```

### Comparing `demerge-2.8.2/pyproject.toml` & `demerge-2.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "demerge"
-version = "2.8.2"
+version = "2.9.0"
 description = "DESHIMA merge code for observed datasets"
 authors = [
     "Tatsuya Takekoshi <tatsuya.takekoshi@gmail.com>",
     "Daisuke Naito <naito@naitosystems.com>",
     "Akio Taniguchi <taniguchi@a.phys.nagoya-u.ac.jp>",
 ]
 keywords = [
```

### Comparing `demerge-2.8.2/PKG-INFO` & `demerge-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: demerge
-Version: 2.8.2
+Version: 2.9.0
 Summary: DESHIMA merge code for observed datasets
 Home-page: https://github.com/deshima-dev/demerge/
 License: MIT
 Keywords: astronomy,radio-astronomy,submillimeter,spectroscopy,deshima
 Author: Tatsuya Takekoshi
 Author-email: tatsuya.takekoshi@gmail.com
 Requires-Python: >=3.9,<3.13
@@ -36,40 +36,40 @@
 DESHIMA merge code for observed datasets
 
 MergeToDfits()クラスの代わりとなるmerge_to_dems()関数を実装し、DEMSオブジェクトを生成できるようにしました。今回の更新では、付属のPythonパッケージ`demerge`をPython環境にインストールすることで、同名のコマンド`demerge`が利用可能となります（`demerge/run.sh`のラッパースクリプトです）。これを実行するとmerge_to_dems()関数が実行され、解析結果がまとまったZarrファイルが生成されます。DEMSの構造については[deshima-dev/dems](https://github.com/deshima-dev/dems)をご覧ください。
 
 ## 動作環境
 
 - CPython: 3.9-3.12
-- Dependent packages: [pyproject.toml](https://github.com/deshima-dev/demerge/blob/v2.8.2/pyproject.toml)をご確認ください
+- Dependent packages: [pyproject.toml](https://github.com/deshima-dev/demerge/blob/v2.9.0/pyproject.toml)をご確認ください
 
 ## インストール
 
 ### 一般ユーザ
 
 pipで[PyPI](https://pypi.org)からインストールしてください。
 
 ```shell
-pip install demerge==2.8.2
+pip install demerge==2.9.0
 ```
 
 インストール後、`demerge`コマンドが利用可能になります。
 
 ### 開発者
 
 以下のコマンドで実行環境にダウンロード（クローン）してください。
 
 ```shell
 # テストデータを含める場合
 git clone --recursive https://github.com/deshima-dev/demerge.git
-cd demerge && git checkout v2.8.2
+cd demerge && git checkout v2.9.0
 
 # 最小構成でダウンロードする場合
 git clone --depth=1 https://github.com/deshima-dev/demerge.git
-cd demerge && git checkout v2.8.2
+cd demerge && git checkout v2.9.0
 ```
 
 続けて、`demerge`パッケージのPython環境へのインストールを行います。
 
 ```shell
 cd /path/to/demerge
 
@@ -107,15 +107,15 @@
 以下の引数を指定すると、データの取得ディレクトリや保存先などを変更することができます。
 
 引数 | 説明 | デフォルト
 --- | --- | ---
 `-d` | 観測データディレクトリの指定 | `data`
 `-c` | キャッシュディレクトリを指定 | `cache`
 `-g` | グラフディレクトリを指定 | `graph`
-`-b` | DDBファイルを指定 | `dmerge/ddb_20231029.fits.gz`（パッケージに同梱）
+`-b` | DDBファイルを指定 | `dmerge/ddb_20231123.fits.gz`（パッケージに同梱）
 `-o` | 出力データディレクトリを指定 | `cache`
 `-m` | マージオプションを指定（例：`-m "--coordinate radec"`） | なし
 
 ### 観測データの保存先の構造
 
 ```
 data
```

