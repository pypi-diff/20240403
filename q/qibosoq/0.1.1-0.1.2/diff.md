# Comparing `tmp/qibosoq-0.1.1.tar.gz` & `tmp/qibosoq-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qibosoq-0.1.1.tar", max compression
+gzip compressed data, was "qibosoq-0.1.2.tar", max compression
```

## Comparing `qibosoq-0.1.1.tar` & `qibosoq-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2024-01-08 09:18:50.552272 qibosoq-0.1.1/LICENSE
--rw-r--r--   0        0        0     2400 2024-01-08 09:18:50.552272 qibosoq-0.1.1/README.md
--rw-r--r--   0        0        0     1730 2024-01-08 09:18:50.556272 qibosoq-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       94 2024-01-08 09:18:50.556272 qibosoq-0.1.1/src/qibosoq/__init__.py
--rw-r--r--   0        0        0      422 2024-01-08 09:18:50.556272 qibosoq-0.1.1/src/qibosoq/__main__.py
--rw-r--r--   0        0        0     2046 2024-01-08 09:18:50.556272 qibosoq-0.1.1/src/qibosoq/client.py
--rw-r--r--   0        0        0       22 2024-01-08 09:18:50.556272 qibosoq-0.1.1/src/qibosoq/components/__init__.py
--rw-r--r--   0        0        0     3017 2024-01-08 09:18:50.556272 qibosoq-0.1.1/src/qibosoq/components/base.py
--rw-r--r--   0        0        0     4036 2024-01-08 09:18:50.556272 qibosoq-0.1.1/src/qibosoq/components/pulses.py
--rw-r--r--   0        0        0      983 2024-01-08 09:18:50.556272 qibosoq-0.1.1/src/qibosoq/configuration.py
--rw-r--r--   0        0        0     1263 2024-01-08 09:18:50.556272 qibosoq-0.1.1/src/qibosoq/log.py
--rw-r--r--   0        0        0       23 2024-01-08 09:18:50.556272 qibosoq-0.1.1/src/qibosoq/programs/__init__.py
--rw-r--r--   0        0        0    12816 2024-01-08 09:18:50.556272 qibosoq-0.1.1/src/qibosoq/programs/base.py
--rw-r--r--   0        0        0     6998 2024-01-08 09:18:50.556272 qibosoq-0.1.1/src/qibosoq/programs/flux.py
--rw-r--r--   0        0        0      638 2024-01-08 09:18:50.556272 qibosoq-0.1.1/src/qibosoq/programs/pulse_sequence.py
--rw-r--r--   0        0        0     6155 2024-01-08 09:18:50.556272 qibosoq-0.1.1/src/qibosoq/programs/sweepers.py
--rw-r--r--   0        0        0        0 2024-01-08 09:18:50.556272 qibosoq-0.1.1/src/qibosoq/py.typed
--rw-r--r--   0        0        0     5570 2024-01-08 09:18:50.556272 qibosoq-0.1.1/src/qibosoq/server.py
--rw-r--r--   0        0        0     3293 1970-01-01 00:00:00.000000 qibosoq-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-03 08:10:11.189061 qibosoq-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3352 2024-04-03 08:10:11.189061 qibosoq-0.1.2/README.md
+-rw-r--r--   0        0        0     1730 2024-04-03 08:10:11.193061 qibosoq-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       94 2024-04-03 08:10:11.193061 qibosoq-0.1.2/src/qibosoq/__init__.py
+-rw-r--r--   0        0        0      422 2024-04-03 08:10:11.193061 qibosoq-0.1.2/src/qibosoq/__main__.py
+-rw-r--r--   0        0        0     2046 2024-04-03 08:10:11.193061 qibosoq-0.1.2/src/qibosoq/client.py
+-rw-r--r--   0        0        0       22 2024-04-03 08:10:11.193061 qibosoq-0.1.2/src/qibosoq/components/__init__.py
+-rw-r--r--   0        0        0     3017 2024-04-03 08:10:11.193061 qibosoq-0.1.2/src/qibosoq/components/base.py
+-rw-r--r--   0        0        0     4036 2024-04-03 08:10:11.193061 qibosoq-0.1.2/src/qibosoq/components/pulses.py
+-rw-r--r--   0        0        0      984 2024-04-03 08:10:11.193061 qibosoq-0.1.2/src/qibosoq/configuration.py
+-rw-r--r--   0        0        0     1263 2024-04-03 08:10:11.193061 qibosoq-0.1.2/src/qibosoq/log.py
+-rw-r--r--   0        0        0       23 2024-04-03 08:10:11.193061 qibosoq-0.1.2/src/qibosoq/programs/__init__.py
+-rw-r--r--   0        0        0    13340 2024-04-03 08:10:11.197061 qibosoq-0.1.2/src/qibosoq/programs/base.py
+-rw-r--r--   0        0        0     6996 2024-04-03 08:10:11.197061 qibosoq-0.1.2/src/qibosoq/programs/flux.py
+-rw-r--r--   0        0        0     1135 2024-04-03 08:10:11.197061 qibosoq-0.1.2/src/qibosoq/programs/pulse_sequence.py
+-rw-r--r--   0        0        0     6273 2024-04-03 08:10:11.197061 qibosoq-0.1.2/src/qibosoq/programs/sweepers.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:10:11.197061 qibosoq-0.1.2/src/qibosoq/py.typed
+-rw-r--r--   0        0        0     5570 2024-04-03 08:10:11.197061 qibosoq-0.1.2/src/qibosoq/server.py
+-rw-r--r--   0        0        0     4245 1970-01-01 00:00:00.000000 qibosoq-0.1.2/PKG-INFO
```

### Comparing `qibosoq-0.1.1/LICENSE` & `qibosoq-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qibosoq-0.1.1/pyproject.toml` & `qibosoq-0.1.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qibosoq"
-version = "0.1.1"
+version = "0.1.2"
 description = "QIBO Server On Qick (qibosoq) is the server component of qibolab to be run on RFSoC boards"
 authors = [
   "Rodolfo Carobene <rodolfo.carobene@gmail.com>",
   "Javier Serrano <javier.serrano@tii.ae>",
 ]
 license = "Apache License 2.0"
 readme = "README.md"
@@ -15,15 +15,15 @@
   "Programming Language :: Python :: 3",
   "Topic :: Scientific/Engineering :: Physics",
 ]
 packages = [{ include = "qibosoq", from = "src" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.12"
-qick = ">=0.2.165, <=0.2.181"
+qick = ">=0.2.211, <=0.2.249"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.group.docs]
 optional = true
```

### Comparing `qibosoq-0.1.1/src/qibosoq/client.py` & `qibosoq-0.1.2/src/qibosoq/client.py`

 * *Files identical despite different names*

### Comparing `qibosoq-0.1.1/src/qibosoq/components/base.py` & `qibosoq-0.1.2/src/qibosoq/components/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 import numpy.typing as npt
 
 
 @dataclass
 class Config:
     """General RFSoC Configuration."""
 
-    repetition_duration: int = 100
+    relaxation_time: float = 100
     """Time to wait between shots (us)."""
-    adc_trig_offset: int = 200
+    ro_time_of_flight: int = 200
     """Time to wait between readout pulse and acquisition (ADC clock ticks)."""
     reps: int = 1000
     """Number of shots."""
     soft_avgs: int = 1
     """Number of software averages."""
     average: bool = True
     """Returns integrated results if true."""
```

### Comparing `qibosoq-0.1.1/src/qibosoq/components/pulses.py` & `qibosoq-0.1.2/src/qibosoq/components/pulses.py`

 * *Files identical despite different names*

### Comparing `qibosoq-0.1.1/src/qibosoq/configuration.py` & `qibosoq-0.1.2/src/qibosoq/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Qibosoq configuration file."""
+
 import os
 
 
 def from_env(name, default=None):
     """Get the value of a QIBOSOQ environment variable."""
     return os.getenv(f"QIBOSOQ_{name}", default)
```

### Comparing `qibosoq-0.1.1/src/qibosoq/log.py` & `qibosoq-0.1.2/src/qibosoq/log.py`

 * *Files identical despite different names*

### Comparing `qibosoq-0.1.1/src/qibosoq/programs/base.py` & `qibosoq-0.1.2/src/qibosoq/programs/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Base program used by qibosoq to execute sequences and sweeps."""
 
 import logging
 from abc import ABC, abstractmethod
 from dataclasses import asdict
-from typing import Dict, List, Tuple
+from typing import Dict, List, Tuple, Union
 
 import numpy as np
 from qick import QickProgram, QickSoc
 
 import qibosoq.configuration as qibosoq_cfg
 from qibosoq.components.base import Config, Qubit
 from qibosoq.components.pulses import (
@@ -29,39 +29,38 @@
 
     def __init__(
         self, soc: QickSoc, qpcfg: Config, sequence: List[Element], qubits: List[Qubit]
     ):
         """In this function we define the most important settings.
 
         In detail:
-            * max_gain, adc_trig_offset, max_sampling_rate, reps are imported from
+            * max_gain, ro_time_of_flight, max_sampling_rate, reps are imported from
               qpcfg (runcard settings)
             * relaxdelay (for each execution) is taken from qpcfg (runcard)
             * syncdelay (for each measurement) is defined explicitly
             * wait_initialize is defined explicitly
             * super.__init__ (this will init AveragerProgram or RAveragerProgram)
         """
         self.soc = soc
         self.soccfg = soc  # this is used by qick
 
         self.sequence = sequence
         self.pulse_sequence = [elem for elem in sequence if isinstance(elem, Pulse)]
         self.qubits = qubits
 
         # general settings
-        self.adc_trig_offset = qpcfg.adc_trig_offset
-        self.reps = qpcfg.reps
+        self.ro_time_of_flight = qpcfg.ro_time_of_flight
 
         # mux settings
         self.is_mux = qibosoq_cfg.IS_MULTIPLEXED
         self.readouts_per_experiment = len(
             [elem for elem in self.sequence if elem.type == "readout"]
         )
 
-        self.relax_delay = self.us2cycles(qpcfg.repetition_duration)
+        self.relax_delay = self.us2cycles(qpcfg.relaxation_time)
         self.syncdelay = self.us2cycles(0)
         self.wait_initialize = self.us2cycles(2.0)
 
         self.pulses_registered = False
         self.registered_waveforms: Dict[int, list] = {}
         for pulse in self.pulse_sequence:
             if pulse.dac not in self.registered_waveforms:
@@ -212,20 +211,20 @@
                 self.add_pulse_to_register(elem)
             adcs = [elem.adc]
 
         if isinstance(elem, Pulse):  #
             self.measure(
                 pulse_ch=elem.dac,
                 adcs=adcs,
-                adc_trig_offset=self.adc_trig_offset,
+                adc_trig_offset=self.ro_time_of_flight,
                 wait=False,
                 syncdelay=self.syncdelay,
             )
         elif isinstance(elem, Measurement):
-            self.trigger(adcs, adc_trig_offset=self.adc_trig_offset)
+            self.trigger(adcs, adc_trig_offset=self.ro_time_of_flight)
             if self.syncdelay is not None:
                 self.sync_all(self.syncdelay)
 
     def perform_experiment(
         self,
         soc: QickSoc,
         average: bool = False,
@@ -237,52 +236,65 @@
         Args:
             average (bool): if true return averaged res, otherwise single shots
         """
         readouts_per_experiment = self.readouts_per_experiment
         # if there are no readouts, temporaray set 1 so that qick can execute properly
         reads_per_rep = 1 if readouts_per_experiment == 0 else readouts_per_experiment
 
-        res = self.acquire(  # pylint: disable=E1123
+        res = self.acquire(  # pylint: disable=E1123,E1120
             soc,
             readouts_per_experiment=reads_per_rep,
         )
         # if there are no actual readouts, return empty lists
         if readouts_per_experiment == 0:
             return [], []
         if average:
             # for sweeps res has 3 parameters, the first is not used
             return np.array(res[-2]).tolist(), np.array(res[-1]).tolist()
         # super().acquire function fill buffers used in collect_shots
         return self.collect_shots()[-2:]
 
     def collect_shots(self) -> Tuple[list, list]:
         """Read the internal buffers and returns single shots (i,q)."""
-        tot_i = []
-        tot_q = []
-
         adcs = []  # list of adcs per readouts (not unique values)
         lengths = []  # length of readouts (only one per adcs)
         for elem in (elem for elem in self.sequence if elem.type == "readout"):
             adc_ch = elem.adc
             ro_ch = elem.dac
             if adc_ch not in adcs:
                 lengths.append(self.soc.us2cycles(elem.duration, gen_ch=ro_ch))
             adcs.append(adc_ch)
 
         unique_adcs, adc_count = np.unique(adcs, return_counts=True)
 
-        for idx, adc_ch in enumerate(unique_adcs):
-            count = adc_count[idx]
-            shape = (count, self.expts, self.reps) if self.expts else (count, self.reps)
-            i_val = self.di_buf[idx].reshape(shape) / lengths[idx]
-            q_val = self.dq_buf[idx].reshape(shape) / lengths[idx]
-
-            tot_i.append(i_val.tolist())
-            tot_q.append(q_val.tolist())
-        return tot_i, tot_q
+        len_acq = len(self.di_buf[0]) // len(unique_adcs)
+        stacked = (
+            np.stack((self.di_buf, self.dq_buf))[:, :, :len_acq]
+            / np.array(lengths)[:, np.newaxis]
+        )
+        tot = []
+
+        for idx, count in enumerate(adc_count.astype(int)):
+            try:
+                # if we are doing sweepers
+                # (adc_channels, number_of_readouts, number_of_points, number_of_shots)
+                shape = (
+                    2,
+                    count,
+                    int(np.prod(self.sweep_axes)),
+                    self.reps,
+                )  # type: Union[Tuple[int, int, int], Tuple[int, int, int, int]]
+            except AttributeError:
+                # if we are not doing sweepers
+                # (adc_channels, number_of_readouts, number_of_shots)
+                shape = (2, count, self.reps)
+
+            tot.append(stacked[:, idx].reshape(shape).tolist())
+
+        return tuple(list(x) for x in zip(*tot))  # type: ignore
 
     def declare_gen_mux_ro(self):
         """Declare nqz zone for multiplexed readout."""
         adc_ch_added = []
 
         mux_freqs = []
         mux_gains = []
```

### Comparing `qibosoq-0.1.1/src/qibosoq/programs/flux.py` & `qibosoq-0.1.2/src/qibosoq/programs/flux.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Flux program used by qibosoq to execute sequences and sweeps."""
 
 import logging
 from typing import Dict, List, Tuple
 
 import numpy as np
 from qick import QickSoc
-from qick.qick_asm import QickRegister
+from qick.asm_v1 import QickRegister
 
 import qibosoq.configuration as qibosoq_cfg
 from qibosoq.components.base import Config, Qubit
 from qibosoq.components.pulses import (
     Arbitrary,
     Element,
     FluxExponential,
```

### Comparing `qibosoq-0.1.1/src/qibosoq/programs/sweepers.py` & `qibosoq-0.1.2/src/qibosoq/programs/sweepers.py`

 * *Files 5% similar despite different names*

```diff
@@ -35,14 +35,17 @@
         qubits: List[Qubit],
         *sweepers: Sweeper,
     ):
         """Init function, sets sweepers parameters before calling super.__init__."""
         self.sweepers = reversed_sweepers(sweepers)
         super().__init__(soc, qpcfg, sequence, qubits)
 
+        self.reps = qpcfg.reps  # must be done after NDAveragerProgram init
+        self.soft_avgs = qpcfg.soft_avgs
+
     def validate(self, sweeper: Sweeper):
         """Check if a sweeper is valid.
 
         In particular, it raises an error if:
             - sweeper is on bias, but not enough information has been given with the qubit
             - sweeper is on bias wih flux pulses in the sequence
             - sweeper is on flux pulses
```

### Comparing `qibosoq-0.1.1/src/qibosoq/server.py` & `qibosoq-0.1.2/src/qibosoq/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -88,19 +88,18 @@
     if num_instructions > max_mem:
         raise MemoryError(
             f"The tproc has a max memory size of {max_mem}, "
             f"but the program had {num_instructions} instructions"
         )
 
     if opcode is OperationCode.EXECUTE_PULSE_SEQUENCE_RAW:
-        results = program.acquire_decimated(
+        results = program.acquire_decimated(  # pylint: disable=E1120
             qick_soc,
             load_pulses=True,
             progress=False,
-            debug=False,
         )
         toti = [[results[0][0].tolist()]]
         totq = [[results[0][1].tolist()]]
     else:
         toti, totq = program.perform_experiment(
             qick_soc,
             average=data["cfg"]["average"],
```

### Comparing `qibosoq-0.1.1/PKG-INFO` & `qibosoq-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,82 +1,94 @@
-Metadata-Version: 2.1
-Name: qibosoq
-Version: 0.1.1
-Summary: QIBO Server On Qick (qibosoq) is the server component of qibolab to be run on RFSoC boards
-Home-page: https://github.com/qiboteam/qibosoq/
-License: Apache-2.0
-Author: Rodolfo Carobene
-Author-email: rodolfo.carobene@gmail.com
-Requires-Python: >=3.8,<3.12
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Dist: qick (>=0.2.165,<=0.2.181)
-Project-URL: Documentation, https://qibo.science/qibosoq/stable/
-Project-URL: Repository, https://github.com/qiboteam/qibosoq/
-Description-Content-Type: text/markdown
-
 # Qibosoq
 
-![Tests](https://github.com/qiboteam/qibosoq/workflows/Tests/badge.svg)
 [![codecov](https://codecov.io/gh/qiboteam/qibosoq/branch/main/graph/badge.svg?token=1EKZKVEVX0)](https://codecov.io/gh/qiboteam/qibosoq)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.8083285.svg)](https://doi.org/10.5281/zenodo.8083285)
+![PyPI - Version](https://img.shields.io/pypi/v/qibosoq)
+![PyPI - Python Version](https://img.shields.io/pypi/pyversions/qibosoq)
+
+Repository for developing server side of RFSoC fpga boards Qibosoq is a server
+for integrating [Qick](https://github.com/openquantumhardware/qick) in the
+[Qibolab](https://github.com/qiboteam/qibolab) ecosystem for executing arbitrary
+pulses sequences on QPUs.
 
-Repository for developing server side of RFSoC fpga boards
-Qibosoq is a server for integrating [Qick](https://github.com/openquantumhardware/qick) in the [Qibolab](https://github.com/qiboteam/qibolab) ecosystem
-for executing arbitrary pulses sequences on QPUs.
+## Documentation
 
-The complete documentation for can be found at:
+[![docs](https://github.com/qiboteam/qibosoq/actions/workflows/publish.yml/badge.svg)](https://qibo.science/qibosoq/stable/)
 
-* [qibo.science/qibosoq/stable](https://qibo.science/qibosoq/stable/)
-* [qibo.science/qibosoq/latest](https://qibo.science/qibosoq/latest/)
+The complete documentation can be found at:
 
+- [qibo.science/qibosoq/stable](https://qibo.science/qibosoq/stable/)
+- [qibo.science/qibosoq/latest](https://qibo.science/qibosoq/latest/)
 
 ## Installation
-Please refer to the [documentation](https://qibo.science/qibosoq/stable/getting-started/installation.html) for installation instructions.
 
-## Configuration parameters
+Please refer to the
+[documentation](https://qibo.science/qibosoq/stable/getting-started/installation.html)
+for installation instructions.
 
-In `configuration.py` some default qibosoq parameters are hardcoded. They can be changed using environment variables ([see documentation](https://qibo.science/qibosoq/stable/getting-started/usage.html)).
+## Configuration parameters
 
-* IP of the server
-* Port of the server
-* Paths of log files
-* Name of python loggers
-* Path of bitstream
-* Type of readout (multiplexed or not, depending on the loaded bitstream)
+In `configuration.py` some default qibosoq parameters are hardcoded. They can be
+changed using environment variables
+([see documentation](https://qibo.science/qibosoq/stable/getting-started/usage.html)).
+
+- IP of the server
+- Port of the server
+- Paths of log files
+- Name of python loggers
+- Path of bitstream
+- Type of readout (multiplexed or not, depending on the loaded bitstream)
 
 ## Run the server
 
 The simplest way of executing the server is:
+
 ```
 sudo -E python -m qibosoq
 ```
+
 and the server can be closed with `Ctrl-C`.\
-Note that with this command the script will close as soon as the terminal where it's running it's closed.
-To run the server in detached mode you can use:
+Note that with this command the script will close as soon as the terminal where
+it's running is closed. To run the server in detached mode you can use:
 
 ```
 nohup sudo -E python -m qibosoq &
 ```
+
 And the server can be closed with `sudo kill <PID>` (PID will be saved in log).
 
+## Supported QICK version
+
+QICK is an evolving project, and as such, Qibosoq frequently adapts to its
+changes to ensure ongoing support. The table below provides a brief overview of
+the supported QICK versions corresponding to specific Qibosoq releases.
+
+| Qibosoq version | Supported QICK version |
+| --------------- | ---------------------- |
+| 0.1.0           | 0.2.135                |
+| 0.1.1           | >=0.2.165, <=0.2.181   |
+| 0.1.2           | >=0.2.211, <=0.2.249   |
+
 ### TII boards
 
-With TII boards the server can also be executed using the alias `server-run-bkg`.
+With TII boards the server can also be executed using the alias
+`server-run-bkg`.
 
-Also, two additional command are added in `.bashrc`: `serverinfo` and `serverclose`.
-`serverinfo` will print the PID if the server is running, otherwise will print "No running server".
-`serverclose` will close the server, if it is running.
+Also, two additional command are added in `.bashrc`: `serverinfo` and
+`serverclose`. `serverinfo` will print the PID if the server is running,
+otherwise will print "No running server". `serverclose` will close the server,
+if it is running.
 
 All these commands require sudo privileges.
 
 ## Contributing
 
-Contributions, issues and feature requests are welcome!
-Feel free to check
+Contributions, issues and feature requests are welcome! Feel free to check
 <a href="https://github.com/qiboteam/qibosoq/issues"><img alt="GitHub issues" src="https://img.shields.io/github/issues-closed/qiboteam/qibosoq"/></a>
 
+## Citation policy
+
+[![arXiv](https://img.shields.io/badge/arXiv-2310.05851-b31b1b.svg)](https://arxiv.org/abs/2310.05851)
+[![DOI](https://zenodo.org/badge/567203263.svg)](https://zenodo.org/badge/latestdoi/567203263)
+
+If you use the package please refer to
+[the documentation](https://qibo.science/qibo/stable/appendix/citing-qibo.html#publications)
+for citation instructions
```

#### html2text {}

```diff
@@ -1,42 +1,42 @@
-Metadata-Version: 2.1 Name: qibosoq Version: 0.1.1 Summary: QIBO Server On Qick
-(qibosoq) is the server component of qibolab to be run on RFSoC boards Home-
-page: https://github.com/qiboteam/qibosoq/ License: Apache-2.0 Author: Rodolfo
-Carobene Author-email: rodolfo.carobene@gmail.com Requires-Python: >=3.8,<3.12
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Programming Language :: Python :: 3 Classifier: Programming Language :: Python
-:: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
-Programming Language :: Python :: 3.10 Classifier: Programming Language ::
-Python :: 3.11 Classifier: Topic :: Scientific/Engineering :: Physics Requires-
-Dist: qick (>=0.2.165,<=0.2.181) Project-URL: Documentation, https://
-qibo.science/qibosoq/stable/ Project-URL: Repository, https://github.com/
-qiboteam/qibosoq/ Description-Content-Type: text/markdown # Qibosoq ![Tests]
-(https://github.com/qiboteam/qibosoq/workflows/Tests/badge.svg) [![codecov]
-(https://codecov.io/gh/qiboteam/qibosoq/branch/main/graph/
-badge.svg?token=1EKZKVEVX0)](https://codecov.io/gh/qiboteam/qibosoq) [![DOI]
-(https://zenodo.org/badge/DOI/10.5281/zenodo.8083285.svg)](https://doi.org/
-10.5281/zenodo.8083285) Repository for developing server side of RFSoC fpga
-boards Qibosoq is a server for integrating [Qick](https://github.com/
-openquantumhardware/qick) in the [Qibolab](https://github.com/qiboteam/qibolab)
-ecosystem for executing arbitrary pulses sequences on QPUs. The complete
-documentation for can be found at: * [qibo.science/qibosoq/stable](https://
-qibo.science/qibosoq/stable/) * [qibo.science/qibosoq/latest](https://
+# Qibosoq [![codecov](https://codecov.io/gh/qiboteam/qibosoq/branch/main/graph/
+badge.svg?token=1EKZKVEVX0)](https://codecov.io/gh/qiboteam/qibosoq) ![PyPI -
+Version](https://img.shields.io/pypi/v/qibosoq) ![PyPI - Python Version](https:
+//img.shields.io/pypi/pyversions/qibosoq) Repository for developing server side
+of RFSoC fpga boards Qibosoq is a server for integrating [Qick](https://
+github.com/openquantumhardware/qick) in the [Qibolab](https://github.com/
+qiboteam/qibolab) ecosystem for executing arbitrary pulses sequences on QPUs.
+## Documentation [![docs](https://github.com/qiboteam/qibosoq/actions/
+workflows/publish.yml/badge.svg)](https://qibo.science/qibosoq/stable/) The
+complete documentation can be found at: - [qibo.science/qibosoq/stable](https:/
+/qibo.science/qibosoq/stable/) - [qibo.science/qibosoq/latest](https://
 qibo.science/qibosoq/latest/) ## Installation Please refer to the
 [documentation](https://qibo.science/qibosoq/stable/getting-started/
 installation.html) for installation instructions. ## Configuration parameters
 In `configuration.py` some default qibosoq parameters are hardcoded. They can
 be changed using environment variables ([see documentation](https://
-qibo.science/qibosoq/stable/getting-started/usage.html)). * IP of the server *
-Port of the server * Paths of log files * Name of python loggers * Path of
-bitstream * Type of readout (multiplexed or not, depending on the loaded
+qibo.science/qibosoq/stable/getting-started/usage.html)). - IP of the server -
+Port of the server - Paths of log files - Name of python loggers - Path of
+bitstream - Type of readout (multiplexed or not, depending on the loaded
 bitstream) ## Run the server The simplest way of executing the server is: ```
 sudo -E python -m qibosoq ``` and the server can be closed with `Ctrl-C`.\ Note
 that with this command the script will close as soon as the terminal where it's
-running it's closed. To run the server in detached mode you can use: ``` nohup
+running is closed. To run the server in detached mode you can use: ``` nohup
 sudo -E python -m qibosoq & ``` And the server can be closed with `sudo kill `
-(PID will be saved in log). ### TII boards With TII boards the server can also
-be executed using the alias `server-run-bkg`. Also, two additional command are
-added in `.bashrc`: `serverinfo` and `serverclose`. `serverinfo` will print the
-PID if the server is running, otherwise will print "No running server".
-`serverclose` will close the server, if it is running. All these commands
-require sudo privileges. ## Contributing Contributions, issues and feature
-requests are welcome! Feel free to check_[_G_i_t_H_u_b_ _i_s_s_u_e_s_]
+(PID will be saved in log). ## Supported QICK version QICK is an evolving
+project, and as such, Qibosoq frequently adapts to its changes to ensure
+ongoing support. The table below provides a brief overview of the supported
+QICK versions corresponding to specific Qibosoq releases. | Qibosoq version |
+Supported QICK version | | --------------- | ---------------------- | | 0.1.0 |
+0.2.135 | | 0.1.1 | >=0.2.165, <=0.2.181 | | 0.1.2 | >=0.2.211, <=0.2.249 | ###
+TII boards With TII boards the server can also be executed using the alias
+`server-run-bkg`. Also, two additional command are added in `.bashrc`:
+`serverinfo` and `serverclose`. `serverinfo` will print the PID if the server
+is running, otherwise will print "No running server". `serverclose` will close
+the server, if it is running. All these commands require sudo privileges. ##
+Contributing Contributions, issues and feature requests are welcome! Feel free
+to check _[_G_i_t_H_u_b_ _i_s_s_u_e_s_]## Citation policy [![arXiv](https://img.shields.io/
+badge/arXiv-2310.05851-b31b1b.svg)](https://arxiv.org/abs/2310.05851) [![DOI]
+(https://zenodo.org/badge/567203263.svg)](https://zenodo.org/badge/latestdoi/
+567203263) If you use the package please refer to [the documentation](https://
+qibo.science/qibo/stable/appendix/citing-qibo.html#publications) for citation
+instructions
```

