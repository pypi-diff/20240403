# Comparing `tmp/impactchart-0.4.4.tar.gz` & `tmp/impactchart-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impactchart-0.4.4.tar", max compression
+gzip compressed data, was "impactchart-0.5.0.tar", max compression
```

## Comparing `impactchart-0.4.4.tar` & `impactchart-0.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    19938 2023-07-26 10:43:07.357770 impactchart-0.4.4/LICENSE.md
--rw-r--r--   0        0        0    10583 2024-02-25 22:57:27.161528 impactchart-0.4.4/README.md
--rw-r--r--   0        0        0        0 2024-02-16 01:12:14.319972 impactchart-0.4.4/impactchart/__init__.py
--rw-r--r--   0        0        0        0 2024-01-06 17:26:12.184230 impactchart-0.4.4/impactchart/cli/__init__.py
--rw-r--r--   0        0        0    15886 2024-02-12 16:41:09.118377 impactchart-0.4.4/impactchart/cli/main.py
--rw-r--r--   0        0        0    28845 2024-03-28 20:08:44.618852 impactchart-0.4.4/impactchart/model.py
--rw-r--r--   0        0        0     1365 2024-03-28 21:14:42.828812 impactchart-0.4.4/pyproject.toml
--rw-r--r--   0        0        0    11643 1970-01-01 00:00:00.000000 impactchart-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0    19938 2023-07-26 10:43:07.357770 impactchart-0.5.0/LICENSE.md
+-rw-r--r--   0        0        0    10583 2024-02-25 22:57:27.161528 impactchart-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2024-02-16 01:12:14.319972 impactchart-0.5.0/impactchart/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-06 17:26:12.184230 impactchart-0.5.0/impactchart/cli/__init__.py
+-rw-r--r--   0        0        0    15886 2024-02-12 16:41:09.118377 impactchart-0.5.0/impactchart/cli/main.py
+-rw-r--r--   0        0        0    30347 2024-04-01 20:32:24.439285 impactchart-0.5.0/impactchart/model.py
+-rw-r--r--   0        0        0     1365 2024-04-01 20:33:01.116034 impactchart-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0    11643 1970-01-01 00:00:00.000000 impactchart-0.5.0/PKG-INFO
```

### Comparing `impactchart-0.4.4/LICENSE.md` & `impactchart-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `impactchart-0.4.4/README.md` & `impactchart-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `impactchart-0.4.4/impactchart/cli/main.py` & `impactchart-0.5.0/impactchart/cli/main.py`

 * *Files identical despite different names*

### Comparing `impactchart-0.4.4/impactchart/model.py` & `impactchart-0.5.0/impactchart/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import shap.maskers
 from matplotlib.ticker import Formatter, FuncFormatter, PercentFormatter
 from scipy import stats
-from shap import Explainer
+from shap import Explainer, TreeExplainer
 from sklearn.base import BaseEstimator
 from sklearn.linear_model import LinearRegression
 from sklearn.model_selection import RandomizedSearchCV
 from sklearn.neighbors import KNeighborsRegressor
 from xgboost import XGBRegressor
 
 
@@ -141,14 +141,17 @@
         if self._optimize_hyperparameters:
             params = self.optimize_hyperparameters(
                 X,
                 y,
                 sample_weight=sample_weight,
                 optimization_scoring_metric=optimization_scoring_metric,
             )
+            # Put the estimator kwargs back in. Mainly for things like
+            # enable_categorical=True.
+            params |= self._estimator_kwargs
         else:
             params = self._estimator_kwargs
 
         estimators = [self.estimator(**params) for _ in range(self._ensemble_size)]
         return estimators
 
     def _training_sample(
@@ -317,14 +320,21 @@
 
         Returns
         -------
             The name of the algorithm.
         """
         return "auto"
 
+    def explainer(self, estimator, X: pd.DataFrame):
+        return Explainer(
+            estimator,
+            masker=self._masker(X),
+            algorithm=self.explainer_algorithm,
+        )
+
     def _estimator_impact(
         self, X: pd.DataFrame, estimator, estimator_id
     ) -> pd.DataFrame:
         """
         Generate the impact of each feature for a given estimator.
 
         Parameters
@@ -338,19 +348,15 @@
             that the impacts came from.
         Returns
         -------
             A dataframe with columns for the impact of each feature and an added `id`
             column with the value we were given, for identification purposes.
         """
         df = pd.DataFrame(
-            Explainer(
-                estimator,
-                masker=self._masker(X),
-                algorithm=self.explainer_algorithm,
-            )(X).values,
+            self.explainer(estimator, X)(X).values,
             columns=X.columns,
         )
         df["estimator"] = estimator_id
         return df
 
     def impact(self, X: pd.DataFrame) -> pd.DataFrame:
         """
@@ -494,15 +500,19 @@
     _formatter_for_arg_value = {
         "percentage": _percent_formatter,
         "dollar": _dollar_formatter,
         "comma": _comma_formatter,
     }
 
     @classmethod
-    def _axis_formatter(cls, formatter: Formatter | str) -> Formatter:
+    def _axis_formatter(
+        cls, formatter: Optional[Formatter | str] = None
+    ) -> Formatter | None:
+        if formatter is None:
+            return None
         if isinstance(formatter, Formatter):
             return formatter
         else:
             return cls._formatter_for_arg_value[formatter]
 
     def impact_charts(
         self,
@@ -514,15 +524,15 @@
         ensemble_markersize: int = 2,
         ensemble_color: str = "lightgray",
         plot_kwargs: Optional[Dict[str, Any]] = None,
         subplots_kwargs: Optional[Dict[str, Any]] = None,
         feature_names: Optional[Callable[[str], str] | Mapping[str, str]] = None,
         y_name: Optional[str] = None,
         subtitle: Optional[str] = None,
-        y_formatter: str = "comma",
+        y_formatter: Optional[str] = None,
         x_formatter_default: str = "comma",
         x_formatters: Optional[Dict[str, str]] = None,
     ) -> Dict[str, Tuple[plt.Figure, plt.Axes]]:
         """
         Generate impact charts for a set of features.
 
         Parameters
@@ -663,20 +673,24 @@
             ax.set_xlabel(feature_name)
             ax.grid()
 
             for handle in ax.legend().legend_handles:
                 handle._sizes = [25]
 
             # Format the axes.
-            ax.yaxis.set_major_formatter(self._axis_formatter(y_formatter))
+            y_axis_formatter = self._axis_formatter(y_formatter)
+            if y_axis_formatter is not None:
+                ax.yaxis.set_major_formatter(y_axis_formatter)
             if x_formatters is not None and feature in x_formatters:
                 x_formatter = x_formatters[feature]
             else:
                 x_formatter = x_formatter_default
-            ax.xaxis.set_major_formatter(self._axis_formatter(x_formatter))
+            x_axis_formatter = self._axis_formatter(x_formatter)
+            if x_axis_formatter is not None:
+                ax.xaxis.set_major_formatter(x_axis_formatter)
 
             if self._plot_id is not None:
                 plot_id = self._plot_id_string(feature, len(X.index))
                 ax.text(
                     0.99,
                     0.02,
                     plot_id,
@@ -790,14 +804,35 @@
         )
 
         self._parameter_distributions = parameter_distributions
 
     def estimator(self, **kwargs) -> BaseEstimator:
         return XGBRegressor(**kwargs)
 
+    def explainer(self, estimator, X: pd.DataFrame):
+        has_categorical_features = False
+
+        for col in X.columns:
+            if X[col].dtype == "category":
+                has_categorical_features = True
+                break
+
+        if has_categorical_features:
+            # When categorical features are present, we have to uss
+            # feature_perturbation="tree_path_dependent".
+            return TreeExplainer(estimator, feature_perturbation="tree_path_dependent")
+        else:
+            # Otherwise, we will use the default feature_perturbation="interventional",
+            # which will run slower but will do causal inference. A sample of 1,000
+            # rows should be sufficient and will reduce large runtime overhead.
+            if len(X.index) > 1000:
+                X = X.sample(n=1000, random_state=self.initial_random_state)
+
+            return TreeExplainer(estimator, X, feature_perturbation="interventional")
+
     def optimize_hyperparameters(
         self,
         X: pd.DataFrame,
         y: pd.Series,
         sample_weight: Optional[pd.Series] = None,
         *,
         optimization_scoring_metric: Optional[str] = None,
```

### Comparing `impactchart-0.4.4/pyproject.toml` & `impactchart-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "impactchart"
-version = "0.4.4"
+version = "0.5.0"
 description = "A package for generating impact charts."
 license = "HL3-CL-ECO-EXTR-FFD-LAW-MIL-SV"
 authors = ["Darren Vengroff"]
 readme = "README.md"
 repository = "https://github.com/vengroff/impactchart"
 keywords = ["impact charts", "regression", "machine learning", "analysis"]
 classifiers = [
```

### Comparing `impactchart-0.4.4/PKG-INFO` & `impactchart-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: impactchart
-Version: 0.4.4
+Version: 0.5.0
 Summary: A package for generating impact charts.
 Home-page: https://github.com/vengroff/impactchart
 License: HL3-CL-ECO-EXTR-FFD-LAW-MIL-SV
 Keywords: impact charts,regression,machine learning,analysis
 Author: Darren Vengroff
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
```

