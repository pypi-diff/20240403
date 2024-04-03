# Comparing `tmp/frc-0.1.0.tar.gz` & `tmp/frc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "frc-0.1.0.tar", max compression
+gzip compressed data, was "frc-0.1.1.tar", max compression
```

## Comparing `frc-0.1.0.tar` & `frc-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      605 2021-11-18 16:02:03.220682 frc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3021 2021-11-15 14:43:55.088449 frc-0.1.0/README.md
--rw-r--r--   0        0        0      288 2021-11-15 14:17:16.364817 frc-0.1.0/src/frc/__init__.py
--rw-r--r--   0        0        0     1448 2021-11-18 12:21:29.295537 frc-0.1.0/src/frc/_internal_utility.py
--rw-r--r--   0        0        0     1118 2021-11-18 12:21:29.296536 frc-0.1.0/src/frc/deps_types.py
--rw-r--r--   0        0        0     8192 2021-11-18 12:21:29.296536 frc-0.1.0/src/frc/frc_functions.py
--rw-r--r--   0        0        0     7369 2021-11-15 11:15:29.464201 frc-0.1.0/src/frc/utility.py
--rw-r--r--   0        0        0     3841 2021-11-18 16:07:11.519677 frc-0.1.0/setup.py
--rw-r--r--   0        0        0     3670 2021-11-18 16:07:11.519677 frc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-03 13:05:36.998278 frc-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4067 2024-04-03 13:05:36.998278 frc-0.1.1/README.md
+-rw-r--r--   0        0        0      889 2024-04-03 13:05:36.998278 frc-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      280 2024-04-03 13:05:36.998278 frc-0.1.1/src/frc/__init__.py
+-rw-r--r--   0        0        0     1398 2024-04-03 13:05:36.998278 frc-0.1.1/src/frc/_internal_utility.py
+-rw-r--r--   0        0        0     1082 2024-04-03 13:05:36.998278 frc-0.1.1/src/frc/deps_types.py
+-rw-r--r--   0        0        0     7982 2024-04-03 13:05:36.998278 frc-0.1.1/src/frc/frc_functions.py
+-rw-r--r--   0        0        0     7184 2024-04-03 13:05:36.998278 frc-0.1.1/src/frc/utility.py
+-rw-r--r--   0        0        0     5154 1970-01-01 00:00:00.000000 frc-0.1.1/PKG-INFO
```

### Comparing `frc-0.1.0/src/frc/deps_types.py` & `frc-0.1.1/src/frc/deps_types.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-"""Shared dependencies and types module for use by other modules. Only
-includes dependencies used in two or more related modules.
-"""
-
-# Copyright (C) 2021                Department of Imaging Physics
-# All rights reserved               Faculty of Applied Sciences
-#                                   TU Delft
-# Tip ten Brink
-
-import typing
-import diplib
-import numpy
-
-__all__ = ['Img', 'Func1D', 'NoIntersectionException']
-
-# Imports are redefined to prevent warnings that imports are unused
-dip = diplib
-np = numpy
-
-Callable = typing.Callable
-Union = typing.Union
-Optional = typing.Optional
-List = typing.List
-Tuple = typing.Tuple
-
-# Img type that allows interchangeable use of diplib Image and numpy array
-Img = typing.TypeVar('Img', dip.Image, np.ndarray)
-
-# One-dimensional function that maps (an array of) floats to (an array of) floats
-Func1D = Callable[[Union[np.ndarray, float]], Union[np.ndarray, float]]
-
-
-class NoIntersectionException(ValueError):
-    """ Intersection could not be found, input did not take correct values for
-    intersection calculation. """
-    pass
+"""Shared dependencies and types module for use by other modules. Only
+includes dependencies used in two or more related modules.
+"""
+
+# Copyright (C) 2021                Department of Imaging Physics
+# All rights reserved               Faculty of Applied Sciences
+#                                   TU Delft
+# Tip ten Brink
+
+import typing
+import diplib
+import numpy
+
+__all__ = ['Img', 'Func1D', 'NoIntersectionException']
+
+# Imports are redefined to prevent warnings that imports are unused
+dip = diplib
+np = numpy
+
+Callable = typing.Callable
+Union = typing.Union
+Optional = typing.Optional
+List = typing.List
+Tuple = typing.Tuple
+
+# Img type that allows interchangeable use of diplib Image and numpy array
+Img = typing.TypeVar('Img', dip.Image, np.ndarray)
+
+# One-dimensional function that maps (an array of) floats to (an array of) floats
+Func1D = Callable[[Union[np.ndarray, float]], Union[np.ndarray, float]]
+
+
+class NoIntersectionException(ValueError):
+    """ Intersection could not be found, input did not take correct values for
+    intersection calculation. """
+    pass
```

### Comparing `frc-0.1.0/src/frc/frc_functions.py` & `frc-0.1.1/src/frc/frc_functions.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,210 +1,210 @@
-"""Functions to compute Fourier Ring Correlation of images.
-"""
-
-# Copyright (C) 2021                Department of Imaging Physics
-# All rights reserved               Faculty of Applied Sciences
-#                                   TU Delft
-# Tip ten Brink
-
-import rustfrc as r_frc
-from frc.deps_types import Img, np, dip, Callable, Optional, Func1D, Union, Tuple
-import frc._internal_utility as _util
-import frc.utility as frc_util
-
-__all__ = ['one_frc', 'two_frc', 'frc_res']
-
-
-def _frc(img1: dip.Image, img2: dip.Image) -> np.ndarray:
-    """
-    Internal function to perform Fourier Ring Correlation on a 2D dip.Image.
-    Arguments img1 and img2 are assumed to be of the same dimensions and
-    square. Do not use this function directly, but use two_frc or one_frc.
-
-    See below paper for FRC formula.
-    Van Heel, M. (1987). Similarity measures between images.
-    Ultramicroscopy, 21(1), 95–100. doi:10.1016/0304-3991(87)90010-6
-
-    :param img1: dip.Image representing the first image.
-    :param img2: dip.Image representing the second image.
-    :return: A 1D array with the FRC value for Fourier ring, with the index
-    representing the pixel distance from the origin.
-    """
-    axis_size = img1.Size(0)
-
-    # Fourier transformation of each image
-    fourier1 = dip.FourierTransform(img1, set(""))
-    fourier2 = dip.FourierTransform(img2, set(""))
-
-    # Numerator of the FRC formula
-    frc_num = np.real(dip.RadialSum(fourier1 * dip.Conjugate(fourier2), None))
-    frc_denom1 = dip.RadialSum(r_frc.sqr_abs(np.array(fourier1).astype(np.complex64)), None)
-    frc_denom2 = dip.RadialSum(r_frc.sqr_abs(np.array(fourier2).astype(np.complex64)), None)
-    frc_denom_prod = frc_denom1 * frc_denom2
-    frc_denom = np.sqrt(frc_denom_prod)
-    frc = frc_num / frc_denom
-
-    # Find last sensible FRC value (beyond axis_size / 2 there are no full
-    # rings)
-    circle_edge = int(axis_size / 2)
-
-    return frc[:circle_edge]
-
-
-def two_frc(img1: Img, img2: Img) -> np.ndarray:
-    """
-    Standard FRC using two input images, which can be either DIP images or
-    NumPy arrays. Input images must be square, have equal dimensions and
-    should have uncorrelated noise.
-
-    NOTE: The input images should be windowed to prevent FFT artifacts, i.e.
-    using a 1/8 Tukey window.
-
-    :param img1: Img representing the first image (half data set)
-    :param img2: Img representing the second image (half data set)
-    :return: A 1D array with the FRC value for Fourier ring, with the index
-    representing the pixel distance from the origin.
-    """
-    # Check if array to test if images must be converted
-    is_arr = isinstance(img1, np.ndarray)
-
-    if is_arr:
-        dip1 = dip.Image(img1)
-        dip2 = dip.Image(img2)
-    else:
-        dip1 = img1
-        dip2 = img2
-        img1 = np.array(img1)
-        img2 = np.array(img2)
-
-    if not _util.are_sizes_equal([img1, img2]):
-        raise ValueError(
-            "Images are not of exact equal dimension, or axes are not equal! Trim or pad the images first.")
-
-    return _frc(dip1, dip2)
-
-
-def one_frc(img: Img, method: int = 1) -> np.ndarray:
-    """
-        FRC using a single input image, which can be either DIP images or NumPy
-        arrays. The image is split into two by sampling binomial distributions
-        for each pixel value. The input image must be a square 2D image.
-
-        NOTE: The input image should be windowed to prevent FFT artifacts, i.e.
-        using a 1/8 Tukey window.
-
-        By default, method 1 performs one split (hence, method '1'), with the
-        second image being the difference between the original image and the
-        binomially sampled image.
-        Method 2 performs two independent splits (hence, method '2').
-        Method 1 is preferred.
-
-        :param Img img: Img representing the image (full data set)
-        :param int method: Int representing which method to use. The default is
-        method 1.
-        :returns: A 1D array with the FRC value for Fourier ring, with the index
-        representing the pixel distance from the origin.
-        """
-    # Check if array to test if images must be converted
-    is_arr = isinstance(img, np.ndarray)
-
-    # Converting is necessary for the binomial split
-    if not is_arr:
-        img = np.array(img)
-
-    if not _util.are_axes_equal(img):
-        raise ValueError("Image does not have equal axes! Trim or pad it first.")
-
-    split_method: Callable[[np.ndarray], Tuple[np.ndarray, np.ndarray]]
-    if method == 1:
-        split_method = _one_frc1
-    elif method == 2:
-        split_method = _one_frc2
-    else:
-        raise ValueError("Choose either method 1 or 2 for binomial split.")
-
-    # Split is performed
-    img_half1, img_half2 = split_method(img)
-
-    # _frc function requires DIP Image inputs
-    dip1 = dip.Image(img_half1)
-    dip2 = dip.Image(img_half2)
-
-    return _frc(dip1, dip2)
-
-
-def _one_frc2(img: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
-    """ Performs two independent binomial splits. """
-    return r_frc.binom_split(img), r_frc.binom_split(img)
-
-
-def _one_frc1(img: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
-    """ Performs a single binomial split, with the second image equal to the
-    difference of the sampled image and the input image. """
-    img_half1 = r_frc.binom_split(img)
-    return img_half1, img - img_half1
-
-
-def half_bit_threshold(img_size: int) -> Func1D:
-    """
-    1/2-bit information threshold curve for Fourier Ring Correlation.
-    Assumes a square image of image_size x image_size pixels.
-
-    Van Heel, M., & Schatz, M. (2005). Fourier shell correlation threshold
-    criteria. Journal of Structural Biology, 151(3), 250–262.
-    doi:10.1016/j.jsb.2005.05.009
-
-    :param img_size:
-    :return: A function representing the 1/2-bit information curve for a
-    specific square size, where an input of 1 for x yields the threshold
-    for the ring that is img_size pixels away from the origin and zero for
-    the ring at the origin.
-    """
-    # Number of pixels in a ring at distance 'array index' from the origin
-    # up to a distance 'img_size'
-    nr = np.array(dip.RadialSum(np.ones((img_size*2, img_size*2)), None))[:img_size]
-    nr_rt = np.sqrt(nr)
-
-    # Exact calculations
-    snr_half_set = 0.5 * np.sqrt(2) - 0.5
-    factor = np.sqrt(snr_half_set) * 2
-    half_bit_thres = (snr_half_set * nr_rt + (factor + 1)) / ((snr_half_set + 1) * nr_rt + factor)
-
-    def half_bit_thres_f(x):
-        """ Maps a number x (0 to 1) to threshold value for FRC value for pixel
-        value (0 to img_size) """
-        indexes = np.array(x * img_size).astype(np.int)
-        return half_bit_thres[indexes]
-
-    return half_bit_thres_f
-
-
-def frc_res(xs: np.ndarray, frc_curve: np.ndarray, img_size: int,
-            threshold: Optional[Union[str, Func1D]] = None) -> Tuple[float, float, Func1D]:
-    """
-    Calculate the resolution from a FRC curve.
-
-    For threshold, choose '1/7' (default) for the 1/7 threshold value or
-    'half_bit' for the 1/2-bit information curve threshold.
-
-    :param xs: Array of FRC curve x-values.
-    :param frc_curve: Array of FRC y-values corresponding to xs.
-    :param img_size: Length of the sides of the square input image
-    :param threshold: String representing which threshold curve to use
-    to calculate the resolution or actual Func1D threshold function.
-    :return: A tuple of FRC resolution as 1/intersection-x (float),
-    intersection-y (float) and the exact threshold Func1D used.
-    """
-    if threshold is None or threshold == '1/7':
-        def threshold_f(x):
-            return x*0 + 1./7
-    elif threshold == 'half_bit':
-        threshold_f = half_bit_threshold(img_size)
-    elif callable(threshold):
-        threshold_f = threshold
-    else:
-        raise ValueError("Unknown threshold!")
-
-    # Calculate intersection using FRC utility module
-    intersect_x, intersect_y = frc_util.intersection(xs, frc_curve, threshold_f)
-
-    return 1. / intersect_x, intersect_y, threshold_f
+"""Functions to compute Fourier Ring Correlation of images.
+"""
+
+# Copyright (C) 2021                Department of Imaging Physics
+# All rights reserved               Faculty of Applied Sciences
+#                                   TU Delft
+# Tip ten Brink
+
+import rustfrc as r_frc
+from frc.deps_types import Img, np, dip, Callable, Optional, Func1D, Union, Tuple
+import frc._internal_utility as _util
+import frc.utility as frc_util
+
+__all__ = ['one_frc', 'two_frc', 'frc_res']
+
+
+def _frc(img1: dip.Image, img2: dip.Image) -> np.ndarray:
+    """
+    Internal function to perform Fourier Ring Correlation on a 2D dip.Image.
+    Arguments img1 and img2 are assumed to be of the same dimensions and
+    square. Do not use this function directly, but use two_frc or one_frc.
+
+    See below paper for FRC formula.
+    Van Heel, M. (1987). Similarity measures between images.
+    Ultramicroscopy, 21(1), 95–100. doi:10.1016/0304-3991(87)90010-6
+
+    :param img1: dip.Image representing the first image.
+    :param img2: dip.Image representing the second image.
+    :return: A 1D array with the FRC value for Fourier ring, with the index
+    representing the pixel distance from the origin.
+    """
+    axis_size = img1.Size(0)
+
+    # Fourier transformation of each image
+    fourier1 = dip.FourierTransform(img1, set(""))
+    fourier2 = dip.FourierTransform(img2, set(""))
+
+    # Numerator of the FRC formula
+    frc_num = np.real(dip.RadialSum(fourier1 * dip.Conjugate(fourier2), None))
+    frc_denom1 = dip.RadialSum(r_frc.sqr_abs(np.array(fourier1).astype(np.complex64)), None)
+    frc_denom2 = dip.RadialSum(r_frc.sqr_abs(np.array(fourier2).astype(np.complex64)), None)
+    frc_denom_prod = frc_denom1 * frc_denom2
+    frc_denom = np.sqrt(frc_denom_prod)
+    frc = frc_num / frc_denom
+
+    # Find last sensible FRC value (beyond axis_size / 2 there are no full
+    # rings)
+    circle_edge = int(axis_size / 2)
+
+    return frc[:circle_edge]
+
+
+def two_frc(img1: Img, img2: Img) -> np.ndarray:
+    """
+    Standard FRC using two input images, which can be either DIP images or
+    NumPy arrays. Input images must be square, have equal dimensions and
+    should have uncorrelated noise.
+
+    NOTE: The input images should be windowed to prevent FFT artifacts, i.e.
+    using a 1/8 Tukey window.
+
+    :param img1: Img representing the first image (half data set)
+    :param img2: Img representing the second image (half data set)
+    :return: A 1D array with the FRC value for Fourier ring, with the index
+    representing the pixel distance from the origin.
+    """
+    # Check if array to test if images must be converted
+    is_arr = isinstance(img1, np.ndarray)
+
+    if is_arr:
+        dip1 = dip.Image(img1)
+        dip2 = dip.Image(img2)
+    else:
+        dip1 = img1
+        dip2 = img2
+        img1 = np.array(img1)
+        img2 = np.array(img2)
+
+    if not _util.are_sizes_equal([img1, img2]):
+        raise ValueError(
+            "Images are not of exact equal dimension, or axes are not equal! Trim or pad the images first.")
+
+    return _frc(dip1, dip2)
+
+
+def one_frc(img: Img, method: int = 1) -> np.ndarray:
+    """
+        FRC using a single input image, which can be either DIP images or NumPy
+        arrays. The image is split into two by sampling binomial distributions
+        for each pixel value. The input image must be a square 2D image.
+
+        NOTE: The input image should be windowed to prevent FFT artifacts, i.e.
+        using a 1/8 Tukey window.
+
+        By default, method 1 performs one split (hence, method '1'), with the
+        second image being the difference between the original image and the
+        binomially sampled image.
+        Method 2 performs two independent splits (hence, method '2').
+        Method 1 is preferred.
+
+        :param Img img: Img representing the image (full data set)
+        :param int method: Int representing which method to use. The default is
+        method 1.
+        :returns: A 1D array with the FRC value for Fourier ring, with the index
+        representing the pixel distance from the origin.
+        """
+    # Check if array to test if images must be converted
+    is_arr = isinstance(img, np.ndarray)
+
+    # Converting is necessary for the binomial split
+    if not is_arr:
+        img = np.array(img)
+
+    if not _util.are_axes_equal(img):
+        raise ValueError("Image does not have equal axes! Trim or pad it first.")
+
+    split_method: Callable[[np.ndarray], Tuple[np.ndarray, np.ndarray]]
+    if method == 1:
+        split_method = _one_frc1
+    elif method == 2:
+        split_method = _one_frc2
+    else:
+        raise ValueError("Choose either method 1 or 2 for binomial split.")
+
+    # Split is performed
+    img_half1, img_half2 = split_method(img)
+
+    # _frc function requires DIP Image inputs
+    dip1 = dip.Image(img_half1)
+    dip2 = dip.Image(img_half2)
+
+    return _frc(dip1, dip2)
+
+
+def _one_frc2(img: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
+    """ Performs two independent binomial splits. """
+    return r_frc.binom_split(img), r_frc.binom_split(img)
+
+
+def _one_frc1(img: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
+    """ Performs a single binomial split, with the second image equal to the
+    difference of the sampled image and the input image. """
+    img_half1 = r_frc.binom_split(img)
+    return img_half1, img - img_half1
+
+
+def half_bit_threshold(img_size: int) -> Func1D:
+    """
+    1/2-bit information threshold curve for Fourier Ring Correlation.
+    Assumes a square image of image_size x image_size pixels.
+
+    Van Heel, M., & Schatz, M. (2005). Fourier shell correlation threshold
+    criteria. Journal of Structural Biology, 151(3), 250–262.
+    doi:10.1016/j.jsb.2005.05.009
+
+    :param img_size:
+    :return: A function representing the 1/2-bit information curve for a
+    specific square size, where an input of 1 for x yields the threshold
+    for the ring that is img_size pixels away from the origin and zero for
+    the ring at the origin.
+    """
+    # Number of pixels in a ring at distance 'array index' from the origin
+    # up to a distance 'img_size'
+    nr = np.array(dip.RadialSum(np.ones((img_size*2, img_size*2)), None))[:img_size]
+    nr_rt = np.sqrt(nr)
+
+    # Exact calculations
+    snr_half_set = 0.5 * np.sqrt(2) - 0.5
+    factor = np.sqrt(snr_half_set) * 2
+    half_bit_thres = (snr_half_set * nr_rt + (factor + 1)) / ((snr_half_set + 1) * nr_rt + factor)
+
+    def half_bit_thres_f(x):
+        """ Maps a number x (0 to 1) to threshold value for FRC value for pixel
+        value (0 to img_size) """
+        indexes = np.array(x * img_size).astype(np.int)
+        return half_bit_thres[indexes]
+
+    return half_bit_thres_f
+
+
+def frc_res(xs: np.ndarray, frc_curve: np.ndarray, img_size: int,
+            threshold: Optional[Union[str, Func1D]] = None) -> Tuple[float, float, Func1D]:
+    """
+    Calculate the resolution from a FRC curve.
+
+    For threshold, choose '1/7' (default) for the 1/7 threshold value or
+    'half_bit' for the 1/2-bit information curve threshold.
+
+    :param xs: Array of FRC curve x-values.
+    :param frc_curve: Array of FRC y-values corresponding to xs.
+    :param img_size: Length of the sides of the square input image
+    :param threshold: String representing which threshold curve to use
+    to calculate the resolution or actual Func1D threshold function.
+    :return: A tuple of FRC resolution as 1/intersection-x (float),
+    intersection-y (float) and the exact threshold Func1D used.
+    """
+    if threshold is None or threshold == '1/7':
+        def threshold_f(x):
+            return x*0 + 1./7
+    elif threshold == 'half_bit':
+        threshold_f = half_bit_threshold(img_size)
+    elif callable(threshold):
+        threshold_f = threshold
+    else:
+        raise ValueError("Unknown threshold!")
+
+    # Calculate intersection using FRC utility module
+    intersect_x, intersect_y = frc_util.intersection(xs, frc_curve, threshold_f)
+
+    return 1. / intersect_x, intersect_y, threshold_f
```

### Comparing `frc-0.1.0/src/frc/utility.py` & `frc-0.1.1/src/frc/utility.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,185 +1,185 @@
-"""General useful utilities for use cases related to the library."""
-
-# Copyright (C) 2021                Department of Imaging Physics
-# All rights reserved               Faculty of Applied Sciences
-#                                   TU Delft
-# Tip ten Brink
-
-from frc.deps_types import Img, dip, np, Union, Func1D, NoIntersectionException
-import frc._internal_utility as _util
-from scipy.signal import windows as wins
-
-__all__ = ['gaussf', 'square_image', 'tukey_square', 'apply_tukey', 'intersection']
-
-
-def square_image(img: Img, add_padding=True) -> Img:
-    """
-    Transforms a 2D input image into a square image, using zero-padding by
-    default and preserving the shortest axis.
-    The padding places the input right/bottom of center. If trimming, top/
-    left portion of the image is preserved.
-    :param img: Array or DIP image that will be transformed.
-    :param add_padding: If True, add zero-padding to make the image square, otherwise trim the image
-    :return: Array or DIP image (based on input).
-    """
-    is_arr = isinstance(img, np.ndarray)
-    if not is_arr:
-        img = np.array(img)
-
-    if img.ndim == 2:
-        x_len = img.shape[0]
-        y_len = img.shape[1]
-        lengths = [x_len, y_len]
-        min_axis = np.argmin(lengths)
-        min_len = lengths[min_axis]
-        if not add_padding:
-            return _util.dipornp(img[:min_len, :min_len], is_arr, True)
-        else:
-            max_axis = 1 - min_axis
-            max_len = lengths[max_axis]
-            new_arr = np.zeros((max_len, max_len), dtype=img.dtype)
-            ax_dif = (max_len - min_len)
-            min_ax_start = int(np.ceil(ax_dif / 2.))
-            min_ax_end = max_len - min_ax_start + (0 if ax_dif % 2 == 0 else 1)
-            x_slice_start = 0 if max_axis == 0 else min_ax_start
-            x_slice_end = x_len if max_axis == 0 else min_ax_end
-            y_slice_start = 0 if max_axis == 1 else min_ax_start
-            y_slice_end = y_len if max_axis == 1 else min_ax_end
-            new_arr[x_slice_start:x_slice_end, y_slice_start:y_slice_end] = img
-            return _util.dipornp(new_arr, is_arr, True)
-    else:
-        raise ValueError("Image not 2D.")
-
-
-def gaussf(img: Img, sigmas=1) -> Img:
-    """
-    Gaussian filter using dip.Derivative.
-    :param img: np.ndarray or dip.Image, input image
-    :param sigmas: Gaussian kernel width, determines smoothing effect.
-    :return: Array or DIP Image representing filtered input.
-    """
-    is_arr = isinstance(img, np.ndarray)
-
-    if is_arr:
-        img = dip.Image(img)
-    # Gaussian filter
-    img = dip.Derivative(img, derivativeOrder=0, sigmas=[sigmas])
-
-    return _util.dipornp(img, is_arr, False)
-
-
-def tukey_square(length, alpha=0.125) -> np.ndarray:
-    """ Creates a square Tukey window mask of length x length of width
-    alpha. """
-    tukey = wins.tukey(length, alpha=alpha)
-    return np.ones((length, length)) * tukey.reshape((length, 1)) * tukey.reshape((1, length))
-
-
-def apply_tukey(img: np.ndarray, alpha=0.125) -> np.ndarray:
-    """ Apply a Tukey window to a 2D, square input image. """
-    main_size = img.shape[0]
-    if img.ndim == 2 and main_size == np.ma.size(img, axis=1):
-        return tukey_square(main_size, alpha) * img
-    else:
-        raise ValueError("Image not 2D or not square.")
-
-
-def intersection(xs: np.ndarray, ys1_f: Union[np.ndarray, Func1D], ys2_f: Func1D, tol=0.08):
-    """
-    Calculates an intersection point between a series of (x,y) points ys1
-    and a float function ys2 defined for xs.
-
-    The algorithm is not designed to be commutative. For an accurate y-
-    value the algorithm assumes uniform xs, which is also recommended.
-
-    The algorithm is not designed to be commutative. Its general workings
-    are as follows:
-
-    It first calculates points for both functions for all x values. It then
-    defines a tolerance region around the second function (y2) based on the
-    maximums of both functions (8%). To prevent strange results, the
-    functions should not diverge within the input range. It calculates a
-    series of points that are this tolerance above and below y2.
-
-    It then looks for indices in y1 that are within this region ("close").
-    It also calculates all the crossings, i.e. the y1 indices where the
-    next value will be below (if y1 started above y2) or above (if y1
-    started below y2) y2. These crossings do not take the threshold into
-    account.
-
-    The crossings, the indices after each crossing as well as the close
-    values are then looked at together as "points of interest". They are
-    then separated into contiguous groups (i.e indexes following each
-    other).
-
-    Each group (a series of indexes) is evaluated independently. The y1 and
-    y2 values of each group are evaluated and the difference computed. If
-    there are both positive and negative values (i.e. there is a crossing),
-    it is seen as a valid crossing group and no more groups are evaluated.
-
-    It then calculates the average x-value of the group and returns that as
-    the intersection point. It also returns the y-value (by inputting the
-    x-value in the y2 function).
-
-    :param xs: Array of x values for the y functions. If ys1_f is a series
-    of points, xs must correspond to those points.
-    :param ys1_f: Either a series of points or a float function.
-    :param ys2_f: A 1D array function (ndarray -> ndarray).
-    :param tol: Optional parameter that determines the tolerance for
-    the region of interest.
-    :return: x and y value of the intersection point, if it can be found.
-    """
-
-    if callable(ys1_f):
-        ys1: np.ndarray = ys2_f(xs)
-    else:
-        ys1 = ys1_f
-
-    ys2: np.ndarray = ys2_f(xs)
-    max_ys1 = np.amax(ys1)
-    max_ys2 = np.amax(ys2)
-    full_max = max(max_ys1, max_ys2)
-    tolerance = tol * full_max
-
-    hi = ys2 + tolerance
-    lo = ys2 - tolerance
-
-    close_indices = np.asarray((ys1 < hi) & (ys1 > lo)).nonzero()[0]
-    next_y = np.diff(ys1)
-    thres_y = (ys2 - ys1)[:-1]
-
-    # artificially increase first value to ensure proper crossings calculated
-    if ys1[0] == ys2[0]:
-        ys1[0] += tolerance * 0.5
-
-    if ys1[0] > ys2[0]:
-        # down
-        crossings = np.asarray((next_y < thres_y) & (thres_y < 0)).nonzero()[0]
-    else:
-        # up
-        crossings = np.asarray((next_y > thres_y) & (thres_y > 0)).nonzero()[0]
-
-    crossings = np.concatenate((crossings, crossings + 1))
-
-    close_indices = np.concatenate((close_indices, crossings))
-    close_indices = np.unique(close_indices)
-    index_groups = _util.separate_noncontiguous(close_indices)
-
-    closest = []
-    y_closest = []
-    for group in index_groups:
-        group_ys1 = ys1[group]
-        group_ys2 = ys2[group]
-        group_diff: np.ndarray = group_ys1 - group_ys2
-
-        if np.any(group_diff >= 0) and np.any(group_diff <= 0):
-            # An accurate y-value assumes uniform distribution of xs
-            x_val = np.average(xs[group])
-            y_closest.append(ys2_f(x_val))
-            closest.append(x_val)
-            break
-
-    if closest:
-        return closest[0], y_closest[0]
-    else:
-        raise NoIntersectionException("Could not find intersection!")
+"""General useful utilities for use cases related to the library."""
+
+# Copyright (C) 2021                Department of Imaging Physics
+# All rights reserved               Faculty of Applied Sciences
+#                                   TU Delft
+# Tip ten Brink
+
+from frc.deps_types import Img, dip, np, Union, Func1D, NoIntersectionException
+import frc._internal_utility as _util
+from scipy.signal import windows as wins
+
+__all__ = ['gaussf', 'square_image', 'tukey_square', 'apply_tukey', 'intersection']
+
+
+def square_image(img: Img, add_padding=True) -> Img:
+    """
+    Transforms a 2D input image into a square image, using zero-padding by
+    default and preserving the shortest axis.
+    The padding places the input right/bottom of center. If trimming, top/
+    left portion of the image is preserved.
+    :param img: Array or DIP image that will be transformed.
+    :param add_padding: If True, add zero-padding to make the image square, otherwise trim the image
+    :return: Array or DIP image (based on input).
+    """
+    is_arr = isinstance(img, np.ndarray)
+    if not is_arr:
+        img = np.array(img)
+
+    if img.ndim == 2:
+        x_len = img.shape[0]
+        y_len = img.shape[1]
+        lengths = [x_len, y_len]
+        min_axis = np.argmin(lengths)
+        min_len = lengths[min_axis]
+        if not add_padding:
+            return _util.dipornp(img[:min_len, :min_len], is_arr, True)
+        else:
+            max_axis = 1 - min_axis
+            max_len = lengths[max_axis]
+            new_arr = np.zeros((max_len, max_len), dtype=img.dtype)
+            ax_dif = (max_len - min_len)
+            min_ax_start = int(np.ceil(ax_dif / 2.))
+            min_ax_end = max_len - min_ax_start + (0 if ax_dif % 2 == 0 else 1)
+            x_slice_start = 0 if max_axis == 0 else min_ax_start
+            x_slice_end = x_len if max_axis == 0 else min_ax_end
+            y_slice_start = 0 if max_axis == 1 else min_ax_start
+            y_slice_end = y_len if max_axis == 1 else min_ax_end
+            new_arr[x_slice_start:x_slice_end, y_slice_start:y_slice_end] = img
+            return _util.dipornp(new_arr, is_arr, True)
+    else:
+        raise ValueError("Image not 2D.")
+
+
+def gaussf(img: Img, sigmas=1) -> Img:
+    """
+    Gaussian filter using dip.Derivative.
+    :param img: np.ndarray or dip.Image, input image
+    :param sigmas: Gaussian kernel width, determines smoothing effect.
+    :return: Array or DIP Image representing filtered input.
+    """
+    is_arr = isinstance(img, np.ndarray)
+
+    if is_arr:
+        img = dip.Image(img)
+    # Gaussian filter
+    img = dip.Derivative(img, derivativeOrder=0, sigmas=[sigmas])
+
+    return _util.dipornp(img, is_arr, False)
+
+
+def tukey_square(length, alpha=0.125) -> np.ndarray:
+    """ Creates a square Tukey window mask of length x length of width
+    alpha. """
+    tukey = wins.tukey(length, alpha=alpha)
+    return np.ones((length, length)) * tukey.reshape((length, 1)) * tukey.reshape((1, length))
+
+
+def apply_tukey(img: np.ndarray, alpha=0.125) -> np.ndarray:
+    """ Apply a Tukey window to a 2D, square input image. """
+    main_size = img.shape[0]
+    if img.ndim == 2 and main_size == np.ma.size(img, axis=1):
+        return tukey_square(main_size, alpha) * img
+    else:
+        raise ValueError("Image not 2D or not square.")
+
+
+def intersection(xs: np.ndarray, ys1_f: Union[np.ndarray, Func1D], ys2_f: Func1D, tol=0.08):
+    """
+    Calculates an intersection point between a series of (x,y) points ys1
+    and a float function ys2 defined for xs.
+
+    The algorithm is not designed to be commutative. For an accurate y-
+    value the algorithm assumes uniform xs, which is also recommended.
+
+    The algorithm is not designed to be commutative. Its general workings
+    are as follows:
+
+    It first calculates points for both functions for all x values. It then
+    defines a tolerance region around the second function (y2) based on the
+    maximums of both functions (8%). To prevent strange results, the
+    functions should not diverge within the input range. It calculates a
+    series of points that are this tolerance above and below y2.
+
+    It then looks for indices in y1 that are within this region ("close").
+    It also calculates all the crossings, i.e. the y1 indices where the
+    next value will be below (if y1 started above y2) or above (if y1
+    started below y2) y2. These crossings do not take the threshold into
+    account.
+
+    The crossings, the indices after each crossing as well as the close
+    values are then looked at together as "points of interest". They are
+    then separated into contiguous groups (i.e indexes following each
+    other).
+
+    Each group (a series of indexes) is evaluated independently. The y1 and
+    y2 values of each group are evaluated and the difference computed. If
+    there are both positive and negative values (i.e. there is a crossing),
+    it is seen as a valid crossing group and no more groups are evaluated.
+
+    It then calculates the average x-value of the group and returns that as
+    the intersection point. It also returns the y-value (by inputting the
+    x-value in the y2 function).
+
+    :param xs: Array of x values for the y functions. If ys1_f is a series
+    of points, xs must correspond to those points.
+    :param ys1_f: Either a series of points or a float function.
+    :param ys2_f: A 1D array function (ndarray -> ndarray).
+    :param tol: Optional parameter that determines the tolerance for
+    the region of interest.
+    :return: x and y value of the intersection point, if it can be found.
+    """
+
+    if callable(ys1_f):
+        ys1: np.ndarray = ys2_f(xs)
+    else:
+        ys1 = ys1_f
+
+    ys2: np.ndarray = ys2_f(xs)
+    max_ys1 = np.amax(ys1)
+    max_ys2 = np.amax(ys2)
+    full_max = max(max_ys1, max_ys2)
+    tolerance = tol * full_max
+
+    hi = ys2 + tolerance
+    lo = ys2 - tolerance
+
+    close_indices = np.asarray((ys1 < hi) & (ys1 > lo)).nonzero()[0]
+    next_y = np.diff(ys1)
+    thres_y = (ys2 - ys1)[:-1]
+
+    # artificially increase first value to ensure proper crossings calculated
+    if ys1[0] == ys2[0]:
+        ys1[0] += tolerance * 0.5
+
+    if ys1[0] > ys2[0]:
+        # down
+        crossings = np.asarray((next_y < thres_y) & (thres_y < 0)).nonzero()[0]
+    else:
+        # up
+        crossings = np.asarray((next_y > thres_y) & (thres_y > 0)).nonzero()[0]
+
+    crossings = np.concatenate((crossings, crossings + 1))
+
+    close_indices = np.concatenate((close_indices, crossings))
+    close_indices = np.unique(close_indices)
+    index_groups = _util.separate_noncontiguous(close_indices)
+
+    closest = []
+    y_closest = []
+    for group in index_groups:
+        group_ys1 = ys1[group]
+        group_ys2 = ys2[group]
+        group_diff: np.ndarray = group_ys1 - group_ys2
+
+        if np.any(group_diff >= 0) and np.any(group_diff <= 0):
+            # An accurate y-value assumes uniform distribution of xs
+            x_val = np.average(xs[group])
+            y_closest.append(ys2_f(x_val))
+            closest.append(x_val)
+            break
+
+    if closest:
+        return closest[0], y_closest[0]
+    else:
+        raise NoIntersectionException("Could not find intersection!")
```

### Comparing `frc-0.1.0/setup.py` & `frc-0.1.1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,84 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+# frc
 
-package_dir = \
-{'': 'src'}
+`frc` is a Python library for calculating Fourier Ring Correlation (FRC) curves and their associated resolution.
 
-packages = \
-['frc']
+This is particularly useful for determining the resolution of images taken with super-resolution microscopy techniques.
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['diplib>=3.1.0,<4.0.0',
- 'numpy>=1.18,<2.0',
- 'rustfrc>=1.1.2,<2.0.0',
- 'scipy>=1.3,<2.0']
-
-setup_kwargs = {
-    'name': 'frc',
-    'version': '0.1.0',
-    'description': 'Library for computing Fourier Ring Correlation (FRC) curves and using them to determine image resolution.',
-    'long_description': '# frc\n\n`frc` is a Python library for calculating Fourier Ring Correlation (FRC) curves and their associated resolution.\n\nThis is particularly useful for determining the resolution of images taken with super-resolution microscopy techniques.\n\nIts most computationally intensive functions are all implemented either in NumPy or Rust, making this library very fast.\n\n### Fourier Ring Correlation\n\nIntroduced in 1982, Fourier Ring Correlation compares two 2D images, which are assumed to be noise-independent. In Fourier space, mage structure dominates the lower spatial frequencies (in the Fourier domain), while noise dominates at the higher frequencies.\n\nIn Fourier space, there are rings of constant spatial frequency around the origin. By calculating the correlation between the rings in the two images, you get the FRC curve:\n\n![formula](https://render.githubusercontent.com/render/math?math=%5Ccolor%7Bgray%7D%5Ctext%7BFRC%7D%28q%29%20%3D%20%5Cfrac%7B%5Csum_%7B%5Cvec%7Bq%7D%20%5Cin%20%5Ctext%7Bcircle%7D%7D%20%5Cwidehat%7Bf_1%7D%28%5Cvec%7Bq%7D%29%20%5Cwidehat%7Bf_2%7D%28%5Cvec%7Bq%7D%29%5E%7B%5Ctextbf%7B%2A%7D%7D%7D%7B%5Csqrt%7B%5Csum_%7B%5Cvec%7Bq%7D%20%5Cin%20%5Ctext%7Bcircle%7D%7D%20%5Clvert%5Cwidehat%7Bf_1%7D%28%5Cvec%7Bq%7D%29%5Crvert%5E2%7D%20%5Csqrt%7B%5Csum_%7B%5Cvec%7Bq%7D%20%5Cin%20%5Ctext%7Bcircle%7D%7D%20%5Clvert%5Cwidehat%7Bf_2%7D%28%5Cvec%7Bq%7D%29%5Crvert%5E2%7D%7D%0A)\n\nSee the accompanying `FRC.pdf` for additional details.\n\nAt some spatial frequency, the signal cannot be separated from the noise. What spatial frequency exactly depends on what threshold function is used. The standard 0.143 and 1/2-bit thresholds are both available, as well as an algorithm to compute the intersection and resulting resolution.\n\n\n\n### Installation\n\nYou can download this library from PyPI:\n\n```shell\npip install frc\n```\n\nThis library depends on [tmtenbrink/rustfrc](https://www.github.com/tmtenbrink/rustfrc), [DIPlib](https://github.com/DIPlib/diplib), [scipy](https://scipy.org/) and of course, [numpy](https://numpy.org/).\n\n### Usage\n\nThe code snippet below (which for illustration purposes assumes you have a numpy array or DIP image representing your input, its associated scale and also matplotlib to plot the result) will calculate the FRC curve and the associated resolution using the standard 1/7 threshold.\n\n```python\nimport frc\nimport numpy as np\nimport matplotlib.pyplot as plt\n\n... # get an image and scale\n\nimg = np.array(img)\n# Input can be a numpy array or DIP image\nimg = frc.util.square_image(img, add_padding=False)\nimg = frc.util.apply_tukey(img)\n# Apply 1FRC technique\nfrc_curve = frc.one_frc(img)\n\nimg_size = img.shape[0]\nxs_pix = np.arange(len(frc_curve)) / img_size\n# scale has units [pixels <length unit>^-1] corresponding to original image\nxs_nm_freq = xs_pix * scale\nfrc_res, res_y, thres = frc.frc_res(xs_nm_freq, frc_curve, img_size)\nplt.plot(xs_nm_freq, thres(xs_nm_freq))\nplt.plot(xs_nm_freq, frc_curve)\nplt.show()\n```',
-    'author': 'Tip ten Brink',
-    'author_email': 'T.M.tenBrink@student.tudelft.nl',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': None,
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7,<3.10',
-}
+Its most computationally intensive functions are all implemented either in NumPy or Rust, making this library quite performant.
 
+### Fourier Ring Correlation
 
-setup(**setup_kwargs)
+Introduced in 1982, Fourier Ring Correlation compares two 2D images, which are assumed to be noise-independent. In Fourier space, mage structure dominates the lower spatial frequencies (in the Fourier domain), while noise dominates at the higher frequencies.
+
+In Fourier space, there are rings of constant spatial frequency around the origin. By calculating the correlation between the rings in the two images (varying the spatial frequency), you can compute an FRC curve (y-axis: correlation, x-axis: spatial frequency).
+
+At some spatial frequency, the signal cannot be separated from the noise. What spatial frequency exactly depends on what threshold function is used. The standard 0.143 and 1/2-bit thresholds are both available, as well as an algorithm to compute the intersection and resulting resolution.
+
+For additional information about Fourier Ring Correlation, see [R.P.J. Nieuwenhuizen et al. (2013)](https://doi.org/10.1038/nmeth.2448).
+
+#### 1FRC
+
+FRC requires two noise-independent images to work. However, modern cameras are often shot noise-limited (Poisson noise). This library includes a new method due to Bernd Rieger and Sjoerd Stallinga (Department of Imaging Physics, TU Delft), called 1FRC, which uses a technique called binomial splitting to derive two images from a single one, where the pixel counts of the derived images are independently Poisson noise distributed.
+
+They have an upcoming paper detailing the method and providing additional theoretical and experimental justification. This library was produced for my bachelor thesis (which focused on 1FRC) and was supervised by Bernd Rieger. [The bachelor thesis can be found here.](http://resolver.tudelft.nl/uuid:abdc31f6-6ecd-4c1b-a0c4-53711829467a).
+
+### Installation
+
+You can download this library from PyPI:
+
+```shell
+pip install frc
+```
+
+This library depends on [tmtenbrink/rustfrc](https://www.github.com/tmtenbrink/rustfrc), [DIPlib](https://github.com/DIPlib/diplib), [scipy](https://scipy.org/) and of course, [numpy](https://numpy.org/).
+
+### Usage
+
+The code snippet below (which for illustration purposes assumes you have a numpy array or DIP image representing your input, its associated scale and also matplotlib to plot the result) will calculate the FRC curve and the associated resolution using the standard 1/7 threshold.
+
+```python
+import frc
+import numpy as np
+import matplotlib.pyplot as plt
+
+... # get an image and scale
+
+img = np.array(img)
+# Input can be a numpy array or DIP image
+img = frc.util.square_image(img, add_padding=False)
+img = frc.util.apply_tukey(img)
+# Apply 1FRC technique
+frc_curve = frc.one_frc(img)
+
+img_size = img.shape[0]
+xs_pix = np.arange(len(frc_curve)) / img_size
+# scale has units [pixels <length unit>^-1] corresponding to original image
+xs_nm_freq = xs_pix * scale
+frc_res, res_y, thres = frc.frc_res(xs_nm_freq, frc_curve, img_size)
+plt.plot(xs_nm_freq, thres(xs_nm_freq))
+plt.plot(xs_nm_freq, frc_curve)
+plt.show()
+```
+
+#### Troubleshooting
+
+If you cannot find an intersection (`NoIntersectionException`), be sure to plot the curve without using the `frc_res` method and see if there even is an intersection. For example:
+
+```python
+import frc
+import numpy as np
+import matplotlib.pyplot as plt
+
+img = ... # get an image and scale
+
+# Apply 1FRC technique
+frc_curve = frc.one_frc(img)
+img_size = img.shape[0]
+xs_pix = np.arange(len(frc_curve)) / img_size
+# scale has units [pixels <length unit>^-1] corresponding to original image
+xs_nm_freq = xs_pix * scale
+plt.plot(xs_nm_freq, frc_curve)
+plt.show()
+```
+
+For images with a significant amount of non-Poisson noise, the 1FRC method has been shown to fail (adjustments are possible).
```

