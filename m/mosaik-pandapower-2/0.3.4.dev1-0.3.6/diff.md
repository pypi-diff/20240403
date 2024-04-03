# Comparing `tmp/mosaik_pandapower_2-0.3.4.dev1.tar.gz` & `tmp/mosaik_pandapower_2-0.3.6.tar.gz`

## Comparing `mosaik_pandapower_2-0.3.4.dev1.tar` & `mosaik_pandapower_2-0.3.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 mosaik_pandapower_2-0.3.4.dev1/mosaik_components/pandapower/__init__.py
--rw-r--r--   0        0        0    15500 2020-02-02 00:00:00.000000 mosaik_pandapower_2-0.3.4.dev1/mosaik_components/pandapower/simulator.py
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 mosaik_pandapower_2-0.3.4.dev1/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 mosaik_pandapower_2-0.3.4.dev1/LICENSE
--rw-r--r--   0        0        0     9524 2020-02-02 00:00:00.000000 mosaik_pandapower_2-0.3.4.dev1/README.md
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 mosaik_pandapower_2-0.3.4.dev1/pyproject.toml
--rw-r--r--   0        0        0    10050 2020-02-02 00:00:00.000000 mosaik_pandapower_2-0.3.4.dev1/PKG-INFO
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 mosaik_pandapower_2-0.3.6/mosaik_components/pandapower/__init__.py
+-rw-r--r--   0        0        0    16745 2020-02-02 00:00:00.000000 mosaik_pandapower_2-0.3.6/mosaik_components/pandapower/simulator.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 mosaik_pandapower_2-0.3.6/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 mosaik_pandapower_2-0.3.6/LICENSE
+-rw-r--r--   0        0        0    10836 2020-02-02 00:00:00.000000 mosaik_pandapower_2-0.3.6/README.md
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 mosaik_pandapower_2-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0    11355 2020-02-02 00:00:00.000000 mosaik_pandapower_2-0.3.6/PKG-INFO
```

### Comparing `mosaik_pandapower_2-0.3.4.dev1/mosaik_components/pandapower/simulator.py` & `mosaik_pandapower_2-0.3.6/mosaik_components/pandapower/simulator.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,14 +116,33 @@
             "children": child_entities,
             "rel": [],
         }
 
     def get_extra_info(self) -> dict[EntityId, Any]:
         return self._extra_info
 
+    def get_net(self) -> pp.pandapowerNet:
+        return self._net
+
+    def disable_elements(self, elements: list[str]) -> None:
+        for eid in elements:
+            model, idx = self.get_model_and_idx(eid)
+            elem_spec = MODEL_TO_ELEMENT_SPECS[model]
+            if not elem_spec.can_switch_off:
+                raise ValueError(f"{model} elements cannot be disabled")
+            self._net[elem_spec.elem].loc[idx, "in_service"] = False
+
+    def enable_elements(self, elements: list[str]) -> None:
+        for eid in elements:
+            model, idx = self.get_model_and_idx(eid)
+            elem_spec = MODEL_TO_ELEMENT_SPECS[model]
+            if not elem_spec.can_switch_off:
+                raise ValueError(f"{model} elements cannot be enabled")
+            self._net[elem_spec.elem].loc[idx, "in_service"] = True
+
     def create_controlled_gen(self, bus: int) -> CreateResult:
         idx = pp.create_gen(self._net, bus, p_mw=0.0)
         return {
             "type": "ControlledGen",
             "eid": f"ControlledGen-{idx}",
             "children": [],
             "rel": [f"Bus-{bus}"],
@@ -233,14 +252,21 @@
     params: list[str] = field(default_factory=list)
     """The mosaik params that may be given when creating this element.
     (Only sensible if ``createable=True``.)
     """
     get_extra_info: Callable[[Any, pp.pandapowerNet], dict[str, Any]] = (  # noqa: E731
         lambda _net, _idx: {}
     )
+    """Function returning the extra info for this type of element given
+    the net and the element's index.
+    """
+    can_switch_off: bool = False
+    """Whether elements of this type may be switched off (and on) using
+    the *disable_element* (*enable_element*) extra methods.
+    """
 
 
 MODEL_TO_ELEMENT_SPECS = {
     "Bus": ModelToElementSpec(
         elem="bus",
         connected_buses=[],
         input_attr_specs={
@@ -279,19 +305,19 @@
         elem="load",
         connected_buses=["bus"],
         input_attr_specs={},
         out_attr_to_column={
             "P[MW]": "p_mw",
             "Q[MVar]": "q_mvar",
         },
-        get_extra_info=lambda elem_tuple, _net: {
-            "profile": elem_tuple.profile,
-        }
-        if "profile" in elem_tuple._fields
-        else {},
+        get_extra_info=lambda elem, _net: {
+            "bus": elem.bus,
+            **({"profile": elem.profile} if "profile" in elem._fields else {}),
+        },
+        can_switch_off=True,
     ),
     "StaticGen": ModelToElementSpec(
         elem="sgen",
         connected_buses=["bus"],
         input_attr_specs={},
         out_attr_to_column={
             "P[MW]": "p_mw",
@@ -373,27 +399,32 @@
             "public": True,
             "params": ["json", "xlsx", "net", "simbench", "network_function", "params"],
             "attrs": [],
             "any_inputs": False,
         },
         **ELEM_META_MODELS,
     },
-    "extra_methods": ["get_extra_info"],
+    "extra_methods": [
+        "get_extra_info",
+        "get_net",
+        "disable_elements",
+        "enable_elements",
+    ],
 }
 
 
 def apply_profiles(net: pp.pandapowerNet, profiles: Any, step: int):
     """Apply element profiles for the given step to the grid.
 
     :param profiles: profiles for elements in the format returned by
         simbench's ``get_absolute_values`` function.
     :param step: the time step to apply
     """
     for (elm, param), series in profiles.items():
-        net[elm].loc[:, param].update(series.loc[step])  # type: ignore
+        net[elm].update(series.loc[step].rename(param))  # type: ignore
 
 
 def load_grid(params: dict[str, Any]) -> tuple[pp.pandapowerNet, Any]:
     """Load a grid and the associated element profiles (if any).
 
     :param params: A dictionary describing which grid to load. It should
         contain one of the following keys (or key combinations).
```

### Comparing `mosaik_pandapower_2-0.3.4.dev1/LICENSE` & `mosaik_pandapower_2-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mosaik_pandapower_2-0.3.4.dev1/README.md` & `mosaik_pandapower_2-0.3.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -178,14 +178,41 @@
 |               | `Va[deg]`      | Out    | the voltage angle for this generator                   |
 | ControlledGen |                |        |**a generator created by the user to control**          |
 | Line          |                |        | **a line in the grid**                                 |
 |               | `I[kA]`        | Out    | the current along the line                             |
 |               | `loading[%]`   | Out    | the loading of the line                                |
 
 
+### Getting the net
+
+The simulator offers a `get_net` extra method which can be called on the simulator object in your mosaik scenario, once you have created the *Grid* entity.
+It will return the internal `pandapowerNet` object for the grid.
+
+**Note**: This method exists purely for visualization and debugging purposes.
+If you change values on this objects, the simulation might crash or the results might be silently incorrect.
+
+**Note**: This method only works if you run the adapter in the same Python process as your scenario (i.e. if you start the simulator using the `"python"` option in your sim config).
+It is not possible to pass the `pandapowerNet` object between processes.
+
+
+### Disabling existing elements
+
+This simulator purposefully does not allow you to overwrite the values of loads and other elements that already exist in the grid.
+However, you may switch them off entirely.
+For this, use the `disable_elements` extra method.
+If `loads` is a list of *Load* entities that you want to disable, you can achieve this via
+
+```python
+pp_sim.disable_elements([load.eid for load in loads])
+```
+
+This works by setting the element's *in_service* value to `False`.
+You can undo this (or enable elements that are not in service in your grid file) by using the analogous `enable_elements` extra method.
+
+
 ## Development
 
 For the development of this simulator, the following tools are employed:
 
 -   [Hatch](https://hatch.pypa.io/latest/) is used as a packaging manager.
     This offers the following commands:
```

### Comparing `mosaik_pandapower_2-0.3.4.dev1/pyproject.toml` & `mosaik_pandapower_2-0.3.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 ]
 license = "MIT"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
   "mosaik-api-v3 ~= 3.0.4",
   "loguru ~= 0.7.2",
-  "pandapower ~= 2.13.1",
+  "pandapower ~= 2.14",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 simbench = [
   "simbench ~= 1.4.0",
 ]
@@ -30,22 +30,18 @@
 
 [tool.hatch.envs.default]
 features = [
   "simbench",
   "numba",
 ]
 dependencies = [
-  "mosaik ~= 3.2.0",
-]
-
-[tool.hatch.envs.test]
-dependencies = [
+  "mosaik ~= 3.2",
   "pytest ~= 7.3.1",
-  "pytest-watch ~= 4.2.0",
   "pyarrow ~= 15.0.0",
+  "pytest-cov ~= 5.0",
 ]
 
 [tool.hatch.envs.test.scripts]
 test = "pytest {args:tests}"
 
 [[tool.hatch.envs.test.matrix]]
 # Remember to also change .gitlab-ci.yml if you change the Python versions here
@@ -68,25 +64,22 @@
   "plotly ~= 5.18.0",
   "matplotlib ~= 3.8.2",
   "nbformat ~= 5.9.2",
   "ipykernel ~= 6.27.1",
 ]
 
 [tool.pytest.ini_options]
-pythonpath = ["tests"]
-addopts = [
-  "--import-mode=importlib"
-]
 filterwarnings = [
-  "ignore:ChainedAssignmentError:FutureWarning",
-  "ignore:Passing literal json:FutureWarning",
-  "ignore:Setting an item:FutureWarning",
-  "ignore:A value is trying:FutureWarning",
-  "ignore:The behavior of DataFrame concatenation:FutureWarning",
-  "ignore:Downcasting object:FutureWarning",
+  "error",
+  "ignore::FutureWarning:simbench",
+]
+
+[tool.coverage.run]
+omit = [
+  "tests/**",
 ]
 
 [tool.ruff]
 line-length = 88
 indent-width = 4
 target-version = "py39"
```

### Comparing `mosaik_pandapower_2-0.3.4.dev1/PKG-INFO` & `mosaik_pandapower_2-0.3.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: mosaik-pandapower-2
-Version: 0.3.4.dev1
+Version: 0.3.6
 Summary: An adapter to connect mosaik to pandapower
 Author-email: Eike Schulte <eike.schulte@offis.de>
 License-Expression: MIT
 License-File: LICENSE
 Requires-Python: >=3.9
 Requires-Dist: loguru~=0.7.2
 Requires-Dist: mosaik-api-v3~=3.0.4
-Requires-Dist: pandapower~=2.13.1
+Requires-Dist: pandapower~=2.14
 Provides-Extra: numba
 Requires-Dist: numba~=0.58.1; extra == 'numba'
 Provides-Extra: simbench
 Requires-Dist: simbench~=1.4.0; extra == 'simbench'
 Description-Content-Type: text/markdown
 
 # mosaik-pandapower-2
@@ -195,14 +195,41 @@
 |               | `Va[deg]`      | Out    | the voltage angle for this generator                   |
 | ControlledGen |                |        |**a generator created by the user to control**          |
 | Line          |                |        | **a line in the grid**                                 |
 |               | `I[kA]`        | Out    | the current along the line                             |
 |               | `loading[%]`   | Out    | the loading of the line                                |
 
 
+### Getting the net
+
+The simulator offers a `get_net` extra method which can be called on the simulator object in your mosaik scenario, once you have created the *Grid* entity.
+It will return the internal `pandapowerNet` object for the grid.
+
+**Note**: This method exists purely for visualization and debugging purposes.
+If you change values on this objects, the simulation might crash or the results might be silently incorrect.
+
+**Note**: This method only works if you run the adapter in the same Python process as your scenario (i.e. if you start the simulator using the `"python"` option in your sim config).
+It is not possible to pass the `pandapowerNet` object between processes.
+
+
+### Disabling existing elements
+
+This simulator purposefully does not allow you to overwrite the values of loads and other elements that already exist in the grid.
+However, you may switch them off entirely.
+For this, use the `disable_elements` extra method.
+If `loads` is a list of *Load* entities that you want to disable, you can achieve this via
+
+```python
+pp_sim.disable_elements([load.eid for load in loads])
+```
+
+This works by setting the element's *in_service* value to `False`.
+You can undo this (or enable elements that are not in service in your grid file) by using the analogous `enable_elements` extra method.
+
+
 ## Development
 
 For the development of this simulator, the following tools are employed:
 
 -   [Hatch](https://hatch.pypa.io/latest/) is used as a packaging manager.
     This offers the following commands:
```

