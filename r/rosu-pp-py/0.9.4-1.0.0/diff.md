# Comparing `tmp/rosu_pp_py-0.9.4.tar.gz` & `tmp/rosu_pp_py-1.0.0.tar.gz`

## Comparing `rosu_pp_py-0.9.4.tar` & `rosu_pp_py-1.0.0.tar`

### file list

```diff
@@ -1,18 +1,26 @@
--rw-r--r--   0        0        0      426 1970-01-01 00:00:00.000000 rosu_pp_py-0.9.4/Cargo.toml
--rw-r--r--   0      501       20     3572 2023-02-09 07:22:29.000000 rosu_pp_py-0.9.4/.github/workflows/publish.yml
--rw-r--r--   0      501       20      686 2023-02-09 07:22:29.000000 rosu_pp_py-0.9.4/.gitignore
--rw-r--r--   0      501       20     2802 2023-02-09 07:22:29.000000 rosu_pp_py-0.9.4/CHANGELOG.md
--rw-r--r--   0      501       20     1060 2023-02-09 07:22:29.000000 rosu_pp_py-0.9.4/LICENSE
--rw-r--r--   0      501       20     4228 2023-02-09 07:22:29.000000 rosu_pp_py-0.9.4/README.md
--rw-r--r--   0      501       20      834 2023-02-09 07:22:29.000000 rosu_pp_py-0.9.4/pyproject.toml
--rw-r--r--   0      501       20     9888 2023-02-09 07:22:29.000000 rosu_pp_py-0.9.4/rosu_pp_py.pyi
--rw-r--r--   0      501       20     4467 2023-02-09 07:22:29.000000 rosu_pp_py-0.9.4/src/beatmap.rs
--rw-r--r--   0      501       20     8362 2023-02-09 07:22:29.000000 rosu_pp_py-0.9.4/src/calculator.rs
--rw-r--r--   0      501       20     6817 2023-02-09 07:22:29.000000 rosu_pp_py-0.9.4/src/diff_attrs.rs
--rw-r--r--   0      501       20      624 2023-02-09 07:22:29.000000 rosu_pp_py-0.9.4/src/error.rs
--rw-r--r--   0      501       20      926 2023-02-09 07:22:29.000000 rosu_pp_py-0.9.4/src/lib.rs
--rw-r--r--   0      501       20     2356 2023-02-09 07:22:29.000000 rosu_pp_py-0.9.4/src/map_attrs.rs
--rw-r--r--   0      501       20     4491 2023-02-09 07:22:29.000000 rosu_pp_py-0.9.4/src/perf_attrs.rs
--rw-r--r--   0      501       20     4691 2023-02-09 07:22:29.000000 rosu_pp_py-0.9.4/src/strains.rs
--rw-r--r--   0      501       20     7145 2023-02-09 07:22:29.000000 rosu_pp_py-0.9.4/Cargo.lock
--rw-r--r--   0        0        0     4957 1970-01-01 00:00:00.000000 rosu_pp_py-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0      527 1970-01-01 00:00:00.000000 rosu_pp_py-1.0.0/Cargo.toml
+-rw-r--r--   0     1001      127     6531 2024-04-03 16:50:55.000000 rosu_pp_py-1.0.0/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127      686 2024-04-03 16:50:55.000000 rosu_pp_py-1.0.0/.gitignore
+-rw-r--r--   0     1001      127     3377 2024-04-03 16:50:55.000000 rosu_pp_py-1.0.0/CHANGELOG.md
+-rw-r--r--   0     1001      127     1060 2024-04-03 16:50:55.000000 rosu_pp_py-1.0.0/LICENSE
+-rw-r--r--   0     1001      127     5693 2024-04-03 16:50:55.000000 rosu_pp_py-1.0.0/README.md
+-rw-r--r--   0     1001      127    29489 2024-04-03 16:50:55.000000 rosu_pp_py-1.0.0/rosu_pp_py.pyi
+-rw-r--r--   0     1001      127     7873 2024-04-03 16:50:55.000000 rosu_pp_py-1.0.0/src/attributes/beatmap.rs
+-rw-r--r--   0     1001      127     8228 2024-04-03 16:50:55.000000 rosu_pp_py-1.0.0/src/attributes/difficulty.rs
+-rw-r--r--   0     1001      127       58 2024-04-03 16:50:55.000000 rosu_pp_py-1.0.0/src/attributes/mod.rs
+-rw-r--r--   0     1001      127     3152 2024-04-03 16:50:55.000000 rosu_pp_py-1.0.0/src/attributes/performance.rs
+-rw-r--r--   0     1001      127     5272 2024-04-03 16:50:55.000000 rosu_pp_py-1.0.0/src/beatmap.rs
+-rw-r--r--   0     1001      127     8261 2024-04-03 16:50:55.000000 rosu_pp_py-1.0.0/src/difficulty.rs
+-rw-r--r--   0     1001      127      225 2024-04-03 16:50:55.000000 rosu_pp_py-1.0.0/src/error.rs
+-rw-r--r--   0     1001      127     1006 2024-04-03 16:50:55.000000 rosu_pp_py-1.0.0/src/gradual/difficulty.rs
+-rw-r--r--   0     1001      127       41 2024-04-03 16:50:55.000000 rosu_pp_py-1.0.0/src/gradual/mod.rs
+-rw-r--r--   0     1001      127      940 2024-04-03 16:50:55.000000 rosu_pp_py-1.0.0/src/gradual/performance.rs
+-rw-r--r--   0     1001      127     1574 2024-04-03 16:50:55.000000 rosu_pp_py-1.0.0/src/lib.rs
+-rw-r--r--   0     1001      127     2407 2024-04-03 16:50:55.000000 rosu_pp_py-1.0.0/src/macros.rs
+-rw-r--r--   0     1001      127      975 2024-04-03 16:50:55.000000 rosu_pp_py-1.0.0/src/mode.rs
+-rw-r--r--   0     1001      127    13895 2024-04-03 16:50:55.000000 rosu_pp_py-1.0.0/src/performance.rs
+-rw-r--r--   0     1001      127     4291 2024-04-03 16:50:55.000000 rosu_pp_py-1.0.0/src/score_state.rs
+-rw-r--r--   0     1001      127     2646 2024-04-03 16:50:55.000000 rosu_pp_py-1.0.0/src/strains.rs
+-rw-r--r--   0     1001      127     7807 2024-04-03 16:50:55.000000 rosu_pp_py-1.0.0/Cargo.lock
+-rw-r--r--   0     1001      127      777 2024-04-03 16:50:55.000000 rosu_pp_py-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     6441 1970-01-01 00:00:00.000000 rosu_pp_py-1.0.0/PKG-INFO
```

### Comparing `rosu_pp_py-0.9.4/.gitignore` & `rosu_pp_py-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rosu_pp_py-0.9.4/CHANGELOG.md` & `rosu_pp_py-1.0.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,18 @@
-# v0.9.4 (2023-02-09)
+# v1.0.0 (2024-04-03)
+
+- Updated to [rosu-pp v1.0.0](https://github.com/MaxOhn/rosu-pp/blob/main/CHANGELOG.md#v100-2024-04-02)
+- Breaking changes ahead! There are now multiple different calculators:
+  - `Difficulty` to calculate `DifficultyAttributes`, `Strains`, or create gradual calculators
+  - `Performance` to calculate `PerformanceAttributes`
+  - `BeatmapAttributesBuilder` to calculate `BeatmapAttributes`
+  - `GradualDifficulty` to calculate `DifficultyAttributes` for each hitobject
+  - `GradualPerformance` to calculate `PerformanceAttributes` for each hitresult
+
+## v0.9.4 (2023-02-09)
 
 - Updated to [rosu-pp v0.9.4](https://github.com/MaxOhn/rosu-pp/blob/main/CHANGELOG.md#v094-2023-02-09).
 
 ## v0.9.3 (2023-01-28)
 
 - Updated to [rosu-pp v0.9.3](https://github.com/MaxOhn/rosu-pp/blob/main/CHANGELOG.md#v093-2023-01-28). Only includes some bug fixes.
 - Fixed the hitobjects counts of map attributes on converted maps.
```

### Comparing `rosu_pp_py-0.9.4/LICENSE` & `rosu_pp_py-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rosu_pp_py-0.9.4/src/calculator.rs` & `rosu_pp_py-1.0.0/src/attributes/beatmap.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,276 +1,253 @@
-use std::borrow::Cow;
-
 use pyo3::{
-    exceptions::{PyTypeError, PyValueError},
+    exceptions::PyTypeError,
     pyclass, pymethods,
-    types::PyDict,
-    PyResult,
+    types::{PyAnyMethods, PyDict},
+    Bound, PyRef, PyResult,
 };
-use rosu_pp::{AnyPP, AnyStars, DifficultyAttributes, GameMode};
+use rosu_pp::model::beatmap::{BeatmapAttributes, BeatmapAttributesBuilder, HitWindows};
 
-use crate::{
-    beatmap::PyBeatmap, diff_attrs::PyDifficultyAttributes, error::KwargsError,
-    map_attrs::PyBeatmapAttributes, perf_attrs::PyPerformanceAttributes, strains::PyStrains,
-};
+use crate::{beatmap::PyBeatmap, error::ArgsError, mode::PyGameMode};
 
-#[pyclass(name = "Calculator")]
+#[pyclass(name = "BeatmapAttributesBuilder")]
 #[derive(Default)]
-pub struct PyCalculator {
-    attributes: Option<DifficultyAttributes>,
-    mode: Option<GameMode>,
-    mods: Option<u32>,
-    acc: Option<f64>,
-    n_geki: Option<usize>,
-    n_katu: Option<usize>,
-    n300: Option<usize>,
-    n100: Option<usize>,
-    n50: Option<usize>,
-    n_misses: Option<usize>,
-    combo: Option<usize>,
-    passed_objects: Option<usize>,
+pub struct PyBeatmapAttributesBuilder {
+    mode: Option<PyGameMode>,
+    is_convert: bool,
+    mods: u32,
     clock_rate: Option<f64>,
-}
-
-macro_rules! set_calc {
-    ( $calc:ident, $this:ident: $( $field:ident ,)* ) => {
-        $(
-            if let Some(val) = $this.$field {
-                $calc = $calc.$field(val);
-            }
-        )*
-    };
+    ar: Option<f32>,
+    ar_with_mods: bool,
+    cs: Option<f32>,
+    cs_with_mods: bool,
+    hp: Option<f32>,
+    hp_with_mods: bool,
+    od: Option<f32>,
+    od_with_mods: bool,
 }
 
 #[pymethods]
-impl PyCalculator {
+impl PyBeatmapAttributesBuilder {
     #[new]
     #[pyo3(signature = (**kwargs))]
-    fn new(kwargs: Option<&PyDict>) -> PyResult<Self> {
-        let kwargs = match kwargs {
-            Some(kwargs) => kwargs,
-            None => return Ok(Self::default()),
-        };
-
+    fn new(kwargs: Option<&Bound<'_, PyDict>>) -> PyResult<Self> {
         let mut this = Self::default();
 
-        for (key, value) in kwargs.iter() {
+        let Some(kwargs) = kwargs else {
+            return Ok(this);
+        };
+
+        for (key, value) in kwargs {
             match key.extract()? {
-                "mode" => {
-                    let int = value
-                        .extract::<u8>()
-                        .map_err(|_| PyTypeError::new_err("kwarg 'mode': must be an int"))?;
-
-                    this.mode = match int {
-                        0 => Some(GameMode::Osu),
-                        1 => Some(GameMode::Taiko),
-                        2 => Some(GameMode::Catch),
-                        3 => Some(GameMode::Mania),
-                        _ => return Err(PyValueError::new_err("invalid mode integer")),
-                    }
-                }
-                "mods" => {
-                    this.mods = value
-                        .extract()
-                        .map_err(|_| PyTypeError::new_err("kwarg 'mods': must be an int"))?;
-                }
-                "n300" => {
-                    this.n300 = value
-                        .extract()
-                        .map_err(|_| PyTypeError::new_err("kwarg 'n300': must be an int"))?;
-                }
-                "n100" => {
-                    this.n100 = value
-                        .extract()
-                        .map_err(|_| PyTypeError::new_err("kwarg 'n100': must be an int"))?;
-                }
-                "n50" => {
-                    this.n50 = value
-                        .extract()
-                        .map_err(|_| PyTypeError::new_err("kwarg 'n50': must be an int"))?;
+                "map" => {
+                    let map = value
+                        .extract::<PyRef<'_, PyBeatmap>>()
+                        .map_err(|_| PyTypeError::new_err("kwarg 'map': must be a Beatmap"))?;
+
+                    this.set_map(map);
                 }
-                "n_misses" => {
-                    this.n_misses = value
-                        .extract()
-                        .map_err(|_| PyTypeError::new_err("kwarg 'n_misses': must be an int"))?;
+                "mode" => {
+                    this.mode =
+                        Some(value.extract().map_err(|_| {
+                            PyTypeError::new_err("kwarg 'mode': must be a GameMode")
+                        })?)
                 }
-                "n_geki" => {
-                    this.n_geki = value
+                "is_convert" => {
+                    this.is_convert = value
                         .extract()
-                        .map_err(|_| PyTypeError::new_err("kwarg 'n_geki': must be an int"))?;
+                        .map_err(|_| PyTypeError::new_err("kwarg 'is_convert': must be a bool"))?
                 }
-                "n_katu" => {
-                    this.n_katu = value
+                "mods" => {
+                    this.mods = value
                         .extract()
-                        .map_err(|_| PyTypeError::new_err("kwarg 'n_katu': must be an int"))?;
+                        .map_err(|_| PyTypeError::new_err("kwarg 'mods': must be an int"))?
                 }
-                "acc" | "accuracy" => {
-                    this.acc = value
-                        .extract()
-                        .map_err(|_| PyTypeError::new_err("kwarg 'acc': must be a real number"))?;
+                "clock_rate" => {
+                    this.clock_rate =
+                        Some(value.extract().map_err(|_| {
+                            PyTypeError::new_err("kwarg 'clock_rate': must be a float")
+                        })?)
+                }
+                "ar" => {
+                    this.ar = Some(
+                        value
+                            .extract()
+                            .map_err(|_| PyTypeError::new_err("kwarg 'ar': must be a float"))?,
+                    )
+                }
+                "ar_with_mods" => {
+                    this.ar_with_mods = value
+                        .extract()
+                        .map_err(|_| PyTypeError::new_err("kwarg 'ar_with_mods': must be a bool"))?
+                }
+                "cs" => {
+                    this.cs = Some(
+                        value
+                            .extract()
+                            .map_err(|_| PyTypeError::new_err("kwarg 'cs': must be a float"))?,
+                    )
+                }
+                "cs_with_mods" => {
+                    this.cs_with_mods = value
+                        .extract()
+                        .map_err(|_| PyTypeError::new_err("kwarg 'cs_with_mods': must be a bool"))?
+                }
+                "hp" => {
+                    this.hp = Some(
+                        value
+                            .extract()
+                            .map_err(|_| PyTypeError::new_err("kwarg 'hp': must be a float"))?,
+                    )
+                }
+                "hp_with_mods" => {
+                    this.hp_with_mods = value
+                        .extract()
+                        .map_err(|_| PyTypeError::new_err("kwarg 'hp_with_mods': must be a bool"))?
+                }
+                "od" => {
+                    this.od = Some(
+                        value
+                            .extract()
+                            .map_err(|_| PyTypeError::new_err("kwarg 'od': must be a float"))?,
+                    )
                 }
-                "combo" => {
-                    this.combo = value
+                "od_with_mods" => {
+                    this.od_with_mods = value
                         .extract()
-                        .map_err(|_| PyTypeError::new_err("kwarg 'combo': must be an int"))?;
-                }
-                "passed_objects" => {
-                    this.passed_objects = value.extract().map_err(|_| {
-                        PyTypeError::new_err("kwarg 'passed_objects': must be an int")
-                    })?;
-                }
-                "clock_rate" => {
-                    this.clock_rate = value.extract().map_err(|_| {
-                        PyTypeError::new_err("kwarg 'clock_rate': must be a real number")
-                    })?;
-                }
-                "difficulty" | "attributes" => {
-                    let attrs = value.extract::<PyDifficultyAttributes>().map_err(|_| {
-                        PyTypeError::new_err("kwarg 'difficulty': must be DifficultyAttributes")
-                    })?;
-
-                    this.attributes = Some(attrs.inner);
+                        .map_err(|_| PyTypeError::new_err("kwarg 'od_with_mods': must be a bool"))?
                 }
                 kwarg => {
                     let err = format!(
-                        "unexpected kwarg '{kwarg}': expected 'mode', 'mods', \n\
-                        'n_geki', 'n_katu', 'n300', 'n100', 'n50', 'n_misses', \n\
-                        'acc', 'combo', 'passed_objects', 'clock_rate', or 'difficulty'"
+                        "unexpected kwarg '{kwarg}': expected 'map', 'mode', \n\
+                        'is_convert', 'mods', 'clock_rate', 'ar', 'ar_with_mods', \n\
+                        'cs', 'cs_with_mods', 'hp', 'hp_with_mods', 'od', \n\
+                        or 'od_with_mods'"
                     );
 
-                    return Err(KwargsError::new_err(err));
+                    return Err(ArgsError::new_err(err));
                 }
             }
         }
 
         Ok(this)
     }
 
-    fn set_mods(&mut self, mods: u32) {
-        self.mods = Some(mods);
-    }
+    fn build(&self) -> PyBeatmapAttributes {
+        let mut builder = BeatmapAttributesBuilder::new().mods(self.mods);
 
-    fn set_acc(&mut self, acc: f64) {
-        self.acc = Some(acc);
-    }
+        if let Some(mode) = self.mode {
+            builder = builder.mode(mode.into(), self.is_convert);
+        }
 
-    fn set_n_geki(&mut self, n_geki: usize) {
-        self.n_geki = Some(n_geki);
-    }
+        if let Some(clock_rate) = self.clock_rate {
+            builder = builder.clock_rate(clock_rate);
+        }
 
-    fn set_n_katu(&mut self, n_katu: usize) {
-        self.n_katu = Some(n_katu);
-    }
+        if let Some(ar) = self.ar {
+            builder = builder.ar(ar, self.ar_with_mods);
+        }
 
-    fn set_n300(&mut self, n300: usize) {
-        self.n300 = Some(n300);
-    }
+        if let Some(cs) = self.cs {
+            builder = builder.cs(cs, self.cs_with_mods);
+        }
 
-    fn set_n100(&mut self, n100: usize) {
-        self.n100 = Some(n100);
-    }
+        if let Some(hp) = self.hp {
+            builder = builder.hp(hp, self.hp_with_mods);
+        }
 
-    fn set_n50(&mut self, n50: usize) {
-        self.n50 = Some(n50);
-    }
+        if let Some(od) = self.od {
+            builder = builder.od(od, self.od_with_mods);
+        }
 
-    fn set_n_misses(&mut self, n_misses: usize) {
-        self.n_misses = Some(n_misses);
+        builder.build().into()
     }
 
-    fn set_combo(&mut self, combo: usize) {
-        self.combo = Some(combo);
-    }
+    fn set_map(&mut self, map: PyRef<'_, PyBeatmap>) {
+        let map = &map.inner;
 
-    fn set_passed_objects(&mut self, passed_objects: usize) {
-        self.passed_objects = Some(passed_objects);
+        self.mode = Some(map.mode.into());
+        self.ar = Some(map.ar);
+        self.cs = Some(map.cs);
+        self.hp = Some(map.hp);
+        self.od = Some(map.od);
+        self.is_convert = map.is_convert;
     }
 
-    fn set_clock_rate(&mut self, clock_rate: f64) {
-        self.clock_rate = Some(clock_rate);
+    #[pyo3(signature = (mode, is_convert))]
+    fn set_mode(&mut self, mode: Option<PyGameMode>, is_convert: bool) {
+        self.mode = mode;
+        self.is_convert = is_convert;
     }
 
-    fn set_difficulty(&mut self, difficulty: PyDifficultyAttributes) {
-        self.attributes = Some(difficulty.inner);
+    fn set_mods(&mut self, mods: Option<u32>) {
+        self.mods = mods.unwrap_or(0);
     }
 
-    fn map_attributes(&self, map: &PyBeatmap) -> PyResult<PyBeatmapAttributes> {
-        let (map, mode) = match self.mode {
-            Some(mode) => (map.inner.convert_mode(mode), mode),
-            None => (Cow::Borrowed(&map.inner), map.inner.mode),
-        };
-
-        let mut calc = map.attributes();
-
-        if let Some(mode) = self.mode {
-            calc.mode(mode);
-
-            if map.mode != mode && map.mode == GameMode::Osu {
-                calc.converted(true);
-            }
-        }
-
-        if let Some(mods) = self.mods {
-            calc.mods(mods);
-        }
-
-        if let Some(clock_rate) = self.clock_rate {
-            calc.clock_rate(clock_rate);
-        }
-
-        Ok(PyBeatmapAttributes::new(calc.build(), mode, map.as_ref()))
+    fn set_clock_rate(&mut self, clock_rate: Option<f64>) {
+        self.clock_rate = clock_rate;
     }
 
-    fn difficulty(&self, map: &PyBeatmap) -> PyResult<PyDifficultyAttributes> {
-        let mut calc = AnyStars::new(&map.inner);
-
-        set_calc! { calc, self:
-            mode,
-            mods,
-            passed_objects,
-            clock_rate,
-        };
-
-        Ok(calc.calculate().into())
+    #[pyo3(signature = (ar, ar_with_mods))]
+    fn set_ar(&mut self, ar: Option<f32>, ar_with_mods: bool) {
+        self.ar = ar;
+        self.ar_with_mods = ar_with_mods;
     }
 
-    fn performance(&self, map: &PyBeatmap) -> PyResult<PyPerformanceAttributes> {
-        let mut calc = AnyPP::new(&map.inner);
-
-        set_calc! { calc, self:
-            mode,
-            mods,
-            n_geki,
-            n_katu,
-            n300,
-            n100,
-            n50,
-            n_misses,
-            combo,
-            passed_objects,
-            clock_rate,
-        };
-
-        if let Some(ref attrs) = self.attributes {
-            calc = calc.attributes(attrs.to_owned());
-        }
+    #[pyo3(signature = (cs, cs_with_mods))]
+    fn set_cs(&mut self, cs: Option<f32>, cs_with_mods: bool) {
+        self.cs = cs;
+        self.cs_with_mods = cs_with_mods;
+    }
 
-        if let Some(acc) = self.acc {
-            calc = calc.accuracy(acc);
-        }
+    #[pyo3(signature = (hp, hp_with_mods))]
+    fn set_hp(&mut self, hp: Option<f32>, hp_with_mods: bool) {
+        self.hp = hp;
+        self.hp_with_mods = hp_with_mods;
+    }
 
-        Ok(calc.calculate().into())
+    #[pyo3(signature = (od, od_with_mods))]
+    fn set_od(&mut self, od: Option<f32>, od_with_mods: bool) {
+        self.od = od;
+        self.od_with_mods = od_with_mods;
     }
+}
 
-    fn strains(&self, map: &PyBeatmap) -> PyResult<PyStrains> {
-        let mut calc = AnyStars::new(&map.inner);
+define_class! {
+    #[pyclass(name = "BeatmapAttributes", frozen)]
+    #[derive(Clone)]
+    pub struct PyBeatmapAttributes {
+        pub ar: f64!,
+        pub od: f64!,
+        pub cs: f64!,
+        pub hp: f64!,
+        pub clock_rate: f64!,
+        pub ar_hitwindow: f64!,
+        pub od_hitwindow: f64!,
+    }
+}
 
-        set_calc! { calc, self:
-            mode,
-            mods,
-            passed_objects,
+impl From<BeatmapAttributes> for PyBeatmapAttributes {
+    fn from(attrs: BeatmapAttributes) -> Self {
+        let BeatmapAttributes {
+            ar,
+            od,
+            cs,
+            hp,
             clock_rate,
-        };
-
-        Ok(calc.strains().into())
+            hit_windows:
+                HitWindows {
+                    ar: ar_hitwindow,
+                    od: od_hitwindow,
+                },
+        } = attrs;
+
+        Self {
+            ar,
+            od,
+            cs,
+            hp,
+            clock_rate,
+            ar_hitwindow,
+            od_hitwindow,
+        }
     }
 }
```

### Comparing `rosu_pp_py-0.9.4/Cargo.lock` & `rosu_pp_py-1.0.0/Cargo.lock`

 * *Files 4% similar despite different names*

```diff
@@ -17,18 +17,24 @@
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
+name = "heck"
+version = "0.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
+
+[[package]]
 name = "indoc"
-version = "1.0.6"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05a0bd019339e5d968b37855180087b7b9d512c5046fbd244cf8c95687927d6e"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "libc"
 version = "0.2.126"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "349d5a591cd28b49e1d1037471617a32ddcda5731b99419008085f72d5a53836"
 
@@ -40,17 +46,17 @@
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.8.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d61c719bcfbcf5d62b3a09efa6088de8c54bc0bfcd3ea7ae39fcc186108b8de1"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.13.0"
@@ -77,109 +83,127 @@
  "libc",
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "proc-macro2"
-version = "1.0.40"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd96a1e8ed2596c337f8eae5f24924ec83f5ad5ab21ea8e455d3566c69fbcaf7"
+checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.18.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ccd4149c8c3975099622b4e1962dac27565cf5663b76452c3e2b66e0b6824277"
+checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.18.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cd09fe469834db21ee60e0051030339e5d361293d8cb5ec02facf7fdcf52dbf"
+checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.18.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c427c9a96b9c5b12156dbc11f76b14f49e9aae8905ca783ea87c249044ef137"
+checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.18.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "16b822bbba9d60630a44d2109bc410489bb2f439b33e3a14ddeb8a40b378a7c4"
+checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.18.0"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84ae898104f7c99db06231160770f3e40dad6eb9021daddc0fedfa3e41dff10a"
+checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
 dependencies = [
+ "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.20"
+version = "1.0.35"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3bcdf212e9776fbcb2d23ab029360416bb1706b1aea2d1a5ba002727cbcab804"
+checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.2.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62f25bc4c7e55e0b0b7a1d43fb893f4fa1361d0abe38b9ce4f323c2adfe6ef42"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
+name = "rosu-map"
+version = "0.1.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3c55926c8f0fed1db12fbe96f7a6083a2c4186443dd32532ab34e6902467a4f3"
+
+[[package]]
 name = "rosu-pp"
-version = "0.9.4"
+version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "21a423903b205528da09d7db2f74facc3d5db3e67890e4c78e2c52bf77bcf00f"
+checksum = "26f146c66bed5900ee1fa2b55ef5cc5dd2dbd45e6cac0f7bee5cae535980afbc"
+dependencies = [
+ "rosu-map",
+]
 
 [[package]]
 name = "rosu-pp-py"
-version = "0.9.4"
+version = "1.0.0"
 dependencies = [
  "pyo3",
  "rosu-pp",
 ]
 
 [[package]]
 name = "scopeguard"
@@ -191,17 +215,17 @@
 name = "smallvec"
 version = "1.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2fd0db749597d91ff862fd1d55ea87f7855a744a8425a64695b6fca237d1dad1"
 
 [[package]]
 name = "syn"
-version = "1.0.98"
+version = "2.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c50aef8a904de4c23c788f104b7dddc7d6f79c647c7c8ce4cc8f73eb0ca773dd"
+checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -214,17 +238,17 @@
 name = "unicode-ident"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5bd2fe26506023ed7b5e1e315add59d6f584c621d037f9368fea9cfb988f368c"
 
 [[package]]
 name = "unindent"
-version = "0.1.9"
+version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "52fee519a3e570f7df377a06a1a7775cdbfb7aa460be7e08de2b1f0e69973a44"
+checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "windows-sys"
 version = "0.36.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ea04155a16a59f9eab786fe12a4a450e75cdb175f9e0d80da1e17db09f55b8d2"
 dependencies = [
```

