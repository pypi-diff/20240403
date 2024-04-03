# Comparing `tmp/likelihood-1.2.8.tar.gz` & `tmp/likelihood-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "likelihood-1.2.8.tar", last modified: Fri Mar 22 16:05:58 2024, max compression
+gzip compressed data, was "likelihood-1.2.9.tar", last modified: Wed Apr  3 19:41:38 2024, max compression
```

## Comparing `likelihood-1.2.8.tar` & `likelihood-1.2.9.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:05:58.792739 likelihood-1.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-22 16:05:54.000000 likelihood-1.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-03-22 16:05:58.792739 likelihood-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-03-22 16:05:54.000000 likelihood-1.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:05:58.788740 likelihood-1.2.8/likelihood/
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-22 16:05:54.000000 likelihood-1.2.8/likelihood/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:05:58.788740 likelihood-1.2.8/likelihood/graph/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-22 16:05:54.000000 likelihood-1.2.8/likelihood/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-03-22 16:05:54.000000 likelihood-1.2.8/likelihood/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     8591 2024-03-22 16:05:54.000000 likelihood-1.2.8/likelihood/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:05:58.788740 likelihood-1.2.8/likelihood/models/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-22 16:05:54.000000 likelihood-1.2.8/likelihood/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-03-22 16:05:54.000000 likelihood-1.2.8/likelihood/models/regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-03-22 16:05:54.000000 likelihood-1.2.8/likelihood/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:05:58.788740 likelihood-1.2.8/likelihood/tools/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-22 16:05:54.000000 likelihood-1.2.8/likelihood/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-03-22 16:05:54.000000 likelihood-1.2.8/likelihood/tools/numeric_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    35049 2024-03-22 16:05:54.000000 likelihood-1.2.8/likelihood/tools/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 16:05:58.792739 likelihood-1.2.8/likelihood.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-03-22 16:05:58.000000 likelihood-1.2.8/likelihood.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-03-22 16:05:58.000000 likelihood-1.2.8/likelihood.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 16:05:58.000000 likelihood-1.2.8/likelihood.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-22 16:05:58.000000 likelihood-1.2.8/likelihood.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-22 16:05:58.000000 likelihood-1.2.8/likelihood.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 16:05:58.792739 likelihood-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-03-22 16:05:54.000000 likelihood-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:38.250659 likelihood-1.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-03 19:41:34.000000 likelihood-1.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-03 19:41:38.250659 likelihood-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-04-03 19:41:34.000000 likelihood-1.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:38.246659 likelihood-1.2.9/likelihood/
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:38.246659 likelihood-1.2.9/likelihood/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2082 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8591 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:38.250659 likelihood-1.2.9/likelihood/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9404 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/models/regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/models/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:38.250659 likelihood-1.2.9/likelihood/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/tools/numeric_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36497 2024-04-03 19:41:35.000000 likelihood-1.2.9/likelihood/tools/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:41:38.250659 likelihood-1.2.9/likelihood.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-03 19:41:38.000000 likelihood-1.2.9/likelihood.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-03 19:41:38.000000 likelihood-1.2.9/likelihood.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:41:38.000000 likelihood-1.2.9/likelihood.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-03 19:41:38.000000 likelihood-1.2.9/likelihood.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 19:41:38.000000 likelihood-1.2.9/likelihood.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:41:38.250659 likelihood-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-03 19:41:35.000000 likelihood-1.2.9/setup.py
```

### Comparing `likelihood-1.2.8/LICENSE` & `likelihood-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `likelihood-1.2.8/PKG-INFO` & `likelihood-1.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: likelihood
-Version: 1.2.8
+Version: 1.2.9
 Summary: A package that performs the maximum likelihood algorithm.
 Home-page: https://github.com/jzsmoreno/likelihood/
 Author: J. A. Moreno-Guerra
 Author-email: jzs.gm27@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `likelihood-1.2.8/README.md` & `likelihood-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `likelihood-1.2.8/likelihood/graph/graph.py` & `likelihood-1.2.9/likelihood/graph/graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 from likelihood.tools import FeatureSelection
 
 
 class DynamicGraph(FeatureSelection):
     """A class to represent a dynamic graph"""
 
-    def __init__(self, df: DataFrame, n_importances: int):
+    def __init__(self, df: DataFrame, n_importances: int, **kwargs):
         self.G = Network(
             notebook=True, cdn_resources="remote", directed=True
         )  # enable interactive visualization in Jupyter Notebooks
         self.df = df
         self.n_importances = n_importances
-        super().__init__()
+        super().__init__(**kwargs)
 
     def fit(self, **kwargs) -> None:
         """Fit the model according to the given data and parameters."""
         self.get_digraph(self.df, self.n_importances)
         # create a dictionary with the indexes and names of the dataframe
         self.get_index = dict(zip(self.df.columns, range(len(self.df.columns))))
         self._make_network()
```

### Comparing `likelihood-1.2.8/likelihood/main.py` & `likelihood-1.2.9/likelihood/main.py`

 * *Files identical despite different names*

### Comparing `likelihood-1.2.8/likelihood/models/regression.py` & `likelihood-1.2.9/likelihood/models/regression.py`

 * *Files identical despite different names*

### Comparing `likelihood-1.2.8/likelihood/models/utils.py` & `likelihood-1.2.9/likelihood/models/utils.py`

 * *Files identical despite different names*

### Comparing `likelihood-1.2.8/likelihood/tools/numeric_tools.py` & `likelihood-1.2.9/likelihood/tools/numeric_tools.py`

 * *Files identical despite different names*

### Comparing `likelihood-1.2.8/likelihood/tools/tools.py` & `likelihood-1.2.9/likelihood/tools/tools.py`

 * *Files 5% similar despite different names*

```diff
@@ -360,15 +360,15 @@
 
     return 1 / (1 + math.exp(-x))
 
 
 class LogisticRegression:
     """class implementing multiple logistic regression"""
 
-    __slots__ = ["importance", "X", "y"]
+    __slots__ = ["importance", "X", "y", "w"]
 
     def __init__(self) -> None:
         """The class initializer"""
 
         self.importance = []
 
     def fit(self, dataset: ndarray, values: ndarray) -> None:
@@ -390,22 +390,22 @@
 
         self.X = dataset
         self.y = values
 
         U, S, VT = np.linalg.svd(self.X, full_matrices=False)
 
         inverse_sig = np.vectorize(sigmoide_inv)
-        w = (VT.T @ np.linalg.inv(np.diag(S)) @ U.T).T @ inverse_sig(self.y)
+        self.w = (VT.T @ np.linalg.inv(np.diag(S)) @ U.T).T @ inverse_sig(self.y)
 
         if self.y.shape[1] > 1:
-            for row in w:
+            for row in self.w:
                 self.importance.append(np.around(np.max(row), decimals=8))
         else:
             for i in range(self.X.shape[0]):
-                a = np.around(w[i], decimals=8)
+                a = np.around(self.w[i], decimals=8)
                 self.importance.append(a)
 
     def predict(self, datapoints: ndarray) -> ndarray:
         """
         Performs predictions for a set of points
 
         Parameters
@@ -439,15 +439,15 @@
                 print(f"The importance of the {i+1} feature is {a}")
         return np.array(self.importance)
 
 
 class LinearRegression:
     """class implementing multiple linear regression"""
 
-    __slots__ = ["importance", "X", "y"]
+    __slots__ = ["importance", "X", "y", "w"]
 
     def __init__(self) -> None:
         """The class initializer"""
 
         self.importance = []
 
     def fit(self, dataset: ndarray, values: ndarray, verbose: bool = False) -> None:
@@ -467,18 +467,18 @@
 
         """
 
         self.X = dataset
         self.y = values
 
         U, S, VT = np.linalg.svd(self.X, full_matrices=False)
-        w = (VT.T @ np.linalg.inv(np.diag(S)) @ U.T).T @ self.y
+        self.w = (VT.T @ np.linalg.inv(np.diag(S)) @ U.T).T @ self.y
 
         for i in range(self.X.shape[0]):
-            a = np.around(w[i], decimals=8)
+            a = np.around(self.w[i], decimals=8)
             self.importance.append(a)
 
         if verbose:
             print("\nSummary:")
             print("--------")
             print("\nParameters:", np.array(self.importance).shape)
             print("RMSE: {:.4f}".format(mean_square_error(self.y, self.predict(self.X))))
@@ -878,51 +878,59 @@
                     else:
                         x = np.where(labels == y_true[j])
                         count_mat[i, x[0]] += 1
 
         return count_mat
 
 
-def one_hot_encoding(x: ndarray | list) -> ndarray:
-    """
-    Calculates the one-hot encoding on a `numpy`/`list` array. Only accepts arrays of numbers as labels.
+class OneHotEncoder:
 
-    Parameters
-    ----------
-    x : `np.array`
-        An array containing the data.
+    __slots__ = ["x"]
 
-    Returns
-    -------
-    y : `ndarray`
-        The one-hot encodig matrix of `x`.
-    """
-    if not isinstance(x, ndarray):
-        x = np.array(x)  # If not numpy array then convert it
+    def __init__(self) -> None:
+        pass
+
+    def encode(self, x: ndarray | list):
+        self.x = x
+
+        if not isinstance(self.x, ndarray):
+            self.x = np.array(self.x)  # If not numpy array then convert it
 
-    y = np.zeros((x.size, x.max() + 1))  # Build matrix of (size num of entries) x (max value + 1)
+        y = np.zeros(
+            (self.x.size, self.x.max() + 1)
+        )  # Build matrix of (size num of entries) x (max value + 1)
 
-    y[np.arange(x.size), x] = 1  # Label with ones
+        y[np.arange(self.x.size), self.x] = 1  # Label with ones
 
-    return y
+        return y
+
+    def decode(self, x: ndarray | list) -> ndarray:
+        if not isinstance(x, ndarray):
+            x = np.array(x)  # If not numpy array then convert it
+
+        # Regresamos los valores max de cada renglon
+        y = np.argmax(x, axis=1)
+
+        return y
 
 
 class FeatureSelection:
     """
     Generate the data graph using a variation of the feature selection algorithm..
 
     - The method `get_digraph` returns the network based on the feature selection method.
     """
 
-    __slots__ = ["not_features", "X", "all_features_imp_graph"]
+    __slots__ = ["not_features", "X", "all_features_imp_graph", "w_dict", "scaler"]
 
     def __init__(self, not_features: list[str] = []) -> None:
         """The initializer of the class. The initial parameter is a list of strings with variables to discard."""
         self.not_features: List[str] = not_features
         self.all_features_imp_graph: List[Tuple] = []
+        self.w_dict = dict()
 
     def get_digraph(self, dataset: DataFrame, n_importances: int) -> str:
         """
         Get directed graph showing importance of features.
 
         Args:
             dataset (`DataFrame`): Dataset to be used for generating the graph.
@@ -939,19 +947,22 @@
 
         # We construct string from causal_graph
         feature_string = " digraph { "
         for column in columns:
             feature_string += column + "; "
 
         numeric_df = curr_dataset.select_dtypes(include="number")
-        scaler = DataScaler(numeric_df.copy().to_numpy(), n=None)
-        numeric_scaled = scaler.rescale()
-        numeric_df = pd.DataFrame(numeric_scaled, columns=numeric_df.columns)
+        self.scaler = DataScaler(numeric_df.copy().to_numpy().T, n=None)
+        numeric_scaled = self.scaler.rescale()
+        numeric_df = pd.DataFrame(numeric_scaled.T, columns=numeric_df.columns)
         curr_dataset[numeric_df.columns] = numeric_df
 
+        # We construct dictionary to save index for scaling
+        numeric_dict = dict(zip(list(numeric_df.columns), range(len(list(numeric_df.columns)))))
+
         # Iterate over all the columns to obtain their importances.
         for index_column, column in enumerate(columns):
 
             # Variable to predict
             Y = curr_dataset[column]
 
             # We check whether it is numerical or categorical.
@@ -967,23 +978,25 @@
                 dfe = DataFrameEncoder(X_aux)
                 encoded_df = dfe.encode(save_mode=False)
                 # We train
 
                 Model.fit(encoded_df.to_numpy().T, Y.to_numpy().T)
                 # We obtain importance
                 importance = Model.get_importances()
+                w = Model.w
             else:
                 Model = LogisticRegression()
                 num_unique_entries = curr_dataset[column].nunique()
 
                 quick_encoder = DataFrameEncoder(Y.to_frame())
                 encoded_Y = quick_encoder.encode(save_mode=False)
 
                 # Mapping to one-hot
-                train_y = one_hot_encoding(encoded_Y[column])
+                one_hot = OneHotEncoder()
+                train_y = one_hot.encode(encoded_Y[column])
                 # PASSING 0 -> 0.5 and 1 -> 0.73105
                 for i in range(len(train_y)):
                     for j in range(num_unique_entries):
                         if train_y[i][j] == 1.0:
                             train_y[i][j] = 0.73105
                         else:
                             train_y[i][j] = 0.5
@@ -996,27 +1009,34 @@
                 encoded_df = dfe.encode(save_mode=False)
 
                 # We train
                 Model.fit(encoded_df.to_numpy().T, train_y)
 
                 # We obtain importance
                 importance = Model.get_importances()
+                w = Model.w
 
             # We obtain the $n$ most important ones
             top_n_indexes = sorted(
                 range(len(importance)), key=lambda i: importance[i], reverse=True
             )[:n_importances]
 
             # We build the string for the column in question
             names_cols = list(X_aux.columns)
             # We store the indices, values and column names in a list of tuples.
             features_imp_node = [
                 (names_cols[top_n_indexes[i]], importance[top_n_indexes[i]])
                 for i in range(n_importances)
             ]
+            # We store w's for predictions
+
+            if column_type != "object":
+                self.w_dict[column] = (w, None, names_cols, dfe, numeric_dict)
+            else:
+                self.w_dict[column] = (w, quick_encoder, names_cols, dfe, numeric_dict)
             # Add to general list
             self.all_features_imp_graph.append((column, features_imp_node))
             # We format it
             for i in top_n_indexes:
                 feature_string += names_cols[i] + " -> "
 
             feature_string += column + "; "
@@ -1036,14 +1056,30 @@
         self.X.replace([np.inf, -np.inf], np.nan, inplace=True)
         self.X.replace(" ", np.nan, inplace=True)
         self.X.dropna(inplace=True)
         self.X = self.X.reset_index()
         self.X = self.X.drop(columns=["index"])
 
 
+def check_nan_inf(df: DataFrame) -> DataFrame:
+    """Check for `NaN` and `Inf` values in the `DataFrame`. If any are found, raise an error."""
+    nan_values = df.isnull().values.any()
+    count = np.isinf(df.select_dtypes(include="number")).values.sum()
+    print("There are null values : ", nan_values)
+    print("It contains " + str(count) + " infinite values")
+    if nan_values:
+        warning_type = "UserWarning"
+        msg = "Some rows may have been deleted due to the existence of nan values."
+        print(f"{warning_type}: {msg}")
+        print("Missing values correctly removed : ", "{:,}".format(df.isnull().values.sum()))
+        df = df.dropna()
+
+    return df
+
+
 # -------------------------------------------------------------------------
 if __name__ == "__main__":
     y_true = np.array([1, 2, 2, 1, 1])
     y_pred = np.array([1, 1, 2, 2, 1])
 
     labels = [1, 2]
     helper = PerformanceMeasures()
```

### Comparing `likelihood-1.2.8/likelihood.egg-info/PKG-INFO` & `likelihood-1.2.9/likelihood.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: likelihood
-Version: 1.2.8
+Version: 1.2.9
 Summary: A package that performs the maximum likelihood algorithm.
 Home-page: https://github.com/jzsmoreno/likelihood/
 Author: J. A. Moreno-Guerra
 Author-email: jzs.gm27@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `likelihood-1.2.8/setup.py` & `likelihood-1.2.9/setup.py`

 * *Files identical despite different names*

