# Comparing `tmp/umap-learn-0.5.5.tar.gz` & `tmp/umap-learn-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "umap-learn-0.5.5.tar", last modified: Sat Nov 18 03:10:52 2023, max compression
+gzip compressed data, was "umap-learn-0.5.6.tar", last modified: Wed Apr  3 16:53:08 2024, max compression
```

## Comparing `umap-learn-0.5.5.tar` & `umap-learn-0.5.6.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 leland     (501) staff       (20)        0 2023-11-18 03:10:52.247222 umap-learn-0.5.5/
--rw-r--r--   0 leland     (501) staff       (20)     1514 2021-03-25 21:34:50.000000 umap-learn-0.5.5/LICENSE.txt
--rw-r--r--   0 leland     (501) staff       (20)    21209 2023-11-18 03:10:52.247048 umap-learn-0.5.5/PKG-INFO
--rw-r--r--   0 leland     (501) staff       (20)    20085 2023-11-18 03:10:32.000000 umap-learn-0.5.5/README.rst
--rw-r--r--   0 leland     (501) staff       (20)       38 2023-11-18 03:10:52.247267 umap-learn-0.5.5/setup.cfg
--rw-r--r--   0 leland     (501) staff       (20)     2308 2023-11-18 03:10:32.000000 umap-learn-0.5.5/setup.py
-drwxr-xr-x   0 leland     (501) staff       (20)        0 2023-11-18 03:10:52.246148 umap-learn-0.5.5/umap/
--rw-r--r--   0 leland     (501) staff       (20)     1188 2023-11-18 03:10:32.000000 umap-learn-0.5.5/umap/__init__.py
--rw-r--r--   0 leland     (501) staff       (20)    20564 2023-09-15 15:21:27.000000 umap-learn-0.5.5/umap/aligned_umap.py
--rw-r--r--   0 leland     (501) staff       (20)    34778 2023-05-12 20:19:15.000000 umap-learn-0.5.5/umap/distances.py
--rw-r--r--   0 leland     (501) staff       (20)    33430 2023-05-12 20:14:22.000000 umap-learn-0.5.5/umap/layouts.py
--rw-r--r--   0 leland     (501) staff       (20)    39979 2023-05-12 20:14:22.000000 umap-learn-0.5.5/umap/parametric_umap.py
--rwxr-xr-x   0 leland     (501) staff       (20)    55518 2023-11-18 03:10:32.000000 umap-learn-0.5.5/umap/plot.py
--rw-r--r--   0 leland     (501) staff       (20)    16711 2021-09-14 13:34:52.000000 umap-learn-0.5.5/umap/sparse.py
--rw-r--r--   0 leland     (501) staff       (20)    19771 2023-09-15 15:21:27.000000 umap-learn-0.5.5/umap/spectral.py
--rw-r--r--   0 leland     (501) staff       (20)   136425 2023-09-15 15:21:27.000000 umap-learn-0.5.5/umap/umap_.py
--rw-r--r--   0 leland     (501) staff       (20)     6695 2023-05-12 20:14:22.000000 umap-learn-0.5.5/umap/utils.py
--rw-r--r--   0 leland     (501) staff       (20)     2460 2021-03-25 21:34:50.000000 umap-learn-0.5.5/umap/validation.py
-drwxr-xr-x   0 leland     (501) staff       (20)        0 2023-11-18 03:10:52.246865 umap-learn-0.5.5/umap_learn.egg-info/
--rw-r--r--   0 leland     (501) staff       (20)    21209 2023-11-18 03:10:52.000000 umap-learn-0.5.5/umap_learn.egg-info/PKG-INFO
--rw-r--r--   0 leland     (501) staff       (20)      421 2023-11-18 03:10:52.000000 umap-learn-0.5.5/umap_learn.egg-info/SOURCES.txt
--rw-r--r--   0 leland     (501) staff       (20)        1 2023-11-18 03:10:52.000000 umap-learn-0.5.5/umap_learn.egg-info/dependency_links.txt
--rw-r--r--   0 leland     (501) staff       (20)        1 2021-10-29 16:29:12.000000 umap-learn-0.5.5/umap_learn.egg-info/not-zip-safe
--rw-r--r--   0 leland     (501) staff       (20)      246 2023-11-18 03:10:52.000000 umap-learn-0.5.5/umap_learn.egg-info/requires.txt
--rw-r--r--   0 leland     (501) staff       (20)        5 2023-11-18 03:10:52.000000 umap-learn-0.5.5/umap_learn.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-03 16:53:08.162125 umap-learn-0.5.6/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1514 2024-04-03 16:52:24.000000 umap-learn-0.5.6/LICENSE.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)    21212 2024-04-03 16:53:08.162125 umap-learn-0.5.6/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)    20085 2024-04-03 16:52:24.000000 umap-learn-0.5.6/README.rst
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-03 16:53:08.162125 umap-learn-0.5.6/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)     2277 2024-04-03 16:52:24.000000 umap-learn-0.5.6/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-03 16:53:08.162125 umap-learn-0.5.6/umap/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1188 2024-04-03 16:52:24.000000 umap-learn-0.5.6/umap/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20564 2024-04-03 16:52:24.000000 umap-learn-0.5.6/umap/aligned_umap.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    34778 2024-04-03 16:52:24.000000 umap-learn-0.5.6/umap/distances.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    33430 2024-04-03 16:52:24.000000 umap-learn-0.5.6/umap/layouts.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    34491 2024-04-03 16:52:24.000000 umap-learn-0.5.6/umap/parametric_umap.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)    55518 2024-04-03 16:52:24.000000 umap-learn-0.5.6/umap/plot.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16711 2024-04-03 16:52:24.000000 umap-learn-0.5.6/umap/sparse.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19771 2024-04-03 16:52:24.000000 umap-learn-0.5.6/umap/spectral.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   136981 2024-04-03 16:52:24.000000 umap-learn-0.5.6/umap/umap_.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6695 2024-04-03 16:52:24.000000 umap-learn-0.5.6/umap/utils.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2460 2024-04-03 16:52:24.000000 umap-learn-0.5.6/umap/validation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-03 16:53:08.162125 umap-learn-0.5.6/umap_learn.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)    21212 2024-04-03 16:53:08.000000 umap-learn-0.5.6/umap_learn.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      421 2024-04-03 16:53:08.000000 umap-learn-0.5.6/umap_learn.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-03 16:53:08.000000 umap-learn-0.5.6/umap_learn.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-03 16:53:05.000000 umap-learn-0.5.6/umap_learn.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      217 2024-04-03 16:53:08.000000 umap-learn-0.5.6/umap_learn.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-04-03 16:53:08.000000 umap-learn-0.5.6/umap_learn.egg-info/top_level.txt
```

### Comparing `umap-learn-0.5.5/LICENSE.txt` & `umap-learn-0.5.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `umap-learn-0.5.5/PKG-INFO` & `umap-learn-0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umap-learn
-Version: 0.5.5
+Version: 0.5.6
 Summary: Uniform Manifold Approximation and Projection
 Home-page: http://github.com/lmcinnes/umap
 Maintainer: Leland McInnes
 Maintainer-email: leland.mcinnes@gmail.com
 License: BSD
 Keywords: dimension reduction t-sne manifold
 Classifier: Development Status :: 3 - Alpha
@@ -15,18 +15,18 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/x-rst
 Provides-Extra: plot
 Provides-Extra: parametric_umap
 Provides-Extra: tbb
 License-File: LICENSE.txt
 
 .. -*- mode: rst -*-
```

### Comparing `umap-learn-0.5.5/README.rst` & `umap-learn-0.5.6/README.rst`

 * *Files identical despite different names*

### Comparing `umap-learn-0.5.5/setup.py` & `umap-learn-0.5.6/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
         with io.open("README.rst", encoding="UTF-8") as readme_file:
             return readme_file.read()
 
 
 configuration = {
     "name": "umap-learn",
-    "version": "0.5.5",
+    "version": "0.5.6",
     "description": "Uniform Manifold Approximation and Projection",
     "long_description": readme(),
     "long_description_content_type": "text/x-rst",
     "classifiers": [
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
@@ -29,18 +29,18 @@
         "Programming Language :: Python",
         "Topic :: Software Development",
         "Topic :: Scientific/Engineering",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: POSIX",
         "Operating System :: Unix",
         "Operating System :: MacOS",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
     ],
     "keywords": "dimension reduction t-sne manifold",
     "url": "http://github.com/lmcinnes/umap",
     "maintainer": "Leland McInnes",
     "maintainer_email": "leland.mcinnes@gmail.com",
     "license": "BSD",
     "packages": ["umap"],
@@ -59,15 +59,15 @@
             "datashader",
             "bokeh",
             "holoviews",
             "colorcet",
             "seaborn",
             "scikit-image",
         ],
-        "parametric_umap": ["tensorflow >= 2.1", "tensorflow-probability >= 0.10"],
+        "parametric_umap": ["tensorflow >= 2.1"],
         "tbb": ["tbb >= 2019.0"],
     },
     "ext_modules": [],
     "cmdclass": {},
     "test_suite": "pytest",
     "tests_require": ["pytest"],
     "data_files": (),
```

### Comparing `umap-learn-0.5.5/umap/__init__.py` & `umap-learn-0.5.6/umap/__init__.py`

 * *Files identical despite different names*

### Comparing `umap-learn-0.5.5/umap/aligned_umap.py` & `umap-learn-0.5.6/umap/aligned_umap.py`

 * *Files identical despite different names*

### Comparing `umap-learn-0.5.5/umap/distances.py` & `umap-learn-0.5.6/umap/distances.py`

 * *Files identical despite different names*

### Comparing `umap-learn-0.5.5/umap/layouts.py` & `umap-learn-0.5.6/umap/layouts.py`

 * *Files identical despite different names*

### Comparing `umap-learn-0.5.5/umap/parametric_umap.py` & `umap-learn-0.5.6/umap/parametric_umap.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,182 +3,117 @@
 from warnings import warn, catch_warnings, filterwarnings
 from numba import TypingError
 import os
 from umap.spectral import spectral_layout
 from sklearn.utils import check_random_state
 import codecs, pickle
 from sklearn.neighbors import KDTree
-import sys
-
 
 try:
+    # Used for tf.data.
     import tensorflow as tf
 except ImportError:
     warn(
         """The umap.parametric_umap package requires Tensorflow > 2.0 to be installed.
     You can install Tensorflow at https://www.tensorflow.org/install
     
     or you can install the CPU version of Tensorflow using 
 
     pip install umap-learn[parametric_umap]
 
     """
     )
     raise ImportError("umap.parametric_umap requires Tensorflow >= 2.0") from None
 
-TF_MAJOR_VERSION = int(tf.__version__.split(".")[0])
-if TF_MAJOR_VERSION < 2:
-    warn(
-        """The umap.parametric_umap package requires Tensorflow > 2.0 to be installed.
-    You can install Tensorflow at https://www.tensorflow.org/install
-    
-    or you can install the CPU version of Tensorflow using 
-
-    pip install umap-learn[parametric_umap]
-
-    """
-    )
-    raise ImportError("umap.parametric_umap requires Tensorflow >= 2.0") from None
-
 try:
-    import tensorflow_probability
+    import keras
+    from keras import ops
 except ImportError:
     warn(
-        """ Global structure preservation in the umap.parametric_umap package requires 
-        tensorflow_probability to be installed. You can install tensorflow_probability at
-        https://www.tensorflow.org/probability, 
-        
-        or via
-
-        pip install --upgrade tensorflow-probability
-
-        Please ensure to install a version which is compatible to your tensorflow 
-        installation. You can verify the correct release at 
-        https://github.com/tensorflow/probability/releases.
-
-        """
+        """The umap.parametric_umap package requires Keras >= 3 to be installed."""
     )
+    raise ImportError("umap.parametric_umap requires Keras") from None
 
 
 class ParametricUMAP(UMAP):
     def __init__(
         self,
-        optimizer=None,
         batch_size=None,
         dims=None,
         encoder=None,
         decoder=None,
-        parametric_embedding=True,
         parametric_reconstruction=False,
-        parametric_reconstruction_loss_fcn=tf.keras.losses.BinaryCrossentropy(
-            from_logits=True
-        ),
+        parametric_reconstruction_loss_fcn=None,
         parametric_reconstruction_loss_weight=1.0,
         autoencoder_loss=False,
         reconstruction_validation=None,
-        loss_report_frequency=10,
-        n_training_epochs=1,
         global_correlation_loss_weight=0,
-        run_eagerly=False,
         keras_fit_kwargs={},
         **kwargs
     ):
         """
         Parametric UMAP subclassing UMAP-learn, based on keras/tensorflow.
         There is also a non-parametric implementation contained within to compare
         with the base non-parametric implementation.
 
         Parameters
         ----------
-        optimizer : tf.keras.optimizers, optional
-            The tensorflow optimizer used for embedding, by default None
         batch_size : int, optional
             size of batch used for batch training, by default None
         dims :  tuple, optional
             dimensionality of data, if not flat (e.g. (32x32x3 images for ConvNet), by default None
-        encoder : tf.keras.Sequential, optional
+        encoder : keras.Sequential, optional
             The encoder Keras network
-        decoder : tf.keras.Sequential, optional
+        decoder : keras.Sequential, optional
             the decoder Keras network
-        parametric_embedding : bool, optional
-            Whether the embedder is parametric or non-parametric, by default True
         parametric_reconstruction : bool, optional
             Whether the decoder is parametric or non-parametric, by default False
         parametric_reconstruction_loss_fcn : bool, optional
-            What loss function to use for parametric reconstruction, by default tf.keras.losses.BinaryCrossentropy
+            What loss function to use for parametric reconstruction,
+            by default keras.losses.BinaryCrossentropy
         parametric_reconstruction_loss_weight : float, optional
             How to weight the parametric reconstruction loss relative to umap loss, by default 1.0
         autoencoder_loss : bool, optional
             [description], by default False
         reconstruction_validation : array, optional
             validation X data for reconstruction loss, by default None
-        loss_report_frequency : int, optional
-            how many times per epoch to report loss, by default 1
-        n_training_epochs : int, optional
-            number of epochs to train for, by default 1
         global_correlation_loss_weight : float, optional
             Whether to additionally train on correlation of global pairwise relationships (>0), by default 0
-        run_eagerly : bool, optional
-            Whether to run tensorflow eagerly
         keras_fit_kwargs : dict, optional
             additional arguments for model.fit (like callbacks), by default {}
         """
         super().__init__(**kwargs)
 
         # add to network
         self.dims = dims  # if this is an image, we should reshape for network
         self.encoder = encoder  # neural network used for embedding
         self.decoder = decoder  # neural network used for decoding
-        self.parametric_embedding = (
-            parametric_embedding  # nonparametric vs parametric embedding
-        )
         self.parametric_reconstruction = parametric_reconstruction
-        self.parametric_reconstruction_loss_fcn = parametric_reconstruction_loss_fcn
         self.parametric_reconstruction_loss_weight = (
             parametric_reconstruction_loss_weight
         )
-        self.run_eagerly = run_eagerly
+        self.parametric_reconstruction_loss_fcn = parametric_reconstruction_loss_fcn
         self.autoencoder_loss = autoencoder_loss
         self.batch_size = batch_size
-        self.loss_report_frequency = (
-            loss_report_frequency  # how many times per epoch to report loss in keras
-        )
-        if "tensorflow_probability" in sys.modules:
-            self.global_correlation_loss_weight = global_correlation_loss_weight
-        else:
-            warn(
-                "tensorflow_probability not installed or incompatible to current \
-                tensorflow installation. Setting global_correlation_loss_weight to zero."
-            )
-            self.global_correlation_loss_weight = 0
+        self.loss_report_frequency = 10
+        self.global_correlation_loss_weight = global_correlation_loss_weight
 
         self.reconstruction_validation = (
             reconstruction_validation  # holdout data for reconstruction acc
         )
         self.keras_fit_kwargs = keras_fit_kwargs  # arguments for model.fit
         self.parametric_model = None
 
-        # how many epochs to train for (different than n_epochs which is specific to each sample)
-        self.n_training_epochs = n_training_epochs
-        # set optimizer
-        if optimizer is None:
-            if parametric_embedding:
-                # Adam is better for parametric_embedding
-                self.optimizer = tf.keras.optimizers.Adam(1e-3)
-            else:
-                # Larger learning rate can be used for embedding
-                self.optimizer = tf.keras.optimizers.Adam(1e-1)
-        else:
-            self.optimizer = optimizer
-        if parametric_reconstruction and not parametric_embedding:
-            warn(
-                "Parametric decoding is not implemented with nonparametric \
-            embedding. Turning off parametric decoding"
-            )
-            self.parametric_reconstruction = False
+        # How many epochs to train for
+        # (different than n_epochs which is specific to each sample)
+        self.n_training_epochs = 1
+
+        # Set optimizer.
+        # Adam is better for parametric_embedding. Use gradient clipping by value.
+        self.optimizer = keras.optimizers.Adam(1e-3, clipvalue=4.0)
 
         if self.encoder is not None:
             if encoder.outputs[0].shape[-1] != self.n_components:
                 raise ValueError(
                     (
                         "Dimensionality of embedder network output ({}) does"
                         "not match n_components ({})".format(
@@ -224,24 +159,17 @@
         X : array, shape (n_samples, n_features)
             New data to be transformed.
         Returns
         -------
         X_new : array, shape (n_samples, n_components)
             Embedding of the new data in low-dimensional space.
         """
-        if self.parametric_embedding:
-            return self.encoder.predict(
-                np.asanyarray(X), batch_size=self.batch_size, verbose=self.verbose
-            )
-        else:
-            warn(
-                "Embedding new data is not supported by ParametricUMAP. \
-                Using original embedder."
-            )
-            return super().transform(X)
+        return self.encoder.predict(
+            np.asanyarray(X), batch_size=self.batch_size, verbose=self.verbose
+        )
 
     def inverse_transform(self, X):
         """ Transform X in the existing embedded space back into the input
         data space and return that transformed output.
         Parameters
         ----------
         X : array, shape (n_samples, n_components)
@@ -256,110 +184,26 @@
                 np.asanyarray(X), batch_size=self.batch_size, verbose=self.verbose
             )
         else:
             return super().inverse_transform(X)
 
     def _define_model(self):
         """Define the model in keras"""
-
-        # network outputs
-        outputs = {}
-
-        # inputs
-        if self.parametric_embedding:
-            to_x = tf.keras.layers.Input(shape=self.dims, name="to_x")
-            from_x = tf.keras.layers.Input(shape=self.dims, name="from_x")
-            inputs = [to_x, from_x]
-
-            # parametric embedding
-            embedding_to = self.encoder(to_x)
-            embedding_from = self.encoder(from_x)
-
-            if self.parametric_reconstruction:
-                # parametric reconstruction
-                if self.autoencoder_loss:
-                    embedding_to_recon = self.decoder(embedding_to)
-                else:
-                    # stop gradient of reconstruction loss before it reaches the encoder
-                    embedding_to_recon = self.decoder(tf.stop_gradient(embedding_to))
-
-                embedding_to_recon = tf.keras.layers.Lambda(
-                    lambda x: x, name="reconstruction"
-                )(embedding_to_recon)
-
-                outputs["reconstruction"] = embedding_to_recon
-
-        else:
-            # this is the sham input (it's just a 0) to make keras think there is input data
-            batch_sample = tf.keras.layers.Input(
-                shape=(1), dtype=tf.int32, name="batch_sample"
-            )
-
-            # gather all of the edges (so keras model is happy)
-            to_x = tf.squeeze(tf.gather(self.head, batch_sample[0]))
-            from_x = tf.squeeze(tf.gather(self.tail, batch_sample[0]))
-
-            # grab relevant embeddings
-            embedding_to = self.encoder(to_x)[:, -1, :]
-            embedding_from = self.encoder(from_x)[:, -1, :]
-
-            inputs = [batch_sample]
-
-        # concatenate to/from projections for loss computation
-        embedding_to_from = tf.concat([embedding_to, embedding_from], axis=1)
-        embedding_to_from = tf.keras.layers.Lambda(lambda x: x, name="umap")(
-            embedding_to_from
-        )
-        outputs["umap"] = embedding_to_from
-
-        if self.global_correlation_loss_weight > 0:
-            outputs["global_correlation"] = tf.keras.layers.Lambda(
-                lambda x: x, name="global_correlation"
-            )(embedding_to)
-
-        # create model
-
-        # self.parametric_model = tf.keras.Model(inputs=inputs, outputs=outputs)
-        self.parametric_model = GradientClippedModel(inputs=inputs, outputs=outputs)
-
-    def _compile_model(self):
-        """
-        Compiles keras model with losses
-        """
-        losses = {}
-        loss_weights = {}
-
-        umap_loss_fn = umap_loss(
-            self.batch_size,
-            self.negative_sample_rate,
+        prlw = self.parametric_reconstruction_loss_weight
+        self.parametric_model = UMAPModel(
             self._a,
             self._b,
-            self.edge_weight,
-            self.parametric_embedding,
-        )
-        losses["umap"] = umap_loss_fn
-        loss_weights["umap"] = 1.0
-
-        if self.global_correlation_loss_weight > 0:
-            losses["global_correlation"] = distance_loss_corr
-            loss_weights["global_correlation"] = self.global_correlation_loss_weight
-            if self.run_eagerly == False:
-                # this is needed to avoid a 'NaN' error bug in tensorflow_probability (v0.12.2)
-                warn("Setting tensorflow to run eagerly for global_correlation_loss.")
-                self.run_eagerly = True
-
-        if self.parametric_reconstruction:
-            losses["reconstruction"] = self.parametric_reconstruction_loss_fcn
-            loss_weights["reconstruction"] = self.parametric_reconstruction_loss_weight
-
-        self.parametric_model.compile(
-            optimizer=self.optimizer,
-            loss=losses,
-            loss_weights=loss_weights,
-            run_eagerly=self.run_eagerly,
+            negative_sample_rate=self.negative_sample_rate,
+            encoder=self.encoder,
+            decoder=self.decoder,
+            parametric_reconstruction_loss_fn=self.parametric_reconstruction_loss_fcn,
+            parametric_reconstruction=self.parametric_reconstruction,
+            parametric_reconstruction_loss_weight=prlw,
+            global_correlation_loss_weight=self.global_correlation_loss_weight,
+            autoencoder_loss=self.autoencoder_loss,
         )
 
     def _fit_embed_data(self, X, n_epochs, init, random_state):
 
         if self.metric == "precomputed":
             X = self._X
 
@@ -385,59 +229,41 @@
             tail,
             self.edge_weight,
         ) = construct_edge_dataset(
             X,
             self.graph_,
             self.n_epochs,
             self.batch_size,
-            self.parametric_embedding,
             self.parametric_reconstruction,
             self.global_correlation_loss_weight,
         )
-        self.head = tf.constant(tf.expand_dims(head.astype(np.int64), 0))
-        self.tail = tf.constant(tf.expand_dims(tail.astype(np.int64), 0))
+        self.head = ops.array(ops.expand_dims(head.astype(np.int64), 0))
+        self.tail = ops.array(ops.expand_dims(tail.astype(np.int64), 0))
 
-        if self.parametric_embedding:
-            init_embedding = None
-        else:
-            init_embedding = init_embedding_from_graph(
-                X,
-                self.graph_,
-                self.n_components,
-                self.random_state,
-                self.metric,
-                self._metric_kwds,
-                init="spectral",
-            )
+        init_embedding = None
 
         # create encoder and decoder model
         n_data = len(X)
         self.encoder, self.decoder = prepare_networks(
             self.encoder,
             self.decoder,
             self.n_components,
             self.dims,
             n_data,
-            self.parametric_embedding,
             self.parametric_reconstruction,
             init_embedding,
         )
 
         # create the model
         self._define_model()
-        self._compile_model()
 
         # report every loss_report_frequency subdivision of an epochs
-        if self.parametric_embedding:
-            steps_per_epoch = int(
-                n_edges / self.batch_size / self.loss_report_frequency
-            )
-        else:
-            # all edges are trained simultaneously with nonparametric, so this is arbitrary
-            steps_per_epoch = 100
+        steps_per_epoch = int(
+            n_edges / self.batch_size / self.loss_report_frequency
+        )
 
         # Validation dataset for reconstruction
         if (
             self.parametric_reconstruction
             and self.reconstruction_validation is not None
         ):
 
@@ -447,38 +273,34 @@
                     self.reconstruction_validation,
                     [len(self.reconstruction_validation)] + list(self.dims),
                 )
 
             validation_data = (
                 (
                     self.reconstruction_validation,
-                    tf.zeros_like(self.reconstruction_validation),
+                    ops.zeros_like(self.reconstruction_validation),
                 ),
                 {"reconstruction": self.reconstruction_validation},
             )
         else:
             validation_data = None
 
         # create embedding
         history = self.parametric_model.fit(
             edge_dataset,
             epochs=self.loss_report_frequency * self.n_training_epochs,
             steps_per_epoch=steps_per_epoch,
-            max_queue_size=100,
             validation_data=validation_data,
             **self.keras_fit_kwargs
         )
         # save loss history dictionary
         self._history = history.history
 
         # get the final embedding
-        if self.parametric_embedding:
-            embedding = self.encoder.predict(X, verbose=self.verbose)
-        else:
-            embedding = self.encoder.trainable_variables[0].numpy()
+        embedding = self.encoder.predict(X, verbose=self.verbose)
 
         return embedding, {}
 
     def __getstate__(self):
         # this function supports pickling, making sure that objects can be pickled
         return dict(
             (k, v)
@@ -486,38 +308,36 @@
             if should_pickle(k, v) and k not in ("optimizer", "encoder", "decoder", "parametric_model")
         )
 
     def save(self, save_location, verbose=True):
 
         # save encoder
         if self.encoder is not None:
-            encoder_output = os.path.join(save_location, "encoder")
+            encoder_output = os.path.join(save_location, "encoder.keras")
             self.encoder.save(encoder_output)
             if verbose:
                 print("Keras encoder model saved to {}".format(encoder_output))
 
         # save decoder
         if self.decoder is not None:
-            decoder_output = os.path.join(save_location, "decoder")
+            decoder_output = os.path.join(save_location, "decoder.keras")
             self.decoder.save(decoder_output)
             if verbose:
                 print("Keras decoder model saved to {}".format(decoder_output))
 
         # save parametric_model
         if self.parametric_model is not None:
-            parametric_model_output = os.path.join(save_location, "parametric_model")
+            parametric_model_output = os.path.join(save_location, "parametric_model.keras")
             self.parametric_model.save(parametric_model_output)
             if verbose:
                 print("Keras full model saved to {}".format(parametric_model_output))
 
         # # save model.pkl (ignoring unpickleable warnings)
         with catch_warnings():
             filterwarnings("ignore")
-            # work around optimizers not pickling anymore (since tf 2.4)
-            self._optimizer_dict = self.optimizer.get_config()
             model_output = os.path.join(save_location, "model.pkl")
             with open(model_output, "wb") as output:
                 pickle.dump(self, output, pickle.HIGHEST_PROTOCOL)
             if verbose:
                 print("Pickle of ParametricUMAP model saved to {}".format(model_output))
 
 
@@ -648,15 +468,15 @@
         parameter based on min_dist, by default 1.0
 
     Returns
     -------
     float
         log probability in embedding space
     """
-    return -tf.math.log1p(a * distances ** (2 * b))
+    return -ops.log1p(a * distances ** (2 * b))
 
 
 def compute_cross_entropy(
     probabilities_graph, log_probabilities_distance, EPS=1e-4, repulsion_strength=1.0
 ):
     """
     Compute cross entropy between low and high probability
@@ -670,248 +490,114 @@
     EPS : float, optional
         offset to ensure log is taken of a positive number, by default 1e-4
     repulsion_strength : float, optional
         strength of repulsion between negative samples, by default 1.0
 
     Returns
     -------
-    attraction_term: tf.float32
+    attraction_term: float
         attraction term for cross entropy loss
-    repellant_term: tf.float32
+    repellant_term: float
         repellent term for cross entropy loss
-    cross_entropy: tf.float32
+    cross_entropy: float
         cross entropy umap loss
 
     """
     # cross entropy
-    attraction_term = -probabilities_graph * tf.math.log_sigmoid(
+    attraction_term = -probabilities_graph * ops.log_sigmoid(
         log_probabilities_distance
     )
     # use numerically stable repellent term
     # Shi et al. 2022 (https://arxiv.org/abs/2111.08851)
     # log(1 - sigmoid(logits)) = log(sigmoid(logits)) - logits
     repellant_term = (
         -(1.0 - probabilities_graph)
-        * (tf.math.log_sigmoid(log_probabilities_distance) - log_probabilities_distance)
+        * (ops.log_sigmoid(log_probabilities_distance) - log_probabilities_distance)
         * repulsion_strength
     )
 
     # balance the expected losses between attraction and repel
     CE = attraction_term + repellant_term
     return attraction_term, repellant_term, CE
 
 
-def umap_loss(
-    batch_size,
-    negative_sample_rate,
-    _a,
-    _b,
-    edge_weights,
-    parametric_embedding,
-    repulsion_strength=1.0,
-):
-    """
-    Generate a keras-compatible loss function for UMAP loss
-
-    Parameters
-    ----------
-    batch_size : int
-        size of mini-batches
-    negative_sample_rate : int
-        number of negative samples per positive samples to train on
-    _a : float
-        distance parameter in embedding space
-    _b : float
-        distance parameter in embedding space
-    edge_weights : array
-        weights of all edges from sparse UMAP graph
-    parametric_embedding : bool
-        whether the embedding is parametric or nonparametric
-    repulsion_strength : float, optional
-        strength of repulsion vs attraction for cross-entropy, by default 1.0
-
-    Returns
-    -------
-    loss : function
-        loss function that takes in a placeholder (0) and the output of the keras network
-    """
-
-    if not parametric_embedding:
-        # multiply loss by weights for nonparametric
-        weights_tiled = np.tile(edge_weights, negative_sample_rate + 1)
-
-    @tf.function
-    def loss(placeholder_y, embed_to_from):
-        # split out to/from
-        embedding_to, embedding_from = tf.split(
-            embed_to_from, num_or_size_splits=2, axis=1
-        )
-
-        # get negative samples
-        embedding_neg_to = tf.repeat(embedding_to, negative_sample_rate, axis=0)
-        repeat_neg = tf.repeat(embedding_from, negative_sample_rate, axis=0)
-        embedding_neg_from = tf.gather(
-            repeat_neg, tf.random.shuffle(tf.range(tf.shape(repeat_neg)[0]))
-        )
-
-        #  distances between samples (and negative samples)
-        distance_embedding = tf.concat(
-            [
-                tf.norm(embedding_to - embedding_from, axis=1),
-                tf.norm(embedding_neg_to - embedding_neg_from, axis=1),
-            ],
-            axis=0,
-        )
-
-        # convert distances to probabilities
-        log_probabilities_distance = convert_distance_to_log_probability(
-            distance_embedding, _a, _b
-        )
-
-        # set true probabilities based on negative sampling
-        probabilities_graph = tf.concat(
-            [tf.ones(batch_size), tf.zeros(batch_size * negative_sample_rate)], axis=0
-        )
-
-        # compute cross entropy
-        (attraction_loss, repellant_loss, ce_loss) = compute_cross_entropy(
-            probabilities_graph,
-            log_probabilities_distance,
-            repulsion_strength=repulsion_strength,
-        )
-
-        if not parametric_embedding:
-            ce_loss = ce_loss * weights_tiled
-
-        return tf.reduce_mean(ce_loss)
-
-    return loss
-
-
-def distance_loss_corr(x, z_x):
-    """Loss based on the distance between elements in a batch"""
-
-    # flatten data
-    x = tf.keras.layers.Flatten()(x)
-    z_x = tf.keras.layers.Flatten()(z_x)
-
-    ## z score data
-    def z_score(x):
-        return (x - tf.reduce_mean(x)) / tf.math.reduce_std(x)
-
-    x = z_score(x)
-    z_x = z_score(z_x)
-
-    # clip distances to 10 standard deviations for stability
-    x = tf.clip_by_value(x, -10, 10)
-    z_x = tf.clip_by_value(z_x, -10, 10)
-
-    dx = tf.math.reduce_euclidean_norm(x[1:] - x[:-1], axis=1)
-    dz = tf.math.reduce_euclidean_norm(z_x[1:] - z_x[:-1], axis=1)
-
-    # jitter dz to prevent mode collapse
-    dz = dz + tf.random.uniform(dz.shape) * 1e-10
-
-    # compute correlation
-    corr_d = tf.squeeze(
-        tensorflow_probability.stats.correlation(
-            x=tf.expand_dims(dx, -1), y=tf.expand_dims(dz, -1)
-        )
-    )
-    if tf.math.is_nan(corr_d):
-        raise ValueError("NaN values found in correlation loss.")
-
-    return -corr_d
-
 
 def prepare_networks(
     encoder,
     decoder,
     n_components,
     dims,
     n_data,
-    parametric_embedding,
     parametric_reconstruction,
     init_embedding=None,
 ):
     """
     Generates a set of keras networks for the encoder and decoder if one has not already
     been predefined.
 
     Parameters
     ----------
-    encoder : tf.keras.Sequential
+    encoder : keras.Sequential
         The encoder Keras network
-    decoder : tf.keras.Sequential
+    decoder : keras.Sequential
         the decoder Keras network
     n_components : int
         the dimensionality of the latent space
     dims : tuple of shape (dim1, dim2, dim3...)
         dimensionality of data
     n_data : number of elements in dataset
         # of elements in training dataset
-    parametric_embedding : bool
-        Whether the embedder is parametric or non-parametric
     parametric_reconstruction : bool
         Whether the decoder is parametric or non-parametric
     init_embedding : array (optional, default None)
         The initial embedding, for nonparametric embeddings
 
     Returns
     -------
-    encoder: tf.keras.Sequential
+    encoder: keras.Sequential
         encoder keras network
-    decoder: tf.keras.Sequential
+    decoder: keras.Sequential
         decoder keras network
     """
 
-    if parametric_embedding:
-        if encoder is None:
-            encoder = tf.keras.Sequential(
-                [
-                    tf.keras.layers.InputLayer(input_shape=dims),
-                    tf.keras.layers.Flatten(),
-                    tf.keras.layers.Dense(units=100, activation="relu"),
-                    tf.keras.layers.Dense(units=100, activation="relu"),
-                    tf.keras.layers.Dense(units=100, activation="relu"),
-                    tf.keras.layers.Dense(units=n_components, name="z"),
-                ]
-            )
-    else:
-        embedding_layer = tf.keras.layers.Embedding(
-            n_data, n_components, input_length=1
+    if encoder is None:
+        encoder = keras.Sequential(
+            [
+                keras.layers.Input(shape=dims),
+                keras.layers.Flatten(),
+                keras.layers.Dense(units=100, activation="relu"),
+                keras.layers.Dense(units=100, activation="relu"),
+                keras.layers.Dense(units=100, activation="relu"),
+                keras.layers.Dense(units=n_components, name="z"),
+            ]
         )
-        embedding_layer.build(input_shape=(1,))
-        embedding_layer.set_weights([init_embedding])
-        encoder = tf.keras.Sequential([embedding_layer])
 
     if decoder is None:
         if parametric_reconstruction:
-            decoder = tf.keras.Sequential(
+            decoder = keras.Sequential(
                 [
-                    tf.keras.layers.InputLayer(input_shape=n_components),
-                    tf.keras.layers.Dense(units=100, activation="relu"),
-                    tf.keras.layers.Dense(units=100, activation="relu"),
-                    tf.keras.layers.Dense(units=100, activation="relu"),
-                    tf.keras.layers.Dense(
+                    keras.layers.Input(shape=(n_components,)),
+                    keras.layers.Dense(units=100, activation="relu"),
+                    keras.layers.Dense(units=100, activation="relu"),
+                    keras.layers.Dense(units=100, activation="relu"),
+                    keras.layers.Dense(
                         units=np.product(dims), name="recon", activation=None
                     ),
-                    tf.keras.layers.Reshape(dims),
+                    keras.layers.Reshape(dims),
                 ]
             )
 
     return encoder, decoder
 
 
 def construct_edge_dataset(
     X,
     graph_,
     n_epochs,
     batch_size,
-    parametric_embedding,
     parametric_reconstruction,
     global_correlation_loss_weight,
 ):
     """
     Construct a tf.data.Dataset of edges, sampled by edge weight.
 
     Parameters
@@ -920,20 +606,17 @@
         New data to be transformed.
     graph_ : scipy.sparse.csr.csr_matrix
         Generated UMAP graph
     n_epochs : int
         # of epochs to train each edge
     batch_size : int
         batch size
-    parametric_embedding : bool
-        Whether the embedder is parametric or non-parametric
     parametric_reconstruction : bool
         Whether the decoder is parametric or non-parametric
     """
-
     def gather_index(index):
         return X[index]
 
     # if X is > 512Mb in size, we need to use a different, slower method for
     #    batching data.
     gather_indices_in_python = True if X.nbytes * 1e-9 > 0.5 else False
 
@@ -944,82 +627,58 @@
             edge_from_batch = tf.py_function(gather_index, [edge_from], [tf.float32])[0]
         else:
             edge_to_batch = tf.gather(X, edge_to)
             edge_from_batch = tf.gather(X, edge_from)
         return edge_to_batch, edge_from_batch
 
     def get_outputs(edge_to_batch, edge_from_batch):
-        outputs = {"umap": tf.repeat(0, batch_size)}
+        outputs = {"umap": ops.repeat(0, batch_size)}
         if global_correlation_loss_weight > 0:
             outputs["global_correlation"] = edge_to_batch
         if parametric_reconstruction:
             # add reconstruction to iterator output
-            # edge_out = tf.concat([edge_to_batch, edge_from_batch], axis=0)
+            # edge_out = ops.concatenate([edge_to_batch, edge_from_batch], axis=0)
             outputs["reconstruction"] = edge_to_batch
         return (edge_to_batch, edge_from_batch), outputs
 
-    def make_sham_generator():
-        """
-        The sham generator is a placeholder when all data is already intrinsic to
-        the model, but keras wants some input data. Used for non-parametric
-        embedding.
-        """
-
-        def sham_generator():
-            while True:
-                yield tf.zeros(1, dtype=tf.int32), tf.zeros(1, dtype=tf.int32)
-
-        return sham_generator
-
     # get data from graph
-    graph, epochs_per_sample, head, tail, weight, n_vertices = get_graph_elements(
+    _, epochs_per_sample, head, tail, weight, n_vertices = get_graph_elements(
         graph_, n_epochs
     )
 
     # number of elements per batch for embedding
     if batch_size is None:
         # batch size can be larger if its just over embeddings
-        if parametric_embedding:
-            batch_size = np.min([n_vertices, 1000])
-        else:
-            batch_size = len(head)
+        batch_size = int(np.min([n_vertices, 1000]))
 
     edges_to_exp, edges_from_exp = (
         np.repeat(head, epochs_per_sample.astype("int")),
         np.repeat(tail, epochs_per_sample.astype("int")),
     )
 
     # shuffle edges
     shuffle_mask = np.random.permutation(range(len(edges_to_exp)))
     edges_to_exp = edges_to_exp[shuffle_mask].astype(np.int64)
     edges_from_exp = edges_from_exp[shuffle_mask].astype(np.int64)
 
     # create edge iterator
-    if parametric_embedding:
-        edge_dataset = tf.data.Dataset.from_tensor_slices(
-            (edges_to_exp, edges_from_exp)
-        )
-        edge_dataset = edge_dataset.repeat()
-        edge_dataset = edge_dataset.shuffle(10000)
-        edge_dataset = edge_dataset.batch(batch_size, drop_remainder=True)
-        edge_dataset = edge_dataset.map(
-            gather_X, num_parallel_calls=tf.data.experimental.AUTOTUNE
-        )
-        edge_dataset = edge_dataset.map(
-            get_outputs, num_parallel_calls=tf.data.experimental.AUTOTUNE
-        )
-        edge_dataset = edge_dataset.prefetch(10)
-    else:
-        # nonparametric embedding uses a sham dataset
-        gen = make_sham_generator()
-        edge_dataset = tf.data.Dataset.from_generator(
-            gen,
-            (tf.int32, tf.int32),
-            output_shapes=(tf.TensorShape(1), tf.TensorShape((1,))),
-        )
+    edge_dataset = tf.data.Dataset.from_tensor_slices(
+        (edges_to_exp, edges_from_exp)
+    )
+    edge_dataset = edge_dataset.repeat()
+    edge_dataset = edge_dataset.shuffle(10000)
+    edge_dataset = edge_dataset.batch(batch_size, drop_remainder=True)
+    edge_dataset = edge_dataset.map(
+        gather_X, num_parallel_calls=tf.data.experimental.AUTOTUNE
+    )
+    edge_dataset = edge_dataset.map(
+        get_outputs, num_parallel_calls=tf.data.experimental.AUTOTUNE
+    )
+    edge_dataset = edge_dataset.prefetch(10)
+
     return edge_dataset, batch_size, len(edges_to_exp), head, tail, weight
 
 
 def should_pickle(key, val):
     """
     Checks if a dictionary item can be pickled
 
@@ -1036,15 +695,15 @@
         whether the dictionary item can be pickled
     """
     try:
         ## make sure object can be pickled and then re-read
         # pickle object
         pickled = codecs.encode(pickle.dumps(val), "base64").decode()
         # unpickle object
-        unpickled = pickle.loads(codecs.decode(pickled.encode(), "base64"))
+        _ = pickle.loads(codecs.decode(pickled.encode(), "base64"))
     except (
         pickle.PicklingError,
         tf.errors.InvalidArgumentError,
         TypeError,
         tf.errors.InternalError,
         tf.errors.NotFoundError,
         OverflowError,
@@ -1080,78 +739,283 @@
     ## Loads a ParametricUMAP model and its related keras models
 
     model_output = os.path.join(save_location, "model.pkl")
     model = pickle.load((open(model_output, "rb")))
     if verbose:
         print("Pickle of ParametricUMAP model loaded from {}".format(model_output))
 
-    # Work around optimizer not pickling anymore (since tf 2.4)
-    class_name = model._optimizer_dict["name"]
-    OptimizerClass = getattr(tf.keras.optimizers, class_name)
-    model.optimizer = OptimizerClass.from_config(model._optimizer_dict)
-
     # load encoder
-    encoder_output = os.path.join(save_location, "encoder")
+    encoder_output = os.path.join(save_location, "encoder.keras")
     if os.path.exists(encoder_output):
-        model.encoder = tf.keras.models.load_model(encoder_output)
+        model.encoder = keras.models.load_model(encoder_output)
         if verbose:
             print("Keras encoder model loaded from {}".format(encoder_output))
 
     # save decoder
-    decoder_output = os.path.join(save_location, "decoder")
+    decoder_output = os.path.join(save_location, "decoder.keras")
     if os.path.exists(decoder_output):
-        model.decoder = tf.keras.models.load_model(decoder_output)
+        model.decoder = keras.models.load_model(decoder_output)
         print("Keras decoder model loaded from {}".format(decoder_output))
 
-    # get the custom loss function
-    umap_loss_fn = umap_loss(
-        model.batch_size,
-        model.negative_sample_rate,
-        model._a,
-        model._b,
-        model.edge_weight,
-        model.parametric_embedding,
-    )
-
     # save parametric_model
     parametric_model_output = os.path.join(save_location, "parametric_model")
     if os.path.exists(parametric_model_output):
-        model.parametric_model = tf.keras.models.load_model(
-            parametric_model_output, custom_objects={"loss": umap_loss_fn}
+        model.parametric_model = keras.models.load_model(
+            parametric_model_output
         )
         print("Keras full model loaded from {}".format(parametric_model_output))
 
     return model
 
 
-class GradientClippedModel(tf.keras.Model):
-    """
-    We need to define a custom keras model here for gradient clipping,
-    to stabilize training.
-    """
+def covariance(x,
+               y=None,
+               keepdims=False):
+    """Adapted from TF Probability."""
+    x = ops.convert_to_tensor(x)
+    # Covariance *only* uses the centered versions of x (and y).
+    x = x - ops.mean(x, axis=0, keepdims=True)
+
+    if y is None:
+        y = x
+        event_axis = ops.mean(
+          x * ops.conj(y), axis=0, keepdims=keepdims)
+    else:
+        y = ops.convert_to_tensor(y, dtype=x.dtype)
+        y = y - ops.mean(y, axis=0, keepdims=True)
+        event_axis = [len(x.shape) - 1]
+    sample_axis = [0]
+
+    event_axis = ops.cast(event_axis, dtype="int32")
+    sample_axis = ops.cast(sample_axis, dtype="int32")
+
+    x_permed = ops.transpose(x)
+    y_permed = ops.transpose(y)
+
+    n_events = ops.shape(x_permed)[0]
+    n_samples = ops.shape(x_permed)[1]
+
+    # Flatten sample_axis into one long dim.
+    x_permed_flat = ops.reshape(
+        x_permed, (n_events, n_samples))
+    y_permed_flat = ops.reshape(
+        y_permed, (n_events, n_samples))
+    # Do the same for event_axis.
+    x_permed_flat = ops.reshape(
+        x_permed, (n_events, n_samples))
+    y_permed_flat = ops.reshape(
+        y_permed, (n_events, n_samples))
+
+    # After matmul, cov.shape = batch_shape + [n_events, n_events]
+    cov = ops.matmul(
+        x_permed_flat, ops.transpose(y_permed_flat)) / ops.cast(
+            n_samples, x.dtype)
+
+    cov = ops.reshape(
+        cov,
+        (n_events**2, 1),
+    )
+
+    # Permuting by the argsort inverts the permutation, making
+    # cov.shape have ones in the position where there were samples, and
+    # [n_events * n_events] in the event position.
+    cov = ops.transpose(cov)
+
+    # Now expand event_shape**2 into event_shape + event_shape.
+    # We here use (for the first time) the fact that we require event_axis to be
+    # contiguous.
+    cov = ops.reshape(
+        cov,
+        ops.shape(cov)[:1] + (n_events, n_events),
+    )
+
+    if not keepdims:
+        cov = ops.squeeze(cov, axis=0)
+    return cov
+
+
+def correlation(x,
+                y=None,
+                keepdims=False):
+    x = x / ops.std(x, axis=0, keepdims=True)
+    if y is not None:
+        y = y / ops.std(y, axis=0, keepdims=True)
+    return covariance(
+        x=x,
+        y=y,
+        keepdims=keepdims)
+
+
+class StopGradient(keras.layers.Layer):
+    def call(self, x):
+        return ops.stop_gradient(x)
+
+
+class UMAPModel(keras.Model):
+    def __init__(self,
+                 umap_loss_a,
+                 umap_loss_b,
+                 negative_sample_rate,
+                 encoder,
+                 decoder,
+                 optimizer=None,
+                 parametric_reconstruction_loss_fn=None,
+                 parametric_reconstruction=False,
+                 parametric_reconstruction_loss_weight=1.,
+                 global_correlation_loss_weight=0.,
+                 autoencoder_loss=False,
+                 name="umap_model"):
+        super().__init__(name=name)
+
+        self.encoder = encoder
+        self.decoder = decoder
+        self.parametric_reconstruction = parametric_reconstruction
+        self.global_correlation_loss_weight = global_correlation_loss_weight
+        self.parametric_reconstruction_loss_weight = (
+            parametric_reconstruction_loss_weight
+        )
+        self.negative_sample_rate = negative_sample_rate
+        self.umap_loss_a = umap_loss_a
+        self.umap_loss_b = umap_loss_b
+        self.autoencoder_loss = autoencoder_loss
+
+        optimizer = optimizer or keras.optimizers.Adam(1e-3, clipvalue=4.0)
+        self.compile(optimizer=optimizer)
+
+        self.flatten = keras.layers.Flatten()
+        self.seed_generator = keras.random.SeedGenerator()
+        if parametric_reconstruction_loss_fn is None:
+            self.parametric_reconstruction_loss_fn = keras.losses.BinaryCrossentropy(
+                from_logits=True
+            )
+        else:
+            self.parametric_reconstruction_loss_fn = (
+                parametric_reconstruction_loss_fn
+            )
+
+    def call(self, inputs):
+        to_x, from_x = inputs
+        embedding_to = self.encoder(to_x)
+        embedding_from = self.encoder(from_x)
+
+        y_pred = {
+            "embedding_to": embedding_to,
+            "embedding_from": embedding_from,
+        }
+        if self.parametric_reconstruction:
+            # parametric reconstruction
+            if self.autoencoder_loss:
+                embedding_to_recon = self.decoder(embedding_to)
+            else:
+                # stop gradient of reconstruction loss before it reaches the encoder
+                embedding_to_recon = self.decoder(ops.stop_gradient(embedding_to))
+            y_pred["reconstruction"] = embedding_to_recon
+        return y_pred
+
+    def compute_loss(
+        self, x=None, y=None, y_pred=None, sample_weight=None, **kwargs
+    ):
+        losses = []
+        # Regularization losses.
+        for loss in self.losses:
+            losses.append(ops.cast(loss, dtype=keras.backend.floatx()))
+
+        # umap loss
+        losses.append(self._umap_loss(y_pred))
+
+        # global correlation loss
+        if self.global_correlation_loss_weight > 0:
+            losses.append(self._global_correlation_loss(y, y_pred))
+
+        # parametric reconstruction loss
+        if self.parametric_reconstruction:
+            losses.append(self._parametric_reconstruction_loss(y, y_pred))
+
+        return ops.sum(losses)
+
+    def _umap_loss(self, y_pred, repulsion_strength=1.0):
+        # split out to/from
+        embedding_to = y_pred["embedding_to"]
+        embedding_from = y_pred["embedding_from"]
+
+        # get negative samples
+        embedding_neg_to = ops.repeat(embedding_to, self.negative_sample_rate, axis=0)
+        repeat_neg = ops.repeat(embedding_from, self.negative_sample_rate, axis=0)
+
+        repeat_neg_batch_dim = ops.shape(repeat_neg)[0]
+        shuffled_indices = keras.random.shuffle(
+            ops.arange(repeat_neg_batch_dim), seed=self.seed_generator)
+
+        if keras.config.backend() == "tensorflow":
+            embedding_neg_from = tf.gather(
+                repeat_neg, shuffled_indices
+            )
+        else:
+            embedding_neg_from = repeat_neg[shuffled_indices]
+
+        #  distances between samples (and negative samples)
+        distance_embedding = ops.concatenate(
+            [
+                ops.norm(embedding_to - embedding_from, axis=1),
+                ops.norm(embedding_neg_to - embedding_neg_from, axis=1),
+            ],
+            axis=0,
+        )
+
+        # convert distances to probabilities
+        log_probabilities_distance = convert_distance_to_log_probability(
+            distance_embedding, self.umap_loss_a, self.umap_loss_b
+        )
+
+        # set true probabilities based on negative sampling
+        batch_size = ops.shape(embedding_to)[0]
+        probabilities_graph = ops.concatenate(
+            [
+                ops.ones((batch_size,)),
+                ops.zeros((batch_size * self.negative_sample_rate,)),
+            ],
+            axis=0
+        )
+
+        # compute cross entropy
+        (attraction_loss, repellant_loss, ce_loss) = compute_cross_entropy(
+            probabilities_graph,
+            log_probabilities_distance,
+            repulsion_strength=repulsion_strength,
+        )
+
+        return ops.mean(ce_loss)
+
+    def _global_correlation_loss(self, y, y_pred):
+        # flatten data
+        x = self.flatten(y["global_correlation"])
+        z_x = self.flatten(y_pred["embedding_to"])
+
+        # z score data
+        def z_score(x):
+            return (x - ops.mean(x)) / ops.std(x)
+
+        x = z_score(x)
+        z_x = z_score(z_x)
+
+        # clip distances to 10 standard deviations for stability
+        x = ops.clip(x, -10, 10)
+        z_x = ops.clip(z_x, -10, 10)
+
+        dx = ops.norm(x[1:] - x[:-1], axis=1)
+        dz = ops.norm(z_x[1:] - z_x[:-1], axis=1)
+
+        # jitter dz to prevent mode collapse
+        dz = dz + keras.random.uniform(dz.shape, seed=self.seed_generator) * 1e-10
+
+        # compute correlation
+        corr_d = ops.squeeze(
+            correlation(
+                x=ops.expand_dims(dx, -1), y=ops.expand_dims(dz, -1)
+            )
+        )
+        return -corr_d * self.global_correlation_loss_weight
 
-    def train_step(self, data):
-        # Unpack the data. Its structure depends on your model and
-        # on what you pass to `fit()`.
-        x, y = data
-
-        with tf.GradientTape() as tape:
-            y_pred = self(x, training=True)  # Forward pass
-            # Compute the loss value
-            # (the loss function is configured in `compile()`)
-            loss = self.compiled_loss(y, y_pred, regularization_losses=self.losses)
-
-        # Compute gradients
-        trainable_vars = self.trainable_variables
-        gradients = tape.gradient(loss, trainable_vars)
-        gradients = [tf.clip_by_value(grad, -4.0, 4.0) for grad in gradients]
-        gradients = [
-            (tf.where(tf.math.is_nan(grad), tf.zeros_like(grad), grad))
-            for grad in gradients
-        ]
-
-        # Update weights
-        self.optimizer.apply_gradients(zip(gradients, trainable_vars))
-        # Update metrics (includes the metric that tracks the loss)
-        self.compiled_metrics.update_state(y, y_pred)
-        # Return a dict mapping metric names to current value
-        return {m.name: m.result() for m in self.metrics}
+    def _parametric_reconstruction_loss(self, y, y_pred):
+        loss = self.parametric_reconstruction_loss_fn(
+            y["reconstruction"], y_pred["reconstruction"])
+        return loss * self.parametric_reconstruction_loss_weight
```

### Comparing `umap-learn-0.5.5/umap/plot.py` & `umap-learn-0.5.6/umap/plot.py`

 * *Files identical despite different names*

### Comparing `umap-learn-0.5.5/umap/sparse.py` & `umap-learn-0.5.6/umap/sparse.py`

 * *Files identical despite different names*

### Comparing `umap-learn-0.5.5/umap/spectral.py` & `umap-learn-0.5.6/umap/spectral.py`

 * *Files identical despite different names*

### Comparing `umap-learn-0.5.5/umap/umap_.py` & `umap-learn-0.5.6/umap/umap_.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,14 +59,15 @@
 NPY_INFINITY = np.inf
 
 DISCONNECTION_DISTANCES = {
     "correlation": 2,
     "cosine": 2,
     "hellinger": 1,
     "jaccard": 1,
+    "bit_jaccard": 1,
     "dice": 1,
 }
 
 
 def flatten_iter(container):
     for i in container:
         if isinstance(i, (list, tuple)):
@@ -1936,14 +1937,15 @@
             "hellinger",
         ):
             self.angular_rp_forest = True
 
         if self.n_jobs < -1 or self.n_jobs == 0:
             raise ValueError("n_jobs must be a postive integer, or -1 (for all cores)")
         if self.n_jobs != 1 and self.random_state is not None:
+            self.n_jobs = 1
             warn(f"n_jobs value {self.n_jobs} overridden to 1 by setting random_state. Use no seed for parallelism.") 
 
         if self.dens_lambda < 0.0:
             raise ValueError("dens_lambda cannot be negative")
         if self.dens_frac < 0.0 or self.dens_frac > 1.0:
             raise ValueError("dens_frac must be between 0.0 and 1.0")
         if self.dens_var_shift < 0.0:
@@ -2346,16 +2348,18 @@
 
         force_all_finite : Whether to raise an error on np.inf, np.nan, pd.NA in array.
             The possibilities are: - True: Force all values of array to be finite.
                                    - False: accepts np.inf, np.nan, pd.NA in array.
                                    - 'allow-nan': accepts only np.nan and pd.NA values in array.
                                      Values cannot be infinite.
         """
-
-        X = check_array(X, dtype=np.float32, accept_sparse="csr", order="C", force_all_finite=force_all_finite)
+        if self.metric in ("bit_hamming", "bit_jaccard"):
+            X = check_array(X, dtype=np.uint8, order="C", force_all_finite=force_all_finite)
+        else:
+            X = check_array(X, dtype=np.float32, accept_sparse="csr", order="C", force_all_finite=force_all_finite)
         self._raw_data = X
 
         # Handle all the optional arguments, setting default
         if self.a is None or self.b is None:
             self._a, self._b = find_ab_params(self.spread, self.min_dist)
         else:
             self._a = self.a
@@ -2921,15 +2925,18 @@
         """
         # If we fit just a single instance then error
         if self._raw_data.shape[0] == 1:
             raise ValueError(
                 "Transform unavailable when model was fit with only a single data sample."
             )
         # If we just have the original input then short circuit things
-        X = check_array(X, dtype=np.float32, accept_sparse="csr", order="C", force_all_finite=force_all_finite)
+        if self.metric in ("bit_hamming", "bit_jaccard"):
+            X = check_array(X, dtype=np.uint8, order="C", force_all_finite=force_all_finite)
+        else:
+            X = check_array(X, dtype=np.float32, accept_sparse="csr", order="C", force_all_finite=force_all_finite)
         x_hash = joblib.hash(X)
         if x_hash == self._input_hash:
             if self.transform_mode == "embedding":
                 return self.embedding_
             elif self.transform_mode == "graph":
                 return self.graph_
             else:
@@ -3292,15 +3299,18 @@
             verbose=self.verbose,
             tqdm_kwds=self.tqdm_kwds,
         )
 
         return inv_transformed_points
 
     def update(self, X, force_all_finite=True):
-        X = check_array(X, dtype=np.float32, accept_sparse="csr", order="C", force_all_finite=force_all_finite)
+        if self.metric in ("bit_hamming", "bit_jaccard"):
+            X = check_array(X, dtype=np.uint8, order="C", force_all_finite=force_all_finite)
+        else:
+            X = check_array(X, dtype=np.float32, accept_sparse="csr", order="C", force_all_finite=force_all_finite)
         random_state = check_random_state(self.transform_seed)
         rng_state = random_state.randint(INT32_MIN, INT32_MAX, 3).astype(np.int64)
 
         original_size = self._raw_data.shape[0]
 
         if self.metric == "precomputed":
             raise ValueError("Update does not currently support precomputed metrics")
```

### Comparing `umap-learn-0.5.5/umap/utils.py` & `umap-learn-0.5.6/umap/utils.py`

 * *Files identical despite different names*

### Comparing `umap-learn-0.5.5/umap/validation.py` & `umap-learn-0.5.6/umap/validation.py`

 * *Files identical despite different names*

### Comparing `umap-learn-0.5.5/umap_learn.egg-info/PKG-INFO` & `umap-learn-0.5.6/umap_learn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: umap-learn
-Version: 0.5.5
+Version: 0.5.6
 Summary: Uniform Manifold Approximation and Projection
 Home-page: http://github.com/lmcinnes/umap
 Maintainer: Leland McInnes
 Maintainer-email: leland.mcinnes@gmail.com
 License: BSD
 Keywords: dimension reduction t-sne manifold
 Classifier: Development Status :: 3 - Alpha
@@ -15,18 +15,18 @@
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development
 Classifier: Topic :: Scientific/Engineering
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/x-rst
 Provides-Extra: plot
 Provides-Extra: parametric_umap
 Provides-Extra: tbb
 License-File: LICENSE.txt
 
 .. -*- mode: rst -*-
```

