# Comparing `tmp/concrete_ml-1.5.0rc0-py3-none-any.whl.zip` & `tmp/concrete_ml-1.5.0rc1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,63 +1,72 @@
-Zip file size: 226390 bytes, number of entries: 61
+Zip file size: 248946 bytes, number of entries: 70
 -rw-r--r--  2.0 unx      284 b- defN 80-Jan-01 00:00 concrete/__init__.py
 -rw-r--r--  2.0 unx       51 b- defN 80-Jan-01 00:00 concrete/ml/__init__.py
 -rw-r--r--  2.0 unx       95 b- defN 80-Jan-01 00:00 concrete/ml/common/__init__.py
 -rw-r--r--  2.0 unx     2519 b- defN 80-Jan-01 00:00 concrete/ml/common/check_inputs.py
 -rw-r--r--  2.0 unx      101 b- defN 80-Jan-01 00:00 concrete/ml/common/debugging/__init__.py
 -rw-r--r--  2.0 unx     2377 b- defN 80-Jan-01 00:00 concrete/ml/common/debugging/custom_assert.py
 -rw-r--r--  2.0 unx     1152 b- defN 80-Jan-01 00:00 concrete/ml/common/serialization/__init__.py
 -rw-r--r--  2.0 unx     8375 b- defN 80-Jan-01 00:00 concrete/ml/common/serialization/decoder.py
 -rw-r--r--  2.0 unx      601 b- defN 80-Jan-01 00:00 concrete/ml/common/serialization/dumpers.py
 -rw-r--r--  2.0 unx    12167 b- defN 80-Jan-01 00:00 concrete/ml/common/serialization/encoder.py
 -rw-r--r--  2.0 unx      743 b- defN 80-Jan-01 00:00 concrete/ml/common/serialization/loaders.py
--rw-r--r--  2.0 unx    19738 b- defN 80-Jan-01 00:00 concrete/ml/common/utils.py
+-rw-r--r--  2.0 unx    21759 b- defN 80-Jan-01 00:00 concrete/ml/common/utils.py
 -rw-r--r--  2.0 unx      235 b- defN 80-Jan-01 00:00 concrete/ml/deployment/Dockerfile.server
 -rw-r--r--  2.0 unx      121 b- defN 80-Jan-01 00:00 concrete/ml/deployment/__init__.py
 -rw-r--r--  2.0 unx    17918 b- defN 80-Jan-01 00:00 concrete/ml/deployment/deploy_to_aws.py
 -rw-r--r--  2.0 unx     3800 b- defN 80-Jan-01 00:00 concrete/ml/deployment/deploy_to_docker.py
 -rw-r--r--  2.0 unx    12989 b- defN 80-Jan-01 00:00 concrete/ml/deployment/fhe_client_server.py
 -rw-r--r--  2.0 unx     2590 b- defN 80-Jan-01 00:00 concrete/ml/deployment/server.py
 -rw-r--r--  2.0 unx       33 b- defN 80-Jan-01 00:00 concrete/ml/deployment/server_requirements.txt
 -rw-r--r--  2.0 unx     3293 b- defN 80-Jan-01 00:00 concrete/ml/deployment/utils.py
 -rw-r--r--  2.0 unx       19 b- defN 80-Jan-01 00:00 concrete/ml/onnx/__init__.py
 -rw-r--r--  2.0 unx    11430 b- defN 80-Jan-01 00:00 concrete/ml/onnx/convert.py
 -rw-r--r--  2.0 unx    11573 b- defN 80-Jan-01 00:00 concrete/ml/onnx/onnx_impl_utils.py
 -rw-r--r--  2.0 unx    11003 b- defN 80-Jan-01 00:00 concrete/ml/onnx/onnx_model_manipulations.py
 -rw-r--r--  2.0 unx    23174 b- defN 80-Jan-01 00:00 concrete/ml/onnx/onnx_utils.py
--rw-r--r--  2.0 unx    67978 b- defN 80-Jan-01 00:00 concrete/ml/onnx/ops_impl.py
+-rw-r--r--  2.0 unx    67985 b- defN 80-Jan-01 00:00 concrete/ml/onnx/ops_impl.py
+-rw-r--r--  2.0 unx     4183 b- defN 80-Jan-01 00:00 concrete/ml/pandas/__init__.py
+-rw-r--r--  2.0 unx      594 b- defN 80-Jan-01 00:00 concrete/ml/pandas/_client_server_files/client.zip
+-rw-r--r--  2.0 unx     1382 b- defN 80-Jan-01 00:00 concrete/ml/pandas/_client_server_files/server.zip
+-rw-r--r--  2.0 unx     6572 b- defN 80-Jan-01 00:00 concrete/ml/pandas/_development.py
+-rw-r--r--  2.0 unx    17264 b- defN 80-Jan-01 00:00 concrete/ml/pandas/_operators.py
+-rw-r--r--  2.0 unx    12823 b- defN 80-Jan-01 00:00 concrete/ml/pandas/_processing.py
+-rw-r--r--  2.0 unx     6485 b- defN 80-Jan-01 00:00 concrete/ml/pandas/_utils.py
+-rw-r--r--  2.0 unx     3558 b- defN 80-Jan-01 00:00 concrete/ml/pandas/client_engine.py
+-rw-r--r--  2.0 unx    12603 b- defN 80-Jan-01 00:00 concrete/ml/pandas/dataframe.py
 -rw-r--r--  2.0 unx      101 b- defN 80-Jan-01 00:00 concrete/ml/pytest/__init__.py
 -rw-r--r--  2.0 unx    47491 b- defN 80-Jan-01 00:00 concrete/ml/pytest/torch_models.py
--rw-r--r--  2.0 unx    25505 b- defN 80-Jan-01 00:00 concrete/ml/pytest/utils.py
+-rw-r--r--  2.0 unx    27970 b- defN 80-Jan-01 00:00 concrete/ml/pytest/utils.py
 -rw-r--r--  2.0 unx     1180 b- defN 80-Jan-01 00:00 concrete/ml/quantization/__init__.py
--rw-r--r--  2.0 unx    42163 b- defN 80-Jan-01 00:00 concrete/ml/quantization/base_quantized_op.py
--rw-r--r--  2.0 unx    48516 b- defN 80-Jan-01 00:00 concrete/ml/quantization/post_training.py
+-rw-r--r--  2.0 unx    43545 b- defN 80-Jan-01 00:00 concrete/ml/quantization/base_quantized_op.py
+-rw-r--r--  2.0 unx    49245 b- defN 80-Jan-01 00:00 concrete/ml/quantization/post_training.py
 -rw-r--r--  2.0 unx     1014 b- defN 80-Jan-01 00:00 concrete/ml/quantization/qat_quantizers.py
--rw-r--r--  2.0 unx    30981 b- defN 80-Jan-01 00:00 concrete/ml/quantization/quantized_module.py
+-rw-r--r--  2.0 unx    30980 b- defN 80-Jan-01 00:00 concrete/ml/quantization/quantized_module.py
 -rw-r--r--  2.0 unx    13734 b- defN 80-Jan-01 00:00 concrete/ml/quantization/quantized_module_passes.py
 -rw-r--r--  2.0 unx    98341 b- defN 80-Jan-01 00:00 concrete/ml/quantization/quantized_ops.py
 -rw-r--r--  2.0 unx    37300 b- defN 80-Jan-01 00:00 concrete/ml/quantization/quantizers.py
 -rw-r--r--  2.0 unx       77 b- defN 80-Jan-01 00:00 concrete/ml/search_parameters/__init__.py
 -rw-r--r--  2.0 unx    21230 b- defN 80-Jan-01 00:00 concrete/ml/search_parameters/p_error_search.py
 -rw-r--r--  2.0 unx    10315 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/__init__.py
 -rw-r--r--  2.0 unx     3385 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/_fhe_training_utils.py
--rw-r--r--  2.0 unx    89334 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/base.py
+-rw-r--r--  2.0 unx    89274 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/base.py
 -rw-r--r--  2.0 unx    12899 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/glm.py
 -rw-r--r--  2.0 unx    67262 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/linear_model.py
 -rw-r--r--  2.0 unx     6121 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/neighbors.py
 -rw-r--r--  2.0 unx    32101 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/qnn.py
 -rw-r--r--  2.0 unx    14188 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/qnn_module.py
 -rw-r--r--  2.0 unx    11440 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/rf.py
 -rw-r--r--  2.0 unx     8897 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/svm.py
 -rw-r--r--  2.0 unx    10500 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/tree.py
 -rw-r--r--  2.0 unx    19152 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/tree_to_numpy.py
 -rw-r--r--  2.0 unx    19694 b- defN 80-Jan-01 00:00 concrete/ml/sklearn/xgb.py
 -rw-r--r--  2.0 unx       83 b- defN 80-Jan-01 00:00 concrete/ml/torch/__init__.py
--rw-r--r--  2.0 unx    23432 b- defN 80-Jan-01 00:00 concrete/ml/torch/compile.py
--rw-r--r--  2.0 unx    32328 b- defN 80-Jan-01 00:00 concrete/ml/torch/hybrid_model.py
+-rw-r--r--  2.0 unx    24629 b- defN 80-Jan-01 00:00 concrete/ml/torch/compile.py
+-rw-r--r--  2.0 unx    32373 b- defN 80-Jan-01 00:00 concrete/ml/torch/hybrid_model.py
 -rw-r--r--  2.0 unx     3167 b- defN 80-Jan-01 00:00 concrete/ml/torch/numpy_module.py
 -rw-r--r--  2.0 unx      128 b- defN 80-Jan-01 00:00 concrete/ml/version.py
--rw-r--r--  2.0 unx     1546 b- defN 80-Jan-01 00:00 concrete_ml-1.5.0rc0.dist-info/LICENSE
--rw-r--r--  2.0 unx    16441 b- defN 80-Jan-01 00:00 concrete_ml-1.5.0rc0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 concrete_ml-1.5.0rc0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     5570 b- defN 16-Jan-01 00:00 concrete_ml-1.5.0rc0.dist-info/RECORD
-61 files, 970063 bytes uncompressed, 217456 bytes compressed:  77.6%
+-rw-r--r--  2.0 unx     1546 b- defN 80-Jan-01 00:00 concrete_ml-1.5.0rc1.dist-info/LICENSE
+-rw-r--r--  2.0 unx    16396 b- defN 80-Jan-01 00:00 concrete_ml-1.5.0rc1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 concrete_ml-1.5.0rc1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     6408 b- defN 16-Jan-01 00:00 concrete_ml-1.5.0rc1.dist-info/RECORD
+70 files, 1044105 bytes uncompressed, 238682 bytes compressed:  77.1%
```

## zipnote {}

```diff
@@ -72,14 +72,41 @@
 
 Filename: concrete/ml/onnx/onnx_utils.py
 Comment: 
 
 Filename: concrete/ml/onnx/ops_impl.py
 Comment: 
 
+Filename: concrete/ml/pandas/__init__.py
+Comment: 
+
+Filename: concrete/ml/pandas/_client_server_files/client.zip
+Comment: 
+
+Filename: concrete/ml/pandas/_client_server_files/server.zip
+Comment: 
+
+Filename: concrete/ml/pandas/_development.py
+Comment: 
+
+Filename: concrete/ml/pandas/_operators.py
+Comment: 
+
+Filename: concrete/ml/pandas/_processing.py
+Comment: 
+
+Filename: concrete/ml/pandas/_utils.py
+Comment: 
+
+Filename: concrete/ml/pandas/client_engine.py
+Comment: 
+
+Filename: concrete/ml/pandas/dataframe.py
+Comment: 
+
 Filename: concrete/ml/pytest/__init__.py
 Comment: 
 
 Filename: concrete/ml/pytest/torch_models.py
 Comment: 
 
 Filename: concrete/ml/pytest/utils.py
@@ -165,20 +192,20 @@
 
 Filename: concrete/ml/torch/numpy_module.py
 Comment: 
 
 Filename: concrete/ml/version.py
 Comment: 
 
-Filename: concrete_ml-1.5.0rc0.dist-info/LICENSE
+Filename: concrete_ml-1.5.0rc1.dist-info/LICENSE
 Comment: 
 
-Filename: concrete_ml-1.5.0rc0.dist-info/METADATA
+Filename: concrete_ml-1.5.0rc1.dist-info/METADATA
 Comment: 
 
-Filename: concrete_ml-1.5.0rc0.dist-info/WHEEL
+Filename: concrete_ml-1.5.0rc1.dist-info/WHEEL
 Comment: 
 
-Filename: concrete_ml-1.5.0rc0.dist-info/RECORD
+Filename: concrete_ml-1.5.0rc1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## concrete/ml/common/utils.py

```diff
@@ -5,14 +5,15 @@
 from functools import partial
 from types import FunctionType
 from typing import Any, Callable, Dict, Iterable, List, Optional, Tuple, Union
 
 import numpy
 import onnx
 import torch
+from concrete.fhe import Exactness
 from concrete.fhe.dtypes import Integer
 from sklearn.base import is_classifier, is_regressor
 
 from ..common.check_inputs import check_array_and_assert
 from ..common.debugging import assert_true
 
 _VALID_ARG_CHARS = set(string.ascii_letters).union(str(i) for i in range(10)).union(("_",))
@@ -32,17 +33,15 @@
 
 SUPPORTED_TYPES = {**SUPPORTED_FLOAT_TYPES, **SUPPORTED_INT_TYPES}
 
 MAX_BITWIDTH_BACKWARD_COMPATIBLE = 8
 
 # Indicate if the old virtual library method should be used instead of the compiler simulation
 # when simulating FHE executions
-# Set 'USE_OLD_VL' to False by default once the new simulation is fixed
-# FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/4091
-USE_OLD_VL = True
+USE_OLD_VL = False
 
 # Debug option for testing round PBS optimization
 # Setting this option to true will make quantizers "round half up"
 # For example: 0.5 -> 1, 1.5 -> 2 instead of "round half to even"
 # When the option is set to false, Concrete ML uses numpy.rint
 # which has the same behavior as torch.round -> Brevitas nets
 # should be exact compared to their Concrete ML QuantizedModule
@@ -603,7 +602,54 @@
             tolerances, False otherwise.
     """
 
     assert isinstance(a, numpy.ndarray)
     assert isinstance(b, numpy.ndarray)
 
     return a.shape == b.shape and numpy.allclose(a, b, rtol, atol, equal_nan)
+
+
+def process_rounding_threshold_bits(rounding_threshold_bits):
+    """Check and process the rounding_threshold_bits parameter.
+
+    Args:
+        rounding_threshold_bits (Union[None, int, Dict[str, Union[str, int]]]): Defines precision
+            rounding for model accumulators. Accepts None, an int, or a dict.
+            The dict can specify 'method' (fhe.Exactness.EXACT or fhe.Exactness.APPROXIMATE)
+            and 'n_bits' ('auto' or int)
+
+    Returns:
+        Dict[str, Union[str, int]]: Processed rounding_threshold_bits dictionary.
+
+    Raises:
+        NotImplementedError: If 'auto' rounding is specified but not implemented.
+        ValueError: If an invalid type or value is provided for rounding_threshold_bits.
+    """
+    n_bits_rounding: Union[None, str, int] = None
+    method: Exactness = Exactness.EXACT
+
+    # Only process if rounding_threshold_bits is not None
+    if rounding_threshold_bits is not None:
+        if isinstance(rounding_threshold_bits, int):
+            n_bits_rounding = rounding_threshold_bits
+        elif isinstance(rounding_threshold_bits, dict):
+            n_bits_rounding = rounding_threshold_bits.get("n_bits")
+            if n_bits_rounding == "auto":
+                raise NotImplementedError("Automatic rounding is not implemented yet.")
+            method = rounding_threshold_bits.get("method", method)
+            if not isinstance(method, Exactness):
+                method_str = method.upper()
+                if method_str in ["EXACT", "APPROXIMATE"]:
+                    method = Exactness[method_str]
+                else:
+                    raise ValueError(
+                        f"{method_str} is not a valid method. Must be one of EXACT, APPROXIMATE."
+                    )
+        else:
+            raise ValueError("Invalid type for rounding_threshold_bits. Must be int or dict.")
+
+        if n_bits_rounding is not None and not 2 <= n_bits_rounding <= 8:
+            raise ValueError("n_bits_rounding must be between 2 and 8 inclusive.")
+
+        rounding_threshold_bits = {"n_bits": n_bits_rounding, "method": method}
+
+    return rounding_threshold_bits
```

## concrete/ml/onnx/ops_impl.py

```diff
@@ -336,15 +336,15 @@
 
     Args:
         x (numpy.ndarray): Input tensor
 
     Returns:
         Tuple[numpy.ndarray]: Output tensor
     """
-    return (1.0 / (1.0 + numpy.exp(-x)),)
+    return (numpy.exp(-numpy.logaddexp(0, -x)),)
 
 
 def numpy_softmax(x, axis=1, keepdims=True):
     """Compute softmax in numpy according to ONNX spec.
 
     Softmax is currently not supported in FHE.
```

## concrete/ml/pytest/utils.py

```diff
@@ -1,14 +1,16 @@
 """Common functions or lists for test files, which can't be put in fixtures."""
+import copy
 import io
 from functools import partial
 from pathlib import Path
 from typing import Any, Callable, Dict, List, Optional, Type, Union
 
 import numpy
+import pandas
 import pytest
 import torch
 from numpy.random import RandomState
 from torch import nn
 
 from ..common.serialization.dumpers import dump, dumps
 from ..common.serialization.loaders import load, loads
@@ -79,15 +81,15 @@
             "n_features": 2,
             "n_classes": n_classes,
             "n_informative": 2,
             "n_redundant": 0,
         }
     else:
         dataset_params = {
-            "n_samples": 1000,
+            "n_samples": 100,
             "n_features": 10,
             "n_classes": n_classes,
             "n_informative": 10,
             "n_redundant": 0,
         }
 
     return pytest.param(
@@ -384,14 +386,19 @@
         parameters (dict): Hyper-parameters for the model instantiation. For QNNs, these parameters
             will override the matching default ones.
 
     Returns:
         model_name (str): The type of the model as a string.
         model (object): The model instance.
     """
+    # Force multi threaded models to be single threaded as it is not working
+    # properly with pytest multi-threading
+    if "n_jobs" in model_class().get_params():
+        parameters["n_jobs"] = 1
+
     # If the model is a QNN, set the model using appropriate bit-widths
     if is_model_class_in_a_list(model_class, _get_sklearn_neural_net_models()):
         extra_kwargs = {}
         if n_bits > 8:
             extra_kwargs["module__n_w_bits"] = 3
             extra_kwargs["module__n_a_bits"] = 3
             extra_kwargs["module__n_accum_bits"] = 12
@@ -680,7 +687,69 @@
 
     # Sanity checks
     assert 0 < n_sample < x.shape[0]
     assert len(x.shape) == 2
 
     random_rows_indices = numpy.random.choice(x.shape[0], size=n_sample, replace=False)
     return x[random_rows_indices]
+
+
+def pandas_dataframe_are_equal(
+    df_1: pandas.DataFrame,
+    df_2: pandas.DataFrame,
+    float_rtol: float = 1.0e-5,
+    float_atol: float = 1.0e-8,
+    equal_nan: bool = False,
+):
+    """Determine if both data-frames are identical.
+
+    Args:
+        df_1 (pandas.DataFrame): The first data-frame to consider.
+        df_2 (pandas.DataFrame): The second data-frame to consider.
+        float_rtol (float): Numpy's relative tolerance parameter to use when comparing columns with
+            floating point values. Default to 1.e-5.
+        float_atol (float): Numpy's absolute tolerance parameter to use when comparing columns with
+            floating point values. Default to 1.e-8.
+        equal_nan (bool):  Whether to compare NaN values as equal. Default to False.
+
+    Returns:
+        Bool: Wether both data-frames are equal.
+    """
+    df_1 = copy.copy(df_1)
+    df_2 = copy.copy(df_2)
+
+    # Select columns with floating point values
+    float_columns = df_1.select_dtypes(include="float").columns
+
+    # Check if the float columns contain the same values
+    float_equal = numpy.isclose(
+        df_1[float_columns],
+        df_2[float_columns],
+        rtol=float_rtol,
+        atol=float_atol,
+        equal_nan=equal_nan,
+    ).all()
+
+    # Select other columns (integers, objects, ...)
+    non_float_columns = df_1.select_dtypes(exclude="float").columns
+
+    # In case NaN values must be considered equal, replace them by a custom placeholder before
+    # comparing the data-frames
+    if equal_nan:
+        placeholder = "<NA>"
+
+        # Make sure this placeholder does not already exist in the data-frames
+        assert (
+            not df_1[non_float_columns].isin([placeholder]).any().any()
+            or not df_2[non_float_columns].isin([placeholder]).any().any()
+        ), (
+            f"The placeholder value '{placeholder}' already exists in the string columns and thus "
+            "cannot be used for comparing the data-frames."
+        )
+
+        df_1 = df_1[non_float_columns].fillna(placeholder)
+        df_2 = df_2[non_float_columns].fillna(placeholder)
+
+    # Check if non-float columns contain the same values
+    string_equal = df_1.eq(df_2).all().all()
+
+    return float_equal and string_equal
```

## concrete/ml/quantization/base_quantized_op.py

```diff
@@ -16,14 +16,16 @@
 from .quantizers import (
     MinMaxQuantizationStats,
     QuantizationOptions,
     QuantizedArray,
     UniformQuantizationParameters,
 )
 
+# pylint: disable=too-many-lines
+
 ONNXOpInputOutputType = Union[
     numpy.ndarray,
     QuantizedArray,
     None,
     bool,
     int,
     float,
@@ -869,21 +871,30 @@
 class QuantizedMixingOp(QuantizedOp, is_utility=True):
     """An operator that mixes (adds or multiplies) together encrypted inputs.
 
     Mixing operators cannot be fused to TLUs.
     """
 
     lsbs_to_remove: Optional[Union[int, dict]] = None
-    rounding_threshold_bits: Optional[int] = None
+    rounding_threshold_bits: Union[None, int, Dict[str, Union[str, int]]] = None
 
-    def __init__(self, *args, rounding_threshold_bits: Optional[int] = None, **kwargs) -> None:
+    def __init__(
+        self,
+        *args,
+        rounding_threshold_bits: Union[None, int, Dict[str, Union[str, int]]] = None,
+        **kwargs,
+    ) -> None:
         """Initialize quantized ops parameters plus specific parameters.
 
         Args:
-            rounding_threshold_bits (Optional[int]): Number of bits to round to.
+            rounding_threshold_bits (Union[None, int, Dict[str, Union[str, int]]]): if not None,
+                every accumulators in the model are rounded down to the given bits of precision.
+                Can be an int or a dictionary with keys 'method' and 'n_bits', where 'method' is
+                either fhe.Exactness.EXACT or fhe.Exactness.APPROXIMATE, and 'n_bits' is either
+                'auto' or an int.
             *args: positional argument to pass to the parent class.
             **kwargs: named argument to pass to the parent class.
         """
         self.rounding_threshold_bits = rounding_threshold_bits
         super().__init__(*args, **kwargs)
 
     def can_fuse(self) -> bool:
@@ -955,23 +966,35 @@
                 operation in a quantized operation. Used to create and access the
                 lsbs_to_remove value in the dictionary. Defaults to "single_rounding_op"
                 if not provided.
 
         Returns:
             numpy.ndarray: The rounded array.
         """
-
         # Ensure lsbs_to_remove is initialized as a dictionary
         if not hasattr(self, "lsbs_to_remove") or not isinstance(self.lsbs_to_remove, dict):
             self.lsbs_to_remove = {}
 
-        if self.rounding_threshold_bits is not None and calibrate_rounding:
+        n_bits = None
+        exactness = fhe.Exactness.EXACT
+
+        if isinstance(self.rounding_threshold_bits, dict):
+            n_bits = self.rounding_threshold_bits.get("n_bits", None)
+            exactness = self.rounding_threshold_bits.get("method", exactness)
+        # PoT is replacing inplace the rounding_threshold_bits to an int
+        elif isinstance(self.rounding_threshold_bits, int):
+            n_bits = self.rounding_threshold_bits
+
+        if n_bits is not None and calibrate_rounding:
             # Compute lsbs_to_remove only when calibration is True
             current_n_bits_accumulator = compute_bits_precision(x)
-            computed_lsbs_to_remove = current_n_bits_accumulator - self.rounding_threshold_bits
+
+            # mypy
+            assert isinstance(n_bits, int)
+            computed_lsbs_to_remove = current_n_bits_accumulator - n_bits
 
             assert_true(
                 not isinstance(x, fhe.tracing.Tracer),
                 "Can't compute lsbs_to_remove at compilation time.",
             )
 
             # Update the lsbs_to_remove value in the dictionary
@@ -983,10 +1006,16 @@
         # Rounding logic
         lsbs_value = self.lsbs_to_remove.get(rounding_operation_id, 0)
 
         # mypy
         assert isinstance(lsbs_value, int)
 
         if lsbs_value > 0:
-            x = fhe.round_bit_pattern(x, lsbs_to_remove=lsbs_value)
-
+            # Rounding to low bit-width with approximate can cause issues with overflow protection
+            # FIXME: https://github.com/zama-ai/concrete-ml-internal/issues/4345
+            if exactness == fhe.Exactness.APPROXIMATE:
+                x = fhe.round_bit_pattern(
+                    x, lsbs_to_remove=lsbs_value, exactness=exactness, overflow_protection=False
+                )
+            else:
+                x = fhe.round_bit_pattern(x, lsbs_to_remove=lsbs_value, exactness=exactness)
         return x
```

## concrete/ml/quantization/post_training.py

```diff
@@ -5,14 +5,15 @@
 
 import numpy
 import onnx
 from concrete.fhe.tracing import Tracer
 from onnx import numpy_helper
 
 from ..common.debugging import assert_true
+from ..common.utils import process_rounding_threshold_bits
 from ..onnx.onnx_utils import ONNX_OPS_TO_NUMPY_IMPL, get_attribute, get_op_type
 from ..onnx.ops_impl import RawOpOutput
 from ..torch.numpy_module import NumpyModule
 from .base_quantized_op import (
     DEFAULT_MODEL_BITS,
     ONNX_OPS_TO_QUANTIZED_IMPL,
     ONNXOpInputOutputType,
@@ -208,36 +209,38 @@
             "op_weights" bits. The maximum between this value and a default value (5) is then
             assigned to the number of "model_inputs" "model_outputs". This default value is a
             compromise between model accuracy and runtime performance in FHE. "model_outputs" gives
             the precision of the final network's outputs, while "model_inputs" gives the precision
             of the network's inputs. "op_inputs" and "op_weights" both control the quantization for
             inputs and weights of all layers.
         numpy_model (NumpyModule): Model in numpy.
-        rounding_threshold_bits (int): if not None, every accumulators in the model are rounded down
-            to the given bits of precision
+        rounding_threshold_bits (Union[None, int, Dict[str, Union[str, int]]]): Defines precision
+            rounding for model accumulators. Accepts None, an int, or a dict.
+            The dict can specify 'method' (fhe.Exactness.EXACT or fhe.Exactness.APPROXIMATE)
+            and 'n_bits' ('auto' or int)
     """
 
     quant_ops_dict: Dict[str, Tuple[Tuple[str, ...], QuantizedOp]]
     n_bits: Dict[str, int]
     quant_params: Dict[str, numpy.ndarray]
     numpy_model: NumpyModule
-    rounding_threshold_bits: Optional[int]
+    rounding_threshold_bits: Union[None, int, Dict[str, Union[str, int]]]
 
     def __init__(
         self,
         n_bits: Union[int, Dict],
         numpy_model: NumpyModule,
-        rounding_threshold_bits: Optional[int] = None,
+        rounding_threshold_bits: Union[None, int, Dict[str, Union[str, int]]] = None,
     ):
         self.quant_ops_dict = {}
 
         self.n_bits = get_n_bits_dict(n_bits)
         self.quant_params = {}
         self.numpy_model = numpy_model
-        self.rounding_threshold_bits = rounding_threshold_bits
+        self.rounding_threshold_bits = process_rounding_threshold_bits(rounding_threshold_bits)
 
     @property
     def n_bits_model_outputs(self):
         """Get the number of bits to use for the quantization of the last layer's output.
 
         Returns:
             n_bits (int): number of bits for output quantization
@@ -830,16 +833,20 @@
                                         "model_outputs" keys with corresponding number of
                                         quantization bits for:
                                         - model_inputs : number of bits for model input
                                         - op_inputs : number of bits to quantize layer input values
                                         - op_weights: learned parameters or constants in the network
                                         - model_outputs: final model output quantization bits
         numpy_model (NumpyModule):      Model in numpy.
-        rounding_threshold_bits (int): if not None, every accumulators in the model are rounded down
-            to the given bits of precision
+        rounding_threshold_bits (Union[None, int, Dict[str, Union[str, int]]]): if not None, every
+                                        accumulators in the model are rounded down to the given
+                                        bits of precision. Can be an int or a dictionary with keys
+                                        'method' and 'n_bits', where 'method' is either
+                                        fhe.Exactness.EXACT or fhe.Exactness.APPROXIMATE, and
+                                        'n_bits' is either 'auto' or an int.
         is_signed:                      Whether the weights of the layers can be signed.
                                         Currently, only the weights can be signed.
 
     Returns:
         QuantizedModule: A quantized version of the numpy model.
     """
```

## concrete/ml/quantization/quantized_module.py

```diff
@@ -43,15 +43,15 @@
 
     raise ValueError(
         "Error occurred during quantization aware training (QAT) import: "
         "The following tensors were expected to be quantized, but the values "
         "found during calibration do not appear to be quantized. \n\n"
         + "\n".join(
             map(
-                lambda info: f"* Tensor {info[0]}, input of an {info[1]} operation",
+                lambda info: f"* Tensor {info[0]}, input of a {info[1]} operation",
                 bad_qat_ops,
             )
         )
         + "\n\nCould not determine a unique scale for the quantization! "
         "Please check the ONNX graph of this model."
     )
 
@@ -522,19 +522,19 @@
             # If the inference should be executed using simulation
             if simulate:
 
                 # If the old simulation method should be used
                 if USE_OLD_VL:
                     predict_method = partial(
                         self.fhe_circuit.graph, p_error=self.fhe_circuit.p_error
-                    )
+                    )  # pragma: no cover
 
                 # Else, use the official simulation method
                 else:
-                    predict_method = self.fhe_circuit.simulate  # pragma: no cover
+                    predict_method = self.fhe_circuit.simulate
 
             # Else, use the FHE execution method
             else:
                 predict_method = self.fhe_circuit.encrypt_run_decrypt
 
             # Execute the forward pass in FHE or with simulation
             q_result = to_tuple(predict_method(*q_input))
```

## concrete/ml/sklearn/base.py

```diff
@@ -1567,26 +1567,26 @@
 000061e0: 7468 6f64 203d 2070 6172 7469 616c 280a  thod = partial(.
 000061f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006200: 2020 2020 2020 2020 2020 2020 7365 6c66              self
 00006210: 2e66 6865 5f63 6972 6375 6974 2e67 7261  .fhe_circuit.gra
 00006220: 7068 2c20 705f 6572 726f 723d 7365 6c66  ph, p_error=self
 00006230: 2e66 6865 5f63 6972 6375 6974 2e70 5f65  .fhe_circuit.p_e
 00006240: 7272 6f72 0a20 2020 2020 2020 2020 2020  rror.           
-00006250: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
-00006260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00006270: 2020 2020 2320 456c 7365 2c20 7573 6520      # Else, use 
-00006280: 7468 6520 6f66 6669 6369 616c 2073 696d  the official sim
-00006290: 756c 6174 696f 6e20 6d65 7468 6f64 0a20  ulation method. 
-000062a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062b0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000062c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000062d0: 2070 7265 6469 6374 5f6d 6574 686f 6420   predict_method 
-000062e0: 3d20 7365 6c66 2e66 6865 5f63 6972 6375  = self.fhe_circu
-000062f0: 6974 2e73 696d 756c 6174 6520 2023 2070  it.simulate  # p
-00006300: 7261 676d 613a 206e 6f20 636f 7665 720a  ragma: no cover.
+00006250: 2020 2020 2020 2020 2020 2020 2029 2020               )  
+00006260: 2320 7072 6167 6d61 3a20 6e6f 2063 6f76  # pragma: no cov
+00006270: 6572 0a0a 2020 2020 2020 2020 2020 2020  er..            
+00006280: 2020 2020 2020 2020 2320 456c 7365 2c20          # Else, 
+00006290: 7573 6520 7468 6520 6f66 6669 6369 616c  use the official
+000062a0: 2073 696d 756c 6174 696f 6e20 6d65 7468   simulation meth
+000062b0: 6f64 0a20 2020 2020 2020 2020 2020 2020  od.             
+000062c0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+000062d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000062e0: 2020 2020 2070 7265 6469 6374 5f6d 6574       predict_met
+000062f0: 686f 6420 3d20 7365 6c66 2e66 6865 5f63  hod = self.fhe_c
+00006300: 6972 6375 6974 2e73 696d 756c 6174 650a  ircuit.simulate.
 00006310: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
 00006320: 2023 2045 6c73 652c 2075 7365 2074 6865   # Else, use the
 00006330: 2046 4845 2065 7865 6375 7469 6f6e 206d   FHE execution m
 00006340: 6574 686f 640a 2020 2020 2020 2020 2020  ethod.          
 00006350: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
 00006360: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00006370: 7072 6564 6963 745f 6d65 7468 6f64 203d  predict_method =
@@ -3556,2029 +3556,2025 @@
 0000de30: 2020 2064 6566 2070 6f73 745f 7072 6f63     def post_proc
 0000de40: 6573 7369 6e67 2873 656c 662c 2079 5f70  essing(self, y_p
 0000de50: 7265 6473 3a20 6e75 6d70 792e 6e64 6172  reds: numpy.ndar
 0000de60: 7261 7929 202d 3e20 6e75 6d70 792e 6e64  ray) -> numpy.nd
 0000de70: 6172 7261 793a 0a20 2020 2020 2020 2023  array:.        #
 0000de80: 2053 756d 2061 6c6c 2074 7265 6520 6f75   Sum all tree ou
 0000de90: 7470 7574 730a 2020 2020 2020 2020 2320  tputs.        # 
-0000dea0: 5265 6d6f 7665 2074 6865 2073 756d 206f  Remove the sum o
-0000deb0: 6e63 6520 7765 2068 616e 646c 6520 6d75  nce we handle mu
-0000dec0: 6c74 692d 7072 6563 6973 696f 6e20 6369  lti-precision ci
-0000ded0: 7263 7569 7473 0a20 2020 2020 2020 2023  rcuits.        #
-0000dee0: 2046 4958 4d45 3a20 6874 7470 733a 2f2f   FIXME: https://
-0000def0: 6769 7468 7562 2e63 6f6d 2f7a 616d 612d  github.com/zama-
-0000df00: 6169 2f63 6f6e 6372 6574 652d 6d6c 2d69  ai/concrete-ml-i
-0000df10: 6e74 6572 6e61 6c2f 6973 7375 6573 2f34  nternal/issues/4
-0000df20: 3531 0a20 2020 2020 2020 2069 6620 6e6f  51.        if no
-0000df30: 7420 7365 6c66 2e5f 6668 655f 656e 7365  t self._fhe_ense
-0000df40: 6d62 6c69 6e67 3a0a 2020 2020 2020 2020  mbling:.        
-0000df50: 2020 2020 795f 7072 6564 7320 3d20 6e75      y_preds = nu
-0000df60: 6d70 792e 7375 6d28 795f 7072 6564 732c  mpy.sum(y_preds,
-0000df70: 2061 7869 733d 2d31 290a 0a20 2020 2020   axis=-1)..     
-0000df80: 2020 2020 2020 2061 7373 6572 745f 7472         assert_tr
-0000df90: 7565 2879 5f70 7265 6473 2e6e 6469 6d20  ue(y_preds.ndim 
-0000dfa0: 3d3d 2032 2c20 2279 5f70 7265 6473 2073  == 2, "y_preds s
-0000dfb0: 686f 756c 6420 6265 2061 2032 4420 6172  hould be a 2D ar
-0000dfc0: 7261 7922 290a 2020 2020 2020 2020 2020  ray").          
-0000dfd0: 2020 7265 7475 726e 2079 5f70 7265 6473    return y_preds
-0000dfe0: 0a0a 2020 2020 2020 2020 7265 7475 726e  ..        return
-0000dff0: 2073 7570 6572 2829 2e70 6f73 745f 7072   super().post_pr
-0000e000: 6f63 6573 7369 6e67 2879 5f70 7265 6473  ocessing(y_preds
-0000e010: 290a 0a0a 636c 6173 7320 4261 7365 5472  )...class BaseTr
-0000e020: 6565 5265 6772 6573 736f 724d 6978 696e  eeRegressorMixin
-0000e030: 2842 6173 6554 7265 6545 7374 696d 6174  (BaseTreeEstimat
-0000e040: 6f72 4d69 7869 6e2c 2073 6b6c 6561 726e  orMixin, sklearn
-0000e050: 2e62 6173 652e 5265 6772 6573 736f 724d  .base.RegressorM
-0000e060: 6978 696e 2c20 4142 4329 3a0a 2020 2020  ixin, ABC):.    
-0000e070: 2222 224d 6978 696e 2063 6c61 7373 2066  """Mixin class f
-0000e080: 6f72 2074 7265 652d 6261 7365 6420 7265  or tree-based re
-0000e090: 6772 6573 736f 7273 2e0a 0a20 2020 2054  gressors...    T
-0000e0a0: 6869 7320 636c 6173 7320 6973 2075 7365  his class is use
-0000e0b0: 6420 746f 2063 7265 6174 6520 6120 7472  d to create a tr
-0000e0c0: 6565 2d62 6173 6564 2072 6567 7265 7373  ee-based regress
-0000e0d0: 6f72 2063 6c61 7373 2074 6861 7420 696e  or class that in
-0000e0e0: 6865 7269 7473 2066 726f 6d0a 2020 2020  herits from.    
-0000e0f0: 736b 6c65 6172 6e2e 6261 7365 2e52 6567  sklearn.base.Reg
-0000e100: 7265 7373 6f72 4d69 7869 6e2c 2077 6869  ressorMixin, whi
-0000e110: 6368 2065 7373 656e 7469 616c 6c79 2067  ch essentially g
-0000e120: 6976 6573 2061 6363 6573 7320 746f 2073  ives access to s
-0000e130: 6369 6b69 742d 6c65 6172 6e27 7320 6073  cikit-learn's `s
-0000e140: 636f 7265 6020 6d65 7468 6f64 0a20 2020  core` method.   
-0000e150: 2066 6f72 2072 6567 7265 7373 6f72 732e   for regressors.
-0000e160: 0a20 2020 2022 2222 0a0a 0a63 6c61 7373  .    """...class
-0000e170: 2042 6173 6554 7265 6543 6c61 7373 6966   BaseTreeClassif
-0000e180: 6965 724d 6978 696e 280a 2020 2020 4261  ierMixin(.    Ba
-0000e190: 7365 436c 6173 7369 6669 6572 2c20 4261  seClassifier, Ba
-0000e1a0: 7365 5472 6565 4573 7469 6d61 746f 724d  seTreeEstimatorM
-0000e1b0: 6978 696e 2c20 736b 6c65 6172 6e2e 6261  ixin, sklearn.ba
-0000e1c0: 7365 2e43 6c61 7373 6966 6965 724d 6978  se.ClassifierMix
-0000e1d0: 696e 2c20 4142 430a 293a 0a20 2020 2022  in, ABC.):.    "
-0000e1e0: 2222 4d69 7869 6e20 636c 6173 7320 666f  ""Mixin class fo
-0000e1f0: 7220 7472 6565 2d62 6173 6564 2063 6c61  r tree-based cla
-0000e200: 7373 6966 6965 7273 2e0a 0a20 2020 2054  ssifiers...    T
-0000e210: 6869 7320 636c 6173 7320 6973 2075 7365  his class is use
-0000e220: 6420 746f 2063 7265 6174 6520 6120 7472  d to create a tr
-0000e230: 6565 2d62 6173 6564 2063 6c61 7373 6966  ee-based classif
-0000e240: 6965 7220 636c 6173 7320 7468 6174 2069  ier class that i
-0000e250: 6e68 6572 6974 7320 6672 6f6d 0a20 2020  nherits from.   
-0000e260: 2073 6b6c 6561 726e 2e62 6173 652e 436c   sklearn.base.Cl
-0000e270: 6173 7369 6669 6572 4d69 7869 6e2c 2077  assifierMixin, w
-0000e280: 6869 6368 2065 7373 656e 7469 616c 6c79  hich essentially
-0000e290: 2067 6976 6573 2061 6363 6573 7320 746f   gives access to
-0000e2a0: 2073 6369 6b69 742d 6c65 6172 6e27 7320   scikit-learn's 
-0000e2b0: 6073 636f 7265 6020 6d65 7468 6f64 0a20  `score` method. 
-0000e2c0: 2020 2066 6f72 2063 6c61 7373 6966 6965     for classifie
-0000e2d0: 7273 2e0a 0a20 2020 2041 6464 6974 696f  rs...    Additio
-0000e2e0: 6e61 6c6c 792c 2074 6869 7320 636c 6173  nally, this clas
-0000e2f0: 7320 6164 6a75 7374 7320 736f 6d65 206f  s adjusts some o
-0000e300: 6620 7468 6520 7472 6565 2d62 6173 6564  f the tree-based
-0000e310: 2062 6173 6520 636c 6173 7327 7320 6d65   base class's me
-0000e320: 7468 6f64 7320 696e 206f 7264 6572 2074  thods in order t
-0000e330: 6f20 6d61 6b65 0a20 2020 2074 6865 6d20  o make.    them 
-0000e340: 636f 6d70 6c69 616e 7420 7769 7468 2063  compliant with c
-0000e350: 6c61 7373 6966 6963 6174 696f 6e20 776f  lassification wo
-0000e360: 726b 666c 6f77 732e 0a20 2020 2022 2222  rkflows..    """
-0000e370: 0a0a 0a23 2070 796c 696e 743a 2064 6973  ...# pylint: dis
-0000e380: 6162 6c65 3d69 6e76 616c 6964 2d6e 616d  able=invalid-nam
-0000e390: 652c 746f 6f2d 6d61 6e79 2d69 6e73 7461  e,too-many-insta
-0000e3a0: 6e63 652d 6174 7472 6962 7574 6573 0a63  nce-attributes.c
-0000e3b0: 6c61 7373 2053 6b6c 6561 726e 4c69 6e65  lass SklearnLine
-0000e3c0: 6172 4d6f 6465 6c4d 6978 696e 2842 6173  arModelMixin(Bas
-0000e3d0: 6545 7374 696d 6174 6f72 2c20 736b 6c65  eEstimator, skle
-0000e3e0: 6172 6e2e 6261 7365 2e42 6173 6545 7374  arn.base.BaseEst
-0000e3f0: 696d 6174 6f72 2c20 4142 4329 3a0a 2020  imator, ABC):.  
-0000e400: 2020 2222 2241 204d 6978 696e 2063 6c61    """A Mixin cla
-0000e410: 7373 2066 6f72 2073 6b6c 6561 726e 206c  ss for sklearn l
-0000e420: 696e 6561 7220 6d6f 6465 6c73 2077 6974  inear models wit
-0000e430: 6820 4648 452e 0a0a 2020 2020 5468 6973  h FHE...    This
-0000e440: 2063 6c61 7373 2069 6e68 6572 6974 7320   class inherits 
-0000e450: 6672 6f6d 2073 6b6c 6561 726e 2e62 6173  from sklearn.bas
-0000e460: 652e 4261 7365 4573 7469 6d61 746f 7220  e.BaseEstimator 
-0000e470: 696e 206f 7264 6572 2074 6f20 6861 7665  in order to have
-0000e480: 2061 6363 6573 7320 746f 2073 6369 6b69   access to sciki
-0000e490: 742d 6c65 6172 6e27 730a 2020 2020 6067  t-learn's.    `g
-0000e4a0: 6574 5f70 6172 616d 7360 2061 6e64 2060  et_params` and `
-0000e4b0: 7365 745f 7061 7261 6d73 6020 6d65 7468  set_params` meth
-0000e4c0: 6f64 732e 0a20 2020 2022 2222 0a0a 2020  ods..    """..  
-0000e4d0: 2020 6465 6620 5f5f 696e 6974 5f73 7562    def __init_sub
-0000e4e0: 636c 6173 735f 5f28 636c 7329 3a0a 2020  class__(cls):.  
-0000e4f0: 2020 2020 2020 666f 7220 6b6c 6173 7320        for klass 
-0000e500: 696e 2063 6c73 2e5f 5f6d 726f 5f5f 3a0a  in cls.__mro__:.
-0000e510: 2020 2020 2020 2020 2020 2020 2320 7079              # py
-0000e520: 6c69 6e74 3a20 6469 7361 626c 652d 6e65  lint: disable-ne
-0000e530: 7874 3d70 726f 7465 6374 6564 2d61 6363  xt=protected-acc
-0000e540: 6573 730a 2020 2020 2020 2020 2020 2020  ess.            
-0000e550: 6966 2067 6574 6174 7472 286b 6c61 7373  if getattr(klass
-0000e560: 2c20 225f 6973 5f61 5f70 7562 6c69 635f  , "_is_a_public_
-0000e570: 636d 6c5f 6d6f 6465 6c22 2c20 4661 6c73  cml_model", Fals
-0000e580: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-0000e590: 2020 2020 5f4c 494e 4541 525f 4d4f 4445      _LINEAR_MODE
-0000e5a0: 4c53 2e61 6464 2863 6c73 290a 2020 2020  LS.add(cls).    
-0000e5b0: 2020 2020 2020 2020 2020 2020 5f41 4c4c              _ALL
-0000e5c0: 5f53 4b4c 4541 524e 5f4d 4f44 454c 532e  _SKLEARN_MODELS.
-0000e5d0: 6164 6428 636c 7329 0a0a 2020 2020 6465  add(cls)..    de
-0000e5e0: 6620 5f5f 696e 6974 5f5f 2873 656c 662c  f __init__(self,
-0000e5f0: 206e 5f62 6974 733a 2055 6e69 6f6e 5b69   n_bits: Union[i
-0000e600: 6e74 2c20 4469 6374 5b73 7472 2c20 696e  nt, Dict[str, in
-0000e610: 745d 5d20 3d20 3829 3a0a 2020 2020 2020  t]] = 8):.      
-0000e620: 2020 2222 2249 6e69 7469 616c 697a 6520    """Initialize 
-0000e630: 7468 6520 4648 4520 6c69 6e65 6172 206d  the FHE linear m
-0000e640: 6f64 656c 2e0a 0a20 2020 2020 2020 2041  odel...        A
-0000e650: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-0000e660: 206e 5f62 6974 7320 2869 6e74 2c20 4469   n_bits (int, Di
-0000e670: 6374 5b73 7472 2c20 696e 745d 293a 204e  ct[str, int]): N
-0000e680: 756d 6265 7220 6f66 2062 6974 7320 746f  umber of bits to
-0000e690: 2071 7561 6e74 697a 6520 7468 6520 6d6f   quantize the mo
-0000e6a0: 6465 6c2e 2049 6620 616e 2069 6e74 2069  del. If an int i
-0000e6b0: 7320 7061 7373 6564 0a20 2020 2020 2020  s passed.       
-0000e6c0: 2020 2020 2020 2020 2066 6f72 206e 5f62           for n_b
-0000e6d0: 6974 732c 2074 6865 2076 616c 7565 2077  its, the value w
-0000e6e0: 696c 6c20 6265 2075 7365 6420 666f 7220  ill be used for 
-0000e6f0: 7175 616e 7469 7a69 6e67 2069 6e70 7574  quantizing input
-0000e700: 7320 616e 6420 7765 6967 6874 732e 2049  s and weights. I
-0000e710: 6620 6120 6469 6374 2069 730a 2020 2020  f a dict is.    
-0000e720: 2020 2020 2020 2020 2020 2020 7061 7373              pass
-0000e730: 6564 2c20 7468 656e 2069 7420 7368 6f75  ed, then it shou
-0000e740: 6c64 2063 6f6e 7461 696e 2022 6f70 5f69  ld contain "op_i
-0000e750: 6e70 7574 7322 2061 6e64 2022 6f70 5f77  nputs" and "op_w
-0000e760: 6569 6768 7473 2220 6173 206b 6579 7320  eights" as keys 
-0000e770: 7769 7468 0a20 2020 2020 2020 2020 2020  with.           
-0000e780: 2020 2020 2063 6f72 7265 7370 6f6e 6469       correspondi
-0000e790: 6e67 206e 756d 6265 7220 6f66 2071 7561  ng number of qua
-0000e7a0: 6e74 697a 6174 696f 6e20 6269 7473 2073  ntization bits s
-0000e7b0: 6f20 7468 6174 3a0a 2020 2020 2020 2020  o that:.        
-0000e7c0: 2020 2020 2020 2020 2020 2020 2d20 6f70              - op
-0000e7d0: 5f69 6e70 7574 7320 3a20 6e75 6d62 6572  _inputs : number
-0000e7e0: 206f 6620 6269 7473 2074 6f20 7175 616e   of bits to quan
-0000e7f0: 7469 7a65 2074 6865 2069 6e70 7574 2076  tize the input v
-0000e800: 616c 7565 730a 2020 2020 2020 2020 2020  alues.          
-0000e810: 2020 2020 2020 2020 2020 2d20 6f70 5f77            - op_w
-0000e820: 6569 6768 7473 3a20 6e75 6d62 6572 206f  eights: number o
-0000e830: 6620 6269 7473 2074 6f20 7175 616e 7469  f bits to quanti
-0000e840: 7a65 2074 6865 206c 6561 726e 6564 2070  ze the learned p
-0000e850: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
-0000e860: 2020 2020 2020 2020 2020 4465 6661 756c            Defaul
-0000e870: 7420 746f 2038 2e0a 2020 2020 2020 2020  t to 8..        
-0000e880: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
-0000e890: 2e6e 5f62 6974 733a 2055 6e69 6f6e 5b69  .n_bits: Union[i
-0000e8a0: 6e74 2c20 4469 6374 5b73 7472 2c20 696e  nt, Dict[str, in
-0000e8b0: 745d 5d20 3d20 6e5f 6269 7473 0a0a 2020  t]] = n_bits..  
-0000e8c0: 2020 2020 2020 233a 2054 6865 2071 7561        #: The qua
-0000e8d0: 6e74 697a 6572 2074 6f20 7573 6520 666f  ntizer to use fo
-0000e8e0: 7220 7175 616e 7469 7a69 6e67 2074 6865  r quantizing the
-0000e8f0: 206d 6f64 656c 2773 2077 6569 6768 7473   model's weights
-0000e900: 0a20 2020 2020 2020 2073 656c 662e 5f77  .        self._w
-0000e910: 6569 6768 745f 7175 616e 7469 7a65 723a  eight_quantizer:
-0000e920: 204f 7074 696f 6e61 6c5b 556e 6966 6f72   Optional[Unifor
-0000e930: 6d51 7561 6e74 697a 6572 5d20 3d20 4e6f  mQuantizer] = No
-0000e940: 6e65 0a0a 2020 2020 2020 2020 233a 2054  ne..        #: T
-0000e950: 6865 206d 6f64 656c 2773 2071 7561 6e74  he model's quant
-0000e960: 697a 6564 2077 6569 6768 7473 0a20 2020  ized weights.   
-0000e970: 2020 2020 2073 656c 662e 5f71 5f77 6569       self._q_wei
-0000e980: 6768 7473 3a20 4f70 7469 6f6e 616c 5b6e  ghts: Optional[n
-0000e990: 756d 7079 2e6e 6461 7272 6179 5d20 3d20  umpy.ndarray] = 
-0000e9a0: 4e6f 6e65 0a0a 2020 2020 2020 2020 233a  None..        #:
-0000e9b0: 2054 6865 206d 6f64 656c 2773 2071 7561   The model's qua
-0000e9c0: 6e74 697a 6564 2062 6961 730a 2020 2020  ntized bias.    
-0000e9d0: 2020 2020 7365 6c66 2e5f 715f 6269 6173      self._q_bias
-0000e9e0: 3a20 4f70 7469 6f6e 616c 5b6e 756d 7079  : Optional[numpy
-0000e9f0: 2e6e 6461 7272 6179 5d20 3d20 4e6f 6e65  .ndarray] = None
-0000ea00: 0a0a 2020 2020 2020 2020 4261 7365 4573  ..        BaseEs
-0000ea10: 7469 6d61 746f 722e 5f5f 696e 6974 5f5f  timator.__init__
-0000ea20: 2873 656c 6629 0a0a 2020 2020 4063 6c61  (self)..    @cla
-0000ea30: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
-0000ea40: 2066 726f 6d5f 736b 6c65 6172 6e5f 6d6f   from_sklearn_mo
-0000ea50: 6465 6c28 0a20 2020 2020 2020 2063 6c73  del(.        cls
-0000ea60: 2c0a 2020 2020 2020 2020 736b 6c65 6172  ,.        sklear
-0000ea70: 6e5f 6d6f 6465 6c3a 2073 6b6c 6561 726e  n_model: sklearn
-0000ea80: 2e62 6173 652e 4261 7365 4573 7469 6d61  .base.BaseEstima
-0000ea90: 746f 722c 0a20 2020 2020 2020 2058 3a20  tor,.        X: 
-0000eaa0: 4461 7461 2c0a 2020 2020 2020 2020 6e5f  Data,.        n_
-0000eab0: 6269 7473 3a20 556e 696f 6e5b 696e 742c  bits: Union[int,
-0000eac0: 2044 6963 745b 7374 722c 2069 6e74 5d5d   Dict[str, int]]
-0000ead0: 203d 2038 2c0a 2020 2020 293a 0a20 2020   = 8,.    ):.   
-0000eae0: 2020 2020 2022 2222 4275 696c 6420 6120       """Build a 
-0000eaf0: 4648 452d 636f 6d70 6c69 616e 7420 6d6f  FHE-compliant mo
-0000eb00: 6465 6c20 7573 696e 6720 6120 6669 7474  del using a fitt
-0000eb10: 6564 2073 6369 6b69 742d 6c65 6172 6e20  ed scikit-learn 
-0000eb20: 6d6f 6465 6c2e 0a0a 2020 2020 2020 2020  model...        
-0000eb30: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-0000eb40: 2020 736b 6c65 6172 6e5f 6d6f 6465 6c20    sklearn_model 
-0000eb50: 2873 6b6c 6561 726e 2e62 6173 652e 4261  (sklearn.base.Ba
-0000eb60: 7365 4573 7469 6d61 746f 7229 3a20 5468  seEstimator): Th
-0000eb70: 6520 6669 7474 6564 2073 6369 6b69 742d  e fitted scikit-
-0000eb80: 6c65 6172 6e20 6d6f 6465 6c20 746f 2063  learn model to c
-0000eb90: 6f6e 7665 7274 2e0a 2020 2020 2020 2020  onvert..        
-0000eba0: 2020 2020 5820 2844 6174 6129 3a20 4120      X (Data): A 
-0000ebb0: 7265 7072 6573 656e 7461 7469 7665 2073  representative s
-0000ebc0: 6574 206f 6620 696e 7075 7420 7661 6c75  et of input valu
-0000ebd0: 6573 2075 7365 6420 666f 7220 636f 6d70  es used for comp
-0000ebe0: 7574 696e 6720 7175 616e 7469 7a61 7469  uting quantizati
-0000ebf0: 6f6e 0a20 2020 2020 2020 2020 2020 2020  on.             
-0000ec00: 2020 2070 6172 616d 6574 6572 732c 2061     parameters, a
-0000ec10: 7320 6120 4e75 6d70 7920 6172 7261 792c  s a Numpy array,
-0000ec20: 2054 6f72 6368 2074 656e 736f 722c 2050   Torch tensor, P
-0000ec30: 616e 6461 7320 4461 7461 4672 616d 6520  andas DataFrame 
-0000ec40: 6f72 204c 6973 742e 2054 6869 7320 6973  or List. This is
-0000ec50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ec60: 2075 7375 616c 6c79 2074 6865 2074 7261   usually the tra
-0000ec70: 696e 696e 6720 6461 7461 2d73 6574 206f  ining data-set o
-0000ec80: 7220 6120 7375 622d 7365 7420 6f66 2069  r a sub-set of i
-0000ec90: 742e 0a20 2020 2020 2020 2020 2020 206e  t..            n
-0000eca0: 5f62 6974 7320 2869 6e74 2c20 4469 6374  _bits (int, Dict
-0000ecb0: 5b73 7472 2c20 696e 745d 293a 204e 756d  [str, int]): Num
-0000ecc0: 6265 7220 6f66 2062 6974 7320 746f 2071  ber of bits to q
-0000ecd0: 7561 6e74 697a 6520 7468 6520 6d6f 6465  uantize the mode
-0000ece0: 6c2e 2049 6620 616e 2069 6e74 2069 7320  l. If an int is 
-0000ecf0: 7061 7373 6564 0a20 2020 2020 2020 2020  passed.         
-0000ed00: 2020 2020 2020 2066 6f72 206e 5f62 6974         for n_bit
-0000ed10: 732c 2074 6865 2076 616c 7565 2077 696c  s, the value wil
-0000ed20: 6c20 6265 2075 7365 6420 666f 7220 7175  l be used for qu
-0000ed30: 616e 7469 7a69 6e67 2069 6e70 7574 7320  antizing inputs 
-0000ed40: 616e 6420 7765 6967 6874 732e 2049 6620  and weights. If 
-0000ed50: 6120 6469 6374 2069 730a 2020 2020 2020  a dict is.      
-0000ed60: 2020 2020 2020 2020 2020 7061 7373 6564            passed
-0000ed70: 2c20 7468 656e 2069 7420 7368 6f75 6c64  , then it should
-0000ed80: 2063 6f6e 7461 696e 2022 6f70 5f69 6e70   contain "op_inp
-0000ed90: 7574 7322 2061 6e64 2022 6f70 5f77 6569  uts" and "op_wei
-0000eda0: 6768 7473 2220 6173 206b 6579 7320 7769  ghts" as keys wi
-0000edb0: 7468 0a20 2020 2020 2020 2020 2020 2020  th.             
-0000edc0: 2020 2063 6f72 7265 7370 6f6e 6469 6e67     corresponding
-0000edd0: 206e 756d 6265 7220 6f66 2071 7561 6e74   number of quant
-0000ede0: 697a 6174 696f 6e20 6269 7473 2073 6f20  ization bits so 
-0000edf0: 7468 6174 3a0a 2020 2020 2020 2020 2020  that:.          
-0000ee00: 2020 2020 2020 2d20 6f70 5f69 6e70 7574        - op_input
-0000ee10: 7320 3a20 6e75 6d62 6572 206f 6620 6269  s : number of bi
-0000ee20: 7473 2074 6f20 7175 616e 7469 7a65 2074  ts to quantize t
-0000ee30: 6865 2069 6e70 7574 2076 616c 7565 730a  he input values.
-0000ee40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ee50: 2d20 6f70 5f77 6569 6768 7473 3a20 6e75  - op_weights: nu
-0000ee60: 6d62 6572 206f 6620 6269 7473 2074 6f20  mber of bits to 
-0000ee70: 7175 616e 7469 7a65 2074 6865 206c 6561  quantize the lea
-0000ee80: 726e 6564 2070 6172 616d 6574 6572 730a  rned parameters.
-0000ee90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000eea0: 4465 6661 756c 7420 746f 2038 2e0a 0a20  Default to 8... 
-0000eeb0: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-0000eec0: 2020 2020 2020 2020 2020 2020 5468 6520              The 
-0000eed0: 4648 452d 636f 6d70 6c69 616e 7420 6669  FHE-compliant fi
-0000eee0: 7474 6564 206d 6f64 656c 2e0a 2020 2020  tted model..    
-0000eef0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-0000ef00: 2023 2043 6865 636b 2074 6861 7420 736b   # Check that sk
-0000ef10: 6c65 6172 6e5f 6d6f 6465 6c20 6973 2061  learn_model is a
-0000ef20: 2070 726f 7065 7220 6669 7474 6564 2073   proper fitted s
-0000ef30: 6369 6b69 742d 6c65 6172 6e20 6d6f 6465  cikit-learn mode
-0000ef40: 6c0a 2020 2020 2020 2020 6368 6563 6b5f  l.        check_
-0000ef50: 6973 5f66 6974 7465 6428 736b 6c65 6172  is_fitted(sklear
-0000ef60: 6e5f 6d6f 6465 6c29 0a0a 2020 2020 2020  n_model)..      
-0000ef70: 2020 2320 4578 7472 6163 7420 7363 696b    # Extract scik
-0000ef80: 6974 2d6c 6561 726e 2773 2069 6e69 7469  it-learn's initi
-0000ef90: 616c 697a 6174 696f 6e20 7061 7261 6d65  alization parame
-0000efa0: 7465 7273 0a20 2020 2020 2020 2069 6e69  ters.        ini
-0000efb0: 745f 7061 7261 6d73 203d 2073 6b6c 6561  t_params = sklea
-0000efc0: 726e 5f6d 6f64 656c 2e67 6574 5f70 6172  rn_model.get_par
-0000efd0: 616d 7328 290a 0a20 2020 2020 2020 2023  ams()..        #
-0000efe0: 2049 6e73 7461 6e74 6961 7465 2074 6865   Instantiate the
-0000eff0: 2043 6f6e 6372 6574 6520 4d4c 206d 6f64   Concrete ML mod
-0000f000: 656c 2061 6e64 2075 7064 6174 6520 696e  el and update in
-0000f010: 6974 6961 6c69 7a61 7469 6f6e 2070 6172  itialization par
-0000f020: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-0000f030: 2320 5468 6973 2075 7064 6174 6520 6973  # This update is
-0000f040: 206e 6563 6573 7361 7279 2061 7320 7765   necessary as we
-0000f050: 2063 7572 7265 6e74 6c79 2073 746f 7265   currently store
-0000f060: 2073 6369 6b69 742d 6c65 6172 6e20 6174   scikit-learn at
-0000f070: 7472 6962 7574 6573 2069 6e20 436f 6e63  tributes in Conc
-0000f080: 7265 7465 204d 4c0a 2020 2020 2020 2020  rete ML.        
-0000f090: 2320 636c 6173 7365 7320 6475 7269 6e67  # classes during
-0000f0a0: 2069 6e69 7469 616c 697a 6174 696f 6e20   initialization 
-0000f0b0: 2866 6f72 2065 7861 6d70 6c65 3a20 6c69  (for example: li
-0000f0c0: 6e6b 206f 7220 706f 7765 7220 6174 7472  nk or power attr
-0000f0d0: 6962 7574 6573 2069 6e20 474c 4d73 290a  ibutes in GLMs).
-0000f0e0: 2020 2020 2020 2020 2320 5769 7468 6f75          # Withou
-0000f0f0: 7420 6974 2c20 7468 6573 6520 6174 7472  t it, these attr
-0000f100: 6962 7574 6573 2077 696c 6c20 6861 7665  ibutes will have
-0000f110: 2064 6566 6175 6c74 2076 616c 7565 7320   default values 
-0000f120: 696e 7374 6561 6420 6f66 2074 6865 206f  instead of the o
-0000f130: 6e65 7320 7573 6564 2062 7920 7468 650a  nes used by the.
-0000f140: 2020 2020 2020 2020 2320 7363 696b 6974          # scikit
-0000f150: 2d6c 6561 726e 206d 6f64 656c 730a 2020  -learn models.  
-0000f160: 2020 2020 2020 2320 5468 6973 2073 686f        # This sho
-0000f170: 756c 6420 6265 2066 6978 6564 206f 6e63  uld be fixed onc
-0000f180: 6520 436f 6e63 7265 7465 204d 4c20 6d6f  e Concrete ML mo
-0000f190: 6465 6c73 2069 6e69 7469 616c 697a 6520  dels initialize 
-0000f1a0: 7468 6569 7220 756e 6465 726c 7969 6e67  their underlying
-0000f1b0: 2073 6369 6b69 742d 6c65 6172 6e0a 2020   scikit-learn.  
-0000f1c0: 2020 2020 2020 2320 6d6f 6465 6c73 2064        # models d
-0000f1d0: 7572 696e 6720 696e 6974 6961 6c69 7a61  uring initializa
-0000f1e0: 7469 6f6e 0a20 2020 2020 2020 2023 2046  tion.        # F
-0000f1f0: 4958 4d45 3a20 6874 7470 733a 2f2f 6769  IXME: https://gi
-0000f200: 7468 7562 2e63 6f6d 2f7a 616d 612d 6169  thub.com/zama-ai
-0000f210: 2f63 6f6e 6372 6574 652d 6d6c 2d69 6e74  /concrete-ml-int
-0000f220: 6572 6e61 6c2f 6973 7375 6573 2f33 3337  ernal/issues/337
-0000f230: 330a 2020 2020 2020 2020 6d6f 6465 6c20  3.        model 
-0000f240: 3d20 636c 7328 6e5f 6269 7473 3d6e 5f62  = cls(n_bits=n_b
-0000f250: 6974 732c 202a 2a69 6e69 745f 7061 7261  its, **init_para
-0000f260: 6d73 290a 0a20 2020 2020 2020 2023 2055  ms)..        # U
-0000f270: 7064 6174 6520 7468 6520 756e 6465 726c  pdate the underl
-0000f280: 7969 6e67 2073 6369 6b69 742d 6c65 6172  ying scikit-lear
-0000f290: 6e20 6d6f 6465 6c20 7769 7468 2074 6865  n model with the
-0000f2a0: 2067 6976 656e 2066 6974 7465 6420 6f6e   given fitted on
-0000f2b0: 650a 2020 2020 2020 2020 6d6f 6465 6c2e  e.        model.
-0000f2c0: 736b 6c65 6172 6e5f 6d6f 6465 6c20 3d20  sklearn_model = 
-0000f2d0: 636f 7079 2e64 6565 7063 6f70 7928 736b  copy.deepcopy(sk
-0000f2e0: 6c65 6172 6e5f 6d6f 6465 6c29 0a0a 2020  learn_model)..  
-0000f2f0: 2020 2020 2020 2320 436f 6d70 7574 6520        # Compute 
-0000f300: 7468 6520 7175 616e 7469 7a61 7469 6f6e  the quantization
-0000f310: 2070 6172 616d 6574 6572 730a 2020 2020   parameters.    
-0000f320: 2020 2020 7265 7475 726e 206d 6f64 656c      return model
-0000f330: 2e5f 7175 616e 7469 7a65 5f6d 6f64 656c  ._quantize_model
-0000f340: 2858 290a 0a20 2020 2064 6566 205f 7365  (X)..    def _se
-0000f350: 745f 6f6e 6e78 5f6d 6f64 656c 2873 656c  t_onnx_model(sel
-0000f360: 662c 2074 6573 745f 696e 7075 743a 206e  f, test_input: n
-0000f370: 756d 7079 2e6e 6461 7272 6179 2920 2d3e  umpy.ndarray) ->
-0000f380: 204e 6f6e 653a 0a20 2020 2020 2020 2022   None:.        "
-0000f390: 2222 5265 7472 6965 7665 2074 6865 206d  ""Retrieve the m
-0000f3a0: 6f64 656c 2773 204f 4e4e 5820 6772 6170  odel's ONNX grap
-0000f3b0: 6820 7573 696e 6720 4875 6d6d 696e 6762  h using Hummingb
-0000f3c0: 6972 6420 636f 6e76 6572 7369 6f6e 2e0a  ird conversion..
-0000f3d0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-0000f3e0: 2020 2020 2020 2020 2020 2074 6573 745f             test_
-0000f3f0: 696e 7075 7420 286e 756d 7079 2e6e 6461  input (numpy.nda
-0000f400: 7272 6179 293a 2041 6e20 696e 7075 7420  rray): An input 
-0000f410: 6461 7461 2075 7365 6420 746f 2074 7261  data used to tra
-0000f420: 6365 2074 6865 206d 6f64 656c 2065 7865  ce the model exe
-0000f430: 6375 7469 6f6e 2e0a 2020 2020 2020 2020  cution..        
-0000f440: 2222 220a 2020 2020 2020 2020 2320 4368  """.        # Ch
-0000f450: 6563 6b20 7468 6174 2074 6865 2075 6e64  eck that the und
-0000f460: 6572 6c79 696e 6720 736b 6c65 6172 6e20  erlying sklearn 
-0000f470: 6d6f 6465 6c20 6861 7320 6265 656e 2073  model has been s
-0000f480: 6574 2061 6e64 2066 6974 0a20 2020 2020  et and fit.     
-0000f490: 2020 2061 7373 6572 7420 7365 6c66 2e73     assert self.s
-0000f4a0: 6b6c 6561 726e 5f6d 6f64 656c 2069 7320  klearn_model is 
-0000f4b0: 6e6f 7420 4e6f 6e65 2c20 7365 6c66 2e5f  not None, self._
-0000f4c0: 736b 6c65 6172 6e5f 6d6f 6465 6c5f 6973  sklearn_model_is
-0000f4d0: 5f6e 6f74 5f66 6974 7465 645f 6572 726f  _not_fitted_erro
-0000f4e0: 725f 6d65 7373 6167 6528 290a 0a20 2020  r_message()..   
-0000f4f0: 2020 2020 2073 656c 662e 6f6e 6e78 5f6d       self.onnx_m
-0000f500: 6f64 656c 5f20 3d20 6862 5f63 6f6e 7665  odel_ = hb_conve
-0000f510: 7274 280a 2020 2020 2020 2020 2020 2020  rt(.            
-0000f520: 7365 6c66 2e73 6b6c 6561 726e 5f6d 6f64  self.sklearn_mod
-0000f530: 656c 2c0a 2020 2020 2020 2020 2020 2020  el,.            
-0000f540: 6261 636b 656e 643d 226f 6e6e 7822 2c0a  backend="onnx",.
-0000f550: 2020 2020 2020 2020 2020 2020 7465 7374              test
-0000f560: 5f69 6e70 7574 3d74 6573 745f 696e 7075  _input=test_inpu
-0000f570: 742c 0a20 2020 2020 2020 2020 2020 2065  t,.            e
-0000f580: 7874 7261 5f63 6f6e 6669 673d 7b22 6f6e  xtra_config={"on
-0000f590: 6e78 5f74 6172 6765 745f 6f70 7365 7422  nx_target_opset"
-0000f5a0: 3a20 4f50 5345 545f 5645 5253 494f 4e5f  : OPSET_VERSION_
-0000f5b0: 464f 525f 4f4e 4e58 5f45 5850 4f52 547d  FOR_ONNX_EXPORT}
-0000f5c0: 2c0a 2020 2020 2020 2020 292e 6d6f 6465  ,.        ).mode
-0000f5d0: 6c0a 0a20 2020 2020 2020 2073 656c 662e  l..        self.
-0000f5e0: 5f63 6c65 616e 5f67 7261 7068 2829 0a0a  _clean_graph()..
-0000f5f0: 2020 2020 6465 6620 5f63 6c65 616e 5f67      def _clean_g
-0000f600: 7261 7068 2873 656c 6629 202d 3e20 4e6f  raph(self) -> No
-0000f610: 6e65 3a0a 2020 2020 2020 2020 2222 2243  ne:.        """C
-0000f620: 6c65 616e 2074 6865 204f 4e4e 5820 6772  lean the ONNX gr
-0000f630: 6170 6820 6672 6f6d 2075 6e64 6573 6972  aph from undesir
-0000f640: 6564 206e 6f64 6573 2e22 2222 0a20 2020  ed nodes.""".   
-0000f650: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
-0000f660: 2e6f 6e6e 785f 6d6f 6465 6c5f 2069 7320  .onnx_model_ is 
-0000f670: 6e6f 7420 4e6f 6e65 2c20 7365 6c66 2e5f  not None, self._
-0000f680: 6973 5f6e 6f74 5f66 6974 7465 645f 6572  is_not_fitted_er
-0000f690: 726f 725f 6d65 7373 6167 6528 290a 0a20  ror_message().. 
-0000f6a0: 2020 2020 2020 2023 2052 656d 6f76 6520         # Remove 
-0000f6b0: 6361 7374 206f 7065 7261 746f 7273 2061  cast operators a
-0000f6c0: 7320 7468 6579 2061 7265 206e 6f74 206e  s they are not n
-0000f6d0: 6565 6465 640a 2020 2020 2020 2020 7265  eeded.        re
-0000f6e0: 6d6f 7665 5f6e 6f64 655f 7479 7065 7328  move_node_types(
-0000f6f0: 6f6e 6e78 5f6d 6f64 656c 3d73 656c 662e  onnx_model=self.
-0000f700: 6f6e 6e78 5f6d 6f64 656c 5f2c 206f 705f  onnx_model_, op_
-0000f710: 7479 7065 735f 746f 5f72 656d 6f76 653d  types_to_remove=
-0000f720: 5b22 4361 7374 225d 290a 0a20 2020 2064  ["Cast"])..    d
-0000f730: 6566 2066 6974 2873 656c 662c 2058 3a20  ef fit(self, X: 
-0000f740: 4461 7461 2c20 793a 2054 6172 6765 742c  Data, y: Target,
-0000f750: 202a 2a66 6974 5f70 6172 616d 6574 6572   **fit_parameter
-0000f760: 7329 3a0a 2020 2020 2020 2020 2320 5265  s):.        # Re
-0000f770: 7365 7420 666f 7220 646f 7562 6c65 2066  set for double f
-0000f780: 6974 0a20 2020 2020 2020 2073 656c 662e  it.        self.
-0000f790: 5f69 735f 6669 7474 6564 203d 2046 616c  _is_fitted = Fal
-0000f7a0: 7365 0a20 2020 2020 2020 2073 656c 662e  se.        self.
-0000f7b0: 696e 7075 745f 7175 616e 7469 7a65 7273  input_quantizers
-0000f7c0: 203d 205b 5d0a 2020 2020 2020 2020 7365   = [].        se
-0000f7d0: 6c66 2e6f 7574 7075 745f 7175 616e 7469  lf.output_quanti
-0000f7e0: 7a65 7273 203d 205b 5d0a 0a20 2020 2020  zers = []..     
-0000f7f0: 2020 2023 204c 696e 6561 7252 6567 7265     # LinearRegre
-0000f800: 7373 696f 6e20 6861 6e64 6c65 7320 6d75  ssion handles mu
-0000f810: 6c74 692d 6c61 6265 6c73 2064 6174 610a  lti-labels data.
-0000f820: 2020 2020 2020 2020 582c 2079 203d 2063          X, y = c
-0000f830: 6865 636b 5f58 5f79 5f61 6e64 5f61 7373  heck_X_y_and_ass
-0000f840: 6572 745f 6d75 6c74 695f 6f75 7470 7574  ert_multi_output
-0000f850: 2858 2c20 7929 0a0a 2020 2020 2020 2020  (X, y)..        
-0000f860: 2320 4669 7420 7468 6520 7363 696b 6974  # Fit the scikit
-0000f870: 2d6c 6561 726e 206d 6f64 656c 0a20 2020  -learn model.   
-0000f880: 2020 2020 2073 656c 662e 5f66 6974 5f73       self._fit_s
-0000f890: 6b6c 6561 726e 5f6d 6f64 656c 2858 2c20  klearn_model(X, 
-0000f8a0: 792c 202a 2a66 6974 5f70 6172 616d 6574  y, **fit_paramet
-0000f8b0: 6572 7329 0a0a 2020 2020 2020 2020 2320  ers)..        # 
-0000f8c0: 436f 6d70 7574 6520 7468 6520 7175 616e  Compute the quan
-0000f8d0: 7469 7a61 7469 6f6e 2070 6172 616d 6574  tization paramet
-0000f8e0: 6572 730a 2020 2020 2020 2020 7265 7475  ers.        retu
-0000f8f0: 726e 2073 656c 662e 5f71 7561 6e74 697a  rn self._quantiz
-0000f900: 655f 6d6f 6465 6c28 5829 0a0a 2020 2020  e_model(X)..    
-0000f910: 6465 6620 5f71 7561 6e74 697a 655f 6d6f  def _quantize_mo
-0000f920: 6465 6c28 7365 6c66 2c20 5829 3a0a 2020  del(self, X):.  
-0000f930: 2020 2020 2020 2222 2243 6f6d 7075 7465        """Compute
-0000f940: 2071 7561 6e74 697a 6174 696f 6e20 7061   quantization pa
-0000f950: 7261 6d65 7465 7273 2e0a 0a20 2020 2020  rameters...     
-0000f960: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-0000f970: 2020 2020 2058 2028 4461 7461 293a 2041       X (Data): A
-0000f980: 2072 6570 7265 7365 6e74 6174 6976 6520   representative 
-0000f990: 7365 7420 6f66 2069 6e70 7574 2076 616c  set of input val
-0000f9a0: 7565 7320 7573 6564 2066 6f72 2063 6f6d  ues used for com
-0000f9b0: 7075 7469 6e67 2071 7561 6e74 697a 6174  puting quantizat
-0000f9c0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-0000f9d0: 2020 2020 7061 7261 6d65 7465 7273 2c20      parameters, 
-0000f9e0: 6173 2061 204e 756d 7079 2061 7272 6179  as a Numpy array
-0000f9f0: 2c20 546f 7263 6820 7465 6e73 6f72 2c20  , Torch tensor, 
-0000fa00: 5061 6e64 6173 2044 6174 6146 7261 6d65  Pandas DataFrame
-0000fa10: 206f 7220 4c69 7374 2e20 5468 6973 2069   or List. This i
-0000fa20: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-0000fa30: 2020 7573 7561 6c6c 7920 7468 6520 7472    usually the tr
-0000fa40: 6169 6e69 6e67 2064 6174 612d 7365 7420  aining data-set 
-0000fa50: 6f72 2061 2073 7562 2d73 6574 206f 6620  or a sub-set of 
-0000fa60: 6974 2e0a 0a20 2020 2020 2020 2052 6574  it...        Ret
-0000fa70: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
-0000fa80: 2020 5468 6520 4648 452d 636f 6d70 6c69    The FHE-compli
-0000fa90: 616e 7420 6669 7474 6564 206d 6f64 656c  ant fitted model
-0000faa0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-0000fab0: 2020 2020 2020 2320 4368 6563 6b20 7468        # Check th
-0000fac0: 6174 2074 6865 2075 6e64 6572 6c79 696e  at the underlyin
-0000fad0: 6720 736b 6c65 6172 6e20 6d6f 6465 6c20  g sklearn model 
-0000fae0: 6861 7320 6265 656e 2073 6574 2061 6e64  has been set and
-0000faf0: 2066 6974 0a20 2020 2020 2020 2061 7373   fit.        ass
-0000fb00: 6572 7420 7365 6c66 2e73 6b6c 6561 726e  ert self.sklearn
-0000fb10: 5f6d 6f64 656c 2069 7320 6e6f 7420 4e6f  _model is not No
-0000fb20: 6e65 2c20 7365 6c66 2e5f 736b 6c65 6172  ne, self._sklear
-0000fb30: 6e5f 6d6f 6465 6c5f 6973 5f6e 6f74 5f66  n_model_is_not_f
-0000fb40: 6974 7465 645f 6572 726f 725f 6d65 7373  itted_error_mess
-0000fb50: 6167 6528 290a 0a20 2020 2020 2020 2023  age()..        #
-0000fb60: 2052 6574 7269 6576 6520 7468 6520 4f4e   Retrieve the ON
-0000fb70: 4e58 2067 7261 7068 0a20 2020 2020 2020  NX graph.       
-0000fb80: 2073 656c 662e 5f73 6574 5f6f 6e6e 785f   self._set_onnx_
-0000fb90: 6d6f 6465 6c28 5829 0a0a 2020 2020 2020  model(X)..      
-0000fba0: 2020 2320 436f 6e76 6572 7420 7468 6520    # Convert the 
-0000fbb0: 6e5f 6269 7473 2061 7474 7269 6275 7465  n_bits attribute
-0000fbc0: 2069 6e74 6f20 6120 7072 6f70 6572 2064   into a proper d
-0000fbd0: 6963 7469 6f6e 6172 790a 2020 2020 2020  ictionary.      
-0000fbe0: 2020 6e5f 6269 7473 203d 2067 6574 5f6e    n_bits = get_n
-0000fbf0: 5f62 6974 735f 6469 6374 2873 656c 662e  _bits_dict(self.
-0000fc00: 6e5f 6269 7473 290a 0a20 2020 2020 2020  n_bits)..       
-0000fc10: 2069 6e70 7574 5f6e 5f62 6974 7320 3d20   input_n_bits = 
-0000fc20: 6e5f 6269 7473 5b22 6f70 5f69 6e70 7574  n_bits["op_input
-0000fc30: 7322 5d0a 2020 2020 2020 2020 696e 7075  s"].        inpu
-0000fc40: 745f 6f70 7469 6f6e 7320 3d20 5175 616e  t_options = Quan
-0000fc50: 7469 7a61 7469 6f6e 4f70 7469 6f6e 7328  tizationOptions(
-0000fc60: 6e5f 6269 7473 3d69 6e70 7574 5f6e 5f62  n_bits=input_n_b
-0000fc70: 6974 732c 2069 735f 7369 676e 6564 3d54  its, is_signed=T
-0000fc80: 7275 6529 0a0a 2020 2020 2020 2020 2320  rue)..        # 
-0000fc90: 5175 616e 7469 7a65 2074 6865 2069 6e70  Quantize the inp
-0000fca0: 7574 7320 616e 6420 7374 6f72 6520 7468  uts and store th
-0000fcb0: 6520 6173 736f 6369 6174 6564 2071 7561  e associated qua
-0000fcc0: 6e74 697a 6572 0a20 2020 2020 2020 2071  ntizer.        q
-0000fcd0: 5f69 6e70 7574 7320 3d20 5175 616e 7469  _inputs = Quanti
-0000fce0: 7a65 6441 7272 6179 286e 5f62 6974 733d  zedArray(n_bits=
-0000fcf0: 696e 7075 745f 6e5f 6269 7473 2c20 7661  input_n_bits, va
-0000fd00: 6c75 6573 3d58 2c20 6f70 7469 6f6e 733d  lues=X, options=
-0000fd10: 696e 7075 745f 6f70 7469 6f6e 7329 0a20  input_options). 
-0000fd20: 2020 2020 2020 2069 6e70 7574 5f71 7561         input_qua
-0000fd30: 6e74 697a 6572 203d 2071 5f69 6e70 7574  ntizer = q_input
-0000fd40: 732e 7175 616e 7469 7a65 720a 2020 2020  s.quantizer.    
-0000fd50: 2020 2020 7365 6c66 2e69 6e70 7574 5f71      self.input_q
-0000fd60: 7561 6e74 697a 6572 7320 3d20 5b69 6e70  uantizers = [inp
-0000fd70: 7574 5f71 7561 6e74 697a 6572 5d0a 0a20  ut_quantizer].. 
-0000fd80: 2020 2020 2020 2077 6569 6768 7473 5f6e         weights_n
-0000fd90: 5f62 6974 7320 3d20 6e5f 6269 7473 5b22  _bits = n_bits["
-0000fda0: 6f70 5f77 6569 6768 7473 225d 0a20 2020  op_weights"].   
-0000fdb0: 2020 2020 2077 6569 6768 745f 6f70 7469       weight_opti
-0000fdc0: 6f6e 7320 3d20 5175 616e 7469 7a61 7469  ons = Quantizati
-0000fdd0: 6f6e 4f70 7469 6f6e 7328 6e5f 6269 7473  onOptions(n_bits
-0000fde0: 3d77 6569 6768 7473 5f6e 5f62 6974 732c  =weights_n_bits,
-0000fdf0: 2069 735f 7369 676e 6564 3d54 7275 6529   is_signed=True)
-0000fe00: 0a0a 2020 2020 2020 2020 2320 5175 616e  ..        # Quan
-0000fe10: 7469 7a65 2074 6865 2077 6569 6768 7473  tize the weights
-0000fe20: 2061 6e64 2073 746f 7265 2074 6865 2061   and store the a
-0000fe30: 7373 6f63 6961 7465 6420 7175 616e 7469  ssociated quanti
-0000fe40: 7a65 720a 2020 2020 2020 2020 2320 5472  zer.        # Tr
-0000fe50: 616e 7370 6f73 6520 616e 6420 6578 7061  anspose and expa
-0000fe60: 6e64 2061 7265 206e 6563 6573 7361 7279  nd are necessary
-0000fe70: 2069 6e20 6f72 6465 7220 746f 206d 616b   in order to mak
-0000fe80: 6520 7375 7265 2074 6865 2077 6569 6768  e sure the weigh
-0000fe90: 7420 6172 7261 7920 6861 7320 7468 6520  t array has the 
-0000fea0: 636f 7272 6563 740a 2020 2020 2020 2020  correct.        
-0000feb0: 2320 7368 6170 6520 7768 656e 2063 616c  # shape when cal
-0000fec0: 6c69 6e67 2074 6865 2047 656d 6d20 6f70  ling the Gemm op
-0000fed0: 6572 6174 6f72 206f 6e20 6974 0a20 2020  erator on it.   
-0000fee0: 2020 2020 2077 6569 6768 7473 203d 2073       weights = s
-0000fef0: 656c 662e 736b 6c65 6172 6e5f 6d6f 6465  elf.sklearn_mode
-0000ff00: 6c2e 636f 6566 5f2e 540a 2020 2020 2020  l.coef_.T.      
-0000ff10: 2020 715f 7765 6967 6874 7320 3d20 5175    q_weights = Qu
-0000ff20: 616e 7469 7a65 6441 7272 6179 280a 2020  antizedArray(.  
-0000ff30: 2020 2020 2020 2020 2020 6e5f 6269 7473            n_bits
-0000ff40: 3d6e 5f62 6974 735b 226f 705f 7765 6967  =n_bits["op_weig
-0000ff50: 6874 7322 5d2c 0a20 2020 2020 2020 2020  hts"],.         
-0000ff60: 2020 2076 616c 7565 733d 6e75 6d70 792e     values=numpy.
-0000ff70: 6578 7061 6e64 5f64 696d 7328 7765 6967  expand_dims(weig
-0000ff80: 6874 732c 2061 7869 733d 3129 2069 6620  hts, axis=1) if 
-0000ff90: 6c65 6e28 7765 6967 6874 732e 7368 6170  len(weights.shap
-0000ffa0: 6529 203d 3d20 3120 656c 7365 2077 6569  e) == 1 else wei
-0000ffb0: 6768 7473 2c0a 2020 2020 2020 2020 2020  ghts,.          
-0000ffc0: 2020 6f70 7469 6f6e 733d 7765 6967 6874    options=weight
-0000ffd0: 5f6f 7074 696f 6e73 2c0a 2020 2020 2020  _options,.      
-0000ffe0: 2020 290a 2020 2020 2020 2020 7365 6c66    ).        self
-0000fff0: 2e5f 715f 7765 6967 6874 7320 3d20 715f  ._q_weights = q_
-00010000: 7765 6967 6874 732e 7176 616c 7565 730a  weights.qvalues.
-00010010: 2020 2020 2020 2020 7765 6967 6874 5f71          weight_q
-00010020: 7561 6e74 697a 6572 203d 2071 5f77 6569  uantizer = q_wei
-00010030: 6768 7473 2e71 7561 6e74 697a 6572 0a20  ghts.quantizer. 
-00010040: 2020 2020 2020 2073 656c 662e 5f77 6569         self._wei
-00010050: 6768 745f 7175 616e 7469 7a65 7220 3d20  ght_quantizer = 
-00010060: 7765 6967 6874 5f71 7561 6e74 697a 6572  weight_quantizer
-00010070: 0a0a 2020 2020 2020 2020 2320 6d79 7079  ..        # mypy
-00010080: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00010090: 696e 7075 745f 7175 616e 7469 7a65 722e  input_quantizer.
-000100a0: 7363 616c 6520 6973 206e 6f74 204e 6f6e  scale is not Non
-000100b0: 650a 2020 2020 2020 2020 6173 7365 7274  e.        assert
-000100c0: 2077 6569 6768 745f 7175 616e 7469 7a65   weight_quantize
-000100d0: 722e 7363 616c 6520 6973 206e 6f74 204e  r.scale is not N
-000100e0: 6f6e 650a 0a20 2020 2020 2020 2023 2043  one..        # C
-000100f0: 6f6d 7075 7465 2074 6865 2073 6361 6c65  ompute the scale
-00010100: 2061 6e64 207a 6572 6f2d 706f 696e 7420   and zero-point 
-00010110: 6f66 2074 6865 206d 6174 6d75 6c27 7320  of the matmul's 
-00010120: 6f75 7470 7574 732c 2066 6f6c 6c6f 7769  outputs, followi
-00010130: 6e67 2074 6865 2073 616d 6520 7374 6570  ng the same step
-00010140: 7320 6672 6f6d 0a20 2020 2020 2020 2023  s from.        #
-00010150: 2074 6865 2051 7561 6e74 697a 6564 4765   the QuantizedGe
-00010160: 6d6d 206f 7065 7261 746f 722c 2077 6869  mm operator, whi
-00010170: 6368 2061 7265 2062 6173 6564 206f 6e20  ch are based on 
-00010180: 6571 7561 7469 6f6e 7320 6465 7461 696c  equations detail
-00010190: 6564 2069 6e0a 2020 2020 2020 2020 2320  ed in.        # 
-000101a0: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
-000101b0: 672f 6162 732f 3137 3132 2e30 3538 3737  g/abs/1712.05877
-000101c0: 0a20 2020 2020 2020 206f 7574 7075 745f  .        output_
-000101d0: 7175 616e 745f 7061 7261 6d73 203d 2055  quant_params = U
-000101e0: 6e69 666f 726d 5175 616e 7469 7a61 7469  niformQuantizati
-000101f0: 6f6e 5061 7261 6d65 7465 7273 280a 2020  onParameters(.  
-00010200: 2020 2020 2020 2020 2020 7363 616c 653d            scale=
-00010210: 696e 7075 745f 7175 616e 7469 7a65 722e  input_quantizer.
-00010220: 7363 616c 6520 2a20 7765 6967 6874 5f71  scale * weight_q
-00010230: 7561 6e74 697a 6572 2e73 6361 6c65 2c0a  uantizer.scale,.
-00010240: 2020 2020 2020 2020 2020 2020 7a65 726f              zero
-00010250: 5f70 6f69 6e74 3d69 6e70 7574 5f71 7561  _point=input_qua
-00010260: 6e74 697a 6572 2e7a 6572 6f5f 706f 696e  ntizer.zero_poin
-00010270: 740a 2020 2020 2020 2020 2020 2020 2a20  t.            * 
-00010280: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00010290: 2020 6e75 6d70 792e 7375 6d28 7365 6c66    numpy.sum(self
-000102a0: 2e5f 715f 7765 6967 6874 732c 2061 7869  ._q_weights, axi
-000102b0: 733d 302c 206b 6565 7064 696d 733d 5472  s=0, keepdims=Tr
-000102c0: 7565 290a 2020 2020 2020 2020 2020 2020  ue).            
-000102d0: 2020 2020 2d20 582e 7368 6170 655b 315d      - X.shape[1]
-000102e0: 202a 2077 6569 6768 745f 7175 616e 7469   * weight_quanti
-000102f0: 7a65 722e 7a65 726f 5f70 6f69 6e74 0a20  zer.zero_point. 
-00010300: 2020 2020 2020 2020 2020 2029 2c0a 2020             ),.  
-00010310: 2020 2020 2020 2020 2020 6f66 6673 6574            offset
-00010320: 3d30 2c0a 2020 2020 2020 2020 290a 0a20  =0,.        ).. 
-00010330: 2020 2020 2020 206f 7574 7075 745f 7175         output_qu
-00010340: 616e 7469 7a65 7220 3d20 556e 6966 6f72  antizer = Unifor
-00010350: 6d51 7561 6e74 697a 6572 2870 6172 616d  mQuantizer(param
-00010360: 733d 6f75 7470 7574 5f71 7561 6e74 5f70  s=output_quant_p
-00010370: 6172 616d 732c 206e 6f5f 636c 6970 7069  arams, no_clippi
-00010380: 6e67 3d54 7275 6529 0a0a 2020 2020 2020  ng=True)..      
-00010390: 2020 2320 5175 616e 7469 7a65 2074 6865    # Quantize the
-000103a0: 2062 6961 7320 7573 696e 6720 7468 6520   bias using the 
-000103b0: 6d61 746d 756c 2773 2073 6361 6c65 2061  matmul's scale a
-000103c0: 6e64 207a 6572 6f2d 706f 696e 742c 2073  nd zero-point, s
-000103d0: 7563 6820 7468 6174 0a20 2020 2020 2020  uch that.       
-000103e0: 2023 2071 5f62 6961 7320 3d20 726f 756e   # q_bias = roun
-000103f0: 6428 2831 2f53 292a 6269 6173 202b 205a  d((1/S)*bias + Z
-00010400: 290a 2020 2020 2020 2020 7365 6c66 2e5f  ).        self._
-00010410: 715f 6269 6173 203d 206f 7574 7075 745f  q_bias = output_
-00010420: 7175 616e 7469 7a65 722e 7175 616e 7428  quantizer.quant(
-00010430: 7365 6c66 2e73 6b6c 6561 726e 5f6d 6f64  self.sklearn_mod
-00010440: 656c 2e69 6e74 6572 6365 7074 5f29 0a0a  el.intercept_)..
-00010450: 2020 2020 2020 2020 2320 5369 6e63 6520          # Since 
-00010460: 7468 6520 6d61 746d 756c 2061 6e64 2074  the matmul and t
-00010470: 6865 2062 6961 7320 626f 7468 2075 7365  he bias both use
-00010480: 2074 6865 2073 616d 6520 7363 616c 6520   the same scale 
-00010490: 616e 6420 7a65 726f 2d70 6f69 6e74 732c  and zero-points,
-000104a0: 2077 6520 6f62 7461 696e 2074 6861 740a   we obtain that.
-000104b0: 2020 2020 2020 2020 2320 7920 3d20 532a          # y = S*
-000104c0: 2871 5f79 202d 2032 2a5a 2920 7768 656e  (q_y - 2*Z) when
-000104d0: 2064 652d 7175 616e 7469 7a69 6e67 2074   de-quantizing t
-000104e0: 6865 2076 616c 7565 732e 2057 6520 7468  he values. We th
-000104f0: 6572 6566 6f72 6520 6e65 6564 2074 6f20  erefore need to 
-00010500: 6d75 6c74 6970 6c79 2074 6865 2069 6e69  multiply the ini
-00010510: 7469 616c 0a20 2020 2020 2020 2023 206f  tial.        # o
-00010520: 7574 7075 7420 7a65 726f 5f70 6f69 6e74  utput zero_point
-00010530: 2062 7920 320a 2020 2020 2020 2020 6173   by 2.        as
-00010540: 7365 7274 206f 7574 7075 745f 7175 616e  sert output_quan
-00010550: 7469 7a65 722e 7a65 726f 5f70 6f69 6e74  tizer.zero_point
-00010560: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
-00010570: 2020 2020 206f 7574 7075 745f 7175 616e       output_quan
-00010580: 7469 7a65 722e 7a65 726f 5f70 6f69 6e74  tizer.zero_point
-00010590: 202a 3d20 320a 2020 2020 2020 2020 7365   *= 2.        se
-000105a0: 6c66 2e6f 7574 7075 745f 7175 616e 7469  lf.output_quanti
-000105b0: 7a65 7273 203d 205b 6f75 7470 7574 5f71  zers = [output_q
-000105c0: 7561 6e74 697a 6572 5d0a 0a20 2020 2020  uantizer]..     
-000105d0: 2020 2023 2055 7064 6174 696e 6720 706f     # Updating po
-000105e0: 7374 2d70 726f 6365 7373 696e 6720 7061  st-processing pa
-000105f0: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-00010600: 2073 656c 662e 5f73 6574 5f70 6f73 745f   self._set_post_
-00010610: 7072 6f63 6573 7369 6e67 5f70 6172 616d  processing_param
-00010620: 7328 290a 0a20 2020 2020 2020 2073 656c  s()..        sel
-00010630: 662e 5f69 735f 6669 7474 6564 203d 2054  f._is_fitted = T
-00010640: 7275 650a 0a20 2020 2020 2020 2072 6574  rue..        ret
-00010650: 7572 6e20 7365 6c66 0a0a 2020 2020 6465  urn self..    de
-00010660: 6620 7175 616e 7469 7a65 5f69 6e70 7574  f quantize_input
-00010670: 2873 656c 662c 2058 3a20 6e75 6d70 792e  (self, X: numpy.
-00010680: 6e64 6172 7261 7929 202d 3e20 6e75 6d70  ndarray) -> nump
-00010690: 792e 6e64 6172 7261 793a 0a20 2020 2020  y.ndarray:.     
-000106a0: 2020 2073 656c 662e 6368 6563 6b5f 6d6f     self.check_mo
-000106b0: 6465 6c5f 6973 5f66 6974 7465 6428 290a  del_is_fitted().
-000106c0: 2020 2020 2020 2020 715f 5820 3d20 7365          q_X = se
-000106d0: 6c66 2e69 6e70 7574 5f71 7561 6e74 697a  lf.input_quantiz
-000106e0: 6572 735b 305d 2e71 7561 6e74 2858 290a  ers[0].quant(X).
-000106f0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00010700: 715f 582e 6474 7970 6520 3d3d 206e 756d  q_X.dtype == num
-00010710: 7079 2e69 6e74 3634 2c20 2249 6e70 7574  py.int64, "Input
-00010720: 7320 7765 7265 206e 6f74 2071 7561 6e74  s were not quant
-00010730: 697a 6564 2074 6f20 696e 7436 3420 7661  ized to int64 va
-00010740: 6c75 6573 220a 2020 2020 2020 2020 7265  lues".        re
-00010750: 7475 726e 2071 5f58 0a0a 2020 2020 6465  turn q_X..    de
-00010760: 6620 6465 7175 616e 7469 7a65 5f6f 7574  f dequantize_out
-00010770: 7075 7428 7365 6c66 2c20 715f 795f 7072  put(self, q_y_pr
-00010780: 6564 733a 206e 756d 7079 2e6e 6461 7272  eds: numpy.ndarr
-00010790: 6179 2920 2d3e 206e 756d 7079 2e6e 6461  ay) -> numpy.nda
-000107a0: 7272 6179 3a0a 2020 2020 2020 2020 7365  rray:.        se
-000107b0: 6c66 2e63 6865 636b 5f6d 6f64 656c 5f69  lf.check_model_i
-000107c0: 735f 6669 7474 6564 2829 0a0a 2020 2020  s_fitted()..    
-000107d0: 2020 2020 2320 4465 2d71 7561 6e74 697a      # De-quantiz
-000107e0: 6520 7468 6520 6f75 7470 7574 2076 616c  e the output val
-000107f0: 7565 730a 2020 2020 2020 2020 795f 7072  ues.        y_pr
-00010800: 6564 7320 3d20 7365 6c66 2e6f 7574 7075  eds = self.outpu
-00010810: 745f 7175 616e 7469 7a65 7273 5b30 5d2e  t_quantizers[0].
-00010820: 6465 7175 616e 7428 715f 795f 7072 6564  dequant(q_y_pred
-00010830: 7329 0a0a 2020 2020 2020 2020 7265 7475  s)..        retu
-00010840: 726e 2079 5f70 7265 6473 0a0a 2020 2020  rn y_preds..    
-00010850: 6465 6620 5f67 6574 5f6d 6f64 756c 655f  def _get_module_
-00010860: 746f 5f63 6f6d 7069 6c65 2873 656c 6629  to_compile(self)
-00010870: 202d 3e20 556e 696f 6e5b 436f 6d70 696c   -> Union[Compil
-00010880: 6572 2c20 5175 616e 7469 7a65 644d 6f64  er, QuantizedMod
-00010890: 756c 655d 3a0a 2020 2020 2020 2020 2320  ule]:.        # 
-000108a0: 4465 6669 6e65 2074 6865 2069 6e66 6572  Define the infer
-000108b0: 656e 6365 2066 756e 6374 696f 6e20 746f  ence function to
-000108c0: 2063 6f6d 7069 6c65 2e0a 2020 2020 2020   compile..      
-000108d0: 2020 2320 5468 6973 2066 756e 6374 696f    # This functio
-000108e0: 6e20 6361 6e20 6e65 6974 6865 7220 6265  n can neither be
-000108f0: 2061 2063 6c61 7373 206d 6574 686f 6420   a class method 
-00010900: 6e6f 7220 6120 7374 6174 6963 206f 6e65  nor a static one
-00010910: 2062 6563 6175 7365 2073 656c 6620 7765   because self we
-00010920: 2077 616e 7420 746f 2061 766f 6964 0a20   want to avoid. 
-00010930: 2020 2020 2020 2023 2068 6176 696e 6720         # having 
-00010940: 7365 6c66 2061 7320 6120 7061 7261 6d65  self as a parame
-00010950: 7465 7220 7768 696c 6520 7374 696c 6c20  ter while still 
-00010960: 6265 696e 6720 6162 6c65 2074 6f20 6163  being able to ac
-00010970: 6365 7373 2073 6f6d 6520 6f66 2069 7473  cess some of its
-00010980: 2061 7474 7269 6275 7465 0a20 2020 2020   attribute.     
-00010990: 2020 2064 6566 2069 6e66 6572 656e 6365     def inference
-000109a0: 5f74 6f5f 636f 6d70 696c 6528 715f 583a  _to_compile(q_X:
-000109b0: 206e 756d 7079 2e6e 6461 7272 6179 2920   numpy.ndarray) 
-000109c0: 2d3e 206e 756d 7079 2e6e 6461 7272 6179  -> numpy.ndarray
-000109d0: 3a0a 2020 2020 2020 2020 2020 2020 2222  :.            ""
-000109e0: 2243 6f6d 7069 6c65 2074 6865 2063 6972  "Compile the cir
-000109f0: 6375 6974 2069 6e20 4648 4520 7573 696e  cuit in FHE usin
-00010a00: 6720 6f6e 6c79 2074 6865 2069 6e70 7574  g only the input
-00010a10: 7320 6173 2070 6172 616d 6574 6572 732e  s as parameters.
-00010a20: 0a0a 2020 2020 2020 2020 2020 2020 4172  ..            Ar
-00010a30: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00010a40: 2020 2020 715f 5820 286e 756d 7079 2e6e      q_X (numpy.n
-00010a50: 6461 7272 6179 293a 2054 6865 2071 7561  darray): The qua
-00010a60: 6e74 697a 6564 2069 6e70 7574 2064 6174  ntized input dat
-00010a70: 610a 0a20 2020 2020 2020 2020 2020 2052  a..            R
-00010a80: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-00010a90: 2020 2020 2020 2020 6e75 6d70 792e 6e64          numpy.nd
-00010aa0: 6172 7261 793a 2054 6865 2063 6972 6375  array: The circu
-00010ab0: 6974 2069 7320 6f75 7470 7574 732e 0a20  it is outputs.. 
-00010ac0: 2020 2020 2020 2020 2020 2022 2222 0a20             """. 
-00010ad0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00010ae0: 6e20 7365 6c66 2e5f 696e 6665 7265 6e63  n self._inferenc
-00010af0: 6528 715f 5829 0a0a 2020 2020 2020 2020  e(q_X)..        
-00010b00: 2320 4372 6561 7465 2074 6865 2063 6f6d  # Create the com
-00010b10: 7069 6c65 7220 696e 7374 616e 6365 0a20  piler instance. 
-00010b20: 2020 2020 2020 2063 6f6d 7069 6c65 7220         compiler 
-00010b30: 3d20 436f 6d70 696c 6572 2869 6e66 6572  = Compiler(infer
-00010b40: 656e 6365 5f74 6f5f 636f 6d70 696c 652c  ence_to_compile,
-00010b50: 207b 2271 5f58 223a 2022 656e 6372 7970   {"q_X": "encryp
-00010b60: 7465 6422 7d29 0a0a 2020 2020 2020 2020  ted"})..        
-00010b70: 7265 7475 726e 2063 6f6d 7069 6c65 720a  return compiler.
-00010b80: 0a20 2020 2064 6566 205f 696e 6665 7265  .    def _infere
-00010b90: 6e63 6528 7365 6c66 2c20 715f 583a 206e  nce(self, q_X: n
-00010ba0: 756d 7079 2e6e 6461 7272 6179 2920 2d3e  umpy.ndarray) ->
-00010bb0: 206e 756d 7079 2e6e 6461 7272 6179 3a0a   numpy.ndarray:.
-00010bc0: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
-00010bd0: 656c 662e 5f77 6569 6768 745f 7175 616e  elf._weight_quan
-00010be0: 7469 7a65 7220 6973 206e 6f74 204e 6f6e  tizer is not Non
-00010bf0: 652c 2073 656c 662e 5f69 735f 6e6f 745f  e, self._is_not_
-00010c00: 6669 7474 6564 5f65 7272 6f72 5f6d 6573  fitted_error_mes
-00010c10: 7361 6765 2829 0a0a 2020 2020 2020 2020  sage()..        
-00010c20: 2320 5175 616e 7469 7a69 6e67 2077 6569  # Quantizing wei
-00010c30: 6768 7473 2061 6e64 2069 6e70 7574 7320  ghts and inputs 
-00010c40: 6d61 6b65 7320 616e 2061 6464 6974 696f  makes an additio
-00010c50: 6e61 6c20 7465 726d 2061 7070 6561 7220  nal term appear 
-00010c60: 696e 2074 6865 2069 6e66 6572 656e 6365  in the inference
-00010c70: 2066 756e 6374 696f 6e0a 2020 2020 2020   function.      
-00010c80: 2020 795f 7072 6564 203d 2071 5f58 2040    y_pred = q_X @
-00010c90: 2073 656c 662e 5f71 5f77 6569 6768 7473   self._q_weights
-00010ca0: 202d 2073 656c 662e 5f77 6569 6768 745f   - self._weight_
-00010cb0: 7175 616e 7469 7a65 722e 7a65 726f 5f70  quantizer.zero_p
-00010cc0: 6f69 6e74 202a 206e 756d 7079 2e73 756d  oint * numpy.sum
-00010cd0: 280a 2020 2020 2020 2020 2020 2020 715f  (.            q_
-00010ce0: 582c 2061 7869 733d 312c 206b 6565 7064  X, axis=1, keepd
-00010cf0: 696d 733d 5472 7565 0a20 2020 2020 2020  ims=True.       
-00010d00: 2029 0a20 2020 2020 2020 2079 5f70 7265   ).        y_pre
-00010d10: 6420 2b3d 2073 656c 662e 5f71 5f62 6961  d += self._q_bia
-00010d20: 730a 2020 2020 2020 2020 7265 7475 726e  s.        return
-00010d30: 2079 5f70 7265 640a 0a0a 636c 6173 7320   y_pred...class 
-00010d40: 536b 6c65 6172 6e4c 696e 6561 7252 6567  SklearnLinearReg
-00010d50: 7265 7373 6f72 4d69 7869 6e28 536b 6c65  ressorMixin(Skle
-00010d60: 6172 6e4c 696e 6561 724d 6f64 656c 4d69  arnLinearModelMi
-00010d70: 7869 6e2c 2073 6b6c 6561 726e 2e62 6173  xin, sklearn.bas
-00010d80: 652e 5265 6772 6573 736f 724d 6978 696e  e.RegressorMixin
-00010d90: 2c20 4142 4329 3a0a 2020 2020 2222 2241  , ABC):.    """A
-00010da0: 204d 6978 696e 2063 6c61 7373 2066 6f72   Mixin class for
-00010db0: 2073 6b6c 6561 726e 206c 696e 6561 7220   sklearn linear 
-00010dc0: 7265 6772 6573 736f 7273 2077 6974 6820  regressors with 
-00010dd0: 4648 452e 0a0a 2020 2020 5468 6973 2063  FHE...    This c
-00010de0: 6c61 7373 2069 7320 7573 6564 2074 6f20  lass is used to 
-00010df0: 6372 6561 7465 2061 206c 696e 6561 7220  create a linear 
-00010e00: 7265 6772 6573 736f 7220 636c 6173 7320  regressor class 
-00010e10: 7468 6174 2069 6e68 6572 6974 7320 6672  that inherits fr
-00010e20: 6f6d 0a20 2020 2073 6b6c 6561 726e 2e62  om.    sklearn.b
-00010e30: 6173 652e 5265 6772 6573 736f 724d 6978  ase.RegressorMix
-00010e40: 696e 2c20 7768 6963 6820 6573 7365 6e74  in, which essent
-00010e50: 6961 6c6c 7920 6769 7665 7320 6163 6365  ially gives acce
-00010e60: 7373 2074 6f20 7363 696b 6974 2d6c 6561  ss to scikit-lea
-00010e70: 726e 2773 2060 7363 6f72 6560 206d 6574  rn's `score` met
-00010e80: 686f 640a 2020 2020 666f 7220 7265 6772  hod.    for regr
-00010e90: 6573 736f 7273 2e0a 2020 2020 2222 220a  essors..    """.
-00010ea0: 0a0a 636c 6173 7320 536b 6c65 6172 6e53  ..class SklearnS
-00010eb0: 4744 5265 6772 6573 736f 724d 6978 696e  GDRegressorMixin
-00010ec0: 2853 6b6c 6561 726e 4c69 6e65 6172 5265  (SklearnLinearRe
-00010ed0: 6772 6573 736f 724d 6978 696e 293a 0a20  gressorMixin):. 
-00010ee0: 2020 2022 2222 4120 4d69 7869 6e20 636c     """A Mixin cl
-00010ef0: 6173 7320 666f 7220 736b 6c65 6172 6e20  ass for sklearn 
-00010f00: 5347 4420 7265 6772 6573 736f 7273 2077  SGD regressors w
-00010f10: 6974 6820 4648 452e 0a0a 2020 2020 5468  ith FHE...    Th
-00010f20: 6973 2063 6c61 7373 2069 7320 7573 6564  is class is used
-00010f30: 2074 6f20 6372 6561 7465 2061 2053 4744   to create a SGD
-00010f40: 2072 6567 7265 7373 6f72 2063 6c61 7373   regressor class
-00010f50: 2077 6861 7420 6361 6e20 6265 2065 7870   what can be exp
-00010f60: 6f72 7465 640a 2020 2020 746f 204f 4e4e  orted.    to ONN
-00010f70: 5820 7573 696e 6720 4875 6d6d 696e 6762  X using Hummingb
-00010f80: 6972 642e 0a20 2020 2022 2222 0a0a 2020  ird..    """..  
-00010f90: 2020 2320 5265 6d6f 7665 206f 6e63 6520    # Remove once 
-00010fa0: 4875 6d6d 696e 6762 6972 6420 7375 7070  Hummingbird supp
-00010fb0: 6f72 7473 2053 4744 5265 6772 6573 736f  orts SGDRegresso
-00010fc0: 720a 2020 2020 2320 4649 584d 453a 2068  r.    # FIXME: h
-00010fd0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00010fe0: 6d2f 7a61 6d61 2d61 692f 636f 6e63 7265  m/zama-ai/concre
-00010ff0: 7465 2d6d 6c2d 696e 7465 726e 616c 2f69  te-ml-internal/i
-00011000: 7373 7565 732f 3431 3030 0a20 2020 2064  ssues/4100.    d
-00011010: 6566 205f 7365 745f 6f6e 6e78 5f6d 6f64  ef _set_onnx_mod
-00011020: 656c 2873 656c 662c 2074 6573 745f 696e  el(self, test_in
-00011030: 7075 743a 206e 756d 7079 2e6e 6461 7272  put: numpy.ndarr
-00011040: 6179 2920 2d3e 204e 6f6e 653a 0a20 2020  ay) -> None:.   
-00011050: 2020 2020 2022 2222 5265 7472 6965 7665       """Retrieve
-00011060: 2074 6865 206d 6f64 656c 2773 204f 4e4e   the model's ONN
-00011070: 5820 6772 6170 6820 7573 696e 6720 4875  X graph using Hu
-00011080: 6d6d 696e 6762 6972 6420 636f 6e76 6572  mmingbird conver
-00011090: 7369 6f6e 2e0a 0a20 2020 2020 2020 2041  sion...        A
-000110a0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-000110b0: 2074 6573 745f 696e 7075 7420 286e 756d   test_input (num
-000110c0: 7079 2e6e 6461 7272 6179 293a 2041 6e20  py.ndarray): An 
-000110d0: 696e 7075 7420 6461 7461 2075 7365 6420  input data used 
-000110e0: 746f 2074 7261 6365 2074 6865 206d 6f64  to trace the mod
-000110f0: 656c 2065 7865 6375 7469 6f6e 2e0a 2020  el execution..  
-00011100: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00011110: 2020 2320 4368 6563 6b20 7468 6174 2074    # Check that t
-00011120: 6865 2075 6e64 6572 6c79 696e 6720 736b  he underlying sk
-00011130: 6c65 6172 6e20 6d6f 6465 6c20 6861 7320  learn model has 
-00011140: 6265 656e 2073 6574 2061 6e64 2066 6974  been set and fit
-00011150: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00011160: 7365 6c66 2e73 6b6c 6561 726e 5f6d 6f64  self.sklearn_mod
-00011170: 656c 2069 7320 6e6f 7420 4e6f 6e65 2c20  el is not None, 
-00011180: 7365 6c66 2e5f 736b 6c65 6172 6e5f 6d6f  self._sklearn_mo
-00011190: 6465 6c5f 6973 5f6e 6f74 5f66 6974 7465  del_is_not_fitte
-000111a0: 645f 6572 726f 725f 6d65 7373 6167 6528  d_error_message(
-000111b0: 290a 0a20 2020 2020 2020 206d 6f64 656c  )..        model
-000111c0: 5f66 6f72 5f6f 6e6e 7820 3d20 4c69 6e65  _for_onnx = Line
-000111d0: 6172 5265 6772 6573 7369 6f6e 2829 0a20  arRegression(). 
-000111e0: 2020 2020 2020 206d 6f64 656c 5f66 6f72         model_for
-000111f0: 5f6f 6e6e 782e 636f 6566 5f20 3d20 7365  _onnx.coef_ = se
-00011200: 6c66 2e73 6b6c 6561 726e 5f6d 6f64 656c  lf.sklearn_model
-00011210: 2e63 6f65 665f 0a20 2020 2020 2020 206d  .coef_.        m
-00011220: 6f64 656c 5f66 6f72 5f6f 6e6e 782e 696e  odel_for_onnx.in
-00011230: 7465 7263 6570 745f 203d 2073 656c 662e  tercept_ = self.
-00011240: 736b 6c65 6172 6e5f 6d6f 6465 6c2e 696e  sklearn_model.in
-00011250: 7465 7263 6570 745f 0a0a 2020 2020 2020  tercept_..      
-00011260: 2020 7365 6c66 2e6f 6e6e 785f 6d6f 6465    self.onnx_mode
-00011270: 6c5f 203d 2068 625f 636f 6e76 6572 7428  l_ = hb_convert(
-00011280: 0a20 2020 2020 2020 2020 2020 206d 6f64  .            mod
-00011290: 656c 5f66 6f72 5f6f 6e6e 782c 0a20 2020  el_for_onnx,.   
-000112a0: 2020 2020 2020 2020 2062 6163 6b65 6e64           backend
-000112b0: 3d22 6f6e 6e78 222c 0a20 2020 2020 2020  ="onnx",.       
-000112c0: 2020 2020 2074 6573 745f 696e 7075 743d       test_input=
-000112d0: 7465 7374 5f69 6e70 7574 2c0a 2020 2020  test_input,.    
-000112e0: 2020 2020 2020 2020 6578 7472 615f 636f          extra_co
-000112f0: 6e66 6967 3d7b 226f 6e6e 785f 7461 7267  nfig={"onnx_targ
-00011300: 6574 5f6f 7073 6574 223a 204f 5053 4554  et_opset": OPSET
-00011310: 5f56 4552 5349 4f4e 5f46 4f52 5f4f 4e4e  _VERSION_FOR_ONN
-00011320: 585f 4558 504f 5254 7d2c 0a20 2020 2020  X_EXPORT},.     
-00011330: 2020 2029 2e6d 6f64 656c 0a0a 2020 2020     ).model..    
-00011340: 2020 2020 7365 6c66 2e5f 636c 6561 6e5f      self._clean_
-00011350: 6772 6170 6828 290a 0a0a 636c 6173 7320  graph()...class 
-00011360: 536b 6c65 6172 6e4c 696e 6561 7243 6c61  SklearnLinearCla
-00011370: 7373 6966 6965 724d 6978 696e 280a 2020  ssifierMixin(.  
-00011380: 2020 4261 7365 436c 6173 7369 6669 6572    BaseClassifier
-00011390: 2c20 536b 6c65 6172 6e4c 696e 6561 724d  , SklearnLinearM
-000113a0: 6f64 656c 4d69 7869 6e2c 2073 6b6c 6561  odelMixin, sklea
-000113b0: 726e 2e62 6173 652e 436c 6173 7369 6669  rn.base.Classifi
-000113c0: 6572 4d69 7869 6e2c 2041 4243 0a29 3a0a  erMixin, ABC.):.
-000113d0: 2020 2020 2222 2241 204d 6978 696e 2063      """A Mixin c
-000113e0: 6c61 7373 2066 6f72 2073 6b6c 6561 726e  lass for sklearn
-000113f0: 206c 696e 6561 7220 636c 6173 7369 6669   linear classifi
-00011400: 6572 7320 7769 7468 2046 4845 2e0a 0a20  ers with FHE... 
-00011410: 2020 2054 6869 7320 636c 6173 7320 6973     This class is
-00011420: 2075 7365 6420 746f 2063 7265 6174 6520   used to create 
-00011430: 6120 6c69 6e65 6172 2063 6c61 7373 6966  a linear classif
-00011440: 6965 7220 636c 6173 7320 7468 6174 2069  ier class that i
-00011450: 6e68 6572 6974 7320 6672 6f6d 0a20 2020  nherits from.   
-00011460: 2073 6b6c 6561 726e 2e62 6173 652e 436c   sklearn.base.Cl
-00011470: 6173 7369 6669 6572 4d69 7869 6e2c 2077  assifierMixin, w
-00011480: 6869 6368 2065 7373 656e 7469 616c 6c79  hich essentially
-00011490: 2067 6976 6573 2061 6363 6573 7320 746f   gives access to
-000114a0: 2073 6369 6b69 742d 6c65 6172 6e27 7320   scikit-learn's 
-000114b0: 6073 636f 7265 6020 6d65 7468 6f64 0a20  `score` method. 
-000114c0: 2020 2066 6f72 2063 6c61 7373 6966 6965     for classifie
-000114d0: 7273 2e0a 0a20 2020 2041 6464 6974 696f  rs...    Additio
-000114e0: 6e61 6c6c 792c 2074 6869 7320 636c 6173  nally, this clas
-000114f0: 7320 6164 6a75 7374 7320 736f 6d65 206f  s adjusts some o
-00011500: 6620 7468 6520 7472 6565 2d62 6173 6564  f the tree-based
-00011510: 2062 6173 6520 636c 6173 7327 7320 6d65   base class's me
-00011520: 7468 6f64 7320 696e 206f 7264 6572 2074  thods in order t
-00011530: 6f20 6d61 6b65 0a20 2020 2074 6865 6d20  o make.    them 
-00011540: 636f 6d70 6c69 616e 7420 7769 7468 2063  compliant with c
-00011550: 6c61 7373 6966 6963 6174 696f 6e20 776f  lassification wo
-00011560: 726b 666c 6f77 732e 0a20 2020 2022 2222  rkflows..    """
-00011570: 0a0a 2020 2020 6465 6620 5f63 6c65 616e  ..    def _clean
-00011580: 5f67 7261 7068 2873 656c 6629 202d 3e20  _graph(self) -> 
-00011590: 4e6f 6e65 3a0a 2020 2020 2020 2020 6173  None:.        as
-000115a0: 7365 7274 2073 656c 662e 6f6e 6e78 5f6d  sert self.onnx_m
-000115b0: 6f64 656c 5f20 6973 206e 6f74 204e 6f6e  odel_ is not Non
-000115c0: 652c 2073 656c 662e 5f69 735f 6e6f 745f  e, self._is_not_
-000115d0: 6669 7474 6564 5f65 7272 6f72 5f6d 6573  fitted_error_mes
-000115e0: 7361 6765 2829 0a0a 2020 2020 2020 2020  sage()..        
-000115f0: 2320 5265 6d6f 7665 2061 6e79 206f 7065  # Remove any ope
-00011600: 7261 746f 7273 2066 6f6c 6c6f 7769 6e67  rators following
-00011610: 2067 656d 6d2c 2061 7320 7468 6579 2077   gemm, as they w
-00011620: 696c 6c20 6265 2064 6f6e 6520 696e 2074  ill be done in t
-00011630: 6865 2063 6c65 6172 0a20 2020 2020 2020  he clear.       
-00011640: 2061 7373 6572 7420 7365 6c66 2e6f 6e6e   assert self.onn
-00011650: 785f 6d6f 6465 6c5f 2069 7320 6e6f 7420  x_model_ is not 
-00011660: 4e6f 6e65 0a20 2020 2020 2020 2063 6c65  None.        cle
-00011670: 616e 5f67 7261 7068 5f61 6674 6572 5f6e  an_graph_after_n
-00011680: 6f64 655f 6f70 5f74 7970 6528 7365 6c66  ode_op_type(self
-00011690: 2e6f 6e6e 785f 6d6f 6465 6c5f 2c20 6e6f  .onnx_model_, no
-000116a0: 6465 5f6f 705f 7479 7065 3d22 4765 6d6d  de_op_type="Gemm
-000116b0: 2229 0a20 2020 2020 2020 2053 6b6c 6561  ").        Sklea
-000116c0: 726e 4c69 6e65 6172 4d6f 6465 6c4d 6978  rnLinearModelMix
-000116d0: 696e 2e5f 636c 6561 6e5f 6772 6170 6828  in._clean_graph(
-000116e0: 7365 6c66 290a 0a20 2020 2064 6566 2064  self)..    def d
-000116f0: 6563 6973 696f 6e5f 6675 6e63 7469 6f6e  ecision_function
-00011700: 280a 2020 2020 2020 2020 7365 6c66 2c20  (.        self, 
-00011710: 583a 2044 6174 612c 2066 6865 3a20 556e  X: Data, fhe: Un
-00011720: 696f 6e5b 4668 654d 6f64 652c 2073 7472  ion[FheMode, str
-00011730: 5d20 3d20 4668 654d 6f64 652e 4449 5341  ] = FheMode.DISA
-00011740: 424c 450a 2020 2020 2920 2d3e 206e 756d  BLE.    ) -> num
-00011750: 7079 2e6e 6461 7272 6179 3a0a 2020 2020  py.ndarray:.    
-00011760: 2020 2020 2222 2250 7265 6469 6374 2063      """Predict c
-00011770: 6f6e 6669 6465 6e63 6520 7363 6f72 6573  onfidence scores
-00011780: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-00011790: 0a20 2020 2020 2020 2020 2020 2058 2028  .            X (
-000117a0: 4461 7461 293a 2054 6865 2069 6e70 7574  Data): The input
-000117b0: 2076 616c 7565 7320 746f 2070 7265 6469   values to predi
-000117c0: 6374 2c20 6173 2061 204e 756d 7079 2061  ct, as a Numpy a
-000117d0: 7272 6179 2c20 546f 7263 6820 7465 6e73  rray, Torch tens
-000117e0: 6f72 2c20 5061 6e64 6173 2044 6174 6146  or, Pandas DataF
-000117f0: 7261 6d65 0a20 2020 2020 2020 2020 2020  rame.           
-00011800: 2020 2020 206f 7220 4c69 7374 2e0a 2020       or List..  
-00011810: 2020 2020 2020 2020 2020 6668 6520 2855            fhe (U
-00011820: 6e69 6f6e 5b46 6865 4d6f 6465 2c20 7374  nion[FheMode, st
-00011830: 725d 293a 2054 6865 206d 6f64 6520 746f  r]): The mode to
-00011840: 2075 7365 2066 6f72 2070 7265 6469 6374   use for predict
-00011850: 696f 6e2e 0a20 2020 2020 2020 2020 2020  ion..           
-00011860: 2020 2020 2043 616e 2062 6520 4668 654d       Can be FheM
-00011870: 6f64 652e 4449 5341 424c 4520 666f 7220  ode.DISABLE for 
-00011880: 436f 6e63 7265 7465 204d 4c20 5079 7468  Concrete ML Pyth
-00011890: 6f6e 2069 6e66 6572 656e 6365 2c0a 2020  on inference,.  
-000118a0: 2020 2020 2020 2020 2020 2020 2020 4668                Fh
-000118b0: 654d 6f64 652e 5349 4d55 4c41 5445 2066  eMode.SIMULATE f
-000118c0: 6f72 2046 4845 2073 696d 756c 6174 696f  or FHE simulatio
-000118d0: 6e20 616e 6420 4668 654d 6f64 652e 4558  n and FheMode.EX
-000118e0: 4543 5554 4520 666f 7220 6163 7475 616c  ECUTE for actual
-000118f0: 2046 4845 2065 7865 6375 7469 6f6e 2e0a   FHE execution..
-00011900: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011910: 4361 6e20 616c 736f 2062 6520 7468 6520  Can also be the 
-00011920: 7374 7269 6e67 2072 6570 7265 7365 6e74  string represent
-00011930: 6174 696f 6e20 6f66 2061 6e79 206f 6620  ation of any of 
-00011940: 7468 6573 6520 7661 6c75 6573 2e0a 2020  these values..  
-00011950: 2020 2020 2020 2020 2020 2020 2020 4465                De
-00011960: 6661 756c 7420 746f 2046 6865 4d6f 6465  fault to FheMode
-00011970: 2e44 4953 4142 4c45 2e0a 0a20 2020 2020  .DISABLE...     
-00011980: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00011990: 2020 2020 2020 2020 6e75 6d70 792e 6e64          numpy.nd
-000119a0: 6172 7261 793a 2054 6865 2070 7265 6469  array: The predi
-000119b0: 6374 6564 2063 6f6e 6669 6465 6e63 6520  cted confidence 
-000119c0: 7363 6f72 6573 2e0a 2020 2020 2020 2020  scores..        
-000119d0: 2222 220a 2020 2020 2020 2020 2320 4865  """.        # He
-000119e0: 7265 2c20 7765 2077 616e 7420 746f 2075  re, we want to u
-000119f0: 7365 2053 6b6c 6561 726e 4c69 6e65 6172  se SklearnLinear
-00011a00: 4d6f 6465 6c4d 6978 696e 2773 2060 7072  ModelMixin's `pr
-00011a10: 6564 6963 7460 206d 6574 686f 6420 6173  edict` method as
-00011a20: 2063 6f6e 6669 6465 6e63 6520 7363 6f72   confidence scor
-00011a30: 6573 2061 7265 0a20 2020 2020 2020 2023  es are.        #
-00011a40: 2074 6865 2064 6f74 2070 726f 6475 6374   the dot product
-00011a50: 2773 206f 7574 7075 7420 7661 6c75 6573  's output values
-00011a60: 2c20 7769 7468 6f75 7420 616e 7920 706f  , without any po
-00011a70: 7374 2d70 726f 6365 7373 696e 670a 2020  st-processing.  
-00011a80: 2020 2020 2020 795f 7072 6564 7320 3d20        y_preds = 
-00011a90: 536b 6c65 6172 6e4c 696e 6561 724d 6f64  SklearnLinearMod
-00011aa0: 656c 4d69 7869 6e2e 7072 6564 6963 7428  elMixin.predict(
-00011ab0: 7365 6c66 2c20 582c 2066 6865 3d66 6865  self, X, fhe=fhe
-00011ac0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00011ad0: 2079 5f70 7265 6473 0a0a 2020 2020 6465   y_preds..    de
-00011ae0: 6620 7072 6564 6963 745f 7072 6f62 6128  f predict_proba(
-00011af0: 7365 6c66 2c20 583a 2044 6174 612c 2066  self, X: Data, f
-00011b00: 6865 3a20 556e 696f 6e5b 4668 654d 6f64  he: Union[FheMod
-00011b10: 652c 2073 7472 5d20 3d20 4668 654d 6f64  e, str] = FheMod
-00011b20: 652e 4449 5341 424c 4529 202d 3e20 6e75  e.DISABLE) -> nu
-00011b30: 6d70 792e 6e64 6172 7261 793a 0a20 2020  mpy.ndarray:.   
-00011b40: 2020 2020 2079 5f6c 6f67 6974 7320 3d20       y_logits = 
-00011b50: 7365 6c66 2e64 6563 6973 696f 6e5f 6675  self.decision_fu
-00011b60: 6e63 7469 6f6e 2858 2c20 6668 653d 6668  nction(X, fhe=fh
-00011b70: 6529 0a20 2020 2020 2020 2079 5f70 726f  e).        y_pro
-00011b80: 6261 203d 2073 656c 662e 706f 7374 5f70  ba = self.post_p
-00011b90: 726f 6365 7373 696e 6728 795f 6c6f 6769  rocessing(y_logi
-00011ba0: 7473 290a 2020 2020 2020 2020 7265 7475  ts).        retu
-00011bb0: 726e 2079 5f70 726f 6261 0a0a 0a63 6c61  rn y_proba...cla
-00011bc0: 7373 2053 6b6c 6561 726e 5347 4443 6c61  ss SklearnSGDCla
-00011bd0: 7373 6966 6965 724d 6978 696e 2853 6b6c  ssifierMixin(Skl
-00011be0: 6561 726e 4c69 6e65 6172 436c 6173 7369  earnLinearClassi
-00011bf0: 6669 6572 4d69 7869 6e29 3a0a 2020 2020  fierMixin):.    
-00011c00: 2222 2241 204d 6978 696e 2063 6c61 7373  """A Mixin class
-00011c10: 2066 6f72 2073 6b6c 6561 726e 2053 4744   for sklearn SGD
-00011c20: 2063 6c61 7373 6966 6965 7273 2077 6974   classifiers wit
-00011c30: 6820 4648 452e 0a0a 2020 2020 5468 6973  h FHE...    This
-00011c40: 2063 6c61 7373 2069 7320 7573 6564 2074   class is used t
-00011c50: 6f20 6372 6561 7465 2061 2053 4744 2063  o create a SGD c
-00011c60: 6c61 7373 6966 6965 7220 636c 6173 7320  lassifier class 
-00011c70: 7768 6174 2063 616e 2062 6520 6578 706f  what can be expo
-00011c80: 7274 6564 0a20 2020 2074 6f20 4f4e 4e58  rted.    to ONNX
-00011c90: 2075 7369 6e67 2048 756d 6d69 6e67 6269   using Hummingbi
-00011ca0: 7264 2e0a 2020 2020 2222 220a 0a20 2020  rd..    """..   
-00011cb0: 2023 2052 656d 6f76 6520 6f6e 6365 2048   # Remove once H
-00011cc0: 756d 6d69 6e67 6269 7264 2073 7570 706f  ummingbird suppo
-00011cd0: 7274 7320 5347 4452 6567 7265 7373 6f72  rts SGDRegressor
-00011ce0: 0a20 2020 2023 2046 4958 4d45 3a20 6874  .    # FIXME: ht
-00011cf0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00011d00: 2f7a 616d 612d 6169 2f63 6f6e 6372 6574  /zama-ai/concret
-00011d10: 652d 6d6c 2d69 6e74 6572 6e61 6c2f 6973  e-ml-internal/is
-00011d20: 7375 6573 2f34 3130 300a 2020 2020 6465  sues/4100.    de
-00011d30: 6620 5f73 6574 5f6f 6e6e 785f 6d6f 6465  f _set_onnx_mode
-00011d40: 6c28 7365 6c66 2c20 7465 7374 5f69 6e70  l(self, test_inp
-00011d50: 7574 3a20 6e75 6d70 792e 6e64 6172 7261  ut: numpy.ndarra
-00011d60: 7929 202d 3e20 4e6f 6e65 3a0a 2020 2020  y) -> None:.    
-00011d70: 2020 2020 2222 2252 6574 7269 6576 6520      """Retrieve 
-00011d80: 7468 6520 6d6f 6465 6c27 7320 4f4e 4e58  the model's ONNX
-00011d90: 2067 7261 7068 2075 7369 6e67 2048 756d   graph using Hum
-00011da0: 6d69 6e67 6269 7264 2063 6f6e 7665 7273  mingbird convers
-00011db0: 696f 6e2e 0a0a 2020 2020 2020 2020 4172  ion...        Ar
-00011dc0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00011dd0: 7465 7374 5f69 6e70 7574 2028 6e75 6d70  test_input (nump
-00011de0: 792e 6e64 6172 7261 7929 3a20 416e 2069  y.ndarray): An i
-00011df0: 6e70 7574 2064 6174 6120 7573 6564 2074  nput data used t
-00011e00: 6f20 7472 6163 6520 7468 6520 6d6f 6465  o trace the mode
-00011e10: 6c20 6578 6563 7574 696f 6e2e 0a20 2020  l execution..   
-00011e20: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00011e30: 2023 2043 6865 636b 2074 6861 7420 7468   # Check that th
-00011e40: 6520 756e 6465 726c 7969 6e67 2073 6b6c  e underlying skl
-00011e50: 6561 726e 206d 6f64 656c 2068 6173 2062  earn model has b
-00011e60: 6565 6e20 7365 7420 616e 6420 6669 740a  een set and fit.
-00011e70: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
-00011e80: 656c 662e 736b 6c65 6172 6e5f 6d6f 6465  elf.sklearn_mode
-00011e90: 6c20 6973 206e 6f74 204e 6f6e 652c 2073  l is not None, s
-00011ea0: 656c 662e 5f73 6b6c 6561 726e 5f6d 6f64  elf._sklearn_mod
-00011eb0: 656c 5f69 735f 6e6f 745f 6669 7474 6564  el_is_not_fitted
-00011ec0: 5f65 7272 6f72 5f6d 6573 7361 6765 2829  _error_message()
-00011ed0: 0a0a 2020 2020 2020 2020 6d6f 6465 6c5f  ..        model_
-00011ee0: 666f 725f 6f6e 6e78 203d 204c 6f67 6973  for_onnx = Logis
-00011ef0: 7469 6352 6567 7265 7373 696f 6e28 290a  ticRegression().
-00011f00: 2020 2020 2020 2020 6d6f 6465 6c5f 666f          model_fo
-00011f10: 725f 6f6e 6e78 2e63 6f65 665f 203d 2073  r_onnx.coef_ = s
-00011f20: 656c 662e 736b 6c65 6172 6e5f 6d6f 6465  elf.sklearn_mode
-00011f30: 6c2e 636f 6566 5f0a 2020 2020 2020 2020  l.coef_.        
-00011f40: 6d6f 6465 6c5f 666f 725f 6f6e 6e78 2e69  model_for_onnx.i
-00011f50: 6e74 6572 6365 7074 5f20 3d20 7365 6c66  ntercept_ = self
-00011f60: 2e73 6b6c 6561 726e 5f6d 6f64 656c 2e69  .sklearn_model.i
-00011f70: 6e74 6572 6365 7074 5f0a 0a20 2020 2020  ntercept_..     
-00011f80: 2020 2073 656c 662e 6f6e 6e78 5f6d 6f64     self.onnx_mod
-00011f90: 656c 5f20 3d20 6862 5f63 6f6e 7665 7274  el_ = hb_convert
-00011fa0: 280a 2020 2020 2020 2020 2020 2020 6d6f  (.            mo
-00011fb0: 6465 6c5f 666f 725f 6f6e 6e78 2c0a 2020  del_for_onnx,.  
-00011fc0: 2020 2020 2020 2020 2020 6261 636b 656e            backen
-00011fd0: 643d 226f 6e6e 7822 2c0a 2020 2020 2020  d="onnx",.      
-00011fe0: 2020 2020 2020 7465 7374 5f69 6e70 7574        test_input
-00011ff0: 3d74 6573 745f 696e 7075 742c 0a20 2020  =test_input,.   
-00012000: 2020 2020 2020 2020 2065 7874 7261 5f63           extra_c
-00012010: 6f6e 6669 673d 7b22 6f6e 6e78 5f74 6172  onfig={"onnx_tar
-00012020: 6765 745f 6f70 7365 7422 3a20 4f50 5345  get_opset": OPSE
-00012030: 545f 5645 5253 494f 4e5f 464f 525f 4f4e  T_VERSION_FOR_ON
-00012040: 4e58 5f45 5850 4f52 547d 2c0a 2020 2020  NX_EXPORT},.    
-00012050: 2020 2020 292e 6d6f 6465 6c0a 0a20 2020      ).model..   
-00012060: 2020 2020 2073 656c 662e 5f63 6c65 616e       self._clean
-00012070: 5f67 7261 7068 2829 0a0a 0a23 2070 796c  _graph()...# pyl
-00012080: 696e 743a 2064 6973 6162 6c65 2d6e 6578  int: disable-nex
-00012090: 743d 696e 7661 6c69 642d 6e61 6d65 2c74  t=invalid-name,t
-000120a0: 6f6f 2d6d 616e 792d 696e 7374 616e 6365  oo-many-instance
-000120b0: 2d61 7474 7269 6275 7465 730a 636c 6173  -attributes.clas
-000120c0: 7320 536b 6c65 6172 6e4b 4e65 6967 6862  s SklearnKNeighb
-000120d0: 6f72 734d 6978 696e 2842 6173 6545 7374  orsMixin(BaseEst
-000120e0: 696d 6174 6f72 2c20 736b 6c65 6172 6e2e  imator, sklearn.
-000120f0: 6261 7365 2e42 6173 6545 7374 696d 6174  base.BaseEstimat
-00012100: 6f72 2c20 4142 4329 3a0a 2020 2020 2222  or, ABC):.    ""
-00012110: 2241 204d 6978 696e 2063 6c61 7373 2066  "A Mixin class f
-00012120: 6f72 2073 6b6c 6561 726e 204b 4e65 6967  or sklearn KNeig
-00012130: 6862 6f72 7320 6d6f 6465 6c73 2077 6974  hbors models wit
-00012140: 6820 4648 452e 0a0a 2020 2020 5468 6973  h FHE...    This
-00012150: 2063 6c61 7373 2069 6e68 6572 6974 7320   class inherits 
-00012160: 6672 6f6d 2073 6b6c 6561 726e 2e62 6173  from sklearn.bas
-00012170: 652e 4261 7365 4573 7469 6d61 746f 7220  e.BaseEstimator 
-00012180: 696e 206f 7264 6572 2074 6f20 6861 7665  in order to have
-00012190: 2061 6363 6573 7320 746f 2073 6369 6b69   access to sciki
-000121a0: 742d 6c65 6172 6e27 730a 2020 2020 6067  t-learn's.    `g
-000121b0: 6574 5f70 6172 616d 7360 2061 6e64 2060  et_params` and `
-000121c0: 7365 745f 7061 7261 6d73 6020 6d65 7468  set_params` meth
-000121d0: 6f64 732e 0a20 2020 2022 2222 0a0a 2020  ods..    """..  
-000121e0: 2020 6465 6620 5f5f 696e 6974 5f73 7562    def __init_sub
-000121f0: 636c 6173 735f 5f28 636c 7329 3a0a 2020  class__(cls):.  
-00012200: 2020 2020 2020 666f 7220 6b6c 6173 7320        for klass 
-00012210: 696e 2063 6c73 2e5f 5f6d 726f 5f5f 3a0a  in cls.__mro__:.
-00012220: 2020 2020 2020 2020 2020 2020 2320 7079              # py
-00012230: 6c69 6e74 3a20 6469 7361 626c 652d 6e65  lint: disable-ne
-00012240: 7874 3d70 726f 7465 6374 6564 2d61 6363  xt=protected-acc
-00012250: 6573 730a 2020 2020 2020 2020 2020 2020  ess.            
-00012260: 6966 2067 6574 6174 7472 286b 6c61 7373  if getattr(klass
-00012270: 2c20 225f 6973 5f61 5f70 7562 6c69 635f  , "_is_a_public_
-00012280: 636d 6c5f 6d6f 6465 6c22 2c20 4661 6c73  cml_model", Fals
-00012290: 6529 3a0a 2020 2020 2020 2020 2020 2020  e):.            
-000122a0: 2020 2020 5f4e 4549 4748 424f 5253 5f4d      _NEIGHBORS_M
-000122b0: 4f44 454c 532e 6164 6428 636c 7329 0a20  ODELS.add(cls). 
-000122c0: 2020 2020 2020 2020 2020 2020 2020 205f                 _
-000122d0: 414c 4c5f 534b 4c45 4152 4e5f 4d4f 4445  ALL_SKLEARN_MODE
-000122e0: 4c53 2e61 6464 2863 6c73 290a 0a20 2020  LS.add(cls)..   
-000122f0: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00012300: 6c66 2c20 6e5f 6269 7473 3a20 696e 7420  lf, n_bits: int 
-00012310: 3d20 3329 3a0a 2020 2020 2020 2020 2222  = 3):.        ""
-00012320: 2249 6e69 7469 616c 697a 6520 7468 6520  "Initialize the 
-00012330: 4648 4520 6b6e 6e20 6d6f 6465 6c2e 0a0a  FHE knn model...
-00012340: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00012350: 2020 2020 2020 2020 2020 6e5f 6269 7473            n_bits
-00012360: 2028 696e 7429 3a20 4e75 6d62 6572 206f   (int): Number o
-00012370: 6620 6269 7473 2074 6f20 7175 616e 7469  f bits to quanti
-00012380: 7a65 2074 6865 206d 6f64 656c 2e20 5468  ze the model. Th
-00012390: 6520 7661 6c75 6520 7769 6c6c 2062 6520  e value will be 
-000123a0: 7573 6564 2066 6f72 0a20 2020 2020 2020  used for.       
-000123b0: 2020 2020 2020 2020 2071 7561 6e74 697a           quantiz
-000123c0: 696e 6720 696e 7075 7473 2061 6e64 2058  ing inputs and X
-000123d0: 5f66 6974 2e20 4465 6661 756c 7420 746f  _fit. Default to
-000123e0: 2033 2e0a 2020 2020 2020 2020 2222 220a   3..        """.
-000123f0: 2020 2020 2020 2020 7365 6c66 2e6e 5f62          self.n_b
-00012400: 6974 733a 2069 6e74 203d 206e 5f62 6974  its: int = n_bit
-00012410: 730a 0a20 2020 2020 2020 2023 205f 715f  s..        # _q_
-00012420: 6669 745f 583a 2049 6e20 6469 7374 616e  fit_X: In distan
-00012430: 6365 206d 6574 7269 6320 616c 676f 7269  ce metric algori
-00012440: 7468 6d73 2c20 605f 715f 6669 745f 5860  thms, `_q_fit_X`
-00012450: 2073 746f 7265 7320 7468 6520 7472 6169   stores the trai
-00012460: 6e69 6e67 2073 6574 2074 6f20 636f 6d70  ning set to comp
-00012470: 7574 650a 2020 2020 2020 2020 2320 7468  ute.        # th
-00012480: 6520 7369 6d69 6c61 7269 7479 206f 7220  e similarity or 
-00012490: 6469 7374 616e 6365 206d 6561 7375 7265  distance measure
-000124a0: 732e 2054 6865 7265 2069 7320 6e6f 2060  s. There is no `
-000124b0: 7765 6967 6874 7360 2061 7474 7269 6275  weights` attribu
-000124c0: 7465 2062 6563 6175 7365 2074 6865 7265  te because there
-000124d0: 2069 736e 2774 0a20 2020 2020 2020 2023   isn't.        #
-000124e0: 2061 2074 7261 696e 696e 6720 7068 6173   a training phas
-000124f0: 650a 2020 2020 2020 2020 7365 6c66 2e5f  e.        self._
-00012500: 715f 6669 745f 583a 206e 756d 7079 2e6e  q_fit_X: numpy.n
-00012510: 6461 7272 6179 0a0a 2020 2020 2020 2020  darray..        
-00012520: 2320 5f79 3a20 4c61 6265 6c73 206f 6620  # _y: Labels of 
-00012530: 605f 715f 6669 745f 5860 0a20 2020 2020  `_q_fit_X`.     
-00012540: 2020 2073 656c 662e 5f79 3a20 6e75 6d70     self._y: nump
-00012550: 792e 6e64 6172 7261 790a 0a20 2020 2020  y.ndarray..     
-00012560: 2020 2023 205f 715f 6669 745f 585f 7175     # _q_fit_X_qu
-00012570: 616e 7469 7a65 723a 2054 6865 2071 7561  antizer: The qua
-00012580: 6e74 697a 6572 2074 6f20 7573 6520 666f  ntizer to use fo
-00012590: 7220 7175 616e 7469 7a69 6e67 2074 6865  r quantizing the
-000125a0: 206d 6f64 656c 2773 2074 7261 696e 696e   model's trainin
-000125b0: 6720 7365 740a 2020 2020 2020 2020 7365  g set.        se
-000125c0: 6c66 2e5f 715f 6669 745f 585f 7175 616e  lf._q_fit_X_quan
-000125d0: 7469 7a65 723a 204f 7074 696f 6e61 6c5b  tizer: Optional[
-000125e0: 556e 6966 6f72 6d51 7561 6e74 697a 6572  UniformQuantizer
-000125f0: 5d20 3d20 4e6f 6e65 0a0a 2020 2020 2020  ] = None..      
-00012600: 2020 4261 7365 4573 7469 6d61 746f 722e    BaseEstimator.
-00012610: 5f5f 696e 6974 5f5f 2873 656c 6629 0a0a  __init__(self)..
-00012620: 2020 2020 6465 6620 5f73 6574 5f6f 6e6e      def _set_onn
-00012630: 785f 6d6f 6465 6c28 7365 6c66 2c20 7465  x_model(self, te
-00012640: 7374 5f69 6e70 7574 3a20 6e75 6d70 792e  st_input: numpy.
-00012650: 6e64 6172 7261 7929 202d 3e20 4e6f 6e65  ndarray) -> None
-00012660: 3a0a 2020 2020 2020 2020 2222 2252 6574  :.        """Ret
-00012670: 7269 6576 6520 7468 6520 6d6f 6465 6c27  rieve the model'
-00012680: 7320 4f4e 4e58 2067 7261 7068 2075 7369  s ONNX graph usi
-00012690: 6e67 2048 756d 6d69 6e67 6269 7264 2063  ng Hummingbird c
-000126a0: 6f6e 7665 7273 696f 6e2e 0a0a 2020 2020  onversion...    
-000126b0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-000126c0: 2020 2020 2020 7465 7374 5f69 6e70 7574        test_input
-000126d0: 2028 6e75 6d70 792e 6e64 6172 7261 7929   (numpy.ndarray)
-000126e0: 3a20 416e 2069 6e70 7574 2064 6174 6120  : An input data 
-000126f0: 7573 6564 2074 6f20 7472 6163 6520 7468  used to trace th
-00012700: 6520 6d6f 6465 6c20 6578 6563 7574 696f  e model executio
-00012710: 6e2e 0a20 2020 2020 2020 2022 2222 0a20  n..        """. 
-00012720: 2020 2020 2020 2023 2043 6865 636b 2074         # Check t
-00012730: 6861 7420 7468 6520 756e 6465 726c 7969  hat the underlyi
-00012740: 6e67 2073 6b6c 6561 726e 206d 6f64 656c  ng sklearn model
-00012750: 2068 6173 2062 6565 6e20 7365 7420 616e   has been set an
-00012760: 6420 6669 740a 2020 2020 2020 2020 6173  d fit.        as
-00012770: 7365 7274 2073 656c 662e 736b 6c65 6172  sert self.sklear
-00012780: 6e5f 6d6f 6465 6c20 6973 206e 6f74 204e  n_model is not N
-00012790: 6f6e 652c 2073 656c 662e 5f73 6b6c 6561  one, self._sklea
-000127a0: 726e 5f6d 6f64 656c 5f69 735f 6e6f 745f  rn_model_is_not_
-000127b0: 6669 7474 6564 5f65 7272 6f72 5f6d 6573  fitted_error_mes
-000127c0: 7361 6765 2829 0a0a 2020 2020 2020 2020  sage()..        
-000127d0: 7365 6c66 2e6f 6e6e 785f 6d6f 6465 6c5f  self.onnx_model_
-000127e0: 203d 2068 625f 636f 6e76 6572 7428 0a20   = hb_convert(. 
-000127f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00012800: 736b 6c65 6172 6e5f 6d6f 6465 6c2c 0a20  sklearn_model,. 
-00012810: 2020 2020 2020 2020 2020 2062 6163 6b65             backe
-00012820: 6e64 3d22 6f6e 6e78 222c 0a20 2020 2020  nd="onnx",.     
-00012830: 2020 2020 2020 2074 6573 745f 696e 7075         test_inpu
-00012840: 743d 7465 7374 5f69 6e70 7574 2c0a 2020  t=test_input,.  
-00012850: 2020 2020 2020 2020 2020 6578 7472 615f            extra_
-00012860: 636f 6e66 6967 3d7b 0a20 2020 2020 2020  config={.       
-00012870: 2020 2020 2020 2020 2022 6f6e 6e78 5f74           "onnx_t
-00012880: 6172 6765 745f 6f70 7365 7422 3a20 4f50  arget_opset": OP
-00012890: 5345 545f 5645 5253 494f 4e5f 464f 525f  SET_VERSION_FOR_
-000128a0: 4f4e 4e58 5f45 5850 4f52 542c 0a20 2020  ONNX_EXPORT,.   
-000128b0: 2020 2020 2020 2020 2020 2020 2023 2070               # p
-000128c0: 796c 696e 743a 2064 6973 6162 6c65 2d6e  ylint: disable-n
-000128d0: 6578 743d 7072 6f74 6563 7465 642d 6163  ext=protected-ac
-000128e0: 6365 7373 2c20 6e6f 2d6d 656d 6265 720a  cess, no-member.
-000128f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012900: 636f 6e73 7461 6e74 732e 4241 5443 485f  constants.BATCH_
-00012910: 5349 5a45 3a20 7365 6c66 2e73 6b6c 6561  SIZE: self.sklea
-00012920: 726e 5f6d 6f64 656c 2e5f 6669 745f 582e  rn_model._fit_X.
-00012930: 7368 6170 655b 305d 2c0a 2020 2020 2020  shape[0],.      
-00012940: 2020 2020 2020 7d2c 0a20 2020 2020 2020        },.       
-00012950: 2029 2e6d 6f64 656c 0a0a 2020 2020 2020   ).model..      
-00012960: 2020 7365 6c66 2e5f 636c 6561 6e5f 6772    self._clean_gr
-00012970: 6170 6828 290a 0a20 2020 2064 6566 205f  aph()..    def _
-00012980: 636c 6561 6e5f 6772 6170 6828 7365 6c66  clean_graph(self
-00012990: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
-000129a0: 2020 2022 2222 436c 6561 6e20 7468 6520     """Clean the 
-000129b0: 4f4e 4e58 2067 7261 7068 2066 726f 6d20  ONNX graph from 
-000129c0: 756e 6465 7369 7265 6420 6e6f 6465 732e  undesired nodes.
-000129d0: 2222 220a 2020 2020 2020 2020 6173 7365  """.        asse
-000129e0: 7274 2073 656c 662e 6f6e 6e78 5f6d 6f64  rt self.onnx_mod
-000129f0: 656c 5f20 6973 206e 6f74 204e 6f6e 652c  el_ is not None,
-00012a00: 2073 656c 662e 5f69 735f 6e6f 745f 6669   self._is_not_fi
-00012a10: 7474 6564 5f65 7272 6f72 5f6d 6573 7361  tted_error_messa
-00012a20: 6765 2829 0a0a 2020 2020 2020 2020 2320  ge()..        # 
-00012a30: 5265 6d6f 7665 2063 6173 7420 6f70 6572  Remove cast oper
-00012a40: 6174 6f72 7320 6173 2074 6865 7920 6172  ators as they ar
-00012a50: 6520 6e6f 7420 6e65 6564 6564 0a20 2020  e not needed.   
-00012a60: 2020 2020 2072 656d 6f76 655f 6e6f 6465       remove_node
-00012a70: 5f74 7970 6573 286f 6e6e 785f 6d6f 6465  _types(onnx_mode
-00012a80: 6c3d 7365 6c66 2e6f 6e6e 785f 6d6f 6465  l=self.onnx_mode
-00012a90: 6c5f 2c20 6f70 5f74 7970 6573 5f74 6f5f  l_, op_types_to_
-00012aa0: 7265 6d6f 7665 3d5b 2243 6173 7422 5d29  remove=["Cast"])
-00012ab0: 0a0a 2020 2020 6465 6620 6669 7428 7365  ..    def fit(se
-00012ac0: 6c66 2c20 583a 2044 6174 612c 2079 3a20  lf, X: Data, y: 
-00012ad0: 5461 7267 6574 2c20 2a2a 6669 745f 7061  Target, **fit_pa
-00012ae0: 7261 6d65 7465 7273 293a 0a20 2020 2020  rameters):.     
-00012af0: 2020 2023 2052 6573 6574 2066 6f72 2064     # Reset for d
-00012b00: 6f75 626c 6520 6669 740a 2020 2020 2020  ouble fit.      
-00012b10: 2020 7365 6c66 2e5f 6973 5f66 6974 7465    self._is_fitte
-00012b20: 6420 3d20 4661 6c73 650a 2020 2020 2020  d = False.      
-00012b30: 2020 7365 6c66 2e69 6e70 7574 5f71 7561    self.input_qua
-00012b40: 6e74 697a 6572 7320 3d20 5b5d 0a20 2020  ntizers = [].   
-00012b50: 2020 2020 2073 656c 662e 6f75 7470 7574       self.output
-00012b60: 5f71 7561 6e74 697a 6572 7320 3d20 5b5d  _quantizers = []
-00012b70: 0a0a 2020 2020 2020 2020 2320 4b4e 6569  ..        # KNei
-00012b80: 6768 626f 7273 2068 616e 646c 6573 206d  ghbors handles m
-00012b90: 756c 7469 2d6c 6162 656c 7320 6461 7461  ulti-labels data
-00012ba0: 0a20 2020 2020 2020 2058 2c20 7920 3d20  .        X, y = 
-00012bb0: 6368 6563 6b5f 585f 795f 616e 645f 6173  check_X_y_and_as
-00012bc0: 7365 7274 5f6d 756c 7469 5f6f 7574 7075  sert_multi_outpu
-00012bd0: 7428 582c 2079 290a 0a20 2020 2020 2020  t(X, y)..       
-00012be0: 2023 2046 6974 2074 6865 2073 6369 6b69   # Fit the sciki
-00012bf0: 742d 6c65 6172 6e20 6d6f 6465 6c0a 2020  t-learn model.  
-00012c00: 2020 2020 2020 7365 6c66 2e5f 6669 745f        self._fit_
-00012c10: 736b 6c65 6172 6e5f 6d6f 6465 6c28 582c  sklearn_model(X,
-00012c20: 2079 2c20 2a2a 6669 745f 7061 7261 6d65   y, **fit_parame
-00012c30: 7465 7273 290a 0a20 2020 2020 2020 2023  ters)..        #
-00012c40: 2043 6865 636b 2074 6861 7420 7468 6520   Check that the 
-00012c50: 756e 6465 726c 7969 6e67 2073 6b6c 6561  underlying sklea
-00012c60: 726e 206d 6f64 656c 2068 6173 2062 6565  rn model has bee
-00012c70: 6e20 7365 7420 616e 6420 6669 740a 2020  n set and fit.  
-00012c80: 2020 2020 2020 6173 7365 7274 2073 656c        assert sel
-00012c90: 662e 736b 6c65 6172 6e5f 6d6f 6465 6c20  f.sklearn_model 
-00012ca0: 6973 206e 6f74 204e 6f6e 652c 2073 656c  is not None, sel
-00012cb0: 662e 5f73 6b6c 6561 726e 5f6d 6f64 656c  f._sklearn_model
-00012cc0: 5f69 735f 6e6f 745f 6669 7474 6564 5f65  _is_not_fitted_e
-00012cd0: 7272 6f72 5f6d 6573 7361 6765 2829 0a0a  rror_message()..
-00012ce0: 2020 2020 2020 2020 2320 5265 7472 6965          # Retrie
-00012cf0: 7665 2074 6865 204f 4e4e 5820 6772 6170  ve the ONNX grap
-00012d00: 680a 2020 2020 2020 2020 7365 6c66 2e5f  h.        self._
-00012d10: 7365 745f 6f6e 6e78 5f6d 6f64 656c 2858  set_onnx_model(X
-00012d20: 290a 0a20 2020 2020 2020 2023 2051 7561  )..        # Qua
-00012d30: 6e74 697a 6520 7468 6520 696e 7075 7473  ntize the inputs
-00012d40: 2061 6e64 2073 746f 7265 2074 6865 2061   and store the a
-00012d50: 7373 6f63 6961 7465 6420 7175 616e 7469  ssociated quanti
-00012d60: 7a65 720a 2020 2020 2020 2020 696e 7075  zer.        inpu
-00012d70: 745f 6f70 7469 6f6e 7320 3d20 5175 616e  t_options = Quan
-00012d80: 7469 7a61 7469 6f6e 4f70 7469 6f6e 7328  tizationOptions(
-00012d90: 6e5f 6269 7473 3d73 656c 662e 6e5f 6269  n_bits=self.n_bi
-00012da0: 7473 2c20 6973 5f73 6967 6e65 643d 5472  ts, is_signed=Tr
-00012db0: 7565 290a 2020 2020 2020 2020 715f 696e  ue).        q_in
-00012dc0: 7075 7473 203d 2051 7561 6e74 697a 6564  puts = Quantized
-00012dd0: 4172 7261 7928 6e5f 6269 7473 3d73 656c  Array(n_bits=sel
-00012de0: 662e 6e5f 6269 7473 2c20 7661 6c75 6573  f.n_bits, values
-00012df0: 3d58 2c20 6f70 7469 6f6e 733d 696e 7075  =X, options=inpu
-00012e00: 745f 6f70 7469 6f6e 7329 0a20 2020 2020  t_options).     
-00012e10: 2020 2069 6e70 7574 5f71 7561 6e74 697a     input_quantiz
-00012e20: 6572 203d 2071 5f69 6e70 7574 732e 7175  er = q_inputs.qu
-00012e30: 616e 7469 7a65 720a 2020 2020 2020 2020  antizer.        
-00012e40: 7365 6c66 2e69 6e70 7574 5f71 7561 6e74  self.input_quant
-00012e50: 697a 6572 732e 6170 7065 6e64 2869 6e70  izers.append(inp
-00012e60: 7574 5f71 7561 6e74 697a 6572 290a 0a20  ut_quantizer).. 
-00012e70: 2020 2020 2020 2023 2051 7561 6e74 697a         # Quantiz
-00012e80: 6520 7468 6520 5f66 6974 5f58 2061 6e64  e the _fit_X and
-00012e90: 2073 746f 7265 2074 6865 2061 7373 6f63   store the assoc
-00012ea0: 6961 7465 6420 7175 616e 7469 7a65 720a  iated quantizer.
-00012eb0: 2020 2020 2020 2020 2320 7079 6c69 6e74          # pylint
-00012ec0: 3a20 6469 7361 626c 652d 6e65 7874 3d70  : disable-next=p
-00012ed0: 726f 7465 6374 6564 2d61 6363 6573 730a  rotected-access.
-00012ee0: 2020 2020 2020 2020 5f66 6974 5f58 203d          _fit_X =
-00012ef0: 2073 656c 662e 736b 6c65 6172 6e5f 6d6f   self.sklearn_mo
-00012f00: 6465 6c2e 5f66 6974 5f58 0a20 2020 2020  del._fit_X.     
-00012f10: 2020 2023 2057 6520 6173 7375 6d65 2074     # We assume t
-00012f20: 6861 7420 7468 6520 696e 7075 7473 2068  hat the inputs h
-00012f30: 6176 6520 7468 6520 7361 6d65 2064 6973  ave the same dis
-00012f40: 7472 6962 7574 696f 6e20 6173 2074 6865  tribution as the
-00012f50: 205f 6669 745f 580a 2020 2020 2020 2020   _fit_X.        
-00012f60: 715f 6669 745f 5820 3d20 5175 616e 7469  q_fit_X = Quanti
-00012f70: 7a65 6441 7272 6179 280a 2020 2020 2020  zedArray(.      
-00012f80: 2020 2020 2020 6e5f 6269 7473 3d73 656c        n_bits=sel
-00012f90: 662e 6e5f 6269 7473 2c0a 2020 2020 2020  f.n_bits,.      
-00012fa0: 2020 2020 2020 7661 6c75 6573 3d6e 756d        values=num
-00012fb0: 7079 2e65 7870 616e 645f 6469 6d73 285f  py.expand_dims(_
-00012fc0: 6669 745f 582c 2061 7869 733d 3129 2069  fit_X, axis=1) i
-00012fd0: 6620 6c65 6e28 5f66 6974 5f58 2e73 6861  f len(_fit_X.sha
-00012fe0: 7065 2920 3d3d 2031 2065 6c73 6520 5f66  pe) == 1 else _f
-00012ff0: 6974 5f58 2c0a 2020 2020 2020 2020 2020  it_X,.          
-00013000: 2020 6f70 7469 6f6e 733d 696e 7075 745f    options=input_
-00013010: 6f70 7469 6f6e 732c 0a20 2020 2020 2020  options,.       
-00013020: 2029 0a20 2020 2020 2020 2073 656c 662e   ).        self.
-00013030: 5f71 5f66 6974 5f58 203d 2071 5f66 6974  _q_fit_X = q_fit
-00013040: 5f58 2e71 7661 6c75 6573 0a20 2020 2020  _X.qvalues.     
-00013050: 2020 2073 656c 662e 5f71 5f66 6974 5f58     self._q_fit_X
-00013060: 5f71 7561 6e74 697a 6572 203d 2071 5f66  _quantizer = q_f
-00013070: 6974 5f58 2e71 7561 6e74 697a 6572 0a0a  it_X.quantizer..
-00013080: 2020 2020 2020 2020 2320 6d79 7079 0a20          # mypy. 
-00013090: 2020 2020 2020 2061 7373 6572 7420 7365         assert se
-000130a0: 6c66 2e5f 715f 6669 745f 585f 7175 616e  lf._q_fit_X_quan
-000130b0: 7469 7a65 722e 7363 616c 6520 6973 206e  tizer.scale is n
-000130c0: 6f74 204e 6f6e 650a 0a20 2020 2020 2020  ot None..       
-000130d0: 2073 656c 662e 5f79 203d 206e 756d 7079   self._y = numpy
-000130e0: 2e61 7272 6179 2879 290a 0a20 2020 2020  .array(y)..     
-000130f0: 2020 2023 2057 6520 6173 7375 6d65 2074     # We assume t
-00013100: 6861 7420 7468 6520 7175 6572 7920 6861  hat the query ha
-00013110: 7320 7468 6520 7361 6d65 2064 6973 7472  s the same distr
-00013120: 6962 7574 696f 6e20 6173 2074 6865 2064  ibution as the d
-00013130: 6174 6120 696e 205f 585f 6669 742e 0a20  ata in _X_fit.. 
-00013140: 2020 2020 2020 2023 2074 6865 7265 666f         # therefo
-00013150: 7265 2c20 7468 6579 2075 7365 2074 6865  re, they use the
-00013160: 2073 616d 6520 7363 616c 696e 6720 616e   same scaling an
-00013170: 6420 7a65 726f 2070 6f69 6e74 2e0a 2020  d zero point..  
-00013180: 2020 2020 2020 2320 6874 7470 733a 2f2f        # https://
-00013190: 6172 7869 762e 6f72 672f 6162 732f 3137  arxiv.org/abs/17
-000131a0: 3132 2e30 3538 3737 0a0a 2020 2020 2020  12.05877..      
-000131b0: 2020 7365 6c66 2e6f 7574 7075 745f 7175    self.output_qu
-000131c0: 616e 745f 7061 7261 6d73 203d 2055 6e69  ant_params = Uni
-000131d0: 666f 726d 5175 616e 7469 7a61 7469 6f6e  formQuantization
-000131e0: 5061 7261 6d65 7465 7273 280a 2020 2020  Parameters(.    
-000131f0: 2020 2020 2020 2020 7363 616c 653d 7365          scale=se
-00013200: 6c66 2e5f 715f 6669 745f 585f 7175 616e  lf._q_fit_X_quan
-00013210: 7469 7a65 722e 7363 616c 652c 0a20 2020  tizer.scale,.   
-00013220: 2020 2020 2020 2020 207a 6572 6f5f 706f           zero_po
-00013230: 696e 743d 7365 6c66 2e5f 715f 6669 745f  int=self._q_fit_
-00013240: 585f 7175 616e 7469 7a65 722e 7a65 726f  X_quantizer.zero
-00013250: 5f70 6f69 6e74 2c0a 2020 2020 2020 2020  _point,.        
-00013260: 2020 2020 6f66 6673 6574 3d30 2c0a 2020      offset=0,.  
-00013270: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00013280: 206f 7574 7075 745f 7175 616e 7469 7a65   output_quantize
-00013290: 7220 3d20 556e 6966 6f72 6d51 7561 6e74  r = UniformQuant
-000132a0: 697a 6572 2870 6172 616d 733d 7365 6c66  izer(params=self
-000132b0: 2e6f 7574 7075 745f 7175 616e 745f 7061  .output_quant_pa
-000132c0: 7261 6d73 2c20 6e6f 5f63 6c69 7070 696e  rams, no_clippin
-000132d0: 673d 5472 7565 290a 0a20 2020 2020 2020  g=True)..       
-000132e0: 2061 7373 6572 7420 6f75 7470 7574 5f71   assert output_q
-000132f0: 7561 6e74 697a 6572 2e7a 6572 6f5f 706f  uantizer.zero_po
-00013300: 696e 7420 6973 206e 6f74 204e 6f6e 650a  int is not None.
-00013310: 2020 2020 2020 2020 7365 6c66 2e6f 7574          self.out
-00013320: 7075 745f 7175 616e 7469 7a65 7273 2e61  put_quantizers.a
-00013330: 7070 656e 6428 6f75 7470 7574 5f71 7561  ppend(output_qua
-00013340: 6e74 697a 6572 290a 0a20 2020 2020 2020  ntizer)..       
-00013350: 2023 2055 7064 6174 696e 6720 706f 7374   # Updating post
-00013360: 2d70 726f 6365 7373 696e 6720 7061 7261  -processing para
-00013370: 6d65 7465 7273 0a20 2020 2020 2020 2073  meters.        s
-00013380: 656c 662e 5f73 6574 5f70 6f73 745f 7072  elf._set_post_pr
-00013390: 6f63 6573 7369 6e67 5f70 6172 616d 7328  ocessing_params(
-000133a0: 290a 0a20 2020 2020 2020 2073 656c 662e  )..        self.
-000133b0: 5f69 735f 6669 7474 6564 203d 2054 7275  _is_fitted = Tru
-000133c0: 650a 0a20 2020 2020 2020 2072 6574 7572  e..        retur
-000133d0: 6e20 7365 6c66 0a0a 2020 2020 6465 6620  n self..    def 
-000133e0: 7175 616e 7469 7a65 5f69 6e70 7574 2873  quantize_input(s
-000133f0: 656c 662c 2058 3a20 6e75 6d70 792e 6e64  elf, X: numpy.nd
-00013400: 6172 7261 7929 202d 3e20 6e75 6d70 792e  array) -> numpy.
-00013410: 6e64 6172 7261 793a 0a20 2020 2020 2020  ndarray:.       
-00013420: 2073 656c 662e 6368 6563 6b5f 6d6f 6465   self.check_mode
-00013430: 6c5f 6973 5f66 6974 7465 6428 290a 2020  l_is_fitted().  
-00013440: 2020 2020 2020 715f 5820 3d20 7365 6c66        q_X = self
-00013450: 2e69 6e70 7574 5f71 7561 6e74 697a 6572  .input_quantizer
-00013460: 735b 305d 2e71 7561 6e74 2858 290a 0a20  s[0].quant(X).. 
-00013470: 2020 2020 2020 2061 7373 6572 7420 715f         assert q_
-00013480: 582e 6474 7970 6520 3d3d 206e 756d 7079  X.dtype == numpy
-00013490: 2e69 6e74 3634 2c20 2249 6e70 7574 7320  .int64, "Inputs 
-000134a0: 7765 7265 206e 6f74 2071 7561 6e74 697a  were not quantiz
-000134b0: 6564 2074 6f20 696e 7436 3420 7661 6c75  ed to int64 valu
-000134c0: 6573 220a 2020 2020 2020 2020 7265 7475  es".        retu
-000134d0: 726e 2071 5f58 0a0a 2020 2020 6465 6620  rn q_X..    def 
-000134e0: 6465 7175 616e 7469 7a65 5f6f 7574 7075  dequantize_outpu
-000134f0: 7428 7365 6c66 2c20 715f 795f 7072 6564  t(self, q_y_pred
-00013500: 733a 206e 756d 7079 2e6e 6461 7272 6179  s: numpy.ndarray
-00013510: 2920 2d3e 206e 756d 7079 2e6e 6461 7272  ) -> numpy.ndarr
-00013520: 6179 3a0a 2020 2020 2020 2020 7365 6c66  ay:.        self
-00013530: 2e63 6865 636b 5f6d 6f64 656c 5f69 735f  .check_model_is_
-00013540: 6669 7474 6564 2829 0a20 2020 2020 2020  fitted().       
-00013550: 2023 2057 6520 636f 6d70 7574 6520 7468   # We compute th
-00013560: 6520 736f 7274 6564 2061 7267 6d61 7820  e sorted argmax 
-00013570: 696e 2046 4845 2c20 7768 6963 6820 6172  in FHE, which ar
-00013580: 6520 696e 7465 6765 7273 2e0a 2020 2020  e integers..    
-00013590: 2020 2020 2320 4e6f 206e 6565 6420 746f      # No need to
-000135a0: 2064 652d 7175 616e 7469 7a65 2074 6865   de-quantize the
-000135b0: 206f 7574 7075 7420 7661 6c75 6573 0a20   output values. 
-000135c0: 2020 2020 2020 2072 6574 7572 6e20 715f         return q_
-000135d0: 795f 7072 6564 730a 0a20 2020 2064 6566  y_preds..    def
-000135e0: 205f 6765 745f 6d6f 6475 6c65 5f74 6f5f   _get_module_to_
-000135f0: 636f 6d70 696c 6528 7365 6c66 2920 2d3e  compile(self) ->
-00013600: 2055 6e69 6f6e 5b43 6f6d 7069 6c65 722c   Union[Compiler,
-00013610: 2051 7561 6e74 697a 6564 4d6f 6475 6c65   QuantizedModule
-00013620: 5d3a 0a20 2020 2020 2020 2023 2044 6566  ]:.        # Def
-00013630: 696e 6520 7468 6520 696e 6665 7265 6e63  ine the inferenc
-00013640: 6520 6675 6e63 7469 6f6e 2074 6f20 636f  e function to co
-00013650: 6d70 696c 652e 0a20 2020 2020 2020 2023  mpile..        #
-00013660: 2054 6869 7320 6675 6e63 7469 6f6e 2063   This function c
-00013670: 616e 206e 6569 7468 6572 2062 6520 6120  an neither be a 
-00013680: 636c 6173 7320 6d65 7468 6f64 206e 6f72  class method nor
-00013690: 2061 2073 7461 7469 6320 6f6e 6520 6265   a static one be
-000136a0: 6361 7573 6520 7365 6c66 2077 6520 7761  cause self we wa
-000136b0: 6e74 2074 6f20 6176 6f69 640a 2020 2020  nt to avoid.    
-000136c0: 2020 2020 2320 6861 7669 6e67 2073 656c      # having sel
-000136d0: 6620 6173 2061 2070 6172 616d 6574 6572  f as a parameter
-000136e0: 2077 6869 6c65 2073 7469 6c6c 2062 6569   while still bei
-000136f0: 6e67 2061 626c 6520 746f 2061 6363 6573  ng able to acces
-00013700: 7320 736f 6d65 206f 6620 6974 7320 6174  s some of its at
-00013710: 7472 6962 7574 650a 2020 2020 2020 2020  tribute.        
-00013720: 6465 6620 696e 6665 7265 6e63 655f 746f  def inference_to
-00013730: 5f63 6f6d 7069 6c65 2871 5f58 3a20 6e75  _compile(q_X: nu
-00013740: 6d70 792e 6e64 6172 7261 7929 202d 3e20  mpy.ndarray) -> 
-00013750: 6e75 6d70 792e 6e64 6172 7261 793a 0a20  numpy.ndarray:. 
-00013760: 2020 2020 2020 2020 2020 2022 2222 436f             """Co
-00013770: 6d70 696c 6520 7468 6520 6369 7263 7569  mpile the circui
-00013780: 7420 696e 2046 4845 2075 7369 6e67 206f  t in FHE using o
-00013790: 6e6c 7920 7468 6520 696e 7075 7473 2061  nly the inputs a
-000137a0: 7320 7061 7261 6d65 7465 7273 2e0a 0a20  s parameters... 
-000137b0: 2020 2020 2020 2020 2020 2041 7267 733a             Args:
-000137c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000137d0: 2071 5f58 2028 6e75 6d70 792e 6e64 6172   q_X (numpy.ndar
-000137e0: 7261 7929 3a20 5468 6520 7175 616e 7469  ray): The quanti
-000137f0: 7a65 6420 696e 7075 7420 6461 7461 0a0a  zed input data..
-00013800: 2020 2020 2020 2020 2020 2020 5265 7475              Retu
-00013810: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-00013820: 2020 2020 206e 756d 7079 2e6e 6461 7272       numpy.ndarr
-00013830: 6179 3a20 5468 6520 6369 7263 7569 7420  ay: The circuit 
-00013840: 6973 206f 7574 7075 7473 2e0a 2020 2020  is outputs..    
-00013850: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00013860: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00013870: 656c 662e 5f69 6e66 6572 656e 6365 2871  elf._inference(q
-00013880: 5f58 290a 0a20 2020 2020 2020 2023 2043  _X)..        # C
-00013890: 7265 6174 6520 7468 6520 636f 6d70 696c  reate the compil
-000138a0: 6572 2069 6e73 7461 6e63 650a 2020 2020  er instance.    
-000138b0: 2020 2020 636f 6d70 696c 6572 203d 2043      compiler = C
-000138c0: 6f6d 7069 6c65 7228 696e 6665 7265 6e63  ompiler(inferenc
-000138d0: 655f 746f 5f63 6f6d 7069 6c65 2c20 7b22  e_to_compile, {"
-000138e0: 715f 5822 3a20 2265 6e63 7279 7074 6564  q_X": "encrypted
-000138f0: 227d 290a 0a20 2020 2020 2020 2072 6574  "})..        ret
-00013900: 7572 6e20 636f 6d70 696c 6572 0a0a 2020  urn compiler..  
-00013910: 2020 4073 7461 7469 636d 6574 686f 640a    @staticmethod.
-00013920: 2020 2020 6465 6620 6d61 6a6f 7269 7479      def majority
-00013930: 5f76 6f74 6528 6e65 6172 6573 745f 636c  _vote(nearest_cl
-00013940: 6173 7365 733a 206e 756d 7079 2e6e 6461  asses: numpy.nda
-00013950: 7272 6179 293a 0a20 2020 2020 2020 2022  rray):.        "
-00013960: 2222 4465 7465 726d 696e 6520 7468 6520  ""Determine the 
-00013970: 6d6f 7374 2063 6f6d 6d6f 6e20 636c 6173  most common clas
-00013980: 7320 616d 6f6e 6720 6e65 6172 6573 7420  s among nearest 
-00013990: 6e65 6967 6862 6f72 7366 6f72 2065 6163  neighborsfor eac
-000139a0: 6820 7175 6572 792e 0a0a 2020 2020 2020  h query...      
-000139b0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-000139c0: 2020 2020 6e65 6172 6573 745f 636c 6173      nearest_clas
-000139d0: 7365 7320 286e 756d 7079 2e6e 6461 7272  ses (numpy.ndarr
-000139e0: 6179 293a 2054 6865 2063 6c61 7373 206c  ay): The class l
-000139f0: 6162 656c 7320 6f66 2074 6865 206e 6561  abels of the nea
-00013a00: 7265 7374 206e 6569 6768 626f 7273 2066  rest neighbors f
-00013a10: 6f72 2061 2071 7565 7279 0a0a 2020 2020  or a query..    
-00013a20: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
-00013a30: 2020 2020 2020 2020 206e 756d 7079 2e6e           numpy.n
-00013a40: 6461 7272 6179 3a20 5468 6520 6d61 6a6f  darray: The majo
-00013a50: 7269 7479 2d76 6f74 6564 2063 6c61 7373  rity-voted class
-00013a60: 206c 6162 656c 2066 6f72 2074 6865 2063   label for the c
-00013a70: 6f72 7265 7370 6f6e 6469 6e67 2071 7565  orresponding que
-00013a80: 7279 2e0a 2020 2020 2020 2020 2222 220a  ry..        """.
-00013a90: 2020 2020 2020 2020 636c 6173 735f 636f          class_co
-00013aa0: 756e 7473 203d 206e 756d 7079 2e62 696e  unts = numpy.bin
-00013ab0: 636f 756e 7428 6e65 6172 6573 745f 636c  count(nearest_cl
-00013ac0: 6173 7365 7329 0a20 2020 2020 2020 206d  asses).        m
-00013ad0: 616a 6f72 6974 795f 766f 7465 7320 3d20  ajority_votes = 
-00013ae0: 6e75 6d70 792e 6172 676d 6178 2863 6c61  numpy.argmax(cla
-00013af0: 7373 5f63 6f75 6e74 7329 0a0a 2020 2020  ss_counts)..    
-00013b00: 2020 2020 7265 7475 726e 206d 616a 6f72      return major
-00013b10: 6974 795f 766f 7465 730a 0a20 2020 2064  ity_votes..    d
-00013b20: 6566 205f 696e 6665 7265 6e63 6528 7365  ef _inference(se
-00013b30: 6c66 2c20 715f 583a 206e 756d 7079 2e6e  lf, q_X: numpy.n
-00013b40: 6461 7272 6179 2920 2d3e 206e 756d 7079  darray) -> numpy
-00013b50: 2e6e 6461 7272 6179 3a0a 2020 2020 2020  .ndarray:.      
-00013b60: 2020 2222 2249 6e66 6572 656e 6365 2066    """Inference f
-00013b70: 756e 6374 696f 6e2e 0a0a 2020 2020 2020  unction...      
-00013b80: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00013b90: 2020 2020 715f 5820 286e 756d 7079 2e6e      q_X (numpy.n
-00013ba0: 6461 7272 6179 293a 2054 6865 2071 7561  darray): The qua
-00013bb0: 6e74 697a 6564 2069 6e70 7574 2076 616c  ntized input val
-00013bc0: 7565 732e 0a0a 2020 2020 2020 2020 5265  ues...        Re
-00013bd0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
-00013be0: 2020 206e 756d 7079 2e6e 6461 7272 6179     numpy.ndarray
-00013bf0: 3a20 5468 6520 7175 616e 7469 7a65 6420  : The quantized 
-00013c00: 7072 6564 6963 7465 6420 7661 6c75 6573  predicted values
-00013c10: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00013c20: 2020 2020 2020 6173 7365 7274 2073 656c        assert sel
-00013c30: 662e 5f71 5f66 6974 5f58 5f71 7561 6e74  f._q_fit_X_quant
-00013c40: 697a 6572 2069 7320 6e6f 7420 4e6f 6e65  izer is not None
-00013c50: 2c20 7365 6c66 2e5f 6973 5f6e 6f74 5f66  , self._is_not_f
-00013c60: 6974 7465 645f 6572 726f 725f 6d65 7373  itted_error_mess
-00013c70: 6167 6528 290a 0a20 2020 2020 2020 2064  age()..        d
-00013c80: 6566 2070 6169 7277 6973 655f 6575 636c  ef pairwise_eucl
-00013c90: 6964 6561 6e5f 6469 7374 616e 6365 2871  idean_distance(q
-00013ca0: 5f58 293a 0a20 2020 2020 2020 2020 2020  _X):.           
-00013cb0: 2023 2031 2e20 5061 6972 7769 7365 2065   # 1. Pairwise e
-00013cc0: 7563 6c69 6465 616e 2064 6973 7461 6e63  uclidean distanc
-00013cd0: 650a 2020 2020 2020 2020 2020 2020 2320  e.            # 
-00013ce0: 6469 7374 2878 2c20 7929 203d 2073 7172  dist(x, y) = sqr
-00013cf0: 7428 646f 7428 782c 2078 2920 2d20 3220  t(dot(x, x) - 2 
-00013d00: 2a20 646f 7428 782c 2079 2920 2b20 646f  * dot(x, y) + do
-00013d10: 7428 792c 2079 2929 0a20 2020 2020 2020  t(y, y)).       
-00013d20: 2020 2020 2072 6574 7572 6e20 280a 2020       return (.  
-00013d30: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
-00013d40: 6d70 792e 7375 6d28 715f 582a 2a32 2c20  mpy.sum(q_X**2, 
-00013d50: 6178 6973 3d31 2c20 6b65 6570 6469 6d73  axis=1, keepdims
-00013d60: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
-00013d70: 2020 2020 2020 202d 2032 202a 2071 5f58         - 2 * q_X
-00013d80: 2040 2073 656c 662e 5f71 5f66 6974 5f58   @ self._q_fit_X
-00013d90: 2e54 0a20 2020 2020 2020 2020 2020 2020  .T.             
-00013da0: 2020 202b 206e 756d 7079 2e65 7870 616e     + numpy.expan
-00013db0: 645f 6469 6d73 286e 756d 7079 2e73 756d  d_dims(numpy.sum
-00013dc0: 2873 656c 662e 5f71 5f66 6974 5f58 2a2a  (self._q_fit_X**
-00013dd0: 322c 2061 7869 733d 3129 2c20 3029 0a20  2, axis=1), 0). 
-00013de0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00013df0: 2020 2020 2020 6465 6620 746f 706b 5f73        def topk_s
-00013e00: 6f72 7469 6e67 2878 2c20 6c61 6265 6c73  orting(x, labels
-00013e10: 293a 0a20 2020 2020 2020 2020 2020 2022  ):.            "
-00013e20: 2222 4172 6773 6f72 7420 696e 2046 4845  ""Argsort in FHE
-00013e30: 2e0a 0a20 2020 2020 2020 2020 2020 2054  ...            T
-00013e40: 696d 6520 636f 6d70 6c65 7869 7479 3a20  ime complexity: 
-00013e50: 4f28 6e6c 6f67 c2b2 286b 2929 0a0a 2020  O(nlog..(k))..  
-00013e60: 2020 2020 2020 2020 2020 4172 6773 3a0a            Args:.
-00013e70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013e80: 7820 286e 756d 7079 2e6e 6461 7272 6179  x (numpy.ndarray
-00013e90: 293a 2054 6865 2071 7561 6e74 697a 6564  ): The quantized
-00013ea0: 2069 6e70 7574 2076 616c 7565 730a 2020   input values.  
-00013eb0: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-00013ec0: 6265 6c73 2028 6e75 6d70 792e 6e64 6172  bels (numpy.ndar
-00013ed0: 7261 7929 3a20 5468 6520 6c61 6265 6c73  ray): The labels
-00013ee0: 206f 6620 7468 6520 7472 6169 6e69 6e67   of the training
-00013ef0: 2064 6174 612d 7365 740a 0a20 2020 2020   data-set..     
-00013f00: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00013f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013f20: 6e75 6d70 792e 6e64 6172 7261 793a 2054  numpy.ndarray: T
-00013f30: 6865 2061 7267 736f 7274 2e0a 2020 2020  he argsort..    
-00013f40: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
-00013f50: 2020 2020 2020 2020 2064 6566 2067 6174           def gat
-00013f60: 6865 7231 6428 782c 2069 6e64 6963 6573  her1d(x, indices
-00013f70: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00013f80: 2020 2022 2222 5365 6c65 6374 2065 6c65     """Select ele
-00013f90: 6d65 6e74 7320 6672 6f6d 2074 6865 2069  ments from the i
-00013fa0: 6e70 7574 2061 7272 6179 2060 7860 2075  nput array `x` u
-00013fb0: 7369 6e67 2074 6865 2070 726f 7669 6465  sing the provide
-00013fc0: 6420 6069 6e64 6963 6573 602e 0a0a 2020  d `indices`...  
-00013fd0: 2020 2020 2020 2020 2020 2020 2020 4172                Ar
-00013fe0: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
-00013ff0: 2020 2020 2020 2020 7820 286e 756d 7079          x (numpy
-00014000: 2e6e 6461 7272 6179 293a 2054 6865 2065  .ndarray): The e
-00014010: 6e63 7279 7074 6564 2069 6e70 7574 2061  ncrypted input a
-00014020: 7272 6179 0a20 2020 2020 2020 2020 2020  rray.           
-00014030: 2020 2020 2020 2020 2069 6e64 6963 6573           indices
-00014040: 2028 6e75 6d70 792e 6e64 6172 7261 7929   (numpy.ndarray)
-00014050: 3a20 5468 6520 6465 7369 7265 6420 696e  : The desired in
-00014060: 6465 7865 730a 0a20 2020 2020 2020 2020  dexes..         
-00014070: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00014080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014090: 2020 2020 6e75 6d70 792e 6e64 6172 7261      numpy.ndarra
-000140a0: 793a 2054 6865 2073 656c 6563 7465 6420  y: The selected 
-000140b0: 656e 6372 7970 7465 6420 696e 6465 7865  encrypted indexe
-000140c0: 732e 0a20 2020 2020 2020 2020 2020 2020  s..             
-000140d0: 2020 2022 2222 0a20 2020 2020 2020 2020     """.         
-000140e0: 2020 2020 2020 2061 7272 203d 205b 5d0a         arr = [].
-000140f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014100: 666f 7220 6920 696e 2069 6e64 6963 6573  for i in indices
-00014110: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00014120: 2020 2020 2020 6172 722e 6170 7065 6e64        arr.append
-00014130: 2878 5b69 5d29 0a20 2020 2020 2020 2020  (x[i]).         
-00014140: 2020 2020 2020 2065 6e63 5f61 7272 203d         enc_arr =
-00014150: 2063 702e 6172 7261 7928 6172 7229 0a20   cp.array(arr). 
-00014160: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00014170: 6574 7572 6e20 656e 635f 6172 720a 0a20  eturn enc_arr.. 
-00014180: 2020 2020 2020 2020 2020 2064 6566 2073             def s
-00014190: 6361 7474 6572 3164 2878 2c20 762c 2069  catter1d(x, v, i
-000141a0: 6e64 6963 6573 293a 0a20 2020 2020 2020  ndices):.       
-000141b0: 2020 2020 2020 2020 2022 2222 5265 6172           """Rear
-000141c0: 7261 6e67 6520 656c 656d 656e 7473 206f  range elements o
-000141d0: 6620 6078 6020 7769 7468 2076 616c 7565  f `x` with value
-000141e0: 7320 6672 6f6d 2060 7660 2061 7420 7468  s from `v` at th
-000141f0: 6520 7370 6563 6966 6965 6420 6069 6e64  e specified `ind
-00014200: 6963 6573 602e 0a0a 2020 2020 2020 2020  ices`...        
-00014210: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00014220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014230: 2020 7820 286e 756d 7079 2e6e 6461 7272    x (numpy.ndarr
-00014240: 6179 293a 2054 6865 2065 6e63 7279 7074  ay): The encrypt
-00014250: 6564 2069 6e70 7574 2061 7272 6179 2069  ed input array i
-00014260: 6e20 7768 6963 6820 6974 656d 7320 7769  n which items wi
-00014270: 6c6c 2062 6520 7570 6461 7465 640a 2020  ll be updated.  
-00014280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014290: 2020 7620 286e 756d 7079 2e6e 6461 7272    v (numpy.ndarr
-000142a0: 6179 293a 2054 6865 2061 7272 6179 2063  ay): The array c
-000142b0: 6f6e 7461 696e 696e 6720 7661 6c75 6573  ontaining values
-000142c0: 2074 6f20 6265 2069 6e73 6572 7465 6420   to be inserted 
-000142d0: 696e 746f 2060 7860 0a20 2020 2020 2020  into `x`.       
-000142e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000142f0: 2061 7420 7468 6520 7370 6563 6966 6965   at the specifie
-00014300: 6420 6069 6e64 6963 6573 602e 0a20 2020  d `indices`..   
-00014310: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014320: 2069 6e64 6963 6573 2028 6e75 6d70 792e   indices (numpy.
-00014330: 6e64 6172 7261 7929 3a20 5468 6520 696e  ndarray): The in
-00014340: 6469 6365 7320 696e 6469 6361 7469 6e67  dices indicating
-00014350: 2077 6865 7265 2074 6f20 696e 7365 7274   where to insert
-00014360: 2074 6865 2065 6c65 6d65 6e74 730a 2020   the elements.  
-00014370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014380: 2020 2020 2020 6672 6f6d 2060 7660 2069        from `v` i
-00014390: 6e74 6f20 6078 602e 0a0a 2020 2020 2020  nto `x`...      
-000143a0: 2020 2020 2020 2020 2020 5265 7475 726e            Return
-000143b0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
-000143c0: 2020 2020 2020 206e 756d 7079 2e6e 6461         numpy.nda
-000143d0: 7272 6179 3a20 5468 6520 7570 6461 7465  rray: The update
-000143e0: 6420 656e 6372 7970 7465 6420 6078 600a  d encrypted `x`.
-000143f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014400: 2222 220a 2020 2020 2020 2020 2020 2020  """.            
-00014410: 2020 2020 666f 7220 6964 782c 2069 2069      for idx, i i
-00014420: 6e20 656e 756d 6572 6174 6528 696e 6469  n enumerate(indi
-00014430: 6365 7329 3a0a 2020 2020 2020 2020 2020  ces):.          
-00014440: 2020 2020 2020 2020 2020 785b 695d 203d            x[i] =
-00014450: 2076 5b69 6478 5d0a 2020 2020 2020 2020   v[idx].        
-00014460: 2020 2020 2020 2020 7265 7475 726e 2078          return x
-00014470: 0a0a 2020 2020 2020 2020 2020 2020 636f  ..            co
-00014480: 6d70 6172 6973 6f6e 7320 3d20 6e75 6d70  mparisons = nump
-00014490: 792e 7a65 726f 7328 782e 7368 6170 6529  y.zeros(x.shape)
-000144a0: 0a20 2020 2020 2020 2020 2020 206c 6162  .            lab
-000144b0: 656c 7320 3d20 6c61 6265 6c73 202b 2063  els = labels + c
-000144c0: 702e 7a65 726f 7328 6c61 6265 6c73 2e73  p.zeros(labels.s
-000144d0: 6861 7065 290a 0a20 2020 2020 2020 2020  hape)..         
-000144e0: 2020 206e 2c20 6b20 3d20 782e 7369 7a65     n, k = x.size
-000144f0: 2c20 7365 6c66 2e6e 5f6e 6569 6768 626f  , self.n_neighbo
-00014500: 7273 0a20 2020 2020 2020 2020 2020 2023  rs.            #
-00014510: 2044 6574 6572 6d69 6e65 2074 6865 206e   Determine the n
-00014520: 756d 6265 7220 6f66 2073 7461 6765 7320  umber of stages 
-00014530: 666f 7220 6120 7365 7175 656e 6365 206f  for a sequence o
-00014540: 6620 6c65 6e67 7468 206e 0a20 2020 2020  f length n.     
-00014550: 2020 2020 2020 206c 6e32 6e20 3d20 696e         ln2n = in
-00014560: 7428 6e75 6d70 792e 6365 696c 286e 756d  t(numpy.ceil(num
-00014570: 7079 2e6c 6f67 3228 6e29 2929 0a0a 2020  py.log2(n)))..  
-00014580: 2020 2020 2020 2020 2020 2320 5374 6167            # Stag
-00014590: 6520 6c6f 6f70 0a20 2020 2020 2020 2020  e loop.         
-000145a0: 2020 2066 6f72 2074 2069 6e20 7261 6e67     for t in rang
-000145b0: 6528 6c6e 326e 202d 2031 2c20 2d31 2c20  e(ln2n - 1, -1, 
-000145c0: 2d31 293a 0a20 2020 2020 2020 2020 2020  -1):.           
-000145d0: 2020 2020 2023 2070 3a20 4465 7465 726d       # p: Determ
-000145e0: 696e 6573 2074 6865 2072 616e 6765 206f  ines the range o
-000145f0: 6620 696e 6465 7865 7320 746f 2062 6520  f indexes to be 
-00014600: 636f 6d70 6172 6564 2069 6e20 6561 6368  compared in each
-00014610: 2070 6173 732e 0a20 2020 2020 2020 2020   pass..         
-00014620: 2020 2020 2020 2070 203d 2032 2a2a 740a         p = 2**t.
-00014630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014640: 2320 723a 204f 6666 7365 7420 7468 6174  # r: Offset that
-00014650: 2061 646a 7573 7473 2074 6865 2072 616e   adjusts the ran
-00014660: 6765 206f 6620 696e 6465 7865 7320 746f  ge of indexes to
-00014670: 2062 6520 636f 6d70 6172 6564 2061 6e64   be compared and
-00014680: 2073 6f72 7465 6420 696e 2065 6163 6820   sorted in each 
-00014690: 7061 7373 0a20 2020 2020 2020 2020 2020  pass.           
-000146a0: 2020 2020 2072 203d 2030 0a20 2020 2020       r = 0.     
-000146b0: 2020 2020 2020 2020 2020 2023 2064 3a20             # d: 
-000146c0: 436f 6d70 6172 6973 6f6e 2064 6973 7461  Comparison dista
-000146d0: 6e63 6520 696e 2065 6163 6820 7061 7373  nce in each pass
-000146e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000146f0: 2064 203d 2070 0a20 2020 2020 2020 2020   d = p.         
-00014700: 2020 2020 2020 2023 204e 756d 6265 7220         # Number 
-00014710: 6f66 2070 6173 7365 7320 666f 7220 6561  of passes for ea
-00014720: 6368 2073 7461 6765 0a20 2020 2020 2020  ch stage.       
-00014730: 2020 2020 2020 2020 2066 6f72 2062 7120           for bq 
-00014740: 696e 2072 616e 6765 286c 6e32 6e20 2d20  in range(ln2n - 
-00014750: 312c 2074 202d 2031 2c20 2d31 293a 0a20  1, t - 1, -1):. 
+0000dea0: 4f6e 6c79 2061 7070 6c79 2074 6865 2073  Only apply the s
+0000deb0: 756d 2069 6e20 7468 6520 636c 6561 7220  um in the clear 
+0000dec0: 6966 2069 7420 6861 7320 6e6f 7420 616c  if it has not al
+0000ded0: 7265 6164 7920 6265 656e 2064 6f6e 6520  ready been done 
+0000dee0: 696e 2046 4845 0a20 2020 2020 2020 2069  in FHE.        i
+0000def0: 6620 6e6f 7420 7365 6c66 2e5f 6668 655f  f not self._fhe_
+0000df00: 656e 7365 6d62 6c69 6e67 3a0a 2020 2020  ensembling:.    
+0000df10: 2020 2020 2020 2020 795f 7072 6564 7320          y_preds 
+0000df20: 3d20 6e75 6d70 792e 7375 6d28 795f 7072  = numpy.sum(y_pr
+0000df30: 6564 732c 2061 7869 733d 2d31 290a 0a20  eds, axis=-1).. 
+0000df40: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+0000df50: 745f 7472 7565 2879 5f70 7265 6473 2e6e  t_true(y_preds.n
+0000df60: 6469 6d20 3d3d 2032 2c20 2279 5f70 7265  dim == 2, "y_pre
+0000df70: 6473 2073 686f 756c 6420 6265 2061 2032  ds should be a 2
+0000df80: 4420 6172 7261 7922 290a 2020 2020 2020  D array").      
+0000df90: 2020 2020 2020 7265 7475 726e 2079 5f70        return y_p
+0000dfa0: 7265 6473 0a0a 2020 2020 2020 2020 7265  reds..        re
+0000dfb0: 7475 726e 2073 7570 6572 2829 2e70 6f73  turn super().pos
+0000dfc0: 745f 7072 6f63 6573 7369 6e67 2879 5f70  t_processing(y_p
+0000dfd0: 7265 6473 290a 0a0a 636c 6173 7320 4261  reds)...class Ba
+0000dfe0: 7365 5472 6565 5265 6772 6573 736f 724d  seTreeRegressorM
+0000dff0: 6978 696e 2842 6173 6554 7265 6545 7374  ixin(BaseTreeEst
+0000e000: 696d 6174 6f72 4d69 7869 6e2c 2073 6b6c  imatorMixin, skl
+0000e010: 6561 726e 2e62 6173 652e 5265 6772 6573  earn.base.Regres
+0000e020: 736f 724d 6978 696e 2c20 4142 4329 3a0a  sorMixin, ABC):.
+0000e030: 2020 2020 2222 224d 6978 696e 2063 6c61      """Mixin cla
+0000e040: 7373 2066 6f72 2074 7265 652d 6261 7365  ss for tree-base
+0000e050: 6420 7265 6772 6573 736f 7273 2e0a 0a20  d regressors... 
+0000e060: 2020 2054 6869 7320 636c 6173 7320 6973     This class is
+0000e070: 2075 7365 6420 746f 2063 7265 6174 6520   used to create 
+0000e080: 6120 7472 6565 2d62 6173 6564 2072 6567  a tree-based reg
+0000e090: 7265 7373 6f72 2063 6c61 7373 2074 6861  ressor class tha
+0000e0a0: 7420 696e 6865 7269 7473 2066 726f 6d0a  t inherits from.
+0000e0b0: 2020 2020 736b 6c65 6172 6e2e 6261 7365      sklearn.base
+0000e0c0: 2e52 6567 7265 7373 6f72 4d69 7869 6e2c  .RegressorMixin,
+0000e0d0: 2077 6869 6368 2065 7373 656e 7469 616c   which essential
+0000e0e0: 6c79 2067 6976 6573 2061 6363 6573 7320  ly gives access 
+0000e0f0: 746f 2073 6369 6b69 742d 6c65 6172 6e27  to scikit-learn'
+0000e100: 7320 6073 636f 7265 6020 6d65 7468 6f64  s `score` method
+0000e110: 0a20 2020 2066 6f72 2072 6567 7265 7373  .    for regress
+0000e120: 6f72 732e 0a20 2020 2022 2222 0a0a 0a63  ors..    """...c
+0000e130: 6c61 7373 2042 6173 6554 7265 6543 6c61  lass BaseTreeCla
+0000e140: 7373 6966 6965 724d 6978 696e 280a 2020  ssifierMixin(.  
+0000e150: 2020 4261 7365 436c 6173 7369 6669 6572    BaseClassifier
+0000e160: 2c20 4261 7365 5472 6565 4573 7469 6d61  , BaseTreeEstima
+0000e170: 746f 724d 6978 696e 2c20 736b 6c65 6172  torMixin, sklear
+0000e180: 6e2e 6261 7365 2e43 6c61 7373 6966 6965  n.base.Classifie
+0000e190: 724d 6978 696e 2c20 4142 430a 293a 0a20  rMixin, ABC.):. 
+0000e1a0: 2020 2022 2222 4d69 7869 6e20 636c 6173     """Mixin clas
+0000e1b0: 7320 666f 7220 7472 6565 2d62 6173 6564  s for tree-based
+0000e1c0: 2063 6c61 7373 6966 6965 7273 2e0a 0a20   classifiers... 
+0000e1d0: 2020 2054 6869 7320 636c 6173 7320 6973     This class is
+0000e1e0: 2075 7365 6420 746f 2063 7265 6174 6520   used to create 
+0000e1f0: 6120 7472 6565 2d62 6173 6564 2063 6c61  a tree-based cla
+0000e200: 7373 6966 6965 7220 636c 6173 7320 7468  ssifier class th
+0000e210: 6174 2069 6e68 6572 6974 7320 6672 6f6d  at inherits from
+0000e220: 0a20 2020 2073 6b6c 6561 726e 2e62 6173  .    sklearn.bas
+0000e230: 652e 436c 6173 7369 6669 6572 4d69 7869  e.ClassifierMixi
+0000e240: 6e2c 2077 6869 6368 2065 7373 656e 7469  n, which essenti
+0000e250: 616c 6c79 2067 6976 6573 2061 6363 6573  ally gives acces
+0000e260: 7320 746f 2073 6369 6b69 742d 6c65 6172  s to scikit-lear
+0000e270: 6e27 7320 6073 636f 7265 6020 6d65 7468  n's `score` meth
+0000e280: 6f64 0a20 2020 2066 6f72 2063 6c61 7373  od.    for class
+0000e290: 6966 6965 7273 2e0a 0a20 2020 2041 6464  ifiers...    Add
+0000e2a0: 6974 696f 6e61 6c6c 792c 2074 6869 7320  itionally, this 
+0000e2b0: 636c 6173 7320 6164 6a75 7374 7320 736f  class adjusts so
+0000e2c0: 6d65 206f 6620 7468 6520 7472 6565 2d62  me of the tree-b
+0000e2d0: 6173 6564 2062 6173 6520 636c 6173 7327  ased base class'
+0000e2e0: 7320 6d65 7468 6f64 7320 696e 206f 7264  s methods in ord
+0000e2f0: 6572 2074 6f20 6d61 6b65 0a20 2020 2074  er to make.    t
+0000e300: 6865 6d20 636f 6d70 6c69 616e 7420 7769  hem compliant wi
+0000e310: 7468 2063 6c61 7373 6966 6963 6174 696f  th classificatio
+0000e320: 6e20 776f 726b 666c 6f77 732e 0a20 2020  n workflows..   
+0000e330: 2022 2222 0a0a 0a23 2070 796c 696e 743a   """...# pylint:
+0000e340: 2064 6973 6162 6c65 3d69 6e76 616c 6964   disable=invalid
+0000e350: 2d6e 616d 652c 746f 6f2d 6d61 6e79 2d69  -name,too-many-i
+0000e360: 6e73 7461 6e63 652d 6174 7472 6962 7574  nstance-attribut
+0000e370: 6573 0a63 6c61 7373 2053 6b6c 6561 726e  es.class Sklearn
+0000e380: 4c69 6e65 6172 4d6f 6465 6c4d 6978 696e  LinearModelMixin
+0000e390: 2842 6173 6545 7374 696d 6174 6f72 2c20  (BaseEstimator, 
+0000e3a0: 736b 6c65 6172 6e2e 6261 7365 2e42 6173  sklearn.base.Bas
+0000e3b0: 6545 7374 696d 6174 6f72 2c20 4142 4329  eEstimator, ABC)
+0000e3c0: 3a0a 2020 2020 2222 2241 204d 6978 696e  :.    """A Mixin
+0000e3d0: 2063 6c61 7373 2066 6f72 2073 6b6c 6561   class for sklea
+0000e3e0: 726e 206c 696e 6561 7220 6d6f 6465 6c73  rn linear models
+0000e3f0: 2077 6974 6820 4648 452e 0a0a 2020 2020   with FHE...    
+0000e400: 5468 6973 2063 6c61 7373 2069 6e68 6572  This class inher
+0000e410: 6974 7320 6672 6f6d 2073 6b6c 6561 726e  its from sklearn
+0000e420: 2e62 6173 652e 4261 7365 4573 7469 6d61  .base.BaseEstima
+0000e430: 746f 7220 696e 206f 7264 6572 2074 6f20  tor in order to 
+0000e440: 6861 7665 2061 6363 6573 7320 746f 2073  have access to s
+0000e450: 6369 6b69 742d 6c65 6172 6e27 730a 2020  cikit-learn's.  
+0000e460: 2020 6067 6574 5f70 6172 616d 7360 2061    `get_params` a
+0000e470: 6e64 2060 7365 745f 7061 7261 6d73 6020  nd `set_params` 
+0000e480: 6d65 7468 6f64 732e 0a20 2020 2022 2222  methods..    """
+0000e490: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+0000e4a0: 5f73 7562 636c 6173 735f 5f28 636c 7329  _subclass__(cls)
+0000e4b0: 3a0a 2020 2020 2020 2020 666f 7220 6b6c  :.        for kl
+0000e4c0: 6173 7320 696e 2063 6c73 2e5f 5f6d 726f  ass in cls.__mro
+0000e4d0: 5f5f 3a0a 2020 2020 2020 2020 2020 2020  __:.            
+0000e4e0: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
+0000e4f0: 652d 6e65 7874 3d70 726f 7465 6374 6564  e-next=protected
+0000e500: 2d61 6363 6573 730a 2020 2020 2020 2020  -access.        
+0000e510: 2020 2020 6966 2067 6574 6174 7472 286b      if getattr(k
+0000e520: 6c61 7373 2c20 225f 6973 5f61 5f70 7562  lass, "_is_a_pub
+0000e530: 6c69 635f 636d 6c5f 6d6f 6465 6c22 2c20  lic_cml_model", 
+0000e540: 4661 6c73 6529 3a0a 2020 2020 2020 2020  False):.        
+0000e550: 2020 2020 2020 2020 5f4c 494e 4541 525f          _LINEAR_
+0000e560: 4d4f 4445 4c53 2e61 6464 2863 6c73 290a  MODELS.add(cls).
+0000e570: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e580: 5f41 4c4c 5f53 4b4c 4541 524e 5f4d 4f44  _ALL_SKLEARN_MOD
+0000e590: 454c 532e 6164 6428 636c 7329 0a0a 2020  ELS.add(cls)..  
+0000e5a0: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+0000e5b0: 656c 662c 206e 5f62 6974 733a 2055 6e69  elf, n_bits: Uni
+0000e5c0: 6f6e 5b69 6e74 2c20 4469 6374 5b73 7472  on[int, Dict[str
+0000e5d0: 2c20 696e 745d 5d20 3d20 3829 3a0a 2020  , int]] = 8):.  
+0000e5e0: 2020 2020 2020 2222 2249 6e69 7469 616c        """Initial
+0000e5f0: 697a 6520 7468 6520 4648 4520 6c69 6e65  ize the FHE line
+0000e600: 6172 206d 6f64 656c 2e0a 0a20 2020 2020  ar model...     
+0000e610: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+0000e620: 2020 2020 206e 5f62 6974 7320 2869 6e74       n_bits (int
+0000e630: 2c20 4469 6374 5b73 7472 2c20 696e 745d  , Dict[str, int]
+0000e640: 293a 204e 756d 6265 7220 6f66 2062 6974  ): Number of bit
+0000e650: 7320 746f 2071 7561 6e74 697a 6520 7468  s to quantize th
+0000e660: 6520 6d6f 6465 6c2e 2049 6620 616e 2069  e model. If an i
+0000e670: 6e74 2069 7320 7061 7373 6564 0a20 2020  nt is passed.   
+0000e680: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+0000e690: 206e 5f62 6974 732c 2074 6865 2076 616c   n_bits, the val
+0000e6a0: 7565 2077 696c 6c20 6265 2075 7365 6420  ue will be used 
+0000e6b0: 666f 7220 7175 616e 7469 7a69 6e67 2069  for quantizing i
+0000e6c0: 6e70 7574 7320 616e 6420 7765 6967 6874  nputs and weight
+0000e6d0: 732e 2049 6620 6120 6469 6374 2069 730a  s. If a dict is.
+0000e6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e6f0: 7061 7373 6564 2c20 7468 656e 2069 7420  passed, then it 
+0000e700: 7368 6f75 6c64 2063 6f6e 7461 696e 2022  should contain "
+0000e710: 6f70 5f69 6e70 7574 7322 2061 6e64 2022  op_inputs" and "
+0000e720: 6f70 5f77 6569 6768 7473 2220 6173 206b  op_weights" as k
+0000e730: 6579 7320 7769 7468 0a20 2020 2020 2020  eys with.       
+0000e740: 2020 2020 2020 2020 2063 6f72 7265 7370           corresp
+0000e750: 6f6e 6469 6e67 206e 756d 6265 7220 6f66  onding number of
+0000e760: 2071 7561 6e74 697a 6174 696f 6e20 6269   quantization bi
+0000e770: 7473 2073 6f20 7468 6174 3a0a 2020 2020  ts so that:.    
+0000e780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e790: 2d20 6f70 5f69 6e70 7574 7320 3a20 6e75  - op_inputs : nu
+0000e7a0: 6d62 6572 206f 6620 6269 7473 2074 6f20  mber of bits to 
+0000e7b0: 7175 616e 7469 7a65 2074 6865 2069 6e70  quantize the inp
+0000e7c0: 7574 2076 616c 7565 730a 2020 2020 2020  ut values.      
+0000e7d0: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
+0000e7e0: 6f70 5f77 6569 6768 7473 3a20 6e75 6d62  op_weights: numb
+0000e7f0: 6572 206f 6620 6269 7473 2074 6f20 7175  er of bits to qu
+0000e800: 616e 7469 7a65 2074 6865 206c 6561 726e  antize the learn
+0000e810: 6564 2070 6172 616d 6574 6572 730a 2020  ed parameters.  
+0000e820: 2020 2020 2020 2020 2020 2020 2020 4465                De
+0000e830: 6661 756c 7420 746f 2038 2e0a 2020 2020  fault to 8..    
+0000e840: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000e850: 7365 6c66 2e6e 5f62 6974 733a 2055 6e69  self.n_bits: Uni
+0000e860: 6f6e 5b69 6e74 2c20 4469 6374 5b73 7472  on[int, Dict[str
+0000e870: 2c20 696e 745d 5d20 3d20 6e5f 6269 7473  , int]] = n_bits
+0000e880: 0a0a 2020 2020 2020 2020 233a 2054 6865  ..        #: The
+0000e890: 2071 7561 6e74 697a 6572 2074 6f20 7573   quantizer to us
+0000e8a0: 6520 666f 7220 7175 616e 7469 7a69 6e67  e for quantizing
+0000e8b0: 2074 6865 206d 6f64 656c 2773 2077 6569   the model's wei
+0000e8c0: 6768 7473 0a20 2020 2020 2020 2073 656c  ghts.        sel
+0000e8d0: 662e 5f77 6569 6768 745f 7175 616e 7469  f._weight_quanti
+0000e8e0: 7a65 723a 204f 7074 696f 6e61 6c5b 556e  zer: Optional[Un
+0000e8f0: 6966 6f72 6d51 7561 6e74 697a 6572 5d20  iformQuantizer] 
+0000e900: 3d20 4e6f 6e65 0a0a 2020 2020 2020 2020  = None..        
+0000e910: 233a 2054 6865 206d 6f64 656c 2773 2071  #: The model's q
+0000e920: 7561 6e74 697a 6564 2077 6569 6768 7473  uantized weights
+0000e930: 0a20 2020 2020 2020 2073 656c 662e 5f71  .        self._q
+0000e940: 5f77 6569 6768 7473 3a20 4f70 7469 6f6e  _weights: Option
+0000e950: 616c 5b6e 756d 7079 2e6e 6461 7272 6179  al[numpy.ndarray
+0000e960: 5d20 3d20 4e6f 6e65 0a0a 2020 2020 2020  ] = None..      
+0000e970: 2020 233a 2054 6865 206d 6f64 656c 2773    #: The model's
+0000e980: 2071 7561 6e74 697a 6564 2062 6961 730a   quantized bias.
+0000e990: 2020 2020 2020 2020 7365 6c66 2e5f 715f          self._q_
+0000e9a0: 6269 6173 3a20 4f70 7469 6f6e 616c 5b6e  bias: Optional[n
+0000e9b0: 756d 7079 2e6e 6461 7272 6179 5d20 3d20  umpy.ndarray] = 
+0000e9c0: 4e6f 6e65 0a0a 2020 2020 2020 2020 4261  None..        Ba
+0000e9d0: 7365 4573 7469 6d61 746f 722e 5f5f 696e  seEstimator.__in
+0000e9e0: 6974 5f5f 2873 656c 6629 0a0a 2020 2020  it__(self)..    
+0000e9f0: 4063 6c61 7373 6d65 7468 6f64 0a20 2020  @classmethod.   
+0000ea00: 2064 6566 2066 726f 6d5f 736b 6c65 6172   def from_sklear
+0000ea10: 6e5f 6d6f 6465 6c28 0a20 2020 2020 2020  n_model(.       
+0000ea20: 2063 6c73 2c0a 2020 2020 2020 2020 736b   cls,.        sk
+0000ea30: 6c65 6172 6e5f 6d6f 6465 6c3a 2073 6b6c  learn_model: skl
+0000ea40: 6561 726e 2e62 6173 652e 4261 7365 4573  earn.base.BaseEs
+0000ea50: 7469 6d61 746f 722c 0a20 2020 2020 2020  timator,.       
+0000ea60: 2058 3a20 4461 7461 2c0a 2020 2020 2020   X: Data,.      
+0000ea70: 2020 6e5f 6269 7473 3a20 556e 696f 6e5b    n_bits: Union[
+0000ea80: 696e 742c 2044 6963 745b 7374 722c 2069  int, Dict[str, i
+0000ea90: 6e74 5d5d 203d 2038 2c0a 2020 2020 293a  nt]] = 8,.    ):
+0000eaa0: 0a20 2020 2020 2020 2022 2222 4275 696c  .        """Buil
+0000eab0: 6420 6120 4648 452d 636f 6d70 6c69 616e  d a FHE-complian
+0000eac0: 7420 6d6f 6465 6c20 7573 696e 6720 6120  t model using a 
+0000ead0: 6669 7474 6564 2073 6369 6b69 742d 6c65  fitted scikit-le
+0000eae0: 6172 6e20 6d6f 6465 6c2e 0a0a 2020 2020  arn model...    
+0000eaf0: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+0000eb00: 2020 2020 2020 736b 6c65 6172 6e5f 6d6f        sklearn_mo
+0000eb10: 6465 6c20 2873 6b6c 6561 726e 2e62 6173  del (sklearn.bas
+0000eb20: 652e 4261 7365 4573 7469 6d61 746f 7229  e.BaseEstimator)
+0000eb30: 3a20 5468 6520 6669 7474 6564 2073 6369  : The fitted sci
+0000eb40: 6b69 742d 6c65 6172 6e20 6d6f 6465 6c20  kit-learn model 
+0000eb50: 746f 2063 6f6e 7665 7274 2e0a 2020 2020  to convert..    
+0000eb60: 2020 2020 2020 2020 5820 2844 6174 6129          X (Data)
+0000eb70: 3a20 4120 7265 7072 6573 656e 7461 7469  : A representati
+0000eb80: 7665 2073 6574 206f 6620 696e 7075 7420  ve set of input 
+0000eb90: 7661 6c75 6573 2075 7365 6420 666f 7220  values used for 
+0000eba0: 636f 6d70 7574 696e 6720 7175 616e 7469  computing quanti
+0000ebb0: 7a61 7469 6f6e 0a20 2020 2020 2020 2020  zation.         
+0000ebc0: 2020 2020 2020 2070 6172 616d 6574 6572         parameter
+0000ebd0: 732c 2061 7320 6120 4e75 6d70 7920 6172  s, as a Numpy ar
+0000ebe0: 7261 792c 2054 6f72 6368 2074 656e 736f  ray, Torch tenso
+0000ebf0: 722c 2050 616e 6461 7320 4461 7461 4672  r, Pandas DataFr
+0000ec00: 616d 6520 6f72 204c 6973 742e 2054 6869  ame or List. Thi
+0000ec10: 7320 6973 0a20 2020 2020 2020 2020 2020  s is.           
+0000ec20: 2020 2020 2075 7375 616c 6c79 2074 6865       usually the
+0000ec30: 2074 7261 696e 696e 6720 6461 7461 2d73   training data-s
+0000ec40: 6574 206f 7220 6120 7375 622d 7365 7420  et or a sub-set 
+0000ec50: 6f66 2069 742e 0a20 2020 2020 2020 2020  of it..         
+0000ec60: 2020 206e 5f62 6974 7320 2869 6e74 2c20     n_bits (int, 
+0000ec70: 4469 6374 5b73 7472 2c20 696e 745d 293a  Dict[str, int]):
+0000ec80: 204e 756d 6265 7220 6f66 2062 6974 7320   Number of bits 
+0000ec90: 746f 2071 7561 6e74 697a 6520 7468 6520  to quantize the 
+0000eca0: 6d6f 6465 6c2e 2049 6620 616e 2069 6e74  model. If an int
+0000ecb0: 2069 7320 7061 7373 6564 0a20 2020 2020   is passed.     
+0000ecc0: 2020 2020 2020 2020 2020 2066 6f72 206e             for n
+0000ecd0: 5f62 6974 732c 2074 6865 2076 616c 7565  _bits, the value
+0000ece0: 2077 696c 6c20 6265 2075 7365 6420 666f   will be used fo
+0000ecf0: 7220 7175 616e 7469 7a69 6e67 2069 6e70  r quantizing inp
+0000ed00: 7574 7320 616e 6420 7765 6967 6874 732e  uts and weights.
+0000ed10: 2049 6620 6120 6469 6374 2069 730a 2020   If a dict is.  
+0000ed20: 2020 2020 2020 2020 2020 2020 2020 7061                pa
+0000ed30: 7373 6564 2c20 7468 656e 2069 7420 7368  ssed, then it sh
+0000ed40: 6f75 6c64 2063 6f6e 7461 696e 2022 6f70  ould contain "op
+0000ed50: 5f69 6e70 7574 7322 2061 6e64 2022 6f70  _inputs" and "op
+0000ed60: 5f77 6569 6768 7473 2220 6173 206b 6579  _weights" as key
+0000ed70: 7320 7769 7468 0a20 2020 2020 2020 2020  s with.         
+0000ed80: 2020 2020 2020 2063 6f72 7265 7370 6f6e         correspon
+0000ed90: 6469 6e67 206e 756d 6265 7220 6f66 2071  ding number of q
+0000eda0: 7561 6e74 697a 6174 696f 6e20 6269 7473  uantization bits
+0000edb0: 2073 6f20 7468 6174 3a0a 2020 2020 2020   so that:.      
+0000edc0: 2020 2020 2020 2020 2020 2d20 6f70 5f69            - op_i
+0000edd0: 6e70 7574 7320 3a20 6e75 6d62 6572 206f  nputs : number o
+0000ede0: 6620 6269 7473 2074 6f20 7175 616e 7469  f bits to quanti
+0000edf0: 7a65 2074 6865 2069 6e70 7574 2076 616c  ze the input val
+0000ee00: 7565 730a 2020 2020 2020 2020 2020 2020  ues.            
+0000ee10: 2020 2020 2d20 6f70 5f77 6569 6768 7473      - op_weights
+0000ee20: 3a20 6e75 6d62 6572 206f 6620 6269 7473  : number of bits
+0000ee30: 2074 6f20 7175 616e 7469 7a65 2074 6865   to quantize the
+0000ee40: 206c 6561 726e 6564 2070 6172 616d 6574   learned paramet
+0000ee50: 6572 730a 2020 2020 2020 2020 2020 2020  ers.            
+0000ee60: 2020 2020 4465 6661 756c 7420 746f 2038      Default to 8
+0000ee70: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+0000ee80: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+0000ee90: 5468 6520 4648 452d 636f 6d70 6c69 616e  The FHE-complian
+0000eea0: 7420 6669 7474 6564 206d 6f64 656c 2e0a  t fitted model..
+0000eeb0: 2020 2020 2020 2020 2222 220a 0a20 2020          """..   
+0000eec0: 2020 2020 2023 2043 6865 636b 2074 6861       # Check tha
+0000eed0: 7420 736b 6c65 6172 6e5f 6d6f 6465 6c20  t sklearn_model 
+0000eee0: 6973 2061 2070 726f 7065 7220 6669 7474  is a proper fitt
+0000eef0: 6564 2073 6369 6b69 742d 6c65 6172 6e20  ed scikit-learn 
+0000ef00: 6d6f 6465 6c0a 2020 2020 2020 2020 6368  model.        ch
+0000ef10: 6563 6b5f 6973 5f66 6974 7465 6428 736b  eck_is_fitted(sk
+0000ef20: 6c65 6172 6e5f 6d6f 6465 6c29 0a0a 2020  learn_model)..  
+0000ef30: 2020 2020 2020 2320 4578 7472 6163 7420        # Extract 
+0000ef40: 7363 696b 6974 2d6c 6561 726e 2773 2069  scikit-learn's i
+0000ef50: 6e69 7469 616c 697a 6174 696f 6e20 7061  nitialization pa
+0000ef60: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+0000ef70: 2069 6e69 745f 7061 7261 6d73 203d 2073   init_params = s
+0000ef80: 6b6c 6561 726e 5f6d 6f64 656c 2e67 6574  klearn_model.get
+0000ef90: 5f70 6172 616d 7328 290a 0a20 2020 2020  _params()..     
+0000efa0: 2020 2023 2049 6e73 7461 6e74 6961 7465     # Instantiate
+0000efb0: 2074 6865 2043 6f6e 6372 6574 6520 4d4c   the Concrete ML
+0000efc0: 206d 6f64 656c 2061 6e64 2075 7064 6174   model and updat
+0000efd0: 6520 696e 6974 6961 6c69 7a61 7469 6f6e  e initialization
+0000efe0: 2070 6172 616d 6574 6572 730a 2020 2020   parameters.    
+0000eff0: 2020 2020 2320 5468 6973 2075 7064 6174      # This updat
+0000f000: 6520 6973 206e 6563 6573 7361 7279 2061  e is necessary a
+0000f010: 7320 7765 2063 7572 7265 6e74 6c79 2073  s we currently s
+0000f020: 746f 7265 2073 6369 6b69 742d 6c65 6172  tore scikit-lear
+0000f030: 6e20 6174 7472 6962 7574 6573 2069 6e20  n attributes in 
+0000f040: 436f 6e63 7265 7465 204d 4c0a 2020 2020  Concrete ML.    
+0000f050: 2020 2020 2320 636c 6173 7365 7320 6475      # classes du
+0000f060: 7269 6e67 2069 6e69 7469 616c 697a 6174  ring initializat
+0000f070: 696f 6e20 2866 6f72 2065 7861 6d70 6c65  ion (for example
+0000f080: 3a20 6c69 6e6b 206f 7220 706f 7765 7220  : link or power 
+0000f090: 6174 7472 6962 7574 6573 2069 6e20 474c  attributes in GL
+0000f0a0: 4d73 290a 2020 2020 2020 2020 2320 5769  Ms).        # Wi
+0000f0b0: 7468 6f75 7420 6974 2c20 7468 6573 6520  thout it, these 
+0000f0c0: 6174 7472 6962 7574 6573 2077 696c 6c20  attributes will 
+0000f0d0: 6861 7665 2064 6566 6175 6c74 2076 616c  have default val
+0000f0e0: 7565 7320 696e 7374 6561 6420 6f66 2074  ues instead of t
+0000f0f0: 6865 206f 6e65 7320 7573 6564 2062 7920  he ones used by 
+0000f100: 7468 650a 2020 2020 2020 2020 2320 7363  the.        # sc
+0000f110: 696b 6974 2d6c 6561 726e 206d 6f64 656c  ikit-learn model
+0000f120: 730a 2020 2020 2020 2020 2320 5468 6973  s.        # This
+0000f130: 2073 686f 756c 6420 6265 2066 6978 6564   should be fixed
+0000f140: 206f 6e63 6520 436f 6e63 7265 7465 204d   once Concrete M
+0000f150: 4c20 6d6f 6465 6c73 2069 6e69 7469 616c  L models initial
+0000f160: 697a 6520 7468 6569 7220 756e 6465 726c  ize their underl
+0000f170: 7969 6e67 2073 6369 6b69 742d 6c65 6172  ying scikit-lear
+0000f180: 6e0a 2020 2020 2020 2020 2320 6d6f 6465  n.        # mode
+0000f190: 6c73 2064 7572 696e 6720 696e 6974 6961  ls during initia
+0000f1a0: 6c69 7a61 7469 6f6e 0a20 2020 2020 2020  lization.       
+0000f1b0: 2023 2046 4958 4d45 3a20 6874 7470 733a   # FIXME: https:
+0000f1c0: 2f2f 6769 7468 7562 2e63 6f6d 2f7a 616d  //github.com/zam
+0000f1d0: 612d 6169 2f63 6f6e 6372 6574 652d 6d6c  a-ai/concrete-ml
+0000f1e0: 2d69 6e74 6572 6e61 6c2f 6973 7375 6573  -internal/issues
+0000f1f0: 2f33 3337 330a 2020 2020 2020 2020 6d6f  /3373.        mo
+0000f200: 6465 6c20 3d20 636c 7328 6e5f 6269 7473  del = cls(n_bits
+0000f210: 3d6e 5f62 6974 732c 202a 2a69 6e69 745f  =n_bits, **init_
+0000f220: 7061 7261 6d73 290a 0a20 2020 2020 2020  params)..       
+0000f230: 2023 2055 7064 6174 6520 7468 6520 756e   # Update the un
+0000f240: 6465 726c 7969 6e67 2073 6369 6b69 742d  derlying scikit-
+0000f250: 6c65 6172 6e20 6d6f 6465 6c20 7769 7468  learn model with
+0000f260: 2074 6865 2067 6976 656e 2066 6974 7465   the given fitte
+0000f270: 6420 6f6e 650a 2020 2020 2020 2020 6d6f  d one.        mo
+0000f280: 6465 6c2e 736b 6c65 6172 6e5f 6d6f 6465  del.sklearn_mode
+0000f290: 6c20 3d20 636f 7079 2e64 6565 7063 6f70  l = copy.deepcop
+0000f2a0: 7928 736b 6c65 6172 6e5f 6d6f 6465 6c29  y(sklearn_model)
+0000f2b0: 0a0a 2020 2020 2020 2020 2320 436f 6d70  ..        # Comp
+0000f2c0: 7574 6520 7468 6520 7175 616e 7469 7a61  ute the quantiza
+0000f2d0: 7469 6f6e 2070 6172 616d 6574 6572 730a  tion parameters.
+0000f2e0: 2020 2020 2020 2020 7265 7475 726e 206d          return m
+0000f2f0: 6f64 656c 2e5f 7175 616e 7469 7a65 5f6d  odel._quantize_m
+0000f300: 6f64 656c 2858 290a 0a20 2020 2064 6566  odel(X)..    def
+0000f310: 205f 7365 745f 6f6e 6e78 5f6d 6f64 656c   _set_onnx_model
+0000f320: 2873 656c 662c 2074 6573 745f 696e 7075  (self, test_inpu
+0000f330: 743a 206e 756d 7079 2e6e 6461 7272 6179  t: numpy.ndarray
+0000f340: 2920 2d3e 204e 6f6e 653a 0a20 2020 2020  ) -> None:.     
+0000f350: 2020 2022 2222 5265 7472 6965 7665 2074     """Retrieve t
+0000f360: 6865 206d 6f64 656c 2773 204f 4e4e 5820  he model's ONNX 
+0000f370: 6772 6170 6820 7573 696e 6720 4875 6d6d  graph using Humm
+0000f380: 696e 6762 6972 6420 636f 6e76 6572 7369  ingbird conversi
+0000f390: 6f6e 2e0a 0a20 2020 2020 2020 2041 7267  on...        Arg
+0000f3a0: 733a 0a20 2020 2020 2020 2020 2020 2074  s:.            t
+0000f3b0: 6573 745f 696e 7075 7420 286e 756d 7079  est_input (numpy
+0000f3c0: 2e6e 6461 7272 6179 293a 2041 6e20 696e  .ndarray): An in
+0000f3d0: 7075 7420 6461 7461 2075 7365 6420 746f  put data used to
+0000f3e0: 2074 7261 6365 2074 6865 206d 6f64 656c   trace the model
+0000f3f0: 2065 7865 6375 7469 6f6e 2e0a 2020 2020   execution..    
+0000f400: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000f410: 2320 4368 6563 6b20 7468 6174 2074 6865  # Check that the
+0000f420: 2075 6e64 6572 6c79 696e 6720 736b 6c65   underlying skle
+0000f430: 6172 6e20 6d6f 6465 6c20 6861 7320 6265  arn model has be
+0000f440: 656e 2073 6574 2061 6e64 2066 6974 0a20  en set and fit. 
+0000f450: 2020 2020 2020 2061 7373 6572 7420 7365         assert se
+0000f460: 6c66 2e73 6b6c 6561 726e 5f6d 6f64 656c  lf.sklearn_model
+0000f470: 2069 7320 6e6f 7420 4e6f 6e65 2c20 7365   is not None, se
+0000f480: 6c66 2e5f 736b 6c65 6172 6e5f 6d6f 6465  lf._sklearn_mode
+0000f490: 6c5f 6973 5f6e 6f74 5f66 6974 7465 645f  l_is_not_fitted_
+0000f4a0: 6572 726f 725f 6d65 7373 6167 6528 290a  error_message().
+0000f4b0: 0a20 2020 2020 2020 2073 656c 662e 6f6e  .        self.on
+0000f4c0: 6e78 5f6d 6f64 656c 5f20 3d20 6862 5f63  nx_model_ = hb_c
+0000f4d0: 6f6e 7665 7274 280a 2020 2020 2020 2020  onvert(.        
+0000f4e0: 2020 2020 7365 6c66 2e73 6b6c 6561 726e      self.sklearn
+0000f4f0: 5f6d 6f64 656c 2c0a 2020 2020 2020 2020  _model,.        
+0000f500: 2020 2020 6261 636b 656e 643d 226f 6e6e      backend="onn
+0000f510: 7822 2c0a 2020 2020 2020 2020 2020 2020  x",.            
+0000f520: 7465 7374 5f69 6e70 7574 3d74 6573 745f  test_input=test_
+0000f530: 696e 7075 742c 0a20 2020 2020 2020 2020  input,.         
+0000f540: 2020 2065 7874 7261 5f63 6f6e 6669 673d     extra_config=
+0000f550: 7b22 6f6e 6e78 5f74 6172 6765 745f 6f70  {"onnx_target_op
+0000f560: 7365 7422 3a20 4f50 5345 545f 5645 5253  set": OPSET_VERS
+0000f570: 494f 4e5f 464f 525f 4f4e 4e58 5f45 5850  ION_FOR_ONNX_EXP
+0000f580: 4f52 547d 2c0a 2020 2020 2020 2020 292e  ORT},.        ).
+0000f590: 6d6f 6465 6c0a 0a20 2020 2020 2020 2073  model..        s
+0000f5a0: 656c 662e 5f63 6c65 616e 5f67 7261 7068  elf._clean_graph
+0000f5b0: 2829 0a0a 2020 2020 6465 6620 5f63 6c65  ()..    def _cle
+0000f5c0: 616e 5f67 7261 7068 2873 656c 6629 202d  an_graph(self) -
+0000f5d0: 3e20 4e6f 6e65 3a0a 2020 2020 2020 2020  > None:.        
+0000f5e0: 2222 2243 6c65 616e 2074 6865 204f 4e4e  """Clean the ONN
+0000f5f0: 5820 6772 6170 6820 6672 6f6d 2075 6e64  X graph from und
+0000f600: 6573 6972 6564 206e 6f64 6573 2e22 2222  esired nodes."""
+0000f610: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+0000f620: 7365 6c66 2e6f 6e6e 785f 6d6f 6465 6c5f  self.onnx_model_
+0000f630: 2069 7320 6e6f 7420 4e6f 6e65 2c20 7365   is not None, se
+0000f640: 6c66 2e5f 6973 5f6e 6f74 5f66 6974 7465  lf._is_not_fitte
+0000f650: 645f 6572 726f 725f 6d65 7373 6167 6528  d_error_message(
+0000f660: 290a 0a20 2020 2020 2020 2023 2052 656d  )..        # Rem
+0000f670: 6f76 6520 6361 7374 206f 7065 7261 746f  ove cast operato
+0000f680: 7273 2061 7320 7468 6579 2061 7265 206e  rs as they are n
+0000f690: 6f74 206e 6565 6465 640a 2020 2020 2020  ot needed.      
+0000f6a0: 2020 7265 6d6f 7665 5f6e 6f64 655f 7479    remove_node_ty
+0000f6b0: 7065 7328 6f6e 6e78 5f6d 6f64 656c 3d73  pes(onnx_model=s
+0000f6c0: 656c 662e 6f6e 6e78 5f6d 6f64 656c 5f2c  elf.onnx_model_,
+0000f6d0: 206f 705f 7479 7065 735f 746f 5f72 656d   op_types_to_rem
+0000f6e0: 6f76 653d 5b22 4361 7374 225d 290a 0a20  ove=["Cast"]).. 
+0000f6f0: 2020 2064 6566 2066 6974 2873 656c 662c     def fit(self,
+0000f700: 2058 3a20 4461 7461 2c20 793a 2054 6172   X: Data, y: Tar
+0000f710: 6765 742c 202a 2a66 6974 5f70 6172 616d  get, **fit_param
+0000f720: 6574 6572 7329 3a0a 2020 2020 2020 2020  eters):.        
+0000f730: 2320 5265 7365 7420 666f 7220 646f 7562  # Reset for doub
+0000f740: 6c65 2066 6974 0a20 2020 2020 2020 2073  le fit.        s
+0000f750: 656c 662e 5f69 735f 6669 7474 6564 203d  elf._is_fitted =
+0000f760: 2046 616c 7365 0a20 2020 2020 2020 2073   False.        s
+0000f770: 656c 662e 696e 7075 745f 7175 616e 7469  elf.input_quanti
+0000f780: 7a65 7273 203d 205b 5d0a 2020 2020 2020  zers = [].      
+0000f790: 2020 7365 6c66 2e6f 7574 7075 745f 7175    self.output_qu
+0000f7a0: 616e 7469 7a65 7273 203d 205b 5d0a 0a20  antizers = [].. 
+0000f7b0: 2020 2020 2020 2023 204c 696e 6561 7252         # LinearR
+0000f7c0: 6567 7265 7373 696f 6e20 6861 6e64 6c65  egression handle
+0000f7d0: 7320 6d75 6c74 692d 6c61 6265 6c73 2064  s multi-labels d
+0000f7e0: 6174 610a 2020 2020 2020 2020 582c 2079  ata.        X, y
+0000f7f0: 203d 2063 6865 636b 5f58 5f79 5f61 6e64   = check_X_y_and
+0000f800: 5f61 7373 6572 745f 6d75 6c74 695f 6f75  _assert_multi_ou
+0000f810: 7470 7574 2858 2c20 7929 0a0a 2020 2020  tput(X, y)..    
+0000f820: 2020 2020 2320 4669 7420 7468 6520 7363      # Fit the sc
+0000f830: 696b 6974 2d6c 6561 726e 206d 6f64 656c  ikit-learn model
+0000f840: 0a20 2020 2020 2020 2073 656c 662e 5f66  .        self._f
+0000f850: 6974 5f73 6b6c 6561 726e 5f6d 6f64 656c  it_sklearn_model
+0000f860: 2858 2c20 792c 202a 2a66 6974 5f70 6172  (X, y, **fit_par
+0000f870: 616d 6574 6572 7329 0a0a 2020 2020 2020  ameters)..      
+0000f880: 2020 2320 436f 6d70 7574 6520 7468 6520    # Compute the 
+0000f890: 7175 616e 7469 7a61 7469 6f6e 2070 6172  quantization par
+0000f8a0: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+0000f8b0: 7265 7475 726e 2073 656c 662e 5f71 7561  return self._qua
+0000f8c0: 6e74 697a 655f 6d6f 6465 6c28 5829 0a0a  ntize_model(X)..
+0000f8d0: 2020 2020 6465 6620 5f71 7561 6e74 697a      def _quantiz
+0000f8e0: 655f 6d6f 6465 6c28 7365 6c66 2c20 5829  e_model(self, X)
+0000f8f0: 3a0a 2020 2020 2020 2020 2222 2243 6f6d  :.        """Com
+0000f900: 7075 7465 2071 7561 6e74 697a 6174 696f  pute quantizatio
+0000f910: 6e20 7061 7261 6d65 7465 7273 2e0a 0a20  n parameters... 
+0000f920: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+0000f930: 2020 2020 2020 2020 2058 2028 4461 7461           X (Data
+0000f940: 293a 2041 2072 6570 7265 7365 6e74 6174  ): A representat
+0000f950: 6976 6520 7365 7420 6f66 2069 6e70 7574  ive set of input
+0000f960: 2076 616c 7565 7320 7573 6564 2066 6f72   values used for
+0000f970: 2063 6f6d 7075 7469 6e67 2071 7561 6e74   computing quant
+0000f980: 697a 6174 696f 6e0a 2020 2020 2020 2020  ization.        
+0000f990: 2020 2020 2020 2020 7061 7261 6d65 7465          paramete
+0000f9a0: 7273 2c20 6173 2061 204e 756d 7079 2061  rs, as a Numpy a
+0000f9b0: 7272 6179 2c20 546f 7263 6820 7465 6e73  rray, Torch tens
+0000f9c0: 6f72 2c20 5061 6e64 6173 2044 6174 6146  or, Pandas DataF
+0000f9d0: 7261 6d65 206f 7220 4c69 7374 2e20 5468  rame or List. Th
+0000f9e0: 6973 2069 730a 2020 2020 2020 2020 2020  is is.          
+0000f9f0: 2020 2020 2020 7573 7561 6c6c 7920 7468        usually th
+0000fa00: 6520 7472 6169 6e69 6e67 2064 6174 612d  e training data-
+0000fa10: 7365 7420 6f72 2061 2073 7562 2d73 6574  set or a sub-set
+0000fa20: 206f 6620 6974 2e0a 0a20 2020 2020 2020   of it...       
+0000fa30: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
+0000fa40: 2020 2020 2020 5468 6520 4648 452d 636f        The FHE-co
+0000fa50: 6d70 6c69 616e 7420 6669 7474 6564 206d  mpliant fitted m
+0000fa60: 6f64 656c 2e0a 2020 2020 2020 2020 2222  odel..        ""
+0000fa70: 220a 2020 2020 2020 2020 2320 4368 6563  ".        # Chec
+0000fa80: 6b20 7468 6174 2074 6865 2075 6e64 6572  k that the under
+0000fa90: 6c79 696e 6720 736b 6c65 6172 6e20 6d6f  lying sklearn mo
+0000faa0: 6465 6c20 6861 7320 6265 656e 2073 6574  del has been set
+0000fab0: 2061 6e64 2066 6974 0a20 2020 2020 2020   and fit.       
+0000fac0: 2061 7373 6572 7420 7365 6c66 2e73 6b6c   assert self.skl
+0000fad0: 6561 726e 5f6d 6f64 656c 2069 7320 6e6f  earn_model is no
+0000fae0: 7420 4e6f 6e65 2c20 7365 6c66 2e5f 736b  t None, self._sk
+0000faf0: 6c65 6172 6e5f 6d6f 6465 6c5f 6973 5f6e  learn_model_is_n
+0000fb00: 6f74 5f66 6974 7465 645f 6572 726f 725f  ot_fitted_error_
+0000fb10: 6d65 7373 6167 6528 290a 0a20 2020 2020  message()..     
+0000fb20: 2020 2023 2052 6574 7269 6576 6520 7468     # Retrieve th
+0000fb30: 6520 4f4e 4e58 2067 7261 7068 0a20 2020  e ONNX graph.   
+0000fb40: 2020 2020 2073 656c 662e 5f73 6574 5f6f       self._set_o
+0000fb50: 6e6e 785f 6d6f 6465 6c28 5829 0a0a 2020  nnx_model(X)..  
+0000fb60: 2020 2020 2020 2320 436f 6e76 6572 7420        # Convert 
+0000fb70: 7468 6520 6e5f 6269 7473 2061 7474 7269  the n_bits attri
+0000fb80: 6275 7465 2069 6e74 6f20 6120 7072 6f70  bute into a prop
+0000fb90: 6572 2064 6963 7469 6f6e 6172 790a 2020  er dictionary.  
+0000fba0: 2020 2020 2020 6e5f 6269 7473 203d 2067        n_bits = g
+0000fbb0: 6574 5f6e 5f62 6974 735f 6469 6374 2873  et_n_bits_dict(s
+0000fbc0: 656c 662e 6e5f 6269 7473 290a 0a20 2020  elf.n_bits)..   
+0000fbd0: 2020 2020 2069 6e70 7574 5f6e 5f62 6974       input_n_bit
+0000fbe0: 7320 3d20 6e5f 6269 7473 5b22 6f70 5f69  s = n_bits["op_i
+0000fbf0: 6e70 7574 7322 5d0a 2020 2020 2020 2020  nputs"].        
+0000fc00: 696e 7075 745f 6f70 7469 6f6e 7320 3d20  input_options = 
+0000fc10: 5175 616e 7469 7a61 7469 6f6e 4f70 7469  QuantizationOpti
+0000fc20: 6f6e 7328 6e5f 6269 7473 3d69 6e70 7574  ons(n_bits=input
+0000fc30: 5f6e 5f62 6974 732c 2069 735f 7369 676e  _n_bits, is_sign
+0000fc40: 6564 3d54 7275 6529 0a0a 2020 2020 2020  ed=True)..      
+0000fc50: 2020 2320 5175 616e 7469 7a65 2074 6865    # Quantize the
+0000fc60: 2069 6e70 7574 7320 616e 6420 7374 6f72   inputs and stor
+0000fc70: 6520 7468 6520 6173 736f 6369 6174 6564  e the associated
+0000fc80: 2071 7561 6e74 697a 6572 0a20 2020 2020   quantizer.     
+0000fc90: 2020 2071 5f69 6e70 7574 7320 3d20 5175     q_inputs = Qu
+0000fca0: 616e 7469 7a65 6441 7272 6179 286e 5f62  antizedArray(n_b
+0000fcb0: 6974 733d 696e 7075 745f 6e5f 6269 7473  its=input_n_bits
+0000fcc0: 2c20 7661 6c75 6573 3d58 2c20 6f70 7469  , values=X, opti
+0000fcd0: 6f6e 733d 696e 7075 745f 6f70 7469 6f6e  ons=input_option
+0000fce0: 7329 0a20 2020 2020 2020 2069 6e70 7574  s).        input
+0000fcf0: 5f71 7561 6e74 697a 6572 203d 2071 5f69  _quantizer = q_i
+0000fd00: 6e70 7574 732e 7175 616e 7469 7a65 720a  nputs.quantizer.
+0000fd10: 2020 2020 2020 2020 7365 6c66 2e69 6e70          self.inp
+0000fd20: 7574 5f71 7561 6e74 697a 6572 7320 3d20  ut_quantizers = 
+0000fd30: 5b69 6e70 7574 5f71 7561 6e74 697a 6572  [input_quantizer
+0000fd40: 5d0a 0a20 2020 2020 2020 2077 6569 6768  ]..        weigh
+0000fd50: 7473 5f6e 5f62 6974 7320 3d20 6e5f 6269  ts_n_bits = n_bi
+0000fd60: 7473 5b22 6f70 5f77 6569 6768 7473 225d  ts["op_weights"]
+0000fd70: 0a20 2020 2020 2020 2077 6569 6768 745f  .        weight_
+0000fd80: 6f70 7469 6f6e 7320 3d20 5175 616e 7469  options = Quanti
+0000fd90: 7a61 7469 6f6e 4f70 7469 6f6e 7328 6e5f  zationOptions(n_
+0000fda0: 6269 7473 3d77 6569 6768 7473 5f6e 5f62  bits=weights_n_b
+0000fdb0: 6974 732c 2069 735f 7369 676e 6564 3d54  its, is_signed=T
+0000fdc0: 7275 6529 0a0a 2020 2020 2020 2020 2320  rue)..        # 
+0000fdd0: 5175 616e 7469 7a65 2074 6865 2077 6569  Quantize the wei
+0000fde0: 6768 7473 2061 6e64 2073 746f 7265 2074  ghts and store t
+0000fdf0: 6865 2061 7373 6f63 6961 7465 6420 7175  he associated qu
+0000fe00: 616e 7469 7a65 720a 2020 2020 2020 2020  antizer.        
+0000fe10: 2320 5472 616e 7370 6f73 6520 616e 6420  # Transpose and 
+0000fe20: 6578 7061 6e64 2061 7265 206e 6563 6573  expand are neces
+0000fe30: 7361 7279 2069 6e20 6f72 6465 7220 746f  sary in order to
+0000fe40: 206d 616b 6520 7375 7265 2074 6865 2077   make sure the w
+0000fe50: 6569 6768 7420 6172 7261 7920 6861 7320  eight array has 
+0000fe60: 7468 6520 636f 7272 6563 740a 2020 2020  the correct.    
+0000fe70: 2020 2020 2320 7368 6170 6520 7768 656e      # shape when
+0000fe80: 2063 616c 6c69 6e67 2074 6865 2047 656d   calling the Gem
+0000fe90: 6d20 6f70 6572 6174 6f72 206f 6e20 6974  m operator on it
+0000fea0: 0a20 2020 2020 2020 2077 6569 6768 7473  .        weights
+0000feb0: 203d 2073 656c 662e 736b 6c65 6172 6e5f   = self.sklearn_
+0000fec0: 6d6f 6465 6c2e 636f 6566 5f2e 540a 2020  model.coef_.T.  
+0000fed0: 2020 2020 2020 715f 7765 6967 6874 7320        q_weights 
+0000fee0: 3d20 5175 616e 7469 7a65 6441 7272 6179  = QuantizedArray
+0000fef0: 280a 2020 2020 2020 2020 2020 2020 6e5f  (.            n_
+0000ff00: 6269 7473 3d6e 5f62 6974 735b 226f 705f  bits=n_bits["op_
+0000ff10: 7765 6967 6874 7322 5d2c 0a20 2020 2020  weights"],.     
+0000ff20: 2020 2020 2020 2076 616c 7565 733d 6e75         values=nu
+0000ff30: 6d70 792e 6578 7061 6e64 5f64 696d 7328  mpy.expand_dims(
+0000ff40: 7765 6967 6874 732c 2061 7869 733d 3129  weights, axis=1)
+0000ff50: 2069 6620 6c65 6e28 7765 6967 6874 732e   if len(weights.
+0000ff60: 7368 6170 6529 203d 3d20 3120 656c 7365  shape) == 1 else
+0000ff70: 2077 6569 6768 7473 2c0a 2020 2020 2020   weights,.      
+0000ff80: 2020 2020 2020 6f70 7469 6f6e 733d 7765        options=we
+0000ff90: 6967 6874 5f6f 7074 696f 6e73 2c0a 2020  ight_options,.  
+0000ffa0: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
+0000ffb0: 7365 6c66 2e5f 715f 7765 6967 6874 7320  self._q_weights 
+0000ffc0: 3d20 715f 7765 6967 6874 732e 7176 616c  = q_weights.qval
+0000ffd0: 7565 730a 2020 2020 2020 2020 7765 6967  ues.        weig
+0000ffe0: 6874 5f71 7561 6e74 697a 6572 203d 2071  ht_quantizer = q
+0000fff0: 5f77 6569 6768 7473 2e71 7561 6e74 697a  _weights.quantiz
+00010000: 6572 0a20 2020 2020 2020 2073 656c 662e  er.        self.
+00010010: 5f77 6569 6768 745f 7175 616e 7469 7a65  _weight_quantize
+00010020: 7220 3d20 7765 6967 6874 5f71 7561 6e74  r = weight_quant
+00010030: 697a 6572 0a0a 2020 2020 2020 2020 2320  izer..        # 
+00010040: 6d79 7079 0a20 2020 2020 2020 2061 7373  mypy.        ass
+00010050: 6572 7420 696e 7075 745f 7175 616e 7469  ert input_quanti
+00010060: 7a65 722e 7363 616c 6520 6973 206e 6f74  zer.scale is not
+00010070: 204e 6f6e 650a 2020 2020 2020 2020 6173   None.        as
+00010080: 7365 7274 2077 6569 6768 745f 7175 616e  sert weight_quan
+00010090: 7469 7a65 722e 7363 616c 6520 6973 206e  tizer.scale is n
+000100a0: 6f74 204e 6f6e 650a 0a20 2020 2020 2020  ot None..       
+000100b0: 2023 2043 6f6d 7075 7465 2074 6865 2073   # Compute the s
+000100c0: 6361 6c65 2061 6e64 207a 6572 6f2d 706f  cale and zero-po
+000100d0: 696e 7420 6f66 2074 6865 206d 6174 6d75  int of the matmu
+000100e0: 6c27 7320 6f75 7470 7574 732c 2066 6f6c  l's outputs, fol
+000100f0: 6c6f 7769 6e67 2074 6865 2073 616d 6520  lowing the same 
+00010100: 7374 6570 7320 6672 6f6d 0a20 2020 2020  steps from.     
+00010110: 2020 2023 2074 6865 2051 7561 6e74 697a     # the Quantiz
+00010120: 6564 4765 6d6d 206f 7065 7261 746f 722c  edGemm operator,
+00010130: 2077 6869 6368 2061 7265 2062 6173 6564   which are based
+00010140: 206f 6e20 6571 7561 7469 6f6e 7320 6465   on equations de
+00010150: 7461 696c 6564 2069 6e0a 2020 2020 2020  tailed in.      
+00010160: 2020 2320 6874 7470 733a 2f2f 6172 7869    # https://arxi
+00010170: 762e 6f72 672f 6162 732f 3137 3132 2e30  v.org/abs/1712.0
+00010180: 3538 3737 0a20 2020 2020 2020 206f 7574  5877.        out
+00010190: 7075 745f 7175 616e 745f 7061 7261 6d73  put_quant_params
+000101a0: 203d 2055 6e69 666f 726d 5175 616e 7469   = UniformQuanti
+000101b0: 7a61 7469 6f6e 5061 7261 6d65 7465 7273  zationParameters
+000101c0: 280a 2020 2020 2020 2020 2020 2020 7363  (.            sc
+000101d0: 616c 653d 696e 7075 745f 7175 616e 7469  ale=input_quanti
+000101e0: 7a65 722e 7363 616c 6520 2a20 7765 6967  zer.scale * weig
+000101f0: 6874 5f71 7561 6e74 697a 6572 2e73 6361  ht_quantizer.sca
+00010200: 6c65 2c0a 2020 2020 2020 2020 2020 2020  le,.            
+00010210: 7a65 726f 5f70 6f69 6e74 3d69 6e70 7574  zero_point=input
+00010220: 5f71 7561 6e74 697a 6572 2e7a 6572 6f5f  _quantizer.zero_
+00010230: 706f 696e 740a 2020 2020 2020 2020 2020  point.          
+00010240: 2020 2a20 280a 2020 2020 2020 2020 2020    * (.          
+00010250: 2020 2020 2020 6e75 6d70 792e 7375 6d28        numpy.sum(
+00010260: 7365 6c66 2e5f 715f 7765 6967 6874 732c  self._q_weights,
+00010270: 2061 7869 733d 302c 206b 6565 7064 696d   axis=0, keepdim
+00010280: 733d 5472 7565 290a 2020 2020 2020 2020  s=True).        
+00010290: 2020 2020 2020 2020 2d20 582e 7368 6170          - X.shap
+000102a0: 655b 315d 202a 2077 6569 6768 745f 7175  e[1] * weight_qu
+000102b0: 616e 7469 7a65 722e 7a65 726f 5f70 6f69  antizer.zero_poi
+000102c0: 6e74 0a20 2020 2020 2020 2020 2020 2029  nt.            )
+000102d0: 2c0a 2020 2020 2020 2020 2020 2020 6f66  ,.            of
+000102e0: 6673 6574 3d30 2c0a 2020 2020 2020 2020  fset=0,.        
+000102f0: 290a 0a20 2020 2020 2020 206f 7574 7075  )..        outpu
+00010300: 745f 7175 616e 7469 7a65 7220 3d20 556e  t_quantizer = Un
+00010310: 6966 6f72 6d51 7561 6e74 697a 6572 2870  iformQuantizer(p
+00010320: 6172 616d 733d 6f75 7470 7574 5f71 7561  arams=output_qua
+00010330: 6e74 5f70 6172 616d 732c 206e 6f5f 636c  nt_params, no_cl
+00010340: 6970 7069 6e67 3d54 7275 6529 0a0a 2020  ipping=True)..  
+00010350: 2020 2020 2020 2320 5175 616e 7469 7a65        # Quantize
+00010360: 2074 6865 2062 6961 7320 7573 696e 6720   the bias using 
+00010370: 7468 6520 6d61 746d 756c 2773 2073 6361  the matmul's sca
+00010380: 6c65 2061 6e64 207a 6572 6f2d 706f 696e  le and zero-poin
+00010390: 742c 2073 7563 6820 7468 6174 0a20 2020  t, such that.   
+000103a0: 2020 2020 2023 2071 5f62 6961 7320 3d20       # q_bias = 
+000103b0: 726f 756e 6428 2831 2f53 292a 6269 6173  round((1/S)*bias
+000103c0: 202b 205a 290a 2020 2020 2020 2020 7365   + Z).        se
+000103d0: 6c66 2e5f 715f 6269 6173 203d 206f 7574  lf._q_bias = out
+000103e0: 7075 745f 7175 616e 7469 7a65 722e 7175  put_quantizer.qu
+000103f0: 616e 7428 7365 6c66 2e73 6b6c 6561 726e  ant(self.sklearn
+00010400: 5f6d 6f64 656c 2e69 6e74 6572 6365 7074  _model.intercept
+00010410: 5f29 0a0a 2020 2020 2020 2020 2320 5369  _)..        # Si
+00010420: 6e63 6520 7468 6520 6d61 746d 756c 2061  nce the matmul a
+00010430: 6e64 2074 6865 2062 6961 7320 626f 7468  nd the bias both
+00010440: 2075 7365 2074 6865 2073 616d 6520 7363   use the same sc
+00010450: 616c 6520 616e 6420 7a65 726f 2d70 6f69  ale and zero-poi
+00010460: 6e74 732c 2077 6520 6f62 7461 696e 2074  nts, we obtain t
+00010470: 6861 740a 2020 2020 2020 2020 2320 7920  hat.        # y 
+00010480: 3d20 532a 2871 5f79 202d 2032 2a5a 2920  = S*(q_y - 2*Z) 
+00010490: 7768 656e 2064 652d 7175 616e 7469 7a69  when de-quantizi
+000104a0: 6e67 2074 6865 2076 616c 7565 732e 2057  ng the values. W
+000104b0: 6520 7468 6572 6566 6f72 6520 6e65 6564  e therefore need
+000104c0: 2074 6f20 6d75 6c74 6970 6c79 2074 6865   to multiply the
+000104d0: 2069 6e69 7469 616c 0a20 2020 2020 2020   initial.       
+000104e0: 2023 206f 7574 7075 7420 7a65 726f 5f70   # output zero_p
+000104f0: 6f69 6e74 2062 7920 320a 2020 2020 2020  oint by 2.      
+00010500: 2020 6173 7365 7274 206f 7574 7075 745f    assert output_
+00010510: 7175 616e 7469 7a65 722e 7a65 726f 5f70  quantizer.zero_p
+00010520: 6f69 6e74 2069 7320 6e6f 7420 4e6f 6e65  oint is not None
+00010530: 0a20 2020 2020 2020 206f 7574 7075 745f  .        output_
+00010540: 7175 616e 7469 7a65 722e 7a65 726f 5f70  quantizer.zero_p
+00010550: 6f69 6e74 202a 3d20 320a 2020 2020 2020  oint *= 2.      
+00010560: 2020 7365 6c66 2e6f 7574 7075 745f 7175    self.output_qu
+00010570: 616e 7469 7a65 7273 203d 205b 6f75 7470  antizers = [outp
+00010580: 7574 5f71 7561 6e74 697a 6572 5d0a 0a20  ut_quantizer].. 
+00010590: 2020 2020 2020 2023 2055 7064 6174 696e         # Updatin
+000105a0: 6720 706f 7374 2d70 726f 6365 7373 696e  g post-processin
+000105b0: 6720 7061 7261 6d65 7465 7273 0a20 2020  g parameters.   
+000105c0: 2020 2020 2073 656c 662e 5f73 6574 5f70       self._set_p
+000105d0: 6f73 745f 7072 6f63 6573 7369 6e67 5f70  ost_processing_p
+000105e0: 6172 616d 7328 290a 0a20 2020 2020 2020  arams()..       
+000105f0: 2073 656c 662e 5f69 735f 6669 7474 6564   self._is_fitted
+00010600: 203d 2054 7275 650a 0a20 2020 2020 2020   = True..       
+00010610: 2072 6574 7572 6e20 7365 6c66 0a0a 2020   return self..  
+00010620: 2020 6465 6620 7175 616e 7469 7a65 5f69    def quantize_i
+00010630: 6e70 7574 2873 656c 662c 2058 3a20 6e75  nput(self, X: nu
+00010640: 6d70 792e 6e64 6172 7261 7929 202d 3e20  mpy.ndarray) -> 
+00010650: 6e75 6d70 792e 6e64 6172 7261 793a 0a20  numpy.ndarray:. 
+00010660: 2020 2020 2020 2073 656c 662e 6368 6563         self.chec
+00010670: 6b5f 6d6f 6465 6c5f 6973 5f66 6974 7465  k_model_is_fitte
+00010680: 6428 290a 2020 2020 2020 2020 715f 5820  d().        q_X 
+00010690: 3d20 7365 6c66 2e69 6e70 7574 5f71 7561  = self.input_qua
+000106a0: 6e74 697a 6572 735b 305d 2e71 7561 6e74  ntizers[0].quant
+000106b0: 2858 290a 0a20 2020 2020 2020 2061 7373  (X)..        ass
+000106c0: 6572 7420 715f 582e 6474 7970 6520 3d3d  ert q_X.dtype ==
+000106d0: 206e 756d 7079 2e69 6e74 3634 2c20 2249   numpy.int64, "I
+000106e0: 6e70 7574 7320 7765 7265 206e 6f74 2071  nputs were not q
+000106f0: 7561 6e74 697a 6564 2074 6f20 696e 7436  uantized to int6
+00010700: 3420 7661 6c75 6573 220a 2020 2020 2020  4 values".      
+00010710: 2020 7265 7475 726e 2071 5f58 0a0a 2020    return q_X..  
+00010720: 2020 6465 6620 6465 7175 616e 7469 7a65    def dequantize
+00010730: 5f6f 7574 7075 7428 7365 6c66 2c20 715f  _output(self, q_
+00010740: 795f 7072 6564 733a 206e 756d 7079 2e6e  y_preds: numpy.n
+00010750: 6461 7272 6179 2920 2d3e 206e 756d 7079  darray) -> numpy
+00010760: 2e6e 6461 7272 6179 3a0a 2020 2020 2020  .ndarray:.      
+00010770: 2020 7365 6c66 2e63 6865 636b 5f6d 6f64    self.check_mod
+00010780: 656c 5f69 735f 6669 7474 6564 2829 0a0a  el_is_fitted()..
+00010790: 2020 2020 2020 2020 2320 4465 2d71 7561          # De-qua
+000107a0: 6e74 697a 6520 7468 6520 6f75 7470 7574  ntize the output
+000107b0: 2076 616c 7565 730a 2020 2020 2020 2020   values.        
+000107c0: 795f 7072 6564 7320 3d20 7365 6c66 2e6f  y_preds = self.o
+000107d0: 7574 7075 745f 7175 616e 7469 7a65 7273  utput_quantizers
+000107e0: 5b30 5d2e 6465 7175 616e 7428 715f 795f  [0].dequant(q_y_
+000107f0: 7072 6564 7329 0a0a 2020 2020 2020 2020  preds)..        
+00010800: 7265 7475 726e 2079 5f70 7265 6473 0a0a  return y_preds..
+00010810: 2020 2020 6465 6620 5f67 6574 5f6d 6f64      def _get_mod
+00010820: 756c 655f 746f 5f63 6f6d 7069 6c65 2873  ule_to_compile(s
+00010830: 656c 6629 202d 3e20 556e 696f 6e5b 436f  elf) -> Union[Co
+00010840: 6d70 696c 6572 2c20 5175 616e 7469 7a65  mpiler, Quantize
+00010850: 644d 6f64 756c 655d 3a0a 2020 2020 2020  dModule]:.      
+00010860: 2020 2320 4465 6669 6e65 2074 6865 2069    # Define the i
+00010870: 6e66 6572 656e 6365 2066 756e 6374 696f  nference functio
+00010880: 6e20 746f 2063 6f6d 7069 6c65 2e0a 2020  n to compile..  
+00010890: 2020 2020 2020 2320 5468 6973 2066 756e        # This fun
+000108a0: 6374 696f 6e20 6361 6e20 6e65 6974 6865  ction can neithe
+000108b0: 7220 6265 2061 2063 6c61 7373 206d 6574  r be a class met
+000108c0: 686f 6420 6e6f 7220 6120 7374 6174 6963  hod nor a static
+000108d0: 206f 6e65 2062 6563 6175 7365 2073 656c   one because sel
+000108e0: 6620 7765 2077 616e 7420 746f 2061 766f  f we want to avo
+000108f0: 6964 0a20 2020 2020 2020 2023 2068 6176  id.        # hav
+00010900: 696e 6720 7365 6c66 2061 7320 6120 7061  ing self as a pa
+00010910: 7261 6d65 7465 7220 7768 696c 6520 7374  rameter while st
+00010920: 696c 6c20 6265 696e 6720 6162 6c65 2074  ill being able t
+00010930: 6f20 6163 6365 7373 2073 6f6d 6520 6f66  o access some of
+00010940: 2069 7473 2061 7474 7269 6275 7465 0a20   its attribute. 
+00010950: 2020 2020 2020 2064 6566 2069 6e66 6572         def infer
+00010960: 656e 6365 5f74 6f5f 636f 6d70 696c 6528  ence_to_compile(
+00010970: 715f 583a 206e 756d 7079 2e6e 6461 7272  q_X: numpy.ndarr
+00010980: 6179 2920 2d3e 206e 756d 7079 2e6e 6461  ay) -> numpy.nda
+00010990: 7272 6179 3a0a 2020 2020 2020 2020 2020  rray:.          
+000109a0: 2020 2222 2243 6f6d 7069 6c65 2074 6865    """Compile the
+000109b0: 2063 6972 6375 6974 2069 6e20 4648 4520   circuit in FHE 
+000109c0: 7573 696e 6720 6f6e 6c79 2074 6865 2069  using only the i
+000109d0: 6e70 7574 7320 6173 2070 6172 616d 6574  nputs as paramet
+000109e0: 6572 732e 0a0a 2020 2020 2020 2020 2020  ers...          
+000109f0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00010a00: 2020 2020 2020 2020 715f 5820 286e 756d          q_X (num
+00010a10: 7079 2e6e 6461 7272 6179 293a 2054 6865  py.ndarray): The
+00010a20: 2071 7561 6e74 697a 6564 2069 6e70 7574   quantized input
+00010a30: 2064 6174 610a 0a20 2020 2020 2020 2020   data..         
+00010a40: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00010a50: 2020 2020 2020 2020 2020 2020 6e75 6d70              nump
+00010a60: 792e 6e64 6172 7261 793a 2054 6865 2063  y.ndarray: The c
+00010a70: 6972 6375 6974 2069 7320 6f75 7470 7574  ircuit is output
+00010a80: 732e 0a20 2020 2020 2020 2020 2020 2022  s..            "
+00010a90: 2222 0a20 2020 2020 2020 2020 2020 2072  "".            r
+00010aa0: 6574 7572 6e20 7365 6c66 2e5f 696e 6665  eturn self._infe
+00010ab0: 7265 6e63 6528 715f 5829 0a0a 2020 2020  rence(q_X)..    
+00010ac0: 2020 2020 2320 4372 6561 7465 2074 6865      # Create the
+00010ad0: 2063 6f6d 7069 6c65 7220 696e 7374 616e   compiler instan
+00010ae0: 6365 0a20 2020 2020 2020 2063 6f6d 7069  ce.        compi
+00010af0: 6c65 7220 3d20 436f 6d70 696c 6572 2869  ler = Compiler(i
+00010b00: 6e66 6572 656e 6365 5f74 6f5f 636f 6d70  nference_to_comp
+00010b10: 696c 652c 207b 2271 5f58 223a 2022 656e  ile, {"q_X": "en
+00010b20: 6372 7970 7465 6422 7d29 0a0a 2020 2020  crypted"})..    
+00010b30: 2020 2020 7265 7475 726e 2063 6f6d 7069      return compi
+00010b40: 6c65 720a 0a20 2020 2064 6566 205f 696e  ler..    def _in
+00010b50: 6665 7265 6e63 6528 7365 6c66 2c20 715f  ference(self, q_
+00010b60: 583a 206e 756d 7079 2e6e 6461 7272 6179  X: numpy.ndarray
+00010b70: 2920 2d3e 206e 756d 7079 2e6e 6461 7272  ) -> numpy.ndarr
+00010b80: 6179 3a0a 2020 2020 2020 2020 6173 7365  ay:.        asse
+00010b90: 7274 2073 656c 662e 5f77 6569 6768 745f  rt self._weight_
+00010ba0: 7175 616e 7469 7a65 7220 6973 206e 6f74  quantizer is not
+00010bb0: 204e 6f6e 652c 2073 656c 662e 5f69 735f   None, self._is_
+00010bc0: 6e6f 745f 6669 7474 6564 5f65 7272 6f72  not_fitted_error
+00010bd0: 5f6d 6573 7361 6765 2829 0a0a 2020 2020  _message()..    
+00010be0: 2020 2020 2320 5175 616e 7469 7a69 6e67      # Quantizing
+00010bf0: 2077 6569 6768 7473 2061 6e64 2069 6e70   weights and inp
+00010c00: 7574 7320 6d61 6b65 7320 616e 2061 6464  uts makes an add
+00010c10: 6974 696f 6e61 6c20 7465 726d 2061 7070  itional term app
+00010c20: 6561 7220 696e 2074 6865 2069 6e66 6572  ear in the infer
+00010c30: 656e 6365 2066 756e 6374 696f 6e0a 2020  ence function.  
+00010c40: 2020 2020 2020 795f 7072 6564 203d 2071        y_pred = q
+00010c50: 5f58 2040 2073 656c 662e 5f71 5f77 6569  _X @ self._q_wei
+00010c60: 6768 7473 202d 2073 656c 662e 5f77 6569  ghts - self._wei
+00010c70: 6768 745f 7175 616e 7469 7a65 722e 7a65  ght_quantizer.ze
+00010c80: 726f 5f70 6f69 6e74 202a 206e 756d 7079  ro_point * numpy
+00010c90: 2e73 756d 280a 2020 2020 2020 2020 2020  .sum(.          
+00010ca0: 2020 715f 582c 2061 7869 733d 312c 206b    q_X, axis=1, k
+00010cb0: 6565 7064 696d 733d 5472 7565 0a20 2020  eepdims=True.   
+00010cc0: 2020 2020 2029 0a20 2020 2020 2020 2079       ).        y
+00010cd0: 5f70 7265 6420 2b3d 2073 656c 662e 5f71  _pred += self._q
+00010ce0: 5f62 6961 730a 2020 2020 2020 2020 7265  _bias.        re
+00010cf0: 7475 726e 2079 5f70 7265 640a 0a0a 636c  turn y_pred...cl
+00010d00: 6173 7320 536b 6c65 6172 6e4c 696e 6561  ass SklearnLinea
+00010d10: 7252 6567 7265 7373 6f72 4d69 7869 6e28  rRegressorMixin(
+00010d20: 536b 6c65 6172 6e4c 696e 6561 724d 6f64  SklearnLinearMod
+00010d30: 656c 4d69 7869 6e2c 2073 6b6c 6561 726e  elMixin, sklearn
+00010d40: 2e62 6173 652e 5265 6772 6573 736f 724d  .base.RegressorM
+00010d50: 6978 696e 2c20 4142 4329 3a0a 2020 2020  ixin, ABC):.    
+00010d60: 2222 2241 204d 6978 696e 2063 6c61 7373  """A Mixin class
+00010d70: 2066 6f72 2073 6b6c 6561 726e 206c 696e   for sklearn lin
+00010d80: 6561 7220 7265 6772 6573 736f 7273 2077  ear regressors w
+00010d90: 6974 6820 4648 452e 0a0a 2020 2020 5468  ith FHE...    Th
+00010da0: 6973 2063 6c61 7373 2069 7320 7573 6564  is class is used
+00010db0: 2074 6f20 6372 6561 7465 2061 206c 696e   to create a lin
+00010dc0: 6561 7220 7265 6772 6573 736f 7220 636c  ear regressor cl
+00010dd0: 6173 7320 7468 6174 2069 6e68 6572 6974  ass that inherit
+00010de0: 7320 6672 6f6d 0a20 2020 2073 6b6c 6561  s from.    sklea
+00010df0: 726e 2e62 6173 652e 5265 6772 6573 736f  rn.base.Regresso
+00010e00: 724d 6978 696e 2c20 7768 6963 6820 6573  rMixin, which es
+00010e10: 7365 6e74 6961 6c6c 7920 6769 7665 7320  sentially gives 
+00010e20: 6163 6365 7373 2074 6f20 7363 696b 6974  access to scikit
+00010e30: 2d6c 6561 726e 2773 2060 7363 6f72 6560  -learn's `score`
+00010e40: 206d 6574 686f 640a 2020 2020 666f 7220   method.    for 
+00010e50: 7265 6772 6573 736f 7273 2e0a 2020 2020  regressors..    
+00010e60: 2222 220a 0a0a 636c 6173 7320 536b 6c65  """...class Skle
+00010e70: 6172 6e53 4744 5265 6772 6573 736f 724d  arnSGDRegressorM
+00010e80: 6978 696e 2853 6b6c 6561 726e 4c69 6e65  ixin(SklearnLine
+00010e90: 6172 5265 6772 6573 736f 724d 6978 696e  arRegressorMixin
+00010ea0: 293a 0a20 2020 2022 2222 4120 4d69 7869  ):.    """A Mixi
+00010eb0: 6e20 636c 6173 7320 666f 7220 736b 6c65  n class for skle
+00010ec0: 6172 6e20 5347 4420 7265 6772 6573 736f  arn SGD regresso
+00010ed0: 7273 2077 6974 6820 4648 452e 0a0a 2020  rs with FHE...  
+00010ee0: 2020 5468 6973 2063 6c61 7373 2069 7320    This class is 
+00010ef0: 7573 6564 2074 6f20 6372 6561 7465 2061  used to create a
+00010f00: 2053 4744 2072 6567 7265 7373 6f72 2063   SGD regressor c
+00010f10: 6c61 7373 2077 6861 7420 6361 6e20 6265  lass what can be
+00010f20: 2065 7870 6f72 7465 640a 2020 2020 746f   exported.    to
+00010f30: 204f 4e4e 5820 7573 696e 6720 4875 6d6d   ONNX using Humm
+00010f40: 696e 6762 6972 642e 0a20 2020 2022 2222  ingbird..    """
+00010f50: 0a0a 2020 2020 2320 5265 6d6f 7665 206f  ..    # Remove o
+00010f60: 6e63 6520 4875 6d6d 696e 6762 6972 6420  nce Hummingbird 
+00010f70: 7375 7070 6f72 7473 2053 4744 5265 6772  supports SGDRegr
+00010f80: 6573 736f 720a 2020 2020 2320 4649 584d  essor.    # FIXM
+00010f90: 453a 2068 7474 7073 3a2f 2f67 6974 6875  E: https://githu
+00010fa0: 622e 636f 6d2f 7a61 6d61 2d61 692f 636f  b.com/zama-ai/co
+00010fb0: 6e63 7265 7465 2d6d 6c2d 696e 7465 726e  ncrete-ml-intern
+00010fc0: 616c 2f69 7373 7565 732f 3431 3030 0a20  al/issues/4100. 
+00010fd0: 2020 2064 6566 205f 7365 745f 6f6e 6e78     def _set_onnx
+00010fe0: 5f6d 6f64 656c 2873 656c 662c 2074 6573  _model(self, tes
+00010ff0: 745f 696e 7075 743a 206e 756d 7079 2e6e  t_input: numpy.n
+00011000: 6461 7272 6179 2920 2d3e 204e 6f6e 653a  darray) -> None:
+00011010: 0a20 2020 2020 2020 2022 2222 5265 7472  .        """Retr
+00011020: 6965 7665 2074 6865 206d 6f64 656c 2773  ieve the model's
+00011030: 204f 4e4e 5820 6772 6170 6820 7573 696e   ONNX graph usin
+00011040: 6720 4875 6d6d 696e 6762 6972 6420 636f  g Hummingbird co
+00011050: 6e76 6572 7369 6f6e 2e0a 0a20 2020 2020  nversion...     
+00011060: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00011070: 2020 2020 2074 6573 745f 696e 7075 7420       test_input 
+00011080: 286e 756d 7079 2e6e 6461 7272 6179 293a  (numpy.ndarray):
+00011090: 2041 6e20 696e 7075 7420 6461 7461 2075   An input data u
+000110a0: 7365 6420 746f 2074 7261 6365 2074 6865  sed to trace the
+000110b0: 206d 6f64 656c 2065 7865 6375 7469 6f6e   model execution
+000110c0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+000110d0: 2020 2020 2020 2320 4368 6563 6b20 7468        # Check th
+000110e0: 6174 2074 6865 2075 6e64 6572 6c79 696e  at the underlyin
+000110f0: 6720 736b 6c65 6172 6e20 6d6f 6465 6c20  g sklearn model 
+00011100: 6861 7320 6265 656e 2073 6574 2061 6e64  has been set and
+00011110: 2066 6974 0a20 2020 2020 2020 2061 7373   fit.        ass
+00011120: 6572 7420 7365 6c66 2e73 6b6c 6561 726e  ert self.sklearn
+00011130: 5f6d 6f64 656c 2069 7320 6e6f 7420 4e6f  _model is not No
+00011140: 6e65 2c20 7365 6c66 2e5f 736b 6c65 6172  ne, self._sklear
+00011150: 6e5f 6d6f 6465 6c5f 6973 5f6e 6f74 5f66  n_model_is_not_f
+00011160: 6974 7465 645f 6572 726f 725f 6d65 7373  itted_error_mess
+00011170: 6167 6528 290a 0a20 2020 2020 2020 206d  age()..        m
+00011180: 6f64 656c 5f66 6f72 5f6f 6e6e 7820 3d20  odel_for_onnx = 
+00011190: 4c69 6e65 6172 5265 6772 6573 7369 6f6e  LinearRegression
+000111a0: 2829 0a20 2020 2020 2020 206d 6f64 656c  ().        model
+000111b0: 5f66 6f72 5f6f 6e6e 782e 636f 6566 5f20  _for_onnx.coef_ 
+000111c0: 3d20 7365 6c66 2e73 6b6c 6561 726e 5f6d  = self.sklearn_m
+000111d0: 6f64 656c 2e63 6f65 665f 0a20 2020 2020  odel.coef_.     
+000111e0: 2020 206d 6f64 656c 5f66 6f72 5f6f 6e6e     model_for_onn
+000111f0: 782e 696e 7465 7263 6570 745f 203d 2073  x.intercept_ = s
+00011200: 656c 662e 736b 6c65 6172 6e5f 6d6f 6465  elf.sklearn_mode
+00011210: 6c2e 696e 7465 7263 6570 745f 0a0a 2020  l.intercept_..  
+00011220: 2020 2020 2020 7365 6c66 2e6f 6e6e 785f        self.onnx_
+00011230: 6d6f 6465 6c5f 203d 2068 625f 636f 6e76  model_ = hb_conv
+00011240: 6572 7428 0a20 2020 2020 2020 2020 2020  ert(.           
+00011250: 206d 6f64 656c 5f66 6f72 5f6f 6e6e 782c   model_for_onnx,
+00011260: 0a20 2020 2020 2020 2020 2020 2062 6163  .            bac
+00011270: 6b65 6e64 3d22 6f6e 6e78 222c 0a20 2020  kend="onnx",.   
+00011280: 2020 2020 2020 2020 2074 6573 745f 696e           test_in
+00011290: 7075 743d 7465 7374 5f69 6e70 7574 2c0a  put=test_input,.
+000112a0: 2020 2020 2020 2020 2020 2020 6578 7472              extr
+000112b0: 615f 636f 6e66 6967 3d7b 226f 6e6e 785f  a_config={"onnx_
+000112c0: 7461 7267 6574 5f6f 7073 6574 223a 204f  target_opset": O
+000112d0: 5053 4554 5f56 4552 5349 4f4e 5f46 4f52  PSET_VERSION_FOR
+000112e0: 5f4f 4e4e 585f 4558 504f 5254 7d2c 0a20  _ONNX_EXPORT},. 
+000112f0: 2020 2020 2020 2029 2e6d 6f64 656c 0a0a         ).model..
+00011300: 2020 2020 2020 2020 7365 6c66 2e5f 636c          self._cl
+00011310: 6561 6e5f 6772 6170 6828 290a 0a0a 636c  ean_graph()...cl
+00011320: 6173 7320 536b 6c65 6172 6e4c 696e 6561  ass SklearnLinea
+00011330: 7243 6c61 7373 6966 6965 724d 6978 696e  rClassifierMixin
+00011340: 280a 2020 2020 4261 7365 436c 6173 7369  (.    BaseClassi
+00011350: 6669 6572 2c20 536b 6c65 6172 6e4c 696e  fier, SklearnLin
+00011360: 6561 724d 6f64 656c 4d69 7869 6e2c 2073  earModelMixin, s
+00011370: 6b6c 6561 726e 2e62 6173 652e 436c 6173  klearn.base.Clas
+00011380: 7369 6669 6572 4d69 7869 6e2c 2041 4243  sifierMixin, ABC
+00011390: 0a29 3a0a 2020 2020 2222 2241 204d 6978  .):.    """A Mix
+000113a0: 696e 2063 6c61 7373 2066 6f72 2073 6b6c  in class for skl
+000113b0: 6561 726e 206c 696e 6561 7220 636c 6173  earn linear clas
+000113c0: 7369 6669 6572 7320 7769 7468 2046 4845  sifiers with FHE
+000113d0: 2e0a 0a20 2020 2054 6869 7320 636c 6173  ...    This clas
+000113e0: 7320 6973 2075 7365 6420 746f 2063 7265  s is used to cre
+000113f0: 6174 6520 6120 6c69 6e65 6172 2063 6c61  ate a linear cla
+00011400: 7373 6966 6965 7220 636c 6173 7320 7468  ssifier class th
+00011410: 6174 2069 6e68 6572 6974 7320 6672 6f6d  at inherits from
+00011420: 0a20 2020 2073 6b6c 6561 726e 2e62 6173  .    sklearn.bas
+00011430: 652e 436c 6173 7369 6669 6572 4d69 7869  e.ClassifierMixi
+00011440: 6e2c 2077 6869 6368 2065 7373 656e 7469  n, which essenti
+00011450: 616c 6c79 2067 6976 6573 2061 6363 6573  ally gives acces
+00011460: 7320 746f 2073 6369 6b69 742d 6c65 6172  s to scikit-lear
+00011470: 6e27 7320 6073 636f 7265 6020 6d65 7468  n's `score` meth
+00011480: 6f64 0a20 2020 2066 6f72 2063 6c61 7373  od.    for class
+00011490: 6966 6965 7273 2e0a 0a20 2020 2041 6464  ifiers...    Add
+000114a0: 6974 696f 6e61 6c6c 792c 2074 6869 7320  itionally, this 
+000114b0: 636c 6173 7320 6164 6a75 7374 7320 736f  class adjusts so
+000114c0: 6d65 206f 6620 7468 6520 7472 6565 2d62  me of the tree-b
+000114d0: 6173 6564 2062 6173 6520 636c 6173 7327  ased base class'
+000114e0: 7320 6d65 7468 6f64 7320 696e 206f 7264  s methods in ord
+000114f0: 6572 2074 6f20 6d61 6b65 0a20 2020 2074  er to make.    t
+00011500: 6865 6d20 636f 6d70 6c69 616e 7420 7769  hem compliant wi
+00011510: 7468 2063 6c61 7373 6966 6963 6174 696f  th classificatio
+00011520: 6e20 776f 726b 666c 6f77 732e 0a20 2020  n workflows..   
+00011530: 2022 2222 0a0a 2020 2020 6465 6620 5f63   """..    def _c
+00011540: 6c65 616e 5f67 7261 7068 2873 656c 6629  lean_graph(self)
+00011550: 202d 3e20 4e6f 6e65 3a0a 2020 2020 2020   -> None:.      
+00011560: 2020 6173 7365 7274 2073 656c 662e 6f6e    assert self.on
+00011570: 6e78 5f6d 6f64 656c 5f20 6973 206e 6f74  nx_model_ is not
+00011580: 204e 6f6e 652c 2073 656c 662e 5f69 735f   None, self._is_
+00011590: 6e6f 745f 6669 7474 6564 5f65 7272 6f72  not_fitted_error
+000115a0: 5f6d 6573 7361 6765 2829 0a0a 2020 2020  _message()..    
+000115b0: 2020 2020 2320 5265 6d6f 7665 2061 6e79      # Remove any
+000115c0: 206f 7065 7261 746f 7273 2066 6f6c 6c6f   operators follo
+000115d0: 7769 6e67 2067 656d 6d2c 2061 7320 7468  wing gemm, as th
+000115e0: 6579 2077 696c 6c20 6265 2064 6f6e 6520  ey will be done 
+000115f0: 696e 2074 6865 2063 6c65 6172 0a20 2020  in the clear.   
+00011600: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
+00011610: 2e6f 6e6e 785f 6d6f 6465 6c5f 2069 7320  .onnx_model_ is 
+00011620: 6e6f 7420 4e6f 6e65 0a20 2020 2020 2020  not None.       
+00011630: 2063 6c65 616e 5f67 7261 7068 5f61 6674   clean_graph_aft
+00011640: 6572 5f6e 6f64 655f 6f70 5f74 7970 6528  er_node_op_type(
+00011650: 7365 6c66 2e6f 6e6e 785f 6d6f 6465 6c5f  self.onnx_model_
+00011660: 2c20 6e6f 6465 5f6f 705f 7479 7065 3d22  , node_op_type="
+00011670: 4765 6d6d 2229 0a20 2020 2020 2020 2053  Gemm").        S
+00011680: 6b6c 6561 726e 4c69 6e65 6172 4d6f 6465  klearnLinearMode
+00011690: 6c4d 6978 696e 2e5f 636c 6561 6e5f 6772  lMixin._clean_gr
+000116a0: 6170 6828 7365 6c66 290a 0a20 2020 2064  aph(self)..    d
+000116b0: 6566 2064 6563 6973 696f 6e5f 6675 6e63  ef decision_func
+000116c0: 7469 6f6e 280a 2020 2020 2020 2020 7365  tion(.        se
+000116d0: 6c66 2c20 583a 2044 6174 612c 2066 6865  lf, X: Data, fhe
+000116e0: 3a20 556e 696f 6e5b 4668 654d 6f64 652c  : Union[FheMode,
+000116f0: 2073 7472 5d20 3d20 4668 654d 6f64 652e   str] = FheMode.
+00011700: 4449 5341 424c 450a 2020 2020 2920 2d3e  DISABLE.    ) ->
+00011710: 206e 756d 7079 2e6e 6461 7272 6179 3a0a   numpy.ndarray:.
+00011720: 2020 2020 2020 2020 2222 2250 7265 6469          """Predi
+00011730: 6374 2063 6f6e 6669 6465 6e63 6520 7363  ct confidence sc
+00011740: 6f72 6573 2e0a 0a20 2020 2020 2020 2041  ores...        A
+00011750: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00011760: 2058 2028 4461 7461 293a 2054 6865 2069   X (Data): The i
+00011770: 6e70 7574 2076 616c 7565 7320 746f 2070  nput values to p
+00011780: 7265 6469 6374 2c20 6173 2061 204e 756d  redict, as a Num
+00011790: 7079 2061 7272 6179 2c20 546f 7263 6820  py array, Torch 
+000117a0: 7465 6e73 6f72 2c20 5061 6e64 6173 2044  tensor, Pandas D
+000117b0: 6174 6146 7261 6d65 0a20 2020 2020 2020  ataFrame.       
+000117c0: 2020 2020 2020 2020 206f 7220 4c69 7374           or List
+000117d0: 2e0a 2020 2020 2020 2020 2020 2020 6668  ..            fh
+000117e0: 6520 2855 6e69 6f6e 5b46 6865 4d6f 6465  e (Union[FheMode
+000117f0: 2c20 7374 725d 293a 2054 6865 206d 6f64  , str]): The mod
+00011800: 6520 746f 2075 7365 2066 6f72 2070 7265  e to use for pre
+00011810: 6469 6374 696f 6e2e 0a20 2020 2020 2020  diction..       
+00011820: 2020 2020 2020 2020 2043 616e 2062 6520           Can be 
+00011830: 4668 654d 6f64 652e 4449 5341 424c 4520  FheMode.DISABLE 
+00011840: 666f 7220 436f 6e63 7265 7465 204d 4c20  for Concrete ML 
+00011850: 5079 7468 6f6e 2069 6e66 6572 656e 6365  Python inference
+00011860: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00011870: 2020 4668 654d 6f64 652e 5349 4d55 4c41    FheMode.SIMULA
+00011880: 5445 2066 6f72 2046 4845 2073 696d 756c  TE for FHE simul
+00011890: 6174 696f 6e20 616e 6420 4668 654d 6f64  ation and FheMod
+000118a0: 652e 4558 4543 5554 4520 666f 7220 6163  e.EXECUTE for ac
+000118b0: 7475 616c 2046 4845 2065 7865 6375 7469  tual FHE executi
+000118c0: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
+000118d0: 2020 2020 4361 6e20 616c 736f 2062 6520      Can also be 
+000118e0: 7468 6520 7374 7269 6e67 2072 6570 7265  the string repre
+000118f0: 7365 6e74 6174 696f 6e20 6f66 2061 6e79  sentation of any
+00011900: 206f 6620 7468 6573 6520 7661 6c75 6573   of these values
+00011910: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00011920: 2020 4465 6661 756c 7420 746f 2046 6865    Default to Fhe
+00011930: 4d6f 6465 2e44 4953 4142 4c45 2e0a 0a20  Mode.DISABLE... 
+00011940: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
+00011950: 2020 2020 2020 2020 2020 2020 6e75 6d70              nump
+00011960: 792e 6e64 6172 7261 793a 2054 6865 2070  y.ndarray: The p
+00011970: 7265 6469 6374 6564 2063 6f6e 6669 6465  redicted confide
+00011980: 6e63 6520 7363 6f72 6573 2e0a 2020 2020  nce scores..    
+00011990: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000119a0: 2320 4865 7265 2c20 7765 2077 616e 7420  # Here, we want 
+000119b0: 746f 2075 7365 2053 6b6c 6561 726e 4c69  to use SklearnLi
+000119c0: 6e65 6172 4d6f 6465 6c4d 6978 696e 2773  nearModelMixin's
+000119d0: 2060 7072 6564 6963 7460 206d 6574 686f   `predict` metho
+000119e0: 6420 6173 2063 6f6e 6669 6465 6e63 6520  d as confidence 
+000119f0: 7363 6f72 6573 2061 7265 0a20 2020 2020  scores are.     
+00011a00: 2020 2023 2074 6865 2064 6f74 2070 726f     # the dot pro
+00011a10: 6475 6374 2773 206f 7574 7075 7420 7661  duct's output va
+00011a20: 6c75 6573 2c20 7769 7468 6f75 7420 616e  lues, without an
+00011a30: 7920 706f 7374 2d70 726f 6365 7373 696e  y post-processin
+00011a40: 670a 2020 2020 2020 2020 795f 7072 6564  g.        y_pred
+00011a50: 7320 3d20 536b 6c65 6172 6e4c 696e 6561  s = SklearnLinea
+00011a60: 724d 6f64 656c 4d69 7869 6e2e 7072 6564  rModelMixin.pred
+00011a70: 6963 7428 7365 6c66 2c20 582c 2066 6865  ict(self, X, fhe
+00011a80: 3d66 6865 290a 2020 2020 2020 2020 7265  =fhe).        re
+00011a90: 7475 726e 2079 5f70 7265 6473 0a0a 2020  turn y_preds..  
+00011aa0: 2020 6465 6620 7072 6564 6963 745f 7072    def predict_pr
+00011ab0: 6f62 6128 7365 6c66 2c20 583a 2044 6174  oba(self, X: Dat
+00011ac0: 612c 2066 6865 3a20 556e 696f 6e5b 4668  a, fhe: Union[Fh
+00011ad0: 654d 6f64 652c 2073 7472 5d20 3d20 4668  eMode, str] = Fh
+00011ae0: 654d 6f64 652e 4449 5341 424c 4529 202d  eMode.DISABLE) -
+00011af0: 3e20 6e75 6d70 792e 6e64 6172 7261 793a  > numpy.ndarray:
+00011b00: 0a20 2020 2020 2020 2079 5f6c 6f67 6974  .        y_logit
+00011b10: 7320 3d20 7365 6c66 2e64 6563 6973 696f  s = self.decisio
+00011b20: 6e5f 6675 6e63 7469 6f6e 2858 2c20 6668  n_function(X, fh
+00011b30: 653d 6668 6529 0a20 2020 2020 2020 2079  e=fhe).        y
+00011b40: 5f70 726f 6261 203d 2073 656c 662e 706f  _proba = self.po
+00011b50: 7374 5f70 726f 6365 7373 696e 6728 795f  st_processing(y_
+00011b60: 6c6f 6769 7473 290a 2020 2020 2020 2020  logits).        
+00011b70: 7265 7475 726e 2079 5f70 726f 6261 0a0a  return y_proba..
+00011b80: 0a63 6c61 7373 2053 6b6c 6561 726e 5347  .class SklearnSG
+00011b90: 4443 6c61 7373 6966 6965 724d 6978 696e  DClassifierMixin
+00011ba0: 2853 6b6c 6561 726e 4c69 6e65 6172 436c  (SklearnLinearCl
+00011bb0: 6173 7369 6669 6572 4d69 7869 6e29 3a0a  assifierMixin):.
+00011bc0: 2020 2020 2222 2241 204d 6978 696e 2063      """A Mixin c
+00011bd0: 6c61 7373 2066 6f72 2073 6b6c 6561 726e  lass for sklearn
+00011be0: 2053 4744 2063 6c61 7373 6966 6965 7273   SGD classifiers
+00011bf0: 2077 6974 6820 4648 452e 0a0a 2020 2020   with FHE...    
+00011c00: 5468 6973 2063 6c61 7373 2069 7320 7573  This class is us
+00011c10: 6564 2074 6f20 6372 6561 7465 2061 2053  ed to create a S
+00011c20: 4744 2063 6c61 7373 6966 6965 7220 636c  GD classifier cl
+00011c30: 6173 7320 7768 6174 2063 616e 2062 6520  ass what can be 
+00011c40: 6578 706f 7274 6564 0a20 2020 2074 6f20  exported.    to 
+00011c50: 4f4e 4e58 2075 7369 6e67 2048 756d 6d69  ONNX using Hummi
+00011c60: 6e67 6269 7264 2e0a 2020 2020 2222 220a  ngbird..    """.
+00011c70: 0a20 2020 2023 2052 656d 6f76 6520 6f6e  .    # Remove on
+00011c80: 6365 2048 756d 6d69 6e67 6269 7264 2073  ce Hummingbird s
+00011c90: 7570 706f 7274 7320 5347 4452 6567 7265  upports SGDRegre
+00011ca0: 7373 6f72 0a20 2020 2023 2046 4958 4d45  ssor.    # FIXME
+00011cb0: 3a20 6874 7470 733a 2f2f 6769 7468 7562  : https://github
+00011cc0: 2e63 6f6d 2f7a 616d 612d 6169 2f63 6f6e  .com/zama-ai/con
+00011cd0: 6372 6574 652d 6d6c 2d69 6e74 6572 6e61  crete-ml-interna
+00011ce0: 6c2f 6973 7375 6573 2f34 3130 300a 2020  l/issues/4100.  
+00011cf0: 2020 6465 6620 5f73 6574 5f6f 6e6e 785f    def _set_onnx_
+00011d00: 6d6f 6465 6c28 7365 6c66 2c20 7465 7374  model(self, test
+00011d10: 5f69 6e70 7574 3a20 6e75 6d70 792e 6e64  _input: numpy.nd
+00011d20: 6172 7261 7929 202d 3e20 4e6f 6e65 3a0a  array) -> None:.
+00011d30: 2020 2020 2020 2020 2222 2252 6574 7269          """Retri
+00011d40: 6576 6520 7468 6520 6d6f 6465 6c27 7320  eve the model's 
+00011d50: 4f4e 4e58 2067 7261 7068 2075 7369 6e67  ONNX graph using
+00011d60: 2048 756d 6d69 6e67 6269 7264 2063 6f6e   Hummingbird con
+00011d70: 7665 7273 696f 6e2e 0a0a 2020 2020 2020  version...      
+00011d80: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00011d90: 2020 2020 7465 7374 5f69 6e70 7574 2028      test_input (
+00011da0: 6e75 6d70 792e 6e64 6172 7261 7929 3a20  numpy.ndarray): 
+00011db0: 416e 2069 6e70 7574 2064 6174 6120 7573  An input data us
+00011dc0: 6564 2074 6f20 7472 6163 6520 7468 6520  ed to trace the 
+00011dd0: 6d6f 6465 6c20 6578 6563 7574 696f 6e2e  model execution.
+00011de0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00011df0: 2020 2020 2023 2043 6865 636b 2074 6861       # Check tha
+00011e00: 7420 7468 6520 756e 6465 726c 7969 6e67  t the underlying
+00011e10: 2073 6b6c 6561 726e 206d 6f64 656c 2068   sklearn model h
+00011e20: 6173 2062 6565 6e20 7365 7420 616e 6420  as been set and 
+00011e30: 6669 740a 2020 2020 2020 2020 6173 7365  fit.        asse
+00011e40: 7274 2073 656c 662e 736b 6c65 6172 6e5f  rt self.sklearn_
+00011e50: 6d6f 6465 6c20 6973 206e 6f74 204e 6f6e  model is not Non
+00011e60: 652c 2073 656c 662e 5f73 6b6c 6561 726e  e, self._sklearn
+00011e70: 5f6d 6f64 656c 5f69 735f 6e6f 745f 6669  _model_is_not_fi
+00011e80: 7474 6564 5f65 7272 6f72 5f6d 6573 7361  tted_error_messa
+00011e90: 6765 2829 0a0a 2020 2020 2020 2020 6d6f  ge()..        mo
+00011ea0: 6465 6c5f 666f 725f 6f6e 6e78 203d 204c  del_for_onnx = L
+00011eb0: 6f67 6973 7469 6352 6567 7265 7373 696f  ogisticRegressio
+00011ec0: 6e28 290a 2020 2020 2020 2020 6d6f 6465  n().        mode
+00011ed0: 6c5f 666f 725f 6f6e 6e78 2e63 6f65 665f  l_for_onnx.coef_
+00011ee0: 203d 2073 656c 662e 736b 6c65 6172 6e5f   = self.sklearn_
+00011ef0: 6d6f 6465 6c2e 636f 6566 5f0a 2020 2020  model.coef_.    
+00011f00: 2020 2020 6d6f 6465 6c5f 666f 725f 6f6e      model_for_on
+00011f10: 6e78 2e69 6e74 6572 6365 7074 5f20 3d20  nx.intercept_ = 
+00011f20: 7365 6c66 2e73 6b6c 6561 726e 5f6d 6f64  self.sklearn_mod
+00011f30: 656c 2e69 6e74 6572 6365 7074 5f0a 0a20  el.intercept_.. 
+00011f40: 2020 2020 2020 2073 656c 662e 6f6e 6e78         self.onnx
+00011f50: 5f6d 6f64 656c 5f20 3d20 6862 5f63 6f6e  _model_ = hb_con
+00011f60: 7665 7274 280a 2020 2020 2020 2020 2020  vert(.          
+00011f70: 2020 6d6f 6465 6c5f 666f 725f 6f6e 6e78    model_for_onnx
+00011f80: 2c0a 2020 2020 2020 2020 2020 2020 6261  ,.            ba
+00011f90: 636b 656e 643d 226f 6e6e 7822 2c0a 2020  ckend="onnx",.  
+00011fa0: 2020 2020 2020 2020 2020 7465 7374 5f69            test_i
+00011fb0: 6e70 7574 3d74 6573 745f 696e 7075 742c  nput=test_input,
+00011fc0: 0a20 2020 2020 2020 2020 2020 2065 7874  .            ext
+00011fd0: 7261 5f63 6f6e 6669 673d 7b22 6f6e 6e78  ra_config={"onnx
+00011fe0: 5f74 6172 6765 745f 6f70 7365 7422 3a20  _target_opset": 
+00011ff0: 4f50 5345 545f 5645 5253 494f 4e5f 464f  OPSET_VERSION_FO
+00012000: 525f 4f4e 4e58 5f45 5850 4f52 547d 2c0a  R_ONNX_EXPORT},.
+00012010: 2020 2020 2020 2020 292e 6d6f 6465 6c0a          ).model.
+00012020: 0a20 2020 2020 2020 2073 656c 662e 5f63  .        self._c
+00012030: 6c65 616e 5f67 7261 7068 2829 0a0a 0a23  lean_graph()...#
+00012040: 2070 796c 696e 743a 2064 6973 6162 6c65   pylint: disable
+00012050: 2d6e 6578 743d 696e 7661 6c69 642d 6e61  -next=invalid-na
+00012060: 6d65 2c74 6f6f 2d6d 616e 792d 696e 7374  me,too-many-inst
+00012070: 616e 6365 2d61 7474 7269 6275 7465 730a  ance-attributes.
+00012080: 636c 6173 7320 536b 6c65 6172 6e4b 4e65  class SklearnKNe
+00012090: 6967 6862 6f72 734d 6978 696e 2842 6173  ighborsMixin(Bas
+000120a0: 6545 7374 696d 6174 6f72 2c20 736b 6c65  eEstimator, skle
+000120b0: 6172 6e2e 6261 7365 2e42 6173 6545 7374  arn.base.BaseEst
+000120c0: 696d 6174 6f72 2c20 4142 4329 3a0a 2020  imator, ABC):.  
+000120d0: 2020 2222 2241 204d 6978 696e 2063 6c61    """A Mixin cla
+000120e0: 7373 2066 6f72 2073 6b6c 6561 726e 204b  ss for sklearn K
+000120f0: 4e65 6967 6862 6f72 7320 6d6f 6465 6c73  Neighbors models
+00012100: 2077 6974 6820 4648 452e 0a0a 2020 2020   with FHE...    
+00012110: 5468 6973 2063 6c61 7373 2069 6e68 6572  This class inher
+00012120: 6974 7320 6672 6f6d 2073 6b6c 6561 726e  its from sklearn
+00012130: 2e62 6173 652e 4261 7365 4573 7469 6d61  .base.BaseEstima
+00012140: 746f 7220 696e 206f 7264 6572 2074 6f20  tor in order to 
+00012150: 6861 7665 2061 6363 6573 7320 746f 2073  have access to s
+00012160: 6369 6b69 742d 6c65 6172 6e27 730a 2020  cikit-learn's.  
+00012170: 2020 6067 6574 5f70 6172 616d 7360 2061    `get_params` a
+00012180: 6e64 2060 7365 745f 7061 7261 6d73 6020  nd `set_params` 
+00012190: 6d65 7468 6f64 732e 0a20 2020 2022 2222  methods..    """
+000121a0: 0a0a 2020 2020 6465 6620 5f5f 696e 6974  ..    def __init
+000121b0: 5f73 7562 636c 6173 735f 5f28 636c 7329  _subclass__(cls)
+000121c0: 3a0a 2020 2020 2020 2020 666f 7220 6b6c  :.        for kl
+000121d0: 6173 7320 696e 2063 6c73 2e5f 5f6d 726f  ass in cls.__mro
+000121e0: 5f5f 3a0a 2020 2020 2020 2020 2020 2020  __:.            
+000121f0: 2320 7079 6c69 6e74 3a20 6469 7361 626c  # pylint: disabl
+00012200: 652d 6e65 7874 3d70 726f 7465 6374 6564  e-next=protected
+00012210: 2d61 6363 6573 730a 2020 2020 2020 2020  -access.        
+00012220: 2020 2020 6966 2067 6574 6174 7472 286b      if getattr(k
+00012230: 6c61 7373 2c20 225f 6973 5f61 5f70 7562  lass, "_is_a_pub
+00012240: 6c69 635f 636d 6c5f 6d6f 6465 6c22 2c20  lic_cml_model", 
+00012250: 4661 6c73 6529 3a0a 2020 2020 2020 2020  False):.        
+00012260: 2020 2020 2020 2020 5f4e 4549 4748 424f          _NEIGHBO
+00012270: 5253 5f4d 4f44 454c 532e 6164 6428 636c  RS_MODELS.add(cl
+00012280: 7329 0a20 2020 2020 2020 2020 2020 2020  s).             
+00012290: 2020 205f 414c 4c5f 534b 4c45 4152 4e5f     _ALL_SKLEARN_
+000122a0: 4d4f 4445 4c53 2e61 6464 2863 6c73 290a  MODELS.add(cls).
+000122b0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+000122c0: 5f28 7365 6c66 2c20 6e5f 6269 7473 3a20  _(self, n_bits: 
+000122d0: 696e 7420 3d20 3329 3a0a 2020 2020 2020  int = 3):.      
+000122e0: 2020 2222 2249 6e69 7469 616c 697a 6520    """Initialize 
+000122f0: 7468 6520 4648 4520 6b6e 6e20 6d6f 6465  the FHE knn mode
+00012300: 6c2e 0a0a 2020 2020 2020 2020 4172 6773  l...        Args
+00012310: 3a0a 2020 2020 2020 2020 2020 2020 6e5f  :.            n_
+00012320: 6269 7473 2028 696e 7429 3a20 4e75 6d62  bits (int): Numb
+00012330: 6572 206f 6620 6269 7473 2074 6f20 7175  er of bits to qu
+00012340: 616e 7469 7a65 2074 6865 206d 6f64 656c  antize the model
+00012350: 2e20 5468 6520 7661 6c75 6520 7769 6c6c  . The value will
+00012360: 2062 6520 7573 6564 2066 6f72 0a20 2020   be used for.   
+00012370: 2020 2020 2020 2020 2020 2020 2071 7561               qua
+00012380: 6e74 697a 696e 6720 696e 7075 7473 2061  ntizing inputs a
+00012390: 6e64 2058 5f66 6974 2e20 4465 6661 756c  nd X_fit. Defaul
+000123a0: 7420 746f 2033 2e0a 2020 2020 2020 2020  t to 3..        
+000123b0: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
+000123c0: 2e6e 5f62 6974 733a 2069 6e74 203d 206e  .n_bits: int = n
+000123d0: 5f62 6974 730a 0a20 2020 2020 2020 2023  _bits..        #
+000123e0: 205f 715f 6669 745f 583a 2049 6e20 6469   _q_fit_X: In di
+000123f0: 7374 616e 6365 206d 6574 7269 6320 616c  stance metric al
+00012400: 676f 7269 7468 6d73 2c20 605f 715f 6669  gorithms, `_q_fi
+00012410: 745f 5860 2073 746f 7265 7320 7468 6520  t_X` stores the 
+00012420: 7472 6169 6e69 6e67 2073 6574 2074 6f20  training set to 
+00012430: 636f 6d70 7574 650a 2020 2020 2020 2020  compute.        
+00012440: 2320 7468 6520 7369 6d69 6c61 7269 7479  # the similarity
+00012450: 206f 7220 6469 7374 616e 6365 206d 6561   or distance mea
+00012460: 7375 7265 732e 2054 6865 7265 2069 7320  sures. There is 
+00012470: 6e6f 2060 7765 6967 6874 7360 2061 7474  no `weights` att
+00012480: 7269 6275 7465 2062 6563 6175 7365 2074  ribute because t
+00012490: 6865 7265 2069 736e 2774 0a20 2020 2020  here isn't.     
+000124a0: 2020 2023 2061 2074 7261 696e 696e 6720     # a training 
+000124b0: 7068 6173 650a 2020 2020 2020 2020 7365  phase.        se
+000124c0: 6c66 2e5f 715f 6669 745f 583a 206e 756d  lf._q_fit_X: num
+000124d0: 7079 2e6e 6461 7272 6179 0a0a 2020 2020  py.ndarray..    
+000124e0: 2020 2020 2320 5f79 3a20 4c61 6265 6c73      # _y: Labels
+000124f0: 206f 6620 605f 715f 6669 745f 5860 0a20   of `_q_fit_X`. 
+00012500: 2020 2020 2020 2073 656c 662e 5f79 3a20         self._y: 
+00012510: 6e75 6d70 792e 6e64 6172 7261 790a 0a20  numpy.ndarray.. 
+00012520: 2020 2020 2020 2023 205f 715f 6669 745f         # _q_fit_
+00012530: 585f 7175 616e 7469 7a65 723a 2054 6865  X_quantizer: The
+00012540: 2071 7561 6e74 697a 6572 2074 6f20 7573   quantizer to us
+00012550: 6520 666f 7220 7175 616e 7469 7a69 6e67  e for quantizing
+00012560: 2074 6865 206d 6f64 656c 2773 2074 7261   the model's tra
+00012570: 696e 696e 6720 7365 740a 2020 2020 2020  ining set.      
+00012580: 2020 7365 6c66 2e5f 715f 6669 745f 585f    self._q_fit_X_
+00012590: 7175 616e 7469 7a65 723a 204f 7074 696f  quantizer: Optio
+000125a0: 6e61 6c5b 556e 6966 6f72 6d51 7561 6e74  nal[UniformQuant
+000125b0: 697a 6572 5d20 3d20 4e6f 6e65 0a0a 2020  izer] = None..  
+000125c0: 2020 2020 2020 4261 7365 4573 7469 6d61        BaseEstima
+000125d0: 746f 722e 5f5f 696e 6974 5f5f 2873 656c  tor.__init__(sel
+000125e0: 6629 0a0a 2020 2020 6465 6620 5f73 6574  f)..    def _set
+000125f0: 5f6f 6e6e 785f 6d6f 6465 6c28 7365 6c66  _onnx_model(self
+00012600: 2c20 7465 7374 5f69 6e70 7574 3a20 6e75  , test_input: nu
+00012610: 6d70 792e 6e64 6172 7261 7929 202d 3e20  mpy.ndarray) -> 
+00012620: 4e6f 6e65 3a0a 2020 2020 2020 2020 2222  None:.        ""
+00012630: 2252 6574 7269 6576 6520 7468 6520 6d6f  "Retrieve the mo
+00012640: 6465 6c27 7320 4f4e 4e58 2067 7261 7068  del's ONNX graph
+00012650: 2075 7369 6e67 2048 756d 6d69 6e67 6269   using Hummingbi
+00012660: 7264 2063 6f6e 7665 7273 696f 6e2e 0a0a  rd conversion...
+00012670: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00012680: 2020 2020 2020 2020 2020 7465 7374 5f69            test_i
+00012690: 6e70 7574 2028 6e75 6d70 792e 6e64 6172  nput (numpy.ndar
+000126a0: 7261 7929 3a20 416e 2069 6e70 7574 2064  ray): An input d
+000126b0: 6174 6120 7573 6564 2074 6f20 7472 6163  ata used to trac
+000126c0: 6520 7468 6520 6d6f 6465 6c20 6578 6563  e the model exec
+000126d0: 7574 696f 6e2e 0a20 2020 2020 2020 2022  ution..        "
+000126e0: 2222 0a20 2020 2020 2020 2023 2043 6865  "".        # Che
+000126f0: 636b 2074 6861 7420 7468 6520 756e 6465  ck that the unde
+00012700: 726c 7969 6e67 2073 6b6c 6561 726e 206d  rlying sklearn m
+00012710: 6f64 656c 2068 6173 2062 6565 6e20 7365  odel has been se
+00012720: 7420 616e 6420 6669 740a 2020 2020 2020  t and fit.      
+00012730: 2020 6173 7365 7274 2073 656c 662e 736b    assert self.sk
+00012740: 6c65 6172 6e5f 6d6f 6465 6c20 6973 206e  learn_model is n
+00012750: 6f74 204e 6f6e 652c 2073 656c 662e 5f73  ot None, self._s
+00012760: 6b6c 6561 726e 5f6d 6f64 656c 5f69 735f  klearn_model_is_
+00012770: 6e6f 745f 6669 7474 6564 5f65 7272 6f72  not_fitted_error
+00012780: 5f6d 6573 7361 6765 2829 0a0a 2020 2020  _message()..    
+00012790: 2020 2020 7365 6c66 2e6f 6e6e 785f 6d6f      self.onnx_mo
+000127a0: 6465 6c5f 203d 2068 625f 636f 6e76 6572  del_ = hb_conver
+000127b0: 7428 0a20 2020 2020 2020 2020 2020 2073  t(.            s
+000127c0: 656c 662e 736b 6c65 6172 6e5f 6d6f 6465  elf.sklearn_mode
+000127d0: 6c2c 0a20 2020 2020 2020 2020 2020 2062  l,.            b
+000127e0: 6163 6b65 6e64 3d22 6f6e 6e78 222c 0a20  ackend="onnx",. 
+000127f0: 2020 2020 2020 2020 2020 2074 6573 745f             test_
+00012800: 696e 7075 743d 7465 7374 5f69 6e70 7574  input=test_input
+00012810: 2c0a 2020 2020 2020 2020 2020 2020 6578  ,.            ex
+00012820: 7472 615f 636f 6e66 6967 3d7b 0a20 2020  tra_config={.   
+00012830: 2020 2020 2020 2020 2020 2020 2022 6f6e               "on
+00012840: 6e78 5f74 6172 6765 745f 6f70 7365 7422  nx_target_opset"
+00012850: 3a20 4f50 5345 545f 5645 5253 494f 4e5f  : OPSET_VERSION_
+00012860: 464f 525f 4f4e 4e58 5f45 5850 4f52 542c  FOR_ONNX_EXPORT,
+00012870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012880: 2023 2070 796c 696e 743a 2064 6973 6162   # pylint: disab
+00012890: 6c65 2d6e 6578 743d 7072 6f74 6563 7465  le-next=protecte
+000128a0: 642d 6163 6365 7373 2c20 6e6f 2d6d 656d  d-access, no-mem
+000128b0: 6265 720a 2020 2020 2020 2020 2020 2020  ber.            
+000128c0: 2020 2020 636f 6e73 7461 6e74 732e 4241      constants.BA
+000128d0: 5443 485f 5349 5a45 3a20 7365 6c66 2e73  TCH_SIZE: self.s
+000128e0: 6b6c 6561 726e 5f6d 6f64 656c 2e5f 6669  klearn_model._fi
+000128f0: 745f 582e 7368 6170 655b 305d 2c0a 2020  t_X.shape[0],.  
+00012900: 2020 2020 2020 2020 2020 7d2c 0a20 2020            },.   
+00012910: 2020 2020 2029 2e6d 6f64 656c 0a0a 2020       ).model..  
+00012920: 2020 2020 2020 7365 6c66 2e5f 636c 6561        self._clea
+00012930: 6e5f 6772 6170 6828 290a 0a20 2020 2064  n_graph()..    d
+00012940: 6566 205f 636c 6561 6e5f 6772 6170 6828  ef _clean_graph(
+00012950: 7365 6c66 2920 2d3e 204e 6f6e 653a 0a20  self) -> None:. 
+00012960: 2020 2020 2020 2022 2222 436c 6561 6e20         """Clean 
+00012970: 7468 6520 4f4e 4e58 2067 7261 7068 2066  the ONNX graph f
+00012980: 726f 6d20 756e 6465 7369 7265 6420 6e6f  rom undesired no
+00012990: 6465 732e 2222 220a 2020 2020 2020 2020  des.""".        
+000129a0: 6173 7365 7274 2073 656c 662e 6f6e 6e78  assert self.onnx
+000129b0: 5f6d 6f64 656c 5f20 6973 206e 6f74 204e  _model_ is not N
+000129c0: 6f6e 652c 2073 656c 662e 5f69 735f 6e6f  one, self._is_no
+000129d0: 745f 6669 7474 6564 5f65 7272 6f72 5f6d  t_fitted_error_m
+000129e0: 6573 7361 6765 2829 0a0a 2020 2020 2020  essage()..      
+000129f0: 2020 2320 5265 6d6f 7665 2063 6173 7420    # Remove cast 
+00012a00: 6f70 6572 6174 6f72 7320 6173 2074 6865  operators as the
+00012a10: 7920 6172 6520 6e6f 7420 6e65 6564 6564  y are not needed
+00012a20: 0a20 2020 2020 2020 2072 656d 6f76 655f  .        remove_
+00012a30: 6e6f 6465 5f74 7970 6573 286f 6e6e 785f  node_types(onnx_
+00012a40: 6d6f 6465 6c3d 7365 6c66 2e6f 6e6e 785f  model=self.onnx_
+00012a50: 6d6f 6465 6c5f 2c20 6f70 5f74 7970 6573  model_, op_types
+00012a60: 5f74 6f5f 7265 6d6f 7665 3d5b 2243 6173  _to_remove=["Cas
+00012a70: 7422 5d29 0a0a 2020 2020 6465 6620 6669  t"])..    def fi
+00012a80: 7428 7365 6c66 2c20 583a 2044 6174 612c  t(self, X: Data,
+00012a90: 2079 3a20 5461 7267 6574 2c20 2a2a 6669   y: Target, **fi
+00012aa0: 745f 7061 7261 6d65 7465 7273 293a 0a20  t_parameters):. 
+00012ab0: 2020 2020 2020 2023 2052 6573 6574 2066         # Reset f
+00012ac0: 6f72 2064 6f75 626c 6520 6669 740a 2020  or double fit.  
+00012ad0: 2020 2020 2020 7365 6c66 2e5f 6973 5f66        self._is_f
+00012ae0: 6974 7465 6420 3d20 4661 6c73 650a 2020  itted = False.  
+00012af0: 2020 2020 2020 7365 6c66 2e69 6e70 7574        self.input
+00012b00: 5f71 7561 6e74 697a 6572 7320 3d20 5b5d  _quantizers = []
+00012b10: 0a20 2020 2020 2020 2073 656c 662e 6f75  .        self.ou
+00012b20: 7470 7574 5f71 7561 6e74 697a 6572 7320  tput_quantizers 
+00012b30: 3d20 5b5d 0a0a 2020 2020 2020 2020 2320  = []..        # 
+00012b40: 4b4e 6569 6768 626f 7273 2068 616e 646c  KNeighbors handl
+00012b50: 6573 206d 756c 7469 2d6c 6162 656c 7320  es multi-labels 
+00012b60: 6461 7461 0a20 2020 2020 2020 2058 2c20  data.        X, 
+00012b70: 7920 3d20 6368 6563 6b5f 585f 795f 616e  y = check_X_y_an
+00012b80: 645f 6173 7365 7274 5f6d 756c 7469 5f6f  d_assert_multi_o
+00012b90: 7574 7075 7428 582c 2079 290a 0a20 2020  utput(X, y)..   
+00012ba0: 2020 2020 2023 2046 6974 2074 6865 2073       # Fit the s
+00012bb0: 6369 6b69 742d 6c65 6172 6e20 6d6f 6465  cikit-learn mode
+00012bc0: 6c0a 2020 2020 2020 2020 7365 6c66 2e5f  l.        self._
+00012bd0: 6669 745f 736b 6c65 6172 6e5f 6d6f 6465  fit_sklearn_mode
+00012be0: 6c28 582c 2079 2c20 2a2a 6669 745f 7061  l(X, y, **fit_pa
+00012bf0: 7261 6d65 7465 7273 290a 0a20 2020 2020  rameters)..     
+00012c00: 2020 2023 2043 6865 636b 2074 6861 7420     # Check that 
+00012c10: 7468 6520 756e 6465 726c 7969 6e67 2073  the underlying s
+00012c20: 6b6c 6561 726e 206d 6f64 656c 2068 6173  klearn model has
+00012c30: 2062 6565 6e20 7365 7420 616e 6420 6669   been set and fi
+00012c40: 740a 2020 2020 2020 2020 6173 7365 7274  t.        assert
+00012c50: 2073 656c 662e 736b 6c65 6172 6e5f 6d6f   self.sklearn_mo
+00012c60: 6465 6c20 6973 206e 6f74 204e 6f6e 652c  del is not None,
+00012c70: 2073 656c 662e 5f73 6b6c 6561 726e 5f6d   self._sklearn_m
+00012c80: 6f64 656c 5f69 735f 6e6f 745f 6669 7474  odel_is_not_fitt
+00012c90: 6564 5f65 7272 6f72 5f6d 6573 7361 6765  ed_error_message
+00012ca0: 2829 0a0a 2020 2020 2020 2020 2320 5265  ()..        # Re
+00012cb0: 7472 6965 7665 2074 6865 204f 4e4e 5820  trieve the ONNX 
+00012cc0: 6772 6170 680a 2020 2020 2020 2020 7365  graph.        se
+00012cd0: 6c66 2e5f 7365 745f 6f6e 6e78 5f6d 6f64  lf._set_onnx_mod
+00012ce0: 656c 2858 290a 0a20 2020 2020 2020 2023  el(X)..        #
+00012cf0: 2051 7561 6e74 697a 6520 7468 6520 696e   Quantize the in
+00012d00: 7075 7473 2061 6e64 2073 746f 7265 2074  puts and store t
+00012d10: 6865 2061 7373 6f63 6961 7465 6420 7175  he associated qu
+00012d20: 616e 7469 7a65 720a 2020 2020 2020 2020  antizer.        
+00012d30: 696e 7075 745f 6f70 7469 6f6e 7320 3d20  input_options = 
+00012d40: 5175 616e 7469 7a61 7469 6f6e 4f70 7469  QuantizationOpti
+00012d50: 6f6e 7328 6e5f 6269 7473 3d73 656c 662e  ons(n_bits=self.
+00012d60: 6e5f 6269 7473 2c20 6973 5f73 6967 6e65  n_bits, is_signe
+00012d70: 643d 5472 7565 290a 2020 2020 2020 2020  d=True).        
+00012d80: 715f 696e 7075 7473 203d 2051 7561 6e74  q_inputs = Quant
+00012d90: 697a 6564 4172 7261 7928 6e5f 6269 7473  izedArray(n_bits
+00012da0: 3d73 656c 662e 6e5f 6269 7473 2c20 7661  =self.n_bits, va
+00012db0: 6c75 6573 3d58 2c20 6f70 7469 6f6e 733d  lues=X, options=
+00012dc0: 696e 7075 745f 6f70 7469 6f6e 7329 0a20  input_options). 
+00012dd0: 2020 2020 2020 2069 6e70 7574 5f71 7561         input_qua
+00012de0: 6e74 697a 6572 203d 2071 5f69 6e70 7574  ntizer = q_input
+00012df0: 732e 7175 616e 7469 7a65 720a 2020 2020  s.quantizer.    
+00012e00: 2020 2020 7365 6c66 2e69 6e70 7574 5f71      self.input_q
+00012e10: 7561 6e74 697a 6572 732e 6170 7065 6e64  uantizers.append
+00012e20: 2869 6e70 7574 5f71 7561 6e74 697a 6572  (input_quantizer
+00012e30: 290a 0a20 2020 2020 2020 2023 2051 7561  )..        # Qua
+00012e40: 6e74 697a 6520 7468 6520 5f66 6974 5f58  ntize the _fit_X
+00012e50: 2061 6e64 2073 746f 7265 2074 6865 2061   and store the a
+00012e60: 7373 6f63 6961 7465 6420 7175 616e 7469  ssociated quanti
+00012e70: 7a65 720a 2020 2020 2020 2020 2320 7079  zer.        # py
+00012e80: 6c69 6e74 3a20 6469 7361 626c 652d 6e65  lint: disable-ne
+00012e90: 7874 3d70 726f 7465 6374 6564 2d61 6363  xt=protected-acc
+00012ea0: 6573 730a 2020 2020 2020 2020 5f66 6974  ess.        _fit
+00012eb0: 5f58 203d 2073 656c 662e 736b 6c65 6172  _X = self.sklear
+00012ec0: 6e5f 6d6f 6465 6c2e 5f66 6974 5f58 0a20  n_model._fit_X. 
+00012ed0: 2020 2020 2020 2023 2057 6520 6173 7375         # We assu
+00012ee0: 6d65 2074 6861 7420 7468 6520 696e 7075  me that the inpu
+00012ef0: 7473 2068 6176 6520 7468 6520 7361 6d65  ts have the same
+00012f00: 2064 6973 7472 6962 7574 696f 6e20 6173   distribution as
+00012f10: 2074 6865 205f 6669 745f 580a 2020 2020   the _fit_X.    
+00012f20: 2020 2020 715f 6669 745f 5820 3d20 5175      q_fit_X = Qu
+00012f30: 616e 7469 7a65 6441 7272 6179 280a 2020  antizedArray(.  
+00012f40: 2020 2020 2020 2020 2020 6e5f 6269 7473            n_bits
+00012f50: 3d73 656c 662e 6e5f 6269 7473 2c0a 2020  =self.n_bits,.  
+00012f60: 2020 2020 2020 2020 2020 7661 6c75 6573            values
+00012f70: 3d6e 756d 7079 2e65 7870 616e 645f 6469  =numpy.expand_di
+00012f80: 6d73 285f 6669 745f 582c 2061 7869 733d  ms(_fit_X, axis=
+00012f90: 3129 2069 6620 6c65 6e28 5f66 6974 5f58  1) if len(_fit_X
+00012fa0: 2e73 6861 7065 2920 3d3d 2031 2065 6c73  .shape) == 1 els
+00012fb0: 6520 5f66 6974 5f58 2c0a 2020 2020 2020  e _fit_X,.      
+00012fc0: 2020 2020 2020 6f70 7469 6f6e 733d 696e        options=in
+00012fd0: 7075 745f 6f70 7469 6f6e 732c 0a20 2020  put_options,.   
+00012fe0: 2020 2020 2029 0a20 2020 2020 2020 2073       ).        s
+00012ff0: 656c 662e 5f71 5f66 6974 5f58 203d 2071  elf._q_fit_X = q
+00013000: 5f66 6974 5f58 2e71 7661 6c75 6573 0a20  _fit_X.qvalues. 
+00013010: 2020 2020 2020 2073 656c 662e 5f71 5f66         self._q_f
+00013020: 6974 5f58 5f71 7561 6e74 697a 6572 203d  it_X_quantizer =
+00013030: 2071 5f66 6974 5f58 2e71 7561 6e74 697a   q_fit_X.quantiz
+00013040: 6572 0a0a 2020 2020 2020 2020 2320 6d79  er..        # my
+00013050: 7079 0a20 2020 2020 2020 2061 7373 6572  py.        asser
+00013060: 7420 7365 6c66 2e5f 715f 6669 745f 585f  t self._q_fit_X_
+00013070: 7175 616e 7469 7a65 722e 7363 616c 6520  quantizer.scale 
+00013080: 6973 206e 6f74 204e 6f6e 650a 0a20 2020  is not None..   
+00013090: 2020 2020 2073 656c 662e 5f79 203d 206e       self._y = n
+000130a0: 756d 7079 2e61 7272 6179 2879 290a 0a20  umpy.array(y).. 
+000130b0: 2020 2020 2020 2023 2057 6520 6173 7375         # We assu
+000130c0: 6d65 2074 6861 7420 7468 6520 7175 6572  me that the quer
+000130d0: 7920 6861 7320 7468 6520 7361 6d65 2064  y has the same d
+000130e0: 6973 7472 6962 7574 696f 6e20 6173 2074  istribution as t
+000130f0: 6865 2064 6174 6120 696e 205f 585f 6669  he data in _X_fi
+00013100: 742e 0a20 2020 2020 2020 2023 2074 6865  t..        # the
+00013110: 7265 666f 7265 2c20 7468 6579 2075 7365  refore, they use
+00013120: 2074 6865 2073 616d 6520 7363 616c 696e   the same scalin
+00013130: 6720 616e 6420 7a65 726f 2070 6f69 6e74  g and zero point
+00013140: 2e0a 2020 2020 2020 2020 2320 6874 7470  ..        # http
+00013150: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
+00013160: 732f 3137 3132 2e30 3538 3737 0a0a 2020  s/1712.05877..  
+00013170: 2020 2020 2020 7365 6c66 2e6f 7574 7075        self.outpu
+00013180: 745f 7175 616e 745f 7061 7261 6d73 203d  t_quant_params =
+00013190: 2055 6e69 666f 726d 5175 616e 7469 7a61   UniformQuantiza
+000131a0: 7469 6f6e 5061 7261 6d65 7465 7273 280a  tionParameters(.
+000131b0: 2020 2020 2020 2020 2020 2020 7363 616c              scal
+000131c0: 653d 7365 6c66 2e5f 715f 6669 745f 585f  e=self._q_fit_X_
+000131d0: 7175 616e 7469 7a65 722e 7363 616c 652c  quantizer.scale,
+000131e0: 0a20 2020 2020 2020 2020 2020 207a 6572  .            zer
+000131f0: 6f5f 706f 696e 743d 7365 6c66 2e5f 715f  o_point=self._q_
+00013200: 6669 745f 585f 7175 616e 7469 7a65 722e  fit_X_quantizer.
+00013210: 7a65 726f 5f70 6f69 6e74 2c0a 2020 2020  zero_point,.    
+00013220: 2020 2020 2020 2020 6f66 6673 6574 3d30          offset=0
+00013230: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+00013240: 2020 2020 206f 7574 7075 745f 7175 616e       output_quan
+00013250: 7469 7a65 7220 3d20 556e 6966 6f72 6d51  tizer = UniformQ
+00013260: 7561 6e74 697a 6572 2870 6172 616d 733d  uantizer(params=
+00013270: 7365 6c66 2e6f 7574 7075 745f 7175 616e  self.output_quan
+00013280: 745f 7061 7261 6d73 2c20 6e6f 5f63 6c69  t_params, no_cli
+00013290: 7070 696e 673d 5472 7565 290a 0a20 2020  pping=True)..   
+000132a0: 2020 2020 2061 7373 6572 7420 6f75 7470       assert outp
+000132b0: 7574 5f71 7561 6e74 697a 6572 2e7a 6572  ut_quantizer.zer
+000132c0: 6f5f 706f 696e 7420 6973 206e 6f74 204e  o_point is not N
+000132d0: 6f6e 650a 2020 2020 2020 2020 7365 6c66  one.        self
+000132e0: 2e6f 7574 7075 745f 7175 616e 7469 7a65  .output_quantize
+000132f0: 7273 2e61 7070 656e 6428 6f75 7470 7574  rs.append(output
+00013300: 5f71 7561 6e74 697a 6572 290a 0a20 2020  _quantizer)..   
+00013310: 2020 2020 2023 2055 7064 6174 696e 6720       # Updating 
+00013320: 706f 7374 2d70 726f 6365 7373 696e 6720  post-processing 
+00013330: 7061 7261 6d65 7465 7273 0a20 2020 2020  parameters.     
+00013340: 2020 2073 656c 662e 5f73 6574 5f70 6f73     self._set_pos
+00013350: 745f 7072 6f63 6573 7369 6e67 5f70 6172  t_processing_par
+00013360: 616d 7328 290a 0a20 2020 2020 2020 2073  ams()..        s
+00013370: 656c 662e 5f69 735f 6669 7474 6564 203d  elf._is_fitted =
+00013380: 2054 7275 650a 0a20 2020 2020 2020 2072   True..        r
+00013390: 6574 7572 6e20 7365 6c66 0a0a 2020 2020  eturn self..    
+000133a0: 6465 6620 7175 616e 7469 7a65 5f69 6e70  def quantize_inp
+000133b0: 7574 2873 656c 662c 2058 3a20 6e75 6d70  ut(self, X: nump
+000133c0: 792e 6e64 6172 7261 7929 202d 3e20 6e75  y.ndarray) -> nu
+000133d0: 6d70 792e 6e64 6172 7261 793a 0a20 2020  mpy.ndarray:.   
+000133e0: 2020 2020 2073 656c 662e 6368 6563 6b5f       self.check_
+000133f0: 6d6f 6465 6c5f 6973 5f66 6974 7465 6428  model_is_fitted(
+00013400: 290a 2020 2020 2020 2020 715f 5820 3d20  ).        q_X = 
+00013410: 7365 6c66 2e69 6e70 7574 5f71 7561 6e74  self.input_quant
+00013420: 697a 6572 735b 305d 2e71 7561 6e74 2858  izers[0].quant(X
+00013430: 290a 0a20 2020 2020 2020 2061 7373 6572  )..        asser
+00013440: 7420 715f 582e 6474 7970 6520 3d3d 206e  t q_X.dtype == n
+00013450: 756d 7079 2e69 6e74 3634 2c20 2249 6e70  umpy.int64, "Inp
+00013460: 7574 7320 7765 7265 206e 6f74 2071 7561  uts were not qua
+00013470: 6e74 697a 6564 2074 6f20 696e 7436 3420  ntized to int64 
+00013480: 7661 6c75 6573 220a 2020 2020 2020 2020  values".        
+00013490: 7265 7475 726e 2071 5f58 0a0a 2020 2020  return q_X..    
+000134a0: 6465 6620 6465 7175 616e 7469 7a65 5f6f  def dequantize_o
+000134b0: 7574 7075 7428 7365 6c66 2c20 715f 795f  utput(self, q_y_
+000134c0: 7072 6564 733a 206e 756d 7079 2e6e 6461  preds: numpy.nda
+000134d0: 7272 6179 2920 2d3e 206e 756d 7079 2e6e  rray) -> numpy.n
+000134e0: 6461 7272 6179 3a0a 2020 2020 2020 2020  darray:.        
+000134f0: 7365 6c66 2e63 6865 636b 5f6d 6f64 656c  self.check_model
+00013500: 5f69 735f 6669 7474 6564 2829 0a20 2020  _is_fitted().   
+00013510: 2020 2020 2023 2057 6520 636f 6d70 7574       # We comput
+00013520: 6520 7468 6520 736f 7274 6564 2061 7267  e the sorted arg
+00013530: 6d61 7820 696e 2046 4845 2c20 7768 6963  max in FHE, whic
+00013540: 6820 6172 6520 696e 7465 6765 7273 2e0a  h are integers..
+00013550: 2020 2020 2020 2020 2320 4e6f 206e 6565          # No nee
+00013560: 6420 746f 2064 652d 7175 616e 7469 7a65  d to de-quantize
+00013570: 2074 6865 206f 7574 7075 7420 7661 6c75   the output valu
+00013580: 6573 0a20 2020 2020 2020 2072 6574 7572  es.        retur
+00013590: 6e20 715f 795f 7072 6564 730a 0a20 2020  n q_y_preds..   
+000135a0: 2064 6566 205f 6765 745f 6d6f 6475 6c65   def _get_module
+000135b0: 5f74 6f5f 636f 6d70 696c 6528 7365 6c66  _to_compile(self
+000135c0: 2920 2d3e 2055 6e69 6f6e 5b43 6f6d 7069  ) -> Union[Compi
+000135d0: 6c65 722c 2051 7561 6e74 697a 6564 4d6f  ler, QuantizedMo
+000135e0: 6475 6c65 5d3a 0a20 2020 2020 2020 2023  dule]:.        #
+000135f0: 2044 6566 696e 6520 7468 6520 696e 6665   Define the infe
+00013600: 7265 6e63 6520 6675 6e63 7469 6f6e 2074  rence function t
+00013610: 6f20 636f 6d70 696c 652e 0a20 2020 2020  o compile..     
+00013620: 2020 2023 2054 6869 7320 6675 6e63 7469     # This functi
+00013630: 6f6e 2063 616e 206e 6569 7468 6572 2062  on can neither b
+00013640: 6520 6120 636c 6173 7320 6d65 7468 6f64  e a class method
+00013650: 206e 6f72 2061 2073 7461 7469 6320 6f6e   nor a static on
+00013660: 6520 6265 6361 7573 6520 7365 6c66 2077  e because self w
+00013670: 6520 7761 6e74 2074 6f20 6176 6f69 640a  e want to avoid.
+00013680: 2020 2020 2020 2020 2320 6861 7669 6e67          # having
+00013690: 2073 656c 6620 6173 2061 2070 6172 616d   self as a param
+000136a0: 6574 6572 2077 6869 6c65 2073 7469 6c6c  eter while still
+000136b0: 2062 6569 6e67 2061 626c 6520 746f 2061   being able to a
+000136c0: 6363 6573 7320 736f 6d65 206f 6620 6974  ccess some of it
+000136d0: 7320 6174 7472 6962 7574 650a 2020 2020  s attribute.    
+000136e0: 2020 2020 6465 6620 696e 6665 7265 6e63      def inferenc
+000136f0: 655f 746f 5f63 6f6d 7069 6c65 2871 5f58  e_to_compile(q_X
+00013700: 3a20 6e75 6d70 792e 6e64 6172 7261 7929  : numpy.ndarray)
+00013710: 202d 3e20 6e75 6d70 792e 6e64 6172 7261   -> numpy.ndarra
+00013720: 793a 0a20 2020 2020 2020 2020 2020 2022  y:.            "
+00013730: 2222 436f 6d70 696c 6520 7468 6520 6369  ""Compile the ci
+00013740: 7263 7569 7420 696e 2046 4845 2075 7369  rcuit in FHE usi
+00013750: 6e67 206f 6e6c 7920 7468 6520 696e 7075  ng only the inpu
+00013760: 7473 2061 7320 7061 7261 6d65 7465 7273  ts as parameters
+00013770: 2e0a 0a20 2020 2020 2020 2020 2020 2041  ...            A
+00013780: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00013790: 2020 2020 2071 5f58 2028 6e75 6d70 792e       q_X (numpy.
+000137a0: 6e64 6172 7261 7929 3a20 5468 6520 7175  ndarray): The qu
+000137b0: 616e 7469 7a65 6420 696e 7075 7420 6461  antized input da
+000137c0: 7461 0a0a 2020 2020 2020 2020 2020 2020  ta..            
+000137d0: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+000137e0: 2020 2020 2020 2020 206e 756d 7079 2e6e           numpy.n
+000137f0: 6461 7272 6179 3a20 5468 6520 6369 7263  darray: The circ
+00013800: 7569 7420 6973 206f 7574 7075 7473 2e0a  uit is outputs..
+00013810: 2020 2020 2020 2020 2020 2020 2222 220a              """.
+00013820: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00013830: 726e 2073 656c 662e 5f69 6e66 6572 656e  rn self._inferen
+00013840: 6365 2871 5f58 290a 0a20 2020 2020 2020  ce(q_X)..       
+00013850: 2023 2043 7265 6174 6520 7468 6520 636f   # Create the co
+00013860: 6d70 696c 6572 2069 6e73 7461 6e63 650a  mpiler instance.
+00013870: 2020 2020 2020 2020 636f 6d70 696c 6572          compiler
+00013880: 203d 2043 6f6d 7069 6c65 7228 696e 6665   = Compiler(infe
+00013890: 7265 6e63 655f 746f 5f63 6f6d 7069 6c65  rence_to_compile
+000138a0: 2c20 7b22 715f 5822 3a20 2265 6e63 7279  , {"q_X": "encry
+000138b0: 7074 6564 227d 290a 0a20 2020 2020 2020  pted"})..       
+000138c0: 2072 6574 7572 6e20 636f 6d70 696c 6572   return compiler
+000138d0: 0a0a 2020 2020 4073 7461 7469 636d 6574  ..    @staticmet
+000138e0: 686f 640a 2020 2020 6465 6620 6d61 6a6f  hod.    def majo
+000138f0: 7269 7479 5f76 6f74 6528 6e65 6172 6573  rity_vote(neares
+00013900: 745f 636c 6173 7365 733a 206e 756d 7079  t_classes: numpy
+00013910: 2e6e 6461 7272 6179 293a 0a20 2020 2020  .ndarray):.     
+00013920: 2020 2022 2222 4465 7465 726d 696e 6520     """Determine 
+00013930: 7468 6520 6d6f 7374 2063 6f6d 6d6f 6e20  the most common 
+00013940: 636c 6173 7320 616d 6f6e 6720 6e65 6172  class among near
+00013950: 6573 7420 6e65 6967 6862 6f72 7366 6f72  est neighborsfor
+00013960: 2065 6163 6820 7175 6572 792e 0a0a 2020   each query...  
+00013970: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+00013980: 2020 2020 2020 2020 6e65 6172 6573 745f          nearest_
+00013990: 636c 6173 7365 7320 286e 756d 7079 2e6e  classes (numpy.n
+000139a0: 6461 7272 6179 293a 2054 6865 2063 6c61  darray): The cla
+000139b0: 7373 206c 6162 656c 7320 6f66 2074 6865  ss labels of the
+000139c0: 206e 6561 7265 7374 206e 6569 6768 626f   nearest neighbo
+000139d0: 7273 2066 6f72 2061 2071 7565 7279 0a0a  rs for a query..
+000139e0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+000139f0: 0a20 2020 2020 2020 2020 2020 206e 756d  .            num
+00013a00: 7079 2e6e 6461 7272 6179 3a20 5468 6520  py.ndarray: The 
+00013a10: 6d61 6a6f 7269 7479 2d76 6f74 6564 2063  majority-voted c
+00013a20: 6c61 7373 206c 6162 656c 2066 6f72 2074  lass label for t
+00013a30: 6865 2063 6f72 7265 7370 6f6e 6469 6e67  he corresponding
+00013a40: 2071 7565 7279 2e0a 2020 2020 2020 2020   query..        
+00013a50: 2222 220a 2020 2020 2020 2020 636c 6173  """.        clas
+00013a60: 735f 636f 756e 7473 203d 206e 756d 7079  s_counts = numpy
+00013a70: 2e62 696e 636f 756e 7428 6e65 6172 6573  .bincount(neares
+00013a80: 745f 636c 6173 7365 7329 0a20 2020 2020  t_classes).     
+00013a90: 2020 206d 616a 6f72 6974 795f 766f 7465     majority_vote
+00013aa0: 7320 3d20 6e75 6d70 792e 6172 676d 6178  s = numpy.argmax
+00013ab0: 2863 6c61 7373 5f63 6f75 6e74 7329 0a0a  (class_counts)..
+00013ac0: 2020 2020 2020 2020 7265 7475 726e 206d          return m
+00013ad0: 616a 6f72 6974 795f 766f 7465 730a 0a20  ajority_votes.. 
+00013ae0: 2020 2064 6566 205f 696e 6665 7265 6e63     def _inferenc
+00013af0: 6528 7365 6c66 2c20 715f 583a 206e 756d  e(self, q_X: num
+00013b00: 7079 2e6e 6461 7272 6179 2920 2d3e 206e  py.ndarray) -> n
+00013b10: 756d 7079 2e6e 6461 7272 6179 3a0a 2020  umpy.ndarray:.  
+00013b20: 2020 2020 2020 2222 2249 6e66 6572 656e        """Inferen
+00013b30: 6365 2066 756e 6374 696f 6e2e 0a0a 2020  ce function...  
+00013b40: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+00013b50: 2020 2020 2020 2020 715f 5820 286e 756d          q_X (num
+00013b60: 7079 2e6e 6461 7272 6179 293a 2054 6865  py.ndarray): The
+00013b70: 2071 7561 6e74 697a 6564 2069 6e70 7574   quantized input
+00013b80: 2076 616c 7565 732e 0a0a 2020 2020 2020   values...      
+00013b90: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00013ba0: 2020 2020 2020 206e 756d 7079 2e6e 6461         numpy.nda
+00013bb0: 7272 6179 3a20 5468 6520 7175 616e 7469  rray: The quanti
+00013bc0: 7a65 6420 7072 6564 6963 7465 6420 7661  zed predicted va
+00013bd0: 6c75 6573 2e0a 2020 2020 2020 2020 2222  lues..        ""
+00013be0: 220a 2020 2020 2020 2020 6173 7365 7274  ".        assert
+00013bf0: 2073 656c 662e 5f71 5f66 6974 5f58 5f71   self._q_fit_X_q
+00013c00: 7561 6e74 697a 6572 2069 7320 6e6f 7420  uantizer is not 
+00013c10: 4e6f 6e65 2c20 7365 6c66 2e5f 6973 5f6e  None, self._is_n
+00013c20: 6f74 5f66 6974 7465 645f 6572 726f 725f  ot_fitted_error_
+00013c30: 6d65 7373 6167 6528 290a 0a20 2020 2020  message()..     
+00013c40: 2020 2064 6566 2070 6169 7277 6973 655f     def pairwise_
+00013c50: 6575 636c 6964 6561 6e5f 6469 7374 616e  euclidean_distan
+00013c60: 6365 2871 5f58 293a 0a20 2020 2020 2020  ce(q_X):.       
+00013c70: 2020 2020 2023 2031 2e20 5061 6972 7769       # 1. Pairwi
+00013c80: 7365 2065 7563 6c69 6465 616e 2064 6973  se euclidean dis
+00013c90: 7461 6e63 650a 2020 2020 2020 2020 2020  tance.          
+00013ca0: 2020 2320 6469 7374 2878 2c20 7929 203d    # dist(x, y) =
+00013cb0: 2073 7172 7428 646f 7428 782c 2078 2920   sqrt(dot(x, x) 
+00013cc0: 2d20 3220 2a20 646f 7428 782c 2079 2920  - 2 * dot(x, y) 
+00013cd0: 2b20 646f 7428 792c 2079 2929 0a20 2020  + dot(y, y)).   
+00013ce0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00013cf0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+00013d00: 2020 6e75 6d70 792e 7375 6d28 715f 582a    numpy.sum(q_X*
+00013d10: 2a32 2c20 6178 6973 3d31 2c20 6b65 6570  *2, axis=1, keep
+00013d20: 6469 6d73 3d54 7275 6529 0a20 2020 2020  dims=True).     
+00013d30: 2020 2020 2020 2020 2020 202d 2032 202a             - 2 *
+00013d40: 2071 5f58 2040 2073 656c 662e 5f71 5f66   q_X @ self._q_f
+00013d50: 6974 5f58 2e54 0a20 2020 2020 2020 2020  it_X.T.         
+00013d60: 2020 2020 2020 202b 206e 756d 7079 2e65         + numpy.e
+00013d70: 7870 616e 645f 6469 6d73 286e 756d 7079  xpand_dims(numpy
+00013d80: 2e73 756d 2873 656c 662e 5f71 5f66 6974  .sum(self._q_fit
+00013d90: 5f58 2a2a 322c 2061 7869 733d 3129 2c20  _X**2, axis=1), 
+00013da0: 3029 0a20 2020 2020 2020 2020 2020 2029  0).            )
+00013db0: 0a0a 2020 2020 2020 2020 6465 6620 746f  ..        def to
+00013dc0: 706b 5f73 6f72 7469 6e67 2878 2c20 6c61  pk_sorting(x, la
+00013dd0: 6265 6c73 293a 0a20 2020 2020 2020 2020  bels):.         
+00013de0: 2020 2022 2222 4172 6773 6f72 7420 696e     """Argsort in
+00013df0: 2046 4845 2e0a 0a20 2020 2020 2020 2020   FHE...         
+00013e00: 2020 2054 696d 6520 636f 6d70 6c65 7869     Time complexi
+00013e10: 7479 3a20 4f28 6e6c 6f67 c2b2 286b 2929  ty: O(nlog..(k))
+00013e20: 0a0a 2020 2020 2020 2020 2020 2020 4172  ..            Ar
+00013e30: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00013e40: 2020 2020 7820 286e 756d 7079 2e6e 6461      x (numpy.nda
+00013e50: 7272 6179 293a 2054 6865 2071 7561 6e74  rray): The quant
+00013e60: 697a 6564 2069 6e70 7574 2076 616c 7565  ized input value
+00013e70: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00013e80: 2020 6c61 6265 6c73 2028 6e75 6d70 792e    labels (numpy.
+00013e90: 6e64 6172 7261 7929 3a20 5468 6520 6c61  ndarray): The la
+00013ea0: 6265 6c73 206f 6620 7468 6520 7472 6169  bels of the trai
+00013eb0: 6e69 6e67 2064 6174 612d 7365 740a 0a20  ning data-set.. 
+00013ec0: 2020 2020 2020 2020 2020 2052 6574 7572             Retur
+00013ed0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00013ee0: 2020 2020 6e75 6d70 792e 6e64 6172 7261      numpy.ndarra
+00013ef0: 793a 2054 6865 2061 7267 736f 7274 2e0a  y: The argsort..
+00013f00: 2020 2020 2020 2020 2020 2020 2222 220a              """.
+00013f10: 0a20 2020 2020 2020 2020 2020 2064 6566  .            def
+00013f20: 2067 6174 6865 7231 6428 782c 2069 6e64   gather1d(x, ind
+00013f30: 6963 6573 293a 0a20 2020 2020 2020 2020  ices):.         
+00013f40: 2020 2020 2020 2022 2222 5365 6c65 6374         """Select
+00013f50: 2065 6c65 6d65 6e74 7320 6672 6f6d 2074   elements from t
+00013f60: 6865 2069 6e70 7574 2061 7272 6179 2060  he input array `
+00013f70: 7860 2075 7369 6e67 2074 6865 2070 726f  x` using the pro
+00013f80: 7669 6465 6420 6069 6e64 6963 6573 602e  vided `indices`.
+00013f90: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00013fa0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00013fb0: 2020 2020 2020 2020 2020 2020 7820 286e              x (n
+00013fc0: 756d 7079 2e6e 6461 7272 6179 293a 2054  umpy.ndarray): T
+00013fd0: 6865 2065 6e63 7279 7074 6564 2069 6e70  he encrypted inp
+00013fe0: 7574 2061 7272 6179 0a20 2020 2020 2020  ut array.       
+00013ff0: 2020 2020 2020 2020 2020 2020 2069 6e64               ind
+00014000: 6963 6573 2028 6e75 6d70 792e 6e64 6172  ices (numpy.ndar
+00014010: 7261 7929 3a20 5468 6520 6465 7369 7265  ray): The desire
+00014020: 6420 696e 6465 7865 730a 0a20 2020 2020  d indexes..     
+00014030: 2020 2020 2020 2020 2020 2052 6574 7572             Retur
+00014040: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00014050: 2020 2020 2020 2020 6e75 6d70 792e 6e64          numpy.nd
+00014060: 6172 7261 793a 2054 6865 2073 656c 6563  array: The selec
+00014070: 7465 6420 656e 6372 7970 7465 6420 696e  ted encrypted in
+00014080: 6465 7865 732e 0a20 2020 2020 2020 2020  dexes..         
+00014090: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000140a0: 2020 2020 2020 2020 2020 2061 7272 203d             arr =
+000140b0: 205b 5d0a 2020 2020 2020 2020 2020 2020   [].            
+000140c0: 2020 2020 666f 7220 6920 696e 2069 6e64      for i in ind
+000140d0: 6963 6573 3a0a 2020 2020 2020 2020 2020  ices:.          
+000140e0: 2020 2020 2020 2020 2020 6172 722e 6170            arr.ap
+000140f0: 7065 6e64 2878 5b69 5d29 0a20 2020 2020  pend(x[i]).     
+00014100: 2020 2020 2020 2020 2020 2065 6e63 5f61             enc_a
+00014110: 7272 203d 2063 702e 6172 7261 7928 6172  rr = cp.array(ar
+00014120: 7229 0a20 2020 2020 2020 2020 2020 2020  r).             
+00014130: 2020 2072 6574 7572 6e20 656e 635f 6172     return enc_ar
+00014140: 720a 0a20 2020 2020 2020 2020 2020 2064  r..            d
+00014150: 6566 2073 6361 7474 6572 3164 2878 2c20  ef scatter1d(x, 
+00014160: 762c 2069 6e64 6963 6573 293a 0a20 2020  v, indices):.   
+00014170: 2020 2020 2020 2020 2020 2020 2022 2222               """
+00014180: 5265 6172 7261 6e67 6520 656c 656d 656e  Rearrange elemen
+00014190: 7473 206f 6620 6078 6020 7769 7468 2076  ts of `x` with v
+000141a0: 616c 7565 7320 6672 6f6d 2060 7660 2061  alues from `v` a
+000141b0: 7420 7468 6520 7370 6563 6966 6965 6420  t the specified 
+000141c0: 6069 6e64 6963 6573 602e 0a0a 2020 2020  `indices`...    
+000141d0: 2020 2020 2020 2020 2020 2020 4172 6773              Args
+000141e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000141f0: 2020 2020 2020 7820 286e 756d 7079 2e6e        x (numpy.n
+00014200: 6461 7272 6179 293a 2054 6865 2065 6e63  darray): The enc
+00014210: 7279 7074 6564 2069 6e70 7574 2061 7272  rypted input arr
+00014220: 6179 2069 6e20 7768 6963 6820 6974 656d  ay in which item
+00014230: 7320 7769 6c6c 2062 6520 7570 6461 7465  s will be update
+00014240: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
+00014250: 2020 2020 2020 7620 286e 756d 7079 2e6e        v (numpy.n
+00014260: 6461 7272 6179 293a 2054 6865 2061 7272  darray): The arr
+00014270: 6179 2063 6f6e 7461 696e 696e 6720 7661  ay containing va
+00014280: 6c75 6573 2074 6f20 6265 2069 6e73 6572  lues to be inser
+00014290: 7465 6420 696e 746f 2060 7860 0a20 2020  ted into `x`.   
+000142a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000142b0: 2020 2020 2061 7420 7468 6520 7370 6563       at the spec
+000142c0: 6966 6965 6420 6069 6e64 6963 6573 602e  ified `indices`.
+000142d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000142e0: 2020 2020 2069 6e64 6963 6573 2028 6e75       indices (nu
+000142f0: 6d70 792e 6e64 6172 7261 7929 3a20 5468  mpy.ndarray): Th
+00014300: 6520 696e 6469 6365 7320 696e 6469 6361  e indices indica
+00014310: 7469 6e67 2077 6865 7265 2074 6f20 696e  ting where to in
+00014320: 7365 7274 2074 6865 2065 6c65 6d65 6e74  sert the element
+00014330: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
+00014340: 2020 2020 2020 2020 2020 6672 6f6d 2060            from `
+00014350: 7660 2069 6e74 6f20 6078 602e 0a0a 2020  v` into `x`...  
+00014360: 2020 2020 2020 2020 2020 2020 2020 5265                Re
+00014370: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+00014380: 2020 2020 2020 2020 2020 206e 756d 7079             numpy
+00014390: 2e6e 6461 7272 6179 3a20 5468 6520 7570  .ndarray: The up
+000143a0: 6461 7465 6420 656e 6372 7970 7465 6420  dated encrypted 
+000143b0: 6078 600a 2020 2020 2020 2020 2020 2020  `x`.            
+000143c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000143d0: 2020 2020 2020 2020 666f 7220 6964 782c          for idx,
+000143e0: 2069 2069 6e20 656e 756d 6572 6174 6528   i in enumerate(
+000143f0: 696e 6469 6365 7329 3a0a 2020 2020 2020  indices):.      
+00014400: 2020 2020 2020 2020 2020 2020 2020 785b                x[
+00014410: 695d 203d 2076 5b69 6478 5d0a 2020 2020  i] = v[idx].    
+00014420: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00014430: 726e 2078 0a0a 2020 2020 2020 2020 2020  rn x..          
+00014440: 2020 636f 6d70 6172 6973 6f6e 7320 3d20    comparisons = 
+00014450: 6e75 6d70 792e 7a65 726f 7328 782e 7368  numpy.zeros(x.sh
+00014460: 6170 6529 0a20 2020 2020 2020 2020 2020  ape).           
+00014470: 206c 6162 656c 7320 3d20 6c61 6265 6c73   labels = labels
+00014480: 202b 2063 702e 7a65 726f 7328 6c61 6265   + cp.zeros(labe
+00014490: 6c73 2e73 6861 7065 290a 0a20 2020 2020  ls.shape)..     
+000144a0: 2020 2020 2020 206e 2c20 6b20 3d20 782e         n, k = x.
+000144b0: 7369 7a65 2c20 7365 6c66 2e6e 5f6e 6569  size, self.n_nei
+000144c0: 6768 626f 7273 0a20 2020 2020 2020 2020  ghbors.         
+000144d0: 2020 2023 2044 6574 6572 6d69 6e65 2074     # Determine t
+000144e0: 6865 206e 756d 6265 7220 6f66 2073 7461  he number of sta
+000144f0: 6765 7320 666f 7220 6120 7365 7175 656e  ges for a sequen
+00014500: 6365 206f 6620 6c65 6e67 7468 206e 0a20  ce of length n. 
+00014510: 2020 2020 2020 2020 2020 206c 6e32 6e20             ln2n 
+00014520: 3d20 696e 7428 6e75 6d70 792e 6365 696c  = int(numpy.ceil
+00014530: 286e 756d 7079 2e6c 6f67 3228 6e29 2929  (numpy.log2(n)))
+00014540: 0a0a 2020 2020 2020 2020 2020 2020 2320  ..            # 
+00014550: 5374 6167 6520 6c6f 6f70 0a20 2020 2020  Stage loop.     
+00014560: 2020 2020 2020 2066 6f72 2074 2069 6e20         for t in 
+00014570: 7261 6e67 6528 6c6e 326e 202d 2031 2c20  range(ln2n - 1, 
+00014580: 2d31 2c20 2d31 293a 0a20 2020 2020 2020  -1, -1):.       
+00014590: 2020 2020 2020 2020 2023 2070 3a20 4465           # p: De
+000145a0: 7465 726d 696e 6573 2074 6865 2072 616e  termines the ran
+000145b0: 6765 206f 6620 696e 6465 7865 7320 746f  ge of indexes to
+000145c0: 2062 6520 636f 6d70 6172 6564 2069 6e20   be compared in 
+000145d0: 6561 6368 2070 6173 732e 0a20 2020 2020  each pass..     
+000145e0: 2020 2020 2020 2020 2020 2070 203d 2032             p = 2
+000145f0: 2a2a 740a 2020 2020 2020 2020 2020 2020  **t.            
+00014600: 2020 2020 2320 723a 204f 6666 7365 7420      # r: Offset 
+00014610: 7468 6174 2061 646a 7573 7473 2074 6865  that adjusts the
+00014620: 2072 616e 6765 206f 6620 696e 6465 7865   range of indexe
+00014630: 7320 746f 2062 6520 636f 6d70 6172 6564  s to be compared
+00014640: 2061 6e64 2073 6f72 7465 6420 696e 2065   and sorted in e
+00014650: 6163 6820 7061 7373 0a20 2020 2020 2020  ach pass.       
+00014660: 2020 2020 2020 2020 2072 203d 2030 0a20           r = 0. 
+00014670: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00014680: 2064 3a20 436f 6d70 6172 6973 6f6e 2064   d: Comparison d
+00014690: 6973 7461 6e63 6520 696e 2065 6163 6820  istance in each 
+000146a0: 7061 7373 0a20 2020 2020 2020 2020 2020  pass.           
+000146b0: 2020 2020 2064 203d 2070 0a20 2020 2020       d = p.     
+000146c0: 2020 2020 2020 2020 2020 2023 204e 756d             # Num
+000146d0: 6265 7220 6f66 2070 6173 7365 7320 666f  ber of passes fo
+000146e0: 7220 6561 6368 2073 7461 6765 0a20 2020  r each stage.   
+000146f0: 2020 2020 2020 2020 2020 2020 2066 6f72               for
+00014700: 2062 7120 696e 2072 616e 6765 286c 6e32   bq in range(ln2
+00014710: 6e20 2d20 312c 2074 202d 2031 2c20 2d31  n - 1, t - 1, -1
+00014720: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00014730: 2020 2020 2020 2077 6974 6820 6370 2e74         with cp.t
+00014740: 6167 2866 2253 7461 6765 5f7b 747d 5f70  ag(f"Stage_{t}_p
+00014750: 6173 735f 7b62 717d 2229 3a0a 2020 2020  ass_{bq}"):.    
 00014760: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014770: 2020 2077 6974 6820 6370 2e74 6167 2866     with cp.tag(f
-00014780: 2253 7461 6765 5f7b 747d 5f70 6173 735f  "Stage_{t}_pass_
-00014790: 7b62 717d 2229 3a0a 2020 2020 2020 2020  {bq}"):.        
-000147a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147b0: 7120 3d20 322a 2a62 710a 2020 2020 2020  q = 2**bq.      
-000147c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000147d0: 2020 2320 4465 7465 726d 696e 6520 7468    # Determine th
-000147e0: 6520 7261 6e67 6520 6f66 2069 6e64 6578  e range of index
-000147f0: 6573 2074 6f20 6265 2063 6f6d 7061 7265  es to be compare
-00014800: 640a 2020 2020 2020 2020 2020 2020 2020  d.              
-00014810: 2020 2020 2020 2020 2020 7261 6e67 655f            range_
-00014820: 6920 3d20 6e75 6d70 792e 6172 7261 7928  i = numpy.array(
-00014830: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014840: 2020 2020 2020 2020 2020 2020 205b 6920               [i 
-00014850: 666f 7220 6920 696e 2072 616e 6765 2830  for i in range(0
-00014860: 2c20 6e20 2d20 6429 2069 6620 6920 2620  , n - d) if i & 
-00014870: 7020 3d3d 2072 2061 6e64 2063 6f6d 7061  p == r and compa
-00014880: 7269 736f 6e73 5b69 5d20 3c20 6b5d 0a20  risons[i] < k]. 
-00014890: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148a0: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
-000148b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148c0: 2069 6620 6c65 6e28 7261 6e67 655f 6929   if len(range_i)
-000148d0: 203d 3d20 303a 0a20 2020 2020 2020 2020   == 0:.         
-000148e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000148f0: 2020 2023 2045 6467 6520 6361 7365 2c20     # Edge case, 
-00014900: 666f 7220 6b3d 310a 2020 2020 2020 2020  for k=1.        
-00014910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014920: 2020 2020 636f 6e74 696e 7565 0a0a 2020      continue..  
-00014930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014940: 2020 2020 2020 2320 5365 6c65 6374 2032        # Select 2
-00014950: 2062 6974 6f6e 6963 2073 6571 7565 6e63   bitonic sequenc
-00014960: 6573 2060 6160 2061 6e64 2060 6260 206f  es `a` and `b` o
-00014970: 6620 6c65 6e67 7468 2060 6460 0a20 2020  f length `d`.   
-00014980: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014990: 2020 2020 2023 2061 203d 2078 5b72 616e       # a = x[ran
-000149a0: 6765 5f69 5d3a 2066 6972 7374 2062 6974  ge_i]: first bit
-000149b0: 6f6e 6963 2073 6571 7565 6e63 650a 2020  onic sequence.  
-000149c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000149d0: 2020 2020 2020 2320 615f 6920 3d20 6964        # a_i = id
-000149e0: 785b 7261 6e67 655f 695d 3a20 496e 6465  x[range_i]: Inde
-000149f0: 7865 7320 6f66 2061 5f69 2065 6c65 6d65  xes of a_i eleme
-00014a00: 6e74 7320 696e 2074 6865 206f 7269 6769  nts in the origi
-00014a10: 6e61 6c20 780a 2020 2020 2020 2020 2020  nal x.          
-00014a20: 2020 2020 2020 2020 2020 2020 2020 6120                a 
-00014a30: 3d20 6761 7468 6572 3164 2878 2c20 7261  = gather1d(x, ra
-00014a40: 6e67 655f 6929 0a20 2020 2020 2020 2020  nge_i).         
-00014a50: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00014a60: 2061 5f69 203d 2067 6174 6865 7231 6428   a_i = gather1d(
-00014a70: 6964 782c 2072 616e 6765 5f69 290a 2020  idx, range_i).  
-00014a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014a90: 2020 2020 2020 2320 6220 3d20 785b 7261        # b = x[ra
-00014aa0: 6e67 655f 6920 2b20 645d 3a20 5365 636f  nge_i + d]: Seco
-00014ab0: 6e64 2062 6974 6f6e 6963 2073 6571 7565  nd bitonic seque
-00014ac0: 6e63 650a 2020 2020 2020 2020 2020 2020  nce.            
-00014ad0: 2020 2020 2020 2020 2020 2020 2320 625f              # b_
-00014ae0: 6920 3d20 6964 785b 7261 6e67 655f 6920  i = idx[range_i 
-00014af0: 2b20 645d 3a20 496e 6465 7865 7320 6f66  + d]: Indexes of
-00014b00: 2062 5f69 2065 6c65 6d65 6e74 7320 696e   b_i elements in
-00014b10: 2074 6865 206f 7269 6769 6e61 6c20 780a   the original x.
+00014770: 2020 2020 7120 3d20 322a 2a62 710a 2020      q = 2**bq.  
+00014780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014790: 2020 2020 2020 2320 4465 7465 726d 696e        # Determin
+000147a0: 6520 7468 6520 7261 6e67 6520 6f66 2069  e the range of i
+000147b0: 6e64 6578 6573 2074 6f20 6265 2063 6f6d  ndexes to be com
+000147c0: 7061 7265 640a 2020 2020 2020 2020 2020  pared.          
+000147d0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+000147e0: 6e67 655f 6920 3d20 6e75 6d70 792e 6172  nge_i = numpy.ar
+000147f0: 7261 7928 0a20 2020 2020 2020 2020 2020  ray(.           
+00014800: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014810: 205b 6920 666f 7220 6920 696e 2072 616e   [i for i in ran
+00014820: 6765 2830 2c20 6e20 2d20 6429 2069 6620  ge(0, n - d) if 
+00014830: 6920 2620 7020 3d3d 2072 2061 6e64 2063  i & p == r and c
+00014840: 6f6d 7061 7269 736f 6e73 5b69 5d20 3c20  omparisons[i] < 
+00014850: 6b5d 0a20 2020 2020 2020 2020 2020 2020  k].             
+00014860: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00014870: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014880: 2020 2020 2069 6620 6c65 6e28 7261 6e67       if len(rang
+00014890: 655f 6929 203d 3d20 303a 0a20 2020 2020  e_i) == 0:.     
+000148a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000148b0: 2020 2020 2020 2023 2045 6467 6520 6361         # Edge ca
+000148c0: 7365 2c20 666f 7220 6b3d 310a 2020 2020  se, for k=1.    
+000148d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000148e0: 2020 2020 2020 2020 636f 6e74 696e 7565          continue
+000148f0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014900: 2020 2020 2020 2020 2020 2320 5365 6c65            # Sele
+00014910: 6374 2032 2062 6974 6f6e 6963 2073 6571  ct 2 bitonic seq
+00014920: 7565 6e63 6573 2060 6160 2061 6e64 2060  uences `a` and `
+00014930: 6260 206f 6620 6c65 6e67 7468 2060 6460  b` of length `d`
+00014940: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014950: 2020 2020 2020 2020 2023 2061 203d 2078           # a = x
+00014960: 5b72 616e 6765 5f69 5d3a 2066 6972 7374  [range_i]: first
+00014970: 2062 6974 6f6e 6963 2073 6571 7565 6e63   bitonic sequenc
+00014980: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+00014990: 2020 2020 2020 2020 2020 2320 615f 6920            # a_i 
+000149a0: 3d20 6964 785b 7261 6e67 655f 695d 3a20  = idx[range_i]: 
+000149b0: 496e 6465 7865 7320 6f66 2061 5f69 2065  Indexes of a_i e
+000149c0: 6c65 6d65 6e74 7320 696e 2074 6865 206f  lements in the o
+000149d0: 7269 6769 6e61 6c20 780a 2020 2020 2020  riginal x.      
+000149e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000149f0: 2020 6120 3d20 6761 7468 6572 3164 2878    a = gather1d(x
+00014a00: 2c20 7261 6e67 655f 6929 0a20 2020 2020  , range_i).     
+00014a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014a20: 2020 2023 2061 5f69 203d 2067 6174 6865     # a_i = gathe
+00014a30: 7231 6428 6964 782c 2072 616e 6765 5f69  r1d(idx, range_i
+00014a40: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00014a50: 2020 2020 2020 2020 2020 2320 6220 3d20            # b = 
+00014a60: 785b 7261 6e67 655f 6920 2b20 645d 3a20  x[range_i + d]: 
+00014a70: 5365 636f 6e64 2062 6974 6f6e 6963 2073  Second bitonic s
+00014a80: 6571 7565 6e63 650a 2020 2020 2020 2020  equence.        
+00014a90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014aa0: 2320 625f 6920 3d20 6964 785b 7261 6e67  # b_i = idx[rang
+00014ab0: 655f 6920 2b20 645d 3a20 496e 6465 7865  e_i + d]: Indexe
+00014ac0: 7320 6f66 2062 5f69 2065 6c65 6d65 6e74  s of b_i element
+00014ad0: 7320 696e 2074 6865 206f 7269 6769 6e61  s in the origina
+00014ae0: 6c20 780a 2020 2020 2020 2020 2020 2020  l x.            
+00014af0: 2020 2020 2020 2020 2020 2020 6220 3d20              b = 
+00014b00: 6761 7468 6572 3164 2878 2c20 7261 6e67  gather1d(x, rang
+00014b10: 655f 6920 2b20 6429 0a20 2020 2020 2020  e_i + d).       
 00014b20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014b30: 2020 2020 2020 2020 6220 3d20 6761 7468          b = gath
-00014b40: 6572 3164 2878 2c20 7261 6e67 655f 6920  er1d(x, range_i 
-00014b50: 2b20 6429 0a20 2020 2020 2020 2020 2020  + d).           
-00014b60: 2020 2020 2020 2020 2020 2020 2023 2062               # b
-00014b70: 5f69 203d 2067 6174 6865 7231 6428 6964  _i = gather1d(id
-00014b80: 782c 2072 616e 6765 5f69 202b 2064 290a  x, range_i + d).
-00014b90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014ba0: 2020 2020 2020 2020 206c 6162 656c 735f           labels_
-00014bb0: 6120 3d20 6761 7468 6572 3164 286c 6162  a = gather1d(lab
-00014bc0: 656c 732c 2072 616e 6765 5f69 2920 2023  els, range_i)  #
-00014bd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014be0: 2020 2020 2020 2020 206c 6162 656c 735f           labels_
-00014bf0: 6220 3d20 6761 7468 6572 3164 286c 6162  b = gather1d(lab
-00014c00: 656c 732c 2072 616e 6765 5f69 202b 2064  els, range_i + d
-00014c10: 2920 2023 2069 6478 5b72 616e 6765 5f69  )  # idx[range_i
-00014c20: 202b 2064 5d0a 0a20 2020 2020 2020 2020   + d]..         
-00014c30: 2020 2020 2020 2020 2020 2020 2020 2077                 w
-00014c40: 6974 6820 6370 2e74 6167 2822 6469 6666  ith cp.tag("diff
-00014c50: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-00014c60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014c70: 2320 5365 6c65 6374 206d 6178 2861 2c20  # Select max(a, 
-00014c80: 6229 0a20 2020 2020 2020 2020 2020 2020  b).             
-00014c90: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00014ca0: 6966 6620 3d20 6220 2d20 610a 0a20 2020  iff = b - a..   
-00014cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014cc0: 2020 2020 2077 6974 6820 6370 2e74 6167       with cp.tag
-00014cd0: 2822 6d61 785f 7661 6c75 6522 293a 0a20  ("max_value"):. 
-00014ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014cf0: 2020 2020 2020 2020 2020 206d 6178 5f78             max_x
-00014d00: 203d 2061 202b 206e 756d 7079 2e6d 6178   = a + numpy.max
-00014d10: 696d 756d 2830 2c20 6469 6666 290a 0a20  imum(0, diff).. 
+00014b30: 2023 2062 5f69 203d 2067 6174 6865 7231   # b_i = gather1
+00014b40: 6428 6964 782c 2072 616e 6765 5f69 202b  d(idx, range_i +
+00014b50: 2064 290a 0a20 2020 2020 2020 2020 2020   d)..           
+00014b60: 2020 2020 2020 2020 2020 2020 206c 6162               lab
+00014b70: 656c 735f 6120 3d20 6761 7468 6572 3164  els_a = gather1d
+00014b80: 286c 6162 656c 732c 2072 616e 6765 5f69  (labels, range_i
+00014b90: 2920 2023 0a20 2020 2020 2020 2020 2020  )  #.           
+00014ba0: 2020 2020 2020 2020 2020 2020 206c 6162               lab
+00014bb0: 656c 735f 6220 3d20 6761 7468 6572 3164  els_b = gather1d
+00014bc0: 286c 6162 656c 732c 2072 616e 6765 5f69  (labels, range_i
+00014bd0: 202b 2064 2920 2023 2069 6478 5b72 616e   + d)  # idx[ran
+00014be0: 6765 5f69 202b 2064 5d0a 0a20 2020 2020  ge_i + d]..     
+00014bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c00: 2020 2077 6974 6820 6370 2e74 6167 2822     with cp.tag("
+00014c10: 6469 6666 2229 3a0a 2020 2020 2020 2020  diff"):.        
+00014c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c30: 2020 2020 2320 5365 6c65 6374 206d 6178      # Select max
+00014c40: 2861 2c20 6229 0a20 2020 2020 2020 2020  (a, b).         
+00014c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c60: 2020 2064 6966 6620 3d20 6220 2d20 610a     diff = b - a.
+00014c70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00014c80: 2020 2020 2020 2020 2077 6974 6820 6370           with cp
+00014c90: 2e74 6167 2822 6d61 785f 7661 6c75 6522  .tag("max_value"
+00014ca0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00014cb0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00014cc0: 6178 5f78 203d 2061 202b 206e 756d 7079  ax_x = a + numpy
+00014cd0: 2e6d 6178 696d 756d 2830 2c20 6469 6666  .maximum(0, diff
+00014ce0: 290a 0a20 2020 2020 2020 2020 2020 2020  )..             
+00014cf0: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+00014d00: 6370 2e74 6167 2822 7377 6170 5f6d 6178  cp.tag("swap_max
+00014d10: 5f76 616c 7565 2229 3a0a 2020 2020 2020  _value"):.      
 00014d20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d30: 2020 2020 2020 2077 6974 6820 6370 2e74         with cp.t
-00014d40: 6167 2822 7377 6170 5f6d 6178 5f76 616c  ag("swap_max_val
-00014d50: 7565 2229 3a0a 2020 2020 2020 2020 2020  ue"):.          
-00014d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014d70: 2020 2320 5377 6170 2069 6620 6120 3e20    # Swap if a > 
-00014d80: 620a 2020 2020 2020 2020 2020 2020 2020  b.              
-00014d90: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00014da0: 785b 7261 6e67 655f 695d 203d 206d 6178  x[range_i] = max
-00014db0: 5f78 2861 2c20 6229 3a20 4669 7273 7420  _x(a, b): First 
-00014dc0: 6269 746f 6e69 6320 7365 7175 656e 6365  bitonic sequence
-00014dd0: 2067 6574 7320 6d69 6e28 612c 2062 290a   gets min(a, b).
-00014de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014df0: 2020 2020 2020 2020 2020 2020 7820 3d20              x = 
-00014e00: 7363 6174 7465 7231 6428 782c 2061 202b  scatter1d(x, a +
-00014e10: 2062 202d 206d 6178 5f78 2c20 7261 6e67   b - max_x, rang
-00014e20: 655f 6929 0a20 2020 2020 2020 2020 2020  e_i).           
-00014e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014e40: 2023 2078 5b72 616e 6765 5f69 202b 2064   # x[range_i + d
-00014e50: 5d20 3d20 6d69 6e28 612c 2062 293a 2053  ] = min(a, b): S
-00014e60: 6563 6f6e 6420 6269 746f 6e69 6320 7365  econd bitonic se
-00014e70: 7175 656e 6365 2067 6574 7320 6d61 7828  quence gets max(
-00014e80: 612c 2062 290a 2020 2020 2020 2020 2020  a, b).          
+00014d30: 2020 2020 2020 2320 5377 6170 2069 6620        # Swap if 
+00014d40: 6120 3e20 620a 2020 2020 2020 2020 2020  a > b.          
+00014d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014d60: 2020 2320 785b 7261 6e67 655f 695d 203d    # x[range_i] =
+00014d70: 206d 6178 5f78 2861 2c20 6229 3a20 4669   max_x(a, b): Fi
+00014d80: 7273 7420 6269 746f 6e69 6320 7365 7175  rst bitonic sequ
+00014d90: 656e 6365 2067 6574 7320 6d69 6e28 612c  ence gets min(a,
+00014da0: 2062 290a 2020 2020 2020 2020 2020 2020   b).            
+00014db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014dc0: 7820 3d20 7363 6174 7465 7231 6428 782c  x = scatter1d(x,
+00014dd0: 2061 202b 2062 202d 206d 6178 5f78 2c20   a + b - max_x, 
+00014de0: 7261 6e67 655f 6929 0a20 2020 2020 2020  range_i).       
+00014df0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e00: 2020 2020 2023 2078 5b72 616e 6765 5f69       # x[range_i
+00014e10: 202b 2064 5d20 3d20 6d69 6e28 612c 2062   + d] = min(a, b
+00014e20: 293a 2053 6563 6f6e 6420 6269 746f 6e69  ): Second bitoni
+00014e30: 6320 7365 7175 656e 6365 2067 6574 7320  c sequence gets 
+00014e40: 6d61 7828 612c 2062 290a 2020 2020 2020  max(a, b).      
+00014e50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014e60: 2020 2020 2020 7820 3d20 7363 6174 7465        x = scatte
+00014e70: 7231 6428 782c 206d 6178 5f78 2c20 7261  r1d(x, max_x, ra
+00014e80: 6e67 655f 6920 2b20 6429 0a0a 2020 2020  nge_i + d)..    
 00014e90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ea0: 2020 7820 3d20 7363 6174 7465 7231 6428    x = scatter1d(
-00014eb0: 782c 206d 6178 5f78 2c20 7261 6e67 655f  x, max_x, range_
-00014ec0: 6920 2b20 6429 0a0a 2020 2020 2020 2020  i + d)..        
-00014ed0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ee0: 2320 5570 6461 7465 206c 6162 656c 7320  # Update labels 
-00014ef0: 6172 7261 7920 6163 636f 7264 696e 6720  array according 
-00014f00: 746f 2074 6865 206d 6178 2076 616c 7565  to the max value
-00014f10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014f20: 2020 2020 2020 2020 2077 6974 6820 6370           with cp
-00014f30: 2e74 6167 2822 6d61 785f 6c61 6265 6c22  .tag("max_label"
-00014f40: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00014f50: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00014f60: 735f 615f 6772 6561 7465 725f 7468 616e  s_a_greater_than
-00014f70: 5f62 203d 2064 6966 6620 3e20 300a 2020  _b = diff > 0.  
-00014f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f90: 2020 2020 2020 2020 2020 6d61 785f 6c61            max_la
-00014fa0: 6265 6c73 203d 206c 6162 656c 735f 6120  bels = labels_a 
-00014fb0: 2b20 286c 6162 656c 735f 6220 2d20 6c61  + (labels_b - la
-00014fc0: 6265 6c73 5f61 2920 2a20 6973 5f61 5f67  bels_a) * is_a_g
-00014fd0: 7265 6174 6572 5f74 6861 6e5f 620a 0a20  reater_than_b.. 
+00014ea0: 2020 2020 2320 5570 6461 7465 206c 6162      # Update lab
+00014eb0: 656c 7320 6172 7261 7920 6163 636f 7264  els array accord
+00014ec0: 696e 6720 746f 2074 6865 206d 6178 2076  ing to the max v
+00014ed0: 616c 7565 0a20 2020 2020 2020 2020 2020  alue.           
+00014ee0: 2020 2020 2020 2020 2020 2020 2077 6974               wit
+00014ef0: 6820 6370 2e74 6167 2822 6d61 785f 6c61  h cp.tag("max_la
+00014f00: 6265 6c22 293a 0a20 2020 2020 2020 2020  bel"):.         
+00014f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014f20: 2020 2069 735f 615f 6772 6561 7465 725f     is_a_greater_
+00014f30: 7468 616e 5f62 203d 2064 6966 6620 3e20  than_b = diff > 
+00014f40: 300a 2020 2020 2020 2020 2020 2020 2020  0.              
+00014f50: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
+00014f60: 785f 6c61 6265 6c73 203d 206c 6162 656c  x_labels = label
+00014f70: 735f 6120 2b20 286c 6162 656c 735f 6220  s_a + (labels_b 
+00014f80: 2d20 6c61 6265 6c73 5f61 2920 2a20 6973  - labels_a) * is
+00014f90: 5f61 5f67 7265 6174 6572 5f74 6861 6e5f  _a_greater_than_
+00014fa0: 620a 0a20 2020 2020 2020 2020 2020 2020  b..             
+00014fb0: 2020 2020 2020 2020 2020 2077 6974 6820             with 
+00014fc0: 6370 2e74 6167 2822 7377 6170 5f6d 6178  cp.tag("swap_max
+00014fd0: 5f6c 6162 656c 2229 3a0a 2020 2020 2020  _label"):.      
 00014fe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014ff0: 2020 2020 2020 2077 6974 6820 6370 2e74         with cp.t
-00015000: 6167 2822 7377 6170 5f6d 6178 5f6c 6162  ag("swap_max_lab
-00015010: 656c 2229 3a0a 2020 2020 2020 2020 2020  el"):.          
-00015020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015030: 2020 6c61 6265 6c73 203d 2073 6361 7474    labels = scatt
-00015040: 6572 3164 286c 6162 656c 732c 206c 6162  er1d(labels, lab
-00015050: 656c 735f 6120 2b20 6c61 6265 6c73 5f62  els_a + labels_b
-00015060: 202d 206d 6178 5f6c 6162 656c 732c 2072   - max_labels, r
-00015070: 616e 6765 5f69 290a 2020 2020 2020 2020  ange_i).        
-00015080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015090: 2020 2020 6c61 6265 6c73 203d 2073 6361      labels = sca
-000150a0: 7474 6572 3164 286c 6162 656c 732c 206d  tter1d(labels, m
-000150b0: 6178 5f6c 6162 656c 732c 2072 616e 6765  ax_labels, range
-000150c0: 5f69 202b 2064 290a 0a20 2020 2020 2020  _i + d)..       
-000150d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000150e0: 2023 2055 7064 6174 650a 2020 2020 2020   # Update.      
-000150f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015100: 2020 7769 7468 2063 702e 7461 6728 2275    with cp.tag("u
-00015110: 7064 6174 6522 293a 0a20 2020 2020 2020  pdate"):.       
-00015120: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015130: 2020 2020 2063 6f6d 7061 7269 736f 6e73       comparisons
-00015140: 5b72 616e 6765 5f69 202b 2064 5d20 3d20  [range_i + d] = 
-00015150: 636f 6d70 6172 6973 6f6e 735b 7261 6e67  comparisons[rang
-00015160: 655f 6920 2b20 645d 202b 2031 0a20 2020  e_i + d] + 1.   
-00015170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015180: 2020 2020 2020 2020 2023 2052 6564 7563           # Reduc
-00015190: 6520 7468 6520 636f 6d70 6172 6973 6f6e  e the comparison
-000151a0: 2064 6973 7461 6e63 6520 6279 2068 616c   distance by hal
-000151b0: 660a 2020 2020 2020 2020 2020 2020 2020  f.              
-000151c0: 2020 2020 2020 2020 2020 2020 2020 6420                d 
-000151d0: 3d20 7120 2d20 700a 2020 2020 2020 2020  = q - p.        
-000151e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000151f0: 2020 2020 7220 3d20 700a 0a20 2020 2020      r = p..     
-00015200: 2020 2020 2020 2072 6574 7572 6e20 6c61         return la
-00015210: 6265 6c73 5b30 203a 2073 656c 662e 6e5f  bels[0 : self.n_
-00015220: 6e65 6967 6862 6f72 735d 0a0a 2020 2020  neighbors]..    
-00015230: 2020 2020 2320 312e 2050 6169 7277 6973      # 1. Pairwis
-00015240: 655f 6575 636c 6964 6965 616e 2064 6973  e_euclidiean dis
-00015250: 7461 6e63 650a 2020 2020 2020 2020 7769  tance.        wi
-00015260: 7468 2063 702e 7461 6728 224f 7269 6769  th cp.tag("Origi
-00015270: 6e61 6c20 6469 7374 616e 6365 2229 3a0a  nal distance"):.
-00015280: 2020 2020 2020 2020 2020 2020 6469 7374              dist
-00015290: 616e 6365 5f6d 6174 7269 7820 3d20 7061  ance_matrix = pa
-000152a0: 6972 7769 7365 5f65 7563 6c69 6465 616e  irwise_euclidean
-000152b0: 5f64 6973 7461 6e63 6528 715f 5829 0a0a  _distance(q_X)..
-000152c0: 2020 2020 2020 2020 2320 5468 6520 7371          # The sq
-000152d0: 7561 7265 2072 6f6f 7420 696e 2074 6865  uare root in the
-000152e0: 2045 7563 6c69 6465 616e 2064 6973 7461   Euclidean dista
-000152f0: 6e63 6520 6361 6c63 756c 6174 696f 6e20  nce calculation 
-00015300: 6973 206e 6f74 2061 7070 6c69 6564 2074  is not applied t
-00015310: 6f20 7370 6565 6420 7570 2046 4845 0a20  o speed up FHE. 
-00015320: 2020 2020 2020 2023 2063 6f6d 7075 7461         # computa
-00015330: 7469 6f6e 732e 0a20 2020 2020 2020 2023  tions..        #
-00015340: 2042 6569 6e67 2061 206d 6f6e 6f74 6f6e   Being a monoton
-00015350: 6963 2066 756e 6374 696f 6e2c 2069 7420  ic function, it 
-00015360: 646f 6573 206e 6f74 2061 6666 6563 7420  does not affect 
-00015370: 7468 6520 6c6f 6769 6320 6f66 2074 6865  the logic of the
-00015380: 2063 616c 6375 6c61 7469 6f6e 2c20 6e6f   calculation, no
-00015390: 7461 626c 7920 666f 720a 2020 2020 2020  tably for.      
-000153a0: 2020 2320 7468 6520 6172 6773 6f72 742e    # the argsort.
-000153b0: 0a0a 2020 2020 2020 2020 746f 706b 5f6c  ..        topk_l
-000153c0: 6162 656c 7320 3d20 746f 706b 5f73 6f72  abels = topk_sor
-000153d0: 7469 6e67 2864 6973 7461 6e63 655f 6d61  ting(distance_ma
-000153e0: 7472 6978 2e66 6c61 7474 656e 2829 2c20  trix.flatten(), 
-000153f0: 7365 6c66 2e5f 7929 0a20 2020 2020 2020  self._y).       
-00015400: 2072 6574 7572 6e20 6e75 6d70 792e 6578   return numpy.ex
-00015410: 7061 6e64 5f64 696d 7328 746f 706b 5f6c  pand_dims(topk_l
-00015420: 6162 656c 732c 2061 7869 733d 3029 0a0a  abels, axis=0)..
-00015430: 2020 2020 6465 6620 706f 7374 5f70 726f      def post_pro
-00015440: 6365 7373 696e 6728 7365 6c66 2c20 795f  cessing(self, y_
-00015450: 7072 6564 733a 206e 756d 7079 2e6e 6461  preds: numpy.nda
-00015460: 7272 6179 2920 2d3e 206e 756d 7079 2e6e  rray) -> numpy.n
-00015470: 6461 7272 6179 3a0a 2020 2020 2020 2020  darray:.        
-00015480: 2222 2250 726f 7669 6465 2074 6865 206d  """Provide the m
-00015490: 616a 6f72 6974 7920 766f 7465 2061 6d6f  ajority vote amo
-000154a0: 6e67 2074 6865 2074 6f70 6b20 6c61 6265  ng the topk labe
-000154b0: 6c73 206f 6620 6561 6368 2070 6f69 6e74  ls of each point
-000154c0: 2e0a 0a20 2020 2020 2020 2046 6f72 204b  ...        For K
-000154d0: 4e4e 2c20 7468 6520 6465 2d71 7561 6e74  NN, the de-quant
-000154e0: 697a 6174 696f 6e20 7374 6570 2069 7320  ization step is 
-000154f0: 6e6f 7420 7265 7175 6972 6564 2e20 4265  not required. Be
-00015500: 6361 7573 6520 5f69 6e66 6572 656e 6365  cause _inference
-00015510: 2072 6574 7572 6e73 2074 6865 206c 6162   returns the lab
-00015520: 656c 206f 660a 2020 2020 2020 2020 7468  el of.        th
-00015530: 6520 6b2d 6e65 6172 6573 7420 6e65 6967  e k-nearest neig
-00015540: 6862 6f72 732e 0a0a 2020 2020 2020 2020  hbors...        
-00015550: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-00015560: 2020 795f 7072 6564 7320 286e 756d 7079    y_preds (numpy
-00015570: 2e6e 6461 7272 6179 293a 2054 6865 2074  .ndarray): The t
-00015580: 6f70 6b20 6e65 6172 6573 7420 6c61 6265  opk nearest labe
-00015590: 6c73 2066 6f72 2065 6163 6820 706f 696e  ls for each poin
-000155a0: 742e 0a0a 2020 2020 2020 2020 5265 7475  t...        Retu
-000155b0: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
-000155c0: 206e 756d 7079 2e6e 6461 7272 6179 3a20   numpy.ndarray: 
-000155d0: 5468 6520 6d61 6a6f 7269 7479 2076 6f74  The majority vot
-000155e0: 6520 666f 7220 6561 6368 2070 6f69 6e74  e for each point
-000155f0: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00015600: 2020 2020 2020 7265 7475 726e 206e 756d        return num
-00015610: 7079 2e61 7272 6179 285b 7365 6c66 2e6d  py.array([self.m
-00015620: 616a 6f72 6974 795f 766f 7465 2879 2e66  ajority_vote(y.f
-00015630: 6c61 7474 656e 2829 2920 666f 7220 7920  latten()) for y 
-00015640: 696e 2079 5f70 7265 6473 5d29 0a0a 2020  in y_preds])..  
-00015650: 2020 6465 6620 6765 745f 746f 706b 5f6c    def get_topk_l
-00015660: 6162 656c 7328 7365 6c66 2c20 583a 2044  abels(self, X: D
-00015670: 6174 612c 2066 6865 3a20 556e 696f 6e5b  ata, fhe: Union[
-00015680: 4668 654d 6f64 652c 2073 7472 5d20 3d20  FheMode, str] = 
-00015690: 4668 654d 6f64 652e 4449 5341 424c 4529  FheMode.DISABLE)
-000156a0: 202d 3e20 6e75 6d70 792e 6e64 6172 7261   -> numpy.ndarra
-000156b0: 793a 0a20 2020 2020 2020 2022 2222 5265  y:.        """Re
-000156c0: 7475 726e 2074 6865 204b 2d6e 6561 7265  turn the K-neare
-000156d0: 7374 206c 6162 656c 7320 6f66 2065 6163  st labels of eac
-000156e0: 6820 706f 696e 742e 0a0a 2020 2020 2020  h point...      
-000156f0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-00015700: 2020 2020 5820 2844 6174 6129 3a20 5468      X (Data): Th
-00015710: 6520 696e 7075 7420 7661 6c75 6573 2074  e input values t
-00015720: 6f20 7072 6564 6963 742c 2061 7320 6120  o predict, as a 
-00015730: 4e75 6d70 7920 6172 7261 792c 2054 6f72  Numpy array, Tor
-00015740: 6368 2074 656e 736f 722c 2050 616e 6461  ch tensor, Panda
-00015750: 7320 4461 7461 4672 616d 650a 2020 2020  s DataFrame.    
-00015760: 2020 2020 2020 2020 2020 2020 6f72 204c              or L
-00015770: 6973 742e 0a20 2020 2020 2020 2020 2020  ist..           
-00015780: 2066 6865 2028 556e 696f 6e5b 4668 654d   fhe (Union[FheM
-00015790: 6f64 652c 2073 7472 5d29 3a20 5468 6520  ode, str]): The 
-000157a0: 6d6f 6465 2074 6f20 7573 6520 666f 7220  mode to use for 
-000157b0: 7072 6564 6963 7469 6f6e 2e0a 2020 2020  prediction..    
-000157c0: 2020 2020 2020 2020 2020 2020 4361 6e20              Can 
-000157d0: 6265 2046 6865 4d6f 6465 2e44 4953 4142  be FheMode.DISAB
-000157e0: 4c45 2066 6f72 2043 6f6e 6372 6574 6520  LE for Concrete 
-000157f0: 4d4c 2050 7974 686f 6e20 696e 6665 7265  ML Python infere
-00015800: 6e63 652c 0a20 2020 2020 2020 2020 2020  nce,.           
-00015810: 2020 2020 2046 6865 4d6f 6465 2e53 494d       FheMode.SIM
-00015820: 554c 4154 4520 666f 7220 4648 4520 7369  ULATE for FHE si
-00015830: 6d75 6c61 7469 6f6e 2061 6e64 2046 6865  mulation and Fhe
-00015840: 4d6f 6465 2e45 5845 4355 5445 2066 6f72  Mode.EXECUTE for
-00015850: 2061 6374 7561 6c20 4648 4520 6578 6563   actual FHE exec
-00015860: 7574 696f 6e2e 0a20 2020 2020 2020 2020  ution..         
-00015870: 2020 2020 2020 2043 616e 2061 6c73 6f20         Can also 
-00015880: 6265 2074 6865 2073 7472 696e 6720 7265  be the string re
-00015890: 7072 6573 656e 7461 7469 6f6e 206f 6620  presentation of 
-000158a0: 616e 7920 6f66 2074 6865 7365 2076 616c  any of these val
-000158b0: 7565 732e 0a20 2020 2020 2020 2020 2020  ues..           
-000158c0: 2020 2020 2044 6566 6175 6c74 2074 6f20       Default to 
-000158d0: 4668 654d 6f64 652e 4449 5341 424c 452e  FheMode.DISABLE.
-000158e0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-000158f0: 733a 0a20 2020 2020 2020 2020 2020 206e  s:.            n
-00015900: 756d 7079 2e6e 6461 7272 6179 3a20 5468  umpy.ndarray: Th
-00015910: 6520 4b2d 4e65 6172 6573 7420 6c61 6265  e K-Nearest labe
-00015920: 6c73 2066 6f72 2065 6163 6820 706f 696e  ls for each poin
-00015930: 742e 0a20 2020 2020 2020 2022 2222 0a0a  t..        """..
-00015940: 2020 2020 2020 2020 5820 3d20 6368 6563          X = chec
-00015950: 6b5f 6172 7261 795f 616e 645f 6173 7365  k_array_and_asse
-00015960: 7274 2858 290a 0a20 2020 2020 2020 2074  rt(X)..        t
-00015970: 6f70 6b5f 6c61 6265 6c73 203d 205b 5d0a  opk_labels = [].
-00015980: 2020 2020 2020 2020 666f 7220 7175 6572          for quer
-00015990: 7920 696e 2058 3a0a 2020 2020 2020 2020  y in X:.        
-000159a0: 2020 2020 7175 6572 7920 3d20 6e75 6d70      query = nump
-000159b0: 792e 6578 7061 6e64 5f64 696d 7328 7175  y.expand_dims(qu
-000159c0: 6572 792c 2030 290a 2020 2020 2020 2020  ery, 0).        
-000159d0: 2020 2020 746f 706b 5f6c 6162 656c 732e      topk_labels.
-000159e0: 6170 7065 6e64 2842 6173 6545 7374 696d  append(BaseEstim
-000159f0: 6174 6f72 2e70 7265 6469 6374 2873 656c  ator.predict(sel
-00015a00: 662c 2071 7565 7279 2c20 6668 653d 6668  f, query, fhe=fh
-00015a10: 6529 5b30 5d29 0a0a 2020 2020 2020 2020  e)[0])..        
-00015a20: 7265 7475 726e 206e 756d 7079 2e61 7272  return numpy.arr
-00015a30: 6179 2874 6f70 6b5f 6c61 6265 6c73 290a  ay(topk_labels).
-00015a40: 0a20 2020 2064 6566 2070 7265 6469 6374  .    def predict
-00015a50: 2873 656c 662c 2058 3a20 4461 7461 2c20  (self, X: Data, 
-00015a60: 6668 653a 2055 6e69 6f6e 5b46 6865 4d6f  fhe: Union[FheMo
-00015a70: 6465 2c20 7374 725d 203d 2046 6865 4d6f  de, str] = FheMo
-00015a80: 6465 2e44 4953 4142 4c45 2920 2d3e 206e  de.DISABLE) -> n
-00015a90: 756d 7079 2e6e 6461 7272 6179 3a0a 0a20  umpy.ndarray:.. 
-00015aa0: 2020 2020 2020 2058 203d 2063 6865 636b         X = check
-00015ab0: 5f61 7272 6179 5f61 6e64 5f61 7373 6572  _array_and_asser
-00015ac0: 7428 5829 0a0a 2020 2020 2020 2020 746f  t(X)..        to
-00015ad0: 706b 5f6c 6162 656c 7320 3d20 7365 6c66  pk_labels = self
-00015ae0: 2e67 6574 5f74 6f70 6b5f 6c61 6265 6c73  .get_topk_labels
-00015af0: 2858 2c20 6668 6529 0a0a 2020 2020 2020  (X, fhe)..      
-00015b00: 2020 795f 7072 6564 7320 3d20 7365 6c66    y_preds = self
-00015b10: 2e70 6f73 745f 7072 6f63 6573 7369 6e67  .post_processing
-00015b20: 2874 6f70 6b5f 6c61 6265 6c73 290a 0a20  (topk_labels).. 
-00015b30: 2020 2020 2020 2072 6574 7572 6e20 795f         return y_
-00015b40: 7072 6564 730a 0a0a 636c 6173 7320 536b  preds...class Sk
-00015b50: 6c65 6172 6e4b 4e65 6967 6862 6f72 7343  learnKNeighborsC
-00015b60: 6c61 7373 6966 6965 724d 6978 696e 2853  lassifierMixin(S
-00015b70: 6b6c 6561 726e 4b4e 6569 6768 626f 7273  klearnKNeighbors
-00015b80: 4d69 7869 6e2c 2073 6b6c 6561 726e 2e62  Mixin, sklearn.b
-00015b90: 6173 652e 436c 6173 7369 6669 6572 4d69  ase.ClassifierMi
-00015ba0: 7869 6e2c 2041 4243 293a 0a20 2020 2022  xin, ABC):.    "
-00015bb0: 2222 4120 4d69 7869 6e20 636c 6173 7320  ""A Mixin class 
-00015bc0: 666f 7220 736b 6c65 6172 6e20 4b4e 6569  for sklearn KNei
-00015bd0: 6768 626f 7273 2063 6c61 7373 6966 6965  ghbors classifie
-00015be0: 7273 2077 6974 6820 4648 452e 0a0a 2020  rs with FHE...  
-00015bf0: 2020 5468 6973 2063 6c61 7373 2069 7320    This class is 
-00015c00: 7573 6564 2074 6f20 6372 6561 7465 2061  used to create a
-00015c10: 204b 4e65 6967 6862 6f72 7320 636c 6173   KNeighbors clas
-00015c20: 7369 6669 6572 2063 6c61 7373 2074 6861  sifier class tha
-00015c30: 7420 696e 6865 7269 7473 2066 726f 6d0a  t inherits from.
-00015c40: 2020 2020 536b 6c65 6172 6e4b 4e65 6967      SklearnKNeig
-00015c50: 6862 6f72 734d 6978 696e 2061 6e64 2073  hborsMixin and s
-00015c60: 6b6c 6561 726e 2e62 6173 652e 436c 6173  klearn.base.Clas
-00015c70: 7369 6669 6572 4d69 7869 6e2e 0a20 2020  sifierMixin..   
-00015c80: 2042 7920 696e 6865 7269 7469 6e67 2066   By inheriting f
-00015c90: 726f 6d20 736b 6c65 6172 6e2e 6261 7365  rom sklearn.base
-00015ca0: 2e43 6c61 7373 6966 6965 724d 6978 696e  .ClassifierMixin
-00015cb0: 2c20 6974 2061 6c6c 6f77 7320 7468 6973  , it allows this
-00015cc0: 2063 6c61 7373 2074 6f20 6265 2072 6563   class to be rec
-00015cd0: 6f67 6e69 7a65 640a 2020 2020 6173 2061  ognized.    as a
-00015ce0: 2063 6c61 7373 6966 6965 722e 220a 2020   classifier.".  
-00015cf0: 2020 2222 220a                             """.
+00014ff0: 2020 2020 2020 6c61 6265 6c73 203d 2073        labels = s
+00015000: 6361 7474 6572 3164 286c 6162 656c 732c  catter1d(labels,
+00015010: 206c 6162 656c 735f 6120 2b20 6c61 6265   labels_a + labe
+00015020: 6c73 5f62 202d 206d 6178 5f6c 6162 656c  ls_b - max_label
+00015030: 732c 2072 616e 6765 5f69 290a 2020 2020  s, range_i).    
+00015040: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015050: 2020 2020 2020 2020 6c61 6265 6c73 203d          labels =
+00015060: 2073 6361 7474 6572 3164 286c 6162 656c   scatter1d(label
+00015070: 732c 206d 6178 5f6c 6162 656c 732c 2072  s, max_labels, r
+00015080: 616e 6765 5f69 202b 2064 290a 0a20 2020  ange_i + d)..   
+00015090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000150a0: 2020 2020 2023 2055 7064 6174 650a 2020       # Update.  
+000150b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000150c0: 2020 2020 2020 7769 7468 2063 702e 7461        with cp.ta
+000150d0: 6728 2275 7064 6174 6522 293a 0a20 2020  g("update"):.   
+000150e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000150f0: 2020 2020 2020 2020 2063 6f6d 7061 7269           compari
+00015100: 736f 6e73 5b72 616e 6765 5f69 202b 2064  sons[range_i + d
+00015110: 5d20 3d20 636f 6d70 6172 6973 6f6e 735b  ] = comparisons[
+00015120: 7261 6e67 655f 6920 2b20 645d 202b 2031  range_i + d] + 1
+00015130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015140: 2020 2020 2020 2020 2020 2020 2023 2052               # R
+00015150: 6564 7563 6520 7468 6520 636f 6d70 6172  educe the compar
+00015160: 6973 6f6e 2064 6973 7461 6e63 6520 6279  ison distance by
+00015170: 2068 616c 660a 2020 2020 2020 2020 2020   half.          
+00015180: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015190: 2020 6420 3d20 7120 2d20 700a 2020 2020    d = q - p.    
+000151a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000151b0: 2020 2020 2020 2020 7220 3d20 700a 0a20          r = p.. 
+000151c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000151d0: 6e20 6c61 6265 6c73 5b30 203a 2073 656c  n labels[0 : sel
+000151e0: 662e 6e5f 6e65 6967 6862 6f72 735d 0a0a  f.n_neighbors]..
+000151f0: 2020 2020 2020 2020 2320 312e 2050 6169          # 1. Pai
+00015200: 7277 6973 655f 6575 636c 6964 6965 616e  rwise_euclidiean
+00015210: 2064 6973 7461 6e63 650a 2020 2020 2020   distance.      
+00015220: 2020 7769 7468 2063 702e 7461 6728 224f    with cp.tag("O
+00015230: 7269 6769 6e61 6c20 6469 7374 616e 6365  riginal distance
+00015240: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
+00015250: 6469 7374 616e 6365 5f6d 6174 7269 7820  distance_matrix 
+00015260: 3d20 7061 6972 7769 7365 5f65 7563 6c69  = pairwise_eucli
+00015270: 6465 616e 5f64 6973 7461 6e63 6528 715f  dean_distance(q_
+00015280: 5829 0a0a 2020 2020 2020 2020 2320 5468  X)..        # Th
+00015290: 6520 7371 7561 7265 2072 6f6f 7420 696e  e square root in
+000152a0: 2074 6865 2045 7563 6c69 6465 616e 2064   the Euclidean d
+000152b0: 6973 7461 6e63 6520 6361 6c63 756c 6174  istance calculat
+000152c0: 696f 6e20 6973 206e 6f74 2061 7070 6c69  ion is not appli
+000152d0: 6564 2074 6f20 7370 6565 6420 7570 2046  ed to speed up F
+000152e0: 4845 0a20 2020 2020 2020 2023 2063 6f6d  HE.        # com
+000152f0: 7075 7461 7469 6f6e 732e 0a20 2020 2020  putations..     
+00015300: 2020 2023 2042 6569 6e67 2061 206d 6f6e     # Being a mon
+00015310: 6f74 6f6e 6963 2066 756e 6374 696f 6e2c  otonic function,
+00015320: 2069 7420 646f 6573 206e 6f74 2061 6666   it does not aff
+00015330: 6563 7420 7468 6520 6c6f 6769 6320 6f66  ect the logic of
+00015340: 2074 6865 2063 616c 6375 6c61 7469 6f6e   the calculation
+00015350: 2c20 6e6f 7461 626c 7920 666f 720a 2020  , notably for.  
+00015360: 2020 2020 2020 2320 7468 6520 6172 6773        # the args
+00015370: 6f72 742e 0a0a 2020 2020 2020 2020 746f  ort...        to
+00015380: 706b 5f6c 6162 656c 7320 3d20 746f 706b  pk_labels = topk
+00015390: 5f73 6f72 7469 6e67 2864 6973 7461 6e63  _sorting(distanc
+000153a0: 655f 6d61 7472 6978 2e66 6c61 7474 656e  e_matrix.flatten
+000153b0: 2829 2c20 7365 6c66 2e5f 7929 0a20 2020  (), self._y).   
+000153c0: 2020 2020 2072 6574 7572 6e20 6e75 6d70       return nump
+000153d0: 792e 6578 7061 6e64 5f64 696d 7328 746f  y.expand_dims(to
+000153e0: 706b 5f6c 6162 656c 732c 2061 7869 733d  pk_labels, axis=
+000153f0: 3029 0a0a 2020 2020 6465 6620 706f 7374  0)..    def post
+00015400: 5f70 726f 6365 7373 696e 6728 7365 6c66  _processing(self
+00015410: 2c20 795f 7072 6564 733a 206e 756d 7079  , y_preds: numpy
+00015420: 2e6e 6461 7272 6179 2920 2d3e 206e 756d  .ndarray) -> num
+00015430: 7079 2e6e 6461 7272 6179 3a0a 2020 2020  py.ndarray:.    
+00015440: 2020 2020 2222 2250 726f 7669 6465 2074      """Provide t
+00015450: 6865 206d 616a 6f72 6974 7920 766f 7465  he majority vote
+00015460: 2061 6d6f 6e67 2074 6865 2074 6f70 6b20   among the topk 
+00015470: 6c61 6265 6c73 206f 6620 6561 6368 2070  labels of each p
+00015480: 6f69 6e74 2e0a 0a20 2020 2020 2020 2046  oint...        F
+00015490: 6f72 204b 4e4e 2c20 7468 6520 6465 2d71  or KNN, the de-q
+000154a0: 7561 6e74 697a 6174 696f 6e20 7374 6570  uantization step
+000154b0: 2069 7320 6e6f 7420 7265 7175 6972 6564   is not required
+000154c0: 2e20 4265 6361 7573 6520 5f69 6e66 6572  . Because _infer
+000154d0: 656e 6365 2072 6574 7572 6e73 2074 6865  ence returns the
+000154e0: 206c 6162 656c 206f 660a 2020 2020 2020   label of.      
+000154f0: 2020 7468 6520 6b2d 6e65 6172 6573 7420    the k-nearest 
+00015500: 6e65 6967 6862 6f72 732e 0a0a 2020 2020  neighbors...    
+00015510: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00015520: 2020 2020 2020 795f 7072 6564 7320 286e        y_preds (n
+00015530: 756d 7079 2e6e 6461 7272 6179 293a 2054  umpy.ndarray): T
+00015540: 6865 2074 6f70 6b20 6e65 6172 6573 7420  he topk nearest 
+00015550: 6c61 6265 6c73 2066 6f72 2065 6163 6820  labels for each 
+00015560: 706f 696e 742e 0a0a 2020 2020 2020 2020  point...        
+00015570: 5265 7475 726e 733a 0a20 2020 2020 2020  Returns:.       
+00015580: 2020 2020 206e 756d 7079 2e6e 6461 7272       numpy.ndarr
+00015590: 6179 3a20 5468 6520 6d61 6a6f 7269 7479  ay: The majority
+000155a0: 2076 6f74 6520 666f 7220 6561 6368 2070   vote for each p
+000155b0: 6f69 6e74 2e0a 2020 2020 2020 2020 2222  oint..        ""
+000155c0: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+000155d0: 206e 756d 7079 2e61 7272 6179 285b 7365   numpy.array([se
+000155e0: 6c66 2e6d 616a 6f72 6974 795f 766f 7465  lf.majority_vote
+000155f0: 2879 2e66 6c61 7474 656e 2829 2920 666f  (y.flatten()) fo
+00015600: 7220 7920 696e 2079 5f70 7265 6473 5d29  r y in y_preds])
+00015610: 0a0a 2020 2020 6465 6620 6765 745f 746f  ..    def get_to
+00015620: 706b 5f6c 6162 656c 7328 7365 6c66 2c20  pk_labels(self, 
+00015630: 583a 2044 6174 612c 2066 6865 3a20 556e  X: Data, fhe: Un
+00015640: 696f 6e5b 4668 654d 6f64 652c 2073 7472  ion[FheMode, str
+00015650: 5d20 3d20 4668 654d 6f64 652e 4449 5341  ] = FheMode.DISA
+00015660: 424c 4529 202d 3e20 6e75 6d70 792e 6e64  BLE) -> numpy.nd
+00015670: 6172 7261 793a 0a20 2020 2020 2020 2022  array:.        "
+00015680: 2222 5265 7475 726e 2074 6865 204b 2d6e  ""Return the K-n
+00015690: 6561 7265 7374 206c 6162 656c 7320 6f66  earest labels of
+000156a0: 2065 6163 6820 706f 696e 742e 0a0a 2020   each point...  
+000156b0: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+000156c0: 2020 2020 2020 2020 5820 2844 6174 6129          X (Data)
+000156d0: 3a20 5468 6520 696e 7075 7420 7661 6c75  : The input valu
+000156e0: 6573 2074 6f20 7072 6564 6963 742c 2061  es to predict, a
+000156f0: 7320 6120 4e75 6d70 7920 6172 7261 792c  s a Numpy array,
+00015700: 2054 6f72 6368 2074 656e 736f 722c 2050   Torch tensor, P
+00015710: 616e 6461 7320 4461 7461 4672 616d 650a  andas DataFrame.
+00015720: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015730: 6f72 204c 6973 742e 0a20 2020 2020 2020  or List..       
+00015740: 2020 2020 2066 6865 2028 556e 696f 6e5b       fhe (Union[
+00015750: 4668 654d 6f64 652c 2073 7472 5d29 3a20  FheMode, str]): 
+00015760: 5468 6520 6d6f 6465 2074 6f20 7573 6520  The mode to use 
+00015770: 666f 7220 7072 6564 6963 7469 6f6e 2e0a  for prediction..
+00015780: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015790: 4361 6e20 6265 2046 6865 4d6f 6465 2e44  Can be FheMode.D
+000157a0: 4953 4142 4c45 2066 6f72 2043 6f6e 6372  ISABLE for Concr
+000157b0: 6574 6520 4d4c 2050 7974 686f 6e20 696e  ete ML Python in
+000157c0: 6665 7265 6e63 652c 0a20 2020 2020 2020  ference,.       
+000157d0: 2020 2020 2020 2020 2046 6865 4d6f 6465           FheMode
+000157e0: 2e53 494d 554c 4154 4520 666f 7220 4648  .SIMULATE for FH
+000157f0: 4520 7369 6d75 6c61 7469 6f6e 2061 6e64  E simulation and
+00015800: 2046 6865 4d6f 6465 2e45 5845 4355 5445   FheMode.EXECUTE
+00015810: 2066 6f72 2061 6374 7561 6c20 4648 4520   for actual FHE 
+00015820: 6578 6563 7574 696f 6e2e 0a20 2020 2020  execution..     
+00015830: 2020 2020 2020 2020 2020 2043 616e 2061             Can a
+00015840: 6c73 6f20 6265 2074 6865 2073 7472 696e  lso be the strin
+00015850: 6720 7265 7072 6573 656e 7461 7469 6f6e  g representation
+00015860: 206f 6620 616e 7920 6f66 2074 6865 7365   of any of these
+00015870: 2076 616c 7565 732e 0a20 2020 2020 2020   values..       
+00015880: 2020 2020 2020 2020 2044 6566 6175 6c74           Default
+00015890: 2074 6f20 4668 654d 6f64 652e 4449 5341   to FheMode.DISA
+000158a0: 424c 452e 0a0a 2020 2020 2020 2020 5265  BLE...        Re
+000158b0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+000158c0: 2020 206e 756d 7079 2e6e 6461 7272 6179     numpy.ndarray
+000158d0: 3a20 5468 6520 4b2d 4e65 6172 6573 7420  : The K-Nearest 
+000158e0: 6c61 6265 6c73 2066 6f72 2065 6163 6820  labels for each 
+000158f0: 706f 696e 742e 0a20 2020 2020 2020 2022  point..        "
+00015900: 2222 0a0a 2020 2020 2020 2020 5820 3d20  ""..        X = 
+00015910: 6368 6563 6b5f 6172 7261 795f 616e 645f  check_array_and_
+00015920: 6173 7365 7274 2858 290a 0a20 2020 2020  assert(X)..     
+00015930: 2020 2074 6f70 6b5f 6c61 6265 6c73 203d     topk_labels =
+00015940: 205b 5d0a 2020 2020 2020 2020 666f 7220   [].        for 
+00015950: 7175 6572 7920 696e 2058 3a0a 2020 2020  query in X:.    
+00015960: 2020 2020 2020 2020 7175 6572 7920 3d20          query = 
+00015970: 6e75 6d70 792e 6578 7061 6e64 5f64 696d  numpy.expand_dim
+00015980: 7328 7175 6572 792c 2030 290a 2020 2020  s(query, 0).    
+00015990: 2020 2020 2020 2020 746f 706b 5f6c 6162          topk_lab
+000159a0: 656c 732e 6170 7065 6e64 2842 6173 6545  els.append(BaseE
+000159b0: 7374 696d 6174 6f72 2e70 7265 6469 6374  stimator.predict
+000159c0: 2873 656c 662c 2071 7565 7279 2c20 6668  (self, query, fh
+000159d0: 653d 6668 6529 5b30 5d29 0a0a 2020 2020  e=fhe)[0])..    
+000159e0: 2020 2020 7265 7475 726e 206e 756d 7079      return numpy
+000159f0: 2e61 7272 6179 2874 6f70 6b5f 6c61 6265  .array(topk_labe
+00015a00: 6c73 290a 0a20 2020 2064 6566 2070 7265  ls)..    def pre
+00015a10: 6469 6374 2873 656c 662c 2058 3a20 4461  dict(self, X: Da
+00015a20: 7461 2c20 6668 653a 2055 6e69 6f6e 5b46  ta, fhe: Union[F
+00015a30: 6865 4d6f 6465 2c20 7374 725d 203d 2046  heMode, str] = F
+00015a40: 6865 4d6f 6465 2e44 4953 4142 4c45 2920  heMode.DISABLE) 
+00015a50: 2d3e 206e 756d 7079 2e6e 6461 7272 6179  -> numpy.ndarray
+00015a60: 3a0a 0a20 2020 2020 2020 2058 203d 2063  :..        X = c
+00015a70: 6865 636b 5f61 7272 6179 5f61 6e64 5f61  heck_array_and_a
+00015a80: 7373 6572 7428 5829 0a0a 2020 2020 2020  ssert(X)..      
+00015a90: 2020 746f 706b 5f6c 6162 656c 7320 3d20    topk_labels = 
+00015aa0: 7365 6c66 2e67 6574 5f74 6f70 6b5f 6c61  self.get_topk_la
+00015ab0: 6265 6c73 2858 2c20 6668 6529 0a0a 2020  bels(X, fhe)..  
+00015ac0: 2020 2020 2020 795f 7072 6564 7320 3d20        y_preds = 
+00015ad0: 7365 6c66 2e70 6f73 745f 7072 6f63 6573  self.post_proces
+00015ae0: 7369 6e67 2874 6f70 6b5f 6c61 6265 6c73  sing(topk_labels
+00015af0: 290a 0a20 2020 2020 2020 2072 6574 7572  )..        retur
+00015b00: 6e20 795f 7072 6564 730a 0a0a 636c 6173  n y_preds...clas
+00015b10: 7320 536b 6c65 6172 6e4b 4e65 6967 6862  s SklearnKNeighb
+00015b20: 6f72 7343 6c61 7373 6966 6965 724d 6978  orsClassifierMix
+00015b30: 696e 2853 6b6c 6561 726e 4b4e 6569 6768  in(SklearnKNeigh
+00015b40: 626f 7273 4d69 7869 6e2c 2073 6b6c 6561  borsMixin, sklea
+00015b50: 726e 2e62 6173 652e 436c 6173 7369 6669  rn.base.Classifi
+00015b60: 6572 4d69 7869 6e2c 2041 4243 293a 0a20  erMixin, ABC):. 
+00015b70: 2020 2022 2222 4120 4d69 7869 6e20 636c     """A Mixin cl
+00015b80: 6173 7320 666f 7220 736b 6c65 6172 6e20  ass for sklearn 
+00015b90: 4b4e 6569 6768 626f 7273 2063 6c61 7373  KNeighbors class
+00015ba0: 6966 6965 7273 2077 6974 6820 4648 452e  ifiers with FHE.
+00015bb0: 0a0a 2020 2020 5468 6973 2063 6c61 7373  ..    This class
+00015bc0: 2069 7320 7573 6564 2074 6f20 6372 6561   is used to crea
+00015bd0: 7465 2061 204b 4e65 6967 6862 6f72 7320  te a KNeighbors 
+00015be0: 636c 6173 7369 6669 6572 2063 6c61 7373  classifier class
+00015bf0: 2074 6861 7420 696e 6865 7269 7473 2066   that inherits f
+00015c00: 726f 6d0a 2020 2020 536b 6c65 6172 6e4b  rom.    SklearnK
+00015c10: 4e65 6967 6862 6f72 734d 6978 696e 2061  NeighborsMixin a
+00015c20: 6e64 2073 6b6c 6561 726e 2e62 6173 652e  nd sklearn.base.
+00015c30: 436c 6173 7369 6669 6572 4d69 7869 6e2e  ClassifierMixin.
+00015c40: 0a20 2020 2042 7920 696e 6865 7269 7469  .    By inheriti
+00015c50: 6e67 2066 726f 6d20 736b 6c65 6172 6e2e  ng from sklearn.
+00015c60: 6261 7365 2e43 6c61 7373 6966 6965 724d  base.ClassifierM
+00015c70: 6978 696e 2c20 6974 2061 6c6c 6f77 7320  ixin, it allows 
+00015c80: 7468 6973 2063 6c61 7373 2074 6f20 6265  this class to be
+00015c90: 2072 6563 6f67 6e69 7a65 640a 2020 2020   recognized.    
+00015ca0: 6173 2061 2063 6c61 7373 6966 6965 722e  as a classifier.
+00015cb0: 220a 2020 2020 2222 220a                 ".    """.
```

## concrete/ml/torch/compile.py

```diff
@@ -17,14 +17,15 @@
 
 from ..common.debugging import assert_false, assert_true
 from ..common.utils import (
     MAX_BITWIDTH_BACKWARD_COMPATIBLE,
     check_there_is_no_p_error_options_in_configuration,
     get_onnx_opset_version,
     manage_parameters_for_pbs_errors,
+    process_rounding_threshold_bits,
     to_tuple,
 )
 from ..onnx.convert import OPSET_VERSION_FOR_ONNX_EXPORT
 from ..onnx.onnx_utils import remove_initializer_from_input
 from ..quantization import PostTrainingAffineQuantization, PostTrainingQATImporter, QuantizedModule
 from . import NumpyModule
 
@@ -68,15 +69,15 @@
 
 
 def build_quantized_module(
     model: Union[torch.nn.Module, onnx.ModelProto],
     torch_inputset: Dataset,
     import_qat: bool = False,
     n_bits: Union[int, Dict[str, int]] = MAX_BITWIDTH_BACKWARD_COMPATIBLE,
-    rounding_threshold_bits: Optional[int] = None,
+    rounding_threshold_bits: Union[None, int, Dict[str, Union[str, int]]] = None,
     reduce_sum_copy=False,
 ) -> QuantizedModule:
     """Build a quantized module from a Torch or ONNX model.
 
     Take a model in torch or ONNX, turn it to numpy, quantize its inputs / weights / outputs and
     retrieve the associated quantized module.
 
@@ -84,22 +85,26 @@
         model (Union[torch.nn.Module, onnx.ModelProto]): The model to quantize, either in torch or
             in ONNX.
         torch_inputset (Dataset): the calibration input-set, can contain either torch
             tensors or numpy.ndarray
         import_qat (bool): Flag to signal that the network being imported contains quantizers in
             in its computation graph and that Concrete ML should not re-quantize it
         n_bits: the number of bits for the quantization
-        rounding_threshold_bits (int): if not None, every accumulators in the model are rounded down
-            to the given bits of precision
+        rounding_threshold_bits (Union[None, int, Dict[str, Union[str, int]]]): Defines precision
+            rounding for model accumulators. Accepts None, an int, or a dict.
+            The dict can specify 'method' (fhe.Exactness.EXACT or fhe.Exactness.APPROXIMATE)
+            and 'n_bits' ('auto' or int)
         reduce_sum_copy (bool): if the inputs of QuantizedReduceSum should be copied to avoid
             bit-width propagation
 
     Returns:
         QuantizedModule: The resulting QuantizedModule.
     """
+    rounding_threshold_bits = process_rounding_threshold_bits(rounding_threshold_bits)
+
     inputset_as_numpy_tuple = tuple(
         convert_torch_tensor_or_numpy_array_to_numpy_array(val) for val in to_tuple(torch_inputset)
     )
 
     # Tracing needs to be done with the batch size of 1 since we compile our models to FHE with
     # this batch size. The input set contains many examples, to determine a representative
     # bit-width, but for tracing we only take a single one. We need the ONNX tracing batch size to
@@ -131,15 +136,15 @@
     model: Union[torch.nn.Module, onnx.ModelProto],
     torch_inputset: Dataset,
     import_qat: bool = False,
     configuration: Optional[Configuration] = None,
     artifacts: Optional[DebugArtifacts] = None,
     show_mlir: bool = False,
     n_bits: Union[int, Dict[str, int]] = MAX_BITWIDTH_BACKWARD_COMPATIBLE,
-    rounding_threshold_bits: Optional[int] = None,
+    rounding_threshold_bits: Union[None, int, Dict[str, Union[str, int]]] = None,
     p_error: Optional[float] = None,
     global_p_error: Optional[float] = None,
     verbose: bool = False,
     inputs_encryption_status: Optional[Sequence[str]] = None,
     reduce_sum_copy=False,
 ) -> QuantizedModule:
     """Compile a torch module or ONNX into an FHE equivalent.
@@ -160,28 +165,31 @@
             to be sent to the compiler backend is shown on the screen, e.g., for debugging or demo
         n_bits (Union[int, Dict[str, int]]): number of bits for quantization, can be a single value
             or a dictionary with the following keys :
             - "op_inputs" and "op_weights" (mandatory)
             - "model_inputs" and "model_outputs" (optional, default to 5 bits).
             When using a single integer for n_bits, its value is assigned to "op_inputs" and
             "op_weights" bits. Default is 8 bits.
-        rounding_threshold_bits (int): if not None, every accumulators in the model are rounded down
-            to the given bits of precision
+        rounding_threshold_bits (Union[None, int, Dict[str, Union[str, int]]]): Defines precision
+            rounding for model accumulators. Accepts None, an int, or a dict.
+            The dict can specify 'method' (fhe.Exactness.EXACT or fhe.Exactness.APPROXIMATE)
+            and 'n_bits' ('auto' or int)
         p_error (Optional[float]): probability of error of a single PBS
         global_p_error (Optional[float]): probability of error of the full circuit. In FHE
             simulation `global_p_error` is set to 0
         verbose (bool): whether to show compilation information
         inputs_encryption_status (Optional[Sequence[str]]): encryption status ('clear', 'encrypted')
             for each input. By default all arguments will be encrypted.
         reduce_sum_copy (bool): if the inputs of QuantizedReduceSum should be copied to avoid
             bit-width propagation
 
     Returns:
         QuantizedModule: The resulting compiled QuantizedModule.
     """
+    rounding_threshold_bits = process_rounding_threshold_bits(rounding_threshold_bits)
 
     inputset_as_numpy_tuple = tuple(
         convert_torch_tensor_or_numpy_array_to_numpy_array(val) for val in to_tuple(torch_inputset)
     )
 
     # Build the quantized module
     quantized_module = build_quantized_module(
@@ -230,15 +238,15 @@
     torch_model: torch.nn.Module,
     torch_inputset: Dataset,
     import_qat: bool = False,
     configuration: Optional[Configuration] = None,
     artifacts: Optional[DebugArtifacts] = None,
     show_mlir: bool = False,
     n_bits: Union[int, Dict[str, int]] = MAX_BITWIDTH_BACKWARD_COMPATIBLE,
-    rounding_threshold_bits: Optional[int] = None,
+    rounding_threshold_bits: Union[None, int, Dict[str, Union[str, int]]] = None,
     p_error: Optional[float] = None,
     global_p_error: Optional[float] = None,
     verbose: bool = False,
     inputs_encryption_status: Optional[Sequence[str]] = None,
     reduce_sum_copy: bool = False,
 ) -> QuantizedModule:
     """Compile a torch module into an FHE equivalent.
@@ -260,16 +268,18 @@
             to be sent to the compiler backend is shown on the screen, e.g., for debugging or demo
         n_bits (Union[int, Dict[str, int]]): number of bits for quantization, can be a single value
             or a dictionary with the following keys :
             - "op_inputs" and "op_weights" (mandatory)
             - "model_inputs" and "model_outputs" (optional, default to 5 bits).
             When using a single integer for n_bits, its value is assigned to "op_inputs" and
             "op_weights" bits. Default is 8 bits.
-        rounding_threshold_bits (int): if not None, every accumulators in the model are rounded down
-            to the given bits of precision
+        rounding_threshold_bits (Union[None, int, Dict[str, Union[str, int]]]): Defines precision
+            rounding for model accumulators. Accepts None, an int, or a dict.
+            The dict can specify 'method' (fhe.Exactness.EXACT or fhe.Exactness.APPROXIMATE)
+            and 'n_bits' ('auto' or int)
         p_error (Optional[float]): probability of error of a single PBS
         global_p_error (Optional[float]): probability of error of the full circuit. In FHE
             simulation `global_p_error` is set to 0
         verbose (bool): whether to show compilation information
         inputs_encryption_status (Optional[Sequence[str]]): encryption status ('clear', 'encrypted')
             for each input. By default all arguments will be encrypted.
         reduce_sum_copy (bool): if the inputs of QuantizedReduceSum should be copied to avoid
@@ -312,15 +322,15 @@
     onnx_model: onnx.ModelProto,
     torch_inputset: Dataset,
     import_qat: bool = False,
     configuration: Optional[Configuration] = None,
     artifacts: Optional[DebugArtifacts] = None,
     show_mlir: bool = False,
     n_bits: Union[int, Dict[str, int]] = MAX_BITWIDTH_BACKWARD_COMPATIBLE,
-    rounding_threshold_bits: Optional[int] = None,
+    rounding_threshold_bits: Union[None, int, Dict[str, Union[str, int]]] = None,
     p_error: Optional[float] = None,
     global_p_error: Optional[float] = None,
     verbose: bool = False,
     inputs_encryption_status: Optional[Sequence[str]] = None,
     reduce_sum_copy: bool = False,
 ) -> QuantizedModule:
     """Compile a torch module into an FHE equivalent.
@@ -342,16 +352,18 @@
             to be sent to the compiler backend is shown on the screen, e.g., for debugging or demo
         n_bits (Union[int, Dict[str, int]]): number of bits for quantization, can be a single value
             or a dictionary with the following keys :
             - "op_inputs" and "op_weights" (mandatory)
             - "model_inputs" and "model_outputs" (optional, default to 5 bits).
             When using a single integer for n_bits, its value is assigned to "op_inputs" and
             "op_weights" bits. Default is 8 bits.
-        rounding_threshold_bits (int): if not None, every accumulators in the model are rounded down
-            to the given bits of precision
+        rounding_threshold_bits (Union[None, int, Dict[str, Union[str, int]]]): Defines precision
+            rounding for model accumulators. Accepts None, an int, or a dict.
+            The dict can specify 'method' (fhe.Exactness.EXACT or fhe.Exactness.APPROXIMATE)
+            and 'n_bits' ('auto' or int)
         p_error (Optional[float]): probability of error of a single PBS
         global_p_error (Optional[float]): probability of error of the full circuit. In FHE
             simulation `global_p_error` is set to 0
         verbose (bool): whether to show compilation information
         inputs_encryption_status (Optional[Sequence[str]]): encryption status ('clear', 'encrypted')
             for each input. By default all arguments will be encrypted.
         reduce_sum_copy (bool): if the inputs of QuantizedReduceSum should be copied to avoid
@@ -389,15 +401,15 @@
 def compile_brevitas_qat_model(
     torch_model: torch.nn.Module,
     torch_inputset: Dataset,
     n_bits: Optional[Union[int, Dict[str, int]]] = None,
     configuration: Optional[Configuration] = None,
     artifacts: Optional[DebugArtifacts] = None,
     show_mlir: bool = False,
-    rounding_threshold_bits: Optional[int] = None,
+    rounding_threshold_bits: Union[None, int, Dict[str, Union[str, int]]] = None,
     p_error: Optional[float] = None,
     global_p_error: Optional[float] = None,
     output_onnx_file: Union[None, Path, str] = None,
     verbose: bool = False,
     inputs_encryption_status: Optional[Sequence[str]] = None,
     reduce_sum_copy: bool = False,
 ) -> QuantizedModule:
@@ -420,16 +432,18 @@
             the 8-bit default or a single integer for both values.
         configuration (Configuration): Configuration object to use
             during compilation
         artifacts (DebugArtifacts): Artifacts object to fill
             during compilation
         show_mlir (bool): if set, the MLIR produced by the converter and which is going
             to be sent to the compiler backend is shown on the screen, e.g., for debugging or demo
-        rounding_threshold_bits (int): if not None, every accumulators in the model are rounded down
-            to the given bits of precision
+        rounding_threshold_bits (Union[None, int, Dict[str, Union[str, int]]]): Defines precision
+            rounding for model accumulators. Accepts None, an int, or a dict.
+            The dict can specify 'method' (fhe.Exactness.EXACT or fhe.Exactness.APPROXIMATE)
+            and 'n_bits' ('auto' or int)
         p_error (Optional[float]): probability of error of a single PBS
         global_p_error (Optional[float]): probability of error of the full circuit. In FHE
             simulation `global_p_error` is set to 0
         output_onnx_file (str): temporary file to store ONNX model. If None a temporary file
             is generated
         verbose (bool): whether to show compilation information
         inputs_encryption_status (Optional[Sequence[str]]): encryption status ('clear', 'encrypted')
```

## concrete/ml/torch/hybrid_model.py

```diff
@@ -33,14 +33,15 @@
 class HybridFHEMode(enum.Enum):
     """Simple enum for different modes of execution of HybridModel."""
 
     DISABLE = "disable"  # Use torch weights
     REMOTE = "remote"  # Use remote FHE server
     SIMULATE = "simulate"  # Use FHE simulation
     CALIBRATE = "calibrate"  # Use calibration (to run before FHE compilation)
+    EXECUTE = "execute"  # Use FHE execution
 
 
 def tuple_to_underscore_str(tup: Tuple) -> str:
     """Convert a tuple to a string representation.
 
     Args:
         tup (Tuple): a tuple to change into string representation
```

## concrete/ml/version.py

```diff
@@ -1,3 +1,3 @@
 """File to manage the version of the package."""
 # Auto-generated by "make set_version" do not modify
-__version__ = "1.5.0-rc0"
+__version__ = "1.5.0-rc1"
```

## Comparing `concrete_ml-1.5.0rc0.dist-info/LICENSE` & `concrete_ml-1.5.0rc1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `concrete_ml-1.5.0rc0.dist-info/METADATA` & `concrete_ml-1.5.0rc1.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: concrete-ml
-Version: 1.5.0rc0
+Version: 1.5.0rc1
 Summary: Concrete ML is an open-source set of tools which aims to simplify the use of fully homomorphic encryption (FHE) for data scientists.
 Home-page: https://zama.ai/concrete-ml/
 License: BSD-3-Clause-Clear
 Keywords: FHE,homomorphic encryption,privacy,security
 Author: Zama
 Author-email: hello@zama.ai
 Requires-Python: >=3.8.1,<3.11
@@ -18,22 +18,23 @@
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Security
 Classifier: Topic :: Security :: Cryptography
 Classifier: Topic :: Software Development :: Compilers
 Requires-Dist: boto3 (>=1.23.5,<2.0.0)
 Requires-Dist: brevitas (==0.8.0)
 Requires-Dist: certifi (==2023.07.22)
-Requires-Dist: concrete-python (==2.5.1)
+Requires-Dist: concrete-python (==2.6.0-rc1)
 Requires-Dist: fastapi (>=0.103.2,<0.104.0)
 Requires-Dist: gitpython (==3.1.41)
 Requires-Dist: hummingbird-ml[onnx] (==0.4.8)
 Requires-Dist: numpy (==1.23.5)
 Requires-Dist: onnx (==1.13.1)
 Requires-Dist: onnxoptimizer (==0.3.10)
 Requires-Dist: onnxruntime (==1.13.1)
+Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: protobuf (==3.20.3)
 Requires-Dist: pytest-json-report (==1.5.0)
 Requires-Dist: scikit-learn (==1.1.3)
 Requires-Dist: scipy (==1.10.1)
 Requires-Dist: setuptools (==65.6.3)
 Requires-Dist: skops (==0.5.0)
 Requires-Dist: skorch (==0.11.0)
@@ -47,15 +48,19 @@
 Project-URL: Documentation, http://docs.zama.ai/concrete-ml/
 Project-URL: Repository, https://github.com/zama-ai/concrete-ml
 Project-URL: README, https://github.com/zama-ai/concrete-ml/blob/main/README.md
 Description-Content-Type: text/markdown
 
 <p align="center">
 <!-- product name logo -->
-  <img width=600 src="https://user-images.githubusercontent.com/5758427/231206363-a6639df8-2253-40d8-836e-e3c22d36d6ad.png">
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="https://github.com/zama-ai/concrete-ml/assets/157474013/5ed658d7-0abd-4444-9063-99d8b76c2602">
+  <source media="(prefers-color-scheme: light)" srcset="https://github.com/zama-ai/concrete-ml/assets/157474013/7c67e594-5e2c-483e-858f-ce473a36e37f">
+  <img width=600 alt="Zama Concrete ML">
+</picture>
 </p>
 
 <hr>
 
 <p align="center">
   <a href="https://docs.zama.ai/concrete-ml"> 📒 Documentation</a> | <a href="https://zama.ai/community"> 💛 Community support</a> | <a href="https://github.com/zama-ai/awesome-zama"> 📚 FHE resources by Zama</a>
 </p>
@@ -78,15 +83,15 @@
 <br></br>
 
 ### Main features
 
 - **Built-in models**: Ready-to-use FHE-friendly models with a user interface that is equivalent to their the scikit-learn and XGBoost counterparts
 - **Customs models**: Concrete ML supports models that can use quantization-aware training. These are developed by the user using PyTorch or keras/tensorflow and are imported into Concrete ML through ONNX
 
-*Learn more about Concrete ML features in the [documentation](https://docs.zama.ai/concrete-ml/readme).*
+*Learn more about Concrete ML features in the [documentation](https://docs.zama.ai/concrete-ml).*
 <br></br>
 
 ### Use cases
 
 By leveraging FHE, Concrete ML can unlock a myriad of new use cases for machine learning, such as enabling secure and private data collaboration, protecting sensitive data while still allowing for analysis, and facilitating machine learning on data-sets that are subject to strict data privacy regulations, for instance
 
 - **Healthcare data analysis**: Improve patient care while maintaining privacy by allowing secure, confidential data sharing between healthcare providers.
@@ -247,26 +252,25 @@
 #### Other demos
 
 - [Encrypted Large Language Model](use_case_examples/llm/): converting a user-defined part of a Large Language Model for encrypted text generation. This demo shows the trade-off between quantization and accuracy for text generation and shows how to run the model in FHE.
 - [Private inference for federated learned models](use_case_examples/federated_learning/): private training of a Logistic Regression model and then importing the model into Concrete ML and performing encrypted prediction.
 - [Titanic](use_case_examples/titanic/KaggleTitanic.ipynb): solving the [Kaggle Titanic competition](https://www.kaggle.com/c/titanic/). Implemented with XGBoost from Concrete ML, this example comes as a companion of the [Kaggle notebook](https://www.kaggle.com/code/concretemlteam/titanic-with-privacy-preserving-machine-learning), and was the subject of a blogpost in [KDnuggets](https://www.kdnuggets.com/2022/08/machine-learning-encrypted-data.html).
 - [CIFAR10 FHE-friendly model with Brevitas](use_case_examples/cifar/cifar_brevitas_training): training a VGG9 FHE-compatible neural network using Brevitas, and a script to run the neural network in FHE. Execution in FHE takes ~4 minutes per image and shows an accuracy of 88.7%.
 - [CIFAR10 / CIFAR100 FHE-friendly models with Transfer Learning approach](use_case_examples/cifar/cifar_brevitas_finetuning): series of three notebooks, that convert a pre-trained FP32 VGG11 neural network into a quantized model using Brevitas. The model is fine-tuned on the CIFAR data-sets, converted for FHE execution with Concrete ML and evaluated using FHE simulation. For CIFAR10 and CIFAR100, respectively, our simulations show an accuracy of 90.2% and 68.2%.
-- [FHE neural network splitting for client/server deployment](use_case_examples/cifar/cifar_brevitas_with_model_splitting): explaining how to split a computationally-intensive neural network model in two parts. First, we execute the first part on the client side in the clear, and the output of this step is encrypted. Next, to complete the computation, the second part of the model is evaluated with FHE. This tutorial also shows the impact of FHE speed/accuracy trade-off on CIFAR10, limiting PBS to 8-bit, and thus achieving 62% accuracy.
 
 *If you have built awesome projects using Concrete ML, please let us know and we will be happy to showcase them here!*
 <br></br>
 
 ### Tutorials
 
 - [\[Video tutorial\] Train a linear classifier on encrypted data using Concrete ML and Fully Homomorphic Encryption (FHE)](https://www.youtube.com/watch?v=QVsZ33jBlq4)
 - [\[Video tutorial\] How To Convert a Scikit-learn Model Into Its Homomorphic Equivalent](https://www.zama.ai/post/how-to-convert-a-scikit-learn-model-into-its-homomorphic-equivalent)
 - [Linear Regression Over Encrypted Data With Homomorphic Encryption](https://www.zama.ai/post/linear-regression-using-linear-svr-and-concrete-ml-homomorphic-encryption)
 - [How to Deploy a Machine Learning Model With Concrete ML](https://www.zama.ai/post/how-to-deploy-machine-learning-models-with-concrete-ml)
-- More [Built-in models tutorials](docs/built-in-models/ml_examples.md) and [Deep learning tutorials](docs/deep-learning/examples.md)
+- More [Built-in models tutorials](docs/tutorials/ml_examples.md) and [Deep learning tutorials](docs/tutorials/dl_examples.md)
 
 *Explore more useful resources in [Awesome Zama repo](https://github.com/zama-ai/awesome-zama)*
 <br></br>
 
 ### Documentation
 
 Full, comprehensive documentation is available here: [https://docs.zama.ai/concrete-ml](https://docs.zama.ai/concrete-ml).
@@ -288,30 +292,34 @@
   year={2022},
   note={\url{https://github.com/zama-ai/concrete-ml}},
 }
 ```
 
 ### Contributing
 
-To contribute to Concrete ML, please refer to [this section of the documentation](docs/developer-guide/contributing.md).
+To contribute to Concrete ML, please refer to [this section of the documentation](docs/developer/contributing.md).
 <br></br>
 
 ### License
 
 This software is distributed under the **BSD-3-Clause-Clear** license. If you have any questions, please contact us at hello@zama.ai.
 
 <p align="right">
   <a href="#about" > ↑ Back to top </a> 
 </p>
 
 ## Support
 
 <a target="_blank" href="https://community.zama.ai">
-  <img src="https://github.com/zama-ai/concrete-ml/assets/157474013/0cb69022-fd02-4dbc-801b-51401f3bc07c">
+<picture>
+  <source media="(prefers-color-scheme: dark)" srcset="https://github.com/zama-ai/concrete-ml/assets/157474013/86502167-4ea4-49e9-a881-0cf97d141818">
+  <source media="(prefers-color-scheme: light)" srcset="https://github.com/zama-ai/concrete-ml/assets/157474013/3dcf41e2-1c00-471b-be53-2c804879b8cb">
+  <img alt="Support">
+</picture>
 </a>
 
 🌟 If you find this project helpful or interesting, please consider giving it a star on GitHub! Your support helps to grow the community and motivates further development.
 
 <p align="right">
-  <a href="#tabout" > ↑ Back to top </a> 
+  <a href="#about" > ↑ Back to top </a> 
 </p>
```

### html2text {}

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1 Name: concrete-ml Version: 1.5.0rc0 Summary: Concrete ML
+Metadata-Version: 2.1 Name: concrete-ml Version: 1.5.0rc1 Summary: Concrete ML
 is an open-source set of tools which aims to simplify the use of fully
 homomorphic encryption (FHE) for data scientists. Home-page: https://zama.ai/
 concrete-ml/ License: BSD-3-Clause-Clear Keywords: FHE,homomorphic
 encryption,privacy,security Author: Zama Author-email: hello@zama.ai Requires-
 Python: >=3.8.1,<3.11 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8 Classifier: Topic ::
 Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
 Artificial Intelligence Classifier: Topic :: Scientific/Engineering ::
 Mathematics Classifier: Topic :: Security Classifier: Topic :: Security ::
 Cryptography Classifier: Topic :: Software Development :: Compilers Requires-
 Dist: boto3 (>=1.23.5,<2.0.0) Requires-Dist: brevitas (==0.8.0) Requires-Dist:
-certifi (==2023.07.22) Requires-Dist: concrete-python (==2.5.1) Requires-Dist:
-fastapi (>=0.103.2,<0.104.0) Requires-Dist: gitpython (==3.1.41) Requires-Dist:
-hummingbird-ml[onnx] (==0.4.8) Requires-Dist: numpy (==1.23.5) Requires-Dist:
-onnx (==1.13.1) Requires-Dist: onnxoptimizer (==0.3.10) Requires-Dist:
-onnxruntime (==1.13.1) Requires-Dist: protobuf (==3.20.3) Requires-Dist:
-pytest-json-report (==1.5.0) Requires-Dist: scikit-learn (==1.1.3) Requires-
-Dist: scipy (==1.10.1) Requires-Dist: setuptools (==65.6.3) Requires-Dist:
-skops (==0.5.0) Requires-Dist: skorch (==0.11.0) Requires-Dist: torch
-(==1.13.1) Requires-Dist: tqdm (>=4.64.1,<5.0.0) Requires-Dist: transformers
-(>=4.36.0,<5.0.0) Requires-Dist: typing-extensions (==4.5.0) Requires-Dist:
-uvicorn (>=0.21.0,<0.22.0) Requires-Dist: xgboost (==1.6.2) Project-URL: Bug
-Tracker, https://github.com/zama-ai/concrete-ml/issues Project-URL:
-Documentation, http://docs.zama.ai/concrete-ml/ Project-URL: Repository, https:
-//github.com/zama-ai/concrete-ml Project-URL: README, https://github.com/zama-
-ai/concrete-ml/blob/main/README.md Description-Content-Type: text/markdown
-  [https://user-images.githubusercontent.com/5758427/231206363-a6639df8-2253-
-                          40d8-836e-e3c22d36d6ad.png]
+certifi (==2023.07.22) Requires-Dist: concrete-python (==2.6.0-rc1) Requires-
+Dist: fastapi (>=0.103.2,<0.104.0) Requires-Dist: gitpython (==3.1.41)
+Requires-Dist: hummingbird-ml[onnx] (==0.4.8) Requires-Dist: numpy (==1.23.5)
+Requires-Dist: onnx (==1.13.1) Requires-Dist: onnxoptimizer (==0.3.10)
+Requires-Dist: onnxruntime (==1.13.1) Requires-Dist: pandas (>=2.0.3,<3.0.0)
+Requires-Dist: protobuf (==3.20.3) Requires-Dist: pytest-json-report (==1.5.0)
+Requires-Dist: scikit-learn (==1.1.3) Requires-Dist: scipy (==1.10.1) Requires-
+Dist: setuptools (==65.6.3) Requires-Dist: skops (==0.5.0) Requires-Dist:
+skorch (==0.11.0) Requires-Dist: torch (==1.13.1) Requires-Dist: tqdm
+(>=4.64.1,<5.0.0) Requires-Dist: transformers (>=4.36.0,<5.0.0) Requires-Dist:
+typing-extensions (==4.5.0) Requires-Dist: uvicorn (>=0.21.0,<0.22.0) Requires-
+Dist: xgboost (==1.6.2) Project-URL: Bug Tracker, https://github.com/zama-ai/
+concrete-ml/issues Project-URL: Documentation, http://docs.zama.ai/concrete-ml/
+Project-URL: Repository, https://github.com/zama-ai/concrete-ml Project-URL:
+README, https://github.com/zama-ai/concrete-ml/blob/main/README.md Description-
+Content-Type: text/markdown
+                              [Zama Concrete ML]
 ===============================================================================
    _ð____ _D_o_c_u_m_e_n_t_a_t_i_o_n | _ð____ _C_o_m_m_u_n_i_t_y_ _s_u_p_p_o_r_t | _ð____ _F_H_E_ _r_e_s_o_u_r_c_e_s_ _b_y_ _Z_a_m_a
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_v_/_r_e_l_e_a_s_e_/_z_a_m_a_-_a_i_/_c_o_n_c_r_e_t_e_-_m_l_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]
          _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_B_S_D_-_-_3_-_-_C_l_a_u_s_e_-_-_C_l_e_a_r_-
      _%_2_3_f_f_b_2_4_3_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_n_t_r_i_b_u_t_e_-
              _Z_a_m_a_%_2_0_B_o_u_n_t_y_%_2_0_P_r_o_g_r_a_m_-_%_2_3_f_f_d_2_0_8_?_s_t_y_l_e_=_f_l_a_t_-_s_q_u_a_r_e_]
 ## About ### What is Concrete ML **Concrete ML** is a Privacy-Preserving
@@ -48,15 +48,15 @@
 learn and it is also possible to convert PyTorch models to FHE.
 ### Main features - **Built-in models**: Ready-to-use FHE-friendly models with
 a user interface that is equivalent to their the scikit-learn and XGBoost
 counterparts - **Customs models**: Concrete ML supports models that can use
 quantization-aware training. These are developed by the user using PyTorch or
 keras/tensorflow and are imported into Concrete ML through ONNX *Learn more
 about Concrete ML features in the [documentation](https://docs.zama.ai/
-concrete-ml/readme).*
+concrete-ml).*
 ### Use cases By leveraging FHE, Concrete ML can unlock a myriad of new use
 cases for machine learning, such as enabling secure and private data
 collaboration, protecting sensitive data while still allowing for analysis, and
 facilitating machine learning on data-sets that are subject to strict data
 privacy regulations, for instance - **Healthcare data analysis**: Improve
 patient care while maintaining privacy by allowing secure, confidential data
 sharing between healthcare providers. - **Financial services**: Facilitate
@@ -166,48 +166,40 @@
 Brevitas, and a script to run the neural network in FHE. Execution in FHE takes
 ~4 minutes per image and shows an accuracy of 88.7%. - [CIFAR10 / CIFAR100 FHE-
 friendly models with Transfer Learning approach](use_case_examples/cifar/
 cifar_brevitas_finetuning): series of three notebooks, that convert a pre-
 trained FP32 VGG11 neural network into a quantized model using Brevitas. The
 model is fine-tuned on the CIFAR data-sets, converted for FHE execution with
 Concrete ML and evaluated using FHE simulation. For CIFAR10 and CIFAR100,
-respectively, our simulations show an accuracy of 90.2% and 68.2%. - [FHE
-neural network splitting for client/server deployment](use_case_examples/cifar/
-cifar_brevitas_with_model_splitting): explaining how to split a
-computationally-intensive neural network model in two parts. First, we execute
-the first part on the client side in the clear, and the output of this step is
-encrypted. Next, to complete the computation, the second part of the model is
-evaluated with FHE. This tutorial also shows the impact of FHE speed/accuracy
-trade-off on CIFAR10, limiting PBS to 8-bit, and thus achieving 62% accuracy.
-*If you have built awesome projects using Concrete ML, please let us know and
-we will be happy to showcase them here!*
+respectively, our simulations show an accuracy of 90.2% and 68.2%. *If you have
+built awesome projects using Concrete ML, please let us know and we will be
+happy to showcase them here!*
 ### Tutorials - [\[Video tutorial\] Train a linear classifier on encrypted data
 using Concrete ML and Fully Homomorphic Encryption (FHE)](https://
 www.youtube.com/watch?v=QVsZ33jBlq4) - [\[Video tutorial\] How To Convert a
 Scikit-learn Model Into Its Homomorphic Equivalent](https://www.zama.ai/post/
 how-to-convert-a-scikit-learn-model-into-its-homomorphic-equivalent) - [Linear
 Regression Over Encrypted Data With Homomorphic Encryption](https://
 www.zama.ai/post/linear-regression-using-linear-svr-and-concrete-ml-
 homomorphic-encryption) - [How to Deploy a Machine Learning Model With Concrete
 ML](https://www.zama.ai/post/how-to-deploy-machine-learning-models-with-
-concrete-ml) - More [Built-in models tutorials](docs/built-in-models/
-ml_examples.md) and [Deep learning tutorials](docs/deep-learning/examples.md)
-*Explore more useful resources in [Awesome Zama repo](https://github.com/zama-
-ai/awesome-zama)*
+concrete-ml) - More [Built-in models tutorials](docs/tutorials/ml_examples.md)
+and [Deep learning tutorials](docs/tutorials/dl_examples.md) *Explore more
+useful resources in [Awesome Zama repo](https://github.com/zama-ai/awesome-
+zama)*
 ### Documentation Full, comprehensive documentation is available here: [https:/
 /docs.zama.ai/concrete-ml](https://docs.zama.ai/concrete-ml).
                                                                 _â___ _B_a_c_k_ _t_o_ _t_o_p
 ## Working with Concrete ML ### Citations To cite Concrete ML in academic
 papers, please use the following entry: ```text @Misc{ConcreteML, title=
 {Concrete {ML}: a Privacy-Preserving Machine Learning Library using Fully
 Homomorphic Encryption for Data Scientists}, author={Zama}, year={2022}, note=
 {\url{https://github.com/zama-ai/concrete-ml}}, } ``` ### Contributing To
 contribute to Concrete ML, please refer to [this section of the documentation]
-(docs/developer-guide/contributing.md).
+(docs/developer/contributing.md).
 ### License This software is distributed under the **BSD-3-Clause-Clear**
 license. If you have any questions, please contact us at hello@zama.ai.
                                                                 _â___ _B_a_c_k_ _t_o_ _t_o_p
-## Support _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_z_a_m_a_-_a_i_/_c_o_n_c_r_e_t_e_-_m_l_/_a_s_s_e_t_s_/_1_5_7_4_7_4_0_1_3_/_0_c_b_6_9_0_2_2_-
-_f_d_0_2_-_4_d_b_c_-_8_0_1_b_-_5_1_4_0_1_f_3_b_c_0_7_c_]ð If you find this project helpful or
-interesting, please consider giving it a star on GitHub! Your support helps to
-grow the community and motivates further development.
+## Support _[_S_u_p_p_o_r_t_]ð If you find this project helpful or interesting,
+please consider giving it a star on GitHub! Your support helps to grow the
+community and motivates further development.
                                                                 _â___ _B_a_c_k_ _t_o_ _t_o_p
```

## Comparing `concrete_ml-1.5.0rc0.dist-info/RECORD` & `concrete_ml-1.5.0rc1.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -5,57 +5,66 @@
 concrete/ml/common/debugging/__init__.py,sha256=_eh1MBBmnk2o1M4YGbH0Cbr_cEPjFOVz5wsp080HonE,101
 concrete/ml/common/debugging/custom_assert.py,sha256=H5ESt7cYnDT2PnUXvDaAvUJR2CKHwsHQ4QWtMLvcLZw,2377
 concrete/ml/common/serialization/__init__.py,sha256=AkC44PnjzgvNnRYwmd9PbpiZiTAXekUwCvVDPWKlK9g,1152
 concrete/ml/common/serialization/decoder.py,sha256=2DCqYdfyKj4kh46L4Thm0GNvvFzQEfaDXGNO2e5q-HU,8375
 concrete/ml/common/serialization/dumpers.py,sha256=uXdo0YHc8WnrlI7NQ78oGdBijpD0vatjgjBEIjrSGF0,601
 concrete/ml/common/serialization/encoder.py,sha256=hNUxaKWTDs1-vFKfTOqLZF73aOAAb0Nl7SZfawOtqLs,12167
 concrete/ml/common/serialization/loaders.py,sha256=Jz10aCeuvOUIlkmKaChGgSmBR0KDsNgAmKj-UBYod6E,743
-concrete/ml/common/utils.py,sha256=fXYGAbkwm_tqYNGfmaBQWlpOIZKjYcHSmRtVxfm3Psw,19738
+concrete/ml/common/utils.py,sha256=l0MGKs6AGR-_u2CnpA2ZuctFa0lgFUuFNxSLG_IW4Co,21759
 concrete/ml/deployment/Dockerfile.server,sha256=ycWhDO6tWKedZSFMnDmD-TGEhdQtzsl6YXRNJqKvkr4,235
 concrete/ml/deployment/__init__.py,sha256=jgaPZMSlsJy1KF45EI92rQ7e2CKEpmLdaWcwwFEPeZ8,121
 concrete/ml/deployment/deploy_to_aws.py,sha256=P94YtL5e_r50eoNHoiklMQmlsFoRHXw9ge6Tn_7dV9c,17918
 concrete/ml/deployment/deploy_to_docker.py,sha256=c7N9XhbgBajyLiu_TvPRke5kSi6_GdmRtOOPSl-LpoE,3800
 concrete/ml/deployment/fhe_client_server.py,sha256=1UwYZPFzCM6AI8E4tvxIMWduvoDLpKsCk9XM-B47InY,12989
 concrete/ml/deployment/server.py,sha256=CB6y1v9NPq3NqOE0spzKUMNywFNmhEta8zsn5YIu42o,2590
 concrete/ml/deployment/server_requirements.txt,sha256=gyd07Mp8qZPWhuz7QI1kgYS3JbjcPbZK4cL9RDOR_x8,33
 concrete/ml/deployment/utils.py,sha256=aZFmDRUW58JHAJLK5c--UANMx1sN8C-ioz4JPcPQV-Q,3293
 concrete/ml/onnx/__init__.py,sha256=LiK0TOCAo7c5-TBk4zcO3PEQmdASN0NgLDYIYUXl464,19
 concrete/ml/onnx/convert.py,sha256=vv-VNhPoNwFdHpOiAD9_bYCVGzf8v_vAGqxuI_7sii8,11430
 concrete/ml/onnx/onnx_impl_utils.py,sha256=usv9wwmjS53mmkt63rHVrntx4IXgckwzRX3wRicXL_A,11573
 concrete/ml/onnx/onnx_model_manipulations.py,sha256=ogrGucdHA5sYXZcWD0cOzBiYFju14UFmd7xtMfUeAe4,11003
 concrete/ml/onnx/onnx_utils.py,sha256=dAogJ9c2apUn0pVAULQpL8l8977avwEQ3if_nv69kV0,23174
-concrete/ml/onnx/ops_impl.py,sha256=qYBelDKNGgomPzjCQgg7Uq89rRi2kpmS3ZJStU_UWf4,67978
+concrete/ml/onnx/ops_impl.py,sha256=RFh_vhQNSEdzKf92y0BD_yMp3MpuvHc8OT-4axTJGqM,67985
+concrete/ml/pandas/__init__.py,sha256=ljdDmsNdogqEbldD8DwUmzlRbKcWpXhCHAYLNhodO58,4183
+concrete/ml/pandas/_client_server_files/client.zip,sha256=XRTkTb_lVLicEc43kiCnOy0SLCBujR09jHQKMYa-0LE,594
+concrete/ml/pandas/_client_server_files/server.zip,sha256=dkJtKS8sd6GrBOCC6CaacWuA6dVmjsMGUhwsToKurVE,1382
+concrete/ml/pandas/_development.py,sha256=_sOHTZyDgKDbVKoow_ttNqnUxjOQVpKKRMXzwfBAsCA,6572
+concrete/ml/pandas/_operators.py,sha256=EhQhmDPBbkbJdc_uW0k_0m4Oa0XAxZbqqX5ilyQvEfo,17264
+concrete/ml/pandas/_processing.py,sha256=VHLCjd9RHDBBX7idlAlry9EUkfWRMAzC_lp93E4LIKM,12823
+concrete/ml/pandas/_utils.py,sha256=ewjqpa-Dv5r_D_SYVMpPHbWXPzArnuRUoCnNcmfv9Hw,6485
+concrete/ml/pandas/client_engine.py,sha256=fIstfY1QGZhvbFHtkpUZoQpp2bQSVMc4W8BPH2GIJ1s,3558
+concrete/ml/pandas/dataframe.py,sha256=WW-jARUpTlZkL9Uk6lU-5BHVPaOAi_Ktp_7uIoIDxP4,12603
 concrete/ml/pytest/__init__.py,sha256=5Zk0w3T-MYPF3485ir5kZ1dP7x_VoMIreDMKnJuyBCo,101
 concrete/ml/pytest/torch_models.py,sha256=gUBxq-Ceeh6-RgwbjcJ8WP40o9jJG-n5BIvD82FVTDk,47491
-concrete/ml/pytest/utils.py,sha256=JVbMJKO-WkOxxgfkpOoiAp2-ZTxi_2oxidc4ov2h4PQ,25505
+concrete/ml/pytest/utils.py,sha256=xggf1tzNSnW8AL7IB5sDjn3r1gqy_olxZba-cEVWStY,27970
 concrete/ml/quantization/__init__.py,sha256=gij1_KfiUJFidN1SrM-YMpbJwi1QyfTNxcocyRo78hA,1180
-concrete/ml/quantization/base_quantized_op.py,sha256=XhwDmlaRKvgaKQr-9YOn4ArRD9xykKeE161qb3p0I08,42163
-concrete/ml/quantization/post_training.py,sha256=banVFyK6LvLlLz7O-gZaSAl1RrWebDHPgifIzhar3rg,48516
+concrete/ml/quantization/base_quantized_op.py,sha256=2Hoy1-6ZjCWHpX3Pj_kbiqG7B2bAJupo-u5zph1ZI0k,43545
+concrete/ml/quantization/post_training.py,sha256=BriCzKZHoFIbJfCiQXm0rzVSqW3qn_5-h3cX22UL6LQ,49245
 concrete/ml/quantization/qat_quantizers.py,sha256=mMKpMDhLRRt9vAIe9sv3sdjQVobgrS5sYLKkladD6yc,1014
-concrete/ml/quantization/quantized_module.py,sha256=wd35GFb0YkIi2KFUeB0t1YJHNbAbk6uuKnHswCLOilc,30981
+concrete/ml/quantization/quantized_module.py,sha256=lNgk8KHpessQOt-e_Yvz9n1lMafFA7wquXuhRKHW7Zs,30980
 concrete/ml/quantization/quantized_module_passes.py,sha256=U3b6G1lW6okOWdymh-TenXmm_rSH4McBtTgbA9xwdjA,13734
 concrete/ml/quantization/quantized_ops.py,sha256=hjaQ5f5Ht0ysffzN5HZzt2BmIbepujyPHURrYceCslg,98341
 concrete/ml/quantization/quantizers.py,sha256=2PRY6xXca8cXghL1cwudxztVJBo1gE78XBQ50GxAOl4,37300
 concrete/ml/search_parameters/__init__.py,sha256=-TGfmte3AvAn2ajLxLd-FCbru6_Ml9DiKeG7ooR819Q,77
 concrete/ml/search_parameters/p_error_search.py,sha256=16JfuLNtj_MQzgppFDIKbkf7LxtM8m11qvMTdyNtsDQ,21230
 concrete/ml/sklearn/__init__.py,sha256=YrJgAktB7GV4cNLJdobD-WVHwEaj5YrqBk2Gzf2BB3M,10315
 concrete/ml/sklearn/_fhe_training_utils.py,sha256=NUFW569lFpwJjB_nYT48jd91LL93UqZyMM5hcBKCl5s,3385
-concrete/ml/sklearn/base.py,sha256=d5XN_R9WoWVLJMal9z9CDUmWHEyNSKeqzEHUkBIvHy0,89334
+concrete/ml/sklearn/base.py,sha256=hjNKcM2GGkJqqh4CXt9K5XNm4ek_KkQUkm9KVSTAcVA,89274
 concrete/ml/sklearn/glm.py,sha256=sXbrxrSJ8_lBH6YaWEP4-5_EUbfjZyWUXNuVJ2gfsZY,12899
 concrete/ml/sklearn/linear_model.py,sha256=FO1lZht6Enz-4wkNp5W61yJnRn8Q7TyNW4kg9W1HSPo,67262
 concrete/ml/sklearn/neighbors.py,sha256=gklkB5TBeAVkG6xdZkVCDNNSOsIi9ARUQcFQJBwhoWc,6121
 concrete/ml/sklearn/qnn.py,sha256=mE1OJs6tQX83MRq8I6nfa41i2YZWu00P5GHlnyzqcQc,32101
 concrete/ml/sklearn/qnn_module.py,sha256=8KD5O_kolpc226P1Kpj4PiGymJIm_PCwneS6WEAS9-o,14188
 concrete/ml/sklearn/rf.py,sha256=Ot6rmUIa4Qs9W3sMUNn1iBvO7eIb0myJNbqwvV1vdiw,11440
 concrete/ml/sklearn/svm.py,sha256=cog3FrugZG47HDbiCw4KU2hRdU37n3U0pmN76Rnx_Z0,8897
 concrete/ml/sklearn/tree.py,sha256=UyXZ3LWeioH-iy7wURkNIGEoJ_m6M0RlDzdniNtez3E,10500
 concrete/ml/sklearn/tree_to_numpy.py,sha256=5SjKjOqzjRJYqp62melCF64QcWkw8Qog-LWnr5UFsfo,19152
 concrete/ml/sklearn/xgb.py,sha256=m1q__-A1Ml_ZBbEI2uil9GlXo6S6wEoBMe0tHFWxsyU,19694
 concrete/ml/torch/__init__.py,sha256=aUQ25-hJdirZCa20KqaVMrt2PnpnSXBCVw7QvLQ_BoQ,83
-concrete/ml/torch/compile.py,sha256=snbbXahWgYPrbTOf5-aJreeeQvWuBVvnpWMaXx5u_Vw,23432
-concrete/ml/torch/hybrid_model.py,sha256=hVn47VfeTaG_7I90kTEZjHxajHrsYgMIvRyjPfNrQ2k,32328
+concrete/ml/torch/compile.py,sha256=oUGGEbrinF9l-BVz7crERg11yE0TGSbK8YnGLmKSb9M,24629
+concrete/ml/torch/hybrid_model.py,sha256=X0WnY696XNssfOnVMRhBIZik5Opxd22eKfLIOOUIg5c,32373
 concrete/ml/torch/numpy_module.py,sha256=kjoft_uK9SbOraPc8UKSxWd_LVF5XKNV-IdAukMd7fQ,3167
-concrete/ml/version.py,sha256=9vTtoQFB_0FSsBK8u9eqqUt4VaCPuJWOcwrzItpPQKE,128
-concrete_ml-1.5.0rc0.dist-info/LICENSE,sha256=Q2TUW9iqL5JOnEcNTstSvNPYRnF-iQi24FUla8oUEwE,1546
-concrete_ml-1.5.0rc0.dist-info/METADATA,sha256=Mz7a6VkQ-G1kxsjLFD5vfcE7_DUbEbM50RK4oDeixiY,16441
-concrete_ml-1.5.0rc0.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
-concrete_ml-1.5.0rc0.dist-info/RECORD,,
+concrete/ml/version.py,sha256=ku-PEmBRnzS3lGgMvB01Sa6RKzcCyG_eqD5RKqECOls,128
+concrete_ml-1.5.0rc1.dist-info/LICENSE,sha256=Q2TUW9iqL5JOnEcNTstSvNPYRnF-iQi24FUla8oUEwE,1546
+concrete_ml-1.5.0rc1.dist-info/METADATA,sha256=fMpx_dJQ86odf_4T8hiNSKxXz5yqT-RrklvpPmWpLys,16396
+concrete_ml-1.5.0rc1.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
+concrete_ml-1.5.0rc1.dist-info/RECORD,,
```

