# Comparing `tmp/codedepot_git_ai-0.0.7.tar.gz` & `tmp/codedepot_git_ai-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "codedepot_git_ai-0.0.7.tar", last modified: Wed Apr  3 09:51:35 2024, max compression
+gzip compressed data, was "codedepot_git_ai-0.0.8.tar", last modified: Wed Apr  3 10:05:45 2024, max compression
```

## Comparing `codedepot_git_ai-0.0.7.tar` & `codedepot_git_ai-0.0.8.tar`

### file list

```diff
@@ -1,39 +1,17 @@
--rw-r--r--   0        0        0     1068 2024-04-02 10:19:19.979567 codedepot_git_ai-0.0.7/LICENSE
--rw-r--r--   0        0        0     1432 2023-11-27 16:02:28.644959 codedepot_git_ai-0.0.7/README.md
--rw-r--r--   0        0        0        0 2023-11-27 16:02:28.645320 codedepot_git_ai-0.0.7/git_ai/__init__.py
--rw-r--r--   0        0        0      220 2023-11-27 16:02:28.645606 codedepot_git_ai-0.0.7/git_ai/cmd/__init__.py
--rw-r--r--   0        0        0       77 2023-11-27 16:02:28.645811 codedepot_git_ai-0.0.7/git_ai/cmd/ai_repo/__init__.py
--rw-r--r--   0        0        0    12757 2024-04-02 07:40:32.935067 codedepot_git_ai-0.0.7/git_ai/cmd/ai_repo/ai_repo.py
--rw-r--r--   0        0        0     2093 2023-11-27 16:02:28.646238 codedepot_git_ai-0.0.7/git_ai/cmd/ai_repo/ai_repo_config.py
--rw-r--r--   0        0        0     5513 2024-04-02 10:13:46.122413 codedepot_git_ai-0.0.7/git_ai/cmd/ai_repo/ai_repo_log.py
--rw-r--r--   0        0        0     1292 2024-04-02 07:32:17.319363 codedepot_git_ai-0.0.7/git_ai/cmd/constants.py
--rw-r--r--   0        0        0     6257 2023-11-27 16:02:28.646779 codedepot_git_ai-0.0.7/git_ai/cmd/diff.py
--rw-r--r--   0        0        0       64 2023-11-27 16:02:28.646875 codedepot_git_ai-0.0.7/git_ai/cmd/error.py
--rw-r--r--   0        0        0      668 2024-04-02 10:11:50.317827 codedepot_git_ai-0.0.7/git_ai/cmd/init.py
--rw-r--r--   0        0        0      370 2024-04-02 10:14:57.943339 codedepot_git_ai-0.0.7/git_ai/cmd/input_repo.py
--rw-r--r--   0        0        0      310 2023-11-27 16:02:28.647348 codedepot_git_ai-0.0.7/git_ai/cmd/log.py
--rw-r--r--   0        0        0      147 2023-11-27 16:02:28.647533 codedepot_git_ai-0.0.7/git_ai/cmd/merge_exp.py
--rw-r--r--   0        0        0       45 2023-11-27 16:02:28.647580 codedepot_git_ai-0.0.7/git_ai/cmd/runner.py
--rw-r--r--   0        0        0       80 2023-11-27 16:02:28.647785 codedepot_git_ai-0.0.7/git_ai/errors/__init__.py
--rw-r--r--   0        0        0     2663 2024-04-02 07:54:03.292350 codedepot_git_ai-0.0.7/git_ai/errors/errors.py
--rw-r--r--   0        0        0        0 2023-11-27 16:02:28.648024 codedepot_git_ai-0.0.7/git_ai/metrics/__init__.py
--rw-r--r--   0        0        0     5677 2024-04-03 09:34:11.343503 codedepot_git_ai-0.0.7/git_ai/metrics/experiment.py
--rw-r--r--   0        0        0    12294 2024-04-02 08:10:43.723916 codedepot_git_ai-0.0.7/git_ai/metrics/writer.py
--rw-r--r--   0        0        0       73 2023-11-27 16:02:28.648608 codedepot_git_ai-0.0.7/git_ai/pygitutils/__init__.py
--rw-r--r--   0        0        0     1094 2023-11-27 16:02:28.648784 codedepot_git_ai-0.0.7/git_ai/pygitutils/pygitutils.py
--rw-r--r--   0        0        0       29 2023-11-27 16:02:28.648937 codedepot_git_ai-0.0.7/git_ai/utils/__init__.py
--rw-r--r--   0        0        0      343 2023-11-27 16:02:28.649108 codedepot_git_ai-0.0.7/git_ai/utils/utils.py
--rw-r--r--   0        0        0      655 2024-04-03 09:51:35.871762 codedepot_git_ai-0.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-27 16:02:28.649767 codedepot_git_ai-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0    11983 2024-04-03 08:08:59.801691 codedepot_git_ai-0.0.7/tests/test_ai_repo.py
--rw-r--r--   0        0        0     2404 2023-11-27 16:02:28.650336 codedepot_git_ai-0.0.7/tests/topologies/cnn.1
--rw-r--r--   0        0        0     2255 2023-11-27 16:02:28.650546 codedepot_git_ai-0.0.7/tests/topologies/cnn.2
--rw-r--r--   0        0        0     2411 2023-11-27 16:02:28.650671 codedepot_git_ai-0.0.7/tests/topologies/cnn.3
--rw-r--r--   0        0        0     2559 2023-11-27 16:02:28.650783 codedepot_git_ai-0.0.7/tests/topologies/cnn.4
--rw-r--r--   0        0        0        0 2023-11-27 16:02:28.650821 codedepot_git_ai-0.0.7/tests/utils/__init__.py
--rw-r--r--   0        0        0     1538 2024-04-02 07:32:17.323195 codedepot_git_ai-0.0.7/tests/utils/ai_repo_read.py
--rw-r--r--   0        0        0    14073 2024-04-03 07:25:22.532230 codedepot_git_ai-0.0.7/tests/utils/data_gen.py
--rw-r--r--   0        0        0     1788 2024-04-03 07:04:45.049450 codedepot_git_ai-0.0.7/tests/utils/interuptable_test.py
--rw-r--r--   0        0        0     2473 2024-04-03 06:48:21.347153 codedepot_git_ai-0.0.7/tests/utils/setup_repo.py
--rw-r--r--   0        0        0      133 2023-11-27 16:02:28.651657 codedepot_git_ai-0.0.7/tests/utils/testutils.py
--rw-r--r--   0        0        0     1990 1970-01-01 00:00:00.000000 codedepot_git_ai-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-02 10:19:19.979567 codedepot_git_ai-0.0.8/LICENSE
+-rw-r--r--   0        0        0     1432 2023-11-27 16:02:28.644959 codedepot_git_ai-0.0.8/README.md
+-rw-r--r--   0        0        0      707 2024-04-03 10:05:45.975027 codedepot_git_ai-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-03 10:02:20.380987 codedepot_git_ai-0.0.8/src/git_ai/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-27 16:02:28.649767 codedepot_git_ai-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0    11983 2024-04-03 08:08:59.801691 codedepot_git_ai-0.0.8/tests/test_ai_repo.py
+-rw-r--r--   0        0        0     2404 2023-11-27 16:02:28.650336 codedepot_git_ai-0.0.8/tests/topologies/cnn.1
+-rw-r--r--   0        0        0     2255 2023-11-27 16:02:28.650546 codedepot_git_ai-0.0.8/tests/topologies/cnn.2
+-rw-r--r--   0        0        0     2411 2023-11-27 16:02:28.650671 codedepot_git_ai-0.0.8/tests/topologies/cnn.3
+-rw-r--r--   0        0        0     2559 2023-11-27 16:02:28.650783 codedepot_git_ai-0.0.8/tests/topologies/cnn.4
+-rw-r--r--   0        0        0        0 2023-11-27 16:02:28.650821 codedepot_git_ai-0.0.8/tests/utils/__init__.py
+-rw-r--r--   0        0        0     1538 2024-04-02 07:32:17.323195 codedepot_git_ai-0.0.8/tests/utils/ai_repo_read.py
+-rw-r--r--   0        0        0    14073 2024-04-03 07:25:22.532230 codedepot_git_ai-0.0.8/tests/utils/data_gen.py
+-rw-r--r--   0        0        0     1788 2024-04-03 07:04:45.049450 codedepot_git_ai-0.0.8/tests/utils/interuptable_test.py
+-rw-r--r--   0        0        0     2473 2024-04-03 06:48:21.347153 codedepot_git_ai-0.0.8/tests/utils/setup_repo.py
+-rw-r--r--   0        0        0      133 2023-11-27 16:02:28.651657 codedepot_git_ai-0.0.8/tests/utils/testutils.py
+-rw-r--r--   0        0        0     2003 1970-01-01 00:00:00.000000 codedepot_git_ai-0.0.8/PKG-INFO
```

### Comparing `codedepot_git_ai-0.0.7/LICENSE` & `codedepot_git_ai-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.7/README.md` & `codedepot_git_ai-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.7/git_ai/metrics/writer.py` & `codedepot_git_ai-0.0.8/tests/utils/data_gen.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,383 +1,382 @@
-import json
-import os
-import time
-from enum import Enum
-from typing import IO, BinaryIO, Union
-from threading import Event, Thread
-import queue
-
-import torch
-from git_ai.cmd.ai_repo import AIRepo
-from git_ai.cmd.constants import AIRepoConstants
-from torch.utils.tensorboard import SummaryWriter
-
-from git_ai.errors.errors import MetricError
-
-
-class DataTypeEnum(Enum):
-    FLOAT = 0
-    STRING = 1
-    INT = 2
-    BOOLEAN = 3
-
-    @classmethod
-    def from_string(cls, str):
-        if str == 'FLOAT':
-            return cls.FLOAT
-        elif str == 'STRING':
-            return cls.STRING
-        elif str == 'INT':
-            return cls.INT
-        elif str == 'BOOLEAN':
-            return cls.BOOLEAN
+import random
+from typing import Iterable, Iterator, Optional, Type, Union
+from typing_extensions import Self
+from dataclasses import dataclass
+import math
+from tests.utils.testutils import sample_array
+
+
+@dataclass(frozen=True)
+class Metric:
+    label: str
+    unit: str
+    metric_type: str
+    value: Union[str, int, float, bool]
+
+    def __eq__(self, x):
+        label_equals = (self.label == x.label)
+        if self.metric_type == 'FLOAT':
+            value_equals = math.isclose(self.value, x.value, rel_tol=.01)
+        elif self.metric_type == 'INT':
+            value_equals = self.value == x.value
+        elif self.metric_type == 'STRING':
+            value_equals = self.value == x.value
+        elif self.metric_type == 'BOOLEAN':
+            value_equals = self.value == x.value
         else:
-            raise MetricError.unknown_data_type_enum(str)
+            raise Exception("metric type %s unknown" % self.metric_type)
+        return label_equals == value_equals
 
-    @classmethod
-    def to_string(cls, v):
-        if v == DataTypeEnum.FLOAT:
-            return 'FLOAT'
-        elif v == DataTypeEnum.STRING:
-            return 'STRING'
-        elif v == DataTypeEnum.INT:
-            return 'INT'
-        elif v == DataTypeEnum.BOOLEAN:
-            return 'BOOLEAN'
+    def format_value(self) -> str:
+        if self.metric_type == 'FLOAT':
+            return '%.03f' % self.value
+        elif self.metric_type == 'INT':
+            return "%i" % self.value
+        elif self.metric_type == 'STRING':
+            return "%s" % self.value
+        elif self.metric_type == 'BOOLEAN':
+            return str(self.value)
         else:
-            raise MetricError.unknown_data_type_enum(str(v))
+            raise Exception("metric type %s unknown" % self.metric_type)
 
+    @ staticmethod
+    def parse_value(v: str, metric_type: str) -> Union[str, int, float, bool]:
+        if metric_type == 'FLOAT':
+            return float(v)
+        elif metric_type == 'INT':
+            return int(v)
+        elif metric_type == 'STRING':
+            return v
+        elif metric_type == 'BOOLEAN':
+            return v in ['true', 'True']
+        else:
+            raise Exception("metric type %s unknown" % metric_type)
+
+    @ classmethod
+    def from_json(cls: Type[Self], j: dict) -> Self:
+        unit = j['unit'] if 'unit' in j else ''
+        return cls(j['label'], unit, j['dataType'],
+                   Metric.parse_value(j['value'], j['dataType']))
+
+    def __str__(self) -> str:
+        if self.unit:
+            return "%s: %s %s" % (self.label, self.format_value(), self.unit)
+        else:
+            return "%s: %s" % (self.label, self.format_value())
+
+    def __repr__(self) -> str:
+        return self.__str__()
+
+    @ classmethod
+    def sample_metric(cls: Type[Self], label: str, unit: str, metric_type: str) -> Self:
+        """samples a single metric
+
+        Args:
+            cls (Type[Self]): class object
+            label (str): label of the metric sampled
+            metric_type (str): type of the metric sampled
 
-class AsynchFileWriter(Thread):
+        Returns:
+            Self: a metric with a value sampled according to the label
+        """
+        return Metric(label, unit, metric_type, Metric.__sample_value(metric_type))
 
-    def __init__(self) -> None:
-        super().__init__()
-        self.stop_event = Event()
-        self.flush_event = Event()
-        self.flush_done_event = Event()
-        self.q = queue.Queue()
-        self.writer_queue = []
-        self.pending_items = {}
-        self.start()
-
-    def flush(self):
-        self.flush_event.set()
-        while not self.stop_event.is_set() and not self.flush_done_event.wait(0.1):
-            pass
-        if self.flush_done_event.is_set():
-            self.flush_done_event.clear()
-
-    def enqueue_write(self, filename, contents):
-        self.q.put((filename, contents.to_dict()), block=True)
-
-    def dequeue_writes(self) -> bool:
-        """Dequees an items from the process queue and puts it in an internal queue.
-        Keeps only the most recent item for each file. Pushes the file to the head
-        of the queue if it is already in the queue.
+    @ staticmethod
+    def __sample_value(metric_type: str) -> Union[str, int, float, bool]:
+        """samples a single value
+
+        Args:
+            metric_type (str): type of the metric to be sampled
 
         Returns:
-            bool: True if is successful false if it fails
+            Union[str, int, float, bool]: value sampled
         """
-        try:
-            while self.q.qsize() > 0:
-                filename, item = self.q.get()
-                # If the file is already in the queue, put it in the front
-                # If it is not, just append it
-                if filename in self.writer_queue:
-                    self.writer_queue.remove(filename)
-
-                self.writer_queue.append(filename)
-                self.pending_items[filename] = item
-        except FileNotFoundError:
-            return False
-        return True
-
-    def __worker_loop(self):
-        process_running = self.dequeue_writes()
-        if process_running:
-            for filename in self.writer_queue:
-                try:
-                    with open(filename, 'w') as f:
-                        json.dump(self.pending_items[filename], f)
-                        f.flush()
-                except Exception as e:
-                    print("Error writing to file %s: %s" % (filename, str(e)))
-                    process_running = False
-                    break
-            self.writer_queue = []
-        return process_running
-
-    def run(self):
-        running = True
-        while not self.stop_event.is_set() and running:
-            running = self.__worker_loop()
-            if self.flush_event.is_set():
-                # Flush the queue
-                running = self.__worker_loop()
-                self.flush_event.clear()
-                self.flush_done_event.set()
-            time.sleep(0.1)
-        # This is flush
-        self.__worker_loop()
-        # Something went wrong
-        if not running:
-            print("File writer failed to write, won't be able to write further.")
-            self.stop_event.set()
-
-    def close(self):
-        self.flush()
-        self.stop_event.set()
-        self.join()
-
-
-class JsonObj(object):
-    def __init__(self):
-        self.run = True
-
-    def log(self, string):
-        print("WORKER %s - %s" % (self.__class__.__name__, string))
-
-    def to_dict(self):
-        raise NotImplementedError("Not implemented!")
-
-    @staticmethod
-    def get_data_type(value):
-        if isinstance(value, str):
-            return DataTypeEnum.STRING
-        elif isinstance(value, float):
-            return DataTypeEnum.FLOAT
-        elif isinstance(value, bool):
-            return DataTypeEnum.BOOLEAN
-        elif isinstance(value, int):
-            return DataTypeEnum.INT
+        if metric_type == 'FLOAT':
+            value = (random.random()*10)
+        elif metric_type == 'INT':
+            value = int(random.random()*1000)
+        elif metric_type == 'STRING':
+            value = random.choice(['ADAM', 'SGD', 'POWER_SGD'])
+        elif metric_type == 'BOOLEAN':
+            value = random.choice([True, False])
         else:
-            raise NotImplementedError("Cannot recoginze type of %s" %
-                                      str(value))
+            raise Exception("metric type %s unknown" % metric_type)
+        return value
+
 
-    @staticmethod
-    def format_value(value, data_type):
-        if data_type == DataTypeEnum.STRING:
-            return value
-        elif data_type == DataTypeEnum.FLOAT:
-            return "%.03f" % value
-        elif data_type == DataTypeEnum.BOOLEAN:
-            return "true" if value else "false"
-        elif data_type == DataTypeEnum.INT:
-            return "%d" % value
-        raise NotImplementedError("Cannot recoginize type %s" % str(data_type))
-
-    @staticmethod
-    def read_value(str, data_type):
-        if data_type == DataTypeEnum.STRING:
-            return str
-        elif data_type == DataTypeEnum.FLOAT:
-            return float(str)
-        elif data_type == DataTypeEnum.BOOLEAN:
-            return True if str == "true" else False
-        elif data_type == DataTypeEnum.INT:
-            return int(str)
-        raise NotImplementedError("Cannot recoginize type %s" % str(data_type))
-
-    @classmethod
-    def from_json(self):
-        raise NotImplementedError("Not implemented!")
-
-    @classmethod
-    def from_file(cls, filename):
-        if os.path.isfile(filename):
-            with open(filename, 'r') as f:
-                return cls.from_json(json.load(f))
+@ dataclass(frozen=True)
+class Plot:
+    label: str
+    values: list[float]
+
+    def __eq__(self, x):
+        return (self.label == x.label and
+                all([math.isclose(this, that, rel_tol=.1) for (this, that) in zip(self.values, x.values)]) and
+                len(self.values) == len(x.values))
+
+    def format_values(self, vs):
+        return ",".join(["%.3f" % v for v in vs])
+
+    @ classmethod
+    def from_json(cls: Type[Self], header: dict, values: dict[str, list[str]]) -> Self:
+        return cls(header['title'], [float(v) for v in values['values']])
+
+    def __str__(self):
+        if len(self.values) <= 6:
+            values_str = self.format_values(self.values)
         else:
-            return None
+            values_str = (
+                self.format_values(self.values[:3]) + " ... " +
+                self.format_values(self.values[-3:])
+            )
+        return "%s: [%s]" % (self.label, values_str)
+
+    def __repr__(self) -> str:
+        return self.__str__()
+
+    def __iter__(self):
+        for v in self.values:
+            yield (self.label, v)
+
+    @ classmethod
+    def sample_plot(cls: Type[Self], total_iterations: int, label: str, plot_type: str,
+                    scale: float) -> Self:
+        """samples a plot object
+
+        Args:
+            cls (Type[Self]): class object
+            total_iterations (int): number of iterations in the plot
+            label (str): label of the plot
+            plot_type (str): type of the plot
+            scale (float): scale of the plot for varying it during experiments
 
+        Returns:
+            Self: plot sampled
+        """
+        values = [
+            Plot.__sample_value(total_iterations, it, plot_type, scale)
+            for it in range(total_iterations)
+        ]
+        return cls(label, values)
+
+    @ staticmethod
+    def __sample_value(total_iterations: int, it: int, plot_type: str,
+                       scale: float) -> float:
+        """samples all values for a plot
+
+        Args:
+            total_iterations (int): number of iterations in the plot
+            it (int): current interation in the plot
+            scale (float): scale of the plot for varying it during experiments
 
-class Metric(JsonObj):
-    def __init__(self, label, value, unit=None, data_type=None):
-        super().__init__()
-        self.label = label
-        self.value = value
-        self.unit = unit
-        if not data_type:
-            self.data_type = self.get_data_type(value)
+        Returns:
+            float: value sampled according to tye plot type
+        """
+        if plot_type == 'log':
+            sampled_value = math.log((it+1)*0.01)*scale
+        elif plot_type == 'exponential':
+            sampled_value = math.exp((it+1)*0.01)*scale
+        elif plot_type == 'inverse_exponential':
+            sampled_value = 1/math.exp((it+1)*0.01)*scale
+        elif plot_type == 'linear_growth':
+            sampled_value = it*scale
+        elif plot_type == 'linear_decrease':
+            sampled_value = (total_iterations-it)*scale
         else:
-            self.data_type = data_type
+            raise Exception('plot type unknown')
 
-    def to_dict(self):
-        dict = {
-            'label': self.label,
-            'value': self.format_value(self.value, self.data_type),
-            'dataType': DataTypeEnum.to_string(self.data_type)
-        }
+        return sampled_value
 
-        if self.unit:
-            dict['unit'] = self.unit
 
-        return dict
+class DataConstants:
+    METRIC_LABELS = [
+        ('f1_score', '', 'FLOAT'), ('training_loss', '', 'FLOAT'),
+        ('test_loss', '', 'FLOAT'), ('hparams/lr', '', 'FLOAT'),
+        ('hparams/batch_size', '', 'FLOAT'), ('hparams/alpha', '', 'FLOAT'),
+        ('hparms/beta', '', 'FLOAT'), ('mean_error', '%', 'FLOAT'),
+        ('mean_squared_error', '%', 'FLOAT'), ('test_error', '%', 'FLOAT'),
+        ('training_error', '%', 'FLOAT'), ('test_accuracy', '%', 'FLOAT'),
+        ('hparams/dropout', '%', 'FLOAT'), ('hparams/optimizer', '', 'STRING'),
+        ('hparams/shuffle', '', 'BOOLEAN'), ('hparams/epochs', '', 'INT'),
+        ('mean_absolute_error', '', 'FLOAT'), ('mrr', '', 'FLOAT'),
+        ('dcg', '', 'FLOAT'), ('ndcg', '', 'FLOAT'),
+        ('perplexity', '', 'FLOAT'), ('bleu_score', 'score', 'FLOAT'),
+        ('psnr', '', 'FLOAT'), ('ssim', '', 'FLOAT'), ('iou', '', 'FLOAT'),
+    ]
+
+    PLOT_TYPES = ['log', 'exponential', 'inverse_exponential', 'linear_growth',
+                  'linear_decrease']
+
+    PLOT_LABELS = [
+        ('test_accuracy', 'iteration',  'FLOAT'),
+        ('test_error', 'iteration', 'FLOAT'),
+        ('test_loss', 'iteration', 'FLOAT'),
+        ('training_accuracy', 'iteration', 'FLOAT'),
+        ('training_error', 'iteration', 'FLOAT'),
+        ('training_loss', 'iteration', 'FLOAT'),
+        ('l1_weight_value', 'iteration', 'FLOAT'),
+        ('f1_score', 'iteration', 'FLOAT'),
+        ('roc', 'iteration', 'FLOAT'),
+        ('mean_absolute_error', 'iteration', 'FLOAT'),
+        ('inception_score', 'iteration', 'FLOAT')
+    ]
+
+    HEADER = ['id', 'name', 'description', 'forkCount', 'watcherCount',
+              'issueCount', 'license', 'pullRequestCount', 'createdAt',
+              'updatedAt', 'isFork', 'isPrivate', 'isMirror', 'isArchived',
+              'ownerId', 'size', 'isAIRepo', 'dataTypeStr',
+              'aiRepositoryTypeStr', 'fileCount', 'layers']
+
+    DATES = ["2017-07-18T21:41:10Z", "2021-10-20T07:09:06Z",
+             "2017-03-22T19:15:24Z", "2021-10-17T20:39:19Z",
+             "2016-06-07T16:56:31Z", "2021-10-20T13:19:01Z"]
+
+
+class ExperimentDataGen:
+    def __sample_metrics(self, metric_spec: list[str]) -> list[Metric]:
+        """samples metrics based on a list of labels provided by the user
+
+        Args:
+            metric_spec (list[str]): list of labels
 
-    @classmethod
-    def from_json(cls, json):
-        unit = None if ('unit' not in json) else json['unit']
-        data_type = DataTypeEnum.from_string(json['dataType'])
-        return cls(json['label'], cls.read_value(json['value'], data_type),
-                   unit, data_type)
-
-
-class Hparams(JsonObj):
-    def __init__(self):
-        super().__init__()
-        self.values = []
-
-    def add_metric(self, metric):
-        self.values.append(metric)
-
-    def to_dict(self):
-        return [v.to_dict() for v in self.values]
-
-    @classmethod
-    def from_json(cls, json_f):
-        hparams = cls()
-        for v in json_f:
-            hparams.add_metric(Metric.from_json(v))
-        return hparams
-
-
-class ScalarHeader(JsonObj):
-    def __init__(self, title, data_type, x_title=None, unit=None):
-        super().__init__()
-        self.title = title
-        self.x_title = x_title
-        self.unit = unit
-        self.data_type = data_type
-
-    def to_dict(self):
-        dict = {
-            'title': self.title,
-            'x_title': self.x_title,
-            'dataType': DataTypeEnum.to_string(self.data_type)
+        Returns:
+            list[Metric]: a list of values with sampled values
+        """
+        metric_labels = {
+            m: Metric.sample_metric(m, u, t)
+            for (m, u, t) in DataConstants.METRIC_LABELS
+            if m in metric_spec
         }
+        # get labels in the same order as specified
+        return [
+            metric_labels[k] for k in metric_spec
+        ]
 
-        if self.unit:
-            dict['unit'] = self.unit
+    def __sample_plots(self, plot_spec: list[str]) -> list[Plot]:
+        """samples a list of plots based on labels provided by the user
 
-        return dict
+        Args:
+            plot_spec (list[str]): list of plot labels
 
-    @classmethod
-    def from_json(cls, json):
-        unit = None if ('unit' not in json) else json['unit']
-        x_title = None if ('x_title' not in json) else json['x_title']
-        data_type = DataTypeEnum.from_string(json['dataType'])
-        return cls(json['title'], data_type=data_type, unit=unit,
-                   x_title=x_title)
-
-
-class Scalar(JsonObj):
-    def __init__(self, values, data_type):
-        super().__init__()
-        self.values = values
-        self.data_type = data_type
-
-    def add_value(self, value):
-        self.values.append(value)
-
-    def to_dict(self):
-        return {
-            'values': [self.format_value(v, self.data_type)
-                       for v in self.values],
-            'dataType': DataTypeEnum.to_string(self.data_type)
+        Returns:
+            list[Plot]: plots with samples values
+        """
+        plot_labels = {
+            p: Plot.sample_plot(self.epoch_count, p, random.choice(
+                DataConstants.PLOT_TYPES), random.random()*.2+.8)
+            for (p, _, _) in DataConstants.PLOT_LABELS
+            if p in plot_spec
         }
 
-    @classmethod
-    def from_json(cls, json):
-        data_type = DataTypeEnum.from_string(json['dataType'])
-        values = [cls.read_value(v, data_type) for v in json['values']]
-        return cls(values, data_type)
-
-
-class GitTensorboardSummaryWriter(SummaryWriter, AIRepoConstants):
-
-    def __init__(self, repo: AIRepo, **kwargs):
-        self.workdir = repo.workdir
-        self._tb_folder = os.path.join(self.workdir, self.GIT_AI_ROOT,
-                                       self.TENSORBOARD_FOLDER)
-
-        super().__init__(log_dir=self._tb_folder, **kwargs)
-        self.hparams = None
-        self.scalars = {}
-        self.scalar_headers = {}
-        self.async_writer = AsynchFileWriter()
-
-    def add_scalar(self, tag, scalar_value, unit=None,
-                   data_type_=None, x_title=None,
-                   global_step=None, walltime=None,
-                   new_style=False, double_precision=False):
-        super().add_scalar(tag, scalar_value, global_step, walltime, new_style,
-                           double_precision)
-
-        data_type = (data_type_ if data_type_
-                     else JsonObj.get_data_type(scalar_value))
-
-        scalar_filename = self.metric_filename(self.workdir, tag)
-        scalar_header_filename = self.metric_filename(
-            self.workdir, tag) + '_header'
-        if scalar_header_filename not in self.scalar_headers:
-            scalar_header = ScalarHeader.from_file(scalar_header_filename)
-            if not scalar_header:
-                scalar_header = ScalarHeader(
-                    title=tag, x_title=x_title, unit=unit, data_type=data_type)
-            self.scalar_headers[scalar_header_filename] = scalar_header
-        else:
-            scalar_header = self.scalar_headers[scalar_header_filename]
+        return [plot_labels[p] for p in plot_spec]
 
-        self.async_writer.enqueue_write(scalar_header_filename, scalar_header)
+    def __init__(self, epoch_count: int, before_metrics_spec: list[str],
+                 after_metrics_spec: list[str], plot_spec: list[str]) -> None:
+        """generates an entire experiment
+
+        Args:
+            epoch_count (int): number of epochs
+            before_metrics_spec (list[str]): metrics to be added before te experiments runs
+            after_metrics_spec (list[str]): metrics to be added after te experiments runs
+            plot_spec (list[str]): list of plot labels
+        """
+        self.name = None
+        self.epoch_count = epoch_count
+        self.before_metrics = self.__sample_metrics(before_metrics_spec)
+        self.after_metrics = self.__sample_metrics(after_metrics_spec)
+        self.plots = self.__sample_plots(plot_spec)
+
+    def get_before_metrics(self) -> list[Metric]:
+        return self.before_metrics
+
+    def get_after_metrics(self) -> list[Metric]:
+        return self.after_metrics
 
-        if scalar_filename not in self.scalars:
-            scalar = Scalar.from_file(scalar_filename)
-            if not scalar:
-                scalar = Scalar(values=[], data_type=data_type)
-            self.scalars[scalar_filename] = scalar
-        else:
-            scalar = self.scalars[scalar_filename]
+    def get_plots(self) -> list[Plot]:
+        return self.plots
 
-        scalar.add_value(scalar_value)
-        self.async_writer.enqueue_write(scalar_filename, scalar)
+    def epochs_generator(self) -> Iterator[list[tuple[str, float]]]:
+        """iterator for epochs generation
 
-    def add_hparams(self, hparam_dict, metric_dict,
-                    hparam_unit_dict={}, metric_unit_dict={},
-                    hparam_domain_discrete=None, run_name=None):
-
-        all_data = {**hparam_dict, **metric_dict}
-        super().add_hparams(all_data, {}, hparam_domain_discrete,
-                            run_name)
-
-        if not self.hparams:
-            hparams_filename = self.hparam_filename(self.workdir)
-            hparams = Hparams.from_file(hparams_filename)
-            if not hparams:
-                hparams = Hparams()
-        else:
-            hparams = self.hparams
+        Yields:
+            Iterator[list[tuple[str, float]]]: an iterator that yields with a list of (label, value) for each epoch
+        """
+        for ps in zip(*self.plots):
+            yield list(ps)
 
-        for k, v in hparam_dict.items():
-            unit = hparam_unit_dict[k] if k in hparam_unit_dict else ""
-            hparams.add_metric(Metric(k, v, unit=unit))
-        for k, v in metric_dict.items():
-            unit = metric_unit_dict[k] if k in metric_unit_dict else ""
-            hparams.add_metric(Metric(k, v, unit=unit))
-
-        self.async_writer.enqueue_write(hparams_filename, hparams)
-
-    def save_artifact(self, obj,
-                      f: Union[str, os.PathLike, BinaryIO, IO[bytes]]):
-        torch.save(obj, self.ARTIFACT_PATH / str(f))
-
-    def add_topology(self, topology):
-        with open(self.TOPOLOGY_PATH, 'w') as f:
-            f.write(topology)
-
-    def flush(self):
-        self.async_writer.flush()
-        super().flush()
-
-    def close(self):
-        self.flush()
-        self.async_writer.close()
-        super().close()
+    def __str__(self) -> str:
+        def indent_v(v) -> str:
+            return "  " + str(v)
+        return ("\n\nExperiment %s: \nBefore metrics:\n" % self.name +
+                "\n".join(map(indent_v, self.before_metrics)) + "\nAfter metrics:\n" +
+                "\n".join(map(indent_v, self.after_metrics)) + "\nPlots:\n" +
+                "\n".join(map(indent_v, self.plots))
+                )
+
+    def __repr__(self) -> str:
+        return self.__str__()
+
+    def match_data(self, metrics: dict[str, Metric], plots: dict[str, Plot]) -> bool:
+        all_metrics = self.before_metrics + self.after_metrics
+        matches = True
+        labels = set([m.label for m in all_metrics])
+        plot_labels = set([p.label for p in self.plots])
+
+        for m in all_metrics:
+            assert m.label in metrics
+            assert m == metrics[m.label]
+
+        for m in metrics.keys():
+            assert m in labels
+
+        for p in self.plots:
+            assert p.label in plots
+            assert p == plots[p.label]
+
+        for p in plots.keys():
+            assert p in plot_labels
+
+
+class RepositoryDataGen:
+    def __init__(self, experiment_count: int,
+                 experiment_epochs: int,
+                 mandatory_before_metrics: list[str],
+                 mandatory_after_metrics: list[str],
+                 mandatory_plots: list[str],
+                 optional_before_metrics: list[str],
+                 optional_after_metrics: list[str],
+                 optional_plots: list[str],
+                 seed=42) -> None:
+        random.seed(seed)
+        self.experiments = [
+            ExperimentDataGen(
+                epoch_count=experiment_epochs,
+                before_metrics_spec=(
+                    mandatory_before_metrics + sample_array(optional_before_metrics)),
+                after_metrics_spec=(
+                    mandatory_after_metrics + sample_array(optional_after_metrics)),
+                plot_spec=mandatory_plots + sample_array(optional_plots))
+            for it in range(experiment_count)
+        ]
+
+    def __iter__(self):
+        yield from self.experiments
+
+    def match_data(self, exp: str, metrics: dict[str, Metric], plots: dict[str, Plot]) -> None:
+        exp_dict = {e.name: e for e in self.experiments}
+        assert (exp in exp_dict)
+        exp_dict[exp].match_data(metrics, plots)
+
+    @ classmethod
+    def default(cls, experiment_count=5, experiment_epochs=10) -> Self:
+        return cls(
+            experiment_count=experiment_count,
+            experiment_epochs=experiment_epochs,
+            mandatory_before_metrics=[
+                'f1_score', 'hparams/epochs', 'hparams/optimizer', 'hparams/shuffle'],
+            mandatory_after_metrics=['dcg', 'psnr', 'test_loss'],
+            mandatory_plots=['test_accuracy', 'test_error'],
+            optional_before_metrics=['hparms/beta', 'hparams/dropout'],
+            optional_after_metrics=['ssim', 'iou', 'mrr'],
+            optional_plots=['training_error', 'training_loss', 'f1_score']
+        )
```

### Comparing `codedepot_git_ai-0.0.7/pyproject.toml` & `codedepot_git_ai-0.0.8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "codedepot-git-ai"
-version = "0.0.7"
+version = "0.0.8"
 description = "Dataset and model support for git"
 readme = "README.md"
 authors = [
     { name = "CodeDepot", email = "contact@codedepot.ai" },
 ]
 classifiers = [
     "License :: OSI Approved :: MIT License",
@@ -20,12 +20,16 @@
 requires-python = ">=3.10"
 dependencies = [
     "pygit2",
     "tensorboard",
     "torch",
 ]
 
+[project.license]
+text = "MIT"
+
 [project.urls]
 Homepage = "https://github.com/codedepotai/git-ai"
 Issues = "https://github.com/codedepotai/git-ai/issues"
 
 [tool.pdm]
+distribution = true
```

### Comparing `codedepot_git_ai-0.0.7/tests/test_ai_repo.py` & `codedepot_git_ai-0.0.8/tests/test_ai_repo.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.7/tests/topologies/cnn.1` & `codedepot_git_ai-0.0.8/tests/topologies/cnn.1`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.7/tests/topologies/cnn.2` & `codedepot_git_ai-0.0.8/tests/topologies/cnn.2`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.7/tests/topologies/cnn.3` & `codedepot_git_ai-0.0.8/tests/topologies/cnn.3`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.7/tests/topologies/cnn.4` & `codedepot_git_ai-0.0.8/tests/topologies/cnn.4`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.7/tests/utils/ai_repo_read.py` & `codedepot_git_ai-0.0.8/tests/utils/ai_repo_read.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.7/tests/utils/interuptable_test.py` & `codedepot_git_ai-0.0.8/tests/utils/interuptable_test.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.7/tests/utils/setup_repo.py` & `codedepot_git_ai-0.0.8/tests/utils/setup_repo.py`

 * *Files identical despite different names*

### Comparing `codedepot_git_ai-0.0.7/PKG-INFO` & `codedepot_git_ai-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: codedepot-git-ai
-Version: 0.0.7
+Version: 0.0.8
 Summary: Dataset and model support for git
 Author-Email: CodeDepot <contact@codedepot.ai>
+License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Project-URL: Homepage, https://github.com/codedepotai/git-ai
 Project-URL: Issues, https://github.com/codedepotai/git-ai/issues
 Requires-Python: >=3.10
 Requires-Dist: pygit2
```

