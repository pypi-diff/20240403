# Comparing `tmp/sklearn_viz-0.3.0.tar.gz` & `tmp/sklearn_viz-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearn_viz-0.3.0.tar", max compression
+gzip compressed data, was "sklearn_viz-0.3.1.tar", max compression
```

## Comparing `sklearn_viz-0.3.0.tar` & `sklearn_viz-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        0 2023-08-27 06:10:46.929402 sklearn_viz-0.3.0/elphick/sklearn_viz/__init__.py
--rw-r--r--   0        0        0      334 2023-09-18 13:02:51.287832 sklearn_viz-0.3.0/elphick/sklearn_viz/features/__init__.py
--rw-r--r--   0        0        0     7873 2023-10-10 12:02:36.000498 sklearn_viz-0.3.0/elphick/sklearn_viz/features/importance.py
--rw-r--r--   0        0        0     4738 2024-03-30 11:59:00.677281 sklearn_viz-0.3.0/elphick/sklearn_viz/features/outlier_detection.py
--rw-r--r--   0        0        0     2471 2024-03-30 11:59:00.682932 sklearn_viz-0.3.0/elphick/sklearn_viz/features/parallel_coordinates.py
--rw-r--r--   0        0        0    16988 2024-03-30 11:59:00.688949 sklearn_viz-0.3.0/elphick/sklearn_viz/features/principal_components.py
--rw-r--r--   0        0        0      668 2023-09-18 11:19:59.559906 sklearn_viz-0.3.0/elphick/sklearn_viz/features/scatter_matrix.py
--rw-r--r--   0        0        0      131 2023-09-18 13:02:51.313708 sklearn_viz-0.3.0/elphick/sklearn_viz/model_selection/__init__.py
--rw-r--r--   0        0        0     6246 2023-09-11 12:55:18.110947 sklearn_viz-0.3.0/elphick/sklearn_viz/model_selection/learning_curve.py
--rw-r--r--   0        0        0     1469 2023-11-15 12:38:46.317925 sklearn_viz-0.3.0/elphick/sklearn_viz/model_selection/metrics.py
--rw-r--r--   0        0        0    22155 2024-04-01 11:49:20.249010 sklearn_viz-0.3.0/elphick/sklearn_viz/model_selection/model_selection.py
--rw-r--r--   0        0        0     2552 2023-09-11 12:55:18.114966 sklearn_viz-0.3.0/elphick/sklearn_viz/model_selection/models.py
--rw-r--r--   0        0        0      318 2023-11-12 09:19:44.575578 sklearn_viz-0.3.0/elphick/sklearn_viz/model_selection/scorers.py
--rw-r--r--   0        0        0       22 2023-09-17 08:40:15.220711 sklearn_viz-0.3.0/elphick/sklearn_viz/residuals/__init__.py
--rw-r--r--   0        0        0     2120 2023-09-05 09:52:35.543294 sklearn_viz-0.3.0/elphick/sklearn_viz/residuals/error.py
--rw-r--r--   0        0        0       28 2023-08-27 06:10:46.931314 sklearn_viz-0.3.0/elphick/sklearn_viz/utils/__init__.py
--rw-r--r--   0        0        0     3191 2023-08-27 06:10:46.931314 sklearn_viz-0.3.0/elphick/sklearn_viz/utils/timer.py
--rw-r--r--   0        0        0     1090 2023-08-27 06:10:46.917578 sklearn_viz-0.3.0/LICENSE
--rw-r--r--   0        0        0      819 2024-04-01 11:42:33.970861 sklearn_viz-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      362 2023-08-27 06:10:46.918992 sklearn_viz-0.3.0/README.md
--rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 sklearn_viz-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-08-27 06:10:46.929402 sklearn_viz-0.3.1/elphick/sklearn_viz/__init__.py
+-rw-r--r--   0        0        0      334 2023-09-18 13:02:51.287832 sklearn_viz-0.3.1/elphick/sklearn_viz/features/__init__.py
+-rw-r--r--   0        0        0     7873 2023-10-10 12:02:36.000498 sklearn_viz-0.3.1/elphick/sklearn_viz/features/importance.py
+-rw-r--r--   0        0        0     4738 2024-03-30 11:59:00.677281 sklearn_viz-0.3.1/elphick/sklearn_viz/features/outlier_detection.py
+-rw-r--r--   0        0        0     2471 2024-03-30 11:59:00.682932 sklearn_viz-0.3.1/elphick/sklearn_viz/features/parallel_coordinates.py
+-rw-r--r--   0        0        0    16988 2024-03-30 11:59:00.688949 sklearn_viz-0.3.1/elphick/sklearn_viz/features/principal_components.py
+-rw-r--r--   0        0        0      668 2023-09-18 11:19:59.559906 sklearn_viz-0.3.1/elphick/sklearn_viz/features/scatter_matrix.py
+-rw-r--r--   0        0        0      131 2023-09-18 13:02:51.313708 sklearn_viz-0.3.1/elphick/sklearn_viz/model_selection/__init__.py
+-rw-r--r--   0        0        0     6246 2023-09-11 12:55:18.110947 sklearn_viz-0.3.1/elphick/sklearn_viz/model_selection/learning_curve.py
+-rw-r--r--   0        0        0     1469 2024-04-02 23:43:43.297303 sklearn_viz-0.3.1/elphick/sklearn_viz/model_selection/metrics.py
+-rw-r--r--   0        0        0    20963 2024-04-02 23:43:43.308707 sklearn_viz-0.3.1/elphick/sklearn_viz/model_selection/model_selection.py
+-rw-r--r--   0        0        0     2552 2023-09-11 12:55:18.114966 sklearn_viz-0.3.1/elphick/sklearn_viz/model_selection/models.py
+-rw-r--r--   0        0        0      318 2023-11-12 09:19:44.575578 sklearn_viz-0.3.1/elphick/sklearn_viz/model_selection/scorers.py
+-rw-r--r--   0        0        0       22 2023-09-17 08:40:15.220711 sklearn_viz-0.3.1/elphick/sklearn_viz/residuals/__init__.py
+-rw-r--r--   0        0        0     2120 2023-09-05 09:52:35.543294 sklearn_viz-0.3.1/elphick/sklearn_viz/residuals/error.py
+-rw-r--r--   0        0        0       28 2023-08-27 06:10:46.931314 sklearn_viz-0.3.1/elphick/sklearn_viz/utils/__init__.py
+-rw-r--r--   0        0        0     3191 2023-08-27 06:10:46.931314 sklearn_viz-0.3.1/elphick/sklearn_viz/utils/timer.py
+-rw-r--r--   0        0        0     1090 2023-08-27 06:10:46.917578 sklearn_viz-0.3.1/LICENSE
+-rw-r--r--   0        0        0      819 2024-04-02 23:43:43.333160 sklearn_viz-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      362 2023-08-27 06:10:46.918992 sklearn_viz-0.3.1/README.md
+-rw-r--r--   0        0        0     1008 1970-01-01 00:00:00.000000 sklearn_viz-0.3.1/PKG-INFO
```

### Comparing `sklearn_viz-0.3.0/elphick/sklearn_viz/features/importance.py` & `sklearn_viz-0.3.1/elphick/sklearn_viz/features/importance.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.3.0/elphick/sklearn_viz/features/outlier_detection.py` & `sklearn_viz-0.3.1/elphick/sklearn_viz/features/outlier_detection.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.3.0/elphick/sklearn_viz/features/parallel_coordinates.py` & `sklearn_viz-0.3.1/elphick/sklearn_viz/features/parallel_coordinates.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.3.0/elphick/sklearn_viz/features/principal_components.py` & `sklearn_viz-0.3.1/elphick/sklearn_viz/features/principal_components.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.3.0/elphick/sklearn_viz/features/scatter_matrix.py` & `sklearn_viz-0.3.1/elphick/sklearn_viz/features/scatter_matrix.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.3.0/elphick/sklearn_viz/model_selection/learning_curve.py` & `sklearn_viz-0.3.1/elphick/sklearn_viz/model_selection/learning_curve.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.3.0/elphick/sklearn_viz/model_selection/metrics.py` & `sklearn_viz-0.3.1/elphick/sklearn_viz/model_selection/metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 
 def r2(y_true, y_est):
     ssr = ((y_true - y_est) ** 2).sum()
     sst = ((y_true - y_true.mean()) ** 2).sum()
     return 1 - (ssr / sst)
 
 
-regression_metrics = {'me': mean_error,
-                      'r2_score': r2_score,
+regression_metrics = {'r2_score': r2_score,
+                      'me': mean_error,
                       'r2': r2,
                       'mae': mean_absolute_error,
                       'mse': mean_squared_error,
                       'rmse': partial(mean_squared_error, squared=False),
                       'moe': partial(moe_95, metric='moe'),
                       'moe_lo': partial(moe_95, metric='lo'),
                       'moe_hi': partial(moe_95, metric='hi')}
```

### Comparing `sklearn_viz-0.3.0/elphick/sklearn_viz/model_selection/model_selection.py` & `sklearn_viz-0.3.1/elphick/sklearn_viz/model_selection/model_selection.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import logging
-from typing import Union, Optional, Dict, List, Callable, Any, Tuple
+from typing import Union, Optional, Dict, List, Callable, Tuple
 
 import matplotlib
 import numpy as np
 import pandas as pd
-
 import plotly.graph_objects as go
 import sklearn
 from plotly import colors
 from plotly.subplots import make_subplots
 from sklearn import model_selection
 from sklearn.base import is_classifier, is_regressor
 from sklearn.model_selection import cross_validate
 from sklearn.pipeline import Pipeline
 
 from elphick.sklearn_viz.model_selection.metrics import regression_metrics, classification_metrics
 from elphick.sklearn_viz.model_selection.scorers import classification_scorers, regression_scorers
-from elphick.sklearn_viz.utils import log_timer
 
 
 def subplot_index(idx: int, col_wrap: int) -> Tuple[int, int]:
     col: int = int(idx % col_wrap + 1)
     row: int = int(np.floor(idx / col_wrap) + 1)
     return row, col
 
@@ -130,15 +128,15 @@
                 results[data_key] = {}
                 x: pd.DataFrame = data[self.features_in]
                 y: pd.DataFrame = data[self.target]
                 if self.pre_processor:
                     x = self.pre_processor.set_output(transform="pandas").fit_transform(X=x)
 
                 for algo_key, algo in self.algorithms.items():
-                    kfold = model_selection.KFold(n_splits=self.k_folds, random_state=self.random_state)
+                    kfold = model_selection.KFold(n_splits=self.k_folds, random_state=self.random_state, shuffle=True)
                     res = cross_validate(algo, x, y, cv=kfold, scoring=self.scorer, **cv_kwargs)
                     if self.metrics is not None:
                         res['metrics'], res['metrics_group'] = self.calculate_metrics(x=x, y=y,
                                                                                       estimators=res['estimator'],
                                                                                       indices=res['indices'],
                                                                                       group=self.group)
                     results[data_key][algo_key] = res
@@ -248,15 +246,15 @@
                                title: Optional[str] = None,
                                col_wrap: Optional[int] = None) -> go.Figure:
         """Plot the category feature analysis
 
         Args:
             algorithm: If supplied, this will be the name of the algorithm tested.  If None the first algorithm is used.
             dataset: If supplied, this will be the name of the dataset tested.  If None the first dataset is used.
-            metrics: The metric or metrics to plot in addition to the scorer.  Each metric will be plotted in a
+            metrics: The metric or metrics to show.  Each metric will be plotted in a
              separate panel.
             title: Title of the plot
             col_wrap: If plotting multiple metrics, col_wrap will wrap columns to new rows, resulting in
              col-wrap columns, and multiple rows.
 
         Returns:
             a plotly GraphObjects.Figure
@@ -268,62 +266,43 @@
             raise KeyError(f"Algorithm {algorithm} is not in the list of available algorithms: {algorithms}")
 
         datasets: list[str] = list(self.datasets.keys())
         dataset: str = datasets[0] if dataset is None else dataset
         if dataset not in datasets:
             raise KeyError(f"Dataset {dataset} is not in the list of available datasets: {datasets}")
 
-        baseline_scores: pd.DataFrame = self.get_cv_scores()[[(dataset, algorithm)]]
-        baseline_scores.columns = ['baseline']
+        metrics: list[str] = [list(self.metrics.keys())[0]] if metrics is None else metrics
+
         baseline_metrics: pd.DataFrame = self.get_cv_metrics(metrics, by_group=True).loc[
             (slice(None), dataset, algorithm)]
         baseline_metrics = baseline_metrics.melt(id_vars=['metric'], value_vars=self.group.unique().tolist(),
                                                  var_name='group',
                                                  ignore_index=False).assign(model='baseline')
 
         # cross-validate the individual models
         by_group_metrics, by_group_scores = self.get_model_by_group_data(algorithm, dataset)
         by_group_metrics = by_group_metrics.melt(id_vars=['group'], value_vars=metrics, var_name='metric',
                                                  ignore_index=False).assign(model='by_group')
         metric_data: pd.DataFrame = pd.concat([baseline_metrics, by_group_metrics]).sort_values(['model', 'metric'])
         metric_data = metric_data.set_index(['metric', 'group'], append=True).pivot(columns='model',
                                                                                     values='value').reset_index(
             'metric')
-        score_data = pd.concat([baseline_scores, by_group_scores], axis=1)
-        score_relative = score_data[[col for col in score_data.columns if col != 'baseline']].div(
-            score_data['baseline'], axis=0)
 
-        vmin, vmax = 0.8, 1.2
-        norm = matplotlib.colors.Normalize(vmin=vmin, vmax=vmax)
-        cmap = matplotlib.cm.get_cmap('RdYlGn')
-
-        subtitle: str = f'Model by Group Test with {self.k_folds} folds'
         if title is None:
-            title = subtitle
-        else:
-            title = title + '<br>' + subtitle
+            title = f'Model by Group Test on {algorithm} with {self.k_folds} folds'
 
-        num_plots: int = len(metrics) + 1 if len(metrics) > 0 else 1
+        num_plots: int = len(metrics) if len(metrics) > 0 else 1
         num_cols: int = num_plots if col_wrap is None else col_wrap
-        num_rows, _ = subplot_index(len(metrics), col_wrap=num_cols)
+        num_rows, _ = subplot_index(len(metrics) - 1, col_wrap=num_cols)
         fig = make_subplots(rows=num_rows, cols=num_cols,
-                            subplot_titles=[f'Relative Score ({self.scorer})<br>(by group / baseline)'] + metrics)
-
-        # scorer
-        for col in score_relative.columns:
-            # For the scorer build the plot by column to color individually based on score
-            median = np.median(score_relative[col])  # find the median
-            color = 'rgb' + str(cmap(norm(median))[0:3])  # normalize
-            fig.add_trace(go.Box(y=score_relative[col], name=col, boxpoints='all', notched=True, fillcolor=color,
-                                 line={"color": "grey"}, marker={"color": "grey"}, showlegend=False,
-                                 offsetgroup='A'), row=1, col=1)
+                            subplot_titles=metrics)
 
         # metrics
         for i, metric in enumerate(metrics):
-            row, col = subplot_index(i + 1, col_wrap=num_cols)
+            row, col = subplot_index(i, col_wrap=num_cols)
             colorscale = colors.qualitative.Plotly
             add_to_legend = True if i == 0 else False
             df_metric: pd.DataFrame = metric_data.query('metric==@metric').drop(columns=['metric'])
             x = df_metric.index.get_level_values('group')
             for g, grp in enumerate(df_metric.columns):
                 fig.add_trace(go.Box(x=x, y=df_metric[grp], name=grp, boxpoints='all', notched=True,
                                      legendgroup=self.group.name,
@@ -344,15 +323,15 @@
         by_group_metric_chunks: list = []
         for grp in self.group.unique():
             grp_index: pd.Index = self.group.loc[self.group == grp].index
             x: pd.DataFrame = self.datasets[dataset][self.features_in].loc[grp_index]
             y: pd.DataFrame = self.datasets[dataset][self.target].loc[grp_index]
             if self.pre_processor:
                 x = self.pre_processor.set_output(transform="pandas").fit_transform(X=x)
-            kfold = model_selection.KFold(n_splits=self.k_folds, random_state=self.random_state)
+            kfold = model_selection.KFold(n_splits=self.k_folds, random_state=self.random_state, shuffle=True)
             res = cross_validate(self.algorithms[algorithm], x, y, cv=kfold, scoring=self.scorer, return_estimator=True,
                                  return_indices=True)
             by_group_score_chunks.append(pd.Series(res['test_score'], name=grp))
             if self.metrics is not None:
                 res['metrics'], _ = self.calculate_metrics(x=x, y=y,
                                                            estimators=res['estimator'],
                                                            indices=res['indices'],
```

### Comparing `sklearn_viz-0.3.0/elphick/sklearn_viz/model_selection/models.py` & `sklearn_viz-0.3.1/elphick/sklearn_viz/model_selection/models.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.3.0/elphick/sklearn_viz/residuals/error.py` & `sklearn_viz-0.3.1/elphick/sklearn_viz/residuals/error.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.3.0/elphick/sklearn_viz/utils/timer.py` & `sklearn_viz-0.3.1/elphick/sklearn_viz/utils/timer.py`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.3.0/LICENSE` & `sklearn_viz-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sklearn_viz-0.3.0/pyproject.toml` & `sklearn_viz-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sklearn-viz"
-version = "0.3.0"
+version = "0.3.1"
 description = ""
 authors = ["Greg <11791585+elphick@users.noreply.github.com>"]
 readme = "README.md"
 packages = [{ include = "elphick/sklearn_viz" }]
 
 [[tool.poetry.source]]
 name = "PyPI"
```

### Comparing `sklearn_viz-0.3.0/PKG-INFO` & `sklearn_viz-0.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearn-viz
-Version: 0.3.0
+Version: 0.3.1
 Summary: 
 Author: Greg
 Author-email: 11791585+elphick@users.noreply.github.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

