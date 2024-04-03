# Comparing `tmp/tap_gainsightpx-1.0.5.tar.gz` & `tmp/tap_gainsightpx-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tap_gainsightpx-1.0.5.tar", max compression
+gzip compressed data, was "tap_gainsightpx-1.0.6.tar", max compression
```

## Comparing `tap_gainsightpx-1.0.5.tar` & `tap_gainsightpx-1.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-10-20 14:33:50.650236 tap_gainsightpx-1.0.5/LICENSE
--rw-r--r--   0        0        0     3956 2023-10-20 14:33:50.650236 tap_gainsightpx-1.0.5/README.md
--rw-r--r--   0        0        0     1076 2023-10-20 14:33:50.650236 tap_gainsightpx-1.0.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-10-20 14:33:50.650236 tap_gainsightpx-1.0.5/tap_gainsightpx/__init__.py
--rw-r--r--   0        0        0     2270 2023-10-20 14:33:50.650236 tap_gainsightpx-1.0.5/tap_gainsightpx/client.py
--rw-r--r--   0        0        0     1947 2023-10-20 14:33:50.650236 tap_gainsightpx-1.0.5/tap_gainsightpx/paginators.py
--rw-r--r--   0        0        0    20296 2023-10-20 14:33:50.654236 tap_gainsightpx-1.0.5/tap_gainsightpx/streams.py
--rw-r--r--   0        0        0     2839 2023-10-20 14:33:50.654236 tap_gainsightpx-1.0.5/tap_gainsightpx/tap.py
--rw-r--r--   0        0        0       38 2023-10-20 14:33:50.654236 tap_gainsightpx-1.0.5/tap_gainsightpx/tests/__init__.py
--rw-r--r--   0        0        0     4200 2023-10-20 14:33:50.654236 tap_gainsightpx-1.0.5/tap_gainsightpx/tests/test_core.py
--rw-r--r--   0        0        0     5006 1970-01-01 00:00:00.000000 tap_gainsightpx-1.0.5/setup.py
--rw-r--r--   0        0        0     4774 1970-01-01 00:00:00.000000 tap_gainsightpx-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-03 15:58:09.569738 tap_gainsightpx-1.0.6/LICENSE
+-rw-r--r--   0        0        0     3956 2024-04-03 15:58:09.569738 tap_gainsightpx-1.0.6/README.md
+-rw-r--r--   0        0        0     1076 2024-04-03 15:58:09.569738 tap_gainsightpx-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-03 15:58:09.569738 tap_gainsightpx-1.0.6/tap_gainsightpx/__init__.py
+-rw-r--r--   0        0        0     2270 2024-04-03 15:58:09.569738 tap_gainsightpx-1.0.6/tap_gainsightpx/client.py
+-rw-r--r--   0        0        0     1947 2024-04-03 15:58:09.569738 tap_gainsightpx-1.0.6/tap_gainsightpx/paginators.py
+-rw-r--r--   0        0        0    20132 2024-04-03 15:58:09.569738 tap_gainsightpx-1.0.6/tap_gainsightpx/streams.py
+-rw-r--r--   0        0        0     2839 2024-04-03 15:58:09.569738 tap_gainsightpx-1.0.6/tap_gainsightpx/tap.py
+-rw-r--r--   0        0        0       38 2024-04-03 15:58:09.569738 tap_gainsightpx-1.0.6/tap_gainsightpx/tests/__init__.py
+-rw-r--r--   0        0        0     4337 2024-04-03 15:58:09.569738 tap_gainsightpx-1.0.6/tap_gainsightpx/tests/test_core.py
+-rw-r--r--   0        0        0     5006 1970-01-01 00:00:00.000000 tap_gainsightpx-1.0.6/setup.py
+-rw-r--r--   0        0        0     4774 1970-01-01 00:00:00.000000 tap_gainsightpx-1.0.6/PKG-INFO
```

### Comparing `tap_gainsightpx-1.0.5/LICENSE` & `tap_gainsightpx-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tap_gainsightpx-1.0.5/README.md` & `tap_gainsightpx-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `tap_gainsightpx-1.0.5/pyproject.toml` & `tap_gainsightpx-1.0.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tap-gainsightpx"
-version = "1.0.5"
+version = "1.0.6"
 description = "`tap-gainsightpx` is a Singer tap for GainsightPX, built with the Meltano Singer SDK."
 authors = ["Josh Lloyd"]
 keywords = [
     "ELT",
     "GainsightPX",
     "Meltano",
     "Singer",
```

### Comparing `tap_gainsightpx-1.0.5/tap_gainsightpx/client.py` & `tap_gainsightpx-1.0.6/tap_gainsightpx/client.py`

 * *Files identical despite different names*

### Comparing `tap_gainsightpx-1.0.5/tap_gainsightpx/paginators.py` & `tap_gainsightpx-1.0.6/tap_gainsightpx/paginators.py`

 * *Files identical despite different names*

### Comparing `tap_gainsightpx-1.0.5/tap_gainsightpx/streams.py` & `tap_gainsightpx-1.0.6/tap_gainsightpx/streams.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,48 +14,46 @@
     name = "accounts"
     path = "/accounts"
     records_jsonpath = "$.accounts[*]"
     next_page_token_jsonpath = "$.scrollId"
     primary_keys = ["id"]
     replication_key = "lastModifiedDate"
     schema = th.PropertiesList(
-        th.Property("id", th.StringType),
-        th.Property("name", th.StringType),
-        th.Property("trackedSubscriptionId", th.StringType),
-        th.Property("sfdcId", th.StringType),
-        th.Property("lastSeenDate", th.IntegerType),
+        th.Property("createDate", th.IntegerType),
+        th.Property("customAttributes", th.ObjectType()),
         th.Property("dunsNumber", th.StringType),
+        th.Property("id", th.StringType),
         th.Property("industry", th.StringType),
-        th.Property("numberOfEmployees", th.IntegerType),
-        th.Property("sicCode", th.StringType),
-        th.Property("website", th.StringType),
-        th.Property("naicsCode", th.StringType),
-        th.Property("plan", th.StringType),
+        th.Property("lastModifiedDate", th.IntegerType),
+        th.Property("lastSeenDate", th.IntegerType),
         th.Property("location", th.ObjectType()),
+        th.Property("naicsCode", th.StringType),
+        th.Property("name", th.StringType),
+        th.Property("numberOfEmployees", th.IntegerType),
         th.Property("numberOfUsers", th.IntegerType),
-        th.Property("propertyKeys", th.ArrayType(th.StringType)),
-        th.Property("createDate", th.IntegerType),
-        th.Property("lastModifiedDate", th.IntegerType),
-        th.Property("customAttributes", th.ObjectType()),
         th.Property("parentGroupId", th.StringType),
+        th.Property("plan", th.StringType),
+        th.Property("propertyKeys", th.ArrayType(th.StringType)),
+        th.Property("sfdcId", th.StringType),
+        th.Property("sicCode", th.StringType),
+        th.Property("trackedSubscriptionId", th.StringType),
+        th.Property("website", th.StringType),
     ).to_dict()
 
-    def add_more_url_params(
-        self, params: dict, next_page_token: Optional[Any]
+    def get_url_params(
+        self, context: Optional[dict], next_page_token: Optional[Any]
     ) -> Dict[str, Any]:
-        """Add more params specific to the stream."""
+        """Return a dictionary of values to be used in URL parameterization."""
+        params: dict = {"pageSize": 100}
+
+        if self.replication_key:
+            params["sort"] = self.replication_key
         if next_page_token:
-            params["scrollId"] = next_page_token
+            params["scrollID"] = next_page_token
 
-            # todo: enable replication key method
-            # bookmarks = self.stream_state['bookmarks']
-            # replication_key_value = bookmarks[self.name]['replication_key_value']
-            # params["filter"] = ";".join([
-            #     f"{self.replication_key}>{replication_key_value}",
-            # ])
         return params
 
 
 class CustomEventsStream(GainsightPXStream):
     """Custom Events Stream."""
 
     name = "custom_events"
```

### Comparing `tap_gainsightpx-1.0.5/tap_gainsightpx/tap.py` & `tap_gainsightpx-1.0.6/tap_gainsightpx/tap.py`

 * *Files identical despite different names*

### Comparing `tap_gainsightpx-1.0.5/tap_gainsightpx/tests/test_core.py` & `tap_gainsightpx-1.0.6/tap_gainsightpx/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,18 @@
         json=json_resp(),
     )
     requests_mock.get(
         "https://api.example.com/v1/feature?pageSize=200",
         json=json_resp(),
     )
     requests_mock.get(
+        "https://api.example.com/v1/accounts?pageSize=100&sort=lastModifiedDate",
+        json=json_resp(),
+    )
+    requests_mock.get(
         "https://api.example.com/v1/events/pageView?pageSize=500&sort=date&filter="
         "date%3E%3D2022-01-01T00%3A00%3A00Z%3B"
         "date%3C%3D2022-01-01T00%3A00%3A00Z",
         json=json_resp(),
     )
     requests_mock.get(
         "https://api.example.com/v1/events/feature_match?pageSize=500&sort=date&filter="
```

### Comparing `tap_gainsightpx-1.0.5/setup.py` & `tap_gainsightpx-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 entry_points = \
 {'console_scripts': ['tap-gainsightpx = '
                      'tap_gainsightpx.tap:TapGainsightPX.cli']}
 
 setup_kwargs = {
     'name': 'tap-gainsightpx',
-    'version': '1.0.5',
+    'version': '1.0.6',
     'description': '`tap-gainsightpx` is a Singer tap for GainsightPX, built with the Meltano Singer SDK.',
     'long_description': "# tap-gainsightpx\n\n`tap-gainsightpx` is a Singer tap for GainsightPX.\n\nBuilt with the [Meltano Tap SDK](https://sdk.meltano.com) for Singer Taps.\n\n\n## Installation\n\nInstall from PyPi:\n\n```bash\npipx install tap-gainsightpx\n```\n\nInstall from GitHub:\n\n```bash\npipx install git+https://github.com/Widen/tap-gainsightpx.git@main\n```\n\n\n## Configuration\n\n### Accepted Config Options\n\n\nA full list of supported settings and capabilities for this\ntap is available by running:\n\n```bash\ntap-gainsightpx --about\n```\n\n<!--\nThis section can be created by copy-pasting the CLI output from:\n\n```\ntap-gainsightpx --about --format=markdown\n```\n-->\n\n| Setting             | Required | Default | Description |\n|:--------------------|:--------:|:-------:|:------------|\n| api_url             | False    | https://api.aptrinsic.com/v1 | The base url for GainsightPX service. See GainsightPX docs. |\n| api_key             | True     | None    | The api key to authenticate against the GainsightPX service |\n| page_size           | False    |     500 | The number of records to return from the API in single page.Default and Max is 500. |\n| start_date          | False    | 2022-10-26T00:00:00Z | The earliest record date to sync (inclusive '>='). ISO Format |\n| end_date            | False    | 2022-10-27T00:00:00Z | The latest record date to sync (inclusive '<='). ISO format. |\n| stream_maps         | False    | None    | Config object for stream maps capability. For more information check out [Stream Maps](https://sdk.meltano.com/en/latest/stream_maps.html). |\n| stream_map_config   | False    | None    | User-defined config values to be used within map expressions. |\n| flattening_enabled  | False    | None    | 'True' to enable schema flattening and automatically expand nested properties. |\n| flattening_max_depth| False    | None    | The max depth to flatten schemas. |\n\n### Configure using environment variables\n\nThis Singer tap will automatically import any environment variables within the working directory's\n`.env` if the `--config=ENV` is provided, such that config values will be considered if a matching\nenvironment variable is set either in the terminal context or in the `.env` file.\n\n### Source Authentication and Authorization\nSee the [GainsightPX documentation](https://support.gainsight.com/PX/API_for_Developers/02Usage_of_Different_APIs/Work_with_the_Gainsight_PX_REST_API#Sample_API_Calls) \nfor how to create an API key and find your base url.\n\n## Usage\n\nYou can easily run `tap-gainsightpx` by itself or in a pipeline using [Meltano](https://meltano.com/).\n\n### Executing the Tap Directly\n\n```bash\ntap-gainsightpx --version\ntap-gainsightpx --help\ntap-gainsightpx --config CONFIG --discover > ./catalog.json\n```\n\n## Developer Resources\n\nFollow these instructions to contribute to this project.\n\n### Initialize your Development Environment\n\n```bash\npipx install poetry\npoetry install\n```\n\n### Create and Run Tests\n\nCreate tests within the `tap_gainsightpx/tests` subfolder and\n  then run:\n\n```bash\npoetry run pytest\n```\n\nYou can also test the `tap-gainsightpx` CLI interface directly using `poetry run`:\n\n```bash\npoetry run tap-gainsightpx --help\n```\n\n### Testing with [Meltano](https://www.meltano.com)\n\n_**Note:** This tap will work in any Singer environment and does not require Meltano.\nExamples here are for convenience and to streamline end-to-end orchestration scenarios._\n\nNext, install Meltano (if you haven't already) and any needed plugins:\n\n```bash\n# Install meltano\npipx install meltano\n# Initialize meltano within this directory\ncd tap-gainsightpx\nmeltano install\n```\n\nNow you can test and orchestrate using Meltano:\n\n```bash\n# Test invocation:\nmeltano invoke tap-gainsightpx --version\n# OR run a test `elt` pipeline:\nmeltano elt tap-gainsightpx target-jsonl\n```\n\n### SDK Dev Guide\n\nSee the [dev guide](https://sdk.meltano.com/en/latest/dev_guide.html) for more instructions on how to use the SDK to\ndevelop your own taps and targets.\n",
     'author': 'Josh Lloyd',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Widen/tap-gainsightpx',
```

### Comparing `tap_gainsightpx-1.0.5/PKG-INFO` & `tap_gainsightpx-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tap-gainsightpx
-Version: 1.0.5
+Version: 1.0.6
 Summary: `tap-gainsightpx` is a Singer tap for GainsightPX, built with the Meltano Singer SDK.
 Home-page: https://github.com/Widen/tap-gainsightpx
 License: Apache 2.0
 Keywords: ELT,GainsightPX,Meltano,Singer,REST,API,tap
 Author: Josh Lloyd
 Requires-Python: >=3.7.1
 Classifier: License :: Other/Proprietary License
```

