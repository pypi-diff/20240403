# Comparing `tmp/guan-0.1.94.tar.gz` & `tmp/guan-0.1.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guan-0.1.94.tar", last modified: Tue Apr  2 06:15:38 2024, max compression
+gzip compressed data, was "guan-0.1.95.tar", last modified: Wed Apr  3 16:29:41 2024, max compression
```

## Comparing `guan-0.1.94.tar` & `guan-0.1.95.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2024-04-02 06:15:38.588860 guan-0.1.94/
--rw-rw-rw-   0        0        0    35821 2021-07-19 21:39:06.000000 guan-0.1.94/LICENSE
--rw-rw-rw-   0        0        0      798 2024-04-02 06:15:38.588860 guan-0.1.94/PKG-INFO
--rw-rw-rw-   0        0        0      294 2023-11-04 17:18:16.000000 guan-0.1.94/README.md
--rw-rw-rw-   0        0        0      108 2021-05-22 13:59:00.000000 guan-0.1.94/pyproject.toml
--rw-rw-rw-   0        0        0      641 2024-04-02 06:15:38.598497 guan-0.1.94/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-02 06:15:38.420287 guan-0.1.94/src/
-drwxrwxrwx   0        0        0        0 2024-04-02 06:15:38.568172 guan-0.1.94/src/guan/
--rw-rw-rw-   0        0        0     5294 2024-02-22 19:01:32.000000 guan-0.1.94/src/guan/Fourier_transform.py
--rw-rw-rw-   0        0        0     6572 2024-02-22 19:01:42.000000 guan-0.1.94/src/guan/Green_functions.py
--rw-rw-rw-   0        0        0    24114 2024-02-22 19:01:51.000000 guan-0.1.94/src/guan/Hamiltonian_of_examples.py
--rw-rw-rw-   0        0        0      811 2024-02-22 19:43:08.000000 guan-0.1.94/src/guan/__init__.py
--rw-rw-rw-   0        0        0    10438 2024-02-22 18:58:28.000000 guan-0.1.94/src/guan/band_structures_and_wave_functions.py
--rw-rw-rw-   0        0        0     2388 2024-02-22 19:00:04.000000 guan-0.1.94/src/guan/basic_functions.py
--rw-rw-rw-   0        0        0     4622 2024-04-02 06:13:43.000000 guan-0.1.94/src/guan/data_processing.py
--rw-rw-rw-   0        0        0     1398 2024-02-22 19:14:25.000000 guan-0.1.94/src/guan/decorators.py
--rw-rw-rw-   0        0        0    10300 2024-02-22 19:01:02.000000 guan-0.1.94/src/guan/density_of_states.py
--rw-rw-rw-   0        0        0    21680 2024-02-22 19:01:14.000000 guan-0.1.94/src/guan/figure_plotting.py
--rw-rw-rw-   0        0        0    12813 2024-02-28 01:45:12.000000 guan-0.1.94/src/guan/file_reading_and_writing.py
--rw-rw-rw-   0        0        0    10505 2024-04-01 13:21:34.000000 guan-0.1.94/src/guan/machine_learning.py
--rw-rw-rw-   0        0        0    41346 2024-03-12 18:43:39.000000 guan-0.1.94/src/guan/others.py
--rw-rw-rw-   0        0        0    41489 2024-03-10 21:28:40.000000 guan-0.1.94/src/guan/quantum_transport.py
--rw-rw-rw-   0        0        0    27324 2024-02-22 19:02:31.000000 guan-0.1.94/src/guan/topological_invariant.py
-drwxrwxrwx   0        0        0        0 2024-04-02 06:15:38.588860 guan-0.1.94/src/guan.egg-info/
--rw-rw-rw-   0        0        0      798 2024-04-02 06:15:38.000000 guan-0.1.94/src/guan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      618 2024-04-02 06:15:38.000000 guan-0.1.94/src/guan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-02 06:15:38.000000 guan-0.1.94/src/guan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-02 06:15:38.000000 guan-0.1.94/src/guan.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 16:29:41.666047 guan-0.1.95/
+-rw-rw-rw-   0        0        0    35821 2021-07-19 21:39:06.000000 guan-0.1.95/LICENSE
+-rw-rw-rw-   0        0        0      798 2024-04-03 16:29:41.666047 guan-0.1.95/PKG-INFO
+-rw-rw-rw-   0        0        0      294 2023-11-04 17:18:16.000000 guan-0.1.95/README.md
+-rw-rw-rw-   0        0        0      108 2021-05-22 13:59:00.000000 guan-0.1.95/pyproject.toml
+-rw-rw-rw-   0        0        0      641 2024-04-03 16:29:41.667921 guan-0.1.95/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 16:29:41.508416 guan-0.1.95/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 16:29:41.644086 guan-0.1.95/src/guan/
+-rw-rw-rw-   0        0        0     5294 2024-02-22 19:01:32.000000 guan-0.1.95/src/guan/Fourier_transform.py
+-rw-rw-rw-   0        0        0     6572 2024-02-22 19:01:42.000000 guan-0.1.95/src/guan/Green_functions.py
+-rw-rw-rw-   0        0        0    24114 2024-02-22 19:01:51.000000 guan-0.1.95/src/guan/Hamiltonian_of_examples.py
+-rw-rw-rw-   0        0        0      811 2024-02-22 19:43:08.000000 guan-0.1.95/src/guan/__init__.py
+-rw-rw-rw-   0        0        0    10438 2024-02-22 18:58:28.000000 guan-0.1.95/src/guan/band_structures_and_wave_functions.py
+-rw-rw-rw-   0        0        0     2388 2024-02-22 19:00:04.000000 guan-0.1.95/src/guan/basic_functions.py
+-rw-rw-rw-   0        0        0     4622 2024-04-02 06:13:43.000000 guan-0.1.95/src/guan/data_processing.py
+-rw-rw-rw-   0        0        0     1398 2024-02-22 19:14:25.000000 guan-0.1.95/src/guan/decorators.py
+-rw-rw-rw-   0        0        0    10300 2024-02-22 19:01:02.000000 guan-0.1.95/src/guan/density_of_states.py
+-rw-rw-rw-   0        0        0    21680 2024-02-22 19:01:14.000000 guan-0.1.95/src/guan/figure_plotting.py
+-rw-rw-rw-   0        0        0    12813 2024-02-28 01:45:12.000000 guan-0.1.95/src/guan/file_reading_and_writing.py
+-rw-rw-rw-   0        0        0    12995 2024-04-03 16:25:13.000000 guan-0.1.95/src/guan/machine_learning.py
+-rw-rw-rw-   0        0        0    41346 2024-03-12 18:43:39.000000 guan-0.1.95/src/guan/others.py
+-rw-rw-rw-   0        0        0    41489 2024-03-10 21:28:40.000000 guan-0.1.95/src/guan/quantum_transport.py
+-rw-rw-rw-   0        0        0    27324 2024-02-22 19:02:31.000000 guan-0.1.95/src/guan/topological_invariant.py
+drwxrwxrwx   0        0        0        0 2024-04-03 16:29:41.664336 guan-0.1.95/src/guan.egg-info/
+-rw-rw-rw-   0        0        0      798 2024-04-03 16:29:41.000000 guan-0.1.95/src/guan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      618 2024-04-03 16:29:41.000000 guan-0.1.95/src/guan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 16:29:41.000000 guan-0.1.95/src/guan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-03 16:29:41.000000 guan-0.1.95/src/guan.egg-info/top_level.txt
```

### Comparing `guan-0.1.94/LICENSE` & `guan-0.1.95/LICENSE`

 * *Files identical despite different names*

### Comparing `guan-0.1.94/PKG-INFO` & `guan-0.1.95/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guan
-Version: 0.1.94
+Version: 0.1.95
 Summary: An open source python package
 Home-page: https://py.guanjihuan.com
 Author: guanjihuan
 Author-email: guanjihuan@163.com
 Project-URL: Bug Tracker, https://py.guanjihuan.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `guan-0.1.94/setup.cfg` & `guan-0.1.95/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2067 7561 6e0d 0a76 6572 7369 6f6e   = guan..version
-00000020: 203d 2030 2e31 2e39 340d 0a61 7574 686f   = 0.1.94..autho
+00000020: 203d 2030 2e31 2e39 350d 0a61 7574 686f   = 0.1.95..autho
 00000030: 7220 3d20 6775 616e 6a69 6875 616e 0d0a  r = guanjihuan..
 00000040: 6175 7468 6f72 5f65 6d61 696c 203d 2067  author_email = g
 00000050: 7561 6e6a 6968 7561 6e40 3136 332e 636f  uanjihuan@163.co
 00000060: 6d0d 0a64 6573 6372 6970 7469 6f6e 203d  m..description =
 00000070: 2041 6e20 6f70 656e 2073 6f75 7263 6520   An open source 
 00000080: 7079 7468 6f6e 2070 6163 6b61 6765 0d0a  python package..
 00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
```

### Comparing `guan-0.1.94/src/guan/Fourier_transform.py` & `guan-0.1.95/src/guan/Fourier_transform.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.94/src/guan/Green_functions.py` & `guan-0.1.95/src/guan/Green_functions.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.94/src/guan/Hamiltonian_of_examples.py` & `guan-0.1.95/src/guan/Hamiltonian_of_examples.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.94/src/guan/__init__.py` & `guan-0.1.95/src/guan/__init__.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.94/src/guan/band_structures_and_wave_functions.py` & `guan-0.1.95/src/guan/band_structures_and_wave_functions.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.94/src/guan/basic_functions.py` & `guan-0.1.95/src/guan/basic_functions.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.94/src/guan/data_processing.py` & `guan-0.1.95/src/guan/data_processing.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.94/src/guan/decorators.py` & `guan-0.1.95/src/guan/decorators.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.94/src/guan/density_of_states.py` & `guan-0.1.95/src/guan/density_of_states.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.94/src/guan/figure_plotting.py` & `guan-0.1.95/src/guan/figure_plotting.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.94/src/guan/file_reading_and_writing.py` & `guan-0.1.95/src/guan/file_reading_and_writing.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.94/src/guan/machine_learning.py` & `guan-0.1.95/src/guan/machine_learning.py`

 * *Files 22% similar despite different names*

```diff
@@ -109,14 +109,42 @@
                 hidden_output_3 = self.hidden_layer_3(hidden_output_2)
             
             output = self.output_layer(hidden_output_3)
             return output
     model = model_class_of_fully_connected_neural_network_with_three_hidden_layers()
     return model
 
+# 卷积神经网络模型（包含两个卷积层和两个全连接层）（模型的类定义成全局的）
+def convolutional_neural_network_with_two_convolutional_layers_and_two_fully_connected_layers(in_channels=1, out_channels_1=10, out_channels_2=10, kernel_size_1=3, kernel_size_2=3, stride_1=1, stride_2=1, padding_1=0, padding_2=0, pooling=1, pooling_kernel_size=2, pooling_stride=2, input_size=1, hidden_size_1=10, hidden_size_2=10, output_size=1):
+    import torch
+    global model_class_of_convolutional_neural_network_with_two_convolutional_layers_and_two_fully_connected_layers
+    class model_class_of_convolutional_neural_network_with_two_convolutional_layers_and_two_fully_connected_layers(torch.nn.Module):
+        def __init__(self):
+            super().__init__()
+            self.convolutional_layer_1 = torch.nn.Conv2d(in_channels=in_channels, out_channels=out_channels_1, kernel_size=kernel_size_1, stride=stride_1, padding=padding_1)
+            self.convolutional_layer_2 = torch.nn.Conv2d(in_channels=out_channels_1, out_channels=out_channels_2, kernel_size=kernel_size_2, stride=stride_2, padding=padding_2)
+            self.pooling_layer = torch.nn.MaxPool2d(kernel_size=pooling_kernel_size, stride=pooling_stride)
+            self.hidden_layer_1 = torch.nn.Linear(input_size, hidden_size_1)
+            self.hidden_layer_2 = torch.nn.Linear(hidden_size_1, hidden_size_2)
+            self.output_layer = torch.nn.Linear(hidden_size_2, output_size)
+        def forward(self, x):
+            if pooling == 1:
+                channel_output_1 = torch.nn.functional.relu(self.pooling_layer(self.convolutional_layer_1(x))) 
+                channel_output_2 = torch.nn.functional.relu(self.pooling_layer(self.convolutional_layer_2(channel_output_1)))
+            else:
+                channel_output_1 = torch.nn.functional.relu(self.convolutional_layer_1(x)) 
+                channel_output_2 = torch.nn.functional.relu(self.convolutional_layer_2(channel_output_1))
+            channel_output_2 = torch.flatten(channel_output_2, 1)
+            hidden_output_1 = torch.nn.functional.relu(self.hidden_layer_1(channel_output_2))
+            hidden_output_2 = torch.nn.functional.relu(self.hidden_layer_2(hidden_output_1))
+            output = self.output_layer(hidden_output_2)
+            return output
+    model = model_class_of_convolutional_neural_network_with_two_convolutional_layers_and_two_fully_connected_layers()
+    return model
+
 # 使用优化器训练模型
 def train_model(model, x_data, y_data, optimizer='Adam', learning_rate=0.001, criterion='MSELoss', num_epochs=1000, print_show=1):
     import torch
     if optimizer == 'Adam':
         optimizer = torch.optim.Adam(model.parameters(), lr=learning_rate)
     elif optimizer == 'SGD':
         optimizer = torch.optim.SGD(model.parameters(), lr=learning_rate)
```

### Comparing `guan-0.1.94/src/guan/others.py` & `guan-0.1.95/src/guan/others.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.94/src/guan/quantum_transport.py` & `guan-0.1.95/src/guan/quantum_transport.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.94/src/guan/topological_invariant.py` & `guan-0.1.95/src/guan/topological_invariant.py`

 * *Files identical despite different names*

### Comparing `guan-0.1.94/src/guan.egg-info/PKG-INFO` & `guan-0.1.95/src/guan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guan
-Version: 0.1.94
+Version: 0.1.95
 Summary: An open source python package
 Home-page: https://py.guanjihuan.com
 Author: guanjihuan
 Author-email: guanjihuan@163.com
 Project-URL: Bug Tracker, https://py.guanjihuan.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `guan-0.1.94/src/guan.egg-info/SOURCES.txt` & `guan-0.1.95/src/guan.egg-info/SOURCES.txt`

 * *Files identical despite different names*

