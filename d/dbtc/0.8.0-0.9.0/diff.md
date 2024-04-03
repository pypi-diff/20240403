# Comparing `tmp/dbtc-0.8.0.tar.gz` & `tmp/dbtc-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbtc-0.8.0.tar", max compression
+gzip compressed data, was "dbtc-0.9.0.tar", max compression
```

## Comparing `dbtc-0.8.0.tar` & `dbtc-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,15 @@
--rw-r--r--   0        0        0     3827 2023-12-05 05:28:39.501978 dbtc-0.8.0/README.md
--rw-r--r--   0        0        0      124 2023-12-05 05:28:39.501978 dbtc-0.8.0/dbtc/__init__.py
--rw-r--r--   0        0        0       22 2023-12-05 05:28:39.501978 dbtc-0.8.0/dbtc/_version.py
--rw-r--r--   0        0        0    39179 2023-12-05 05:28:39.501978 dbtc-0.8.0/dbtc/cli.py
--rw-r--r--   0        0        0        0 2023-12-05 05:28:39.501978 dbtc-0.8.0/dbtc/client/__init__.py
--rw-r--r--   0        0        0    60697 2023-12-05 05:28:39.501978 dbtc-0.8.0/dbtc/client/admin.py
--rw-r--r--   0        0        0   352525 2023-12-05 05:28:39.501978 dbtc-0.8.0/dbtc/client/artifacts/metadata_schema.json
--rw-r--r--   0        0        0     2349 2023-12-05 05:28:39.501978 dbtc-0.8.0/dbtc/client/base.py
--rw-r--r--   0        0        0      258 2023-12-05 05:28:39.501978 dbtc-0.8.0/dbtc/client/main.py
--rw-r--r--   0        0        0    24548 2023-12-05 05:28:39.501978 dbtc-0.8.0/dbtc/client/metadata.py
--rw-r--r--   0        0        0    62305 2023-12-05 05:28:39.501978 dbtc-0.8.0/dbtc/client/schema.py
--rw-r--r--   0        0        0      103 2023-12-05 05:28:39.505978 dbtc-0.8.0/dbtc/console.py
--rw-r--r--   0        0        0       44 2023-12-05 05:28:39.505978 dbtc-0.8.0/dbtc/models/__init__.py
--rw-r--r--   0        0        0      524 2023-12-05 05:28:39.505978 dbtc-0.8.0/dbtc/models/webhooks.py
--rw-r--r--   0        0        0      428 2023-12-05 05:28:39.505978 dbtc-0.8.0/dbtc/utils.py
--rw-r--r--   0        0        0      905 2023-12-05 05:28:53.322143 dbtc-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     4738 1970-01-01 00:00:00.000000 dbtc-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     4679 2024-01-12 03:28:21.520709 dbtc-0.9.0/README.md
+-rw-r--r--   0        0        0      124 2024-01-12 03:28:21.520709 dbtc-0.9.0/dbtc/__init__.py
+-rw-r--r--   0        0        0       22 2024-01-12 03:28:21.520709 dbtc-0.9.0/dbtc/_version.py
+-rw-r--r--   0        0        0    33762 2024-01-12 03:28:21.520709 dbtc-0.9.0/dbtc/cli.py
+-rw-r--r--   0        0        0        0 2024-01-12 03:28:21.520709 dbtc-0.9.0/dbtc/client/__init__.py
+-rw-r--r--   0        0        0    60772 2024-01-12 03:28:21.520709 dbtc-0.9.0/dbtc/client/admin.py
+-rw-r--r--   0        0        0     2349 2024-01-12 03:28:21.520709 dbtc-0.9.0/dbtc/client/base.py
+-rw-r--r--   0        0        0      258 2024-01-12 03:28:21.520709 dbtc-0.9.0/dbtc/client/main.py
+-rw-r--r--   0        0        0     4580 2024-01-12 03:28:21.520709 dbtc-0.9.0/dbtc/client/metadata.py
+-rw-r--r--   0        0        0      103 2024-01-12 03:28:21.520709 dbtc-0.9.0/dbtc/console.py
+-rw-r--r--   0        0        0       44 2024-01-12 03:28:21.520709 dbtc-0.9.0/dbtc/models/__init__.py
+-rw-r--r--   0        0        0      480 2024-01-12 03:28:21.520709 dbtc-0.9.0/dbtc/models/webhooks.py
+-rw-r--r--   0        0        0      317 2024-01-12 03:28:21.520709 dbtc-0.9.0/dbtc/utils.py
+-rw-r--r--   0        0        0      887 2024-01-12 03:28:31.200780 dbtc-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     5553 1970-01-01 00:00:00.000000 dbtc-0.9.0/PKG-INFO
```

### Comparing `dbtc-0.8.0/README.md` & `dbtc-0.9.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -79,32 +79,58 @@
 )
 
 # This returns a dictionary containing two keys
 run['data']
 run['status']
 ```
 
-Similarly, use the `metadata` property to retrieve information about certain resources within your project - the example below shows how to retrieve metadata from models related to the most recent run for a given `job_id`.
+Similarly, use the `metadata` property to retrieve information from the [Discovery API](https://docs.getdbt.com/docs/dbt-cloud-apis/discovery-api).
+Here's how you could retrieve all of the metrics for your project.
 
 ```python
 from dbtc import dbtCloudClient
 
 client = dbtCloudClient()
-
-job_id = 1
-
-models = client.metadata.get_models(job_id)
-
-# Models nested inside a couple keys
-models['data']['models']
-
-# This is a list
-models['data']['models'][0]
+query = '''
+query ($environmentId: BigInt!, $first: Int!) {
+  environment(id: $environmentId) {
+    definition {
+      metrics(first: $first) {
+        edges {
+          node {
+            name
+            description
+            type
+            formula
+            filter
+            tags
+            parents {
+              name
+              resourceType
+            }
+          }
+        }
+      }
+    }
+  }
+}
+'''
+variables = {'environmentId': 1, 'first': 500}
+data = client.metadata.query(query, variables)
+
+# Data will be in the edges key, which will be a list of nodes
+nodes = data['data']['definition']['metrics']['edges']
+for node in nodes:
+    # node is a dictionary
+    node_name = node['name']
+    ...
 ```
 
+If you're unfamiliar either with the Schema to query or even how to write a GraphQL query, I highly recommend going to the [dbt Cloud Discovery API playground](https://metadata.cloud.getdbt.com/beta/graphql).  You'll be able to interactively explore the Schema while watching it write a GraphQL query for you!
+
 ### CLI
 
 The CLI example below will map to the python cloud example above:
 
 ```bash
 dbtc trigger-job-from-failure \
     --account-id 1 \
```

#### html2text {}

```diff
@@ -21,20 +21,28 @@
 method, `trigger_job_from_failure`, that allows you to restart a job from its
 last point of failure. ```python from dbtc import dbtCloudClient # Assumes that
 DBT_CLOUD_SERVICE_TOKEN env var is set client = dbtCloudClient() account_id = 1
 job_id = 1 payload = {'cause': 'Restarting from failure'} run =
 client.cloud.trigger_job_from_failure( account_id, job_id, payload,
 should_poll=False, ) # This returns a dictionary containing two keys run
 ['data'] run['status'] ``` Similarly, use the `metadata` property to retrieve
-information about certain resources within your project - the example below
-shows how to retrieve metadata from models related to the most recent run for a
-given `job_id`. ```python from dbtc import dbtCloudClient client =
-dbtCloudClient() job_id = 1 models = client.metadata.get_models(job_id) #
-Models nested inside a couple keys models['data']['models'] # This is a list
-models['data']['models'][0] ``` ### CLI The CLI example below will map to the
-python cloud example above: ```bash dbtc trigger-job-from-failure \ --account-
-id 1 \ --job-id 1 \ --payload '{"cause": "Restarting from failure"}' \ --no-
-should-poll ``` Similarly, for the metadata example above: ```bash dbtc get-
-models --job-id 1 ``` If not setting your service token as an environment
-variable, do the following: ```bash dbtc --token this_is_my_token get_models --
-job-id 1 ``` ## License This project is licensed under the terms of the MIT
-license.
+information from the [Discovery API](https://docs.getdbt.com/docs/dbt-cloud-
+apis/discovery-api). Here's how you could retrieve all of the metrics for your
+project. ```python from dbtc import dbtCloudClient client = dbtCloudClient()
+query = ''' query ($environmentId: BigInt!, $first: Int!) { environment(id:
+$environmentId) { definition { metrics(first: $first) { edges { node { name
+description type formula filter tags parents { name resourceType } } } } } } }
+''' variables = {'environmentId': 1, 'first': 500} data = client.metadata.query
+(query, variables) # Data will be in the edges key, which will be a list of
+nodes nodes = data['data']['definition']['metrics']['edges'] for node in nodes:
+# node is a dictionary node_name = node['name'] ... ``` If you're unfamiliar
+either with the Schema to query or even how to write a GraphQL query, I highly
+recommend going to the [dbt Cloud Discovery API playground](https://
+metadata.cloud.getdbt.com/beta/graphql). You'll be able to interactively
+explore the Schema while watching it write a GraphQL query for you! ### CLI The
+CLI example below will map to the python cloud example above: ```bash dbtc
+trigger-job-from-failure \ --account-id 1 \ --job-id 1 \ --payload '{"cause":
+"Restarting from failure"}' \ --no-should-poll ``` Similarly, for the metadata
+example above: ```bash dbtc get-models --job-id 1 ``` If not setting your
+service token as an environment variable, do the following: ```bash dbtc --
+token this_is_my_token get_models --job-id 1 ``` ## License This project is
+licensed under the terms of the MIT license.
```

### Comparing `dbtc-0.8.0/dbtc/cli.py` & `dbtc-0.9.0/dbtc/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -145,18 +145,14 @@
             include_related = kwargs["include_related"]
             kwargs["include_related"] = json.loads(include_related)
         except ValueError as e:
             raise ValueError(f'"{include_related}" is not a valid JSON string') from e
     _dbt_api_request(ctx, "cloud", method, *args, **kwargs)
 
 
-def _dbt_metadata_request(ctx: typer.Context, method: str, *args, **kwargs):
-    _dbt_api_request(ctx, "metadata", method, *args, **kwargs)
-
-
 @app.callback()
 def common(
     ctx: typer.Context,
     api_key: Optional[str] = API_KEY,
     service_token: Optional[str] = TOKEN,
     host: Optional[str] = HOST,
     do_not_track: Optional[bool] = DO_NOT_TRACK,
@@ -459,134 +455,14 @@
 @app.command()
 def get_account_licenses(ctx: typer.Context, account_id: int = ACCOUNT_ID):
     """Get an account by its ID."""
     _dbt_cloud_request(ctx, "get_account_licenses", account_id)
 
 
 @app.command()
-def get_exposure(
-    ctx: typer.Context,
-    job_id: int = JOB_ID,
-    name: str = typer.Option(..., "--name", help="Name of the exposure to retrieve"),
-    run_id: int = RUN_ID_OPTIONAL,
-):
-    """Query information about a particular exposure."""
-    _dbt_metadata_request(ctx, "get_exposure", job_id, name, run_id=run_id)
-
-
-@app.command()
-def get_exposures(
-    ctx: typer.Context, job_id: int = JOB_ID, run_id: int = RUN_ID_OPTIONAL
-):
-    """Query information about all exposures in a given job."""
-    _dbt_metadata_request(ctx, "get_exposures", job_id, run_id=run_id)
-
-
-@app.command()
-def get_macro(
-    ctx: typer.Context,
-    job_id: int = JOB_ID,
-    unique_id: str = UNIQUE_ID,
-    run_id: int = RUN_ID_OPTIONAL,
-):
-    """Query information about a particular macro."""
-    _dbt_metadata_request(ctx, "get_macro", job_id, unique_id, run_id=run_id)
-
-
-@app.command()
-def get_macros(ctx: typer.Context, job_id: int = JOB_ID, run_id: int = RUN_ID_OPTIONAL):
-    """Query information about all macros in a given job."""
-    _dbt_metadata_request(ctx, "get_macros", job_id, run_id=run_id)
-
-
-@app.command()
-def get_metric(
-    ctx: typer.Context,
-    job_id: int = JOB_ID,
-    unique_id: str = UNIQUE_ID,
-    run_id: int = RUN_ID_OPTIONAL,
-):
-    """Query information about a particular metric."""
-    _dbt_metadata_request(ctx, "get_metric", job_id, unique_id, run_id=run_id)
-
-
-@app.command()
-def get_metrics(
-    ctx: typer.Context, job_id: int = JOB_ID, run_id: int = RUN_ID_OPTIONAL
-):
-    """Query information about all metrics in a given job."""
-    _dbt_metadata_request(ctx, "get_metrics", job_id, run_id=run_id)
-
-
-@app.command()
-def get_model(
-    ctx: typer.Context,
-    job_id: int = JOB_ID,
-    unique_id: str = UNIQUE_ID,
-    run_id: int = RUN_ID_OPTIONAL,
-):
-    """Query information about a particular model."""
-    _dbt_metadata_request(ctx, "get_model", job_id, unique_id, run_id=run_id)
-
-
-@app.command()
-def get_model_by_environment(
-    ctx: typer.Context,
-    environment_id: int = ENVIRONMENT_ID,
-    unique_id: str = UNIQUE_ID,
-    last_run_count: int = typer.Option(
-        10,
-        "--last-run-count",
-        help="Number of run results where this model was built to return (max of 10)",
-    ),
-    with_catalog: bool = typer.Option(
-        False,
-        "--with-catalog",
-        help="If true, return only runs that have catalog information for this model",
-    ),
-):
-    """Query information about a particular model based on environment_id."""
-    _dbt_metadata_request(
-        ctx,
-        "get_model_by_environment",
-        environment_id,
-        unique_id,
-        last_run_count=last_run_count,
-        with_catalog=with_catalog,
-    )
-
-
-@app.command()
-def get_models(
-    ctx: typer.Context,
-    job_id: int = JOB_ID,
-    run_id: int = RUN_ID_OPTIONAL,
-    database: str = typer.Option(
-        None, "--database", help="The database where this table/view lives"
-    ),
-    schema: str = typer.Option(
-        None, "--schema", help="The schema where this table/view lives"
-    ),
-    identifier: str = typer.Option(
-        None, "--identifier", help="The identifier of this table/view"
-    ),
-):
-    """Query information about all models in a given job."""
-    _dbt_metadata_request(
-        ctx,
-        "get_models",
-        job_id,
-        run_id=run_id,
-        database=database,
-        schema=schema,
-        identifier=identifier,
-    )
-
-
-@app.command()
 def get_most_recent_run(
     ctx: typer.Context,
     account_id: int = ACCOUNT_ID,
     include_related: str = INCLUDE_RELATED,
     job_id: int = typer.Option(
         None, "--job-id", "-j", help="Numeric ID of job to retrieve"
     ),
@@ -655,105 +531,14 @@
         project_id=json.loads(project_id) if project_id else project_id,
         deferring_run_id=deferring_run_id,
         step=step,
     )
 
 
 @app.command()
-def get_seed(
-    ctx: typer.Context,
-    job_id: int = JOB_ID,
-    unique_id: str = UNIQUE_ID,
-    run_id: int = RUN_ID_OPTIONAL,
-):
-    """Query information about a particular seed."""
-    _dbt_metadata_request(ctx, "get_seed", job_id, unique_id, run_id=run_id)
-
-
-@app.command()
-def get_seeds(ctx: typer.Context, job_id: int = JOB_ID, run_id: int = RUN_ID_OPTIONAL):
-    """Query information about all seeds in a given job."""
-    _dbt_metadata_request(ctx, "get_seeds", job_id, run_id=run_id)
-
-
-@app.command()
-def get_snapshot(
-    ctx: typer.Context,
-    job_id: int = JOB_ID,
-    unique_id: str = UNIQUE_ID,
-    run_id: int = RUN_ID_OPTIONAL,
-):
-    """Query information about a particular snapshot."""
-    _dbt_metadata_request(ctx, "get_snapshot", job_id, unique_id, run_id=run_id)
-
-
-@app.command()
-def get_snapshots(
-    ctx: typer.Context, job_id: int = JOB_ID, run_id: int = RUN_ID_OPTIONAL
-):
-    """Query information about all snapshots in a given job."""
-    _dbt_metadata_request(ctx, "get_snapshots", job_id, run_id=run_id)
-
-
-@app.command()
-def get_source(
-    ctx: typer.Context,
-    job_id: int = JOB_ID,
-    unique_id: str = UNIQUE_ID,
-    run_id: int = RUN_ID_OPTIONAL,
-):
-    """Query information about a particular source."""
-    _dbt_metadata_request(ctx, "get_source", job_id, unique_id, run_id=run_id)
-
-
-@app.command()
-def get_sources(
-    ctx: typer.Context,
-    job_id: int = JOB_ID,
-    run_id: int = RUN_ID_OPTIONAL,
-    database: str = typer.Option(
-        None, "--database", help="The database where this table/view lives"
-    ),
-    schema: str = typer.Option(
-        None, "--schema", help="The schema where this table/view lives"
-    ),
-    identifier: str = typer.Option(
-        None, "--identifier", help="The identifier of this table/view"
-    ),
-):
-    """Query information about all sources in a given job."""
-    _dbt_metadata_request(
-        ctx,
-        "get_sources",
-        job_id,
-        run_id=run_id,
-        database=database,
-        schema=schema,
-        identifier=identifier,
-    )
-
-
-@app.command()
-def get_test(
-    ctx: typer.Context,
-    job_id: int = JOB_ID,
-    unique_id: str = UNIQUE_ID,
-    run_id: int = RUN_ID_OPTIONAL,
-):
-    """Query information about a particular test."""
-    _dbt_metadata_request(ctx, "get_test", job_id, unique_id, run_id=run_id)
-
-
-@app.command()
-def get_tests(ctx: typer.Context, job_id: int = JOB_ID, run_id: int = RUN_ID_OPTIONAL):
-    """Query information about all tests in a given job."""
-    _dbt_metadata_request(ctx, "get_tests", job_id, run_id=run_id)
-
-
-@app.command()
 def get_job(
     ctx: typer.Context,
     account_id: int = ACCOUNT_ID,
     job_id: int = JOB_ID,
     order_by: str = ORDER_BY,
 ):
     """Return job details for a job on an account."""
@@ -1231,14 +1016,35 @@
         account_id,
         offset=offset,
         limit=limit,
     )
 
 
 @app.command()
+def query(
+    ctx: typer.Context,
+    query: str = typer.Option(..., "--query", "-q", help="The GraphQL query to run."),
+    variables: str = typer.Option(
+        None, "--variables", help="The variables to include in the request."
+    ),
+    max_pages: int = typer.Option(
+        None, "--max-pages", help="Maximum number of pages to retrieve."
+    ),
+    paginated_request_to_list: bool = typer.Option(
+        True, "--to-list", help="Whether to convert paginated requests to a list."
+    ),
+):
+    if variables is not None:
+        variables = json.loads(variables)
+    _dbt_api_request(
+        ctx, "metadata", "query", query, variables, max_pages, paginated_request_to_list
+    )
+
+
+@app.command()
 def test_connection(
     ctx: typer.Context,
     account_id: int = ACCOUNT_ID,
     project_id: int = PROJECT_ID,
     payload: str = PAYLOAD,
 ):
     """Test a warehouse connection."""
```

### Comparing `dbtc-0.8.0/dbtc/client/admin.py` & `dbtc-0.9.0/dbtc/client/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1524,14 +1524,15 @@
             account_id (int): Numeric ID of the account to retrieve
             job_id (int): Numeric ID of the job to trigger
             payload (dict): Payload required for post request
             should_poll (bool, optional): Poll until completion if `True`, completion
                 is one of success, failure, or cancelled
             poll_interval (int, optional): Number of seconds to wait in between
                 polling
+            retries (int, optional): Number of times to retry a failed job
         """
 
         def is_run_complete(run: Dict):
             return run["data"]["status"] in [
                 JobRunStatus.SUCCESS,
                 JobRunStatus.CANCELLED,
             ]
```

### Comparing `dbtc-0.8.0/dbtc/client/base.py` & `dbtc-0.9.0/dbtc/client/base.py`

 * *Files identical despite different names*

### Comparing `dbtc-0.8.0/PKG-INFO` & `dbtc-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: dbtc
-Version: 0.8.0
+Version: 0.9.0
 Summary: An unaffiliated python wrapper for dbt Cloud APIs
 License: MIT
 Keywords: dbt,requests,API,dbt Cloud
 Author: Doug Guthrie
 Author-email: douglas.p.guthrie@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: pydantic (>=1.10.5,<2.0.0)
+Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: rudder-sdk-python (>=1.0.6,<2.0.0)
-Requires-Dist: sgqlc (>=15.0,<16.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Project-URL: Documentation, https://dbtc.dpguthrie.com
 Description-Content-Type: text/markdown
 
 <p align="center">
     <a href="#"><img src="docs/img/dbt-standalone.png"></a>
 </p>
@@ -103,32 +102,58 @@
 )
 
 # This returns a dictionary containing two keys
 run['data']
 run['status']
 ```
 
-Similarly, use the `metadata` property to retrieve information about certain resources within your project - the example below shows how to retrieve metadata from models related to the most recent run for a given `job_id`.
+Similarly, use the `metadata` property to retrieve information from the [Discovery API](https://docs.getdbt.com/docs/dbt-cloud-apis/discovery-api).
+Here's how you could retrieve all of the metrics for your project.
 
 ```python
 from dbtc import dbtCloudClient
 
 client = dbtCloudClient()
-
-job_id = 1
-
-models = client.metadata.get_models(job_id)
-
-# Models nested inside a couple keys
-models['data']['models']
-
-# This is a list
-models['data']['models'][0]
+query = '''
+query ($environmentId: BigInt!, $first: Int!) {
+  environment(id: $environmentId) {
+    definition {
+      metrics(first: $first) {
+        edges {
+          node {
+            name
+            description
+            type
+            formula
+            filter
+            tags
+            parents {
+              name
+              resourceType
+            }
+          }
+        }
+      }
+    }
+  }
+}
+'''
+variables = {'environmentId': 1, 'first': 500}
+data = client.metadata.query(query, variables)
+
+# Data will be in the edges key, which will be a list of nodes
+nodes = data['data']['definition']['metrics']['edges']
+for node in nodes:
+    # node is a dictionary
+    node_name = node['name']
+    ...
 ```
 
+If you're unfamiliar either with the Schema to query or even how to write a GraphQL query, I highly recommend going to the [dbt Cloud Discovery API playground](https://metadata.cloud.getdbt.com/beta/graphql).  You'll be able to interactively explore the Schema while watching it write a GraphQL query for you!
+
 ### CLI
 
 The CLI example below will map to the python cloud example above:
 
 ```bash
 dbtc trigger-job-from-failure \
     --account-id 1 \
```

#### html2text {}

```diff
@@ -1,20 +1,19 @@
-Metadata-Version: 2.1 Name: dbtc Version: 0.8.0 Summary: An unaffiliated python
+Metadata-Version: 2.1 Name: dbtc Version: 0.9.0 Summary: An unaffiliated python
 wrapper for dbt Cloud APIs License: MIT Keywords: dbt,requests,API,dbt Cloud
 Author: Doug Guthrie Author-email: douglas.p.guthrie@gmail.com Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
-Dist: pydantic (>=1.10.5,<2.0.0) Requires-Dist: requests (>=2.27.1,<3.0.0)
-Requires-Dist: rudder-sdk-python (>=1.0.6,<2.0.0) Requires-Dist: sgqlc
-(>=15.0,<16.0) Requires-Dist: typer[all] (>=0.9.0,<0.10.0) Project-URL:
-Documentation, https://dbtc.dpguthrie.com Description-Content-Type: text/
-markdown
+Dist: pydantic (>=2.5.3,<3.0.0) Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: rudder-sdk-python (>=1.0.6,<2.0.0) Requires-Dist: typer[all]
+(>=0.9.0,<0.10.0) Project-URL: Documentation, https://dbtc.dpguthrie.com
+Description-Content-Type: text/markdown
                          _[_d_o_c_s_/_i_m_g_/_d_b_t_-_s_t_a_n_d_a_l_o_n_e_._p_n_g_]
               AAnn uunnaaffffiilliiaatteedd ppyytthhoonn iinntteerrffaaccee ffoorr ddbbtt CClloouudd AAPPIIss
                     _[_C_o_v_e_r_a_g_e_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]
 --- **Documentation**: _h_t_t_p_s_:_/_/_d_b_t_c_._d_p_g_u_t_h_r_i_e_._c_o_m **Interactive Demo**: _h_t_t_p_s_:_/
 _/_d_p_g_u_t_h_r_i_e_-_d_b_t_c_-_s_t_r_e_a_m_l_i_t_-_h_o_m_e_-_y_y_7_c_0_b_._s_t_r_e_a_m_l_i_t_._a_p_p_/ **Source Code**: _h_t_t_p_s_:_/_/
 _g_i_t_h_u_b_._c_o_m_/_d_p_g_u_t_h_r_i_e_/_d_b_t_c **V2 Docs**: _h_t_t_p_s_:_/_/_d_o_c_s_._g_e_t_d_b_t_._c_o_m_/_d_b_t_-_c_l_o_u_d_/_a_p_i_-_v_2
 **V3 Docs**: _h_t_t_p_s_:_/_/_d_o_c_s_._g_e_t_d_b_t_._c_o_m_/_d_b_t_-_c_l_o_u_d_/_a_p_i_-_v_3 --- ## Overview dbtc is
@@ -34,20 +33,28 @@
 method, `trigger_job_from_failure`, that allows you to restart a job from its
 last point of failure. ```python from dbtc import dbtCloudClient # Assumes that
 DBT_CLOUD_SERVICE_TOKEN env var is set client = dbtCloudClient() account_id = 1
 job_id = 1 payload = {'cause': 'Restarting from failure'} run =
 client.cloud.trigger_job_from_failure( account_id, job_id, payload,
 should_poll=False, ) # This returns a dictionary containing two keys run
 ['data'] run['status'] ``` Similarly, use the `metadata` property to retrieve
-information about certain resources within your project - the example below
-shows how to retrieve metadata from models related to the most recent run for a
-given `job_id`. ```python from dbtc import dbtCloudClient client =
-dbtCloudClient() job_id = 1 models = client.metadata.get_models(job_id) #
-Models nested inside a couple keys models['data']['models'] # This is a list
-models['data']['models'][0] ``` ### CLI The CLI example below will map to the
-python cloud example above: ```bash dbtc trigger-job-from-failure \ --account-
-id 1 \ --job-id 1 \ --payload '{"cause": "Restarting from failure"}' \ --no-
-should-poll ``` Similarly, for the metadata example above: ```bash dbtc get-
-models --job-id 1 ``` If not setting your service token as an environment
-variable, do the following: ```bash dbtc --token this_is_my_token get_models --
-job-id 1 ``` ## License This project is licensed under the terms of the MIT
-license.
+information from the [Discovery API](https://docs.getdbt.com/docs/dbt-cloud-
+apis/discovery-api). Here's how you could retrieve all of the metrics for your
+project. ```python from dbtc import dbtCloudClient client = dbtCloudClient()
+query = ''' query ($environmentId: BigInt!, $first: Int!) { environment(id:
+$environmentId) { definition { metrics(first: $first) { edges { node { name
+description type formula filter tags parents { name resourceType } } } } } } }
+''' variables = {'environmentId': 1, 'first': 500} data = client.metadata.query
+(query, variables) # Data will be in the edges key, which will be a list of
+nodes nodes = data['data']['definition']['metrics']['edges'] for node in nodes:
+# node is a dictionary node_name = node['name'] ... ``` If you're unfamiliar
+either with the Schema to query or even how to write a GraphQL query, I highly
+recommend going to the [dbt Cloud Discovery API playground](https://
+metadata.cloud.getdbt.com/beta/graphql). You'll be able to interactively
+explore the Schema while watching it write a GraphQL query for you! ### CLI The
+CLI example below will map to the python cloud example above: ```bash dbtc
+trigger-job-from-failure \ --account-id 1 \ --job-id 1 \ --payload '{"cause":
+"Restarting from failure"}' \ --no-should-poll ``` Similarly, for the metadata
+example above: ```bash dbtc get-models --job-id 1 ``` If not setting your
+service token as an environment variable, do the following: ```bash dbtc --
+token this_is_my_token get_models --job-id 1 ``` ## License This project is
+licensed under the terms of the MIT license.
```

