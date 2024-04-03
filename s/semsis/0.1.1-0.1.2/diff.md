# Comparing `tmp/semsis-0.1.1.tar.gz` & `tmp/semsis-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semsis-0.1.1.tar", max compression
+gzip compressed data, was "semsis-0.1.2.tar", max compression
```

## Comparing `semsis-0.1.1.tar` & `semsis-0.1.2.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0     1131 2023-09-28 10:07:17.382286 semsis-0.1.1/LICENSE
--rw-r--r--   0        0        0     3815 2023-10-25 23:11:29.445869 semsis-0.1.1/README.rst
--rw-r--r--   0        0        0      681 2023-10-31 09:50:47.581773 semsis-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      377 2023-09-28 10:07:17.382286 semsis-0.1.1/semsis/__init__.py
--rw-r--r--   0        0        0     2842 2023-10-25 23:11:29.445869 semsis-0.1.1/semsis/cli/README.rst
--rw-r--r--   0        0        0     6296 2023-10-25 23:11:29.445869 semsis-0.1.1/semsis/cli/build_retriever.py
--rw-r--r--   0        0        0     6120 2023-10-25 23:11:29.445869 semsis-0.1.1/semsis/cli/query_interactive.py
--rw-r--r--   0        0        0     5698 2023-10-11 07:07:17.875658 semsis-0.1.1/semsis/cli/store_kv.py
--rw-r--r--   0        0        0      247 2023-09-25 04:47:52.719653 semsis-0.1.1/semsis/encoder/__init__.py
--rw-r--r--   0        0        0     5132 2023-10-04 10:47:57.543925 semsis-0.1.1/semsis/encoder/sentence_encoder.py
--rw-r--r--   0        0        0     5225 2023-09-28 10:07:17.382286 semsis-0.1.1/semsis/encoder/sentence_encoder_test.py
--rw-r--r--   0        0        0     2004 2023-09-28 10:07:17.382286 semsis-0.1.1/semsis/encoder/tokenizer.py
--rw-r--r--   0        0        0     1719 2023-09-28 10:07:17.382286 semsis-0.1.1/semsis/encoder/tokenizer_test.py
--rw-r--r--   0        0        0     2567 2023-09-25 04:47:52.719653 semsis-0.1.1/semsis/kvstore.py
--rw-r--r--   0        0        0     2426 2023-09-25 04:47:52.719653 semsis-0.1.1/semsis/kvstore_test.py
--rw-r--r--   0        0        0      264 2023-09-28 10:07:17.382286 semsis-0.1.1/semsis/retriever/__init__.py
--rw-r--r--   0        0        0     6177 2023-10-31 09:49:43.556693 semsis-0.1.1/semsis/retriever/base.py
--rw-r--r--   0        0        0     3683 2023-10-31 09:49:43.556693 semsis-0.1.1/semsis/retriever/base_test.py
--rw-r--r--   0        0        0     7140 2023-09-28 10:07:17.382286 semsis-0.1.1/semsis/retriever/faiss_cpu.py
--rw-r--r--   0        0        0     9404 2023-10-04 10:35:35.529530 semsis-0.1.1/semsis/retriever/faiss_cpu_test.py
--rw-r--r--   0        0        0    11260 2023-10-17 04:57:54.997138 semsis-0.1.1/semsis/retriever/faiss_gpu.py
--rw-r--r--   0        0        0     1445 2023-09-28 10:07:17.382286 semsis-0.1.1/semsis/retriever/faiss_gpu_test.py
--rw-r--r--   0        0        0      812 2023-09-28 10:07:17.382286 semsis-0.1.1/semsis/utils.py
--rw-r--r--   0        0        0      780 2023-09-28 10:07:17.382286 semsis-0.1.1/semsis/utils_test.py
--rw-r--r--   0        0        0     4484 1970-01-01 00:00:00.000000 semsis-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1131 2023-09-28 10:07:17.382286 semsis-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3815 2024-04-03 07:09:13.844694 semsis-0.1.2/README.rst
+-rw-r--r--   0        0        0      682 2024-04-03 07:09:58.617577 semsis-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      331 2023-11-10 16:36:36.404226 semsis-0.1.2/semsis/__init__.py
+-rw-r--r--   0        0        0     2842 2023-11-08 03:12:33.344394 semsis-0.1.2/semsis/cli/README.rst
+-rw-r--r--   0        0        0     7012 2023-11-10 16:36:36.404226 semsis-0.1.2/semsis/cli/build_retriever.py
+-rw-r--r--   0        0        0     6148 2023-11-10 16:36:36.404226 semsis-0.1.2/semsis/cli/query_interactive.py
+-rw-r--r--   0        0        0     5779 2023-11-10 16:36:36.404226 semsis-0.1.2/semsis/cli/store_kv.py
+-rw-r--r--   0        0        0      275 2023-11-10 16:36:36.404226 semsis-0.1.2/semsis/encoder/__init__.py
+-rw-r--r--   0        0        0     4852 2023-11-14 07:12:25.235176 semsis-0.1.2/semsis/encoder/sentence_encoder.py
+-rw-r--r--   0        0        0     5225 2023-09-28 10:07:17.382286 semsis-0.1.2/semsis/encoder/sentence_encoder_test.py
+-rw-r--r--   0        0        0     2004 2023-09-28 10:07:17.382286 semsis-0.1.2/semsis/encoder/tokenizer.py
+-rw-r--r--   0        0        0     1719 2023-09-28 10:07:17.382286 semsis-0.1.2/semsis/encoder/tokenizer_test.py
+-rw-r--r--   0        0        0     2693 2023-11-08 03:13:51.917973 semsis-0.1.2/semsis/kvstore.py
+-rw-r--r--   0        0        0     2545 2023-11-08 03:13:51.917973 semsis-0.1.2/semsis/kvstore_test.py
+-rw-r--r--   0        0        0     1339 2023-11-10 16:36:36.404226 semsis-0.1.2/semsis/registry.py
+-rw-r--r--   0        0        0      776 2023-11-10 16:36:36.404226 semsis-0.1.2/semsis/registry_test.py
+-rw-r--r--   0        0        0      792 2023-11-10 16:36:36.404226 semsis-0.1.2/semsis/retriever/__init__.py
+-rw-r--r--   0        0        0     5533 2023-11-10 16:36:36.404226 semsis-0.1.2/semsis/retriever/base.py
+-rw-r--r--   0        0        0     3034 2023-11-10 16:36:36.404226 semsis-0.1.2/semsis/retriever/base_test.py
+-rw-r--r--   0        0        0     7135 2023-11-10 16:36:36.404226 semsis-0.1.2/semsis/retriever/faiss_cpu.py
+-rw-r--r--   0        0        0     9404 2023-10-04 10:35:35.529530 semsis-0.1.2/semsis/retriever/faiss_cpu_test.py
+-rw-r--r--   0        0        0    11255 2023-11-10 16:36:36.404226 semsis-0.1.2/semsis/retriever/faiss_gpu.py
+-rw-r--r--   0        0        0     1445 2023-09-28 10:07:17.382286 semsis-0.1.2/semsis/retriever/faiss_gpu_test.py
+-rw-r--r--   0        0        0      812 2023-09-28 10:07:17.382286 semsis-0.1.2/semsis/utils.py
+-rw-r--r--   0        0        0      780 2023-09-28 10:07:17.382286 semsis-0.1.2/semsis/utils_test.py
+-rw-r--r--   0        0        0     4542 1970-01-01 00:00:00.000000 semsis-0.1.2/PKG-INFO
```

### Comparing `semsis-0.1.1/LICENSE` & `semsis-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `semsis-0.1.1/README.rst` & `semsis-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `semsis-0.1.1/pyproject.toml` & `semsis-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "semsis"
-version = "0.1.1"
+version = "0.1.2"
 description = "A libary for semantic similarity search"
 authors = ["Hiroyuki Deguchi <deguchi.hiroyuki@nict.go.jp>"]
 license = "MIT"
 readme = "README.rst"
 packages = [{include = "semsis"}]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
-torch = "2.0.0"
+torch = "^2.0.0"
 transformers = "^4.33.2"
 sentence-transformers = "^2.2.2"
 h5py = "^3.9.0"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.9.1"
```

### Comparing `semsis-0.1.1/semsis/cli/README.rst` & `semsis-0.1.2/semsis/cli/README.rst`

 * *Files identical despite different names*

### Comparing `semsis-0.1.1/semsis/cli/build_retriever.py` & `semsis-0.1.2/semsis/cli/build_retriever.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 #!/usr/bin/env python3
-
+import contextlib
 import logging
 import math
 import os
 import sys
 from argparse import ArgumentParser, Namespace
 
 import numpy as np
 import torch
 from tqdm import tqdm
 
 from semsis.kvstore import KVStore
-from semsis.retriever import Retriever, get_retriever_type
+from semsis.retriever import Retriever
 from semsis.utils import Stopwatch
 
 logging.basicConfig(
     format="| %(asctime)s | %(levelname)s | %(message)s",
     datefmt="%Y-%m-%d %H:%M:%S",
     level="INFO",
     stream=sys.stdout,
 )
 logger = logging.getLogger("semsis.cli.build_retriever")
 
 
 def parse_args() -> Namespace:
     parser = ArgumentParser()
     # fmt: off
-    parser.add_argument("--kvstore", metavar="FILE", required=True,
-                        help="Path to a key--value store file.")
+    parser.add_argument("--kvstore", metavar="FILE", nargs="+", required=True,
+                        help="Path to key--value store files.")
     parser.add_argument("--index-path", metavar="FILE", required=True,
                         help="Path to an index file.")
     parser.add_argument("--trained-index-path", metavar="FILE",
                         help="Path to a trained index file. If this option is not specified, "
                         "the final index path will be set.")
     parser.add_argument("--config-path", metavar="FILE", required=True,
                         help="Path to a configuration file.")
@@ -57,23 +57,25 @@
                         help="Use OPQ to minimize the quantization error.")
     parser.add_argument("--pca", action="store_true",
                         help="Use PCA to reduce the dimension size.")
     parser.add_argument("--pca-dim", metavar="N", type=int, default=-1,
                         help="The dimension size which is reduced by PCA.")
     parser.add_argument("--append-sequential", action="store_true",
                         help="Append entries from the tail.")
+    parser.add_argument("--save-checkpoint", action="store_true",
+                        help="Save checkpoint after adding each key--value set.")
     # fmt: on
     return parser.parse_args()
 
 
 def train_retriever(
     args: Namespace, training_vectors: np.ndarray, use_gpu: bool = False
 ) -> Retriever:
     train_size, dim = training_vectors.shape
-    retriever_type = get_retriever_type(args.backend)
+    retriever_type = Retriever.get_cls(args.backend)
     dim = training_vectors.shape[1]
     cfg_dc = retriever_type.Config
     cfg_dict = {"dim": dim, "backend": args.backend, "metric": args.metric}
 
     def set_if_hasattr(name: str):
         if hasattr(cfg_dc, name):
             cfg_dict[name] = getattr(args, name)
@@ -116,43 +118,55 @@
 
 def main(args: Namespace) -> None:
     logger.info(args)
 
     timer = Stopwatch()
     use_gpu = torch.cuda.is_available() and not args.cpu
     chunk_size = args.chunk_size
-    with KVStore.open(args.kvstore, mode="r") as kvstore:
-        training_vectors = kvstore.key[: min(args.train_size, len(kvstore))]
-
-        retriever = train_retriever(args, training_vectors)
+    with contextlib.ExitStack() as stack:
+        kvstores = [
+            stack.enter_context(KVStore.open(fname, mode="r")) for fname in args.kvstore
+        ]
+        training_vectors = np.concatenate(
+            [
+                kvstore.key[: min(args.train_size // len(kvstores), len(kvstore))]
+                for kvstore in kvstores
+            ]
+        )
+        retriever = train_retriever(args, training_vectors, use_gpu=use_gpu)
         if use_gpu:
             retriever.to_gpu_add()
 
-        offset = 0
-        if args.append_sequential:
-            offset = len(retriever)
         logger.info(f"Build a retriever in {args.index_path}")
-        with timer.measure():
-            for i in tqdm(
-                range(math.ceil(len(kvstore) / chunk_size)), desc="Building a retriever"
-            ):
-                start_idx = i * chunk_size
-                end_idx = min(start_idx + chunk_size, len(kvstore))
-                num_added = end_idx - start_idx
-                logger.info(f"Add vectors: {num_added:,} / {len(kvstore):,}")
-                retriever.add(
-                    kvstore.key[start_idx:end_idx],
-                    kvstore.value[start_idx:end_idx] + offset,
-                )
-                logger.info(f"Retriever index size: {len(retriever):,}")
+        for kvstore in kvstores:
+            logger.info(f"Add {len(kvstore):,} vectors from {kvstore.filename}")
+            offset = len(retriever) if args.append_sequential else 0
+            with timer.measure():
+                for i in tqdm(
+                    range(math.ceil(len(kvstore) / chunk_size)),
+                    desc="Building a retriever",
+                ):
+                    start_idx = i * chunk_size
+                    end_idx = min(start_idx + chunk_size, len(kvstore))
+                    num_added = end_idx - start_idx
+                    logger.info(f"Add vectors: {num_added:,} / {len(kvstore):,}")
+                    retriever.add(
+                        kvstore.key[start_idx:end_idx],
+                        kvstore.value[start_idx:end_idx] + offset,
+                    )
+                    logger.info(f"Retriever index size: {len(retriever):,}")
+
+            if args.save_checkpoint:
+                retriever.save(args.index_path, args.config_path)
 
+        if not args.save_checkpoint:
             retriever.save(args.index_path, args.config_path)
 
-    logger.info(f"Added {len(retriever):,} datapoints")
-    logger.info(f"Retriever index size: {len(retriever):,}")
+        logger.info(f"Added {len(retriever):,} datapoints")
+        logger.info(f"Retriever index size: {len(retriever):,}")
     logger.info(f"Built the retriever in {timer.total:.1f} seconds")
 
 
 def cli_main() -> None:
     args = parse_args()
     main(args)
```

### Comparing `semsis-0.1.1/semsis/cli/query_interactive.py` & `semsis-0.1.2/semsis/cli/query_interactive.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from collections import defaultdict
 from os import PathLike
 from typing import Generator, List
 
 import torch
 
 from semsis.encoder import SentenceEncoder
-from semsis.retriever import get_retriever_type
-from semsis.retriever.base import load_backend_from_config
+from semsis.registry import get_registry
+from semsis.retriever import load_backend_from_config
 from semsis.utils import Stopwatch
 
 logging.basicConfig(
     format="| %(asctime)s | %(levelname)s | %(message)s",
     datefmt="%Y-%m-%d %H:%M:%S",
     level="INFO",
     stream=sys.stdout,
@@ -51,15 +51,16 @@
                         help="Input file.")
     parser.add_argument("--index-path", metavar="FILE",
                         help="Path to an index file.")
     parser.add_argument("--config-path", metavar="FILE", required=True,
                         help="Path to a configuration file.")
     parser.add_argument("--model", type=str, default="sentence-transformers/LaBSE",
                         help="Model name")
-    parser.add_argument("--representation", type=str, default="sbert", choices=["avg", "cls", "sbert"],
+    parser.add_argument("--representation", type=str, default="sbert",
+                        choices=get_registry("sentence_encoder").keys(),
                         help="Sentence representation type.")
     parser.add_argument("--gpu-encode", action="store_true",
                         help="Transfer the encoder to GPUs.")
     parser.add_argument("--gpu-retrieve", action="store_true",
                         help="Transfer the retriever to GPUs.")
     parser.add_argument("--fp16", action="store_true",
                         help="Use FP16.")
```

### Comparing `semsis-0.1.1/semsis/cli/store_kv.py` & `semsis-0.1.2/semsis/cli/store_kv.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 import torch
 from tqdm import tqdm
 from transformers import BatchEncoding
 
 from semsis.encoder import SentenceEncoder
 from semsis.encoder.tokenizer import Tokenizer
 from semsis.kvstore import KVStore
+from semsis.registry import get_registry
 from semsis.utils import Stopwatch
 
 logging.basicConfig(
     format="| %(asctime)s | %(levelname)s | %(message)s",
     datefmt="%Y-%m-%d %H:%M:%S",
     level="INFO",
     stream=sys.stdout,
@@ -130,15 +131,16 @@
     # fmt: off
     parser.add_argument("--input", type=str, required=True,
                         help="Input file.")
     parser.add_argument("--output", type=str, default="kv.bin",
                         help="Path to the key--value store.")
     parser.add_argument("--model", type=str, default="sentence-transformers/LaBSE",
                         help="Model name")
-    parser.add_argument("--representation", type=str, default="sbert", choices=["avg", "cls", "sbert"],
+    parser.add_argument("--representation", type=str, default="sbert",
+                        choices=get_registry("sentence_encoder").keys(),
                         help="Sentence representation type.")
     parser.add_argument("--batch-size", type=int, default=128,
                         help="Batch size.")
     parser.add_argument("--fp16", action="store_true",
                         help="Use FP16.")
     parser.add_argument("--workers", type=int, default=16,
                         help="Number of workers to preprocess the data.")
```

### Comparing `semsis-0.1.1/semsis/encoder/sentence_encoder.py` & `semsis-0.1.2/semsis/encoder/sentence_encoder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 import abc
-from typing import Dict, List, Literal
+from typing import Dict, List
 
 import torch
 import torch.nn as nn
 from sentence_transformers import SentenceTransformer
 from torch import Tensor
 from transformers import AutoModel
 
+from semsis import registry
+
 from .tokenizer import Tokenizer
 
+register, get_cls = registry.setup("sentence_encoder")
+
 
 class SentenceEncoder(nn.Module, metaclass=abc.ABCMeta):
     """Huggingface model wrapper.
 
     Args:
         name_or_path (str): Model name or path.
     """
@@ -40,36 +44,25 @@
     def freeze(self) -> None:
         for p in self.parameters():
             if getattr(p, "requires_grad", None) is not None:
                 p.requires_grad = False
         self.eval()
 
     @classmethod
-    def build(
-        cls,
-        model_name_or_path: str,
-        representation: Literal["avg", "cls", "sbert"],
-    ) -> "SentenceEncoder":
+    def build(cls, model_name_or_path: str, representation: str) -> "SentenceEncoder":
         """Build the sentence encoder model.
 
         Args:
             model_name_or_path (str): Model name or path of huggingface transformer models.
-            representation (Literal["avg", "cls", "sbert"]): Type of the sentence representation.
+            representation (str): Type of the sentence representation.
 
         Returns:
             SentenceEncoder: This class.
         """
-        if representation == "sbert":
-            return SentenceEncoderSbert(model_name_or_path)
-        elif representation == "avg":
-            return SentenceEncoderAvg(model_name_or_path)
-        elif representation == "cls":
-            return SentenceEncoderCls(model_name_or_path)
-        else:
-            raise NotImplementedError(f"`{representation}` is not supported.")
+        return get_cls(representation)(model_name_or_path)
 
     def encode(self, sentences: List[str]) -> Tensor:
         """Encode sentences into their sentence vectors.
 
         Args:
             sentences (List[str]): Input sentences.
 
@@ -96,14 +89,15 @@
             int: The size of the embedding dimension.
         """
         if hasattr(self.model.config, "hidden_size"):
             return self.model.config.hidden_size
         return self.model.get_input_embeddings().embedding_dim
 
 
+@register("avg")
 class SentenceEncoderAvg(SentenceEncoder):
     def forward(self, net_inputs: Dict[str, Tensor]) -> Tensor:
         """Return the feature vectors of the given inputs.
 
         Args:
             net_inputs (Dict[str, Tensor]): The inputs of huggingface models.
 
@@ -112,28 +106,30 @@
         """
         net_outputs = self.model(**net_inputs)
         non_pad_mask = net_inputs["attention_mask"]
         active_hiddens = net_outputs["last_hidden_state"] * non_pad_mask.unsqueeze(-1)
         return active_hiddens.sum(dim=1) / non_pad_mask.sum(dim=1, keepdim=True)
 
 
+@register("cls")
 class SentenceEncoderCls(SentenceEncoder):
     def forward(self, net_inputs: Dict[str, Tensor]) -> Tensor:
         """Return the feature vectors of the given inputs.
 
         Args:
             net_inputs (Dict[str, Tensor]): The inputs of huggingface models.
 
         Returns:
             Tensor: Output tensor of shape `(batch_size, embed_dim)`.
         """
         net_outputs = self.model(**net_inputs)
         return net_outputs["pooler_output"]
 
 
+@register("sbert")
 class SentenceEncoderSbert(SentenceEncoder):
     def load_model(self, name_or_path: str) -> None:
         """Load the model and tokenizer.
 
         Args:
             name_or_path (str): Model name or path.
         """
```

### Comparing `semsis-0.1.1/semsis/encoder/sentence_encoder_test.py` & `semsis-0.1.2/semsis/encoder/sentence_encoder_test.py`

 * *Files identical despite different names*

### Comparing `semsis-0.1.1/semsis/encoder/tokenizer.py` & `semsis-0.1.2/semsis/encoder/tokenizer.py`

 * *Files identical despite different names*

### Comparing `semsis-0.1.1/semsis/encoder/tokenizer_test.py` & `semsis-0.1.2/semsis/encoder/tokenizer_test.py`

 * *Files identical despite different names*

### Comparing `semsis-0.1.1/semsis/kvstore.py` & `semsis-0.1.2/semsis/kvstore.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,19 @@
         f (h5py.File): HDF5 file object.
     """
 
     def __init__(self, f: h5py.File) -> None:
         self.f = f
 
     @property
+    def filename(self) -> str:
+        """Returns the file name on the disk."""
+        return self.f.filename
+
+    @property
     def key(self) -> h5py.Dataset:
         """Return the key array."""
         return self.f["key"]
 
     @property
     def value(self) -> h5py.Dataset:
         """Return the value array."""
```

### Comparing `semsis-0.1.1/semsis/kvstore_test.py` & `semsis-0.1.2/semsis/kvstore_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,18 @@
         assert kvstore.f is f
 
     def test__len__(self, f: h5py.File):
         kvstore = KVStore(f)
         kvstore.new(D)
         assert len(kvstore) == 0
 
+    def test_filename(self, f: h5py.File):
+        kvstore = KVStore(f)
+        assert kvstore.filename == f.filename
+
     @pytest.mark.parametrize("dtype", [np.float32, np.float16])
     def test_dtype(self, f: h5py.File, dtype):
         kvstore = KVStore(f)
         kvstore.new(D, dtype=dtype)
         assert np.issubdtype(kvstore.dtype, dtype)
 
     @pytest.mark.parametrize("dtype", [np.float32, np.float16])
```

### Comparing `semsis-0.1.1/semsis/retriever/base.py` & `semsis-0.1.2/semsis/retriever/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import abc
 from dataclasses import asdict, dataclass
 from os import PathLike
-from typing import Any, Callable, Optional, Tuple, Type, TypeVar
+from typing import Any, Optional, Tuple, Type, TypeVar
 
 import numpy as np
 import yaml
 
+from semsis import retriever
+
 T = TypeVar("T")
 
 
 class Retriever(abc.ABC):
     """Base class of retriever classes.
 
     Args:
@@ -141,15 +143,15 @@
             distances (np.ndarray): Distances between the querys and the k nearest
                neighbor vectors.
             indices (np.ndarray): Indices of the k nearest neighbor vectors.
         """
 
     @classmethod
     def load(cls: Type[T], index_path: PathLike, cfg_path: PathLike) -> T:
-        """Loads the index and its configuration.
+        """Load the index and its configuration.
 
         Args:
             index_path (os.PathLike): Index file path.
             cfg_path (os.PathLike): Configuration file path.
 
         Returns:
             Retriever: This class.
@@ -178,53 +180,24 @@
 
         Returns:
             Any: Index object.
         """
 
     @abc.abstractmethod
     def save_index(self, path: PathLike) -> None:
-        """Saves the index.
+        """Save the index.
 
         Args:
             path (os.PathLike): Index file path to save.
         """
 
+    @classmethod
+    def get_cls(cls, name: str) -> Type["Retriever"]:
+        """Return the retriever class from the given name.
 
-T = TypeVar("T")
-
-REGISTRY = {}
-
-
-def register(name: str) -> Callable[[Type[T]], Type[T]]:
-    """Register a retriever class as the given name.
-
-    Args:
-        name (str): The name of a class.
-    """
-
-    def _register(cls: Type[T]):
-        if name in REGISTRY:
-            raise ValueError(
-                f"{name} already registered as {REGISTRY[name].__name__}. ({cls.__name__})"
-            )
-        REGISTRY[name] = cls
-        return cls
-
-    return _register
-
-
-def get_retriever_type(name: str) -> Type[Retriever]:
-    return REGISTRY[name]
-
-
-def load_backend_from_config(cfg_path: PathLike) -> Type[Retriever]:
-    """Load the backend retriever type from the configuration file.
-
-    Args:
-        cfg_path (os.PathLike): Path to the configuration file.
+        Args:
+            name (str): Registered name.
 
-    Returns:
-        Type[Retriever]: The backend retriever type.
-    """
-    with open(cfg_path, mode="r") as f:
-        cfg = yaml.safe_load(f)
-    return get_retriever_type(cfg["backend"])
+        Returns:
+            Type[Retriever]: Retriever class.
+        """
+        return retriever.get_cls(name)
```

### Comparing `semsis-0.1.1/semsis/retriever/base_test.py` & `semsis-0.1.2/semsis/retriever/base_test.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,21 +4,16 @@
 from pathlib import Path
 from typing import Any, Optional, Tuple
 
 import numpy as np
 import pytest
 import yaml
 
-from semsis.retriever.base import (
-    REGISTRY,
-    Retriever,
-    get_retriever_type,
-    load_backend_from_config,
-    register,
-)
+from semsis.retriever import load_backend_from_config, register
+from semsis.retriever.base import Retriever
 
 D = 8
 
 
 class RetrieverMock(Retriever):
     def __len__(self) -> int:
         ...
@@ -86,40 +81,14 @@
         retriever = RetrieverMock(index, cfg)
         retriever.save(idx_path, cfg_path)
         new_retriever = RetrieverMock.load(idx_path, cfg_path)
         assert new_retriever.index == retriever.index
         assert new_retriever.cfg == retriever.cfg
 
 
-def test_register():
-    assert "mock1" not in REGISTRY
-
-    @register("mock1")
-    class MockClass1(RetrieverMock):
-        ...
-
-    assert "mock1" in REGISTRY
-    assert issubclass(REGISTRY["mock1"], MockClass1)
-    assert issubclass(get_retriever_type("mock1"), MockClass1)
-
-    @register("mock2")
-    class MockClass2(RetrieverMock):
-        ...
-
-    assert "mock2" in REGISTRY
-    assert issubclass(REGISTRY["mock2"], MockClass2)
-    assert issubclass(get_retriever_type("mock2"), MockClass2)
-
-    with pytest.raises(ValueError):
-
-        @register("mock1")
-        class MockClass3(RetrieverMock):
-            ...
-
-
 def test_load_backend_from_config(tmp_path: Path):
     backend = "mock"
 
     @register(backend)
     class MockClass(RetrieverMock):
         @dataclass
         class Config(RetrieverMock.Config):
```

### Comparing `semsis-0.1.1/semsis/retriever/faiss_cpu.py` & `semsis-0.1.2/semsis/retriever/faiss_cpu.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from dataclasses import dataclass
 from os import PathLike
 from typing import Any, Dict, Optional, Tuple
 
 import faiss
 import numpy as np
 
-from semsis.retriever.base import Retriever, register
+from semsis.retriever import Retriever, register
 
 MetricType = int
 
 
 def faiss_index_builder(
     cfg: "RetrieverFaissCPU.Config", dim: int, metric: MetricType
 ) -> faiss.Index:
```

### Comparing `semsis-0.1.1/semsis/retriever/faiss_cpu_test.py` & `semsis-0.1.2/semsis/retriever/faiss_cpu_test.py`

 * *Files identical despite different names*

### Comparing `semsis-0.1.1/semsis/retriever/faiss_gpu.py` & `semsis-0.1.2/semsis/retriever/faiss_gpu.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from dataclasses import dataclass
 from typing import Optional, Union
 
 import faiss
 import numpy as np
 import torch
 
-from semsis.retriever.base import register
+from semsis.retriever import register
 from semsis.retriever.faiss_cpu import RetrieverFaissCPU
 
 logger = logging.getLogger(__name__)
 
 GpuIndex = (
     faiss.GpuIndex if hasattr(faiss, "GpuIndex") else faiss.Index
 )  # avoid error on faiss-cpu
```

### Comparing `semsis-0.1.1/semsis/retriever/faiss_gpu_test.py` & `semsis-0.1.2/semsis/retriever/faiss_gpu_test.py`

 * *Files identical despite different names*

### Comparing `semsis-0.1.1/semsis/utils.py` & `semsis-0.1.2/semsis/utils.py`

 * *Files identical despite different names*

### Comparing `semsis-0.1.1/semsis/utils_test.py` & `semsis-0.1.2/semsis/utils_test.py`

 * *Files identical despite different names*

### Comparing `semsis-0.1.1/PKG-INFO` & `semsis-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: semsis
-Version: 0.1.1
+Version: 0.1.2
 Summary: A libary for semantic similarity search
 License: MIT
 Author: Hiroyuki Deguchi
 Author-email: deguchi.hiroyuki@nict.go.jp
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: h5py (>=3.9.0,<4.0.0)
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0)
-Requires-Dist: torch (==2.0.0)
+Requires-Dist: torch (>=2.0.0,<3.0.0)
 Requires-Dist: transformers (>=4.33.2,<5.0.0)
 Description-Content-Type: text/x-rst
 
 SEMSIS: Semantic Similarity Search
 ##################################
 
 *Semsis* is a library for semantic similarity search.
```

