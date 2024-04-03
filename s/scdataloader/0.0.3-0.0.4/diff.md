# Comparing `tmp/scdataloader-0.0.3.tar.gz` & `tmp/scdataloader-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scdataloader-0.0.3.tar", max compression
+gzip compressed data, was "scdataloader-0.0.4.tar", max compression
```

## Comparing `scdataloader-0.0.3.tar` & `scdataloader-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0    35149 2023-12-30 13:53:34.323097 scdataloader-0.0.3/LICENSE
--rw-r--r--   0        0        0     2180 2024-02-14 12:07:03.422958 scdataloader-0.0.3/README.md
--rw-r--r--   0        0        0     1145 2024-02-15 10:35:30.804937 scdataloader-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        1 2023-12-30 14:13:14.273866 scdataloader-0.0.3/scdataloader/VERSION
--rw-r--r--   0        0        0      122 2024-02-12 14:09:56.907233 scdataloader-0.0.3/scdataloader/__init__.py
--rw-r--r--   0        0        0     5733 2024-02-15 08:58:53.879874 scdataloader-0.0.3/scdataloader/__main__.py
--rw-r--r--   0        0        0      338 2023-12-13 16:55:17.140286 scdataloader-0.0.3/scdataloader/base.py
--rw-r--r--   0        0        0     9524 2024-02-13 13:22:25.216190 scdataloader-0.0.3/scdataloader/collator.py
--rw-r--r--   0        0        0    13029 2024-02-15 09:36:52.401371 scdataloader-0.0.3/scdataloader/data.py
--rw-r--r--   0        0        0    10281 2024-02-14 18:58:01.436831 scdataloader-0.0.3/scdataloader/dataloader.py
--rw-r--r--   0        0        0    12635 2024-02-07 07:52:19.873085 scdataloader-0.0.3/scdataloader/mapped.py
--rw-r--r--   0        0        0    22550 2024-02-15 08:56:45.758619 scdataloader-0.0.3/scdataloader/preprocess.py
--rw-r--r--   0        0        0    17282 2024-02-14 12:51:23.439168 scdataloader-0.0.3/scdataloader/utils.py
--rw-r--r--   0        0        0    38289 1970-01-01 00:00:00.000000 scdataloader-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-02-28 08:39:17.422061 scdataloader-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3624 2024-04-03 12:40:42.337843 scdataloader-0.0.4/README.md
+-rw-r--r--   0        0        0     1145 2024-04-03 13:02:16.615956 scdataloader-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        6 2024-04-03 12:56:31.356328 scdataloader-0.0.4/scdataloader/VERSION
+-rw-r--r--   0        0        0      122 2024-04-03 12:35:50.130200 scdataloader-0.0.4/scdataloader/__init__.py
+-rw-r--r--   0        0        0     6297 2024-04-03 12:35:50.130200 scdataloader-0.0.4/scdataloader/__main__.py
+-rw-r--r--   0        0        0      338 2024-02-28 08:39:17.430061 scdataloader-0.0.4/scdataloader/base.py
+-rw-r--r--   0        0        0    11714 2024-04-03 12:35:50.134200 scdataloader-0.0.4/scdataloader/collator.py
+-rw-r--r--   0        0        0     2780 2024-04-03 12:35:50.134200 scdataloader-0.0.4/scdataloader/config.py
+-rw-r--r--   0        0        0    12292 2024-04-03 12:36:56.295058 scdataloader-0.0.4/scdataloader/data.py
+-rw-r--r--   0        0        0    14789 2024-04-03 12:35:50.134200 scdataloader-0.0.4/scdataloader/datamodule.py
+-rw-r--r--   0        0        0    13301 2024-04-03 12:35:50.134200 scdataloader-0.0.4/scdataloader/mapped.py
+-rw-r--r--   0        0        0    38205 2024-04-03 12:35:50.134200 scdataloader-0.0.4/scdataloader/preprocess.py
+-rw-r--r--   0        0        0    19365 2024-04-03 12:36:18.914576 scdataloader-0.0.4/scdataloader/utils.py
+-rw-r--r--   0        0        0    39733 1970-01-01 00:00:00.000000 scdataloader-0.0.4/PKG-INFO
```

### Comparing `scdataloader-0.0.3/LICENSE` & `scdataloader-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scdataloader-0.0.3/pyproject.toml` & `scdataloader-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "scdataloader"
-version = "0.0.3"
+version = "0.0.4"
 description = "a dataloader for single cell data in lamindb"
 authors = ["jkobject"]
 license = "GPL3"
 readme = ["README.md", "LICENSE"]
 repository = "https://github.com/jkobject/scDataLoader"
 keywords = ["scRNAseq", "dataloader", "pytorch", "lamindb", "scPrint"]
```

### Comparing `scdataloader-0.0.3/scdataloader/__main__.py` & `scdataloader-0.0.4/scdataloader/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,181 +1,202 @@
 import argparse
-from scdataloader.preprocess import LaminPreprocessor
+from scdataloader.preprocess import (
+    LaminPreprocessor,
+    additional_preprocess,
+    additional_postprocess,
+)
 import lamindb as ln
 from typing import Optional, Union
 
+
+# scdataloader --instance="laminlabs/cellxgene" --name="cellxgene-census" --version="2023-12-15" --description="preprocessed for scprint" --new_name="scprint main" --start_at=39
 def main():
     parser = argparse.ArgumentParser(
         description="Preprocess datasets in a given lamindb collection."
     )
     parser.add_argument(
         "--name", type=str, required=True, help="Name of the input dataset"
     )
     parser.add_argument(
-        "--new_name", type=str, required=True, help="Name of the preprocessed dataset."
+        "--new_name",
+        type=str,
+        default="preprocessed dataset",
+        help="Name of the preprocessed dataset.",
     )
     parser.add_argument(
         "--description",
         type=str,
-        default="preprocessed by scDataLoader"
+        default="preprocessed by scDataLoader",
         help="Description of the preprocessed dataset.",
     )
     parser.add_argument(
         "--start_at", type=int, default=0, help="Position to start preprocessing at."
     )
     parser.add_argument(
-        "--new_version", type=str, default="2", help="Version of the output dataset and files."
+        "--new_version",
+        type=str,
+        default="2",
+        help="Version of the output dataset and files.",
     )
     parser.add_argument(
-        "--instance", type=str, default=None, help="Instance storing the input dataset, if not local"
+        "--instance",
+        type=str,
+        default=None,
+        help="Instance storing the input dataset, if not local",
     )
     parser.add_argument(
         "--version", type=str, default=None, help="Version of the input dataset."
     )
     parser.add_argument(
         "--filter_gene_by_counts",
         type=Union[int, bool],
         default=False,
-        help="Determines whether to filter genes by counts."
+        help="Determines whether to filter genes by counts.",
     )
     parser.add_argument(
         "--filter_cell_by_counts",
         type=Union[int, bool],
         default=False,
-        help="Determines whether to filter cells by counts."
+        help="Determines whether to filter cells by counts.",
     )
     parser.add_argument(
         "--normalize_sum",
         type=float,
         default=1e4,
-        help="Determines whether to normalize the total counts of each cell to a specific value."
-    )
-    parser.add_argument(
-        "--keep_norm_layer",
-        type=bool,
-        default=False,
-        help="Determines whether to keep the normalization layer."
+        help="Determines whether to normalize the total counts of each cell to a specific value.",
     )
     parser.add_argument(
         "--subset_hvg",
         type=int,
         default=0,
-        help="Determines whether to subset highly variable genes."
+        help="Determines whether to subset highly variable genes.",
     )
     parser.add_argument(
         "--hvg_flavor",
         type=str,
         default="seurat_v3",
-        help="Specifies the flavor of highly variable genes selection."
+        help="Specifies the flavor of highly variable genes selection.",
     )
     parser.add_argument(
         "--binning",
         type=Optional[int],
         default=None,
-        help="Determines whether to bin the data into discrete values of number of bins provided."
+        help="Determines whether to bin the data into discrete values of number of bins provided.",
     )
     parser.add_argument(
         "--result_binned_key",
         type=str,
         default="X_binned",
-        help="Specifies the key of AnnData to store the binned data."
+        help="Specifies the key of AnnData to store the binned data.",
     )
     parser.add_argument(
         "--length_normalize",
         type=bool,
         default=False,
-        help="Determines whether to normalize the length."
+        help="Determines whether to normalize the length.",
     )
     parser.add_argument(
         "--force_preprocess",
         type=bool,
         default=False,
-        help="Determines whether to force preprocessing."
+        help="Determines whether to force preprocessing.",
     )
     parser.add_argument(
         "--min_dataset_size",
         type=int,
         default=100,
-        help="Specifies the minimum dataset size."
+        help="Specifies the minimum dataset size.",
     )
     parser.add_argument(
         "--min_valid_genes_id",
         type=int,
         default=10_000,
-        help="Specifies the minimum valid genes id."
+        help="Specifies the minimum valid genes id.",
     )
     parser.add_argument(
         "--min_nnz_genes",
         type=int,
-        default=200,
-        help="Specifies the minimum non-zero genes."
+        default=400,
+        help="Specifies the minimum non-zero genes.",
     )
     parser.add_argument(
         "--maxdropamount",
         type=int,
-        default=2,
-        help="Specifies the maximum drop amount."
+        default=50,
+        help="Specifies the maximum drop amount.",
     )
     parser.add_argument(
-        "--madoutlier",
-        type=int,
-        default=5,
-        help="Specifies the MAD outlier."
+        "--madoutlier", type=int, default=5, help="Specifies the MAD outlier."
     )
     parser.add_argument(
         "--pct_mt_outlier",
         type=int,
         default=8,
-        help="Specifies the percentage of MT outlier."
+        help="Specifies the percentage of MT outlier.",
     )
     parser.add_argument(
-        "--batch_key",
-        type=Optional[str],
-        default=None,
-        help="Specifies the batch key."
+        "--batch_key", type=Optional[str], default=None, help="Specifies the batch key."
     )
     parser.add_argument(
         "--skip_validate",
         type=bool,
         default=False,
-        help="Determines whether to skip validation."
+        help="Determines whether to skip validation.",
+    )
+    parser.add_argument(
+        "--do_postp",
+        type=bool,
+        default=False,
+        help="Determines whether to do postprocessing.",
     )
     args = parser.parse_args()
 
     # Load the collection
+    # if not args.preprocess:
+    #    print("Only preprocess is available for now")
+    #    return
     if args.instance is not None:
-        collection = ln.Collection.using(instance=args.instance).filter(name=args.name, version=args.version).first()
+        collection = (
+            ln.Collection.using(instance=args.instance)
+            .filter(name=args.name, version=args.version)
+            .first()
+        )
+    else:
+        collection = ln.Collection.filter(name=args.name, version=args.version).first()
 
-    collection = ln.Collection.filter(name=args.name, version=args.version).first()
-
-    print("using the dataset ",collection, " of size ",len(collection.artifacts.all()))
+    print(
+        "using the dataset ", collection, " of size ", len(collection.artifacts.all())
+    )
     # Initialize the preprocessor
     preprocessor = LaminPreprocessor(
         filter_gene_by_counts=args.filter_gene_by_counts,
         filter_cell_by_counts=args.filter_cell_by_counts,
         normalize_sum=args.normalize_sum,
-        keep_norm_layer=args.keep_norm_layer,
         subset_hvg=args.subset_hvg,
         hvg_flavor=args.hvg_flavor,
         binning=args.binning,
         result_binned_key=args.result_binned_key,
         length_normalize=args.length_normalize,
         force_preprocess=args.force_preprocess,
         min_dataset_size=args.min_dataset_size,
         min_valid_genes_id=args.min_valid_genes_id,
         min_nnz_genes=args.min_nnz_genes,
         maxdropamount=args.maxdropamount,
         madoutlier=args.madoutlier,
         pct_mt_outlier=args.pct_mt_outlier,
         batch_key=args.batch_key,
         skip_validate=args.skip_validate,
+        do_postp=args.do_postp,
+        additional_preprocess=additional_preprocess,
+        additional_postprocess=additional_postprocess,
+        keep_files=False,
     )
 
     # Preprocess the dataset
-    preprocessed_dataset = preprocessor(
+    preprocessor(
         collection,
         name=args.new_name,
         description=args.description,
         start_at=args.start_at,
         version=args.new_version,
     )
```

### Comparing `scdataloader-0.0.3/scdataloader/collator.py` & `scdataloader-0.0.4/scdataloader/collator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,81 +1,96 @@
 import numpy as np
 from .utils import load_genes
-from torch import Tensor
+from torch import Tensor, long
 
 # class SimpleCollator:
 
 
 class Collator:
     def __init__(
         self,
         organisms: list,
+        how="all",
         org_to_id: dict = None,
         valid_genes: list = [],
         max_len=2000,
-        n_bins=0,
-        add_zero_genes=200,
+        add_zero_genes=0,
         logp1=False,
         norm_to=None,
-        how="all",
+        n_bins=0,
         tp_name=None,
         organism_name="organism_ontology_term_id",
         class_names=[],
+        genelist=[],
     ):
         """
         This class is responsible for collating data for the scPRINT model. It handles the
         organization and preparation of gene expression data from different organisms,
         allowing for various configurations such as maximum gene list length, normalization,
         and selection method for gene expression.
 
+        This Collator should work with scVI's dataloader as well!
+
         Args:
             organisms (list): List of organisms to be considered for gene expression data.
+                it will drop any other organism it sees (might lead to batches of different sizes!)
+            how (flag, optional): Method for selecting gene expression. Defaults to "most expr".
+                one of ["most expr", "random expr", "all", "some"]:
+                "most expr": selects the max_len most expressed genes,
+                if less genes are expressed, will sample random unexpressed genes,
+                "random expr": uses a random set of max_len expressed genes.
+                if less genes are expressed, will sample random unexpressed genes
+                "all": uses all genes
+                "some": uses only the genes provided through the genelist param
             org_to_id (dict): Dictionary mapping organisms to their respective IDs.
-            labels (list, optional): List of labels for the data. Defaults to [].
             valid_genes (list, optional): List of genes from the datasets, to be considered. Defaults to [].
-            max_len (int, optional): Maximum length of the gene list. Defaults to 2000.
-            n_bins (int, optional): Number of bins for binning the data. Defaults to 0.
-            add_zero_genes (int, optional): Number of zero genes to add. Defaults to 200.
+                it will drop any other genes from the input expression data (usefull when your model only works on some genes)
+            max_len (int, optional): Maximum number of genes to use (for random expr and most expr). Defaults to 2000.
+            n_bins (int, optional): Number of bins for binning the data. Defaults to 0. meaning, no binning of expression.
+            add_zero_genes (int, optional): Number of additional unexpressed genes to add to the input data. Defaults to 0.
             logp1 (bool, optional): If True, logp1 normalization is applied. Defaults to False.
             norm_to (str, optional): Normalization method to be applied. Defaults to None.
-            how (str, optional): Method for selecting gene expression. Defaults to "most expr".
         """
         self.organisms = organisms
-        self.valid_genes = valid_genes
         self.max_len = max_len
         self.n_bins = n_bins
         self.add_zero_genes = add_zero_genes
         self.logp1 = logp1
         self.norm_to = norm_to
         self.org_to_id = org_to_id
         self.how = how
         self.organism_ids = (
             set([org_to_id[k] for k in organisms])
             if org_to_id is not None
             else set(organisms)
         )
+        if self.how == "some":
+            assert len(genelist) > 0, "if how is some, genelist must be provided"
         self.organism_name = organism_name
         self.tp_name = tp_name
         self.class_names = class_names
 
         self.start_idx = {}
         self.accepted_genes = {}
         self.genedf = load_genes(organisms)
+        self.to_subset = {}
         for organism in set(self.genedf.organism):
             ogenedf = self.genedf[self.genedf.organism == organism]
+            tot = self.genedf[self.genedf.index.isin(valid_genes)]
             org = org_to_id[organism] if org_to_id is not None else organism
-            self.start_idx.update(
-                {org: np.where(self.genedf.organism == organism)[0][0]}
-            )
+            self.start_idx.update({org: np.where(tot.organism == organism)[0][0]})
             if len(valid_genes) > 0:
                 self.accepted_genes.update({org: ogenedf.index.isin(valid_genes)})
+            if len(genelist) > 0:
+                df = ogenedf[ogenedf.index.isin(valid_genes)]
+                self.to_subset.update({org: df.index.isin(genelist)})
 
     def __call__(self, batch):
         """
-        __call__ is a special method in Python that is called when an instance of the class is called.
+        __call__ applies the collator to a minibatch of data
 
         Args:
             batch (list[dict[str: array]]): List of dicts of arrays containing gene expression data.
                 the first list is for the different samples, the second list is for the different elements with
                 elem["x"]: gene expression
                 elem["organism_name"]: organism ontology term id
                 elem["tp_name"]: heat diff
@@ -88,54 +103,84 @@
         # get the unseen info and don't add any unseen
         # get the I most expressed genes, add randomly some unexpressed genes that are not unseen
         exprs = []
         total_count = []
         other_classes = []
         gene_locs = []
         tp = []
+        dataset = []
+        nnz_loc = []
         for elem in batch:
             organism_id = elem[self.organism_name]
             if organism_id not in self.organism_ids:
                 continue
+            if "dataset" in elem:
+                dataset.append(elem["dataset"])
             expr = np.array(elem["x"])
             total_count.append(expr.sum())
             if len(self.accepted_genes) > 0:
                 expr = expr[self.accepted_genes[organism_id]]
             if self.how == "most expr":
-                loc = np.argsort(expr)[-(self.max_len) :][::-1]
+                nnz_loc = np.where(expr > 0)[0]
+                ma = self.max_len if self.max_len < len(nnz_loc) else len(nnz_loc)
+                loc = np.argsort(expr)[-(ma):][::-1]
+                # nnz_loc = [1] * 30_000
+                # loc = np.argsort(expr)[-(self.max_len) :][::-1]
             elif self.how == "random expr":
                 nnz_loc = np.where(expr > 0)[0]
                 loc = nnz_loc[
-                    np.random.choice(len(nnz_loc), self.max_len, replace=False)
+                    np.random.choice(
+                        len(nnz_loc),
+                        self.max_len if self.max_len < len(nnz_loc) else len(nnz_loc),
+                        replace=False,
+                        # p=(expr.max() + (expr[nnz_loc])*19) / expr.max(), # 20 at most times more likely to be selected
+                    )
                 ]
-            elif self.how == "all":
+            elif self.how in ["all", "some"]:
                 loc = np.arange(len(expr))
             else:
                 raise ValueError("how must be either most expr or random expr")
-            if self.add_zero_genes > 0 and self.how != "all":
+            if (
+                (self.add_zero_genes > 0) or (self.max_len > len(nnz_loc))
+            ) and self.how not in ["all", "some"]:
                 zero_loc = np.where(expr == 0)[0]
-                zero_loc = [
-                    np.random.choice(len(zero_loc), self.add_zero_genes, replace=False)
+                zero_loc = zero_loc[
+                    np.random.choice(
+                        len(zero_loc),
+                        self.add_zero_genes
+                        + (
+                            0
+                            if self.max_len < len(nnz_loc)
+                            else self.max_len - len(nnz_loc)
+                        ),
+                        replace=False,
+                    )
                 ]
                 loc = np.concatenate((loc, zero_loc), axis=None)
-            exprs.append(expr[loc])
-            gene_locs.append(loc + self.start_idx[organism_id])
+            expr = expr[loc]
+            loc = loc + self.start_idx[organism_id]
+            if self.how == "some":
+                expr = expr[self.to_subset[organism_id]]
+                loc = loc[self.to_subset[organism_id]]
+            exprs.append(expr)
+            gene_locs.append(loc)
 
             if self.tp_name is not None:
                 tp.append(elem[self.tp_name])
             else:
                 tp.append(0)
 
             other_classes.append([elem[i] for i in self.class_names])
 
         expr = np.array(exprs)
         tp = np.array(tp)
         gene_locs = np.array(gene_locs)
         total_count = np.array(total_count)
         other_classes = np.array(other_classes)
+        dataset = np.array(dataset)
 
         # normalize counts
         if self.norm_to is not None:
             expr = (expr * self.norm_to) / total_count[:, None]
         if self.logp1:
             expr = np.log2(1 + expr)
 
@@ -148,25 +193,34 @@
         # get the NN cells
 
         # do encoding / selection a la scGPT
 
         # do encoding of graph location
         # encode all the edges in some sparse way
         # normalizing total counts between 0,1
-        return {
+        ret = {
             "x": Tensor(expr),
             "genes": Tensor(gene_locs).int(),
             "class": Tensor(other_classes).int(),
             "tp": Tensor(tp),
             "depth": Tensor(total_count),
         }
+        if len(dataset) > 0:
+            ret.update({"dataset": Tensor(dataset).to(long)})
+        return ret
 
 
 class AnnDataCollator(Collator):
     def __init__(self, *args, **kwargs):
+        """
+        AnnDataCollator Collator to use if working with AnnData's experimental dataloader (it is very slow!!!)
+
+        Args:
+            @see Collator
+        """
         super().__init__(*args, **kwargs)
 
     def __call__(self, batch):
         exprs = []
         total_count = []
         other_classes = []
         gene_locs = []
@@ -214,47 +268,37 @@
             "x": Tensor(expr),
             "genes": Tensor(gene_locs).int(),
             "depth": Tensor(total_count),
             "class": Tensor(other_classes),
         }
 
 
-class SCVICollator(Collator):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-
-    def __call__(self, batch):
-        expr = batch["x"]
-        total_count = expr.sum(axis=1)
-        if self.how == "most expr":
-            loc = np.argsort(expr)[:, -(self.max_len) :][:, ::-1]
-        else:
-            raise ValueError("how must be either most expr or random expr")
-        if self.logp1:
-            expr = np.log2(1 + expr)
-        return {
-            "x": Tensor(expr[np.arange(expr.shape[0])[:, None], loc]),
-            "genes": Tensor(loc.copy()).int(),
-            "depth": Tensor(total_count),
-        }
-
-
 class GeneformerCollator(Collator):
     def __init__(self, *args, gene_norm_list: list, **kwargs):
+        """
+        GeneformerCollator to finish
+
+        Args:
+            gene_norm_list (list): the normalization of expression through all datasets, per gene.
+        """
         super().__init__(*args, **kwargs)
         self.gene_norm_list = gene_norm_list
 
     def __call__(self, batch):
         super().__call__(batch)
         # normlization per gene
 
         # tokenize the empty locations
 
 
 class scGPTCollator(Collator):
+    """
+    scGPTCollator to finish
+    """
+
     def __call__(self, batch):
         super().__call__(batch)
         # binning
 
         # tokenize the empty locations
```

### Comparing `scdataloader-0.0.3/scdataloader/data.py` & `scdataloader-0.0.4/scdataloader/data.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,120 +1,92 @@
 from dataclasses import dataclass, field
 
 import lamindb as ln
-import lnschema_bionty as lb
+import bionty as bt
 import pandas as pd
 from torch.utils.data import Dataset as torchDataset
-from typing import Union
+from typing import Union, Optional, Literal
 from scdataloader import mapped
 import warnings
 
-# TODO: manage load gene embeddings to make
-# from scprint.dataloader.embedder import embed
+from anndata import AnnData
+
 from scdataloader.utils import get_ancestry_mapping, load_genes
 
-LABELS_TOADD = {
-    "assay_ontology_term_id": {
-        "10x transcription profiling": "EFO:0030003",
-        "spatial transcriptomics": "EFO:0008994",
-        "10x 3' transcription profiling": "EFO:0030003",
-        "10x 5' transcription profiling": "EFO:0030004",
-    },
-    "disease_ontology_term_id": {
-        "metabolic disease": "MONDO:0005066",
-        "chronic kidney disease": "MONDO:0005300",
-        "chromosomal disorder": "MONDO:0019040",
-        "infectious disease": "MONDO:0005550",
-        "inflammatory disease": "MONDO:0021166",
-        # "immune system disease",
-        "disorder of development or morphogenesis": "MONDO:0021147",
-        "mitochondrial disease": "MONDO:0044970",
-        "psychiatric disorder": "MONDO:0002025",
-        "cancer or benign tumor": "MONDO:0002025",
-        "neoplasm": "MONDO:0005070",
-    },
-    "cell_type_ontology_term_id": {
-        "progenitor cell": "CL:0011026",
-        "hematopoietic cell": "CL:0000988",
-        "myoblast": "CL:0000056",
-        "myeloid cell": "CL:0000763",
-        "neuron": "CL:0000540",
-        "electrically active cell": "CL:0000211",
-        "epithelial cell": "CL:0000066",
-        "secretory cell": "CL:0000151",
-        "stem cell": "CL:0000034",
-        "non-terminally differentiated cell": "CL:0000055",
-        "supporting cell": "CL:0000630",
-    },
-}
+from .config import LABELS_TOADD
 
 
 @dataclass
 class Dataset(torchDataset):
     """
-    Dataset class to load a bunch of anndata from a lamin dataset in a memory efficient way.
+    Dataset class to load a bunch of anndata from a lamin dataset (Collection) in a memory efficient way.
+
+    This serves as a wrapper around lamin's mappedCollection to provide more features,
+    mostly, the management of hierarchical labels, the encoding of labels, the management of multiple species
 
-    For an example, see :meth:`~lamindb.Dataset.mapped`.
+    For an example of mappedDataset, see :meth:`~lamindb.Dataset.mapped`.
 
     .. note::
 
-        A similar data loader exists `here
+        A related data loader exists `here
         <https://github.com/Genentech/scimilarity>`__.
 
-    Attributes:
+    Args:
     ----
         lamin_dataset (lamindb.Dataset): lamin dataset to load
         genedf (pd.Dataframe): dataframe containing the genes to load
-        gene_embedding: dataframe containing the gene embeddings
         organisms (list[str]): list of organisms to load
-        obs (list[str]): list of observations to load
+            (for now only validates the the genes map to this organism)
+        obs (list[str]): list of observations to load from the Collection
         clss_to_pred (list[str]): list of observations to encode
-        hierarchical_clss: list of observations to map to a hierarchy
+        join_vars (flag): join variables @see :meth:`~lamindb.Dataset.mapped`.
+        hierarchical_clss: list of observations to map to a hierarchy using lamin's bionty
     """
 
     lamin_dataset: ln.Collection
-    genedf: pd.DataFrame = None
-    # gene_embedding: pd.DataFrame = None  # TODO: make it part of specialized dataset
-    organisms: Union[list[str], str] = field(
+    genedf: Optional[pd.DataFrame] = None
+    organisms: Optional[Union[list[str], str]] = field(
         default_factory=["NCBITaxon:9606", "NCBITaxon:10090"]
     )
-    obs: list[str] = field(
+    obs: Optional[list[str]] = field(
         default_factory=[
             "self_reported_ethnicity_ontology_term_id",
             "assay_ontology_term_id",
             "development_stage_ontology_term_id",
             "disease_ontology_term_id",
             "cell_type_ontology_term_id",
             "tissue_ontology_term_id",
             "sex_ontology_term_id",
             #'dataset_id',
             #'cell_culture',
-            "dpt_group",
-            "heat_diff",
-            "nnz",
+            #"dpt_group",
+            #"heat_diff",
+            #"nnz",
         ]
     )
     # set of obs to prepare for prediction (encode)
-    clss_to_pred: list[str] = field(default_factory=list)
+    clss_to_pred: Optional[list[str]] = field(default_factory=list)
     # set of obs that need to be hierarchically prepared
-    hierarchical_clss: list[str] = field(default_factory=list)
-    join_vars: str = "None"
+    hierarchical_clss: Optional[list[str]] = field(default_factory=list)
+    join_vars: Optional[Literal["auto", "inner", "None"]] = "None"
 
     def __post_init__(self):
         self.mapped_dataset = mapped.mapped(
             self.lamin_dataset,
             label_keys=self.obs,
             encode_labels=self.clss_to_pred,
             stream=True,
             parallel=True,
             join_vars=self.join_vars,
         )
         print(
             "won't do any check but we recommend to have your dataset coming from local storage"
         )
+        self.class_groupings = {}
+        self.class_topred = {}
         # generate tree from ontologies
         if len(self.hierarchical_clss) > 0:
             self.define_hierarchies(self.hierarchical_clss)
         if len(self.clss_to_pred) > 0:
             for clss in self.clss_to_pred:
                 if clss not in self.hierarchical_clss:
                     # otherwise it's already been done
@@ -145,70 +117,60 @@
 
     @property
     def encoder(self):
         return self.mapped_dataset.encoders
 
     def __getitem__(self, *args, **kwargs):
         item = self.mapped_dataset.__getitem__(*args, **kwargs)
-        #item.update({"unseen_genes": self.get_unseen_mapped_dataset_elements(*args, **kwargs)})
+        # import pdb
+
+        # pdb.set_trace()
+        # item.update(
+        #    {"unseen_genes": self.get_unseen_mapped_dataset_elements(*args, **kwargs)}
+        # )
         # ret = {}
         # ret["count"] = item[0]
         # for i, val in enumerate(self.obs):
         #    ret[val] = item[1][i]
         ## mark unseen genes with a flag
         ## send the associated
         # print(item[0].shape)
         return item
 
     def __repr__(self):
-        print(
-            "total dataset size is {} Gb".format(
+        return (
+            "total dataset size is {} Gb\n".format(
                 sum([file.size for file in self.lamin_dataset.artifacts.all()]) / 1e9
             )
-        )
-        print("---")
-        print("dataset contains:")
-        print("     {} cells".format(self.mapped_dataset.__len__()))
-        print("     {} genes".format(self.genedf.shape[0]))
-        print("     {} labels".format(len(self.obs)))
-        print("     {} organisms".format(len(self.organisms)))
-        print(
-            "dataset contains {} classes to predict".format(
-                sum([len(self.class_topred[i]) for i in self.class_topred])
+            + "---\n"
+            + "dataset contains:\n"
+            + "     {} cells\n".format(self.mapped_dataset.__len__())
+            + "     {} genes\n".format(self.genedf.shape[0])
+            + "     {} labels\n".format(len(self.obs))
+            + "     {} clss_to_pred\n".format(len(self.clss_to_pred))
+            + "     {} hierarchical_clss\n".format(len(self.hierarchical_clss))
+            + "     {} join_vars\n".format(len(self.join_vars))
+            + "     {} organisms\n".format(len(self.organisms))
+            + (
+                "dataset contains {} classes to predict\n".format(
+                    sum([len(self.class_topred[i]) for i in self.class_topred])
+                )
+                if len(self.class_topred) > 0
+                else ""
             )
         )
-        # print("embedding size is {}".format(self.gene_embedding.shape[1]))
-        return ""
 
     def get_label_weights(self, *args, **kwargs):
         return self.mapped_dataset.get_label_weights(*args, **kwargs)
 
-    def get_unseen_mapped_dataset_elements(self, idx):
+    def get_unseen_mapped_dataset_elements(self, idx: int):
         return [str(i)[2:-1] for i in self.mapped_dataset.uns(idx, "unseen_genes")]
 
-    # def load_embeddings(self, genedfs, embedding_size=128, cache=True):
-    #    embeddings = []
-    #    for o in self.organisms:
-    #        genedf = genedfs[genedfs.organism == o]
-    #        org_name = lb.Organism.filter(ontology_id=o).one().scientific_name
-    #        embedding = embed(
-    #            genedf=genedf,
-    #            organism=org_name,
-    #            cache=cache,
-    #            fasta_path="/tmp/data/fasta/",
-    #            embedding_size=embedding_size,
-    #        )
-    #        genedf = pd.concat(
-    #            [genedf.set_index("ensembl_gene_id"), embedding], axis=1, join="inner"
-    #        )
-    #        genedf.columns = genedf.columns.astype(str)
-    #        embeddings.append(genedf)
-    #    return pd.concat(embeddings)
-
-    def define_hierarchies(self, labels):
+    def define_hierarchies(self, labels: list[str]):
+        # TODO: use all possible hierarchies instead of just the ones for which we have a sample annotated with
         self.class_groupings = {}
         self.class_topred = {}
         for label in labels:
             if label not in [
                 "cell_type_ontology_term_id",
                 "tissue_ontology_term_id",
                 "disease_ontology_term_id",
@@ -219,58 +181,61 @@
                 raise ValueError(
                     "label {} not in accepted labels, for now only supported from bionty sources".format(
                         label
                     )
                 )
             elif label == "cell_type_ontology_term_id":
                 parentdf = (
-                    lb.CellType.filter()
+                    bt.CellType.filter()
                     .df(include=["parents__ontology_id"])
                     .set_index("ontology_id")
                 )
             elif label == "tissue_ontology_term_id":
                 parentdf = (
-                    lb.Tissue.filter()
+                    bt.Tissue.filter()
                     .df(include=["parents__ontology_id"])
                     .set_index("ontology_id")
                 )
             elif label == "disease_ontology_term_id":
                 parentdf = (
-                    lb.Disease.filter()
+                    bt.Disease.filter()
                     .df(include=["parents__ontology_id"])
                     .set_index("ontology_id")
                 )
             elif label == "development_stage_ontology_term_id":
                 parentdf = (
-                    lb.DevelopmentalStage.filter()
+                    bt.DevelopmentalStage.filter()
                     .df(include=["parents__ontology_id"])
                     .set_index("ontology_id")
                 )
             elif label == "assay_ontology_term_id":
                 parentdf = (
-                    lb.ExperimentalFactor.filter()
+                    bt.ExperimentalFactor.filter()
                     .df(include=["parents__ontology_id"])
                     .set_index("ontology_id")
                 )
             elif label == "self_reported_ethnicity_ontology_term_id":
                 parentdf = (
-                    lb.Ethnicity.filter()
+                    bt.Ethnicity.filter()
                     .df(include=["parents__ontology_id"])
                     .set_index("ontology_id")
                 )
 
             else:
                 raise ValueError(
                     "label {} not in accepted labels, for now only supported from bionty sources".format(
                         label
                     )
                 )
             cats = self.mapped_dataset.get_merged_categories(label)
             addition = set(LABELS_TOADD.get(label, {}).values())
             cats |= addition
+            # import pdb
+
+            # pdb.set_trace()
             groupings, _, lclass = get_ancestry_mapping(cats, parentdf)
             for i, j in groupings.items():
                 if len(j) == 0:
                     groupings.pop(i)
             self.class_groupings[label] = groupings
             if label in self.clss_to_pred:
                 # if we have added new labels, we need to update the encoder with them too.
@@ -312,15 +277,30 @@
                         self.class_topred[label] -= set([k])
                     else:
                         update.update({k: (v - c) - d})
                 self.mapped_dataset.encoders[label] = update
 
 
 class SimpleAnnDataset:
-    def __init__(self, adata, obs_to_output=[], layer=None):
+    def __init__(
+        self,
+        adata: AnnData,
+        obs_to_output: Optional[list[str]] = [],
+        layer: Optional[str] = None,
+    ):
+        """
+        SimpleAnnDataset is a simple dataloader for an AnnData dataset. this is to interface nicely with the rest of
+        scDataloader and with your model during inference.
+
+        Args:
+        ----
+            adata (anndata.AnnData): anndata object to use
+            obs_to_output (list[str]): list of observations to output from anndata.obs
+            layer (str): layer of the anndata to use
+        """
         self.adata = adata
         self.obs_to_output = obs_to_output
         self.layer = layer
 
     def __len__(self):
         return self.adata.shape[0]
```

### Comparing `scdataloader-0.0.3/scdataloader/mapped.py` & `scdataloader-0.0.4/scdataloader/mapped.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,14 +89,30 @@
         self.path_list = path_list
         self._make_connections(path_list, parallel)
 
         self.n_obs_list = []
         for storage in self.storages:
             with _Connect(storage) as store:
                 X = store["X"]
+                index = (
+                    store["var"]["ensembl_gene_id"]
+                    if "ensembl_gene_id" in store["var"]
+                    else store["var"]["_index"]
+                )
+                if join_vars == "None":
+                    if not all(
+                        [
+                            i <= j
+                            for i, j in zip(
+                                index[:99],
+                                index[1:100],
+                            )
+                        ]
+                    ):
+                        raise ValueError("The variables are not sorted.")
                 if isinstance(X, ArrayTypes):  # type: ignore
                     self.n_obs_list.append(X.shape[0])
                 else:
                     self.n_obs_list.append(X.attrs["shape"][0])
         self.n_obs = sum(self.n_obs_list)
 
         self.indices = np.hstack([np.arange(n_obs) for n_obs in self.n_obs_list])
@@ -175,26 +191,23 @@
         if self.var_indices is not None:
             var_idxs = self.var_indices[storage_idx]
         else:
             var_idxs = None
         with _Connect(self.storages[storage_idx]) as store:
             out = {"x": self.get_data_idx(store, obs_idx, var_idxs)}
             if self.label_keys is not None:
-                for i, label in enumerate(self.label_keys):
+                for _, label in enumerate(self.label_keys):
                     label_idx = self.get_label_idx(store, obs_idx, label)
                     if label in self.encoders:
                         out.update({label: self.encoders[label][label_idx]})
                     else:
                         out.update({label: label_idx})
+                out.update({"dataset": storage_idx})
         return out
 
-    def uns(self, idx, key):
-        storage = self.storages[self.storage_idx[idx]]
-        return storage["uns"][key]
-
     def get_data_idx(
         self,
         storage: StorageType,
         idx: int,
         var_idxs: Optional[list] = None,
         layer_key: Optional[str] = None,  # type: ignore # noqa
     ):
@@ -243,17 +256,19 @@
             if val not in self.label_keys:
                 raise ValueError(f"{val} is not a valid label key.")
             if i == 0:
                 labels = self.get_merged_labels(val)
             else:
                 labels += "_" + self.get_merged_labels(val).astype(str).astype("O")
         counter = Counter(labels)  # type: ignore
-        counter = np.array([counter[label] for label in labels])
+        rn = {n: i for i, n in enumerate(counter.keys())}
+        labels = np.array([rn[label] for label in labels])
+        counter = np.array(list(counter.values()))
         weights = scaler / (counter + scaler)
-        return weights
+        return weights, labels
 
     def get_merged_labels(self, label_key: str):
         """Get merged labels."""
         labels_merge = []
         decode = np.frompyfunc(lambda x: x.decode("utf-8"), 1, 1)
         for storage in self.storages:
             with _Connect(storage) as store:
```

### Comparing `scdataloader-0.0.3/scdataloader/utils.py` & `scdataloader-0.0.4/scdataloader/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,56 +7,64 @@
 import numpy as np
 import pandas as pd
 from biomart import BiomartServer
 from django.db import IntegrityError
 from scipy.sparse import csr_matrix
 from scipy.stats import median_abs_deviation
 from functools import lru_cache
+from collections import Counter
 
+from typing import Union, List, Optional
 
-def createFoldersFor(filepath):
+from anndata import AnnData
+
+
+def createFoldersFor(filepath: str):
     """
     will recursively create folders if needed until having all the folders required to save the file in this filepath
     """
     prevval = ""
     for val in os.path.expanduser(filepath).split("/")[:-1]:
         prevval += val + "/"
         if not os.path.exists(prevval):
             os.mkdir(prevval)
 
 
-def _fetchFromServer(ensemble_server, attributes):
+def _fetchFromServer(
+    ensemble_server: str, attributes: list, database: str = "hsapiens_gene_ensembl"
+):
     """
     Fetches data from the specified ensemble server.
 
     Args:
         ensemble_server (str): The URL of the ensemble server to fetch data from.
         attributes (list): The list of attributes to fetch from the server.
 
     Returns:
         pd.DataFrame: A pandas DataFrame containing the fetched data.
     """
     server = BiomartServer(ensemble_server)
-    ensmbl = server.datasets["hsapiens_gene_ensembl"]
+    ensmbl = server.datasets[database]
     print(attributes)
     res = pd.read_csv(
         io.StringIO(
             ensmbl.search({"attributes": attributes}, header=1).content.decode()
         ),
         sep="\t",
     )
     return res
 
 
 def getBiomartTable(
-    ensemble_server="http://jul2023.archive.ensembl.org/biomart",
-    useCache=False,
-    cache_folder="/tmp/biomart/",
-    attributes=[],
-    bypass_attributes=False,
+    ensemble_server: str = "http://jul2023.archive.ensembl.org/biomart",
+    useCache: bool = False,
+    cache_folder: str = "/tmp/biomart/",
+    attributes: List[str] = [],
+    bypass_attributes: bool = False,
+    database: str = "hsapiens_gene_ensembl",
 ):
     """generate a genelist dataframe from ensembl's biomart
 
     Args:
         ensemble_server (str, optional): the biomart server. Defaults to "http://jul2023.archive.ensembl.org/biomart".
         useCache (bool, optional): whether to use the cache or not. Defaults to False.
         cache_folder (str, optional): the cache folder. Defaults to "/tmp/biomart/".
@@ -84,29 +92,29 @@
     cachefile = os.path.join(cache_folder, ".biomart.csv")
     if useCache & os.path.isfile(cachefile):
         print("fetching gene names from biomart cache")
         res = pd.read_csv(cachefile)
     else:
         print("downloading gene names from biomart")
 
-        res = _fetchFromServer(ensemble_server, attr + attributes)
+        res = _fetchFromServer(ensemble_server, attr + attributes, database=database)
         res.to_csv(cachefile, index=False)
 
     res.columns = attr + attributes
     if type(res) is not type(pd.DataFrame()):
         raise ValueError("should be a dataframe")
     res = res[~(res["ensembl_gene_id"].isna() & res["hgnc_symbol"].isna())]
     res.loc[res[res.hgnc_symbol.isna()].index, "hgnc_symbol"] = res[
         res.hgnc_symbol.isna()
     ]["ensembl_gene_id"]
 
     return res
 
 
-def validate(adata, organism):
+def validate(adata: AnnData, organism: str):
     """
     validate checks if the adata object is valid for lamindb
 
     Args:
         adata (anndata): the anndata object
         lb (lamindb): the lamindb instance
         organism (str): the organism
@@ -140,17 +148,14 @@
         "tissue_ontology_term_id",
         "assay_ontology_term_id",
     ]:
         if val not in adata.obs.columns:
             raise ValueError(
                 f"Column '{val}' is missing in the provided anndata object."
             )
-    bionty_source = bt.PublicSource.filter(
-        entity="DevelopmentalStage", organism=organism
-    ).one()
 
     if not bt.Ethnicity.validate(
         adata.obs["self_reported_ethnicity_ontology_term_id"],
         field="ontology_id",
     ).all():
         raise ValueError("Invalid ethnicity ontology term id found")
     if not bt.Organism.validate(
@@ -165,53 +170,47 @@
         adata.obs["disease_ontology_term_id"], field="ontology_id"
     ).all():
         raise ValueError("Invalid disease ontology term id found")
     if not bt.CellType.validate(
         adata.obs["cell_type_ontology_term_id"], field="ontology_id"
     ).all():
         raise ValueError("Invalid cell type ontology term id found")
-    if (
-        not bt.DevelopmentalStage.filter(bionty_source=bionty_source)
-        .validate(
-            adata.obs["development_stage_ontology_term_id"],
-            field="ontology_id",
-        )
-        .all()
-    ):
+    if not bt.DevelopmentalStage.validate(
+        adata.obs["development_stage_ontology_term_id"],
+        field="ontology_id",
+    ).all():
         raise ValueError("Invalid dev stage ontology term id found")
     if not bt.Tissue.validate(
         adata.obs["tissue_ontology_term_id"], field="ontology_id"
     ).all():
         raise ValueError("Invalid tissue ontology term id found")
     if not bt.ExperimentalFactor.validate(
         adata.obs["assay_ontology_term_id"], field="ontology_id"
     ).all():
         raise ValueError("Invalid assay ontology term id found")
-    if (
-        not bt.Gene.filter(organism=bt.settings.organism)
-        .validate(adata.var.index, field="ensembl_gene_id")
-        .all()
-    ):
+    if not bt.Gene.validate(
+        adata.var.index, field="ensembl_gene_id", organism=organism
+    ).all():
         raise ValueError("Invalid gene ensembl id found")
     return True
 
 
 # setting a cache of 200 elements
 # @lru_cache(maxsize=200)
-def get_all_ancestors(val, df):
+def get_all_ancestors(val: str, df: pd.DataFrame):
     if val not in df.index:
         return set()
     parents = df.loc[val].parents__ontology_id
     if parents is None or len(parents) == 0:
         return set()
     else:
         return set.union(set(parents), *[get_all_ancestors(val, df) for val in parents])
 
 
-def get_ancestry_mapping(all_elem, onto_df):
+def get_ancestry_mapping(all_elem: list, onto_df: pd.DataFrame):
     """
     This function generates a mapping of all elements to their ancestors in the ontology dataframe.
 
     Args:
         all_elem (list): A list of all elements.
         onto_df (DataFrame): The ontology dataframe.
 
@@ -238,20 +237,20 @@
             if ancestor in full_ancestors:
                 groupings[ancestor].add(leaf)
 
     return groupings, full_ancestors, leafs
 
 
 def load_dataset_local(
-    remote_dataset,
-    download_folder,
-    name,
-    description,
-    use_cache=True,
-    only=None,
+    remote_dataset: ln.Collection,
+    download_folder: str,
+    name: str,
+    description: str,
+    use_cache: bool = True,
+    only: Optional[List[int]] = None,
 ):
     """
     This function loads a remote lamindb dataset to local.
 
     Args:
         lb (lamindb): The lamindb instance.
         remote_dataset (lamindb.Dataset): The remote Dataset.
@@ -299,45 +298,45 @@
             print(f"File {file.key} already exists in storage")
         saved_files.append(file)
     dataset = ln.Collection(saved_files, name=name, description=description)
     dataset.save()
     return dataset
 
 
-def load_genes(organisms):
+def load_genes(organisms: Union[str, list] = "NCBITaxon:9606"):  # "NCBITaxon:10090",
     organismdf = []
     if type(organisms) == str:
         organisms = [organisms]
     for organism in organisms:
         genesdf = bt.Gene.filter(
             organism_id=bt.Organism.filter(ontology_id=organism).first().id
         ).df()
         genesdf = genesdf[~genesdf["public_source_id"].isna()]
         genesdf = genesdf.drop_duplicates(subset="ensembl_gene_id")
-        genesdf = genesdf.set_index("ensembl_gene_id")
+        genesdf = genesdf.set_index("ensembl_gene_id").sort_index()
         # mitochondrial genes
         genesdf["mt"] = genesdf.symbol.astype(str).str.startswith("MT-")
         # ribosomal genes
         genesdf["ribo"] = genesdf.symbol.astype(str).str.startswith(("RPS", "RPL"))
         # hemoglobin genes.
         genesdf["hb"] = genesdf.symbol.astype(str).str.contains(("^HB[^(P)]"))
         genesdf["organism"] = organism
         organismdf.append(genesdf)
     return pd.concat(organismdf)
 
 
 def populate_my_ontology(
-    organisms=["NCBITaxon:10090", "NCBITaxon:9606"],
-    sex=["PATO:0000384", "PATO:0000383"],
-    celltypes=[],
-    ethnicities=[],
-    assays=[],
-    tissues=[],
-    diseases=[],
-    dev_stages=[],
+    organisms: List[str] = ["NCBITaxon:10090", "NCBITaxon:9606"],
+    sex: List[str] = ["PATO:0000384", "PATO:0000383"],
+    celltypes: List[str] = [],
+    ethnicities: List[str] = [],
+    assays: List[str] = [],
+    tissues: List[str] = [],
+    diseases: List[str] = [],
+    dev_stages: List[str] = [],
 ):
     """
     creates a local version of the lamin ontologies and add the required missing values in base ontologies
 
     run this function just one for each new lamin storage
 
     erase everything with bt.$ontology.filter().delete()
@@ -356,69 +355,80 @@
         ethnicities (list, optional): List of ethnicities. Defaults to [].
         assays (list, optional): List of assays. Defaults to [].
         tissues (list, optional): List of tissues. Defaults to [].
         diseases (list, optional): List of diseases. Defaults to [].
         dev_stages (list, optional): List of developmental stages. Defaults to [].
     """
 
-    names = bt.CellType.from_public().df().index if not celltypes else celltypes
+    names = bt.CellType.public().df().index if not celltypes else celltypes
     records = bt.CellType.from_values(names, field="ontology_id")
-    ln.save(records)
+    ln.save(records, parents=bool(celltypes))
     bt.CellType(name="unknown", ontology_id="unknown").save()
     # Organism
-    names = bt.Organism.from_public().df().index if not organisms else organisms
+    names = bt.Organism.public().df().index if not organisms else organisms
     records = [
         i[0] if type(i) is list else i
         for i in [bt.Organism.from_public(ontology_id=i) for i in names]
     ]
-    ln.save(records)
+    ln.save(records, parents=bool(organisms))
     bt.Organism(name="unknown", ontology_id="unknown").save()
     # Phenotype
-    names = bt.Phenotype.from_public().df().index if not sex else sex
+    names = bt.Phenotype.public().df().index if not sex else sex
     records = [
         bt.Phenotype.from_public(
             ontology_id=i,
             public_source=bt.PublicSource.filter(
                 entity="Phenotype", source="pato"
             ).one(),
         )
         for i in names
     ]
-    ln.save(records)
+    ln.save(records, parents=bool(sex))
     bt.Phenotype(name="unknown", ontology_id="unknown").save()
     # ethnicity
-    names = bt.Ethnicity.from_public().df().index if not ethnicities else ethnicities
+    names = bt.Ethnicity.public().df().index if not ethnicities else ethnicities
     records = bt.Ethnicity.from_values(names, field="ontology_id")
-    ln.save(records)
+    ln.save(records, parents=bool(ethnicities))
     bt.Ethnicity(
         name="unknown", ontology_id="unknown"
     ).save()  # multi ethnic will have to get renamed
     # ExperimentalFactor
-    names = bt.ExperimentalFactor.from_public().df().index if not assays else assays
+    names = bt.ExperimentalFactor.public().df().index if not assays else assays
     records = bt.ExperimentalFactor.from_values(names, field="ontology_id")
-    ln.save(records)
+    ln.save(records, parents=bool(assays))
     bt.ExperimentalFactor(name="unknown", ontology_id="unknown").save()
     # lookup = bt.ExperimentalFactor.lookup()
     # lookup.smart_seq_v4.parents.add(lookup.smart_like)
     # Tissue
-    names = bt.Tissue.from_public().df().index if not tissues else tissues
+    names = bt.Tissue.public().df().index if not tissues else tissues
     records = bt.Tissue.from_values(names, field="ontology_id")
-    ln.save(records)
+    ln.save(records, parents=bool(tissues))
     bt.Tissue(name="unknown", ontology_id="unknown").save()
     # DevelopmentalStage
     names = (
-        bt.DevelopmentalStage.from_public().df().index if not dev_stages else dev_stages
+        bt.DevelopmentalStage.public().df().index if not dev_stages else dev_stages
     )
     records = bt.DevelopmentalStage.from_values(names, field="ontology_id")
-    ln.save(records)
+    ln.save(records, parents=bool(dev_stages))
     bt.DevelopmentalStage(name="unknown", ontology_id="unknown").save()
+
+    names = bt.DevelopmentalStage.public(organism="mouse").df().name
+    bionty_source = bt.PublicSource.filter(
+        entity="DevelopmentalStage", organism="mouse"
+    ).one()
+    records = [
+        bt.DevelopmentalStage.from_public(name=i, public_source=bionty_source)
+        for i in names.tolist()
+    ]
+    records[-4] = records[-4][0]
+    ln.save(records)
     # Disease
-    names = bt.Disease.from_public().df().index if not diseases else diseases
+    names = bt.Disease.public().df().index if not diseases else diseases
     records = bt.Disease.from_values(names, field="ontology_id")
-    ln.save(records)
+    ln.save(records, parents=bool(diseases))
     bt.Disease(name="normal", ontology_id="PATO:0000461").save()
     bt.Disease(name="unknown", ontology_id="unknown").save()
     # genes
     for organism in ["NCBITaxon:10090", "NCBITaxon:9606"]:
         # convert onto to name
         organism = bt.Organism.filter(ontology_id=organism).one().name
         names = bt.Gene.public(organism=organism).df()["ensembl_gene_id"]
@@ -426,15 +436,15 @@
             names,
             field="ensembl_gene_id",
             organism=organism,
         )
         ln.save(records)
 
 
-def is_outlier(adata, metric: str, nmads: int):
+def is_outlier(adata: AnnData, metric: str, nmads: int):
     """
     is_outlier detects outliers in adata.obs[metric]
 
     Args:
         adata (annData): the anndata object
         metric (str): the metric column to use
         nmads (int): the number of median absolute deviations to use as a threshold
@@ -445,30 +455,30 @@
     M = adata.obs[metric]
     outlier = (M < np.median(M) - nmads * median_abs_deviation(M)) | (
         np.median(M) + nmads * median_abs_deviation(M) < M
     )
     return outlier
 
 
-def length_normalize(adata, gene_lengths):
+def length_normalize(adata: AnnData, gene_lengths: list):
     """
     length_normalize normalizes the counts by the gene length
 
     Args:
         adata (anndata): the anndata object
         gene_lengths (list): the gene lengths
 
     Returns:
         anndata: the anndata object
     """
     adata.X = csr_matrix((adata.X.T / gene_lengths).T)
     return adata
 
 
-def pd_load_cached(url, loc="/tmp/", cache=True, **kwargs):
+def pd_load_cached(url: str, loc: str = "/tmp/", cache: bool = True, **kwargs):
     """
     pd_load_cached downloads a file from a url and loads it as a pandas dataframe
 
     Args:
         url (str): the url to download the file from
         loc (str, optional): the location to save the file to. Defaults to "/tmp/".
         cache (bool, optional): whether to use the cached file or not. Defaults to True.
@@ -478,7 +488,40 @@
     """
     # Check if the file exists, if not, download it
     loc += url.split("/")[-1]
     if not os.path.isfile(loc) or not cache:
         urllib.request.urlretrieve(url, loc)
     # Load the data from the file
     return pd.read_csv(loc, **kwargs)
+
+
+def translate(
+    val: Union[str, list, set, Counter, dict], t: str = "cell_type_ontology_term_id"
+):
+    """
+    translate translates the ontology term id to the name
+
+    Args:
+        val (str, dict, set, list, dict): the object to translate
+        t (flat, optional): the type of ontology terms.
+            one of cell_type_ontology_term_id, assay_ontology_term_id, tissue_ontology_term_id.
+            Defaults to "cell_type_ontology_term_id".
+
+    Returns:
+        dict: the mapping for the translation
+    """
+    if t == "cell_type_ontology_term_id":
+        obj = bt.CellType.public(organism="all")
+    elif t == "assay_ontology_term_id":
+        obj = bt.ExperimentalFactor.public()
+    elif t == "tissue_ontology_term_id":
+        obj = bt.Tissue.public()
+    else:
+        return None
+    if type(val) is str:
+        return {val: obj.search(val, field=obj.ontology_id).name.iloc[0]}
+    elif type(val) is list or type(val) is set:
+        return {i: obj.search(i, field=obj.ontology_id).name.iloc[0] for i in set(val)}
+    elif type(val) is dict or type(val) is Counter:
+        return {
+            obj.search(k, field=obj.ontology_id).name.iloc[0]: v for k, v in val.items()
+        }
```

### Comparing `scdataloader-0.0.3/PKG-INFO` & `scdataloader-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scdataloader
-Version: 0.0.3
+Version: 0.0.4
 Summary: a dataloader for single cell data in lamindb
 Home-page: https://github.com/jkobject/scDataLoader
 License: GPL3
 Keywords: scRNAseq,dataloader,pytorch,lamindb,scPrint
 Author: jkobject
 Requires-Python: ==3.10.*
 Classifier: License :: Other/Proprietary License
@@ -30,14 +30,16 @@
 Project-URL: Repository, https://github.com/jkobject/scDataLoader
 Description-Content-Type: text/markdown
 
 # scdataloader
 
 [![codecov](https://codecov.io/gh/jkobject/scDataLoader/branch/main/graph/badge.svg?token=scDataLoader_token_here)](https://codecov.io/gh/jkobject/scDataLoader)
 [![CI](https://github.com/jkobject/scDataLoader/actions/workflows/main.yml/badge.svg)](https://github.com/jkobject/scDataLoader/actions/workflows/main.yml)
+[![DOI](https://zenodo.org/badge/731248665.svg)](https://zenodo.org/doi/10.5281/zenodo.10573143)
+
 
 Awesome single cell dataloader created by @jkobject 
 
 built on top of `lamindb` and the `.mapped()` function by Sergey: https://github.com/Koncopd 
 
 This data loader is designed to be used with:
 
@@ -62,15 +64,15 @@
 1. loading from lamin 
 2. doing some dataset specific preprocessing if needed 
 3. creating a dataset object on top of .mapped() (that is needed for mapping genes, cell labels etc..)
 4. passing it to a dataloader object that can work with it correctly
 
 Currently one would have to use the preprocess function to make the dataset fit for different tools like scGPT / Geneformer. But I would want to enable it through different Collators. This is still missing and a WIP... (please do contribute!)
 
-![](docs/scdataloader.drawio.png)
+![docs/scdataloader.drawio.png](docs/scdataloader.drawio.png)
 
 ## Install it from PyPI
 
 ```bash
 pip install scdataloader
 ```
 
@@ -81,14 +83,56 @@
 cd scDataLoader
 poetry install
 ```
 then run the notebooks with the poetry installed environment
 
 ## Usage
 
+```python
+# initialize a local lamin database
+# !lamin init --storage ~/scdataloader --schema bionty
+
+from scdataloader import utils
+from scdataloader.preprocess import LaminPreprocessor, additional_postprocess, additional_preprocess
+
+# preprocess datasets
+DESCRIPTION='preprocessed by scDataLoader'
+
+cx_dataset = ln.Collection.using(instance="laminlabs/cellxgene").filter(name="cellxgene-census", version='2023-12-15').one()
+cx_dataset, len(cx_dataset.artifacts.all())
+
+
+do_preprocess = LaminPreprocessor(additional_postprocess=additional_postprocess, additional_preprocess=additional_preprocess, skip_validate=True, subset_hvg=0)
+
+preprocessed_dataset = do_preprocess(cx_dataset, name=DESCRIPTION, description=DESCRIPTION, start_at=6, version="2")
+
+# create dataloaders
+from scdataloader import DataModule
+import tqdm
+
+datamodule = DataModule(
+    collection_name="preprocessed dataset",
+    organisms=["NCBITaxon:9606"], #organism that we will work on
+    how="most expr", # for the collator (most expr genes only will be selected)
+    max_len=1000, # only the 1000 most expressed
+    batch_size=64,
+    num_workers=1,
+    validation_split=0.1,
+    test_split=0)
+
+for i in tqdm.tqdm(datamodule.train_dataloader()):
+    # pass #or do pass
+    print(i)
+    break
+
+# with lightning:
+# Trainer(model, datamodule)
+
+```
+
 see the notebooks in [docs](https://jkobject.github.io/scDataLoader/):
 
 1. [load a dataset](https://jkobject.github.io/scDataLoader/notebooks/01_load_dataset.html)
 2. [create a dataset](https://jkobject.github.io/scDataLoader/notebooks/02_create_dataset.html)
 
 ## Development
```

