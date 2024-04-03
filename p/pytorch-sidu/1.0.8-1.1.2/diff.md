# Comparing `tmp/pytorch-sidu-1.0.8.tar.gz` & `tmp/pytorch-sidu-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-sidu-1.0.8.tar", last modified: Mon Apr  1 14:36:23 2024, max compression
+gzip compressed data, was "pytorch-sidu-1.1.2.tar", last modified: Wed Apr  3 11:07:39 2024, max compression
```

## Comparing `pytorch-sidu-1.0.8.tar` & `pytorch-sidu-1.1.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:36:23.675958 pytorch-sidu-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35150 2024-04-01 14:34:55.000000 pytorch-sidu-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-01 14:34:55.000000 pytorch-sidu-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-01 14:36:23.675958 pytorch-sidu-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-01 14:34:55.000000 pytorch-sidu-1.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:36:23.675958 pytorch-sidu-1.0.8/pytorch_sidu/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-01 14:34:55.000000 pytorch-sidu-1.0.8/pytorch_sidu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5724 2024-04-01 14:34:55.000000 pytorch-sidu-1.0.8/pytorch_sidu/sidu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:36:23.675958 pytorch-sidu-1.0.8/pytorch_sidu/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-01 14:34:55.000000 pytorch-sidu-1.0.8/pytorch_sidu/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 14:36:23.675958 pytorch-sidu-1.0.8/pytorch_sidu.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3311 2024-04-01 14:36:23.000000 pytorch-sidu-1.0.8/pytorch_sidu.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-01 14:36:23.000000 pytorch-sidu-1.0.8/pytorch_sidu.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 14:36:23.000000 pytorch-sidu-1.0.8/pytorch_sidu.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-01 14:36:23.000000 pytorch-sidu-1.0.8/pytorch_sidu.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-01 14:36:23.000000 pytorch-sidu-1.0.8/pytorch_sidu.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-01 14:34:55.000000 pytorch-sidu-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-01 14:36:23.675958 pytorch-sidu-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-01 14:34:55.000000 pytorch-sidu-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:39.823689 pytorch-sidu-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35150 2024-04-03 11:06:12.000000 pytorch-sidu-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 11:06:12.000000 pytorch-sidu-1.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-03 11:07:39.823689 pytorch-sidu-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-04-03 11:06:12.000000 pytorch-sidu-1.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:39.819689 pytorch-sidu-1.1.2/pytorch_sidu/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 11:06:12.000000 pytorch-sidu-1.1.2/pytorch_sidu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7090 2024-04-03 11:06:12.000000 pytorch-sidu-1.1.2/pytorch_sidu/sidu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:39.823689 pytorch-sidu-1.1.2/pytorch_sidu/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-03 11:06:12.000000 pytorch-sidu-1.1.2/pytorch_sidu/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:07:39.823689 pytorch-sidu-1.1.2/pytorch_sidu.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-03 11:07:39.000000 pytorch-sidu-1.1.2/pytorch_sidu.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-03 11:07:39.000000 pytorch-sidu-1.1.2/pytorch_sidu.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 11:07:39.000000 pytorch-sidu-1.1.2/pytorch_sidu.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 11:07:39.000000 pytorch-sidu-1.1.2/pytorch_sidu.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-03 11:07:39.000000 pytorch-sidu-1.1.2/pytorch_sidu.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-03 11:06:12.000000 pytorch-sidu-1.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-03 11:07:39.823689 pytorch-sidu-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-03 11:06:12.000000 pytorch-sidu-1.1.2/setup.py
```

### Comparing `pytorch-sidu-1.0.8/LICENSE` & `pytorch-sidu-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch-sidu-1.0.8/PKG-INFO` & `pytorch-sidu-1.1.2/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,7 @@
-Metadata-Version: 2.1
-Name: pytorch-sidu
-Version: 1.0.8
-Summary: SIDU: SImilarity Difference and Uniqueness method for explainable AI
-Home-page: https://github.com/MarcoParola/pytorch-sidu
-Author: Marco Parola
-Author-email: marcoparola96@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: torch
-Requires-Dist: torchvision
-Requires-Dist: numpy
-
 # **pytorch-sidu**
 
 ![example workflow](https://github.com/MarcoParola/pytorch-sidu/actions/workflows/python-publish.yml/badge.svg)
 [![size](https://img.shields.io/github/languages/code-size/MarcoParola/pytorch-sidu)]()
 
 SIDU: SImilarity Difference and Uniqueness method for explainable AI from the [original paper](https://arxiv.org/pdf/2006.03122.pdf)
 
@@ -43,44 +25,46 @@
 ## Usage
 
 Load models from the pretrainde ones available in pytorch
 
 ```py
 import pytorch_sidu as sidu
 
-weights = "ResNet18_Weights.IMAGENET1K_V1"
-backbone = sidu.load_torch_backbone(weights)
+model_name = 'ResNet34_Weights.IMAGENET1K_V1'
+model = load_torch_model_by_string(model_name)
 ```
 
 After instantianting your model, generate saliency maps from Dataloader
 
 ```py
 data_loader = <your dataloader>
+target_layer = 'layer4.2.conv2'
 image, _ = next(iter(data_loader))
-saliency_maps = sidu.sidu(backbone, image)
+saliency_maps = sidu.sidu(model, target_layer, image)
 ```
 
 ### A complete example on CIFAR-10
 
 ```py
 import torch
 import torchvision
 from matplotlib import pyplot as plt
 import pytorch_sidu as sidu
 
 
-transform = torchvision.transforms.Compose([torchvision.transforms.Resize((256, 256)), torchvision.transforms.ToTensor()])
+transform = torchvision.transforms.Compose([torchvision.transforms.Resize((224, 224)), torchvision.transforms.ToTensor()])
 data_loader = torch.utils.data.DataLoader(
     torchvision.datasets.CIFAR10(root='./data', download=True, transform=transform), batch_size=2)
 
-weights = "ResNet18_Weights.IMAGENET1K_V1"
-backbone = sidu.load_torch_backbone(weights)
+target_layer = 'layer4.2.conv2'
+model_name = 'ResNet34_Weights.IMAGENET1K_V1'
+model = load_torch_model_by_string(model_name)
 
 for image, _ in data_loader:
-    saliency_maps = sidu.sidu(backbone, image)
+    saliency_maps = sidu.sidu(model, target_layer, image)
     image, saliency_maps = image.cpu(), saliency_maps.cpu()
 
     for j in range(len(image)):
         plt.figure(figsize=(5, 2.5))
         plt.subplot(1, 2, 1)
         plt.imshow(image[j].permute(1, 2, 0))
         plt.axis('off')
```

### Comparing `pytorch-sidu-1.0.8/pytorch_sidu/sidu.py` & `pytorch-sidu-1.1.2/pytorch_sidu/sidu.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,68 @@
+# pytorch_sidu/sidu.py
+
+r""" SIDU SImilarity Difference and Uniqueness method
+
+The SIDU method is a method for explaining the predictions of a model by computing the similarity differences and the uniqueness of the masks generated from the feature map of the model. The method is based on the paper **SIDU: Similarity Difference and Uniqueness Method for Explainable AI** by Satya M. Muddamsetty, Mohammad N. S. Jahromi, and Thomas B. Moeslund.
+
+The module contains the following functions:
+    - kernel: Kernel function for computing the weights of the differences
+    - normalize: Normalize the array
+    - uniqness_measure: Compute the uniqueness measure
+    - similarity_differences: Compute the similarity differences
+    - generate_masks: Generate masks from the feature map
+    - sidu: SIDU SImilarity Difference and Uniqueness method
+"""
+
 import torch
 import torchvision
 import numpy as np
-
+from torchvision.models.feature_extraction import create_feature_extractor
 
 
 def kernel(vector: torch.Tensor, kernel_width: float = 0.1) -> torch.Tensor:
-    r""" Kernel function for computing the weights of the differences
+    """
+    Kernel function for computing the weights of the differences.
+
     Args:
-        d: torch.Tensor
-            The difference tensor
-        kernel_width: float
-            The kernel width
+        vector (torch.Tensor): 
+            The difference tensor.
+        kernel_width (float, optional): 
+            The kernel width. Defaults to 0.1.
+
     Returns:
-        weights: torch.Tensor
-            The weights
+        torch.Tensor: 
+            The weights.
     """
     return torch.sqrt(torch.exp(-(vector ** 2) / kernel_width ** 2))
 
 
 def normalize(array: torch.Tensor) -> torch.Tensor:
-    r""" Normalize the array
+    r"""
+    Normalize the array
+
     Args:
         array: torch.Tensor
             The input array
+
     Returns:
         normalized_array: torch.Tensor
             The normalized array
     """
     return (array - array.min()) / (array.max() - array.min() + 1e-13)
 
 
 
 def uniqness_measure(masked_feature_map: torch.Tensor) -> torch.Tensor:
     r""" Compute the uniqueness measure
+
     Args:
         masked_feature_map: torch.Tensor
             The masked feature map
+
     Returns:
         uniqueness: torch.Tensor
             The uniqueness measure
     """
     batch_size, num_masks, feature_len, w, h = masked_feature_map.size()
 
     # Reshape tensor to have size (batch * num_masks, feature_len, w * h)
@@ -54,19 +77,21 @@
 
     return uniqueness
 
 
 
 def similarity_differences(orig_predictions: torch.Tensor, masked_predictions: torch.Tensor):
     r""" Compute the similarity differences
+
     Args:
         orig_predictions: torch.Tensor
             The original predictions
         masked_predictions: torch.Tensor
             The masked predictions
+
     Returns:
          : torch.Tensor
             The weights
         diff: torch.Tensor
             The differences
     """
     diff = abs(masked_predictions - orig_predictions)
@@ -77,21 +102,23 @@
     weighted_diff = weighted_diff.mean(dim=(2, 3))
     return weighted_diff, diff
 
 
 
 def generate_masks(img_size: tuple, feature_map: torch.Tensor, s: int = 8) -> torch.Tensor:
     r""" Generate masks from the feature map
+
     Args:
         img_size: tuple
             The size of the input image
         feature_map: torch.Tensor
             The feature map from the model
         s: int
             The scale factor
+
     Returns:
         masks: torch.Tensor
             The generated masks
     """
     h, w = img_size
     cell_size = np.ceil(np.array(img_size) / s)
     up_size = (s) * cell_size
@@ -103,47 +130,54 @@
     
     # resize to the size of the input image torch.nn.functional.F.interpolate: (batch, N, f_h, f_w) -> (batch, N, h, w)
     masks = torch.nn.functional.interpolate(feature_map, size=(h, w), mode='bilinear', align_corners=True)
         
     return masks
 
 
-
-def sidu(model: torch.nn.Module, image: torch.Tensor) -> torch.Tensor:
+def sidu(model: torch.nn.Module, layer_name: str, image: torch.Tensor, device: torch.device = torch.device("cpu")) -> torch.Tensor:
     r""" SIDU SImilarity Difference and Uniqueness method
+    
     Args:
         model: torch.nn.Module
             The model to be explained
         image: torch.Tensor
             The input image to be explained
-        masks: torch.Tensor
-            The generated masks
-    """
+        layer_name: str
+            The layer name of the model to be explained
+            It must be contained in named_modules() of the model
+        device: torch.device, optional
+            The device to use. Defaults to torch.device("cpu")
 
-    # check device
-    device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-    model.to(device)
-    image = image.to(device)
+    Returns:
+        saliency_maps: torch.Tensor
+            The saliency maps
 
+    """
     model.eval()
+    model.to(device)
+    image = image.to(device)
+    return_nodes = {layer_name: 'target_layer'}
+    model = create_feature_extractor(model, return_nodes=return_nodes)
+    
     with torch.no_grad():
-        orig_feature_map = model(image)
+        orig_feature_map = model(image)['target_layer']
         input_size = image.shape[2:]
         masks = generate_masks(input_size, orig_feature_map, 16)
         batch = image.shape[0]
         num_masks = masks.shape[1]
 
         # Repeat the masks 3 times along the channel dimension to match the number of channels of the image and masks
         masks = masks.unsqueeze(2).repeat(1, 1, 3, 1, 1)
         images = image.unsqueeze(1).repeat(1, num_masks, 1, 1, 1)
         masked_images = images * masks
 
         masked_feature_map = []
         for i in range(num_masks):
-            masked_feature_map.append(model(masked_images[:, i, :, :, :]))
+            masked_feature_map.append(model(masked_images[:, i, :, :, :])['target_layer'])
         masked_feature_map = torch.stack(masked_feature_map, dim=1) # TODO speed up this part
         
         orig_feature_map = orig_feature_map.unsqueeze(1).repeat(1, num_masks, 1, 1, 1)
 
         # compute the differences of the similarity and the uniqueness
         weighted_diff, difference = similarity_differences(orig_feature_map, masked_feature_map)
         uniqness = uniqness_measure(masked_feature_map)
@@ -160,8 +194,7 @@
         saliency_maps = masks * sidu.unsqueeze(2).unsqueeze(3)
 
         # reduce the saliency maps to a single map by summing over the masks dimension
         saliency_maps = saliency_maps.sum(dim=1)
         saliency_maps /= num_masks
 
         return saliency_maps
-
```

### Comparing `pytorch-sidu-1.0.8/pytorch_sidu.egg-info/PKG-INFO` & `pytorch-sidu-1.1.2/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytorch-sidu
-Version: 1.0.8
+Version: 1.1.2
 Summary: SIDU: SImilarity Difference and Uniqueness method for explainable AI
 Home-page: https://github.com/MarcoParola/pytorch-sidu
 Author: Marco Parola
 Author-email: marcoparola96@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -43,44 +43,46 @@
 ## Usage
 
 Load models from the pretrainde ones available in pytorch
 
 ```py
 import pytorch_sidu as sidu
 
-weights = "ResNet18_Weights.IMAGENET1K_V1"
-backbone = sidu.load_torch_backbone(weights)
+model_name = 'ResNet34_Weights.IMAGENET1K_V1'
+model = load_torch_model_by_string(model_name)
 ```
 
 After instantianting your model, generate saliency maps from Dataloader
 
 ```py
 data_loader = <your dataloader>
+target_layer = 'layer4.2.conv2'
 image, _ = next(iter(data_loader))
-saliency_maps = sidu.sidu(backbone, image)
+saliency_maps = sidu.sidu(model, target_layer, image)
 ```
 
 ### A complete example on CIFAR-10
 
 ```py
 import torch
 import torchvision
 from matplotlib import pyplot as plt
 import pytorch_sidu as sidu
 
 
-transform = torchvision.transforms.Compose([torchvision.transforms.Resize((256, 256)), torchvision.transforms.ToTensor()])
+transform = torchvision.transforms.Compose([torchvision.transforms.Resize((224, 224)), torchvision.transforms.ToTensor()])
 data_loader = torch.utils.data.DataLoader(
     torchvision.datasets.CIFAR10(root='./data', download=True, transform=transform), batch_size=2)
 
-weights = "ResNet18_Weights.IMAGENET1K_V1"
-backbone = sidu.load_torch_backbone(weights)
+target_layer = 'layer4.2.conv2'
+model_name = 'ResNet34_Weights.IMAGENET1K_V1'
+model = load_torch_model_by_string(model_name)
 
 for image, _ in data_loader:
-    saliency_maps = sidu.sidu(backbone, image)
+    saliency_maps = sidu.sidu(model, target_layer, image)
     image, saliency_maps = image.cpu(), saliency_maps.cpu()
 
     for j in range(len(image)):
         plt.figure(figsize=(5, 2.5))
         plt.subplot(1, 2, 1)
         plt.imshow(image[j].permute(1, 2, 0))
         plt.axis('off')
```

### Comparing `pytorch-sidu-1.0.8/setup.cfg` & `pytorch-sidu-1.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytorch-sidu-1.0.8/setup.py` & `pytorch-sidu-1.1.2/setup.py`

 * *Files identical despite different names*

