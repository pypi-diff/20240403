# Comparing `tmp/exoverses-0.1.1.tar.gz` & `tmp/exoverses-0.2.0.tar.gz`

## Comparing `exoverses-0.1.1.tar` & `exoverses-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 exoverses-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 exoverses-0.1.1/README.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 exoverses-0.1.1/.github/dependabot.yml
--rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 exoverses-0.1.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 exoverses-0.1.1/src/exoverses/__init__.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 exoverses-0.1.1/src/exoverses/base/__init__.py
--rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 exoverses-0.1.1/src/exoverses/base/disk.py
--rw-r--r--   0        0        0    10523 2020-02-02 00:00:00.000000 exoverses-0.1.1/src/exoverses/base/planet.py
--rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 exoverses-0.1.1/src/exoverses/base/star.py
--rw-r--r--   0        0        0    15173 2020-02-02 00:00:00.000000 exoverses-0.1.1/src/exoverses/base/system.py
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 exoverses-0.1.1/src/exoverses/base/universe.py
--rw-r--r--   0        0        0     7537 2020-02-02 00:00:00.000000 exoverses-0.1.1/src/exoverses/data/mamajek_rhk.csv
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 exoverses-0.1.1/src/exoverses/exosims/__init__.py
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 exoverses-0.1.1/src/exoverses/exosims/planet.py
--rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 exoverses-0.1.1/src/exoverses/exosims/star.py
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 exoverses-0.1.1/src/exoverses/exosims/system.py
--rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 exoverses-0.1.1/src/exoverses/exosims/universe.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 exoverses-0.1.1/src/exoverses/exovista/__init__.py
--rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 exoverses-0.1.1/src/exoverses/exovista/disk.py
--rw-r--r--   0        0        0     4868 2020-02-02 00:00:00.000000 exoverses-0.1.1/src/exoverses/exovista/planet.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 exoverses-0.1.1/src/exoverses/exovista/star.py
--rw-r--r--   0        0        0     7598 2020-02-02 00:00:00.000000 exoverses-0.1.1/src/exoverses/exovista/system.py
--rw-r--r--   0        0        0     7554 2020-02-02 00:00:00.000000 exoverses-0.1.1/src/exoverses/exovista/universe.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 exoverses-0.1.1/src/exoverses/fit/__init__.py
--rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 exoverses-0.1.1/src/exoverses/fit/planet.py
--rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 exoverses-0.1.1/src/exoverses/fit/system.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 exoverses-0.1.1/src/exoverses/util/__init__.py
--rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 exoverses-0.1.1/src/exoverses/util/misc.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 exoverses-0.1.1/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 exoverses-0.1.1/LICENSE
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 exoverses-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 exoverses-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 exoverses-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 exoverses-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     4290 2020-02-02 00:00:00.000000 exoverses-0.2.0/README.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 exoverses-0.2.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1143 2020-02-02 00:00:00.000000 exoverses-0.2.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 exoverses-0.2.0/.github/workflows/release-please.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/__init__.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/base/__init__.py
+-rw-r--r--   0        0        0       49 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/base/disk.py
+-rw-r--r--   0        0        0     9844 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/base/planet.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/base/star.py
+-rw-r--r--   0        0        0    15238 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/base/system.py
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/base/universe.py
+-rw-r--r--   0        0        0     7395 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/data/mamajek_rhk.csv
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/exosims/__init__.py
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/exosims/planet.py
+-rw-r--r--   0        0        0     2554 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/exosims/star.py
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/exosims/system.py
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/exosims/universe.py
+-rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/exovista/__init__.py
+-rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/exovista/disk.py
+-rw-r--r--   0        0        0     4868 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/exovista/planet.py
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/exovista/star.py
+-rw-r--r--   0        0        0     7603 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/exovista/system.py
+-rw-r--r--   0        0        0     7554 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/exovista/universe.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/fit/__init__.py
+-rw-r--r--   0        0        0     2644 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/fit/planet.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/fit/system.py
+-rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/util/__init__.py
+-rw-r--r--   0        0        0    11910 2020-02-02 00:00:00.000000 exoverses-0.2.0/src/exoverses/util/misc.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 exoverses-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 exoverses-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 exoverses-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6309 2020-02-02 00:00:00.000000 exoverses-0.2.0/PKG-INFO
```

### Comparing `exoverses-0.1.1/README.md` & `exoverses-0.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -91,8 +91,7 @@
 3   0.006867    686.959991  0.305634     0.0  2450809.4793391167   1.523662  ...  0.865309  0.0  305.87478  2000.0    0.1070   0.532
 4  10.948237   4333.286713  0.219983     0.0  2446990.8777174116   5.203363  ...  1.755036  0.0  293.84823  2000.0  317.8300  11.209
 5   2.448455  10756.199527  0.232703     0.0  2440189.9239725103   9.537070  ...  1.984702  0.0  296.22928  2000.0   95.1600   9.449
 6   0.259398  30707.489457  0.217181     0.0   2423941.940415186  19.191264  ...  1.295556  0.0  239.00230  2000.0   14.5400   4.007
 
 [7 rows x 14 columns]
 ```
-
```

### Comparing `exoverses-0.1.1/src/exoverses/base/planet.py` & `exoverses-0.2.0/src/exoverses/base/planet.py`

 * *Files 11% similar despite different names*

```diff
@@ -225,89 +225,78 @@
 
     def classify_planet(self):
         """
         This determines the Kopparapu bin of the planet This is adapted from
         the EXOSIMS SubtypeCompleteness method classifyPlanets so that EXOSIMS
         isn't a mandatory import
         """
+
+        # # Calculate the luminosity of the star, assuming main-sequence
+        Rp = self.radius.to("earthRad").value
+        #
+        # Find the stellar flux at the planet's location as a fraction of earth's
+        earth_Lp = const.L_sun / (1 * (1 + (0.0167**2) / 2)) ** 2
+        Lp = (
+            (
+                self.star.luminosity
+                / (self.a.to("AU").value * (1 + (self.e**2) / 2)) ** 2
+                / earth_Lp
+            )
+            .decompose()
+            .value
+        )
+
+        # Find Planet Rp range
+        Rp_bins = np.array([0, 0.5, 1.0, 1.75, 3.5, 6.0, 14.3, 11.2 * 4.6])
+        Rp_types = [
+            "Sub-Rocky",
+            "Rocky",
+            "Super-Earth",
+            "Sub-Neptune",
+            "Sub-Jovian",
+            "Jovian",
+            "Super-Jovian",
+        ]
+        L_bins = np.array(
+            [
+                [1000, 182, 1.0, 0.28, 0.0035, 5e-5],
+                [1000, 182, 1.0, 0.28, 0.0035, 5e-5],
+                [1000, 187, 1.12, 0.30, 0.0030, 5e-5],
+                [1000, 188, 1.15, 0.32, 0.0030, 5e-5],
+                [1000, 220, 1.65, 0.45, 0.0030, 5e-5],
+                [1000, 220, 1.65, 0.40, 0.0025, 5e-5],
+                [1000, 220, 1.68, 0.45, 0.0025, 5e-5],
+                [1000, 220, 1.68, 0.45, 0.0025, 5e-5],
+            ]
+        )
+        # Find the bin of the radius
+        Rp_bin = np.digitize(Rp, Rp_bins) - 1
+        Rp_bin = max(0, min(Rp_bin, len(Rp_types) - 1))
+        Rp_type = Rp_types[Rp_bin]
+        # TODO Fix this to give correct when at edge cases since technically
+        # they're not straight lines
+
+        # # index of planet temp. cold,warm,hot
+        L_types = ["Very Hot", "Hot", "Warm", "Cold", "Very Cold"]
+        specific_L_bins = L_bins[Rp_bin, :]
+        L_bin = np.digitize(Lp, specific_L_bins) - 1
+        L_bin = max(0, min(L_bin, len(L_types) - 1))
+        L_type = L_types[L_bin]
+        self.subtype = f"{Rp_type} {L_type}"
+
+        # Determine if the planet is Earth-like
         # Reverse luminosity scaling
         a = self.a.to("AU").value / np.sqrt(self.star.luminosity.to("Lsun").value)
 
         lower_a = 0.95
         upper_a = 1.67
 
         lower_R = 0.8 / np.sqrt(a)
         upper_R = 1.4
         self.is_earth = (lower_a <= a < upper_a) and (
             lower_R <= self.radius.to("earthRad").value < upper_R
         )
 
-        # # Calculate the luminosity of the star, assuming main-sequence
-        # if self.mass < 2 * u.M_sun:
-        #     self.Ls = const.L_sun * (self.star.mass / const.M_sun) ** 4
-        # else:
-        #     self.Ls = 1.4 * const.L_sun * (self.star.mass / const.M_sun) ** 3.5
-        #
-        # Rp = self.radius.to("earthRad").value
-        # # a = self.a.to("AU").value
-        # # e = self.e
-        #
-        # # Find the stellar flux at the planet's location as a fraction of earth's
-        # earth_Lp = const.L_sun / (1 * (1 + (0.0167**2) / 2)) ** 2
-        # self.Lp = (
-        #     self.Ls / (self.a.to("AU").value * (1 + (self.e**2) / 2)) ** 2 / earth_Lp
-        # )
-        #
-        # # Find Planet Rp range
-        # Rp_bins = np.array([0, 0.5, 1.0, 1.75, 3.5, 6.0, 14.3, 11.2 * 4.6])
-        # # Rp_lo = Rp_bins[:-1]
-        # # Rp_hi = Rp_bins[1:]
-        # Rp_types = [
-        #     "Sub-Rocky",
-        #     "Rocky",
-        #     "Super-Earth",
-        #     "Sub-Neptune",
-        #     "Sub-Jovian",
-        #     "Jovian",
-        #     "Super-Jovian",
-        # ]
-        # self.L_bins = np.array(
-        #     [
-        #         [1000, 182, 1.0, 0.28, 0.0035, 5e-5],
-        #         [1000, 182, 1.0, 0.28, 0.0035, 5e-5],
-        #         [1000, 187, 1.12, 0.30, 0.0030, 5e-5],
-        #         [1000, 188, 1.15, 0.32, 0.0030, 5e-5],
-        #         [1000, 220, 1.65, 0.45, 0.0030, 5e-5],
-        #         [1000, 220, 1.65, 0.40, 0.0025, 5e-5],
-        #         [1000, 220, 1.68, 0.45, 0.0025, 5e-5],
-        #         [1000, 220, 1.68, 0.45, 0.0025, 5e-5],
-        #     ]
-        # )
-        # # self.L_bins = np.array(
-        # #     [
-        # #         [1000, 182, 1.0, 0.28, 0.0035, 5e-5],
-        # #         [1000, 187, 1.12, 0.30, 0.0030, 5e-5],
-        # #         [1000, 188, 1.15, 0.32, 0.0030, 5e-5],
-        # #         [1000, 220, 1.65, 0.45, 0.0030, 5e-5],
-        # #         [1000, 220, 1.65, 0.40, 0.0025, 5e-5],
-        # #     ]
-        # # )
-        #
-        # # Find the bin of the radius
-        # self.Rp_bin = np.digitize(Rp, Rp_bins) - 1
-        # try:
-        #     self.Rp_type = Rp_types[self.Rp_bin]
-        # except IndexError:
-        #     print(f"Error handling Rp_type of planet with Rp_bin of {self.Rp_bin}")
-        #     self.Rp_type = None
-        #
-        # # TODO Fix this to give correct when at edge cases since technically
-        # # they're not straight lines
-        #
-        # # index of planet temp. cold,warm,hot
-        # L_types = ["Very Hot", "Hot", "Warm", "Cold", "Very Cold"]
-        # specific_L_bins = self.L_bins[self.Rp_bin, :]
-        # self.L_bin = np.digitize(self.Lp.decompose().value, specific_L_bins) - 1
-        # try:
-        #     self.L_type = L_types[self.L_bin]
-        # except IndexError:
-        #     print(f"Error handling L_type of planet with L_bin of {self.L_bin}")
+        # Determine EXOSIMS phase function information
+        Rp_phase_inds = [0, 2, 2, 7, 7, 4, 4]
+        self.exosims_phiIndex = Rp_phase_inds[Rp_bin]
+        # TODO Inform the geometric albedo from this
```

### Comparing `exoverses-0.1.1/src/exoverses/base/star.py` & `exoverses-0.2.0/src/exoverses/base/star.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.1.1/src/exoverses/base/system.py` & `exoverses-0.2.0/src/exoverses/base/system.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,18 @@
     def __repr__(self):
         return (
             f"{self.star.name}\tdist:{self.star.dist}\t"
             f"Type:{self.star.spectral_type}\n\n"
             f"Planets:\n{self.get_p_df()}"
         )
 
+    @property
+    def name(self):
+        return self.star.name
+
     def planet_cleanup(self):
         self.pInds = np.arange(len(self.planets))
         # Sort the planets in the system by semi-major axis
         a_vals = [planet.a.value for planet in self.planets]
         self.planets = np.array(self.planets)[np.argsort(a_vals)].tolist()
         self.pInds = self.pInds[np.argsort(a_vals)]
```

### Comparing `exoverses-0.1.1/src/exoverses/data/mamajek_rhk.csv` & `exoverses-0.2.0/src/exoverses/data/mamajek_rhk.csv`

 * *Files 2% similar despite different names*

```diff
@@ -98,39 +98,36 @@
 HIP 64924,9.9770006382e-06,-5.0010000000011114
 HIP 68184,1.02565192625e-05,-4.989000000000596
 HIP 69965,1.47910838816e-05,-4.83000000000241
 HIP 70497,4.35511873685e-05,-4.361000000000567
 HIP 71284,3.1117163371e-05,-4.50700000000084
 HIP 71681,1.09622575177e-05,-4.960100000001232
 HIP 71683,8.2375867276e-06,-5.084200000000989
-HIP 72659,3.76703798983e-05,-4.4240000000010475
 HIP 72659,4.33510878387e-05,-4.36300000000053
 HIP 73184,3.28095293113e-05,-4.484000000000157
 HIP 73996,2.917427014e-05,-4.535000000000173
 HIP 75181,1.16949939101e-05,-4.932000000003666
 HIP 77052,1.8197008586e-05,-4.740000000002382
 HIP 77257,9.9083194489e-06,-5.004000000001213
 HIP 77358,1.64816239152e-05,-4.783000000001452
 HIP 77760,9.0782053017e-06,-5.042000000003916
 HIP 78072,1.51356124843e-05,-4.820000000001781
 HIP 78459,9.1411324147e-06,-5.039000000000119
 HIP 79672,1.17489755493e-05,-4.930000000003522
 HIP 80337,3.54813389233e-05,-4.4500000000007045
 HIP 81300,2.61216135439e-05,-4.5830000000015305
-HIP 84405,2.69153480392e-05,-4.570000000001116
 HIP 84405,2.76057785622e-05,-4.559000000000054
 HIP 84478,2.17770977235e-05,-4.66200000000063
 HIP 84720,1.14551294144e-05,-4.941000000002099
 HIP 84862,1.01624869287e-05,-4.993000000000297
 HIP 85235,1.09900583943e-05,-4.959000000000996
 HIP 86486,2.16271852372e-05,-4.66500000000141
 HIP 86736,2.00447202736e-05,-4.698000000001119
 HIP 86796,9.1201083935e-06,-5.040000000002814
 HIP 88601,2.83139199579e-05,-4.548000000001439
-HIP 88601,1.94984459975e-05,-4.710000000001792
 HIP 88694,3.92644935399e-05,-4.406000000000663
 HIP 88972,1.10917481526e-05,-4.95500000000094
 HIP 89042,1.39958732257e-05,-4.854000000000813
 HIP 89348,2.8510182675e-05,-4.545000000000596
 HIP 95447,7.9615935041e-06,-5.099000000003993
 HIP 96100,1.47231250243e-05,-4.832000000000802
 HIP 97295,1.1967405313e-05,-4.922000000002629
```

### Comparing `exoverses-0.1.1/src/exoverses/exosims/planet.py` & `exoverses-0.2.0/src/exoverses/exosims/planet.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.1.1/src/exoverses/exosims/star.py` & `exoverses-0.2.0/src/exoverses/exosims/star.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.1.1/src/exoverses/exosims/system.py` & `exoverses-0.2.0/src/exoverses/exosims/system.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.1.1/src/exoverses/exosims/universe.py` & `exoverses-0.2.0/src/exoverses/exosims/universe.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.1.1/src/exoverses/exovista/disk.py` & `exoverses-0.2.0/src/exoverses/exovista/disk.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.1.1/src/exoverses/exovista/planet.py` & `exoverses-0.2.0/src/exoverses/exovista/planet.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.1.1/src/exoverses/exovista/star.py` & `exoverses-0.2.0/src/exoverses/exovista/star.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.1.1/src/exoverses/exovista/system.py` & `exoverses-0.2.0/src/exoverses/exovista/system.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     Args:
         infile (Path):
             Path to the exoVista fits file
     """
 
     def __init__(self, infile, initial_epoc=2000, convert=False, filter=True):
         self.file = infile
-        self.name = self.file.name
+        self.file_name = self.file.name
 
         # fits file extensions, exoVista hard codes these
         planet_ext = 5
         disk_ext = 2
 
         # Get the number of planets
         with open(infile, "rb") as f:
```

### Comparing `exoverses-0.1.1/src/exoverses/exovista/universe.py` & `exoverses-0.2.0/src/exoverses/exovista/universe.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.1.1/src/exoverses/fit/planet.py` & `exoverses-0.2.0/src/exoverses/fit/planet.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.1.1/src/exoverses/fit/system.py` & `exoverses-0.2.0/src/exoverses/fit/system.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.1.1/src/exoverses/util/misc.py` & `exoverses-0.2.0/src/exoverses/util/misc.py`

 * *Files identical despite different names*

### Comparing `exoverses-0.1.1/.gitignore` & `exoverses-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `exoverses-0.1.1/LICENSE` & `exoverses-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exoverses-0.1.1/pyproject.toml` & `exoverses-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `exoverses-0.1.1/PKG-INFO` & `exoverses-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: exoverses
-Version: 0.1.1
+Version: 0.2.0
 Summary: A unified interface for the various tools that create universes for exoplanet simulations
 Project-URL: Homepage, https://github.com/CoreySpohn/exoverses
 Project-URL: Issues, https://github.com/CoreySpohn/exoverses/issues
 Author-email: Corey Spohn <corey.a.spohn@nasa.gov>
 License: MIT License
         
         Copyright (c) 2023 CoreySpohn
@@ -135,8 +135,7 @@
 3   0.006867    686.959991  0.305634     0.0  2450809.4793391167   1.523662  ...  0.865309  0.0  305.87478  2000.0    0.1070   0.532
 4  10.948237   4333.286713  0.219983     0.0  2446990.8777174116   5.203363  ...  1.755036  0.0  293.84823  2000.0  317.8300  11.209
 5   2.448455  10756.199527  0.232703     0.0  2440189.9239725103   9.537070  ...  1.984702  0.0  296.22928  2000.0   95.1600   9.449
 6   0.259398  30707.489457  0.217181     0.0   2423941.940415186  19.191264  ...  1.295556  0.0  239.00230  2000.0   14.5400   4.007
 
 [7 rows x 14 columns]
 ```
-
```

