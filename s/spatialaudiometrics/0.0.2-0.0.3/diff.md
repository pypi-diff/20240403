# Comparing `tmp/spatialaudiometrics-0.0.2.tar.gz` & `tmp/spatialaudiometrics-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spatialaudiometrics-0.0.2.tar", last modified: Fri Mar 22 14:55:11 2024, max compression
+gzip compressed data, was "spatialaudiometrics-0.0.3.tar", last modified: Wed Apr  3 14:12:40 2024, max compression
```

## Comparing `spatialaudiometrics-0.0.2.tar` & `spatialaudiometrics-0.0.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-03-22 14:55:11.192501 spatialaudiometrics-0.0.2/
--rw-rw-rw-   0        0        0    35821 2024-01-23 15:39:56.000000 spatialaudiometrics-0.0.2/LICENSE
--rw-rw-rw-   0        0        0       69 2024-03-22 14:45:33.000000 spatialaudiometrics-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0    43571 2024-03-22 14:55:11.189984 spatialaudiometrics-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1116 2024-03-22 14:54:14.000000 spatialaudiometrics-0.0.2/README.md
--rw-rw-rw-   0        0        0     1142 2024-03-22 14:50:37.000000 spatialaudiometrics-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-22 14:55:11.192501 spatialaudiometrics-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-22 14:55:11.174978 spatialaudiometrics-0.0.2/spatialaudiometrics/
--rw-rw-rw-   0        0        0        0 2024-01-23 11:19:56.000000 spatialaudiometrics-0.0.2/spatialaudiometrics/__init__.py
--rw-rw-rw-   0        0        0     3268 2024-03-22 11:15:48.000000 spatialaudiometrics-0.0.2/spatialaudiometrics/angular_metrics.py
--rw-rw-rw-   0        0        0    59698 2024-01-23 12:23:14.000000 spatialaudiometrics-0.0.2/spatialaudiometrics/example_data_1.csv
--rw-rw-rw-   0        0        0  2835501 2024-03-22 11:15:48.000000 spatialaudiometrics-0.0.2/spatialaudiometrics/example_sofa_1.sofa
--rw-rw-rw-   0        0        0  2969993 2024-03-22 11:15:48.000000 spatialaudiometrics-0.0.2/spatialaudiometrics/example_sofa_2.sofa
--rw-rw-rw-   0        0        0     5954 2024-03-22 11:15:48.000000 spatialaudiometrics-0.0.2/spatialaudiometrics/hrtf_metrics.py
--rw-rw-rw-   0        0        0     1698 2024-03-22 11:15:48.000000 spatialaudiometrics-0.0.2/spatialaudiometrics/lap_challenge.py
--rw-rw-rw-   0        0        0     5777 2024-03-22 14:25:23.000000 spatialaudiometrics-0.0.2/spatialaudiometrics/load_data.py
--rw-rw-rw-   0        0        0     6240 2024-03-22 11:15:48.000000 spatialaudiometrics-0.0.2/spatialaudiometrics/localisation_metrics.py
--rw-rw-rw-   0        0        0     1261 2024-03-22 11:35:28.000000 spatialaudiometrics-0.0.2/spatialaudiometrics/signal_processing.py
--rw-rw-rw-   0        0        0     7462 2024-03-20 09:54:51.000000 spatialaudiometrics-0.0.2/spatialaudiometrics/statistics.py
--rw-rw-rw-   0        0        0     8399 2024-03-22 11:36:12.000000 spatialaudiometrics-0.0.2/spatialaudiometrics/visualisation.py
-drwxrwxrwx   0        0        0        0 2024-03-22 14:55:11.188984 spatialaudiometrics-0.0.2/spatialaudiometrics.egg-info/
--rw-rw-rw-   0        0        0    43571 2024-03-22 14:55:11.000000 spatialaudiometrics-0.0.2/spatialaudiometrics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      710 2024-03-22 14:55:11.000000 spatialaudiometrics-0.0.2/spatialaudiometrics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-22 14:55:11.000000 spatialaudiometrics-0.0.2/spatialaudiometrics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      389 2024-03-22 14:55:11.000000 spatialaudiometrics-0.0.2/spatialaudiometrics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-03-22 14:55:11.000000 spatialaudiometrics-0.0.2/spatialaudiometrics.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 14:12:40.518863 spatialaudiometrics-0.0.3/
+-rw-rw-rw-   0        0        0    35821 2024-03-20 09:59:16.000000 spatialaudiometrics-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0       69 2024-04-03 08:31:29.000000 spatialaudiometrics-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    44001 2024-04-03 14:12:40.517866 spatialaudiometrics-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1116 2024-04-03 08:31:29.000000 spatialaudiometrics-0.0.3/README.md
+-rw-rw-rw-   0        0        0     1417 2024-04-03 14:11:32.000000 spatialaudiometrics-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 14:12:40.518863 spatialaudiometrics-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 14:12:40.504901 spatialaudiometrics-0.0.3/spatialaudiometrics/
+-rw-rw-rw-   0        0        0        0 2024-03-20 09:59:17.000000 spatialaudiometrics-0.0.3/spatialaudiometrics/__init__.py
+-rw-rw-rw-   0        0        0     3268 2024-03-20 09:59:17.000000 spatialaudiometrics-0.0.3/spatialaudiometrics/angular_metrics.py
+-rw-rw-rw-   0        0        0    60165 2024-03-20 09:59:17.000000 spatialaudiometrics-0.0.3/spatialaudiometrics/example_data_1.csv
+-rw-rw-rw-   0        0        0  2833739 2023-10-23 10:30:19.000000 spatialaudiometrics-0.0.3/spatialaudiometrics/example_sofa_1.sofa
+-rw-rw-rw-   0        0        0  2838236 2023-11-07 09:18:47.000000 spatialaudiometrics-0.0.3/spatialaudiometrics/example_sofa_2.sofa
+-rw-rw-rw-   0        0        0     6024 2024-04-03 11:37:57.000000 spatialaudiometrics-0.0.3/spatialaudiometrics/hrtf_metrics.py
+-rw-rw-rw-   0        0        0     2182 2024-04-03 09:09:17.000000 spatialaudiometrics-0.0.3/spatialaudiometrics/lap_challenge.py
+-rw-rw-rw-   0        0        0     5922 2024-04-03 08:54:17.000000 spatialaudiometrics-0.0.3/spatialaudiometrics/load_data.py
+-rw-rw-rw-   0        0        0     6240 2024-03-20 10:48:46.000000 spatialaudiometrics-0.0.3/spatialaudiometrics/localisation_metrics.py
+-rw-rw-rw-   0        0        0     1401 2024-04-03 09:01:23.000000 spatialaudiometrics-0.0.3/spatialaudiometrics/signal_processing.py
+-rw-rw-rw-   0        0        0     7462 2024-03-20 09:59:17.000000 spatialaudiometrics-0.0.3/spatialaudiometrics/statistics.py
+-rw-rw-rw-   0        0        0    13819 2024-04-03 14:01:00.000000 spatialaudiometrics-0.0.3/spatialaudiometrics/visualisation.py
+drwxrwxrwx   0        0        0        0 2024-04-03 14:12:40.515871 spatialaudiometrics-0.0.3/spatialaudiometrics.egg-info/
+-rw-rw-rw-   0        0        0    44001 2024-04-03 14:12:40.000000 spatialaudiometrics-0.0.3/spatialaudiometrics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      710 2024-04-03 14:12:40.000000 spatialaudiometrics-0.0.3/spatialaudiometrics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 14:12:40.000000 spatialaudiometrics-0.0.3/spatialaudiometrics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      611 2024-04-03 14:12:40.000000 spatialaudiometrics-0.0.3/spatialaudiometrics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-04-03 14:12:40.000000 spatialaudiometrics-0.0.3/spatialaudiometrics.egg-info/top_level.txt
```

### Comparing `spatialaudiometrics-0.0.2/LICENSE` & `spatialaudiometrics-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spatialaudiometrics-0.0.2/PKG-INFO` & `spatialaudiometrics-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialaudiometrics
-Version: 0.0.2
+Version: 0.0.3
 Summary: For calculating spatial audio metrics
 Author-email: "Katarina C. Poole" <katarina.poole@imperial.ac.uk>
 Maintainer-email: "Katarina C. Poole" <katarina.poole@imperial.ac.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -678,37 +678,50 @@
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 Project-URL: url, https://github.com/Katarina-Poole/Spatial-Audio-Metrics
 Keywords: spatial,audio,localisation,perception,psychoacoustic,psychophysics,hrtf,hrtfs
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: alabaster>=0.7.16
+Requires-Dist: Babel>=2.14.0
 Requires-Dist: certifi>=2024.2.2
 Requires-Dist: cftime>=1.6.3
+Requires-Dist: charset-normalizer>=3.3.2
+Requires-Dist: colorama>=0.4.6
 Requires-Dist: contourpy>=1.2.0
 Requires-Dist: cycler>=0.12.1
+Requires-Dist: docutils>=0.20.1
 Requires-Dist: fonttools>=4.50.0
+Requires-Dist: idna>=3.6
+Requires-Dist: imagesize>=1.4.1
+Requires-Dist: Jinja2>=3.1.3
 Requires-Dist: kiwisolver>=1.4.5
+Requires-Dist: MarkupSafe>=2.1.5
 Requires-Dist: matplotlib>=3.8.3
 Requires-Dist: netCDF4>=1.6.5
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: packaging>=24.0
 Requires-Dist: pandas>=2.2.1
 Requires-Dist: patsy>=0.5.6
 Requires-Dist: pillow>=10.2.0
+Requires-Dist: Pygments>=2.17.2
 Requires-Dist: pyparsing>=3.1.2
 Requires-Dist: pysofaconventions>=0.1.5
 Requires-Dist: python-dateutil>=2.9.0.post0
 Requires-Dist: pytz>=2024.1
+Requires-Dist: requests>=2.31.0
 Requires-Dist: scikit-posthocs>=0.9.0
 Requires-Dist: scipy>=1.12.0
 Requires-Dist: seaborn>=0.13.2
 Requires-Dist: six>=1.16.0
+Requires-Dist: snowballstemmer>=2.2.0
 Requires-Dist: statsmodels>=0.14.1
 Requires-Dist: tzdata>=2024.1
+Requires-Dist: urllib3>=2.2.1
 
 # Spatial-Audio-Metrics
 Spatial Audio Metrics (SAM) is a Python toolbox to analyse spatial audio and spatial audio perceptual experiments.
 It is still underdevelopment so more functionality will be added
 
 # Documentation
 Detailed coumentation of the Spatial Audio Metrics can be found here: <https://spatial-audio-metrics.readthedocs.io>
```

### Comparing `spatialaudiometrics-0.0.2/README.md` & `spatialaudiometrics-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `spatialaudiometrics-0.0.2/spatialaudiometrics/angular_metrics.py` & `spatialaudiometrics-0.0.3/spatialaudiometrics/angular_metrics.py`

 * *Files identical despite different names*

### Comparing `spatialaudiometrics-0.0.2/spatialaudiometrics/hrtf_metrics.py` & `spatialaudiometrics-0.0.3/spatialaudiometrics/hrtf_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import numpy as np
 import scipy.signal as sn
 from spatialaudiometrics import signal_processing as sp
 
 def hrir2hrtf(hrir:np.array,fs,db_flag = 1):
     '''
     Converts all hrirs in a 3D array (location x ear x sample) into hrtfs. 
+    
     :param hrir: HRIRs in a 3D array (location x ear x sample)
     :param fs: sample rate
     :param db_flag: if you want the spectra in dB rather than magnitude
     :return hrtfs: head related transfer functions (location x ear x sample)
     :return freqs: frequencies of the transfer function (length of hrtf)
     :return hrtfs_phase: phase information (location x ear x sample)
     '''
@@ -38,25 +39,27 @@
     '''
     lsd = 20*np.log10(tf1/tf2)
     return lsd
 
 def calculate_lsd_across_freqs(tf1:np.array,tf2:np.array):
     '''
     Calculates the log spectral distortion across frequencies between two transfer functions tf1 and tf2
+    
     :param tf1: First transfer function 
     :param tf2: Second transfer function to compare against the first
     :return lsd: Return a value that is the RMS across frequencies
     '''
     lsd = calculate_lsd(tf1,tf2)
     lsd = np.sqrt(np.mean(lsd**2))
     return lsd 
 
 def calculate_lsd_across_locations(hrir1,hrir2,fs):
     '''
     Calculates the log spectral distortion across locations between two location matched hrirs only between 20 and 20000Hz
+    
     :param hrir1: 3d array of the impulse response at each location x ear. Shape should be locations x ears x samples
     :param hrir2: 3d array of another impulse response at each location x ear. Shape should be locations x ears x samples
     :param fs: sample rate
     :param lsd: the mean lsd of across ears and locations
     :param lsd_mat: the lsd at each ear x location.
     '''
     if np.shape(hrir1)[2] != np.shape(hrir2)[2]:
@@ -70,63 +73,66 @@
     hrtfs2  = hrtfs2[:,:,idx]
     
     lsd_mat = np.empty(np.shape(hrir1)[0:2])
     for l,loc in enumerate(hrtfs1):
         for e,ear in enumerate(loc):
             lsd_mat[l,e] = calculate_lsd_across_freqs(hrtfs1[l,e,:],hrtfs2[l,e,:])
     
-    lsd = np.mean(lsd_mat)  
+    lsd = np.mean(lsd_mat)
     return lsd,lsd_mat
 
-    
 def itd_estimator_maxiacce(hrir,fs):
     '''
-    Calculates the ITD based on the MAXIACCe mode (transcribed from the itd_estimator in the AMTtoolbox 20/03/24)
+    Calculates the ITD based on the MAXIACCe mode (transcribed from the itd_estimator in the AMTtoolbox 20/03/24, based on Andreopoulou et al. 2017)
+    
     :param hrir: 3d array of the impulse response at each location x ear. Shape should be locations x ears x samples
     :return itd_s: ITD in seconds for each location
     :return itd_samps: ITD in samples for each location
     :return maxiacc: The max interaural cross correlation calculated 
     '''
-    itd_samps = list()
-    maxiacc      = list()
+    itd_samps   = list()
+    maxiacc     = list()
     for loc in hrir:
         # Take the maximum absolute value of the cross correlation between the two ears to get the maxiacc
         correlation     = sn.correlate(np.abs(sn.hilbert(loc[0,:])),np.abs(sn.hilbert(loc[1,:])))
         maxiacc.append(np.max(np.abs(correlation)))
         idx_lag         = np.argmax(np.abs(correlation))
         itd_samps.append(idx_lag - np.shape(hrir)[2])
     itd_s = itd_samps/fs
     
     return itd_s,itd_samps,maxiacc
 
 def ild_estimator_rms(hrir):
     '''
     Calculate the ILD by taking the rms of the impulse response at each ear and taking the difference
+    
     :paran hrir: 3d array of the impulse response at each location x ear. Shape should be locations x ears x samples
     :return ild: ILD in dB for each location
     '''
     rms = np.sqrt(np.mean(hrir**2,axis = 2))
     ild = sp.mag2db(rms[:,0]) - sp.mag2db(rms[:,1])
     return ild
 
 def calculate_itd_difference(hrtf1,hrtf2):
     '''
     Calculates the absolute difference in itd values between two hrtfs
+    
     :param hrtf1: first hrtf (custom hrtf object)
     :param hrtf2: second hrtf (custom hrtf object)
     :return itd_diff: the average itd difference across locations in us 
     '''
     itd_s1,itd_samps,maxiacc = itd_estimator_maxiacce(hrtf1.hrir,hrtf1.fs)
     itd_s2,itd_samps,maxiacc = itd_estimator_maxiacce(hrtf2.hrir,hrtf2.fs)
     itd_diff = np.mean(np.abs(itd_s1-itd_s2)) * 1000000
     return itd_diff
 
 def calculate_ild_difference(hrtf1,hrtf2):
     '''
     Calculates the absolute difference in ild values between two hrtfs
+    
     :param hrtf1: first hrtf (custom hrtf object)
     :param hrtf2: second hrtf (custom hrtf object)
     :return ild_diff: the average ild difference across locations in dB 
     '''
     ild1        = ild_estimator_rms(hrtf1.hrir)
     ild2        = ild_estimator_rms(hrtf2.hrir)
     ild_diff    = np.mean(np.abs(ild1-ild2))
```

### Comparing `spatialaudiometrics-0.0.2/spatialaudiometrics/lap_challenge.py` & `spatialaudiometrics-0.0.3/spatialaudiometrics/lap_challenge.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,23 +3,29 @@
 '''
 import pandas as pd
 from spatialaudiometrics import load_data as ld
 from spatialaudiometrics import hrtf_metrics as hf
 
 class Parameters:
     '''
-    Parameters derived from a dataset
+    Parameters derived from A. Hoggs dataset
     '''
-    itd_threshold = 32
-    ild_threshold = 4
-    lsd_threshold = 7
+    itd_threshold = 31.6
+    ild_threshold = 4.37
+    lsd_threshold = 7.36
     
-def calculate_lap_challenge_metrics(original_hrtf_path,upsampled_hrtf_path):
+def calculate_task_two_metrics(original_hrtf_path,upsampled_hrtf_path):
     '''
     Function that calculates all the metrics for the lab challenge
+    
+    :param original_hrtf_path: full path of the original sofa file
+    :param upsampled_hrtf_path: full path of the upsampled sofa file
+    :return metrics: a list of the itd difference, ild difference and lsd calculated metrics
+    :return threshold_bool: a list of the booleans saying whether the metric is below (True) or above (False) the LAP challenge thresholds
+    :return df: a pandas dataframe including the metrics, threshold_bool and thresholds themselves
     '''
     # Load in the sofa files
     hrtf1 = ld.HRTF(original_hrtf_path)
     hrtf2 = ld.HRTF(upsampled_hrtf_path)
     
     # Match the locations
     hrtf1,hrtf2 = ld.match_hrtf_locations(hrtf1,hrtf2)
@@ -38,9 +44,8 @@
     
     # dictionary of lists 
     dict = {'Metric name': metric_names,'Calculated value': metrics, 'Threshold value':thresholds,'Below threshold?': threshold_bool} 
     df = pd.DataFrame(dict)
     print('Comparison metric table of ' + original_hrtf_path + ' and ' + upsampled_hrtf_path)
     print(df)
     
-    return metrics,threshold_bool,df
-
+    return metrics,threshold_bool,df
```

### Comparing `spatialaudiometrics-0.0.2/spatialaudiometrics/load_data.py` & `spatialaudiometrics-0.0.3/spatialaudiometrics/load_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 '''
 Load data module
 '''
+import os
 import sys
 from importlib import resources
 from pysofaconventions import SOFAFile
 import numpy as np
 import pandas as pd
 from spatialaudiometrics import angular_metrics as am
 from spatialaudiometrics import localisation_metrics as lm
@@ -15,17 +16,20 @@
     '''
     def __init__(self,sofa_path):
         '''
         Loads in the data from the sofa path into the custom class
 
         :param sofa: sofa object from SOFAFile(sofa_path,'r')
         '''
+        # Firstly check if each path exists
+        assert os.path.isfile(sofa_path) is True, 'Sofa file does not exist'
+        
         sofa            = SOFAFile(sofa_path,'r')
         self.sofa_path  = sofa_path
-        self.locs       = np.round(sofa.getVariableValue('SourcePosition'),2) # Round to avoid any bizarre precision errors
+        self.locs       = np.round(sofa.getVariableValue('SourcePosition').data,2) # Round to avoid any bizarre precision errors
         self.hrir       = sofa.getDataIR().data
         self.fs         = sofa.getSamplingRate().data[0]
 
 def load_example_behavioural_data():
     '''
     Loads in example data from a spatial audio experiment (example_data_1.csv)
     '''
@@ -122,9 +126,8 @@
     df['signed_lateral_error']   = df.signed_lateral_error.apply(am.wrap_angle)
     df['signed_polar_error']     = df.signed_polar_error.apply(am.wrap_angle)
     
     # Calculate the unsigned version
     df['unsigned_lateral_error'] = abs(df.signed_lateral_error)
     df['unsigned_polar_error']   = abs(df.signed_polar_error)
 
-    return df
-
+    return df
```

### Comparing `spatialaudiometrics-0.0.2/spatialaudiometrics/localisation_metrics.py` & `spatialaudiometrics-0.0.3/spatialaudiometrics/localisation_metrics.py`

 * *Files identical despite different names*

### Comparing `spatialaudiometrics-0.0.2/spatialaudiometrics/signal_processing.py` & `spatialaudiometrics-0.0.3/spatialaudiometrics/signal_processing.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 '''
-signal_processing.py. Functions that calculate metrics to numerically analyse differences between hrtfs
+signal_processing.py. Generic signal processing functions
 '''
 import numpy as np
 from scipy.fft import fft, fftfreq
 
 def mag2db(x):
     '''
     Convert values from magnitude to dB using 20log10
     
     :param x: float value
     :returns y: float value (dB)
     '''
     y = 20*np.log10(x)
     return y
 
+def db2mag(x):
+    '''
+    Convert values from dB to magnitude
+    
+    :param x: float value (dB)
+    :returns y: float value 
+    '''
+    y = np.float_power(10,x/20)
+    return y
+
 def calculate_spectrum(x:np.array,fs,db_flag = 1):
     '''
     Converts a time domain signal (such as an impulse reponse) to the frequency domain (such as a transfer function). The default is to return the output in dB
     
     :param x: 1D numpy array
     :param fs: sample rate of the signal (e.g. 48000)
     :param db_flag: if you want the spectra in dB rather than magnitude
@@ -33,8 +43,7 @@
     phase   = np.imag(y[0:n//2])
     db      = mag2db(amp)
     if db_flag == 1:
         spec = db
     else:
         spec = amp
     return spec, freqs, phase
-
```

### Comparing `spatialaudiometrics-0.0.2/spatialaudiometrics/statistics.py` & `spatialaudiometrics-0.0.3/spatialaudiometrics/statistics.py`

 * *Files identical despite different names*

### Comparing `spatialaudiometrics-0.0.2/spatialaudiometrics.egg-info/PKG-INFO` & `spatialaudiometrics-0.0.3/spatialaudiometrics.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spatialaudiometrics
-Version: 0.0.2
+Version: 0.0.3
 Summary: For calculating spatial audio metrics
 Author-email: "Katarina C. Poole" <katarina.poole@imperial.ac.uk>
 Maintainer-email: "Katarina C. Poole" <katarina.poole@imperial.ac.uk>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -678,37 +678,50 @@
         the library.  If this is what you want to do, use the GNU Lesser General
         Public License instead of this License.  But first, please read
         <https://www.gnu.org/licenses/why-not-lgpl.html>.
 Project-URL: url, https://github.com/Katarina-Poole/Spatial-Audio-Metrics
 Keywords: spatial,audio,localisation,perception,psychoacoustic,psychophysics,hrtf,hrtfs
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: alabaster>=0.7.16
+Requires-Dist: Babel>=2.14.0
 Requires-Dist: certifi>=2024.2.2
 Requires-Dist: cftime>=1.6.3
+Requires-Dist: charset-normalizer>=3.3.2
+Requires-Dist: colorama>=0.4.6
 Requires-Dist: contourpy>=1.2.0
 Requires-Dist: cycler>=0.12.1
+Requires-Dist: docutils>=0.20.1
 Requires-Dist: fonttools>=4.50.0
+Requires-Dist: idna>=3.6
+Requires-Dist: imagesize>=1.4.1
+Requires-Dist: Jinja2>=3.1.3
 Requires-Dist: kiwisolver>=1.4.5
+Requires-Dist: MarkupSafe>=2.1.5
 Requires-Dist: matplotlib>=3.8.3
 Requires-Dist: netCDF4>=1.6.5
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: packaging>=24.0
 Requires-Dist: pandas>=2.2.1
 Requires-Dist: patsy>=0.5.6
 Requires-Dist: pillow>=10.2.0
+Requires-Dist: Pygments>=2.17.2
 Requires-Dist: pyparsing>=3.1.2
 Requires-Dist: pysofaconventions>=0.1.5
 Requires-Dist: python-dateutil>=2.9.0.post0
 Requires-Dist: pytz>=2024.1
+Requires-Dist: requests>=2.31.0
 Requires-Dist: scikit-posthocs>=0.9.0
 Requires-Dist: scipy>=1.12.0
 Requires-Dist: seaborn>=0.13.2
 Requires-Dist: six>=1.16.0
+Requires-Dist: snowballstemmer>=2.2.0
 Requires-Dist: statsmodels>=0.14.1
 Requires-Dist: tzdata>=2024.1
+Requires-Dist: urllib3>=2.2.1
 
 # Spatial-Audio-Metrics
 Spatial Audio Metrics (SAM) is a Python toolbox to analyse spatial audio and spatial audio perceptual experiments.
 It is still underdevelopment so more functionality will be added
 
 # Documentation
 Detailed coumentation of the Spatial Audio Metrics can be found here: <https://spatial-audio-metrics.readthedocs.io>
```

### Comparing `spatialaudiometrics-0.0.2/spatialaudiometrics.egg-info/SOURCES.txt` & `spatialaudiometrics-0.0.3/spatialaudiometrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

