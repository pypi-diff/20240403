# Comparing `tmp/cosimtlk-0.6.1.tar.gz` & `tmp/cosimtlk-0.6.2.tar.gz`

## Comparing `cosimtlk-0.6.1.tar` & `cosimtlk-0.6.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
--rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/Makefile
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/__about__.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/__init__.py
--rw-r--r--   0        0        0    20686 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/_fmu.py
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/cli.py
--rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/client.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/models.py
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/app/__init__.py
--rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/app/client.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/app/config.py
--rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/app/dependencies.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/app/main.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/app/schemas.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/app/routers/__init__.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/app/routers/fmus.py
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/app/routers/simulators.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/app/services/__init__.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/app/services/simulator.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/simulation/__init__.py
--rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/simulation/environment.py
--rw-r--r--   0        0        0     5616 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/simulation/simulator.py
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/simulation/state.py
--rw-r--r--   0        0        0     4744 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/simulation/storage.py
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/simulation/utils.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/simulation/entities/__init__.py
--rw-r--r--   0        0        0     4239 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/simulation/entities/base.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/simulation/entities/fmu.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/simulation/entities/generic.py
--rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/simulation/entities/input.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/simulation/entities/oberver.py
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/src/cosimtlk/simulation/entities/stateobserver.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/tests/__init__.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/tests/conftest.py
--rwxr-xr-x   0        0        0   881408 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/tests/fixtures/fmus/ModSim.Examples.InputTest.fmu
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/tests/test_fmus/__init__.py
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/tests/test_fmus/test_local_fmu.py
--rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/tests/test_fmus/test_local_fmu_instance.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/tests/test_simulation/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/tests/test_simulation/test_storage/__init__.py
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/tests/test_simulation/test_storage/test_observation_store.py
--rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/tests/test_simulation/test_storage/test_schedule_store.py
--rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/tests/test_simulation/test_storage/test_state.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/tests/test_simulation/test_storage/test_utils.py
--rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/.gitignore
--rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/LICENCE
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/README.md
--rw-r--r--   0        0        0     4288 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     3236 2020-02-02 00:00:00.000000 cosimtlk-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     4414 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/Makefile
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/__about__.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/__init__.py
+-rw-r--r--   0        0        0    20686 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/_fmu.py
+-rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/cli.py
+-rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/client.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/models.py
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/app/__init__.py
+-rw-r--r--   0        0        0     4165 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/app/client.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/app/config.py
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/app/dependencies.py
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/app/main.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/app/schemas.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/app/routers/__init__.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/app/routers/fmus.py
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/app/routers/simulators.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/app/services/__init__.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/app/services/simulator.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/simulation/__init__.py
+-rw-r--r--   0        0        0     2616 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/simulation/environment.py
+-rw-r--r--   0        0        0     5855 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/simulation/simulator.py
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/simulation/state.py
+-rw-r--r--   0        0        0     4744 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/simulation/storage.py
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/simulation/utils.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/simulation/entities/__init__.py
+-rw-r--r--   0        0        0     4454 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/simulation/entities/base.py
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/simulation/entities/fmu.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/simulation/entities/generic.py
+-rw-r--r--   0        0        0     2806 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/simulation/entities/input.py
+-rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/simulation/entities/oberver.py
+-rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/src/cosimtlk/simulation/entities/stateobserver.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/tests/__init__.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/tests/conftest.py
+-rwxr-xr-x   0        0        0   881408 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/tests/fixtures/fmus/ModSim.Examples.InputTest.fmu
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/tests/test_fmus/__init__.py
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/tests/test_fmus/test_local_fmu.py
+-rw-r--r--   0        0        0     7207 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/tests/test_fmus/test_local_fmu_instance.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/tests/test_simulation/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/tests/test_simulation/test_storage/__init__.py
+-rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/tests/test_simulation/test_storage/test_observation_store.py
+-rw-r--r--   0        0        0     4026 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/tests/test_simulation/test_storage/test_schedule_store.py
+-rw-r--r--   0        0        0     1324 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/tests/test_simulation/test_storage/test_state.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/tests/test_simulation/test_storage/test_utils.py
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/.gitignore
+-rw-r--r--   0        0        0     1512 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/LICENCE
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/README.md
+-rw-r--r--   0        0        0     4287 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 cosimtlk-0.6.2/PKG-INFO
```

### Comparing `cosimtlk-0.6.1/Makefile` & `cosimtlk-0.6.2/Makefile`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.1/src/cosimtlk/_fmu.py` & `cosimtlk-0.6.2/src/cosimtlk/_fmu.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.1/src/cosimtlk/cli.py` & `cosimtlk-0.6.2/src/cosimtlk/cli.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.1/src/cosimtlk/client.py` & `cosimtlk-0.6.2/src/cosimtlk/client.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.1/src/cosimtlk/app/client.py` & `cosimtlk-0.6.2/src/cosimtlk/app/client.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.1/src/cosimtlk/app/routers/fmus.py` & `cosimtlk-0.6.2/src/cosimtlk/app/routers/fmus.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.1/src/cosimtlk/app/routers/simulators.py` & `cosimtlk-0.6.2/src/cosimtlk/app/routers/simulators.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.1/src/cosimtlk/app/services/simulator.py` & `cosimtlk-0.6.2/src/cosimtlk/app/services/simulator.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.1/src/cosimtlk/simulation/environment.py` & `cosimtlk-0.6.2/src/cosimtlk/simulation/environment.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.1/src/cosimtlk/simulation/simulator.py` & `cosimtlk-0.6.2/src/cosimtlk/simulation/simulator.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,22 +4,24 @@
 
 import numpy as np
 from simpy.util import start_delayed
 
 from cosimtlk.models import DateTimeLike
 from cosimtlk.simulation.entities import Entity
 from cosimtlk.simulation.environment import Environment
+from cosimtlk.simulation.state import SimulationState
 from cosimtlk.simulation.utils import ensure_tz
 
 
 class Simulator:
     def __init__(
         self,
         *,
         initial_time: DateTimeLike,
+        state: SimulationState,
         entities: list[Entity] | None = None,
         logger: logging.Logger | None = None,
         **kwargs,
     ) -> None:
         """Simulation runner.
 
         Organizes the entities processes into a discrete event simulation. If multiple entities would run at the same
@@ -34,14 +36,15 @@
         self.tzinfo: ZoneInfo = initial_time.tzinfo
 
         # Set up logger
         self._logger = logger or logging.getLogger(__name__)
 
         # Create simulation environment
         self._environment = Environment(initial_time=initial_timestamp)
+        self._state = state
 
         # Add entities to the simulation
         self._current_process = 0
         self._process_delays = np.linspace(0.005, 0.995, 10000)
         self._entities: dict[str, Entity] = {}
         for entity in entities or []:
             self.add_entity(entity)
@@ -102,14 +105,19 @@
 
     @property
     def logger(self) -> logging.Logger:
         """The logger for the simulation."""
         return self._logger
 
     @property
+    def state(self) -> SimulationState:
+        """The state of the simulation."""
+        return self._state
+
+    @property
     def env(self) -> Environment:
         """The simulation environment."""
         return self._environment
 
     @property
     def current_timestamp(self) -> int:
         """The current simulation time as a unix timestamp."""
```

### Comparing `cosimtlk-0.6.1/src/cosimtlk/simulation/state.py` & `cosimtlk-0.6.2/src/cosimtlk/simulation/state.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.1/src/cosimtlk/simulation/storage.py` & `cosimtlk-0.6.2/src/cosimtlk/simulation/storage.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.1/src/cosimtlk/simulation/utils.py` & `cosimtlk-0.6.2/src/cosimtlk/simulation/utils.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.1/src/cosimtlk/simulation/entities/base.py` & `cosimtlk-0.6.2/src/cosimtlk/simulation/entities/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -108,31 +108,41 @@
             Timeout event.
         """
         duration = ts - self.ctx.current_timestamp
         return self.wait_for(duration)
 
 
 class Source(Entity, metaclass=ABCMeta):
+
+    def __init__(self, name: str):
+        super().__init__(name)
+        self._build_count = 0
+
     @property
     def processes(self) -> list[Callable[[], Generator]]:
         return [self.generate]
 
     @abstractmethod
     def interarrival_time(self) -> int | float:
         raise NotImplementedError
 
     @abstractmethod
     def build_entity(self):
         raise NotImplementedError
 
+    @property
+    def build_count(self) -> int:
+        return self._build_count
+
     def _generate_interarrival_time(self):
         # if first_creation exists, emit it as the first time, else just use the interarrival_time
         while True:
             yield self.interarrival_time()
 
     def generate(self):
         for arrival_time in self._generate_interarrival_time():
             timeout = self.wait_for(arrival_time)
             yield timeout
             entity = self.build_entity()
+            self._build_count += 1
             self.ctx.add_entity(entity)
             self.log.debug(f"created entity={entity} with attributes={entity.attributes}")
```

### Comparing `cosimtlk-0.6.1/src/cosimtlk/simulation/entities/fmu.py` & `cosimtlk-0.6.2/src/cosimtlk/simulation/entities/fmu.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.1/src/cosimtlk/simulation/entities/generic.py` & `cosimtlk-0.6.2/src/cosimtlk/simulation/entities/generic.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.1/src/cosimtlk/simulation/entities/input.py` & `cosimtlk-0.6.2/src/cosimtlk/simulation/entities/input.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.1/src/cosimtlk/simulation/entities/oberver.py` & `cosimtlk-0.6.2/src/cosimtlk/simulation/entities/oberver.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.1/src/cosimtlk/simulation/entities/stateobserver.py` & `cosimtlk-0.6.2/src/cosimtlk/simulation/entities/stateobserver.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.1/tests/conftest.py` & `cosimtlk-0.6.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.1/tests/fixtures/fmus/ModSim.Examples.InputTest.fmu` & `cosimtlk-0.6.2/tests/fixtures/fmus/ModSim.Examples.InputTest.fmu`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.1/tests/test_fmus/test_local_fmu.py` & `cosimtlk-0.6.2/tests/test_fmus/test_local_fmu.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.1/tests/test_fmus/test_local_fmu_instance.py` & `cosimtlk-0.6.2/tests/test_fmus/test_local_fmu_instance.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.1/tests/test_simulation/test_storage/test_observation_store.py` & `cosimtlk-0.6.2/tests/test_simulation/test_storage/test_observation_store.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.1/tests/test_simulation/test_storage/test_schedule_store.py` & `cosimtlk-0.6.2/tests/test_simulation/test_storage/test_schedule_store.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.1/tests/test_simulation/test_storage/test_state.py` & `cosimtlk-0.6.2/tests/test_simulation/test_storage/test_state.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.1/tests/test_simulation/test_storage/test_utils.py` & `cosimtlk-0.6.2/tests/test_simulation/test_storage/test_utils.py`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.1/.gitignore` & `cosimtlk-0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.1/LICENCE` & `cosimtlk-0.6.2/LICENCE`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.1/README.md` & `cosimtlk-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `cosimtlk-0.6.1/pyproject.toml` & `cosimtlk-0.6.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "cosimtlk"
 dynamic = ["version"]
 description = 'Cosimulation toolkit.'
 readme = "README.md"
 requires-python = ">=3.10"
-license = "BSD-2-Clause"
+license = "BSD-3-Clause"
 keywords = []
 authors = [
     { name = "Attila Balint", email = "attila.balint@kuleuven.be" },
 ]
 packages = [{ include = "cosimtlk", from = "src" }]
 classifiers = [
     "Development Status :: 4 - Beta",
@@ -29,15 +29,15 @@
     "License :: OSI Approved :: BSD License",
 ]
 dependencies = [
     "attrs>=23.0.0,<24.0.0",
     "cattrs>=23.0.0,<24.0.0",
     "cron_converter>=1.0.0,<2.0.0",
     "FMPy>=0.3.0,<0.4.0",
-    "pandas>=1.4.0,<=3.1.0",
+    "pandas>=1.4.0,<3.0.0",
     "simpy>=4.0.0,<5.0.0",
     "tqdm>=4.0.0,<5.0.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/attila-balint-kul/cosimulation-toolkit"
 Source = "https://github.com/attila-balint-kul/cosimulation-toolkit"
```

### Comparing `cosimtlk-0.6.1/PKG-INFO` & `cosimtlk-0.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.3
 Name: cosimtlk
-Version: 0.6.1
+Version: 0.6.2
 Summary: Cosimulation toolkit.
 Project-URL: Homepage, https://github.com/attila-balint-kul/cosimulation-toolkit
 Project-URL: Source, https://github.com/attila-balint-kul/cosimulation-toolkit
 Project-URL: Documentation, https://github.com/attila-balint-kul/cosimulation-toolkit#readme
 Project-URL: Issues, https://github.com/attila-balint-kul/cosimulation-toolkit/issues
 Author-email: Attila Balint <attila.balint@kuleuven.be>
-License-Expression: BSD-2-Clause
+License-Expression: BSD-3-Clause
 License-File: LICENCE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
@@ -22,15 +22,15 @@
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.10
 Requires-Dist: attrs<24.0.0,>=23.0.0
 Requires-Dist: cattrs<24.0.0,>=23.0.0
 Requires-Dist: cron-converter<2.0.0,>=1.0.0
 Requires-Dist: fmpy<0.4.0,>=0.3.0
-Requires-Dist: pandas<=3.1.0,>=1.4.0
+Requires-Dist: pandas<3.0.0,>=1.4.0
 Requires-Dist: simpy<5.0.0,>=4.0.0
 Requires-Dist: tqdm<5.0.0,>=4.0.0
 Provides-Extra: server
 Requires-Dist: fastapi<1.0.0,>=0.100.0; extra == 'server'
 Requires-Dist: pydantic-settings<3.0.0,>=2.0.0; extra == 'server'
 Requires-Dist: pydantic>=2.0.0; extra == 'server'
 Requires-Dist: requests<3.0.0,>=2.26.0; extra == 'server'
```

