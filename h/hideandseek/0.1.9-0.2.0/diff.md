# Comparing `tmp/hideandseek-0.1.9.tar.gz` & `tmp/hideandseek-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hideandseek-0.1.9.tar", last modified: Thu Jan 25 02:44:36 2024, max compression
+gzip compressed data, was "hideandseek-0.2.0.tar", last modified: Wed Apr  3 19:23:06 2024, max compression
```

## Comparing `hideandseek-0.1.9.tar` & `hideandseek-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-01-25 02:44:36.326722 hideandseek-0.1.9/
--rw-rw-rw-   0        0        0     1089 2022-06-27 07:10:00.000000 hideandseek-0.1.9/LICENSE
--rw-rw-rw-   0        0        0     2744 2024-01-25 02:44:36.325667 hideandseek-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     2230 2022-08-16 19:15:37.000000 hideandseek-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2024-01-25 02:44:36.296659 hideandseek-0.1.9/hideandseek/
--rw-rw-rw-   0        0        0      475 2024-01-25 02:44:23.000000 hideandseek-0.1.9/hideandseek/__init__.py
--rw-rw-rw-   0        0        0     2063 2024-01-23 22:58:05.000000 hideandseek-0.1.9/hideandseek/dataset.py
--rw-rw-rw-   0        0        0    16068 2024-01-25 02:42:44.000000 hideandseek-0.1.9/hideandseek/eval.py
--rw-rw-rw-   0        0        0     7428 2022-06-27 08:00:35.000000 hideandseek-0.1.9/hideandseek/fv.py
--rw-rw-rw-   0        0        0     2470 2022-10-04 19:05:33.000000 hideandseek-0.1.9/hideandseek/loss.py
--rw-rw-rw-   0        0        0     2998 2024-01-25 02:24:07.000000 hideandseek-0.1.9/hideandseek/model.py
--rw-rw-rw-   0        0        0      598 2022-06-27 08:00:35.000000 hideandseek-0.1.9/hideandseek/plot.py
--rw-rw-rw-   0        0        0    20703 2024-01-25 02:44:17.000000 hideandseek-0.1.9/hideandseek/trainer.py
--rw-rw-rw-   0        0        0     2392 2024-01-05 17:16:54.000000 hideandseek-0.1.9/hideandseek/utils.py
--rw-rw-rw-   0        0        0    11679 2024-01-25 02:44:00.000000 hideandseek-0.1.9/hideandseek/validation.py
-drwxrwxrwx   0        0        0        0 2024-01-25 02:44:36.322711 hideandseek-0.1.9/hideandseek.egg-info/
--rw-rw-rw-   0        0        0     2744 2024-01-25 02:44:35.000000 hideandseek-0.1.9/hideandseek.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      416 2024-01-25 02:44:36.000000 hideandseek-0.1.9/hideandseek.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-25 02:44:35.000000 hideandseek-0.1.9/hideandseek.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-01-25 02:44:35.000000 hideandseek-0.1.9/hideandseek.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-01-25 02:44:35.000000 hideandseek-0.1.9/hideandseek.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-01-25 02:44:36.326722 hideandseek-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      946 2024-01-22 19:47:04.000000 hideandseek-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:23:06.936522 hideandseek-0.2.0/
+-rw-rw-rw-   0        0        0     1089 2022-06-27 07:10:00.000000 hideandseek-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2757 2024-04-03 19:23:06.935528 hideandseek-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2243 2024-01-25 04:08:16.000000 hideandseek-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-03 19:23:06.900141 hideandseek-0.2.0/hideandseek/
+-rw-rw-rw-   0        0        0      375 2024-04-03 19:20:38.000000 hideandseek-0.2.0/hideandseek/__init__.py
+-rw-rw-rw-   0        0        0     2063 2024-01-23 22:58:05.000000 hideandseek-0.2.0/hideandseek/dataset.py
+-rw-rw-rw-   0        0        0    16568 2024-03-18 18:58:07.000000 hideandseek-0.2.0/hideandseek/eval.py
+-rw-rw-rw-   0        0        0     7428 2022-06-27 08:00:35.000000 hideandseek-0.2.0/hideandseek/fv.py
+-rw-rw-rw-   0        0        0     2354 2024-03-04 21:20:35.000000 hideandseek-0.2.0/hideandseek/loss.py
+-rw-rw-rw-   0        0        0     3187 2024-01-25 21:40:22.000000 hideandseek-0.2.0/hideandseek/model.py
+-rw-rw-rw-   0        0        0      598 2022-06-27 08:00:35.000000 hideandseek-0.2.0/hideandseek/plot.py
+-rw-rw-rw-   0        0        0    24677 2024-04-03 19:22:41.000000 hideandseek-0.2.0/hideandseek/trainer.py
+-rw-rw-rw-   0        0        0     4761 2024-01-26 19:12:55.000000 hideandseek-0.2.0/hideandseek/utils.py
+-rw-rw-rw-   0        0        0    11727 2024-01-25 21:35:05.000000 hideandseek-0.2.0/hideandseek/validation.py
+drwxrwxrwx   0        0        0        0 2024-04-03 19:23:06.933528 hideandseek-0.2.0/hideandseek.egg-info/
+-rw-rw-rw-   0        0        0     2757 2024-04-03 19:23:06.000000 hideandseek-0.2.0/hideandseek.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      416 2024-04-03 19:23:06.000000 hideandseek-0.2.0/hideandseek.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 19:23:06.000000 hideandseek-0.2.0/hideandseek.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-03 19:23:06.000000 hideandseek-0.2.0/hideandseek.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-03 19:23:06.000000 hideandseek-0.2.0/hideandseek.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-03 19:23:06.936522 hideandseek-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      946 2024-01-22 19:47:04.000000 hideandseek-0.2.0/setup.py
```

### Comparing `hideandseek-0.1.9/LICENSE` & `hideandseek-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hideandseek-0.1.9/PKG-INFO` & `hideandseek-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hideandseek
-Version: 0.1.9
+Version: 0.2.0
 Summary: library for deep learning and privacy preserving deep learning
 Home-page: https://github.com/jsyoo61/hideandseek
 Author: JaeSung Yoo
 Author-email: jsyoo61@unc.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -31,43 +31,43 @@
     import torch
     import torch.nn as nn
 
     # Generate data
     x = torch.rand(200,1)
     y = 5*x+2
 
-    model = nn.Linear(1,1)
+    network = nn.Linear(1,1)
     dataset = torch.utils.data.TensorDataset(x, y)
     criterion = nn.MSELoss()
     cfg = {
     'lr': 1e-2,
     'batch_size': 32,
     'epoch': 10 # optional
     }
 
     # Training configuration. All you need to train a neural network
     kwargs = {
-    'model':model,
+    'network':network,
     'dataset':dataset,
     'cfg_train':cfg,
     'criterion':criterion,
     'name': 'Test' # optional
     }
     trainer = hs.N.Node(**kwargs)
 
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-    trainer.model.to(device)
+    trainer.network.to(device)
 
     # Train for predefined number of epochs
     trainer.train() # Train for predefined number of epochs
     trainer.train(5) # Train for specified number of epochs
     trainer.train(epoch=5) # Same thing with trainer.train(5)
     trainer.train(step=500) # Train for specified number of updates
 
-    node.model.cpu()
+    trainer.network.cpu()
 
 and simply run multiple batch of experiments with a single line command such as:
 
     python train.py -m lr=1e-3,1e-2 batch_size=32,64 "random_seed=range(0,5)" \
     hydra/launcher=joblib hydra.launcher.n_jobs=8
     # Runs total of 2*2*5=40 batch of experiments, with 8 processes at a time. Experiment results are stored in hydra.sweep.dir which can be overridden.
```

### Comparing `hideandseek-0.1.9/README.md` & `hideandseek-0.2.0/hideandseek.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: hideandseek
+Version: 0.2.0
+Summary: library for deep learning and privacy preserving deep learning
+Home-page: https://github.com/jsyoo61/hideandseek
+Author: JaeSung Yoo
+Author-email: jsyoo61@unc.edu
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # hideandseek
 Highly modularized deep learning training library.
 
 Why use `hideandseek`?
 
 - Easy training & saving deep learning models along with other modules (ex: preprocessing modules) required in inference
 - Run multiple deep learning experiments in parallel on multiples GPUs (powered by [hydra](https://hydra.cc/docs/intro/), and python multiprocessing)
@@ -15,46 +31,48 @@
     import torch
     import torch.nn as nn
 
     # Generate data
     x = torch.rand(200,1)
     y = 5*x+2
 
-    model = nn.Linear(1,1)
+    network = nn.Linear(1,1)
     dataset = torch.utils.data.TensorDataset(x, y)
     criterion = nn.MSELoss()
     cfg = {
     'lr': 1e-2,
     'batch_size': 32,
     'epoch': 10 # optional
     }
 
     # Training configuration. All you need to train a neural network
     kwargs = {
-    'model':model,
+    'network':network,
     'dataset':dataset,
     'cfg_train':cfg,
     'criterion':criterion,
     'name': 'Test' # optional
     }
     trainer = hs.N.Node(**kwargs)
 
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-    trainer.model.to(device)
+    trainer.network.to(device)
 
     # Train for predefined number of epochs
     trainer.train() # Train for predefined number of epochs
     trainer.train(5) # Train for specified number of epochs
     trainer.train(epoch=5) # Same thing with trainer.train(5)
     trainer.train(step=500) # Train for specified number of updates
 
-    node.model.cpu()
+    trainer.network.cpu()
 
 and simply run multiple batch of experiments with a single line command such as:
 
     python train.py -m lr=1e-3,1e-2 batch_size=32,64 "random_seed=range(0,5)" \
     hydra/launcher=joblib hydra.launcher.n_jobs=8
     # Runs total of 2*2*5=40 batch of experiments, with 8 processes at a time. Experiment results are stored in hydra.sweep.dir which can be overridden.
 
 To do
 - [ ] Draw figures to explain hideandseek
 - [ ] GUI for generating experiment scripts when conducting variable sweeps
+
+
```

### Comparing `hideandseek-0.1.9/hideandseek/dataset.py` & `hideandseek-0.2.0/hideandseek/dataset.py`

 * *Files identical despite different names*

### Comparing `hideandseek-0.1.9/hideandseek/eval.py` & `hideandseek-0.2.0/hideandseek/eval.py`

 * *Files 5% similar despite different names*

```diff
@@ -66,20 +66,20 @@
         # Infer targets_type and create corresponding test_f and result_dict
         if targets_type is None:
             if hasattr(dataset, 'targets_type'):
                 targets_type = dataset.targets_type
             else:
                 raise Exception('When test_f and result_dict is not given, targets_type must be given or the dataset must have the attribute "targets_type"')
         assert targets_type in targets_type_list, f'targets_type must be one of {targets_type_list}, received: {targets_type}'
-        test_f, result_f = get_test_f(targets_type, keep_x=keep_x)
+        test_f, result_dict = get_test_f(targets_type, keep_x=keep_x)
     else:
         raise Exception(f'test_f and result_dict must either both be provided or None, received [test_f: {test_f}][result_dict: {result_dict}]')
     return test_f, result_dict
 
-def test_torch(network, dataset, batch_size=64, targets_type=None, test_f=None, result_dict=None, keep_x=False, num_workers=0, amp=False):
+def test_network(network, dataset, batch_size=64, targets_type=None, test_f=None, result_dict=None, keep_x=False, num_workers=0, amp=False):
     '''
     inference stage of network.
     '''
     test_f, result_dict = _test_assertion(dataset=dataset, targets_type=targets_type, test_f=test_f, result_dict=result_dict, keep_x=keep_x)
 
     device = T.torch.get_device(network) # Test on the network's device
     network.eval()
@@ -87,35 +87,37 @@
     # dataset, misc_temp = transfer_misc(node, dataset) # Assume the dataset is consistent
     kwargs_dataloader = reproducible_worker_dict()
     test_loader = D.DataLoader(dataset, batch_size=batch_size, shuffle=False, drop_last=False, num_workers=num_workers, **kwargs_dataloader)
 
     with torch.no_grad():
         # Mixed precision for acceleration
         if amp:
-            with torch.cuda.amp.autocast():
+            with torch.autocast(device_type=device.type):
                 for data in test_loader:
                     result_dict = test_f(data=data, network=network, result_dict=result_dict, device=device, keep_x=keep_x)
         else:
             for data in test_loader:
                 result_dict = test_f(data=data, network=network, result_dict=result_dict, device=device, keep_x=keep_x)
 
-    result_dict = {k: np.concatenate(v, axis=0) if len(v)>0 else v for k, v in result_dict.items()}
+    result_dict = {k: torch.cat(v, dim=0) if len(v)>0 else v for k, v in result_dict.items()}
+    if amp: result_dict = {k: v.to(torch.float16) for k, v in result_dict.items()} # Transform bfloat16 (amp) to regular float16
+    result_dict = {k: v.numpy() for k, v in result_dict.items()}
 
-    network.train() # Is this necessary?
+    # network.train() # Is this necessary?
 
     return result_dict
 
 def test_model(model, dataset, batch_size=64, targets_type=None, test_f=None, result_dict=None, keep_x=False, num_workers=0, amp=False):
     '''
     wrapper around model.
     transfers get_f (preprocessing modules) of node to dataset, and returns them to original dataset after inference.
     '''
     network = model.network
     dataset, misc_temp = transfer_misc(model, dataset)
-    result_dict = test_torch(network, dataset, batch_size, targets_type, test_f, result_dict, keep_x, num_workers, amp)
+    result_dict = test_network(network, dataset, batch_size, targets_type, test_f, result_dict, keep_x, num_workers, amp)
     dataset = inverse_transfer_misc(misc_temp, dataset)
 
     return result_dict
 
 def evaluate(results, metrics):
     if type(metrics) is dict:
         scores = {}
@@ -152,52 +154,52 @@
 
 def _test_base(data, network, result_dict, device=None, keep_x=False):
     # device = device if device is not None else T.torch.get_device(network)
     x = data['x'].to(device)
     y = data['y'].to(device)
     y_hat = network(x)
 
-    result_dict['y_true'].append(y.cpu().numpy())
-    result_dict['y_hat'].append(y_hat.cpu().numpy())
-    if keep_x: result_dict['x'].append(x.cpu().numpy())
+    result_dict['y_true'].append(y.cpu())
+    result_dict['y_hat'].append(y_hat.cpu())
+    if keep_x: result_dict['x'].append(x.cpu())
     return result_dict
 
 def _test_categorical(data, network, result_dict, device=None, keep_x=False):
     # Is y_hat necessary? for torch_crossentropyloss? any other methods?
     x = data['x'].to(device)
     y = data['y'].to(device)
     y_hat = network(x)
     y_score = torch.softmax(y_hat, dim=1) # (N, n_classes)
 
-    result_dict['y_true'].append(y.cpu().numpy())
-    result_dict['y_hat'].append(y_hat.cpu().numpy())
-    result_dict['y_score'].append(y_score.cpu().numpy())
-    result_dict['y_pred'].append(y_score.argmax(axis=-1).cpu().numpy())
-    if keep_x: result_dict['x'].append(x.cpu().numpy())
+    result_dict['y_true'].append(y.cpu())
+    result_dict['y_hat'].append(y_hat.cpu())
+    result_dict['y_score'].append(y_score.cpu())
+    result_dict['y_pred'].append(y_score.argmax(axis=-1).cpu())
+    if keep_x: result_dict['x'].append(x.cpu())
     return result_dict
 
 def _test_multihead_categorical(data, network, result_dict, device=None, keep_x=False):
     x = data['x'].to(device)
     y = data['y'].to(device)
     y_hat = network(x)
     y_score = torch.softmax(y_hat, dim=-1) # (N, subtype, n_classes)
 
-    result_dict['y_true'].append(y.cpu().numpy())
-    result_dict['y_hat'].append(y_hat.cpu().numpy())
-    result_dict['y_score'].append(y_score.cpu().numpy())
-    result_dict['y_pred'].append(y_score.argmax(axis=-1).cpu().numpy())
-    if keep_x: result_dict['x'].append(x.cpu().numpy())
+    result_dict['y_true'].append(y.cpu())
+    result_dict['y_hat'].append(y_hat.cpu())
+    result_dict['y_score'].append(y_score.cpu())
+    result_dict['y_pred'].append(y_score.argmax(axis=-1).cpu())
+    if keep_x: result_dict['x'].append(x.cpu())
     return result_dict
 
 def _test_autoencode(data, network, result_dict, device=None):
     x = data['x'].to(device)
     z = network.encoder(x)
     x_hat = torch.sigmoid(network.decoder(z))
 
-    x, z, x_hat = x.cpu().numpy(), z.cpu().numpy(), x_hat.cpu().numpy()
+    x, z, x_hat = x.cpu(), z.cpu(), x_hat.cpu()
 
     result_dict['x'].append(x)
     result_dict['z'].append(z)
     result_dict['x_hat'].append(x_hat)
     return result_dict
 
 # %%
@@ -256,50 +258,57 @@
     (tn, fp), (fn, tp) = metrics.confusion_matrix(result['y_true'], result['y_pred'])
     if (tn+fp)==0:
         warnings.warn('invalid value in specificity_score, setting to 0.0')
         return 0
     return tn / (tn+fp)
 
 # Multiclass classification
-def classification_report_full(result, discard_ovr=False):
+def classification_report_full(result, ovr=True):
     '''
     Adds additional metrics to sklearn.classification_report
     '''
-    # TODO: add y_score
     y_score = result['y_score'] if 'y_score' in result else None
-
     y_true, y_pred = result['y_true'], result['y_pred']
+    
     scores = metrics.classification_report(y_true, y_pred, output_dict=True)
-    scores_ovr = {k:dcopy(v) for k, v in scores.items() if k.isnumeric()}
-    scores_all = {k:dcopy(v) for k, v in scores.items() if not k.isnumeric()}
-    more_scorers = {'sensitivity': sensitivity_score, 'specificity': specificity_score, 'accuracy': accuracy_score} # Optimize to reduce redundant computations?
-
-    # Additional metrics
-    for c in scores_ovr.keys():
-        c_int = int(c)
-        y_true__c, y_pred_c = y_true==c_int, y_pred==c_int
-        for scorer_name, scorer in more_scorers.items():
-            scores_ovr[c][scorer_name] = scorer({'y_true': y_true__c, 'y_pred': y_pred_c})
+    scores['mcc'] = metrics.matthews_corrcoef(y_true, y_pred)
+
+    if ovr:
+        scores_ovr = {k:dcopy(v) for k, v in scores.items() if k.isnumeric()}
+        scores_all = {k:dcopy(v) for k, v in scores.items() if not k.isnumeric()}
 
-    if y_score is not None:
+        more_scorers_y_pred = {'sensitivity': sensitivity_score, 'specificity': specificity_score, 'accuracy': accuracy_score} # Optimize to reduce redundant computations?
+        more_scorers_y_score = {}
+
+        # Additional metrics
         for c in scores_ovr.keys():
             c_int = int(c)
-            y_score_ = y_score[:, c_int]
-            metrics.roc_auc_score(y_true, y_score_)
+            y_true__c, y_pred_c = y_true==c_int, y_pred==c_int
+            for scorer_name, scorer in more_scorers_y_pred.items():
+                scores_ovr[c][scorer_name] = scorer({'y_true': y_true__c, 'y_pred': y_pred_c})
+
+        if y_score is not None:
+            more_scorers_y_score['auroc'] = metrics.roc_auc_score
+            for c in scores_ovr.keys():
+                c_int = int(c)
+                y_true_ = y_true==c_int
+                y_score_ = y_score[:, c_int]
+                for scorer_name, scorer in more_scorers_y_score.items():
+                    scores_ovr[c][scorer_name] = scorer(y_true_, y_score_)
+
+        # summary
+        more_scorers = list(more_scorers_y_pred.keys()) + list(more_scorers_y_score.keys())
+        for scorer_name in more_scorers:
+            scores_all['macro avg'][scorer_name] = np.mean([scores_ovr_[scorer_name] for scores_ovr_ in scores_ovr.values()])
+            scores_all['weighted avg'][scorer_name] = np.sum([scores_ovr_[scorer_name]*scores_ovr_['support'] for scores_ovr_ in scores_ovr.values()]) / scores_all['weighted avg']['support']
 
-    # summary
-    for scorer_name, scorer in more_scorers.items():
-        scores_all['macro avg'][scorer_name] = np.mean([scores_ovr_[scorer_name] for scores_ovr_ in scores_ovr.values()])
-        scores_all['weighted avg'][scorer_name] = np.sum([scores_ovr_[scorer_name]*scores_ovr_['support'] for scores_ovr_ in scores_ovr.values()]) / scores_all['weighted avg']['support']
+        scores.update(scores_ovr)
+        scores.update(scores_all)
 
-    if discard_ovr:
-        return scores_all
-    else:
-        scores_ovr.update(scores_all)
-        return scores_ovr
+    return scores
 
 # Multihead classification score
 def multihead_accuracy_score(y_pred, y):
     '''
     :param y_pred: array of shape (N, subtype)
     :param y: array of shape (N, subtype)
     '''
```

### Comparing `hideandseek-0.1.9/hideandseek/fv.py` & `hideandseek-0.2.0/hideandseek/fv.py`

 * *Files identical despite different names*

### Comparing `hideandseek-0.1.9/hideandseek/loss.py` & `hideandseek-0.2.0/hideandseek/loss.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 
-import numpy as np
 import torch
 import torch.nn as nn
 
 log = logging.getLogger(__name__)
 
 def weighted_crossentropy_loss(dataset, classes=None):
     """
@@ -22,37 +21,36 @@
     Returns
     -------
     criterion: nn.CrossEntropyLoss object
         nn.CrossEntropyLoss with class weights applied
     """
     # Loss function
     if hasattr(dataset, 'get_y_all'):
-        y = np.array(dataset.get_y_all())
+        y = dataset.get_y_all()
     elif hasattr(dataset, 'get_y'):
-        y = np.array([dataset.get_y(idx) in idx in range(len(dataset))])
+        y = torch.stack([dataset.get_y(idx) for idx in range(len(dataset))])
     else:
         data_sample = next(iter(dataset))
         if isinstance(data_sample, dict):
-            y = np.array([data['y'] for data in dataset])
+            y = torch.stack([data['y'] for data in dataset])
         elif isinstance(data_sample, tuple) and len(data_sample)==2:
-            y = np.array([data[1] for data in dataset])
+            y = torch.stack([data[1] for data in dataset])
         else:
             raise Exception(f'unknown dataset return type: {type(data_sample)}')
-    y_unique, y_count = np.unique(y, return_counts=True)
-    y_count = y_count[np.argsort(y_unique)] # Sort
+    y_unique, y_count = torch.unique(y, return_counts=True, sorted=True) # sorted by default
+
     if classes is None:
-        class_weight = torch.tensor(1/y_count, dtype=torch.float)
-        class_weight /= class_weight.sum()
+        class_weight = 1/y_count
     else:
         log.info(f'[weighted_crossentropyloss] classes found, expanding weight vector to: {len(classes)}')
         class_weight = torch.zeros(len(classes))
         assert set(y_unique).issubset(set(classes))
         for c, y_count_ in zip(y_unique, y_count):
-            class_weight[c] = 1/y_count_
-        class_weight /= class_weight.sum()
+            class_weight[c] = 1/y_count_ 
+    class_weight /= class_weight.sum()
 
     criterion = nn.CrossEntropyLoss(weight = class_weight)
-    log.info('weighted_crossentropyloss - CrossEntropyLoss')
+    log.info('Weighted_crossentropyloss - CrossEntropyLoss')
     log.info(f'y_count: {y_count}')
     log.info(f'CrossEntropy Weighted: {criterion.weight}')
 
-    return criterion
+    return criterion
```

### Comparing `hideandseek-0.1.9/hideandseek/model.py` & `hideandseek-0.2.0/hideandseek/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,20 @@
+import torch
+
+import tools
+
+from . import utils as U
 
 class BaseModel(object):
     call_arguments = []
 
-    def __init__(self, nn, amp=False):
-        self.nn = nn
+    def __init__(self, network, amp=False, misc={}):
+        self.network = network
         self.amp = amp
+        self.misc = misc # For certain metadata used for pre/postprocessing
 
     def __call__(self, batch=False, *args, **kwargs):
         """
         The preprocess/postprocess assumes batch dimension always exists.
 
         Parameters
         ----------
@@ -23,19 +29,19 @@
             The return value of a model
         """
         # Trim call_arguments (which are mostly not np.ndarray)
         call_arguments = {k:v for k, v in kwargs.items() if k in self.call_arguments}
         kwargs = {k:v for k, v in kwargs.items() if k not in self.call_arguments}
 
         # Setup inference
-        self.nn.eval()
-        device = U.get_device(self.nn)
+        self.network.eval()
+        device = tools.torch.get_device(self.network)
         if not batch: # If the given values are does not have batch dimension,
-            args = tuple(O.add_batch_dim(arg) for arg in args)
-            kwargs = {k: O.add_batch_dim(v) for k, v in kwargs.items()}
+            args = tuple(U.add_batch_dim(arg) for arg in args)
+            kwargs = {k: U.add_batch_dim(v) for k, v in kwargs.items()}
 
         # Preprocess & Convert to torch.Tensor
         arrays = self.preprocess(*args, **kwargs)
         arrays = arrays if isinstance(arrays, tuple) else (arrays,)
         tensors = [torch.as_tensor(array, device=device) for array in arrays]
 
         # Forward pass without gradient & Convert to numpy.ndarray
@@ -46,27 +52,27 @@
             with torch.no_grad(): tensors = self.forward(*tensors, **call_arguments)
         tensors = tensors if isinstance(tensors, tuple) else (tensors,)
         arrays = [tensor.cpu().numpy() if isinstance(tensor, torch.Tensor) else tensor for tensor in tensors]
 
         # Postprocess
         arrays = self.postprocess(*arrays)
         if not batch:
-            arrays = tuple(O.remove_batch_dim(array) if isinstance(array, (np.ndarray, dict)) else array for array in arrays) if isinstance(arrays, tuple) else O.remove_batch_dim(arrays)
+            arrays = tuple(U.remove_batch_dim(array) if isinstance(array, (np.ndarray, dict)) else array for array in arrays) if isinstance(arrays, tuple) else U.remove_batch_dim(arrays)
 
         return arrays # May be tuple or numpy.ndarray
 
     def forward(self, *args, **kwargs):
         '''
         May be overridden in children classes
         '''
-        return self.nn(*args, **kwargs)
+        return self.network(*args, **kwargs)
 
     def preprocess(self, *args, **kwargs):
         '''
-        Preprocess the arguments into a form that NN could compute.
+        Preprocess the arguments into a form that network could compute.
         '''
         return *args, *kwargs.values()
 
     def inv_preprocess(self, *args, **kwargs):
         return *args, *kwargs.values()
 
     def postprocess(self, *args, **kwargs):
```

### Comparing `hideandseek-0.1.9/hideandseek/plot.py` & `hideandseek-0.2.0/hideandseek/plot.py`

 * *Files identical despite different names*

### Comparing `hideandseek-0.1.9/hideandseek/trainer.py` & `hideandseek-0.2.0/hideandseek/trainer.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,36 +3,39 @@
 
 '''
 import logging
 import os
 import shutil
 from copy import deepcopy as dcopy
 
+import numpy as np
+
 import torch
 import torch.optim as optim
 import torch.utils.data as D
 
 import tools # since T is used as a variable in this module, refrain from "import tools as T"
 import tools.torch
 import tools.modules
 
 # from . import validation as V
 from . import utils as U
+from . import eval as E
+from . import model as M
 
 # __all__ = [
 # 'Trainer'
 # ]
 
 # %%
 log = logging.getLogger(__name__)
 
 # %%
-
 class Trainer:
-    def __init__(self, network, train_dataset=None, cfg_train={}, criterion=None, network_dir=None, node_dir=None, cfg_val=None, val_dataset=None, val_metrics=None, name='default', verbose=True, amp=False, reproduce=True):
+    def __init__(self, network, train_dataset=None, cfg_train={}, criterion=None, network_dir=None, model_dir=None, cfg_val=None, val_dataset=None, val_metrics=None, name='default', verbose=True, amp=False, reproduce=True):
         '''
         Things Trainer do:
         - train network with early stopping, given hyperparameters
         - save/load network with necessary preprocessing pipeline
 
         :param network: torch.nn.Module object
         :param train_dataset: torch.utils.data.Dataset object
@@ -55,46 +58,47 @@
             criterion (optional, if val_metrics is dict for multiple metrics) 
 
         :param criterion: torch.nn.Module object, used to compute loss function
 
         Recommended way of making hs.node.Node object is like the following:
 
             kwargs = {'network': Network(), 'train_dataset': train_dataset, 'validation': None, 'cfg_train': cfg.train,
-                    'criterion': criterion, 'network_dir': path['network'], 'node_dir': path['node'], 'verbose': True, 'amp': True}
+                    'criterion': criterion, 'network_dir': path['network'], 'model_dir': path['node'], 'verbose': True, 'amp': True}
             node = hs.node.Node(**kwargs)
         '''
         # Store configurations
         self.network = network
         self.train_dataset = train_dataset
         self.cfg_train = dcopy(dict(cfg_train))
         self.criterion = criterion
         self.network_dir = network_dir
-        self.node_dir = node_dir
+        self.model_dir = model_dir
 
-        self.cfg_val = dcopy(dict(cfg_val))
+        self.cfg_val = dcopy(dict(cfg_val)) if cfg_val is not None else {}
         self.val_dataset = val_dataset
         self.val_metrics = val_metrics
         self.earlystopper = EarlyStopper(increase_better=cfg_val['increase_better'], patience=cfg_val['patience']) if self.val_dataset is not None else None
         if 'target_dataset' in self.cfg_val:
-            assert self.cfg_val['target_dataset'] in self.val_dataset, f'[Validation setup] target_dataset: {self.cfg_val["target_dataset"]} not found in val_dataset: {self.val_dataset.keys()}'
-        assert self.val_dataset is not None and self.val_metrics is not None, f'val_dataset and val_metrics must be given together or neither. val_dataset: {self.val_dataset}, val_metrics: {self.val_metrics}'
+            if type(self.val_dataset)==dict:
+                assert self.cfg_val['target_dataset'] in self.val_dataset, f'[Validation setup] target_dataset: {self.cfg_val["target_dataset"]} not found in val_dataset: {self.val_dataset.keys()}'
+            assert ~((self.val_dataset is not None) ^ (self.val_metrics is not None)), f'val_dataset and val_metrics must be given together or neither. val_dataset: {self.val_dataset}, val_metrics: {self.val_metrics}'
 
         self.name = name
         self.verbose = verbose
         self.amp = amp
         self.reproduce = reproduce
 
         # Initializations
         if self.network_dir is not None:
             if os.path.exists(self.network_dir): log.warning(f'path: {self.network_dir} exists. Be careful')
             os.makedirs(self.network_dir, exist_ok=True)
 
-        if self.node_dir is not None:
-            if os.path.exists(self.node_dir): log.warning(f'path: {self.node_dir} exists. Be careful')
-            os.makedirs(self.node_dir, exist_ok=True)
+        if self.model_dir is not None:
+            if os.path.exists(self.model_dir): log.warning(f'path: {self.model_dir} exists. Be careful')
+            os.makedirs(self.model_dir, exist_ok=True)
 
         self.train_meter = tools.modules.AverageMeter() # Tracks loss per epoch
         self.loss_tracker = tools.modules.ValueTracker() # Tracks loss over all training
         self.set_model()
         self.reset()
 
         self._targets_type = self.infer_targets_type()
@@ -107,45 +111,58 @@
         if self.verbose:
             print(content)
         else:
             log.info(content)
 
     def set_model(self):
         '''Set miscellaneous variables'''
-        self.model = BaseModel(self.network, amp=self.amp)
+        self.model = M.BaseModel(self.network, amp=self.amp)
         self.misc = tools.TDict()
         if self.train_dataset is not None:
             if hasattr(self.train_dataset, 'get_f'): # get_f equal to preprocessing pipeline before feeding to network
                 self.print('get_f found in loader.dataset')
                 self.misc.get_f = self.train_dataset.get_f
 
     def validate(self):
         patience_end = False
+        self.print(f'[Node: {self.name}] Validation')
         if self.val_dataset is not None:
             if type(self.val_dataset)==dict:
                 scores = {}
                 for name, dataset in self.val_dataset.items():
-                    d_results = hs.E.test_model(self.model, dataset, batch_size=self.cfg_train['batch_size'], amp=self.amp)
-                    score = evaluate(d_results, self.val_metrics)
+                    d_results = E.test_model(self.model, dataset, batch_size=self.cfg_val['batch_size'], amp=self.amp)
+                    if any([np.isnan(v).any() for v in d_results.values()]):
+                        log.warning(f'[Node: {self.name}][validate] NaN found in d_results. Skipping validation...')
+                        score = {self.cfg_val['criterion']: self.earlystopper.best_score}
+                    else:
+                        score = E.evaluate(d_results, self.val_metrics)
                     scores[name] = score
                     self.print(f'[dataset_name: {name}] Validation Score: {score}')
                 score = scores[self.cfg_val['target_dataset']]
             else:
-                d_results = hs.E.test_model(self.model, self.val_dataset, batch_size=self.cfg_train['batch_size'], amp=self.amp)
-                score = evaluate(d_results, self.val_metrics)
-                self.print(f'Validation Score: {scores}')
+                d_results = E.test_model(self.model, self.val_dataset, batch_size=self.cfg_val['batch_size'], amp=self.amp)
+                if any([np.isnan(v).any() for v in d_results.values()]):
+                    log.warning(f'[Node: {self.name}][validate] NaN found in d_results. Skipping validation...')
+                    score = {self.cfg_val['criterion']: self.earlystopper.best_score}
+                else:
+                    score = E.evaluate(d_results, self.val_metrics)
+                self.print(f'Validation Score: {score}')
             
             if self.earlystopper is not None:
                 if type(score) is dict:
                     score_ = score[self.cfg_val['criterion']]
-
+                else:
+                    score_ = score
+                    
                 patience_end = self.earlystopper.step(self, score_)
                 if patience_end:
                     self.print('patience met, flushing earlystopper history')
                     self.earlystopper.history.reset()
+                    
+        torch.cuda.empty_cache()
         return patience_end
 
     def generate_loader(self):
         if self.train_dataset is not None:
             reproduce_kwargs = U.reproducible_worker_dict() if self.reproduce else {}
             drop_last = len(self.train_dataset) % self.cfg_train['batch_size'] == 1 # To avoid batch normalization layers from raising exceptions
             self.loader = D.DataLoader(self.train_dataset, batch_size=self.cfg_train['batch_size'], shuffle=True, drop_last=drop_last, **reproduce_kwargs)
@@ -188,29 +205,29 @@
                 self.cfg_train['cv_step'] = len(self.loader)
             self.validate() # initial testing
 
         # Make new optimizer
         if new_op or not hasattr(self, 'op'):
             if not hasattr(self, 'op') and not new_op:
                 log.warning("new_op=False when there's no pre-existing optimizer. Ignoring new_op...")
-            # Weight decay optional
-            self.op = optim.Adam(self.network.parameters(), lr=self.cfg_train['lr'], weight_decay=self.cfg_train['weight_decay']) if 'weight_decay' in self.cfg_train \
-                        else optim.Adam(self.network.parameters(), lr=self.cfg_train['lr'])
-            # self.op = optim.Adam(self.network.parameters(), **self.cfg_train)
+            
+            l_kwargs = ['lr', 'weight_decay', 'amsgrad']
+            kwargs = {key: self.cfg_train[key] for key in l_kwargs if key in self.cfg_train}
+            self.op = optim.Adam(self.network.parameters(), **kwargs)
 
         if horizon == 'epoch':
-            self._step_epoch(T=epoch, no_val=no_val, device=device)
+            self._update_epoch(T=epoch, no_val=no_val, device=device)
         elif horizon=='step':
-            self._step_step(T=step, no_val=no_val, device=device)
+            self._update_step(T=step, no_val=no_val, device=device)
 
         # TODO: Return criterion back to its original device, meaning we have to store its previous device info
         self.criterion = self.criterion.cpu()
         return self.loss_tracker
 
-    def _step_epoch(self, T, no_val=False, device=None):
+    def _update_epoch(self, T, no_val=False, device=None):
         self._device = device if device is not None else tools.torch.get_device(self.network)
 
         _iter = 0
         for epoch in range(1, T+1):
             self.train_meter.reset()
             self.epoch_f()
             for batch_i, data in enumerate(self.loader, 1):
@@ -223,15 +240,15 @@
                 # Validation
                 if (self.val_dataset is not None) and (not no_val) and (_iter % self.cfg_train['cv_step']==0):
                     patience_end = self.validate()
                     if patience_end: # If patience has reached, stop training
                         self.print('Patience met, stopping training')
                         return None # return None since double break is impossible in python
 
-    def _step_step(self, T, no_val=False, device=None):
+    def _update_step(self, T, no_val=False, device=None):
         self._device = device if device is not None else tools.torch.get_device(self.network)
         if hasattr(self, '_loader_inst'): del self._loader_inst # Load data from the 1st batch
 
         for _iter in range(1, T+1):
             # Get Data
             try:
                 if hasattr(self, '_loader_inst'):
@@ -244,15 +261,15 @@
                 self.epoch_f()
                 self._loader_inst = iter(self.loader)
                 data = next(self._loader_inst)
                 self.n_batch = 1
 
             self.iter += 1
             loss = self._update(data)
-            self.print(f'[Node: {self.name}][iter_sum: {self.iter}][Iter: {_iter}/{T}][Batch: {self.n_batch}/{len(self.loader)}][Loss: {loss:.7f} (Avg: {self.train_meter.avg:.7f})]')
+            self.print(f'[iter_sum: {self.iter}][Iter: {_iter}/{T}][Batch: {self.n_batch}/{len(self.loader)}][Loss: {loss:.6f} (Avg: {self.train_meter.avg:.6f})]')
 
             self.loss_tracker.step(self.iter, loss)
 
             # Validation
             if (self.val_dataset is not None) and (not no_val) and (_iter % self.cfg_train['cv_step']==0):
             # if (not no_val) and (self.iter % self.cfg_train.cv_step==0):
                 patience_end = self.validate()
@@ -314,15 +331,15 @@
             data = [x.to(self._device) for x in data]
             N = len(data[0]) # number of data in batch
             outputs = self.forward(*data)
 
         # When data is given as a dict
         elif datatype is dict:
             data = {key: value.to(self._device) for key, value in data.items()}
-            N = len(next(iter(data))) # number of data in batch
+            N = len(next(iter(data.values()))) # number of data in batch
             outputs = self.forward(**data)
 
         else:
             raise Exception(f'return type from dataset must be one of [tuple, list, dict], received: {datatype}')
         return outputs, N
 
     def forward(self, x, y):
@@ -334,21 +351,21 @@
         """
 
         y_hat = self.network(x)
 
         return y_hat, y
 
     def _criterion(self, outputs):
-        outputstype = outputstype
+        outputstype = type(outputs)
         if outputstype is tuple or outputstype is list:
             loss = self.criterion(*outputs)
         elif outputstype==dict:
             loss = self.criterion(**outputs)
         else:
-            raise Exception(f'return type from forward must be one of [tuple, list, dict], received: {type(data_pred)}')
+            raise Exception(f'return type from forward must be one of [tuple, list, dict], received: {type(outputs)}')
         return loss
 
     def epoch_f(self):
         # TODO: rename to forward hook? epoch_hook?
         '''function to call every other epoch. May be used in child class'''
         pass
 
@@ -413,22 +430,32 @@
 
         if 'threshold' in state_dict.keys():
             self.print(f'Updating threshold: {state_dict["threshold"]}')
             self.threshold = state_dict['threshold']
             del state_dict['threshold']
 
         self.__dict__.update(state_dict) # update attributes
+        
+    def load_best_model(self):
+        if self.earlystopper is not None:
+            if self.earlystopper.best_network != None:
+                self.print(f'Loading best network: {self.earlystopper.best_network}')
+                self.network.load_state_dict(torch.load(self.earlystopper.best_network))
+            else:
+                self.print(f'No best_network found in self.earlystopper. No network loaded.')
+        else:
+            self.print('self.earlystopper not defined. No network loaded.')
 
     def save(self, path=None, best=True):
         '''
         Save the following:
         state_dict() -> path/state_dict.p
         network.state_dict() -> path/network.pt
         '''
-        path = self.node_dir if path is None else path
+        path = self.model_dir if path is None else path
         self.print(f'[Node: {self.name}]')
 
         state_dict_path = os.path.join(path, 'node.p')
         self.print(f'[save] Saving node info to: {state_dict_path}')
         state_dict = self.state_dict()
         self.print(f'[save] state_dict: {list(state_dict.keys())}')
         tools.save_pickle(state_dict, state_dict_path)
@@ -451,19 +478,89 @@
 
     def load(self, path=None):
         '''
         load state_dict() and network:
         path/node.p -> state_dict
         path/network.pt -> network.state_dict
         '''
-        path = self.node_dir if path is None else path
+        path = self.model_dir if path is None else path
         self.print(f'[Node: {self.name}]')
 
         state_dict_path = os.path.join(path, 'node.p')
         self.print(f'[load] Loading from path: {state_dict_path}')
         state_dict = tools.load_pickle(state_dict_path)
         self.print(f'[load] Updating: {list(state_dict.keys())}')
         self.load_state_dict(state_dict)
 
         network_path = os.path.join(path, 'network.pt')
         self.print(f'[load] Loading network from: {network_path}')
         self.network.load_state_dict(torch.load(network_path))
+
+class EarlyStopper():
+    """
+    Returns True if the metric has stopped improving for the given number of patience steps.
+    Saves network in the given path and remembers which network is the best.
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
+    def __repr__(self):
+        return f'<EarlyStopper>\npatience: {self.patience}\nincrease_better: {self.increase_better}'
+
+    def __init__(self, increase_better, patience, save_dir='network_temp', discard_best=True):
+        self.increase_better = increase_better
+        self.patience = patience
+        self.save_dir = save_dir
+        self.discard_best = discard_best
+
+        os.makedirs(self.save_dir, exist_ok=True)
+        self.history = tools.modules.ValueTracker() # For now, only track single score
+        self.reset()
+
+    def step(self, trainer, score, filename=None):
+        filename = f'network_{trainer.iter}.pt' if filename is None else filename
+
+        self.history.step(trainer.iter, score)
+
+        # Save best network
+        if isbetter(score_best=self.best_score, score=score, increase_better=self.increase_better):
+            path = os.path.join(self.save_dir, filename)
+
+            log.info(f'[EarlyStopping] New best score: {self.best_score} -> {score}')
+            log.info(f'[EarlyStopping] Saved network: {path}')
+            torch.save(trainer.network.state_dict(), path)
+            if self.discard_best and self.best_network!=None:
+                os.remove(self.best_network)
+
+            self.best_score = score
+            self.best_network = path
+
+            # Clear patience tracking
+            self.history.reset()
+
+        # patience_end == True when best network did not appear for self.patience times
+        patience_end = self.patience == len(self.history)
+        log.info(f'[EarlyStopping][patience: {len(self.history)}/{self.patience}]')
+
+        return patience_end
+
+    def reset(self):
+        # log.info('[EarlyStopper] Resetting...')
+        self.history.reset()
+        self.best_network = None
+        if self.increase_better:
+            self.best_score = -float('inf')
+        else:
+            self.best_score = float('inf')
+
+def isbetter(score_best: float, score: float, increase_better: bool):
+    return (not increase_better and score<score_best) or (increase_better and score>score_best)
```

### Comparing `hideandseek-0.1.9/hideandseek/validation.py` & `hideandseek-0.2.0/hideandseek/validation.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,20 +79,18 @@
         for (score_type, valuetracker), ax_ in zip(self.history.items(), ax):
             valuetracker.plot(ax=ax_)
             ax_.set_title(score_type)
         return ax
 
     def reset(self):
         pass
-
-
 class EarlyStopper():
     """
     Returns True if the metric has stopped improving for the given number of patience steps.
-    Saves model in the given path and remembers which model is the best.
+    Saves network in the given path and remembers which network is the best.
 
     Parameters
     ----------
     arg : array-like of shape (n_samples,), default=None
         Argument explanation.
         If ``None`` is given, those that appear at least once
         .. versionadded:: 0.18
@@ -117,40 +115,40 @@
         self.reset()
 
     def step(self, trainer, score, filename=None):
         filename = f'network_{trainer.iter}.pt' if filename is None else filename
 
         self.history.step(trainer.iter, score)
 
-        # Save best model
+        # Save best network
         if isbetter(score_best=self.best_score, score=score, increase_better=self.increase_better):
             path = os.path.join(self.save_dir, filename)
 
             log.info(f'[EarlyStopping] New best score: {self.best_score} -> {score}')
-            log.info(f'[EarlyStopping] Saved model: {path}')
-            torch.save(trainer.model.state_dict(), path)
-            if self.discard_best and self.best_model!=None:
-                os.remove(self.best_model)
+            log.info(f'[EarlyStopping] Saved network: {path}')
+            torch.save(trainer.network.state_dict(), path)
+            if self.discard_best and self.best_network!=None:
+                os.remove(self.best_network)
 
             self.best_score = score
-            self.best_model = path
+            self.best_network = path
 
             # Clear patience tracking
             self.history.reset()
 
-        # patience_end == True when best model did not appear for self.patience times
+        # patience_end == True when best network did not appear for self.patience times
         patience_end = self.patience == len(self.history)
         log.info(f'[EarlyStopping][patience: {len(self.history)}/{self.patience}]')
 
         return patience_end
 
     def reset(self):
         # log.info('[EarlyStopper] Resetting...')
         self.history.reset()
-        self.best_model = None
+        self.best_network = None
         if self.increase_better:
             self.best_score = -float('inf')
         else:
             self.best_score = float('inf')
 
 # class EarlyStopper():
 #     def __repr__(self):
@@ -178,38 +176,38 @@
 #             assert len(score_target_validation)==1, f"primary_score must be specified when there's more than 1 scorer functions, received: {len(score_target_validation)}"
 #             score = list(score_target_validation.values())[0]
 #             # assert type(score) is not dict, 'when primary_score is not given, the given score must be a scalar'
 #         else:
 #             score = score_target_validation[self.primary_score]
 #         self.history.step(node.iter, score)
 
-#         # Save best model
+#         # Save best network
 #         if isbetter(score_best=self.best_score, score=score, increase_better=self.increase_better):
 #             log.info(f'[EarlyStopping]New best score: {self.best_score} -> {score}')
-#             log.info(f'[EarlyStopping]Saved model: {path}')
-#             torch.save(node.model.state_dict(), path)
-#             if self.discard_best and self.best_model!=None:
-#                 os.remove(self.best_model)
+#             log.info(f'[EarlyStopping]Saved network: {path}')
+#             torch.save(node.network.state_dict(), path)
+#             if self.discard_best and self.best_network!=None:
+#                 os.remove(self.best_network)
 
 #             self.best_score = score
-#             self.best_model=path
+#             self.best_network=path
 
 #             # Clear patience tracking
 #             self.history.reset()
 
-#         # patience_end == True when best model did not appear for self.patience times
+#         # patience_end == True when best network did not appear for self.patience times
 #         patience_end = self.patience == len(self.history)
 #         log.info(f'[EarlyStopping][patience: {len(self.history)}/{self.patience}]')
 
 #         return patience_end
 
 #     def reset(self):
 #         # log.info('[EarlyStopper] Resetting...')
 #         self.history.reset()
-#         self.best_model = None
+#         self.best_network = None
 #         if self.increase_better:
 #             self.best_score = -float('inf')
 #         else:
 #             self.best_score = float('inf')
 
 class EarlyStopping(Validation):
     def __init__(self, dataset, scorer, primary_score=None, increase_better=False, discard_best=True, patience=None):
@@ -238,38 +236,38 @@
         score = super().step(node)
         if type(self.scorer)==dict:
             score_ = score[self.primary_score]
         else:
             score_ = score
         self.cv_history.append(score_)
 
-        # Save best model
+        # Save best network
         if isbetter(score_best=self.best_score, score=score_, increase_better=self.increase_better):
         # (not self.increase_better and score_<self.best_score) or (self.increase_better and score_>self.best_score):
-            log.info(f'Saved model: {name}')
-            torch.save(node.model.state_dict(), name)
-            if self.discard_best and self.best_model!=None:
-                os.remove(self.best_model)
+            log.info(f'Saved network: {name}')
+            torch.save(node.network.state_dict(), name)
+            if self.discard_best and self.best_network!=None:
+                os.remove(self.best_network)
 
             self.best_score = score_
-            self.best_model=name
+            self.best_network=name
 
             # Clear patience tracking
             self.cv_history.clear()
 
-        # patience_end == True when best model did not appear for self.patience times
+        # patience_end == True when best network did not appear for self.patience times
         patience_end = self.patience == len(self.cv_history)
         log.info(f'[EarlyStopping][patience: {len(self.cv_history)}/{self.cv_history.maxlen}]')
 
         return score, patience_end
 
     def reset(self):
         log.info('[EarlyStopping] Resetting...')
         self.cv_history.clear()
-        self.best_model = None
+        self.best_network = None
         if self.increase_better:
             self.best_score = -float('inf')
         else:
             self.best_score = float('inf')
 
 # %%
 class VDict(dict):
```

### Comparing `hideandseek-0.1.9/hideandseek.egg-info/PKG-INFO` & `hideandseek-0.2.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: hideandseek
-Version: 0.1.9
-Summary: library for deep learning and privacy preserving deep learning
-Home-page: https://github.com/jsyoo61/hideandseek
-Author: JaeSung Yoo
-Author-email: jsyoo61@unc.edu
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # hideandseek
 Highly modularized deep learning training library.
 
 Why use `hideandseek`?
 
 - Easy training & saving deep learning models along with other modules (ex: preprocessing modules) required in inference
 - Run multiple deep learning experiments in parallel on multiples GPUs (powered by [hydra](https://hydra.cc/docs/intro/), and python multiprocessing)
@@ -31,48 +15,46 @@
     import torch
     import torch.nn as nn
 
     # Generate data
     x = torch.rand(200,1)
     y = 5*x+2
 
-    model = nn.Linear(1,1)
+    network = nn.Linear(1,1)
     dataset = torch.utils.data.TensorDataset(x, y)
     criterion = nn.MSELoss()
     cfg = {
     'lr': 1e-2,
     'batch_size': 32,
     'epoch': 10 # optional
     }
 
     # Training configuration. All you need to train a neural network
     kwargs = {
-    'model':model,
+    'network':network,
     'dataset':dataset,
     'cfg_train':cfg,
     'criterion':criterion,
     'name': 'Test' # optional
     }
     trainer = hs.N.Node(**kwargs)
 
     device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-    trainer.model.to(device)
+    trainer.network.to(device)
 
     # Train for predefined number of epochs
     trainer.train() # Train for predefined number of epochs
     trainer.train(5) # Train for specified number of epochs
     trainer.train(epoch=5) # Same thing with trainer.train(5)
     trainer.train(step=500) # Train for specified number of updates
 
-    node.model.cpu()
+    trainer.network.cpu()
 
 and simply run multiple batch of experiments with a single line command such as:
 
     python train.py -m lr=1e-3,1e-2 batch_size=32,64 "random_seed=range(0,5)" \
     hydra/launcher=joblib hydra.launcher.n_jobs=8
     # Runs total of 2*2*5=40 batch of experiments, with 8 processes at a time. Experiment results are stored in hydra.sweep.dir which can be overridden.
 
 To do
 - [ ] Draw figures to explain hideandseek
 - [ ] GUI for generating experiment scripts when conducting variable sweeps
-
-
```

### Comparing `hideandseek-0.1.9/setup.py` & `hideandseek-0.2.0/setup.py`

 * *Files identical despite different names*

