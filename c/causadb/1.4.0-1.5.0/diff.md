# Comparing `tmp/causadb-1.4.0.tar.gz` & `tmp/causadb-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "causadb-1.4.0.tar", max compression
+gzip compressed data, was "causadb-1.5.0.tar", max compression
```

## Comparing `causadb-1.4.0.tar` & `causadb-1.5.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      642 2024-03-30 19:46:21.840438 causadb-1.4.0/README.md
--rw-r--r--   0        0        0      115 2024-03-30 19:46:21.840438 causadb-1.4.0/causadb/__init__.py
--rw-r--r--   0        0        0       22 2024-03-30 19:46:43.424324 causadb-1.4.0/causadb/__version__.py
--rw-r--r--   0        0        0     5118 2024-03-30 19:46:21.840438 causadb-1.4.0/causadb/causadb.py
--rw-r--r--   0        0        0     2855 2024-03-30 19:46:21.840438 causadb-1.4.0/causadb/cli/account.py
--rw-r--r--   0        0        0     3116 2024-03-30 19:46:21.840438 causadb-1.4.0/causadb/cli/data.py
--rwxr-xr-x   0        0        0      743 2024-03-30 19:46:21.840438 causadb-1.4.0/causadb/cli/main.py
--rw-r--r--   0        0        0     7085 2024-03-30 19:46:21.840438 causadb-1.4.0/causadb/cli/models.py
--rw-r--r--   0        0        0      891 2024-03-30 19:46:21.840438 causadb-1.4.0/causadb/cli/utils.py
--rw-r--r--   0        0        0     2297 2024-03-30 19:46:21.840438 causadb-1.4.0/causadb/data.py
--rw-r--r--   0        0        0    14420 2024-03-30 19:46:21.840438 causadb-1.4.0/causadb/model.py
--rw-r--r--   0        0        0      215 2024-03-30 19:46:21.840438 causadb-1.4.0/causadb/utils.py
--rw-r--r--   0        0        0      695 2024-03-30 19:46:42.528329 causadb-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 causadb-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0      642 2024-04-03 16:57:41.182521 causadb-1.5.0/README.md
+-rw-r--r--   0        0        0      115 2024-04-03 16:57:41.182521 causadb-1.5.0/causadb/__init__.py
+-rw-r--r--   0        0        0       22 2024-04-03 16:58:00.026551 causadb-1.5.0/causadb/__version__.py
+-rw-r--r--   0        0        0     5189 2024-04-03 16:57:41.182521 causadb-1.5.0/causadb/causadb.py
+-rw-r--r--   0        0        0     2855 2024-04-03 16:57:41.182521 causadb-1.5.0/causadb/cli/account.py
+-rw-r--r--   0        0        0     3116 2024-04-03 16:57:41.182521 causadb-1.5.0/causadb/cli/data.py
+-rwxr-xr-x   0        0        0      743 2024-04-03 16:57:41.182521 causadb-1.5.0/causadb/cli/main.py
+-rw-r--r--   0        0        0     7085 2024-04-03 16:57:41.182521 causadb-1.5.0/causadb/cli/models.py
+-rw-r--r--   0        0        0      891 2024-04-03 16:57:41.182521 causadb-1.5.0/causadb/cli/utils.py
+-rw-r--r--   0        0        0     2646 2024-04-03 16:57:41.182521 causadb-1.5.0/causadb/data.py
+-rw-r--r--   0        0        0    14837 2024-04-03 16:57:41.182521 causadb-1.5.0/causadb/model.py
+-rw-r--r--   0        0        0      215 2024-04-03 16:57:41.182521 causadb-1.5.0/causadb/utils.py
+-rw-r--r--   0        0        0      695 2024-04-03 16:57:59.022549 causadb-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 causadb-1.5.0/PKG-INFO
```

### Comparing `causadb-1.4.0/README.md` & `causadb-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `causadb-1.4.0/causadb/causadb.py` & `causadb-1.5.0/causadb/causadb.py`

 * *Files 6% similar despite different names*

```diff
@@ -111,16 +111,16 @@
         """
         headers = {"token": self.token}
 
         try:
             response = requests.get(
                 f"{get_causadb_url()}/models/{model_name}", headers=headers
             ).json()
-        except:
-            raise Exception("CausaDB server request failed")
+        except Exception as e:
+            raise Exception(f"CausaDB server request failed: {e}")
 
         # If the model exists, return it
         model = Model(model_name, self)
 
         return model
 
     def list_models(self) -> list[Model]:
@@ -131,16 +131,16 @@
         """
         headers = {"token": self.token}
 
         try:
             response = requests.get(
                 f"{get_causadb_url()}/models", headers=headers
             ).json()
-        except:
-            raise Exception("CausaDB server request failed")
+        except Exception as e:
+            raise Exception(f"CausaDB server request failed: {e}")
 
         model_list = []
         for model_spec in response.get("models", []):
             model = Model(model_spec["name"], self)
             model_list.append(model)
 
         return model_list
@@ -155,16 +155,16 @@
             Data: The data object.
         """
         headers = {"token": self.token}
         try:
             response = requests.get(
                 f"{get_causadb_url()}/data/{data_name}", headers=headers
             ).json()
-        except:
-            raise Exception("CausaDB server request failed")
+        except Exception as e:
+            raise Exception(f"CausaDB server request failed: {e}")
 
         data = Data(data_name, self)
 
         return data
 
     def list_data(self) -> list[Data]:
         """List all data.
@@ -174,16 +174,16 @@
         """
         headers = {"token": self.token}
 
         try:
             response = requests.get(
                 f"{get_causadb_url()}/data", headers=headers
             ).json()
-        except:
-            raise Exception("CausaDB client failed to connect to server")
+        except Exception as e:
+            raise Exception(f"CausaDB server request failed: {e}")
 
         data_list = []
         for data_spec in response.get("data", []):
             data = Data(data_spec["name"], self)
             data_list.append(data)
 
         return data_list
```

### Comparing `causadb-1.4.0/causadb/cli/account.py` & `causadb-1.5.0/causadb/cli/account.py`

 * *Files identical despite different names*

### Comparing `causadb-1.4.0/causadb/cli/data.py` & `causadb-1.5.0/causadb/cli/data.py`

 * *Files identical despite different names*

### Comparing `causadb-1.4.0/causadb/cli/main.py` & `causadb-1.5.0/causadb/cli/main.py`

 * *Files identical despite different names*

### Comparing `causadb-1.4.0/causadb/cli/models.py` & `causadb-1.5.0/causadb/cli/models.py`

 * *Files identical despite different names*

### Comparing `causadb-1.4.0/causadb/cli/utils.py` & `causadb-1.5.0/causadb/cli/utils.py`

 * *Files identical despite different names*

### Comparing `causadb-1.4.0/causadb/data.py` & `causadb-1.5.0/causadb/data.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,16 +21,16 @@
         """Remove the data from the CausaDB system."""
         headers = {"token": self.client.token}
         try:
             requests.delete(
                 f"{get_causadb_url()}/data/{self.data_name}",
                 headers=headers,
             )
-        except:
-            raise Exception("CausaDB server request failed")
+        except Exception as e:
+            raise Exception(f"CausaDB server request failed: {e}")
 
     def from_csv(self, filepath: str) -> None:
         """Add data from a CSV file.
 
         Args:
             filepath (str): The path to the CSV file.
         """
@@ -59,21 +59,28 @@
     def _update(self, data: dict) -> None:
         """Pushes the data to the CausaDB server.
 
         Args:
             data (dict): The new data.
         """
 
+        # Check if the data are valid (no missing values, all numeric)
+        df = pd.DataFrame.from_dict(data) \
+            .apply(pd.to_numeric, errors="coerce")
+        if df.isnull().values.any():
+            raise Exception(
+                "Data contains missing values. Missing values are not yet supported.")
+
         # Send a POST request to the CausaDB server to update the data
         try:
             headers = {"token": self.client.token}
             response = requests.post(
                 f"{get_causadb_url()}/data/{self.data_name}",
                 headers=headers,
                 json=data,
             ).json()
-        except:
-            raise Exception("CausaDB client failed to connect to server")
+        except Exception as e:
+            raise Exception(f"CausaDB server request failed: {e}")
 
         if response["status"] != "success":
             # If the response is not successful, raise an exception and include the error message
             raise Exception(f"Failed to update data: {response['message']}")
```

### Comparing `causadb-1.4.0/causadb/model.py` & `causadb-1.5.0/causadb/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -38,16 +38,16 @@
         """Remove the model from the CausaDB system."""
         headers = {"token": self.client.token}
         try:
             requests.delete(
                 f"{get_causadb_url()}/models/{self.model_name}",
                 headers=headers,
             )
-        except:
-            raise Exception("CausaDB server request failed")
+        except Exception as e:
+            raise Exception(f"CausaDB server request failed: {e}")
 
     def set_nodes(self, nodes: list[str]) -> None:
         """Set the nodes of the model.
 
         Args:
             nodes (list[str]): A list of node names.
 
@@ -56,16 +56,16 @@
         """
         headers = {"token": self.client.token}
 
         try:
             response = requests.get(
                 f"{get_causadb_url()}/models/{self.model_name}", headers=headers
             ).json()
-        except:
-            raise Exception("CausaDB server request failed")
+        except Exception as e:
+            raise Exception(f"CausaDB server request failed: {e}")
 
         self.config = response["details"]["config"]
         self.config["nodes"] = nodes
 
         self._update()
 
     def get_nodes(self) -> list[str]:
@@ -76,16 +76,16 @@
         """
         headers = {"token": self.client.token}
 
         try:
             response = requests.get(
                 f"{get_causadb_url()}/models/{self.model_name}", headers=headers
             ).json()
-        except:
-            raise Exception("CausaDB server request failed")
+        except Exception as e:
+            raise Exception(f"CausaDB server request failed: {e}")
 
         return response["details"]["config"]["nodes"]
 
     def set_edges(self, edges: list[tuple[str, str]]) -> None:
         """Set the edges of the model.
 
         Args:
@@ -99,16 +99,16 @@
         """
         headers = {"token": self.client.token}
 
         try:
             response = requests.get(
                 f"{get_causadb_url()}/models/{self.model_name}", headers=headers
             ).json()
-        except:
-            raise Exception("CausaDB server request failed")
+        except Exception as e:
+            raise Exception(f"CausaDB server request failed: {e}")
 
         self.config = response["details"]["config"]
         self.config["edges"] = edges
 
         self._update()
 
     def get_edges(self) -> list[tuple[str, str]]:
@@ -119,16 +119,16 @@
         """
         headers = {"token": self.client.token}
 
         try:
             response = requests.get(
                 f"{get_causadb_url()}/models/{self.model_name}", headers=headers
             ).json()
-        except:
-            raise Exception("CausaDB server request failed")
+        except Exception as e:
+            raise Exception(f"CausaDB server request failed: {e}")
 
         edges = response["details"]["config"]["edges"]
         # Convert the edges to a list of tuples
         return [(edge[0], edge[1]) for edge in edges]
 
     def set_node_types(self, node_types: dict) -> None:
         """Set the node types of the model.
@@ -143,16 +143,16 @@
         """
         headers = {"token": self.client.token}
 
         try:
             response = requests.get(
                 f"{get_causadb_url()}/models/{self.model_name}", headers=headers
             ).json()
-        except:
-            raise Exception("CausaDB server request failed")
+        except Exception as e:
+            raise Exception(f"CausaDB server request failed: {e}")
 
         self.config = response["details"]["config"]
         self.config["node_types"] = node_types
 
         self._update()
 
     def get_node_types(self) -> dict:
@@ -163,16 +163,16 @@
         """
         headers = {"token": self.client.token}
 
         try:
             response = requests.get(
                 f"{get_causadb_url()}/models/{self.model_name}", headers=headers
             ).json()
-        except:
-            raise Exception("CausaDB server request failed")
+        except Exception as e:
+            raise Exception(f"CausaDB server request failed: {e}")
 
         return response["details"]["config"]["node_types"]
 
     def attach(self, data_name: str) -> None:
         """Attach data to the model.
 
         Args:
@@ -181,32 +181,32 @@
         headers = {"token": self.client.token}
 
         try:
             response = requests.post(
                 f"{get_causadb_url()}/models/{self.model_name}/attach/{data_name}",
                 headers=headers
             ).json()
-        except:
-            raise Exception("CausaDB server request failed")
+        except Exception as e:
+            raise Exception(f"CausaDB server request failed: {e}")
 
     def detach(self, data_name: str) -> None:
         """Detach data from the model.
 
         Args:
             data_name (str): The name of the data to detach.
         """
         headers = {"token": self.client.token}
 
         try:
             response = requests.delete(
                 f"{get_causadb_url()}/models/{self.model_name}/detach",
                 headers=headers
             ).json()
-        except:
-            raise Exception("CausaDB server request failed")
+        except Exception as e:
+            raise Exception(f"CausaDB server request failed: {e}")
 
     def train(self, data_name: str = None, wait: bool = True, poll_interval: float = 0.2, poll_limit: float = 30.0, verbose: bool = False, progress_interval: float = 1.0) -> None:
         """Train the model.
 
         Args:
             wait (bool): Whether to wait for the model to finish training.
             poll_interval (float): The interval at which to poll the server for the model status.
@@ -225,16 +225,16 @@
         headers = {"token": self.client.token}
 
         try:
             response = requests.post(
                 f"{get_causadb_url()}/models/{self.model_name}/train",
                 headers=headers
             )
-        except:
-            raise Exception("CausaDB server request failed")
+        except Exception as e:
+            raise Exception(f"CausaDB server request failed: {e}")
 
         # If HTTPException status code is 400, raise an exception
         if response.status_code == 400:
             raise Exception(response.json()["detail"])
         response = response.json()
 
         if wait:
@@ -248,15 +248,16 @@
 
                 if verbose and time_elapsed - last_progress >= progress_interval:
                     # Display model training time elapsed time_elapsed
                     print(f"Training model... ({round(time_elapsed)}s)")
                     last_progress = time_elapsed
 
                 if time_elapsed > poll_limit:
-                    raise Exception("Model training took too long")
+                    raise Exception(
+                        "Model training took too long. Waiting time exceeded but the model is still training.")
             if verbose:
                 print(f"Model training progress: {self.status()}")
 
     def status(self) -> str:
         """Get the status of the model.
 
         Returns:
@@ -265,16 +266,16 @@
         headers = {"token": self.client.token}
 
         try:
             response = requests.get(
                 f"{get_causadb_url()}/models/{self.model_name}",
                 headers=headers,
             ).json()
-        except:
-            raise Exception("CausaDB server request failed")
+        except Exception as e:
+            raise Exception(f"CausaDB server request failed: {e}")
 
         model_status = response["details"]["status"]
 
         return model_status
 
     def simulate_actions(self, actions: dict, fixed: dict = {}, interval: float = 0.9, observation_noise: bool = False) -> dict:
         """Simulate an action on the model.
@@ -304,16 +305,16 @@
 
         try:
             response = requests.post(
                 f"{get_causadb_url()}/models/{self.model_name}/simulate-actions",
                 headers=headers,
                 json=query,
             ).json()
-        except:
-            raise Exception("CausaDB server request failed")
+        except Exception as e:
+            raise Exception(f"CausaDB server request failed: {e}")
 
         if "outcome" in response:
             outcome = response["outcome"]
             return {
                 "median": pd.DataFrame.from_dict(outcome["median"]),
                 "lower": pd.DataFrame.from_dict(outcome["lower"]),
                 "upper": pd.DataFrame.from_dict(outcome["upper"])
@@ -350,16 +351,16 @@
 
         try:
             response = requests.post(
                 f"{get_causadb_url()}/models/{self.model_name}/causal-effects",
                 headers=headers,
                 json=query,
             ).json()
-        except:
-            raise Exception("CausaDB server request failed")
+        except Exception as e:
+            raise Exception(f"CausaDB server request failed: {e}")
 
         if "outcome" in response:
             return pd.DataFrame.from_dict(response["outcome"])
 
         raise Exception("CausaDB server request failed")
 
     def find_best_actions(self, targets: dict[str, float], actionable: list[str], fixed: dict[str, float] = {}) -> dict:
@@ -389,16 +390,16 @@
 
         try:
             response = requests.post(
                 f"{get_causadb_url()}/models/{self.model_name}/find-best-actions",
                 headers=headers,
                 json=query,
             ).json()
-        except:
-            raise Exception("CausaDB server request failed")
+        except Exception as e:
+            raise Exception(f"CausaDB server request failed: {e}")
 
         if "best_actions" in response:
             return pd.DataFrame.from_dict(response["best_actions"])
 
         raise Exception("CausaDB server request failed")
 
     def causal_attributions(self, outcome: str, normalise: bool = False) -> pd.DataFrame:
@@ -423,16 +424,16 @@
 
         try:
             response = requests.post(
                 f"{get_causadb_url()}/models/{self.model_name}/causal-attributions",
                 headers=headers,
                 json=query,
             ).json()
-        except:
-            raise Exception("CausaDB server request failed")
+        except Exception as e:
+            raise Exception(f"CausaDB server request failed: {e}")
 
         if "outcome" in response:
             return pd.DataFrame.from_dict(response["outcome"])
 
         raise Exception("CausaDB server request failed")
 
     def _update(self) -> None:
@@ -441,9 +442,9 @@
 
         try:
             requests.post(
                 f"{get_causadb_url()}/models/{self.model_name}",
                 headers=headers,
                 json=self.config
             ).json()
-        except:
-            raise Exception("CausaDB server request failed")
+        except Exception as e:
+            raise Exception(f"CausaDB server request failed: {e}")
```

### Comparing `causadb-1.4.0/pyproject.toml` & `causadb-1.5.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "causadb"
-version = "1.4.0"
+version = "1.5.0"
 description = ""
 authors = ["Jordan hart <jordan@causa.tech>"]
 readme = "README.md"
 packages = [
     { include = "causadb", from = "." }
 ]
```

### Comparing `causadb-1.4.0/PKG-INFO` & `causadb-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: causadb
-Version: 1.4.0
+Version: 1.5.0
 Summary: 
 Author: Jordan hart
 Author-email: jordan@causa.tech
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

