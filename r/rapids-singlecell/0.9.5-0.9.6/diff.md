# Comparing `tmp/rapids_singlecell-0.9.5.tar.gz` & `tmp/rapids_singlecell-0.9.6.tar.gz`

## Comparing `rapids_singlecell-0.9.5.tar` & `rapids_singlecell-0.9.6.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/.cirun.yml
--rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/.readthedocs.yml
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/.github/ISSUE_TEMPLATE/submit-question.md
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/.github/workflows/test-gpu.yml
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/ci/rsc_test_env.yml
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/conda/rsc_rapids_23.04.yml
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/conda/rsc_rapids_23.12.yml
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/_version.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/dcg.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/gr.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/pp.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/tl.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/utils.py
--rw-r--r--   0        0        0    26245 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/cunnData/__init__.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/decoupler_gpu/__init__.py
--rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/decoupler_gpu/_method_mlm.py
--rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/decoupler_gpu/_method_wsum.py
--rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/__init__.py
--rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_harmony_integrate.py
--rw-r--r--   0        0        0    12301 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_harmonypy_gpu.py
--rw-r--r--   0        0        0    36396 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_hvg.py
--rw-r--r--   0        0        0    11853 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_neighbors.py
--rw-r--r--   0        0        0     9615 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_normalize.py
--rw-r--r--   0        0        0    10009 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_pca.py
--rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_regress_out.py
--rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_scale.py
--rw-r--r--   0        0        0    14223 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_simple.py
--rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_utils.py
--rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_kernels/_mean_var_kernel.py
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_kernels/_norm_kernel.py
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_kernels/_pca_sparse_kernel.py
--rw-r--r--   0        0        0     9353 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_kernels/_pr_kernels.py
--rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_kernels/_qc_kernels.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/squidpy_gpu/__init__.py
--rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/squidpy_gpu/_autocorr.py
--rw-r--r--   0        0        0     8268 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/squidpy_gpu/_gearysc.py
--rw-r--r--   0        0        0    29550 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/squidpy_gpu/_ligrec.py
--rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/squidpy_gpu/_moransi.py
--rw-r--r--   0        0        0     6230 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/squidpy_gpu/_utils.py
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/tools/__init__.py
--rw-r--r--   0        0        0    10110 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/tools/_clustering.py
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/tools/_diffmap.py
--rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/tools/_draw_graph.py
--rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/tools/_embedding_density.py
--rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/tools/_pymde.py
--rw-r--r--   0        0        0     7921 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/tools/_rank_gene_groups.py
--rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/tools/_tsne.py
--rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/tools/_umap.py
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/src/rapids_singlecell/tools/_utils.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/LICENSE
--rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/README.md
--rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/pyproject.toml
--rw-r--r--   0        0        0     6318 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.5/PKG-INFO
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/.cirun.yml
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/.readthedocs.yml
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      511 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/.github/ISSUE_TEMPLATE/submit-question.md
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/.github/workflows/test-gpu.yml
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/ci/rsc_test_env.yml
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/conda/rsc_rapids_23.12.yml
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/conda/rsc_rapids_24.02.yml
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/_version.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/dcg.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/gr.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/pp.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/tl.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/utils.py
+-rw-r--r--   0        0        0    26245 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/cunnData/__init__.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/decoupler_gpu/__init__.py
+-rw-r--r--   0        0        0     4791 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/decoupler_gpu/_method_mlm.py
+-rw-r--r--   0        0        0     6520 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/decoupler_gpu/_method_wsum.py
+-rw-r--r--   0        0        0      423 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/__init__.py
+-rw-r--r--   0        0        0     1780 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_harmony_integrate.py
+-rw-r--r--   0        0        0    12301 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_harmonypy_gpu.py
+-rw-r--r--   0        0        0    36396 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_hvg.py
+-rw-r--r--   0        0        0    11853 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_neighbors.py
+-rw-r--r--   0        0        0     9612 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_normalize.py
+-rw-r--r--   0        0        0    10023 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_pca.py
+-rw-r--r--   0        0        0     4875 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_regress_out.py
+-rw-r--r--   0        0        0     1725 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_scale.py
+-rw-r--r--   0        0        0    14223 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_simple.py
+-rw-r--r--   0        0        0     2962 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_utils.py
+-rw-r--r--   0        0        0     1568 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_kernels/_mean_var_kernel.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_kernels/_norm_kernel.py
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_kernels/_pca_sparse_kernel.py
+-rw-r--r--   0        0        0     9353 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_kernels/_pr_kernels.py
+-rw-r--r--   0        0        0     5020 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_kernels/_qc_kernels.py
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/squidpy_gpu/__init__.py
+-rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/squidpy_gpu/_autocorr.py
+-rw-r--r--   0        0        0     8268 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/squidpy_gpu/_gearysc.py
+-rw-r--r--   0        0        0    29550 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/squidpy_gpu/_ligrec.py
+-rw-r--r--   0        0        0     8699 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/squidpy_gpu/_moransi.py
+-rw-r--r--   0        0        0     6230 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/squidpy_gpu/_utils.py
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/tools/__init__.py
+-rw-r--r--   0        0        0    10323 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/tools/_clustering.py
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/tools/_diffmap.py
+-rw-r--r--   0        0        0     4046 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/tools/_draw_graph.py
+-rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/tools/_embedding_density.py
+-rw-r--r--   0        0        0     2440 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/tools/_pymde.py
+-rw-r--r--   0        0        0     7921 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/tools/_rank_gene_groups.py
+-rw-r--r--   0        0        0     3727 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/tools/_tsne.py
+-rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/tools/_umap.py
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/src/rapids_singlecell/tools/_utils.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/LICENSE
+-rw-r--r--   0        0        0     3612 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/README.md
+-rw-r--r--   0        0        0     2456 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/pyproject.toml
+-rw-r--r--   0        0        0     6318 2020-02-02 00:00:00.000000 rapids_singlecell-0.9.6/PKG-INFO
```

### Comparing `rapids_singlecell-0.9.5/.pre-commit-config.yaml` & `rapids_singlecell-0.9.6/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 repos:
 -   repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.1.9
+    rev: v0.2.2
     hooks:
     -   id: ruff
         args: [--fix, --exit-non-zero-on-fix]
     - id: ruff-format
 -   repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.5.0
     hooks:
```

### Comparing `rapids_singlecell-0.9.5/.github/ISSUE_TEMPLATE/bug_report.md` & `rapids_singlecell-0.9.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/.github/workflows/publish.yml` & `rapids_singlecell-0.9.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/.github/workflows/test-gpu.yml` & `rapids_singlecell-0.9.6/.github/workflows/test-gpu.yml`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/utils.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/utils.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/cunnData/__init__.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/cunnData/__init__.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/decoupler_gpu/_method_mlm.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/decoupler_gpu/_method_mlm.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/decoupler_gpu/_method_wsum.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/decoupler_gpu/_method_wsum.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_harmony_integrate.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_harmony_integrate.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_harmonypy_gpu.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_harmonypy_gpu.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_hvg.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_hvg.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_neighbors.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_neighbors.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_normalize.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_normalize.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,18 +19,18 @@
     inplace: bool = True,
 ) -> Optional[Union[sparse.csr_matrix, cp.ndarray]]:
     """
     Normalizes rows in matrix so they sum to `target_sum`
 
     Parameters
     ----------
-        adata:
+        adata
             AnnData/ cunnData object
 
-        target_sum :
+        target_sum
             If `None`, after normalization, each observation (cell) has a total count equal to the median of total counts for observations (cells) before normalization.
 
         layer
             Layer to normalize instead of `X`. If `None`, `X` is normalized.
 
         inplace
             Whether to update `adata` or return the normalized matrix.
```

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_pca.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_pca.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,56 +24,57 @@
     chunk_size: int = None,
 ) -> None:
     """
     Performs PCA using the cuml decomposition function.
 
     Parameters
     ----------
-        adata :
+        adata
             AnnData/ cunnData object
 
         layer
             If provided, use `adata.layers[layer]` for expression values instead of `adata.X`.
 
         n_comps
-            Number of principal components to compute. Defaults to 50, or 1 - minimum
+            Number of principal components to compute. Defaults to 50, or 1 - minimum \
             dimension size of selected representation
 
         zero_center
-            If `True`, compute standard PCA from covariance matrix.
+            If `True`, compute standard PCA from covariance matrix. \
             If `False`, omit zero-centering variables
 
         random_state
             Change to use different initial states for the optimization.
 
         use_highly_variable
-            Whether to use highly variable genes only, stored in
-            `.var['highly_variable']`.
+            Whether to use highly variable genes only, stored in \
+            `.var['highly_variable']`. \
             By default uses them if they have been determined beforehand.
 
         chunked
-            If `True`, perform an incremental PCA on segments of `chunk_size`.
-            The incremental PCA automatically zero centers and ignores settings of
+            If `True`, perform an incremental PCA on segments of `chunk_size`. \
+            The incremental PCA automatically zero centers and ignores settings of \
             `random_seed` and `svd_solver`. If `False`, perform a full PCA.
 
         chunk_size
-            Number of observations to include in each chunk.
+            Number of observations to include in each chunk. \
             Required if `chunked=True` was passed.
 
     Returns
     -------
-        adds fields to `adata` :
+        adds fields to `adata`:
+
             `.obsm['X_pca']`
                 PCA representation of data.
             `.varm['PCs']`
                 The principal components containing the loadings.
             `.uns['pca']['variance_ratio']`
                 Ratio of explained variance.
             `.uns['pca']['variance']`
-                Explained variance, equivalent to the eigenvalues of the
+                Explained variance, equivalent to the eigenvalues of the \
                 covariance matrix.
     """
     if use_highly_variable is True and "highly_variable" not in adata.var.keys():
         raise ValueError(
             "Did not find adata.var['highly_variable']. "
             "Either your data already only consists of highly-variable genes "
             "or consider running `highly_variable_genes` first."
```

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_regress_out.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_regress_out.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_scale.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_scale.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_simple.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_simple.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_utils.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_utils.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_kernels/_mean_var_kernel.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_kernels/_mean_var_kernel.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_kernels/_norm_kernel.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_kernels/_norm_kernel.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_kernels/_pca_sparse_kernel.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_kernels/_pca_sparse_kernel.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_kernels/_pr_kernels.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_kernels/_pr_kernels.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/preprocessing/_kernels/_qc_kernels.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/preprocessing/_kernels/_qc_kernels.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/squidpy_gpu/_autocorr.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/squidpy_gpu/_autocorr.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/squidpy_gpu/_gearysc.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/squidpy_gpu/_gearysc.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/squidpy_gpu/_ligrec.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/squidpy_gpu/_ligrec.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -233,18 +233,18 @@
         * `pvalues` -
             :class:`pandas.DataFrame` containing the possibly corrected p-values.
         * `metadata` -
             :class:`pandas.DataFrame` containing interaction metadata.
     Otherwise, modifies the adata object with the following key:
         * :attr:`~anndata.AnnData.uns` `['{key_added}']` -
             the above mentioned dict.
+
     NaN p-values mark combinations for which the mean expression of one of the \
     interacting components was 0 or it didnt pass the threshold percentage of \
     cells being expressed within a given cluster.
-
     """
     # Get and Check interactions
     if interactions is None:
         interactions = _get_interactions(
             interactions_params, transmitter_params, receiver_params
         )
```

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/squidpy_gpu/_moransi.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/squidpy_gpu/_moransi.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/squidpy_gpu/_utils.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/squidpy_gpu/_utils.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/tools/_clustering.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/tools/_clustering.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,18 +88,18 @@
     adata = adata.copy() if copy else adata
 
     if adjacency is None:
         adjacency = _choose_graph(adata, obsp, neighbors_key)
     if restrict_to is not None:
         restrict_key, restrict_categories = restrict_to
         adjacency, restrict_indices = restrict_adjacency(
-            adata,
-            restrict_key,
-            restrict_categories,
-            adjacency,
+            adata=adata,
+            restrict_key=restrict_key,
+            restrict_categories=restrict_categories,
+            adjacency=adjacency,
         )
     offsets = cudf.Series(adjacency.indptr)
     indices = cudf.Series(adjacency.indices)
     if use_weights:
         weights = cudf.Series(adjacency.data)
     else:
         weights = None
@@ -121,19 +121,19 @@
         leiden_parts.to_pandas().sort_values("vertex")[["partition"]].to_numpy().ravel()
     )
     if restrict_to is not None:
         if key_added == "leiden":
             key_added += "_R"
         groups = rename_groups(
             adata,
-            key_added,
-            restrict_key,
-            restrict_categories,
-            restrict_indices,
-            groups,
+            key_added=key_added,
+            restrict_key=restrict_key,
+            restrict_categories=restrict_categories,
+            restrict_indices=restrict_indices,
+            groups=groups,
         )
     adata.obs[key_added] = pd.Categorical(
         values=groups.astype("U"),
         categories=natsorted(map(str, np.unique(groups))),
     )
     # store information on the clustering parameters
     adata.uns["leiden"] = {}
@@ -229,16 +229,16 @@
     if adjacency is None:
         adjacency = _choose_graph(adata, obsp, neighbors_key)
     if restrict_to is not None:
         restrict_key, restrict_categories = restrict_to
         adjacency, restrict_indices = restrict_adjacency(
             adata,
             restrict_key,
-            restrict_categories,
-            adjacency,
+            restrict_categories=restrict_categories,
+            adjacency=adjacency,
         )
 
     offsets = cudf.Series(adjacency.indptr)
     indices = cudf.Series(adjacency.indices)
     if use_weights:
         weights = cudf.Series(adjacency.data)
     else:
@@ -271,19 +271,19 @@
         .ravel()
     )
     if restrict_to is not None:
         if key_added == "louvain":
             key_added += "_R"
         groups = rename_groups(
             adata,
-            key_added,
-            restrict_key,
-            restrict_categories,
-            restrict_indices,
-            groups,
+            key_added=key_added,
+            restrict_key=restrict_key,
+            restrict_categories=restrict_categories,
+            restrict_indices=restrict_indices,
+            groups=groups,
         )
 
     adata.obs[key_added] = pd.Categorical(
         values=groups.astype("U"),
         categories=natsorted(map(str, np.unique(groups))),
     )
     adata.uns["louvain"] = {}
```

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/tools/_diffmap.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/tools/_diffmap.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/tools/_draw_graph.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/tools/_draw_graph.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/tools/_embedding_density.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/tools/_embedding_density.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/tools/_pymde.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/tools/_pymde.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/tools/_rank_gene_groups.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/tools/_rank_gene_groups.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/tools/_tsne.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/tools/_tsne.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/tools/_umap.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/tools/_umap.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/src/rapids_singlecell/tools/_utils.py` & `rapids_singlecell-0.9.6/src/rapids_singlecell/tools/_utils.py`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/LICENSE` & `rapids_singlecell-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/README.md` & `rapids_singlecell-0.9.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 Our commitment with rapids-singlecell is to deliver a powerful, user-centric tool that significantly enhances single-cell data analysis capabilities in bioinformatics.
 
 ## Installation
 ### Conda
 The easiest way to install *rapids-singlecell* is to use one of the *yaml* file provided in the [conda](https://github.com/scverse/rapids_singlecell/tree/main/conda) folder. These *yaml* files install everything needed to run the example notbooks and get you started.
 ```
-conda env create -f conda/rsc_rapids_23.04.yml
+conda env create -f conda/rsc_rapids_24.02.yml
 # or
 mamba env create -f conda/rsc_rapids_23.12.yml
 ```
 ### PyPI
 ```
 pip install rapids-singlecell
 ```
```

### Comparing `rapids_singlecell-0.9.5/pyproject.toml` & `rapids_singlecell-0.9.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `rapids_singlecell-0.9.5/PKG-INFO` & `rapids_singlecell-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapids_singlecell
-Version: 0.9.5
+Version: 0.9.6
 Summary: running single cell analysis on Nvidia GPUs
 Project-URL: Documentation, https://rapids-singlecell.readthedocs.io
 Project-URL: Source, https://github.com/scverse/rapids_singlecell
 Author: Severin Dicks
 License: MIT License
         
         Copyright (c) 2022 Severin Dicks
@@ -77,15 +77,15 @@
 
 Our commitment with rapids-singlecell is to deliver a powerful, user-centric tool that significantly enhances single-cell data analysis capabilities in bioinformatics.
 
 ## Installation
 ### Conda
 The easiest way to install *rapids-singlecell* is to use one of the *yaml* file provided in the [conda](https://github.com/scverse/rapids_singlecell/tree/main/conda) folder. These *yaml* files install everything needed to run the example notbooks and get you started.
 ```
-conda env create -f conda/rsc_rapids_23.04.yml
+conda env create -f conda/rsc_rapids_24.02.yml
 # or
 mamba env create -f conda/rsc_rapids_23.12.yml
 ```
 ### PyPI
 ```
 pip install rapids-singlecell
 ```
```

