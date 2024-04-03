# Comparing `tmp/openwfs-0.1.0rc1.tar.gz` & `tmp/openwfs-0.1.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openwfs-0.1.0rc1.tar", max compression
+gzip compressed data, was "openwfs-0.1.0rc2.tar", max compression
```

## Comparing `openwfs-0.1.0rc1.tar` & `openwfs-0.1.0rc2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0        4 2024-01-31 10:37:53.916211 openwfs-0.1.0rc1/openwfs/__init__.py
--rw-r--r--   0        0        0      198 2024-02-16 22:59:47.323141 openwfs-0.1.0rc1/openwfs/algorithms/__init__.py
--rw-r--r--   0        0        0     3194 2024-02-16 21:56:07.217200 openwfs-0.1.0rc1/openwfs/algorithms/basic_fourier.py
--rw-r--r--   0        0        0     9821 2024-02-18 11:24:43.094904 openwfs-0.1.0rc1/openwfs/algorithms/fourier.py
--rw-r--r--   0        0        0     3102 2024-02-16 22:14:36.325829 openwfs-0.1.0rc1/openwfs/algorithms/ssa.py
--rw-r--r--   0        0        0    21070 2024-02-18 11:54:53.635887 openwfs-0.1.0rc1/openwfs/algorithms/troubleshoot.py
--rw-r--r--   0        0        0    16223 2024-02-17 19:10:30.718743 openwfs-0.1.0rc1/openwfs/algorithms/utilities.py
--rw-r--r--   0        0        0    28757 2024-02-18 11:36:28.536983 openwfs-0.1.0rc1/openwfs/core.py
--rw-r--r--   0        0        0      162 2024-01-09 19:51:52.086741 openwfs-0.1.0rc1/openwfs/devices/__init__.py
--rw-r--r--   0        0        0     9307 2024-02-16 22:09:25.354651 openwfs-0.1.0rc1/openwfs/devices/camera.py
--rw-r--r--   0        0        0    19554 2024-02-18 11:34:10.791139 openwfs-0.1.0rc1/openwfs/devices/galvo_scanner.py
--rw-r--r--   0        0        0     3268 2024-02-16 22:00:11.217864 openwfs-0.1.0rc1/openwfs/devices/nidaq_gain.py
--rw-r--r--   0        0        0      817 2024-01-26 09:45:18.032042 openwfs-0.1.0rc1/openwfs/plot_utilities.py
--rw-r--r--   0        0        0      126 2024-02-18 16:06:45.699051 openwfs-0.1.0rc1/openwfs/processors/__init__.py
--rw-r--r--   0        0        0    15046 2024-02-18 16:05:09.701727 openwfs-0.1.0rc1/openwfs/processors/processors.py
--rw-r--r--   0        0        0      306 2024-02-18 11:35:25.222704 openwfs-0.1.0rc1/openwfs/simulation/__init__.py
--rw-r--r--   0        0        0    13473 2024-02-18 15:45:26.842846 openwfs-0.1.0rc1/openwfs/simulation/microscope.py
--rw-r--r--   0        0        0    12218 2024-02-18 11:42:03.176084 openwfs-0.1.0rc1/openwfs/simulation/mockdevices.py
--rw-r--r--   0        0        0    12632 2024-02-18 15:46:39.472390 openwfs-0.1.0rc1/openwfs/simulation/slm.py
--rw-r--r--   0        0        0     2962 2024-02-17 22:17:21.836523 openwfs-0.1.0rc1/openwfs/simulation/transmission.py
--rw-r--r--   0        0        0      188 2024-02-16 08:12:17.837278 openwfs-0.1.0rc1/openwfs/slm/__init__.py
--rw-r--r--   0        0        0     1412 2024-02-18 11:51:08.144314 openwfs-0.1.0rc1/openwfs/slm/context.py
--rw-r--r--   0        0        0     8891 2024-02-16 22:28:02.569015 openwfs-0.1.0rc1/openwfs/slm/geometry.py
--rw-r--r--   0        0        0    10116 2024-02-18 11:14:00.093051 openwfs-0.1.0rc1/openwfs/slm/patch.py
--rw-r--r--   0        0        0     2362 2024-02-16 08:12:48.576547 openwfs-0.1.0rc1/openwfs/slm/shaders.py
--rw-r--r--   0        0        0    27646 2024-02-18 21:34:20.181293 openwfs-0.1.0rc1/openwfs/slm/slm.py
--rw-r--r--   0        0        0     4179 2024-02-18 11:14:52.556815 openwfs-0.1.0rc1/openwfs/slm/texture.py
--rw-r--r--   0        0        0      262 2024-02-18 21:34:20.189448 openwfs-0.1.0rc1/openwfs/utilities/__init__.py
--rw-r--r--   0        0        0     7955 2024-02-16 22:00:11.198213 openwfs-0.1.0rc1/openwfs/utilities/patterns.py
--rw-r--r--   0        0        0    16440 2024-02-18 11:51:08.416342 openwfs-0.1.0rc1/openwfs/utilities/utilities.py
--rw-r--r--   0        0        0     1310 2024-02-21 10:38:29.194528 openwfs-0.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0     1580 2024-02-16 22:00:11.207396 openwfs-0.1.0rc1/README.rst
--rw-r--r--   0        0        0     2688 1970-01-01 00:00:00.000000 openwfs-0.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0       87 2024-03-12 14:24:56.103053 openwfs-0.1.0rc2/openwfs/__init__.py
+-rw-r--r--   0        0        0      160 2024-03-28 18:24:55.473201 openwfs-0.1.0rc2/openwfs/algorithms/__init__.py
+-rw-r--r--   0        0        0     3194 2024-02-16 21:56:07.217200 openwfs-0.1.0rc2/openwfs/algorithms/basic_fourier.py
+-rw-r--r--   0        0        0    10398 2024-03-29 13:37:47.739530 openwfs-0.1.0rc2/openwfs/algorithms/fourier.py
+-rw-r--r--   0        0        0     2982 2024-03-20 11:29:22.200961 openwfs-0.1.0rc2/openwfs/algorithms/ssa.py
+-rw-r--r--   0        0        0    27677 2024-03-29 13:37:47.718135 openwfs-0.1.0rc2/openwfs/algorithms/troubleshoot.py
+-rw-r--r--   0        0        0    16232 2024-03-29 13:37:47.736012 openwfs-0.1.0rc2/openwfs/algorithms/utilities.py
+-rw-r--r--   0        0        0    27787 2024-03-29 13:37:47.726551 openwfs-0.1.0rc2/openwfs/core.py
+-rw-r--r--   0        0        0      201 2024-03-27 12:11:18.952643 openwfs-0.1.0rc2/openwfs/devices/__init__.py
+-rw-r--r--   0        0        0     9315 2024-03-29 13:44:11.371913 openwfs-0.1.0rc2/openwfs/devices/camera.py
+-rw-r--r--   0        0        0    20740 2024-03-29 13:37:47.713997 openwfs-0.1.0rc2/openwfs/devices/galvo_scanner.py
+-rw-r--r--   0        0        0     3268 2024-02-16 22:00:11.217864 openwfs-0.1.0rc2/openwfs/devices/nidaq_gain.py
+-rw-r--r--   0        0        0      188 2024-03-26 11:59:17.638273 openwfs-0.1.0rc2/openwfs/devices/slm/__init__.py
+-rw-r--r--   0        0        0     1414 2024-03-26 11:59:17.628399 openwfs-0.1.0rc2/openwfs/devices/slm/context.py
+-rw-r--r--   0        0        0     8895 2024-03-28 18:30:46.153146 openwfs-0.1.0rc2/openwfs/devices/slm/geometry.py
+-rw-r--r--   0        0        0    10119 2024-03-26 11:59:17.646306 openwfs-0.1.0rc2/openwfs/devices/slm/patch.py
+-rw-r--r--   0        0        0     2365 2024-03-29 13:37:47.732846 openwfs-0.1.0rc2/openwfs/devices/slm/shaders.py
+-rw-r--r--   0        0        0    26454 2024-03-29 13:37:47.752208 openwfs-0.1.0rc2/openwfs/devices/slm/slm.py
+-rw-r--r--   0        0        0     4181 2024-03-28 19:02:12.402442 openwfs-0.1.0rc2/openwfs/devices/slm/texture.py
+-rw-r--r--   0        0        0     1484 2024-04-03 13:57:13.188592 openwfs-0.1.0rc2/openwfs/plot_utilities.py
+-rw-r--r--   0        0        0      126 2024-02-18 16:06:45.699051 openwfs-0.1.0rc2/openwfs/processors/__init__.py
+-rw-r--r--   0        0        0    15916 2024-04-03 13:57:13.194595 openwfs-0.1.0rc2/openwfs/processors/processors.py
+-rw-r--r--   0        0        0      306 2024-02-18 11:35:25.222704 openwfs-0.1.0rc2/openwfs/simulation/__init__.py
+-rw-r--r--   0        0        0    13751 2024-04-03 12:19:23.778125 openwfs-0.1.0rc2/openwfs/simulation/microscope.py
+-rw-r--r--   0        0        0    12366 2024-04-03 14:51:16.437292 openwfs-0.1.0rc2/openwfs/simulation/mockdevices.py
+-rw-r--r--   0        0        0    12635 2024-03-28 18:31:29.071183 openwfs-0.1.0rc2/openwfs/simulation/slm.py
+-rw-r--r--   0        0        0     3275 2024-03-28 20:58:28.515712 openwfs-0.1.0rc2/openwfs/simulation/transmission.py
+-rw-r--r--   0        0        0      262 2024-02-18 21:34:20.189448 openwfs-0.1.0rc2/openwfs/utilities/__init__.py
+-rw-r--r--   0        0        0     7965 2024-03-29 13:37:47.742666 openwfs-0.1.0rc2/openwfs/utilities/patterns.py
+-rw-r--r--   0        0        0    17847 2024-04-03 12:07:54.087375 openwfs-0.1.0rc2/openwfs/utilities/utilities.py
+-rw-r--r--   0        0        0     1491 2024-04-03 14:53:50.361485 openwfs-0.1.0rc2/pyproject.toml
+-rw-r--r--   0        0        0    16223 2024-03-29 14:27:33.544890 openwfs-0.1.0rc2/README.md
+-rw-r--r--   0        0        0    17129 1970-01-01 00:00:00.000000 openwfs-0.1.0rc2/PKG-INFO
```

### Comparing `openwfs-0.1.0rc1/openwfs/algorithms/basic_fourier.py` & `openwfs-0.1.0rc2/openwfs/algorithms/basic_fourier.py`

 * *Files identical despite different names*

### Comparing `openwfs-0.1.0rc1/openwfs/algorithms/fourier.py` & `openwfs-0.1.0rc2/openwfs/algorithms/fourier.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,25 @@
 import numpy as np
-from ..core import Detector, PhaseSLM
+
 from .utilities import analyze_phase_stepping, WFSResult
+from ..core import Detector, PhaseSLM
 from ..utilities.patterns import tilt
 
 
 class FourierBase:
-    """Base class definition for the Fourier algorithms.
+    """Base class definition for the Fourier algorithms as described in [1].
 
-      Can run natively, provided you input the k-space for the reference and measurement part of the SLM.
+      This algorithm optimises the wavefront in a Fourier-basis. The modes that are tested are provided into a 'k-space'
+      of which each 'k-vector' represents a certain angled wavefront that will be tested. (more detailed explanation is
+      found in _get_phase_pattern).
+
+      As described in [1], these modes are measured by interfering a certain mode on one half of the SLM with a
+      'reference beam'. This is done by not modulating the other half of the SLM. In order to find a full corrective
+      wavefront therefore, the experiment has to be repeated twice for each side of the SLM. Finally, the two wavefronts
+      are combined.
 
       [1]: Bahareh Mastiani, Gerwin Osnabrugge, and Ivo M. Vellekoop,
       "Wavefront shaping for forward scattering," Opt. Express 30, 37436-37445 (2022)
       """
 
     def __init__(self, feedback: Detector, slm: PhaseSLM, slm_shape: tuple[int, int], k_left: np.ndarray,
                  k_right: np.ndarray, phase_steps: int = 4):
@@ -19,15 +27,15 @@
 
         Args:
             feedback (Detector): The feedback source, usually a detector that provides measurement data.
             slm (PhaseSLM): slm object.
                 The slm may have the `extent` property set to indicate the extent of the back pupil of the microscope
                 objective in slm coordinates. By default, a value of 2.0, 2.0 is used (indicating that the pupil
                 corresponds to a circle of radius 1.0 on the SLM). However, to prevent artefacts at the edges of the
-                SLM,it may be overfilled, such that the `phases` image is mapped to an extent of e.g. (2.2, 2.2), i.e.
+                SLM,it may be overfilled, such that the `phases` image is mapped to an extent of e. g. (2.2, 2.2), i. e.
                 10% larger than the back pupil.
             slm_shape (tuple[int, int]): The shape of the SLM patterns and transmission matrices.
             k_left (numpy.ndarray): 2-row matrix containing the y, and x components of the spatial frequencies
                 used as a basis for the left-hand side of the SLM.
                 The frequencies are defined such that a frequency of (1,0) or (0,1) corresponds to
                 a phase gradient of -π to π over the back pupil of the microscope objective, which results in
                 a displacement in the focal plane of exactly a distance corresponding to the Abbe diffraction limit.
```

### Comparing `openwfs-0.1.0rc1/openwfs/algorithms/ssa.py` & `openwfs-0.1.0rc2/openwfs/algorithms/ssa.py`

 * *Files 22% similar despite different names*

```diff
@@ -47,16 +47,15 @@
                 for p in range(self.phase_steps):
                     phase_pattern[y, x] = p * 2 * np.pi / self.phase_steps
                     self.slm.set_phases(phase_pattern)
                     self.feedback.trigger(out=measurements[y, x, p, ...])
                 phase_pattern[y, x] = 0
 
         self.feedback.wait()
-        starting_intensity = np.mean(measurements[:, :, 0])  # flat wavefront intensity
-        return analyze_phase_stepping(measurements, axis=2, A=np.sqrt(starting_intensity))
+        return analyze_phase_stepping(measurements, axis=2)
 
     @property
     def n_x(self) -> int:
         """The number of SLM elements in the x direction."""
         return self._n_x
 
     @n_x.setter
```

### Comparing `openwfs-0.1.0rc1/openwfs/algorithms/utilities.py` & `openwfs-0.1.0rc2/openwfs/algorithms/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 class WFSResult:
     """
     Data structure for holding wavefront shaping results and statistics.
 
     Attributes:
         t (ndarray): Measured transmission matrix. If multiple targets were used, the first dimension(s) of `t`
             denote the columns of the transmission matrix (`a` indices), and the last dimensions(s) denote the targets,
-            i.e., the rows of the transmission matrix (`b` indices).
+            i. e., the rows of the transmission matrix (`b` indices).
         axis (int): Number of dimensions used for denoting a single column of the transmission matrix
-            (e.g., 2 dimensions representing the x and y coordinates of the SLM pixels).
+            (e. g., 2 dimensions representing the x and y coordinates of the SLM pixels).
         fidelity_noise (ndarray): The estimated loss in fidelity caused by the limited SNR (for each target).
         fidelity_amplitude (ndarray): Estimated reduction of the fidelity due to phase-only modulation (for each target)
             (≈ π/4 for fully developed speckle).
         fidelity_calibration (ndarray): Estimated deviation from a sinusoid response.
         n (int): Total number of segments used in the optimization. When missing, this value is set to the number of
             elements in the first `axis` dimensions of `t`.
         estimated_optimized_intensity (ndarray): When missing, estimated intensity in the target(s) after displaying the
@@ -37,15 +37,15 @@
                  n: Optional[int] = None,
                  intensity_offset: Optional[ArrayLike] = 0.0):
         """
         Args:
             t(ndarray): measured transmission matrix.
             axis(int):
                 number of dimensions used for denoting a single columns of the transmission matrix
-                (e.g. 2 dimensions representing the x and y coordinates of the SLM pixels)
+                (e. g. 2 dimensions representing the x and y coordinates of the SLM pixels)
             fidelity_noise(ArrayLike):
                 the estimated loss in fidelity caused by the the limited snr (for each target).
             fidelity_amplitude(ArrayLike):
                 estimated reduction of the fidelity due to phase-only modulation (for each target)
                 (≈ π/4 for fully developed speckle)
             fidelity_calibration(ArrayLike):
                 estimated deviation from a sinusoid responds (TODO: experimental, untested)
```

### Comparing `openwfs-0.1.0rc1/openwfs/core.py` & `openwfs-0.1.0rc2/openwfs/core.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,72 +13,15 @@
 
 from .utilities import set_pixel_size
 
 
 class Device(ABC):
     """Base class for detectors and actuators
 
-    Multi-threading:
-        OpenWFS is not designed to be thread-safe, and the user
-        is responsible for guaranteeing that devices are only accessed
-        from a single thread at a time.
-
-        For detectors, OpenWFS does provide threading support by the means
-        of a worker thread that is automatically started when the `trigger` method
-        is called. The worker thread calls `_fetch` on the detector object,
-        which acquires and processes the data.
-
-        While a measurement is busy (between `trigger` and the end of the
-        corresponding `_fetch`), write access to the attributes of the detector
-        is blocked. This is to prevent the user from modifying the detector settings
-        while a measurement is in progress, which would give unpredictable results.
-
-    Synchronization:
-        Device implements the synchronization between detectors and actuators.
-        The idea is that a measurement can only be made when all actuators are stable,
-        and that an actuator can only be moved when all detectors are ready.
-
-        The synchronization mechanism is implemented using a global state variable `_moving`.
-        A detector can request a state switch to the `measuring` state (`_moving=False`),
-        and an actuator can request a state switch to the `moving` state (`_moving=True`)
-        by calling `_start`.
-
-        Before making the state switch, `_start` waits for all devices of the _other_ type
-        (actuators or detectors) to become ready by calling
-        `wait(up_to=latency, await_data=False)` on those devices.
-        Here, `latency` is the minimum latency of all devices of the _same_ type as the one
-        requesting the state switch.
-        If this minimum latency is positive, it means that the devices will not start their
-        measurement or movement immediately, so we can make the state switch slightly before
-        the devices of the other type are all ready.
-        For example, a spatial light modulator has a relatively long latency, meaning that
-        we can send the next frame even before a camera has finished reading the previous frame.
-
-        For detectors, `_start` is called automatically by `trigger()`, so there is never a need to call it.
-        Implementations of an actuator should call `_start` explicitly before starting to move the actuator.
-
-    Usage::
-        >>> f1 = np.zeros((N, P, *cam1.data_shape))
-        >>> f2 = np.zeros((N, P, *cam2.data_shape))
-        >>> for n in range(N):
-        >>>     for p in range(P)
-        >>>         phase = 2 * np.pi * p / P
-        >>>
-        >>>         # wait for all measurements to complete (up to the latency of the slm), and trigger the slm.
-        >>>         slm.set_phases(phase)
-        >>>
-        >>>         # wait for the image on the slm to stabilize, then trigger the measurement.
-        >>>         cam1.trigger(out = f1[n, p, ...])
-        >>>
-        >>>         # directly trigger cam2, since we already are in the 'measuring' state.
-        >>>         cam2.trigger(out = f2[n, p, ...])
-        >>>
-        >>> cam1.wait() # wait until camera 1 is done grabbing frames
-        >>> cam2.wait() # wait until camera 2 is done grabbing frames
-        >>> fields = (f2 - f1) * np.exp(-j * phase)
+        See :ref:`key_concepts` for more information.
 
     """
     __slots__ = ('_end_time_ns', '_timeout_margin', '_locking_thread', '_error',
                  '__weakref__', '_latency', '_duration', '_multi_threaded')
     _workers = ThreadPoolExecutor(thread_name_prefix='Device._workers')
     _moving = False
     _state_lock = threading.Lock()
@@ -103,15 +46,15 @@
     def _start(self):
         """Switches the state to 'moving' (for actuators) or 'measuring' (for detectors).
 
         This function changes the global state to 'moving' or 'measuring' if needed,
         and it may block until this state switch is completed.
 
         After switching, stores the time at which the operation will have ended in the `_end_time_ns`
-        field (i.e., `time.time_ns() + self.latency + self.duration`).
+        field (i. e., `time.time_ns() + self.latency + self.duration`).
         """
 
         # acquire a global lock, to prevent multiple threads to switch moving/measuring state simultaneously
         with Device._state_lock:
             # check if transition from moving/measuring or vice versa is needed
             if Device._moving != self._is_actuator():
                 if Device._moving:
@@ -127,15 +70,15 @@
                 # detectors actually starts a measurement.
                 # If this is a positive number, we can make the switch to 'measuring' slightly _before_
                 # all actuators have stabilized.
                 latency = min([device.latency for device in same_type], default=0.0 * u.ns)  # noqa - incorrect warning
 
                 # wait until all devices of the other type have (almost) finished
                 for device in other_type:
-                    device.wait(up_to=latency, await_data=False)
+                    device.wait(up_to=latency)
 
                 # changes the state from moving to measuring and vice versa
                 Device._moving = not Device._moving
                 if Device._moving:
                     logging.debug("state is now MOVING.")
                 else:
                     logging.debug("state is now MEASURING.")
@@ -176,54 +119,46 @@
 
         For a detector, this is the maximum amount of time that elapses between returning from `trigger()` and the
         end of the measurement.
         For an actuator, this is the maximum amount of time that elapses from returning from a command like `update(
         )` and the stabilization of the device.
 
         If the duration of an operation is not known in advance,
-        (e.g., when waiting for a hardware trigger), this function should return `np.inf * u.ms`.
+        (e. g., when waiting for a hardware trigger), this function should return `np.inf * u.ms`.
 
         Note: A device may update the duration dynamically.
         For example, a stage may compute the required time to
         move to the target position and update the duration accordingly.
 
         Note: If `latency` is a (lower) estimate, the duration should be high enough to guarantee that `latency +
         duration` is at least as large as the time between starting the operation and finishing it.
         """
         return self._duration
 
-    def wait(self, up_to: Quantity[u.ms] = 0 * u.ns, await_data=True) -> None:
-        """Waits until the device is (almost) in the `ready` state, i.e., has finished measuring or moving.
+    def wait(self, up_to: Optional[Quantity[u.ms]] = None) -> None:
+        """Waits until the device is (almost) in the `ready` state, i. e., has finished measuring or moving.
 
         This function is called by `_start` automatically to ensure proper synchronization between detectors and
         actuators, and it is called by `__del__` to ensure the device is not active when it is destroyed.
         The only time to call `wait` explicitly is when using pipelined measurements, see `Detector.trigger()`.
 
         For devices that report a duration (`duration ≠ ∞`), this function waits until
         `current_time - up_to >= self._end_time_ns`,
         where `_end_time_ns` was set by the last call to `_start`.
 
         For devices that report no duration `duration = ∞`, this function repeatedly calls `busy` until `busy`
-        returns `False`.
-        In this case, `up_to` is ignored.
+        returns `False`. In this case, `up_to` is ignored.
 
         Args:
             up_to(Quantity[u.ms]):
-                when non-zero, specifies that this function may return 'up_to' milliseconds
+                when specified, specifies that this function may return 'up_to' milliseconds
                 *before* the device is finished.
-            await_data(bool):
-                If True, after waiting until the device is no longer busy, briefly locks the device.
-                For detectors, this has the effect of waiting until all acquisitions and processing of
-                previously triggered frames are completed.
-                If an `out` parameter was specified in `trigger()`, this guarantees that the data is stored
-                in the `out` array.
-                For actuators, this flag has no effect other than briefly locking the device.
 
         Raises:
-            Any other exception raised by the device in another thread (e.g., during `_fetch`).
+            Any other exception raised by the device in another thread (e. g., during `_fetch`).
             TimeoutError: if the device has `duration = ∞`, and `busy` does not return `True` within
                 `self.timeout`
             RuntimeError: if `wait` is called from inside a setter or from inside `_fetch`.
                 This would cause a deadlock.
 
         """
         if self._error is not None:
@@ -236,15 +171,17 @@
             start = time.time_ns()
             timeout = self.timeout.to_value(u.ns)
             while self.busy():
                 time.sleep(0.01)
                 if time.time_ns() - start > timeout:
                     raise TimeoutError("Timeout in %s (tid %i)", self, threading.get_ident())
         else:
-            time_to_wait = self._end_time_ns - up_to.to_value(u.ns) - time.time_ns()
+            time_to_wait = self._end_time_ns - time.time_ns()
+            if up_to is not None:
+                time_to_wait -= up_to.to_value(u.ns)
             if time_to_wait > 0:
                 time.sleep(time_to_wait / 1.0E9)
 
     def busy(self) -> bool:
         """Returns true if the device is measuring or moving (see `wait()`).
 
         Note: if a device does not define a finite `duration`, it must override this function to poll for
@@ -280,14 +217,16 @@
     @final
     def _is_actuator(self):
         return True
 
 
 class Detector(Device, ABC):
     """Base class for all detectors, cameras and other data sources with possible dynamic behavior.
+
+    See :numref:`Detectors` in the documentation for more information.
     """
     __slots__ = ('_measurements_pending', '_lock_condition', '_pixel_size', '_data_shape')
 
     def __init__(self, *, data_shape: Optional[tuple[int, ...]], pixel_size: Optional[Quantity],
                  duration: Optional[Quantity[u.ms]], latency: Optional[Quantity[u.ms]], multi_threaded: bool = True):
         """
         Constructor for the Detector class.
@@ -295,15 +234,15 @@
         Args:
             data_shape:  The shape of the data array that `read()` will return. When None is passed,
                 the subclass should override the `data_shape` property to return the actual shape.
             pixel_size:  The pixel size (in astropy length units). None if the pixels do not have a size.
                 Subclassed can override the `pixel_size` property to return the actual pixel size.
             duration: The maximum amount of time that elapses between returning from `trigger()`
                 and the end of the measurement. If the duration of an operation is not known in advance,
-                (e.g., when waiting for a hardware trigger), this value should be `np.inf * u.ms`
+                (e. g., when waiting for a hardware trigger), this value should be `np.inf * u.ms`
                 and the `busy` method should be overridden to return `False` when the measurement is finished.
                 If None is passed, the subclass should override the `duration` property to return the actual duration.
             latency: The minimum amount of time between sending a command or trigger to the device
                 and the moment the device starts responding. If None is passed, the subclass should override
                 the `latency` property to return the actual latency.
             multi_threaded: If True, `_fetch` is called from a worker thread. Otherwise, `_fetch` is called
                 directly from `trigger`. If the device is not thread-safe, or threading provides no benefit,
@@ -327,37 +266,85 @@
 
     def _decrease_measurements_pending(self):
         with self._lock_condition:
             self._measurements_pending -= 1
             if self._measurements_pending == 0:
                 self._lock_condition.notify_all()
 
-    def wait(self, up_to: Quantity[u.ms] = 0 * u.ns, await_data=True) -> None:
-        super().wait(up_to, await_data)
-        if await_data:
+    def wait(self, up_to: Quantity[u.ms] = None) -> None:
+        """Waits until the hardware has (almost) finished measuring
+
+        Due to the automatic synchronization between detectors and actuators, this function only needs to be called
+        explicitly when waiting for data to be stored in the `out` argument of :meth:`~.Detector.trigger()`.
+
+        Args:
+            up_to: if specified, this function may return `up_to` milliseconds *before* the hardware has finished measurements.
+                If None, this function waits until the hardware has finished all measurements *and* all data is fetched,
+                and stored in the `out` array if that was passed to trigger().
+
+        """
+        super().wait(up_to)
+        if up_to is None:
             # wait until all pending measurements are processed.
             with self._lock_condition:
                 while self._measurements_pending > 0:
                     self._lock_condition.wait()
 
     def trigger(self, *args, out=None, immediate=False, **kwargs) -> Future:
         """Triggers the detector to start acquisition of the data.
 
-        This function returns a `concurrent.futures.Future`.
+        This function does not wait for the measurement to complete.
+        Instead, it returns a `concurrent.futures.Future`..
         Call `.result()` on the returned object to wait for the data.
+        Here is a typical usage pattern:
 
-        All parameters are passed to the _fetch function of the detector.
-        If any of these parameters is a Future, it is awaited before calling _fetch.
-        This way, data from multiple sources can be combined (see Processor).
+        .. code-block:: python
+
+            # Trigger the detector, which starts the data capture process
+            future = detector.trigger()
+
+            # Do some other work, perhaps trigger other detectors to capture
+            # data simultaneously...
 
+            # Now read the data from the detector. If the data is not ready yet,
+            # this will block until it is.
+            data = future.result()
+
+        An alternative method for asynchronous data capture is to use
+        the `out` parameter to specify a location where to store the data:
+
+        .. code-block:: python
+
+            out = np.zeros((2,), dtype='float32')
+            detector.trigger(out=out[0])  # start the first measurement
+            detector.trigger(out=out[1])  # queue the second measurement
+            detector.wait()  # wait for both measurements to complete
+            # Now the data is stored in the `out` array.
+
+        All input parameters are passed to the _fetch function of the detector.
         Child classes may override trigger() to call `super().trigger()` with additional parameters.
+        If any of these parameters is a Future, it is awaited before calling _fetch.
+        This way, data from multiple sources can be combined (see Processor).
 
         Note:
             To implement hardware triggering, do not override this function.
-            Instead, override `_do_trigger()` instead to ensure proper synchronization and locking.
+            Instead, override `_do_trigger()` to ensure proper synchronization and locking.
+
+        Args:
+            out: If specified, the data is stored in this array once it is available.
+            immediate: If True, the data is fetched in the current thread. This is useful for debugging,
+                and for cases where the data is needed immediately. It avoids the overhead (and debugging complications)
+                of dispatching the call to _fetch to a worker thread.
+            *args: Additional arguments passed to the _fetch function.
+                If any of these arguments is a `concurrent.futures.Future`, the data is awaited before calling _fetch,
+                and the data is passed instead of the `Future`.
+                This is useful for combining data from multiple sources (see `Processor`).
+            **kwargs: Additional keyword arguments passed to the _fetch function. Any `concurrent.futures.Future`
+                in the keyword arguments is awaited before calling _fetch,
+                and the data is passed instead of the `Future`.
         """
         self._increase_measurements_pending()
         try:
             self._start()
             self._do_trigger()
         except:  # noqa  - ok, we are not really catching the exception, just making sure the lock gets released
             self._decrease_measurements_pending()
@@ -461,44 +448,43 @@
 
     @property
     def pixel_size(self) -> Optional[Quantity]:
         """Physical dimension of one element in the returned data array.
 
         For cameras, this is the pixel size (in astropy length units).
         For detectors returning a time trace, this value is specified in astropy time units.
-
         The pixel_size is a 1-D array with an element for each dimension of the returned data.
 
         By default, the pixel size cannot be set.
         However, in some cases (such as when the `pixel_size` is actually a sampling interval),
         it makes sense for the child class to implement a setter.
         """
         return self._pixel_size
 
     @final
-    def coordinates(self, dim: int) -> Quantity:
+    def coordinates(self, dimension: int) -> Quantity:
         """Returns an array with the coordinate values along the d-th axis.
 
         The coordinates represent the _centers_ of the grid points. For example,
         for an array of shape `(2,)` the coordinates are `[0.5, 1.5] * pixel_size`
         and not `[0, 1] * pixel_size`. If `self.pixel_size is None`, a pixel size
         of 1.0 is used.
 
         The coordinates are returned as an array with the same number of
         dimensions as `data_shape`, with the d-th dimension holding the coordinates.
-        This facilitates meshgrid-like computations, e.g.
+        This facilitates meshgrid-like computations, e. g.
         `cam.coordinates(0) + cam.coordinates(1)` gives a 2-dimensional array of coordinates.
 
         Args:
-            dim: Dimension for which to return the coordinates.
+            dimension: Dimension for which to return the coordinates.
         """
-        unit = u.dimensionless_unscaled if self.pixel_size is None else self.pixel_size[dim]
+        unit = u.dimensionless_unscaled if self.pixel_size is None else self.pixel_size[dimension]
         shape = np.ones_like(self.data_shape)
-        shape[dim] = self.data_shape[dim]
-        return np.arange(0.5, 0.5 + self.data_shape[dim], 1.0).reshape(shape) * unit
+        shape[dimension] = self.data_shape[dimension]
+        return np.arange(0.5, 0.5 + self.data_shape[dimension], 1.0).reshape(shape) * unit
 
     @final
     @property
     def extent(self) -> Quantity:
         """Physical size of the data array
 
         If a `pixel_size` is set, this function returns `data_shape * pixel_size`
@@ -510,15 +496,15 @@
         return np.array(self.data_shape) * unit
 
 
 class Processor(Detector, ABC):
     """Base class for all Processors.
 
     Processors can be used to build data processing graphs, where each Processor takes input from one or
-    more input Detectors and processes that data (e.g., cropping an image, averaging over an ROI, etc.).
+    more input Detectors and processes that data (e. g., cropping an image, averaging over an ROI, etc.).
     A processor, itself, is a Detector to allow chaining multiple processors together to combine functionality.
 
     To implement a processor, implement `_fetch`, and optionally override `data_shape`, `pixel_size`, and `__init__`.
     The `latency` and `duration` properties are computed from the latency and duration of the inputs and cannot be set.
     By default, the `pixel_size` and `data_shape` are the same as the `pixel_size` and `data_shape` of the first input.
     To override this behavior, override the `pixel_size` and `data_shape` properties.
     """
@@ -543,15 +529,15 @@
         """Returns the shortest latency for all detectors."""
         return min((source.latency for source in self._sources if source is not None), default=0.0 * u.ms)
 
     @final
     @property
     def duration(self) -> Quantity[u.ms]:
         """Returns the last end time minus the first start time for all detectors
-        i.e., max (duration + latency) - min(latency).
+        i. e., max (duration + latency) - min(latency).
 
         Note that `latency` is allowed to vary over time for devices that can only be triggered periodically,
         so this `duration` may also vary over time.
         """
         times = [(source.duration, source.latency) for source in self._sources if source is not None]
         if len(times) == 0:
             return 0.0 * u.ms
```

### Comparing `openwfs-0.1.0rc1/openwfs/devices/camera.py` & `openwfs-0.1.0rc2/openwfs/devices/camera.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-from astropy.units import Quantity
 from typing import Optional
-from ..core import Detector
-from harvesters.core import Harvester
-import numpy as np
+
 import astropy.units as u
+import numpy as np
+from astropy.units import Quantity
+from harvesters.core import Harvester
+
+from ..core import Detector
 
 
 class Camera(Detector):
     """Adapter for GenICam/GenTL cameras.
 
     Attributes:
         _nodes: The GenICam node map of the camera.
@@ -15,16 +17,16 @@
             see the `GenICam/GenAPI documentation <https://www.emva.org/standards-technology/genicam/>`_
             and the `Standard Features Naming Convention
             <https://www.emva.org/wp-content/uploads/GenICam_SFNC_2_3.pdf>` for more details.
 
             The node map should not be used to set properties that are available as properties in the Camera object,
             such as `duration` (exposure time), `width`, `height`, `binning`, etc.
 
-            Also, the node map should not be used to set properties while the camera is fetching a frame (i.e.,
-            between `trigger()` and calling `result()` on the returned concurrent.futures.Future obect).
+            Also, the node map should not be used to set properties while the camera is fetching a frame (i. e.,
+            between `trigger()` and calling `result()` on the returned concurrent.futures.Future object).
 
     Note:
         This class is a thin wrapper around the Harvesters module,
         which is a generic adapter for GenICam/GenTL cameras.
 
     Example:
         >>> camera = Camera(serial_number='12345678')
```

### Comparing `openwfs-0.1.0rc1/openwfs/devices/galvo_scanner.py` & `openwfs-0.1.0rc2/openwfs/devices/galvo_scanner.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     These images are obtained by raster-scanning a focus using two galvo mirrors, controlled by a nidaq card,
     and recording a detector signal (typically from a photon multiplier tube (PMT)) with the same card.
 
     Upon construction, the maximum scan range (in volt) is set for both axes,
     and a scale parameter should be specified to convert these voltages to positions in the object plane.
     The number of pixels in the full scan range is specified with the `data_shape` parameter.
 
-    After construction, a sub-region of the scan range (i.e., a region of interest ROI) may be selected using
+    After construction, a sub-region of the scan range (i. e., a region of interest ROI) may be selected using
     the `top`, `left`, `height` and `width` properties.
     Note that changing the ROI does not change the pixel size.
     Only the number of pixels in the returned image changes, as with a regular camera.
 
     The `binning` property can be used to change the pixel size without changing the ROI.
     By decreasing the `binning` property, more points are measured for the same ROI,
     thereby increasing the resolution.
@@ -64,23 +64,24 @@
                  scale: Quantity[u.um / u.V],
                  sample_rate: Quantity[u.Hz],
                  delay: float = 0.0,
                  padding: float = 0.05,
                  binning: int = 1,
                  bidirectional: bool = True,
                  simulation: Optional[str] = None,
-                 multi_threaded: bool = True):
+                 multi_threaded: bool = True,
+                 preprocess: Optional[callable] = None):
         """
         Args:
             data_shape (tuple[int, int]): number of data points (height, width) in the full field of view.
                 Note that the ROI can be reduced later by setting width, height, top and left,
                 and the resolution can be changed by modifying the `binning` property.
             input: tuple[str, Quantity[u.V], Quantity[u.V]],
                  Description of the NI-DAQ channel to use for the input.
-                 Tuple of: (name of the channel (e.g., 'ai/1'), minimum voltage, maximum voltage).
+                 Tuple of: (name of the channel (e. g., 'ai/1'), minimum voltage, maximum voltage).
             axis0: tuple[str, Quantity[u.V], Quantity[u.V], TerminalConfiguration],
                  Description of the NI-DAQ channel to use for controlling the axis 0 galvo (slow axis).
                  The TerminalConfiguration element is optional and defaults to TerminalConfiguration.DEFAULT.
             axis1: tuple[str, Quantity[u.V], Quantity[u.V], TerminalConfiguration],
                  Description of the NI-DAQ channel to use for controlling the axis 1 galvo (fast axis).
                  The TerminalConfiguration element is optional and defaults to TerminalConfiguration.DEFAULT.
             scale (u.um / u.V):
@@ -92,14 +93,17 @@
                 Sample rate of the NI-DAQ input channel.
                 The sample rate affects the total time needed to scan a single frame.
                 Setting the ROI, padding, or binning does not affect the sample rate.
             delay (float): Delay between mirror control and data acquisition, measured in pixels
             padding (float): Padding fraction at the sides of the scan. The scanner will scan a larger area than will be
                 reconstructed, to make sure the reconstructed image is within the linear scan range of the mirrors.
             bidirectional (bool): If true, enables bidirectional scanning along the fast axis.
+            preprocess (callable): Process the raw data with this function before cropping. When None, the preprocessing
+                will be skipped. The function must take input arguments data and sample_rate, and must return the
+                preprocessed data.
         """
         # settings for input/output channels
         self._in_channel = input[0]
         self._in_v_min = input[1].to(u.V)
         self._in_v_max = input[2].to(u.V)
         self._in_terminal_configuration = input[3] if len(input) > 3 else TerminalConfiguration.DEFAULT
         self._axis0_channel = axis0[0]
@@ -131,14 +135,16 @@
 
         self._valid = False  # indicates that `trigger()` should initialize the NI-DAQ tasks and scan pattern
         self._scan_pattern = None
         self._simulation = simulation
 
         self._original_pixel_size = ((self._out_v_max - self._out_v_min) * self._scale / data_shape).to(u.um)
 
+        self._preprocess = preprocess
+
         # the pixel size and duration are computed dynamically
         # data_shape just returns self._data shape, and latency = 0.0 ms
         super().__init__(data_shape=data_shape, pixel_size=None, duration=None, latency=0.0 * u.ms,
                          multi_threaded=multi_threaded)
         self._update()
 
     def _update(self):
@@ -225,15 +231,15 @@
         self._writer.write_many_sample(self._scan_pattern)
 
         # Start the tasks
         self._read_task.start()  # waits for trigger coming from the write task
         self._write_task.start()
 
     def _raw_to_cropped(self, raw: np.ndarray) -> np.ndarray:
-        """Converts the raw scanner data back into a 2-Dimensional image.
+        """Converts the raw scanner data back into a 2-dimensional image.
 
         Because the scanner can return both signed and unsigned integers, both cases are accounted for.
         This function crops the data if padding was added, and it
         flips the even rows back if scanned in bidirectional mode.
         """
         start = (self._padded_data_shape - self._data_shape) // 2
         end = self._padded_data_shape - start
@@ -262,15 +268,33 @@
             raw = (self._scan_pattern[1, :] * 1000.0).round().astype('int16')  # in mV
         elif self._simulation == 'vertical':
             raw = (self._scan_pattern[0, :] * 1000.0).round().astype('int16')
         else:
             raise ValueError(
                 f"Invalid simulation option {self._simulation}. Should be 'horizontal', 'vertical', or 'None'")
 
-        return self._raw_to_cropped(raw)
+        # Preprocess raw data if a preprocess function is set
+        if self._preprocess is None:
+            preprocessed_raw = raw
+        elif callable(self._preprocess):
+            preprocessed_raw = self._preprocess(data=raw, sample_rate=self._sample_rate)
+        else:
+            raise TypeError(f"Invalid type for {self._preprocess}. Should be callable or None.")
+        return self._raw_to_cropped(preprocessed_raw)
+
+    @property
+    def preprocess(self):
+        """The function to preprocess raw data before cropping."""
+        return self._preprocess
+
+    @preprocess.setter
+    def preprocess(self, value: Optional[callable]):
+        if not callable(value) and not (value is None):
+            raise TypeError(f"Invalid type for {self._preprocess}. Should be callable or None.")
+        self._preprocess = value
 
     @property
     def pixel_size(self) -> Quantity:
         """The size of a pixel in the object plane."""
         return self._original_pixel_size * self._binning / self._zoom
 
     @property
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openwfs-0.1.0rc1/openwfs/devices/nidaq_gain.py` & `openwfs-0.1.0rc2/openwfs/devices/nidaq_gain.py`

 * *Files identical despite different names*

### Comparing `openwfs-0.1.0rc1/openwfs/processors/processors.py` & `openwfs-0.1.0rc2/openwfs/processors/processors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from typing import Sequence, Optional, Union
+from typing import Sequence, Optional
 
 import cv2
 import numpy as np
 from astropy.units import Quantity
 
 from ..core import Processor, Detector
-from ..utilities import project
+from ..utilities import project, Transform
 from ..utilities.patterns import disk, gaussian
 
 
 class Roi:
     """
     Represents a Region of Interest (ROI) to compute a (weighted) average over.
 
@@ -334,47 +334,57 @@
             cv2.destroyWindow(title)
             return None
 
 
 class TransformProcessor(Processor):
     """
     Performs a 2-D transform of the input data (including shifting, padding, cropping, resampling).
+
+    By default, the output shape and pixel_size are the same as the input shape.
+    If desired, explicit values can be provided for the output shape and pixel_size. The unit of the pixel_size
+    should match the unit of the input data after applying the transform.
     """
 
-    def __init__(self, source, transform, data_shape: Optional[Sequence[int]] = None,
-                 pixel_size: Union[Optional[Quantity], bool] = False, multi_threaded: bool = True):
+    def __init__(self, source: Detector,
+                 transform: Transform = None,
+                 data_shape: Optional[Sequence[int]] = None,
+                 pixel_size: Optional[Quantity] = None,
+                 multi_threaded: bool = True):
         """
 
         Args:
-            transform: Transform object that describes the transformation from the source
-            data_shape: defaults to source.data_shape
-            pixel_size: defaults to source.pixel_size.
-                Specify any pixel size (including `None`) to override the pixel size of the source.
-        """
+            transform: Transform object that describes the transformation from the source to the target image
+            data_shape: Shape of the output. If omitted, the shape of the input data is used.
+            multi_threaded: Whether to perform processing in a worker thread.
+            """
         if (data_shape is not None and len(data_shape) != 2) or len(source.data_shape) != 2:
             raise ValueError("TransformProcessor only supports 2-D data")
+        if transform is None:
+            transform = Transform()
 
+        # check if input and output pixel sizes are compatible
+        dst_unit = transform.destination_unit(source.pixel_size.unit)
+        if pixel_size is not None and not pixel_size.unit.is_equivalent(dst_unit):
+            raise ValueError("Pixel size unit does not match the unit of the transformed data")
+        if pixel_size is None and not source.pixel_size.unit.is_equivalent(dst_unit):
+            raise ValueError("The transform changes the unit of the coordinates."
+                             " An output pixel_size must be provided.")
+
+        self.transform = transform
+        super().__init__(source, multi_threaded=multi_threaded)
         self._pixel_size = pixel_size
         self._data_shape = data_shape
-        super().__init__(source, multi_threaded=multi_threaded)
-        self.transform = transform
 
     @property
     def data_shape(self):
-        if self._data_shape is not None:
-            return self._data_shape
-        else:
-            return super().data_shape
+        return self._data_shape if self._data_shape is not None else super().data_shape
 
     @property
     def pixel_size(self) -> Optional[Quantity]:
-        if self._pixel_size is not False:
-            return self._pixel_size
-        else:
-            return super().pixel_size
+        return self._pixel_size if self._pixel_size is not None else super().pixel_size
 
     def _fetch(self, source: np.ndarray) -> np.ndarray:  # noqa
         """
         Args:
             source (Detector): A Detector object as described in openwfs.core.Detector
 
         Returns: ndarray that has been transformed
```

### Comparing `openwfs-0.1.0rc1/openwfs/simulation/microscope.py` & `openwfs-0.1.0rc2/openwfs/simulation/microscope.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from numpy.typing import ArrayLike
 from scipy.signal import fftconvolve
 
 from ..core import Processor, Detector
 from ..plot_utilities import imshow  # noqa - for debugging
 from ..processors import TransformProcessor
 from ..simulation.mockdevices import XYStage, Camera, StaticSource
-from ..utilities import project, place, Transform, get_pixel_size, patterns
+from ..utilities import project, place, Transform, get_pixel_size, patterns, CoordinateType
 
 
 class Microscope(Processor):
     """A simulated microscope with pupil-conjugate SLM.
 
     The microscope simulates physical effects such as aberrations and noise, as well as devices typically found in a
     wavefront shaping microscope: a spatial light modulator, translation stages, and a camera.
@@ -38,16 +38,16 @@
                  incident_field: Union[Detector, ArrayLike, None] = None,
                  incident_transform: Optional[Transform] = None,
                  aberrations: Union[Detector, np.ndarray, None] = None,
                  aberration_transform: Optional[Transform] = None,
                  multi_threaded: bool = True):
         """
         Args:
-            source: 2-d image (must have `pixel_size` metadata), or
-                a detector that produces 2-d images of the original 'specimen'
+            source: 2-D image (must have `pixel_size` metadata), or
+                a detector that produces 2-D images of the original 'specimen'
             data_shape: shape (size in pixels) of the output.
                 Default value: source.data_shape
             numerical_aperture: Numerical aperture of the microscope objective
             wavelength: Wavelength of the light used for imaging,
                 the wavelength and numerical_aperture together determine the resolution of the microscope.
             magnification: Scalar magnification factor between input and output image.
                 Note that this factor does not affect the effective image resolution.
@@ -55,33 +55,33 @@
                 The default settings for data_shape, pixel_size and magnification cause the simulated microscope
                 to only convolve the source image with the point-spread function (PSF) without applying any scaling.
             xy_stage (XYStage): Optional stage object that can be used to move the sample laterally.
                 Defaults to a MockXYStage.
             z_stage (Stage): Optional stage object that moves the sample up and down to focus the microscope.
                 Higher values are further away from the microscope objective.
                 Defaults to a MockStage.
-            incident_field: Produces 2-d complex images containing the field output of the SLM.
+            incident_field: Produces 2-D complex images containing the field output of the SLM.
                 If no `slm_transform` is specified, the `pixel_size` attribute should
                  correspond to normalized pupil coordinates
-                (e.g. with a disk of radius 1.0, i.e. an extent of 2.0, corresponding to an NA of 1.0)
+                (e. g. with a disk of radius 1.0, i. e. an extent of 2.0, corresponding to an NA of 1.0)
             incident_transform (Optional[Transform]):
                 Optional Transform that transforms the phase pattern from the slm object
                 (in slm.pixel_size units) to normalized pupil coordinates.
                 Typically, the slm image is already in normalized pupil coordinates,
                 but this transform can be used to mimic SLM misalignment.
             aberrations: 2-D image containing the phase (in radians) of aberrations observed
                 in the back pupil of the microscope objective, or a Detector object that automatically produces such
                 images. The `extent` attribute corresponds to normalized pupil coordinates. For example, with a
                 numerical aperture of 0.6, the extent of the image should be 1.2. If a 2-D image without pixel_size
                 metadata is provided, the extent is automatically set to 2.0 * numerical_aperture.
             aberration_transform (Optional[Transform]):
                 Optional Transform that transforms the phase pattern from the aberration object
                 (in slm.pixel_size units) to normalized pupil coordinates.
                 Typically, the slm image is already in normalized pupil coordinates,
-                but this transform may e.g., be used to scale an aberration pattern
+                but this transform may e. g., be used to scale an aberration pattern
                 from extent 2.0 to 2.0 * NA.
 
         Note:
             The aberration map and slm phase map are cropped/padded to the NA of the microscope objective, and
             scaled to have the same pixel resolution so that they can be added.
         """
         if not isinstance(source, Detector):
@@ -221,15 +221,18 @@
         return self._sources[0].pixel_size * self.magnification
 
     @property
     def data_shape(self):
         """Returns the shape of the image in the image plane"""
         return self._data_shape
 
-    def get_camera(self, *, transform: Optional[Transform] = None, **kwargs) -> Detector:
+    def get_camera(self, *, transform: Optional[Transform] = None,
+                   data_shape: Optional[tuple[int, int]] = None,
+                   pixel_size: Optional[CoordinateType] = None,
+                   **kwargs) -> Detector:
         """
         Returns a simulated camera that observes the microscope image.
 
         The camera is a MockCamera object that simulates an AD-converter with optional noise.
         shot noise and readout noise (see MockCamera for options).
         In addition to the inputs accepted by the MockCamera constructor (data_shape, analog_max, shot_noise, etc.),
         it is also possible to specify a transform, to mimic the (mis)alignment of the camera.
@@ -237,13 +240,13 @@
         Args:
             transform ():
             **kwargs ():
 
         Returns:
 
         """
-        if transform is None:
+        if transform is None and data_shape is None and pixel_size is None:
             src = self
         else:
-            src = TransformProcessor(self, transform)
+            src = TransformProcessor(self, data_shape=data_shape, pixel_size=pixel_size, transform=transform)
 
         return Camera(src, **kwargs)
```

### Comparing `openwfs-0.1.0rc1/openwfs/simulation/mockdevices.py` & `openwfs-0.1.0rc2/openwfs/simulation/mockdevices.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,18 +69,19 @@
         self._data = value
         self._pixel_size = get_pixel_size(value)
         self._data_shape = value.shape
 
 
 class NoiseSource(Detector):
     def __init__(self, noise_type: str, *, data_shape: tuple[int, ...], pixel_size: Quantity, multi_threaded=True,
+                 generator=None,
                  **kwargs):
         self._noise_type = noise_type
         self._noise_arguments = kwargs
-        self._rng = np.random.default_rng()
+        self._rng = generator if generator is not None else np.random.default_rng()
         super().__init__(data_shape=data_shape, pixel_size=pixel_size, latency=0 * u.ms, duration=0 * u.ms,
                          multi_threaded=multi_threaded)
 
     def _fetch(self) -> np.ndarray:  # noqa
         if self._noise_type == 'uniform':
             return self._rng.uniform(**self._noise_arguments, size=self.data_shape)
         elif self._noise_type == 'gaussian':
@@ -96,15 +97,16 @@
 class ADCProcessor(Processor):
     """Mimics an analog-digital converter.
 
     At the moment, only positive input and output values are supported.
     """
 
     def __init__(self, source: Detector, analog_max: float = 0.0, digital_max: int = 0xFFFF,
-                 shot_noise: bool = False, gaussian_noise_std: float = 0.0, multi_threaded: bool = True):
+                 shot_noise: bool = False, gaussian_noise_std: float = 0.0, multi_threaded: bool = True,
+                 generator=None):
         """
         Initializes the ADCProcessor class, which mimics an analog-digital converter.
 
         Args:
             source (Detector): The source detector providing analog data.
             analog_max (float): The maximum analog value that can be handled by the ADC.
                 If set to 0.0, each measurement will be automatically scaled so that the maximum
@@ -122,15 +124,15 @@
                 If >0, add gaussian noise with std of this value to the data.
         """
         super().__init__(source, multi_threaded=multi_threaded)
         self._analog_max = None
         self._digital_max = None
         self._shot_noise = None
         self._gaussian_noise_std = None
-        self._rng = np.random.default_rng()
+        self._rng = generator if generator is not None else np.random.default_rng()
         self.gaussian_noise_std = gaussian_noise_std
         self.shot_noise = shot_noise
         self.analog_max = analog_max  # check value
         self.digital_max = digital_max  # check value
 
     def _fetch(self, data) -> np.ndarray:  # noqa
         """Clips the data to the range of the ADC, and digitizes the values."""
@@ -195,15 +197,15 @@
 
     @gaussian_noise_std.setter
     def gaussian_noise_std(self, value: int):
         self._gaussian_noise_std = value
 
 
 class Camera(ADCProcessor):
-    """Wraps any 2-d image source as a camera.
+    """Wraps any 2-D image source as a camera.
 
     To implement the camera interface, in addition to the Detector interface,
     we must implement left,right,top, and bottom.
     In addition, the data should be returned as uint16.
     Conversion to uint16 is implemented in the ADCProcessor base class.
     """
```

### Comparing `openwfs-0.1.0rc1/openwfs/simulation/slm.py` & `openwfs-0.1.0rc2/openwfs/simulation/slm.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     def __init__(self, slm_phases: Detector, field_amplitude: ArrayLike = 1.0,
                  non_modulated_field_fraction: float = 0.0):
         """
         Args:
             slm_phases: The `Detector` that returns the phases of the slm pixels.
             field_amplitude: Field amplitude of the modulated pixels.
-            non_modulated_field_fraction: Non-modulated field (e.g. a front reflection).
+            non_modulated_field_fraction: Non-modulated field (e. g. a front reflection).
         """
         super().__init__(slm_phases, multi_threaded=False)
         self.modulated_field_amplitude = field_amplitude
         self.non_modulated_field = non_modulated_field_fraction
 
     def _fetch(self, slm_phases: np.ndarray) -> np.ndarray:  # noqa
         """
```

### Comparing `openwfs-0.1.0rc1/openwfs/simulation/transmission.py` & `openwfs-0.1.0rc2/openwfs/simulation/transmission.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+from typing import Optional
+
 import numpy as np
+
 from .slm import SLM, Processor
 
 
 class SimulatedWFS(Processor):
     """A simple simulation of a wavefront shaping experiment.
 
     Simulates a configuration where both the SLM and the aberrations are placed in the back pupil
@@ -10,37 +13,40 @@
 
     The simulation computes (Σ A·exp(i·(aberrations-slm)))², which is the 0,0 component of the Fourier transform
     of the field in the pupil plane (including aberrations and the correction by the SLM).
 
     For a more advanced (but slower) simulation, use `Microscope`
     """
 
-    def __init__(self, aberrations: np.ndarray, slm=None, multi_threaded=True):
+    def __init__(self, *, t: Optional[np.ndarray] = None, aberrations: Optional[np.ndarray] = None, slm=None,
+                 multi_threaded=True):
         """
         Initializes the optical system with specified aberrations and optionally a Gaussian beam profile.
 
         This constructor sets up an optical system by specifying the aberrations across the SLM (Spatial Light
         Modulator) and, optionally, by defining a Gaussian beam profile. The aberrations array defines phase shifts at
         each point of the SLM. If a beam profile waist is provided, the input electric field is shaped into a
         Gaussian beam.
 
         Args:
-            aberrations (np.ndarray): An array containing the aberrations in radians.
+            t: Transmission matrix.
+            aberrations: An array containing the aberrations in radians. Can be used instead of a transmission matrix,
+                equivalent to specifying t = np.exp(1j * aberrations) / (aberrations.shape[0] * aberrations.shape[1]).
             slm:
             multi_threaded (bool, optional): If True, the simulation will use multiple threads to compute the
                 intensity in the focus. If False, the simulation will use a single thread. Defaults to True.
 
         The constructor creates a MockSLM instance based on the shape of the aberrations, calculates the electric
         field at the SLM considering the aberrations and optionally the Gaussian beam profile, and initializes the
         system with these parameters.
         """
-        self.slm = slm if slm is not None else SLM(aberrations.shape[0:2])
 
         # transmission matrix (normalized so that the maximum transmission is 1)
-        self._t = np.exp(1.0j * aberrations) / (aberrations.shape[0] * aberrations.shape[1])
+        self._t = t if t is not None else np.exp(1.0j * aberrations) / (aberrations.shape[0] * aberrations.shape[1])
+        self.slm = slm if slm is not None else SLM(self._t.shape[0:2])
 
         super().__init__(self.slm.field, multi_threaded=multi_threaded)
 
     def _fetch(self, incident_field):  # noqa
         """
         Computes the intensity in the focus by applying phase corrections to the input electric field.
```

### Comparing `openwfs-0.1.0rc1/openwfs/slm/context.py` & `openwfs-0.1.0rc2/openwfs/devices/slm/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import threading
 import weakref
+
 import glfw
 
 SLM = 'slm.SLM'
 
 
 class Context:
     """Holds a weak reference to an SLM window
```

### Comparing `openwfs-0.1.0rc1/openwfs/slm/geometry.py` & `openwfs-0.1.0rc2/openwfs/devices/slm/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Sequence
 
 import numpy as np
 from numpy.typing import ArrayLike
 
-from ..utilities import ExtentType, CoordinateType, unitless
+from ...utilities import ExtentType, CoordinateType, unitless
 
 
 class Geometry:
     """Class that represents the shape of a Patch object that can be drawn on the screen.
 
     The geometry is defined by a set of vertices
     and a set of indices that define the order in which the vertices are drawn.
@@ -19,15 +19,15 @@
 
     The vertices and indices define a triangle strip (see OpenGL specification) that is drawn on the screen.
     A triangle strip is a sequence of connected triangles, where each triangle shares two vertices with the previous
     triangle. The indices are used to determine the order in which the vertices are connected to form the triangles.
     To start a new triangle strip, insert the special index 0xFFFF into the index array.
 
     (tx, ty) are the texture coordinates that determine which pixel of the texture
-    (e.g. the array passed to `set_phases`) is drawn at each vertex.
+    (e. g. the array passed to `set_phases`) is drawn at each vertex.
     For each triangle, the screen coordinates (x,y) define a triangle on the screen, whereas the texture coordinates
     (tx, ty) define a triangle in the texture.
     OpenGL maps the texture triangle onto the screen triangle, using linear interpolation of the coordinates between
     the vertex points.
 
     The vertex data is uploaded to the GPU when the Geometry object is assigned to the `geometry` property of a Patch.
     """
```

### Comparing `openwfs-0.1.0rc1/openwfs/slm/patch.py` & `openwfs-0.1.0rc2/openwfs/devices/slm/patch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
+import warnings
+from typing import Sequence
+
 import numpy as np
 from numpy.typing import ArrayLike
-from typing import Sequence
-import warnings
 
 from .context import Context
 
 try:
     import OpenGL.GL as GL
     from OpenGL.GL import glGenBuffers, glBindBuffer, glBufferData, glDeleteBuffers, glEnable, glBlendFunc, \
         glBlendEquation, glDisable, glUseProgram, glBindVertexBuffer, glDrawElements, glGenFramebuffers, \
@@ -16,15 +17,15 @@
     from OpenGL.GL import shaders
 except AttributeError:
     warnings.warn("OpenGL not found, SLM will not work")
 from .geometry import rectangle, Geometry
 from .shaders import default_vertex_shader, default_fragment_shader, \
     post_process_fragment_shader, post_process_vertex_shader
 from .texture import Texture
-from ..core import PhaseSLM
+from ...core import PhaseSLM
 
 
 class Patch(PhaseSLM):
     _PHASES_TEXTURE = 0  # indices of the phases texture in the _texture array
 
     def __init__(self, slm, geometry=None, vertex_shader=default_vertex_shader,
                  fragment_shader=default_fragment_shader):
```

### Comparing `openwfs-0.1.0rc1/openwfs/slm/shaders.py` & `openwfs-0.1.0rc2/openwfs/devices/slm/shaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 # This shader is used to apply a software lookup table to phase image.
 # The phase in radians is converted to a coordinate in the lookup table
 # using the equation: texCoord = phase / (2 * pi) + 0.5 / 256
 # where the offset is used for proper rounding, so that with the standard lookup table
 # the range -δ to δ maps to a gray value 0 instead of
 # negative values mapping to 255 and positive values mapping to 0.
 # Since the lookup table texture is configured to use GL_WRAP,
-# only the fractional part of texCoord is used (i.e., texCoord - floor(texCoord)).
+# only the fractional part of texCoord is used (i. e., texCoord - floor(texCoord)).
 #
 post_process_fragment_shader = """
         #version 440 core
         in vec2 texCoord;
         out vec4 colorOut;
         layout(binding = 0) uniform sampler2D texSampler;
         layout(binding = 1) uniform sampler1D LUT;
```

### Comparing `openwfs-0.1.0rc1/openwfs/slm/slm.py` & `openwfs-0.1.0rc2/openwfs/devices/slm/slm.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,57 +5,35 @@
 import astropy.units as u
 import glfw
 import numpy as np
 from astropy.units import Quantity
 from numpy.typing import ArrayLike
 
 from .context import Context
-from ..simulation import PhaseToField
+from ...simulation import PhaseToField
 
 try:
     import OpenGL.GL as GL
     from OpenGL.GL import glViewport, glClearColor, glClear, glGenBuffers, glReadBuffer, glReadPixels, glFinish, \
         glBindBuffer, glBufferData, glBindBufferBase, glBindFramebuffer
 except AttributeError:
     warnings.warn("OpenGL not found, SLM will not work")
 from .patch import FrameBufferPatch, Patch, VertexArray
-from ..core import PhaseSLM, Actuator, Device, Detector
-from ..utilities import Transform
+from ...core import PhaseSLM, Actuator, Device, Detector
+from ...utilities import Transform
 
 TimeType = Union[Quantity[u.ms], int]
 
 
 class SLM(Actuator, PhaseSLM):
     """
     An OpenGL object to control a spatial light modulator connected to a graphics card.
 
-    The SLM can be created in windowed mode (useful for debugging), or full screen.
-    It is possible to have multiple windowed SLMs on the same monitor, but only one full-screen SLM per monitor.
+    See :numref:`section-slms` for more information.
 
-    An SLM holds a list of patches, which are shapes that can be drawn on the SLM.
-    Each of these patches can have a different texture, which is a 2D array of values that are drawn on the SLM.
-    In addition, each patch can have its own geometry, which determines how the texture is mapped onto the SLM window.
-    For more information, see the documentation of the Patch class.
-
-    If an SLM holds multiple patches, the patches are drawn in the order they are present in the `patches` list.
-    If patches overlap, the pixels of the previous patch are either overwritten (when the `additive_blend` property
-    of the patch is False), or added to the phase values of the previous patch (when `additive_blend` is True).
-
-    This way, a large range of use cases is enabled, including:
-
-    - Drawing a single square patch with a single texture (the default).
-    - Mapping the phase values to a disk, with an effective resolution depending on the distance to the center
-      of the disk (see `geometry.disk`).
-    - Applying an additive patch (an offset layer) that corrects for system aberrations.
-    - etc.
-
-    The SLM object also holds a lookup table that maps the phase values to gray values.
-    By default, this is a linear table that maps wrapped phase values from 0-2pi to gray values from 0-255.
-    This table can be modified to correct for the non-linear response of the hardware, or to scale the range
-    of gray values that is used.
     """
     __slots__ = ['_vertex_array', '_frame_buffer', '_monitor_id', '_position', '_refresh_rate',
                  '_transform', '_shape', '_window', '_globals', '_frame_buffer', 'patches', 'primary_patch',
                  '_coordinate_system', '_pixel_reader', '_phase_reader', '_field_reader', '_context']
 
     _active_slms = WeakSet()
     """Keep track of all active SLMs. This is done for two reasons. First, to check if we are not putting two
@@ -175,15 +153,15 @@
 
         return shape, mode.refresh_rate, min([mode.bits.red, mode.bits.green, mode.bits.blue])
 
     def _on_resize(self):
         """Updates shape and refresh rate to the actual values of the window.
 
         Note that these values are in pixels, which may be different from the window size because the window size is
-        in screen coordinates, which may not always the same as pixels (e.g. on a retina display).
+        in screen coordinates, which may not always the same as pixels (e. g. on a retina display).
 
         For windowed SLMs, the refresh rate property is set to the refresh rate of the primary monitor.
 
         If the width, height or refresh rate differ from the requested values, or if the bit depth is less than 8,
         a warning is issued.
 
         This function also sets the viewport to the full window size and creates a frame buffer.
@@ -368,14 +346,21 @@
         Therefore, it can be used as software synchronization to the SLM.
 
         Note:
             This function *does not* wait for the image to appear on the SLM.
             To wait for the image stabilization explicitly, use 'wait()'.
             However, this should rarely be needed since all Detectors
             already call wait_finished before starting a measurement.
+
+        Note:
+            At the moment, :meth:`~.SLM.update` blocks until all OpenGL commands are processed,
+            and a vertical retrace occurs (i. e., the hardware signals the start of a new frame).
+            This behavior may change in the future and should not be relied on.
+            Instead, use the automatic synchronization mechanism to synchronize detectors with
+            the SLM hardware.
         """
         with self._context:
             # first draw all patches into the frame buffer
             glBindFramebuffer(GL.GL_FRAMEBUFFER, self._frame_buffer._frame_buffer)  # noqa - ok to access 'friend class'
             glClear(GL.GL_COLOR_BUFFER_BIT)
             for patch in self.patches:
                 patch._draw()  # noqa - ok to access 'friend class'
```

### Comparing `openwfs-0.1.0rc1/openwfs/slm/texture.py` & `openwfs-0.1.0rc2/openwfs/devices/slm/texture.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import numpy as np
 import warnings
 
+import numpy as np
+
 from .context import Context
 
 try:
     import OpenGL.GL as GL
     from OpenGL.GL import glGenTextures, glBindTexture, glTexImage2D, glTexSubImage2D, glTexImage1D, glTexSubImage1D, \
         glTexParameteri, glActiveTexture, glDeleteTextures, glGetTextureImage, glPixelStorei
 except AttributeError:
@@ -67,15 +68,15 @@
                     # overwrite existing texture
                     glTexSubImage1D(GL.GL_TEXTURE_1D, 0, 0, value.shape[0], data_format, data_type, value)
 
             elif self.type == GL.GL_TEXTURE_2D:
                 if value.ndim == 0:
                     value = value.reshape((1, 1))
                 elif value.ndim != 2:
-                    raise ValueError("Data should be a 2-d array or a scalar")
+                    raise ValueError("Data should be a 2-D array or a scalar")
                 if value.shape != self._data_shape:
                     glTexImage2D(GL.GL_TEXTURE_2D, 0, internal_format, value.shape[1], value.shape[0], 0,
                                  data_format, data_type, value)
                     self._data_shape = value.shape
                 else:
                     glTexSubImage2D(GL.GL_TEXTURE_2D, 0, 0, 0, value.shape[1], value.shape[0], data_format,
                                     data_type, value)
```

### Comparing `openwfs-0.1.0rc1/openwfs/utilities/patterns.py` & `openwfs-0.1.0rc2/openwfs/utilities/patterns.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-import numpy as np
 from typing import Union, Sequence, Optional
+
+import numpy as np
 from astropy.units import Quantity
+
 from .utilities import ExtentType, CoordinateType, unitless
 
 # shape of a numpy array, or a single integer that is broadcast to a square shape
 ShapeType = Union[int, Sequence[int]]
 
 # a scalar quantity with optional unit attached
 ScalarType = Union[float, np.ndarray, Quantity]
@@ -89,15 +91,15 @@
         shape: see module documentation
         g(tuple of two floats): gradient vector.
           This has the unit: 1 / extent.unit.
           For the default extent of (2.0, 2.0), a value of g=(1,0)
           corresponds to having a ramp from -2 to +2 over the height of the pattern
           When this pattern is used as a phase in a pupil-conjugate configuration,
           this corresponds to a displacement of -2/π times the Abbe diffraction limit
-          (e.g. a positive x-gradient g causes the focal point to move in the _negative_ x-direction)
+          (e. g. a positive x-gradient g causes the focal point to move in the _negative_ x-direction)
         extent: see module documentation
         phase_offset: optional additional phase offset to be added to the pattern
     """
     c0, c1 = coordinate_range(shape, extent * (Quantity(g) * 2.0))
     return unitless(c0 + (c1 + phase_offset))
 
 
@@ -159,15 +161,15 @@
     """Constructs an image of a centered Gaussian
 
     `waist`, `extent` and the optional `truncation_radius` should all have the same unit.
 
     Args:
         shape: see module documentation
         waist (ScalarType): location of the beam waist (1/e value)
-            relative to half of the size of the pattern (i.e. relative to the `radius` of the square)
+            relative to half of the size of the pattern (i. e. relative to the `radius` of the square)
         truncation_radius (ScalarType): when not None, specifies the radius of a disk that is used to truncate the
             Gaussian. All values outside the disk are set to 0.
         extent: see module documentation
 
     """
     r_sqr = r2_range(shape, extent)
     w2inv = -1.0 / waist ** 2
```

### Comparing `openwfs-0.1.0rc1/openwfs/utilities/utilities.py` & `openwfs-0.1.0rc2/openwfs/utilities/utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from dataclasses import dataclass
+from typing import Union, Sequence, Optional
+
+import cv2
+import numpy as np
 from astropy import units as u
 from astropy.units import Quantity
 from numpy.typing import ArrayLike
-from typing import Union, Sequence, Optional
-import numpy as np
-import cv2
-from dataclasses import dataclass
 
 # A coordinate is a sequence of two floats with an optional unit attached
 CoordinateType = Union[Sequence[float], np.ndarray, Quantity]
 
 # A transform is a 2x2 array with optional units attached
 TransformType = Union[np.ndarray, Quantity, Sequence[Sequence[float]]]
 
@@ -47,18 +48,23 @@
         return data.to_value(u.dimensionless_unscaled)
     else:
         return np.array(data)
 
 
 @dataclass
 class Transform:
-    """Represents a transformation from one coordinate system to the other.
+    """Represents a transformation from one 2-d coordinate system to another.
 
     Transform objects are used to specify any combination of shift, (anisotropic) scaling, rotation and shear.
-    Elements of the transformation are specified with an `astropy.unit` attached.
+    The transform matrix, as well as the source and destination origins, can be specified with astropy units attached.
+
+    Note that a Transform object does not contain any information about the extent and pixel size
+    of the source or destination image, it only specifies the coordinate transformation itself.
+    When a Transform object is used to transform image data (see :func:`project` and :func:`place`),
+    the pixel_size information should be specified separately.
     """
 
     """
     Args:
         transform:
             2x2 transformation matrix that transforms (y,x)
             coordinates in the source image to (y,x) coordinates in the destination image.
@@ -87,21 +93,41 @@
                  source_origin: Optional[CoordinateType] = None,
                  destination_origin: Optional[CoordinateType] = None):
 
         self.transform = Quantity(transform if transform is not None else np.eye(2))
         self.source_origin = Quantity(source_origin) if source_origin is not None else None
         self.destination_origin = Quantity(destination_origin) if destination_origin is not None else None
 
-    def cv2_matrix(self, source_shape: Sequence[int],
+        if source_origin is not None:
+            self.destination_unit(self.source_origin.unit)  # check if the units are consistent
+
+    def destination_unit(self, src_unit: u.Unit) -> u.Unit:
+        """Computes the unit of the output of the transformation, given the unit of the input.
+
+        Raises:
+            ValueError: If src_unit does not match the unit of the source_origin (if specified) or
+                if dst_unit does not match the unit of the destination_origin (if specified).
+        """
+        if self.source_origin is not None and not self.source_origin.unit.is_equivalent(src_unit):
+            raise ValueError("src_unit must match the units of source_origin.")
+
+        dst_unit = (self.transform[0, 0] * src_unit).unit
+        if self.destination_origin is not None and not self.destination_origin.unit.is_equivalent(dst_unit):
+            raise ValueError("dst_unit must match the units of destination_origin.")
+
+        return dst_unit
+
+    def cv2_matrix(self,
+                   source_shape: Sequence[int],
                    source_pixel_size: CoordinateType,
                    destination_shape: Sequence[int],
                    destination_pixel_size: CoordinateType) -> np.ndarray:
         """Returns the transformation matrix in the format used by cv2.warpAffine."""
 
-        # correct the origin. OpenCV uses the _center_ of teh top-left corner as the origin
+        # correct the origin. OpenCV uses the _center_ of the top-left corner as the origin
         # and openwfs uses the center of the image as the origin, so we need to shift the origin
         # by half the image size minus half a pixel.
         if min(source_shape) < 1 or min(destination_shape) < 1:
             raise ValueError("Image size must be positive")
 
         source_origin = 0.5 * (np.array(source_shape) - 1.0) * source_pixel_size
         if self.source_origin is not None:
@@ -214,35 +240,36 @@
     It is scaled (using area interpolation) so that the pixel size matches that of the output.
     Then, the source array is placed into the output array at the position given by offset,
     where `offset=None` or `offset=(0.0, 0.0) * pixel_size` corresponds to centering the source image
     with respect to the output array.
     Parts of the source array that extend beyond the output are cropped, and parts of the array that are not
     covered by the source array are zero padded.
 
-    Note: this function currently works for 2-d inputs only
+    Note: this function currently works for 2-D inputs only
 
     Args:
 
     """
     out_extent = out_pixel_size * np.array(out_shape)
     transform = Transform(destination_origin=offset)
     return project(source, out_extent=out_extent, out_shape=out_shape, transform=transform, out=out)
 
 
-def project(source: np.ndarray, *,
-            transform: Optional[Transform] = None,
-            out: Optional[np.ndarray] = None,
-            source_extent: Optional[ExtentType] = None,
-            out_extent: Optional[ExtentType] = None,
-            out_shape: Optional[tuple[int, ...]] = None) -> np.ndarray:
+def project(
+        source: np.ndarray, *,
+        source_extent: Optional[ExtentType] = None,
+        transform: Optional[Transform] = None,
+        out: Optional[np.ndarray] = None,
+        out_extent: Optional[ExtentType] = None,
+        out_shape: Optional[tuple[int, ...]] = None) -> np.ndarray:
     """Projects the input image onto an array with specified shape and resolution.
 
     The input image is scaled so that the pixel sizes match those of the output,
     and cropped/zero-padded so that the data shape matches that of the output.
-    Optionally, an additional transformation can be specified, e.g., to scale or translate the source image.
+    Optionally, an additional transformation can be specified, e. g., to scale or translate the source image.
     This transformation is specified as a 2x3 transformation matrix in homogeneous coordinates.
 
     Args:
         source (np.ndarray): input image.
             Must have the pixel_size set (see set_pixel_size)
         transform: transformation to appy to the source image before placing it in the output
         out (np.ndarray): optional array where the output image is stored in.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `openwfs-0.1.0rc1/pyproject.toml` & `openwfs-0.1.0rc2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "openwfs"
-version = "0.1.0rc1"
+version = "0.1.0rc2"
 description = 'A libary for performing wavefront shaping experiments and simulations'
 authors = ["Ivo Vellekoop <i.m.vellekoop@utwente.nl>", "Daniël Cox", "Jeroen Doornbos"]
 license = "BSD-3-Clause"
-readme = "README.rst"
+readme = "readme.md"
 repository = "https://github.com/ivovellekoop/openwfs"
 documentation = "https://openwfs.readthedocs.io/en/latest/"
 classifiers = [
     'Programming Language :: Python :: 3',
     'Development Status :: 3 - Alpha',
     'License :: OSI Approved :: BSD License',
     'Operating System :: OS Independent',
 ]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = ">=3.9, <3.12"    # The genicam dependency is currently not available for Python 3.12
 numpy = ">=1.25.2"
 astropy = ">=5.3.4"
 glfw = ">=2.5.9"
 opencv-python = ">=4.9.0.80"
 matplotlib = ">=3.7.3"
 scipy = ">=1.11.3"
 nidaqmx = ">=0.8.0"
@@ -43,8 +43,11 @@
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = ">=4.1.2"
 sphinx_mdinclude = ">= 0.5.0"
 sphinx-rtd-theme = ">= 2.0.0"
 sphinx-autodoc-typehints = ">= 1.11.0"
+sphinxcontrib-bibtex = ">= 2.6.0"
+sphinx-markdown-builder = ">= 0.6.6"
+sphinx-gallery = ">= 0.15.0"
```

