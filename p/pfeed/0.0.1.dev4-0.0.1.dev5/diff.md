# Comparing `tmp/pfeed-0.0.1.dev4.tar.gz` & `tmp/pfeed-0.0.1.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfeed-0.0.1.dev4.tar", max compression
+gzip compressed data, was "pfeed-0.0.1.dev5.tar", max compression
```

## Comparing `pfeed-0.0.1.dev4.tar` & `pfeed-0.0.1.dev5.tar`

### file list

```diff
@@ -1,33 +1,37 @@
--rw-r--r--   0        0        0    11355 2024-02-06 15:06:07.719273 pfeed-0.0.1.dev4/LICENSE
--rw-r--r--   0        0        0     6097 2024-02-14 14:15:57.739759 pfeed-0.0.1.dev4/README.md
--rw-r--r--   0        0        0      304 2024-02-05 08:05:18.720787 pfeed-0.0.1.dev4/pfeed/__init__.py
--rw-r--r--   0        0        0       66 2024-02-05 13:31:08.419626 pfeed-0.0.1.dev4/pfeed/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-02-05 06:26:40.936701 pfeed-0.0.1.dev4/pfeed/cli/commands/__init__.py
--rw-r--r--   0        0        0     2788 2024-02-14 07:44:31.786343 pfeed-0.0.1.dev4/pfeed/cli/commands/config.py
--rw-r--r--   0        0        0     1630 2024-02-14 07:49:34.075745 pfeed-0.0.1.dev4/pfeed/cli/commands/docker_compose.py
--rw-r--r--   0        0        0     2644 2024-02-14 06:32:45.693081 pfeed-0.0.1.dev4/pfeed/cli/commands/download.py
--rw-r--r--   0        0        0        0 2024-02-05 13:19:50.128762 pfeed-0.0.1.dev4/pfeed/cli/commands/stream.py
--rw-r--r--   0        0        0      646 2024-02-14 07:35:50.460026 pfeed-0.0.1.dev4/pfeed/cli/main.py
--rw-r--r--   0        0        0     1707 2024-02-14 09:35:20.041272 pfeed-0.0.1.dev4/pfeed/config/logging.yml
--rw-r--r--   0        0        0     2248 2024-02-14 07:35:30.269091 pfeed-0.0.1.dev4/pfeed/config_handler.py
--rw-r--r--   0        0        0      210 2024-02-06 07:58:44.150126 pfeed-0.0.1.dev4/pfeed/const/commons.py
--rw-r--r--   0        0        0      529 2024-02-05 14:51:47.591199 pfeed-0.0.1.dev4/pfeed/const/paths.py
--rw-r--r--   0        0        0     4844 2024-02-12 09:18:11.375052 pfeed-0.0.1.dev4/pfeed/datastore.py
--rw-r--r--   0        0        0      104 2024-01-30 15:20:33.101612 pfeed-0.0.1.dev4/pfeed/feeds/__init__.py
--rw-r--r--   0        0        0      547 2024-02-14 09:56:55.268792 pfeed-0.0.1.dev4/pfeed/feeds/base_feed.py
--rw-r--r--   0        0        0     3806 2024-02-14 09:10:34.697854 pfeed-0.0.1.dev4/pfeed/feeds/bybit_feed.py
--rw-r--r--   0        0        0      281 2024-01-30 15:20:33.109541 pfeed-0.0.1.dev4/pfeed/feeds/custom_csv_feed.py
--rw-r--r--   0        0        0     3423 2024-02-14 09:08:41.350701 pfeed-0.0.1.dev4/pfeed/feeds/yahoo_finance_feed.py
--rw-r--r--   0        0        0     2149 2024-02-08 07:41:10.026656 pfeed-0.0.1.dev4/pfeed/filepath.py
--rw-r--r--   0        0        0      159 2024-02-05 14:16:07.092251 pfeed-0.0.1.dev4/pfeed/main.py
--rw-r--r--   0        0        0       32 2024-01-30 15:20:33.113060 pfeed-0.0.1.dev4/pfeed/sources/__init__.py
--rw-r--r--   0        0        0      331 2024-02-09 07:53:41.280756 pfeed-0.0.1.dev4/pfeed/sources/bybit/__init__.py
--rw-r--r--   0        0        0     2111 2024-01-30 15:20:33.116592 pfeed-0.0.1.dev4/pfeed/sources/bybit/api.py
--rw-r--r--   0        0        0     1385 2024-02-08 05:19:46.486217 pfeed-0.0.1.dev4/pfeed/sources/bybit/const.py
--rw-r--r--   0        0        0     6998 2024-02-14 09:02:02.787789 pfeed-0.0.1.dev4/pfeed/sources/bybit/download.py
--rw-r--r--   0        0        0     5927 2024-02-14 09:59:46.520385 pfeed-0.0.1.dev4/pfeed/sources/bybit/etl.py
--rw-r--r--   0        0        0      103 2024-02-06 10:42:07.356942 pfeed-0.0.1.dev4/pfeed/sources/bybit/stream.py
--rw-r--r--   0        0        0     3221 2024-02-12 09:31:27.417239 pfeed-0.0.1.dev4/pfeed/utils/utils.py
--rw-r--r--   0        0        0     1610 2024-02-06 09:42:43.428966 pfeed-0.0.1.dev4/pfeed/utils/validate.py
--rw-r--r--   0        0        0     1377 2024-02-14 14:17:02.208269 pfeed-0.0.1.dev4/pyproject.toml
--rw-r--r--   0        0        0     7488 1970-01-01 00:00:00.000000 pfeed-0.0.1.dev4/PKG-INFO
+-rw-r--r--   0        0        0    11355 2024-02-06 15:06:07.719273 pfeed-0.0.1.dev5/LICENSE
+-rw-r--r--   0        0        0    11225 2024-04-02 17:30:09.523671 pfeed-0.0.1.dev5/README.md
+-rw-r--r--   0        0        0      326 2024-03-21 17:02:33.426143 pfeed-0.0.1.dev5/pfeed/__init__.py
+-rw-r--r--   0        0        0       66 2024-02-05 13:31:08.419626 pfeed-0.0.1.dev5/pfeed/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-05 06:26:40.936701 pfeed-0.0.1.dev5/pfeed/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2939 2024-03-15 11:20:38.762756 pfeed-0.0.1.dev5/pfeed/cli/commands/config.py
+-rw-r--r--   0        0        0     1486 2024-03-14 15:50:37.098725 pfeed-0.0.1.dev5/pfeed/cli/commands/docker_compose.py
+-rw-r--r--   0        0        0     3158 2024-04-02 17:39:01.214981 pfeed-0.0.1.dev5/pfeed/cli/commands/download.py
+-rw-r--r--   0        0        0        0 2024-02-05 13:19:50.128762 pfeed-0.0.1.dev5/pfeed/cli/commands/stream.py
+-rw-r--r--   0        0        0      646 2024-02-14 07:35:50.460026 pfeed-0.0.1.dev5/pfeed/cli/main.py
+-rw-r--r--   0        0        0     1707 2024-03-29 05:54:20.034871 pfeed-0.0.1.dev5/pfeed/config/logging.yml
+-rw-r--r--   0        0        0     2248 2024-02-14 07:35:30.269091 pfeed-0.0.1.dev5/pfeed/config_handler.py
+-rw-r--r--   0        0        0      441 2024-03-19 12:53:31.753710 pfeed-0.0.1.dev5/pfeed/const/commons.py
+-rw-r--r--   0        0        0      529 2024-03-14 15:44:43.813400 pfeed-0.0.1.dev5/pfeed/const/paths.py
+-rw-r--r--   0        0        0     4918 2024-03-21 17:00:48.770498 pfeed-0.0.1.dev5/pfeed/data_tools/data_tool_pandas.py
+-rw-r--r--   0        0        0     3817 2024-03-21 17:01:02.837107 pfeed-0.0.1.dev5/pfeed/data_tools/data_tool_polars.py
+-rw-r--r--   0        0        0       79 2024-03-19 16:55:54.124645 pfeed-0.0.1.dev5/pfeed/data_tools/data_tool_pyspark.py
+-rw-r--r--   0        0        0     4340 2024-04-02 06:47:39.157808 pfeed-0.0.1.dev5/pfeed/datastore.py
+-rw-r--r--   0        0        0     9131 2024-04-02 08:03:20.745776 pfeed-0.0.1.dev5/pfeed/etl.py
+-rw-r--r--   0        0        0      104 2024-01-30 15:20:33.101612 pfeed-0.0.1.dev5/pfeed/feeds/__init__.py
+-rw-r--r--   0        0        0     1850 2024-04-02 14:17:52.023481 pfeed-0.0.1.dev5/pfeed/feeds/base_feed.py
+-rw-r--r--   0        0        0     8836 2024-04-02 17:45:30.611913 pfeed-0.0.1.dev5/pfeed/feeds/bybit_feed.py
+-rw-r--r--   0        0        0      281 2024-01-30 15:20:33.109541 pfeed-0.0.1.dev5/pfeed/feeds/custom_csv_feed.py
+-rw-r--r--   0        0        0     3964 2024-03-29 09:42:51.709699 pfeed-0.0.1.dev5/pfeed/feeds/yahoo_finance_feed.py
+-rw-r--r--   0        0        0     2208 2024-03-29 06:50:06.585159 pfeed-0.0.1.dev5/pfeed/filepath.py
+-rw-r--r--   0        0        0      159 2024-02-05 14:16:07.092251 pfeed-0.0.1.dev5/pfeed/main.py
+-rw-r--r--   0        0        0       32 2024-01-30 15:20:33.113060 pfeed-0.0.1.dev5/pfeed/sources/__init__.py
+-rw-r--r--   0        0        0      364 2024-04-02 17:44:35.831803 pfeed-0.0.1.dev5/pfeed/sources/bybit/__init__.py
+-rw-r--r--   0        0        0     2414 2024-03-28 14:14:20.130078 pfeed-0.0.1.dev5/pfeed/sources/bybit/api.py
+-rw-r--r--   0        0        0     1450 2024-03-28 13:44:42.597445 pfeed-0.0.1.dev5/pfeed/sources/bybit/const.py
+-rw-r--r--   0        0        0     7258 2024-03-30 06:58:44.787802 pfeed-0.0.1.dev5/pfeed/sources/bybit/download.py
+-rw-r--r--   0        0        0       72 2024-04-02 17:44:46.087958 pfeed-0.0.1.dev5/pfeed/sources/bybit/stream.py
+-rw-r--r--   0        0        0      480 2024-03-21 08:53:06.857716 pfeed-0.0.1.dev5/pfeed/utils/monitor.py
+-rw-r--r--   0        0        0     3390 2024-03-17 09:20:15.751908 pfeed-0.0.1.dev5/pfeed/utils/utils.py
+-rw-r--r--   0        0        0     1964 2024-03-17 07:37:10.997985 pfeed-0.0.1.dev5/pfeed/utils/validate.py
+-rw-r--r--   0        0        0     1503 2024-04-03 03:52:03.651170 pfeed-0.0.1.dev5/pyproject.toml
+-rw-r--r--   0        0        0    12751 1970-01-01 00:00:00.000000 pfeed-0.0.1.dev5/PKG-INFO
```

### Comparing `pfeed-0.0.1.dev4/LICENSE` & `pfeed-0.0.1.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev4/pfeed/cli/commands/config.py` & `pfeed-0.0.1.dev5/pfeed/cli/commands/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 import click
 
 from pfeed.const.paths import USER_CONFIG_FILE_PATH
 from pfeed.config_handler import ConfigHandler
 
 
 def save_config(config: ConfigHandler, config_file_path: str | Path):
+    if type(config_file_path) is str:
+        config_file_path = Path(config_file_path)
+    config_file_path.parent.mkdir(parents=True, exist_ok=True)
     with open(config_file_path, 'w') as f:
         yaml.dump(config.__dict__, f, default_flow_style=False)
         
 
 def remove_config(config_file_path: str | Path):
     config_file_path = Path(config_file_path)
     if config_file_path.is_file():
```

### Comparing `pfeed-0.0.1.dev4/pfeed/cli/commands/docker_compose.py` & `pfeed-0.0.1.dev5/pfeed/cli/commands/docker_compose.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,24 +15,23 @@
 ))
 @click.pass_context
 @click.option('--env-file', 'env_file_path', type=click.Path(exists=True), help='Path to the .env file')
 @click.option('--docker-file', 'docker_file_path', type=click.Path(exists=True), help='Path to the docker-compose.yml file')
 def docker_compose(ctx, env_file_path, docker_file_path):
     """Forwards commands to docker-compose with the package's docker-compose.yml file if not specified."""
     if not env_file_path:
-        env_file_path = find_dotenv(usecwd=True, raise_error_if_not_found=True)
-        click.echo(f'.env file path is not specified, using env file in "{env_file_path}"')
+        if env_file_path := find_dotenv(usecwd=True, raise_error_if_not_found=False):
+            click.echo(f'.env file path is not specified, using env file in "{env_file_path}"')
+        else:
+            click.echo('.env file is not found')
     load_dotenv(env_file_path, override=True)
     
-    # write config's data path to environment variable if not set
-    if not os.getenv('PFEED_DATA_PATH'):
-        config = ctx.obj['config']
-        click.echo(f'PFEED_DATA_PATH is not set, using data path "{config.data_path}" in config')
-        os.environ['PFEED_DATA_PATH'] = config.data_path
-        
+    config = ctx.obj['config']
+    os.environ['PFEED_DATA_PATH'] = config.data_path
+    
     if not docker_file_path:
         package_dir = Path(importlib.resources.files(PROJ_NAME)).resolve().parents[0]
         docker_file_path = package_dir / 'docker-compose.yml'
     else:
         click.echo(f'loaded custom docker-compose.yml file from "{docker_file_path}"')
     command = ['docker-compose', '-f', str(docker_file_path)] + ctx.args
     subprocess.run(command)
```

### Comparing `pfeed-0.0.1.dev4/pfeed/cli/commands/download.py` & `pfeed-0.0.1.dev5/pfeed/cli/commands/download.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,54 +1,53 @@
-import os
 import importlib
 
 import click
 from dotenv import find_dotenv, load_dotenv
 
-from pfeed.utils.validate import validate_pdts_and_ptypes
 from pfeed.const.commons import ALIASES, SUPPORTED_DOWNLOAD_DATA_SOURCES, SUPPORTED_DATA_TYPES
 
 
 # add aliases to supported download data sources
 SUPPORTED_DOWNLOAD_DATA_SOURCES_ALIASES_INCLUDED = SUPPORTED_DOWNLOAD_DATA_SOURCES + [k for k, v in ALIASES.items() if v in SUPPORTED_DOWNLOAD_DATA_SOURCES]
 
+# 'raw' data type is implicit since it doesn't have the timeframe specified, but still allow it for convenience
+# since for data source like bybit, there's only one raw data type, 'raw_tick', i.e. 'raw' will be converted to 'raw_tick'
+SUPPORTED_DATA_TYPES_IMPLICIT_RAW_ALLOWED = SUPPORTED_DATA_TYPES + ['raw']
+
 
 @click.command()
 @click.pass_context
 @click.option('--env-file', 'env_file_path', type=click.Path(exists=True), help='Path to the .env file')
-@click.option('-s', '--source', required=True, type=click.Choice(SUPPORTED_DOWNLOAD_DATA_SOURCES_ALIASES_INCLUDED, case_sensitive=False), help='Data source')
-@click.option('-p', '--pdts', multiple=True, default=[], help='List of trading products')
-@click.option('--dtypes', '--dt', multiple=True, type=click.Choice(SUPPORTED_DATA_TYPES, case_sensitive=False), help='List of data types, e.g. raw, tick, second, minute, hour, daily')
-@click.option('--ptypes', '--pt', multiple=True, default=[], help='List of product types, e.g. PERP = get all perpetuals')
-@click.option('-b', '--start-date', type=click.DateTime(formats=["%Y-%m-%d"]), help='Start date in YYYY-MM-DD format')
-@click.option('-n', '--end-date', type=click.DateTime(formats=["%Y-%m-%d"]), help='End date in YYYY-MM-DD format')
+@click.option('--data-source', '-d', required=True, type=click.Choice(SUPPORTED_DOWNLOAD_DATA_SOURCES_ALIASES_INCLUDED, case_sensitive=False), help='Data source')
+@click.option('--dtype', '--dt', 'dtypes', multiple=True, default=['raw'], type=click.Choice(SUPPORTED_DATA_TYPES_IMPLICIT_RAW_ALLOWED, case_sensitive=False), help=f'{SUPPORTED_DATA_TYPES=}. How to pass in multiple values: --dt raw --dt tick')
+@click.option('--pdt', '-p', 'pdts', multiple=True, default=[], help='List of trading products')
+@click.option('--ptype', '--pt', 'ptypes', multiple=True, default=[], help='List of product types, e.g. PERP = get all perpetuals')
+@click.option('--start-date', '-s', type=click.DateTime(formats=["%Y-%m-%d"]), help='Start date in YYYY-MM-DD format')
+@click.option('--end-date', '-e', type=click.DateTime(formats=["%Y-%m-%d"]), help='End date in YYYY-MM-DD format')
 @click.option('--batch-size', default=8, type=int, help='batch size for Ray tasks')  # REVIEW
-@click.option('--no-ray', is_flag=True)
-@click.option('--use-minio', is_flag=True)
-@click.option('--debug', is_flag=True)
-def download(ctx, env_file_path, source, pdts, dtypes, ptypes, start_date, end_date, batch_size, no_ray, use_minio, debug):
+@click.option('--no-ray', is_flag=True, help='if enabled, Ray will not be used')
+@click.option('--use-minio', is_flag=True, help='if enabled, data will be loaded into Minio')
+@click.option('--debug', is_flag=True, help='if enabled, debug mode will be enabled where logs at DEBUG level will be printed')
+def download(ctx, env_file_path, data_source, pdts, dtypes, ptypes, start_date, end_date, batch_size, no_ray, use_minio, debug):
     if not env_file_path:
-        env_file_path = find_dotenv(usecwd=True, raise_error_if_not_found=True)
-        click.echo(f'.env file path is not specified, using env file in "{env_file_path}"')
+        if env_file_path := find_dotenv(usecwd=True, raise_error_if_not_found=False):
+            click.echo(f'.env file path is not specified, using env file in "{env_file_path}"')
+        else:
+            click.echo('.env file is not found')
     load_dotenv(env_file_path, override=True)
     
-    if source in ALIASES:
-        source = ALIASES[source]
-    pdts = [pdt.replace('-', '_') for pdt in pdts]
-    validate_pdts_and_ptypes(source, pdts, ptypes, is_cli=True)
-    if start_date:
-        start_date = start_date.date()
-    if end_date:
-        end_date = end_date.date()
-    pipeline = importlib.import_module(f'pfeed.sources.{source.lower()}.download')
-    pipeline.run(
-        pdts=list(pdts),
+    if data_source in ALIASES:
+        data_source = ALIASES[data_source]
+        
+    pipeline = importlib.import_module(f'pfeed.sources.{data_source.lower()}.download')
+    pipeline.download_historical_data(
+        pdts=pdts,
         dtypes=list(dtypes),
         ptypes=list(ptypes),
-        start_date=start_date,
-        end_date=end_date,
+        start_date=start_date.date().strftime('%Y-%m-%d') if start_date else start_date,
+        end_date=end_date.date().strftime('%Y-%m-%d') if end_date else end_date,
         batch_size=batch_size,
         use_ray=not no_ray,
         use_minio=use_minio,
         debug=debug,
         config=ctx.obj['config'],
     )
```

### Comparing `pfeed-0.0.1.dev4/pfeed/cli/main.py` & `pfeed-0.0.1.dev5/pfeed/cli/main.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev4/pfeed/config/logging.yml` & `pfeed-0.0.1.dev5/pfeed/config/logging.yml`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev4/pfeed/config_handler.py` & `pfeed-0.0.1.dev5/pfeed/config_handler.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev4/pfeed/const/paths.py` & `pfeed-0.0.1.dev5/pfeed/const/paths.py`

 * *Files identical despite different names*

### Comparing `pfeed-0.0.1.dev4/pfeed/datastore.py` & `pfeed-0.0.1.dev5/pfeed/datastore.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,59 +3,49 @@
 import requests
 import logging
 from requests.exceptions import RequestException, ReadTimeout
 
 from typing import Generator
 
 from minio import Minio, S3Error
+from minio.error import MinioException
 from minio.api import ObjectWriteResult
 
 
 logger = logging.getLogger('minio')
 
 
-def check_if_minio_running():
+def assert_if_minio_running():
     endpoint = os.getenv('MINIO_HOST', 'localhost')+':'+os.getenv('MINIO_PORT', '9000')
-    if 'http' not in endpoint:
-        if 'localhost' in endpoint:
+    if not endpoint.startswith('http'):
+        if any(local in endpoint for local in ['localhost:', '127.0.0.1:']):
             endpoint = f'http://{endpoint}'
         else:
             endpoint = f'https://{endpoint}'
     try:
         response = requests.get(f'{endpoint}/minio/health/live', timeout=3)
-        if response.status_code == 200:
-            print(f"MinIO is running on {endpoint}")
-            return True
-        else:
-            raise Exception(f"Unhandled response: {response.status_code=} {response.content} {response}")
+        if response.status_code != 200:
+            raise MinioException(f"Unhandled response: {response.status_code=} {response.content} {response}")
     except (ReadTimeout, RequestException) as e:
-        print(f"MinIO is not running on {endpoint}: {e}")
-    return False
-
-
-def assert_access_key_and_secret_key_exists():
-    console_endpoint = os.getenv('MINIO_HOST', 'localhost')+':'+os.getenv('MINIO_CONSOLE_PORT', '9001')
-    assert os.getenv('MINIO_ACCESS_KEY') and os.getenv('MINIO_SECRET_KEY'), \
-        f'MINIO_ACCESS_KEY and MINIO_SECRET_KEY are required in environment variables,\nPlease create them using MinIO Console on {console_endpoint}.\n' \
-        'For details, please refer to https://min.io/docs/minio/container/administration/console/security-and-access.html'
+        raise MinioException(f"MinIO is not running or not detected on {endpoint}: {e}")
 
 
 # EXTEND, currently only consider using MinIO
 class Datastore:
     DATA_PART_SIZE = 5 * (1024 ** 2)  # part size for S3, 5 MB
-    BUCKET_NAME = 'pfeed' + '-' + os.getenv('PFEED_ENV', 'DEV').lower()
+    BUCKET_NAME = 'pfeed'
     
     def __init__(self, **kwargs):
-        assert_access_key_and_secret_key_exists()
+        assert_if_minio_running()
         self.minio = Minio(
             endpoint=os.getenv('MINIO_HOST', 'localhost')+':'+os.getenv('MINIO_PORT', '9000'),
-            access_key=os.getenv('MINIO_ACCESS_KEY'),
-            secret_key=os.getenv('MINIO_SECRET_KEY'),
+            access_key=os.getenv('MINIO_ROOT_USER', 'pfunder'),
+            secret_key=os.getenv('MINIO_ROOT_PASSWORD', 'password'),
             # turn off TLS, i.e. not using HTTPS
-            secure=True if os.getenv('PFEED_ENV', 'DEV').upper() == 'PRD' else False,
+            secure=True if os.getenv('MINIO_HOST', 'localhost') not in ['localhost', '127.0.0.1'] else False,
             **kwargs,
         )
 
     def __getattr__(self, attr):
         '''gets triggered only when the attribute is not found'''
         return getattr(self.minio, attr)
```

### Comparing `pfeed-0.0.1.dev4/pfeed/feeds/bybit_feed.py` & `pfeed-0.0.1.dev5/pfeed/data_tools/data_tool_polars.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,92 +1,104 @@
+"""This module contains functions for data manipulation using Polars."""
 import io
+import logging
 import datetime
 
-import pandas as pd
+import polars as pl
+from pfund.datas.resolution import Resolution
 
-from pfeed.config_handler import ConfigHandler
-from pfeed.feeds.base_feed import BaseFeed
-from pfeed.sources.bybit import api
-from pfeed.sources.bybit import etl
-from pfeed.sources.bybit.const import DATA_SOURCE, create_efilename
-from pfeed.utils.utils import get_dates_in_between, rollback_date_range
 
+logger = logging.getLogger('pfeed')
 
-__all__ = ['BybitFeed']
 
-
-class BybitFeed(BaseFeed):
-    def __init__(self, config: ConfigHandler | None=None):
-        super().__init__('bybit', config=config)
-    
-    @staticmethod
-    def _derive_dtype_from_resolution(resolution):
-        from pfund.datas.resolution import Resolution
+def estimate_memory_usage(lf: pl.LazyFrame) -> float:
+    """
+    Returns the estimated memory usage of the given LazyFrame in GB.
+    """
+    num_rows: int = lf.select(pl.len()).collect().item()
+    first_n_rows = min(num_rows, 1000)
+    memory_usage_in_gb = lf.limit(first_n_rows).collect().to_pandas().memory_usage(deep=True).sum() / (1024 ** 3)
+    estimated_memory_usage_in_gb = memory_usage_in_gb * (num_rows / first_n_rows)
+    return estimated_memory_usage_in_gb
+
+
+def to_parquet(df: pl.DataFrame, compression: str='snappy') -> bytes:
+    """Converts a Polars DataFrame to Parquet bytes format.
+
+    Args:
+        df (pl.DataFrame): The Polars DataFrame to be converted.
+        compression (optional): The compression algorithm to be used. Defaults to 'snappy'.
+
+    Returns:
+        bytes: The Parquet data in bytes format.
+    """
+    buffer = io.BytesIO()
+    df.write_parquet(buffer, compression=compression)
+    buffer.seek(0)
+    data: bytes = buffer.read()
+    return data
+
+
+def resample_data(data: bytes, resolution: str | Resolution, check_if_drop_last_bar: bool=False) -> bytes:
+    """
+    Resamples the given data based on the specified resolution.
+
+    Args:
+        data (bytes): The input data to be resampled.
+        resolution (str): The desired resolution for resampling.
+        check_if_drop_last_bar: Whether to check if the last bar is complete. Defaults to False.
+
+    Returns:
+        bytes: The resampled data in bytes format.
+    """
+    # standardize resolution by following pfund's standard, e.g. '1minute' -> '1m', which also follows Polars' standard for s/m/h/d
+    if type(resolution) is not Resolution:
         resolution = Resolution(resolution)
-        if resolution.is_tick():
-            return 'tick'
-        elif resolution.is_second():
-            return 'second'
-        elif resolution.is_minute():
-            return 'minute'
-        elif resolution.is_hour():
-            return 'hour'
-        elif resolution.is_day():
-            return 'daily'
-        else:
-            raise Exception(f'{resolution=} is not supported')
-    
-    def get_historical_data(
-        self,
-        pdt: str,
-        rollback_period: str='1w',
-        resolution: str='1d',
-        start_date: str=None,
-        end_date: str=None,
-    ) -> pd.DataFrame:
-        from pfund.exchanges.bybit.exchange import Exchange
-        
-        source = DATA_SOURCE
-        exchange = Exchange(env='LIVE')
-        adapter = exchange.adapter
-        dtype = self._derive_dtype_from_resolution(resolution)
-        product = exchange.create_product(*pdt.split('_'))
-        category = product.category
-        epdt = adapter(pdt, ref_key=category)
-        efilenames = api.get_efilenames(category, epdt)
-        
-        if start_date:
-            # default for end_date is yesterday
-            end_date: str = end_date or (datetime.datetime.now(tz=datetime.timezone.utc) - datetime.timedelta(days=1)).strftime('%Y-%m-%d')
-        else:
-            start_date, end_date = rollback_date_range(rollback_period)
-        dates: list[datetime.date] = get_dates_in_between(start_date, end_date)
-        
-        dfs = []
-        dates = [date for date in dates if create_efilename(epdt, date, is_spot=product.is_spot()) in efilenames]
-        for date in dates:
-            data_str = f'{source} {pdt} {date}'
-            if local_data := etl.extract_data(pdt, date, dtype, mode='historical', data_path=self.data_path):
-                # e.g. local_data could be 1m data (period always = 1), but resampled_data could be 3m data
-                resampled_data: bytes = etl.resample_data(local_data, resolution, is_tick=(dtype == 'tick'), category=category)
-                print(f'loaded {data_str} local {dtype} data')
-            else:
-                print(f'Downloading {data_str} data on the fly, please consider using {source.lower()}.run_historical(...) to pre-download data to your local computer first')
-                if raw_data := api.get_data(category, epdt, date):
-                    tick_data: bytes = etl.clean_data(category, raw_data)
-                    resampled_data: bytes = etl.resample_data(tick_data, resolution, is_tick=True, category=category)
-                    print(f'resampled {data_str} data to {resolution=}')
-                else:
-                    raise Exception(f'failed to download {data_str} historical data')
-            df = pd.read_parquet(io.BytesIO(resampled_data))
-            dfs.append(df)
-        return pd.concat(dfs)
-    
-    # TODO?: maybe useful if used as a standalone program, not useful at all if used with PFund
-    def get_real_time_data(self, env='LIVE'):
-        pass
-    
-        
-if __name__ == '__main__':
-    feed = BybitFeed()
-    df = feed.get_historical_data('BCH_USDT_PERP', resolution='1d', rollback_period='2d')
-    print(df)
+    eresolution = repr(resolution)
+    
+    if type(data) is bytes:
+        df = pl.read_parquet(data)
+    else:
+        raise TypeError(f'Invalid data type {type(data)}, expected bytes')
+    
+    is_tick_data = True if 'price' in df.columns else False  # REVIEW
+    assert not df.is_empty(), 'data is empty'
+    df = df.sort('ts')
+    
+    if is_tick_data:
+        resample_logic = [
+            pl.first('price').alias('open'),
+            pl.max('price').alias('high'),
+            pl.min('price').alias('low'),
+            pl.last('price').alias('close'),
+            pl.sum('volume'),
+        ]
+    else:
+        resample_logic = [
+            pl.first('open'),
+            pl.max('high'),
+            pl.min('low'),
+            pl.last('close'),
+            pl.sum('volume'),
+        ]
+    
+    # NOTE: if check_if_drop_last_bar is True, meaning data_dtype == resample_data_dtype, e.g. 'daily' -> '2d'
+    # polars will offset the ts column, making the first row e.g. 2024-03-01 to be 2024-02-29
+    # need to set start_by = 'datapoint' to avoid this
+    start_by = 'window' if not check_if_drop_last_bar else 'datapoint'
+    
+    resampled_df = (
+        df
+        .group_by_dynamic('ts', every=eresolution, closed='left', start_by=start_by)
+        .agg(resample_logic)
+    )
+    
+    # REVIEW
+    if check_if_drop_last_bar:
+        correct_timedelta = datetime.timedelta(seconds=resolution._value())
+        final_timedelta = df.select('ts')[-1].item() - resampled_df.select('ts')[-1].item() + datetime.timedelta(seconds=resolution.timeframe.unit)
+        is_drop_last_bar = (final_timedelta - correct_timedelta).total_seconds() != 0
+        if is_drop_last_bar:
+            logger.info(f'dropped the incomplete last bar {resampled_df.select("ts")[-1].item()} in the resampled data where {resolution=}')
+            resampled_df = resampled_df.slice(0, -1)
+    
+    return to_parquet(resampled_df)
```

### Comparing `pfeed-0.0.1.dev4/pfeed/feeds/yahoo_finance_feed.py` & `pfeed-0.0.1.dev5/pfeed/feeds/yahoo_finance_feed.py`

 * *Files 22% similar despite different names*

```diff
@@ -29,25 +29,29 @@
     
     def __init__(self, config: ConfigHandler | None=None):
         super().__init__('yahoo_finance', config=config)
     
     def get_ticker(self, symbol):
         return yf.Ticker(symbol.upper())
     
+    # TODO: should manipulate the input resolution and support e.g. '2d' resolution even it is not in the SUPPORTED_TIMEFRAMES_AND_PERIODS
     def get_historical_data(
         self, 
         symbol: str,
         rollback_period: str='1M', 
         resolution: str='1d', 
         start_date: str=None,
         end_date: str=None, 
         **kwargs
     ) -> pd.DataFrame:
         """Simple Wrapper of yfinance history().
         For the details of args and kwargs, please refer to https://github.com/ranaroussi/yfinance
+        
+        Args:
+            **kwargs: kwargs supported by `yfinance`
         """
         from pfund.datas.resolution import Resolution
         
         # convert pfund's rollback_period format to yfinance's period
         rollback_period = Resolution(rollback_period)
         timeframe = repr(rollback_period.timeframe)
         etimeframe = self._ADAPTER['timeframe'].get(timeframe, timeframe)
@@ -70,28 +74,29 @@
             del kwargs['interval']
         else:
             interval = eresolution
         
         if start_date:
             # default for end_date is today
             end_date = end_date or datetime.datetime.now(tz=datetime.timezone.utc).strftime('%Y-%m-%d')
+            assert start_date != end_date, f'{start_date=} and {end_date=} cannot be the same, end_date in yfinance is exclusive'    
         else:
             start_date = end_date = None
         
         ticker = self.get_ticker(symbol)
         df = ticker.history(period=period, interval=interval, start=start_date, end=end_date, **kwargs)
+        
+        assert not df.empty, f'No data found for {symbol=}, {resolution=}, {rollback_period=}, {start_date=}, {end_date=}. SUPPORTED_TIMEFRAMES_AND_PERIODS={self.SUPPORTED_TIMEFRAMES_AND_PERIODS}'
+        
         df.rename_axis('ts', inplace=True)  # rename index 'Date' to 'ts'
         df.columns = df.columns.str.lower()
         # if there are spaces in column names, they will be turned into some weird names like "_10" 
         # during "for row in df.itertuples()"
         df = df.rename(columns={'stock splits': 'stock_splits'})
         # convert to UTC
         df.index = df.index.tz_convert('UTC')
         # convert to UTC and remove +hh:mm from YYYY-MM-DD hh:mm:ss+hh:mm
-        # df.index = df.index.tz_convert('UTC').tz_localize(None)
+        df.index = df.index.tz_convert('UTC').tz_localize(None)
+        
+        df.insert(0, 'symbol', symbol)
+        df.insert(1, 'resolution', repr(resolution))
         return df
-    
-    
-if __name__ == '__main__':
-    feed = YahooFinanceFeed()
-    df = feed.get_historical_data('TSLA')
-    print(df)
```

### Comparing `pfeed-0.0.1.dev4/pfeed/filepath.py` & `pfeed-0.0.1.dev5/pfeed/filepath.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 
 from pfeed.utils.utils import create_filename
 from pfeed.const.paths import DATA_PATH
 
 
 @dataclass
 class FilePath:
-    data_source: str
+    data_source: Literal['BYBIT']
     mode: Literal['historical', 'streaming']
-    data_type: Literal['raw', 'tick', 'second', 'minute', 'hour', 'daily']
+    dtype: Literal['raw_tick', 'raw_second', 'raw_minute', 'raw_hour', 'raw_daily', 'tick', 'second', 'minute', 'hour', 'daily']
     pdt: str
     date: str
     file_extension: str = '.parquet.gz'
     data_path: str = str(DATA_PATH)
     # Derived attributes initialized via the `field(init=False)` to exclude them from the generated __init__ method
     filename: str = field(init=False)
     storage_path: str = field(init=False)
@@ -60,15 +60,15 @@
     @property
     def parent(self) -> Path:
         return self.file_Path.parent
     
     def __post_init__(self):
         self.data_source = self.data_source.lower()
         self.mode = self.mode.lower()
-        self.data_type = self.dtype = self.data_type.lower()
+        self.dtype = self.dtype = self.dtype.lower()
         self.pdt = self.pdt.lower()
         self.date = str(self.date)
         
         # derived attributes
         self.filename = create_filename(self.pdt.upper(), self.date, self.file_extension)
         self.storage_path = str(Path(self.data_source) / self.mode / self.dtype / self.pdt.upper() / self.filename)
         self.file_path = str(self.data_Path / self.storage_Path)
```

### Comparing `pfeed-0.0.1.dev4/pfeed/sources/bybit/api.py` & `pfeed-0.0.1.dev5/pfeed/sources/bybit/api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,21 @@
 import re
 import time
 import logging
 
 import requests
 
 from bs4 import BeautifulSoup
-from pfeed.sources.bybit.const import DATA_SOURCE, DATA_SOURCE_URLS, DATA_NAMING_REGEX_PATTERNS, create_efilename
+from pfeed.sources.bybit.const import DATA_SOURCE, DATA_SOURCE_URLS, DATA_NAMING_REGEX_PATTERNS, PTYPE_TO_CATEGORY, create_efilename
+from pfund.exchanges.bybit.exchange import Exchange
 
 
 logger = logging.getLogger(DATA_SOURCE.lower())
+exchange = Exchange(env='LIVE')
+adapter = exchange.adapter
 
 
 def get(url, handle_func, frequency=1, num_retry=3):
     '''
     Handles general requests.get with control on frequency and number of retry
     Args:
         handle_func: specific logic for handling response
@@ -28,36 +31,40 @@
         else:
             logger.warning(f'{res.status_code=} {res.text=}')
         time.sleep(frequency)
     else:
         logger.error(f'failed to call {url}')
 
 
-def get_efilenames(category: str, epdt: str):
+def get_efilenames(pdt: str):
     '''
     Get efilenames (e.g. BTCUSDT2022-10-04.csv.gz)
     '''
     def _handle_response(res):
         soup = BeautifulSoup(res.text, 'html.parser')
         efilenames = [node.get('href') for node in soup.find_all('a')]
         return efilenames
-    url = '/'.join([DATA_SOURCE_URLS[category], epdt])
+    ptype = pdt.split('_')[-1].upper()  # REVIEW: is this always the case?
+    epdt = adapter(pdt, ref_key=PTYPE_TO_CATEGORY[ptype])
+    url = '/'.join([DATA_SOURCE_URLS[ptype], epdt])
     return get(url, _handle_response, frequency=1, num_retry=3)
     
 
-def get_epdts(category: str, ptype: str):
+def get_epdts(ptype: str):
     def _handle_response(res):
         soup = BeautifulSoup(res.text, 'html.parser')
         epdts = [node.get('href').replace('/', '') for node in soup.find_all('a') if pattern.search(node.get('href'))]
         return epdts
     pattern = re.compile(DATA_NAMING_REGEX_PATTERNS[ptype])
-    url = DATA_SOURCE_URLS[category]
+    url = DATA_SOURCE_URLS[ptype]
     return get(url, _handle_response, frequency=1, num_retry=3)
 
 
-def get_data(category: str, epdt: str, date: str):
+def get_data(pdt: str, date: str):
     def _handle_response(res):
         data = res.content
         return data
-    efilename = create_efilename(epdt, date, is_spot=(category.upper()=='SPOT'))
-    url = f"{DATA_SOURCE_URLS[category]}/{epdt}/{efilename}"
+    ptype = pdt.split('_')[-1].upper()  # REVIEW: is this always the case?
+    epdt = adapter(pdt, ref_key=PTYPE_TO_CATEGORY[ptype])
+    efilename = create_efilename(pdt, date)
+    url = f"{DATA_SOURCE_URLS[ptype]}/{epdt}/{efilename}"
     return get(url, _handle_response, frequency=1, num_retry=3)
```

### Comparing `pfeed-0.0.1.dev4/pfeed/sources/bybit/const.py` & `pfeed-0.0.1.dev5/pfeed/sources/bybit/const.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,38 @@
+"""Metadata of bybit's data"""
+from pfund.exchanges.bybit.exchange import Exchange
+PTYPE_TO_CATEGORY = Exchange.PTYPE_TO_CATEGORY
+
 DATA_SOURCE = 'BYBIT'
-# EXTEND: support FUT and IFUT
-# SUPPORTED_PRODUCT_TYPES = ['SPOT', 'PERP', 'IPERP', 'FUT', 'IFUT']
-SUPPORTED_PRODUCT_TYPES = ['SPOT', 'PERP', 'IPERP']
-RAW_DATA_TYPE = 'tick'
-DATA_START_DATE = '2020-01-01'  # do not need to be precise
+SUPPORTED_PRODUCT_TYPES = ['SPOT', 'PERP', 'IPERP', 'FUT', 'IFUT']
+SUPPORTED_RAW_DATA_TYPES = ['raw_tick']
+DATA_START_DATE = '2020-01-01'  # do not need to be precise, if it doesn't exist, it will be skipped
 DATA_SOURCE_URLS = {
-    'linear': 'https://public.bybit.com/trading',
-    'inverse': 'https://public.bybit.com/trading',
-    'spot': 'https://public.bybit.com/spot',
+    'PERP': 'https://public.bybit.com/trading',
+    'FUT': 'https://public.bybit.com/trading',
+    'IPERP': 'https://public.bybit.com/trading',
+    'IFUT': 'https://public.bybit.com/trading',
+    'SPOT': 'https://public.bybit.com/spot',
 }
 DATA_NAMING_REGEX_PATTERNS = {
     'PERP': '(USDT\/|PERP\/)$',  # USDT perp or USDC perp;
     'FUT': '-\d{2}[A-Z]{3}\d{2}\/$',  # USDC futures e.g. BTC-10NOV23/
     'IPERP': 'USD\/$',  # inverse perps;
     'IFUT': 'USD[A-Z]\d{2}\/$',  # inverse futures e.g. BTCUSDH24/
     # match everything since everything from https://public.bybit.com/spot is spot
     'SPOT': '.*',
 }
-SELECTED_RAW_COLS = {
-    'linear': ['timestamp', 'side', 'size', 'price'],
-    'inverse': ['timestamp', 'side', 'size', 'price'],
-    'spot': ['timestamp', 'side', 'volume', 'price'],
-}
-RENAMING_COLS = {
-    'linear': {'timestamp': 'ts', 'size': 'volume'},
-    'inverse': {'timestamp': 'ts', 'size': 'volume'},
-    'spot': {'timestamp': 'ts'},
-}
-RAW_DATA_TIMESTAMP_UNITS = {
-    'linear': 's',
-    'inverse': 's',
-    'spot': 'ms'
-}
+MAPPING_COLS = {'Buy': 1, 'Sell': -1}
+RENAMING_COLS = {'timestamp': 'ts', 'size': 'volume'}
 
 
-def create_efilename(epdt, date, is_spot=False):
+def create_efilename(pdt: str, date: str):
+    adapter = Exchange(env='LIVE').adapter
+    ptype = pdt.split('_')[-1].upper()  # REVIEW: is this always the case?
+    epdt = adapter(pdt, ref_key=PTYPE_TO_CATEGORY[ptype])
+    is_spot = (ptype == 'SPOT')
     if is_spot:
         return f'{epdt}_{date}.csv.gz'
     else:
-        return f'{epdt}{date}.csv.gz'
+        return f'{epdt}{date}.csv.gz'
+    
+
```

### Comparing `pfeed-0.0.1.dev4/pfeed/sources/bybit/download.py` & `pfeed-0.0.1.dev5/pfeed/sources/bybit/download.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,155 +4,169 @@
 import datetime
 from collections import defaultdict
 from logging.handlers import QueueHandler, QueueListener
 
 from tqdm import tqdm
 from rich.console import Console
 
-from pfund.products.product_base import BaseProduct
+from pfeed import etl
 from pfeed.config_handler import ConfigHandler
 from pfeed.utils.utils import get_dates_in_between
 from pfeed.utils.validate import validate_pdts_and_ptypes
 from pfeed.const.commons import SUPPORTED_DATA_TYPES
-from pfeed.sources.bybit.const import DATA_START_DATE, DATA_SOURCE, SUPPORTED_PRODUCT_TYPES, create_efilename
+from pfeed.sources.bybit.const import DATA_START_DATE, DATA_SOURCE, SUPPORTED_RAW_DATA_TYPES, SUPPORTED_PRODUCT_TYPES, PTYPE_TO_CATEGORY, create_efilename
 from pfeed.sources.bybit import api
-from pfeed.sources.bybit import etl
-from pfeed.datastore import check_if_minio_running
+from pfund.products.product_base import BaseProduct
+from pfund.exchanges.bybit.exchange import Exchange
+from pfund.plogging import set_up_loggers
 
 
 logger = logging.getLogger(DATA_SOURCE.lower())
 cprint = Console().print
+exchange = Exchange(env='LIVE')
+adapter = exchange.adapter
 
 
 __all__ = ['download_historical_data']
 
 
-def create_pdts_using_ptypes(exchange, ptypes) -> list[str]:
-    adapter = exchange.adapter
+def create_pdts_using_ptypes(ptypes) -> list[str]:
     pdts = []
     for ptype in ptypes:
-        category = exchange.categorize_product_type(ptype)
-        epdts = api.get_epdts(category, ptype)
+        category = PTYPE_TO_CATEGORY(ptype)
+        epdts = api.get_epdts(ptype)
         # NOTE: if adapter(epdt, ref_key=category) == epdt, i.e. key is not found in pdt matching, meaning the product has been delisted
         pdts.extend([adapter(epdt, ref_key=category) for epdt in epdts if adapter(epdt, ref_key=category) != epdt])
     return pdts
 
 
-def run_etl(product: BaseProduct, date, dtypes, data_path, use_minio):
-    category, pdt, epdt = product.category, product.pdt, product.epdt
-    if raw_data := api.get_data(category, epdt, date):
-        # EXTEND: currently the transformations are fixed and not independent, maybe allow user to pass in custom transformation functions?
-        tick_data: bytes = etl.clean_data(category, raw_data)
-        second_data: bytes = etl.resample_data(tick_data, resolution='1s', is_tick=True, category=category)
+def run_etl(product: BaseProduct, date, dtypes, use_minio):
+    pdt = product.pdt
+    if raw_data := api.get_data(pdt, date):
+        raw_tick: bytes = etl.clean_raw_data(DATA_SOURCE, raw_data)
+        tick_data: bytes = etl.clean_raw_tick_data(raw_tick)
+        second_data: bytes = etl.resample_data(tick_data, resolution='1s')
         minute_data: bytes = etl.resample_data(second_data, resolution='1m')
         hour_data: bytes = etl.resample_data(minute_data, resolution='1h')
         daily_data: bytes = etl.resample_data(hour_data, resolution='1d')
         logger.debug(f'resampled {DATA_SOURCE} {pdt} {date} data')
         resampled_datas = {
-            'raw': raw_data,
+            'raw_tick': raw_tick,
             'tick': tick_data,
             'second': second_data,
             'minute': minute_data,
             'hour': hour_data,
             'daily': daily_data,
         }
         for dtype in dtypes:
-            data = resampled_datas[dtype]
-            etl.load_data('historical', dtype, pdt, date, data, data_path=data_path, use_minio=use_minio)
+            data: bytes = resampled_datas[dtype]
+            data_sink = 'minio' if use_minio else 'local'
+            etl.load_data(data_sink, DATA_SOURCE, data, dtype, pdt, date, mode='historical')
     else:
         raise Exception(f'failed to download {DATA_SOURCE} {pdt} {date} historical data')
 
 
 def download_historical_data(
-    pdts: list[str] | None=None, 
-    dtypes: list[str] | None=None,
-    ptypes: list[str] | None=None, 
-    start_date: datetime.date | None=None, 
-    end_date: datetime.date | None=None,
+    pdts: str | list[str] | None=None, 
+    dtypes: str | list[str] | None=None,
+    ptypes: str | list[str] | None=None, 
+    start_date: str | None=None,
+    end_date: str | None=None,
     batch_size: int=8,
     use_ray: bool=True,
-    use_minio: bool=True,
+    use_minio: bool=False,
     debug: bool=False,
     config: ConfigHandler | None=None,
-):
-    from pfund.exchanges.bybit.exchange import Exchange
-    from pfund.plogging import set_up_loggers
-    
+) -> None:
     # setup
     source = DATA_SOURCE
-    exchange = Exchange(env='LIVE')
-    adapter = exchange.adapter
     
     # configure
     if not config:
         config = ConfigHandler.load_config()
         
-    if debug:
+    print(f'''Hint: 
+        You can use the command "pfeed config --data-path ..." to set your data path that stores downloaded data.
+        The current data path is: {config.data_path}.
+    ''')
+    
+    # make stream_handler level INFO if not debug, default level is DEBUG in logging.yml
+    if not debug:
         if 'handlers' not in config.logging_config:
             config.logging_config['handlers'] = {}
-        config.logging_config['handlers']['stream_handler'] = {'level': 'DEBUG'}
-    set_up_loggers(f'{config.log_path}/{os.getenv("PFEED_ENV", "DEV")}', config.logging_config_file_path, user_logging_config=config.logging_config)
-    data_path = config.data_path
+        config.logging_config['handlers']['stream_handler'] = {'level': 'INFO'}
+    set_up_loggers(config.log_path, config.logging_config_file_path, user_logging_config=config.logging_config)
     
     # prepare dtypes
-    dtypes = [dtype.lower() for dtype in dtypes] if dtypes else SUPPORTED_DATA_TYPES[:]
+    if dtypes is None:
+        dtypes = [SUPPORTED_RAW_DATA_TYPES[0]]
+    elif type(dtypes) is str:
+        dtypes = [dtypes]
+    # NOTE: if the data source supports only one raw data type, e.g. bybit has only 'raw_tick', 
+    # then 'raw' data type will be converted to 'raw_tick' implicitly
+    dtypes = [SUPPORTED_RAW_DATA_TYPES[0] if dtype.lower() == 'raw' else dtype.lower() for dtype in dtypes]
     assert all(dtype in SUPPORTED_DATA_TYPES for dtype in dtypes), f'{dtypes=} but {SUPPORTED_DATA_TYPES=}'
-    
+
     # prepare pdts
+    if pdts is None:
+        pdts = []
+    elif type(pdts) is str:
+        pdts = [pdts]
+    pdts = [pdt.replace('-', '_').upper() for pdt in pdts]
+    if ptypes is None:
+        ptypes = []
+    elif type(ptypes) is str:
+        ptypes = [ptypes]
+    ptypes = [ptype.upper() for ptype in ptypes]
     validate_pdts_and_ptypes(source, pdts, ptypes, is_cli=False)
-    ptypes = [ptype.upper() for ptype in ptypes] if ptypes else SUPPORTED_PRODUCT_TYPES[:]
-    pdts = [pdt.replace('-', '_').upper() for pdt in pdts] if pdts else []
     if not pdts:
-        pdts = create_pdts_using_ptypes(exchange, ptypes)
+        pdts = create_pdts_using_ptypes(ptypes)
+    if not ptypes:
+        ptypes = SUPPORTED_PRODUCT_TYPES[:]
     
     # prepare dates
     start_date = start_date or datetime.datetime.strptime(DATA_START_DATE, '%Y-%m-%d').date()
     end_date = end_date or datetime.datetime.now(tz=datetime.timezone.utc).date()
     dates: list[datetime.date] = get_dates_in_between(start_date, end_date)
     
     # check if use Ray
     ray_tasks = defaultdict(list)
     cprint(f"Ray is {'enabled' if use_ray else 'disabled'}", style='bold')
     
     # check if use MinIO
-    if use_minio:
-        assert check_if_minio_running(), "MinIO is not running or not detected"
     cprint(f"MinIO is {'enabled' if use_minio else 'disabled'}", style='bold')
 
     cprint(f'PFeed: downloading historical data from {source}, {start_date=} {end_date=}', style='bold yellow')
     for pdt in pdts if use_ray else tqdm(pdts, desc=f'Downloading {source} historical data by product', colour='green'):
-        product = exchange.create_product(*pdt.split('_'))
-        category = product.category
-        epdt = adapter(pdt, ref_key=category)
-        product.epdt = epdt  # HACK: add epdt to product for convenience
-        efilenames = api.get_efilenames(category, epdt)
+        try:
+            product = exchange.create_product(*pdt.split('_'))
+        except KeyError:
+            raise ValueError(f'"{pdt}" is not a valid product in {source}')
+        efilenames = api.get_efilenames(pdt)
         # check if the efilename created by the date exists in the efilenames (files on the data server)
-        dates = [date for date in dates if create_efilename(epdt, date, is_spot=product.is_spot()) in efilenames]
+        dates = [date for date in dates if create_efilename(pdt, date) in efilenames]
         for date in dates if use_ray else tqdm(dates, desc=f'Downloading {source} {pdt} historical data by date', colour='yellow'):
             if use_ray:
                 ray_tasks[pdt].append((product, date))
             else:
-                run_etl(product, date, dtypes, data_path, use_minio)
+                run_etl(product, date, dtypes, use_minio)
 
     if use_ray:
         import ray
         from ray.util.queue import Queue
 
         @ray.remote
         def _run_task(log_queue: Queue, product: BaseProduct, date: str):
             if not logger.handlers:
                 logger.addHandler(QueueHandler(log_queue))
                 logger.setLevel(logging.DEBUG)
-            run_etl(product, date, dtypes, data_path, use_minio)
+            run_etl(product, date, dtypes, use_minio)
 
         log_queue = Queue()
         QueueListener(log_queue, *logger.handlers, respect_handler_level=True).start()
         for pdt in tqdm(ray_tasks, desc=f'Downloading {source} historical data by product', colour='green'):
             batches = [ray_tasks[pdt][i: i + batch_size] for i in range(0, len(ray_tasks[pdt]), batch_size)]
             for batch in tqdm(batches, desc=f'Downloading {source} {pdt} historical data by batch ({batch_size=})', colour='yellow'):
                 futures = [_run_task.remote(log_queue, *task) for task in batch]
                 ray.get(futures)
-                
-    logger.warning(f'finished downloading {source} historical data to {data_path}')
-    
-    
-run = download_historical_data
+        
+    logger.warning(f'finished downloading {source} historical data to {config.data_path}')
```

### Comparing `pfeed-0.0.1.dev4/pfeed/sources/bybit/etl.py` & `pfeed-0.0.1.dev5/pfeed/data_tools/data_tool_pandas.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,161 +1,132 @@
-'''ETL = Extract, Transform, Load data'''
+"""This module contains functions for data manipulation using Pandas."""
 import io
+import datetime
 import logging
 
-from typing import Literal
-
 import numpy as np
 import pandas as pd
 
-from pfeed.const.paths import DATA_PATH
-from pfeed.sources.bybit.const import DATA_SOURCE, SELECTED_RAW_COLS, RENAMING_COLS, RAW_DATA_TIMESTAMP_UNITS
-from pfeed.datastore import Datastore, check_if_minio_running
-from pfeed.filepath import FilePath
-
-
-logger = logging.getLogger(DATA_SOURCE.lower())
-
-
-def extract_data(
-    pdt: str,
-    date: str,
-    dtype: Literal['raw', 'tick', 'second', 'minute', 'hour', 'daily'],
-    mode: Literal['historical', 'streaming']='historical',
-    data_path: str=str(DATA_PATH),
-) -> bytes | None:
-    file_extension = '.csv.gz' if dtype == 'raw' else '.parquet.gz'
-    fp = FilePath(DATA_SOURCE, mode, dtype, pdt, date, data_path=data_path, file_extension=file_extension)
-    if fp.exists():
-        with open(fp.file_path, 'rb') as f:
-            data: bytes = f.read()
-            logger.debug(f'read data from {fp.file_path}')
-            return data
-    else:
-        # print(f'failed to find {fp.file_path}, trying to extract data from MinIO')
-        if check_if_minio_running():
-            datastore = Datastore()
-            object_name = fp.storage_path
-            data: bytes | None = datastore.get_object(object_name)
-            if data:
-                logger.debug(f'extracted data from MinIO object {object_name}')
-            else:
-                logger.error(f'failed to extract data from MinIO object {object_name}')
-            return data
-        else:
-            return None
-
-
-def load_data(
-    mode: Literal['historical', 'streaming'],
-    dtype: Literal['raw', 'tick', 'second', 'minute', 'hour', 'daily'],
-    pdt: str,
-    date: str,
-    data: bytes,
-    data_path: str=str(DATA_PATH),
-    use_minio=True,
-    **kwargs
-):  
-    file_extension = '.csv.gz' if dtype == 'raw' else '.parquet.gz'
-    fp = FilePath(DATA_SOURCE, mode, dtype, pdt, date, data_path=data_path, file_extension=file_extension)
-    if use_minio:
-        datastore = Datastore()
-        object_name = fp.storage_path
-        datastore.put_object(object_name, data, **kwargs)
-        logger.debug(f'loaded data to object {object_name} {kwargs=}')
-    else:
-        fp.parent.mkdir(parents=True, exist_ok=True)
-        with open(fp.file_path, 'wb') as f:
-            f.write(data)
-            logger.debug(f'loaded data to {fp.file_path}')
+from pfund.datas.resolution import Resolution
 
 
-def clean_data(category: str, data: bytes) -> bytes:
-    df = pd.read_csv(io.BytesIO(data), compression='gzip')
-    df = df.loc[:, SELECTED_RAW_COLS[category]]
-    df['side'] = df['side'].map({'Buy': 1, 'Sell': -1})
-    df = df.rename(columns=RENAMING_COLS[category])
-    return df.to_parquet()
+logger = logging.getLogger('pfeed')
 
 
-def resample_data(data: bytes, resolution: str, is_tick=False, category='') -> bytes:
+# TODO: separate features from OHLCV
+def resample_data(data: bytes, resolution: str | Resolution, check_if_drop_last_bar: bool=False) -> bytes:
     '''
+    Resamples the input data based on the specified resolution and returns the resampled data in Parquet format.
+    
     Args:
-        is_tick: if True, use tick data to resample data
-        resolution: # + unit (s/m/h/d), e.g. 1s
+        data (bytes): The input data to be resampled.
+        resolution (str): The resolution at which the data should be resampled. It should be in the format of "# + unit (s/m/h/d)", e.g. "1s".
+        check_if_drop_last_bar: Whether to check if the last bar is complete. Defaults to False.
+    
+    Returns:
+        bytes: The resampled data in Parquet format.
     '''
     def find_high_or_low_first(series: pd.Series):
         if not series.empty:
             argmax, argmin = series.argmax(), series.argmin()
             if argmax < argmin:
                 return 'H'
             elif argmax > argmin:
                 return 'L'
-            else:
-                return 'N'
-    # EXTEND:
+        return np.nan
+    
+    def determine_first(row):
+        if row['arg_high'] < row['arg_low']:
+            return 'H'
+        elif row['arg_high'] > row['arg_low']:
+            return 'L'
+        else:
+            # If arg_high == arg_low, return the original value of 'first'
+            return row['first']
+    
+    # standardize resolution by following pfund's standard, e.g. '1minute' -> '1m'
+    if type(resolution) is not Resolution:
+        resolution = Resolution(resolution)
+    eresolution = repr(resolution)
+        
     # 'min' means minute in pandas, please refer to https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html#dateoffset-objects
-    if 'm' in resolution:
-        resolution = resolution.replace('m', 'min')
-    elif 'd' in resolution:
-        resolution = resolution.replace('d', 'D')
-    df = pd.read_parquet(io.BytesIO(data))
-    if 'ts' in df.columns:
-        assert category, 'category must be provided'
-        df.set_index('ts', inplace=True)
-        # NOTE: this may make the `ts` value inaccurate, 
-        # e.g. 1671580800.9906 -> 1671580800.990600192
-        df.index = pd.to_datetime(df.index, unit=RAW_DATA_TIMESTAMP_UNITS[category])
-    if is_tick:
-        df['num_buys'] = df['side'].map({1: 1, -1: np.nan})
-        df['num_sells'] = df['side'].map({1: np.nan, -1: 1})
-        df['buy_volume'] = np.where(df['side'] == 1, df['volume'], np.nan)
-        df['sell_volume'] = np.where(df['side'] == -1, df['volume'], np.nan)
-        df['first'] = df['price']
+    eresolution = eresolution.replace('m', 'min')
+    eresolution = eresolution.replace('d', 'D')
+    
+    if type(data) is bytes:
+        df = pd.read_parquet(io.BytesIO(data))
+    else:
+        raise TypeError(f'Invalid data type {type(data)}, expected bytes')
+    
+    is_tick_data = True if 'price' in df.columns else False  # REVIEW
+    assert not df.empty, 'data is empty'
+    df.set_index('ts', inplace=True)
+    
+    if is_tick_data:
+        # TEMP
+        # df['num_buys'] = df['side'].map({1: 1, -1: np.nan})
+        # df['num_sells'] = df['side'].map({1: np.nan, -1: 1})
+        # df['buy_volume'] = np.where(df['side'] == 1, df['volume'], np.nan)
+        # df['sell_volume'] = np.where(df['side'] == -1, df['volume'], np.nan)
+        # df['first'] = df['price']
         resample_logic = {
-            'num_buys': 'sum',
-            'num_sells': 'sum',
-            'volume': 'sum',
-            'buy_volume': 'sum',
-            'sell_volume': 'sum',
+            # TEMP
+            # 'num_buys': 'sum',
+            # 'num_sells': 'sum',
+            # 'buy_volume': 'sum',
+            # 'sell_volume': 'sum',
+            # 'first': find_high_or_low_first
             'price': 'ohlc',
-            'first': find_high_or_low_first
+            'volume': 'sum',
         }
     else:
-        df['arg_high'] = df['high']
-        df['arg_low'] = df['low']
+        # TEMP
+        # df['arg_high'] = df['high']
+        # df['arg_low'] = df['low']
         resample_logic = {
-            'num_buys': 'sum',
-            'num_sells': 'sum',
-            'buy_volume': 'sum',
-            'sell_volume': 'sum',
-            'volume': 'sum',
+            # TEMP
+            # 'num_buys': 'sum',
+            # 'num_sells': 'sum',
+            # 'buy_volume': 'sum',
+            # 'sell_volume': 'sum',
+            # 'arg_high': lambda series: series.argmax() if not series.empty else None,
+            # 'arg_low': lambda series: series.argmin() if not series.empty else None,
             'open': 'first',
             'high': 'max',
             'low': 'min',
             'close': 'last',
-            'arg_high': lambda series: series.argmax() if not series.empty else None,
-            'arg_low': lambda series: series.argmin() if not series.empty else None,
+            'volume': 'sum',
         }
+        # TEMP
+        # if 'first' in df.columns:
+        #     resample_logic['first'] = 'first'
+            
     resampled_df = (
         df
-        .resample(resolution)
+        .resample(eresolution)
         .apply(resample_logic)
-        .dropna()
     )
-    if is_tick:
+    
+    if is_tick_data:
         resampled_df = resampled_df.droplevel(0, axis=1)
-        # convert float to int
-        resampled_df['num_buys'] = resampled_df['num_buys'].astype(int)
-        resampled_df['num_sells'] = resampled_df['num_sells'].astype(int)
-    else:
-        resampled_df['first'] = (resampled_df['arg_high'] < resampled_df['arg_low']).map({True: 'H', False: 'L'})
-        resampled_df['first'] = resampled_df['first'].where(resampled_df['arg_high'] != resampled_df['arg_low'], other='N')
-        resampled_df.drop(columns=['arg_high', 'arg_low'], inplace=True)
-    return resampled_df.to_parquet()
-
-
-if __name__ == '__main__':
-    pdt = 'BTC_USDT_PERP'
-    date = '2023-11-02'
-    dtype = 'raw'
-    data: bytes = extract_data(pdt, date, dtype)
+    # TEMP
+    #     # convert float to int
+    #     resampled_df['num_buys'] = resampled_df['num_buys'].astype(int)
+    #     resampled_df['num_sells'] = resampled_df['num_sells'].astype(int)
+    # else:
+    #     resampled_df['first'] = resampled_df.apply(determine_first, axis=1)
+    #     resampled_df.drop(columns=['arg_high', 'arg_low'], inplace=True)
+
+    resampled_df.dropna(subset=[col for col in resampled_df.columns if col != 'first'], inplace=True)
+    
+    # REVIEW
+    if check_if_drop_last_bar:
+        correct_timedelta = datetime.timedelta(seconds=resolution._value())
+        final_timedelta = df.index[-1] - resampled_df.index[-1] + datetime.timedelta(seconds=resolution.timeframe.unit)
+        is_drop_last_bar = (final_timedelta - correct_timedelta).total_seconds() != 0
+        if is_drop_last_bar:
+            logger.info(f'dropped the incomplete last bar {resampled_df.index[-1]} in the resampled data where {resolution=}') 
+            resampled_df = resampled_df.iloc[:-1]
+    
+    resampled_df.reset_index(inplace=True)
+    
+    return resampled_df.to_parquet(compression='snappy')
```

### Comparing `pfeed-0.0.1.dev4/pfeed/utils/utils.py` & `pfeed-0.0.1.dev5/pfeed/utils/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -39,14 +39,19 @@
     match = re.search(date_pattern, filename)
     if match:
         date = match.group(0)
         return date
 
 
 def rollback_date_range(rollback_period: str) -> tuple[datetime.date, datetime.date]:
+    from pfund.datas.resolution import Resolution
+    
+    # check if rollback_period is a valid Resolution
+    rollback_period = repr(Resolution(rollback_period))
+    
     '''Returns start_date and end_date based on the rollback_period (e.g. '1w', '1M').'''
     def _nextmonth(year, month):
         if month == 12:
             return year+1, 1
         else:
             return year, month+1
     utcnow = datetime.datetime.now(tz=datetime.timezone.utc)
```

### Comparing `pfeed-0.0.1.dev4/pfeed/utils/validate.py` & `pfeed-0.0.1.dev5/pfeed/utils/validate.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,27 +2,35 @@
 import re
 import importlib
 
 import click
 from rich.console import Console
 
 
+def validate_pdt(source: str, pdt: str) -> bool:
+    SUPPORTED_PRODUCT_TYPES = getattr(importlib.import_module(f'pfeed.sources.{source.lower()}.const'), 'SUPPORTED_PRODUCT_TYPES')
+    # REVIEW: pattern: XXX_YYY_PTYPE, hard-coded the max length of XXX and YYY is 8
+    pdt_pattern = re.compile(r'^[A-Za-z]{1,8}_[A-Za-z]{1,8}_(.+)$')
+    match = pdt_pattern.match(pdt)
+    if not match or match.group(1) not in SUPPORTED_PRODUCT_TYPES:
+        return False
+    else:
+        return True
+
+
 def validate_pdts_and_ptypes(source: str, pdts: list[str], ptypes: list[str], is_cli=False):
     SUPPORTED_PRODUCT_TYPES = getattr(importlib.import_module(f'pfeed.sources.{source.lower()}.const'), 'SUPPORTED_PRODUCT_TYPES')
     if not pdts and not ptypes:
         Console().print(f'Warning: no "--pdts" or "--ptypes" provided, will download ALL products with ALL product types {SUPPORTED_PRODUCT_TYPES} from {source}', style='bold red')
         if is_cli and not click.confirm('Do you want to continue?', default=False):
             sys.exit(1)
     elif pdts:
-        # REVIEW: pattern: XXX_YYY_PTYPE, hard-coded the max length of XXX and YYY is 8
-        pdt_pattern = re.compile(r'^[A-Za-z]{1,8}_[A-Za-z]{1,8}_(.+)$')
         for pdt in pdts:
-            match = pdt_pattern.match(pdt)
-            if not match or match.group(1) not in SUPPORTED_PRODUCT_TYPES:
-                error_msg = f'"{pdt}" does not match the required format "XXX_YYY_PTYPE" or has an unsupported product type.'
+            if not validate_pdt(source, pdt):
+                error_msg = f'"{pdt}" does not match the required format "XXX_YYY_PTYPE" or has an unsupported product type. (PTYPE means product type, e.g. PERP, Supported types for {source} are: {SUPPORTED_PRODUCT_TYPES})'
                 raise click.BadParameter(error_msg) if is_cli else ValueError(error_msg)
     elif ptypes:
         for ptype in ptypes:
             if ptype not in SUPPORTED_PRODUCT_TYPES:
                 error_msg = f'{ptype} is not supported. Supported types are: {SUPPORTED_PRODUCT_TYPES}'
                 raise click.BadParameter(error_msg) if is_cli else ValueError(error_msg)
```

### Comparing `pfeed-0.0.1.dev4/pyproject.toml` & `pfeed-0.0.1.dev5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 [tool.poetry]
 name = "pfeed"
-version = "0.0.1.dev4"
+version = "0.0.1.dev5"
 description = "Data pipeline for algo-trading, getting and storing both real-time and historical data made easy."
 license = "Apache-2.0"
 authors = ["Stephen Yau <softwareentrepreneer+pfeed@gmail.com>"]
 readme = "README.md"
 homepage = "https://pfund.ai"
 repository = "https://github.com/PFund-Software-Ltd/pfeed"
-documentation = "https://pfund.ai/docs"
+documentation = "https://pfeed-docs.pfund.ai"
 keywords = ["trading", "algo-trading", "data pipeline", "ETL", "data lake", "data warehouse", "data integration", "historical data", "live data", "data streaming"]
 
 [tool.poetry.dependencies]
 python = "^3.10 <3.12"
 pfund = "^0.0.1.dev4"
 python-dotenv = "^1.0.1"
 pyyaml = "^6.0.1"
 beautifulsoup4 = "^4.12.3"
 requests = "^2.31.0"
 rich = "^13.7.0"
 tqdm = "^4.66.2"
-yfinance = "^0.2.36"
 pandas = "^2.2.0"
-ray = "^2.9.2"
 pyarrow = "^15.0.0"
-minio = "^7.2.4"
 click = "^8.1.7"
 platformdirs = "^4.2.0"
+polars = "^0.20.16"
+s3fs = "^2024.3.1"
+connectorx = "^0.3.2"
+ray = "^2.10.0"
+minio = "^7.2.5"
+yfinance = "^0.2.37"
 
 [tool.poetry.scripts]
 pfeed = "pfeed.main:run_cli"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pfund = {path = "../pfund", develop = true}
 pytest = "^8.0.0"
 pre-commit = "^3.6.0"
 bandit = "^1.7.7"
 ruff = "^0.1.15"
 pyright = "^1.1.349"
+pytest-xdist = "^3.5.0"
+faker = "^24.4.0"
+tox = "^4.14.2"
 
 [tool.poetry.group.doc]
 optional = true
 
 [tool.poetry.group.doc.dependencies]
 jupyter-book = "^1.0.0"
 notebook = "^7.1.0"
```

