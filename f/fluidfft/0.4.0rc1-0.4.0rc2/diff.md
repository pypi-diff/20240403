# Comparing `tmp/fluidfft-0.4.0rc1.tar.gz` & `tmp/fluidfft-0.4.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluidfft-0.4.0rc1.tar", last modified: Sat Feb 10 15:13:23 2024, max compression
+gzip compressed data, was "fluidfft-0.4.0rc2.tar", last modified: Sun Feb 11 05:55:45 2024, max compression
```

## Comparing `fluidfft-0.4.0rc1.tar` & `fluidfft-0.4.0rc2.tar`

### file list

```diff
@@ -1,280 +1,280 @@
--rw-r--r--   0        0        0       58 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/.flake8
--rw-r--r--   0        0        0       44 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/.github/pythranrc-windows
--rw-r--r--   0        0        0     1570 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/.github/workflows/ci-linux.yml
--rw-r--r--   0        0        0      705 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/.github/workflows/ci-pixi.yml
--rw-r--r--   0        0        0     3178 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/.github/workflows/wheels.yml
--rw-r--r--   0        0        0     3117 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/.gitlab-ci.yml
--rw-r--r--   0        0        0     1221 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/.hgtags
--rw-r--r--   0        0        0      492 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/.readthedocs.yml
--rw-r--r--   0        0        0     2998 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/CHANGES.md
--rw-r--r--   0        0        0     1262 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/CONTRIBUTING.md
--rw-r--r--   0        0        0    21781 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/LICENSE.txt
--rw-r--r--   0        0        0     1155 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/Makefile
--rw-r--r--   0        0        0     5957 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/README.md
--rw-r--r--   0        0        0      568 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/benchcpp2d.py
--rw-r--r--   0        0        0      562 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/benchcpp3d.py
--rw-r--r--   0        0        0      792 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/check_openmp.py
--rw-r--r--   0        0        0     1147 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/compare_cypythran/Makefile
--rw-r--r--   0        0        0     2664 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/compare_cypythran/bench.py
--rw-r--r--   0        0        0     1665 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/compare_cypythran/grad_cy.pyx
--rw-r--r--   0        0        0      306 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/compare_cypythran/grad_pythran.py
--rw-r--r--   0        0        0      182 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/compare_cypythran/setup.py
--rw-r--r--   0        0        0     1342 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/compare_mpi4py_fft/Makefile
--rw-r--r--   0        0        0      752 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/compare_mpi4py_fft/bench.py
--rw-r--r--   0        0        0     2644 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/compare_mpi4py_fft/transforms.py
--rw-r--r--   0        0        0     1194 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/dask/try_dask_fft.py
--rw-r--r--   0        0        0     4905 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/debug_mpi4py-fft/README.md
--rw-r--r--   0        0        0      662 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/debug_mpi4py-fft/check_segfault.sh
--rw-r--r--   0        0        0      531 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/debug_mpi4py-fft/prepare_env.sh
--rw-r--r--   0        0        0      698 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/debug_mpi4py-fft/site.cfg.debug
--rw-r--r--   0        0        0      342 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/issue14/README.md
--rw-r--r--   0        0        0     3046 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/issue14/cpp/Makefile
--rw-r--r--   0        0        0      815 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/issue14/cpp/main.cpp
--rw-r--r--   0        0        0      492 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/issue14/investigate_segfault.py
--rw-r--r--   0        0        0      798 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/issue14/investigate_small.py
--rwxr-xr-x   0        0        0     1883 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/operator2d/Makefile
--rw-r--r--   0        0        0     1354 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/operator2d/bench.py
--rw-r--r--   0        0        0     1586 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/projperpk3d/Makefile
--rw-r--r--   0        0        0     1859 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/projperpk3d/README.md
--rw-r--r--   0        0        0      788 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/projperpk3d/bench.py
--rw-r--r--   0        0        0     2735 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/projperpk3d/bench_proj_fortran.f90
--rw-r--r--   0        0        0     1504 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/projperpk3d/proj.py
--rw-r--r--   0        0        0     1404 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/projperpk3d/proj1.py
--rw-r--r--   0        0        0     1545 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/projperpk3d/proj2.py
--rw-r--r--   0        0        0     1495 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/projperpk3d_inplace/Makefile
--rw-r--r--   0        0        0      132 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/projperpk3d_inplace/README.md
--rw-r--r--   0        0        0      970 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/projperpk3d_inplace/bench.py
--rw-r--r--   0        0        0     2224 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/projperpk3d_inplace/bench_proj_fortran.f90
--rw-r--r--   0        0        0     1151 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/projperpk3d_inplace/proj.py
--rwxr-xr-x   0        0        0     1860 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/pythran_implicit_loop/Makefile
--rw-r--r--   0        0        0     2987 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/pythran_implicit_loop/README.md
--rw-r--r--   0        0        0     1207 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/pythran_implicit_loop/bench.py
--rw-r--r--   0        0        0      909 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/pythran_implicit_loop/mymod.py
--rw-r--r--   0        0        0     2124 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/pythran_implicit_loop/pythran_issue807.md
--rw-r--r--   0        0        0     1388 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/pythran_implicit_loop/results2d.txt
--rw-r--r--   0        0        0     1252 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/pythran_implicit_loop/results2d_complex_hook_False.txt
--rw-r--r--   0        0        0     1519 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/pythran_implicit_loop/results3d.txt
--rw-r--r--   0        0        0      231 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/pythran_implicit_loop/work.py
--rwxr-xr-x   0        0        0     3626 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/pythran_implicit_loop2/Makefile
--rw-r--r--   0        0        0     3150 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/pythran_implicit_loop2/README.md
--rw-r--r--   0        0        0      680 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/pythran_implicit_loop2/bench.py
--rw-r--r--   0        0        0     1707 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/pythran_implicit_loop2/mymod.py
--rw-r--r--   0        0        0     1819 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/pythran_implicit_loop2/results_with_gcc.txt
--rw-r--r--   0        0        0      867 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/pythran_implicit_loop2/results_with_marchnative.txt
--rw-r--r--   0        0        0      965 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/pythran_implicit_loop2/results_without_pythranrc.txt
--rw-r--r--   0        0        0     4700 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/pythran_pep_func-not-avail-at-compile-time/README.md
--rw-r--r--   0        0        0      376 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/pythran_pep_func-not-avail-at-compile-time/mymod.py
--rwxr-xr-x   0        0        0     1094 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/submit_benchmarks2d_legi.py
--rwxr-xr-x   0        0        0     1218 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/submit_benchmarks3d_legi.py
--rwxr-xr-x   0        0        0      445 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/submit_benchmarks3d_occigen.py
--rw-r--r--   0        0        0     1078 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/submit_benchmarks_legi.py
--rwxr-xr-x   0        0        0     3157 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/submit_benchmarks_snic.py
--rw-r--r--   0        0        0     3686 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/vector_product/Makefile
--rw-r--r--   0        0        0     1599 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/vector_product/bench.py
--rw-r--r--   0        0        0     2412 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/bench/vector_product/vectprod.py
--rw-r--r--   0        0        0     5997 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/Makefile
--rw-r--r--   0        0        0     3858 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/bench.md
--rw-r--r--   0        0        0     8506 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/build-from-source.md
--rw-r--r--   0        0        0     2998 2024-02-10 15:13:22.943098 fluidfft-0.4.0rc1/doc/changes.md
--rw-r--r--   0        0        0    11623 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/conf.py
--rw-r--r--   0        0        0   104172 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/doxygen/Doxyfile
--rw-r--r--   0        0        0     3739 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/examples/Makefile
--rw-r--r--   0        0        0     3279 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/examples/Makefile.2d
--rw-r--r--   0        0        0     1237 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/examples/compute_energy.cpp
--rw-r--r--   0        0        0     1078 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/examples/compute_energy2d.cpp
--rw-r--r--   0        0        0      369 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/examples/compute_grad.py
--rw-r--r--   0        0        0      382 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/examples/cpp.md
--rw-r--r--   0        0        0      123 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/examples/python.md
--rw-r--r--   0        0        0       72 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/examples.md
--rw-r--r--   0        0        0     5423 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/index.md
--rw-r--r--   0        0        0     4492 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/install/beskow.md
--rwxr-xr-x   0        0        0     1342 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/install/beskow_install_autotools.sh
--rwxr-xr-x   0        0        0     2173 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/install/beskow_install_fftw.sh
--rwxr-xr-x   0        0        0     2449 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/install/beskow_install_p3dfft.sh
--rwxr-xr-x   0        0        0     2215 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/install/beskow_install_pfft.sh
--rw-r--r--   0        0        0      886 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/install/blas_libs.md
--rw-r--r--   0        0        0     3678 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/install/fft_libs.md
--rw-r--r--   0        0        0     1166 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/install/froggy.md
--rwxr-xr-x   0        0        0     2283 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/install/install_fftw.sh
--rwxr-xr-x   0        0        0     2074 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/install/install_openblas.sh
--rwxr-xr-x   0        0        0     1751 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/install/install_p3dfft.sh
--rwxr-xr-x   0        0        0     1893 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/install/install_pfft.sh
--rw-r--r--   0        0        0     1825 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/install/occigen.md
--rw-r--r--   0        0        0       57 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/install/occigen_.pythranrc
--rw-r--r--   0        0        0      791 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/install/occigen_install_fftw3.sh
--rw-r--r--   0        0        0      336 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/install/occigen_install_p3dfft.sh
--rw-r--r--   0        0        0      226 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/install/occigen_install_pfft.sh
--rw-r--r--   0        0        0      524 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/install/occigen_setenv.sh
--rw-r--r--   0        0        0     1619 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/install/triolith.md
--rw-r--r--   0        0        0     2363 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/install.md
--rw-r--r--   0        0        0      150 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/ipynb/README_for_ipynb_writers.txt
--rw-r--r--   0        0        0     7868 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/ipynb/executed/tuto_fft2d_mpi.ipynb
--rw-r--r--   0        0        0     8839 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/ipynb/executed/tuto_fft2d_mpi_domain_decomp.ipynb
--rw-r--r--   0        0        0     9488 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/ipynb/executed/tuto_fft3d_mpi.ipynb
--rw-r--r--   0        0        0    16975 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/ipynb/executed/tuto_fft3d_mpi_domain_decomp.ipynb
--rw-r--r--   0        0        0     2777 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/ipynb/tuto_fft2d_seq.md
--rw-r--r--   0        0        0     2509 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/ipynb/tuto_fft3d_seq.md
--rw-r--r--   0        0        0    39338 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/logo.svg
--rw-r--r--   0        0        0     2304 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/overview.md
--rw-r--r--   0        0        0     1375 2024-02-10 15:13:22.947099 fluidfft-0.4.0rc1/doc/plugins.md
--rw-r--r--   0        0        0       69 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/to_do.md
--rw-r--r--   0        0        0      582 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/doc/tutorials.md
--rw-r--r--   0        0        0     2079 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/docker/Dockerfile
--rw-r--r--   0        0        0     1135 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/docker/Makefile
--rw-r--r--   0        0        0      618 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/docker/hgrc
--rw-r--r--   0        0        0       77 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/docker/pythranrc
--rw-r--r--   0        0        0     2055 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/meson.build
--rw-r--r--   0        0        0      655 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/meson.options
--rw-r--r--   0        0        0     7333 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/noxfile.py
--rw-r--r--   0        0        0   236165 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/pdm.lock
--rw-r--r--   0        0        0   378028 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/pixi.lock
--rw-r--r--   0        0        0     1630 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/pixi.toml
--rw-r--r--   0        0        0     1375 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/README.md
--rw-r--r--   0        0        0     1061 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/LICENSE
--rw-r--r--   0        0        0      169 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/README.md
--rw-r--r--   0        0        0      394 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/__init__.py
--rw-r--r--   0        0        0     2886 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/create_fake_mod_for_doc.py
--rw-r--r--   0        0        0      927 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/include_cy/base.pyx
--rw-r--r--   0        0        0      150 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/include_cy/base_mpi.pyx
--rw-r--r--   0        0        0     1689 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/include_cy/cpu.pxd
--rw-r--r--   0        0        0     6902 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/include_cy/util_pyfftw.pyx
--rw-r--r--   0        0        0     2602 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/make_cy_files.py
--rw-r--r--   0        0        0     5916 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft.cpp
--rw-r--r--   0        0        0     1864 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft.h
--rw-r--r--   0        0        0     1141 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft2d.cpp
--rw-r--r--   0        0        0      629 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft2d.h
--rw-r--r--   0        0        0      123 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft2dmpi.cpp
--rw-r--r--   0        0        0      218 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft2dmpi.h
--rw-r--r--   0        0        0     1916 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft3d.cpp
--rw-r--r--   0        0        0      886 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft3d.h
--rw-r--r--   0        0        0     2038 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft3dmpi.cpp
--rw-r--r--   0        0        0      522 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft3dmpi.h
--rw-r--r--   0        0        0      321 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fftmpi.cpp
--rw-r--r--   0        0        0      184 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fftmpi.h
--rw-r--r--   0        0        0     3432 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/src_cpp/cpu.h
--rw-r--r--   0        0        0      896 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/src_cpp/cpu_builtin.h
--rw-r--r--   0        0        0      736 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/src_cpp/mainpage.h
--rw-r--r--   0        0        0      285 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/src_cpp/mpi-compat.h
--rw-r--r--   0        0        0        0 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/templates/__init__.py
--rw-r--r--   0        0        0     1010 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/templates/template2d.pxd
--rw-r--r--   0        0        0     9974 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/templates/template2d.pyx
--rw-r--r--   0        0        0     1232 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/templates/template3d.pxd
--rw-r--r--   0        0        0    17358 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/templates/template3d.pyx
--rw-r--r--   0        0        0      695 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-builder/pyproject.toml
--rw-r--r--   0        0        0    35149 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftw/LICENSE
--rw-r--r--   0        0        0      112 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftw/Makefile
--rw-r--r--   0        0        0      165 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftw/README.md
--rw-r--r--   0        0        0      896 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftw/meson.build
--rw-r--r--   0        0        0      737 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftw/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftw/src/fluidfft_fftw/__init__.py
--rw-r--r--   0        0        0        0 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftw/src/fluidfft_fftw/fft2d/__init__.py
--rw-r--r--   0        0        0     6895 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftw/src/fluidfft_fftw/fft2d/fft2d_with_fftw1d.cpp
--rw-r--r--   0        0        0      680 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftw/src/fluidfft_fftw/fft2d/fft2d_with_fftw1d.h
--rw-r--r--   0        0        0     4538 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftw/src/fluidfft_fftw/fft2d/fft2d_with_fftw2d.cpp
--rw-r--r--   0        0        0      630 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftw/src/fluidfft_fftw/fft2d/fft2d_with_fftw2d.h
--rw-r--r--   0        0        0      901 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftw/src/fluidfft_fftw/fft2d/meson.build
--rw-r--r--   0        0        0        0 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftw/src/fluidfft_fftw/fft3d/__init__.py
--rw-r--r--   0        0        0     6873 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftw/src/fluidfft_fftw/fft3d/fft3d_with_fftw3d.cpp
--rw-r--r--   0        0        0      727 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftw/src/fluidfft_fftw/fft3d/fft3d_with_fftw3d.h
--rw-r--r--   0        0        0      770 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftw/src/fluidfft_fftw/fft3d/meson.build
--rw-r--r--   0        0        0      138 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftw/src/fluidfft_fftw/meson.build
--rw-r--r--   0        0        0      202 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftw/tests/test_2d.py
--rw-r--r--   0        0        0      176 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftw/tests/test_3d.py
--rw-r--r--   0        0        0    35149 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftwmpi/LICENSE
--rw-r--r--   0        0        0      128 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftwmpi/Makefile
--rw-r--r--   0        0        0      186 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftwmpi/README.md
--rw-r--r--   0        0        0     1257 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftwmpi/meson.build
--rw-r--r--   0        0        0      745 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftwmpi/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/__init__.py
--rw-r--r--   0        0        0        0 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/fft2d/__init__.py
--rw-r--r--   0        0        0     8193 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/fft2d/fft2dmpi_with_fftwmpi2d.cpp
--rw-r--r--   0        0        0      852 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/fft2d/fft2dmpi_with_fftwmpi2d.h
--rw-r--r--   0        0        0      965 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/fft2d/meson.build
--rw-r--r--   0        0        0        0 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/fft3d/__init__.py
--rw-r--r--   0        0        0     8937 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/fft3d/fft3dmpi_with_fftwmpi3d.cpp
--rw-r--r--   0        0        0      945 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/fft3d/fft3dmpi_with_fftwmpi3d.h
--rw-r--r--   0        0        0      965 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/fft3d/meson.build
--rw-r--r--   0        0        0      102 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/meson.build
--rw-r--r--   0        0        0      183 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftwmpi/tests/test_2d.py
--rw-r--r--   0        0        0      183 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-fftwmpi/tests/test_3d.py
--rw-r--r--   0        0        0     1080 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-mpi4pyfft/LICENSE
--rw-r--r--   0        0        0      659 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-mpi4pyfft/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-mpi4pyfft/src/fluidfft_mpi4pyfft/__init__.py
--rw-r--r--   0        0        0     4517 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-mpi4pyfft/src/fluidfft_mpi4pyfft/mpi_with_mpi4pyfft.py
--rw-r--r--   0        0        0      749 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-mpi4pyfft/src/fluidfft_mpi4pyfft/mpi_with_mpi4pyfft_slab.py
--rw-r--r--   0        0        0      262 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-mpi4pyfft/tests/test_with_mpi4pyfft.py
--rw-r--r--   0        0        0    35149 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-mpi_with_fftw/LICENSE
--rw-r--r--   0        0        0      128 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-mpi_with_fftw/Makefile
--rw-r--r--   0        0        0      165 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-mpi_with_fftw/README.md
--rw-r--r--   0        0        0      968 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-mpi_with_fftw/meson.build
--rw-r--r--   0        0        0      747 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-mpi_with_fftw/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/__init__.py
--rw-r--r--   0        0        0        0 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/fft2d/__init__.py
--rw-r--r--   0        0        0     6979 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/fft2d/fft2dmpi_with_fftw1d.cpp
--rw-r--r--   0        0        0      772 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/fft2d/fft2dmpi_with_fftw1d.h
--rw-r--r--   0        0        0      926 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/fft2d/meson.build
--rw-r--r--   0        0        0        0 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/fft3d/__init__.py
--rw-r--r--   0        0        0    12823 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/fft3d/fft3dmpi_with_fftw1d.cpp
--rw-r--r--   0        0        0     1186 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/fft3d/fft3dmpi_with_fftw1d.h
--rw-r--r--   0        0        0      927 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/fft3d/meson.build
--rw-r--r--   0        0        0      108 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/meson.build
--rw-r--r--   0        0        0      180 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-mpi_with_fftw/tests/test_2d.py
--rw-r--r--   0        0        0      180 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-mpi_with_fftw/tests/test_3d.py
--rw-r--r--   0        0        0    35149 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-p3dfft/LICENSE
--rw-r--r--   0        0        0      128 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-p3dfft/Makefile
--rw-r--r--   0        0        0      451 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-p3dfft/README.md
--rw-r--r--   0        0        0     2247 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-p3dfft/meson.build
--rw-r--r--   0        0        0      654 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-p3dfft/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-p3dfft/src/fluidfft_p3dfft/__init__.py
--rw-r--r--   0        0        0     8275 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-p3dfft/src/fluidfft_p3dfft/fft3dmpi_with_p3dfft.cpp
--rw-r--r--   0        0        0     1197 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-p3dfft/src/fluidfft_p3dfft/fft3dmpi_with_p3dfft.h
--rw-r--r--   0        0        0      907 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-p3dfft/src/fluidfft_p3dfft/meson.build
--rw-r--r--   0        0        0      180 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-p3dfft/tests/test_p3dfft.py
--rw-r--r--   0        0        0    35149 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-pfft/LICENSE
--rw-r--r--   0        0        0      128 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-pfft/Makefile
--rw-r--r--   0        0        0      439 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-pfft/README.md
--rw-r--r--   0        0        0     2193 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-pfft/meson.build
--rw-r--r--   0        0        0      646 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-pfft/pyproject.toml
--rw-r--r--   0        0        0        0 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-pfft/src/fluidfft_pfft/__init__.py
--rw-r--r--   0        0        0    11202 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-pfft/src/fluidfft_pfft/fft3dmpi_with_pfft.cpp
--rw-r--r--   0        0        0     1265 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-pfft/src/fluidfft_pfft/fft3dmpi_with_pfft.h
--rw-r--r--   0        0        0      885 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-pfft/src/fluidfft_pfft/meson.build
--rw-r--r--   0        0        0      263 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/fluidfft-pfft/tests/test_pfft.py
--rw-r--r--   0        0        0     2720 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/pure_cpp/2d/Makefile
--rw-r--r--   0        0        0      832 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/pure_cpp/2d/README.rst
--rw-r--r--   0        0        0       39 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/pure_cpp/2d/TODOLIST.rst
--rw-r--r--   0        0        0      996 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/pure_cpp/2d/plot_results.py
--rw-r--r--   0        0        0     2190 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/pure_cpp/2d/run_benchs.py
--rw-r--r--   0        0        0     1663 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/pure_cpp/2d/test_bench.cpp
--rw-r--r--   0        0        0     3618 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/pure_cpp/3d/Makefile
--rw-r--r--   0        0        0     3698 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/pure_cpp/3d/Makefile.beskow
--rw-r--r--   0        0        0     1428 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/pure_cpp/3d/README.rst
--rwxr-xr-x   0        0        0      556 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/pure_cpp/3d/launch.oar
--rw-r--r--   0        0        0     2118 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/plugins/pure_cpp/3d/test_bench.cpp
--rw-r--r--   0        0        0    11023 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/pylintrc
--rw-r--r--   0        0        0     4194 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/pyproject.toml
--rw-r--r--   0        0        0     7834 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/src/fluidfft/__init__.py
--rw-r--r--   0        0        0       76 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/src/fluidfft/_version.py
--rw-r--r--   0        0        0     1487 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/src/fluidfft/base.py
--rw-r--r--   0        0        0     7927 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/src/fluidfft/bench.py
--rw-r--r--   0        0        0     6628 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/src/fluidfft/bench_analysis.py
--rw-r--r--   0        0        0     1353 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/src/fluidfft/fft2d/__init__.py
--rw-r--r--   0        0        0      447 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/src/fluidfft/fft2d/meson.build
--rw-r--r--   0        0        0    26473 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/src/fluidfft/fft2d/operators.py
--rw-r--r--   0        0        0     5022 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/src/fluidfft/fft2d/testing.py
--rw-r--r--   0        0        0     3983 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/src/fluidfft/fft2d/with_dask.py
--rw-r--r--   0        0        0      833 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/src/fluidfft/fft2d/with_pyfftw.py
--rw-r--r--   0        0        0     1353 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/src/fluidfft/fft3d/__init__.py
--rw-r--r--   0        0        0    14337 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/src/fluidfft/fft3d/base.py
--rw-r--r--   0        0        0      442 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/src/fluidfft/fft3d/meson.build
--rw-r--r--   0        0        0    25839 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/src/fluidfft/fft3d/operators.py
--rw-r--r--   0        0        0     5630 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/src/fluidfft/fft3d/testing.py
--rw-r--r--   0        0        0      972 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/src/fluidfft/fft3d/with_pyfftw.py
--rw-r--r--   0        0        0      347 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/src/fluidfft/meson.build
--rw-r--r--   0        0        0     2324 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/src/fluidfft/util.py
--rw-r--r--   0        0        0      974 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/tests/test_2d.py
--rw-r--r--   0        0        0      885 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/tests/test_3d.py
--rw-r--r--   0        0        0     1128 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/tests/test_bench.py
--rw-r--r--   0        0        0     1005 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/tests/test_init.py
--rw-r--r--   0        0        0     1630 2024-02-10 14:15:54.000000 fluidfft-0.4.0rc1/tests/test_plugins.py
--rw-r--r--   0        0        0     7623 2024-02-10 15:13:23.292431 fluidfft-0.4.0rc1/PKG-INFO
+-rw-r--r--   0        0        0       58 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/.flake8
+-rw-r--r--   0        0        0       44 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/.github/pythranrc-windows
+-rw-r--r--   0        0        0     1570 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/.github/workflows/ci-linux.yml
+-rw-r--r--   0        0        0      705 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/.github/workflows/ci-pixi.yml
+-rw-r--r--   0        0        0     3178 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/.github/workflows/wheels.yml
+-rw-r--r--   0        0        0     3117 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/.gitlab-ci.yml
+-rw-r--r--   0        0        0     1271 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/.hgtags
+-rw-r--r--   0        0        0      492 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/.readthedocs.yml
+-rw-r--r--   0        0        0     2998 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/CHANGES.md
+-rw-r--r--   0        0        0     1262 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/CONTRIBUTING.md
+-rw-r--r--   0        0        0    21781 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/LICENSE.txt
+-rw-r--r--   0        0        0     1155 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/Makefile
+-rw-r--r--   0        0        0     5957 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/README.md
+-rw-r--r--   0        0        0      568 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/benchcpp2d.py
+-rw-r--r--   0        0        0      562 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/benchcpp3d.py
+-rw-r--r--   0        0        0      792 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/check_openmp.py
+-rw-r--r--   0        0        0     1147 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/compare_cypythran/Makefile
+-rw-r--r--   0        0        0     2664 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/compare_cypythran/bench.py
+-rw-r--r--   0        0        0     1665 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/compare_cypythran/grad_cy.pyx
+-rw-r--r--   0        0        0      306 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/compare_cypythran/grad_pythran.py
+-rw-r--r--   0        0        0      182 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/compare_cypythran/setup.py
+-rw-r--r--   0        0        0     1342 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/compare_mpi4py_fft/Makefile
+-rw-r--r--   0        0        0      752 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/compare_mpi4py_fft/bench.py
+-rw-r--r--   0        0        0     2644 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/compare_mpi4py_fft/transforms.py
+-rw-r--r--   0        0        0     1194 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/dask/try_dask_fft.py
+-rw-r--r--   0        0        0     4905 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/debug_mpi4py-fft/README.md
+-rw-r--r--   0        0        0      662 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/debug_mpi4py-fft/check_segfault.sh
+-rw-r--r--   0        0        0      531 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/debug_mpi4py-fft/prepare_env.sh
+-rw-r--r--   0        0        0      698 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/debug_mpi4py-fft/site.cfg.debug
+-rw-r--r--   0        0        0      342 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/issue14/README.md
+-rw-r--r--   0        0        0     3046 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/issue14/cpp/Makefile
+-rw-r--r--   0        0        0      815 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/issue14/cpp/main.cpp
+-rw-r--r--   0        0        0      492 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/issue14/investigate_segfault.py
+-rw-r--r--   0        0        0      798 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/issue14/investigate_small.py
+-rwxr-xr-x   0        0        0     1883 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/operator2d/Makefile
+-rw-r--r--   0        0        0     1354 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/operator2d/bench.py
+-rw-r--r--   0        0        0     1586 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/projperpk3d/Makefile
+-rw-r--r--   0        0        0     1859 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/projperpk3d/README.md
+-rw-r--r--   0        0        0      788 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/projperpk3d/bench.py
+-rw-r--r--   0        0        0     2735 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/projperpk3d/bench_proj_fortran.f90
+-rw-r--r--   0        0        0     1504 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/projperpk3d/proj.py
+-rw-r--r--   0        0        0     1404 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/projperpk3d/proj1.py
+-rw-r--r--   0        0        0     1545 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/projperpk3d/proj2.py
+-rw-r--r--   0        0        0     1495 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/projperpk3d_inplace/Makefile
+-rw-r--r--   0        0        0      132 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/projperpk3d_inplace/README.md
+-rw-r--r--   0        0        0      970 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/projperpk3d_inplace/bench.py
+-rw-r--r--   0        0        0     2224 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/projperpk3d_inplace/bench_proj_fortran.f90
+-rw-r--r--   0        0        0     1151 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/projperpk3d_inplace/proj.py
+-rwxr-xr-x   0        0        0     1860 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/pythran_implicit_loop/Makefile
+-rw-r--r--   0        0        0     2987 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/pythran_implicit_loop/README.md
+-rw-r--r--   0        0        0     1207 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/pythran_implicit_loop/bench.py
+-rw-r--r--   0        0        0      909 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/pythran_implicit_loop/mymod.py
+-rw-r--r--   0        0        0     2124 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/pythran_implicit_loop/pythran_issue807.md
+-rw-r--r--   0        0        0     1388 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/pythran_implicit_loop/results2d.txt
+-rw-r--r--   0        0        0     1252 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/pythran_implicit_loop/results2d_complex_hook_False.txt
+-rw-r--r--   0        0        0     1519 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/pythran_implicit_loop/results3d.txt
+-rw-r--r--   0        0        0      231 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/pythran_implicit_loop/work.py
+-rwxr-xr-x   0        0        0     3626 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/pythran_implicit_loop2/Makefile
+-rw-r--r--   0        0        0     3150 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/pythran_implicit_loop2/README.md
+-rw-r--r--   0        0        0      680 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/pythran_implicit_loop2/bench.py
+-rw-r--r--   0        0        0     1707 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/pythran_implicit_loop2/mymod.py
+-rw-r--r--   0        0        0     1819 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/pythran_implicit_loop2/results_with_gcc.txt
+-rw-r--r--   0        0        0      867 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/pythran_implicit_loop2/results_with_marchnative.txt
+-rw-r--r--   0        0        0      965 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/pythran_implicit_loop2/results_without_pythranrc.txt
+-rw-r--r--   0        0        0     4700 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/pythran_pep_func-not-avail-at-compile-time/README.md
+-rw-r--r--   0        0        0      376 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/pythran_pep_func-not-avail-at-compile-time/mymod.py
+-rwxr-xr-x   0        0        0     1094 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/submit_benchmarks2d_legi.py
+-rwxr-xr-x   0        0        0     1218 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/submit_benchmarks3d_legi.py
+-rwxr-xr-x   0        0        0      445 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/submit_benchmarks3d_occigen.py
+-rw-r--r--   0        0        0     1078 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/submit_benchmarks_legi.py
+-rwxr-xr-x   0        0        0     3157 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/submit_benchmarks_snic.py
+-rw-r--r--   0        0        0     3686 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/vector_product/Makefile
+-rw-r--r--   0        0        0     1599 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/vector_product/bench.py
+-rw-r--r--   0        0        0     2412 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/bench/vector_product/vectprod.py
+-rw-r--r--   0        0        0     5997 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/Makefile
+-rw-r--r--   0        0        0     3858 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/bench.md
+-rw-r--r--   0        0        0     8506 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/build-from-source.md
+-rw-r--r--   0        0        0     2998 2024-02-11 05:55:45.559628 fluidfft-0.4.0rc2/doc/changes.md
+-rw-r--r--   0        0        0    11664 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/conf.py
+-rw-r--r--   0        0        0   104172 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/doxygen/Doxyfile
+-rw-r--r--   0        0        0     3739 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/examples/Makefile
+-rw-r--r--   0        0        0     3279 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/examples/Makefile.2d
+-rw-r--r--   0        0        0     1237 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/examples/compute_energy.cpp
+-rw-r--r--   0        0        0     1078 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/examples/compute_energy2d.cpp
+-rw-r--r--   0        0        0      369 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/examples/compute_grad.py
+-rw-r--r--   0        0        0      382 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/examples/cpp.md
+-rw-r--r--   0        0        0      123 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/examples/python.md
+-rw-r--r--   0        0        0       72 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/examples.md
+-rw-r--r--   0        0        0     5423 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/index.md
+-rw-r--r--   0        0        0     4492 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/install/beskow.md
+-rwxr-xr-x   0        0        0     1342 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/install/beskow_install_autotools.sh
+-rwxr-xr-x   0        0        0     2173 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/install/beskow_install_fftw.sh
+-rwxr-xr-x   0        0        0     2449 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/install/beskow_install_p3dfft.sh
+-rwxr-xr-x   0        0        0     2215 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/install/beskow_install_pfft.sh
+-rw-r--r--   0        0        0      886 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/install/blas_libs.md
+-rw-r--r--   0        0        0     3678 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/install/fft_libs.md
+-rw-r--r--   0        0        0     1166 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/install/froggy.md
+-rwxr-xr-x   0        0        0     2283 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/install/install_fftw.sh
+-rwxr-xr-x   0        0        0     2074 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/install/install_openblas.sh
+-rwxr-xr-x   0        0        0     1751 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/install/install_p3dfft.sh
+-rwxr-xr-x   0        0        0     1893 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/install/install_pfft.sh
+-rw-r--r--   0        0        0     1825 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/install/occigen.md
+-rw-r--r--   0        0        0       57 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/install/occigen_.pythranrc
+-rw-r--r--   0        0        0      791 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/install/occigen_install_fftw3.sh
+-rw-r--r--   0        0        0      336 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/install/occigen_install_p3dfft.sh
+-rw-r--r--   0        0        0      226 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/install/occigen_install_pfft.sh
+-rw-r--r--   0        0        0      524 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/install/occigen_setenv.sh
+-rw-r--r--   0        0        0     1619 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/install/triolith.md
+-rw-r--r--   0        0        0     2363 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/install.md
+-rw-r--r--   0        0        0      150 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/ipynb/README_for_ipynb_writers.txt
+-rw-r--r--   0        0        0     7868 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/ipynb/executed/tuto_fft2d_mpi.ipynb
+-rw-r--r--   0        0        0     8839 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/ipynb/executed/tuto_fft2d_mpi_domain_decomp.ipynb
+-rw-r--r--   0        0        0     9488 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/ipynb/executed/tuto_fft3d_mpi.ipynb
+-rw-r--r--   0        0        0    16975 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/ipynb/executed/tuto_fft3d_mpi_domain_decomp.ipynb
+-rw-r--r--   0        0        0     2777 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/ipynb/tuto_fft2d_seq.md
+-rw-r--r--   0        0        0     2509 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/ipynb/tuto_fft3d_seq.md
+-rw-r--r--   0        0        0    39338 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/logo.svg
+-rw-r--r--   0        0        0     2304 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/overview.md
+-rw-r--r--   0        0        0     1375 2024-02-11 05:55:45.567628 fluidfft-0.4.0rc2/doc/plugins.md
+-rw-r--r--   0        0        0       69 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/to_do.md
+-rw-r--r--   0        0        0      582 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/doc/tutorials.md
+-rw-r--r--   0        0        0     2079 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/docker/Dockerfile
+-rw-r--r--   0        0        0     1135 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/docker/Makefile
+-rw-r--r--   0        0        0      618 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/docker/hgrc
+-rw-r--r--   0        0        0       77 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/docker/pythranrc
+-rw-r--r--   0        0        0     2055 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/meson.build
+-rw-r--r--   0        0        0      655 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/meson.options
+-rw-r--r--   0        0        0     7333 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/noxfile.py
+-rw-r--r--   0        0        0   236165 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/pdm.lock
+-rw-r--r--   0        0        0   378028 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/pixi.lock
+-rw-r--r--   0        0        0     1630 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/pixi.toml
+-rw-r--r--   0        0        0     1375 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/README.md
+-rw-r--r--   0        0        0     1061 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/LICENSE
+-rw-r--r--   0        0        0      169 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/README.md
+-rw-r--r--   0        0        0      394 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/__init__.py
+-rw-r--r--   0        0        0     2886 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/create_fake_mod_for_doc.py
+-rw-r--r--   0        0        0      927 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/include_cy/base.pyx
+-rw-r--r--   0        0        0      150 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/include_cy/base_mpi.pyx
+-rw-r--r--   0        0        0     1689 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/include_cy/cpu.pxd
+-rw-r--r--   0        0        0     6902 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/include_cy/util_pyfftw.pyx
+-rw-r--r--   0        0        0     2602 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/make_cy_files.py
+-rw-r--r--   0        0        0     5916 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft.cpp
+-rw-r--r--   0        0        0     1864 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft.h
+-rw-r--r--   0        0        0     1141 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft2d.cpp
+-rw-r--r--   0        0        0      629 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft2d.h
+-rw-r--r--   0        0        0      123 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft2dmpi.cpp
+-rw-r--r--   0        0        0      218 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft2dmpi.h
+-rw-r--r--   0        0        0     1916 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft3d.cpp
+-rw-r--r--   0        0        0      886 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft3d.h
+-rw-r--r--   0        0        0     2038 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft3dmpi.cpp
+-rw-r--r--   0        0        0      522 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft3dmpi.h
+-rw-r--r--   0        0        0      321 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fftmpi.cpp
+-rw-r--r--   0        0        0      184 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fftmpi.h
+-rw-r--r--   0        0        0     3432 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/src_cpp/cpu.h
+-rw-r--r--   0        0        0      896 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/src_cpp/cpu_builtin.h
+-rw-r--r--   0        0        0      736 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/src_cpp/mainpage.h
+-rw-r--r--   0        0        0      285 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/src_cpp/mpi-compat.h
+-rw-r--r--   0        0        0        0 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/templates/__init__.py
+-rw-r--r--   0        0        0     1010 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/templates/template2d.pxd
+-rw-r--r--   0        0        0     9974 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/templates/template2d.pyx
+-rw-r--r--   0        0        0     1232 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/templates/template3d.pxd
+-rw-r--r--   0        0        0    17358 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/templates/template3d.pyx
+-rw-r--r--   0        0        0      695 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-builder/pyproject.toml
+-rw-r--r--   0        0        0    35149 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftw/LICENSE
+-rw-r--r--   0        0        0      112 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftw/Makefile
+-rw-r--r--   0        0        0      165 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftw/README.md
+-rw-r--r--   0        0        0      896 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftw/meson.build
+-rw-r--r--   0        0        0      737 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftw/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftw/src/fluidfft_fftw/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftw/src/fluidfft_fftw/fft2d/__init__.py
+-rw-r--r--   0        0        0     6895 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftw/src/fluidfft_fftw/fft2d/fft2d_with_fftw1d.cpp
+-rw-r--r--   0        0        0      680 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftw/src/fluidfft_fftw/fft2d/fft2d_with_fftw1d.h
+-rw-r--r--   0        0        0     4538 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftw/src/fluidfft_fftw/fft2d/fft2d_with_fftw2d.cpp
+-rw-r--r--   0        0        0      630 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftw/src/fluidfft_fftw/fft2d/fft2d_with_fftw2d.h
+-rw-r--r--   0        0        0      901 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftw/src/fluidfft_fftw/fft2d/meson.build
+-rw-r--r--   0        0        0        0 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftw/src/fluidfft_fftw/fft3d/__init__.py
+-rw-r--r--   0        0        0     6873 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftw/src/fluidfft_fftw/fft3d/fft3d_with_fftw3d.cpp
+-rw-r--r--   0        0        0      727 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftw/src/fluidfft_fftw/fft3d/fft3d_with_fftw3d.h
+-rw-r--r--   0        0        0      770 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftw/src/fluidfft_fftw/fft3d/meson.build
+-rw-r--r--   0        0        0      138 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftw/src/fluidfft_fftw/meson.build
+-rw-r--r--   0        0        0      202 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftw/tests/test_2d.py
+-rw-r--r--   0        0        0      176 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftw/tests/test_3d.py
+-rw-r--r--   0        0        0    35149 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftwmpi/LICENSE
+-rw-r--r--   0        0        0      128 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftwmpi/Makefile
+-rw-r--r--   0        0        0      186 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftwmpi/README.md
+-rw-r--r--   0        0        0     1257 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftwmpi/meson.build
+-rw-r--r--   0        0        0      745 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftwmpi/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/fft2d/__init__.py
+-rw-r--r--   0        0        0     8193 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/fft2d/fft2dmpi_with_fftwmpi2d.cpp
+-rw-r--r--   0        0        0      852 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/fft2d/fft2dmpi_with_fftwmpi2d.h
+-rw-r--r--   0        0        0      965 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/fft2d/meson.build
+-rw-r--r--   0        0        0        0 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/fft3d/__init__.py
+-rw-r--r--   0        0        0     8937 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/fft3d/fft3dmpi_with_fftwmpi3d.cpp
+-rw-r--r--   0        0        0      945 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/fft3d/fft3dmpi_with_fftwmpi3d.h
+-rw-r--r--   0        0        0      965 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/fft3d/meson.build
+-rw-r--r--   0        0        0      102 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/meson.build
+-rw-r--r--   0        0        0      183 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftwmpi/tests/test_2d.py
+-rw-r--r--   0        0        0      183 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-fftwmpi/tests/test_3d.py
+-rw-r--r--   0        0        0     1080 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-mpi4pyfft/LICENSE
+-rw-r--r--   0        0        0      659 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-mpi4pyfft/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-mpi4pyfft/src/fluidfft_mpi4pyfft/__init__.py
+-rw-r--r--   0        0        0     4517 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-mpi4pyfft/src/fluidfft_mpi4pyfft/mpi_with_mpi4pyfft.py
+-rw-r--r--   0        0        0      749 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-mpi4pyfft/src/fluidfft_mpi4pyfft/mpi_with_mpi4pyfft_slab.py
+-rw-r--r--   0        0        0      262 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-mpi4pyfft/tests/test_with_mpi4pyfft.py
+-rw-r--r--   0        0        0    35149 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-mpi_with_fftw/LICENSE
+-rw-r--r--   0        0        0      128 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-mpi_with_fftw/Makefile
+-rw-r--r--   0        0        0      165 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-mpi_with_fftw/README.md
+-rw-r--r--   0        0        0      968 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-mpi_with_fftw/meson.build
+-rw-r--r--   0        0        0      747 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-mpi_with_fftw/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/fft2d/__init__.py
+-rw-r--r--   0        0        0     6979 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/fft2d/fft2dmpi_with_fftw1d.cpp
+-rw-r--r--   0        0        0      772 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/fft2d/fft2dmpi_with_fftw1d.h
+-rw-r--r--   0        0        0      926 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/fft2d/meson.build
+-rw-r--r--   0        0        0        0 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/fft3d/__init__.py
+-rw-r--r--   0        0        0    12823 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/fft3d/fft3dmpi_with_fftw1d.cpp
+-rw-r--r--   0        0        0     1186 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/fft3d/fft3dmpi_with_fftw1d.h
+-rw-r--r--   0        0        0      927 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/fft3d/meson.build
+-rw-r--r--   0        0        0      108 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/meson.build
+-rw-r--r--   0        0        0      180 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-mpi_with_fftw/tests/test_2d.py
+-rw-r--r--   0        0        0      180 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-mpi_with_fftw/tests/test_3d.py
+-rw-r--r--   0        0        0    35149 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-p3dfft/LICENSE
+-rw-r--r--   0        0        0      128 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-p3dfft/Makefile
+-rw-r--r--   0        0        0      451 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-p3dfft/README.md
+-rw-r--r--   0        0        0     2247 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-p3dfft/meson.build
+-rw-r--r--   0        0        0      654 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-p3dfft/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-p3dfft/src/fluidfft_p3dfft/__init__.py
+-rw-r--r--   0        0        0     8275 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-p3dfft/src/fluidfft_p3dfft/fft3dmpi_with_p3dfft.cpp
+-rw-r--r--   0        0        0     1197 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-p3dfft/src/fluidfft_p3dfft/fft3dmpi_with_p3dfft.h
+-rw-r--r--   0        0        0      907 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-p3dfft/src/fluidfft_p3dfft/meson.build
+-rw-r--r--   0        0        0      180 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-p3dfft/tests/test_p3dfft.py
+-rw-r--r--   0        0        0    35149 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-pfft/LICENSE
+-rw-r--r--   0        0        0      128 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-pfft/Makefile
+-rw-r--r--   0        0        0      439 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-pfft/README.md
+-rw-r--r--   0        0        0     2193 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-pfft/meson.build
+-rw-r--r--   0        0        0      646 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-pfft/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-pfft/src/fluidfft_pfft/__init__.py
+-rw-r--r--   0        0        0    11202 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-pfft/src/fluidfft_pfft/fft3dmpi_with_pfft.cpp
+-rw-r--r--   0        0        0     1265 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-pfft/src/fluidfft_pfft/fft3dmpi_with_pfft.h
+-rw-r--r--   0        0        0      885 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-pfft/src/fluidfft_pfft/meson.build
+-rw-r--r--   0        0        0      263 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/fluidfft-pfft/tests/test_pfft.py
+-rw-r--r--   0        0        0     2720 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/pure_cpp/2d/Makefile
+-rw-r--r--   0        0        0      832 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/pure_cpp/2d/README.rst
+-rw-r--r--   0        0        0       39 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/pure_cpp/2d/TODOLIST.rst
+-rw-r--r--   0        0        0      996 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/pure_cpp/2d/plot_results.py
+-rw-r--r--   0        0        0     2190 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/pure_cpp/2d/run_benchs.py
+-rw-r--r--   0        0        0     1663 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/pure_cpp/2d/test_bench.cpp
+-rw-r--r--   0        0        0     3618 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/pure_cpp/3d/Makefile
+-rw-r--r--   0        0        0     3698 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/pure_cpp/3d/Makefile.beskow
+-rw-r--r--   0        0        0     1428 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/pure_cpp/3d/README.rst
+-rwxr-xr-x   0        0        0      556 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/pure_cpp/3d/launch.oar
+-rw-r--r--   0        0        0     2118 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/plugins/pure_cpp/3d/test_bench.cpp
+-rw-r--r--   0        0        0    11023 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/pylintrc
+-rw-r--r--   0        0        0     4194 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     7834 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/src/fluidfft/__init__.py
+-rw-r--r--   0        0        0       76 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/src/fluidfft/_version.py
+-rw-r--r--   0        0        0     1487 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/src/fluidfft/base.py
+-rw-r--r--   0        0        0     7927 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/src/fluidfft/bench.py
+-rw-r--r--   0        0        0     6628 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/src/fluidfft/bench_analysis.py
+-rw-r--r--   0        0        0     1374 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/src/fluidfft/fft2d/__init__.py
+-rw-r--r--   0        0        0      447 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/src/fluidfft/fft2d/meson.build
+-rw-r--r--   0        0        0    26473 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/src/fluidfft/fft2d/operators.py
+-rw-r--r--   0        0        0     5022 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/src/fluidfft/fft2d/testing.py
+-rw-r--r--   0        0        0     3983 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/src/fluidfft/fft2d/with_dask.py
+-rw-r--r--   0        0        0      833 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/src/fluidfft/fft2d/with_pyfftw.py
+-rw-r--r--   0        0        0     1374 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/src/fluidfft/fft3d/__init__.py
+-rw-r--r--   0        0        0    14337 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/src/fluidfft/fft3d/base.py
+-rw-r--r--   0        0        0      442 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/src/fluidfft/fft3d/meson.build
+-rw-r--r--   0        0        0    25839 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/src/fluidfft/fft3d/operators.py
+-rw-r--r--   0        0        0     5630 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/src/fluidfft/fft3d/testing.py
+-rw-r--r--   0        0        0      972 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/src/fluidfft/fft3d/with_pyfftw.py
+-rw-r--r--   0        0        0      347 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/src/fluidfft/meson.build
+-rw-r--r--   0        0        0     2324 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/src/fluidfft/util.py
+-rw-r--r--   0        0        0      974 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/tests/test_2d.py
+-rw-r--r--   0        0        0      885 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/tests/test_3d.py
+-rw-r--r--   0        0        0     1128 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/tests/test_bench.py
+-rw-r--r--   0        0        0     1005 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/tests/test_init.py
+-rw-r--r--   0        0        0     1630 2024-02-11 05:48:00.000000 fluidfft-0.4.0rc2/tests/test_plugins.py
+-rw-r--r--   0        0        0     7623 2024-02-11 05:55:45.922574 fluidfft-0.4.0rc2/PKG-INFO
```

### Comparing `fluidfft-0.4.0rc1/.github/workflows/ci-linux.yml` & `fluidfft-0.4.0rc2/.github/workflows/ci-linux.yml`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/.github/workflows/ci-pixi.yml` & `fluidfft-0.4.0rc2/.github/workflows/ci-pixi.yml`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/.github/workflows/wheels.yml` & `fluidfft-0.4.0rc2/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/.gitlab-ci.yml` & `fluidfft-0.4.0rc2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/.hgtags` & `fluidfft-0.4.0rc2/.hgtags`

 * *Files 8% similar despite different names*

```diff
@@ -19,7 +19,8 @@
 e302f26f53694b8fbd1f13f4555758954f3b7df6 0.3.0
 3429428ab5eb3fce259b05a85c7d4c998c12fb2a 0.3.1
 12ba3b547a45db626ffcd18edd56914f7c50a435 0.3.2
 28eb25600d6e3e87508743ba97d676151c1f27ba 0.3.3
 e886db1ed3779bfdaed891b524a363cf3839a61d 0.3.4
 ca39f64d2f123fda4f26c3bf23b68e893f073d61 0.3.5
 5b3029b088f9867167d2bb4121ebf023406375b2 0.4.0rc0
+399eed881f7046b560432f1d206adb9d18e66b87 0.4.0rc1
```

### Comparing `fluidfft-0.4.0rc1/CHANGES.md` & `fluidfft-0.4.0rc2/CHANGES.md`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/CONTRIBUTING.md` & `fluidfft-0.4.0rc2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/LICENSE.txt` & `fluidfft-0.4.0rc2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/Makefile` & `fluidfft-0.4.0rc2/Makefile`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/README.md` & `fluidfft-0.4.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/benchcpp2d.py` & `fluidfft-0.4.0rc2/bench/benchcpp2d.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/benchcpp3d.py` & `fluidfft-0.4.0rc2/bench/benchcpp3d.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/check_openmp.py` & `fluidfft-0.4.0rc2/bench/check_openmp.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/compare_cypythran/Makefile` & `fluidfft-0.4.0rc2/bench/compare_cypythran/Makefile`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/compare_cypythran/bench.py` & `fluidfft-0.4.0rc2/bench/compare_cypythran/bench.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/compare_cypythran/grad_cy.pyx` & `fluidfft-0.4.0rc2/bench/compare_cypythran/grad_cy.pyx`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/compare_mpi4py_fft/Makefile` & `fluidfft-0.4.0rc2/bench/compare_mpi4py_fft/Makefile`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/compare_mpi4py_fft/bench.py` & `fluidfft-0.4.0rc2/bench/compare_mpi4py_fft/bench.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/compare_mpi4py_fft/transforms.py` & `fluidfft-0.4.0rc2/bench/compare_mpi4py_fft/transforms.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/dask/try_dask_fft.py` & `fluidfft-0.4.0rc2/bench/dask/try_dask_fft.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/debug_mpi4py-fft/README.md` & `fluidfft-0.4.0rc2/bench/debug_mpi4py-fft/README.md`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/debug_mpi4py-fft/check_segfault.sh` & `fluidfft-0.4.0rc2/bench/debug_mpi4py-fft/check_segfault.sh`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/debug_mpi4py-fft/prepare_env.sh` & `fluidfft-0.4.0rc2/bench/debug_mpi4py-fft/prepare_env.sh`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/debug_mpi4py-fft/site.cfg.debug` & `fluidfft-0.4.0rc2/bench/debug_mpi4py-fft/site.cfg.debug`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/issue14/cpp/Makefile` & `fluidfft-0.4.0rc2/bench/issue14/cpp/Makefile`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/issue14/cpp/main.cpp` & `fluidfft-0.4.0rc2/bench/issue14/cpp/main.cpp`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/issue14/investigate_small.py` & `fluidfft-0.4.0rc2/bench/issue14/investigate_small.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/operator2d/Makefile` & `fluidfft-0.4.0rc2/bench/operator2d/Makefile`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/operator2d/bench.py` & `fluidfft-0.4.0rc2/bench/operator2d/bench.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/projperpk3d/Makefile` & `fluidfft-0.4.0rc2/bench/projperpk3d/Makefile`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/projperpk3d/README.md` & `fluidfft-0.4.0rc2/bench/projperpk3d/README.md`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/projperpk3d/bench.py` & `fluidfft-0.4.0rc2/bench/projperpk3d/bench.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/projperpk3d/bench_proj_fortran.f90` & `fluidfft-0.4.0rc2/bench/projperpk3d/bench_proj_fortran.f90`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/projperpk3d/proj.py` & `fluidfft-0.4.0rc2/bench/projperpk3d/proj.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/projperpk3d/proj1.py` & `fluidfft-0.4.0rc2/bench/projperpk3d/proj1.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/projperpk3d/proj2.py` & `fluidfft-0.4.0rc2/bench/projperpk3d/proj2.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/projperpk3d_inplace/Makefile` & `fluidfft-0.4.0rc2/bench/projperpk3d_inplace/Makefile`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/projperpk3d_inplace/bench.py` & `fluidfft-0.4.0rc2/bench/projperpk3d_inplace/bench.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/projperpk3d_inplace/bench_proj_fortran.f90` & `fluidfft-0.4.0rc2/bench/projperpk3d_inplace/bench_proj_fortran.f90`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/projperpk3d_inplace/proj.py` & `fluidfft-0.4.0rc2/bench/projperpk3d_inplace/proj.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/pythran_implicit_loop/Makefile` & `fluidfft-0.4.0rc2/bench/pythran_implicit_loop/Makefile`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/pythran_implicit_loop/README.md` & `fluidfft-0.4.0rc2/bench/pythran_implicit_loop/README.md`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/pythran_implicit_loop/bench.py` & `fluidfft-0.4.0rc2/bench/pythran_implicit_loop/bench.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/pythran_implicit_loop/mymod.py` & `fluidfft-0.4.0rc2/bench/pythran_implicit_loop/mymod.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/pythran_implicit_loop/pythran_issue807.md` & `fluidfft-0.4.0rc2/bench/pythran_implicit_loop/pythran_issue807.md`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/pythran_implicit_loop/results2d.txt` & `fluidfft-0.4.0rc2/bench/pythran_implicit_loop/results2d.txt`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/pythran_implicit_loop/results2d_complex_hook_False.txt` & `fluidfft-0.4.0rc2/bench/pythran_implicit_loop/results2d_complex_hook_False.txt`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/pythran_implicit_loop/results3d.txt` & `fluidfft-0.4.0rc2/bench/pythran_implicit_loop/results3d.txt`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/pythran_implicit_loop2/Makefile` & `fluidfft-0.4.0rc2/bench/pythran_implicit_loop2/Makefile`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/pythran_implicit_loop2/README.md` & `fluidfft-0.4.0rc2/bench/pythran_implicit_loop2/README.md`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/pythran_implicit_loop2/bench.py` & `fluidfft-0.4.0rc2/bench/pythran_implicit_loop2/bench.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/pythran_implicit_loop2/mymod.py` & `fluidfft-0.4.0rc2/bench/pythran_implicit_loop2/mymod.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/pythran_implicit_loop2/results_with_gcc.txt` & `fluidfft-0.4.0rc2/bench/pythran_implicit_loop2/results_with_gcc.txt`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/pythran_implicit_loop2/results_with_marchnative.txt` & `fluidfft-0.4.0rc2/bench/pythran_implicit_loop2/results_with_marchnative.txt`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/pythran_implicit_loop2/results_without_pythranrc.txt` & `fluidfft-0.4.0rc2/bench/pythran_implicit_loop2/results_without_pythranrc.txt`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/pythran_pep_func-not-avail-at-compile-time/README.md` & `fluidfft-0.4.0rc2/bench/pythran_pep_func-not-avail-at-compile-time/README.md`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/submit_benchmarks2d_legi.py` & `fluidfft-0.4.0rc2/bench/submit_benchmarks2d_legi.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/submit_benchmarks3d_legi.py` & `fluidfft-0.4.0rc2/bench/submit_benchmarks3d_legi.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/submit_benchmarks_legi.py` & `fluidfft-0.4.0rc2/bench/submit_benchmarks_legi.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/submit_benchmarks_snic.py` & `fluidfft-0.4.0rc2/bench/submit_benchmarks_snic.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/vector_product/Makefile` & `fluidfft-0.4.0rc2/bench/vector_product/Makefile`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/vector_product/bench.py` & `fluidfft-0.4.0rc2/bench/vector_product/bench.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/bench/vector_product/vectprod.py` & `fluidfft-0.4.0rc2/bench/vector_product/vectprod.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/Makefile` & `fluidfft-0.4.0rc2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/bench.md` & `fluidfft-0.4.0rc2/doc/bench.md`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/build-from-source.md` & `fluidfft-0.4.0rc2/doc/build-from-source.md`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/changes.md` & `fluidfft-0.4.0rc2/doc/changes.md`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/conf.py` & `fluidfft-0.4.0rc2/doc/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,17 @@
 mpl.use("Agg")
 import matplotlib.pyplot as plt
 
 plt.ioff()
 
 from fluiddyn.util import modification_date
 
+os.environ["FLUIDFFT_BUILD_DOC"] = "1"
+
+
 import fluidfft
 import fluidfft.bench_analysis
 from fluidfft.bench_analysis import plot_scaling
 
 here = os.path.dirname(__file__)
 here_tmp = os.path.join(here, "tmp")
 html = os.path.join(here, "_build/html")
```

### Comparing `fluidfft-0.4.0rc1/doc/doxygen/Doxyfile` & `fluidfft-0.4.0rc2/doc/doxygen/Doxyfile`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/examples/Makefile` & `fluidfft-0.4.0rc2/doc/examples/Makefile`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/examples/Makefile.2d` & `fluidfft-0.4.0rc2/doc/examples/Makefile.2d`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/examples/compute_energy.cpp` & `fluidfft-0.4.0rc2/doc/examples/compute_energy.cpp`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/examples/compute_energy2d.cpp` & `fluidfft-0.4.0rc2/doc/examples/compute_energy2d.cpp`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/index.md` & `fluidfft-0.4.0rc2/doc/index.md`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/install/beskow.md` & `fluidfft-0.4.0rc2/doc/install/beskow.md`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/install/beskow_install_autotools.sh` & `fluidfft-0.4.0rc2/doc/install/beskow_install_autotools.sh`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/install/beskow_install_fftw.sh` & `fluidfft-0.4.0rc2/doc/install/beskow_install_fftw.sh`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/install/beskow_install_p3dfft.sh` & `fluidfft-0.4.0rc2/doc/install/beskow_install_p3dfft.sh`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/install/beskow_install_pfft.sh` & `fluidfft-0.4.0rc2/doc/install/beskow_install_pfft.sh`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/install/blas_libs.md` & `fluidfft-0.4.0rc2/doc/install/blas_libs.md`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/install/fft_libs.md` & `fluidfft-0.4.0rc2/doc/install/fft_libs.md`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/install/froggy.md` & `fluidfft-0.4.0rc2/doc/install/froggy.md`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/install/install_fftw.sh` & `fluidfft-0.4.0rc2/doc/install/install_fftw.sh`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/install/install_openblas.sh` & `fluidfft-0.4.0rc2/doc/install/install_openblas.sh`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/install/install_p3dfft.sh` & `fluidfft-0.4.0rc2/doc/install/install_p3dfft.sh`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/install/install_pfft.sh` & `fluidfft-0.4.0rc2/doc/install/install_pfft.sh`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/install/occigen.md` & `fluidfft-0.4.0rc2/doc/install/occigen.md`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/install/occigen_install_fftw3.sh` & `fluidfft-0.4.0rc2/doc/install/occigen_install_fftw3.sh`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/install/occigen_setenv.sh` & `fluidfft-0.4.0rc2/doc/install/occigen_setenv.sh`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/install/triolith.md` & `fluidfft-0.4.0rc2/doc/install/triolith.md`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/install.md` & `fluidfft-0.4.0rc2/doc/install.md`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/ipynb/executed/tuto_fft2d_mpi.ipynb` & `fluidfft-0.4.0rc2/doc/ipynb/executed/tuto_fft2d_mpi.ipynb`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/ipynb/executed/tuto_fft2d_mpi_domain_decomp.ipynb` & `fluidfft-0.4.0rc2/doc/ipynb/executed/tuto_fft2d_mpi_domain_decomp.ipynb`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/ipynb/executed/tuto_fft3d_mpi.ipynb` & `fluidfft-0.4.0rc2/doc/ipynb/executed/tuto_fft3d_mpi.ipynb`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/ipynb/executed/tuto_fft3d_mpi_domain_decomp.ipynb` & `fluidfft-0.4.0rc2/doc/ipynb/executed/tuto_fft3d_mpi_domain_decomp.ipynb`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/ipynb/tuto_fft2d_seq.md` & `fluidfft-0.4.0rc2/doc/ipynb/tuto_fft2d_seq.md`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/ipynb/tuto_fft3d_seq.md` & `fluidfft-0.4.0rc2/doc/ipynb/tuto_fft3d_seq.md`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/logo.svg` & `fluidfft-0.4.0rc2/doc/logo.svg`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/overview.md` & `fluidfft-0.4.0rc2/doc/overview.md`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/plugins.md` & `fluidfft-0.4.0rc2/doc/plugins.md`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/doc/tutorials.md` & `fluidfft-0.4.0rc2/doc/tutorials.md`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/docker/Dockerfile` & `fluidfft-0.4.0rc2/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/docker/Makefile` & `fluidfft-0.4.0rc2/docker/Makefile`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/docker/hgrc` & `fluidfft-0.4.0rc2/docker/hgrc`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/meson.build` & `fluidfft-0.4.0rc2/meson.build`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/meson.options` & `fluidfft-0.4.0rc2/meson.options`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/noxfile.py` & `fluidfft-0.4.0rc2/noxfile.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/pdm.lock` & `fluidfft-0.4.0rc2/pdm.lock`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/pixi.lock` & `fluidfft-0.4.0rc2/pixi.lock`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/pixi.toml` & `fluidfft-0.4.0rc2/pixi.toml`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/README.md` & `fluidfft-0.4.0rc2/plugins/README.md`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-builder/LICENSE` & `fluidfft-0.4.0rc2/plugins/fluidfft-builder/LICENSE`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/create_fake_mod_for_doc.py` & `fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/create_fake_mod_for_doc.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/include_cy/base.pyx` & `fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/include_cy/base.pyx`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/include_cy/cpu.pxd` & `fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/include_cy/cpu.pxd`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/include_cy/util_pyfftw.pyx` & `fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/include_cy/util_pyfftw.pyx`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/make_cy_files.py` & `fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/make_cy_files.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft.cpp` & `fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft.cpp`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft.h` & `fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft.h`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft2d.cpp` & `fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft2d.cpp`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft2d.h` & `fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft2d.h`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft3d.cpp` & `fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft3d.cpp`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft3d.h` & `fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft3d.h`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft3dmpi.cpp` & `fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft3dmpi.cpp`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft3dmpi.h` & `fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/src_cpp/base_fft3dmpi.h`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/src_cpp/cpu.h` & `fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/src_cpp/cpu.h`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/src_cpp/cpu_builtin.h` & `fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/src_cpp/cpu_builtin.h`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/src_cpp/mainpage.h` & `fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/src_cpp/mainpage.h`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/templates/template2d.pxd` & `fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/templates/template2d.pxd`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/templates/template2d.pyx` & `fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/templates/template2d.pyx`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/templates/template3d.pxd` & `fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/templates/template3d.pxd`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-builder/fluidfft_builder/templates/template3d.pyx` & `fluidfft-0.4.0rc2/plugins/fluidfft-builder/fluidfft_builder/templates/template3d.pyx`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-builder/pyproject.toml` & `fluidfft-0.4.0rc2/plugins/fluidfft-builder/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-fftw/LICENSE` & `fluidfft-0.4.0rc2/plugins/fluidfft-fftw/LICENSE`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-fftw/meson.build` & `fluidfft-0.4.0rc2/plugins/fluidfft-fftw/meson.build`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-fftw/pyproject.toml` & `fluidfft-0.4.0rc2/plugins/fluidfft-fftw/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-fftw/src/fluidfft_fftw/fft2d/fft2d_with_fftw1d.cpp` & `fluidfft-0.4.0rc2/plugins/fluidfft-fftw/src/fluidfft_fftw/fft2d/fft2d_with_fftw1d.cpp`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-fftw/src/fluidfft_fftw/fft2d/fft2d_with_fftw1d.h` & `fluidfft-0.4.0rc2/plugins/fluidfft-fftw/src/fluidfft_fftw/fft2d/fft2d_with_fftw1d.h`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-fftw/src/fluidfft_fftw/fft2d/fft2d_with_fftw2d.cpp` & `fluidfft-0.4.0rc2/plugins/fluidfft-fftw/src/fluidfft_fftw/fft2d/fft2d_with_fftw2d.cpp`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-fftw/src/fluidfft_fftw/fft2d/fft2d_with_fftw2d.h` & `fluidfft-0.4.0rc2/plugins/fluidfft-fftw/src/fluidfft_fftw/fft2d/fft2d_with_fftw2d.h`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-fftw/src/fluidfft_fftw/fft2d/meson.build` & `fluidfft-0.4.0rc2/plugins/fluidfft-fftw/src/fluidfft_fftw/fft2d/meson.build`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-fftw/src/fluidfft_fftw/fft3d/fft3d_with_fftw3d.cpp` & `fluidfft-0.4.0rc2/plugins/fluidfft-fftw/src/fluidfft_fftw/fft3d/fft3d_with_fftw3d.cpp`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-fftw/src/fluidfft_fftw/fft3d/fft3d_with_fftw3d.h` & `fluidfft-0.4.0rc2/plugins/fluidfft-fftw/src/fluidfft_fftw/fft3d/fft3d_with_fftw3d.h`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-fftw/src/fluidfft_fftw/fft3d/meson.build` & `fluidfft-0.4.0rc2/plugins/fluidfft-fftw/src/fluidfft_fftw/fft3d/meson.build`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-fftwmpi/LICENSE` & `fluidfft-0.4.0rc2/plugins/fluidfft-fftwmpi/LICENSE`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-fftwmpi/meson.build` & `fluidfft-0.4.0rc2/plugins/fluidfft-fftwmpi/meson.build`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-fftwmpi/pyproject.toml` & `fluidfft-0.4.0rc2/plugins/fluidfft-fftwmpi/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/fft2d/fft2dmpi_with_fftwmpi2d.cpp` & `fluidfft-0.4.0rc2/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/fft2d/fft2dmpi_with_fftwmpi2d.cpp`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/fft2d/fft2dmpi_with_fftwmpi2d.h` & `fluidfft-0.4.0rc2/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/fft2d/fft2dmpi_with_fftwmpi2d.h`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/fft2d/meson.build` & `fluidfft-0.4.0rc2/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/fft2d/meson.build`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/fft3d/fft3dmpi_with_fftwmpi3d.cpp` & `fluidfft-0.4.0rc2/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/fft3d/fft3dmpi_with_fftwmpi3d.cpp`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/fft3d/fft3dmpi_with_fftwmpi3d.h` & `fluidfft-0.4.0rc2/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/fft3d/fft3dmpi_with_fftwmpi3d.h`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/fft3d/meson.build` & `fluidfft-0.4.0rc2/plugins/fluidfft-fftwmpi/src/fluidfft_fftwmpi/fft3d/meson.build`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-mpi4pyfft/LICENSE` & `fluidfft-0.4.0rc2/plugins/fluidfft-mpi4pyfft/LICENSE`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-mpi4pyfft/pyproject.toml` & `fluidfft-0.4.0rc2/plugins/fluidfft-mpi4pyfft/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-mpi4pyfft/src/fluidfft_mpi4pyfft/mpi_with_mpi4pyfft.py` & `fluidfft-0.4.0rc2/plugins/fluidfft-mpi4pyfft/src/fluidfft_mpi4pyfft/mpi_with_mpi4pyfft.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-mpi4pyfft/src/fluidfft_mpi4pyfft/mpi_with_mpi4pyfft_slab.py` & `fluidfft-0.4.0rc2/plugins/fluidfft-mpi4pyfft/src/fluidfft_mpi4pyfft/mpi_with_mpi4pyfft_slab.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-mpi_with_fftw/LICENSE` & `fluidfft-0.4.0rc2/plugins/fluidfft-mpi_with_fftw/LICENSE`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-mpi_with_fftw/meson.build` & `fluidfft-0.4.0rc2/plugins/fluidfft-mpi_with_fftw/meson.build`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-mpi_with_fftw/pyproject.toml` & `fluidfft-0.4.0rc2/plugins/fluidfft-mpi_with_fftw/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/fft2d/fft2dmpi_with_fftw1d.cpp` & `fluidfft-0.4.0rc2/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/fft2d/fft2dmpi_with_fftw1d.cpp`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/fft2d/fft2dmpi_with_fftw1d.h` & `fluidfft-0.4.0rc2/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/fft2d/fft2dmpi_with_fftw1d.h`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/fft2d/meson.build` & `fluidfft-0.4.0rc2/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/fft2d/meson.build`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/fft3d/fft3dmpi_with_fftw1d.cpp` & `fluidfft-0.4.0rc2/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/fft3d/fft3dmpi_with_fftw1d.cpp`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/fft3d/fft3dmpi_with_fftw1d.h` & `fluidfft-0.4.0rc2/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/fft3d/fft3dmpi_with_fftw1d.h`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/fft3d/meson.build` & `fluidfft-0.4.0rc2/plugins/fluidfft-mpi_with_fftw/src/fluidfft_mpi_with_fftw/fft3d/meson.build`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-p3dfft/LICENSE` & `fluidfft-0.4.0rc2/plugins/fluidfft-p3dfft/LICENSE`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-p3dfft/meson.build` & `fluidfft-0.4.0rc2/plugins/fluidfft-p3dfft/meson.build`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-p3dfft/pyproject.toml` & `fluidfft-0.4.0rc2/plugins/fluidfft-p3dfft/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-p3dfft/src/fluidfft_p3dfft/fft3dmpi_with_p3dfft.cpp` & `fluidfft-0.4.0rc2/plugins/fluidfft-p3dfft/src/fluidfft_p3dfft/fft3dmpi_with_p3dfft.cpp`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-p3dfft/src/fluidfft_p3dfft/fft3dmpi_with_p3dfft.h` & `fluidfft-0.4.0rc2/plugins/fluidfft-p3dfft/src/fluidfft_p3dfft/fft3dmpi_with_p3dfft.h`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-p3dfft/src/fluidfft_p3dfft/meson.build` & `fluidfft-0.4.0rc2/plugins/fluidfft-p3dfft/src/fluidfft_p3dfft/meson.build`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-pfft/LICENSE` & `fluidfft-0.4.0rc2/plugins/fluidfft-pfft/LICENSE`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-pfft/meson.build` & `fluidfft-0.4.0rc2/plugins/fluidfft-pfft/meson.build`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-pfft/pyproject.toml` & `fluidfft-0.4.0rc2/plugins/fluidfft-pfft/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-pfft/src/fluidfft_pfft/fft3dmpi_with_pfft.cpp` & `fluidfft-0.4.0rc2/plugins/fluidfft-pfft/src/fluidfft_pfft/fft3dmpi_with_pfft.cpp`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-pfft/src/fluidfft_pfft/fft3dmpi_with_pfft.h` & `fluidfft-0.4.0rc2/plugins/fluidfft-pfft/src/fluidfft_pfft/fft3dmpi_with_pfft.h`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/fluidfft-pfft/src/fluidfft_pfft/meson.build` & `fluidfft-0.4.0rc2/plugins/fluidfft-pfft/src/fluidfft_pfft/meson.build`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/pure_cpp/2d/Makefile` & `fluidfft-0.4.0rc2/plugins/pure_cpp/2d/Makefile`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/pure_cpp/2d/README.rst` & `fluidfft-0.4.0rc2/plugins/pure_cpp/2d/README.rst`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/pure_cpp/2d/plot_results.py` & `fluidfft-0.4.0rc2/plugins/pure_cpp/2d/plot_results.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/pure_cpp/2d/run_benchs.py` & `fluidfft-0.4.0rc2/plugins/pure_cpp/2d/run_benchs.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/pure_cpp/2d/test_bench.cpp` & `fluidfft-0.4.0rc2/plugins/pure_cpp/2d/test_bench.cpp`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/pure_cpp/3d/Makefile` & `fluidfft-0.4.0rc2/plugins/pure_cpp/3d/Makefile`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/pure_cpp/3d/Makefile.beskow` & `fluidfft-0.4.0rc2/plugins/pure_cpp/3d/Makefile.beskow`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/pure_cpp/3d/README.rst` & `fluidfft-0.4.0rc2/plugins/pure_cpp/3d/README.rst`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/pure_cpp/3d/launch.oar` & `fluidfft-0.4.0rc2/plugins/pure_cpp/3d/launch.oar`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/plugins/pure_cpp/3d/test_bench.cpp` & `fluidfft-0.4.0rc2/plugins/pure_cpp/3d/test_bench.cpp`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/pylintrc` & `fluidfft-0.4.0rc2/pylintrc`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/pyproject.toml` & `fluidfft-0.4.0rc2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["meson-python", "numpy", "transonic>=0.6.0", "pythran>=0.9.7"]
 build-backend = 'mesonpy'
 
 [project]
 name = "fluidfft"
-version = "0.4.0rc1"
+version = "0.4.0rc2"
 description = "Efficient and easy Fast Fourier Transform (FFT) for Python."
 authors = [
     {name = "Pierre Augier", email = "pierre.augier@legi.cnrs.fr"},
 ]
 dependencies = [
     "fluiddyn >= 0.2.3",
     "transonic >= 0.4",
```

### Comparing `fluidfft-0.4.0rc1/src/fluidfft/__init__.py` & `fluidfft-0.4.0rc2/src/fluidfft/__init__.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/src/fluidfft/base.py` & `fluidfft-0.4.0rc2/src/fluidfft/base.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/src/fluidfft/bench.py` & `fluidfft-0.4.0rc2/src/fluidfft/bench.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/src/fluidfft/bench_analysis.py` & `fluidfft-0.4.0rc2/src/fluidfft/bench_analysis.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/src/fluidfft/fft2d/__init__.py` & `fluidfft-0.4.0rc2/src/fluidfft/fft2d/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,25 +20,26 @@
 
 .. autoclass:: FFT2dFakeForDoc
    :members:
    :undoc-members:
 
 """
 
+import os
 import sys
 
 from .. import _get_classes
 
 __all__ = [
     "FFT2dFakeForDoc",
     "get_classes_seq",
     "get_classes_mpi",
 ]
 
-if "sphinx" in sys.modules:
+if "FLUIDFFT_BUILD_DOC" in os.environ:
     from .fake_mod_fft2d_for_doc import FFT2dFakeForDoc
 
 
 def get_classes_seq():
     """Return all sequential 2d classes."""
     return _get_classes(2, sequential=True)
```

### Comparing `fluidfft-0.4.0rc1/src/fluidfft/fft2d/operators.py` & `fluidfft-0.4.0rc2/src/fluidfft/fft2d/operators.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/src/fluidfft/fft2d/testing.py` & `fluidfft-0.4.0rc2/src/fluidfft/fft2d/testing.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/src/fluidfft/fft2d/with_dask.py` & `fluidfft-0.4.0rc2/src/fluidfft/fft2d/with_dask.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/src/fluidfft/fft2d/with_pyfftw.py` & `fluidfft-0.4.0rc2/src/fluidfft/fft2d/with_pyfftw.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/src/fluidfft/fft3d/__init__.py` & `fluidfft-0.4.0rc2/src/fluidfft/fft3d/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,25 +20,26 @@
 
 .. autoclass:: FFT3dFakeForDoc
    :members:
    :undoc-members:
 
 """
 
+import os
 import sys
 
 from .. import _get_classes
 
 __all__ = [
     "FFT3dFakeForDoc",
     "get_classes_seq",
     "get_classes_mpi",
 ]
 
-if "sphinx" in sys.modules:
+if "FLUIDFFT_BUILD_DOC" in os.environ:
     from .fake_mod_fft3d_for_doc import FFT3dFakeForDoc
 
 
 def get_classes_seq():
     """Return all sequential 3d classes."""
     return _get_classes(3, sequential=True)
```

### Comparing `fluidfft-0.4.0rc1/src/fluidfft/fft3d/base.py` & `fluidfft-0.4.0rc2/src/fluidfft/fft3d/base.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/src/fluidfft/fft3d/operators.py` & `fluidfft-0.4.0rc2/src/fluidfft/fft3d/operators.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/src/fluidfft/fft3d/testing.py` & `fluidfft-0.4.0rc2/src/fluidfft/fft3d/testing.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/src/fluidfft/fft3d/with_pyfftw.py` & `fluidfft-0.4.0rc2/src/fluidfft/fft3d/with_pyfftw.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/src/fluidfft/util.py` & `fluidfft-0.4.0rc2/src/fluidfft/util.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/tests/test_2d.py` & `fluidfft-0.4.0rc2/tests/test_2d.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/tests/test_3d.py` & `fluidfft-0.4.0rc2/tests/test_3d.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/tests/test_bench.py` & `fluidfft-0.4.0rc2/tests/test_bench.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/tests/test_init.py` & `fluidfft-0.4.0rc2/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/tests/test_plugins.py` & `fluidfft-0.4.0rc2/tests/test_plugins.py`

 * *Files identical despite different names*

### Comparing `fluidfft-0.4.0rc1/PKG-INFO` & `fluidfft-0.4.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluidfft
-Version: 0.4.0rc1
+Version: 0.4.0rc2
 Summary: Efficient and easy Fast Fourier Transform (FFT) for Python.
 Keywords: Fast Fourier Transform FFT spectral code
 Author-Email: Pierre Augier <pierre.augier@legi.cnrs.fr>
 License: CeCILL License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

