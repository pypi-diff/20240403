# Comparing `tmp/pytest_container-0.4.0.tar.gz` & `tmp/pytest_container-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_container-0.4.0.tar", max compression
+gzip compressed data, was "pytest_container-0.4.1.tar", max compression
```

## Comparing `pytest_container-0.4.0.tar` & `pytest_container-0.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    26529 2024-03-27 13:36:52.078136 pytest_container-0.4.0/LICENSE
--rw-r--r--   0        0        0     3098 2024-03-27 13:36:52.078136 pytest_container-0.4.0/README.rst
--rw-r--r--   0        0        0     2075 2024-03-27 13:36:52.078136 pytest_container-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      946 2024-03-27 13:36:52.078136 pytest_container-0.4.0/pytest_container/__init__.py
--rw-r--r--   0        0        0    10564 2024-03-27 13:36:52.078136 pytest_container-0.4.0/pytest_container/build.py
--rw-r--r--   0        0        0    42313 2024-03-27 13:36:52.078136 pytest_container-0.4.0/pytest_container/container.py
--rw-r--r--   0        0        0     5725 2024-03-27 13:36:52.078136 pytest_container-0.4.0/pytest_container/helpers.py
--rw-r--r--   0        0        0     8932 2024-03-27 13:36:52.078136 pytest_container-0.4.0/pytest_container/inspect.py
--rw-r--r--   0        0        0      362 2024-03-27 13:36:52.078136 pytest_container-0.4.0/pytest_container/logging.py
--rw-r--r--   0        0        0     7721 2024-03-27 13:36:52.078136 pytest_container-0.4.0/pytest_container/plugin.py
--rw-r--r--   0        0        0     7973 2024-03-27 13:36:52.078136 pytest_container-0.4.0/pytest_container/pod.py
--rw-r--r--   0        0        0    21718 2024-03-27 13:36:52.078136 pytest_container-0.4.0/pytest_container/runtime.py
--rw-r--r--   0        0        0     4842 1970-01-01 00:00:00.000000 pytest_container-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    26529 2024-04-03 11:39:43.392852 pytest_container-0.4.1/LICENSE
+-rw-r--r--   0        0        0     3098 2024-04-03 11:39:43.392852 pytest_container-0.4.1/README.rst
+-rw-r--r--   0        0        0     2075 2024-04-03 11:39:43.392852 pytest_container-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0      946 2024-04-03 11:39:43.392852 pytest_container-0.4.1/pytest_container/__init__.py
+-rw-r--r--   0        0        0    10564 2024-04-03 11:39:43.392852 pytest_container-0.4.1/pytest_container/build.py
+-rw-r--r--   0        0        0    42407 2024-04-03 11:39:43.392852 pytest_container-0.4.1/pytest_container/container.py
+-rw-r--r--   0        0        0     5725 2024-04-03 11:39:43.392852 pytest_container-0.4.1/pytest_container/helpers.py
+-rw-r--r--   0        0        0     8932 2024-04-03 11:39:43.392852 pytest_container-0.4.1/pytest_container/inspect.py
+-rw-r--r--   0        0        0      362 2024-04-03 11:39:43.392852 pytest_container-0.4.1/pytest_container/logging.py
+-rw-r--r--   0        0        0     7754 2024-04-03 11:39:43.392852 pytest_container-0.4.1/pytest_container/plugin.py
+-rw-r--r--   0        0        0     7973 2024-04-03 11:39:43.392852 pytest_container-0.4.1/pytest_container/pod.py
+-rw-r--r--   0        0        0    21722 2024-04-03 11:39:43.392852 pytest_container-0.4.1/pytest_container/runtime.py
+-rw-r--r--   0        0        0     4842 1970-01-01 00:00:00.000000 pytest_container-0.4.1/PKG-INFO
```

### Comparing `pytest_container-0.4.0/LICENSE` & `pytest_container-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_container-0.4.0/README.rst` & `pytest_container-0.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `pytest_container-0.4.0/pyproject.toml` & `pytest_container-0.4.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest_container"
-version = "0.4.0"
+version = "0.4.1"
 description = "Pytest fixtures for writing container based tests"
 authors = ["Dan Čermák <dcermak@suse.com>"]
 homepage = "https://dcermak.github.io/pytest_container/"
 repository = "https://github.com/dcermak/pytest_container/"
 readme = "README.rst"
 license = "LGPL-2.1-or-later"
 classifiers = [
```

### Comparing `pytest_container-0.4.0/pytest_container/__init__.py` & `pytest_container-0.4.1/pytest_container/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_container-0.4.0/pytest_container/build.py` & `pytest_container-0.4.1/pytest_container/build.py`

 * *Files identical despite different names*

### Comparing `pytest_container-0.4.0/pytest_container/container.py` & `pytest_container-0.4.1/pytest_container/container.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,19 +36,21 @@
 from typing import overload
 from typing import Tuple
 from typing import Type
 from typing import Union
 from uuid import uuid4
 
 import deprecation
-import pytest
 import testinfra
+from _pytest.mark import Mark
+from _pytest.mark import MarkDecorator
 from _pytest.mark import ParameterSet
 from filelock import BaseFileLock
 from filelock import FileLock
+from pytest import param
 from pytest_container.helpers import get_always_pull_option
 from pytest_container.inspect import ContainerHealth
 from pytest_container.inspect import ContainerInspect
 from pytest_container.inspect import PortForwarding
 from pytest_container.inspect import VolumeMount
 from pytest_container.logging import _logger
 from pytest_container.runtime import get_selected_runtime
@@ -892,82 +894,80 @@
 
         """
         return self._container_runtime.inspect_container(self.container_id)
 
 
 def container_to_pytest_param(
     container: ContainerBase,
-    marks: Optional[
-        Union[Collection[pytest.MarkDecorator], pytest.MarkDecorator]
-    ] = None,
+    marks: Optional[Union[Collection[MarkDecorator], MarkDecorator]] = None,
 ) -> ParameterSet:
     """Converts a subclass of :py:class:`~pytest_container.container.ContainerBase`
     (:py:class:`~pytest_container.container.Container` or
     :py:class:`~pytest_container.container.DerivedContainer`) into a
     `pytest.param
     <https://docs.pytest.org/en/stable/reference.html?#pytest.param>`_ with the
     given marks and sets the id of the parameter to the pretty printed version
     of the container (i.e. its
     :py:attr:`~pytest_container.container.ContainerBase.url` or
     :py:attr:`~pytest_container.container.ContainerBase.container_id`)
 
     """
-    return pytest.param(container, marks=marks or [], id=str(container))
+    return param(container, marks=marks or [], id=str(container))
 
 
 @overload
 def container_and_marks_from_pytest_param(
-    param: Container,
+    ctr_or_param: Container,
 ) -> Tuple[Container, Literal[None]]:
     ...
 
 
 @overload
 def container_and_marks_from_pytest_param(
-    param: DerivedContainer,
+    ctr_or_param: DerivedContainer,
 ) -> Tuple[DerivedContainer, Literal[None]]:
     ...
 
 
 @overload
 def container_and_marks_from_pytest_param(
-    param: ParameterSet,
+    ctr_or_param: ParameterSet,
 ) -> Tuple[
     Union[Container, DerivedContainer],
-    Optional[Collection[Union[pytest.MarkDecorator, pytest.Mark]]],
+    Optional[Collection[Union[MarkDecorator, Mark]]],
 ]:
     ...
 
 
 def container_and_marks_from_pytest_param(
-    param: Union[ParameterSet, Container, DerivedContainer],
+    ctr_or_param: Union[ParameterSet, Container, DerivedContainer],
 ) -> Tuple[
     Union[Container, DerivedContainer],
-    Optional[Collection[Union[pytest.MarkDecorator, pytest.Mark]]],
+    Optional[Collection[Union[MarkDecorator, Mark]]],
 ]:
     """Extracts the :py:class:`~pytest_container.container.Container` or
     :py:class:`~pytest_container.container.DerivedContainer` and the
     corresponding marks from a `pytest.param
     <https://docs.pytest.org/en/stable/reference.html?#pytest.param>`_ and
     returns both.
 
     If ``param`` is either a :py:class:`~pytest_container.container.Container`
     or a :py:class:`~pytest_container.container.DerivedContainer`, then param is
     returned directly and the second return value is ``None``.
 
     """
-    if isinstance(param, (Container, DerivedContainer)):
-        return param, None
+    if isinstance(ctr_or_param, (Container, DerivedContainer)):
+        return ctr_or_param, None
 
-    if len(param.values) > 0 and isinstance(
-        param.values[0], (Container, DerivedContainer)
+    if len(ctr_or_param.values) > 0 and isinstance(
+        ctr_or_param.values[0], (Container, DerivedContainer)
     ):
-        return param.values[0], param.marks
+        return ctr_or_param.values[0], ctr_or_param.marks
 
-    raise ValueError(f"Invalid pytest.param values: {param.values}")
+    raise ValueError(f"Invalid pytest.param values: {ctr_or_param.values}")
 
 
 @deprecation.deprecated(
     deprecated_in="0.4.0",
     removed_in="0.5.0",
     current_version=metadata.version("pytest_container"),
     details="use container_and_marks_from_pytest_param instead",
```

### Comparing `pytest_container-0.4.0/pytest_container/helpers.py` & `pytest_container-0.4.1/pytest_container/helpers.py`

 * *Files identical despite different names*

### Comparing `pytest_container-0.4.0/pytest_container/inspect.py` & `pytest_container-0.4.1/pytest_container/inspect.py`

 * *Files identical despite different names*

### Comparing `pytest_container-0.4.0/pytest_container/plugin.py` & `pytest_container-0.4.1/pytest_container/plugin.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,20 +22,21 @@
 from pytest_container.runtime import OciRuntimeBase
 
 if sys.version_info >= (3, 8):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-import pytest
+from pytest import fixture
+from pytest import skip
 from _pytest.config import Config
 from _pytest.fixtures import SubRequest
 
 
-@pytest.fixture(scope="session")
+@fixture(scope="session")
 def container_runtime() -> OciRuntimeBase:
     """pytest fixture that returns the currently selected container runtime
     according to the rules outlined :ref:`here <runtime selection rules>`.
 
     """
     return get_selected_runtime()
 
@@ -59,15 +60,15 @@
 
 
 def _create_auto_container_fixture(
     scope: Literal["session", "function"]
 ) -> Callable[
     [SubRequest, OciRuntimeBase, Config], Generator[ContainerData, None, None]
 ]:
-    def fixture(
+    def fixture_funct(
         request: SubRequest,
         # we must call this parameter container runtime, so that pytest will
         # treat it as a fixture, but that causes pylint to complain…
         # pylint: disable=redefined-outer-name
         container_runtime: OciRuntimeBase,
         pytestconfig: Config,
     ) -> Generator[ContainerData, None, None]:
@@ -121,32 +122,32 @@
                 yield container_data
             finally:
                 if launcher._container_id:
                     _log_container_logs(
                         launcher._container_id, container_runtime
                     )
 
-    return pytest.fixture(scope=scope)(fixture)
+    return fixture(scope=scope)(fixture_funct)
 
 
 def _create_auto_pod_fixture(
     scope: Literal["session", "function"]
 ) -> Callable[
     [SubRequest, OciRuntimeBase, Config], Generator[PodData, None, None]
 ]:
-    def fixture(
+    def fixture_funct(
         request: SubRequest,
         # we must call this parameter container runtime, so that pytest will
         # treat it as a fixture, but that causes pylint to complain…
         # pylint: disable=redefined-outer-name
         container_runtime: OciRuntimeBase,
         pytestconfig: Config,
     ) -> Generator[PodData, None, None]:
         if "podman" not in container_runtime.runner_binary:
-            pytest.skip("Pods are only supported in podman")
+            skip("Pods are only supported in podman")
 
         pod = pod_from_pytest_param(request.param)
         with PodLauncher(
             pod,
             rootdir=pytestconfig.rootpath,
             extra_build_args=get_extra_build_args(pytestconfig),
             extra_run_args=get_extra_run_args(pytestconfig),
@@ -159,15 +160,15 @@
             finally:
                 for ctr_launcher in launcher._launchers:
                     if ctr_launcher._container_id:
                         _log_container_logs(
                             ctr_launcher._container_id, container_runtime
                         )
 
-    return pytest.fixture(scope=scope)(fixture)
+    return fixture(scope=scope)(fixture_funct)
 
 
 #: This fixture parametrizes the test function once for each container image
 #: defined in the module level variable ``CONTAINER_IMAGES`` of the current test
 #: module and yield an instance of
 #: :py:attr:`~pytest_container.container.ContainerData`.
 #: This fixture will reuse the same container for all tests of the same session.
```

### Comparing `pytest_container-0.4.0/pytest_container/pod.py` & `pytest_container-0.4.1/pytest_container/pod.py`

 * *Files identical despite different names*

### Comparing `pytest_container-0.4.0/pytest_container/runtime.py` & `pytest_container-0.4.1/pytest_container/runtime.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 from typing import Any
 from typing import Callable
 from typing import List
 from typing import Optional
 from typing import TYPE_CHECKING
 from typing import Union
 
-import pytest
 import testinfra
 from _pytest.mark.structures import ParameterSet
+from pytest import param
 from pytest_container.inspect import BindMount
 from pytest_container.inspect import Config
 from pytest_container.inspect import ContainerHealth
 from pytest_container.inspect import ContainerInspect
 from pytest_container.inspect import ContainerNetworkSettings
 from pytest_container.inspect import ContainerState
 from pytest_container.inspect import HealthCheck
@@ -61,15 +61,15 @@
     a pytest.param with self.__str__() as the default id and optional marks
     """
 
     marks: Any = None
 
     def to_pytest_param(self) -> ParameterSet:
         """Convert this class into a ``pytest.param``"""
-        return pytest.param(self, id=str(self), marks=self.marks or ())
+        return param(self, id=str(self), marks=self.marks or ())
 
 
 @dataclass(frozen=True)
 class Version:
     """Representation of a version of the form
     ``$major.$minor.$patch[-|+]$release build $build``.
```

### Comparing `pytest_container-0.4.0/PKG-INFO` & `pytest_container-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest_container
-Version: 0.4.0
+Version: 0.4.1
 Summary: Pytest fixtures for writing container based tests
 Home-page: https://dcermak.github.io/pytest_container/
 License: LGPL-2.1-or-later
 Author: Dan Čermák
 Author-email: dcermak@suse.com
 Requires-Python: >=3.6.2,<4.0
 Classifier: Development Status :: 4 - Beta
```

