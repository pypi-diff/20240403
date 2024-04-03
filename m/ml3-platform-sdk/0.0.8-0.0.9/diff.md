# Comparing `tmp/ml3_platform_sdk-0.0.8.tar.gz` & `tmp/ml3_platform_sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml3_platform_sdk-0.0.8.tar", max compression
+gzip compressed data, was "ml3_platform_sdk-0.0.9.tar", max compression
```

## Comparing `ml3_platform_sdk-0.0.8.tar` & `ml3_platform_sdk-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      176 2023-11-23 11:45:36.773067 ml3_platform_sdk-0.0.8/README.md
--rw-r--r--   0        0        0       22 2023-11-23 11:45:36.773067 ml3_platform_sdk-0.0.8/ml3_platform_sdk/__init__.py
--rw-r--r--   0        0        0    55017 2023-11-23 11:45:36.773067 ml3_platform_sdk-0.0.8/ml3_platform_sdk/client.py
--rw-r--r--   0        0        0        0 2023-11-23 11:45:36.773067 ml3_platform_sdk-0.0.8/ml3_platform_sdk/core/__init__.py
--rw-r--r--   0        0        0    87555 2023-11-23 11:45:36.777067 ml3_platform_sdk-0.0.8/ml3_platform_sdk/core/client_impl.py
--rw-r--r--   0        0        0     1355 2023-11-23 11:45:36.777067 ml3_platform_sdk-0.0.8/ml3_platform_sdk/core/connection.py
--rw-r--r--   0        0        0      576 2023-11-23 11:45:36.777067 ml3_platform_sdk-0.0.8/ml3_platform_sdk/core/enums.py
--rw-r--r--   0        0        0    10044 2023-11-23 11:45:36.777067 ml3_platform_sdk-0.0.8/ml3_platform_sdk/core/requests.py
--rw-r--r--   0        0        0      330 2023-11-23 11:45:36.777067 ml3_platform_sdk-0.0.8/ml3_platform_sdk/core/responses.py
--rw-r--r--   0        0        0      534 2023-11-23 11:45:36.777067 ml3_platform_sdk-0.0.8/ml3_platform_sdk/core/singleton.py
--rw-r--r--   0        0        0     4412 2023-11-23 11:45:36.777067 ml3_platform_sdk-0.0.8/ml3_platform_sdk/enums.py
--rw-r--r--   0        0        0     2560 2023-11-23 11:45:36.777067 ml3_platform_sdk-0.0.8/ml3_platform_sdk/exceptions.py
--rw-r--r--   0        0        0    12767 2023-11-23 11:45:36.777067 ml3_platform_sdk-0.0.8/ml3_platform_sdk/models.py
--rw-r--r--   0        0        0      496 2023-11-23 11:45:36.777067 ml3_platform_sdk-0.0.8/ml3_platform_sdk/utils.py
--rw-r--r--   0        0        0     1450 2023-11-23 11:45:36.781067 ml3_platform_sdk-0.0.8/pyproject.toml
--rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 ml3_platform_sdk-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      176 2024-01-18 10:46:23.046512 ml3_platform_sdk-0.0.9/README.md
+-rw-r--r--   0        0        0       22 2024-01-18 10:46:23.046512 ml3_platform_sdk-0.0.9/ml3_platform_sdk/__init__.py
+-rw-r--r--   0        0        0    58437 2024-01-18 10:46:23.046512 ml3_platform_sdk-0.0.9/ml3_platform_sdk/client.py
+-rw-r--r--   0        0        0        0 2024-01-18 10:46:23.046512 ml3_platform_sdk-0.0.9/ml3_platform_sdk/core/__init__.py
+-rw-r--r--   0        0        0    89752 2024-01-18 10:46:23.046512 ml3_platform_sdk-0.0.9/ml3_platform_sdk/core/client_impl.py
+-rw-r--r--   0        0        0     1355 2024-01-18 10:46:23.046512 ml3_platform_sdk-0.0.9/ml3_platform_sdk/core/connection.py
+-rw-r--r--   0        0        0      576 2024-01-18 10:46:23.046512 ml3_platform_sdk-0.0.9/ml3_platform_sdk/core/enums.py
+-rw-r--r--   0        0        0    10581 2024-01-18 10:46:23.046512 ml3_platform_sdk-0.0.9/ml3_platform_sdk/core/requests.py
+-rw-r--r--   0        0        0      330 2024-01-18 10:46:23.050512 ml3_platform_sdk-0.0.9/ml3_platform_sdk/core/responses.py
+-rw-r--r--   0        0        0      534 2024-01-18 10:46:23.050512 ml3_platform_sdk-0.0.9/ml3_platform_sdk/core/singleton.py
+-rw-r--r--   0        0        0     5707 2024-01-18 10:46:23.050512 ml3_platform_sdk-0.0.9/ml3_platform_sdk/enums.py
+-rw-r--r--   0        0        0     2762 2024-01-18 10:46:23.050512 ml3_platform_sdk-0.0.9/ml3_platform_sdk/exceptions.py
+-rw-r--r--   0        0        0    15548 2024-01-18 10:46:23.050512 ml3_platform_sdk-0.0.9/ml3_platform_sdk/models.py
+-rw-r--r--   0        0        0      496 2024-01-18 10:46:23.050512 ml3_platform_sdk-0.0.9/ml3_platform_sdk/utils.py
+-rw-r--r--   0        0        0     1450 2024-01-18 10:46:23.054513 ml3_platform_sdk-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 ml3_platform_sdk-0.0.9/PKG-INFO
```

### Comparing `ml3_platform_sdk-0.0.8/ml3_platform_sdk/client.py` & `ml3_platform_sdk-0.0.9/ml3_platform_sdk/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     ApiKeyExpirationTime,
     DetectionEventSeverity,
     DetectionEventType,
     JobStatus,
     ModelMetricName,
     MonitoringTarget,
     StoragePolicy,
+    SuggestionType,
     TaskType,
     UserCompanyRole,
     UserProjectRole,
 )
 from ml3_platform_sdk.models import (
     KPI,
     ApiKey,
@@ -28,16 +29,17 @@
     Job,
     Model,
     PredictionDataSourceInfo,
     Project,
     RetrainingReport,
     RetrainTrigger,
     SecretAWSCredentials,
-    Suggestion,
+    SuggestionInfo,
     Task,
+    TaskCostInfo,
 )
 
 
 class ML3PlatformClient(ML3PlatformClientImpl):
     """
     Client class is the single point of interaction with ML cube
     Platform APIs, it is initialized providing the `url` and the User
@@ -246,15 +248,20 @@
             ------------------------  ----------
             6475f8c9ebac5081e529s63f  my project
             ```
         """
         super().show_projects()
 
     def create_task(
-        self, project_id: str, name: str, tags: List[str], task_type: TaskType
+        self,
+        project_id: str,
+        name: str,
+        tags: List[str],
+        task_type: TaskType,
+        cost_info: Optional[TaskCostInfo] = None,
     ) -> str:
         """
         Create a task inside the project.
 
         **Allowed Roles:**
 
             - At least `PROJECT_EDIT` for that project
@@ -262,23 +269,64 @@
             - `COMPANY_ADMIN`
         Args:
             project_id: the identifier of the project
             name: the name of the task
             tags: a list of tags associated with the task
             task_type: the type of the task. See `TaskType`
                 documentation for more information
+            cost_info: optional argument that specify the cost
+                information of the task
 
         Returns:
             task_id: `str`
 
         Raises:
             `CreateTaskException`
         """
         return super().create_task(
-            project_id=project_id, name=name, tags=tags, task_type=task_type
+            project_id=project_id,
+            name=name,
+            tags=tags,
+            task_type=task_type,
+            cost_info=cost_info,
+        )
+
+    def update_task(
+        self,
+        task_id: str,
+        name: Optional[str] = None,
+        tags: Optional[List[str]] = None,
+        cost_info: Optional[TaskCostInfo] = None,
+    ):
+        """
+        Update task attributes.
+
+        `None` parameters are ignored for the update.
+
+        **Allowed Roles:**
+
+            - At least `PROJECT_EDIT` for that project
+            - `COMPANY_OWNER`
+            - `COMPANY_ADMIN`
+        Args:
+            task_id: the identifier of the task
+            name: the name of the task
+            tags: a list of tags associated with the task. To remove
+                all the tags then pass an empty list.
+            cost_info: optional argument that specify the cost
+                information of the task
+
+        Raises:
+            `UpdateTaskException`
+        """
+        super().update_task(
+            task_id=task_id,
+            name=name,
+            tags=tags,
+            cost_info=cost_info,
         )
 
     def get_tasks(self, project_id: str) -> List[Task]:
         """
         Get the list of the Tasks inside the project.
 
         Args:
@@ -333,14 +381,17 @@
 
     def create_model(
         self,
         task_id: str,
         name: str,
         version: str,
         metric_name: ModelMetricName,
+        preferred_suggestion_type: SuggestionType,
+        retraining_cost: float = 0.0,
+        resampled_dataset_size: Optional[int] = None,
     ) -> str:
         """
         Create a model inside the task.
 
         **Allowed Roles:**
 
             - At least `PROJECT_EDIT` for that project
@@ -349,26 +400,40 @@
 
         Args:
             task_id: the identifier of the task
             name: the name of the model
             version: the current version of the model
             metric_name: performance or error metric associated with
                 the model
+            retraining_cost: estimated costs in the Task currency to
+                retrain the model. This information is used by the
+                retraining tool to show gain-cost information.
+                Default value is 0.0 meaning that the cost is negligible
+            preferred_suggestion_type: preferred type of suggestion that
+                will be computed to retrain the model
+            resampled_dataset_size: size of the resampled dataset that
+                will be proposed to retrain the model
+                note: this parameter is required if
+                `preferred_suggestion_type` is
+                `SuggestionType.RESAMPLED_DATASET`
 
         Returns:
             model_id: `str` identifier of the created model
 
         Raises:
             `CreateModelException`
         """
         return super().create_model(
             task_id=task_id,
             name=name,
             version=version,
             metric_name=metric_name,
+            retraining_cost=retraining_cost,
+            preferred_suggestion_type=preferred_suggestion_type,
+            resampled_dataset_size=resampled_dataset_size,
         )
 
     def get_models(self, task_id: str) -> List[Model]:
         """
         Get all models of a task.
 
         **Allowed Roles:**
@@ -459,38 +524,38 @@
         Model Id                  Task Id                   Name                    Version    Status           Status start timestamp    Status insert date          Metric Name
         ------------------------  ------------------------  ----------------------  ---------  ---------------  ------------------------  --------------------------  --------------------
         64fecf7d323311ab78f17280  64fecf7c323311ab78f17262  model_local_experiment  v0.0.1     not_initialized                            2023-09-11 08:27:41.431000  ModelMetricName.RMSE
         ```
         """
         super().show_models(task_id=task_id)
 
-    def get_suggestions(
+    def get_suggestions_info(
         self, model_id: str, model_version: str
-    ) -> List[Suggestion]:
+    ) -> List[SuggestionInfo]:
         """
         Retrieve suggestions associated with a model.
 
         **Allowed Roles:**
 
             - At least `PROJECT_VIEW` for that project
             - `COMPANY_OWNER`
             - `COMPANY_ADMIN`
 
         Args:
             model_id: the identifier of the model
             model_version: the version of the model
 
         Returns:
-            suggestion_list: `List[Suggestion]`
+            suggestion_info_list: `List[SuggestionInfo]`
 
         Raises:
             `SDKClientException`
         """
 
-        return super().get_suggestions(
+        return super().get_suggestions_info(
             model_id=model_id, model_version=model_version
         )
 
     def show_suggestions(self, model_id: str, model_version: str) -> None:
         """
         Show the list of suggestions associated with a
         model printing them to stdout.
@@ -515,24 +580,58 @@
         Raises:
             `SDKClientException`
         """
         super().show_suggestions(
             model_id=model_id, model_version=model_version
         )
 
+    def set_model_suggestion_type(
+        self,
+        model_id: str,
+        preferred_suggestion_type: SuggestionType,
+        resampled_dataset_size: Optional[int] = None,
+    ):
+        """
+        Set model suggestion type.
+
+        **Allowed Roles:**
+
+            - At least `PROJECT_EDIT` for that project
+            - `COMPANY_OWNER`
+            - `COMPANY_ADMIN`
+
+        Args:
+            model_id: the identifier of the task
+            preferred_suggestion_type: preferred type of suggestion that
+                will be computed to retrain the model
+            resampled_dateset_size: size of the resampled dataset that
+                will be proposed to retrain the model
+                note: this parameter is required if
+                `preferred_suggestion_type` is
+                `SuggestionType.RESAMPLED_DATASET`
+
+        Raises:
+            `SetModelSuggestionTypeException`
+        """
+        return super().set_model_suggestion_type(
+            model_id=model_id,
+            preferred_suggestion_type=preferred_suggestion_type,
+            resampled_dataset_size=resampled_dataset_size,
+        )
+
     def update_model_version_by_suggestion_id(
         self,
         model_id: str,
         new_model_version: str,
         suggestion_id: str,
     ) -> str:
         """
         Update model version by suggestion id.
         To retrain the Model, ML cube Platform provides importance
-        weights through a `Suggestion`.
+        weights through a `SuggestionInfo`.
         After the retraining is completed, you use this method to
         create the new model version in ML cube Platform.
         By specifying the `suggestion_id`, ML cube Platform
         automatically knows which is the reference data the model is
         trained on.
 
         This request starts an operation pipeline that is
@@ -571,15 +670,15 @@
         new_model_version: str,
         features_data_source: DataSource,
         targets_data_source: DataSource,
     ) -> str:
         """
         Update model version by suggestion id.
         To retrain the Model, ML cube Platform provides importance
-        weights through a `Suggestion`.
+        weights through a `SuggestionInfo`.
         However, it is possible to train the model with new data that
         has been not already upload to ML cube Platform.
         After the retraining is completed, you use this method to
         create the new model version in ML cube Platform by
         specifying the data to load.
 
         This request starts an operation pipeline that is
```

### Comparing `ml3_platform_sdk-0.0.8/ml3_platform_sdk/core/client_impl.py` & `ml3_platform_sdk-0.0.9/ml3_platform_sdk/core/client_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 # In pydantic v1, parse_raw_as was in the top level module
 # In pydantic v2, parse_raw_as was moved to submodule v1
 try:
     from pydantic.v1 import parse_raw_as
 except ImportError:
     from pydantic import parse_raw_as  # type: ignore
+
 from requests import Response
 from tabulate import tabulate
 
 from ml3_platform_sdk.core.connection import Connection
 from ml3_platform_sdk.core.enums import (
     DataCategory,
     HTTPMethod,
@@ -62,21 +63,23 @@
     GetPresignedUrlRequest,
     GetRetrainingReportRequest,
     GetSuggestionsRequest,
     GetTaskRequest,
     GetTasksRequest,
     GetUserApiRequest,
     RetrainModelRequest,
+    SetModelSuggestionTypeRequest,
     TestRetrainTriggerRequest,
     UpdateCompanyRequest,
     UpdateDetectionEventRuleRequest,
     UpdateModelVersionBySuggestionIDRequest,
     UpdateModelVersionFromRawDataRequest,
     UpdateModelVersionFromRemoteRawDataRequest,
     UpdateProjectRequest,
+    UpdateTaskRequest,
 )
 from ml3_platform_sdk.core.responses import (
     GetPresignedUrlResponse,
     StandardErrorResponse,
 )
 from ml3_platform_sdk.enums import (
     ApiKeyExpirationTime,
@@ -86,14 +89,15 @@
     ExternalIntegration,
     FileType,
     JobStatus,
     ModelMetricName,
     MonitoringTarget,
     StoragePolicy,
     StoringDataType,
+    SuggestionType,
     TaskType,
     UserCompanyRole,
     UserProjectRole,
 )
 from ml3_platform_sdk.exceptions import (
     AddDataSchemaException,
     AddHistoricalDataException,
@@ -109,18 +113,20 @@
     CreateTaskException,
     GetRetrainingReportException,
     InvalidActionList,
     JobFailureException,
     JobNotFoundException,
     JobWaitTimeoutException,
     SDKClientException,
+    SetModelSuggestionTypeException,
     UpdateCompanyException,
     UpdateDetectionEventRuleException,
     UpdateModelVersionException,
     UpdateProjectException,
+    UpdateTaskException,
 )
 from ml3_platform_sdk.models import (
     KPI,
     ApiKey,
     AWSCredentials,
     AzureBlobDataSource,
     AzureCredentials,
@@ -140,16 +146,17 @@
     Project,
     RemoteDataSource,
     RetrainAction,
     RetrainingReport,
     RetrainTrigger,
     S3DataSource,
     SecretAWSCredentials,
-    Suggestion,
+    SuggestionInfo,
     Task,
+    TaskCostInfo,
 )
 from ml3_platform_sdk.utils import read_csv_file
 
 STANDARD_TIMEOUT = 60
 
 logger = logging.getLogger("ML3_PLATFORM_SDK")
 logging.basicConfig(level=logging.INFO)
@@ -503,35 +510,70 @@
         show_projects implementation
         """
         projects = self.get_projects()
 
         self._print_table(items=projects, headers=['Project Id', 'Name'])
 
     def create_task(
-        self, project_id: str, name: str, tags: List[str], task_type: TaskType
+        self,
+        project_id: str,
+        name: str,
+        tags: List[str],
+        task_type: TaskType,
+        cost_info: Optional[TaskCostInfo] = None,
     ) -> str:
         """
         create_task implementation
         """
         payload = CreateTaskRequest(
-            project_id=project_id, name=name, tags=tags, task_type=task_type
+            project_id=project_id,
+            name=name,
+            tags=tags,
+            task_type=task_type,
+            cost_info=cost_info,
         )
 
         response = self._api_call(
             method=HTTPMethod.POST,
             path='/task',
             json_payload=payload.json(),
         )
 
         if response.status_code != 200:
             self._default_exception_handler(
                 response=response, exception_type=CreateTaskException
             )
         return response.json()
 
+    def update_task(
+        self,
+        task_id: str,
+        name: Optional[str] = None,
+        tags: Optional[List[str]] = None,
+        cost_info: Optional[TaskCostInfo] = None,
+    ):
+        """
+        Update task attributes.
+        """
+        payload = UpdateTaskRequest(
+            task_id=task_id,
+            name=name,
+            tags=tags,
+            cost_info=cost_info,
+        )
+
+        response = self._api_call(
+            method=HTTPMethod.PATCH,
+            path='/task',
+            json_payload=payload.json(),
+        )
+
+        if response.status_code != 200:
+            self._default_exception_handler(response, UpdateTaskException)
+
     def get_tasks(self, project_id: str) -> List[Task]:
         """
         get_tasks implementation
         """
         payload = GetTasksRequest(project_id=project_id)
 
         response = self._api_call(
@@ -569,38 +611,72 @@
 
     def create_model(
         self,
         task_id: str,
         name: str,
         version: str,
         metric_name: ModelMetricName,
+        preferred_suggestion_type: SuggestionType,
+        retraining_cost: float = 0.0,
+        resampled_dataset_size: Optional[int] = None,
     ) -> str:
         """
         create_model implementation
         """
 
         payload: CreateModelRequest = CreateModelRequest(
             task_id=task_id,
             name=name,
             version=version,
             metric_name=metric_name.value,
+            retraining_cost=retraining_cost,
+            preferred_suggestion_type=preferred_suggestion_type.value,
+            resampled_dataset_size=resampled_dataset_size,
         )
 
         response = self._api_call(
             method=HTTPMethod.POST,
             path='/model',
             json_payload=payload.json(),
         )
 
         if response.status_code != 200:
             self._default_exception_handler(
                 response=response, exception_type=CreateModelException
             )
         return response.json()
 
+    def set_model_suggestion_type(
+        self,
+        model_id: str,
+        preferred_suggestion_type: SuggestionType,
+        resampled_dataset_size: Optional[int] = None,
+    ):
+        """
+        update_model_info implementation
+        """
+
+        payload: SetModelSuggestionTypeRequest = SetModelSuggestionTypeRequest(
+            model_id=model_id,
+            preferred_suggestion_type=preferred_suggestion_type.value,
+            resampled_dataset_size=resampled_dataset_size,
+        )
+
+        response = self._api_call(
+            method=HTTPMethod.PUT,
+            path='/model/suggestion-type',
+            json_payload=payload.json(),
+        )
+
+        if response.status_code != 200:
+            self._default_exception_handler(
+                response=response,
+                exception_type=SetModelSuggestionTypeException,
+            )
+
     def get_models(self, task_id: str) -> List[Model]:
         """
         get_models implementation
         """
         payload = GetModelsRequest(task_id=task_id)
 
         response = self._api_call(
@@ -862,46 +938,46 @@
                 'Status',
                 'Status start timestamp',
                 'Status insert date',
                 'Metric Name',
             ],
         )
 
-    def get_suggestions(
+    def get_suggestions_info(
         self, model_id: str, model_version: str
-    ) -> List[Suggestion]:
+    ) -> List[SuggestionInfo]:
         """
-        get_suggestions implementation
+        get_suggestions_info implementation
         """
         payload = GetSuggestionsRequest(
             model_id=model_id, model_version=model_version
         )
 
         response = self._api_call(
             method=HTTPMethod.GET,
             path=f'/suggestions/{payload.model_id}/{payload.model_version}',
         )
 
         if response.status_code == 200:
-            return parse_raw_as(List[Suggestion], response.content)
+            return parse_raw_as(List[SuggestionInfo], response.content)
         raise SDKClientException()
 
     def show_suggestions(self, model_id: str, model_version: str) -> None:
         """
         show_suggestions implementation
         """
 
-        suggestions = self.get_suggestions(
+        suggestions = self.get_suggestions_info(
             model_id=model_id, model_version=model_version
         )
 
         self._print_table(
             suggestions,
             [
-                'Suggestion Id',
+                'SuggestionInfo Id',
                 'Executed',
                 'Timestamp',
             ],
         )
 
     # TODO controllare validazione DataSchema
     def add_data_schema(self, task_id: str, data_schema: DataSchema) -> None:
```

### Comparing `ml3_platform_sdk-0.0.8/ml3_platform_sdk/core/connection.py` & `ml3_platform_sdk-0.0.9/ml3_platform_sdk/core/connection.py`

 * *Files identical despite different names*

### Comparing `ml3_platform_sdk-0.0.8/ml3_platform_sdk/core/enums.py` & `ml3_platform_sdk-0.0.9/ml3_platform_sdk/core/enums.py`

 * *Files identical despite different names*

### Comparing `ml3_platform_sdk-0.0.8/ml3_platform_sdk/core/requests.py` & `ml3_platform_sdk-0.0.9/ml3_platform_sdk/core/requests.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     FileType,
     MonitoringTarget,
     StoragePolicy,
     TaskType,
     UserCompanyRole,
     UserProjectRole,
 )
-from ml3_platform_sdk.models import DataSchema, RetrainTrigger
+from ml3_platform_sdk.models import DataSchema, RetrainTrigger, TaskCostInfo
 
 
 class DataSourceInfo(BaseModel):
     """
     Support base model for data source info
     """
 
@@ -93,14 +93,27 @@
     CreateModelRequest
     """
 
     task_id: str
     name: str
     version: str
     metric_name: str
+    retraining_cost: float
+    preferred_suggestion_type: str
+    resampled_dataset_size: Optional[int]
+
+
+class SetModelSuggestionTypeRequest(BaseModel):
+    """
+    SetModelSuggestionTypeRequest
+    """
+
+    model_id: str
+    preferred_suggestion_type: str
+    resampled_dataset_size: Optional[int] = None
 
 
 class GetModelsRequest(BaseModel):
     """
     Get models request model
     """
 
@@ -122,15 +135,15 @@
 
     model_id: str
     model_version: str
 
 
 class UpdateModelVersionBySuggestionIDRequest(BaseModel):
     """
-    Update Model Version By Suggestion ID Request
+    Update Model Version By SuggestionInfo ID Request
     """
 
     model_id: str
     new_model_version: str
     suggestion_id: str
 
 
@@ -188,21 +201,32 @@
     task_id: str
     data_schema: DataSchema
 
 
 class CreateTaskRequest(BaseModel):
     """
     Create Data Schema Request model
-    TODO sistemare docs
     """
 
     project_id: str
     name: str
     tags: Optional[List[str]]
     task_type: TaskType
+    cost_info: Optional[TaskCostInfo]
+
+
+class UpdateTaskRequest(BaseModel):
+    """
+    Update a task request payload
+    """
+
+    task_id: str
+    name: Optional[str]
+    tags: Optional[List[str]]
+    cost_info: Optional[TaskCostInfo]
 
 
 class ComputeRetrainingReportRequest(BaseModel):
     """
     request to compute retraining report
     """
```

### Comparing `ml3_platform_sdk-0.0.8/ml3_platform_sdk/core/singleton.py` & `ml3_platform_sdk-0.0.9/ml3_platform_sdk/core/singleton.py`

 * *Files identical despite different names*

### Comparing `ml3_platform_sdk-0.0.8/ml3_platform_sdk/enums.py` & `ml3_platform_sdk-0.0.9/ml3_platform_sdk/enums.py`

 * *Files 22% similar despite different names*

```diff
@@ -76,14 +76,17 @@
     **Fields:**
 
         - TABULAR
     """
 
     TABULAR = 'tabular'
 
+    def __str__(self):
+        return self.value
+
 
 class StoringDataType(Enum):
     """
     **Fields:**
 
         - HISTORICAL
         - REFERENCE
@@ -91,26 +94,32 @@
     """
 
     HISTORICAL = 'historical'
     REFERENCE = 'reference'
     PRODUCTION = 'production'
     KPI = 'kpi'
 
+    def __str__(self):
+        return self.value
+
 
 class FileType(Enum):
     """
     **Fields:**
 
         - CSV
         - JSON
     """
 
     CSV = 'csv'
     JSON = 'json'
 
+    def __str__(self):
+        return self.value
+
 
 class JobStatus(Enum):
     """
     **Fields:**
 
         - IDLE
         - STARTING
@@ -121,14 +130,17 @@
 
     IDLE = 'idle'
     STARTING = 'starting'
     RUNNING = 'running'
     COMPLETED = 'completed'
     ERROR = 'error'
 
+    def __str__(self):
+        return self.value
+
 
 class UserCompanyRole(Enum):
     """
     **Fields:**
 
         - COMPANY_OWNER
         - COMPANY_ADMIN
@@ -137,66 +149,81 @@
     """
 
     COMPANY_OWNER = "COMPANY_OWNER"
     COMPANY_ADMIN = "COMPANY_ADMIN"
     COMPANY_USER = "COMPANY_USER"
     COMPANY_NONE = "COMPANY_NONE"
 
+    def __str__(self):
+        return self.value
+
 
 class UserProjectRole(Enum):
     """
     **Fields:**
 
         - PROJECT_ADMIN
         - PROJECT_USER
         - PROJECT_VIEW
     """
 
     PROJECT_ADMIN = "PROJECT_ADMIN"
     PROJECT_USER = "PROJECT_USER"
     PROJECT_VIEW = "PROJECT_VIEW"
 
+    def __str__(self):
+        return self.value
+
 
 class DetectionEventSeverity(Enum):
     """
     **Fields:**
 
         - LOW
         - MEDIUM
         - HIGH
     """
 
     LOW = 'low'
     MEDIUM = 'medium'
     HIGH = 'high'
 
+    def __str__(self):
+        return self.value
+
 
 class DetectionEventType(Enum):
     """
     **Fields:**
 
         - DRIFT
     """
 
     DRIFT = 'drift'
 
+    def __str__(self):
+        return self.value
+
 
 class MonitoringTarget(Enum):
     """
     **Fields:**
 
         - MODEL
         - INPUT
         - CONCEPT
     """
 
     MODEL = 'model'
     INPUT = 'input'
     CONCEPT = 'concept'
 
+    def __str__(self):
+        return self.value
+
 
 class DetectionEventActionType(Enum):
     """
     **Fields:**
 
         - DISCORD_NOTIFICATION
         - SLACK_NOTIFICATION
@@ -205,27 +232,50 @@
 
     DISCORD_NOTIFICATION = 'discord_notification'
     SLACK_NOTIFICATION = 'slack_notification'
     EMAIL_NOTIFICATION = 'email_notification'
     TEAMS_NOTIFICATION = 'teams_notification'
     RETRAIN = 'retrain'
 
+    def __str__(self):
+        return self.value
+
 
 class ModelMetricName(Enum):
     """
     Name of the model metrics that is associated with the model
 
     **Fields:**
         - RMSE
         - RSQUARE
     """
 
     RMSE = 'rmse'
     RSQUARE = 'rsquare'
 
+    def __str__(self):
+        return self.value
+
+
+class SuggestionType(Enum):
+    """
+    Enum to specify the preferred
+    type of suggestion
+
+    **Fields:**
+        - SAMPLE_WEIGHTS
+        - RESAMPLED_DATASET
+    """
+
+    SAMPLE_WEIGHTS = 'sample_weights'
+    RESAMPLED_DATASET = 'resampled_dataset'
+
+    def __str__(self):
+        return self.value
+
 
 class ApiKeyExpirationTime(Enum):
     """
     **Fields:**
 
         - ONE_MONTH
         - THREE_MONTHS
@@ -237,14 +287,17 @@
 
     ONE_MONTH = 'one_month'
     THREE_MONTHS = 'three_months'
     SIX_MONTHS = 'six_months'
     ONE_YEAR = 'one_year'
     NEVER = 'never'
 
+    def __str__(self):
+        return self.value
+
 
 class ExternalIntegration(Enum):
     """
     An integration with a 3rd party service provider
 
     **Fields:**
         - AWS
@@ -252,14 +305,17 @@
         - AZURE
     """
 
     AWS = 'aws'
     GCP = 'gcp'
     AZURE = 'azure'
 
+    def __str__(self):
+        return self.value
+
 
 class StoragePolicy(Enum):
     """
     Enumeration that specifies the storage policy for the data sent to
     ML cube Platform
 
     **Fields:**
@@ -269,14 +325,34 @@
             Platform will access to this storage source every time
             it needs to read data
     """
 
     MLCUBE = 'mlcube'
     CUSTOMER = 'customer'
 
+    def __str__(self):
+        return self.value
+
 
 class RetrainTriggerType(Enum):
     """
     Enumeration of the possible retrain triggers
     """
 
     AWS_EVENT_BRIDGE = 'aws_event_bridge'
+    GCP_PUBSUB = 'gcp_pubsub'
+    AZURE_EVENT_GRID = 'azure_event_grid'
+
+    def __str__(self):
+        return self.value
+
+
+class Currency(Enum):
+    """
+    Currency of to use for the Task
+    """
+
+    EURO = 'euro'
+    DOLLAR = 'dollar'
+
+    def __str__(self):
+        return self.value
```

### Comparing `ml3_platform_sdk-0.0.8/ml3_platform_sdk/exceptions.py` & `ml3_platform_sdk-0.0.9/ml3_platform_sdk/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,20 @@
 
 class CreateTaskException(SDKClientException):
     """
     CreateTaskException
     """
 
 
+class UpdateTaskException(SDKClientException):
+    """
+    UpdateTaskException
+    """
+
+
 class CreateModelException(SDKClientException):
     """
     CreateModelException
     """
 
 
 class AddDataSchemaException(SDKClientException):
@@ -62,14 +68,20 @@
 
 class AddModelReferenceException(SDKClientException):
     """
     AddModelReferenceException
     """
 
 
+class SetModelSuggestionTypeException(SDKClientException):
+    """
+    SetModelSuggestionTypeException
+    """
+
+
 class UpdateModelVersionException(SDKClientException):
     """
     UpdateModelVersionException
     """
 
 
 class AddProductionDataException(SDKClientException):
```

### Comparing `ml3_platform_sdk-0.0.8/ml3_platform_sdk/models.py` & `ml3_platform_sdk-0.0.9/ml3_platform_sdk/models.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from datetime import datetime
 from typing import Any, Dict, List, Optional, Union
 
-from pydantic import BaseModel
+from pydantic import BaseModel, Extra
 
 from ml3_platform_sdk.enums import (
+    Currency,
     DatasetType,
     DetectionEventActionType,
     DetectionEventSeverity,
     DetectionEventType,
     ExternalIntegration,
     KPIStatus,
     ModelMetricName,
     ModelStatus,
     MonitoringTarget,
     RetrainTriggerType,
     StoragePolicy,
+    SuggestionType,
     TaskStatus,
     TaskType,
     UserCompanyRole,
 )
 
 # Used for polymorphic classes (de)serialization
 subclass_registry: Dict = {}
@@ -51,14 +53,63 @@
 
     """
 
     project_id: str
     name: str
 
 
+class TaskCostInfo(BaseModel):
+    """
+    Base class for task cost info.
+    It depends on TaskType because classification is different from
+    regression in terms of business costs due to errors
+    """
+
+    currency: Currency
+
+    class Config:
+        """
+        Allow extra fields
+        """
+
+        extra = Extra.allow
+
+
+class RegressionTaskCostInfo(TaskCostInfo):
+    """
+    Regression cost info is expressed in two terms:
+    - cost due to overestimation
+    - cost due to underestimation
+
+    Fields:
+        currency
+        overestimation_cost
+        underestimation_cost
+    """
+
+    overestimation_cost: float
+    underestimation_cost: float
+
+
+class ClassificationTaskCostInfo(TaskCostInfo):
+    """
+    Regression cost info is expressed in two terms:
+    - cost due to overestimation
+    - cost due to underestimation
+
+    Fields:
+        currency
+        false_positive_cost
+        false_negative_cost
+    """
+
+    false_positive_cost: float
+    false_negative_cost: float
+
+
 class Task(BaseModel):
     """
     Task model
 
     Attributes:
         task_id: str
         name: str
@@ -68,14 +119,15 @@
     """
 
     task_id: str
     name: str
     type: TaskType
     status: TaskStatus
     status_start_date: str
+    cost_info: Optional[TaskCostInfo]
 
 
 class RetrainTrigger(BaseModel):
     """
     Base model to define a retrain trigger
 
     Fields:
@@ -90,24 +142,51 @@
 class AWSEventBridgeRetrainTrigger(RetrainTrigger):
     """
     Base model to define an AWS EventBridge retrain trigger
 
     Fields:
         type
         credentials_id
-        credentials_name
         aws_region_name
         event_bus_name
     """
 
     type: RetrainTriggerType = RetrainTriggerType.AWS_EVENT_BRIDGE
     aws_region_name: str
     event_bus_name: str
 
 
+class GCPPubSubRetrainTrigger(RetrainTrigger):
+    """
+    Base model to define a GCP PubSub retrain trigger
+
+    Fields:
+        type
+        credentials_id
+        topic_name
+    """
+
+    type: RetrainTriggerType = RetrainTriggerType.GCP_PUBSUB
+    topic_name: str
+
+
+class AzureEventGridRetrainTrigger(RetrainTrigger):
+    """
+    Base model to define an Azure EventGrid retrain trigger
+
+    Fields:
+        type
+        credentials_id
+        topic_endpoint
+    """
+
+    type: RetrainTriggerType = RetrainTriggerType.AZURE_EVENT_GRID
+    topic_endpoint: str
+
+
 class Model(BaseModel):
     """
     Base model to define model item
 
     Attributes:
         model_id: str
         task_id: str
@@ -127,15 +206,22 @@
     name: str
     version: str
     status: ModelStatus
     status_data_start_timestamp: Optional[str]
     status_insert_datetime: datetime
     metric_name: ModelMetricName
     creation_datetime: Optional[datetime]
-    retrain_trigger: Optional[Union[AWSEventBridgeRetrainTrigger]]
+    retrain_trigger: Optional[
+        Union[
+            AWSEventBridgeRetrainTrigger,
+            GCPPubSubRetrainTrigger,
+            AzureEventGridRetrainTrigger,
+        ]
+    ]
+    retraining_cost: float
 
 
 class Job(BaseModel):
     """
     Job information item model
 
     Attributes:
@@ -214,51 +300,101 @@
     kpi_id: str
     name: str
     status: KPIStatus
     status_kpi_start_timestamp: Optional[datetime]
     status_insert_datetime: datetime
 
 
-class Suggestion(BaseModel):
+class SuggestionInfo(BaseModel):
     """
-    Suggestion base model
+    SuggestionInfo base model
 
     Attributes:
         id: str
         executed: bool
         timestamp: str
     """
 
     id: str
     executed: bool
     timestamp: str
 
 
+class Suggestion(BaseModel):
+    """
+    Suggestion base model
+
+    Attributes:
+        suggestion_id: str
+        suggestion_type: SuggestionType
+    """
+
+    suggestion_id: str
+    suggestion_type: SuggestionType
+    sample_ids: List[str]
+
+    class Config:
+        """
+        Config class for Suggestion
+        """
+
+        extra = Extra.allow
+
+
+class SampleWeightsSuggestion(Suggestion):
+    """
+    SampleWeightsSuggestion base model
+
+    Attributes:
+        suggestion_id: str
+        suggestion_type: SuggestionType
+        sample_ids: List[str]
+        sample_weights: List[float]
+    """
+
+    sample_weights: List[float]
+
+
+class ResampledDatasetSuggestion(Suggestion):
+    """
+    ResampledDatasetSuggestion base model
+
+    Attributes:
+        suggestion_id: str
+        suggestion_type: SuggestionType
+        sample_ids: List[str]
+        sample_counts: List[int]
+    """
+
+    sample_counts: List[int]
+
+
 class RetrainingReport(BaseModel):
     """
     base model for Retraining Report
 
     Attributes:
         report_id: str
-        sample_ids: List[str]
-        sample_weights: List[float]
+        suggestion: Suggestion
         effective_sample_size: float
         model_metric_name: str
-        upper_bound: float
-        lower_bound: float
+        performance_upper_bound: float
+        performance_lower_bound: float
+        cost_upper_bound: float
+        cost_lower_bound: float
     """
 
     report_id: str
-    suggestion_id: str
-    sample_ids: List[str]
-    sample_weights: List[float]
+    suggestion: Suggestion
     effective_sample_size: float
     model_metric_name: str
-    upper_bound: float
-    lower_bound: float
+    performance_upper_bound: float
+    performance_lower_bound: float
+    cost_upper_bound: Optional[float]
+    cost_lower_bound: Optional[float]
 
 
 class CompanyUser(BaseModel):
     """
     base model for company user
 
     Attributes:
```

### Comparing `ml3_platform_sdk-0.0.8/pyproject.toml` & `ml3_platform_sdk-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ml3-platform-sdk"
-version = "0.0.8"
+version = "0.0.9"
 authors = [ "MLcube",]
 description = "ML Platform SDK"
 license = "GPL"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: GNU General Public License (GPL)",
```

### Comparing `ml3_platform_sdk-0.0.8/PKG-INFO` & `ml3_platform_sdk-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml3-platform-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: ML Platform SDK
 License: GPL
 Author: MLcube
 Requires-Python: >=3.8.1,<3.13
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License (GPL)
 Classifier: License :: Other/Proprietary License
```

