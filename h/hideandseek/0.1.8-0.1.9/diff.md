# Comparing `tmp/hideandseek-0.1.8.tar.gz` & `tmp/hideandseek-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hideandseek-0.1.8.tar", last modified: Thu Jan 25 02:34:56 2024, max compression
+gzip compressed data, was "hideandseek-0.1.9.tar", last modified: Thu Jan 25 02:44:36 2024, max compression
```

## Comparing `hideandseek-0.1.8.tar` & `hideandseek-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-01-25 02:34:56.461303 hideandseek-0.1.8/
--rw-rw-rw-   0        0        0     1089 2022-06-27 07:10:00.000000 hideandseek-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     2744 2024-01-25 02:34:56.460299 hideandseek-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     2230 2022-08-16 19:15:37.000000 hideandseek-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-01-25 02:34:56.435775 hideandseek-0.1.8/hideandseek/
--rw-rw-rw-   0        0        0      475 2024-01-25 02:34:37.000000 hideandseek-0.1.8/hideandseek/__init__.py
--rw-rw-rw-   0        0        0     2063 2024-01-23 22:58:05.000000 hideandseek-0.1.8/hideandseek/dataset.py
--rw-rw-rw-   0        0        0    16340 2024-01-25 02:34:33.000000 hideandseek-0.1.8/hideandseek/eval.py
--rw-rw-rw-   0        0        0     7428 2022-06-27 08:00:35.000000 hideandseek-0.1.8/hideandseek/fv.py
--rw-rw-rw-   0        0        0     2470 2022-10-04 19:05:33.000000 hideandseek-0.1.8/hideandseek/loss.py
--rw-rw-rw-   0        0        0     2998 2024-01-25 02:24:07.000000 hideandseek-0.1.8/hideandseek/model.py
--rw-rw-rw-   0        0        0      598 2022-06-27 08:00:35.000000 hideandseek-0.1.8/hideandseek/plot.py
--rw-rw-rw-   0        0        0    19379 2024-01-23 21:58:34.000000 hideandseek-0.1.8/hideandseek/trainer.py
--rw-rw-rw-   0        0        0     2392 2024-01-05 17:16:54.000000 hideandseek-0.1.8/hideandseek/utils.py
--rw-rw-rw-   0        0        0     9152 2024-01-23 21:26:13.000000 hideandseek-0.1.8/hideandseek/validation.py
-drwxrwxrwx   0        0        0        0 2024-01-25 02:34:56.458301 hideandseek-0.1.8/hideandseek.egg-info/
--rw-rw-rw-   0        0        0     2744 2024-01-25 02:34:55.000000 hideandseek-0.1.8/hideandseek.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2024-01-25 02:34:56.000000 hideandseek-0.1.8/hideandseek.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-25 02:34:55.000000 hideandseek-0.1.8/hideandseek.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-01-25 02:34:55.000000 hideandseek-0.1.8/hideandseek.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-01-25 02:34:55.000000 hideandseek-0.1.8/hideandseek.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-25 02:34:56.462300 hideandseek-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      946 2024-01-22 19:47:04.000000 hideandseek-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-01-25 02:44:36.326722 hideandseek-0.1.9/
+-rw-rw-rw-   0        0        0     1089 2022-06-27 07:10:00.000000 hideandseek-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     2744 2024-01-25 02:44:36.325667 hideandseek-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2230 2022-08-16 19:15:37.000000 hideandseek-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-01-25 02:44:36.296659 hideandseek-0.1.9/hideandseek/
+-rw-rw-rw-   0        0        0      475 2024-01-25 02:44:23.000000 hideandseek-0.1.9/hideandseek/__init__.py
+-rw-rw-rw-   0        0        0     2063 2024-01-23 22:58:05.000000 hideandseek-0.1.9/hideandseek/dataset.py
+-rw-rw-rw-   0        0        0    16068 2024-01-25 02:42:44.000000 hideandseek-0.1.9/hideandseek/eval.py
+-rw-rw-rw-   0        0        0     7428 2022-06-27 08:00:35.000000 hideandseek-0.1.9/hideandseek/fv.py
+-rw-rw-rw-   0        0        0     2470 2022-10-04 19:05:33.000000 hideandseek-0.1.9/hideandseek/loss.py
+-rw-rw-rw-   0        0        0     2998 2024-01-25 02:24:07.000000 hideandseek-0.1.9/hideandseek/model.py
+-rw-rw-rw-   0        0        0      598 2022-06-27 08:00:35.000000 hideandseek-0.1.9/hideandseek/plot.py
+-rw-rw-rw-   0        0        0    20703 2024-01-25 02:44:17.000000 hideandseek-0.1.9/hideandseek/trainer.py
+-rw-rw-rw-   0        0        0     2392 2024-01-05 17:16:54.000000 hideandseek-0.1.9/hideandseek/utils.py
+-rw-rw-rw-   0        0        0    11679 2024-01-25 02:44:00.000000 hideandseek-0.1.9/hideandseek/validation.py
+drwxrwxrwx   0        0        0        0 2024-01-25 02:44:36.322711 hideandseek-0.1.9/hideandseek.egg-info/
+-rw-rw-rw-   0        0        0     2744 2024-01-25 02:44:35.000000 hideandseek-0.1.9/hideandseek.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2024-01-25 02:44:36.000000 hideandseek-0.1.9/hideandseek.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-01-25 02:44:35.000000 hideandseek-0.1.9/hideandseek.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-01-25 02:44:35.000000 hideandseek-0.1.9/hideandseek.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-01-25 02:44:35.000000 hideandseek-0.1.9/hideandseek.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-01-25 02:44:36.326722 hideandseek-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      946 2024-01-22 19:47:04.000000 hideandseek-0.1.9/setup.py
```

### Comparing `hideandseek-0.1.8/LICENSE` & `hideandseek-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hideandseek-0.1.8/PKG-INFO` & `hideandseek-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hideandseek
-Version: 0.1.8
+Version: 0.1.9
 Summary: library for deep learning and privacy preserving deep learning
 Home-page: https://github.com/jsyoo61/hideandseek
 Author: JaeSung Yoo
 Author-email: jsyoo61@unc.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hideandseek-0.1.8/README.md` & `hideandseek-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `hideandseek-0.1.8/hideandseek/dataset.py` & `hideandseek-0.1.9/hideandseek/dataset.py`

 * *Files identical despite different names*

### Comparing `hideandseek-0.1.8/hideandseek/eval.py` & `hideandseek-0.1.9/hideandseek/eval.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,16 +66,15 @@
         # Infer targets_type and create corresponding test_f and result_dict
         if targets_type is None:
             if hasattr(dataset, 'targets_type'):
                 targets_type = dataset.targets_type
             else:
                 raise Exception('When test_f and result_dict is not given, targets_type must be given or the dataset must have the attribute "targets_type"')
         assert targets_type in targets_type_list, f'targets_type must be one of {targets_type_list}, received: {targets_type}'
-        test_f = get_test_f(targets_type)
-        result_dict = get_result_dict(targets_type, keep_x=keep_x)
+        test_f, result_f = get_test_f(targets_type, keep_x=keep_x)
     else:
         raise Exception(f'test_f and result_dict must either both be provided or None, received [test_f: {test_f}][result_dict: {result_dict}]')
     return test_f, result_dict
 
 def test_torch(network, dataset, batch_size=64, targets_type=None, test_f=None, result_dict=None, keep_x=False, num_workers=0, amp=False):
     '''
     inference stage of network.
@@ -125,40 +124,35 @@
     elif type(metrics) is list:
         scores = [metric(results) for metric in metrics]
     else:
         scores = metrics(results)
     return scores
 
 targets_type_list = [None, 'categorical', 'multihead_classification', 'autoencode', 'regression'] # move this to utils?
-def get_test_f(targets_type):
+def get_test_f(targets_type, keep_x=False):
     assert targets_type in targets_type_list, f'targets_type must be one of {targets_type_list}, received: {targets_type}'
     if targets_type is None or targets_type == 'regression':
-        return _test_base
+        test_f = _test_base
+        result_list = ['y_true', 'y_hat']
     elif targets_type == 'categorical':
-        return _test_categorical
+        test_f = _test_categorical
+        result_list = ['y_true', 'y_hat', 'y_score', 'y_pred']
     elif targets_type == 'multihead_classification':
-        return _test_multihead_categorical
-    elif targets_type == 'autoencode':
-        return _test_autoencode
-    else:
-        raise Exception(f'unknown targets_type: {targets_type}')
-
-def get_result_dict(targets_type, keep_x=False):
-    assert targets_type in targets_type_list, f'targets_type must be one of {targets_type_list}, received: {targets_type}'
-    if targets_type is None:
-        result_list = ['y_true', 'y_hat']
-        if keep_x: result_list.append('x')
-    elif targets_type in ['categorical', 'multihead_classification']:
+        test_f = _test_multihead_categorical
         result_list = ['y_true', 'y_hat', 'y_score', 'y_pred']
-        if keep_x: result_list.append('x')
     elif targets_type == 'autoencode':
+        test_f = _test_autoencode
         result_list = ['x', 'z', 'x_hat']
     else:
         raise Exception(f'unknown targets_type: {targets_type}')
-    return {r:[] for r in result_list}
+    
+    if keep_x and 'x' not in result_list: result_list.append('x')
+    result_dict = {r:[] for r in result_list}
+
+    return test_f, result_dict
 
 def _test_base(data, network, result_dict, device=None, keep_x=False):
     # device = device if device is not None else T.torch.get_device(network)
     x = data['x'].to(device)
     y = data['y'].to(device)
     y_hat = network(x)
 
@@ -187,28 +181,27 @@
     y_hat = network(x)
     y_score = torch.softmax(y_hat, dim=-1) # (N, subtype, n_classes)
 
     result_dict['y_true'].append(y.cpu().numpy())
     result_dict['y_hat'].append(y_hat.cpu().numpy())
     result_dict['y_score'].append(y_score.cpu().numpy())
     result_dict['y_pred'].append(y_score.argmax(axis=-1).cpu().numpy())
-
+    if keep_x: result_dict['x'].append(x.cpu().numpy())
     return result_dict
 
 def _test_autoencode(data, network, result_dict, device=None):
     x = data['x'].to(device)
     z = network.encoder(x)
     x_hat = torch.sigmoid(network.decoder(z))
 
     x, z, x_hat = x.cpu().numpy(), z.cpu().numpy(), x_hat.cpu().numpy()
 
     result_dict['x'].append(x)
     result_dict['z'].append(z)
     result_dict['x_hat'].append(x_hat)
-
     return result_dict
 
 # %%
 '''
 Scorers
 
 They all receive dict of numpy arrays.
```

### Comparing `hideandseek-0.1.8/hideandseek/fv.py` & `hideandseek-0.1.9/hideandseek/fv.py`

 * *Files identical despite different names*

### Comparing `hideandseek-0.1.8/hideandseek/loss.py` & `hideandseek-0.1.9/hideandseek/loss.py`

 * *Files identical despite different names*

### Comparing `hideandseek-0.1.8/hideandseek/model.py` & `hideandseek-0.1.9/hideandseek/model.py`

 * *Files identical despite different names*

### Comparing `hideandseek-0.1.8/hideandseek/plot.py` & `hideandseek-0.1.9/hideandseek/plot.py`

 * *Files identical despite different names*

### Comparing `hideandseek-0.1.8/hideandseek/trainer.py` & `hideandseek-0.1.9/hideandseek/trainer.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,128 +22,145 @@
 # 'Trainer'
 # ]
 
 # %%
 log = logging.getLogger(__name__)
 
 # %%
+
 class Trainer:
-    def __init__(self, nn, train_dataset=None, cfg_train={}, criterion=None, nn_dir=None, node_dir=None, val_dataset=None, val_metrics=None, earlystopper=None, name='default', verbose=True, amp=False, reproduce=True):
+    def __init__(self, network, train_dataset=None, cfg_train={}, criterion=None, network_dir=None, node_dir=None, cfg_val=None, val_dataset=None, val_metrics=None, name='default', verbose=True, amp=False, reproduce=True):
         '''
         Things Trainer do:
-        - train nn with early stopping, given hyperparameters
-        - save/load nn with necessary preprocessing pipeline
+        - train network with early stopping, given hyperparameters
+        - save/load network with necessary preprocessing pipeline
 
-        :param nn: torch.nn.Module object
+        :param network: torch.nn.Module object
         :param train_dataset: torch.utils.data.Dataset object
             This dataset is used for training.
             Recommended return format from dataset is: {'x': x, 'y': y}
             where 'x' is the input, and 'y' is the target values.
 
         :param validation: dict of Validation objects
 
         :param cfg_train: dict-like object which contains:
             lr
             batch_size
             weight_decay (optional)
-            patience (optional)
+        
+        :param cfg_val (optional): dict-like object which contains:
+            increase_better
+            patience
+            batch_size
+            target_dataset (optional, if val_dataset is dict for multiple datasets)
+            criterion (optional, if val_metrics is dict for multiple metrics) 
 
         :param criterion: torch.nn.Module object, used to compute loss function
 
         Recommended way of making hs.node.Node object is like the following:
 
-            kwargs = {'nn': NN(), 'train_dataset': train_dataset, 'validation': None, 'cfg_train': cfg.train,
-                    'criterion': criterion, 'nn_dir': path['nn'], 'node_dir': path['node'], 'verbose': True, 'amp': True}
+            kwargs = {'network': Network(), 'train_dataset': train_dataset, 'validation': None, 'cfg_train': cfg.train,
+                    'criterion': criterion, 'network_dir': path['network'], 'node_dir': path['node'], 'verbose': True, 'amp': True}
             node = hs.node.Node(**kwargs)
         '''
         # Store configurations
-        self.nn = nn
+        self.network = network
         self.train_dataset = train_dataset
         self.cfg_train = dcopy(dict(cfg_train))
         self.criterion = criterion
-        self.nn_dir = nn_dir
+        self.network_dir = network_dir
         self.node_dir = node_dir
 
+        self.cfg_val = dcopy(dict(cfg_val))
         self.val_dataset = val_dataset
         self.val_metrics = val_metrics
-        self.earlystopper = earlystopper
+        self.earlystopper = EarlyStopper(increase_better=cfg_val['increase_better'], patience=cfg_val['patience']) if self.val_dataset is not None else None
+        if 'target_dataset' in self.cfg_val:
+            assert self.cfg_val['target_dataset'] in self.val_dataset, f'[Validation setup] target_dataset: {self.cfg_val["target_dataset"]} not found in val_dataset: {self.val_dataset.keys()}'
+        assert self.val_dataset is not None and self.val_metrics is not None, f'val_dataset and val_metrics must be given together or neither. val_dataset: {self.val_dataset}, val_metrics: {self.val_metrics}'
 
-        # self.validation = validation if issubclass(type(validation), dict) or validation is None else V.VDict({'default': validation}) # wrap with VDict if single validation object is given.
         self.name = name
         self.verbose = verbose
         self.amp = amp
         self.reproduce = reproduce
 
         # Initializations
-        if self.nn_dir is not None:
-            if os.path.exists(self.nn_dir): log.warning(f'path: {self.nn_dir} exists. Be careful')
-            os.makedirs(self.nn_dir, exist_ok=True)
+        if self.network_dir is not None:
+            if os.path.exists(self.network_dir): log.warning(f'path: {self.network_dir} exists. Be careful')
+            os.makedirs(self.network_dir, exist_ok=True)
 
         if self.node_dir is not None:
             if os.path.exists(self.node_dir): log.warning(f'path: {self.node_dir} exists. Be careful')
             os.makedirs(self.node_dir, exist_ok=True)
 
-        if self.validation is None and self.earlystopper is not None: log.warning('validation is None but earlystopper is given. earlystopper will be ignored')
-        if self.earlystopper is not None:
-            assert earlystopper.target_validation in self.validation.keys(), 'earlystopper.target_valiation not provided in validation'
-
-        self.train_meter = tools.modules.AveratgeMeter() # Tracks loss per epoch
+        self.train_meter = tools.modules.AverageMeter() # Tracks loss per epoch
         self.loss_tracker = tools.modules.ValueTracker() # Tracks loss over all training
-        self.set_misc()
+        self.set_model()
         self.reset()
 
         self._targets_type = self.infer_targets_type()
 
     def reset(self):
         self.iter = 0
         self.n_batch=0
 
     def print(self, content):
         if self.verbose:
             print(content)
         else:
             log.info(content)
 
-    def set_misc(self):
+    def set_model(self):
         '''Set miscellaneous variables'''
+        self.model = BaseModel(self.network, amp=self.amp)
         self.misc = tools.TDict()
         if self.train_dataset is not None:
-            if hasattr(self.train_dataset, 'get_f'): # get_f equal to preprocessing pipeline before feeding to nn
+            if hasattr(self.train_dataset, 'get_f'): # get_f equal to preprocessing pipeline before feeding to network
                 self.print('get_f found in loader.dataset')
                 self.misc.get_f = self.train_dataset.get_f
 
     def validate(self):
-        if self.validation is not None:
-            score_summary = {}
-            for cv_name, validation in self.validation.items(): # Different types of datasets
-                score = validation.step(self)
-                score_summary[cv_name] = score
-                self.print(f'[cv_name: {cv_name}] Validation Score: {score}')
+        patience_end = False
+        if self.val_dataset is not None:
+            if type(self.val_dataset)==dict:
+                scores = {}
+                for name, dataset in self.val_dataset.items():
+                    d_results = hs.E.test_model(self.model, dataset, batch_size=self.cfg_train['batch_size'], amp=self.amp)
+                    score = evaluate(d_results, self.val_metrics)
+                    scores[name] = score
+                    self.print(f'[dataset_name: {name}] Validation Score: {score}')
+                score = scores[self.cfg_val['target_dataset']]
+            else:
+                d_results = hs.E.test_model(self.model, self.val_dataset, batch_size=self.cfg_train['batch_size'], amp=self.amp)
+                score = evaluate(d_results, self.val_metrics)
+                self.print(f'Validation Score: {scores}')
+            
             if self.earlystopper is not None:
-                patience_end = self.earlystopper.step(self, score_summary, os.path.join(self.nn_dir, f'nn_{self.iter}.pt'))
+                if type(score) is dict:
+                    score_ = score[self.cfg_val['criterion']]
+
+                patience_end = self.earlystopper.step(self, score_)
                 if patience_end:
                     self.print('patience met, flushing earlystopper history')
                     self.earlystopper.history.reset()
-            else:
-                patience_end = False
         return patience_end
 
     def generate_loader(self):
         if self.train_dataset is not None:
             reproduce_kwargs = U.reproducible_worker_dict() if self.reproduce else {}
             drop_last = len(self.train_dataset) % self.cfg_train['batch_size'] == 1 # To avoid batch normalization layers from raising exceptions
             self.loader = D.DataLoader(self.train_dataset, batch_size=self.cfg_train['batch_size'], shuffle=True, drop_last=drop_last, **reproduce_kwargs)
             # self.loader = D.DataLoader(self.train_dataset, batch_size=self.cfg_train['batch_size'], shuffle=True, drop_last=True, **U.reproducible_worker_dict()) if len(self.train_dataset) % self.cfg_train['batch_size'] == 1 \
             #         else D.DataLoader(self.train_dataset, batch_size=self.cfg_train['batch_size'], shuffle=True, drop_last=False, **U.reproducible_worker_dict())
         else:
             log.warning('No train_dataset found. Skipping generate_loader()')
 
     def train(self, epoch=None, new_op=True, no_val=False, step=None, reset_loss_tracker=False):
         '''
-        Trains the nn with the specified duration.
+        Trains the network with the specified duration.
         '''
         assert epoch is None or step is None, f'only one of epoch or step can be specified. received epoch: {epoch}, step: {step}'
         if step is None:
             horizon = 'epoch'
             if epoch is None: # When neither epoch or step are specified
                 assert 'epoch' in self.cfg_train, 'key "epoch" must be provided in cfg_train, or the argument "epoch" must be provided \
                                                 when argument "step" is not specified.'
@@ -151,72 +168,71 @@
             log.debug(f'[Node: {self.name}] train for {epoch} epochs')
         else:
             assert epoch is None, f'Either epoch or step must be specified. Received epoch: {epoch}, step: {step}'
             horizon = 'step'
             step = step
             log.debug(f'[Node: {self.name}] train for {step} steps')
 
-        self.nn.train()
-        device = tools.torch.get_device(self.nn)
+        self.network.train()
+        device = tools.torch.get_device(self.network)
         self.criterion = self.criterion.to(device)
         if reset_loss_tracker: self.loss_tracker.reset()
         self.generate_loader()
         '''
         There may be one or more loaders, but self.loader is the standard of synchronization
         Either return multiple values from dataset, or modify self.forward to use other loaders
         '''
 
-        if self.validation is not None:
+        if self.val_dataset is not None:
             if 'cv_step' not in self.cfg_train:
                 self.print('Node.validation given, but "cv_step" not specified in cfg_train. Defaults to 1 epoch')
                 self.cfg_train['cv_step'] = len(self.loader)
-            self.validation.reset()
             self.validate() # initial testing
 
         # Make new optimizer
         if new_op or not hasattr(self, 'op'):
             if not hasattr(self, 'op') and not new_op:
                 log.warning("new_op=False when there's no pre-existing optimizer. Ignoring new_op...")
             # Weight decay optional
-            self.op = optim.Adam(self.nn.parameters(), lr=self.cfg_train['lr'], weight_decay=self.cfg_train['weight_decay']) if 'weight_decay' in self.cfg_train \
-                        else optim.Adam(self.nn.parameters(), lr=self.cfg_train['lr'])
-            # self.op = optim.Adam(self.nn.parameters(), **self.cfg_train)
+            self.op = optim.Adam(self.network.parameters(), lr=self.cfg_train['lr'], weight_decay=self.cfg_train['weight_decay']) if 'weight_decay' in self.cfg_train \
+                        else optim.Adam(self.network.parameters(), lr=self.cfg_train['lr'])
+            # self.op = optim.Adam(self.network.parameters(), **self.cfg_train)
 
         if horizon == 'epoch':
             self._step_epoch(T=epoch, no_val=no_val, device=device)
         elif horizon=='step':
             self._step_step(T=step, no_val=no_val, device=device)
 
         # TODO: Return criterion back to its original device, meaning we have to store its previous device info
         self.criterion = self.criterion.cpu()
         return self.loss_tracker
 
     def _step_epoch(self, T, no_val=False, device=None):
-        self._device = device if device is not None else tools.torch.get_device(self.nn)
+        self._device = device if device is not None else tools.torch.get_device(self.network)
 
         _iter = 0
         for epoch in range(1, T+1):
             self.train_meter.reset()
             self.epoch_f()
             for batch_i, data in enumerate(self.loader, 1):
                 self.iter += 1
                 _iter += 1
                 loss = self._update(data)
                 self.print(f'[Node: {self.name}][iter_sum: {self.iter}][Epoch: {epoch}/{T}][Batch: {batch_i}/{len(self.loader)}][Loss: {loss:.7f} (Avg: {self.train_meter.avg:.7f})]')
                 self.loss_tracker.step(self.iter, loss)
 
                 # Validation
-                if (self.validation is not None) and (not no_val) and (_iter % self.cfg_train['cv_step']==0):
+                if (self.val_dataset is not None) and (not no_val) and (_iter % self.cfg_train['cv_step']==0):
                     patience_end = self.validate()
                     if patience_end: # If patience has reached, stop training
                         self.print('Patience met, stopping training')
                         return None # return None since double break is impossible in python
 
     def _step_step(self, T, no_val=False, device=None):
-        self._device = device if device is not None else tools.torch.get_device(self.nn)
+        self._device = device if device is not None else tools.torch.get_device(self.network)
         if hasattr(self, '_loader_inst'): del self._loader_inst # Load data from the 1st batch
 
         for _iter in range(1, T+1):
             # Get Data
             try:
                 if hasattr(self, '_loader_inst'):
                     data = next(self._loader_inst)
@@ -233,15 +249,15 @@
             self.iter += 1
             loss = self._update(data)
             self.print(f'[Node: {self.name}][iter_sum: {self.iter}][Iter: {_iter}/{T}][Batch: {self.n_batch}/{len(self.loader)}][Loss: {loss:.7f} (Avg: {self.train_meter.avg:.7f})]')
 
             self.loss_tracker.step(self.iter, loss)
 
             # Validation
-            if (self.validation is not None) and (not no_val) and (_iter % self.cfg_train['cv_step']==0):
+            if (self.val_dataset is not None) and (not no_val) and (_iter % self.cfg_train['cv_step']==0):
             # if (not no_val) and (self.iter % self.cfg_train.cv_step==0):
                 patience_end = self.validate()
                 if patience_end: # If patience has reached, stop training
                     self.print('Patience met, stopping training')
                     return None # return None since double break is impossible in python
 
     def _update(self, data):
@@ -313,15 +329,15 @@
         """
         Forward pass. Receive data and return the loss function.
         Inherit Node and define new forward() function to build custom forward pass.
 
         May return tuple or dictionary, whichever will be feeded to criterion.
         """
 
-        y_hat = self.nn(x)
+        y_hat = self.network(x)
 
         return y_hat, y
 
     def _criterion(self, outputs):
         outputstype = outputstype
         if outputstype is tuple or outputstype is list:
             loss = self.criterion(*outputs)
@@ -333,29 +349,33 @@
 
     def epoch_f(self):
         # TODO: rename to forward hook? epoch_hook?
         '''function to call every other epoch. May be used in child class'''
         pass
 
     def infer_targets_type(self):
-        if self.dataset is not None and hasattr(self.dataset, 'targets_type'):
-            return self.dataset.targets_type
-        elif self.validation is not None and 'val' in self.validation:
-            if type(self.validation['val'].dataset)==list:
-                return self.validation['val'].dataset[0].targets_type
-            else:
-                return self.validation['val'].dataset.targets_type
+        if self.train_dataset is not None and hasattr(self.train_dataset, 'targets_type'):
+            return self.train_dataset.targets_type
+        elif self.val_dataset is not None:
+            if type(self.val_dataset)==dict:
+                for name, dataset in self.val_dataset.items():
+                    if hasattr(dataset, 'targets_type'):
+                        return dataset.targets_type
+            elif hasattr(self.val_dataset, 'targets_type'):
+                return self.val_dataset.targets_type
         else:
             return None
 
     def post_train(self, val_dataset=None):
-        # Deafult to self.validation['val'].dataset
         if val_dataset is None:
-            assert 'val' in self.validation, f'if no val_dataset is given, then "val" must exist in self.validation: {self.validation.keys()}'
-            val_dataset = self.validation['val'].dataset
+            assert self.val_dataset is not None, f'val_dataset must be given if self.val_dataset is None'
+            if type(self.val_dataset)==dict:
+                val_dataset = self.val_dataset[self.cfg_val['target_dataset']]
+            else:
+                val_datset = self.val_dataset
 
         if self._targets_type == 'binary':
             self.print(f'[Node: {self.name}][post_train] binary classfication: choose threshold based on validation set')
             self.threshold = E.binary_threshold(self, val_dataset)
         else:
             self.print(f'[Node: {self.name}][post_train] no post-train procedure for _targets_type: {self._targets_type}')
 
@@ -372,78 +392,78 @@
         state_dict = {
         'loss_tracker': self.loss_tracker,
         }
         if 'get_f' in self.misc:
             state_dict['misc.get_f'] = self.misc.get_f
         if hasattr(self, 'threshold'):
             state_dict['threshold'] = self.threshold
-        if self.validation is not None:
-            state_dict['validation.history'] = {name: validation.history for name, validation in self.validation.items()}
+        if self.earlystopper is not None:
+            state_dict['earlystopper.history'] = self.earlystopper.history
         return state_dict
 
     def load_state_dict(self, state_dict):
         state_dict = dcopy(state_dict)
 
         if 'misc.get_f' in state_dict.keys():
             self.print(f'Updating get_f: {state_dict["misc.get_f"]}')
             self.misc.get_f = state_dict['misc.get_f']
-            if self.dataset is not None:
+            if self.train_dataset is not None:
                 self.print('updating get_f to loader...')
-                self.dataset.get_f = self.misc.get_f
+                self.train_dataset.get_f = self.misc.get_f
             del state_dict['misc.get_f']
 
         if 'threshold' in state_dict.keys():
             self.print(f'Updating threshold: {state_dict["threshold"]}')
             self.threshold = state_dict['threshold']
             del state_dict['threshold']
 
         self.__dict__.update(state_dict) # update attributes
 
     def save(self, path=None, best=True):
         '''
         Save the following:
         state_dict() -> path/state_dict.p
-        nn.state_dict() -> path/nn.pt
+        network.state_dict() -> path/network.pt
         '''
         path = self.node_dir if path is None else path
         self.print(f'[Node: {self.name}]')
 
         state_dict_path = os.path.join(path, 'node.p')
         self.print(f'[save] Saving node info to: {state_dict_path}')
         state_dict = self.state_dict()
         self.print(f'[save] state_dict: {list(state_dict.keys())}')
         tools.save_pickle(state_dict, state_dict_path)
 
-        nn_path = os.path.join(path, 'nn.pt')
+        network_path = os.path.join(path, 'network.pt')
         if best:
             if self.earlystopper is None:
-                self.print(f'[save][best: {best}] earlystopper not defined. Saving current nn -> [{nn_path}]')
-                torch.save(self.nn.state_dict(), nn_path)
+                self.print(f'[save][best: {best}] earlystopper not defined. Saving current network -> [{network_path}]')
+                torch.save(self.network.state_dict(), network_path)
             else:
-                if self.earlystopper.best_nn != None:
-                    self.print(f'[save][best: {best}] Saving [{self.earlystopper.best_nn}] -> [{nn_path}]')
-                    shutil.copy(self.earlystopper.best_nn, nn_path)
+                if self.earlystopper.best_network != None:
+                    self.print(f'[save][best: {best}] Saving [{self.earlystopper.best_network}] -> [{network_path}]')
+                    shutil.copy(self.earlystopper.best_network, network_path)
                 else:
-                    self.print(f'[save][best: {best}] no best_nn in self.earlystopper, Saving current nn -> [{nn_path}]')
-                    torch.save(self.nn.state_dict(), nn_path)
+                    self.print(f'[save][best: {best}] no best_network in self.earlystopper, Saving current network -> [{network_path}]')
+                    torch.save(self.network.state_dict(), network_path)
         else:
-            self.print(f'[save][best: {best}] Saving nn to: {nn_path}')
-            torch.save(self.nn.state_dict(), nn_path)
+            self.print(f'[save][best: {best}] Saving network to: {network_path}')
+            torch.save(self.network.state_dict(), network_path)
 
     def load(self, path=None):
         '''
-        load state_dict() and nn:
+        load state_dict() and network:
         path/node.p -> state_dict
-        path/nn.pt -> nn.state_dict
+        path/network.pt -> network.state_dict
         '''
         path = self.node_dir if path is None else path
         self.print(f'[Node: {self.name}]')
 
         state_dict_path = os.path.join(path, 'node.p')
         self.print(f'[load] Loading from path: {state_dict_path}')
         state_dict = tools.load_pickle(state_dict_path)
         self.print(f'[load] Updating: {list(state_dict.keys())}')
         self.load_state_dict(state_dict)
 
-        nn_path = os.path.join(path, 'nn.pt')
-        self.print(f'[load] Loading nn from: {nn_path}')
-        self.nn.load_state_dict(torch.load(nn_path))
+        network_path = os.path.join(path, 'network.pt')
+        self.print(f'[load] Loading network from: {network_path}')
+        self.network.load_state_dict(torch.load(network_path))
```

### Comparing `hideandseek-0.1.8/hideandseek/utils.py` & `hideandseek-0.1.9/hideandseek/utils.py`

 * *Files identical despite different names*

### Comparing `hideandseek-0.1.8/hideandseek/validation.py` & `hideandseek-0.1.9/hideandseek/validation.py`

 * *Files 12% similar despite different names*

```diff
@@ -80,54 +80,63 @@
             valuetracker.plot(ax=ax_)
             ax_.set_title(score_type)
         return ax
 
     def reset(self):
         pass
 
+
 class EarlyStopper():
+    """
+    Returns True if the metric has stopped improving for the given number of patience steps.
+    Saves model in the given path and remembers which model is the best.
+
+    Parameters
+    ----------
+    arg : array-like of shape (n_samples,), default=None
+        Argument explanation.
+        If ``None`` is given, those that appear at least once
+        .. versionadded:: 0.18
+    
+    Functions
+    -------
+    step()
+        returns True/False
+    """
+
     def __repr__(self):
         return f'<EarlyStopper>\npatience: {self.patience}\nincrease_better: {self.increase_better}'
 
-    def __init__(self, increase_better, patience, primary_score=None, target_validation='default', discard_best=True):
+    def __init__(self, increase_better, patience, save_dir='network_temp', discard_best=True):
         self.increase_better = increase_better
         self.patience = patience
-        self.primary_score = primary_score
-        self.target_validation = target_validation
+        self.save_dir = save_dir
         self.discard_best = discard_best
 
-
-        self.history = T.modules.ValueTracker() # For now, only track single score
+        os.makedirs(self.save_dir, exist_ok=True)
+        self.history = tools.modules.ValueTracker() # For now, only track single score
         self.reset()
 
-    def step(self, node, score_summary, path):
-        '''
-        score_summary: 2-level nested dictionary of scores.
-            1st-level keys are validation object names,
-            2nd-level keys are score names
-        '''
-        score_target_validation = score_summary[self.target_validation]
-        if self.primary_score is None:
-            assert len(score_target_validation)==1, f"primary_score must be specified when there's more than 1 scorer functions, received: {len(score_target_validation)}"
-            score = list(score_target_validation.values())[0]
-            # assert type(score) is not dict, 'when primary_score is not given, the given score must be a scalar'
-        else:
-            score = score_target_validation[self.primary_score]
-        self.history.step(node.iter, score)
+    def step(self, trainer, score, filename=None):
+        filename = f'network_{trainer.iter}.pt' if filename is None else filename
+
+        self.history.step(trainer.iter, score)
 
         # Save best model
         if isbetter(score_best=self.best_score, score=score, increase_better=self.increase_better):
-            log.info(f'[EarlyStopping]New best score: {self.best_score} -> {score}')
-            log.info(f'[EarlyStopping]Saved model: {path}')
-            torch.save(node.model.state_dict(), path)
+            path = os.path.join(self.save_dir, filename)
+
+            log.info(f'[EarlyStopping] New best score: {self.best_score} -> {score}')
+            log.info(f'[EarlyStopping] Saved model: {path}')
+            torch.save(trainer.model.state_dict(), path)
             if self.discard_best and self.best_model!=None:
                 os.remove(self.best_model)
 
             self.best_score = score
-            self.best_model=path
+            self.best_model = path
 
             # Clear patience tracking
             self.history.reset()
 
         # patience_end == True when best model did not appear for self.patience times
         patience_end = self.patience == len(self.history)
         log.info(f'[EarlyStopping][patience: {len(self.history)}/{self.patience}]')
@@ -139,14 +148,73 @@
         self.history.reset()
         self.best_model = None
         if self.increase_better:
             self.best_score = -float('inf')
         else:
             self.best_score = float('inf')
 
+# class EarlyStopper():
+#     def __repr__(self):
+#         return f'<EarlyStopper>\npatience: {self.patience}\nincrease_better: {self.increase_better}'
+
+#     def __init__(self, increase_better, patience, primary_score=None, target_validation='default', discard_best=True):
+#         self.increase_better = increase_better
+#         self.patience = patience
+#         self.primary_score = primary_score
+#         self.target_validation = target_validation
+#         self.discard_best = discard_best
+
+
+#         self.history = T.modules.ValueTracker() # For now, only track single score
+#         self.reset()
+
+#     def step(self, node, score_summary, path):
+#         '''
+#         score_summary: 2-level nested dictionary of scores.
+#             1st-level keys are validation object names,
+#             2nd-level keys are score names
+#         '''
+#         score_target_validation = score_summary[self.target_validation]
+#         if self.primary_score is None:
+#             assert len(score_target_validation)==1, f"primary_score must be specified when there's more than 1 scorer functions, received: {len(score_target_validation)}"
+#             score = list(score_target_validation.values())[0]
+#             # assert type(score) is not dict, 'when primary_score is not given, the given score must be a scalar'
+#         else:
+#             score = score_target_validation[self.primary_score]
+#         self.history.step(node.iter, score)
+
+#         # Save best model
+#         if isbetter(score_best=self.best_score, score=score, increase_better=self.increase_better):
+#             log.info(f'[EarlyStopping]New best score: {self.best_score} -> {score}')
+#             log.info(f'[EarlyStopping]Saved model: {path}')
+#             torch.save(node.model.state_dict(), path)
+#             if self.discard_best and self.best_model!=None:
+#                 os.remove(self.best_model)
+
+#             self.best_score = score
+#             self.best_model=path
+
+#             # Clear patience tracking
+#             self.history.reset()
+
+#         # patience_end == True when best model did not appear for self.patience times
+#         patience_end = self.patience == len(self.history)
+#         log.info(f'[EarlyStopping][patience: {len(self.history)}/{self.patience}]')
+
+#         return patience_end
+
+#     def reset(self):
+#         # log.info('[EarlyStopper] Resetting...')
+#         self.history.reset()
+#         self.best_model = None
+#         if self.increase_better:
+#             self.best_score = -float('inf')
+#         else:
+#             self.best_score = float('inf')
+
 class EarlyStopping(Validation):
     def __init__(self, dataset, scorer, primary_score=None, increase_better=False, discard_best=True, patience=None):
         '''
         :param dataset: dataloader or list of dataloaders
         '''
         super().__init__(dataset, scorer)
         self.increase_better = increase_better
```

### Comparing `hideandseek-0.1.8/hideandseek.egg-info/PKG-INFO` & `hideandseek-0.1.9/hideandseek.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hideandseek
-Version: 0.1.8
+Version: 0.1.9
 Summary: library for deep learning and privacy preserving deep learning
 Home-page: https://github.com/jsyoo61/hideandseek
 Author: JaeSung Yoo
 Author-email: jsyoo61@unc.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `hideandseek-0.1.8/setup.py` & `hideandseek-0.1.9/setup.py`

 * *Files identical despite different names*

