# Comparing `tmp/annofabapi_3dpc_extensions-0.2.1.tar.gz` & `tmp/annofabapi_3dpc_extensions-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annofabapi_3dpc_extensions-0.2.1.tar", max compression
+gzip compressed data, was "annofabapi_3dpc_extensions-0.2.2.tar", max compression
```

## Comparing `annofabapi_3dpc_extensions-0.2.1.tar` & `annofabapi_3dpc_extensions-0.2.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1081 2023-05-16 07:20:49.314808 annofabapi_3dpc_extensions-0.2.1/LICENSE
--rw-r--r--   0        0        0     2905 2023-05-16 07:20:49.314808 annofabapi_3dpc_extensions-0.2.1/README.md
--rw-r--r--   0        0        0       71 2023-05-16 07:20:49.314808 annofabapi_3dpc_extensions-0.2.1/annofab_3dpc/__init__.py
--rw-r--r--   0        0        0      131 2023-05-16 07:21:02.919369 annofabapi_3dpc_extensions-0.2.1/annofab_3dpc/__version__.py
--rw-r--r--   0        0        0    10506 2023-05-16 07:20:49.314808 annofabapi_3dpc_extensions-0.2.1/annofab_3dpc/annotation.py
--rw-r--r--   0        0        0        0 2023-05-16 07:20:49.314808 annofabapi_3dpc_extensions-0.2.1/annofab_3dpc/py.typed
--rw-r--r--   0        0        0     1612 2023-05-16 07:21:02.919369 annofabapi_3dpc_extensions-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3729 1970-01-01 00:00:00.000000 annofabapi_3dpc_extensions-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-04-03 08:41:01.589774 annofabapi_3dpc_extensions-0.2.2/LICENSE
+-rw-r--r--   0        0        0     3057 2024-04-03 08:41:01.589774 annofabapi_3dpc_extensions-0.2.2/README.md
+-rw-r--r--   0        0        0       71 2024-04-03 08:41:01.589774 annofabapi_3dpc_extensions-0.2.2/annofab_3dpc/__init__.py
+-rw-r--r--   0        0        0      131 2024-04-03 08:41:15.449832 annofabapi_3dpc_extensions-0.2.2/annofab_3dpc/__version__.py
+-rw-r--r--   0        0        0    10633 2024-04-03 08:41:01.589774 annofabapi_3dpc_extensions-0.2.2/annofab_3dpc/annotation.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:41:01.589774 annofabapi_3dpc_extensions-0.2.2/annofab_3dpc/py.typed
+-rw-r--r--   0        0        0     4498 2024-04-03 08:41:15.445832 annofabapi_3dpc_extensions-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0     4068 1970-01-01 00:00:00.000000 annofabapi_3dpc_extensions-0.2.2/PKG-INFO
```

### Comparing `annofabapi_3dpc_extensions-0.2.1/LICENSE` & `annofabapi_3dpc_extensions-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `annofabapi_3dpc_extensions-0.2.1/README.md` & `annofabapi_3dpc_extensions-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # annofabapi-3dpc-extensions
-[![Build Status](https://travis-ci.com/kurusugawa-computer/annofabapi-3dpc-extensions.svg?branch=master)](https://travis-ci.com/kurusugawa-computer/annofabapi-3dpc-extensions)
+[![Build Status](https://app.travis-ci.com/kurusugawa-computer/annofabapi-3dpc-extensions.svg?branch=main)](https://app.travis-ci.com/kurusugawa-computer/annofabapi-3dpc-extensions)
 [![PyPI version](https://badge.fury.io/py/annofabapi-3dpc-extensions.svg)](https://badge.fury.io/py/annofabapi-3dpc-extensions)
 [![Python Versions](https://img.shields.io/pypi/pyversions/annofabapi-3dpc-extensions.svg)](https://pypi.org/project/annofabapi-3dpc-extensions/)
 [![Documentation Status](https://readthedocs.org/projects/annofabapi-3dpc-extensions/badge/?version=latest)](https://annofabapi-3dpc-extensions.readthedocs.io/en/latest/?badge=latest)
 
 
 
 [annofabapi](https://github.com/kurusugawa-computer/annofab-api-python-client)の3次元アノテーション用の拡張機能です。
@@ -67,7 +67,12 @@
     segment_data = SegmentData.from_dict(dict_segmenta_data)
     assert type(segment_data) == SegmentData
     assert len(segment_data.points) > 0
     print(segment_data.points)
     # => [130439, 130442, ... ]
 
 ```
+
+
+# 開発者向けドキュメント
+
+https://github.com/kurusugawa-computer/annofabapi-3dpc-extensions/blob/main/README_for_developer.md 参照
```

### Comparing `annofabapi_3dpc_extensions-0.2.1/annofab_3dpc/annotation.py` & `annofabapi_3dpc_extensions-0.2.2/annofab_3dpc/annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 
 @dataclass
 class Location(DataClassJsonMixin):
     x: float
     y: float
     z: float
 
-    def __add__(self, other):
+    def __add__(self, other: "Location") -> "Location":
         return self.__class__(
             x=self.x + other.x,
             y=self.y + other.y,
             z=self.z + other.z,
         )
 
-    def __sub__(self, other):
+    def __sub__(self, other: "Location") -> "Location":
         return self.__class__(
             x=self.x - other.x,
             y=self.y - other.y,
             z=self.z - other.z,
         )
 
 
@@ -47,47 +47,47 @@
     回転行列を算出するために、クラスを作った。
 
     Notes:
         以下のコードを流用した。
         https://github.com/KieranWynn/pyquaternion/blob/99025c17bab1c55265d61add13375433b35251af/pyquaternion/quaternion.py#L138
     """
 
-    def __init__(self, array: Union[Sequence[float], numpy.ndarray]):
+    def __init__(self, array: Union[Sequence[float], numpy.ndarray]) -> None:
         self.q = numpy.array(array)
 
-    def _q_matrix(self):
+    def _q_matrix(self) -> numpy.ndarray:
         """Matrix representation of quaternion for multiplication purposes."""
         return numpy.array(
             [
                 [self.q[0], -self.q[1], -self.q[2], -self.q[3]],
                 [self.q[1], self.q[0], -self.q[3], self.q[2]],
                 [self.q[2], self.q[3], self.q[0], -self.q[1]],
                 [self.q[3], -self.q[2], self.q[1], self.q[0]],
             ]
         )
 
-    def _q_bar_matrix(self):
+    def _q_bar_matrix(self) -> numpy.ndarray:
         """Matrix representation of quaternion for multiplication purposes."""
         return numpy.array(
             [
                 [self.q[0], -self.q[1], -self.q[2], -self.q[3]],
                 [self.q[1], self.q[0], self.q[3], -self.q[2]],
                 [self.q[2], -self.q[3], self.q[0], self.q[1]],
                 [self.q[3], self.q[2], -self.q[1], self.q[0]],
             ]
         )
 
     @property
-    def rotation_matrix(self):
+    def rotation_matrix(self) -> numpy.ndarray:
         """Get the 3x3 rotation matrix equivalent of the quaternion rotation.
         Returns:
             A 3x3 orthogonal rotation matrix as a 3x3 Numpy array
         Note:
-            This feature only makes sense when referring to a unit quaternion. Calling this method will implicitly normalise the Quaternion object to a unit quaternion if it is not already one.  # noqa: E501
-        """
+            This feature only makes sense when referring to a unit quaternion. Calling this method will implicitly normalise the Quaternion object to a unit quaternion if it is not already one.
+        """  # noqa: E501
         product_matrix = numpy.dot(self._q_matrix(), self._q_bar_matrix().conj().transpose())
         return product_matrix[1:][:, 1:]
 
 
 @dataclass
 class EulerAnglesZXY(DataClassJsonMixin):
     """
@@ -294,15 +294,15 @@
 
     def dump(self) -> Dict[str, Any]:
         """SimpleAnnotationDetailクラスのdataプロパティに対応するdictを生成する。"""
         str_data = json.dumps(self.to_dict(), separators=(",", ":"))
         return {"data": str_data, "_type": ANNOTATION_TYPE_UNKNOWN}
 
 
-def convert_annotation_detail_data(dict_data: Dict[str, Any]) -> Any:
+def convert_annotation_detail_data(dict_data: Dict[str, Any]) -> Any:  # noqa: ANN401
     """
     SimpleAnnotationDetailクラスのdict型であるdataプロパティを、3DPC Editor用のDataclassに変換します。
     3DPC Editor用のDataclassに変換できない場合は、引数をそのまま返します。
 
     Args:
         dict_data: SimpleAnnotationDetailクラスのdict型のdataプロパティ
```

### Comparing `annofabapi_3dpc_extensions-0.2.1/PKG-INFO` & `annofabapi_3dpc_extensions-0.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 Metadata-Version: 2.1
 Name: annofabapi-3dpc-extensions
-Version: 0.2.1
+Version: 0.2.2
 Summary: annofabapiの3DPC Editor用の拡張機能です。
 Home-page: https://github.com/kurusugawa-computer/annofabapi-3dpc-extensions
 Author: Kurusugawa Computer Inc.
-Requires-Python: >=3.8.1,<4.0.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Utilities
 Requires-Dist: dataclasses-json
-Requires-Dist: numpy
+Requires-Dist: numpy (<1.25) ; python_version == "3.8"
+Requires-Dist: numpy (>=1.26) ; python_version >= "3.9"
 Project-URL: Repository, https://github.com/kurusugawa-computer/annofabapi-3dpc-extensions
 Description-Content-Type: text/markdown
 
 # annofabapi-3dpc-extensions
-[![Build Status](https://travis-ci.com/kurusugawa-computer/annofabapi-3dpc-extensions.svg?branch=master)](https://travis-ci.com/kurusugawa-computer/annofabapi-3dpc-extensions)
+[![Build Status](https://app.travis-ci.com/kurusugawa-computer/annofabapi-3dpc-extensions.svg?branch=main)](https://app.travis-ci.com/kurusugawa-computer/annofabapi-3dpc-extensions)
 [![PyPI version](https://badge.fury.io/py/annofabapi-3dpc-extensions.svg)](https://badge.fury.io/py/annofabapi-3dpc-extensions)
 [![Python Versions](https://img.shields.io/pypi/pyversions/annofabapi-3dpc-extensions.svg)](https://pypi.org/project/annofabapi-3dpc-extensions/)
 [![Documentation Status](https://readthedocs.org/projects/annofabapi-3dpc-extensions/badge/?version=latest)](https://annofabapi-3dpc-extensions.readthedocs.io/en/latest/?badge=latest)
 
 
 
 [annofabapi](https://github.com/kurusugawa-computer/annofab-api-python-client)の3次元アノテーション用の拡張機能です。
@@ -88,7 +91,12 @@
     assert type(segment_data) == SegmentData
     assert len(segment_data.points) > 0
     print(segment_data.points)
     # => [130439, 130442, ... ]
 
 ```
 
+
+# 開発者向けドキュメント
+
+https://github.com/kurusugawa-computer/annofabapi-3dpc-extensions/blob/main/README_for_developer.md 参照
+
```

