# Comparing `tmp/revolve2_mujoco_simulator-1.0.2-py3-none-any.whl.zip` & `tmp/revolve2_mujoco_simulator-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,21 @@
-Zip file size: 18424 bytes, number of entries: 17
+Zip file size: 22026 bytes, number of entries: 19
 -rw-r--r--  2.0 unx      118 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/__init__.py
--rw-r--r--  2.0 unx     1059 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_abstraction_to_mujoco_mapping.py
+-rw-r--r--  2.0 unx     1340 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_abstraction_to_mujoco_mapping.py
 -rw-r--r--  2.0 unx     1598 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_control_interface_impl.py
--rw-r--r--  2.0 unx     7618 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_custom_mujoco_viewer.py
--rw-r--r--  2.0 unx     4551 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_local_simulator.py
--rw-r--r--  2.0 unx    14355 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_scene_to_model.py
--rw-r--r--  2.0 unx     3134 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_simulate_manual_scene.py
--rw-r--r--  2.0 unx     5716 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_simulate_scene.py
--rw-r--r--  2.0 unx     4092 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_simulation_state_impl.py
+-rw-r--r--  2.0 unx     8088 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_custom_mujoco_viewer.py
+-rw-r--r--  2.0 unx     4703 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_local_simulator.py
+-rw-r--r--  2.0 unx     4220 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_open_gl_vision.py
+-rw-r--r--  2.0 unx      162 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_render_backend.py
+-rw-r--r--  2.0 unx    16964 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_scene_to_model.py
+-rw-r--r--  2.0 unx     3314 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_simulate_manual_scene.py
+-rw-r--r--  2.0 unx     6912 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_simulate_scene.py
+-rw-r--r--  2.0 unx     4727 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/_simulation_state_impl.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/py.typed
--rw-r--r--  2.0 unx      161 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/textures/__init__.py
+-rw-r--r--  2.0 unx      162 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/textures/__init__.py
 -rw-r--r--  2.0 unx      507 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/textures/_checker.py
 -rw-r--r--  2.0 unx      414 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/textures/_flat.py
 -rw-r--r--  2.0 unx      462 b- defN 80-Jan-01 00:00 revolve2/simulators/mujoco_simulator/textures/_gradient.py
--rw-r--r--  2.0 unx     3260 b- defN 80-Jan-01 00:00 revolve2_mujoco_simulator-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 revolve2_mujoco_simulator-1.0.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1854 b- defN 16-Jan-01 00:00 revolve2_mujoco_simulator-1.0.2.dist-info/RECORD
-17 files, 48987 bytes uncompressed, 15214 bytes compressed:  68.9%
+-rw-r--r--  2.0 unx     3265 b- defN 80-Jan-01 00:00 revolve2_mujoco_simulator-1.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 revolve2_mujoco_simulator-1.1.1.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2077 b- defN 16-Jan-01 00:00 revolve2_mujoco_simulator-1.1.1.dist-info/RECORD
+19 files, 59121 bytes uncompressed, 18444 bytes compressed:  68.8%
```

## zipnote {}

```diff
@@ -9,14 +9,20 @@
 
 Filename: revolve2/simulators/mujoco_simulator/_custom_mujoco_viewer.py
 Comment: 
 
 Filename: revolve2/simulators/mujoco_simulator/_local_simulator.py
 Comment: 
 
+Filename: revolve2/simulators/mujoco_simulator/_open_gl_vision.py
+Comment: 
+
+Filename: revolve2/simulators/mujoco_simulator/_render_backend.py
+Comment: 
+
 Filename: revolve2/simulators/mujoco_simulator/_scene_to_model.py
 Comment: 
 
 Filename: revolve2/simulators/mujoco_simulator/_simulate_manual_scene.py
 Comment: 
 
 Filename: revolve2/simulators/mujoco_simulator/_simulate_scene.py
@@ -36,17 +42,17 @@
 
 Filename: revolve2/simulators/mujoco_simulator/textures/_flat.py
 Comment: 
 
 Filename: revolve2/simulators/mujoco_simulator/textures/_gradient.py
 Comment: 
 
-Filename: revolve2_mujoco_simulator-1.0.2.dist-info/METADATA
+Filename: revolve2_mujoco_simulator-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: revolve2_mujoco_simulator-1.0.2.dist-info/WHEEL
+Filename: revolve2_mujoco_simulator-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: revolve2_mujoco_simulator-1.0.2.dist-info/RECORD
+Filename: revolve2_mujoco_simulator-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## revolve2/simulators/mujoco_simulator/_abstraction_to_mujoco_mapping.py

```diff
@@ -1,11 +1,11 @@
 from dataclasses import dataclass, field
 
 from revolve2.simulation.scene import JointHinge, MultiBodySystem, UUIDKey
-from revolve2.simulation.scene.sensors import IMUSensor
+from revolve2.simulation.scene.sensors import CameraSensor, IMUSensor
 
 
 @dataclass
 class JointHingeMujoco:
     """Information about a MuJoCo hinge joint."""
 
     id: int
@@ -24,14 +24,22 @@
 class IMUSensorMujoco:
     """Information about a MuJoCo IMU sensor."""
 
     gyro_id: int
     accelerometer_id: int
 
 
+@dataclass
+class CameraSensorMujoco:
+    """Information about a MuJoCo camera sensor."""
+
+    camera_id: int
+    camera_size: tuple[int, int]
+
+
 @dataclass(eq=False)
 class AbstractionToMujocoMapping:
     """Data to interpret a MuJoCo model using the simulation abstraction."""
 
     hinge_joint: dict[UUIDKey[JointHinge], JointHingeMujoco] = field(
         init=False, default_factory=dict
     )
@@ -39,7 +47,10 @@
     multi_body_system: dict[UUIDKey[MultiBodySystem], MultiBodySystemMujoco] = field(
         init=False, default_factory=dict
     )
 
     imu_sensor: dict[UUIDKey[IMUSensor], IMUSensorMujoco] = field(
         init=False, default_factory=dict
     )
+    camera_sensor: dict[UUIDKey[CameraSensor], CameraSensorMujoco] = field(
+        init=False, default_factory=dict
+    )
```

## revolve2/simulators/mujoco_simulator/_custom_mujoco_viewer.py

```diff
@@ -1,15 +1,18 @@
 """A custom viewer for mujoco with additional features."""
+
 from enum import Enum
 from typing import Any
 
 import glfw
 import mujoco
 import mujoco_viewer
 
+from ._render_backend import RenderBackend
+
 
 class CustomMujocoViewerMode(Enum):
     """
     Enumerate different viewer modes for the CustomMujocoViewer.
 
     - CLASSIC mode gives an informative interface for regular simulations.
     - MANUAL mode gives a cut down interface, specific for targeting robot movement manually.
@@ -39,36 +42,47 @@
     _advance_by_one_step: bool
     _position: int
 
     def __init__(
         self,
         model: mujoco.MjModel,
         data: mujoco.MjData,
+        backend: RenderBackend,
         start_paused: bool = False,
         render_every_frame: bool = False,
         mode: CustomMujocoViewerMode = CustomMujocoViewerMode.CLASSIC,
     ):
         """
         Initialize the Viewer.
 
         :param model: The mujoco models.
         :param data: The mujoco data.
+        :param backend: The backend for rendering.
         :param start_paused: If the simulation starts paused or not.
         :param render_every_frame: If every frame is rendered or not.
         :param mode: The mode of the viewer (classic, manual).
         """
+        match backend:
+            case RenderBackend.EGL:
+                glfw.window_hint(glfw.CONTEXT_CREATION_API, glfw.EGL_CONTEXT_API)
+            case RenderBackend.OSMESA:
+                glfw.window_hint(glfw.CONTEXT_CREATION_API, glfw.OSMESA_CONTEXT_API)
+            case _:  # By default, we are using GLFW.
+                pass
+
         super().__init__(
             model,
             data,
             mode="window",
             title="custom-mujoco-viewer",
             width=None,
             height=None,
             hide_menus=False,
         )
+
         self._viewer_mode = mode
         self._position = 0
         self._paused = start_paused
         self._mujoco_version = tuple(map(int, mujoco.__version__.split(".")))
         self._render_every_frame = render_every_frame
 
     def _add_overlay(self, gridpos: int, text1: str, text2: str) -> None:
```

## revolve2/simulators/mujoco_simulator/_local_simulator.py

```diff
@@ -82,15 +82,15 @@
 
         if self._num_simulators > 1:
             with concurrent.futures.ProcessPoolExecutor(
                 max_workers=self._num_simulators
             ) as executor:
                 futures = [
                     executor.submit(
-                        simulate_scene,
+                        simulate_scene,  # This is the function to call, followed by the parameters of the function
                         scene_index,
                         scene,
                         self._headless,
                         batch.record_settings,
                         self._start_paused,
                         control_step,
                         sample_step,
@@ -101,15 +101,15 @@
                     )
                     for scene_index, scene in enumerate(batch.scenes)
                 ]
                 results = [future.result() for future in futures]
         else:
             results = [
                 simulate_scene(
-                    scene_index,
+                    scene_index,  # This is the function to call, followed by the parameters of the function
                     scene,
                     self._headless,
                     batch.record_settings,
                     self._start_paused,
                     control_step,
                     sample_step,
                     batch.parameters.simulation_time,
```

## revolve2/simulators/mujoco_simulator/_scene_to_model.py

```diff
@@ -1,9 +1,10 @@
 import os
 import tempfile
+from itertools import product
 from typing import Any
 
 import mujoco
 
 try:
     import logging
 
@@ -18,20 +19,25 @@
     ), "dm_control not adding logging handler as expected. Maybe they fixed their annoying behaviour? https://github.com/deepmind/dm_control/issues/314"
 
     logging.root.removeHandler(logging.root.handlers[-1])
 except Exception as e:
     print("Failed to fix absl logging bug", e)
     pass
 
-from revolve2.simulation.scene import Scene, UUIDKey
+from revolve2.simulation.scene import JointHinge, RigidBody, Scene, UUIDKey
 from revolve2.simulation.scene.conversion import multi_body_system_to_urdf
-from revolve2.simulation.scene.geometry import Geometry, GeometryHeightmap
+from revolve2.simulation.scene.geometry import (
+    Geometry,
+    GeometryHeightmap,
+    GeometryPlane,
+)
 
 from ._abstraction_to_mujoco_mapping import (
     AbstractionToMujocoMapping,
+    CameraSensorMujoco,
     IMUSensorMujoco,
     JointHingeMujoco,
     MultiBodySystemMujoco,
 )
 
 
 def scene_to_model(
@@ -75,245 +81,65 @@
             scene.multi_body_systems
         )
     ]
     all_joints_and_names = [c[3] for c in conversions]
     all_rigid_bodies_and_names = [c[5] for c in conversions]
 
     heightmaps: list[GeometryHeightmap] = []
-
     for mbs_i, (
         multi_body_system,
         (
             urdf,
             plane_geometries,
             heightmap_geometries,
             joints_and_names,
             geoms_and_names,
             rigid_bodies_and_names,
         ),
     ) in enumerate(zip(scene.multi_body_systems, conversions, strict=True)):
         multi_body_system_model = mujoco.MjModel.from_xml_string(urdf)
-
-        # MuJoCo can only save to a file, not directly to string,
-        # so we create a temporary file.
-        try:
-            with tempfile.NamedTemporaryFile(
-                mode="r+", delete=True, suffix="_revolve2_mujoco.mjcf"
-            ) as mjcf_file:
-                mujoco.mj_saveLastXML(mjcf_file.name, multi_body_system_model)
-                multi_body_system_mjcf = mjcf.from_file(mjcf_file)
-        # handle an exception when the xml saving fails, it's almost certain to occur on Windows
-        # since NamedTemporaryFile can't be opened twice when the file is still open.
-        except Exception:
-            with tempfile.NamedTemporaryFile(
-                mode="r+", delete=False, suffix="_revolve2_mujoco.mjcf"
-            ) as mjcf_file:
-                # to make sure the temp file is always deleted,
-                # an error catching is needed, in case the xml saving fails and crashes the program
-                try:
-                    mujoco.mj_saveLastXML(mjcf_file.name, multi_body_system_model)
-                    multi_body_system_mjcf = mjcf.from_file(
-                        mjcf_file,
-                    )
-                    # On Windows, an open file can’t be deleted, and hence it has to be closed first before removing
-                    mjcf_file.close()
-                    os.remove(mjcf_file.name)
-                except Exception as e:
-                    logging.info(repr(e))
-                    # On Windows, an open file can’t be deleted, and hence it has to be closed first before removing
-                    mjcf_file.close()
-                    os.remove(mjcf_file.name)
+        multi_body_system_mjcf = _create_tmp_file(multi_body_system_model)
 
         # The following few are set automatically during the urdf conversion,
         # but make no sense when we combine multiple URDFs.
         # So, we remote them and have mujoco calculate them for us.
         multi_body_system_mjcf.statistic.extent = None
         multi_body_system_mjcf.statistic.center = None
         multi_body_system_mjcf.statistic.meansize = None
         attachment_frame = env_mjcf.attach(multi_body_system_mjcf)
-        attachment_frame.pos = [
-            multi_body_system.pose.position.x,
-            multi_body_system.pose.position.y,
-            multi_body_system.pose.position.z,
-        ]
-        attachment_frame.quat = [
-            multi_body_system.pose.orientation.x,
-            multi_body_system.pose.orientation.y,
-            multi_body_system.pose.orientation.z,
-            multi_body_system.pose.orientation.w,
-        ]
+        attachment_frame.pos = [*multi_body_system.pose.position]
+        attachment_frame.quat = [*multi_body_system.pose.orientation]
         if not multi_body_system.is_static:
             attachment_frame.add("freejoint")
 
         # Add actuation to joints
-        for joint, name in joints_and_names:
-            # Add rotor inertia to joints. This value is arbitrarily chosen and appears stable enough.
-            # Fine-tuning the armature value might be needed later.
-            multi_body_system_mjcf.find(
-                namespace="joint", identifier=name
-            ).armature = joint.armature
-            multi_body_system_mjcf.actuator.add(
-                "position",
-                kp=joint.pid_gain_p,
-                joint=multi_body_system_mjcf.find(
-                    namespace="joint",
-                    identifier=name,
-                ),
-                name=f"actuator_position_{name}",
-            )
-            multi_body_system_mjcf.actuator.add(
-                "velocity",
-                kv=joint.pid_gain_d,
-                joint=multi_body_system_mjcf.find(namespace="joint", identifier=name),
-                name=f"actuator_velocity_{name}",
-            )
+        _add_joint_actuators(joints_and_names, multi_body_system_mjcf)
 
-        # Add IMUs
-        for rigid_body, name in rigid_bodies_and_names:
-            if len(rigid_body.imu_sensors) > 0:
-                if name == f"mbs{mbs_i}":
-                    rigid_body_mjcf = multi_body_system_mjcf.worldbody
-                else:
-                    rigid_body_mjcf = multi_body_system_mjcf.find(
-                        namespace="body", identifier=name
-                    )
-                for imu_i, imu in enumerate(rigid_body.imu_sensors):
-                    site_name = f"{name}_site_imu_{imu_i}"
-                    rigid_body_mjcf.add(
-                        "site",
-                        name=site_name,
-                        pos=[
-                            imu.pose.position.x,
-                            imu.pose.position.y,
-                            imu.pose.position.z,
-                        ],
-                        quat=[
-                            imu.pose.orientation.x,
-                            imu.pose.orientation.y,
-                            imu.pose.orientation.z,
-                            imu.pose.orientation.w,
-                        ],
-                    )
-                    gyro_name = f"imu_gyro_{name}_{imu_i}"
-                    multi_body_system_mjcf.sensor.add(
-                        "gyro", name=gyro_name, site=site_name
-                    )
-                    accelerometer_name = f"imu_accelerometer_{name}_{imu_i}"
-                    multi_body_system_mjcf.sensor.add(
-                        "accelerometer",
-                        name=accelerometer_name,
-                        site=site_name,
-                    )
+        # Add Sensors
+        _add_sensors(rigid_bodies_and_names, mbs_i, multi_body_system_mjcf, env_mjcf)
 
         # Add plane geometries
-        i_plane = 0
-        for plane in plane_geometries:
-            name = f"heightmap_{i_plane}"
-            plane_kwargs: dict[str, Any] = {}
-            if fast_sim:
-                plane_kwargs[
-                    "rgba"
-                ] = plane.texture.primary_color.to_normalized_rgba_list()
-            else:
-                plane_kwargs["material"] = f"{name}_material"
-                __make_material(env_mjcf, name=name, element=plane)
-
-            env_mjcf.worldbody.add(
-                "geom",
-                type="plane",
-                pos=[
-                    plane.pose.position.x,
-                    plane.pose.position.y,
-                    plane.pose.position.z,
-                ],
-                quat=[
-                    plane.pose.orientation.x,
-                    plane.pose.orientation.y,
-                    plane.pose.orientation.z,
-                    plane.pose.orientation.w,
-                ],
-                size=[plane.size.x / 2.0, plane.size.y / 2.0, 1.0],
-                **plane_kwargs,
-            )
-            i_plane += 1
+        _add_planes(plane_geometries, fast_sim, env_mjcf)
 
         # Add heightmap geometries
-        i_heightmap = 0
-        for heightmap in heightmap_geometries:
-            env_mjcf.asset.add(
-                "hfield",
-                name=f"hfield_{i_heightmap}",
-                nrow=len(heightmap.heights),
-                ncol=len(heightmap.heights[0]),
-                size=[
-                    heightmap.size.x,
-                    heightmap.size.y,
-                    heightmap.size.z,
-                    heightmap.base_thickness,
-                ],
-            )
-
-            name = f"heightmap_{i_heightmap}"
-            hm_kwargs: dict[str, Any] = {}
-            if fast_sim:
-                hm_kwargs[
-                    "rgba"
-                ] = heightmap.texture.primary_color.to_normalized_rgba_list()
-            else:
-                hm_kwargs["material"] = f"{name}_material"
-                __make_material(env_mjcf, name=name, element=heightmap)
-
-            env_mjcf.worldbody.add(
-                "geom",
-                type="hfield",
-                hfield=f"hfield_{i_heightmap}",
-                pos=[
-                    heightmap.pose.position.x,
-                    heightmap.pose.position.y,
-                    heightmap.pose.position.z,
-                ],
-                quat=[
-                    heightmap.pose.orientation.x,
-                    heightmap.pose.orientation.y,
-                    heightmap.pose.orientation.z,
-                    heightmap.pose.orientation.w,
-                ],
-                **hm_kwargs,
-            )
-
-            heightmaps.append(heightmap)
-            i_heightmap += 1
+        hmps = _add_heightmaps(heightmap_geometries, fast_sim, env_mjcf)
+        heightmaps.extend(hmps)
 
         # Set colors of geometries
-        for geom, name in geoms_and_names:
-            if fast_sim:
-                multi_body_system_mjcf.find(
-                    "geom", name
-                ).rgba = geom.texture.primary_color.to_normalized_rgba_list()
-            else:
-                m_name = f"geom_{name}"
-                __make_material(multi_body_system_mjcf, name=m_name, element=geom)
-                multi_body_system_mjcf.find(
-                    "geom", name
-                ).material = f"{m_name}_material"
+        _set_colors_and_materials(
+            geoms_and_names, multi_body_system_mjcf, fast_sim=fast_sim
+        )
 
     xml = env_mjcf.to_xml_string()
     assert isinstance(xml, str)
 
     model = mujoco.MjModel.from_xml_string(xml)
 
     # set height map values
-    heightmap_offset = 0
-    for heightmap in heightmaps:
-        for x in range(len(heightmap.heights)):
-            for y in range(len(heightmap.heights[0])):
-                model.hfield_data[y * len(heightmap.heights) + x] = heightmap.heights[
-                    x
-                ][y]
-        heightmap_offset += len(heightmap.heights) * len(heightmap.heights[0])
+    _set_heightmap_values(heightmaps, model)
 
     # Create map from hinge joints to their corresponding indices in the ctrl and position array
     for mbs_i, joints_and_names in enumerate(all_joints_and_names):
         for joint, name in joints_and_names:
             mapping.hinge_joint[UUIDKey(joint)] = JointHingeMujoco(
                 id=model.joint(f"mbs{mbs_i}/{name}").id,
                 ctrl_index_position=model.actuator(
@@ -325,28 +151,306 @@
             )
 
     for mbs_i, multi_body_system in enumerate(scene.multi_body_systems):
         mapping.multi_body_system[UUIDKey(multi_body_system)] = MultiBodySystemMujoco(
             id=model.body(f"mbs{mbs_i}/").id
         )
 
-    # Create IMU map
+    # Create sensor maps
+    _creat_sensor_maps(all_rigid_bodies_and_names, mapping, model)
+
+    return model, mapping
+
+
+def _create_tmp_file(multi_body_system_model: mujoco.MjModel) -> mjcf.RootElement:
+    """
+    Create a temporary file.
+
+    MuJoCo can only save to a file, not directly to string,
+
+    :param multi_body_system_model: The multi-body-system model.
+    :return: The root element for the mujoco viewer.
+    """
+    try:
+        with tempfile.NamedTemporaryFile(
+            mode="r+", delete=True, suffix="_revolve2_mujoco.mjcf"
+        ) as mjcf_file:
+            mujoco.mj_saveLastXML(mjcf_file.name, multi_body_system_model)
+            multi_body_system_mjcf = mjcf.from_file(mjcf_file)
+    # handle an exception when the xml saving fails, it's almost certain to occur on Windows
+    # since NamedTemporaryFile can't be opened twice when the file is still open.
+    except Exception:
+        with tempfile.NamedTemporaryFile(
+            mode="r+", delete=False, suffix="_revolve2_mujoco.mjcf"
+        ) as mjcf_file:
+            # to make sure the temp file is always deleted,
+            # an error catching is needed, in case the xml saving fails and crashes the program
+            try:
+                mujoco.mj_saveLastXML(mjcf_file.name, multi_body_system_model)
+                multi_body_system_mjcf = mjcf.from_file(
+                    mjcf_file,
+                )
+                # On Windows, an open file can’t be deleted, and hence it has to be closed first before removing
+                mjcf_file.close()
+                os.remove(mjcf_file.name)
+            except Exception as e:
+                logging.info(repr(e))
+                # On Windows, an open file can’t be deleted, and hence it has to be closed first before removing
+                mjcf_file.close()
+                os.remove(mjcf_file.name)
+    return multi_body_system_mjcf
+
+
+def _add_planes(
+    plane_geometries: list[GeometryPlane], fast_sim: bool, env_mjcf: mjcf.RootElement
+) -> None:
+    """
+    Add plane objects to the mujoco simulation.
+
+    :param plane_geometries: The plane geometries.
+    :param fast_sim: Whether fast sim is used.
+    :param env_mjcf: The mujoco environment to simulate.
+    """
+    i_plane = 0
+    for plane in plane_geometries:
+        name = f"heightmap_{i_plane}"
+        plane_kwargs: dict[str, Any] = {}
+        if fast_sim:
+            plane_kwargs["rgba"] = plane.texture.primary_color.to_normalized_rgba_list()
+        else:
+            plane_kwargs["material"] = f"{name}_material"
+            __make_material(env_mjcf, name=name, element=plane)
+
+        env_mjcf.worldbody.add(
+            "geom",
+            type="plane",
+            pos=[*plane.pose.position],
+            quat=[*plane.pose.orientation],
+            size=[plane.size.x / 2.0, plane.size.y / 2.0, 1.0],
+            **plane_kwargs,
+        )
+        i_plane += 1
+
+
+def _add_heightmaps(
+    heightmap_geometries: list[GeometryHeightmap],
+    fast_sim: bool,
+    env_mjcf: mjcf.RootElement,
+) -> list[GeometryHeightmap]:
+    """
+    Add heightmap geometries to the model.
+
+    :param heightmap_geometries: The heightmap geometries.
+    :param fast_sim: If fast sim is used.
+    :param env_mjcf: The mujoco root object.
+    :return: A list of heightmap geometries.
+    """
+    heightmaps: list[GeometryHeightmap] = []
+
+    i_heightmap = 0
+    for heightmap in heightmap_geometries:
+        env_mjcf.asset.add(
+            "hfield",
+            name=f"hfield_{i_heightmap}",
+            nrow=len(heightmap.heights),
+            ncol=len(heightmap.heights[0]),
+            size=[
+                *heightmap.size,
+                heightmap.base_thickness,
+            ],
+        )
+
+        name = f"heightmap_{i_heightmap}"
+        hm_kwargs: dict[str, Any] = {}
+        if fast_sim:
+            hm_kwargs["rgba"] = (
+                heightmap.texture.primary_color.to_normalized_rgba_list()
+            )
+        else:
+            hm_kwargs["material"] = f"{name}_material"
+            __make_material(env_mjcf, name=name, element=heightmap)
+
+        env_mjcf.worldbody.add(
+            "geom",
+            type="hfield",
+            hfield=f"hfield_{i_heightmap}",
+            pos=[*heightmap.pose.position],
+            quat=[*heightmap.pose.orientation],
+            **hm_kwargs,
+        )
+
+        heightmaps.append(heightmap)
+        i_heightmap += 1
+    return heightmaps
+
+
+def _add_sensors(
+    rigid_bodies_and_names: list[tuple[RigidBody, str]],
+    mbs_i: int,
+    multi_body_system_mjcf: mjcf.RootElement,
+    env_mjcf: mjcf.RootElement,
+) -> None:
+    """
+    Add sensors to the model.
+
+    :param rigid_bodies_and_names: The rigid bodies and names.
+    :param mbs_i: The current index of the multi body system.
+    :param multi_body_system_mjcf: The MBS in mujoco format.
+    :param env_mjcf: The environment in mujoco format.
+    """
+    for rigid_body, name in rigid_bodies_and_names:
+        if name == f"mbs{mbs_i}":
+            rigid_body_mjcf = multi_body_system_mjcf.worldbody
+        else:
+            rigid_body_mjcf = multi_body_system_mjcf.find(
+                namespace="body", identifier=name
+            )
+
+        """Here we add the IMU Sensors."""
+        for imu_i, imu in enumerate(rigid_body.sensors.imu_sensors):
+            site_name = f"{name}_site_imu_{imu_i}"
+            rigid_body_mjcf.add(
+                "site",
+                name=site_name,
+                pos=[*imu.pose.position],
+                quat=[*imu.pose.orientation],
+            )
+            gyro_name = f"imu_gyro_{name}_{imu_i}"
+            multi_body_system_mjcf.sensor.add("gyro", name=gyro_name, site=site_name)
+            accelerometer_name = f"imu_accelerometer_{name}_{imu_i}"
+            multi_body_system_mjcf.sensor.add(
+                "accelerometer",
+                name=accelerometer_name,
+                site=site_name,
+            )
+
+        """Here we add camera Sensors."""
+        for camera_i, camera in enumerate(rigid_body.sensors.camera_sensors):
+            camera_name = f"camera_{name}_{camera_i+1}"
+            env_mjcf.worldbody.add(
+                "camera",
+                name=camera_name,
+                mode="fixed",
+                xyaxes="0 -1 0 0 0 1",
+                dclass=env_mjcf.full_identifier,
+            )
+            site_name = f"{name}_site_camera_{camera_i+1}"
+            env_mjcf.worldbody.add(
+                "site",
+                name=site_name,
+                pos=[*camera.pose.position],
+                quat=[*camera.pose.orientation],
+            )
+
+
+def _add_joint_actuators(
+    joints_and_names: list[tuple[JointHinge, str]],
+    multi_body_system_mjcf: mjcf.RootElement,
+) -> None:
+    """
+    Add actuation to the joints.
+
+    :param joints_and_names: The joints.
+    :param multi_body_system_mjcf: The multi body system.
+    """
+    for joint, name in joints_and_names:
+        # Add rotor inertia to joints. This value is arbitrarily chosen and appears stable enough.
+        # Fine-tuning the armature value might be needed later.
+        multi_body_system_mjcf.find(namespace="joint", identifier=name).armature = (
+            joint.armature
+        )
+        multi_body_system_mjcf.actuator.add(
+            "position",
+            kp=joint.pid_gain_p,
+            joint=multi_body_system_mjcf.find(
+                namespace="joint",
+                identifier=name,
+            ),
+            name=f"actuator_position_{name}",
+        )
+        multi_body_system_mjcf.actuator.add(
+            "velocity",
+            kv=joint.pid_gain_d,
+            joint=multi_body_system_mjcf.find(namespace="joint", identifier=name),
+            name=f"actuator_velocity_{name}",
+        )
+
+
+def _set_colors_and_materials(
+    geoms_and_names: list[tuple[Geometry, str]],
+    multi_body_system_mjcf: mjcf.RootElement,
+    fast_sim: bool,
+) -> None:
+    """
+    Set the colors and materials for the geometries contained in the model.
+
+    :param geoms_and_names: The geometries with their respective names in the model.
+    :param multi_body_system_mjcf: The mujoco model.
+    :param fast_sim: Whether fast sim is used.
+    """
+    for geom, name in geoms_and_names:
+        if fast_sim:
+            multi_body_system_mjcf.find("geom", name).rgba = (
+                geom.texture.primary_color.to_normalized_rgba_list()
+            )
+        else:
+            m_name = f"geom_{name}"
+            __make_material(multi_body_system_mjcf, name=m_name, element=geom)
+            multi_body_system_mjcf.find("geom", name).material = f"{m_name}_material"
+
+
+def _set_heightmap_values(
+    heightmaps: list[GeometryHeightmap], model: mujoco.MjModel
+) -> None:
+    """
+    Set the values for the heightmaps.
+
+    :param heightmaps: The heightmaps.
+    :param model: The mujoco model.
+    """
+    heightmap_offset = 0
+
+    for heightmap in heightmaps:
+        for x, y in product(
+            range(len(heightmap.heights)), range(len(heightmap.heights[0]))
+        ):
+            model.hfield_data[y * len(heightmap.heights) + x] = heightmap.heights[x][y]
+        heightmap_offset += len(heightmap.heights) * len(heightmap.heights[0])
+
+
+def _creat_sensor_maps(
+    all_rigid_bodies_and_names: list[list[tuple[RigidBody, str]]],
+    mapping: AbstractionToMujocoMapping,
+    model: mujoco.MjModel,
+) -> None:
+    """
+    Create mappings of the imu sensors to the gyro and accelerator sensors in mujoco.
+
+    :param all_rigid_bodies_and_names: The rigid bodies and their respective name in the model.
+    :param mapping: The mapping of revolve2 components to Mujoco components.
+    :param model: The mujoco model.
+    """
     for mbs_i, rigid_bodies_and_names in enumerate(all_rigid_bodies_and_names):
         for rigid_body, name in rigid_bodies_and_names:
-            for imu_i, imu in enumerate(rigid_body.imu_sensors):
+            for imu_i, imu in enumerate(rigid_body.sensors.imu_sensors):
                 gyro_name = f"imu_gyro_{name}_{imu_i}"
                 accelerometer_name = f"imu_accelerometer_{name}_{imu_i}"
                 mapping.imu_sensor[UUIDKey(imu)] = IMUSensorMujoco(
                     gyro_id=model.sensor(f"mbs{mbs_i}/{gyro_name}").id,
                     accelerometer_id=model.sensor(
                         f"mbs{mbs_i}/{accelerometer_name}"
                     ).id,
                 )
 
-    return (model, mapping)
+            for camera_i, camera in enumerate(rigid_body.sensors.camera_sensors):
+                camera_name = f"camera_{name}_{camera_i+1}"
+                mapping.camera_sensor[UUIDKey(camera)] = CameraSensorMujoco(
+                    camera_id=model.camera(camera_name).id,
+                    camera_size=camera.camera_size,
+                )
 
 
 def __make_material(env: mjcf.RootElement, name: str, element: Geometry) -> None:
     width, height = element.texture.size
     mat_kwargs = {}
 
     if element.texture.reference is not None:
```

## revolve2/simulators/mujoco_simulator/_simulate_manual_scene.py

```diff
@@ -1,49 +1,52 @@
 """Iterative Scene Simulator."""
+
 import logging
 
 import mujoco
 
 from revolve2.ci_group.simulation_parameters import (
     STANDARD_CONTROL_FREQUENCY,
     STANDARD_SIMULATION_TIMESTEP,
 )
 from revolve2.simulation.scene import Scene
 
 from ._control_interface_impl import ControlInterfaceImpl
 from ._custom_mujoco_viewer import CustomMujocoViewer, CustomMujocoViewerMode
+from ._render_backend import RenderBackend
 from ._scene_to_model import scene_to_model
 from ._simulation_state_impl import SimulationStateImpl
 
 
 def simulate_manual_scene(
     scene: Scene,
+    render_backend: RenderBackend = RenderBackend.GLFW,
 ) -> None:
     """
     Simulate a scene for checking if a robot was built correctly.
 
     :param scene: The scene to simulate.
+    :param render_backend: The render backend.
     """
     logging.info("Simulating scene")
 
     model, mapping = scene_to_model(
         scene, STANDARD_SIMULATION_TIMESTEP, cast_shadows=False, fast_sim=False
     )
     data = mujoco.MjData(model)
     viewer = CustomMujocoViewer(
-        model,
-        data,
-        mode=CustomMujocoViewerMode.MANUAL,
+        model, data, mode=CustomMujocoViewerMode.MANUAL, backend=render_backend
     )
 
     # Compute forward dynamics without actually stepping forward in time.
     mujoco.mj_forward(model, data)
 
     control_interface = ControlInterfaceImpl(
-        data=data, abstraction_to_mujoco_mapping=mapping
+        data=data,
+        abstraction_to_mujoco_mapping=mapping,
     )
 
     """Here we set our values for cycling different positions."""
     prev_position: int = (
         0  # This is the initial idle position for all hinges (index of the positions).
     )
     positions: list[float] = [
@@ -56,15 +59,15 @@
     target, current = (
         0.0,
         0.0,
     )  # Here we can check whether we are currently on the correct position.
     try:
         while True:
             simulation_state = SimulationStateImpl(
-                data=data, abstraction_to_mujoco_mapping=mapping
+                data=data, abstraction_to_mujoco_mapping=mapping, camera_views={}
             )
             scene.handler.handle(
                 simulation_state, control_interface, STANDARD_CONTROL_FREQUENCY
             )
             # step simulation
             if target != current:
                 """
```

## revolve2/simulators/mujoco_simulator/_simulate_scene.py

```diff
@@ -7,14 +7,16 @@
 import numpy.typing as npt
 
 from revolve2.simulation.scene import Scene, SimulationState
 from revolve2.simulation.simulator import RecordSettings
 
 from ._control_interface_impl import ControlInterfaceImpl
 from ._custom_mujoco_viewer import CustomMujocoViewer
+from ._open_gl_vision import OpenGLVision
+from ._render_backend import RenderBackend
 from ._scene_to_model import scene_to_model
 from ._simulation_state_impl import SimulationStateImpl
 
 
 def simulate_scene(
     scene_id: int,
     scene: Scene,
@@ -23,14 +25,15 @@
     start_paused: bool,
     control_step: float,
     sample_step: float | None,
     simulation_time: int | None,
     simulation_timestep: float,
     cast_shadows: bool,
     fast_sim: bool,
+    render_backend: RenderBackend = RenderBackend.EGL,
 ) -> list[SimulationState]:
     """
     Simulate a scene.
 
     :param scene_id: An id for this scene, unique between all scenes ran in parallel.
     :param scene: The scene to simulate.
     :param headless: If False, a viewer will be opened that allows a user to manually view and manually interact with the simulation.
@@ -38,30 +41,42 @@
     :param start_paused: If true, the simulation will start in a paused state. Only makessense when headless is False.
     :param control_step: The time between each call to the handle function of the scene handler. In seconds.
     :param sample_step: The time between each state sample of the simulation. In seconds.
     :param simulation_time: How long to simulate for. In seconds.
     :param simulation_timestep: The duration to integrate over during each step of the simulation. In seconds.
     :param cast_shadows: If shadows are cast.
     :param fast_sim: If fancy rendering is disabled.
+    :param render_backend: The backend to be used for rendering (EGL by default and switches to GLFW if no cameras are on the robot).
     :returns: The results of simulation. The number of returned states depends on `sample_step`.
     """
     logging.info(f"Simulating scene {scene_id}")
 
     model, mapping = scene_to_model(
         scene, simulation_timestep, cast_shadows=cast_shadows, fast_sim=fast_sim
     )
+
+    """If we dont have cameras and the backend is not set we go to the default GLFW."""
+    if len(mapping.camera_sensor.values()) == 0:
+        render_backend = RenderBackend.GLFW
     data = mujoco.MjData(model)
 
     if not headless or record_settings is not None:
         viewer = CustomMujocoViewer(
             model,
             data,
+            backend=render_backend,
             start_paused=start_paused,
             render_every_frame=False,
         )
+    camera_viewers = {
+        camera.camera_id: OpenGLVision(
+            model=model, camera=camera, headless=headless, open_gl_lib=render_backend
+        )
+        for camera in mapping.camera_sensor.values()
+    }
 
     if record_settings is not None:
         video_step = 1 / record_settings.fps
         video_file_path = f"{record_settings.video_directory}/{scene_id}.mp4"
         fourcc = cv2.VideoWriter.fourcc(*"mp4v")
         video = cv2.VideoWriter(
             video_file_path,
@@ -78,48 +93,61 @@
 
     # The measured states of the simulation
     simulation_states: list[SimulationState] = []
 
     # Compute forward dynamics without actually stepping forward in time.
     # This updates the data so we can read out the initial state.
     mujoco.mj_forward(model, data)
+    images = {
+        camera_id: camera_viewer.process(model, data)
+        for camera_id, camera_viewer in camera_viewers.items()
+    }
 
     # Sample initial state.
     if sample_step is not None:
         simulation_states.append(
-            SimulationStateImpl(data=data, abstraction_to_mujoco_mapping=mapping)
+            SimulationStateImpl(
+                data=data, abstraction_to_mujoco_mapping=mapping, camera_views=images
+            )
         )
 
     control_interface = ControlInterfaceImpl(
         data=data, abstraction_to_mujoco_mapping=mapping
     )
     while (time := data.time) < (
         float("inf") if simulation_time is None else simulation_time
     ):
+
         # do control if it is time
         if time >= last_control_time + control_step:
             last_control_time = math.floor(time / control_step) * control_step
 
             simulation_state = SimulationStateImpl(
-                data=data, abstraction_to_mujoco_mapping=mapping
+                data=data, abstraction_to_mujoco_mapping=mapping, camera_views=images
             )
             scene.handler.handle(simulation_state, control_interface, control_step)
 
         # sample state if it is time
         if sample_step is not None:
             if time >= last_sample_time + sample_step:
                 last_sample_time = int(time / sample_step) * sample_step
                 simulation_states.append(
                     SimulationStateImpl(
-                        data=data, abstraction_to_mujoco_mapping=mapping
+                        data=data,
+                        abstraction_to_mujoco_mapping=mapping,
+                        camera_views=images,
                     )
                 )
 
         # step simulation
         mujoco.mj_step(model, data)
+        images = {
+            camera_id: camera_viewer.process(model, data)
+            for camera_id, camera_viewer in camera_viewers.items()
+        }
 
         # render if not headless. also render when recording and if it time for a new video frame.
         if not headless or (
             record_settings is not None and time >= last_video_time + video_step
         ):
             viewer.render()
 
@@ -147,13 +175,15 @@
 
     if record_settings is not None:
         video.release()
 
     # Sample one final time.
     if sample_step is not None:
         simulation_states.append(
-            SimulationStateImpl(data=data, abstraction_to_mujoco_mapping=mapping)
+            SimulationStateImpl(
+                data=data, abstraction_to_mujoco_mapping=mapping, camera_views=images
+            )
         )
 
     logging.info(f"Scene {scene_id} done.")
 
     return simulation_states
```

## revolve2/simulators/mujoco_simulator/_simulation_state_impl.py

```diff
@@ -7,47 +7,51 @@
     JointHinge,
     MultiBodySystem,
     Pose,
     RigidBody,
     SimulationState,
     UUIDKey,
 )
-from revolve2.simulation.scene.sensors import IMUSensor
+from revolve2.simulation.scene.sensors import CameraSensor, IMUSensor
 
 from ._abstraction_to_mujoco_mapping import AbstractionToMujocoMapping
 
 
 class SimulationStateImpl(SimulationState):
     """Implementation of the simulation state interface for MuJoCo."""
 
     _xpos: npt.NDArray[np.float_]
     _xquat: npt.NDArray[np.float_]
     _qpos: npt.NDArray[np.float_]
     _sensordata: npt.NDArray[np.float_]
     _abstraction_to_mujoco_mapping: AbstractionToMujocoMapping
+    _camera_views: dict[int, npt.NDArray[np.uint8]]
 
     def __init__(
         self,
         data: mujoco.MjData,
         abstraction_to_mujoco_mapping: AbstractionToMujocoMapping,
+        camera_views: dict[int, npt.NDArray[np.uint8]],
     ) -> None:
         """
         Initialize this object.
 
         The copies required information from the provided data.
         As such the data can be modified after this constructor without causing problems.
 
         :param data: The data to copy from.
         :param abstraction_to_mujoco_mapping: A mapping between simulation abstraction and mujoco.
+        :param camera_views: The camera views.
         """
         self._xpos = data.xpos.copy()
         self._xquat = data.xquat.copy()
         self._qpos = data.qpos.copy()
         self._sensordata = data.sensordata.copy()
         self._abstraction_to_mujoco_mapping = abstraction_to_mujoco_mapping
+        self._camera_views = camera_views
 
     def get_rigid_body_relative_pose(self, rigid_body: RigidBody) -> Pose:
         """
         Get the pose of a rigid body, relative to its parent multi-body system's reference frame.
 
         :param rigid_body: The rigid body to get the pose for.
         :returns: The relative pose.
@@ -113,7 +117,20 @@
         :returns: The angular rate.
         """
         gyro_id = self._abstraction_to_mujoco_mapping.imu_sensor[
             UUIDKey(imu_sensor)
         ].gyro_id
         angular_rate = self._sensordata[gyro_id : gyro_id + 3]
         return Vector3(angular_rate)
+
+    def get_camera_view(self, camera_sensor: CameraSensor) -> npt.NDArray[np.uint8]:
+        """
+        Get the current view of the camera.
+
+        :param camera_sensor: The camera.
+        :return: The image (RGB).
+        """
+        camera_id = self._abstraction_to_mujoco_mapping.camera_sensor[
+            UUIDKey(camera_sensor)
+        ].camera_id
+        image = self._camera_views[camera_id]
+        return image
```

## revolve2/simulators/mujoco_simulator/textures/__init__.py

```diff
@@ -1,6 +1,7 @@
 """Mujoco specific Textures."""
+
 from ._checker import Checker
 from ._flat import Flat
 from ._gradient import Gradient
 
 __all__ = ["Checker", "Flat", "Gradient"]
```

## Comparing `revolve2_mujoco_simulator-1.0.2.dist-info/METADATA` & `revolve2_mujoco_simulator-1.1.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revolve2-mujoco-simulator
-Version: 1.0.2
+Version: 1.1.1
 Summary: Revolve2: MuJoCo simulator.
 Home-page: https://github.com/ci-group/revolve2
 Author: Aart Stuurman
 Author-email: aartstuurman@hotmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -16,19 +16,19 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Typing :: Typed
 Provides-Extra: dev
 Requires-Dist: dm-control (>=1.0.3,<2.0.0)
 Requires-Dist: mujoco (>=2.2.0,<3.0.0)
 Requires-Dist: mujoco-python-viewer (>=0.1.3,<0.2.0)
 Requires-Dist: opencv-python (>=4.6.0.66,<5.0.0.0)
-Requires-Dist: revolve2-simulation (==1.0.2)
+Requires-Dist: revolve2-simulation (==1.1.1)
 Project-URL: Repository, https://github.com/ci-group/revolve2
 Description-Content-Type: text/markdown
 
-<img  align="right" width="150" height="150"  src="./docs/source/logo.png">
+<img align="right" width="150" height="150"  src="./docs/source/logo_light.png">
 
 # Revolve2
 
 Revolve2 is a collection of Python packages used for researching evolutionary algorithms and modular robotics.
 Its primary features are a modular robot framework, an abstraction layer around physics simulators, and evolutionary algorithms.
 
 **Documentation: [ci-group.github.io/revolve2](https://ci-group.github.io/revolve2)**
```

## Comparing `revolve2_mujoco_simulator-1.0.2.dist-info/RECORD` & `revolve2_mujoco_simulator-1.1.1.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 revolve2/simulators/mujoco_simulator/__init__.py,sha256=KKu1kVyrG86GveMs8QMCQ-3zj2dTBM6z1rTeDRa2Exw,118
-revolve2/simulators/mujoco_simulator/_abstraction_to_mujoco_mapping.py,sha256=reKky2TXlrx--92ZecwC8uyJ1InK4e2CKBEczd4JrE8,1059
+revolve2/simulators/mujoco_simulator/_abstraction_to_mujoco_mapping.py,sha256=JO-7pw5znDwTpD68D4-tr9srBAURHgLxWuL_etYMyLs,1340
 revolve2/simulators/mujoco_simulator/_control_interface_impl.py,sha256=l_ItaWGmR5bNVWIcIbAYQwNZ2ph-sSuFrkP65cJQ4Oc,1598
-revolve2/simulators/mujoco_simulator/_custom_mujoco_viewer.py,sha256=2NaX-4C-ko-wgaRUHm1t_w0Td4hfSGypCqlUM8C_uSs,7618
-revolve2/simulators/mujoco_simulator/_local_simulator.py,sha256=zu8HRZjO69eLXdufjXAXLgAUOLn7rCSecEVrILOLM9w,4551
-revolve2/simulators/mujoco_simulator/_scene_to_model.py,sha256=uPJw9HamV5hdmc5KN6Jca-PvHex4CkQ1XgfVdembgDA,14355
-revolve2/simulators/mujoco_simulator/_simulate_manual_scene.py,sha256=2HG0MqTTRMkbFYP2tiSWRtwxxPqjlu6KjxbWCManpbQ,3134
-revolve2/simulators/mujoco_simulator/_simulate_scene.py,sha256=D6az8N5b8Odshi_Bg1CsueJLJUcTVyj1enTU6r_iIRA,5716
-revolve2/simulators/mujoco_simulator/_simulation_state_impl.py,sha256=UfD1-V-UqCdObuj3s7-y2Dr7VWpZ06zsV4V31ywBYzk,4092
+revolve2/simulators/mujoco_simulator/_custom_mujoco_viewer.py,sha256=3JfrEyPZxq9LarJhPcDeyOSYxUp1lHH_DLJg5uDop9A,8088
+revolve2/simulators/mujoco_simulator/_local_simulator.py,sha256=2BOhtVbsgSTqwzQZW-fF6ABRAgqa-CYt_Ugzxh6-Pn0,4703
+revolve2/simulators/mujoco_simulator/_open_gl_vision.py,sha256=cU2ormlCrKXS8ZKQm6hey5qYGKsMfDyEQwa9E6yVJfM,4220
+revolve2/simulators/mujoco_simulator/_render_backend.py,sha256=XscUnbywbJueXsaLCfjvtykZX0l-8aJwSRFLYDeebjk,162
+revolve2/simulators/mujoco_simulator/_scene_to_model.py,sha256=E25z38KyxEya4fhlrbXeMBgIXgOORFApeoxATn2PrHY,16964
+revolve2/simulators/mujoco_simulator/_simulate_manual_scene.py,sha256=s0C5QezPsTJgzBfPTRlkAB9A0w0oK5T-yBp4TAr3r1w,3314
+revolve2/simulators/mujoco_simulator/_simulate_scene.py,sha256=ETM9uHZYDayhP3rLQOZcLIvhfKiTjt2-TDT4_TaSSv8,6912
+revolve2/simulators/mujoco_simulator/_simulation_state_impl.py,sha256=3m_C9LLlk5fgCP2OtD9r9Rv8NVO1DXbciR8S6jrnejg,4727
 revolve2/simulators/mujoco_simulator/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-revolve2/simulators/mujoco_simulator/textures/__init__.py,sha256=ZosqlIqqjq50eW-2kvLnxIHj-447V3sTmiGcUlEzYR8,161
+revolve2/simulators/mujoco_simulator/textures/__init__.py,sha256=yU3N9CwuuZHeNigXmrxQvsY7ExoBhZHt7p6_-awbiZ0,162
 revolve2/simulators/mujoco_simulator/textures/_checker.py,sha256=gICg92sSTKuKg3wupPQGIMZlshi4rqiPCIj6L301N94,507
 revolve2/simulators/mujoco_simulator/textures/_flat.py,sha256=rZ55XG5sAjvrauKRXW82SPZ70X-qI5SPhyb99ToRdOQ,414
 revolve2/simulators/mujoco_simulator/textures/_gradient.py,sha256=utAbc4U9p0BMJEKNzCuBZJigqZ_d8MMTU8xOytS2sHQ,462
-revolve2_mujoco_simulator-1.0.2.dist-info/METADATA,sha256=K2oOjFHzhSadvDk6EuliiNgAfnDRjBSp4uPKx_4lJnk,3260
-revolve2_mujoco_simulator-1.0.2.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
-revolve2_mujoco_simulator-1.0.2.dist-info/RECORD,,
+revolve2_mujoco_simulator-1.1.1.dist-info/METADATA,sha256=KEhcNYW9-XEeblgoyy95MUpSA4zCdjGi86psWqpQx88,3265
+revolve2_mujoco_simulator-1.1.1.dist-info/WHEEL,sha256=sP946D7jFCHeNz5Iq4fL4Lu-PrWrFsgfLXbbkciIZwg,88
+revolve2_mujoco_simulator-1.1.1.dist-info/RECORD,,
```

