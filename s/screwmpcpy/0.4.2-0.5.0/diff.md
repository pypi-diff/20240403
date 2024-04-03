# Comparing `tmp/screwmpcpy-0.4.2.tar.gz` & `tmp/screwmpcpy-0.5.0.tar.gz`

## Comparing `screwmpcpy-0.4.2.tar` & `screwmpcpy-0.5.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/.readthedocs.yaml
--rw-r--r--   0        0        0    18294 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/logo.jpg
--rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/noxfile.py
--rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/.github/dependabot.yml
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/.github/workflows/precommit.yml
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/.vscode/extensions.json
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/.vscode/settings.json
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/.vscode/tasks.json
--rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/docs/conf.py
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/docs/index.md
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/docs/api/screwmpcpy.rst
--rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/examples/motiongenerator.py
--rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/examples/panda_screwmotion_ik.py
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/src/screwmpcpy/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/src/screwmpcpy/_version.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/src/screwmpcpy/_version.pyi
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/src/screwmpcpy/basemg.py
--rw-r--r--   0        0        0    10086 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/src/screwmpcpy/dqutil.py
--rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/src/screwmpcpy/mpcutil.py
--rw-r--r--   0        0        0    15167 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/src/screwmpcpy/pandamg.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/src/screwmpcpy/posegen.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/src/screwmpcpy/py.typed
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/src/screwmpcpy/screwintegrator.py
--rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/src/screwmpcpy/screwmpc.py
--rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/tests/test_dqutil.py
--rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/tests/test_mpcutil.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/tests/test_package.py
--rw-r--r--   0        0        0     6004 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/tests/test_pandamg.py
--rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/tests/test_screwintegrator.py
--rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/tests/test_screwmpc_ctrl_signal.py
--rw-r--r--   0        0        0    18967 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/tests/test_screwmpc_matrices.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/.gitignore
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/LICENSE
--rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/README.md
--rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/pyproject.toml
--rw-r--r--   0        0        0     7566 2020-02-02 00:00:00.000000 screwmpcpy-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/.readthedocs.yaml
+-rw-r--r--   0        0        0    18294 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/logo.jpg
+-rw-r--r--   0        0        0     3935 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/noxfile.py
+-rw-r--r--   0        0        0     1054 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/.github/workflows/precommit.yml
+-rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1115 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/.vscode/extensions.json
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/.vscode/settings.json
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/.vscode/tasks.json
+-rw-r--r--   0        0        0      845 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/docs/conf.py
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/docs/index.md
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/docs/api/screwmpcpy.rst
+-rw-r--r--   0        0        0     2329 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/examples/motiongenerator.py
+-rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/examples/panda_screwmotion_ik.py
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/src/screwmpcpy/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/src/screwmpcpy/_version.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/src/screwmpcpy/_version.pyi
+-rw-r--r--   0        0        0     3692 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/src/screwmpcpy/basemg.py
+-rw-r--r--   0        0        0    10086 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/src/screwmpcpy/dqutil.py
+-rw-r--r--   0        0        0     5026 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/src/screwmpcpy/mpcutil.py
+-rw-r--r--   0        0        0    15167 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/src/screwmpcpy/pandamg.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/src/screwmpcpy/posegen.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/src/screwmpcpy/py.typed
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/src/screwmpcpy/screwintegrator.py
+-rw-r--r--   0        0        0     6414 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/src/screwmpcpy/screwmpc.py
+-rw-r--r--   0        0        0     4082 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/tests/test_dqutil.py
+-rw-r--r--   0        0        0     4887 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/tests/test_mpcutil.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/tests/test_package.py
+-rw-r--r--   0        0        0     6235 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/tests/test_pandamg.py
+-rw-r--r--   0        0        0     2258 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/tests/test_screwintegrator.py
+-rw-r--r--   0        0        0     2899 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/tests/test_screwmpc_ctrl_signal.py
+-rw-r--r--   0        0        0    18967 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/tests/test_screwmpc_matrices.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/.gitignore
+-rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3668 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/README.md
+-rw-r--r--   0        0        0     4269 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     7566 2020-02-02 00:00:00.000000 screwmpcpy-0.5.0/PKG-INFO
```

### Comparing `screwmpcpy-0.4.2/.pre-commit-config.yaml` & `screwmpcpy-0.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.4.2/logo.jpg` & `screwmpcpy-0.5.0/logo.jpg`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.4.2/noxfile.py` & `screwmpcpy-0.5.0/noxfile.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.4.2/.devcontainer/devcontainer.json` & `screwmpcpy-0.5.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.4.2/.github/workflows/python-package.yml` & `screwmpcpy-0.5.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.4.2/.github/workflows/python-publish.yml` & `screwmpcpy-0.5.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.4.2/.vscode/tasks.json` & `screwmpcpy-0.5.0/.vscode/tasks.json`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.4.2/docs/conf.py` & `screwmpcpy-0.5.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.4.2/docs/api/screwmpcpy.rst` & `screwmpcpy-0.5.0/docs/api/screwmpcpy.rst`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.4.2/examples/motiongenerator.py` & `screwmpcpy-0.5.0/examples/motiongenerator.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.4.2/examples/panda_screwmotion_ik.py` & `screwmpcpy-0.5.0/examples/panda_screwmotion_ik.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.4.2/src/screwmpcpy/__init__.py` & `screwmpcpy-0.5.0/src/screwmpcpy/__init__.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.4.2/src/screwmpcpy/basemg.py` & `screwmpcpy-0.5.0/src/screwmpcpy/basemg.py`

 * *Files 25% similar despite different names*

```diff
@@ -54,14 +54,20 @@
 
         # setup internal states, matrices and kinematics
         self._mpc_state = np.zeros((18,))
         self._u_state = np.zeros((6,))
         self._sparse_state_transition = scp.sparse.csc_matrix(self.a_matrix)
         self._sparse_ctrl = scp.sparse.csc_matrix(self.b_matrix)
 
+    def reset(self) -> None:
+        """Reset internal states and solver."""
+        self._u_state = np.zeros_like(self._u_state)
+        self._mpc_state = np.zeros_like(self._mpc_state)
+        self._solver = None
+
     def step(self, current_dq: DQ, goal_dq: DQ) -> tuple[DQ, DQ]:
         """Perform one step for motion generation.
 
         :param current_dq: Current pose represented as Dual Quaternion.
         :type current_dq: DQ
         :param goal_dq: Goal pose represented as Dual Quaternion.
         :type goal_dq: DQ
@@ -81,7 +87,25 @@
         # update necessary states
         self._mpc_state = (
             self._sparse_state_transition @ self._mpc_state + self._sparse_ctrl @ du
         )
         self._u_state += du
 
         return error, smooth_traj
+
+    @property
+    def mpc_state(self) -> np.ndarray:
+        r"""Read the mpc state
+
+        :return: :math:`\boldsymbol{s}_{mpc} \in \mathbb{R}^{18}`.
+        :rtype: np.ndarray
+        """
+        return self._mpc_state
+
+    @property
+    def u_state(self) -> np.ndarray:
+        r"""Read current internal twist state
+
+        :return: Current internal twist state :math:`\boldsymbol{u} \in \mathbb{R}^6`.
+        :rtype: np.ndarray
+        """
+        return self._u_state
```

### Comparing `screwmpcpy-0.4.2/src/screwmpcpy/dqutil.py` & `screwmpcpy-0.5.0/src/screwmpcpy/dqutil.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.4.2/src/screwmpcpy/mpcutil.py` & `screwmpcpy-0.5.0/src/screwmpcpy/mpcutil.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.4.2/src/screwmpcpy/pandamg.py` & `screwmpcpy-0.5.0/src/screwmpcpy/pandamg.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.4.2/src/screwmpcpy/posegen.py` & `screwmpcpy-0.5.0/src/screwmpcpy/posegen.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.4.2/src/screwmpcpy/screwintegrator.py` & `screwmpcpy-0.5.0/src/screwmpcpy/screwintegrator.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.4.2/src/screwmpcpy/screwmpc.py` & `screwmpcpy-0.5.0/src/screwmpcpy/screwmpc.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.4.2/tests/test_dqutil.py` & `screwmpcpy-0.5.0/tests/test_dqutil.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.4.2/tests/test_mpcutil.py` & `screwmpcpy-0.5.0/tests/test_mpcutil.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.4.2/tests/test_pandamg.py` & `screwmpcpy-0.5.0/tests/test_pandamg.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,14 +57,22 @@
         [0.173898, 0.667434, 0.782032, -1.86421, 1.44847, 1.57491, 0.889156]
     )
 
     mg = PandaScrewMotionGenerator(Np, Nc, Q, R, vel_bound, acc_bound, jerk_bound)
     dq = mg.step(JOINT_STATE[: JOINT_STATE.shape[0] // 2], goal)
 
     np.testing.assert_almost_equal(dq, JOINT_STATE[JOINT_STATE.shape[0] // 2 :])
+    mg.reset()
+    assert mg._solver is None
+
+    # assert that reset enforces all zeros
+    assert not np.any(mg._mpc_state)
+    assert not np.any(mg._u_state)
+    assert not np.any(mg.mpc_state)
+    assert not np.any(mg.u_state)
 
     error_msg = "Select sclerp between 0 and 1!"
     with pytest.raises(ValueError, match=error_msg):
         PandaScrewMotionGenerator(Np, Nc, Q, R, vel_bound, acc_bound, jerk_bound, -1)
 
 
 def test_panda_manipulability_mg():
```

### Comparing `screwmpcpy-0.4.2/tests/test_screwintegrator.py` & `screwmpcpy-0.5.0/tests/test_screwintegrator.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.4.2/tests/test_screwmpc_ctrl_signal.py` & `screwmpcpy-0.5.0/tests/test_screwmpc_ctrl_signal.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.4.2/tests/test_screwmpc_matrices.py` & `screwmpcpy-0.5.0/tests/test_screwmpc_matrices.py`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.4.2/.gitignore` & `screwmpcpy-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.4.2/LICENSE` & `screwmpcpy-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.4.2/README.md` & `screwmpcpy-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.4.2/pyproject.toml` & `screwmpcpy-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `screwmpcpy-0.4.2/PKG-INFO` & `screwmpcpy-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: screwmpcpy
-Version: 0.4.2
+Version: 0.5.0
 Summary: Dual Quaternion based MPC generating screw motion for n-DOF robot arm.
 Project-URL: Homepage, https://github.com/greinerth/screwmpcpy
 Project-URL: Bug Tracker, https://github.com/greinerth/screwmpcpy/issues
 Project-URL: Discussions, https://github.com/greinerth/screwmpcpy/discussions
 Project-URL: Changelog, https://github.com/greinerth/screwmpcpy/releases
 Author-email: Gerhard Reinerth <g.reinerth@tum.de>
 License: Copyright 2024 Gerhard Reinerth
```

