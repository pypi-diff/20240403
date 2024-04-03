# Comparing `tmp/exotic-ld-3.0.0.tar.gz` & `tmp/exotic-ld-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exotic-ld-3.0.0.tar", last modified: Wed Dec 14 13:52:44 2022, max compression
+gzip compressed data, was "exotic-ld-3.2.0.tar", last modified: Wed Apr  3 15:35:20 2024, max compression
```

## Comparing `exotic-ld-3.0.0.tar` & `exotic-ld-3.2.0.tar`

### file list

```diff
@@ -1,18 +1,27 @@
-drwxr-xr-x   0 davidgrant   (501) staff       (20)        0 2022-12-14 13:52:44.115157 exotic-ld-3.0.0/
--rw-r--r--   0 davidgrant   (501) staff       (20)     1064 2022-03-11 17:11:52.000000 exotic-ld-3.0.0/LICENSE
--rw-r--r--   0 davidgrant   (501) staff       (20)      747 2022-12-14 13:52:44.114851 exotic-ld-3.0.0/PKG-INFO
--rw-r--r--   0 davidgrant   (501) staff       (20)      895 2022-12-14 13:49:47.000000 exotic-ld-3.0.0/README.rst
-drwxr-xr-x   0 davidgrant   (501) staff       (20)        0 2022-12-14 13:52:44.105712 exotic-ld-3.0.0/exotic_ld/
--rw-r--r--   0 davidgrant   (501) staff       (20)       92 2022-06-21 16:19:12.000000 exotic-ld-3.0.0/exotic_ld/__init__.py
--rwxr-xr-x   0 davidgrant   (501) staff       (20)    25449 2022-12-14 10:27:04.000000 exotic-ld-3.0.0/exotic_ld/ld_computation.py
--rw-r--r--   0 davidgrant   (501) staff       (20)    12339 2022-11-24 13:36:46.000000 exotic-ld-3.0.0/exotic_ld/ld_grids.py
--rw-r--r--   0 davidgrant   (501) staff       (20)      749 2022-11-25 11:59:29.000000 exotic-ld-3.0.0/exotic_ld/ld_laws.py
-drwxr-xr-x   0 davidgrant   (501) staff       (20)        0 2022-12-14 13:52:44.113901 exotic-ld-3.0.0/exotic_ld.egg-info/
--rw-r--r--   0 davidgrant   (501) staff       (20)      747 2022-12-14 13:52:43.000000 exotic-ld-3.0.0/exotic_ld.egg-info/PKG-INFO
--rw-r--r--   0 davidgrant   (501) staff       (20)      312 2022-12-14 13:52:44.000000 exotic-ld-3.0.0/exotic_ld.egg-info/SOURCES.txt
--rw-r--r--   0 davidgrant   (501) staff       (20)        1 2022-12-14 13:52:43.000000 exotic-ld-3.0.0/exotic_ld.egg-info/dependency_links.txt
--rw-r--r--   0 davidgrant   (501) staff       (20)       12 2022-12-14 13:52:43.000000 exotic-ld-3.0.0/exotic_ld.egg-info/requires.txt
--rw-r--r--   0 davidgrant   (501) staff       (20)       10 2022-12-14 13:52:43.000000 exotic-ld-3.0.0/exotic_ld.egg-info/top_level.txt
--rw-r--r--   0 davidgrant   (501) staff       (20)        1 2022-11-28 11:16:28.000000 exotic-ld-3.0.0/exotic_ld.egg-info/zip-safe
--rw-r--r--   0 davidgrant   (501) staff       (20)       38 2022-12-14 13:52:44.115296 exotic-ld-3.0.0/setup.cfg
--rw-r--r--   0 davidgrant   (501) staff       (20)     1011 2022-12-14 13:52:39.000000 exotic-ld-3.0.0/setup.py
+drwxr-xr-x   0 bp21742    (503) staff       (20)        0 2024-04-03 15:35:20.500725 exotic-ld-3.2.0/
+-rw-r--r--   0 bp21742    (503) staff       (20)     1064 2023-04-28 08:31:37.000000 exotic-ld-3.2.0/LICENSE
+-rw-r--r--   0 bp21742    (503) staff       (20)      753 2024-04-03 15:35:20.500366 exotic-ld-3.2.0/PKG-INFO
+-rw-r--r--   0 bp21742    (503) staff       (20)      895 2023-04-28 09:00:26.000000 exotic-ld-3.2.0/README.rst
+drwxr-xr-x   0 bp21742    (503) staff       (20)        0 2024-04-03 15:35:20.459263 exotic-ld-3.2.0/exotic_ld/
+-rw-r--r--   0 bp21742    (503) staff       (20)       92 2023-04-28 08:31:37.000000 exotic-ld-3.2.0/exotic_ld/__init__.py
+-rwxr-xr-x   0 bp21742    (503) staff       (20)    30876 2024-03-21 15:58:30.000000 exotic-ld-3.2.0/exotic_ld/ld_computation.py
+-rw-r--r--   0 bp21742    (503) staff       (20)    11023 2024-03-21 17:12:53.000000 exotic-ld-3.2.0/exotic_ld/ld_grids.py
+-rw-r--r--   0 bp21742    (503) staff       (20)      935 2024-03-20 14:49:56.000000 exotic-ld-3.2.0/exotic_ld/ld_laws.py
+-rw-r--r--   0 bp21742    (503) staff       (20)     1265 2024-02-23 16:26:53.000000 exotic-ld-3.2.0/exotic_ld/ld_requests.py
+drwxr-xr-x   0 bp21742    (503) staff       (20)        0 2024-04-03 15:35:20.470508 exotic-ld-3.2.0/exotic_ld.egg-info/
+-rw-r--r--   0 bp21742    (503) staff       (20)      753 2024-04-03 15:35:20.000000 exotic-ld-3.2.0/exotic_ld.egg-info/PKG-INFO
+-rw-r--r--   0 bp21742    (503) staff       (20)      562 2024-04-03 15:35:20.000000 exotic-ld-3.2.0/exotic_ld.egg-info/SOURCES.txt
+-rw-r--r--   0 bp21742    (503) staff       (20)        1 2024-04-03 15:35:20.000000 exotic-ld-3.2.0/exotic_ld.egg-info/dependency_links.txt
+-rw-r--r--   0 bp21742    (503) staff       (20)       33 2024-04-03 15:35:20.000000 exotic-ld-3.2.0/exotic_ld.egg-info/requires.txt
+-rw-r--r--   0 bp21742    (503) staff       (20)       21 2024-04-03 15:35:20.000000 exotic-ld-3.2.0/exotic_ld.egg-info/top_level.txt
+-rw-r--r--   0 bp21742    (503) staff       (20)        1 2024-02-23 15:07:48.000000 exotic-ld-3.2.0/exotic_ld.egg-info/zip-safe
+drwxr-xr-x   0 bp21742    (503) staff       (20)        0 2024-04-03 15:35:20.434549 exotic-ld-3.2.0/grid_build/
+drwxr-xr-x   0 bp21742    (503) staff       (20)        0 2024-04-03 15:35:20.499902 exotic-ld-3.2.0/grid_build/kd_trees/
+-rw-r--r--   0 bp21742    (503) staff       (20)        0 2023-10-30 13:07:38.000000 exotic-ld-3.2.0/grid_build/kd_trees/__init__.py
+-rw-r--r--   0 bp21742    (503) staff       (20)    40500 2024-02-23 14:55:39.000000 exotic-ld-3.2.0/grid_build/kd_trees/kurucz_tree.pickle
+-rw-r--r--   0 bp21742    (503) staff       (20)  1781265 2024-02-23 14:55:39.000000 exotic-ld-3.2.0/grid_build/kd_trees/mps1_tree.pickle
+-rw-r--r--   0 bp21742    (503) staff       (20)  1781265 2024-02-23 14:55:39.000000 exotic-ld-3.2.0/grid_build/kd_trees/mps2_tree.pickle
+-rw-r--r--   0 bp21742    (503) staff       (20)   270344 2024-02-23 14:55:39.000000 exotic-ld-3.2.0/grid_build/kd_trees/phoenix_tree.pickle
+-rw-r--r--   0 bp21742    (503) staff       (20)     5697 2024-02-23 14:55:40.000000 exotic-ld-3.2.0/grid_build/kd_trees/stagger_tree.pickle
+-rw-r--r--   0 bp21742    (503) staff       (20)       38 2024-04-03 15:35:20.500792 exotic-ld-3.2.0/setup.cfg
+-rw-r--r--   0 bp21742    (503) staff       (20)     1098 2024-03-22 09:30:36.000000 exotic-ld-3.2.0/setup.py
```

### Comparing `exotic-ld-3.0.0/LICENSE` & `exotic-ld-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exotic-ld-3.0.0/README.rst` & `exotic-ld-3.2.0/README.rst`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 .. image:: https://github.com/DavoGrant/ExoTiC-LD/actions/workflows/unittests.yml/badge.svg
    :target: https://github.com/DavoGrant/ExoTiC-LD/actions/workflows/unittests.yml
    
 .. image:: https://readthedocs.org/projects/exotic-ld/badge/?version=latest
    :target: https://exotic-ld.readthedocs.io/en/latest/?badge=latest
    
 .. image:: https://zenodo.org/badge/DOI/10.5281/zenodo.7437681.svg
-   :target: https://doi.org/10.5281/zenodo.7437681
+   :target: https://doi.org/10.5281/zenodo.7874921
 |
 
 ::
 
    pip install exotic-ld
 
 | ExoTiC-LD supports spectroscopic (JWST, HST), photometric (Spitzer, TESS), and custom instrument modes.
```

### Comparing `exotic-ld-3.0.0/exotic_ld/ld_computation.py` & `exotic-ld-3.2.0/exotic_ld/ld_computation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import os
 import numpy as np
 from scipy.optimize import curve_fit
 from scipy.interpolate import interp1d
 from scipy.special import roots_legendre
 
 from exotic_ld.ld_grids import StellarGrids
+from exotic_ld.ld_requests import download
 from exotic_ld.ld_laws import linear_ld_law, quadratic_ld_law, \
-    squareroot_ld_law, nonlinear_3param_ld_law, nonlinear_4param_ld_law
+    squareroot_ld_law, nonlinear_3param_ld_law, nonlinear_4param_ld_law, \
+    kipping_ld_law
 
 
 class StellarLimbDarkening(object):
     """
     Stellar limb darkening class.
 
     Compute the limb-darkening coefficients for a specified
@@ -21,91 +23,106 @@
     M_H : float
         Stellar metallicity [dex].
     Teff : int
         Stellar effective temperature [kelvin].
     logg : float
         Stellar log(g) [dex].
     ld_model : string
-        Choose between 'kurucz', 'stagger', 'mps1', 'mps2', or 'custom'.
+        Choose between 'phoenix', 'kurucz', 'stagger', 'mps1', 'mps2', or 'custom'.
         kurucz are 1D stellar models, can be referenced as '1D'.
         stagger are 3D stellar models, can be referenced as '3D'.
         mps1 are the MPS-ATLAS set 1 models. mps2 are the MPS-ATLAS
         set 2 models. If custom, must also provide custom_wavelengths,
         custom_mus, and custom_stellar_model.
     ld_data_path : string
-        Path to ExoTiC-LD_data directory downloaded from Zenodo. These
-        data include the stellar models and instrument throughputs.
+        Path to exotic-ld-data directory. As of version>=3.2.0 this path
+        specifies where stellar and instrument data are automatically
+        downloaded and stored. Only the required data is downloaded, and
+        if the data has previsouly been used, then no download is required.
+        The directory will be automatically created on the first call.
+        It remains an option, and is backwards compatible, to download
+        all the data from zenodo and specify the path.
     interpolate_type : string
         Choose between 'nearest' and 'trilinear'.
     custom_wavelengths : numpy.ndarray, shape (n,)
         If ld_model='custom', pass the wavelengths of you stellar model
         in angstroms.
     custom_mus : numpy.ndarray, shape (m,)
         If ld_model='custom', pass the mu values at which you stellar
         model is defined.
     custom_stellar_model : numpy.ndarray, shape (n, m)
         If ld_model='custom', pass the specific intensity of your stellar
         for each wavelength and mu value. Note specific intensity must
         be in units of [n_photons / s / cm^2 / Angstrom / steradian].
-    verbose : boolean
-        Print information during calculation. Default: False.
+    ld_data_version : string
+        Version number of the data files. Implemented at 3.2.0, and
+        this corresponds to files with no version number appended.
+        Recommend not changing this from the default value.
+    verbose : int
+        Level of printed information during calculation. Default: 1.
+        0 (no info), 1 (warnings/downloads), 2 (step-by-step info).
 
     Examples
     --------
     >>> from exotic_ld import StellarLimbDarkening
     >>> sld = StellarLimbDarkening(
             M_H=0.1, Teff=6045, logg=4.2, ld_model='mps1',
             ld_data_path='path/to/ExoTiC-LD_data')
     >>> c1, c2 = sld.compute_quadratic_ld_coeffs(
             wavelength_range=np.array([20000., 30000.]),
-            mode='JWST_NIRSpec_prism')
+            mode='JWST_NIRSpec_Prism')
 
     """
 
     def __init__(self, M_H=None, Teff=None, logg=None, ld_model="mps1",
-                 ld_data_path="", interpolate_type="nearest",
+                 ld_data_path="exotic_ld_data", interpolate_type="nearest",
                  custom_wavelengths=None, custom_mus=None,
-                 custom_stellar_model=None, verbose=False):
+                 custom_stellar_model=None, ld_data_version="3.2.0",
+                 verbose=1):
         self.verbose = verbose
 
         # Stellar input parameters.
         self.M_H_input = float(M_H) if M_H is not None else None
         self.Teff_input = int(Teff) if Teff is not None else None
         self.logg_input = float(logg) if logg is not None else None
         self.interpolate_type = interpolate_type
-        if self.verbose:
+        if self.verbose > 1:
             print("Input stellar parameters are M_H={}, Teff={}, logg={}."
                   .format(self.M_H_input, self.Teff_input, self.logg_input))
 
         # Set stellar grid.
         self.ld_data_path = ld_data_path
-        if ld_model == '1D':
-            self.ld_model = 'kurucz'
-        elif ld_model == '3D':
-            self.ld_model = 'stagger'
+        self.remote_ld_data_path = "https://www.star.bris.ac.uk/exotic-ld-data"
+        self.ld_data_version = ld_data_version
+        if self.ld_data_version == "3.2.0":
+            self.ld_data_version = ""  # Ensures backwards compatibility.
+        if ld_model == "1D":
+            self.ld_model = "kurucz"
+        elif ld_model == "3D":
+            self.ld_model = "stagger"
         else:
             self.ld_model = ld_model
 
         # Load/build stellar model.
         self.stellar_wavelengths = None
         self.mus = None
         self.stellar_intensities = None
         self.I_mu = None
         if self.ld_model == "custom":
             self.stellar_wavelengths = custom_wavelengths
             self.mus = custom_mus
             self.stellar_intensities = custom_stellar_model
-            if self.verbose:
+            if self.verbose > 1:
                 print("Using custom stellar model.")
         else:
             self._load_stellar_model()
         self._check_stellar_model()
 
     def __repr__(self):
-        return 'Stellar limb darkening: {} models.'.format(self.ld_model)
+        return "Stellar limb darkening: {} models.".format(self.ld_model)
 
     def compute_linear_ld_coeffs(self, wavelength_range, mode,
                                  custom_wavelengths=None,
                                  custom_throughput=None,
                                  mu_min=0.10, return_sigmas=False):
         """
         Compute the linear limb-darkening coefficients.
@@ -217,14 +234,83 @@
         # Compute I(mu) for a given response function.
         self._integrate_I_mu(wavelength_range, mode,
                              custom_wavelengths, custom_throughput)
 
         # Fit limb-darkening law.
         return self._fit_ld_law(quadratic_ld_law, mu_min, return_sigmas)
 
+    def compute_kipping_ld_coeffs(self, wavelength_range, mode,
+                                  custom_wavelengths=None,
+                                  custom_throughput=None,
+                                  mu_min=0.10, return_sigmas=False):
+        """
+        Compute the Kipping limb-darkening coefficients. These are based on
+        a reparameterisation of the quadratic law as described in
+        Kipping 2013, MNRAS, 435, 2152. See equations 15 -- 18:
+
+        u1 = 2 * q1^0.5 * q2
+        u2 = q1^0.5 * (1 - 2 * q2)
+
+        or,
+
+        q1 = (u1 + u2)^2,
+        q2 = 0.5 * u1 * (u1 + u2)^-1.
+
+        Parameters
+        ----------
+        wavelength_range : array_like, (start, end)
+            Wavelength range over which to compute the limb-darkening
+            coefficients. Wavelengths must be given in angstroms and
+            the values must fall within the supported range of the
+            corresponding instrument mode.
+        mode : string
+            Instrument mode that defines the throughput.
+            Modes supported for Hubble:
+                'HST_STIS_G430L', 'HST_STIS_G750L', 'HST_WFC3_G280p1',
+                'HST_WFC3_G280n1', 'HST_WFC3_G102', 'HST_WFC3_G141'.
+            Modes supported for JWST:
+                'JWST_NIRSpec_Prism', 'JWST_NIRSpec_G395H',
+                'JWST_NIRSpec_G395M', 'JWST_NIRSpec_G235H',
+                'JWST_NIRSpec_G235M', 'JWST_NIRSpec_G140H-f100',
+                'JWST_NIRSpec_G140M-f100', 'JWST_NIRSpec_G140H-f070',
+                'JWST_NIRSpec_G140M-f070', 'JWST_NIRISS_SOSSo1',
+                'JWST_NIRISS_SOSSo2', 'JWST_NIRCam_F322W2',
+                'JWST_NIRCam_F444', 'JWST_MIRI_LRS'.
+            Modes for photometry:
+                'Spitzer_IRAC_Ch1', 'Spitzer_IRAC_Ch2', 'TESS'.
+            Alternatively, use 'custom' mode. In this case the custom
+            wavelength and custom throughput must also be specified.
+        custom_wavelengths : array_like, optional
+            Wavelengths corresponding to custom_throughput [angstroms].
+        custom_throughput : array_like, optional
+            Throughputs corresponding to custom_wavelengths.
+        mu_min : float
+            Minimum value of mu to include in the fitting process.
+        return_sigmas : boolean
+            Return the uncertainties, or standard deviations, of each
+            fitted limb-darkening coefficient. Default: False.
+
+        Returns
+        -------
+        if return_sigmas == False:
+            (c1, c2) : tuple
+                Limb-darkening coefficients for the Kipping law.
+        else:
+            ((c1, c2), (c1_sigma, c2_sigma)) : tuple of tuples
+                Limb-darkening coefficients for the Kipping law
+                and uncertainties on each coefficient.
+
+        """
+        # Compute I(mu) for a given response function.
+        self._integrate_I_mu(wavelength_range, mode,
+                             custom_wavelengths, custom_throughput)
+
+        # Fit limb-darkening law.
+        return self._fit_ld_law(kipping_ld_law, mu_min, return_sigmas)
+
     def compute_squareroot_ld_coeffs(self, wavelength_range, mode,
                                      custom_wavelengths=None,
                                      custom_throughput=None,
                                      mu_min=0.10, return_sigmas=False):
         """
         Compute the square root limb-darkening coefficients.
 
@@ -398,68 +484,76 @@
         self._integrate_I_mu(wavelength_range, mode,
                              custom_wavelengths, custom_throughput)
 
         # Fit limb-darkening law.
         return self._fit_ld_law(nonlinear_4param_ld_law, mu_min, return_sigmas)
 
     def _load_stellar_model(self):
-        if self.verbose:
+        if self.verbose > 1:
             print("Loading stellar model from {} grid.".format(self.ld_model))
 
         sg = StellarGrids(self.M_H_input, self.Teff_input,
-                          self.logg_input, self.ld_model, self.ld_data_path,
-                          self.interpolate_type, self.verbose)
+                          self.logg_input, self.ld_model,
+                          self.ld_data_path, self.remote_ld_data_path,
+                          self.ld_data_version, self.interpolate_type,
+                          self.verbose)
         self.stellar_wavelengths, self.mus, self.stellar_intensities = \
             sg.get_stellar_data()
 
-        if self.verbose:
+        if self.verbose > 1:
             print("Stellar model loaded.")
 
     def _check_stellar_model(self):
         if not self.stellar_intensities.ndim == 2:
-            raise ValueError('Stellar intensities must be 2D, with shape '
-                             '(n wavelengths, n mu values)')
+            raise ValueError("Stellar intensities must be 2D, with shape "
+                             "(n wavelengths, n mu values)")
         if not self.stellar_wavelengths.shape[0] == \
                self.stellar_intensities.shape[0]:
-            raise ValueError('Stellar wavelengths must have the same shape as '
-                             'stellar_intensities.shape[0].')
+            raise ValueError("Stellar wavelengths must have the same shape as "
+                             "stellar_intensities.shape[0].")
         if not self.mus.shape[0] == self.stellar_intensities.shape[1]:
-            raise ValueError('mu values must have the same shape as '
-                             'stellar_intensities.shape[1].')
+            raise ValueError("mu values must have the same shape as "
+                             "stellar_intensities.shape[1].")
 
     def _read_sensitivity_data(self, mode):
-        sensitivity_file_path = os.path.join(
+        local_sensitivity_file_path = os.path.join(
             self.ld_data_path,
-            'Sensitivity_files/{}_throughput.csv'.format(mode))
-        if not os.path.exists(sensitivity_file_path):
-            raise FileNotFoundError(
-                'Sensitivity_file not found mode={} at path={}.'.format(
-                 mode, sensitivity_file_path))
+            "Sensitivity_files/{}_throughput{}.csv".format(mode, self.ld_data_version))
+        remote_sensitivity_file_path = os.path.join(
+            self.remote_ld_data_path,
+            "Sensitivity_files/{}_throughput{}.csv".format(mode, self.ld_data_version))
+
+        # Check if exists locally.
+        if not os.path.exists(local_sensitivity_file_path):
+            download(remote_sensitivity_file_path,
+                     local_sensitivity_file_path, self.verbose)
+            if self.verbose > 1:
+                print("Downloaded {}.".format(local_sensitivity_file_path))
 
-        sensitivity_data = np.loadtxt(sensitivity_file_path,
+        sensitivity_data = np.loadtxt(local_sensitivity_file_path,
                                       skiprows=1, delimiter=",")
         sensitivity_wavelengths = sensitivity_data[:, 0]
         sensitivity_throughputs = sensitivity_data[:, 1]
 
         return sensitivity_wavelengths, sensitivity_throughputs
 
     def _integrate_I_mu(self, wavelength_range, mode, custom_wavelengths,
                         custom_throughput):
-        if mode == 'custom':
+        if mode == "custom":
             # Custom throughput provided.
             s_wavelengths = custom_wavelengths
             s_throughputs = custom_throughput
-            if self.verbose:
+            if self.verbose > 1:
                 print("Using custom instrument throughput with wavelength "
                       "range {}-{} A.".format(s_wavelengths[0],
                                               s_wavelengths[-1]))
         else:
             # Read in mode specific throughput.
             s_wavelengths, s_throughputs = self._read_sensitivity_data(mode)
-            if self.verbose:
+            if self.verbose > 1:
                 print("Loading instrument mode={} with wavelength range "
                       "{}-{} A.".format(mode, s_wavelengths[0],
                                         s_wavelengths[-1]))
 
         # Select wavelength range.
         wavelength_range = np.sort(np.array(wavelength_range))
         s_mask = np.logical_and(wavelength_range[0] < s_wavelengths,
@@ -485,40 +579,40 @@
         s_wvs = s_wavelengths[s_mask]
         s_thp = s_throughputs[s_mask]
         i_wvs = self.stellar_wavelengths[i_mask]
         i_int = self.stellar_intensities[i_mask]
 
         # Ready sensitivity interpolator.
         if s_wvs.shape[0] >= 2:
-            s_interp_func = interp1d(s_wvs, s_thp, kind='linear',
+            s_interp_func = interp1d(s_wvs, s_thp, kind="linear",
                                      bounds_error=False, fill_value=0.)
         else:
             mean_wv = np.mean(wavelength_range)
             match_wv_idx = np.argmin(np.abs(s_wavelengths - mean_wv))
             match_s = s_throughputs[match_wv_idx]
             s_interp_func = lambda _sw: np.ones(_sw.shape) * match_s
 
         # Pre-compute Gauss-legendre roots and rescale to lims.
         roots, weights = roots_legendre(500)
         a = wavelength_range[0]
         b = wavelength_range[1]
         t = (b - a) / 2 * roots + (a + b) / 2
 
-        if self.verbose:
+        if self.verbose > 1:
             print("Integrating I(mu) for wavelength limits of {}-{} A."
                   .format(a, b))
 
         # Iterate mu values computing intensity.
         self.I_mu = np.zeros(i_int.shape[1])
         for mu_idx in range(self.mus.shape[0]):
 
             # Ready intensity interpolator.
             if i_wvs.shape[0] >= 2:
                 i_interp_func = interp1d(
-                    i_wvs, i_int[:, mu_idx], kind='linear',
+                    i_wvs, i_int[:, mu_idx], kind="linear",
                     bounds_error=False, fill_value=0.)
             else:
                 mean_wv = np.mean(wavelength_range)
                 match_wv_idx = np.argmin(np.abs(self.stellar_wavelengths - mean_wv))
                 match_i = self.stellar_intensities[match_wv_idx, mu_idx]
                 i_interp_func = lambda _iw: np.ones(_iw.shape) * match_i
 
@@ -531,35 +625,52 @@
         # Set I(mu=1) = 1.
         if not self.I_mu[0] == 0.:
             self.I_mu /= self.I_mu[0]
         else:
             raise ValueError("Zero intensity in this passband, check your "
                              "wavelength range is correct and in angstroms.")
 
-        if self.verbose:
+        if self.verbose > 1:
             print("Integral done for I(mu).")
 
     def _fit_ld_law(self, ld_law_func, mu_min, return_sigmas):
         # Truncate mu range to be fitted.
         mu_mask = self.mus >= mu_min
 
-        if self.verbose:
-            print("Fitting limb-darkening law to {} I(mu) data points "
-                  "where {} <= mu <= 1.".format(np.sum(mu_mask), mu_min))
-
         if np.sum(mu_mask) < 2:
-            raise ValueError('mu_min={} set too high, must be >= 2 mu '
-                             'values remaining.'.format(mu_min))
+            raise ValueError("mu_min={} set too high, must be >= 2 mu "
+                             "values remaining.".format(mu_min))
 
-        # Fit limb-darkening law: levenberg marquardt, guess default=1.
-        popt, pcov = curve_fit(ld_law_func,
-                               self.mus[mu_mask],
-                               self.I_mu[mu_mask],
-                               method='lm')
+        if not ld_law_func == kipping_ld_law:
+            if self.verbose > 1:
+                print("Fitting limb-darkening law to {} I(mu) data points "
+                      "where {} <= mu <= 1, with the Levenberg-Marquardt "
+                      "algorithm.".format(np.sum(mu_mask), mu_min))
+
+            # Fit limb-darkening law: Levenberg-Marquardt (LM), guess=1.
+            popt, pcov = curve_fit(ld_law_func,
+                                   self.mus[mu_mask],
+                                   self.I_mu[mu_mask],
+                                   method="lm")
+
+        else:
+            if self.verbose > 1:
+                print("Fitting limb-darkening law to {} I(mu) data points "
+                      "where {} <= mu <= 1, with the constrained Trust-Region "
+                      "Reflective algorithm.".format(np.sum(mu_mask), mu_min))
+
+            # Fit limb-darkening law: Trust-Region Reflective (TRF), guess=0.5.
+            # For the Kipping law, constrain q1, q2 to [0, 1].
+            popt, pcov = curve_fit(kipping_ld_law,
+                                   self.mus[mu_mask],
+                                   self.I_mu[mu_mask],
+                                   p0=(0.5, 0.5),
+                                   bounds=((0, 0), (1, 1)),
+                                   method="trf")
 
-        if self.verbose:
+        if self.verbose > 1:
             print("Fit done, resulting coefficients are {}.".format(popt))
 
         if return_sigmas:
             return tuple(popt), tuple(np.sqrt(np.diag(pcov)))
         else:
             return tuple(popt)
```

### Comparing `exotic-ld-3.0.0/exotic_ld/ld_laws.py` & `exotic-ld-3.2.0/exotic_ld/ld_laws.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 
 
 def quadratic_ld_law(mu, u1, u2):
     """ Quadratic limb darkening law. """
     return 1. - u1 * (1. - mu) - u2 * (1. - mu)**2
 
 
+def kipping_ld_law(mu, q1, q2):
+    """ Kipping limb darkening law. """
+    u1 = 2. * q1**0.5 * q2
+    u2 = q1**0.5 * (1. - 2. * q2)
+    return 1. - u1 * (1. - mu) - u2 * (1. - mu)**2
+
+
 def squareroot_ld_law(mu, u1, u2):
     """ Square root limb darkening law. """
     return 1. - u1 * (1. - mu) - u2 * (1. - mu**0.5)
 
 
 def nonlinear_3param_ld_law(mu, u1, u2, u3):
     """ Non-linear 3-parameter limb darkening law. """
```

### Comparing `exotic-ld-3.0.0/setup.py` & `exotic-ld-3.2.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from setuptools import setup
 
 
 setup(
     name='exotic-ld',
-    version='3.0.0',
+    version='3.2.0',
     author='David Grant and Hannah R Wakeford',
     author_email='hannah.wakeford@bristol.ac.uk',
     url='https://github.com/Exo-TiC/ExoTiC-LD',
     license='MIT',
-    packages=['exotic_ld'],
+    packages=['exotic_ld', 'grid_build.kd_trees'],
     description='ExoTiC limb-darkening calculator',
-    long_description='Calculate limb-darkening coefficients for specific '
-                     'instruments, stars, and wavelength ranges.',
+    long_description="Calculate limb-darkening coefficients for specific "
+                     "instruments, stars, and wavelength ranges.",
+    python_requires='>=3.8.0',
+    install_requires=['scipy>=1.8.0', 'numpy', 'requests', 'tqdm'],
     package_data={
-        '': ['README.rst', 'LICENSE']
+        'grid_build.kd_trees': ['*.pickle']
     },
-    install_requires=['numpy', 'scipy'],
     include_package_data=True,
     classifiers=[
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
```

