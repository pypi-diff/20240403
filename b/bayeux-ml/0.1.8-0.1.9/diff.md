# Comparing `tmp/bayeux_ml-0.1.8.tar.gz` & `tmp/bayeux_ml-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bayeux_ml-0.1.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "bayeux_ml-0.1.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `bayeux_ml-0.1.8.tar` & `bayeux_ml-0.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2024-02-14 20:12:12.288185 bayeux_ml-0.1.8/LICENSE
--rw-r--r--   0        0        0     7498 2024-02-14 20:12:12.288185 bayeux_ml-0.1.8/README.md
--rw-r--r--   0        0        0     1250 2024-02-14 20:12:12.288185 bayeux_ml-0.1.8/bayeux/__init__.py
--rw-r--r--   0        0        0      584 2024-02-14 20:12:12.288185 bayeux_ml-0.1.8/bayeux/_src/__init__.py
--rw-r--r--   0        0        0     7107 2024-02-14 20:12:12.288185 bayeux_ml-0.1.8/bayeux/_src/bayeux.py
--rw-r--r--   0        0        0    16707 2024-02-14 20:12:12.288185 bayeux_ml-0.1.8/bayeux/_src/debug.py
--rw-r--r--   0        0        0     2018 2024-02-14 20:12:12.288185 bayeux_ml-0.1.8/bayeux/_src/initialization.py
--rw-r--r--   0        0        0      584 2024-02-14 20:12:12.288185 bayeux_ml-0.1.8/bayeux/_src/mcmc/__init__.py
--rw-r--r--   0        0        0    13205 2024-02-14 20:12:12.288185 bayeux_ml-0.1.8/bayeux/_src/mcmc/blackjax.py
--rw-r--r--   0        0        0     8688 2024-02-14 20:12:12.288185 bayeux_ml-0.1.8/bayeux/_src/mcmc/flowmc.py
--rw-r--r--   0        0        0     4392 2024-02-14 20:12:12.288185 bayeux_ml-0.1.8/bayeux/_src/mcmc/numpyro.py
--rw-r--r--   0        0        0     8771 2024-02-14 20:12:12.288185 bayeux_ml-0.1.8/bayeux/_src/mcmc/tfp.py
--rw-r--r--   0        0        0      584 2024-02-14 20:12:12.288185 bayeux_ml-0.1.8/bayeux/_src/optimize/__init__.py
--rw-r--r--   0        0        0     3370 2024-02-14 20:12:12.288185 bayeux_ml-0.1.8/bayeux/_src/optimize/jaxopt.py
--rw-r--r--   0        0        0     5510 2024-02-14 20:12:12.288185 bayeux_ml-0.1.8/bayeux/_src/optimize/optax.py
--rw-r--r--   0        0        0     3369 2024-02-14 20:12:12.288185 bayeux_ml-0.1.8/bayeux/_src/optimize/optimistix.py
--rw-r--r--   0        0        0     3125 2024-02-14 20:12:12.292184 bayeux_ml-0.1.8/bayeux/_src/optimize/shared.py
--rw-r--r--   0        0        0     4754 2024-02-14 20:12:12.292184 bayeux_ml-0.1.8/bayeux/_src/shared.py
--rw-r--r--   0        0        0      865 2024-02-14 20:12:12.292184 bayeux_ml-0.1.8/bayeux/_src/types.py
--rw-r--r--   0        0        0      584 2024-02-14 20:12:12.292184 bayeux_ml-0.1.8/bayeux/_src/vi/__init__.py
--rw-r--r--   0        0        0     5776 2024-02-14 20:12:12.292184 bayeux_ml-0.1.8/bayeux/_src/vi/tfp.py
--rw-r--r--   0        0        0     2410 2024-02-14 20:12:12.292184 bayeux_ml-0.1.8/bayeux/mcmc/__init__.py
--rw-r--r--   0        0        0     3367 2024-02-14 20:12:12.292184 bayeux_ml-0.1.8/bayeux/optimize/__init__.py
--rw-r--r--   0        0        0      790 2024-02-14 20:12:12.292184 bayeux_ml-0.1.8/bayeux/vi/__init__.py
--rw-r--r--   0        0        0     2612 2024-02-14 20:12:12.296185 bayeux_ml-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     9134 1970-01-01 00:00:00.000000 bayeux_ml-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-02-28 15:25:11.886568 bayeux_ml-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1805 2024-02-28 15:25:11.886568 bayeux_ml-0.1.9/README.md
+-rw-r--r--   0        0        0     1250 2024-02-28 15:25:11.886568 bayeux_ml-0.1.9/bayeux/__init__.py
+-rw-r--r--   0        0        0      584 2024-02-28 15:25:11.886568 bayeux_ml-0.1.9/bayeux/_src/__init__.py
+-rw-r--r--   0        0        0     7242 2024-02-28 15:25:11.886568 bayeux_ml-0.1.9/bayeux/_src/bayeux.py
+-rw-r--r--   0        0        0    16707 2024-02-28 15:25:11.886568 bayeux_ml-0.1.9/bayeux/_src/debug.py
+-rw-r--r--   0        0        0     2018 2024-02-28 15:25:11.886568 bayeux_ml-0.1.9/bayeux/_src/initialization.py
+-rw-r--r--   0        0        0      584 2024-02-28 15:25:11.890569 bayeux_ml-0.1.9/bayeux/_src/mcmc/__init__.py
+-rw-r--r--   0        0        0    12897 2024-02-28 15:25:11.890569 bayeux_ml-0.1.9/bayeux/_src/mcmc/blackjax.py
+-rw-r--r--   0        0        0     8688 2024-02-28 15:25:11.890569 bayeux_ml-0.1.9/bayeux/_src/mcmc/flowmc.py
+-rw-r--r--   0        0        0     4392 2024-02-28 15:25:11.890569 bayeux_ml-0.1.9/bayeux/_src/mcmc/numpyro.py
+-rw-r--r--   0        0        0     8771 2024-02-28 15:25:11.890569 bayeux_ml-0.1.9/bayeux/_src/mcmc/tfp.py
+-rw-r--r--   0        0        0      584 2024-02-28 15:25:11.890569 bayeux_ml-0.1.9/bayeux/_src/optimize/__init__.py
+-rw-r--r--   0        0        0     3370 2024-02-28 15:25:11.890569 bayeux_ml-0.1.9/bayeux/_src/optimize/jaxopt.py
+-rw-r--r--   0        0        0     5510 2024-02-28 15:25:11.890569 bayeux_ml-0.1.9/bayeux/_src/optimize/optax.py
+-rw-r--r--   0        0        0     3369 2024-02-28 15:25:11.890569 bayeux_ml-0.1.9/bayeux/_src/optimize/optimistix.py
+-rw-r--r--   0        0        0     3125 2024-02-28 15:25:11.890569 bayeux_ml-0.1.9/bayeux/_src/optimize/shared.py
+-rw-r--r--   0        0        0     4754 2024-02-28 15:25:11.890569 bayeux_ml-0.1.9/bayeux/_src/shared.py
+-rw-r--r--   0        0        0      865 2024-02-28 15:25:11.890569 bayeux_ml-0.1.9/bayeux/_src/types.py
+-rw-r--r--   0        0        0      584 2024-02-28 15:25:11.890569 bayeux_ml-0.1.9/bayeux/_src/vi/__init__.py
+-rw-r--r--   0        0        0     5776 2024-02-28 15:25:11.890569 bayeux_ml-0.1.9/bayeux/_src/vi/tfp.py
+-rw-r--r--   0        0        0     2410 2024-02-28 15:25:11.890569 bayeux_ml-0.1.9/bayeux/mcmc/__init__.py
+-rw-r--r--   0        0        0     3367 2024-02-28 15:25:11.890569 bayeux_ml-0.1.9/bayeux/optimize/__init__.py
+-rw-r--r--   0        0        0      790 2024-02-28 15:25:11.890569 bayeux_ml-0.1.9/bayeux/vi/__init__.py
+-rw-r--r--   0        0        0     2612 2024-02-28 15:25:11.894569 bayeux_ml-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3441 1970-01-01 00:00:00.000000 bayeux_ml-0.1.9/PKG-INFO
```

### Comparing `bayeux_ml-0.1.8/LICENSE` & `bayeux_ml-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bayeux_ml-0.1.8/bayeux/__init__.py` & `bayeux_ml-0.1.9/bayeux/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """bayeux API."""
 
 # A new PyPI release will be pushed everytime `__version__` is increased
 # When changing this, also update the CHANGELOG.md
-__version__ = '0.1.8'
+__version__ = '0.1.9'
 
 # Note: import <name> as <name> is required for names to be exported.
 # See PEP 484 & https://github.com/google/jax/issues/7570
 # pylint: disable=useless-import-alias
 from bayeux import mcmc as mcmc
 from bayeux import optimize as optimize
 from bayeux._src import debug as debug
```

### Comparing `bayeux_ml-0.1.8/bayeux/_src/__init__.py` & `bayeux_ml-0.1.9/bayeux/_src/__init__.py`

 * *Files identical despite different names*

### Comparing `bayeux_ml-0.1.8/bayeux/_src/bayeux.py` & `bayeux_ml-0.1.9/bayeux/_src/bayeux.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,23 +32,23 @@
     "inverse_log_det_jacobian",
     "initial_state",)
 
 
 class _Namespace:
 
   def __init__(self):
-    self._fns = []
+    self.methods = []
 
   def __repr__(self):
-    return "\n".join(self._fns)
+    return "\n".join(self.methods)
 
   def __setclass__(self, clas, parent):
     kwargs = {k: getattr(parent, k) for k in _REQUIRED_KWARGS}
     setattr(self, clas.name, clas(**kwargs))
-    self._fns.append(clas.name)
+    self.methods.append(clas.name)
 
 
 def is_tfp_bijector(bij):
   return hasattr(bij, "__class__") and bij.__class__.__module__.startswith(
       "tensorflow_probability")
 
 
@@ -96,20 +96,26 @@
                      transform_fn=self.transform_fn,
                      initial_state=self.initial_state,
                      inverse_transform_fn=self.inverse_transform_fn,
                      inverse_log_det_jacobian=self.inverse_log_det_jacobian)
 
   def __repr__(self):
     methods = []
-    for name in self._namespaces:
-      methods.append(name)
-      k = getattr(self, name)
-      methods.append("\t." + "\n\t.".join(str(k).split()))
+    for key, values in self.methods.items():
+      methods.append(key)
+      methods.append("\t." + "\n\t.".join(values))
     return "\n".join(methods)
 
+  @property
+  def methods(self):
+    methods = {}
+    for name in self._namespaces:
+      methods[name] = getattr(self, name).methods
+    return methods
+
   @classmethod
   def from_tfp(cls, pinned_joint_distribution, initial_state=None):
     log_density = pinned_joint_distribution.log_prob
     test_point = pinned_joint_distribution.sample_unpinned(
         seed=jax.random.PRNGKey(0))
     transform_fn = (
         pinned_joint_distribution.experimental_default_event_space_bijector()
```

### Comparing `bayeux_ml-0.1.8/bayeux/_src/debug.py` & `bayeux_ml-0.1.9/bayeux/_src/debug.py`

 * *Files identical despite different names*

### Comparing `bayeux_ml-0.1.8/bayeux/_src/initialization.py` & `bayeux_ml-0.1.9/bayeux/_src/initialization.py`

 * *Files identical despite different names*

### Comparing `bayeux_ml-0.1.8/bayeux/_src/mcmc/__init__.py` & `bayeux_ml-0.1.9/bayeux/_src/mcmc/__init__.py`

 * *Files identical despite different names*

### Comparing `bayeux_ml-0.1.8/bayeux/_src/mcmc/blackjax.py` & `bayeux_ml-0.1.9/bayeux/_src/mcmc/blackjax.py`

 * *Files 6% similar despite different names*

```diff
@@ -145,15 +145,14 @@
   adapt = adapt_fn(**kwarg_dict[adapt_fn])
   (last_state, parameters), _ = adapt.run(
       rng_key=seed, **kwargs,
       **kwarg_dict["adapt.run"])
   return last_state, parameters
 
 
-# TODO(colcarroll): Use blackjax.util.run_inference_algorithm here.
 def _blackjax_inference(
     seed,
     adapt_state,
     adapt_parameters,
     algorithm,
     num_draws,
     kwargs):
@@ -169,32 +168,22 @@
 
   Returns:
   The results of the inference and the adaptation:
     (states, infos), adaptation_parameters
   """
 
   algorithm_kwargs = kwargs[algorithm] | adapt_parameters
-  kernel = algorithm(**algorithm_kwargs).step
-
-  @jax.jit
-  def inference_loop(rng_key):
-
-    def one_step(state, rng_key):
-      state, info = kernel(rng_key, state)
-      return state, (state, info)
-
-    keys = jax.random.split(rng_key, num_draws)
-    _, (states, infos) = jax.lax.scan(one_step, adapt_state, keys)
-
-    return states, infos
-
-  # Functions returned by chees adaptation.
-  adapt_parameters.pop("next_random_arg_fn", None)
-  adapt_parameters.pop("integration_steps_fn", None)
-  return inference_loop(seed), adapt_parameters
+  inference_algorithm = algorithm(**algorithm_kwargs)
+  _, states, infos = blackjax.util.run_inference_algorithm(
+      rng_key=seed,
+      initial_state_or_position=adapt_state,
+      inference_algorithm=inference_algorithm,
+      num_steps=num_draws,
+      progress_bar=False)
+  return states, infos
 
 
 def _blackjax_inference_loop(
     seed,
     init_position,
     adapt_fn,
     algorithm,
@@ -206,15 +195,15 @@
       adapt_seed, adapt_fn, kwarg_dict=kwargs, position=init_position)
   return _blackjax_inference(
       inference_seed,
       adapt_state,
       adapt_parameters,
       algorithm,
       num_draws,
-      kwargs)
+      kwargs), adapt_parameters
 
 
 def _blackjax_stats_to_dict(sample_stats, potential_energy, adapt_parameters):
   """Extract ArviZ compatible stats from blackjax sampler.
 
   Adapted from https://github.com/pymc-devs/pymc
 
@@ -358,15 +347,15 @@
       adapt_parameters=adapt_parameters,
       algorithm=algorithm,
       num_draws=num_draws,
       kwargs=kwargs)
   map_seed = jax.random.split(seed, num_chains)
   mapped_sampler = shared.map_fn(chain_method, sampler)
 
-  (states, stats), adapt_parameters = mapped_sampler(map_seed, adapt_state)
+  states, stats = mapped_sampler(map_seed, adapt_state)
   draws = transform_fn(states.position)
   if extra_parameters["return_pytree"]:
     return draws
   else:
     potential_energy = states.logdensity
     sample_stats = _blackjax_stats_to_dict(
         stats, potential_energy, adapt_parameters)
```

### Comparing `bayeux_ml-0.1.8/bayeux/_src/mcmc/flowmc.py` & `bayeux_ml-0.1.9/bayeux/_src/mcmc/flowmc.py`

 * *Files identical despite different names*

### Comparing `bayeux_ml-0.1.8/bayeux/_src/mcmc/numpyro.py` & `bayeux_ml-0.1.9/bayeux/_src/mcmc/numpyro.py`

 * *Files identical despite different names*

### Comparing `bayeux_ml-0.1.8/bayeux/_src/mcmc/tfp.py` & `bayeux_ml-0.1.9/bayeux/_src/mcmc/tfp.py`

 * *Files identical despite different names*

### Comparing `bayeux_ml-0.1.8/bayeux/_src/optimize/__init__.py` & `bayeux_ml-0.1.9/bayeux/_src/optimize/__init__.py`

 * *Files identical despite different names*

### Comparing `bayeux_ml-0.1.8/bayeux/_src/optimize/jaxopt.py` & `bayeux_ml-0.1.9/bayeux/_src/optimize/jaxopt.py`

 * *Files identical despite different names*

### Comparing `bayeux_ml-0.1.8/bayeux/_src/optimize/optax.py` & `bayeux_ml-0.1.9/bayeux/_src/optimize/optax.py`

 * *Files identical despite different names*

### Comparing `bayeux_ml-0.1.8/bayeux/_src/optimize/optimistix.py` & `bayeux_ml-0.1.9/bayeux/_src/optimize/optimistix.py`

 * *Files identical despite different names*

### Comparing `bayeux_ml-0.1.8/bayeux/_src/optimize/shared.py` & `bayeux_ml-0.1.9/bayeux/_src/optimize/shared.py`

 * *Files identical despite different names*

### Comparing `bayeux_ml-0.1.8/bayeux/_src/shared.py` & `bayeux_ml-0.1.9/bayeux/_src/shared.py`

 * *Files identical despite different names*

### Comparing `bayeux_ml-0.1.8/bayeux/_src/types.py` & `bayeux_ml-0.1.9/bayeux/_src/types.py`

 * *Files identical despite different names*

### Comparing `bayeux_ml-0.1.8/bayeux/_src/vi/__init__.py` & `bayeux_ml-0.1.9/bayeux/_src/vi/__init__.py`

 * *Files identical despite different names*

### Comparing `bayeux_ml-0.1.8/bayeux/_src/vi/tfp.py` & `bayeux_ml-0.1.9/bayeux/_src/vi/tfp.py`

 * *Files identical despite different names*

### Comparing `bayeux_ml-0.1.8/bayeux/mcmc/__init__.py` & `bayeux_ml-0.1.9/bayeux/mcmc/__init__.py`

 * *Files identical despite different names*

### Comparing `bayeux_ml-0.1.8/bayeux/optimize/__init__.py` & `bayeux_ml-0.1.9/bayeux/optimize/__init__.py`

 * *Files identical despite different names*

### Comparing `bayeux_ml-0.1.8/bayeux/vi/__init__.py` & `bayeux_ml-0.1.9/bayeux/vi/__init__.py`

 * *Files identical despite different names*

### Comparing `bayeux_ml-0.1.8/pyproject.toml` & `bayeux_ml-0.1.9/pyproject.toml`

 * *Files identical despite different names*

