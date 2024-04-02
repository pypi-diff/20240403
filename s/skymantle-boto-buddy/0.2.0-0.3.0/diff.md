# Comparing `tmp/skymantle_boto_buddy-0.2.0.tar.gz` & `tmp/skymantle_boto_buddy-0.3.0.tar.gz`

## Comparing `skymantle_boto_buddy-0.2.0.tar` & `skymantle_boto_buddy-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.2.0/src/skymantle_boto_buddy/__init__.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.2.0/src/skymantle_boto_buddy/cloudformation.py
--rw-r--r--   0        0        0     3646 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.2.0/src/skymantle_boto_buddy/dynamodb.py
--rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.2.0/src/skymantle_boto_buddy/logs.py
--rw-r--r--   0        0        0     7247 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.2.0/src/skymantle_boto_buddy/s3.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.2.0/src/skymantle_boto_buddy/ssm.py
--rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.2.0/src/skymantle_boto_buddy/stepfunctions.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.2.0/src/skymantle_boto_buddy/sts.py
--rw-r--r--   0        0        0     3447 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.2.0/tests/test_cloudformation.py
--rw-r--r--   0        0        0     9616 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.2.0/tests/test_dynamodb.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.2.0/tests/test_init.py
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.2.0/tests/test_logs.py
--rw-r--r--   0        0        0    10626 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.2.0/tests/test_s3.py
--rw-r--r--   0        0        0     2251 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.2.0/tests/test_ssm.py
--rw-r--r--   0        0        0     5762 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.2.0/tests/test_stepfunctions.py
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.2.0/tests/test_sts.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.2.0/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.2.0/LICENSE
--rw-r--r--   0        0        0     4323 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.2.0/README.md
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.2.0/pyproject.toml
--rw-r--r--   0        0        0    17989 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.2.0/PKG-INFO
--rw-r--r--   0        0        0     5146 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.2.0/setup.py
+-rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.3.0/src/skymantle_boto_buddy/__init__.py
+-rw-r--r--   0        0        0     1531 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.3.0/src/skymantle_boto_buddy/cloudformation.py
+-rw-r--r--   0        0        0     5186 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.3.0/src/skymantle_boto_buddy/dynamodb.py
+-rw-r--r--   0        0        0      626 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.3.0/src/skymantle_boto_buddy/logs.py
+-rw-r--r--   0        0        0     7379 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.3.0/src/skymantle_boto_buddy/s3.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.3.0/src/skymantle_boto_buddy/ssm.py
+-rw-r--r--   0        0        0     2334 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.3.0/src/skymantle_boto_buddy/stepfunctions.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.3.0/src/skymantle_boto_buddy/sts.py
+-rw-r--r--   0        0        0     3089 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.3.0/tests/test_cloudformation.py
+-rw-r--r--   0        0        0    15021 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.3.0/tests/test_dynamodb.py
+-rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.3.0/tests/test_init.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.3.0/tests/test_logs.py
+-rw-r--r--   0        0        0    10264 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.3.0/tests/test_s3.py
+-rw-r--r--   0        0        0     2007 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.3.0/tests/test_ssm.py
+-rw-r--r--   0        0        0     5634 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.3.0/tests/test_stepfunctions.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.3.0/tests/test_sts.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.3.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4683 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.3.0/README.md
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    18357 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     5512 2020-02-02 00:00:00.000000 skymantle_boto_buddy-0.3.0/setup.py
```

### Comparing `skymantle_boto_buddy-0.2.0/src/skymantle_boto_buddy/__init__.py` & `skymantle_boto_buddy-0.3.0/src/skymantle_boto_buddy/__init__.py`

 * *Files identical despite different names*

### Comparing `skymantle_boto_buddy-0.2.0/src/skymantle_boto_buddy/cloudformation.py` & `skymantle_boto_buddy-0.3.0/src/skymantle_boto_buddy/cloudformation.py`

 * *Files 18% similar despite different names*

```diff
@@ -21,26 +21,26 @@
 
 
 # When imported in a lambda function will load the boto client during initialization
 if os.environ.get("AWS_LAMBDA_FUNCTION_NAME") is not None:
     get_cloudformation_client()
 
 
-def describe_stacks(stack_name: str, region_name: str | None = None, session: Session = None) -> dict:
+def describe_stacks(stack_name: str, *, region_name: str | None = None, session: Session = None) -> dict:
     cloudformation_client = get_cloudformation_client(region_name, session)
     try:
         response = cloudformation_client.describe_stacks(StackName=stack_name)
     except ClientError as e:
         raise Exception(f"Cannot find stack {stack_name} in {cloudformation_client.meta.region_name}") from e
 
     return response
 
 
-def get_stack_outputs(stack_name: str, region_name: str | None = None, session: Session = None) -> dict:
-    response = describe_stacks(stack_name, region_name, session)
+def get_stack_outputs(stack_name: str, *, region_name: str | None = None, session: Session = None) -> dict:
+    response = describe_stacks(stack_name, region_name=region_name, session=session)
 
     stack_outputs = response["Stacks"][0]["Outputs"]
 
     outputs = {}
     for stack_output in stack_outputs:
         outputs[stack_output["OutputKey"]] = stack_output["OutputValue"]
```

### Comparing `skymantle_boto_buddy-0.2.0/src/skymantle_boto_buddy/logs.py` & `skymantle_boto_buddy-0.3.0/src/skymantle_boto_buddy/logs.py`

 * *Files identical despite different names*

### Comparing `skymantle_boto_buddy-0.2.0/src/skymantle_boto_buddy/s3.py` & `skymantle_boto_buddy-0.3.0/src/skymantle_boto_buddy/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,95 +32,96 @@
 if os.environ.get("AWS_LAMBDA_FUNCTION_NAME") is not None:
     get_s3_client()
     get_s3_resource()
 
 
 def get_bucket(
     name: str,
+    *,
     region_name: str | None = None,
     session: Session = None,
     config: Config = None,
     enable_cache: EnableCache = EnableCache.YES,
 ) -> Any:
     s3 = get_s3_resource(region_name, session, config, enable_cache)
     return s3.Bucket(name)
 
 
 def get_object_signed_url(
-    bucket: str, key: str, expires_in: int = 300, region_name: str | None = None, session: Session = None
+    bucket: str, key: str, expires_in: int = 300, *, region_name: str | None = None, session: Session = None
 ):
     s3_client = get_s3_client(region_name, session, Config(signature_version="s3v4"))
 
     response = s3_client.generate_presigned_url(
         "get_object", Params={"Bucket": bucket, "Key": key}, HttpMethod="GET", ExpiresIn=expires_in
     )
 
     return response
 
 
 def put_object_signed_url(
-    bucket: str, key: str, expires_in: int = 300, region_name: str | None = None, session: Session = None
+    bucket: str, key: str, expires_in: int = 300, *, region_name: str | None = None, session: Session = None
 ):
     s3_client = get_s3_client(region_name, session, Config(signature_version="s3v4"))
 
     response = s3_client.generate_presigned_url(
         "put_object", Params={"Bucket": bucket, "Key": key}, HttpMethod="PUT", ExpiresIn=expires_in
     )
 
     return response
 
 
-def get_object(bucket: str, key: str, region_name: str | None = None, session: Session = None):
+def get_object(bucket: str, key: str, *, region_name: str | None = None, session: Session = None):
     s3_client = get_s3_client(region_name, session)
     response = s3_client.get_object(
         Bucket=bucket,
         Key=key,
     )
     return response
 
 
-def get_object_bytes(bucket: str, key: str, region_name: str | None = None, session: Session = None):
-    response = get_object(bucket, key, region_name, session)
+def get_object_bytes(bucket: str, key: str, *, region_name: str | None = None, session: Session = None):
+    response = get_object(bucket, key, region_name=region_name, session=session)
     return response["Body"].read()
 
 
-def get_object_json(bucket: str, key: str, region_name: str | None = None, session: Session = None):
-    s3_object = get_object_bytes(bucket, key, region_name, session)
+def get_object_json(bucket: str, key: str, *, region_name: str | None = None, session: Session = None):
+    s3_object = get_object_bytes(bucket, key, region_name=region_name, session=session)
     return json.loads(s3_object.decode("utf-8"))
 
 
-def get_object_csv_reader(bucket: str, key: str, region_name: str | None = None, session: Session = None):
-    s3_object: bytes = get_object_bytes(bucket, key, region_name, session)
+def get_object_csv_reader(bucket: str, key: str, *, region_name: str | None = None, session: Session = None):
+    s3_object: bytes = get_object_bytes(bucket, key, region_name=region_name, session=session)
     return csv.DictReader(s3_object.decode("utf-8").splitlines(keepends=True))
 
 
 def upload_fileobj(
-    bucket: str, key: str, object_data: BytesIO, region_name: str | None = None, session: Session = None
+    bucket: str, key: str, object_data: BytesIO, *, region_name: str | None = None, session: Session = None
 ):
     object_data.seek(0)
 
     s3_client = get_s3_client(region_name, session)
     response = s3_client.upload_fileobj(Bucket=bucket, Key=key, Fileobj=object_data)
 
     return response
 
 
-def put_object(bucket: str, key: str, object_data, region_name: str | None = None, session: Session = None):
+def put_object(bucket: str, key: str, object_data, *, region_name: str | None = None, session: Session = None):
     s3_client = get_s3_client(region_name, session)
     response = s3_client.put_object(
         Bucket=bucket,
         Key=key,
         Body=object_data,
     )
 
     return response
 
 
 def put_object_json(bucket: str, key: str, json_object, *, region_name: str | None = None, session: Session = None):
-    return put_object(bucket, key, json.dumps(json_object), region_name, session)
+    return put_object(bucket, key, json.dumps(json_object), region_name=region_name, session=session)
 
 
 def delete_object(bucket: str, key: str, region_name: str | None = None, session: Session = None):
     s3_client = get_s3_client(region_name, session)
 
     response = s3_client.delete_object(Bucket=bucket, Key=key)
 
@@ -137,14 +138,15 @@
 
 
 def copy(
     source_bucket: str,
     source_key: str,
     destination_bucket: str,
     destination_key: str,
+    *,
     region_name: str | None = None,
     session: Session = None,
 ):
     s3_client = get_s3_client(region_name, session)
 
     source = {
         "Bucket": source_bucket,
@@ -156,14 +158,15 @@
 
 
 def list_objects_v2(
     bucket: str,
     prefix: str,
     max_keys: int | None = None,
     continuation_token: str | None = None,
+    *,
     region_name: str | None = None,
     session: Session = None,
 ):
     s3_client = get_s3_client(region_name, session)
 
     kwargs = {"Bucket": bucket, "Prefix": prefix}
 
@@ -184,14 +187,15 @@
 
 
 def execute_sql_query_simplified(
     bucket: str,
     key: str,
     query: str,
     input_type: str,
+    *,
     region_name: str | None = None,
     session: Session = None,
 ) -> list[Any]:
     """Performs an S3 Select statement against a file in S3.
     The aws region used is the 'DefaultRegion' in os.environ.
 
     Args:
```

### Comparing `skymantle_boto_buddy-0.2.0/src/skymantle_boto_buddy/ssm.py` & `skymantle_boto_buddy-0.3.0/src/skymantle_boto_buddy/ssm.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,23 +17,23 @@
 
 
 # When imported in a lambda function will load the boto client during initialization
 if os.environ.get("AWS_LAMBDA_FUNCTION_NAME") is not None:
     get_ssm_client()
 
 
-def get_parameter(key: str, region_name: str | None = None, session: Session = None) -> str:
+def get_parameter(key: str, *, region_name: str | None = None, session: Session = None) -> str:
     client = get_ssm_client(region_name, session)
 
     response = client.get_parameter(Name=key)
     value = response.get("Parameter", {}).get("Value")
 
     return value
 
 
-def get_parameter_decrypted(key: str, region_name: str | None = None, session: Session = None) -> str:
+def get_parameter_decrypted(key: str, *, region_name: str | None = None, session: Session = None) -> str:
     client = get_ssm_client(region_name, session)
 
     response = client.get_parameter(Name=key, WithDecryption=True)
     value = response.get("Parameter", {}).get("Value")
 
     return value
```

### Comparing `skymantle_boto_buddy-0.2.0/src/skymantle_boto_buddy/stepfunctions.py` & `skymantle_boto_buddy-0.3.0/src/skymantle_boto_buddy/stepfunctions.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,37 +23,38 @@
 
 # When imported in a lambda function will load the boto client during initialization
 if os.environ.get("AWS_LAMBDA_FUNCTION_NAME") is not None:
     get_stepfunctions_client()
 
 
 def start_execution(
-    stepfunction_arn: str, json_input: dict, region_name: str | None = None, session: Session = None
+    stepfunction_arn: str, json_input: dict, *, region_name: str | None = None, session: Session = None
 ) -> dict:
     sf_client = get_stepfunctions_client(region_name, session)
     return sf_client.start_execution(stateMachineArn=stepfunction_arn, input=json.dumps(json_input))
 
 
 def start_sync_execution(
-    stepfunction_arn: str, json_input: dict, region_name: str | None = None, session: Session = None
+    stepfunction_arn: str, json_input: dict, *, region_name: str | None = None, session: Session = None
 ) -> dict:
     sf_client = get_stepfunctions_client(region_name, session)
     return sf_client.start_sync_execution(stateMachineArn=stepfunction_arn, input=json.dumps(json_input))
 
 
-def describe_execution(execution_arn: str, region_name: str | None = None, session: Session = None) -> dict:
+def describe_execution(execution_arn: str, *, region_name: str | None = None, session: Session = None) -> dict:
     sf_client = get_stepfunctions_client(region_name, session)
     return sf_client.describe_execution(executionArn=execution_arn)
 
 
 def start_with_wait_for_completion(
     stepfunction_arn: str,
     json_input: dict,
     max_retries: int = 5,
     delay_in_seconds: int = 1,
+    *,
     region_name: str | None = None,
     session: Session = None,
 ) -> dict:
     sf_client = get_stepfunctions_client(region_name, session)
     response = sf_client.start_execution(stateMachineArn=stepfunction_arn, input=json.dumps(json_input))
 
     execution_arn = response["executionArn"]
```

### Comparing `skymantle_boto_buddy-0.2.0/src/skymantle_boto_buddy/sts.py` & `skymantle_boto_buddy-0.3.0/src/skymantle_boto_buddy/sts.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,8 +26,8 @@
 
 def get_caller_identity(region_name: str | None = None, session: Session = None) -> dict:
     sts_client = get_sts_client(region_name, session)
     return sts_client.get_caller_identity()
 
 
 def get_caller_account(region_name: str | None = None, session: Session = None) -> str:
-    return get_caller_identity()["Account"]
+    return get_caller_identity(region_name, session)["Account"]
```

### Comparing `skymantle_boto_buddy-0.2.0/tests/test_cloudformation.py` & `skymantle_boto_buddy-0.3.0/tests/test_cloudformation.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import json
 import os
 from importlib import reload
 
 import boto3
 import pytest
 from boto3 import Session
-from botocore.exceptions import NoRegionError
-from moto import mock_cloudformation
+from moto import mock_aws
 from pytest_mock import MockerFixture
 
 from skymantle_boto_buddy import EnableCache, cloudformation
 
 cfn_template = {
     "AWSTemplateFormatVersion": "2010-09-09",
     "Description": "sample template",
@@ -33,43 +32,33 @@
 def environment(mocker: MockerFixture):
     return mocker.patch.dict(
         os.environ,
         {"AWS_DEFAULT_REGION": "ca-central-1", "AWS_LAMBDA_FUNCTION_NAME": "Test_Lambda_Function"},
     )
 
 
-@mock_cloudformation
-def test_no_default_region():
-    reload(cloudformation)
-
-    with pytest.raises(NoRegionError) as e:
-        cloudformation.describe_stacks("some_stack")
-
-    assert str(e.value) == "You must specify a region."
-
-
-@mock_cloudformation
+@mock_aws
 def test_manual_region():
     reload(cloudformation)
 
     client = cloudformation.get_cloudformation_client("ca-central-1")
 
     assert type(client).__name__ == "CloudFormation"
 
 
-@mock_cloudformation
+@mock_aws
 def test_manual_session():
     reload(cloudformation)
 
     client = cloudformation.get_cloudformation_client("ca-central-1", Session())
 
     assert type(client).__name__ == "CloudFormation"
 
 
-@mock_cloudformation
+@mock_aws
 def test_cloudformation_client_cache():
     reload(cloudformation)
 
     cfn_client_cached_one = cloudformation.get_cloudformation_client("ca-central-1", enable_cache=EnableCache.YES)
     cfn_client_cached_two = cloudformation.get_cloudformation_client("ca-central-1", enable_cache=EnableCache.YES)
 
     assert cfn_client_cached_one == cfn_client_cached_two
@@ -78,39 +67,39 @@
     cfn_client_no_cache_two = cloudformation.get_cloudformation_client("ca-central-1", enable_cache=EnableCache.NO)
 
     assert cfn_client_no_cache_one != cfn_client_no_cache_two
     assert cfn_client_cached_one != cfn_client_no_cache_one
     assert cfn_client_cached_one != cfn_client_no_cache_two
 
 
-@mock_cloudformation
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_describe_stacks():
     reload(cloudformation)
 
     cfn_client = boto3.client("cloudformation", region_name="ca-central-1")
     cfn_client.create_stack(StackName="some_stack", TemplateBody=json.dumps(cfn_template))
 
     response = cloudformation.describe_stacks("some_stack")
 
     assert response["Stacks"][0]["StackName"] == "some_stack"
 
 
-@mock_cloudformation
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_describe_stacks_no_stack():
     reload(cloudformation)
 
     with pytest.raises(Exception) as e:
         cloudformation.describe_stacks("some_stack")
 
     assert str(e.value) == "Cannot find stack some_stack in ca-central-1"
 
 
-@mock_cloudformation
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_get_stack_outputs():
     reload(cloudformation)
 
     cfn_client = boto3.client("cloudformation", region_name="ca-central-1")
     cfn_client.create_stack(StackName="some_stack", TemplateBody=json.dumps(cfn_template))
```

### Comparing `skymantle_boto_buddy-0.2.0/tests/test_dynamodb.py` & `skymantle_boto_buddy-0.3.0/tests/test_dynamodb.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,76 +1,65 @@
 import os
 from importlib import reload
 
 import boto3
 import pytest
 from boto3 import Session
 from boto3.dynamodb.conditions import Key
-from botocore.exceptions import NoRegionError
-from moto import mock_dynamodb
+from moto import mock_aws
 from pytest_mock import MockerFixture
 
 from skymantle_boto_buddy import EnableCache, dynamodb
 from skymantle_boto_buddy.dynamodb import ReturnValues
 
 
 @pytest.fixture()
 def environment(mocker: MockerFixture):
     return mocker.patch.dict(
         os.environ,
         {"AWS_DEFAULT_REGION": "ca-central-1", "AWS_LAMBDA_FUNCTION_NAME": "Test_Lambda_Function"},
     )
 
 
-@mock_dynamodb
-def test_no_default_region():
-    reload(dynamodb)
-
-    with pytest.raises(NoRegionError) as e:
-        dynamodb.get_item("some_table", {"PK": "some_pk"})
-
-    assert str(e.value) == "You must specify a region."
-
-
-@mock_dynamodb
+@mock_aws
 def test_manual_region():
     reload(dynamodb)
 
-    client = dynamodb.get_dynamodb_resource("ca-central-1")
+    client = dynamodb.get_dynamodb_resource(region_name="ca-central-1")
 
     assert type(client).__name__ == "dynamodb.ServiceResource"
 
 
-@mock_dynamodb
+@mock_aws
 def test_manual_session():
     reload(dynamodb)
 
-    client = dynamodb.get_dynamodb_resource("ca-central-1", Session())
+    client = dynamodb.get_dynamodb_resource(region_name="ca-central-1", session=Session())
 
     assert type(client).__name__ == "dynamodb.ServiceResource"
 
 
-@mock_dynamodb
+@mock_aws
 def test_dynamodb_client_cache():
     reload(dynamodb)
 
-    db_client_cached_one = dynamodb.get_dynamodb_resource("ca-central-1", enable_cache=EnableCache.YES)
-    db_client_cached_two = dynamodb.get_dynamodb_resource("ca-central-1", enable_cache=EnableCache.YES)
+    db_client_cached_one = dynamodb.get_dynamodb_resource(region_name="ca-central-1", enable_cache=EnableCache.YES)
+    db_client_cached_two = dynamodb.get_dynamodb_resource(region_name="ca-central-1", enable_cache=EnableCache.YES)
 
     assert id(db_client_cached_one) == id(db_client_cached_two)
 
-    db_client_no_cache_one = dynamodb.get_dynamodb_resource("ca-central-1", enable_cache=EnableCache.NO)
-    db_client_no_cache_two = dynamodb.get_dynamodb_resource("ca-central-1", enable_cache=EnableCache.NO)
+    db_client_no_cache_one = dynamodb.get_dynamodb_resource(region_name="ca-central-1", enable_cache=EnableCache.NO)
+    db_client_no_cache_two = dynamodb.get_dynamodb_resource(region_name="ca-central-1", enable_cache=EnableCache.NO)
 
     assert id(db_client_no_cache_one) != id(db_client_no_cache_two)
     assert id(db_client_cached_one) != id(db_client_no_cache_one)
     assert id(db_client_cached_one) != id(db_client_no_cache_two)
 
 
-@mock_dynamodb
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_put_item_simplified():
     reload(dynamodb)
 
     dynamodb_client = boto3.client("dynamodb")
 
     dynamodb_client.create_table(
@@ -84,15 +73,15 @@
     assert response["ResponseMetadata"]["RetryAttempts"] == 0
 
     response = dynamodb_client.get_item(TableName="some_table", Key={"PK": {"S": "some_pk"}})
 
     assert response["Item"] == {"PK": {"S": "some_pk"}, "Name": {"S": "some value"}}
 
 
-@mock_dynamodb
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_update_item_simplified():
     reload(dynamodb)
 
     dynamodb_client = boto3.client("dynamodb")
 
     dynamodb_client.create_table(
@@ -109,15 +98,15 @@
     assert response["Attributes"]["Name"] == "some value"
 
     response = dynamodb_client.get_item(TableName="some_table", Key={"PK": {"S": "some_pk"}})
 
     assert response["Item"] == {"PK": {"S": "some_pk"}, "Name": {"S": "some new value"}}
 
 
-@mock_dynamodb
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_get_item():
     reload(dynamodb)
 
     dynamodb_client = boto3.client("dynamodb")
 
     dynamodb_client.create_table(
@@ -126,18 +115,38 @@
         AttributeDefinitions=[{"AttributeName": "PK", "AttributeType": "S"}],
         KeySchema=[{"AttributeName": "PK", "KeyType": "HASH"}],
     )
     dynamodb_client.put_item(TableName="some_table", Item={"PK": {"S": "some_pk"}, "Name": {"S": "some value"}})
 
     item = dynamodb.get_item("some_table", {"PK": "some_pk"})
 
-    assert item["Name"] == "some value"
+    assert item == {"PK": "some_pk", "Name": "some value"}
 
 
-@mock_dynamodb
+@mock_aws
+@pytest.mark.usefixtures("environment")
+def test_get_item_projection_expressions():
+    reload(dynamodb)
+
+    dynamodb_client = boto3.client("dynamodb")
+
+    dynamodb_client.create_table(
+        BillingMode="PAY_PER_REQUEST",
+        TableName="some_table",
+        AttributeDefinitions=[{"AttributeName": "PK", "AttributeType": "S"}],
+        KeySchema=[{"AttributeName": "PK", "KeyType": "HASH"}],
+    )
+    dynamodb_client.put_item(TableName="some_table", Item={"PK": {"S": "some_pk"}, "Field_Name": {"S": "some value"}})
+
+    item = dynamodb.get_item("some_table", {"PK": "some_pk"}, ["Field_Name"])
+
+    assert item == {"Field_Name": "some value"}
+
+
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_delete_item():
     reload(dynamodb)
 
     dynamodb_client = boto3.client("dynamodb")
 
     dynamodb_client.create_table(
@@ -151,15 +160,99 @@
     dynamodb.delete_item("some_table", {"PK": "some_pk"})
 
     response = dynamodb_client.get_item(TableName="some_table", Key={"PK": {"S": "some_pk"}})
 
     assert response.get("Item") is None
 
 
-@mock_dynamodb
+@mock_aws
+@pytest.mark.usefixtures("environment")
+def test_query():
+    reload(dynamodb)
+
+    dynamodb_client = boto3.client("dynamodb")
+
+    dynamodb_client.create_table(
+        BillingMode="PAY_PER_REQUEST",
+        TableName="some_table",
+        AttributeDefinitions=[
+            {"AttributeName": "PK", "AttributeType": "S"},
+            {"AttributeName": "Name", "AttributeType": "S"},
+        ],
+        KeySchema=[{"AttributeName": "PK", "KeyType": "HASH"}],
+        GlobalSecondaryIndexes=[
+            {
+                "IndexName": "Index1",
+                "KeySchema": [{"AttributeName": "Name", "KeyType": "HASH"}],
+                "Projection": {"ProjectionType": "ALL"},
+            }
+        ],
+    )
+    dynamodb_client.put_item(TableName="some_table", Item={"PK": {"S": "some_pk_1"}, "Name": {"S": "some value"}})
+    dynamodb_client.put_item(TableName="some_table", Item={"PK": {"S": "some_pk_2"}, "Name": {"S": "some value"}})
+    dynamodb_client.put_item(TableName="some_table", Item={"PK": {"S": "some_pk_3"}, "Name": {"S": "some value"}})
+    dynamodb_client.put_item(TableName="some_table", Item={"PK": {"S": "some_pk_4"}, "Name": {"S": "some value"}})
+    dynamodb_client.put_item(TableName="some_table", Item={"PK": {"S": "some_pk_5"}, "Name": {"S": "some other value"}})
+
+    result = dynamodb.query("some_table", Key("Name").eq("some value"), "Index1")
+
+    assert len(result["Items"]) == 4
+    assert result["Items"][0] == {"PK": "some_pk_1", "Name": "some value"}
+    assert result["Items"][1] == {"PK": "some_pk_2", "Name": "some value"}
+    assert result["Items"][2] == {"PK": "some_pk_3", "Name": "some value"}
+    assert result["Items"][3] == {"PK": "some_pk_4", "Name": "some value"}
+
+
+@mock_aws
+@pytest.mark.usefixtures("environment")
+def test_query_paging():
+    reload(dynamodb)
+
+    dynamodb_client = boto3.client("dynamodb")
+
+    dynamodb_client.create_table(
+        BillingMode="PAY_PER_REQUEST",
+        TableName="some_table",
+        AttributeDefinitions=[
+            {"AttributeName": "PK", "AttributeType": "S"},
+            {"AttributeName": "Name", "AttributeType": "S"},
+        ],
+        KeySchema=[{"AttributeName": "PK", "KeyType": "HASH"}],
+        GlobalSecondaryIndexes=[
+            {
+                "IndexName": "Index1",
+                "KeySchema": [{"AttributeName": "Name", "KeyType": "HASH"}],
+                "Projection": {"ProjectionType": "ALL"},
+            }
+        ],
+    )
+    dynamodb_client.put_item(TableName="some_table", Item={"PK": {"S": "some_pk_1"}, "Name": {"S": "some value"}})
+    dynamodb_client.put_item(TableName="some_table", Item={"PK": {"S": "some_pk_2"}, "Name": {"S": "some value"}})
+    dynamodb_client.put_item(TableName="some_table", Item={"PK": {"S": "some_pk_3"}, "Name": {"S": "some value"}})
+    dynamodb_client.put_item(TableName="some_table", Item={"PK": {"S": "some_pk_4"}, "Name": {"S": "some value"}})
+    dynamodb_client.put_item(TableName="some_table", Item={"PK": {"S": "some_pk_5"}, "Name": {"S": "some other value"}})
+
+    result = dynamodb.query("some_table", Key("Name").eq("some value"), "Index1", limit=2)
+
+    assert len(result["Items"]) == 2
+    assert result["Items"][0] == {"PK": "some_pk_1", "Name": "some value"}
+    assert result["Items"][1] == {"PK": "some_pk_2", "Name": "some value"}
+
+    last_evaluated_key = result["LastEvaluatedKey"]
+
+    result = dynamodb.query(
+        "some_table", Key("Name").eq("some value"), "Index1", limit=2, last_evaluated_key=last_evaluated_key
+    )
+
+    assert len(result["Items"]) == 2
+    assert result["Items"][0] == {"PK": "some_pk_3", "Name": "some value"}
+    assert result["Items"][1] == {"PK": "some_pk_4", "Name": "some value"}
+
+
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_query_no_paging():
     reload(dynamodb)
 
     dynamodb_client = boto3.client("dynamodb")
 
     dynamodb_client.create_table(
@@ -189,15 +282,15 @@
     assert len(result) == 4
     assert result[0] == {"PK": "some_pk_1", "Name": "some value"}
     assert result[1] == {"PK": "some_pk_2", "Name": "some value"}
     assert result[2] == {"PK": "some_pk_3", "Name": "some value"}
     assert result[3] == {"PK": "some_pk_4", "Name": "some value"}
 
 
-@mock_dynamodb
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_query_no_paging_with_limit():
     reload(dynamodb)
 
     dynamodb_client = boto3.client("dynamodb")
 
     dynamodb_client.create_table(
@@ -228,15 +321,15 @@
     assert result[0] == {"PK": "some_pk_1", "Name": "some value"}
     assert result[1] == {"PK": "some_pk_2", "Name": "some value"}
     assert result[2] == {"PK": "some_pk_3", "Name": "some value"}
     assert result[3] == {"PK": "some_pk_4", "Name": "some value"}
     assert result[4] == {"PK": "some_pk_5", "Name": "some value"}
 
 
-@mock_dynamodb
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_query_no_paging_no_index():
     reload(dynamodb)
 
     dynamodb_client = boto3.client("dynamodb")
 
     dynamodb_client.create_table(
@@ -256,7 +349,43 @@
     dynamodb_client.put_item(TableName="some_table", Item={"PK": {"S": "some_pk_2"}, "Name": {"S": "some value 3"}})
 
     result = dynamodb.query_no_paging("some_table", Key("PK").eq("some_pk_1"))
 
     assert len(result) == 2
     assert result[0] == {"PK": "some_pk_1", "Name": "some value 1"}
     assert result[1] == {"PK": "some_pk_1", "Name": "some value 2"}
+
+
+@mock_aws
+@pytest.mark.usefixtures("environment")
+def test_query_no_paging_project_expressions():
+    reload(dynamodb)
+
+    dynamodb_client = boto3.client("dynamodb")
+
+    dynamodb_client.create_table(
+        BillingMode="PAY_PER_REQUEST",
+        TableName="some_table",
+        AttributeDefinitions=[
+            {"AttributeName": "PK", "AttributeType": "S"},
+            {"AttributeName": "Field_Name", "AttributeType": "S"},
+        ],
+        KeySchema=[
+            {"AttributeName": "PK", "KeyType": "HASH"},
+            {"AttributeName": "Field_Name", "KeyType": "RANGE"},
+        ],
+    )
+    dynamodb_client.put_item(
+        TableName="some_table", Item={"PK": {"S": "some_pk_1"}, "Field_Name": {"S": "some value 1"}}
+    )
+    dynamodb_client.put_item(
+        TableName="some_table", Item={"PK": {"S": "some_pk_1"}, "Field_Name": {"S": "some value 2"}}
+    )
+    dynamodb_client.put_item(
+        TableName="some_table", Item={"PK": {"S": "some_pk_2"}, "Field_Name": {"S": "some value 3"}}
+    )
+
+    result = dynamodb.query_no_paging("some_table", Key("PK").eq("some_pk_1"), projection_expressions=["Field_Name"])
+
+    assert len(result) == 2
+    assert result[0] == {"Field_Name": "some value 1"}
+    assert result[1] == {"Field_Name": "some value 2"}
```

### Comparing `skymantle_boto_buddy-0.2.0/tests/test_init.py` & `skymantle_boto_buddy-0.3.0/tests/test_init.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import os
 from importlib import reload
 
 import pytest
-from moto import mock_s3
+from moto import mock_aws
 from pytest_mock import MockerFixture
 
 import skymantle_boto_buddy
 
 
 @pytest.fixture()
 def environment(mocker: MockerFixture):
     return mocker.patch.dict(
         os.environ,
         {"AWS_DEFAULT_REGION": "us-east-1", "BOTO_BUDDY_DISABLE_CACHE": "true"},
     )
 
 
-@mock_s3
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_disable_client_cache():
     reload(skymantle_boto_buddy)
 
     s3_client_cached_one = skymantle_boto_buddy.get_boto3_client("s3")
     s3_client_cached_two = skymantle_boto_buddy.get_boto3_client("s3")
 
     assert id(s3_client_cached_one) != id(s3_client_cached_two)
 
 
-@mock_s3
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_disable_resource_cache():
     reload(skymantle_boto_buddy)
 
     s3_client_cached_one = skymantle_boto_buddy.get_boto3_resource("s3")
     s3_client_cached_two = skymantle_boto_buddy.get_boto3_resource("s3")
```

### Comparing `skymantle_boto_buddy-0.2.0/tests/test_logs.py` & `skymantle_boto_buddy-0.3.0/tests/test_logs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,45 @@
 import os
 from importlib import reload
 
 import pytest
 from boto3 import Session
-from moto import mock_logs
+from moto import mock_aws
 from pytest_mock import MockerFixture
 
 from skymantle_boto_buddy import EnableCache, logs
 
 
 @pytest.fixture()
 def environment(mocker: MockerFixture):
     return mocker.patch.dict(
         os.environ,
         {"AWS_DEFAULT_REGION": "ca-central-1", "AWS_LAMBDA_FUNCTION_NAME": "Test_Lambda_Function"},
     )
 
 
-# @mock_logs
-# def test_no_default_region():
-#     reload(logs)
-
-#     with pytest.raises(NoRegionError) as e:
-#         logs.get_parameter("some_key")
-
-#     assert str(e.value) == "You must specify a region."
-
-
-@mock_logs
+@mock_aws
 def test_manual_region():
     reload(logs)
 
     client = logs.get_logs_client("ca-central-1")
 
     assert type(client).__name__ == "CloudWatchLogs"
 
 
-@mock_logs
+@mock_aws
 def test_manual_session():
     reload(logs)
 
     client = logs.get_logs_client("ca-central-1", Session())
 
     assert type(client).__name__ == "CloudWatchLogs"
 
 
-@mock_logs
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_logs_client_cache():
     reload(logs)
 
     logs_client_cached_one = logs.get_logs_client(enable_cache=EnableCache.YES)
     logs_client_cached_two = logs.get_logs_client(enable_cache=EnableCache.YES)
```

### Comparing `skymantle_boto_buddy-0.2.0/tests/test_s3.py` & `skymantle_boto_buddy-0.3.0/tests/test_s3.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,62 +1,47 @@
 import os
 from importlib import reload
 from io import BytesIO
 
 import boto3
 import pytest
 from boto3 import Session
-from moto import mock_s3
+from moto import mock_aws
 from pytest_mock import MockerFixture
 
 from skymantle_boto_buddy import EnableCache, s3
 
 
 @pytest.fixture()
 def environment(mocker: MockerFixture):
     return mocker.patch.dict(
         os.environ,
         {"AWS_DEFAULT_REGION": "us-east-1", "AWS_LAMBDA_FUNCTION_NAME": "Test_Lambda_Function"},
     )
 
 
-@mock_s3
-def test_no_default_region():
-    reload(s3)
-
-    # S3 doesn't require a region
-
-    s3_client = boto3.client("s3")
-    s3_client.create_bucket(Bucket="some_bucket")
-    s3_client.put_object(Bucket="some_bucket", Key="some_key", Body=b"File Data")
-
-    response = s3.get_object("some_bucket", "some_key")
-
-    assert response["Body"].read() == b"File Data"
-
-
-@mock_s3
+@mock_aws
 def test_manual_region():
     reload(s3)
 
     client = s3.get_s3_client("ca-central-1")
 
     assert type(client).__name__ == "S3"
 
 
-@mock_s3
+@mock_aws
 def test_manual_session():
     reload(s3)
 
     client = s3.get_s3_client("ca-central-1", Session())
 
     assert type(client).__name__ == "S3"
 
 
-@mock_s3
+@mock_aws
 def test_s3_client_cache():
     reload(s3)
 
     s3_client_cached_one = s3.get_s3_client("ca-central-1", enable_cache=EnableCache.YES)
     s3_client_cached_two = s3.get_s3_client("ca-central-1", enable_cache=EnableCache.YES)
 
     assert s3_client_cached_one == s3_client_cached_two
@@ -65,15 +50,15 @@
     s3_client_no_cache_two = s3.get_s3_client("ca-central-1", enable_cache=EnableCache.NO)
 
     assert s3_client_no_cache_one != s3_client_no_cache_two
     assert s3_client_cached_one != s3_client_no_cache_one
     assert s3_client_cached_one != s3_client_no_cache_two
 
 
-@mock_s3
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_get_bucket():
     reload(s3)
 
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
@@ -81,15 +66,15 @@
     bucket.put_object(Key="some_key", Body=b"File Data")
 
     response = s3_client.get_object(Bucket="some_bucket", Key="some_key")
 
     assert response["Body"].read() == b"File Data"
 
 
-@mock_s3
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_get_object_signed_url():
     reload(s3)
 
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
     s3_client.put_object(Bucket="some_bucket", Key="some_key", Body=b"File Data")
@@ -101,15 +86,15 @@
     assert "X-Amz-Credential" in url
     assert "X-Amz-Date" in url
     assert "X-Amz-Expires" in url
     assert "X-Amz-SignedHeaders" in url
     assert "X-Amz-Signature" in url
 
 
-@mock_s3
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_put_object_signed_url():
     reload(s3)
 
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
@@ -120,57 +105,57 @@
     assert "X-Amz-Credential" in url
     assert "X-Amz-Date" in url
     assert "X-Amz-Expires" in url
     assert "X-Amz-SignedHeaders" in url
     assert "X-Amz-Signature" in url
 
 
-@mock_s3
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_get_object():
     reload(s3)
 
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
     s3_client.put_object(Bucket="some_bucket", Key="some_key", Body=b"File Data")
 
     response = s3.get_object("some_bucket", "some_key")
 
     assert response["Body"].read() == b"File Data"
 
 
-@mock_s3
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_get_object_bytes():
     reload(s3)
 
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
     s3_client.put_object(Bucket="some_bucket", Key="some_key", Body=b"File Data")
 
     data = s3.get_object_bytes("some_bucket", "some_key")
 
     assert data == b"File Data"
 
 
-@mock_s3
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_get_object_json():
     reload(s3)
 
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
     s3_client.put_object(Bucket="some_bucket", Key="some_key", Body=b'{"key": "value"}')
 
     data = s3.get_object_json("some_bucket", "some_key")
 
     assert data == {"key": "value"}
 
 
-@mock_s3
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_get_object_csv_reader():
     reload(s3)
 
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
     s3_client.put_object(Bucket="some_bucket", Key="some_key", Body=b"col1,col2\ncol1value1,col2value2")
@@ -178,60 +163,60 @@
     csv_reader = s3.get_object_csv_reader("some_bucket", "some_key")
     data = list(csv_reader)
 
     assert data[0]["col1"] == "col1value1"
     assert data[0]["col2"] == "col2value2"
 
 
-@mock_s3
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_upload_fileobj():
     reload(s3)
 
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
     s3.upload_fileobj("some_bucket", "some_key", BytesIO(b"File Data"))
 
     response = s3_client.get_object(Bucket="some_bucket", Key="some_key")
 
     assert response["Body"].read() == b"File Data"
 
 
-@mock_s3
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_put_object():
     reload(s3)
 
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
     s3.put_object("some_bucket", "some_key", b"File Data")
 
     response = s3_client.get_object(Bucket="some_bucket", Key="some_key")
 
     assert response["Body"].read() == b"File Data"
 
 
-@mock_s3
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_put_object_json():
     reload(s3)
 
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
 
     s3.put_object_json("some_bucket", "some_key", {"key": "value"})
 
     response = s3_client.get_object(Bucket="some_bucket", Key="some_key")
 
     assert response["Body"].read() == b'{"key": "value"}'
 
 
-@mock_s3
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_delete_object():
     reload(s3)
 
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
     s3_client.put_object(Bucket="some_bucket", Key="some_key", Body=b"File Data")
@@ -240,15 +225,15 @@
 
     with pytest.raises(Exception) as e:
         s3_client.get_object(Bucket="some_bucket", Key="some_key")
 
     assert "The specified key does not exist." in str(e.value)
 
 
-@mock_s3
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_delete_objects_simplified():
     reload(s3)
 
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
     s3_client.put_object(Bucket="some_bucket", Key="some_key_1", Body=b"File Data")
@@ -263,15 +248,15 @@
 
     with pytest.raises(Exception) as e:
         s3_client.get_object(Bucket="some_bucket", Key="some_key_2")
 
     assert "The specified key does not exist." in str(e.value)
 
 
-@mock_s3
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_copy():
     reload(s3)
 
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
     s3_client.create_bucket(Bucket="another_bucket")
@@ -281,15 +266,15 @@
     s3.copy("some_bucket", "some_key_1", "another_bucket", "some_key_2")
 
     response = s3_client.get_object(Bucket="another_bucket", Key="some_key_2")
 
     assert response["Body"].read() == b"File Data"
 
 
-@mock_s3
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_list_objects_v2():
     reload(s3)
 
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
     s3_client.put_object(Bucket="some_bucket", Key="prefix1/some_key_1", Body=b"File Data")
@@ -301,15 +286,15 @@
     assert len(result["keys"]) == 3
 
     assert result["keys"][0] == "prefix1/some_key_1"
     assert result["keys"][1] == "prefix1/some_key_2"
     assert result["keys"][2] == "prefix1/some_key_3"
 
 
-@mock_s3
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_list_objects_v2_paging():
     reload(s3)
 
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
     s3_client.put_object(Bucket="some_bucket", Key="prefix1/some_key_1", Body=b"File Data")
@@ -318,24 +303,24 @@
     s3_client.put_object(Bucket="some_bucket", Key="prefix1/some_key_4", Body=b"File Data")
 
     result = s3.list_objects_v2("some_bucket", "prefix1", 2)
     assert len(result["keys"]) == 2
     assert result["keys"][0] == "prefix1/some_key_1"
     assert result["keys"][1] == "prefix1/some_key_2"
 
-    assert result["NextContinuationToken"] == "prefix1/some_key_2"
+    assert len(result["NextContinuationToken"]) > 0
 
     result = s3.list_objects_v2("some_bucket", "prefix1", 2, result["NextContinuationToken"])
 
     assert len(result["keys"]) == 2
     assert result["keys"][0] == "prefix1/some_key_3"
     assert result["keys"][1] == "prefix1/some_key_4"
 
 
-@mock_s3
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_execute_sql_query_simplified():
     reload(s3)
 
     simple_csv = """a,b,c
     e,r,f
     y,u,i
@@ -348,15 +333,15 @@
     query = "SELECT count(*) FROM S3Object"
 
     data = s3.execute_sql_query_simplified("some_bucket", "some_key", query, "csv")
 
     assert data[0] == {"_1": 4}
 
 
-@mock_s3
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_execute_sql_query_simplified_invalid_input_type():
     reload(s3)
 
     s3_client = boto3.client("s3")
     s3_client.create_bucket(Bucket="some_bucket")
```

### Comparing `skymantle_boto_buddy-0.2.0/tests/test_ssm.py` & `skymantle_boto_buddy-0.3.0/tests/test_ssm.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,57 +1,46 @@
 import os
 from importlib import reload
 
 import boto3
 import pytest
 from boto3 import Session
-from botocore.exceptions import NoRegionError
-from moto import mock_ssm
+from moto import mock_aws
 from pytest_mock import MockerFixture
 
 from skymantle_boto_buddy import EnableCache, ssm
 
 
 @pytest.fixture()
 def environment(mocker: MockerFixture):
     return mocker.patch.dict(
         os.environ,
         {"AWS_DEFAULT_REGION": "ca-central-1", "AWS_LAMBDA_FUNCTION_NAME": "Test_Lambda_Function"},
     )
 
 
-@mock_ssm
-def test_no_default_region():
-    reload(ssm)
-
-    with pytest.raises(NoRegionError) as e:
-        ssm.get_parameter("some_key")
-
-    assert str(e.value) == "You must specify a region."
-
-
-@mock_ssm
+@mock_aws
 def test_manual_region():
     reload(ssm)
 
     client = ssm.get_ssm_client("ca-central-1")
 
     assert type(client).__name__ == "SSM"
 
 
-@mock_ssm
+@mock_aws
 def test_manual_session():
     reload(ssm)
 
     client = ssm.get_ssm_client("ca-central-1", Session())
 
     assert type(client).__name__ == "SSM"
 
 
-@mock_ssm
+@mock_aws
 def test_ssm_client_cache():
     reload(ssm)
 
     ssm_client_cached_one = ssm.get_ssm_client("ca-central-1", enable_cache=EnableCache.YES)
     ssm_client_cached_two = ssm.get_ssm_client("ca-central-1", enable_cache=EnableCache.YES)
 
     assert ssm_client_cached_one == ssm_client_cached_two
@@ -60,28 +49,28 @@
     ssm_client_no_cache_two = ssm.get_ssm_client("ca-central-1", enable_cache=EnableCache.NO)
 
     assert ssm_client_no_cache_one != ssm_client_no_cache_two
     assert ssm_client_cached_one != ssm_client_no_cache_one
     assert ssm_client_cached_one != ssm_client_no_cache_two
 
 
-@mock_ssm
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_get_parameter():
     reload(ssm)
 
     ssm_client = boto3.client("ssm")
     ssm_client.put_parameter(Name="some_key", Type="String", Value="some value")
 
     result = ssm.get_parameter("some_key")
 
     assert result == "some value"
 
 
-@mock_ssm
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_get_parameter_decrypted():
     reload(ssm)
 
     ssm_client = boto3.client("ssm")
     ssm_client.put_parameter(Name="some_key", Type="String", Value="some value")
```

### Comparing `skymantle_boto_buddy-0.2.0/tests/test_stepfunctions.py` & `skymantle_boto_buddy-0.3.0/tests/test_stepfunctions.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,16 +2,15 @@
 import os
 from importlib import reload
 from unittest.mock import ANY, MagicMock, call
 
 import boto3
 import pytest
 from boto3 import Session
-from botocore.exceptions import NoRegionError
-from moto import mock_stepfunctions
+from moto import mock_aws
 from pytest_mock import MockerFixture
 
 from skymantle_boto_buddy import EnableCache, stepfunctions
 
 simple_definition = (
     '{"Comment": "An example of the Amazon States Language using a choice state.",'
     '"StartAt": "DefaultState",'
@@ -24,43 +23,33 @@
 def environment(mocker: MockerFixture):
     return mocker.patch.dict(
         os.environ,
         {"AWS_DEFAULT_REGION": "ca-central-1", "AWS_LAMBDA_FUNCTION_NAME": "Test_Lambda_Function"},
     )
 
 
-@mock_stepfunctions
-def test_no_default_region():
-    reload(stepfunctions)
-
-    with pytest.raises(NoRegionError) as e:
-        stepfunctions.describe_execution("some_arn")
-
-    assert str(e.value) == "You must specify a region."
-
-
-@mock_stepfunctions
+@mock_aws
 def test_manual_region():
     reload(stepfunctions)
 
     client = stepfunctions.get_stepfunctions_client("ca-central-1")
 
     assert type(client).__name__ == "SFN"
 
 
-@mock_stepfunctions
+@mock_aws
 def test_manual_session():
     reload(stepfunctions)
 
     client = stepfunctions.get_stepfunctions_client("ca-central-1", Session())
 
     assert type(client).__name__ == "SFN"
 
 
-@mock_stepfunctions
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_stepfunctions_client_cache():
     reload(stepfunctions)
 
     stepfunctions_client_cached_one = stepfunctions.get_stepfunctions_client(enable_cache=EnableCache.YES)
     stepfunctions_client_cached_two = stepfunctions.get_stepfunctions_client(enable_cache=EnableCache.YES)
 
@@ -70,58 +59,59 @@
     stepfunctions_client_no_cache_two = stepfunctions.get_stepfunctions_client(enable_cache=EnableCache.NO)
 
     assert stepfunctions_client_no_cache_one != stepfunctions_client_no_cache_two
     assert stepfunctions_client_cached_one != stepfunctions_client_no_cache_one
     assert stepfunctions_client_cached_one != stepfunctions_client_no_cache_two
 
 
-@mock_stepfunctions
+@mock_aws
 @pytest.mark.usefixtures("environment")
-def test_start_exection():
+def test_start_execution():
     reload(stepfunctions)
 
     client = boto3.client("stepfunctions")
 
     sm = client.create_state_machine(
         name="name", definition=str(simple_definition), roleArn="arn:aws:iam::123456789012:role/a_role"
     )
 
     execution = stepfunctions.start_execution(sm["stateMachineArn"], {"some": "data"})
 
     assert "arn:aws:states:ca-central-1:123456789012:execution:name" in execution["executionArn"]
 
 
-@mock_stepfunctions
+@mock_aws
 @pytest.mark.usefixtures("environment")
-def test_describe_exection():
+def test_describe_execution():
     reload(stepfunctions)
 
     client = boto3.client("stepfunctions")
 
     sm = client.create_state_machine(
         name="name", definition=str(simple_definition), roleArn="arn:aws:iam::123456789012:role/a_role"
     )
 
     execution = client.start_execution(stateMachineArn=sm["stateMachineArn"], input=json.dumps({"some": "data"}))
 
     response = stepfunctions.describe_execution(execution["executionArn"])
 
     assert response["ResponseMetadata"]["HTTPStatusCode"] == 200
     assert response["executionArn"] == execution["executionArn"]
-    assert response["input"] == json.dumps({"some": "data"})
+    # ! Need to look into why the input requires two json.loads
+    assert json.loads(json.loads(response["input"])) == {"some": "data"}
     assert response["status"] == "RUNNING"
 
 
 @pytest.fixture()
 def mock_time(mocker: MockerFixture) -> MagicMock:
     mock = mocker.patch("skymantle_boto_buddy.stepfunctions.time")
     return mock
 
 
-@mock_stepfunctions
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_start_with_wait_for_completion(mock_time):
     # reload(stepfunctions)
 
     client = boto3.client("stepfunctions")
 
     sm = client.create_state_machine(
@@ -130,19 +120,20 @@
 
     response = stepfunctions.start_with_wait_for_completion(sm["stateMachineArn"], {"some": "data"})
 
     mock_time.sleep.assert_has_calls([call(1), call(1), call(1), call(1), call(1)])
     assert mock_time.sleep.call_count == 5
 
     assert response["ResponseMetadata"]["HTTPStatusCode"] == 200
-    assert response["input"] == json.dumps({"some": "data"})
+    # ! Need to look into why the input requires two json.loads
+    assert json.loads(json.loads(response["input"])) == {"some": "data"}
     assert response["status"] == "RUNNING"
 
 
-@mock_stepfunctions
+@mock_aws
 @pytest.mark.usefixtures("environment")
 def test_start_with_wait_for_completion_failure(mock_time):
     os.environ["SF_EXECUTION_HISTORY_TYPE"] = "FAILURE"
 
     client = boto3.client("stepfunctions")
 
     sm = client.create_state_machine(
@@ -150,26 +141,27 @@
     )
 
     response = stepfunctions.start_with_wait_for_completion(sm["stateMachineArn"], {"some": "data"})
 
     assert mock_time.sleep.call_count == 0
 
     assert response["ResponseMetadata"]["HTTPStatusCode"] == 200
-    assert response["input"] == json.dumps({"some": "data"})
+    # ! Need to look into why the input requires two json.loads
+    assert json.loads(json.loads(response["input"])) == {"some": "data"}
     assert response["status"] == "FAILED"
 
 
 @pytest.fixture()
 def mock_get_boto3_client(mocker: MockerFixture) -> MagicMock:
     mock = mocker.patch("skymantle_boto_buddy.stepfunctions.get_boto3_client", autospec=True)
     return mock
 
 
 @pytest.mark.usefixtures("environment")
-def test_start_sync_exection(mock_get_boto3_client):
+def test_start_sync_execution(mock_get_boto3_client):
     # ! No Moto support for start_sync_execution
     stepfunctions.start_sync_execution("an_arn", {"some": "data"})
 
     mock_get_boto3_client.assert_called_once_with("stepfunctions", None, None, None, ANY)
     mock_get_boto3_client.return_value.start_sync_execution.assert_called_once_with(
         stateMachineArn="an_arn", input=json.dumps({"some": "data"})
     )
```

### Comparing `skymantle_boto_buddy-0.2.0/.gitignore` & `skymantle_boto_buddy-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `skymantle_boto_buddy-0.2.0/LICENSE` & `skymantle_boto_buddy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skymantle_boto_buddy-0.2.0/README.md` & `skymantle_boto_buddy-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+[![Status Checks](https://github.com/skymantle-tech/skymantle-boto-buddy/actions/workflows/status_checks.yml/badge.svg)](https://github.com/skymantle-tech/skymantle-boto-buddy/actions/workflows/status_checks.yml)
+
 # Skymantle Boto Buddy
 
-A wrappper for boto3 to access common aws severless services primarily used for aws Lambda. By default the wrapper is dependent on using boto3 configuration through [environment variables](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html#using-environment-variables) for setting credentials for accessing aws resources. It's also possible to provide a `boto3.Session` object for setting credentials.
+A wrapper for boto3 to access common aws serverless services primarily used for aws Lambda. By default the wrapper is dependent on using boto3 configuration through [environment variables](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html#using-environment-variables) for setting credentials for accessing aws resources. It's also possible to provide a `boto3.Session` object for setting credentials.
 
-When used within the context of an aws lambda function, no creditials are required and instances of boto3 resource and clients are created during lambda initialization when importing helpers. The library determines its running in the context of a lambda function but looking for the `AWS_LAMBDA_FUNCTION_NAME` environment variable.
+When used within the context of an aws lambda function, no credentials are required and instances of boto3 resource and clients are created during lambda initialization when importing helpers. The library determines its running in the context of a lambda function but looking for the `AWS_LAMBDA_FUNCTION_NAME` environment variable.
 
 The boto3 client and resource objects are cached but it is possible to also get uncached instances or cache can be disabled globally by setting the `BOTO_BUDDY_DISABLE_CACHE` environment variable. Supported values are `1`, `true`, `yes` and `on`.
 
 ## Installation
 To install use:
 
 ```
@@ -29,14 +31,15 @@
 - DynamoDb
   - `get_dynamodb_resource`
   - `get_table`
   - `put_item_simplified`
   - `update_item_simplified`
   - `get_item`
   - `delete_item`
+  - `query`
   - `query_no_paging`
 - S3
   - `get_s3_client`
   - `get_s3_resource`
   - `get_bucket`
   - `get_object_signed_url`
   - `put_object_signed_url`
@@ -71,23 +74,23 @@
   - `describe_execution`
 - Logs
   - `get_logs_client`
 
 
 ### Examples
 
-- running inside a lambda function or using environment variable creditional
+- running inside a lambda function or using environment variable credentials
 
 ```python
 from skymantle_boto_buddy import dynamodb
 
 dynamodb.put_item_simplified("table_name", {"PK": "some_key", "Description": "Some description"})
 ```
 
-- providing a Session and specifiying a profile named `developer`
+- providing a Session and specifying a profile named `developer`
 
 ```python
 from boto3 import Session
 from skymantle_boto_buddy import dynamodb
 
 session = Session(profile_name="developer")
 dynamodb.put_item_simplified("table_name", {"PK": "some_key", "Description": "Some description"}, session=session)
@@ -126,17 +129,20 @@
     mock = mocker.patch("my_file.dynamodb")
     return mock
 
 def test_some_function(mock_dynamodb):
     mock_dynamodb.get_item.return_value = {"PK": "some_pk", "Name": "some value"}
 
     result = my_file.some_function()
+    
+    mock_dynamodb.get_item.assert_called_with("table_name", {"PK": "some_key"})
     assert result == {"PK": "some_pk", "Name": "some value"}
 ```
 
 ## Source Code Dev Notes
 
 The following project commands are supported:
-- `make setup` - Installs all dependencies ands creates virtual environment
-- `make unitTests` - runs unit tests
-- `make lintAndAnalysis` - Runs [ruff](https://github.com/astral-sh/ruff), [bandit](https://github.com/PyCQA/bandit) and [black](https://github.com/psf/black)
+- `make clean` - Deletes virtual environment
+- `make install` - Installs all dependencies and creates virtual environment
+- `make unit_tests` - runs unit tests
+- `make lint_and_analysis` - Runs [ruff](https://github.com/astral-sh/ruff), [bandit](https://github.com/PyCQA/bandit) and [black](https://github.com/psf/black)
 - `make build` - Creates distribution
```

### Comparing `skymantle_boto_buddy-0.2.0/pyproject.toml` & `skymantle_boto_buddy-0.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "skymantle_boto_buddy"
-version = "0.2.0"
+version = "0.3.0"
 dependencies=[]
 requires-python = ">=3.11"
 authors = [{ name = "Artin Yong-Bannayan", email = "ayongbannayan@skymantle.com" }]
 description = "A wrappper for boto3 to help access and test usage of common aws services."
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
@@ -18,59 +18,45 @@
   "Programming Language :: Python",
 ]
 
 [project.optional-dependencies]
 boto = ["boto3"]
 
 [project.urls]
-Home = "https://github.com/skymantle-tech/boto3-powertools"
-Issues = "https://github.com/skymantle-tech/boto3-powertools/issues"
+Home = "https://github.com/skymantle-tech/skymantle-boto-buddy"
+Issues = "https://github.com/skymantle-tech/skymantle-boto-buddy/issues"
 
 [tool.hatch.metadata]
 allow-direct-references = true
 
 [tool.hatch.envs.default]
 features = ["boto"]
 dependencies = [
-  "mypy",
   "pytest",
   "pytest-cov",
   "pytest-mock",
   "bandit",
   "black",
   "ruff",
-  "moto[s3,dynamodb,ssm,cloudformation,sts,logs,stepfunction]"
+  "moto[s3,dynamodb,ssm,cloudformation,sts,logs]"
 ]
 path = ".venv"
 
-[tool.hatch.envs.default.scripts]
-_bandit = "bandit -c pyproject.toml -r {args:.}"
-_ruff = "ruff {args:.}"
-_black = "black --check --diff {args:.}"
-_mypy = "mypy --install-types --non-interactive {args:.}"
-cov = "pytest -v --cov-config=pyproject.toml --cov {args:./src} "
-
-[tool.mypy]
-exclude = [
-    "dist",
-    ".venv"
-]
-
 [tool.black]
 line-length = 120
 
 [tool.bandit]
 skips = ['B324']
 exclude_dirs = [".venv", "tests", "dist"]
 
 [tool.ruff]
 exclude = [".venv"]
 target-version = "py311"
 line-length = 120
-select = [
+lint.select = [
   "A",
   "B",
   "C",
   "DTZ",
   "E",
   "EM",
   "F",
@@ -89,31 +75,31 @@
   "SIM",
   "T",
   "TID",
   "UP",
   "W",
   "YTT",
 ]
-ignore = [
+lint.ignore = [
   # Ignore checks for use `datetime.UTC` alias
   "UP017",
   # Ignore checks for f-string literal in exception message
   "EM102",
   # Ignore too many arguments in function definition
   "PLR0913"
 ]
-unfixable = []
+lint.unfixable = []
 
-[tool.ruff.flake8-quotes]
+[tool.ruff.lint.flake8-quotes]
 inline-quotes = "double"
 
-[tool.ruff.flake8-tidy-imports]
+[tool.ruff.lint.flake8-tidy-imports]
 ban-relative-imports = "all"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "I001"]
 
 [tool.coverage.run]
 branch = true
 parallel = true
 source = ["src"]
@@ -133,12 +119,11 @@
 pythonpath = "src"
 markers = []
 
 [tool.hatch.build.targets.sdist]
 support-legacy = true
 exclude = [
   "/.vscode",
-  "/.vscode",
   "/.github",
   ".gitignore",
   "Makefile"
 ]
```

### Comparing `skymantle_boto_buddy-0.2.0/PKG-INFO` & `skymantle_boto_buddy-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: skymantle_boto_buddy
-Version: 0.2.0
+Version: 0.3.0
 Summary: A wrappper for boto3 to help access and test usage of common aws services.
-Project-URL: Home, https://github.com/skymantle-tech/boto3-powertools
-Project-URL: Issues, https://github.com/skymantle-tech/boto3-powertools/issues
+Project-URL: Home, https://github.com/skymantle-tech/skymantle-boto-buddy
+Project-URL: Issues, https://github.com/skymantle-tech/skymantle-boto-buddy/issues
 Author-email: Artin Yong-Bannayan <ayongbannayan@skymantle.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -212,19 +212,21 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Requires-Python: >=3.11
 Provides-Extra: boto
 Requires-Dist: boto3; extra == 'boto'
 Description-Content-Type: text/markdown
 
+[![Status Checks](https://github.com/skymantle-tech/skymantle-boto-buddy/actions/workflows/status_checks.yml/badge.svg)](https://github.com/skymantle-tech/skymantle-boto-buddy/actions/workflows/status_checks.yml)
+
 # Skymantle Boto Buddy
 
-A wrappper for boto3 to access common aws severless services primarily used for aws Lambda. By default the wrapper is dependent on using boto3 configuration through [environment variables](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html#using-environment-variables) for setting credentials for accessing aws resources. It's also possible to provide a `boto3.Session` object for setting credentials.
+A wrapper for boto3 to access common aws serverless services primarily used for aws Lambda. By default the wrapper is dependent on using boto3 configuration through [environment variables](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html#using-environment-variables) for setting credentials for accessing aws resources. It's also possible to provide a `boto3.Session` object for setting credentials.
 
-When used within the context of an aws lambda function, no creditials are required and instances of boto3 resource and clients are created during lambda initialization when importing helpers. The library determines its running in the context of a lambda function but looking for the `AWS_LAMBDA_FUNCTION_NAME` environment variable.
+When used within the context of an aws lambda function, no credentials are required and instances of boto3 resource and clients are created during lambda initialization when importing helpers. The library determines its running in the context of a lambda function but looking for the `AWS_LAMBDA_FUNCTION_NAME` environment variable.
 
 The boto3 client and resource objects are cached but it is possible to also get uncached instances or cache can be disabled globally by setting the `BOTO_BUDDY_DISABLE_CACHE` environment variable. Supported values are `1`, `true`, `yes` and `on`.
 
 ## Installation
 To install use:
 
 ```
@@ -247,14 +249,15 @@
 - DynamoDb
   - `get_dynamodb_resource`
   - `get_table`
   - `put_item_simplified`
   - `update_item_simplified`
   - `get_item`
   - `delete_item`
+  - `query`
   - `query_no_paging`
 - S3
   - `get_s3_client`
   - `get_s3_resource`
   - `get_bucket`
   - `get_object_signed_url`
   - `put_object_signed_url`
@@ -289,23 +292,23 @@
   - `describe_execution`
 - Logs
   - `get_logs_client`
 
 
 ### Examples
 
-- running inside a lambda function or using environment variable creditional
+- running inside a lambda function or using environment variable credentials
 
 ```python
 from skymantle_boto_buddy import dynamodb
 
 dynamodb.put_item_simplified("table_name", {"PK": "some_key", "Description": "Some description"})
 ```
 
-- providing a Session and specifiying a profile named `developer`
+- providing a Session and specifying a profile named `developer`
 
 ```python
 from boto3 import Session
 from skymantle_boto_buddy import dynamodb
 
 session = Session(profile_name="developer")
 dynamodb.put_item_simplified("table_name", {"PK": "some_key", "Description": "Some description"}, session=session)
@@ -344,17 +347,20 @@
     mock = mocker.patch("my_file.dynamodb")
     return mock
 
 def test_some_function(mock_dynamodb):
     mock_dynamodb.get_item.return_value = {"PK": "some_pk", "Name": "some value"}
 
     result = my_file.some_function()
+    
+    mock_dynamodb.get_item.assert_called_with("table_name", {"PK": "some_key"})
     assert result == {"PK": "some_pk", "Name": "some value"}
 ```
 
 ## Source Code Dev Notes
 
 The following project commands are supported:
-- `make setup` - Installs all dependencies ands creates virtual environment
-- `make unitTests` - runs unit tests
-- `make lintAndAnalysis` - Runs [ruff](https://github.com/astral-sh/ruff), [bandit](https://github.com/PyCQA/bandit) and [black](https://github.com/psf/black)
+- `make clean` - Deletes virtual environment
+- `make install` - Installs all dependencies and creates virtual environment
+- `make unit_tests` - runs unit tests
+- `make lint_and_analysis` - Runs [ruff](https://github.com/astral-sh/ruff), [bandit](https://github.com/PyCQA/bandit) and [black](https://github.com/psf/black)
 - `make build` - Creates distribution
```

### Comparing `skymantle_boto_buddy-0.2.0/setup.py` & `skymantle_boto_buddy-0.3.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 setup(
     name='skymantle-boto-buddy',
-    version='0.2.0',
+    version='0.3.0',
     description='A wrappper for boto3 to help access and test usage of common aws services.',
-    long_description='# Skymantle Boto Buddy\n\nA wrappper for boto3 to access common aws severless services primarily used for aws Lambda. By default the wrapper is dependent on using boto3 configuration through [environment variables](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html#using-environment-variables) for setting credentials for accessing aws resources. It\'s also possible to provide a `boto3.Session` object for setting credentials.\n\nWhen used within the context of an aws lambda function, no creditials are required and instances of boto3 resource and clients are created during lambda initialization when importing helpers. The library determines its running in the context of a lambda function but looking for the `AWS_LAMBDA_FUNCTION_NAME` environment variable.\n\nThe boto3 client and resource objects are cached but it is possible to also get uncached instances or cache can be disabled globally by setting the `BOTO_BUDDY_DISABLE_CACHE` environment variable. Supported values are `1`, `true`, `yes` and `on`.\n\n## Installation\nTo install use:\n\n```\npip3 install skymantle_boto_buddy\n```\n\nUsing `skymantle_boto_buddy` will not include the boto3 dependency, useful when part of a lambda function and the lambda runtime version or a layer is used.  To include boto3 use:\n\n```\npip3 install skymantle_boto_buddy[boto3]\n```\n\n## Usage\n\nThe library provides the following functions.\n\n- Package\n  - `get_boto3_client`\n  - `get_boto3_resource`\n- DynamoDb\n  - `get_dynamodb_resource`\n  - `get_table`\n  - `put_item_simplified`\n  - `update_item_simplified`\n  - `get_item`\n  - `delete_item`\n  - `query_no_paging`\n- S3\n  - `get_s3_client`\n  - `get_s3_resource`\n  - `get_bucket`\n  - `get_object_signed_url`\n  - `put_object_signed_url`\n  - `get_object`\n  - `get_object_bytes`\n  - `get_object_json`\n  - `get_object_csv_reader`\n  - `upload_fileobj`\n  - `put_object`\n  - `delete_object`\n  - `delete_objects`\n  - `copy`\n  - `list_objects_v2`\n  - `execute_sql_query_simplified`\n- SSM\n  - `get_ssm_client`\n  - `get_parameter`\n  - `get_parameter_decrypted`\n- CloudFormation\n  - `get_cloudformation_client`\n  - `describe_stacks`\n  - `get_stack_outputs`\n- STS\n  - `get_sts_client`\n  - `get_caller_identity`\n  - `get_caller_account`\n- StepFunction\n  - `get_stepfunction_client`\n  - `start_execution`\n  - `start_sync_execution`\n  - `start_with_wait_for_completion`\n  - `describe_execution`\n- Logs\n  - `get_logs_client`\n\n\n### Examples\n\n- running inside a lambda function or using environment variable creditional\n\n```python\nfrom skymantle_boto_buddy import dynamodb\n\ndynamodb.put_item_simplified("table_name", {"PK": "some_key", "Description": "Some description"})\n```\n\n- providing a Session and specifiying a profile named `developer`\n\n```python\nfrom boto3 import Session\nfrom skymantle_boto_buddy import dynamodb\n\nsession = Session(profile_name="developer")\ndynamodb.put_item_simplified("table_name", {"PK": "some_key", "Description": "Some description"}, session=session)\n```\n\n- Get a version of the s3 client that is not cached\n\n```python\nfrom boto3 import Session\nfrom skymantle_boto_buddy import EnableCache, s3\n\ns3_client = get_s3_client(enable_cache=EnableCache.NO)\n```\n\n- unit test a function with patching (also possible to use packages like [moto](https://github.com/getmoto/moto))\n\n```python\n# my_file.py\nfrom skymantle_boto_buddy import dynamodb\n\ndef some_function():\n  # ...\n  item = dynamodb.get_item("table_name", {"PK": "some_key"})\n  \n  return item\n\n\n# my_test.py\nfrom unittest.mock import MagicMock\nimport pytest\nfrom pytest_mock import MockerFixture\nimport my_file\n\n@pytest.fixture()\ndef mock_dynamodb(mocker: MockerFixture) -> MagicMock:\n    mock = mocker.patch("my_file.dynamodb")\n    return mock\n\ndef test_some_function(mock_dynamodb):\n    mock_dynamodb.get_item.return_value = {"PK": "some_pk", "Name": "some value"}\n\n    result = my_file.some_function()\n    assert result == {"PK": "some_pk", "Name": "some value"}\n```\n\n## Source Code Dev Notes\n\nThe following project commands are supported:\n- `make setup` - Installs all dependencies ands creates virtual environment\n- `make unitTests` - runs unit tests\n- `make lintAndAnalysis` - Runs [ruff](https://github.com/astral-sh/ruff), [bandit](https://github.com/PyCQA/bandit) and [black](https://github.com/psf/black)\n- `make build` - Creates distribution',
+    long_description='[![Status Checks](https://github.com/skymantle-tech/skymantle-boto-buddy/actions/workflows/status_checks.yml/badge.svg)](https://github.com/skymantle-tech/skymantle-boto-buddy/actions/workflows/status_checks.yml)\n\n# Skymantle Boto Buddy\n\nA wrapper for boto3 to access common aws serverless services primarily used for aws Lambda. By default the wrapper is dependent on using boto3 configuration through [environment variables](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/configuration.html#using-environment-variables) for setting credentials for accessing aws resources. It\'s also possible to provide a `boto3.Session` object for setting credentials.\n\nWhen used within the context of an aws lambda function, no credentials are required and instances of boto3 resource and clients are created during lambda initialization when importing helpers. The library determines its running in the context of a lambda function but looking for the `AWS_LAMBDA_FUNCTION_NAME` environment variable.\n\nThe boto3 client and resource objects are cached but it is possible to also get uncached instances or cache can be disabled globally by setting the `BOTO_BUDDY_DISABLE_CACHE` environment variable. Supported values are `1`, `true`, `yes` and `on`.\n\n## Installation\nTo install use:\n\n```\npip3 install skymantle_boto_buddy\n```\n\nUsing `skymantle_boto_buddy` will not include the boto3 dependency, useful when part of a lambda function and the lambda runtime version or a layer is used.  To include boto3 use:\n\n```\npip3 install skymantle_boto_buddy[boto3]\n```\n\n## Usage\n\nThe library provides the following functions.\n\n- Package\n  - `get_boto3_client`\n  - `get_boto3_resource`\n- DynamoDb\n  - `get_dynamodb_resource`\n  - `get_table`\n  - `put_item_simplified`\n  - `update_item_simplified`\n  - `get_item`\n  - `delete_item`\n  - `query`\n  - `query_no_paging`\n- S3\n  - `get_s3_client`\n  - `get_s3_resource`\n  - `get_bucket`\n  - `get_object_signed_url`\n  - `put_object_signed_url`\n  - `get_object`\n  - `get_object_bytes`\n  - `get_object_json`\n  - `get_object_csv_reader`\n  - `upload_fileobj`\n  - `put_object`\n  - `delete_object`\n  - `delete_objects`\n  - `copy`\n  - `list_objects_v2`\n  - `execute_sql_query_simplified`\n- SSM\n  - `get_ssm_client`\n  - `get_parameter`\n  - `get_parameter_decrypted`\n- CloudFormation\n  - `get_cloudformation_client`\n  - `describe_stacks`\n  - `get_stack_outputs`\n- STS\n  - `get_sts_client`\n  - `get_caller_identity`\n  - `get_caller_account`\n- StepFunction\n  - `get_stepfunction_client`\n  - `start_execution`\n  - `start_sync_execution`\n  - `start_with_wait_for_completion`\n  - `describe_execution`\n- Logs\n  - `get_logs_client`\n\n\n### Examples\n\n- running inside a lambda function or using environment variable credentials\n\n```python\nfrom skymantle_boto_buddy import dynamodb\n\ndynamodb.put_item_simplified("table_name", {"PK": "some_key", "Description": "Some description"})\n```\n\n- providing a Session and specifying a profile named `developer`\n\n```python\nfrom boto3 import Session\nfrom skymantle_boto_buddy import dynamodb\n\nsession = Session(profile_name="developer")\ndynamodb.put_item_simplified("table_name", {"PK": "some_key", "Description": "Some description"}, session=session)\n```\n\n- Get a version of the s3 client that is not cached\n\n```python\nfrom boto3 import Session\nfrom skymantle_boto_buddy import EnableCache, s3\n\ns3_client = get_s3_client(enable_cache=EnableCache.NO)\n```\n\n- unit test a function with patching (also possible to use packages like [moto](https://github.com/getmoto/moto))\n\n```python\n# my_file.py\nfrom skymantle_boto_buddy import dynamodb\n\ndef some_function():\n  # ...\n  item = dynamodb.get_item("table_name", {"PK": "some_key"})\n  \n  return item\n\n\n# my_test.py\nfrom unittest.mock import MagicMock\nimport pytest\nfrom pytest_mock import MockerFixture\nimport my_file\n\n@pytest.fixture()\ndef mock_dynamodb(mocker: MockerFixture) -> MagicMock:\n    mock = mocker.patch("my_file.dynamodb")\n    return mock\n\ndef test_some_function(mock_dynamodb):\n    mock_dynamodb.get_item.return_value = {"PK": "some_pk", "Name": "some value"}\n\n    result = my_file.some_function()\n    \n    mock_dynamodb.get_item.assert_called_with("table_name", {"PK": "some_key"})\n    assert result == {"PK": "some_pk", "Name": "some value"}\n```\n\n## Source Code Dev Notes\n\nThe following project commands are supported:\n- `make clean` - Deletes virtual environment\n- `make install` - Installs all dependencies and creates virtual environment\n- `make unit_tests` - runs unit tests\n- `make lint_and_analysis` - Runs [ruff](https://github.com/astral-sh/ruff), [bandit](https://github.com/PyCQA/bandit) and [black](https://github.com/psf/black)\n- `make build` - Creates distribution',
     author_email='Artin Yong-Bannayan <ayongbannayan@skymantle.com>',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: Apache Software License',
         'Programming Language :: Python',
     ],
```

