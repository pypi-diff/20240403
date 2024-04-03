# Comparing `tmp/svc_toolkit-1.0.0.tar.gz` & `tmp/svc_toolkit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svc_toolkit-1.0.0.tar", max compression
+gzip compressed data, was "svc_toolkit-1.0.1.tar", max compression
```

## Comparing `svc_toolkit-1.0.0.tar` & `svc_toolkit-1.0.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0      267 2024-03-29 05:41:39.161642 svc_toolkit-1.0.0/README.md
--rw-r--r--   0        0        0     1450 2024-04-03 17:38:49.215490 svc_toolkit-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-03 11:29:46.323243 svc_toolkit-1.0.0/src/vc_toolkit/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 11:29:59.020663 svc_toolkit-1.0.0/src/vc_toolkit/conversion/__init__.py
--rw-r--r--   0        0        0      787 2024-04-03 06:50:41.723163 svc_toolkit-1.0.0/src/vc_toolkit/conversion/converter.py
--rw-r--r--   0        0        0     2443 2024-04-02 13:30:25.496921 svc_toolkit-1.0.0/src/vc_toolkit/conversion/converter_trainer.py
--rw-r--r--   0        0        0     1056 2024-04-01 10:08:33.620466 svc_toolkit-1.0.0/src/vc_toolkit/conversion/mixer.py
--rw-r--r--   0        0        0    12669 2024-04-01 10:08:33.619605 svc_toolkit-1.0.0/src/vc_toolkit/img/icon.png
--rw-r--r--   0        0        0    31498 2024-03-31 04:03:54.961742 svc_toolkit-1.0.0/src/vc_toolkit/img/loading.gif
--rw-r--r--   0        0        0     2363 2024-04-03 14:16:22.182486 svc_toolkit-1.0.0/src/vc_toolkit/main.py
--rw-r--r--   0        0        0      214 2024-04-01 10:08:33.619904 svc_toolkit-1.0.0/src/vc_toolkit/models/manifest.yml
--rw-r--r--   0        0        0        0 2024-04-03 11:29:56.944821 svc_toolkit-1.0.0/src/vc_toolkit/presenter/__init__.py
--rw-r--r--   0        0        0      293 2024-02-02 01:04:50.556319 svc_toolkit-1.0.0/src/vc_toolkit/presenter/common.py
--rw-r--r--   0        0        0      825 2024-04-03 10:58:50.553108 svc_toolkit-1.0.0/src/vc_toolkit/presenter/conversion.py
--rw-r--r--   0        0        0      611 2024-04-03 11:02:26.465772 svc_toolkit-1.0.0/src/vc_toolkit/presenter/mixing.py
--rw-r--r--   0        0        0     2591 2024-04-03 11:02:26.465729 svc_toolkit-1.0.0/src/vc_toolkit/presenter/separation.py
--rw-r--r--   0        0        0      673 2024-04-03 11:02:26.460803 svc_toolkit-1.0.0/src/vc_toolkit/presenter/training.py
--rw-r--r--   0        0        0        0 2024-04-03 11:29:52.077076 svc_toolkit-1.0.0/src/vc_toolkit/separation/__init__.py
--rw-r--r--   0        0        0      987 2024-03-29 05:41:39.165414 svc_toolkit-1.0.0/src/vc_toolkit/separation/audio.py
--rw-r--r--   0        0        0      196 2024-03-29 05:41:39.165763 svc_toolkit-1.0.0/src/vc_toolkit/separation/constants.py
--rw-r--r--   0        0        0     7063 2024-04-03 11:02:26.456563 svc_toolkit-1.0.0/src/vc_toolkit/separation/data.py
--rw-r--r--   0        0        0     2166 2024-04-03 11:02:26.451566 svc_toolkit-1.0.0/src/vc_toolkit/separation/evaluator.py
--rw-r--r--   0        0        0     1985 2024-03-12 23:58:32.947458 svc_toolkit-1.0.0/src/vc_toolkit/separation/logger.py
--rw-r--r--   0        0        0     7133 2024-04-02 16:52:09.533746 svc_toolkit-1.0.0/src/vc_toolkit/separation/models.py
--rw-r--r--   0        0        0     3578 2024-04-03 11:02:26.446431 svc_toolkit-1.0.0/src/vc_toolkit/separation/preprocess.py
--rw-r--r--   0        0        0     4695 2024-04-03 11:02:26.446368 svc_toolkit-1.0.0/src/vc_toolkit/separation/separator.py
--rw-r--r--   0        0        0      751 2024-04-03 11:02:26.434628 svc_toolkit-1.0.0/src/vc_toolkit/separation/utility.py
--rw-r--r--   0        0        0     1289 2024-04-03 11:02:26.434295 svc_toolkit-1.0.0/src/vc_toolkit/separation_evaluation.py
--rw-r--r--   0        0        0      976 2024-04-03 11:02:26.432789 svc_toolkit-1.0.0/src/vc_toolkit/separation_preprocess.py
--rw-r--r--   0        0        0     3916 2024-04-03 11:02:24.294196 svc_toolkit-1.0.0/src/vc_toolkit/separation_train.py
--rw-r--r--   0        0        0        0 2024-04-03 11:29:50.803353 svc_toolkit-1.0.0/src/vc_toolkit/utility/__init__.py
--rw-r--r--   0        0        0      239 2024-04-01 10:08:33.622860 svc_toolkit-1.0.0/src/vc_toolkit/utility/functions.py
--rw-r--r--   0        0        0        0 2024-04-03 11:29:49.453738 svc_toolkit-1.0.0/src/vc_toolkit/widget/__init__.py
--rw-r--r--   0        0        0     7941 2024-04-02 19:23:15.771626 svc_toolkit-1.0.0/src/vc_toolkit/widget/common.py
--rw-r--r--   0        0        0     8010 2024-04-03 15:08:54.274873 svc_toolkit-1.0.0/src/vc_toolkit/widget/conversion.py
--rw-r--r--   0        0        0      760 2024-04-03 15:13:29.736064 svc_toolkit-1.0.0/src/vc_toolkit/widget/loading_overlay.py
--rw-r--r--   0        0        0      993 2024-04-01 10:08:33.624228 svc_toolkit-1.0.0/src/vc_toolkit/widget/loading_window.py
--rw-r--r--   0        0        0      578 2024-04-02 19:58:26.288401 svc_toolkit-1.0.0/src/vc_toolkit/widget/main_window.py
--rw-r--r--   0        0        0     3324 2024-04-03 11:02:26.434307 svc_toolkit-1.0.0/src/vc_toolkit/widget/mixing.py
--rw-r--r--   0        0        0     4678 2024-04-03 11:01:56.679887 svc_toolkit-1.0.0/src/vc_toolkit/widget/separation.py
--rw-r--r--   0        0        0     5277 2024-04-03 11:04:19.010345 svc_toolkit-1.0.0/src/vc_toolkit/widget/training.py
--rw-r--r--   0        0        0     1287 1970-01-01 00:00:00.000000 svc_toolkit-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      490 2024-04-03 21:10:25.723821 svc_toolkit-1.0.1/README.md
+-rw-r--r--   0        0        0     1455 2024-04-03 21:10:25.723821 svc_toolkit-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-03 21:10:25.723821 svc_toolkit-1.0.1/src/svc_toolkit/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 21:10:25.723821 svc_toolkit-1.0.1/src/svc_toolkit/conversion/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-03 21:10:25.723821 svc_toolkit-1.0.1/src/svc_toolkit/conversion/converter.py
+-rw-r--r--   0        0        0     2443 2024-04-03 21:10:25.723821 svc_toolkit-1.0.1/src/svc_toolkit/conversion/converter_trainer.py
+-rw-r--r--   0        0        0     1056 2024-04-03 21:10:25.723821 svc_toolkit-1.0.1/src/svc_toolkit/conversion/mixer.py
+-rw-r--r--   0        0        0    12669 2024-04-03 21:10:25.723821 svc_toolkit-1.0.1/src/svc_toolkit/img/icon.png
+-rw-r--r--   0        0        0    31498 2024-04-03 21:10:25.723821 svc_toolkit-1.0.1/src/svc_toolkit/img/loading.gif
+-rw-r--r--   0        0        0     2377 2024-04-03 21:10:25.723821 svc_toolkit-1.0.1/src/svc_toolkit/main.py
+-rw-r--r--   0        0        0      214 2024-04-03 21:10:25.723821 svc_toolkit-1.0.1/src/svc_toolkit/models/manifest.yml
+-rw-r--r--   0        0        0        0 2024-04-03 21:10:25.723821 svc_toolkit-1.0.1/src/svc_toolkit/presenter/__init__.py
+-rw-r--r--   0        0        0      293 2024-04-03 21:10:25.723821 svc_toolkit-1.0.1/src/svc_toolkit/presenter/common.py
+-rw-r--r--   0        0        0      828 2024-04-03 21:10:25.723821 svc_toolkit-1.0.1/src/svc_toolkit/presenter/conversion.py
+-rw-r--r--   0        0        0      613 2024-04-03 21:10:25.723821 svc_toolkit-1.0.1/src/svc_toolkit/presenter/mixing.py
+-rw-r--r--   0        0        0     2595 2024-04-03 21:10:25.723821 svc_toolkit-1.0.1/src/svc_toolkit/presenter/separation.py
+-rw-r--r--   0        0        0      675 2024-04-03 21:10:25.727821 svc_toolkit-1.0.1/src/svc_toolkit/presenter/training.py
+-rw-r--r--   0        0        0        0 2024-04-03 21:10:25.727821 svc_toolkit-1.0.1/src/svc_toolkit/separation/__init__.py
+-rw-r--r--   0        0        0      987 2024-04-03 21:10:25.727821 svc_toolkit-1.0.1/src/svc_toolkit/separation/audio.py
+-rw-r--r--   0        0        0      196 2024-04-03 21:10:25.727821 svc_toolkit-1.0.1/src/svc_toolkit/separation/constants.py
+-rw-r--r--   0        0        0     7065 2024-04-03 21:10:25.727821 svc_toolkit-1.0.1/src/svc_toolkit/separation/data.py
+-rw-r--r--   0        0        0     2168 2024-04-03 21:10:25.727821 svc_toolkit-1.0.1/src/svc_toolkit/separation/evaluator.py
+-rw-r--r--   0        0        0     1985 2024-04-03 21:10:25.727821 svc_toolkit-1.0.1/src/svc_toolkit/separation/logger.py
+-rw-r--r--   0        0        0     7133 2024-04-03 21:10:25.727821 svc_toolkit-1.0.1/src/svc_toolkit/separation/models.py
+-rw-r--r--   0        0        0     3580 2024-04-03 21:10:25.727821 svc_toolkit-1.0.1/src/svc_toolkit/separation/preprocess.py
+-rw-r--r--   0        0        0     4697 2024-04-03 21:10:25.727821 svc_toolkit-1.0.1/src/svc_toolkit/separation/separator.py
+-rw-r--r--   0        0        0      752 2024-04-03 21:10:25.727821 svc_toolkit-1.0.1/src/svc_toolkit/separation/utility.py
+-rw-r--r--   0        0        0     1290 2024-04-03 21:10:25.727821 svc_toolkit-1.0.1/src/svc_toolkit/separation_evaluation.py
+-rw-r--r--   0        0        0      978 2024-04-03 21:10:25.727821 svc_toolkit-1.0.1/src/svc_toolkit/separation_preprocess.py
+-rw-r--r--   0        0        0     3922 2024-04-03 21:10:25.727821 svc_toolkit-1.0.1/src/svc_toolkit/separation_train.py
+-rw-r--r--   0        0        0        0 2024-04-03 21:10:25.727821 svc_toolkit-1.0.1/src/svc_toolkit/utility/__init__.py
+-rw-r--r--   0        0        0      239 2024-04-03 21:10:25.727821 svc_toolkit-1.0.1/src/svc_toolkit/utility/functions.py
+-rw-r--r--   0        0        0        0 2024-04-03 21:10:25.727821 svc_toolkit-1.0.1/src/svc_toolkit/widget/__init__.py
+-rw-r--r--   0        0        0     7941 2024-04-03 21:10:25.727821 svc_toolkit-1.0.1/src/svc_toolkit/widget/common.py
+-rw-r--r--   0        0        0     7972 2024-04-03 21:10:25.727821 svc_toolkit-1.0.1/src/svc_toolkit/widget/conversion.py
+-rw-r--r--   0        0        0      760 2024-04-03 21:10:25.727821 svc_toolkit-1.0.1/src/svc_toolkit/widget/loading_overlay.py
+-rw-r--r--   0        0        0      993 2024-04-03 21:10:25.727821 svc_toolkit-1.0.1/src/svc_toolkit/widget/loading_window.py
+-rw-r--r--   0        0        0      578 2024-04-03 21:10:25.727821 svc_toolkit-1.0.1/src/svc_toolkit/widget/main_window.py
+-rw-r--r--   0        0        0     3325 2024-04-03 21:10:25.727821 svc_toolkit-1.0.1/src/svc_toolkit/widget/mixing.py
+-rw-r--r--   0        0        0     4679 2024-04-03 21:10:25.727821 svc_toolkit-1.0.1/src/svc_toolkit/widget/separation.py
+-rw-r--r--   0        0        0     5279 2024-04-03 21:10:25.727821 svc_toolkit-1.0.1/src/svc_toolkit/widget/training.py
+-rw-r--r--   0        0        0     1510 1970-01-01 00:00:00.000000 svc_toolkit-1.0.1/PKG-INFO
```

### Comparing `svc_toolkit-1.0.0/pyproject.toml` & `svc_toolkit-1.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "svc-toolkit"
-version = "1.0.0"
+version = "1.0.1"
 description = "A self-contained singing voice conversion toolkit."
 authors = ["jljl1337 <lckjack123@gmail.com>"]
 license = ""
 readme = "README.md"
 #repository = ""
 #documentation = ""
 classifiers = [
     "Operating System :: OS Independent",
 ]
 packages = [
-   { include = "vc_toolkit", from = "src" },
+   { include = "svc_toolkit", from = "src" },
 ]
 
 [tool.poetry.scripts]
-vct = "vc_toolkit.main:main"
-vspreprocess = "vc_toolkit.separation_preprocess:main"
-vstrain = "vc_toolkit.separation_train:main"
-vseval = "vc_toolkit.separation_train:main"
+vct = "svc_toolkit.main:main"
+vspreprocess = "svc_toolkit.separation_preprocess:main"
+vstrain = "svc_toolkit.separation_train:main"
+vseval = "svc_toolkit.separation_train:main"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.13"
 numpy = "1.26.3"
 scipy = "1.12.0"
 pyyaml = "6.0.1"
 torch = "2.1.1"
```

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/conversion/converter.py` & `svc_toolkit-1.0.1/src/svc_toolkit/conversion/converter.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/conversion/converter_trainer.py` & `svc_toolkit-1.0.1/src/svc_toolkit/conversion/converter_trainer.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/conversion/mixer.py` & `svc_toolkit-1.0.1/src/svc_toolkit/conversion/mixer.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/img/icon.png` & `svc_toolkit-1.0.1/src/svc_toolkit/img/icon.png`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/img/loading.gif` & `svc_toolkit-1.0.1/src/svc_toolkit/img/loading.gif`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/main.py` & `svc_toolkit-1.0.1/src/svc_toolkit/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 import os
 
 from PySide6.QtWidgets import QApplication
 from PySide6.QtGui import QIcon
 
-from vc_toolkit.widget.loading_window import LoadingWindow
+from svc_toolkit.widget.loading_window import LoadingWindow
 
 def main():
     app = QApplication([])
 
     app.setWindowIcon(QIcon(os.path.join(os.path.dirname(__file__), 'img/icon.png')))
 
     # Show loading window before importing other modules and creating main window
     loading_window = LoadingWindow()
     loading_window.show()
     app.processEvents()
 
-    from vc_toolkit.widget.main_window import MainWindow
-    from vc_toolkit.widget.separation import SeparationWidget
-    from vc_toolkit.widget.training import TrainingWidget
-    from vc_toolkit.widget.conversion import ConversionWidget
-    from vc_toolkit.widget.mixing import MixingWidget
-    from vc_toolkit.separation.separator import SeparatorFactory
-    from vc_toolkit.conversion.converter_trainer import ConverterTrainerFactory
-    from vc_toolkit.conversion.converter import ConverterFactory
-    from vc_toolkit.conversion.mixer import MixerFactory
-    from vc_toolkit.presenter.separation import SeparationPresenter
-    from vc_toolkit.presenter.training import TrainingPresenter
-    from vc_toolkit.presenter.conversion import ConversionPresenter
-    from vc_toolkit.presenter.mixing import MixingPresenter
+    from svc_toolkit.widget.main_window import MainWindow
+    from svc_toolkit.widget.separation import SeparationWidget
+    from svc_toolkit.widget.training import TrainingWidget
+    from svc_toolkit.widget.conversion import ConversionWidget
+    from svc_toolkit.widget.mixing import MixingWidget
+    from svc_toolkit.separation.separator import SeparatorFactory
+    from svc_toolkit.conversion.converter_trainer import ConverterTrainerFactory
+    from svc_toolkit.conversion.converter import ConverterFactory
+    from svc_toolkit.conversion.mixer import MixerFactory
+    from svc_toolkit.presenter.separation import SeparationPresenter
+    from svc_toolkit.presenter.training import TrainingPresenter
+    from svc_toolkit.presenter.conversion import ConversionPresenter
+    from svc_toolkit.presenter.mixing import MixingPresenter
 
     vocal_separation_widget = SeparationWidget()
     separator_factory = SeparatorFactory()
     vocal_separation_presenter = SeparationPresenter(vocal_separation_widget, separator_factory)
 
     training_widget = TrainingWidget()
     trainer_factory = ConverterTrainerFactory()
```

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/presenter/conversion.py` & `svc_toolkit-1.0.1/src/svc_toolkit/presenter/conversion.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from vc_toolkit.widget.conversion import ConversionWidget
-from vc_toolkit.conversion.converter import ConverterFactory
-from vc_toolkit.presenter.common import get_available_device
+from svc_toolkit.widget.conversion import ConversionWidget
+from svc_toolkit.conversion.converter import ConverterFactory
+from svc_toolkit.presenter.common import get_available_device
 
 class ConversionPresenter:
     def __init__(self, view: ConversionWidget, model_factory: ConverterFactory):
         self.view = view
         self.model_factory = model_factory
 
         self.view.set_device_list(get_available_device())
```

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/presenter/mixing.py` & `svc_toolkit-1.0.1/src/svc_toolkit/presenter/mixing.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from vc_toolkit.widget.mixing import MixingWidget
-from vc_toolkit.conversion.mixer import MixerFactory
+from svc_toolkit.widget.mixing import MixingWidget
+from svc_toolkit.conversion.mixer import MixerFactory
 
 class MixingPresenter:
     def __init__(self, view: MixingWidget, mixer_factory: MixerFactory):
         self.view = view
         self.mixer_factory = mixer_factory
 
         self.view.set_mixer_function(self.mix)
```

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/presenter/separation.py` & `svc_toolkit-1.0.1/src/svc_toolkit/presenter/separation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 from huggingface_hub import hf_hub_download
 
-from vc_toolkit.utility.functions import load_yaml
-from vc_toolkit.widget.separation import SeparationWidget
-from vc_toolkit.separation.separator import SeparatorFactory
-from vc_toolkit.presenter.common import get_available_device
+from svc_toolkit.utility.functions import load_yaml
+from svc_toolkit.widget.separation import SeparationWidget
+from svc_toolkit.separation.separator import SeparatorFactory
+from svc_toolkit.presenter.common import get_available_device
 
 VOCAL_FILE_NAME = 'vocal.wav'
 NON_VOCAL_FILE_NAME = 'instrument.wav'
 
 class SeparationPresenter:
     def __init__(self, view: SeparationWidget, model_factory: SeparatorFactory):
         self.view = view
```

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/presenter/training.py` & `svc_toolkit-1.0.1/src/svc_toolkit/presenter/training.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from vc_toolkit.widget.training import TrainingWidget
-from vc_toolkit.conversion.converter_trainer import ConverterTrainerFactory
+from svc_toolkit.widget.training import TrainingWidget
+from svc_toolkit.conversion.converter_trainer import ConverterTrainerFactory
 
 class TrainingPresenter:
     def __init__(self, view: TrainingWidget, trainer_factory: ConverterTrainerFactory):
         self.view = view
         self.trainer = trainer_factory.create()
 
         self.view.set_preprocess_function(self.preprocess)
```

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/separation/audio.py` & `svc_toolkit-1.0.1/src/svc_toolkit/separation/audio.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/separation/data.py` & `svc_toolkit-1.0.1/src/svc_toolkit/separation/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 import numpy as np
 import pytorch_lightning as pl
 from pandas import read_csv
 from torch.utils.data import Dataset, DataLoader
 from pytorch_lightning.trainer.states import TrainerFn
 from tqdm import tqdm
 
-from vc_toolkit.separation.audio import load, to_magnitude
-from vc_toolkit.separation.constants import CSV_MIXTURE_PATH_COLUMN, CSV_STEM_PATH_COLUMN, NYQUIST, ZERO, NEGLECT_FREQUENCY_OPTIONS
+from svc_toolkit.separation.audio import load, to_magnitude
+from svc_toolkit.separation.constants import CSV_MIXTURE_PATH_COLUMN, CSV_STEM_PATH_COLUMN, NYQUIST, ZERO, NEGLECT_FREQUENCY_OPTIONS
 
 class MagnitudeRandomDataset(Dataset):
     def __init__(
         self,
         mixture_path_list: list[str],
         stem_path_list: list[str],
         expand_factor: float,
```

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/separation/evaluator.py` & `svc_toolkit-1.0.1/src/svc_toolkit/separation/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch
 import pandas as pd
 from torchmetrics.audio import SignalDistortionRatio, ScaleInvariantSignalDistortionRatio
 from tqdm import tqdm
 
-from vc_toolkit.separation.separator import Separator
-from vc_toolkit.separation.constants import CSV_SONG_COLUMN, CSV_MIXTURE_PATH_COLUMN, CSV_STEM_PATH_COLUMN
+from svc_toolkit.separation.separator import Separator
+from svc_toolkit.separation.constants import CSV_SONG_COLUMN, CSV_MIXTURE_PATH_COLUMN, CSV_STEM_PATH_COLUMN
 
 class Evaluator:
     def __init__(self, model_dir: str, device: str, precision: str, last: bool):
         self.separator = Separator(model_dir, device, precision, last)
         self.sdr = SignalDistortionRatio()
         self.sisdr = ScaleInvariantSignalDistortionRatio()
```

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/separation/logger.py` & `svc_toolkit-1.0.1/src/svc_toolkit/separation/logger.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/separation/models.py` & `svc_toolkit-1.0.1/src/svc_toolkit/separation/models.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/separation/preprocess.py` & `svc_toolkit-1.0.1/src/svc_toolkit/separation/preprocess.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 import pandas as pd
 from tqdm import tqdm
 from sklearn.model_selection import train_test_split
 from moisesdb.dataset import MoisesDB
 from moisesdb.track import MoisesDBTrack
 from moisesdb.defaults import all_stems, default_sample_rate
 
-import vc_toolkit.separation.audio as audio
-from vc_toolkit.separation.constants import CSV_SONG_COLUMN, CSV_MIXTURE_PATH_COLUMN, CSV_STEM_PATH_COLUMN
+import svc_toolkit.separation.audio as audio
+from svc_toolkit.separation.constants import CSV_SONG_COLUMN, CSV_MIXTURE_PATH_COLUMN, CSV_STEM_PATH_COLUMN
 
 def mix_track(track: MoisesDBTrack, stem, save_dir):
     if stem in track.stems:
         track_dir = f'{track.artist} - {track.name}'.strip().replace('ö', 'o')
 
         output_stems = {
             "mixture": all_stems,
```

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/separation/separator.py` & `svc_toolkit-1.0.1/src/svc_toolkit/separation/separator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import math
 
 import numpy as np
 import torch
 
-from vc_toolkit.utility.functions import load_yaml
-from vc_toolkit.separation import utility, models, audio, constants
+from svc_toolkit.utility.functions import load_yaml
+from svc_toolkit.separation import utility, models, audio, constants
 
 class SeparatorFactory():
     def __init__(self) -> None:
         pass
 
     def create(self, model_dir, device, precision):
         return Separator(model_dir, device, precision)
```

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/separation/utility.py` & `svc_toolkit-1.0.1/src/svc_toolkit/separation/utility.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 
 import pandas as pd
 
-from vc_toolkit.separation.constants import CSV_SONG_COLUMN
+from svc_toolkit.separation.constants import CSV_SONG_COLUMN
 
 def get_best_checkpoint_path(model_dir):
     return get_checkpoint_path(model_dir, 'best')
 
 def get_last_checkpoint_path(model_dir):
     return get_checkpoint_path(model_dir, 'last')
```

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/separation_evaluation.py` & `svc_toolkit-1.0.1/src/svc_toolkit/separation_evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import argparse
 from argparse import ArgumentParser
 
 import torch
 import matplotlib.pyplot as plt
 
-from vc_toolkit.separation.evaluator import Evaluator
+from svc_toolkit.separation.evaluator import Evaluator
 
 def main():
     parser = ArgumentParser()
     parser.add_argument('-m', '--model_dir', type=str, required=True)
     parser.add_argument('-t', '--test_csv', type=str, required=True)
     parser.add_argument('-p', '--precision', type=str, default='bf16')
     parser.add_argument('-l', '--last', default=False, action=argparse.BooleanOptionalAction)
```

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/separation_preprocess.py` & `svc_toolkit-1.0.1/src/svc_toolkit/separation_preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 from argparse import ArgumentParser
 
-from vc_toolkit.separation import constants
-from vc_toolkit.separation.preprocess import moisesdb_mix, preprocess
+from svc_toolkit.separation import constants
+from svc_toolkit.separation.preprocess import moisesdb_mix, preprocess
 
 def main():
     parser = ArgumentParser()
     parser.add_argument('-o', '--output_dir', type=str, default='./input_csv')
     parser.add_argument('-v', '--val_size', type=float, default=0.2)
     parser.add_argument('-s', '--stem', type=str, default='vocals')
     parser.add_argument('-m', '--musdb_dir', type=str, required=True)
```

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/separation_train.py` & `svc_toolkit-1.0.1/src/svc_toolkit/separation_train.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import os
 from argparse import ArgumentParser
 from datetime import datetime
 
 import pytorch_lightning as pl
 from pytorch_lightning.callbacks import EarlyStopping, ModelCheckpoint
 
-from vc_toolkit.utility.functions import load_yaml, save_yaml
-from vc_toolkit.separation import constants
-from vc_toolkit.separation import utility
-from vc_toolkit.separation.data import MagnitudeDataModule
-from vc_toolkit.separation.logger import MyLogger
-from vc_toolkit.separation.models import UNetLightning
+from svc_toolkit.utility.functions import load_yaml, save_yaml
+from svc_toolkit.separation import constants
+from svc_toolkit.separation import utility
+from svc_toolkit.separation.data import MagnitudeDataModule
+from svc_toolkit.separation.logger import MyLogger
+from svc_toolkit.separation.models import UNetLightning
 
 def main():
     parser = ArgumentParser()
     parser.add_argument('-t', '--train_csv', type=str, required=True)
     parser.add_argument('-v', '--val_csv', type=str, required=True)
     parser.add_argument('-e', '--experiment', type=str, default='exp')
     parser.add_argument('-m', '--model_dir', type=str, default='./model/')
```

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/widget/common.py` & `svc_toolkit-1.0.1/src/svc_toolkit/widget/common.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/widget/conversion.py` & `svc_toolkit-1.0.1/src/svc_toolkit/widget/conversion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,26 @@
-import time
 import json
 
 from PySide6.QtWidgets import QWidget, QVBoxLayout, QPushButton, QGroupBox
 from PySide6.QtCore import QThread
 from pyside6_utils.widgets import OverlayWidget
 
-from vc_toolkit.widget.common import SliderWidget, FloatSliderWidget, FileWidget, SaveFileWidget, DropdownWidget, CheckboxWidget, DropdownWidget, info_message_box, error_message_box
-from vc_toolkit.widget.loading_overlay import LoadingOverlayWidget
+from svc_toolkit.widget.common import SliderWidget, FloatSliderWidget, FileWidget, SaveFileWidget, DropdownWidget, CheckboxWidget, DropdownWidget, info_message_box, error_message_box
+from svc_toolkit.widget.loading_overlay import LoadingOverlayWidget
 
 class ConversionThread(QThread):
     def __init__(self, conversion_function, kwargs):
         super().__init__()
         self.conversion_function = conversion_function
         self.kwargs = kwargs
 
     def run(self):
         try:
             self.error_message = None
-            time.sleep(5)
-            # self.conversion_function(**self.kwargs)
+            self.conversion_function(**self.kwargs)
 
         except Exception as e:
             self.error_message = str(e)
 
 class ConversionWidget(OverlayWidget):
     def __init__(self):
         super().__init__(parent=None)
```

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/widget/loading_overlay.py` & `svc_toolkit-1.0.1/src/svc_toolkit/widget/loading_overlay.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/widget/loading_window.py` & `svc_toolkit-1.0.1/src/svc_toolkit/widget/loading_window.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/widget/main_window.py` & `svc_toolkit-1.0.1/src/svc_toolkit/widget/main_window.py`

 * *Files identical despite different names*

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/widget/mixing.py` & `svc_toolkit-1.0.1/src/svc_toolkit/widget/mixing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from PySide6.QtWidgets import QWidget, QVBoxLayout, QPushButton, QGroupBox
 from PySide6.QtCore import QThread, Signal
 
-from vc_toolkit.widget.common import info_message_box, error_message_box, FileWidget, SaveFileWidget, CheckboxWidget, FloatSliderWidget
+from svc_toolkit.widget.common import info_message_box, error_message_box, FileWidget, SaveFileWidget, CheckboxWidget, FloatSliderWidget
 
 class MixingThread(QThread):
     def __init__(self, mixer_function, kwargs):
         super().__init__()
         self.mixer_function = mixer_function
         self.kwargs = kwargs
```

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/widget/separation.py` & `svc_toolkit-1.0.1/src/svc_toolkit/widget/separation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from PySide6.QtWidgets import QWidget, QVBoxLayout, QPushButton, QProgressBar, QGroupBox
 from PySide6.QtCore import QThread, Signal
 
-from vc_toolkit.widget.common import info_message_box, error_message_box, FileWidget, DirectoryWidget, CheckboxWidget, DropdownWidget
+from svc_toolkit.widget.common import info_message_box, error_message_box, FileWidget, DirectoryWidget, CheckboxWidget, DropdownWidget
 
 class SeparationThread(QThread):
     progress_signal = Signal(int)
 
     def __init__(self, separation_function, kwargs):
         super().__init__()
         self.separation_function = separation_function
```

### Comparing `svc_toolkit-1.0.0/src/vc_toolkit/widget/training.py` & `svc_toolkit-1.0.1/src/svc_toolkit/widget/training.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from PySide6.QtWidgets import QVBoxLayout, QPushButton, QGroupBox
 from PySide6.QtCore import QThread
 from pyside6_utils.widgets import OverlayWidget
 
-from vc_toolkit.widget.common import FileWidget, DirectoryWidget, CheckboxWidget, info_message_box, error_message_box
-from vc_toolkit.widget.loading_overlay import LoadingOverlayWidget
+from svc_toolkit.widget.common import FileWidget, DirectoryWidget, CheckboxWidget, info_message_box, error_message_box
+from svc_toolkit.widget.loading_overlay import LoadingOverlayWidget
 
 class PreprocessThread(QThread):
     def __init__(self, preprocess_function, dataset_dir, output_dir, split=False):
         super().__init__()
         self.preprocess_function = preprocess_function
         self.dataset_dir = dataset_dir
         self.output_dir = output_dir
```

### Comparing `svc_toolkit-1.0.0/PKG-INFO` & `svc_toolkit-1.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: svc-toolkit
-Version: 1.0.0
+Version: 1.0.1
 Summary: A self-contained singing voice conversion toolkit.
 Author: jljl1337
 Author-email: lckjack123@gmail.com
 Requires-Python: >=3.10,<3.13
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -25,14 +25,17 @@
 Requires-Dist: torch (==2.1.1)
 Requires-Dist: torchaudio (==2.1.1)
 Requires-Dist: torchmetrics (==1.2.0)
 Description-Content-Type: text/markdown
 
 # Singing Voice Conversion with GUI
 
+![Tests](https://github.com/jljl1337/svc-toolkit/actions/workflows/tests.yml/badge.svg)
+[![Codecov](https://codecov.io/gh/jljl1337/svc-toolkit/graph/badge.svg?token=QBM6OLIG00)](https://codecov.io/gh/jljl1337/svc-toolkit)
+
 ## Useful commands for singularity container
 
 ```
 singularity shell --nv --bind /public:/public ~/test.simg 
 source ~/.bashrc
 conda activate svc
 python src/separation_train.py -t input_csv/train.csv -v input_csv/val.csv -e all
```

