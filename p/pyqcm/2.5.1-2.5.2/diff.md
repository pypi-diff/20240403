# Comparing `tmp/pyqcm-2.5.1.tar.gz` & `tmp/pyqcm-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqcm-2.5.1.tar", last modified: Thu Mar 28 17:17:58 2024, max compression
+gzip compressed data, was "pyqcm-2.5.2.tar", last modified: Wed Apr  3 21:30:03 2024, max compression
```

## Comparing `pyqcm-2.5.1.tar` & `pyqcm-2.5.2.tar`

### file list

```diff
@@ -1,327 +1,327 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 17:17:58.803934 pyqcm-2.5.1/
--rw-rw-rw-   0 root         (0) root         (0)      131 2024-03-28 17:17:49.000000 pyqcm-2.5.1/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      427 2024-03-28 17:17:49.000000 pyqcm-2.5.1/.readthedocs.yaml
--rw-rw-rw-   0 root         (0) root         (0)    11718 2024-03-28 17:17:49.000000 pyqcm-2.5.1/CMakeLists.txt
--rw-rw-rw-   0 root         (0) root         (0)     5088 2024-03-28 17:17:49.000000 pyqcm-2.5.1/INSTALL.md
--rw-rw-rw-   0 root         (0) root         (0)    35216 2024-03-28 17:17:49.000000 pyqcm-2.5.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)     2773 2024-03-28 17:17:58.803934 pyqcm-2.5.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2467 2024-03-28 17:17:49.000000 pyqcm-2.5.1/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 17:17:58.779934 pyqcm-2.5.1/bench/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 17:17:58.779934 pyqcm-2.5.1/bench/ED/
--rw-rw-rw-   0 root         (0) root         (0)      693 2024-03-28 17:17:49.000000 pyqcm-2.5.1/bench/ED/bench_ED.py
--rw-rw-rw-   0 root         (0) root         (0)      940 2024-03-28 17:17:49.000000 pyqcm-2.5.1/bench/ED/bench_ED2.py
--rw-rw-rw-   0 root         (0) root         (0)      268 2024-03-28 17:17:49.000000 pyqcm-2.5.1/bench/ED/bench_ED2_laptop.txt
--rw-rw-rw-   0 root         (0) root         (0)      862 2024-03-28 17:17:49.000000 pyqcm-2.5.1/bench/ED/bench_GS.py
--rw-rw-rw-   0 root         (0) root         (0)     1437 2024-03-28 17:17:49.000000 pyqcm-2.5.1/bench/ED/bench_GS2.py
--rw-rw-rw-   0 root         (0) root         (0)     1088 2024-03-28 17:17:49.000000 pyqcm-2.5.1/bench/ED/bench_GS_loop.py
--rw-rw-rw-   0 root         (0) root         (0)     1261 2024-03-28 17:17:49.000000 pyqcm-2.5.1/bench/ED/model_1D.py
--rw-rw-rw-   0 root         (0) root         (0)      751 2024-03-28 17:17:49.000000 pyqcm-2.5.1/bench/ED/model_2D.py
--rw-rw-rw-   0 root         (0) root         (0)     1017 2024-03-28 17:17:49.000000 pyqcm-2.5.1/bench/ED/plot_bench_ED.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 17:17:58.779934 pyqcm-2.5.1/bench/integrals/
--rw-rw-rw-   0 root         (0) root         (0)     1062 2024-03-28 17:17:49.000000 pyqcm-2.5.1/bench/integrals/plot_concurrent.py
--rw-rw-rw-   0 root         (0) root         (0)     1091 2024-03-28 17:17:49.000000 pyqcm-2.5.1/bench/integrals/plot_integrals.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 17:17:58.779934 pyqcm-2.5.1/bench/integrals/small/
--rw-rw-rw-   0 root         (0) root         (0)      324 2024-03-28 17:17:49.000000 pyqcm-2.5.1/bench/integrals/small/integrals_small.py
--rw-rw-rw-   0 root         (0) root         (0)      396 2024-03-28 17:17:49.000000 pyqcm-2.5.1/bench/integrals/small/integrals_small_concurrent.txt
--rw-rw-rw-   0 root         (0) root         (0)      266 2024-03-28 17:17:49.000000 pyqcm-2.5.1/bench/integrals/small/integrals_small_results.txt
--rw-rw-rw-   0 root         (0) root         (0)      533 2024-03-28 17:17:49.000000 pyqcm-2.5.1/bench/integrals/small/model_small.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 17:17:58.779934 pyqcm-2.5.1/bench/vca/
--rw-rw-rw-   0 root         (0) root         (0)     1738 2024-03-28 17:17:49.000000 pyqcm-2.5.1/bench/vca/bench_vca.py
--rw-rw-rw-   0 root         (0) root         (0)     2022 2024-03-28 17:17:49.000000 pyqcm-2.5.1/bench/vca/bench_vca2.py
--rw-rw-rw-   0 root         (0) root         (0)      276 2024-03-28 17:17:49.000000 pyqcm-2.5.1/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 17:17:58.779934 pyqcm-2.5.1/docs/
--rwxrwxrwx   0 root         (0) root         (0)      623 2024-03-28 17:17:49.000000 pyqcm-2.5.1/docs/Makefile
--rwxrwxrwx   0 root         (0) root         (0)      134 2024-03-28 17:17:49.000000 pyqcm-2.5.1/docs/makedoc
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 17:17:58.783934 pyqcm-2.5.1/docs/source/
--rwxrwxrwx   0 root         (0) root         (0)     7924 2024-03-28 17:17:49.000000 pyqcm-2.5.1/docs/source/2x2.png
--rwxrwxrwx   0 root         (0) root         (0)    65032 2024-03-28 17:17:49.000000 pyqcm-2.5.1/docs/source/T6.png
--rwxrwxrwx   0 root         (0) root         (0)      917 2024-03-28 17:17:49.000000 pyqcm-2.5.1/docs/source/cdmft.rst
--rwxrwxrwx   0 root         (0) root         (0)     5631 2024-03-28 17:17:49.000000 pyqcm-2.5.1/docs/source/conf.py
--rw-rw-rw-   0 root         (0) root         (0)     5720 2024-03-28 17:17:49.000000 pyqcm-2.5.1/docs/source/defining_cluster_models.rst
--rwxrwxrwx   0 root         (0) root         (0)     9560 2024-03-28 17:17:49.000000 pyqcm-2.5.1/docs/source/defining_models.rst
--rwxrwxrwx   0 root         (0) root         (0)    37228 2024-03-28 17:17:49.000000 pyqcm-2.5.1/docs/source/h4-6b.png
--rwxrwxrwx   0 root         (0) root         (0)     1265 2024-03-28 17:17:49.000000 pyqcm-2.5.1/docs/source/h8.asy
--rw-rw-rw-   0 root         (0) root         (0)    57104 2024-03-28 17:17:49.000000 pyqcm-2.5.1/docs/source/h8.png
--rw-rw-rw-   0 root         (0) root         (0)     1935 2024-03-28 17:17:49.000000 pyqcm-2.5.1/docs/source/hartree.rst
--rwxrwxrwx   0 root         (0) root         (0)    66076 2024-03-28 17:17:49.000000 pyqcm-2.5.1/docs/source/hexa6.png
--rwxrwxrwx   0 root         (0) root         (0)      579 2024-03-28 17:17:49.000000 pyqcm-2.5.1/docs/source/index.rst
--rwxrwxrwx   0 root         (0) root         (0)     5217 2024-03-28 17:17:49.000000 pyqcm-2.5.1/docs/source/intro.rst
--rwxrwxrwx   0 root         (0) root         (0)    18237 2024-03-28 17:17:49.000000 pyqcm-2.5.1/docs/source/models.rst
--rw-rw-rw-   0 root         (0) root         (0)     6033 2024-03-28 17:17:49.000000 pyqcm-2.5.1/docs/source/options.rst
--rwxrwxrwx   0 root         (0) root         (0)      782 2024-03-28 17:17:49.000000 pyqcm-2.5.1/docs/source/options_intro.txt
--rwxrwxrwx   0 root         (0) root         (0)      236 2024-03-28 17:17:49.000000 pyqcm-2.5.1/docs/source/other_functions.rst
--rwxrwxrwx   0 root         (0) root         (0)     6231 2024-03-28 17:17:49.000000 pyqcm-2.5.1/docs/source/parallel.rst
--rw-rw-rw-   0 root         (0) root         (0)    23261 2024-03-28 17:17:49.000000 pyqcm-2.5.1/docs/source/parallel_performance_concurrent.png
--rw-rw-rw-   0 root         (0) root         (0)    23202 2024-03-28 17:17:49.000000 pyqcm-2.5.1/docs/source/parallel_performance_ed.png
--rw-rw-rw-   0 root         (0) root         (0)    34896 2024-03-28 17:17:49.000000 pyqcm-2.5.1/docs/source/parallel_performance_integrals.png
--rwxrwxrwx   0 root         (0) root         (0)     8130 2024-03-28 17:17:49.000000 pyqcm-2.5.1/docs/source/parameters.rst
--rw-rw-rw-   0 root         (0) root         (0)    43029 2024-03-28 17:17:49.000000 pyqcm-2.5.1/docs/source/t15.png
--rwxrwxrwx   0 root         (0) root         (0)      535 2024-03-28 17:17:49.000000 pyqcm-2.5.1/docs/source/vca.rst
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 17:17:58.779934 pyqcm-2.5.1/examples/
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 17:17:58.783934 pyqcm-2.5.1/examples/1D_2_4b/
--rw-rw-rw-   0 root         (0) root         (0)       95 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_2_4b/QCM_params.def
--rw-rw-rw-   0 root         (0) root         (0)   116475 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_2_4b/averages.tsv
--rw-rw-rw-   0 root         (0) root         (0)    37866 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_2_4b/cdmft.tsv
--rw-rw-rw-   0 root         (0) root         (0)     2620 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_2_4b/cdmft_distance.tsv
--rw-rw-rw-   0 root         (0) root         (0)   114242 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_2_4b/cdmft_grid.tsv
--rw-rw-rw-   0 root         (0) root         (0)   548325 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_2_4b/cdmft_iter.tsv
--rw-rw-rw-   0 root         (0) root         (0)      679 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_2_4b/debug.py
--rw-rw-rw-   0 root         (0) root         (0)      797 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_2_4b/debug_complex.py
--rw-rw-rw-   0 root         (0) root         (0)      540 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_2_4b/debug_dvmc.py
--rw-rw-rw-   0 root         (0) root         (0)      666 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_2_4b/debug_variable_parameter.py
--rw-rw-rw-   0 root         (0) root         (0)    20439 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_2_4b/dos.tsv
--rw-rw-rw-   0 root         (0) root         (0)    17095 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_2_4b/h1.pdf
--rw-rw-rw-   0 root         (0) root         (0)    35032 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_2_4b/h2.pdf
--rw-rw-rw-   0 root         (0) root         (0)      704 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_2_4b/hop.npy
--rw-rw-rw-   0 root         (0) root         (0)      318 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_2_4b/hopping.def
--rw-rw-rw-   0 root         (0) root         (0)       16 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_2_4b/interaction.def
--rw-rw-rw-   0 root         (0) root         (0)      176 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_2_4b/interaction.npy
--rwxrwxrwx   0 root         (0) root         (0)     2491 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_2_4b/model_1D_2_4b.py
--rw-rw-rw-   0 root         (0) root         (0)    10812 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_2_4b/out
--rw-rw-rw-   0 root         (0) root         (0)    20251 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_2_4b/s1.pdf
--rw-rw-rw-   0 root         (0) root         (0)    21433 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_2_4b/s2.pdf
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 17:17:58.787934 pyqcm-2.5.1/examples/1D_4/
--rw-rw-rw-   0 root         (0) root         (0)     3185 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_4/GS.tsv
--rw-rw-rw-   0 root         (0) root         (0)    18259 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_4/ave.tsv
--rw-rw-rw-   0 root         (0) root         (0)    18259 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_4/averages.tsv
--rw-rw-rw-   0 root         (0) root         (0)      287 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_4/debug.py
--rw-rw-rw-   0 root         (0) root         (0)     1269 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_4/debug_cdw.py
--rw-rw-rw-   0 root         (0) root         (0)      244 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_4/debug_dvmc.py
--rw-rw-rw-   0 root         (0) root         (0)     1971 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_4/debug_rhoAB.py
--rw-rw-rw-   0 root         (0) root         (0)    11556 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_4/hartree.tsv
--rwxrwxrwx   0 root         (0) root         (0)     1572 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_4/model_1D_4.py
--rw-rw-rw-   0 root         (0) root         (0)      467 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_4/model_1D_4_C2.py
--rw-rw-rw-   0 root         (0) root         (0)     3315 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_4/record.py
--rw-rw-rw-   0 root         (0) root         (0)  1077770 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_4/sef.tsv
--rw-rw-rw-   0 root         (0) root         (0)    29277 2024-03-28 17:17:49.000000 pyqcm-2.5.1/examples/1D_4/vca.tsv
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 17:17:58.787934 pyqcm-2.5.1/external/
--rw-rw-rw-   0 root         (0) root         (0)     1639 2024-03-28 17:17:49.000000 pyqcm-2.5.1/external/FindAVX2.cmake
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 17:17:58.787934 pyqcm-2.5.1/notebooks/
--rw-rw-rw-   0 root         (0) root         (0)    21298 2024-03-28 17:17:49.000000 pyqcm-2.5.1/notebooks/AF_VCA_vs_L.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     1742 2024-03-28 17:17:49.000000 pyqcm-2.5.1/notebooks/AF_VCA_vs_L.py
--rw-rw-rw-   0 root         (0) root         (0)   188540 2024-03-28 17:17:49.000000 pyqcm-2.5.1/notebooks/CDW_1D.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     4051 2024-03-28 17:17:49.000000 pyqcm-2.5.1/notebooks/CDW_1D.py
--rw-rw-rw-   0 root         (0) root         (0)     9942 2024-03-28 17:17:49.000000 pyqcm-2.5.1/notebooks/Mott_Weyl.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     4186 2024-03-28 17:17:49.000000 pyqcm-2.5.1/notebooks/Mott_Weyl.py
--rw-rw-rw-   0 root         (0) root         (0)     8976 2024-03-28 17:17:49.000000 pyqcm-2.5.1/notebooks/Mott_transition_graphene_CDMFT.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     4928 2024-03-28 17:17:49.000000 pyqcm-2.5.1/notebooks/Mott_transition_graphene_CDMFT.py
--rw-rw-rw-   0 root         (0) root         (0)     6067 2024-03-28 17:17:49.000000 pyqcm-2.5.1/notebooks/Rashba_coupling.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     2616 2024-03-28 17:17:49.000000 pyqcm-2.5.1/notebooks/Rashba_coupling.py
--rw-rw-rw-   0 root         (0) root         (0)     9414 2024-03-28 17:17:49.000000 pyqcm-2.5.1/notebooks/antiferromagnetism_VCA.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     6699 2024-03-28 17:17:49.000000 pyqcm-2.5.1/notebooks/antiferromagnetism_VCA.py
--rw-rw-rw-   0 root         (0) root         (0)   216639 2024-03-28 17:17:49.000000 pyqcm-2.5.1/notebooks/dimerization_1D.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     1486 2024-03-28 17:17:49.000000 pyqcm-2.5.1/notebooks/dimerization_1D.py
--rw-rw-rw-   0 root         (0) root         (0)     2875 2024-03-28 17:17:49.000000 pyqcm-2.5.1/notebooks/intro1.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     1727 2024-03-28 17:17:49.000000 pyqcm-2.5.1/notebooks/intro1.py
--rw-rw-rw-   0 root         (0) root         (0)     3139 2024-03-28 17:17:49.000000 pyqcm-2.5.1/notebooks/intro2.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     1834 2024-03-28 17:17:49.000000 pyqcm-2.5.1/notebooks/intro2.py
--rw-rw-rw-   0 root         (0) root         (0)     3696 2024-03-28 17:17:49.000000 pyqcm-2.5.1/notebooks/intro3.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     2310 2024-03-28 17:17:49.000000 pyqcm-2.5.1/notebooks/intro3.py
--rw-rw-rw-   0 root         (0) root         (0)     3395 2024-03-28 17:17:49.000000 pyqcm-2.5.1/notebooks/periodic_cluster.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     1780 2024-03-28 17:17:49.000000 pyqcm-2.5.1/notebooks/periodic_cluster.py
--rw-rw-rw-   0 root         (0) root         (0)     6472 2024-03-28 17:17:49.000000 pyqcm-2.5.1/notebooks/superconductivity_VCA.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     2237 2024-03-28 17:17:49.000000 pyqcm-2.5.1/notebooks/superconductivity_VCA.py
--rw-rw-rw-   0 root         (0) root         (0)      419 2024-03-28 17:17:49.000000 pyqcm-2.5.1/print_version.py
--rw-rw-rw-   0 root         (0) root         (0)      202 2024-03-28 17:17:49.000000 pyqcm-2.5.1/pyproject.toml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 17:17:58.791934 pyqcm-2.5.1/pyqcm/
--rw-rw-rw-   0 root         (0) root         (0)     3647 2024-03-28 17:17:49.000000 pyqcm-2.5.1/pyqcm/Kolmogorov_Smirnov.py
--rwxrwxrwx   0 root         (0) root         (0)    89530 2024-03-28 17:17:49.000000 pyqcm-2.5.1/pyqcm/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    16492 2024-03-28 17:17:49.000000 pyqcm-2.5.1/pyqcm/_draw.py
--rw-rw-rw-   0 root         (0) root         (0)    18464 2024-03-28 17:17:49.000000 pyqcm-2.5.1/pyqcm/_loop.py
--rwxrwxrwx   0 root         (0) root         (0)    73917 2024-03-28 17:17:49.000000 pyqcm-2.5.1/pyqcm/_spectral.py
--rw-rw-rw-   0 root         (0) root         (0)    56083 2024-03-28 17:17:49.000000 pyqcm-2.5.1/pyqcm/cdmft.py
--rw-rw-rw-   0 root         (0) root         (0)    19152 2024-03-28 17:17:49.000000 pyqcm-2.5.1/pyqcm/cdw.py
--rw-rw-rw-   0 root         (0) root         (0)     8979 2024-03-28 17:17:49.000000 pyqcm-2.5.1/pyqcm/dca.py
--rw-rw-rw-   0 root         (0) root         (0)     2047 2024-03-28 17:17:49.000000 pyqcm-2.5.1/pyqcm/external.py
--rw-rw-rw-   0 root         (0) root         (0)       40 2024-03-28 17:17:58.000000 pyqcm-2.5.1/pyqcm/qcm_git_hash.py
--rw-rw-rw-   0 root         (0) root         (0)     4314 2024-03-28 17:17:49.000000 pyqcm-2.5.1/pyqcm/slab.py
--rw-rw-rw-   0 root         (0) root         (0)     5806 2024-03-28 17:17:49.000000 pyqcm-2.5.1/pyqcm/variable_parameter.py
--rw-rw-rw-   0 root         (0) root         (0)    39526 2024-03-28 17:17:49.000000 pyqcm-2.5.1/pyqcm/vca.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 17:17:58.791934 pyqcm-2.5.1/pyqcm.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     2773 2024-03-28 17:17:58.000000 pyqcm-2.5.1/pyqcm.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     8580 2024-03-28 17:17:58.000000 pyqcm-2.5.1/pyqcm.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-03-28 17:17:58.000000 pyqcm-2.5.1/pyqcm.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-03-28 17:17:58.000000 pyqcm-2.5.1/pyqcm.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        6 2024-03-28 17:17:58.000000 pyqcm-2.5.1/pyqcm.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)       23 2024-03-28 17:17:49.000000 pyqcm-2.5.1/requirements.txt
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-03-28 17:17:58.803934 pyqcm-2.5.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1587 2024-03-28 17:17:49.000000 pyqcm-2.5.1/setup.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 17:17:58.791934 pyqcm-2.5.1/src_ed/
--rw-rw-rw-   0 root         (0) root         (0)     1288 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/.clang-format
--rw-rw-rw-   0 root         (0) root         (0)   108593 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Doxyfile
--rw-rw-rw-   0 root         (0) root         (0)    12658 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/ED_basis.cpp
--rw-rw-rw-   0 root         (0) root         (0)     3338 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/ED_basis.hpp
--rw-rw-rw-   0 root         (0) root         (0)     1134 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Green_function_set.hpp
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 17:17:58.791934 pyqcm-2.5.1/src_ed/Hamiltonian/
--rw-rw-rw-   0 root         (0) root         (0)     2473 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Hamiltonian/CSR_hermitian.hpp
--rw-rw-rw-   0 root         (0) root         (0)     6351 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Hamiltonian/Davidson.hpp
--rw-rw-rw-   0 root         (0) root         (0)     3925 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Hamiltonian/Hamiltonian_CSR.hpp
--rw-rw-rw-   0 root         (0) root         (0)     5826 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Hamiltonian/Hamiltonian_Dense.hpp
--rw-rw-rw-   0 root         (0) root         (0)     3826 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Hamiltonian/Hamiltonian_Eigen.hpp
--rw-rw-rw-   0 root         (0) root         (0)     2343 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Hamiltonian/Hamiltonian_Factorized.hpp
--rw-rw-rw-   0 root         (0) root         (0)     1744 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Hamiltonian/Hamiltonian_OnTheFly.hpp
--rw-rw-rw-   0 root         (0) root         (0)     2558 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Hamiltonian/Hamiltonian_Operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     8025 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Hamiltonian/Hamiltonian_base.hpp
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Hamiltonian/Hamiltonian_ops.hpp
--rw-rw-rw-   0 root         (0) root         (0)     1654 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Hamiltonian/Lanczos.cpp
--rw-rw-rw-   0 root         (0) root         (0)    12662 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Hamiltonian/Lanczos.hpp
--rw-rw-rw-   0 root         (0) root         (0)      487 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Hamiltonian/PRIMME_solver.cpp
--rw-rw-rw-   0 root         (0) root         (0)     5263 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Hamiltonian/PRIMME_solver.hpp
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 17:17:58.795934 pyqcm-2.5.1/src_ed/Operators/
--rw-rw-rw-   0 root         (0) root         (0)     4737 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Operators/HS_Heisenberg_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     2054 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Operators/HS_Hermitian_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     2230 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Operators/HS_Hund_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     2073 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Operators/HS_anomalous_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     4076 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Operators/HS_factorized_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     2452 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Operators/HS_general_interaction_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     2640 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Operators/HS_half_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     3816 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Operators/HS_interaction_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     6854 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Operators/HS_nondiagonal_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     2107 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Operators/HS_one_body_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     1598 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Operators/HS_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     2592 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Operators/Heisenberg_operator.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1354 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Operators/Heisenberg_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     3757 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Operators/Hermitian_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     2485 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Operators/Hund_operator.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1212 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Operators/Hund_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)    13374 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Operators/anomalous_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     1956 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Operators/destruction_operator.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1963 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Operators/destruction_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     4497 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Operators/general_interaction_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     5113 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Operators/interaction_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)    16552 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Operators/one_body_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)     8220 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Q_matrix.hpp
--rw-rw-rw-   0 root         (0) root         (0)     4798 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/Q_matrix_set.hpp
--rw-rw-rw-   0 root         (0) root         (0)     4156 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/binary_state.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2305 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/binary_state.hpp
--rw-rw-rw-   0 root         (0) root         (0)     1854 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/continued_fraction.cpp
--rw-rw-rw-   0 root         (0) root         (0)      731 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/continued_fraction.hpp
--rw-rw-rw-   0 root         (0) root         (0)     5328 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/continued_fraction_set.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1041 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/continued_fraction_set.hpp
--rw-rw-rw-   0 root         (0) root         (0)     2195 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/flex_array.hpp
--rw-rw-rw-   0 root         (0) root         (0)      791 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/fraction.hpp
--rw-rw-rw-   0 root         (0) root         (0)     2034 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/index.hpp
--rw-rw-rw-   0 root         (0) root         (0)      784 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/index_pair.hpp
--rw-rw-rw-   0 root         (0) root         (0)     1296 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/matrix_element.hpp
--rw-rw-rw-   0 root         (0) root         (0)     9564 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/model.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2667 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/model.hpp
--rw-rw-rw-   0 root         (0) root         (0)     8222 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/model_instance.cpp
--rw-rw-rw-   0 root         (0) root         (0)    43555 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/model_instance.hpp
--rw-rw-rw-   0 root         (0) root         (0)     5566 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/model_instance_base.cpp
--rw-rw-rw-   0 root         (0) root         (0)     3655 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/model_instance_base.hpp
--rw-rw-rw-   0 root         (0) root         (0)    13893 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/qcm_ED.cpp
--rw-rw-rw-   0 root         (0) root         (0)    10059 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/qcm_ED.hpp
--rw-rw-rw-   0 root         (0) root         (0)      788 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/sector.cpp
--rw-rw-rw-   0 root         (0) root         (0)     3979 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/sector.hpp
--rw-rw-rw-   0 root         (0) root         (0)     1620 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/sparse_matrix.hpp
--rw-rw-rw-   0 root         (0) root         (0)     3017 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/state.hpp
--rw-rw-rw-   0 root         (0) root         (0)     1674 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/symmetric_orbital.hpp
--rw-rw-rw-   0 root         (0) root         (0)    18543 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/symmetry_group.cpp
--rw-rw-rw-   0 root         (0) root         (0)     5610 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_ed/symmetry_group.hpp
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 17:17:58.795934 pyqcm-2.5.1/src_python/
--rw-rw-rw-   0 root         (0) root         (0)    12457 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_python/common_Py.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1395 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_python/common_Py.hpp
--rw-rw-rw-   0 root         (0) root         (0)     5230 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_python/qcm_ED_lib.cpp
--rw-rw-rw-   0 root         (0) root         (0)      721 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_python/qcm_ED_only.hpp
--rw-rw-rw-   0 root         (0) root         (0)    37936 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_python/qcm_ED_wrap.hpp
--rw-rw-rw-   0 root         (0) root         (0)    11030 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_python/qcm_lib.cpp
--rwxrwxrwx   0 root         (0) root         (0)    79768 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_python/qcm_wrap.hpp
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 17:17:58.795934 pyqcm-2.5.1/src_qcm/
--rwxrwxrwx   0 root         (0) root         (0)    12342 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_qcm/CPT.cpp
--rwxrwxrwx   0 root         (0) root         (0)    12499 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_qcm/Chern.cpp
--rwxrwxrwx   0 root         (0) root         (0)   108585 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_qcm/Doxyfile
--rwxrwxrwx   0 root         (0) root         (0)     1556 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_qcm/Green_function.hpp
--rwxrwxrwx   0 root         (0) root         (0)    32998 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_qcm/QCM.cpp
--rwxrwxrwx   0 root         (0) root         (0)     6294 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_qcm/QCM.hpp
--rwxrwxrwx   0 root         (0) root         (0)    16971 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_qcm/average.cpp
--rwxrwxrwx   0 root         (0) root         (0)     3401 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_qcm/basis3D.cpp
--rwxrwxrwx   0 root         (0) root         (0)     1033 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_qcm/basis3D.hpp
--rwxrwxrwx   0 root         (0) root         (0)     5745 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_qcm/lattice3D.cpp
--rwxrwxrwx   0 root         (0) root         (0)     1212 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_qcm/lattice3D.hpp
--rwxrwxrwx   0 root         (0) root         (0)     2892 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_qcm/lattice_matrix_element.hpp
--rwxrwxrwx   0 root         (0) root         (0)    39191 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_qcm/lattice_model.cpp
--rwxrwxrwx   0 root         (0) root         (0)     9353 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_qcm/lattice_model.hpp
--rwxrwxrwx   0 root         (0) root         (0)    22767 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_qcm/lattice_model_instance.cpp
--rwxrwxrwx   0 root         (0) root         (0)     5941 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_qcm/lattice_model_instance.hpp
--rwxrwxrwx   0 root         (0) root         (0)     8228 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_qcm/lattice_operator.cpp
--rwxrwxrwx   0 root         (0) root         (0)     2751 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_qcm/lattice_operator.hpp
--rw-rw-rw-   0 root         (0) root         (0)    16126 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_qcm/omp.h
--rwxrwxrwx   0 root         (0) root         (0)     6655 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_qcm/parameter_set.cpp
--rwxrwxrwx   0 root         (0) root         (0)     1611 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_qcm/parameter_set.hpp
--rwxrwxrwx   0 root         (0) root         (0)    12256 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_qcm/print.cpp
--rwxrwxrwx   0 root         (0) root         (0)     5341 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_qcm/profile.cpp
--rwxrwxrwx   0 root         (0) root         (0)     7224 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_qcm/vector3D.hpp
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 17:17:58.799934 pyqcm-2.5.1/src_util/
--rw-rw-rw-   0 root         (0) root         (0)     9275 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_util/ED_global_parameter.cpp
--rw-rw-rw-   0 root         (0) root         (0)    10036 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_util/VDVH_kernel.cpp
--rw-rw-rw-   0 root         (0) root         (0)     1469 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_util/VDVH_kernel.hpp
--rw-rw-rw-   0 root         (0) root         (0)     7156 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_util/block_matrix.hpp
--rw-rw-rw-   0 root         (0) root         (0)    47325 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_util/cblas.h
--rw-rw-rw-   0 root         (0) root         (0)   263401 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_util/clapack.h
--rw-rw-rw-   0 root         (0) root         (0)    13424 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_util/f2c.h
--rwxrwxrwx   0 root         (0) root         (0)     6941 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_util/global_parameter.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2650 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_util/global_parameter.hpp
--rwxrwxrwx   0 root         (0) root         (0)    24433 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_util/integrate.cpp
--rwxrwxrwx   0 root         (0) root         (0)     5770 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_util/integrate.hpp
--rw-rw-rw-   0 root         (0) root         (0)      124 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_util/lapack-blas.h
--rw-rw-rw-   0 root         (0) root         (0)     7187 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_util/matrix.cpp
--rw-rw-rw-   0 root         (0) root         (0)    20538 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_util/matrix.hpp
--rw-rw-rw-   0 root         (0) root         (0)     6702 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_util/parser.cpp
--rw-rw-rw-   0 root         (0) root         (0)     2395 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_util/parser.hpp
--rw-rw-rw-   0 root         (0) root         (0)      828 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_util/types.hpp
--rw-rw-rw-   0 root         (0) root         (0)     4354 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_util/vector_num.cpp
--rw-rw-rw-   0 root         (0) root         (0)     5978 2024-03-28 17:17:49.000000 pyqcm-2.5.1/src_util/vector_num.hpp
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 17:17:58.799934 pyqcm-2.5.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)      489 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1124 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_all.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 17:17:58.799934 pyqcm-2.5.1/tests/test_diagonalization/
--rw-rw-rw-   0 root         (0) root         (0)    27349 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_diagonalization/S_format.ref
--rw-rw-rw-   0 root         (0) root         (0)     2575 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_diagonalization/S_format_complex.ref
--rw-rw-rw-   0 root         (0) root         (0)     1341 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_diagonalization/cluster_2x2_2C_8b_C2v_L.py
--rw-rw-rw-   0 root         (0) root         (0)      684 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_diagonalization/common.py
--rw-rw-rw-   0 root         (0) root         (0)      566 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_diagonalization/model_1D_8.py
--rw-rw-rw-   0 root         (0) root         (0)     1608 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_diagonalization/model_2x2_2C_8b_C2v_L.py
--rw-rw-rw-   0 root         (0) root         (0)     2370 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_diagonalization/test_pole_distribution.py
--rw-rw-rw-   0 root         (0) root         (0)     1002 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_diagonalization/test_pole_distribution_complex.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-03-28 17:17:58.803934 pyqcm-2.5.1/tests/test_files/
--rw-rw-rw-   0 root         (0) root         (0)     1290 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/model_1D.py
--rw-rw-rw-   0 root         (0) root         (0)     1281 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/model_1D_2.py
--rw-rw-rw-   0 root         (0) root         (0)     2712 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/model_1D_2_4b.py
--rwxrwxrwx   0 root         (0) root         (0)     1297 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/model_1D_4.py
--rw-rw-rw-   0 root         (0) root         (0)      952 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/model_1D_4_C2.py
--rwxrwxrwx   0 root         (0) root         (0)     1220 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/model_2x2_C2.py
--rw-rw-rw-   0 root         (0) root         (0)     1198 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/model_2x2_C2_vca.py
--rw-rw-rw-   0 root         (0) root         (0)     1320 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/model_G4_6b_2C.py
--rw-rw-rw-   0 root         (0) root         (0)      751 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/model_WSM.py
--rw-rw-rw-   0 root         (0) root         (0)     2064 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/model_graphene_bath.py
--rw-rw-rw-   0 root         (0) root         (0)      833 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/model_hartree.py
--rw-rw-rw-   0 root         (0) root         (0)     4846 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/record_2x2.py
--rw-rw-rw-   0 root         (0) root         (0)     8484 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/record_2x2_8b.py
--rw-rw-rw-   0 root         (0) root         (0)   108854 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/record_2x2_anom.py
--rw-rw-rw-   0 root         (0) root         (0)    19410 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/record_WSM.py
--rw-rw-rw-   0 root         (0) root         (0)   208082 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/record_WSM2.py
--rw-rw-rw-   0 root         (0) root         (0)     5989 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/record_spin.py
--rw-rw-rw-   0 root         (0) root         (0)     2359 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/test_2clusters.py
--rw-rw-rw-   0 root         (0) root         (0)     1496 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/test_CF.py
--rw-rw-rw-   0 root         (0) root         (0)      937 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/test_averages.py
--rw-rw-rw-   0 root         (0) root         (0)      471 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/test_averages_bath.py
--rw-rw-rw-   0 root         (0) root         (0)     1995 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/test_berry.py
--rw-rw-rw-   0 root         (0) root         (0)     1275 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/test_cdmft.py
--rw-rw-rw-   0 root         (0) root         (0)     1293 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/test_cdmft_hartree.py
--rw-rw-rw-   0 root         (0) root         (0)      638 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/test_cluster_average.py
--rw-rw-rw-   0 root         (0) root         (0)      954 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/test_controlled_loop.py
--rw-rw-rw-   0 root         (0) root         (0)      893 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/test_draw.py
--rw-rw-rw-   0 root         (0) root         (0)     1427 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/test_fidelity.py
--rw-rw-rw-   0 root         (0) root         (0)      726 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/test_fixed_density_loop.py
--rw-rw-rw-   0 root         (0) root         (0)     1845 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/test_hartree.py
--rw-rw-rw-   0 root         (0) root         (0)      359 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/test_hybridization.py
--rw-rw-rw-   0 root         (0) root         (0)      433 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/test_instances.py
--rw-rw-rw-   0 root         (0) root         (0)     1149 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/test_mixing.py
--rw-rw-rw-   0 root         (0) root         (0)      897 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/test_mixing2.py
--rw-rw-rw-   0 root         (0) root         (0)     1197 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/test_mixing_cf.py
--rw-rw-rw-   0 root         (0) root         (0)     2431 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/test_reset.py
--rw-rw-rw-   0 root         (0) root         (0)     4290 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/test_spectral.py
--rw-rw-rw-   0 root         (0) root         (0)      475 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/test_varia.py
--rw-rw-rw-   0 root         (0) root         (0)     1982 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/test_vca.py
--rw-rw-rw-   0 root         (0) root         (0)      637 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/test_vca_MPI.py
--rw-rw-rw-   0 root         (0) root         (0)      528 2024-03-28 17:17:49.000000 pyqcm-2.5.1/tests/test_files/test_write.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.641532 pyqcm-2.5.2/
+-rw-rw-rw-   0 root         (0) root         (0)      131 2024-04-03 21:29:54.000000 pyqcm-2.5.2/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      427 2024-04-03 21:29:54.000000 pyqcm-2.5.2/.readthedocs.yaml
+-rw-rw-rw-   0 root         (0) root         (0)    11718 2024-04-03 21:29:54.000000 pyqcm-2.5.2/CMakeLists.txt
+-rw-rw-rw-   0 root         (0) root         (0)     5088 2024-04-03 21:29:54.000000 pyqcm-2.5.2/INSTALL.md
+-rw-rw-rw-   0 root         (0) root         (0)    35216 2024-04-03 21:29:54.000000 pyqcm-2.5.2/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)     2773 2024-04-03 21:30:03.641532 pyqcm-2.5.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2467 2024-04-03 21:29:54.000000 pyqcm-2.5.2/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.617531 pyqcm-2.5.2/bench/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.617531 pyqcm-2.5.2/bench/ED/
+-rw-rw-rw-   0 root         (0) root         (0)      693 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/ED/bench_ED.py
+-rw-rw-rw-   0 root         (0) root         (0)      940 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/ED/bench_ED2.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/ED/bench_ED2_laptop.txt
+-rw-rw-rw-   0 root         (0) root         (0)      862 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/ED/bench_GS.py
+-rw-rw-rw-   0 root         (0) root         (0)     1437 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/ED/bench_GS2.py
+-rw-rw-rw-   0 root         (0) root         (0)     1088 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/ED/bench_GS_loop.py
+-rw-rw-rw-   0 root         (0) root         (0)     1261 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/ED/model_1D.py
+-rw-rw-rw-   0 root         (0) root         (0)      751 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/ED/model_2D.py
+-rw-rw-rw-   0 root         (0) root         (0)     1017 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/ED/plot_bench_ED.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.617531 pyqcm-2.5.2/bench/integrals/
+-rw-rw-rw-   0 root         (0) root         (0)     1062 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/integrals/plot_concurrent.py
+-rw-rw-rw-   0 root         (0) root         (0)     1091 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/integrals/plot_integrals.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.617531 pyqcm-2.5.2/bench/integrals/small/
+-rw-rw-rw-   0 root         (0) root         (0)      324 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/integrals/small/integrals_small.py
+-rw-rw-rw-   0 root         (0) root         (0)      396 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/integrals/small/integrals_small_concurrent.txt
+-rw-rw-rw-   0 root         (0) root         (0)      266 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/integrals/small/integrals_small_results.txt
+-rw-rw-rw-   0 root         (0) root         (0)      533 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/integrals/small/model_small.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.617531 pyqcm-2.5.2/bench/vca/
+-rw-rw-rw-   0 root         (0) root         (0)     1738 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/vca/bench_vca.py
+-rw-rw-rw-   0 root         (0) root         (0)     2022 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bench/vca/bench_vca2.py
+-rw-rw-rw-   0 root         (0) root         (0)      276 2024-04-03 21:29:54.000000 pyqcm-2.5.2/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.621531 pyqcm-2.5.2/docs/
+-rwxrwxrwx   0 root         (0) root         (0)      623 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/Makefile
+-rwxrwxrwx   0 root         (0) root         (0)      134 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/makedoc
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.621531 pyqcm-2.5.2/docs/source/
+-rwxrwxrwx   0 root         (0) root         (0)     7924 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/2x2.png
+-rwxrwxrwx   0 root         (0) root         (0)    65032 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/T6.png
+-rwxrwxrwx   0 root         (0) root         (0)      917 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/cdmft.rst
+-rwxrwxrwx   0 root         (0) root         (0)     5631 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/conf.py
+-rw-rw-rw-   0 root         (0) root         (0)     5720 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/defining_cluster_models.rst
+-rwxrwxrwx   0 root         (0) root         (0)     9560 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/defining_models.rst
+-rwxrwxrwx   0 root         (0) root         (0)    37228 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/h4-6b.png
+-rwxrwxrwx   0 root         (0) root         (0)     1265 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/h8.asy
+-rw-rw-rw-   0 root         (0) root         (0)    57104 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/h8.png
+-rw-rw-rw-   0 root         (0) root         (0)     1935 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/hartree.rst
+-rwxrwxrwx   0 root         (0) root         (0)    66076 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/hexa6.png
+-rwxrwxrwx   0 root         (0) root         (0)      579 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/index.rst
+-rwxrwxrwx   0 root         (0) root         (0)     5217 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/intro.rst
+-rwxrwxrwx   0 root         (0) root         (0)    18237 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/models.rst
+-rw-rw-rw-   0 root         (0) root         (0)     6033 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/options.rst
+-rwxrwxrwx   0 root         (0) root         (0)      782 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/options_intro.txt
+-rwxrwxrwx   0 root         (0) root         (0)      236 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/other_functions.rst
+-rwxrwxrwx   0 root         (0) root         (0)     6231 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/parallel.rst
+-rw-rw-rw-   0 root         (0) root         (0)    23261 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/parallel_performance_concurrent.png
+-rw-rw-rw-   0 root         (0) root         (0)    23202 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/parallel_performance_ed.png
+-rw-rw-rw-   0 root         (0) root         (0)    34896 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/parallel_performance_integrals.png
+-rwxrwxrwx   0 root         (0) root         (0)     8130 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/parameters.rst
+-rw-rw-rw-   0 root         (0) root         (0)    43029 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/t15.png
+-rwxrwxrwx   0 root         (0) root         (0)      535 2024-04-03 21:29:54.000000 pyqcm-2.5.2/docs/source/vca.rst
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.617531 pyqcm-2.5.2/examples/
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.621531 pyqcm-2.5.2/examples/1D_2_4b/
+-rw-rw-rw-   0 root         (0) root         (0)       95 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/QCM_params.def
+-rw-rw-rw-   0 root         (0) root         (0)   116475 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/averages.tsv
+-rw-rw-rw-   0 root         (0) root         (0)    37866 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/cdmft.tsv
+-rw-rw-rw-   0 root         (0) root         (0)     2620 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/cdmft_distance.tsv
+-rw-rw-rw-   0 root         (0) root         (0)   114242 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/cdmft_grid.tsv
+-rw-rw-rw-   0 root         (0) root         (0)   548325 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/cdmft_iter.tsv
+-rw-rw-rw-   0 root         (0) root         (0)      679 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/debug.py
+-rw-rw-rw-   0 root         (0) root         (0)      797 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/debug_complex.py
+-rw-rw-rw-   0 root         (0) root         (0)      540 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/debug_dvmc.py
+-rw-rw-rw-   0 root         (0) root         (0)      666 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/debug_variable_parameter.py
+-rw-rw-rw-   0 root         (0) root         (0)    20439 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/dos.tsv
+-rw-rw-rw-   0 root         (0) root         (0)    17095 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/h1.pdf
+-rw-rw-rw-   0 root         (0) root         (0)    35032 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/h2.pdf
+-rw-rw-rw-   0 root         (0) root         (0)      704 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/hop.npy
+-rw-rw-rw-   0 root         (0) root         (0)      318 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/hopping.def
+-rw-rw-rw-   0 root         (0) root         (0)       16 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/interaction.def
+-rw-rw-rw-   0 root         (0) root         (0)      176 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/interaction.npy
+-rwxrwxrwx   0 root         (0) root         (0)     2491 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/model_1D_2_4b.py
+-rw-rw-rw-   0 root         (0) root         (0)    10812 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/out
+-rw-rw-rw-   0 root         (0) root         (0)    20251 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/s1.pdf
+-rw-rw-rw-   0 root         (0) root         (0)    21433 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_2_4b/s2.pdf
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.625532 pyqcm-2.5.2/examples/1D_4/
+-rw-rw-rw-   0 root         (0) root         (0)     3185 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_4/GS.tsv
+-rw-rw-rw-   0 root         (0) root         (0)    18259 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_4/ave.tsv
+-rw-rw-rw-   0 root         (0) root         (0)    18259 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_4/averages.tsv
+-rw-rw-rw-   0 root         (0) root         (0)      287 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_4/debug.py
+-rw-rw-rw-   0 root         (0) root         (0)     1269 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_4/debug_cdw.py
+-rw-rw-rw-   0 root         (0) root         (0)      244 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_4/debug_dvmc.py
+-rw-rw-rw-   0 root         (0) root         (0)     1971 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_4/debug_rhoAB.py
+-rw-rw-rw-   0 root         (0) root         (0)    11556 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_4/hartree.tsv
+-rwxrwxrwx   0 root         (0) root         (0)     1572 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_4/model_1D_4.py
+-rw-rw-rw-   0 root         (0) root         (0)      467 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_4/model_1D_4_C2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3315 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_4/record.py
+-rw-rw-rw-   0 root         (0) root         (0)  1077770 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_4/sef.tsv
+-rw-rw-rw-   0 root         (0) root         (0)    29277 2024-04-03 21:29:54.000000 pyqcm-2.5.2/examples/1D_4/vca.tsv
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.625532 pyqcm-2.5.2/external/
+-rw-rw-rw-   0 root         (0) root         (0)     1639 2024-04-03 21:29:54.000000 pyqcm-2.5.2/external/FindAVX2.cmake
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.625532 pyqcm-2.5.2/notebooks/
+-rw-rw-rw-   0 root         (0) root         (0)    21298 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/AF_VCA_vs_L.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     1742 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/AF_VCA_vs_L.py
+-rw-rw-rw-   0 root         (0) root         (0)   188540 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/CDW_1D.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     4051 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/CDW_1D.py
+-rw-rw-rw-   0 root         (0) root         (0)     9942 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/Mott_Weyl.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     4186 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/Mott_Weyl.py
+-rw-rw-rw-   0 root         (0) root         (0)     8976 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/Mott_transition_graphene_CDMFT.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     4928 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/Mott_transition_graphene_CDMFT.py
+-rw-rw-rw-   0 root         (0) root         (0)     6067 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/Rashba_coupling.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     2616 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/Rashba_coupling.py
+-rw-rw-rw-   0 root         (0) root         (0)     9414 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/antiferromagnetism_VCA.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     6699 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/antiferromagnetism_VCA.py
+-rw-rw-rw-   0 root         (0) root         (0)   216639 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/dimerization_1D.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     1486 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/dimerization_1D.py
+-rw-rw-rw-   0 root         (0) root         (0)     2875 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/intro1.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     1727 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/intro1.py
+-rw-rw-rw-   0 root         (0) root         (0)     3139 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/intro2.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     1834 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/intro2.py
+-rw-rw-rw-   0 root         (0) root         (0)     3696 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/intro3.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     2310 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/intro3.py
+-rw-rw-rw-   0 root         (0) root         (0)     3395 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/periodic_cluster.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     1780 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/periodic_cluster.py
+-rw-rw-rw-   0 root         (0) root         (0)     6472 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/superconductivity_VCA.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     2237 2024-04-03 21:29:54.000000 pyqcm-2.5.2/notebooks/superconductivity_VCA.py
+-rw-rw-rw-   0 root         (0) root         (0)      419 2024-04-03 21:29:54.000000 pyqcm-2.5.2/print_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      202 2024-04-03 21:29:54.000000 pyqcm-2.5.2/pyproject.toml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.629531 pyqcm-2.5.2/pyqcm/
+-rw-rw-rw-   0 root         (0) root         (0)     3647 2024-04-03 21:29:54.000000 pyqcm-2.5.2/pyqcm/Kolmogorov_Smirnov.py
+-rwxrwxrwx   0 root         (0) root         (0)    90393 2024-04-03 21:29:54.000000 pyqcm-2.5.2/pyqcm/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    16492 2024-04-03 21:29:54.000000 pyqcm-2.5.2/pyqcm/_draw.py
+-rw-rw-rw-   0 root         (0) root         (0)    18556 2024-04-03 21:29:54.000000 pyqcm-2.5.2/pyqcm/_loop.py
+-rwxrwxrwx   0 root         (0) root         (0)    73917 2024-04-03 21:29:54.000000 pyqcm-2.5.2/pyqcm/_spectral.py
+-rw-rw-rw-   0 root         (0) root         (0)    56083 2024-04-03 21:29:54.000000 pyqcm-2.5.2/pyqcm/cdmft.py
+-rw-rw-rw-   0 root         (0) root         (0)    19152 2024-04-03 21:29:54.000000 pyqcm-2.5.2/pyqcm/cdw.py
+-rw-rw-rw-   0 root         (0) root         (0)     8979 2024-04-03 21:29:54.000000 pyqcm-2.5.2/pyqcm/dca.py
+-rw-rw-rw-   0 root         (0) root         (0)     2047 2024-04-03 21:29:54.000000 pyqcm-2.5.2/pyqcm/external.py
+-rw-rw-rw-   0 root         (0) root         (0)       40 2024-04-03 21:30:03.000000 pyqcm-2.5.2/pyqcm/qcm_git_hash.py
+-rw-rw-rw-   0 root         (0) root         (0)     4314 2024-04-03 21:29:54.000000 pyqcm-2.5.2/pyqcm/slab.py
+-rw-rw-rw-   0 root         (0) root         (0)     5806 2024-04-03 21:29:54.000000 pyqcm-2.5.2/pyqcm/variable_parameter.py
+-rw-rw-rw-   0 root         (0) root         (0)    39560 2024-04-03 21:29:54.000000 pyqcm-2.5.2/pyqcm/vca.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.629531 pyqcm-2.5.2/pyqcm.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     2773 2024-04-03 21:30:03.000000 pyqcm-2.5.2/pyqcm.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     8580 2024-04-03 21:30:03.000000 pyqcm-2.5.2/pyqcm.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-03 21:30:03.000000 pyqcm-2.5.2/pyqcm.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-04-03 21:30:03.000000 pyqcm-2.5.2/pyqcm.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        6 2024-04-03 21:30:03.000000 pyqcm-2.5.2/pyqcm.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)       23 2024-04-03 21:29:54.000000 pyqcm-2.5.2/requirements.txt
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-03 21:30:03.641532 pyqcm-2.5.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1587 2024-04-03 21:29:54.000000 pyqcm-2.5.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.629531 pyqcm-2.5.2/src_ed/
+-rw-rw-rw-   0 root         (0) root         (0)     1288 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/.clang-format
+-rw-rw-rw-   0 root         (0) root         (0)   108593 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Doxyfile
+-rw-rw-rw-   0 root         (0) root         (0)    12658 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/ED_basis.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     3338 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/ED_basis.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     1134 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Green_function_set.hpp
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.633531 pyqcm-2.5.2/src_ed/Hamiltonian/
+-rw-rw-rw-   0 root         (0) root         (0)     2473 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Hamiltonian/CSR_hermitian.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     6351 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Hamiltonian/Davidson.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     3925 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_CSR.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     5826 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_Dense.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     3826 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_Eigen.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     2343 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_Factorized.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     1744 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_OnTheFly.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     2558 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_Operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     8025 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_base.hpp
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_ops.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     1654 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Hamiltonian/Lanczos.cpp
+-rw-rw-rw-   0 root         (0) root         (0)    12662 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Hamiltonian/Lanczos.hpp
+-rw-rw-rw-   0 root         (0) root         (0)      487 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Hamiltonian/PRIMME_solver.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     5263 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Hamiltonian/PRIMME_solver.hpp
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.633531 pyqcm-2.5.2/src_ed/Operators/
+-rw-rw-rw-   0 root         (0) root         (0)     4737 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/HS_Heisenberg_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     2054 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/HS_Hermitian_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     2230 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/HS_Hund_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     2073 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/HS_anomalous_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     4076 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/HS_factorized_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     2452 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/HS_general_interaction_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     2640 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/HS_half_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     3816 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/HS_interaction_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     6854 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/HS_nondiagonal_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     2107 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/HS_one_body_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     1598 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/HS_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     2592 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/Heisenberg_operator.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     1354 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/Heisenberg_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     3757 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/Hermitian_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     2485 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/Hund_operator.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     1212 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/Hund_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)    13374 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/anomalous_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     1956 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/destruction_operator.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     1963 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/destruction_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     4497 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/general_interaction_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     5113 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/interaction_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)    16552 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Operators/one_body_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     8220 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Q_matrix.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     4798 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/Q_matrix_set.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     4156 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/binary_state.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     2305 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/binary_state.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     1854 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/continued_fraction.cpp
+-rw-rw-rw-   0 root         (0) root         (0)      731 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/continued_fraction.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     5328 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/continued_fraction_set.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     1041 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/continued_fraction_set.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     2195 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/flex_array.hpp
+-rw-rw-rw-   0 root         (0) root         (0)      791 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/fraction.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     2034 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/index.hpp
+-rw-rw-rw-   0 root         (0) root         (0)      784 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/index_pair.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     1296 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/matrix_element.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     9564 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/model.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     2667 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/model.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     8222 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/model_instance.cpp
+-rw-rw-rw-   0 root         (0) root         (0)    43555 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/model_instance.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     5566 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/model_instance_base.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     3655 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/model_instance_base.hpp
+-rw-rw-rw-   0 root         (0) root         (0)    13893 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/qcm_ED.cpp
+-rw-rw-rw-   0 root         (0) root         (0)    10059 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/qcm_ED.hpp
+-rw-rw-rw-   0 root         (0) root         (0)      788 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/sector.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     3979 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/sector.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     1620 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/sparse_matrix.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     3017 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/state.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     1674 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/symmetric_orbital.hpp
+-rw-rw-rw-   0 root         (0) root         (0)    18543 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/symmetry_group.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     5610 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_ed/symmetry_group.hpp
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.633531 pyqcm-2.5.2/src_python/
+-rw-rw-rw-   0 root         (0) root         (0)    12457 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_python/common_Py.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     1395 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_python/common_Py.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     5230 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_python/qcm_ED_lib.cpp
+-rw-rw-rw-   0 root         (0) root         (0)      721 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_python/qcm_ED_only.hpp
+-rw-rw-rw-   0 root         (0) root         (0)    37936 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_python/qcm_ED_wrap.hpp
+-rw-rw-rw-   0 root         (0) root         (0)    11030 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_python/qcm_lib.cpp
+-rwxrwxrwx   0 root         (0) root         (0)    79768 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_python/qcm_wrap.hpp
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.637531 pyqcm-2.5.2/src_qcm/
+-rwxrwxrwx   0 root         (0) root         (0)    12342 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/CPT.cpp
+-rwxrwxrwx   0 root         (0) root         (0)    12499 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/Chern.cpp
+-rwxrwxrwx   0 root         (0) root         (0)   108585 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/Doxyfile
+-rwxrwxrwx   0 root         (0) root         (0)     1556 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/Green_function.hpp
+-rwxrwxrwx   0 root         (0) root         (0)    32998 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/QCM.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     6294 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/QCM.hpp
+-rwxrwxrwx   0 root         (0) root         (0)    16971 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/average.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     3401 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/basis3D.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     1033 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/basis3D.hpp
+-rwxrwxrwx   0 root         (0) root         (0)     5745 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/lattice3D.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     1212 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/lattice3D.hpp
+-rwxrwxrwx   0 root         (0) root         (0)     2892 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/lattice_matrix_element.hpp
+-rwxrwxrwx   0 root         (0) root         (0)    39191 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/lattice_model.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     9353 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/lattice_model.hpp
+-rwxrwxrwx   0 root         (0) root         (0)    22767 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/lattice_model_instance.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     5941 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/lattice_model_instance.hpp
+-rwxrwxrwx   0 root         (0) root         (0)     8228 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/lattice_operator.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     2751 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/lattice_operator.hpp
+-rw-rw-rw-   0 root         (0) root         (0)    16126 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/omp.h
+-rwxrwxrwx   0 root         (0) root         (0)     6655 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/parameter_set.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     1611 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/parameter_set.hpp
+-rwxrwxrwx   0 root         (0) root         (0)    12256 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/print.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     5341 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/profile.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     7224 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_qcm/vector3D.hpp
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.637531 pyqcm-2.5.2/src_util/
+-rw-rw-rw-   0 root         (0) root         (0)     9275 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/ED_global_parameter.cpp
+-rw-rw-rw-   0 root         (0) root         (0)    10036 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/VDVH_kernel.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     1469 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/VDVH_kernel.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     7156 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/block_matrix.hpp
+-rw-rw-rw-   0 root         (0) root         (0)    47325 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/cblas.h
+-rw-rw-rw-   0 root         (0) root         (0)   263401 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/clapack.h
+-rw-rw-rw-   0 root         (0) root         (0)    13424 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/f2c.h
+-rwxrwxrwx   0 root         (0) root         (0)     6941 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/global_parameter.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     2650 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/global_parameter.hpp
+-rwxrwxrwx   0 root         (0) root         (0)    24433 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/integrate.cpp
+-rwxrwxrwx   0 root         (0) root         (0)     5770 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/integrate.hpp
+-rw-rw-rw-   0 root         (0) root         (0)      124 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/lapack-blas.h
+-rw-rw-rw-   0 root         (0) root         (0)     7187 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/matrix.cpp
+-rw-rw-rw-   0 root         (0) root         (0)    20538 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/matrix.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     6702 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/parser.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     2395 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/parser.hpp
+-rw-rw-rw-   0 root         (0) root         (0)      828 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/types.hpp
+-rw-rw-rw-   0 root         (0) root         (0)     4354 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/vector_num.cpp
+-rw-rw-rw-   0 root         (0) root         (0)     5978 2024-04-03 21:29:54.000000 pyqcm-2.5.2/src_util/vector_num.hpp
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.637531 pyqcm-2.5.2/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      489 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_all.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.637531 pyqcm-2.5.2/tests/test_diagonalization/
+-rw-rw-rw-   0 root         (0) root         (0)    27349 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_diagonalization/S_format.ref
+-rw-rw-rw-   0 root         (0) root         (0)     2575 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_diagonalization/S_format_complex.ref
+-rw-rw-rw-   0 root         (0) root         (0)     1341 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_diagonalization/cluster_2x2_2C_8b_C2v_L.py
+-rw-rw-rw-   0 root         (0) root         (0)      684 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_diagonalization/common.py
+-rw-rw-rw-   0 root         (0) root         (0)      566 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_diagonalization/model_1D_8.py
+-rw-rw-rw-   0 root         (0) root         (0)     1608 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_diagonalization/model_2x2_2C_8b_C2v_L.py
+-rw-rw-rw-   0 root         (0) root         (0)     2370 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_diagonalization/test_pole_distribution.py
+-rw-rw-rw-   0 root         (0) root         (0)     1002 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_diagonalization/test_pole_distribution_complex.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-03 21:30:03.641532 pyqcm-2.5.2/tests/test_files/
+-rw-rw-rw-   0 root         (0) root         (0)     1290 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/model_1D.py
+-rw-rw-rw-   0 root         (0) root         (0)     1281 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/model_1D_2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2712 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/model_1D_2_4b.py
+-rwxrwxrwx   0 root         (0) root         (0)     1297 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/model_1D_4.py
+-rw-rw-rw-   0 root         (0) root         (0)      952 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/model_1D_4_C2.py
+-rwxrwxrwx   0 root         (0) root         (0)     1220 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/model_2x2_C2.py
+-rw-rw-rw-   0 root         (0) root         (0)     1198 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/model_2x2_C2_vca.py
+-rw-rw-rw-   0 root         (0) root         (0)     1320 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/model_G4_6b_2C.py
+-rw-rw-rw-   0 root         (0) root         (0)      751 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/model_WSM.py
+-rw-rw-rw-   0 root         (0) root         (0)     2064 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/model_graphene_bath.py
+-rw-rw-rw-   0 root         (0) root         (0)      833 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/model_hartree.py
+-rw-rw-rw-   0 root         (0) root         (0)     4846 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/record_2x2.py
+-rw-rw-rw-   0 root         (0) root         (0)     8484 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/record_2x2_8b.py
+-rw-rw-rw-   0 root         (0) root         (0)   108854 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/record_2x2_anom.py
+-rw-rw-rw-   0 root         (0) root         (0)    19410 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/record_WSM.py
+-rw-rw-rw-   0 root         (0) root         (0)   208082 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/record_WSM2.py
+-rw-rw-rw-   0 root         (0) root         (0)     5989 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/record_spin.py
+-rw-rw-rw-   0 root         (0) root         (0)     2359 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_2clusters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1496 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_CF.py
+-rw-rw-rw-   0 root         (0) root         (0)      937 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_averages.py
+-rw-rw-rw-   0 root         (0) root         (0)      471 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_averages_bath.py
+-rw-rw-rw-   0 root         (0) root         (0)     1995 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_berry.py
+-rw-rw-rw-   0 root         (0) root         (0)     1275 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_cdmft.py
+-rw-rw-rw-   0 root         (0) root         (0)     1293 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_cdmft_hartree.py
+-rw-rw-rw-   0 root         (0) root         (0)      638 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_cluster_average.py
+-rw-rw-rw-   0 root         (0) root         (0)      954 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_controlled_loop.py
+-rw-rw-rw-   0 root         (0) root         (0)      893 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_draw.py
+-rw-rw-rw-   0 root         (0) root         (0)     1427 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_fidelity.py
+-rw-rw-rw-   0 root         (0) root         (0)      726 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_fixed_density_loop.py
+-rw-rw-rw-   0 root         (0) root         (0)     1845 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_hartree.py
+-rw-rw-rw-   0 root         (0) root         (0)      359 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_hybridization.py
+-rw-rw-rw-   0 root         (0) root         (0)      433 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_instances.py
+-rw-rw-rw-   0 root         (0) root         (0)     1149 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_mixing.py
+-rw-rw-rw-   0 root         (0) root         (0)      897 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_mixing2.py
+-rw-rw-rw-   0 root         (0) root         (0)     1197 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_mixing_cf.py
+-rw-rw-rw-   0 root         (0) root         (0)     2431 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_reset.py
+-rw-rw-rw-   0 root         (0) root         (0)     4290 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_spectral.py
+-rw-rw-rw-   0 root         (0) root         (0)      475 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_varia.py
+-rw-rw-rw-   0 root         (0) root         (0)     1982 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_vca.py
+-rw-rw-rw-   0 root         (0) root         (0)      637 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_vca_MPI.py
+-rw-rw-rw-   0 root         (0) root         (0)      528 2024-04-03 21:29:54.000000 pyqcm-2.5.2/tests/test_files/test_write.py
```

### Comparing `pyqcm-2.5.1/CMakeLists.txt` & `pyqcm-2.5.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/INSTALL.md` & `pyqcm-2.5.2/INSTALL.md`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/LICENSE` & `pyqcm-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/PKG-INFO` & `pyqcm-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqcm
-Version: 2.5.1
+Version: 2.5.2
 Summary: Quantum cluster methods for the physics of strongly correlated systems
 Home-page: https://bitbucket.org/dsenechQCM/qcm_wed/
 Author: David Sénéchal
 License: GPL
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyqcm-2.5.1/README.md` & `pyqcm-2.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/bench/ED/bench_ED.py` & `pyqcm-2.5.2/bench/ED/bench_ED.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/bench/ED/bench_ED2.py` & `pyqcm-2.5.2/bench/ED/bench_ED2.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/bench/ED/bench_GS.py` & `pyqcm-2.5.2/bench/ED/bench_GS.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/bench/ED/bench_GS2.py` & `pyqcm-2.5.2/bench/ED/bench_GS2.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/bench/ED/bench_GS_loop.py` & `pyqcm-2.5.2/bench/ED/bench_GS_loop.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/bench/ED/model_1D.py` & `pyqcm-2.5.2/bench/ED/model_1D.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/bench/ED/model_2D.py` & `pyqcm-2.5.2/bench/ED/model_2D.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/bench/ED/plot_bench_ED.py` & `pyqcm-2.5.2/bench/ED/plot_bench_ED.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/bench/integrals/plot_concurrent.py` & `pyqcm-2.5.2/bench/integrals/plot_concurrent.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/bench/integrals/plot_integrals.py` & `pyqcm-2.5.2/bench/integrals/plot_integrals.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/bench/integrals/small/model_small.py` & `pyqcm-2.5.2/bench/integrals/small/model_small.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/bench/vca/bench_vca.py` & `pyqcm-2.5.2/bench/vca/bench_vca.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/bench/vca/bench_vca2.py` & `pyqcm-2.5.2/bench/vca/bench_vca2.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/docs/Makefile` & `pyqcm-2.5.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/docs/source/2x2.png` & `pyqcm-2.5.2/docs/source/2x2.png`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/docs/source/T6.png` & `pyqcm-2.5.2/docs/source/T6.png`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/docs/source/cdmft.rst` & `pyqcm-2.5.2/docs/source/cdmft.rst`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/docs/source/conf.py` & `pyqcm-2.5.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/docs/source/defining_cluster_models.rst` & `pyqcm-2.5.2/docs/source/defining_cluster_models.rst`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/docs/source/defining_models.rst` & `pyqcm-2.5.2/docs/source/defining_models.rst`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/docs/source/h4-6b.png` & `pyqcm-2.5.2/docs/source/h4-6b.png`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/docs/source/h8.asy` & `pyqcm-2.5.2/docs/source/h8.asy`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/docs/source/h8.png` & `pyqcm-2.5.2/docs/source/h8.png`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/docs/source/hartree.rst` & `pyqcm-2.5.2/docs/source/hartree.rst`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/docs/source/hexa6.png` & `pyqcm-2.5.2/docs/source/hexa6.png`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/docs/source/index.rst` & `pyqcm-2.5.2/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/docs/source/intro.rst` & `pyqcm-2.5.2/docs/source/intro.rst`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/docs/source/models.rst` & `pyqcm-2.5.2/docs/source/models.rst`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/docs/source/options.rst` & `pyqcm-2.5.2/docs/source/options.rst`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/docs/source/options_intro.txt` & `pyqcm-2.5.2/docs/source/options_intro.txt`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/docs/source/parallel.rst` & `pyqcm-2.5.2/docs/source/parallel.rst`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/docs/source/parallel_performance_concurrent.png` & `pyqcm-2.5.2/docs/source/parallel_performance_concurrent.png`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/docs/source/parallel_performance_ed.png` & `pyqcm-2.5.2/docs/source/parallel_performance_ed.png`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/docs/source/parallel_performance_integrals.png` & `pyqcm-2.5.2/docs/source/parallel_performance_integrals.png`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/docs/source/parameters.rst` & `pyqcm-2.5.2/docs/source/parameters.rst`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/docs/source/t15.png` & `pyqcm-2.5.2/docs/source/t15.png`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/docs/source/vca.rst` & `pyqcm-2.5.2/docs/source/vca.rst`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/examples/1D_2_4b/averages.tsv` & `pyqcm-2.5.2/examples/1D_2_4b/averages.tsv`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/examples/1D_2_4b/cdmft.tsv` & `pyqcm-2.5.2/examples/1D_2_4b/cdmft.tsv`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/examples/1D_2_4b/cdmft_distance.tsv` & `pyqcm-2.5.2/examples/1D_2_4b/cdmft_distance.tsv`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/examples/1D_2_4b/cdmft_grid.tsv` & `pyqcm-2.5.2/examples/1D_2_4b/cdmft_grid.tsv`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/examples/1D_2_4b/cdmft_iter.tsv` & `pyqcm-2.5.2/examples/1D_2_4b/cdmft_iter.tsv`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/examples/1D_2_4b/debug.py` & `pyqcm-2.5.2/examples/1D_2_4b/debug.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/examples/1D_2_4b/debug_complex.py` & `pyqcm-2.5.2/examples/1D_2_4b/debug_complex.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/examples/1D_2_4b/debug_dvmc.py` & `pyqcm-2.5.2/examples/1D_2_4b/debug_dvmc.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/examples/1D_2_4b/debug_variable_parameter.py` & `pyqcm-2.5.2/examples/1D_2_4b/debug_variable_parameter.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/examples/1D_2_4b/dos.tsv` & `pyqcm-2.5.2/examples/1D_2_4b/dos.tsv`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/examples/1D_2_4b/h1.pdf` & `pyqcm-2.5.2/examples/1D_2_4b/h1.pdf`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/examples/1D_2_4b/h2.pdf` & `pyqcm-2.5.2/examples/1D_2_4b/h2.pdf`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/examples/1D_2_4b/hop.npy` & `pyqcm-2.5.2/examples/1D_2_4b/hop.npy`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/examples/1D_2_4b/model_1D_2_4b.py` & `pyqcm-2.5.2/examples/1D_2_4b/model_1D_2_4b.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/examples/1D_2_4b/out` & `pyqcm-2.5.2/examples/1D_2_4b/out`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/examples/1D_2_4b/s1.pdf` & `pyqcm-2.5.2/examples/1D_2_4b/s1.pdf`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/examples/1D_2_4b/s2.pdf` & `pyqcm-2.5.2/examples/1D_2_4b/s2.pdf`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/examples/1D_4/GS.tsv` & `pyqcm-2.5.2/examples/1D_4/GS.tsv`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/examples/1D_4/ave.tsv` & `pyqcm-2.5.2/examples/1D_4/ave.tsv`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/examples/1D_4/averages.tsv` & `pyqcm-2.5.2/examples/1D_4/averages.tsv`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/examples/1D_4/debug_cdw.py` & `pyqcm-2.5.2/examples/1D_4/debug_cdw.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/examples/1D_4/debug_rhoAB.py` & `pyqcm-2.5.2/examples/1D_4/debug_rhoAB.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/examples/1D_4/hartree.tsv` & `pyqcm-2.5.2/examples/1D_4/hartree.tsv`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/examples/1D_4/model_1D_4.py` & `pyqcm-2.5.2/examples/1D_4/model_1D_4.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/examples/1D_4/record.py` & `pyqcm-2.5.2/examples/1D_4/record.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/examples/1D_4/sef.tsv` & `pyqcm-2.5.2/examples/1D_4/sef.tsv`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/examples/1D_4/vca.tsv` & `pyqcm-2.5.2/examples/1D_4/vca.tsv`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/external/FindAVX2.cmake` & `pyqcm-2.5.2/external/FindAVX2.cmake`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/notebooks/AF_VCA_vs_L.ipynb` & `pyqcm-2.5.2/notebooks/AF_VCA_vs_L.ipynb`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/notebooks/AF_VCA_vs_L.py` & `pyqcm-2.5.2/notebooks/AF_VCA_vs_L.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/notebooks/CDW_1D.ipynb` & `pyqcm-2.5.2/notebooks/CDW_1D.ipynb`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/notebooks/CDW_1D.py` & `pyqcm-2.5.2/notebooks/CDW_1D.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/notebooks/Mott_Weyl.ipynb` & `pyqcm-2.5.2/notebooks/Mott_Weyl.ipynb`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/notebooks/Mott_Weyl.py` & `pyqcm-2.5.2/notebooks/Mott_Weyl.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/notebooks/Mott_transition_graphene_CDMFT.ipynb` & `pyqcm-2.5.2/notebooks/Mott_transition_graphene_CDMFT.ipynb`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/notebooks/Mott_transition_graphene_CDMFT.py` & `pyqcm-2.5.2/notebooks/Mott_transition_graphene_CDMFT.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/notebooks/Rashba_coupling.ipynb` & `pyqcm-2.5.2/notebooks/Rashba_coupling.ipynb`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/notebooks/Rashba_coupling.py` & `pyqcm-2.5.2/notebooks/Rashba_coupling.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/notebooks/antiferromagnetism_VCA.ipynb` & `pyqcm-2.5.2/notebooks/antiferromagnetism_VCA.ipynb`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/notebooks/antiferromagnetism_VCA.py` & `pyqcm-2.5.2/notebooks/antiferromagnetism_VCA.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/notebooks/dimerization_1D.ipynb` & `pyqcm-2.5.2/notebooks/dimerization_1D.ipynb`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/notebooks/dimerization_1D.py` & `pyqcm-2.5.2/notebooks/dimerization_1D.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/notebooks/intro1.ipynb` & `pyqcm-2.5.2/notebooks/intro1.ipynb`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/notebooks/intro1.py` & `pyqcm-2.5.2/notebooks/intro1.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/notebooks/intro2.ipynb` & `pyqcm-2.5.2/notebooks/intro2.ipynb`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/notebooks/intro2.py` & `pyqcm-2.5.2/notebooks/intro2.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/notebooks/intro3.ipynb` & `pyqcm-2.5.2/notebooks/intro3.ipynb`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/notebooks/intro3.py` & `pyqcm-2.5.2/notebooks/intro3.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/notebooks/periodic_cluster.ipynb` & `pyqcm-2.5.2/notebooks/periodic_cluster.ipynb`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/notebooks/periodic_cluster.py` & `pyqcm-2.5.2/notebooks/periodic_cluster.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/notebooks/superconductivity_VCA.ipynb` & `pyqcm-2.5.2/notebooks/superconductivity_VCA.ipynb`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/notebooks/superconductivity_VCA.py` & `pyqcm-2.5.2/notebooks/superconductivity_VCA.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/pyqcm/Kolmogorov_Smirnov.py` & `pyqcm-2.5.2/pyqcm/Kolmogorov_Smirnov.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/pyqcm/__init__.py` & `pyqcm-2.5.2/pyqcm/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,14 +112,17 @@
         :return: None
             
         """
 
         if self.is_closed:
             raise ValueError('cluster_model.new_operator() cannot be called any more : the model is closed')
 
+        if '_' in op_name:
+            raise ValueError('names of operators must not include the character "_" (underline)')
+
         if op_type == 'anomalous':
             for x in elem:  
                 if x[0] >= x[1] :
                     raise ValueError(f'anomalous matrix elements of {op_name} must be such that row index < column index')
 
         qcm.new_operator(self.name, op_name, op_type, elem)
 
@@ -136,14 +139,17 @@
         """
 
         global the_model
 
         if self.is_closed:
             raise ValueError('cluster_model.new_operator() cannot be called any more : the model is closed')
 
+        if '_' in op_name:
+            raise ValueError('names of operators must not include the character "_" (underline)')
+
         if op_type == 'anomalous':
             for x in elem:  
                 if x[0] >= x[1] :
                     raise ValueError(f'anomalous matrix elements of {op_name} must be such that row index < column index')
 
         qcm.new_operator_complex(self.name, op_name, op_type, elem)
 
@@ -249,14 +255,17 @@
             * tau (*int*) -- specifies the tau Pauli matrix  (0,1,2,3)
             * sigma (*int*) -- specifies the sigma Pauli matrix  (0,1,2,3)
     
         :return: None
 
         """
 
+        if '_' in name:
+            raise ValueError('names of operators must not include the character "_" (underline)')
+
         if link == ( 0, 0, 0):
             if "tau" in kwargs:
                 if kwargs["tau"] != 0: kwargs["tau"] = 0
             else:
                 kwargs["tau"] = 0
 
         orb1, orb2 = orbital_pair_manager(orbitals) 
@@ -278,14 +287,17 @@
         
             * type (*str*) -- one of 'singlet' (default), 'dz', 'dy', 'dx'
     
         :return: None
 
         """
         
+        if '_' in name:
+            raise ValueError('names of operators must not include the character "_" (underline)')
+
         orb1, orb2 = orbital_pair_manager(orbitals) 
 
         for orb_no1 in orb1:
             for orb_no2 in orb2:
                 qcm.anomalous_operator(name, link, amplitude, orb1=orb_no1, orb2=orb_no2, **kwargs)
 
     #-----------------------------------------------------------------------------------------------
@@ -301,14 +313,17 @@
             * tau (*int*) -- specifies the tau Pauli matrix  (0,1,2,3)
             * sigma (*int*) -- specifies the sigma Pauli matrix  (0,1,2,3)
             * type (*str*) -- one of 'one-body' [default], 'singlet', 'dz', 'dy', 'dx', 'Hubbard', 'Hund', 'Heisenberg', 'X', 'Y', 'Z'
 
         :return: None
 
         """
+        if '_' in name:
+            raise ValueError('names of operators must not include the character "_" (underline)')
+
         qcm.explicit_operator(name, elem, **kwargs)
 
     #-----------------------------------------------------------------------------------------------
     def density_wave(self, name, t, Q, **kwargs):
         """
         Defines a density wave
 
@@ -322,15 +337,16 @@
             * amplitude (*complex*) -- amplitude multiplier. **Caution**: A factor of 2 must be used in some situations (see :ref:`density wave theory`)
             * orb (*int*) -- orbital label (0 by default = all orbitals)
             * phase (*float*) -- real phase (as a multiple of :math:`pi`)
 
         :return: None
 
         """
-
+        if '_' in name:
+            raise ValueError('names of operators must not include the character "_" (underline)')
         qcm.density_wave(name, t, Q, **kwargs)
 
     #-----------------------------------------------------------------------------------------------
     def set_basis(self, B):
         """
         Define the working basis in terms of a physical basis, i.e., provides a transformation matrix between
         the two.
@@ -357,15 +373,16 @@
             * type (*str*): one of 'Hubbard', 'Heisenberg', 'Hund', 'X', 'Y', 'Z'
 
         :return: None
 
         """
 
         orb1, orb2 = orbital_pair_manager(orbitals) 
-
+        if '_' in name:
+            raise ValueError('names of operators must not include the character "_" (underline)')
         for orb_no1 in orb1:
             for orb_no2 in orb2:
                 qcm.interaction_operator(name, orb1=orb_no1, orb2=orb_no2, link=link, **kwargs)
 
     #-----------------------------------------------------------------------------------------------
     def set_target_sectors(self, sec):
         """
```

### Comparing `pyqcm-2.5.1/pyqcm/_draw.py` & `pyqcm-2.5.2/pyqcm/_draw.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/pyqcm/_loop.py` & `pyqcm-2.5.2/pyqcm/_loop.py`

 * *Files 1% similar despite different names*

```diff
@@ -474,14 +474,16 @@
 		print('density = ', n[0])
 		mu = np.roll(mu, 1)  # cycles the values of the loop parameter
 		n = np.roll(n, 1)  # cycles the values of the loop parameter
 		sol = np.roll(sol, 1, 0)  # cycles the solutions
 
 
 		n[0] = n[1] + delta_n
+		if delta_n < 0 and n[0] < final_n: break
+		if delta_n > 0 and n[0] > final_n: break
 
 		# predicting the starting value from previous solutions (do nothing if loop_counter=0)
 		fit_type = ''
 		if loop_counter == 1:
 			start = sol[1, :]  # the starting point is the previous value in the loop
 			mu[0] = mu[1] + initial_step  # updates the loop parameter
 		elif loop_counter == 2:
@@ -507,15 +509,15 @@
 			pol_mu = np.polyfit(z, x, 2)
 			pol = np.polyfit(x, y, 2)
 			mu[0] = np.polyval(pol_mu, n[0])
 			for i in range(nvar):
 				start[i] = np.polyval(pol[:, i], mu[0])
 
 		if loop_counter > 1:
-			print('flexible_loop step : mu = ', mu[0])
+			print('flexible_loop step : mu = ', mu[0]-mu[1])
 			print('predictor : ', start, fit_type)
 			for i in range(len(varia)):
 				self.set_parameter(varia[i], start[i])
 				print(' ---> ', varia[i], ' = ', start[i])
 
 		loop_counter += 1
```

### Comparing `pyqcm-2.5.1/pyqcm/_spectral.py` & `pyqcm-2.5.2/pyqcm/_spectral.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/pyqcm/cdmft.py` & `pyqcm-2.5.2/pyqcm/cdmft.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/pyqcm/cdw.py` & `pyqcm-2.5.2/pyqcm/cdw.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/pyqcm/dca.py` & `pyqcm-2.5.2/pyqcm/dca.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/pyqcm/external.py` & `pyqcm-2.5.2/pyqcm/external.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/pyqcm/slab.py` & `pyqcm-2.5.2/pyqcm/slab.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/pyqcm/variable_parameter.py` & `pyqcm-2.5.2/pyqcm/variable_parameter.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/pyqcm/vca.py` & `pyqcm-2.5.2/pyqcm/vca.py`

 * *Files 1% similar despite different names*

```diff
@@ -587,15 +587,15 @@
         self.consistency_check = consistency_check
 
         SEF_eval = 0
         def var2x(x):
             global current_instance, root
             for i in range(len(x)):
                 if np.abs(x[i]) > max[i]:
-                    raise pyqcm.OutOfBoundsError(variable=varia[i])
+                    raise pyqcm.OutOfBoundsError('parameter {:s} is out of bounds!'.format(varia[i]))
             global SEF_eval
             if var2sef is None:
                 for i in range(len(varia)): 
                     model.set_parameter(varia[i], x[i])
                 print('x = ', x) # new
             else:
                 var2sef(x)
```

### Comparing `pyqcm-2.5.1/pyqcm.egg-info/PKG-INFO` & `pyqcm-2.5.2/pyqcm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqcm
-Version: 2.5.1
+Version: 2.5.2
 Summary: Quantum cluster methods for the physics of strongly correlated systems
 Home-page: https://bitbucket.org/dsenechQCM/qcm_wed/
 Author: David Sénéchal
 License: GPL
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `pyqcm-2.5.1/pyqcm.egg-info/SOURCES.txt` & `pyqcm-2.5.2/pyqcm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/setup.py` & `pyqcm-2.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/.clang-format` & `pyqcm-2.5.2/src_ed/.clang-format`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Doxyfile` & `pyqcm-2.5.2/src_ed/Doxyfile`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/ED_basis.cpp` & `pyqcm-2.5.2/src_ed/ED_basis.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/ED_basis.hpp` & `pyqcm-2.5.2/src_ed/ED_basis.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Green_function_set.hpp` & `pyqcm-2.5.2/src_ed/Green_function_set.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Hamiltonian/CSR_hermitian.hpp` & `pyqcm-2.5.2/src_ed/Hamiltonian/CSR_hermitian.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Hamiltonian/Davidson.hpp` & `pyqcm-2.5.2/src_ed/Hamiltonian/Davidson.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Hamiltonian/Hamiltonian_CSR.hpp` & `pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_CSR.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Hamiltonian/Hamiltonian_Dense.hpp` & `pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_Dense.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Hamiltonian/Hamiltonian_Eigen.hpp` & `pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_Eigen.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Hamiltonian/Hamiltonian_Factorized.hpp` & `pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_Factorized.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Hamiltonian/Hamiltonian_OnTheFly.hpp` & `pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_OnTheFly.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Hamiltonian/Hamiltonian_Operator.hpp` & `pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_Operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Hamiltonian/Hamiltonian_base.hpp` & `pyqcm-2.5.2/src_ed/Hamiltonian/Hamiltonian_base.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Hamiltonian/Lanczos.cpp` & `pyqcm-2.5.2/src_ed/Hamiltonian/Lanczos.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Hamiltonian/Lanczos.hpp` & `pyqcm-2.5.2/src_ed/Hamiltonian/Lanczos.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Hamiltonian/PRIMME_solver.hpp` & `pyqcm-2.5.2/src_ed/Hamiltonian/PRIMME_solver.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Operators/HS_Heisenberg_operator.hpp` & `pyqcm-2.5.2/src_ed/Operators/HS_Heisenberg_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Operators/HS_Hermitian_operator.hpp` & `pyqcm-2.5.2/src_ed/Operators/HS_Hermitian_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Operators/HS_Hund_operator.hpp` & `pyqcm-2.5.2/src_ed/Operators/HS_Hund_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Operators/HS_anomalous_operator.hpp` & `pyqcm-2.5.2/src_ed/Operators/HS_anomalous_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Operators/HS_factorized_operator.hpp` & `pyqcm-2.5.2/src_ed/Operators/HS_factorized_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Operators/HS_general_interaction_operator.hpp` & `pyqcm-2.5.2/src_ed/Operators/HS_general_interaction_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Operators/HS_half_operator.hpp` & `pyqcm-2.5.2/src_ed/Operators/HS_half_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Operators/HS_interaction_operator.hpp` & `pyqcm-2.5.2/src_ed/Operators/HS_interaction_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Operators/HS_nondiagonal_operator.hpp` & `pyqcm-2.5.2/src_ed/Operators/HS_nondiagonal_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Operators/HS_one_body_operator.hpp` & `pyqcm-2.5.2/src_ed/Operators/HS_one_body_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Operators/HS_operator.hpp` & `pyqcm-2.5.2/src_ed/Operators/HS_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Operators/Heisenberg_operator.cpp` & `pyqcm-2.5.2/src_ed/Operators/Heisenberg_operator.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Operators/Heisenberg_operator.hpp` & `pyqcm-2.5.2/src_ed/Operators/Heisenberg_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Operators/Hermitian_operator.hpp` & `pyqcm-2.5.2/src_ed/Operators/Hermitian_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Operators/Hund_operator.cpp` & `pyqcm-2.5.2/src_ed/Operators/Hund_operator.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Operators/Hund_operator.hpp` & `pyqcm-2.5.2/src_ed/Operators/Hund_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Operators/anomalous_operator.hpp` & `pyqcm-2.5.2/src_ed/Operators/anomalous_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Operators/destruction_operator.cpp` & `pyqcm-2.5.2/src_ed/Operators/destruction_operator.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Operators/destruction_operator.hpp` & `pyqcm-2.5.2/src_ed/Operators/destruction_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Operators/general_interaction_operator.hpp` & `pyqcm-2.5.2/src_ed/Operators/general_interaction_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Operators/interaction_operator.hpp` & `pyqcm-2.5.2/src_ed/Operators/interaction_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Operators/one_body_operator.hpp` & `pyqcm-2.5.2/src_ed/Operators/one_body_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Q_matrix.hpp` & `pyqcm-2.5.2/src_ed/Q_matrix.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/Q_matrix_set.hpp` & `pyqcm-2.5.2/src_ed/Q_matrix_set.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/binary_state.cpp` & `pyqcm-2.5.2/src_ed/binary_state.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/binary_state.hpp` & `pyqcm-2.5.2/src_ed/binary_state.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/continued_fraction.cpp` & `pyqcm-2.5.2/src_ed/continued_fraction.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/continued_fraction.hpp` & `pyqcm-2.5.2/src_ed/continued_fraction.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/continued_fraction_set.cpp` & `pyqcm-2.5.2/src_ed/continued_fraction_set.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/continued_fraction_set.hpp` & `pyqcm-2.5.2/src_ed/continued_fraction_set.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/flex_array.hpp` & `pyqcm-2.5.2/src_ed/flex_array.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/fraction.hpp` & `pyqcm-2.5.2/src_ed/fraction.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/index.hpp` & `pyqcm-2.5.2/src_ed/index.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/index_pair.hpp` & `pyqcm-2.5.2/src_ed/index_pair.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/matrix_element.hpp` & `pyqcm-2.5.2/src_ed/matrix_element.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/model.cpp` & `pyqcm-2.5.2/src_ed/model.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/model.hpp` & `pyqcm-2.5.2/src_ed/model.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/model_instance.cpp` & `pyqcm-2.5.2/src_ed/model_instance.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/model_instance.hpp` & `pyqcm-2.5.2/src_ed/model_instance.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/model_instance_base.cpp` & `pyqcm-2.5.2/src_ed/model_instance_base.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/model_instance_base.hpp` & `pyqcm-2.5.2/src_ed/model_instance_base.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/qcm_ED.cpp` & `pyqcm-2.5.2/src_ed/qcm_ED.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/qcm_ED.hpp` & `pyqcm-2.5.2/src_ed/qcm_ED.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/sector.cpp` & `pyqcm-2.5.2/src_ed/sector.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/sector.hpp` & `pyqcm-2.5.2/src_ed/sector.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/sparse_matrix.hpp` & `pyqcm-2.5.2/src_ed/sparse_matrix.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/state.hpp` & `pyqcm-2.5.2/src_ed/state.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/symmetric_orbital.hpp` & `pyqcm-2.5.2/src_ed/symmetric_orbital.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/symmetry_group.cpp` & `pyqcm-2.5.2/src_ed/symmetry_group.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_ed/symmetry_group.hpp` & `pyqcm-2.5.2/src_ed/symmetry_group.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_python/common_Py.cpp` & `pyqcm-2.5.2/src_python/common_Py.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_python/common_Py.hpp` & `pyqcm-2.5.2/src_python/common_Py.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_python/qcm_ED_lib.cpp` & `pyqcm-2.5.2/src_python/qcm_ED_lib.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_python/qcm_ED_only.hpp` & `pyqcm-2.5.2/src_python/qcm_ED_only.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_python/qcm_ED_wrap.hpp` & `pyqcm-2.5.2/src_python/qcm_ED_wrap.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_python/qcm_lib.cpp` & `pyqcm-2.5.2/src_python/qcm_lib.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_python/qcm_wrap.hpp` & `pyqcm-2.5.2/src_python/qcm_wrap.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_qcm/CPT.cpp` & `pyqcm-2.5.2/src_qcm/CPT.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_qcm/Chern.cpp` & `pyqcm-2.5.2/src_qcm/Chern.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_qcm/Doxyfile` & `pyqcm-2.5.2/src_qcm/Doxyfile`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_qcm/Green_function.hpp` & `pyqcm-2.5.2/src_qcm/Green_function.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_qcm/QCM.cpp` & `pyqcm-2.5.2/src_qcm/QCM.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_qcm/QCM.hpp` & `pyqcm-2.5.2/src_qcm/QCM.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_qcm/average.cpp` & `pyqcm-2.5.2/src_qcm/average.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_qcm/basis3D.cpp` & `pyqcm-2.5.2/src_qcm/basis3D.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_qcm/basis3D.hpp` & `pyqcm-2.5.2/src_qcm/basis3D.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_qcm/lattice3D.cpp` & `pyqcm-2.5.2/src_qcm/lattice3D.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_qcm/lattice3D.hpp` & `pyqcm-2.5.2/src_qcm/lattice3D.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_qcm/lattice_matrix_element.hpp` & `pyqcm-2.5.2/src_qcm/lattice_matrix_element.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_qcm/lattice_model.cpp` & `pyqcm-2.5.2/src_qcm/lattice_model.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_qcm/lattice_model.hpp` & `pyqcm-2.5.2/src_qcm/lattice_model.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_qcm/lattice_model_instance.cpp` & `pyqcm-2.5.2/src_qcm/lattice_model_instance.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_qcm/lattice_model_instance.hpp` & `pyqcm-2.5.2/src_qcm/lattice_model_instance.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_qcm/lattice_operator.cpp` & `pyqcm-2.5.2/src_qcm/lattice_operator.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_qcm/lattice_operator.hpp` & `pyqcm-2.5.2/src_qcm/lattice_operator.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_qcm/omp.h` & `pyqcm-2.5.2/src_qcm/omp.h`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_qcm/parameter_set.cpp` & `pyqcm-2.5.2/src_qcm/parameter_set.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_qcm/parameter_set.hpp` & `pyqcm-2.5.2/src_qcm/parameter_set.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_qcm/print.cpp` & `pyqcm-2.5.2/src_qcm/print.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_qcm/profile.cpp` & `pyqcm-2.5.2/src_qcm/profile.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_qcm/vector3D.hpp` & `pyqcm-2.5.2/src_qcm/vector3D.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_util/ED_global_parameter.cpp` & `pyqcm-2.5.2/src_util/ED_global_parameter.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_util/VDVH_kernel.cpp` & `pyqcm-2.5.2/src_util/VDVH_kernel.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_util/VDVH_kernel.hpp` & `pyqcm-2.5.2/src_util/VDVH_kernel.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_util/block_matrix.hpp` & `pyqcm-2.5.2/src_util/block_matrix.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_util/cblas.h` & `pyqcm-2.5.2/src_util/cblas.h`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_util/clapack.h` & `pyqcm-2.5.2/src_util/clapack.h`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_util/f2c.h` & `pyqcm-2.5.2/src_util/f2c.h`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_util/global_parameter.cpp` & `pyqcm-2.5.2/src_util/global_parameter.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_util/global_parameter.hpp` & `pyqcm-2.5.2/src_util/global_parameter.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_util/integrate.cpp` & `pyqcm-2.5.2/src_util/integrate.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_util/integrate.hpp` & `pyqcm-2.5.2/src_util/integrate.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_util/matrix.cpp` & `pyqcm-2.5.2/src_util/matrix.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_util/matrix.hpp` & `pyqcm-2.5.2/src_util/matrix.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_util/parser.cpp` & `pyqcm-2.5.2/src_util/parser.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_util/parser.hpp` & `pyqcm-2.5.2/src_util/parser.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_util/types.hpp` & `pyqcm-2.5.2/src_util/types.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_util/vector_num.cpp` & `pyqcm-2.5.2/src_util/vector_num.cpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/src_util/vector_num.hpp` & `pyqcm-2.5.2/src_util/vector_num.hpp`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_all.py` & `pyqcm-2.5.2/tests/test_all.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_diagonalization/S_format.ref` & `pyqcm-2.5.2/tests/test_diagonalization/S_format.ref`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_diagonalization/S_format_complex.ref` & `pyqcm-2.5.2/tests/test_diagonalization/S_format_complex.ref`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_diagonalization/cluster_2x2_2C_8b_C2v_L.py` & `pyqcm-2.5.2/tests/test_diagonalization/cluster_2x2_2C_8b_C2v_L.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_diagonalization/common.py` & `pyqcm-2.5.2/tests/test_diagonalization/common.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_diagonalization/model_1D_8.py` & `pyqcm-2.5.2/tests/test_diagonalization/model_1D_8.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_diagonalization/model_2x2_2C_8b_C2v_L.py` & `pyqcm-2.5.2/tests/test_diagonalization/model_2x2_2C_8b_C2v_L.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_diagonalization/test_pole_distribution.py` & `pyqcm-2.5.2/tests/test_diagonalization/test_pole_distribution.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_diagonalization/test_pole_distribution_complex.py` & `pyqcm-2.5.2/tests/test_diagonalization/test_pole_distribution_complex.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/model_1D.py` & `pyqcm-2.5.2/tests/test_files/model_1D.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/model_1D_2.py` & `pyqcm-2.5.2/tests/test_files/model_1D_2.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/model_1D_2_4b.py` & `pyqcm-2.5.2/tests/test_files/model_1D_2_4b.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/model_1D_4.py` & `pyqcm-2.5.2/tests/test_files/model_1D_4.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/model_1D_4_C2.py` & `pyqcm-2.5.2/tests/test_files/model_1D_4_C2.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/model_2x2_C2.py` & `pyqcm-2.5.2/tests/test_files/model_2x2_C2.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/model_2x2_C2_vca.py` & `pyqcm-2.5.2/tests/test_files/model_2x2_C2_vca.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/model_G4_6b_2C.py` & `pyqcm-2.5.2/tests/test_files/model_G4_6b_2C.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/model_WSM.py` & `pyqcm-2.5.2/tests/test_files/model_WSM.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/model_graphene_bath.py` & `pyqcm-2.5.2/tests/test_files/model_graphene_bath.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/model_hartree.py` & `pyqcm-2.5.2/tests/test_files/model_hartree.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/record_2x2.py` & `pyqcm-2.5.2/tests/test_files/record_2x2.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/record_2x2_8b.py` & `pyqcm-2.5.2/tests/test_files/record_2x2_8b.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/record_2x2_anom.py` & `pyqcm-2.5.2/tests/test_files/record_2x2_anom.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/record_WSM.py` & `pyqcm-2.5.2/tests/test_files/record_WSM.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/record_WSM2.py` & `pyqcm-2.5.2/tests/test_files/record_WSM2.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/record_spin.py` & `pyqcm-2.5.2/tests/test_files/record_spin.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/test_2clusters.py` & `pyqcm-2.5.2/tests/test_files/test_2clusters.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/test_CF.py` & `pyqcm-2.5.2/tests/test_files/test_CF.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/test_averages.py` & `pyqcm-2.5.2/tests/test_files/test_averages.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/test_berry.py` & `pyqcm-2.5.2/tests/test_files/test_berry.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/test_cdmft.py` & `pyqcm-2.5.2/tests/test_files/test_cdmft.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/test_cdmft_hartree.py` & `pyqcm-2.5.2/tests/test_files/test_cdmft_hartree.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/test_cluster_average.py` & `pyqcm-2.5.2/tests/test_files/test_cluster_average.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/test_controlled_loop.py` & `pyqcm-2.5.2/tests/test_files/test_controlled_loop.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/test_draw.py` & `pyqcm-2.5.2/tests/test_files/test_draw.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/test_fidelity.py` & `pyqcm-2.5.2/tests/test_files/test_fidelity.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/test_fixed_density_loop.py` & `pyqcm-2.5.2/tests/test_files/test_fixed_density_loop.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/test_hartree.py` & `pyqcm-2.5.2/tests/test_files/test_hartree.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/test_mixing.py` & `pyqcm-2.5.2/tests/test_files/test_mixing.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/test_mixing2.py` & `pyqcm-2.5.2/tests/test_files/test_mixing2.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/test_mixing_cf.py` & `pyqcm-2.5.2/tests/test_files/test_mixing_cf.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/test_reset.py` & `pyqcm-2.5.2/tests/test_files/test_reset.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/test_spectral.py` & `pyqcm-2.5.2/tests/test_files/test_spectral.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/test_vca.py` & `pyqcm-2.5.2/tests/test_files/test_vca.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/test_vca_MPI.py` & `pyqcm-2.5.2/tests/test_files/test_vca_MPI.py`

 * *Files identical despite different names*

### Comparing `pyqcm-2.5.1/tests/test_files/test_write.py` & `pyqcm-2.5.2/tests/test_files/test_write.py`

 * *Files identical despite different names*

