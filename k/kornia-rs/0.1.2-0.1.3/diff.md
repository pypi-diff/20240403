# Comparing `tmp/kornia_rs-0.1.2.tar.gz` & `tmp/kornia_rs-0.1.3.tar.gz`

## Comparing `kornia_rs-0.1.2.tar` & `kornia_rs-0.1.3.tar`

### file list

```diff
@@ -1,81 +1,96 @@
--rw-r--r--   0      501       20     1033 2024-03-17 17:16:25.000000 kornia_rs-0.1.2/Cargo.toml
--rw-r--r--   0      501       20      948 2024-03-17 17:16:24.000000 kornia_rs-0.1.2/.github/workflows/devel_docker.yml
--rw-r--r--   0      501       20      665 2024-03-17 17:16:24.000000 kornia_rs-0.1.2/.github/workflows/python_package.yml
--rw-r--r--   0      501       20     3070 2024-03-17 17:16:25.000000 kornia_rs-0.1.2/.github/workflows/python_release.yml
--rw-r--r--   0      501       20     1599 2024-03-17 17:16:25.000000 kornia_rs-0.1.2/.github/workflows/python_test.yml
--rw-r--r--   0      501       20     1146 2024-03-17 17:16:25.000000 kornia_rs-0.1.2/.github/workflows/release_docker.yml
--rw-r--r--   0      501       20     1347 2024-03-17 17:16:25.000000 kornia_rs-0.1.2/.github/workflows/rust_lint.yml
--rw-r--r--   0      501       20      727 2024-03-17 17:16:25.000000 kornia_rs-0.1.2/.github/workflows/rust_release.yml
--rw-r--r--   0      501       20      710 2024-03-17 17:16:25.000000 kornia_rs-0.1.2/.github/workflows/rust_test.yml
--rw-r--r--   0      501       20       31 2024-03-17 17:16:25.000000 kornia_rs-0.1.2/.gitignore
--rw-r--r--   0      501       20      516 2024-03-17 17:16:25.000000 kornia_rs-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0      501       20   181618 2024-03-17 17:16:25.000000 kornia_rs-0.1.2/Cargo.lock
--rw-r--r--   0      501       20      272 2024-03-17 17:16:25.000000 kornia_rs-0.1.2/Cross.toml
--rw-r--r--   0      501       20    11357 2024-03-17 17:16:25.000000 kornia_rs-0.1.2/LICENSE
--rw-r--r--   0      501       20     1830 2024-03-17 17:16:25.000000 kornia_rs-0.1.2/Makefile
--rw-r--r--   0      501       20     6764 2024-03-17 17:16:25.000000 kornia_rs-0.1.2/README.md
--rw-r--r--   0      501       20     4522 2024-03-17 17:16:25.000000 kornia_rs-0.1.2/benches/bench_color.rs
--rw-r--r--   0      501       20     1632 2024-03-17 17:16:25.000000 kornia_rs-0.1.2/benches/bench_io.rs
--rw-r--r--   0      501       20     1290 2024-03-17 17:16:25.000000 kornia_rs-0.1.2/benches/bench_metrics.rs
--rw-r--r--   0      501       20     2013 2024-03-17 17:16:26.000000 kornia_rs-0.1.2/benches/bench_resize.rs
--rwxr-xr-x   0      501       20      316 2024-03-17 17:16:26.000000 kornia_rs-0.1.2/build_wheels.sh
--rw-r--r--   0      501       20      163 2024-03-17 17:16:26.000000 kornia_rs-0.1.2/devel-aarch64.Dockerfile
--rw-r--r--   0      501       20      170 2024-03-17 17:16:26.000000 kornia_rs-0.1.2/devel-i686.Dockerfile
--rw-r--r--   0      501       20      155 2024-03-17 17:16:26.000000 kornia_rs-0.1.2/devel-x86_64.Dockerfile
--rwxr-xr-x   0      501       20      111 2024-03-17 17:16:26.000000 kornia_rs-0.1.2/devel.sh
--rwxr-xr-x   0      501       20      146 2024-03-17 17:16:26.000000 kornia_rs-0.1.2/docker/build_devel.sh
--rwxr-xr-x   0      501       20      150 2024-03-17 17:16:26.000000 kornia_rs-0.1.2/docker/build_release.sh
--rw-r--r--   0      501       20      611 2024-03-17 17:16:26.000000 kornia_rs-0.1.2/docker/devel.Dockerfile
--rwxr-xr-x   0      501       20      329 2024-03-17 17:16:26.000000 kornia_rs-0.1.2/docker/devel.sh
--rw-r--r--   0      501       20     1065 2024-03-17 17:16:26.000000 kornia_rs-0.1.2/docker/release-amd64.Dockerfile
--rw-r--r--   0      501       20      282 2024-03-17 17:16:26.000000 kornia_rs-0.1.2/docker/release-arm64.Dockerfile
--rwxr-xr-x   0      501       20      331 2024-03-17 17:16:26.000000 kornia_rs-0.1.2/docker/release.sh
--rw-r--r--   0      501       20     1155 2024-03-17 17:16:26.000000 kornia_rs-0.1.2/examples/binarize.rs
--rw-r--r--   0      501       20      401 2024-03-17 17:16:26.000000 kornia_rs-0.1.2/examples/hello_world.rs
--rw-r--r--   0      501       20     1140 2024-03-17 17:16:26.000000 kornia_rs-0.1.2/examples/imgproc.rs
--rw-r--r--   0      501       20     1351 2024-03-17 17:16:27.000000 kornia_rs-0.1.2/examples/metrics.rs
--rw-r--r--   0      501       20     1128 2024-03-17 17:16:27.000000 kornia_rs-0.1.2/examples/normalize.rs
--rw-r--r--   0      501       20     1138 2024-03-17 17:16:27.000000 kornia_rs-0.1.2/examples/normalize_ii.rs
--rw-r--r--   0      501       20      490 2024-03-17 17:16:27.000000 kornia_rs-0.1.2/examples/rerun_viz.rs
--rw-r--r--   0      501       20       44 2024-03-17 17:16:27.000000 kornia_rs-0.1.2/kornia-rs.code-workspace
--rwxr-xr-x   0      501       20      113 2024-03-17 17:16:28.000000 kornia_rs-0.1.2/release.sh
--rwxr-xr-x   0      501       20      136 2024-03-17 17:16:28.000000 kornia_rs-0.1.2/run_tests.sh
--rw-r--r--   0      501       20       42 2024-03-17 17:16:28.000000 kornia_rs-0.1.2/rust-toolchain.toml
--rw-r--r--   0      501       20     2259 2024-03-17 17:16:28.000000 kornia_rs-0.1.2/src/color.rs
--rw-r--r--   0      501       20     3577 2024-03-17 17:16:28.000000 kornia_rs-0.1.2/src/distance_transform.rs
--rw-r--r--   0      501       20     3216 2024-03-17 17:16:28.000000 kornia_rs-0.1.2/src/flip.rs
--rw-r--r--   0      501       20    11604 2024-03-17 17:16:28.000000 kornia_rs-0.1.2/src/image.rs
--rw-r--r--   0      501       20     4949 2024-03-17 17:16:28.000000 kornia_rs-0.1.2/src/io/functional.rs
--rw-r--r--   0      501       20     5027 2024-03-17 17:16:28.000000 kornia_rs-0.1.2/src/io/jpeg.rs
--rw-r--r--   0      501       20       34 2024-03-17 17:16:28.000000 kornia_rs-0.1.2/src/io/mod.rs
--rw-r--r--   0      501       20      223 2024-03-17 17:16:29.000000 kornia_rs-0.1.2/src/lib.rs
--rw-r--r--   0      501       20     2585 2024-03-17 17:16:29.000000 kornia_rs-0.1.2/src/metrics/huber.rs
--rw-r--r--   0      501       20     2202 2024-03-17 17:16:29.000000 kornia_rs-0.1.2/src/metrics/l1.rs
--rw-r--r--   0      501       20       98 2024-03-17 17:16:29.000000 kornia_rs-0.1.2/src/metrics/mod.rs
--rw-r--r--   0      501       20     4889 2024-03-17 17:16:29.000000 kornia_rs-0.1.2/src/metrics/mse.rs
--rw-r--r--   0      501       20     7300 2024-03-17 17:16:29.000000 kornia_rs-0.1.2/src/normalize.rs
--rw-r--r--   0      501       20    11083 2024-03-17 17:16:29.000000 kornia_rs-0.1.2/src/resize.rs
--rw-r--r--   0      501       20     2621 2024-03-17 17:16:29.000000 kornia_rs-0.1.2/src/tensor.rs
--rw-r--r--   0      501       20    10938 2024-03-17 17:16:29.000000 kornia_rs-0.1.2/src/threshold.rs
--rw-r--r--   0      501       20     5029 2024-03-17 17:16:29.000000 kornia_rs-0.1.2/tests/data/dog.jpeg
--rw-r--r--   0      501       20      686 2024-03-17 17:16:30.000000 kornia_rs-0.1.2/tests/data/image.jpeg
--rw-r--r--   0        0        0      268 1970-01-01 00:00:00.000000 kornia_rs-0.1.2/py-kornia/Cargo.toml
--rw-r--r--   0      501       20      686 2024-03-17 17:16:27.000000 kornia_rs-0.1.2/py-kornia/.gitignore
--rw-r--r--   0      501       20    11357 2024-03-17 17:16:25.000000 kornia_rs-0.1.2/py-kornia/LICENSE
--rw-r--r--   0      501       20     6764 2024-03-17 17:16:25.000000 kornia_rs-0.1.2/py-kornia/README.md
--rw-r--r--   0      501       20     1544 2024-03-17 17:16:27.000000 kornia_rs-0.1.2/py-kornia/benchmark/bench_io.py
--rw-r--r--   0      501       20     1533 2024-03-17 17:16:27.000000 kornia_rs-0.1.2/py-kornia/benchmark/bench_resize.py
--rw-r--r--   0      501       20      101 2024-03-17 17:16:27.000000 kornia_rs-0.1.2/py-kornia/requirements-dev.txt
--rw-r--r--   0      501       20     3319 2024-03-17 17:16:27.000000 kornia_rs-0.1.2/py-kornia/src/dlpack.rs
--rw-r--r--   0      501       20     2420 2024-03-17 17:16:27.000000 kornia_rs-0.1.2/py-kornia/src/image.rs
--rw-r--r--   0      501       20     1044 2024-03-17 17:16:27.000000 kornia_rs-0.1.2/py-kornia/src/io/functional.rs
--rw-r--r--   0      501       20     2113 2024-03-17 17:16:27.000000 kornia_rs-0.1.2/py-kornia/src/io/jpeg.rs
--rw-r--r--   0      501       20       34 2024-03-17 17:16:27.000000 kornia_rs-0.1.2/py-kornia/src/io/mod.rs
--rw-r--r--   0      501       20     1236 2024-03-17 17:16:28.000000 kornia_rs-0.1.2/py-kornia/src/lib.rs
--rw-r--r--   0      501       20     1038 2024-03-17 17:16:28.000000 kornia_rs-0.1.2/py-kornia/src/resize.rs
--rw-r--r--   0      501       20     2673 2024-03-17 17:16:28.000000 kornia_rs-0.1.2/py-kornia/tests/test_io.py
--rw-r--r--   0      501       20       75 2024-03-17 17:16:28.000000 kornia_rs-0.1.2/py-kornia/tests/test_package.py
--rw-r--r--   0      501       20      524 2024-03-17 17:16:28.000000 kornia_rs-0.1.2/py-kornia/tests/test_resize.py
--rw-r--r--   0      501       20    40560 2024-03-17 17:18:32.000000 kornia_rs-0.1.2/py-kornia/Cargo.lock
--rw-r--r--   0        0        0     1513 1970-01-01 00:00:00.000000 kornia_rs-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     8303 1970-01-01 00:00:00.000000 kornia_rs-0.1.2/PKG-INFO
+-rw-r--r--   0      501       20     1497 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/Cargo.toml
+-rw-r--r--   0      501       20      948 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/.github/workflows/devel_docker.yml
+-rw-r--r--   0      501       20      665 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/.github/workflows/python_package.yml
+-rw-r--r--   0      501       20     3070 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/.github/workflows/python_release.yml
+-rw-r--r--   0      501       20     1530 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/.github/workflows/python_test.yml
+-rw-r--r--   0      501       20     1146 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/.github/workflows/release_docker.yml
+-rw-r--r--   0      501       20     1428 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/.github/workflows/rust_lint.yml
+-rw-r--r--   0      501       20      762 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/.github/workflows/rust_release.yml
+-rw-r--r--   0      501       20     1149 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/.github/workflows/rust_test.yml
+-rw-r--r--   0      501       20       55 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/.gitignore
+-rw-r--r--   0      501       20      516 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0      501       20   183366 2024-04-03 16:10:43.000000 kornia_rs-0.1.3/Cargo.lock
+-rw-r--r--   0      501       20      272 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/Cross.toml
+-rw-r--r--   0      501       20    11357 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/LICENSE
+-rw-r--r--   0      501       20     1830 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/Makefile
+-rw-r--r--   0      501       20     7139 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/README.md
+-rw-r--r--   0      501       20     4522 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/benches/bench_color.rs
+-rw-r--r--   0      501       20     1632 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/benches/bench_io.rs
+-rw-r--r--   0      501       20     1290 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/benches/bench_metrics.rs
+-rw-r--r--   0      501       20     2013 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/benches/bench_resize.rs
+-rw-r--r--   0      501       20     1076 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/benches/bench_warp.rs
+-rwxr-xr-x   0      501       20      316 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/build_wheels.sh
+-rw-r--r--   0      501       20      287 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/devel-aarch64.Dockerfile
+-rw-r--r--   0      501       20      291 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/devel-i686.Dockerfile
+-rw-r--r--   0      501       20      220 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/devel-x86_64.Dockerfile
+-rwxr-xr-x   0      501       20      111 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/devel.sh
+-rwxr-xr-x   0      501       20      146 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/docker/build_devel.sh
+-rwxr-xr-x   0      501       20      150 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/docker/build_release.sh
+-rw-r--r--   0      501       20      611 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/docker/devel.Dockerfile
+-rwxr-xr-x   0      501       20      329 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/docker/devel.sh
+-rw-r--r--   0      501       20     1065 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/docker/release-amd64.Dockerfile
+-rw-r--r--   0      501       20      282 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/docker/release-arm64.Dockerfile
+-rwxr-xr-x   0      501       20      331 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/docker/release.sh
+-rw-r--r--   0      501       20     1132 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/examples/binarize.rs
+-rw-r--r--   0      501       20      401 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/examples/hello_world.rs
+-rw-r--r--   0      501       20     2051 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/examples/histogram.rs
+-rw-r--r--   0      501       20     1117 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/examples/imgproc.rs
+-rw-r--r--   0      501       20     1328 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/examples/metrics.rs
+-rw-r--r--   0      501       20     1128 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/examples/normalize.rs
+-rw-r--r--   0      501       20     1138 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/examples/normalize_ii.rs
+-rw-r--r--   0      501       20      481 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/examples/rerun_viz.rs
+-rw-r--r--   0      501       20     1073 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/examples/rotate.rs
+-rw-r--r--   0      501       20     3193 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/examples/std_mean.rs
+-rw-r--r--   0      501       20       44 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/kornia-rs.code-workspace
+-rwxr-xr-x   0      501       20      113 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/release.sh
+-rwxr-xr-x   0      501       20      136 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/run_tests.sh
+-rw-r--r--   0      501       20       42 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/rust-toolchain.toml
+-rw-r--r--   0      501       20     2259 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/src/color.rs
+-rw-r--r--   0      501       20     2198 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/src/core.rs
+-rw-r--r--   0      501       20     3577 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/src/distance_transform.rs
+-rw-r--r--   0      501       20     3216 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/src/flip.rs
+-rw-r--r--   0      501       20     1996 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/src/histogram.rs
+-rw-r--r--   0      501       20    15976 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/src/image.rs
+-rw-r--r--   0      501       20      791 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/src/io/fps_counter.rs
+-rw-r--r--   0      501       20     4949 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/src/io/functional.rs
+-rw-r--r--   0      501       20     5027 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/src/io/jpeg.rs
+-rw-r--r--   0      501       20      101 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/src/io/mod.rs
+-rw-r--r--   0      501       20     7415 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/src/io/webcam.rs
+-rw-r--r--   0      501       20      270 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/src/lib.rs
+-rw-r--r--   0      501       20     2585 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/src/metrics/huber.rs
+-rw-r--r--   0      501       20     2202 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/src/metrics/l1.rs
+-rw-r--r--   0      501       20       98 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/src/metrics/mod.rs
+-rw-r--r--   0      501       20     4889 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/src/metrics/mse.rs
+-rw-r--r--   0      501       20     7300 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/src/normalize.rs
+-rw-r--r--   0      501       20    12262 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/src/resize.rs
+-rw-r--r--   0      501       20     2621 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/src/tensor.rs
+-rw-r--r--   0      501       20    10938 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/src/threshold.rs
+-rw-r--r--   0      501       20     8012 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/src/warp.rs
+-rw-r--r--   0      501       20     5029 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/tests/data/dog.jpeg
+-rw-r--r--   0      501       20      686 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/tests/data/image.jpeg
+-rw-r--r--   0        0        0      267 1970-01-01 00:00:00.000000 kornia_rs-0.1.3/kornia-py/Cargo.toml
+-rw-r--r--   0      501       20      686 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/kornia-py/.gitignore
+-rw-r--r--   0      501       20    11357 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/kornia-py/LICENSE
+-rw-r--r--   0      501       20     7139 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/kornia-py/README.md
+-rw-r--r--   0      501       20      957 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/kornia-py/benchmark/bench_histogram.py
+-rw-r--r--   0      501       20     1545 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/kornia-py/benchmark/bench_io.py
+-rw-r--r--   0      501       20     1533 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/kornia-py/benchmark/bench_resize.py
+-rw-r--r--   0      501       20     1658 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/kornia-py/benchmark/bench_warp_affine.py
+-rw-r--r--   0      501       20      101 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/kornia-py/requirements-dev.txt
+-rw-r--r--   0      501       20     3319 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/kornia-py/src/dlpack.rs
+-rw-r--r--   0      501       20      920 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/kornia-py/src/histogram.rs
+-rw-r--r--   0      501       20     2418 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/kornia-py/src/image.rs
+-rw-r--r--   0      501       20     1044 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/kornia-py/src/io/functional.rs
+-rw-r--r--   0      501       20     2113 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/kornia-py/src/io/jpeg.rs
+-rw-r--r--   0      501       20       34 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/kornia-py/src/io/mod.rs
+-rw-r--r--   0      501       20     1396 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/kornia-py/src/lib.rs
+-rw-r--r--   0      501       20     1038 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/kornia-py/src/resize.rs
+-rw-r--r--   0      501       20     1697 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/kornia-py/src/warp.rs
+-rw-r--r--   0      501       20      451 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/kornia-py/tests/test_histogram.py
+-rw-r--r--   0      501       20     2673 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/kornia-py/tests/test_io.py
+-rw-r--r--   0      501       20       75 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/kornia-py/tests/test_package.py
+-rw-r--r--   0      501       20      524 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/kornia-py/tests/test_resize.py
+-rw-r--r--   0      501       20      609 2024-04-03 16:10:06.000000 kornia_rs-0.1.3/kornia-py/tests/test_warp_affine.py
+-rw-r--r--   0      501       20    33693 2024-04-03 16:10:37.000000 kornia_rs-0.1.3/kornia-py/Cargo.lock
+-rw-r--r--   0        0        0     1513 1970-01-01 00:00:00.000000 kornia_rs-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     8678 1970-01-01 00:00:00.000000 kornia_rs-0.1.3/PKG-INFO
```

### Comparing `kornia_rs-0.1.2/Cargo.toml` & `kornia_rs-0.1.3/Cargo.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,46 @@
 [package]
 name = "kornia-rs"
-version = "0.1.2"
+version = "0.1.3"
 edition = "2021"
 description = "Low-level computer vision library in Rust"
 homepage = "http://kornia.org"
 repository = "https://github.com/kornia/kornia-rs"
 categories = ["image-processing", "computer-vision", "machine-learning"]
 license-file = "LICENSE"
 
 [dependencies]
 anyhow = "1.0.80"
-num-traits = "0.2.17"
+fast_image_resize = "3.0.4"
+gst = { version = "0.22.2", package = "gstreamer", optional = true }
+gst-app = { version = "0.22.0", package = "gstreamer-app", optional = true }
 image = { version = "0.25.0" }
-turbojpeg = {version = "1.0.0"}
 memmap2 = "0.9.4"
 ndarray = { version = "0.15.6", features = ["rayon"] }
-fast_image_resize = "3.0.4"
+num-traits = "0.2.17"
+tokio = { version = "1", features = ["full"], optional = true }
+turbojpeg = {version = "1.0.0"}
 # this is experimental and only used for benchmarking, so it's optional
 # consider removing it in the future.
 candle-core = { version = "0.3.2", optional = true }
 
 [dev-dependencies]
+clap = { version = "4.5.3", features = ["derive"] }
+criterion = { version = "0.5.1", features = ["html_reports"] }
+indicatif = { version = "0.17.8", features = ["rayon"] }
 tempfile = "3.9.0"
+rayon = "1.10.0"
 rerun = "0.14.1"
-criterion = { version = "0.5.1", features = ["html_reports"] }
+walkdir = "2.5.0"
+packed_simd = "0.3.9"
+
 
 [features]
 candle = ["candle-core"]
+gstreamer = ["gst", "gst-app", "tokio"]
 
 [[bench]]
 name = "bench_color"
 harness = false
 
 [[bench]]
 name = "bench_resize"
@@ -39,7 +49,11 @@
 [[bench]]
 name = "bench_metrics"
 harness = false
 
 [[bench]]
 name = "bench_io"
 harness = false
+
+[[bench]]
+name = "bench_warp"
+harness = false
```

### Comparing `kornia_rs-0.1.2/.github/workflows/devel_docker.yml` & `kornia_rs-0.1.3/.github/workflows/devel_docker.yml`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/.github/workflows/python_package.yml` & `kornia_rs-0.1.3/.github/workflows/python_package.yml`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/.github/workflows/python_release.yml` & `kornia_rs-0.1.3/.github/workflows/python_release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
       - uses: ilammy/setup-nasm@v1
       - uses: actions/checkout@v4
       - uses: messense/maturin-action@v1
         with:
           target: ${{ matrix.target }}
           manylinux: auto
           command: build
-          args: --release --out dist -i python${{ matrix.python-version }} -m py-kornia/Cargo.toml --sdist
+          args: --release --out dist -i python${{ matrix.python-version }} -m kornia-py/Cargo.toml --sdist
       - name: Upload wheels
         uses: actions/upload-artifact@v2
         with:
           name: wheels
           path: dist
 
   macos:
@@ -49,15 +49,15 @@
           toolchain: stable
           target: ${{ matrix.target }}-apple-darwin
           override: true
       - uses: messense/maturin-action@v1
         with:
           command: build
           maturin-version: latest
-          args: --release --target ${{ matrix.target }}-apple-darwin --out dist -i python${{ matrix.python-version }} -m py-kornia/Cargo.toml --sdist
+          args: --release --target ${{ matrix.target }}-apple-darwin --out dist -i python${{ matrix.python-version }} -m kornia-py/Cargo.toml --sdist
       - name: Upload wheels
         uses: actions/upload-artifact@v2
         with:
           name: wheels
           path: dist
 
   windows:
@@ -78,15 +78,15 @@
           profile: minimal
           toolchain: stable
           override: true
       - uses: messense/maturin-action@v1
         with:
           command: build
           maturin-version: latest
-          args: --release --out dist -i python${{ matrix.python-version }} -m py-kornia/Cargo.toml --sdist
+          args: --release --out dist -i python${{ matrix.python-version }} -m kornia-py/Cargo.toml --sdist
       - name: Upload wheels
         uses: actions/upload-artifact@v2
         with:
           name: wheels
           path: dist
 
   release:
```

### Comparing `kornia_rs-0.1.2/.github/workflows/python_test.yml` & `kornia_rs-0.1.3/.github/workflows/python_test.yml`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,16 @@
 name: Python Test
 
 on:
   pull_request:
-    paths:
-      - Cargo.lock
-      - py-kornia/**
-      - .github/workflows/test-python.yml
+    branches:
+      - main
   push:
     branches:
       - main
-    paths:
-      - Cargo.lock
-      - py-kornia/**
-      - .github/workflows/test-python.yml
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 jobs:
   test-python-linux:
@@ -47,15 +41,17 @@
           toolchain: stable
           target: x86_64-apple-darwin
           override: true
       - uses: messense/maturin-action@v1
         with:
           command: build
           maturin-version: latest
-          args: --target x86_64-apple-darwin --out dist -m py-kornia/Cargo.toml
+          args: --target x86_64-apple-darwin --out dist -m kornia-py/Cargo.toml
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip |
           python -m pip install dist/*.whl |
-          python -m pip install pytest torch numpy
+          python -m pip install pytest numpy |
+          python -m pip install torch --extra-index-url https://download.pytorch.org/whl/cpu
+
       - name: Build and test
-        run: pytest py-kornia/tests
+        run: pytest kornia-py/tests
```

### Comparing `kornia_rs-0.1.2/.github/workflows/release_docker.yml` & `kornia_rs-0.1.3/.github/workflows/release_docker.yml`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/.github/workflows/rust_lint.yml` & `kornia_rs-0.1.3/.github/workflows/rust_lint.yml`

 * *Files 24% similar despite different names*

```diff
@@ -25,28 +25,29 @@
           command: fmt
           args: --all -- --check
 
   clippy:
     name: Clippy
     runs-on: ubuntu-latest
     steps:
-      - name: Install system dependencies
-        run: sudo apt-get install -y cmake nasm
+      #- name: Install system dependencies
+      #  run: sudo apt-get install -y cmake nasm libgstreamer1.0-dev libgstreamer-plugins-base1.0-dev
       - uses: actions/checkout@v4
       - uses: actions-rs/toolchain@v1
         with:
           profile: minimal
           toolchain: stable
           override: true
           components: clippy
       - uses: actions-rs/clippy-check@v1
         with:
           token: ${{ secrets.GITHUB_TOKEN }}
           args: --all-features
           name: Clippy Output
+          use-cross: true
 
   check:
     name: Check
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - uses: actions-rs/toolchain@v1
```

### Comparing `kornia_rs-0.1.2/.github/workflows/rust_release.yml` & `kornia_rs-0.1.3/.github/workflows/rust_release.yml`

 * *Files 7% similar despite different names*

```diff
@@ -8,14 +8,15 @@
     name: Release Rust
     strategy:
       matrix:
         target:
           - x86_64-unknown-linux-gnu
     runs-on: ubuntu-latest
     steps:
+      - uses: ilammy/setup-nasm@v1
       - uses: actions/checkout@v4
       - uses: actions-rs/toolchain@v1
         with:
           profile: minimal
           toolchain: stable
           target: ${{ matrix.target }}
           override: true
```

### Comparing `kornia_rs-0.1.2/.pre-commit-config.yaml` & `kornia_rs-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/Cargo.lock` & `kornia_rs-0.1.3/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 name = "ab_glyph_rasterizer"
 version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c71b1793ee61086797f5c80b6efa2b8ffa6d5dd703f118545808a7f2e27f7046"
 
 [[package]]
 name = "accesskit"
-version = "0.12.2"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6cb10ed32c63247e4e39a8f42e8e30fb9442fbf7878c8e4a9849e7e381619bea"
+checksum = "74a4b14f3d99c1255dcba8f45621ab1a2e7540a0009652d33989005a4d0bfc6b"
 dependencies = [
  "enumn",
  "serde",
 ]
 
 [[package]]
 name = "accesskit_consumer"
@@ -106,31 +106,31 @@
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "ahash"
-version = "0.8.7"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77c3a9648d43b9cd48db467b3f87fdd6e146bcc88ab0180006cef2179fe11d01"
+checksum = "e89da841a80418a9b391ebaea17f5c112ffaaa96f621d2c285b5174da76b9011"
 dependencies = [
  "cfg-if",
  "getrandom",
  "once_cell",
  "serde",
  "version_check",
  "zerocopy",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.1.2"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "aligned-vec"
 version = "0.5.0"
@@ -146,15 +146,15 @@
 [[package]]
 name = "android-activity"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ee91c0c2905bae44f84bfa4e044536541df26b7703fd0888deeb9060fcc44289"
 dependencies = [
  "android-properties",
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "cc",
  "cesu8",
  "jni",
  "jni-sys",
  "libc",
  "log",
  "ndk",
@@ -183,31 +183,31 @@
 name = "anes"
 version = "0.1.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4b46cbb362ab8752921c97e041f5e366ee6297bd428a31275b9fcf1e380f7299"
 
 [[package]]
 name = "anstream"
-version = "0.6.11"
+version = "0.6.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6e2e1ebcb11de5c03c67de28a7df593d32191b44939c482e97702baaaa6ab6a5"
+checksum = "d96bd03f33fe50a863e394ee9718a706f988b9079b20c3784fb726e7678b62fb"
 dependencies = [
  "anstyle",
  "anstyle-parse",
  "anstyle-query",
  "anstyle-wincon",
  "colorchoice",
  "utf8parse",
 ]
 
 [[package]]
 name = "anstyle"
-version = "1.0.4"
+version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7079075b41f533b8c61d2a4d073c4676e1f8b249ff94a393b0595db304e0dd87"
+checksum = "8901269c6307e8d93993578286ac0edf7f195079ffff5ebdeea6a59ffb7e36bc"
 
 [[package]]
 name = "anstyle-parse"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c75ac65da39e5fe5ab759307499ddad880d724eed2f6ce5b5e8a26f4f387928c"
 dependencies = [
@@ -231,58 +231,52 @@
 dependencies = [
  "anstyle",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "anyhow"
-version = "1.0.80"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ad32ce52e4161730f7098c077cd2ed6229b5804ccf99e5366be1ab72a98b4e1"
-
-[[package]]
-name = "arbitrary"
-version = "0.4.7"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "db55d72333851e17d572bec876e390cd3b11eb1ef53ae821dd9f3b653d2b4569"
+checksum = "0952808a6c2afd1aa8947271f3a60f1a6763c7b912d210184c5149b5cf147247"
 
 [[package]]
 name = "arbitrary"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7d5a26814d8dcb93b0e5a0ff3c6d80a8843bafb21b39e8e18a6f05471870e110"
 
 [[package]]
 name = "arboard"
-version = "3.3.0"
+version = "3.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "aafb29b107435aa276664c1db8954ac27a6e105cdad3c88287a199eb0e313c08"
+checksum = "a2041f1943049c7978768d84e6d0fd95de98b76d6c4727b09e78ec253d29fa58"
 dependencies = [
  "clipboard-win",
- "core-graphics 0.22.3",
- "image 0.24.8",
+ "core-graphics",
+ "image 0.24.9",
  "log",
  "objc",
  "objc-foundation",
  "objc_id",
  "parking_lot",
  "thiserror",
- "winapi",
- "x11rb 0.12.0",
+ "windows-sys 0.48.0",
+ "x11rb",
 ]
 
 [[package]]
 name = "arg_enum_proc_macro"
 version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ae92a5119aa49cdbcf6b9f893fe4e1d98b04ccbf82ee0584ad948a44a734dea"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "array-init"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3d62b7694a562cdf5a74227903507c56ab2cc8bdd1f781ed5cb4cf9c9f810bfc"
@@ -294,17 +288,14 @@
 checksum = "bf7d0a018de4f6aa429b9d33d69edf69072b1c5b1cb8d3e4a5f7ef898fc3eb76"
 
 [[package]]
 name = "arrayvec"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
-dependencies = [
- "serde",
-]
 
 [[package]]
 name = "arrow-format"
 version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "07884ea216994cdc32a2d5f8274a8bee979cfe90274b83f86f440866ee3132c7"
 dependencies = [
@@ -329,15 +320,15 @@
 
 [[package]]
 name = "ashpd"
 version = "0.6.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ac22eda5891cc086690cb6fa10121c0390de0e3b04eb269f2d766b00d3f2d81"
 dependencies = [
- "async-fs 2.1.0",
+ "async-fs 2.1.1",
  "async-net",
  "enumflags2",
  "futures-channel",
  "futures-util",
  "once_cell",
  "rand",
  "serde",
@@ -354,36 +345,36 @@
 dependencies = [
  "event-listener 2.5.3",
  "futures-core",
 ]
 
 [[package]]
 name = "async-channel"
-version = "2.1.1"
+version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ca33f4bc4ed1babef42cad36cc1f51fa88be00420404e5b1e80ab1b18f7678c"
+checksum = "f28243a43d821d11341ab73c80bed182dc015c514b951616cf79bd4af39af0c3"
 dependencies = [
  "concurrent-queue",
- "event-listener 4.0.3",
- "event-listener-strategy",
+ "event-listener 5.2.0",
+ "event-listener-strategy 0.5.1",
  "futures-core",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "async-executor"
-version = "1.8.0"
+version = "1.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "17ae5ebefcc48e7452b4987947920dac9450be1110cadf34d1b8c116bdbaf97c"
+checksum = "10b3e585719c2358d2660232671ca8ca4ddb4be4ce8a1842d6c2dc8685303316"
 dependencies = [
  "async-lock 3.3.0",
  "async-task",
  "concurrent-queue",
- "fastrand 2.0.1",
- "futures-lite 2.2.0",
+ "fastrand 2.0.2",
+ "futures-lite 2.3.0",
  "slab",
 ]
 
 [[package]]
 name = "async-fs"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -393,21 +384,21 @@
  "autocfg",
  "blocking",
  "futures-lite 1.13.0",
 ]
 
 [[package]]
 name = "async-fs"
-version = "2.1.0"
+version = "2.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd1f344136bad34df1f83a47f3fd7f2ab85d75cb8a940af4ccf6d482a84ea01b"
+checksum = "bc19683171f287921f2405677dd2ed2549c3b3bda697a563ebc3a121ace2aba1"
 dependencies = [
  "async-lock 3.3.0",
  "blocking",
- "futures-lite 2.2.0",
+ "futures-lite 2.3.0",
 ]
 
 [[package]]
 name = "async-io"
 version = "1.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fc5b45d93ef0529756f812ca52e44c221b35341892d3dcc34132ac02f3dd2af"
@@ -424,26 +415,26 @@
  "slab",
  "socket2 0.4.10",
  "waker-fn",
 ]
 
 [[package]]
 name = "async-io"
-version = "2.3.0"
+version = "2.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb41eb19024a91746eba0773aa5e16036045bbf45733766661099e182ea6a744"
+checksum = "dcccb0f599cfa2f8ace422d3555572f47424da5648a4382a9dd0310ff8210884"
 dependencies = [
  "async-lock 3.3.0",
  "cfg-if",
  "concurrent-queue",
  "futures-io",
- "futures-lite 2.2.0",
+ "futures-lite 2.3.0",
  "parking",
- "polling 3.3.2",
- "rustix 0.38.30",
+ "polling 3.6.0",
+ "rustix 0.38.32",
  "slab",
  "tracing",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "async-lock"
@@ -457,27 +448,27 @@
 [[package]]
 name = "async-lock"
 version = "3.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d034b430882f8381900d3fe6f0aaa3ad94f2cb4ac519b429692a1bc2dda4ae7b"
 dependencies = [
  "event-listener 4.0.3",
- "event-listener-strategy",
+ "event-listener-strategy 0.4.0",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "async-net"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b948000fad4873c1c9339d60f2623323a0cfd3816e5181033c6a5cb68b2accf7"
 dependencies = [
- "async-io 2.3.0",
+ "async-io 2.3.2",
  "blocking",
- "futures-lite 2.2.0",
+ "futures-lite 2.3.0",
 ]
 
 [[package]]
 name = "async-once-cell"
 version = "0.5.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9338790e78aa95a416786ec8389546c4b6a1dfc3dc36071ed9518a9413a542eb"
@@ -491,71 +482,77 @@
  "async-io 1.13.0",
  "async-lock 2.8.0",
  "async-signal",
  "blocking",
  "cfg-if",
  "event-listener 3.1.0",
  "futures-lite 1.13.0",
- "rustix 0.38.30",
+ "rustix 0.38.32",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "async-recursion"
-version = "1.0.5"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5fd55a5ba1179988837d24ab4c7cc8ed6efdeff578ede0416b4225a5fca35bd0"
+checksum = "30c5ef0ede93efbf733c1a727f3b6b5a1060bbedd5600183e66f6e4be4af0ec5"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "async-signal"
 version = "0.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e47d90f65a225c4527103a8d747001fc56e375203592b25ad103e1ca13124c5"
 dependencies = [
- "async-io 2.3.0",
+ "async-io 2.3.2",
  "async-lock 2.8.0",
  "atomic-waker",
  "cfg-if",
  "futures-core",
  "futures-io",
- "rustix 0.38.30",
+ "rustix 0.38.32",
  "signal-hook-registry",
  "slab",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "async-task"
 version = "4.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fbb36e985947064623dbd357f727af08ffd077f93d696782f3c56365fa2e2799"
 
 [[package]]
 name = "async-trait"
-version = "0.1.77"
+version = "0.1.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c980ee35e870bd1a4d2c8294d4c04d0499e67bca1e4b5cefcc693c2fa00caea9"
+checksum = "a507401cad91ec6a857ed5513a2073c82a9b9048762b885bb98655b306964681"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "atomic-waker"
 version = "1.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1505bd5d3d116872e7271a6d4e16d81d0c8570876c8de68093a09ac269d8aac0"
 
 [[package]]
+name = "atomic_refcell"
+version = "0.1.13"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "41e67cd8309bbd06cd603a9e693a784ac2e5d1e955f11286e355089fcab3047c"
+
+[[package]]
 name = "atspi"
 version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6059f350ab6f593ea00727b334265c4dfc7fd442ee32d264794bd9bdc68e87ca"
 dependencies = [
  "atspi-common",
  "atspi-connection",
@@ -597,30 +594,29 @@
  "atspi-common",
  "serde",
  "zbus",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "av1-grain"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6678909d8c5d46a42abcf571271e15fdbc0a225e3646cf23762cd415046c78bf"
 dependencies = [
  "anyhow",
  "arrayvec",
  "log",
  "nom",
  "num-rational",
- "serde",
  "v_frame",
 ]
 
 [[package]]
 name = "avif-serialize"
 version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -633,17 +629,17 @@
 name = "az"
 version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7b7e4c2464d97fe331d41de9d5db0def0a96f4d823b8b32a2efd503578988973"
 
 [[package]]
 name = "backtrace"
-version = "0.3.69"
+version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2089b7e3f35b9dd2d0ed921ead4f6d318c27680d4a5bd167b3ee120edb105837"
+checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
@@ -696,30 +692,24 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.4.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed570934406eb16438a4e976b1b4500774099c13b8cb96eec99f620f05090ddf"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 dependencies = [
  "bytemuck",
  "serde",
 ]
 
 [[package]]
 name = "bitstream-io"
-version = "1.10.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e445576659fd04a57b44cbd00aa37aaa815ebefa0aa3cb677a6b5e63d883074f"
-
-[[package]]
-name = "bitstream-io"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06c9989a51171e2e81038ab168b6ae22886fe9ded214430dbb4f41c28cf176da"
 
 [[package]]
 name = "block"
 version = "0.1.6"
@@ -778,17 +768,17 @@
 version = "1.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a37913e8dc4ddcc604f0c6d3bf2887c995153af3611de9e23c352b44c1b9118"
 dependencies = [
  "async-channel",
  "async-lock 3.3.0",
  "async-task",
- "fastrand 2.0.1",
+ "fastrand 2.0.2",
  "futures-io",
- "futures-lite 2.2.0",
+ "futures-lite 2.3.0",
  "piper",
  "tracing",
 ]
 
 [[package]]
 name = "bstr"
 version = "0.2.17"
@@ -798,93 +788,84 @@
  "lazy_static",
  "memchr",
  "regex-automata 0.1.10",
 ]
 
 [[package]]
 name = "built"
-version = "0.5.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b9c056b9ed43aee5e064b683aa1ec783e19c6acec7559e3ae931b7490472fbe"
-dependencies = [
- "cargo-lock",
-]
-
-[[package]]
-name = "built"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "38d17f4d6e4dc36d1a02fbedc2753a096848e7c1b0772f7654eab8e2c927dd53"
 
 [[package]]
 name = "bumpalo"
-version = "3.14.0"
+version = "3.15.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f30e7476521f6f8af1a1c4c0b8cc94f0bee37d91763d0ca2665f299b6cd8aec"
+checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
 
 [[package]]
 name = "bytecount"
 version = "0.6.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1e5f035d16fc623ae5f74981db80a439803888314e3a555fd6f04acd51a3205"
 
 [[package]]
 name = "bytemuck"
-version = "1.14.1"
+version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed2490600f404f2b94c167e31d3ed1d5f3c225a0f3b80230053b3e0b7b962bd9"
+checksum = "5d6d68c57235a3a081186990eca2867354726650f42f7516ca50c28d6281fd15"
 dependencies = [
  "bytemuck_derive",
 ]
 
 [[package]]
 name = "bytemuck_derive"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "965ab7eb5f8f97d2a083c799f3a1b994fc397b2fe2da5d1da1626ce15a39f2b1"
+checksum = "4da9a32f3fed317401fa3c862968128267c3106685286e15d5aaa3d7389c2f60"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
 name = "bytes"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
+checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "calloop"
 version = "0.12.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fba7adb4dd5aa98e5553510223000e7148f621165ec5f9acd7113f6ca4995298"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "log",
- "polling 3.3.2",
- "rustix 0.38.30",
+ "polling 3.6.0",
+ "rustix 0.38.32",
  "slab",
  "thiserror",
 ]
 
 [[package]]
 name = "calloop-wayland-source"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0f0ea9b9476c7fad82841a8dbb380e2eae480c21910feba80725b46931ed8f02"
 dependencies = [
  "calloop",
- "rustix 0.38.30",
+ "rustix 0.38.32",
  "wayland-backend",
  "wayland-client",
 ]
 
 [[package]]
 name = "camino"
 version = "1.1.6"
@@ -892,50 +873,38 @@
 checksum = "c59e92b5a388f549b863a7bea62612c09f24c8393560709a54558a9abdfb3b9c"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "candle-core"
-version = "0.3.2"
+version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "57433f80b510bc603fd9e52c5a15eb44a8ac70112b95b28b0ab8fb1c1f001822"
+checksum = "6db8659ea87ee8197d2fc627348916cce0561330ee7ae3874e771691d3cecb2f"
 dependencies = [
  "byteorder",
  "gemm",
  "half",
- "memmap2 0.7.1",
+ "memmap2",
  "num-traits",
  "num_cpus",
  "rand",
  "rand_distr",
  "rayon",
  "safetensors",
  "thiserror",
  "yoke",
  "zip",
 ]
 
 [[package]]
-name = "cargo-lock"
-version = "8.0.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "031718ddb8f78aa5def78a09e90defe30151d1f6c672f937af4dd916429ed996"
-dependencies = [
- "semver",
- "serde",
- "toml 0.5.11",
- "url",
-]
-
-[[package]]
 name = "cargo-platform"
-version = "0.1.6"
+version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ceed8ef69d8518a5dda55c07425450b58a4e1946f4951eab6d7191ee86c2443d"
+checksum = "24b1f0365a6c6bb4020cd05806fd0d33c44d38046b8bd7f0e40814b9763cabfc"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "cargo_metadata"
 version = "0.14.2"
@@ -967,17 +936,17 @@
 name = "cast"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "37b2a672a2cb129a2e41c10b1224bb368f9f37a2b16b612598138befd7b37eb5"
 
 [[package]]
 name = "cc"
-version = "1.0.83"
+version = "1.0.90"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1174fb0b6ec23863f8b971027804a42614e347eafb0a95bf0b12cdae21fc4d0"
+checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
 dependencies = [
  "jobserver",
  "libc",
 ]
 
 [[package]]
 name = "cesu8"
@@ -1022,17 +991,17 @@
 name = "cfg_aliases"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77e53693616d3075149f4ead59bdeecd204ac6b8192d8969757601b74bddf00f"
 
 [[package]]
 name = "chrono"
-version = "0.4.33"
+version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f13690e35a5e4ace198e7beea2895d29f3a9cc55015fcebe6336bd2010af9eb"
+checksum = "8a0d04d43504c61aa6c7531f1871dd0d418d91130162063b789da00fd7057a5e"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "ciborium"
 version = "0.2.2"
@@ -1067,67 +1036,65 @@
 checksum = "696283b40e1a39d208ee614b92e5f6521d16962edeb47c48372585ec92419943"
 dependencies = [
  "thiserror",
 ]
 
 [[package]]
 name = "clap"
-version = "4.4.18"
+version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e578d6ec4194633722ccf9544794b71b1385c3c027efe0c55db226fc880865c"
+checksum = "90bc066a67923782aa8515dbaea16946c5bcc5addbd668bb80af688e53e548a0"
 dependencies = [
  "clap_builder",
  "clap_derive",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.4.18"
+version = "4.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4df4df40ec50c46000231c914968278b1eb05098cf8f1b3a518a95030e71d1c7"
+checksum = "ae129e2e766ae0ec03484e609954119f123cc1fe650337e155d03b022f24f7b4"
 dependencies = [
  "anstream",
  "anstyle",
  "clap_lex",
  "strsim",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "4.4.7"
+version = "4.5.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cf9804afaaf59a91e75b022a30fb7229a7901f60c755489cc61c9b423b836442"
+checksum = "528131438037fd55894f62d6e9f068b8f45ac57ffa77517819645d10aed04f64"
 dependencies = [
- "heck",
+ "heck 0.5.0",
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "clap_lex"
-version = "0.6.0"
+version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "702fc72eb24e5a1e48ce58027a675bc24edd52096d5397d4aea7c6dd9eca0bd1"
+checksum = "98cc8fbded0c607b7ba9dd60cd98df59af97e84d24e49c8557331cfc26d301ce"
 
 [[package]]
 name = "clean-path"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aaa6b4b263a5d737e9bf6b7c09b72c41a5480aec4d7219af827f6564e950b6a5"
 
 [[package]]
 name = "clipboard-win"
-version = "4.5.0"
+version = "5.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7191c27c2357d9b7ef96baac1773290d4ca63b24205b82a3fd8a0637afcf0362"
+checksum = "d517d4b86184dbb111d3556a10f1c8a04da7428d2987bf1081602bf11c3aa9ee"
 dependencies = [
  "error-code",
- "str-buf",
- "winapi",
 ]
 
 [[package]]
 name = "cmake"
 version = "0.1.50"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a31c789563b815f77f4250caee12365734369f942439b7defd71e18a48197130"
@@ -1141,16 +1108,16 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f6140449f97a6e97f9511815c5632d84c8aacf8ac271ad77c559218161a1373c"
 dependencies = [
  "bitflags 1.3.2",
  "block",
  "cocoa-foundation",
  "core-foundation",
- "core-graphics 0.23.1",
- "foreign-types 0.5.0",
+ "core-graphics",
+ "foreign-types",
  "libc",
  "objc",
 ]
 
 [[package]]
 name = "cocoa-foundation"
 version = "0.1.2"
@@ -1253,14 +1220,15 @@
 version = "0.15.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0e1f83fc076bd6dd27517eacdf25fef6c4dfe5f1d7448bafaaf3a26f13b5e4eb"
 dependencies = [
  "encode_unicode",
  "lazy_static",
  "libc",
+ "unicode-width",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "convert_case"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1283,35 +1251,22 @@
 name = "core-foundation-sys"
 version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
 
 [[package]]
 name = "core-graphics"
-version = "0.22.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2581bbab3b8ffc6fcbd550bf46c355135d16e9ff2a6ea032ad6b9bf1d7efe4fb"
-dependencies = [
- "bitflags 1.3.2",
- "core-foundation",
- "core-graphics-types",
- "foreign-types 0.3.2",
- "libc",
-]
-
-[[package]]
-name = "core-graphics"
 version = "0.23.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "970a29baf4110c26fedbc7f82107d42c23f7e88e404c4577ed73fe99ff85a212"
 dependencies = [
  "bitflags 1.3.2",
  "core-foundation",
  "core-graphics-types",
- "foreign-types 0.5.0",
+ "foreign-types",
  "libc",
 ]
 
 [[package]]
 name = "core-graphics-types"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -1329,17 +1284,17 @@
 checksum = "53fe5e26ff1b7aef8bca9c6080520cfb8d9333c7568e1829cef191a9723e5504"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crc32fast"
-version = "1.3.2"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
+checksum = "b3855a8a784b474f333699ef2bbca9db2c4a1f6d9088a90a2d25b1eb53111eaa"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "criterion"
 version = "0.5.1"
@@ -1387,17 +1342,17 @@
  "crossbeam-epoch",
  "crossbeam-queue",
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-channel"
-version = "0.5.11"
+version = "0.5.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "176dc175b78f56c0f321911d9c8eb2b77a78a4860b9c19db83835fea1a46649b"
+checksum = "ab3db02a9c5b5121e1e42fbdb1aeb65f5e02624cc58c43f2884c6ccac0b82f95"
 dependencies = [
  "crossbeam-utils",
 ]
 
 [[package]]
 name = "crossbeam-deque"
 version = "0.8.5"
@@ -1452,44 +1407,44 @@
 name = "cursor-icon"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96a6ac251f4a2aca6b3f91340350eab87ae57c3f127ffeb585e92bd336717991"
 
 [[package]]
 name = "darling"
-version = "0.20.3"
+version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0209d94da627ab5605dcccf08bb18afa5009cfbef48d8a8b7d7bdbc79be25c5e"
+checksum = "54e36fcd13ed84ffdfda6f5be89b31287cbb80c439841fe69e04841435464391"
 dependencies = [
  "darling_core",
  "darling_macro",
 ]
 
 [[package]]
 name = "darling_core"
-version = "0.20.3"
+version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "177e3443818124b357d8e76f53be906d60937f0d3a90773a664fa63fa253e621"
+checksum = "9c2cf1c23a687a1feeb728783b993c4e1ad83d99f351801977dd809b48d0a70f"
 dependencies = [
  "fnv",
  "ident_case",
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "darling_macro"
-version = "0.20.3"
+version = "0.20.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "836a9bbc7ad63342d6d6e7b815ccab164bc77a2d95d84bc3117a8c0d5c98e2d5"
+checksum = "a668eda54683121533a393014d8692171709ff57a7d61f187b6e782719f8933f"
 dependencies = [
  "darling_core",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "data-encoding"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7e962a19be5cfc3f3bf6dd8f61eb50107f356ad6270fbb3ed41476571db78be5"
@@ -1554,15 +1509,15 @@
 
 [[package]]
 name = "dlib"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "330c60081dcc4c72131f8eb70510f1ac07223e5d4163db481a04a0befcffa412"
 dependencies = [
- "libloading 0.8.1",
+ "libloading 0.8.3",
 ]
 
 [[package]]
 name = "document-features"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef5282ad69563b5fc40319526ba27e0e7363d552a896f0297d54f767717f9b95"
@@ -1574,17 +1529,17 @@
 name = "downcast-rs"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ea835d29036a4087793836fa931b08837ad5e957da9e23886b29586fb9b6650"
 
 [[package]]
 name = "dyn-clone"
-version = "1.0.16"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "545b22097d44f8a9581187cdf93de7a71e4722bf51200cfaba810865b49a495d"
+checksum = "0d6ef0072f8a535281e4876be788938b528e9a1d43900b82c2569af7da799125"
 
 [[package]]
 name = "dyn-stack"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "56e53799688f5632f364f8fb387488dd05db9fe45db7011be066fc20e7027f8b"
 dependencies = [
@@ -1612,22 +1567,22 @@
  "cocoa",
  "directories-next",
  "document-features",
  "egui",
  "egui-wgpu",
  "egui-winit",
  "egui_glow",
- "image 0.24.8",
+ "image 0.24.9",
  "js-sys",
  "log",
  "objc",
  "parking_lot",
  "percent-encoding",
  "pollster",
- "puffin 0.19.0",
+ "puffin",
  "raw-window-handle 0.6.0",
  "ron",
  "serde",
  "static_assertions",
  "thiserror",
  "wasm-bindgen",
  "wasm-bindgen-futures",
@@ -1646,15 +1601,15 @@
 dependencies = [
  "accesskit",
  "ahash",
  "backtrace",
  "epaint",
  "log",
  "nohash-hasher",
- "puffin 0.19.0",
+ "puffin",
  "ron",
  "serde",
 ]
 
 [[package]]
 name = "egui-wgpu"
 version = "0.26.2"
@@ -1662,15 +1617,15 @@
 checksum = "86f2d75e1e70228e7126f828bac05f9fe0e7ea88e9660c8cebe609bb114c61d4"
 dependencies = [
  "bytemuck",
  "document-features",
  "egui",
  "epaint",
  "log",
- "puffin 0.19.0",
+ "puffin",
  "thiserror",
  "type-map",
  "web-time",
  "wgpu",
  "winit",
 ]
 
@@ -1680,15 +1635,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa4d44f8d89f70d4480545eb2346b76ea88c3022e9f4706cebc799dbe8b004a2"
 dependencies = [
  "accesskit_winit",
  "arboard",
  "egui",
  "log",
- "puffin 0.19.0",
+ "puffin",
  "raw-window-handle 0.6.0",
  "serde",
  "smithay-clipboard",
  "web-time",
  "webbrowser",
  "winit",
 ]
@@ -1709,34 +1664,34 @@
 version = "0.26.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f4a6962241a76da5be5e64e41b851ee1c95fda11f76635522a3c82b119b5475"
 dependencies = [
  "egui",
  "ehttp",
  "enum-map",
- "image 0.24.8",
+ "image 0.24.9",
  "log",
  "mime_guess2",
- "puffin 0.19.0",
+ "puffin",
  "serde",
 ]
 
 [[package]]
 name = "egui_glow"
 version = "0.26.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a08e3be8728b4c59493dbfec041c657e6725bdeafdbd49aef3f1dbb9e551fa01"
 dependencies = [
  "bytemuck",
  "egui",
  "egui-winit",
  "glow",
  "log",
- "memoffset 0.9.0",
- "puffin 0.19.0",
+ "memoffset 0.9.1",
+ "puffin",
  "wasm-bindgen",
  "web-sys",
  "winit",
 ]
 
 [[package]]
 name = "egui_plot"
@@ -1751,15 +1706,15 @@
 name = "egui_tiles"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bb10cef7bdbd1adb158aec9cca20f34779fd40ea126e02662ab558189f1c435"
 dependencies = [
  "ahash",
  "egui",
- "itertools 0.12.0",
+ "itertools 0.12.1",
  "log",
  "serde",
 ]
 
 [[package]]
 name = "ehttp"
 version = "0.4.0"
@@ -1774,17 +1729,17 @@
  "wasm-bindgen-futures",
  "wasm-streams",
  "web-sys",
 ]
 
 [[package]]
 name = "either"
-version = "1.9.0"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
+checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
 
 [[package]]
 name = "emath"
 version = "0.26.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6916301ecf80448f786cdf3eb51d9dbdd831538732229d49119e2d4312eaaf09"
 dependencies = [
@@ -1795,14 +1750,26 @@
 [[package]]
 name = "encode_unicode"
 version = "0.3.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a357d28ed41a50f9c765dbfe56cbc04a64e53e5fc58ba79fbc34c10ef3df831f"
 
 [[package]]
+name = "enum-as-inner"
+version = "0.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5ffccbb6966c05b32ef8fbac435df276c4ae4d3dc55a8cd0eb9745e6c12f546a"
+dependencies = [
+ "heck 0.4.1",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.57",
+]
+
+[[package]]
 name = "enum-map"
 version = "2.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6866f3bfdf8207509a033af1a75a7b08abda06bbaaeae6669323fd5a097df2e9"
 dependencies = [
  "enum-map-derive",
  "serde",
@@ -1812,47 +1779,47 @@
 name = "enum-map-derive"
 version = "0.17.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f282cfdfe92516eb26c2af8589c274c7c17681f5ecc03c18255fe741c6aa64eb"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "enumflags2"
-version = "0.7.8"
+version = "0.7.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5998b4f30320c9d93aed72f63af821bfdac50465b75428fce77b48ec482c3939"
+checksum = "3278c9d5fb675e0a51dabcf4c0d355f692b064171535ba72361be1528a9d8e8d"
 dependencies = [
  "enumflags2_derive",
  "serde",
 ]
 
 [[package]]
 name = "enumflags2_derive"
-version = "0.7.8"
+version = "0.7.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f95e2801cd355d4a1a3e3953ce6ee5ae9603a5c833455343a8bfe3f44d418246"
+checksum = "5c785274071b1b420972453b306eeca06acf4633829db4223b58a2a8c5953bc4"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "enumn"
 version = "0.1.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6fd000fd6988e73bbe993ea3db9b1aa64906ab88766d654973924340c8cddb42"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "enumset"
 version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "226c0da7462c13fb57e5cc9e0dc8f0635e7d27f276a3a7fd30054647f669007d"
@@ -1865,15 +1832,15 @@
 version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e08b6c6ab82d70f08844964ba10c7babb716de2ecaeab9be5717918a5177d3af"
 dependencies = [
  "darling",
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "env_logger"
 version = "0.10.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4cd405aab171cb85d6735e5c8d9db038c17d3ca007a4d2c25f337935c3d90580"
@@ -1894,15 +1861,15 @@
  "ahash",
  "bytemuck",
  "ecolor",
  "emath",
  "log",
  "nohash-hasher",
  "parking_lot",
- "puffin 0.19.0",
+ "puffin",
  "rayon",
  "serde",
 ]
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
@@ -1926,21 +1893,17 @@
 checksum = "2d2f06b9cac1506ece98fe3231e3cc9c4410ec3d5b1f24ae1c8946f0742cdefc"
 dependencies = [
  "version_check",
 ]
 
 [[package]]
 name = "error-code"
-version = "2.3.1"
+version = "3.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "64f18991e7bf11e7ffee451b5318b5c1a73c52d0d0ada6e5a3017c8c1ced6a21"
-dependencies = [
- "libc",
- "str-buf",
-]
+checksum = "a0474425d51df81997e2f90a21591180b38eccf27292d755f3e30750225c175b"
 
 [[package]]
 name = "ethnum"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b90ca2580b73ab6a1f724b76ca11ab632df820fd6040c336200d2c1df7b3c82c"
 
@@ -1969,24 +1932,45 @@
 dependencies = [
  "concurrent-queue",
  "parking",
  "pin-project-lite",
 ]
 
 [[package]]
+name = "event-listener"
+version = "5.2.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2b5fb89194fa3cad959b833185b3063ba881dbfc7030680b314250779fb4cc91"
+dependencies = [
+ "concurrent-queue",
+ "parking",
+ "pin-project-lite",
+]
+
+[[package]]
 name = "event-listener-strategy"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "958e4d70b6d5e81971bebec42271ec641e7ff4e170a6fa605f2b8a8b65cb97d3"
 dependencies = [
  "event-listener 4.0.3",
  "pin-project-lite",
 ]
 
 [[package]]
+name = "event-listener-strategy"
+version = "0.5.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "332f51cb23d20b0de8458b86580878211da09bcd4503cb579c225b3d124cabb3"
+dependencies = [
+ "event-listener 5.2.0",
+ "pin-project-lite",
+]
+
+[[package]]
 name = "ewebsock"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6177769715c6ec5a324acee995183b22721ea23c58e49af14a828eadec85d120"
 dependencies = [
  "document-features",
  "js-sys",
@@ -1995,17 +1979,17 @@
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
 ]
 
 [[package]]
 name = "exr"
-version = "1.6.4"
+version = "1.72.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "279d3efcc55e19917fff7ab3ddd6c14afb6a90881a0078465196fe2f99d08c56"
+checksum = "887d93f60543e9a9362ef8a21beedd0a833c5d9610e18c67abe15a5963dcb1a4"
 dependencies = [
  "bit_field",
  "flume",
  "half",
  "lebe",
  "miniz_oxide",
  "rayon-core",
@@ -2031,17 +2015,17 @@
 checksum = "e51093e27b0797c359783294ca4f0a911c270184cb10f85783b118614a1501be"
 dependencies = [
  "instant",
 ]
 
 [[package]]
 name = "fastrand"
-version = "2.0.1"
+version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25cbce373ec4653f1a01a31e8a5e5ec0c622dc27ff9c4e6606eefef5cbbed4a5"
+checksum = "658bd65b1cf4c852a3cc96f18a8ce7b5640f6b703f905c7d74532294c2a63984"
 
 [[package]]
 name = "fdeflate"
 version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4f9bfee30e4dedf0ab8b422f03af778d9612b63f502710fc500a334ebe2de645"
 dependencies = [
@@ -2058,17 +2042,17 @@
  "libc",
  "redox_syscall 0.4.1",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "fixed"
-version = "1.24.0"
+version = "1.27.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "02c69ce7e7c0f17aa18fdd9d0de39727adb9c6281f2ad12f57cbe54ae6e76e7d"
+checksum = "2fc715d38bea7b5bf487fcd79bcf8c209f0b58014f3018a7a19c2b855f472048"
 dependencies = [
  "az",
  "bytemuck",
  "half",
  "serde",
  "typenum",
 ]
@@ -2091,69 +2075,50 @@
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "flume"
-version = "0.10.14"
+version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1657b4441c3403d9f7b3409e47575237dac27b1b5726df654a6ecbf92f0f7577"
+checksum = "55ac459de2512911e4b674ce33cf20befaba382d05b62b008afc1c8b57cbf181"
 dependencies = [
- "futures-core",
- "futures-sink",
- "nanorand",
- "pin-project",
  "spin",
 ]
 
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "foreign-types"
-version = "0.3.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f6f339eb8adc052cd2ca78910fda869aefa38d22d5cb648e6485e4d3fc06f3b1"
-dependencies = [
- "foreign-types-shared 0.1.1",
-]
-
-[[package]]
-name = "foreign-types"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d737d9aa519fb7b749cbc3b962edcf310a8dd1f4b67c91c4f83975dbdd17d965"
 dependencies = [
  "foreign-types-macros",
- "foreign-types-shared 0.3.1",
+ "foreign-types-shared",
 ]
 
 [[package]]
 name = "foreign-types-macros"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a5c6c585bc94aaf2c7b51dd4c2ba22680844aba4c687be581871a6f518c5742"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "foreign-types-shared"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "00b0228411908ca8685dba7fc2cdd70ec9990a6e753e89b6ac91a84c40fbaf4b"
-
-[[package]]
-name = "foreign-types-shared"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aa9a19cbb55df58761df49b23516a86d432839add4af60fc256da840f66ed35b"
 
 [[package]]
 name = "foreign_vec"
 version = "0.1.0"
@@ -2190,14 +2155,25 @@
 [[package]]
 name = "futures-core"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dfc6580bb841c5a68e9ef15c77ccc837b40a7504914d52e47b8b0e9bbda25a1d"
 
 [[package]]
+name = "futures-executor"
+version = "0.3.30"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "a576fc72ae164fca6b9db127eaa9a9dda0d61316034f33a0a0d4eda41f02b01d"
+dependencies = [
+ "futures-core",
+ "futures-task",
+ "futures-util",
+]
+
+[[package]]
 name = "futures-io"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a44623e20b9681a318efdd71c299b6b222ed6f231972bfe2f224ebad6311f0c1"
 
 [[package]]
 name = "futures-lite"
@@ -2212,34 +2188,34 @@
  "parking",
  "pin-project-lite",
  "waker-fn",
 ]
 
 [[package]]
 name = "futures-lite"
-version = "2.2.0"
+version = "2.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "445ba825b27408685aaecefd65178908c36c6e96aaf6d8599419d46e624192ba"
+checksum = "52527eb5074e35e9339c6b4e8d12600c7128b68fb25dcb9fa9dec18f7c25f3a5"
 dependencies = [
- "fastrand 2.0.1",
+ "fastrand 2.0.2",
  "futures-core",
  "futures-io",
  "parking",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "futures-macro"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "futures-sink"
 version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
@@ -2265,17 +2241,17 @@
  "pin-project-lite",
  "pin-utils",
  "slab",
 ]
 
 [[package]]
 name = "gemm"
-version = "0.16.15"
+version = "0.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b3afa707040531a7527477fd63a81ea4f6f3d26037a2f96776e57fb843b258e"
+checksum = "6ab24cc62135b40090e31a76a9b2766a501979f3070fa27f689c27ec04377d32"
 dependencies = [
  "dyn-stack",
  "gemm-c32",
  "gemm-c64",
  "gemm-common",
  "gemm-f16",
  "gemm-f32",
@@ -2285,66 +2261,67 @@
  "paste",
  "raw-cpuid",
  "seq-macro",
 ]
 
 [[package]]
 name = "gemm-c32"
-version = "0.16.15"
+version = "0.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1cc3973a4c30c73f26a099113953d0c772bb17ee2e07976c0a06b8fe1f38a57d"
+checksum = "b9c030d0b983d1e34a546b86e08f600c11696fde16199f971cd46c12e67512c0"
 dependencies = [
  "dyn-stack",
  "gemm-common",
  "num-complex",
  "num-traits",
  "paste",
  "raw-cpuid",
  "seq-macro",
 ]
 
 [[package]]
 name = "gemm-c64"
-version = "0.16.15"
+version = "0.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "30362894b93dada374442cb2edf4512ddf19513c9bec88e06a445bcb6b22e64f"
+checksum = "fbb5f2e79fefb9693d18e1066a557b4546cd334b226beadc68b11a8f9431852a"
 dependencies = [
  "dyn-stack",
  "gemm-common",
  "num-complex",
  "num-traits",
  "paste",
  "raw-cpuid",
  "seq-macro",
 ]
 
 [[package]]
 name = "gemm-common"
-version = "0.16.15"
+version = "0.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "988499faa80566b046b4fee2c5f15af55b5a20c1fe8486b112ebb34efa045ad6"
+checksum = "a2e7ea062c987abcd8db95db917b4ffb4ecdfd0668471d8dc54734fdff2354e8"
 dependencies = [
  "bytemuck",
  "dyn-stack",
  "half",
  "num-complex",
  "num-traits",
  "once_cell",
  "paste",
  "pulp",
  "raw-cpuid",
  "rayon",
  "seq-macro",
+ "sysctl",
 ]
 
 [[package]]
 name = "gemm-f16"
-version = "0.16.15"
+version = "0.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d6cf2854a12371684c38d9a865063a27661812a3ff5803454c5742e8f5a388ce"
+checksum = "7ca4c06b9b11952071d317604acb332e924e817bd891bec8dfb494168c7cedd4"
 dependencies = [
  "dyn-stack",
  "gemm-common",
  "gemm-f32",
  "half",
  "num-complex",
  "num-traits",
@@ -2352,32 +2329,32 @@
  "raw-cpuid",
  "rayon",
  "seq-macro",
 ]
 
 [[package]]
 name = "gemm-f32"
-version = "0.16.15"
+version = "0.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0bc84003cf6d950a7c7ca714ad6db281b6cef5c7d462f5cd9ad90ea2409c7227"
+checksum = "e9a69f51aaefbd9cf12d18faf273d3e982d9d711f60775645ed5c8047b4ae113"
 dependencies = [
  "dyn-stack",
  "gemm-common",
  "num-complex",
  "num-traits",
  "paste",
  "raw-cpuid",
  "seq-macro",
 ]
 
 [[package]]
 name = "gemm-f64"
-version = "0.16.15"
+version = "0.17.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "35187ef101a71eed0ecd26fb4a6255b4192a12f1c5335f3a795698f2d9b6cf33"
+checksum = "aa397a48544fadf0b81ec8741e5c0fba0043008113f71f2034def1935645d2b0"
 dependencies = [
  "dyn-stack",
  "gemm-common",
  "num-complex",
  "num-traits",
  "paste",
  "raw-cpuid",
@@ -2392,24 +2369,14 @@
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "gethostname"
-version = "0.3.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb65d4ba3173c56a500b555b532f72c42e8d1fe64962b518897f8959fae2c177"
-dependencies = [
- "libc",
- "winapi",
-]
-
-[[package]]
-name = "gethostname"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0176e0459c2e4a1fe232f984bca6890e681076abb9934f6cea7c326f3fc47818"
 dependencies = [
  "libc",
  "windows-targets 0.48.5",
 ]
@@ -2440,14 +2407,27 @@
 [[package]]
 name = "gimli"
 version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 
 [[package]]
+name = "gio-sys"
+version = "0.19.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bcf8e1d9219bb294636753d307b030c1e8a032062cba74f493c431a5c8b81ce4"
+dependencies = [
+ "glib-sys",
+ "gobject-sys",
+ "libc",
+ "system-deps",
+ "windows-sys 0.52.0",
+]
+
+[[package]]
 name = "gl_generator"
 version = "0.14.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a95dfc23a2b4a9a2f5ab41d194f8bfda3cabec42af4e39f08c339eb2a0c124d"
 dependencies = [
  "khronos_api",
  "log",
@@ -2461,14 +2441,59 @@
 checksum = "12f597d56c1bd55a811a1be189459e8fad2bbc272616375602443bdfb37fa774"
 dependencies = [
  "bytemuck",
  "serde",
 ]
 
 [[package]]
+name = "glib"
+version = "0.19.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "01e191cc1af1f35b9699213107068cd3fe05d9816275ac118dc785a0dd8faebf"
+dependencies = [
+ "bitflags 2.5.0",
+ "futures-channel",
+ "futures-core",
+ "futures-executor",
+ "futures-task",
+ "futures-util",
+ "gio-sys",
+ "glib-macros",
+ "glib-sys",
+ "gobject-sys",
+ "libc",
+ "memchr",
+ "smallvec",
+ "thiserror",
+]
+
+[[package]]
+name = "glib-macros"
+version = "0.19.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9972bb91643d589c889654693a4f1d07697fdcb5d104b5c44fb68649ba1bf68d"
+dependencies = [
+ "heck 0.5.0",
+ "proc-macro-crate 3.1.0",
+ "proc-macro2",
+ "quote",
+ "syn 2.0.57",
+]
+
+[[package]]
+name = "glib-sys"
+version = "0.19.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "630f097773d7c7a0bb3258df4e8157b47dc98bbfa0e60ad9ab56174813feced4"
+dependencies = [
+ "libc",
+ "system-deps",
+]
+
+[[package]]
 name = "glob"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d2fabcfbdc87f4758337ca535fb41a6d701b65693ce38287d856d1674551ec9b"
 
 [[package]]
 name = "glow"
@@ -2487,30 +2512,30 @@
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3b78f069cf941075835822953c345b9e1edd67ae347b81ace3aea9de38c2ef33"
 dependencies = [
  "base64 0.13.1",
  "byteorder",
  "gltf-json",
- "image 0.24.8",
+ "image 0.24.9",
  "lazy_static",
  "serde_json",
  "urlencoding",
 ]
 
 [[package]]
 name = "gltf-derive"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "438ffe1a5540d75403feaf23636b164e816e93f6f03131674722b3886ce32a57"
 dependencies = [
  "inflections",
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "gltf-json"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "655951ba557f2bc69ea4b0799446bae281fa78efae6319968bdd2c3e9a06d8e1"
@@ -2527,30 +2552,41 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c8098adac955faa2d31079b65dc48841251f69efd3ac25477903fc424362ead"
 dependencies = [
  "gl_generator",
 ]
 
 [[package]]
+name = "gobject-sys"
+version = "0.19.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "c85e2b1080b9418dd0c58b498da3a5c826030343e0ef07bde6a955d28de54979"
+dependencies = [
+ "glib-sys",
+ "libc",
+ "system-deps",
+]
+
+[[package]]
 name = "gpu-alloc"
 version = "0.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fbcd2dba93594b227a1f57ee09b8b9da8892c34d55aa332e034a228d0fe6a171"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "gpu-alloc-types",
 ]
 
 [[package]]
 name = "gpu-alloc-types"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "98ff03b468aa837d70984d55f5d3f846f6ec31fe34bbb97c4f85219caeee1ca4"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "gpu-allocator"
 version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6f56f6318968d03c18e1bcf4857ff88c61157e9da8e47c5f29055d60e1228884"
@@ -2564,52 +2600,144 @@
 
 [[package]]
 name = "gpu-descriptor"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cc11df1ace8e7e564511f53af41f3e42ddc95b56fd07b3f4445d2a6048bc682c"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "gpu-descriptor-types",
  "hashbrown",
 ]
 
 [[package]]
 name = "gpu-descriptor-types"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6bf0b36e6f090b7e1d8a4b49c0cb81c1f8376f72198c65dd3ad9ff3556b8b78c"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
+]
+
+[[package]]
+name = "gstreamer"
+version = "0.22.3"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "066f3c354c526792a3deb8b6d349eba8ffcc13bae4d0bf05d4adf4bf1b91e459"
+dependencies = [
+ "cfg-if",
+ "futures-channel",
+ "futures-core",
+ "futures-util",
+ "glib",
+ "gstreamer-sys",
+ "itertools 0.12.1",
+ "libc",
+ "muldiv",
+ "num-integer",
+ "num-rational",
+ "once_cell",
+ "option-operations",
+ "paste",
+ "pin-project-lite",
+ "smallvec",
+ "thiserror",
+]
+
+[[package]]
+name = "gstreamer-app"
+version = "0.22.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "50184e88d3462a796a5924fb329839c102b22f9383c1636323fa4ef5255dea92"
+dependencies = [
+ "futures-core",
+ "futures-sink",
+ "glib",
+ "gstreamer",
+ "gstreamer-app-sys",
+ "gstreamer-base",
+ "libc",
+]
+
+[[package]]
+name = "gstreamer-app-sys"
+version = "0.22.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6771c0939f286fb261525494a0aad29435b37e802284756bab24afe3bbca7476"
+dependencies = [
+ "glib-sys",
+ "gstreamer-base-sys",
+ "gstreamer-sys",
+ "libc",
+ "system-deps",
+]
+
+[[package]]
+name = "gstreamer-base"
+version = "0.22.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "514c71195b53c7eced4842b66ca9149833e41cf6a1d949e45e2ca4a4fa929850"
+dependencies = [
+ "atomic_refcell",
+ "cfg-if",
+ "glib",
+ "gstreamer",
+ "gstreamer-base-sys",
+ "libc",
+]
+
+[[package]]
+name = "gstreamer-base-sys"
+version = "0.22.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "286591e0f85bbda1adf9bab6f21d015acd9ca0a4d4acb61da65e3d0487e23c4e"
+dependencies = [
+ "glib-sys",
+ "gobject-sys",
+ "gstreamer-sys",
+ "libc",
+ "system-deps",
+]
+
+[[package]]
+name = "gstreamer-sys"
+version = "0.22.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d5ddf526b3bf90ea627224c804f00b8bcb0452e3b447978b4d5092f8e8ff5918"
+dependencies = [
+ "glib-sys",
+ "gobject-sys",
+ "libc",
+ "system-deps",
 ]
 
 [[package]]
 name = "h2"
-version = "0.3.24"
+version = "0.3.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bb2c4422095b67ee78da96fbb51a4cc413b3b25883c7717ff7ca1ab31022c9c9"
+checksum = "4fbd2820c5e49886948654ab546d0688ff24530286bdcf8fca3cefb16d4618eb"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
- "http",
+ "http 0.2.12",
  "indexmap",
  "slab",
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
 name = "half"
-version = "2.3.1"
+version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bc52e53916c08643f1b56ec082790d1e86a32e58dc5268f897f313fbae7b4872"
+checksum = "b5eceaaeec696539ddaf7b333340f1af35a5aa87ae3e4f3ead0532f72affab2e"
 dependencies = [
  "bytemuck",
  "cfg-if",
  "crunchy",
  "num-traits",
  "rand",
  "rand_distr",
@@ -2633,34 +2761,40 @@
 
 [[package]]
 name = "hassle-rs"
 version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "af2a7e73e1f34c48da31fb668a907f250794837e08faa144fd24f0b8b741e890"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "com",
  "libc",
- "libloading 0.8.1",
+ "libloading 0.8.3",
  "thiserror",
  "widestring",
  "winapi",
 ]
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
+name = "heck"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2304e00983f87ffb38b55b444b5e3b60a884b5d30c0fca7d82fe33449bbe55ea"
+
+[[package]]
 name = "hermit-abi"
-version = "0.3.4"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5d3d0e0f38255e7fa3cf31335b3a56f05febd18025f4db5ef7a0cfb4f8da651f"
+checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
 [[package]]
 name = "hex"
 version = "0.4.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f24254aa9a54b5c858eaee2f5bccdb46aaf0e486a595ed5fd8f86ba55232a70"
 
@@ -2677,31 +2811,42 @@
 checksum = "e3d1354bf6b7235cb4a0576c2619fd4ed18183f689b12b006a0ee7329eeff9a5"
 dependencies = [
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "http"
-version = "0.2.11"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8947b1a6fad4393052c7ba1f4cd97bed3e953a95c79c92ad9b051a04611d9fbb"
+checksum = "601cbb57e577e2f5ef5be8e7b83f0f63994f25aa94d673e54a92d5c516d101f1"
+dependencies = [
+ "bytes",
+ "fnv",
+ "itoa",
+]
+
+[[package]]
+name = "http"
+version = "1.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "21b9ddb458710bc376481b842f5da65cdf31522de232c1ca8146abce2a358258"
 dependencies = [
  "bytes",
  "fnv",
  "itoa",
 ]
 
 [[package]]
 name = "http-body"
 version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7ceab25649e9960c0311ea418d17bee82c0dcec1bd053b5f9a66e265a693bed2"
 dependencies = [
  "bytes",
- "http",
+ "http 0.2.12",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "httparse"
 version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -2726,21 +2871,21 @@
 checksum = "bf96e135eb83a2a8ddf766e426a841d8ddd7449d5f00d34ea02b41d2f19eef80"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
  "h2",
- "http",
+ "http 0.2.12",
  "http-body",
  "httparse",
  "httpdate",
  "itoa",
  "pin-project-lite",
- "socket2 0.5.5",
+ "socket2 0.5.6",
  "tokio",
  "tower-service",
  "tracing",
  "want",
 ]
 
 [[package]]
@@ -2768,17 +2913,17 @@
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "image"
-version = "0.24.8"
+version = "0.24.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "034bbe799d1909622a74d1193aa50147769440040ff36cb2baa947609b0a4e23"
+checksum = "5690139d2f55868e080017335e4b94cb7414274c74f1669c84fb5feba2c9f69d"
 dependencies = [
  "bytemuck",
  "byteorder",
  "color_quant",
  "jpeg-decoder",
  "num-traits",
  "png",
@@ -2806,17 +2951,17 @@
  "tiff",
  "zune-core",
  "zune-jpeg",
 ]
 
 [[package]]
 name = "image-webp"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba6107a25f04af48ceeb4093eebc9b405ee5a1813a0bab5ecf1805d3eabb3337"
+checksum = "7a84a25dcae3ac487bc24ef280f9e20c79c9b1a3e5e32cbed3041d1c514aa87c"
 dependencies = [
  "byteorder",
  "thiserror",
 ]
 
 [[package]]
 name = "imgref"
@@ -2828,23 +2973,37 @@
 name = "indent"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d9f1a0777d972970f204fdf8ef319f1f4f8459131636d7e3c96c5d59570d0fa6"
 
 [[package]]
 name = "indexmap"
-version = "2.1.0"
+version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d530e1a18b1cb4c484e6e34556a0d948706958449fca0cab753d649f2bce3d1f"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
  "hashbrown",
 ]
 
 [[package]]
+name = "indicatif"
+version = "0.17.8"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "763a5a8f45087d6bcea4222e7b72c291a054edf80e4ef6efd2a4979878c7bea3"
+dependencies = [
+ "console",
+ "instant",
+ "number_prefix",
+ "portable-atomic",
+ "rayon",
+ "unicode-width",
+]
+
+[[package]]
 name = "infer"
 version = "0.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cb33622da908807a06f9513c19b3c1ad50fab3e4137d82a78107d502075aa199"
 dependencies = [
  "cfb",
 ]
@@ -2888,15 +3047,15 @@
 name = "interpolate_name"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c34819042dc3d3971c46c2190835914dfbe0c3c13f61449b2997f4e9722dfa60"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "io-lifetimes"
 version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eae7b9aee968036d54dce06cebaefd919e4472e753296daccd6d344e3e2df0c2"
@@ -2904,46 +3063,46 @@
  "hermit-abi",
  "libc",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "is-terminal"
-version = "0.4.10"
+version = "0.4.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0bad00257d07be169d870ab665980b06cdb366d792ad690bf2e76876dc503455"
+checksum = "f23ff5ef2b80d608d61efee834934d862cd92461afc0560dedf493e4c033738b"
 dependencies = [
  "hermit-abi",
- "rustix 0.38.30",
+ "libc",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itertools"
-version = "0.12.0"
+version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25db6b064527c5d482d0423354fcd07a89a2dfe07b67892e62411946db7f07b0"
+checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "jni"
 version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1a87aa2bb7d2af34197c04845522473242e1aa17c12f4935d5856491a7fb8c97"
 dependencies = [
@@ -2961,68 +3120,76 @@
 name = "jni-sys"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8eaf4bc02d17cbdd7ff4c7438cafcdf7fb9a4613313ad11b4f8fefe7d3fa0130"
 
 [[package]]
 name = "jobserver"
-version = "0.1.27"
+version = "0.1.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c37f63953c4c63420ed5fd3d6d398c719489b9f872b9fa683262f8edd363c7d"
+checksum = "ab46a6e9526ddef3ae7f787c06f0f2600639ba80ea3eade3d8e670a2230f51d6"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "jpeg-decoder"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f5d4a7da358eff58addd2877a45865158f0d78c911d43a5784ceb7bbf52833b0"
 
 [[package]]
 name = "js-sys"
-version = "0.3.67"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a1d36f1235bc969acba30b7f5990b864423a6068a10f7c90ae8f0112e3a59d1"
+checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "khronos-egl"
 version = "6.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6aae1df220ece3c0ada96b8153459b67eebe9ae9212258bb0134ae60416fdf76"
 dependencies = [
  "libc",
- "libloading 0.8.1",
+ "libloading 0.8.3",
  "pkg-config",
 ]
 
 [[package]]
 name = "khronos_api"
 version = "3.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2db585e1d738fc771bf08a151420d3ed193d9d895a36df7f6f8a9456b911ddc"
 
 [[package]]
 name = "kornia-rs"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "anyhow",
  "candle-core",
+ "clap",
  "criterion",
  "fast_image_resize",
+ "gstreamer",
+ "gstreamer-app",
  "image 0.25.0",
- "memmap2 0.9.4",
+ "indicatif",
+ "memmap2",
  "ndarray",
  "num-traits",
+ "packed_simd",
+ "rayon",
  "rerun",
  "tempfile",
+ "tokio",
  "turbojpeg",
+ "walkdir",
 ]
 
 [[package]]
 name = "kqueue"
 version = "1.0.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7447f1ca1b7b563588a205fe93dea8df60fd981423a768bc1c0ded35ed147d0c"
@@ -3051,35 +3218,25 @@
 name = "lebe"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "03087c2bad5e1034e8cace5926dec053fb3790248370865f5117a7d0213354c8"
 
 [[package]]
 name = "libc"
-version = "0.2.152"
+version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "13e3bf6590cbc649f4d1a3eefc9d5d6eb746f5200ffb04e5e142700b8faa56e7"
-
-[[package]]
-name = "libfuzzer-sys"
-version = "0.3.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fcf184a4b6b274f82a5df6b357da6055d3e82272327bba281c28bbba6f1664ef"
-dependencies = [
- "arbitrary 0.4.7",
- "cc",
-]
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "libfuzzer-sys"
 version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a96cfd5557eb82f2b83fed4955246c988d331975a002961b07c81584d107e7f7"
 dependencies = [
- "arbitrary 1.3.2",
+ "arbitrary",
  "cc",
  "once_cell",
 ]
 
 [[package]]
 name = "libloading"
 version = "0.7.4"
@@ -3088,46 +3245,46 @@
 dependencies = [
  "cfg-if",
  "winapi",
 ]
 
 [[package]]
 name = "libloading"
-version = "0.8.1"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c571b676ddfc9a8c12f1f3d3085a7b163966a8fd8098a90640953ce5f6170161"
+checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
 dependencies = [
  "cfg-if",
- "windows-sys 0.48.0",
+ "windows-targets 0.52.4",
 ]
 
 [[package]]
 name = "libm"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
 
 [[package]]
 name = "libredox"
 version = "0.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "85c833ca1e66078851dba29046874e38f08b2c883700aa29a03ddd3b23814ee8"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "libc",
  "redox_syscall 0.4.1",
 ]
 
 [[package]]
 name = "libredox"
 version = "0.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3af92c55d7d839293953fcd0fda5ecfe93297cfde6ffbdec13b41d99c0ba6607"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "libc",
  "redox_syscall 0.4.1",
 ]
 
 [[package]]
 name = "linked-hash-map"
 version = "0.5.6"
@@ -3161,17 +3318,17 @@
  "autocfg",
  "scopeguard",
  "serde",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.20"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "log-once"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6d8a05e3879b317b1b6dbf353e5bba7062bedcc59815267bb23eaa0c576cebf0"
 dependencies = [
@@ -3185,17 +3342,17 @@
 checksum = "0fae87c125b03c1d2c0150c90365d7d6bcc53fb73a9acaef207d2d065860f062"
 dependencies = [
  "imgref",
 ]
 
 [[package]]
 name = "lz4_flex"
-version = "0.11.2"
+version = "0.11.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "912b45c753ff5f7f5208307e8ace7d2a2e30d024e26d3509f3dce546c044ce15"
+checksum = "75761162ae2b0e580d7e7c390558127e5f01b4194debd6221fd8c207fc80e3f5"
 dependencies = [
  "twox-hash",
 ]
 
 [[package]]
 name = "macaw"
 version = "0.18.6"
@@ -3234,51 +3391,42 @@
 dependencies = [
  "cfg-if",
  "rayon",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
-
-[[package]]
-name = "memmap2"
-version = "0.7.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f49388d20533534cd19360ad3d6a7dadc885944aa802ba3995040c5ec11288c6"
-dependencies = [
- "libc",
- "stable_deref_trait",
-]
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memmap2"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fe751422e4a8caa417e13c3ea66452215d7d63e19e604f4980461212f3ae1322"
 dependencies = [
  "libc",
+ "stable_deref_trait",
 ]
 
 [[package]]
 name = "memoffset"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5de893c32cde5f383baa4c04c5d6dbdd735cfd4a794b0debdb2bb1b421da5ff4"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "memory-stats"
 version = "1.1.0"
@@ -3291,18 +3439,18 @@
 
 [[package]]
 name = "metal"
 version = "0.27.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c43f73953f8cbe511f021b58f18c3ce1c3d1ae13fe953293e13345bf83217f25"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "block",
  "core-graphics-types",
- "foreign-types 0.5.0",
+ "foreign-types",
  "log",
  "objc",
  "paste",
 ]
 
 [[package]]
 name = "mime"
@@ -3324,64 +3472,61 @@
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
  "simd-adler32",
 ]
 
 [[package]]
 name = "mio"
-version = "0.8.10"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8f3d0b296e374a4e6f3c7b0a1f5a51d748a0d34c85e7dc48fc3fa9a87657fe09"
+checksum = "a4a650543ca06a924e8b371db273b2756685faae30f8487da1b56505a8f78b0c"
 dependencies = [
  "libc",
  "log",
  "wasi",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
+name = "muldiv"
+version = "1.0.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "956787520e75e9bd233246045d19f42fb73242759cc57fba9611d940ae96d4b0"
+
+[[package]]
 name = "naga"
-version = "0.19.0"
+version = "0.19.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8878eb410fc90853da3908aebfe61d73d26d4437ef850b70050461f939509899"
+checksum = "50e3524642f53d9af419ab5e8dd29d3ba155708267667c2f3f06c88c9e130843"
 dependencies = [
  "bit-set",
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "codespan-reporting",
  "hexf-parse",
  "indexmap",
  "log",
  "num-traits",
  "rustc-hash",
  "spirv",
  "termcolor",
  "thiserror",
  "unicode-xid",
 ]
 
 [[package]]
-name = "nanorand"
-version = "0.7.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a51313c5820b0b02bd422f4b44776fbf47961755c74ce64afc73bfad10226c3"
-dependencies = [
- "getrandom",
-]
-
-[[package]]
 name = "natord"
 version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "308d96db8debc727c3fd9744aac51751243420e46edf401010908da7f8d5e57c"
 
 [[package]]
 name = "ndarray"
@@ -3399,15 +3544,15 @@
 
 [[package]]
 name = "ndk"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2076a31b7010b17a38c01907c45b945e8f11495ee4dd588309718901b1f7a5b7"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "jni-sys",
  "log",
  "ndk-sys",
  "num_enum",
  "raw-window-handle 0.6.0",
  "thiserror",
 ]
@@ -3431,17 +3576,17 @@
 name = "never"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c96aba5aa877601bb3f6dd6a63a969e1f82e60646e81e71b14496995e9853c91"
 
 [[package]]
 name = "new_debug_unreachable"
-version = "1.0.4"
+version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e4a24736216ec316047a1fc4252e27dabb04218aa4a3f37c6e7ddbf1f9782b54"
+checksum = "650eef8c711430f1a879fdd01d4745a7deea475becfb90269c06775983bbf086"
 
 [[package]]
 name = "nix"
 version = "0.26.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "598beaf3cc6fdd9a5dfb1630c2800c7acd31df7aaf0f565796fba2b53ca1af1b"
 dependencies = [
@@ -3475,15 +3620,15 @@
 
 [[package]]
 name = "notify"
 version = "6.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6205bd8bb1e454ad2e27422015fb5e4f2bcc7e08fa8f27058670d208324a4d2d"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "crossbeam-channel",
  "filetime",
  "fsevent-sys",
  "inotify",
  "kqueue",
  "libc",
  "log",
@@ -3510,51 +3655,45 @@
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-complex"
-version = "0.4.4"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ba157ca0885411de85d6ca030ba7e2a83a28636056c7c699b07c8b6f7383214"
+checksum = "23c6602fda94a57c990fe0df199a035d83576b496aa29f4e634a8ac6004e68a6"
 dependencies = [
  "bytemuck",
  "num-traits",
 ]
 
 [[package]]
-name = "num-derive"
-version = "0.3.3"
+name = "num-conv"
+version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "876a53fff98e03a936a674b29568b0e605f06b29372c2489ff4de23f1949743d"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 1.0.109",
-]
+checksum = "51d515d32fb182ee37cda2ccdcb92950d6a3c2893aa280e540671c2cd0f3b1d9"
 
 [[package]]
 name = "num-derive"
-version = "0.4.1"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cfb77679af88f8b125209d354a202862602672222e7f2313fdd6dc349bad4712"
+checksum = "ed3955f1a9c7c0c15e092f9c887db08b1fc683305fdf6eb6684f22555355e202"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "num-integer"
-version = "0.1.45"
+version = "0.1.46"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
+checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
 dependencies = [
- "autocfg",
  "num-traits",
 ]
 
 [[package]]
 name = "num-rational"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -3564,17 +3703,17 @@
  "num-bigint",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.17"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39e3200413f237f41ab11ad6d161bc7239c84dcb631773ccd7de3dfe4b5c267c"
+checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "num_cpus"
@@ -3597,30 +3736,36 @@
 
 [[package]]
 name = "num_enum_derive"
 version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "681030a937600a36906c185595136d26abfebb4aa9c65701cefcaf8578bb982b"
 dependencies = [
- "proc-macro-crate",
+ "proc-macro-crate 3.1.0",
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "num_threads"
-version = "0.1.6"
+version = "0.1.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2819ce041d2ee131036f4fc9d6ae7ae125a3a40e97ba64d04fe799ad9dabbb44"
+checksum = "5c7398b9c8b70908f6371f47ed36737907c87c52af34c268fed0bf0ceb92ead9"
 dependencies = [
  "libc",
 ]
 
 [[package]]
+name = "number_prefix"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "830b246a0e5f20af87141b25c173cd1b609bd7779a4617d6ec582abaf90870f3"
+
+[[package]]
 name = "objc"
 version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "915b1b472bc21c53464d6c8461c9d3af805ba1ef837e1cac254428f4a77177b1"
 dependencies = [
  "malloc_buf",
  "objc_exception",
@@ -3721,14 +3866,23 @@
 [[package]]
 name = "oorandom"
 version = "11.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ab1bc2a289d34bd04a330323ac98a1b4bc82c9d9fcb1e66b63caa84da26b575"
 
 [[package]]
+name = "option-operations"
+version = "0.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7c26d27bb1aeab65138e4bf7666045169d1717febcc9ff870166be8348b223d0"
+dependencies = [
+ "paste",
+]
+
+[[package]]
 name = "orbclient"
 version = "0.3.47"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "52f0d54bde9774d3a51dcf281a5def240c71996bc6ca05d2c847ec8b2b216166"
 dependencies = [
  "libredox 0.0.2",
 ]
@@ -3758,14 +3912,24 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d4586edfe4c648c71797a74c84bacb32b52b212eff5dfe2bb9f2c599844023e7"
 dependencies = [
  "ttf-parser",
 ]
 
 [[package]]
+name = "packed_simd"
+version = "0.3.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1f9f08af0c877571712e2e3e686ad79efad9657dbf0f7c3c8ba943ff6c38932d"
+dependencies = [
+ "cfg-if",
+ "num-traits",
+]
+
+[[package]]
 name = "parking"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bb813b8af86854136c6922af0598d719255ecb2179515e6e7730d468f05c9cae"
 
 [[package]]
 name = "parking_lot"
@@ -3832,61 +3996,41 @@
 [[package]]
 name = "percent-encoding"
 version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
-name = "pin-project"
-version = "1.1.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0302c4a0442c456bd56f841aee5c3bfd17967563f6fadc9ceb9f9c23cf3807e0"
-dependencies = [
- "pin-project-internal",
-]
-
-[[package]]
-name = "pin-project-internal"
-version = "1.1.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "266c042b60c9c76b8d53061e52b2e0d1116abc57cefc8c5cd671619a56ac3690"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 2.0.48",
-]
-
-[[package]]
 name = "pin-project-lite"
-version = "0.2.13"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "piper"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "668d31b1c4eba19242f2088b2bf3316b82ca31082a8335764db4e083db7485d4"
 dependencies = [
  "atomic-waker",
- "fastrand 2.0.1",
+ "fastrand 2.0.2",
  "futures-io",
 ]
 
 [[package]]
 name = "pkg-config"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2900ede94e305130c13ddd391e0ab7cbaeb783945ae07a279c268cb05109c6cb"
+checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
 
 [[package]]
 name = "planus"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fc1691dd09e82f428ce8d6310bd6d5da2557c82ff17694d2a32cad7242aea89f"
 dependencies = [
@@ -3931,17 +4075,17 @@
  "linked-hash-map",
  "peg",
  "skeptic",
 ]
 
 [[package]]
 name = "png"
-version = "0.17.11"
+version = "0.17.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f6c3c3e617595665b8ea2ff95a86066be38fb121ff920a9c0eb282abcd1da5a"
+checksum = "06e4b0d3d1312775e782c86c91a111aa1f910cbb65e1337f9975b5f9a554b5e1"
 dependencies = [
  "bitflags 1.3.2",
  "crc32fast",
  "fdeflate",
  "flate2",
  "miniz_oxide",
 ]
@@ -3972,33 +4116,40 @@
  "log",
  "pin-project-lite",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "polling"
-version = "3.3.2"
+version = "3.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "545c980a3880efd47b2e262f6a4bb6daad6555cf3367aa9c4e52895f69537a41"
+checksum = "e0c976a60b2d7e99d6f229e414670a9b85d13ac305cc6d1e9c134de58c5aaaf6"
 dependencies = [
  "cfg-if",
  "concurrent-queue",
+ "hermit-abi",
  "pin-project-lite",
- "rustix 0.38.30",
+ "rustix 0.38.32",
  "tracing",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "pollster"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "22686f4785f02a4fcc856d3b3bb19bf6c8160d103f7a99cc258bddd0251dc7f2"
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "powerfmt"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "439ee305def115ba05938db6eb1644ff94165c5ab5e9420d1c1bcedbba909391"
 
 [[package]]
 name = "ppv-lite86"
@@ -4010,71 +4161,68 @@
 name = "presser"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e8cf8e6a8aa66ce33f63993ffc4ea4271eb5b0530a9002db8455ea6050c77bfa"
 
 [[package]]
 name = "prettyplease"
-version = "0.2.16"
+version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a41cf62165e97c7f814d2221421dbb9afcbcdb0a88068e5ea206e19951c2cbb5"
+checksum = "8d3928fb5db768cb86f891ff014f0144589297e3c6a1aba6ed7cecfdace270c7"
 dependencies = [
  "proc-macro2",
- "syn 2.0.48",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "proc-macro-crate"
 version = "1.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f4c021e1093a56626774e81216a4ce732a735e5bad4868a03f3ed65ca0c3919"
 dependencies = [
  "once_cell",
  "toml_edit 0.19.15",
 ]
 
 [[package]]
+name = "proc-macro-crate"
+version = "3.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6d37c51ca738a55da99dc0c4a34860fd675453b8b36209178c2249bb13651284"
+dependencies = [
+ "toml_edit 0.21.1",
+]
+
+[[package]]
 name = "proc-macro2"
-version = "1.0.78"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
+checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "profiling"
-version = "1.0.13"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d135ede8821cf6376eb7a64148901e1690b788c11ae94dc297ae917dbc91dc0e"
+checksum = "43d84d1d7a6ac92673717f9f6d1518374ef257669c24ebc5ac25d5033828be58"
 dependencies = [
  "profiling-procmacros",
- "puffin 0.18.1",
+ "puffin",
 ]
 
 [[package]]
 name = "profiling-procmacros"
-version = "1.0.13"
+version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4b322d7d65c1ab449be3c890fcbd0db6e1092d0dd05d79dba2dd28032cebeb05"
+checksum = "8021cf59c8ec9c432cfc2526ac6b8aa508ecaf29cd415f271b8406c1b851c3fd"
 dependencies = [
  "quote",
- "syn 2.0.48",
-]
-
-[[package]]
-name = "puffin"
-version = "0.18.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "02330f795caafc2007510f742624c10aa813b8c3097c77ff344b1b86eb6be846"
-dependencies = [
- "anyhow",
- "byteorder",
- "cfg-if",
- "once_cell",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "puffin"
 version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b9f76ad4bb049fded4e572df72cbb6381ff5d1f41f85c3a04b56e4eca287a02f"
@@ -4095,33 +4243,33 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4936c085e48efc86f6d96609dc5086d1d236afe3ec4676f09b157a4f4be83ff6"
 dependencies = [
  "anyhow",
  "crossbeam-channel",
  "log",
  "parking_lot",
- "puffin 0.19.0",
+ "puffin",
 ]
 
 [[package]]
 name = "pulldown-cmark"
-version = "0.9.3"
+version = "0.9.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77a1a2f1f0a7ecff9c31abbe177637be0e97a0aef46cf8738ece09327985d998"
+checksum = "57206b407293d2bcd3af849ce869d52068623f19e1b5ff8e8778e3309439682b"
 dependencies = [
- "bitflags 1.3.2",
+ "bitflags 2.5.0",
  "memchr",
  "unicase",
 ]
 
 [[package]]
 name = "pulp"
-version = "0.18.6"
+version = "0.18.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "16785ee69419641c75affff7c9fdbdb7c0ab26dc9a5fb5218c2a2e9e4ef2087d"
+checksum = "03457ac216146f43f921500bac4e892d5cd32b0479b929cbfc90f95cd6c599c2"
 dependencies = [
  "bytemuck",
  "libm",
  "num-complex",
  "reborrow",
 ]
 
@@ -4196,94 +4344,58 @@
 dependencies = [
  "num-traits",
  "rand",
 ]
 
 [[package]]
 name = "rav1e"
-version = "0.6.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "16c383692a5e7abd9f6d1eddb1a5e0269f859392387883361bb09e5555852ec1"
-dependencies = [
- "arbitrary 0.4.7",
- "arg_enum_proc_macro",
- "arrayvec",
- "av1-grain",
- "bitstream-io 1.10.0",
- "built 0.5.2",
- "cfg-if",
- "interpolate_name",
- "itertools 0.10.5",
- "libc",
- "libfuzzer-sys 0.3.5",
- "log",
- "maybe-rayon",
- "new_debug_unreachable",
- "noop_proc_macro",
- "num-derive 0.3.3",
- "num-traits",
- "once_cell",
- "paste",
- "rand",
- "rand_chacha",
- "rust_hawktracer",
- "rustc_version",
- "simd_helpers",
- "system-deps",
- "thiserror",
- "v_frame",
- "wasm-bindgen",
-]
-
-[[package]]
-name = "rav1e"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cd87ce80a7665b1cce111f8a16c1f3929f6547ce91ade6addf4ec86a8dda5ce9"
 dependencies = [
- "arbitrary 1.3.2",
+ "arbitrary",
  "arg_enum_proc_macro",
  "arrayvec",
  "av1-grain",
- "bitstream-io 2.2.0",
- "built 0.7.1",
+ "bitstream-io",
+ "built",
  "cfg-if",
  "interpolate_name",
- "itertools 0.12.0",
+ "itertools 0.12.1",
  "libc",
- "libfuzzer-sys 0.4.7",
+ "libfuzzer-sys",
  "log",
  "maybe-rayon",
  "new_debug_unreachable",
  "noop_proc_macro",
- "num-derive 0.4.1",
+ "num-derive",
  "num-traits",
  "once_cell",
  "paste",
  "profiling",
  "rand",
  "rand_chacha",
  "simd_helpers",
  "system-deps",
  "thiserror",
  "v_frame",
+ "wasm-bindgen",
 ]
 
 [[package]]
 name = "ravif"
-version = "0.11.4"
+version = "0.11.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d44feba0b8a381a5efa2c0baf8dace8418904403260233f4a614503b018fc288"
+checksum = "bc13288f5ab39e6d7c9d501759712e6969fcc9734220846fc9ed26cae2cc4234"
 dependencies = [
  "avif-serialize",
  "imgref",
  "loop9",
  "quick-error",
- "rav1e 0.6.6",
- "rav1e 0.7.1",
+ "rav1e",
  "rayon",
  "rgb",
 ]
 
 [[package]]
 name = "raw-cpuid"
 version = "10.7.0"
@@ -4309,17 +4421,17 @@
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
 name = "rayon"
-version = "1.8.1"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa7237101a77a10773db45d62004a272517633fbcc3df19d96455ede1122e051"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
@@ -4399,31 +4511,31 @@
 [[package]]
 name = "re_crash_handler"
 version = "0.14.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "036d809ac9bb83b6536712373320bf6f7e8f2848fb6caa2905dde17cda1fb456"
 dependencies = [
  "backtrace",
- "itertools 0.12.0",
+ "itertools 0.12.1",
  "libc",
  "parking_lot",
  "re_analytics",
  "re_build_info",
 ]
 
 [[package]]
 name = "re_data_source"
 version = "0.14.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e71c3b1fe5e8b40fe9388c6dbc03ec06bbd577737f6810d29c4cd17d146eacb1"
 dependencies = [
  "ahash",
  "anyhow",
- "image 0.24.8",
- "itertools 0.12.0",
+ "image 0.24.9",
+ "itertools 0.12.1",
  "once_cell",
  "parking_lot",
  "rayon",
  "re_build_tools",
  "re_log",
  "re_log_encoding",
  "re_log_types",
@@ -4440,15 +4552,15 @@
 version = "0.14.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f4ba3191c5c83a4bd64bdcebab0df0b78570a0681b2e00b07651ab4bb7ed955c"
 dependencies = [
  "ahash",
  "document-features",
  "indent",
- "itertools 0.12.0",
+ "itertools 0.12.1",
  "nohash-hasher",
  "once_cell",
  "parking_lot",
  "re_arrow2",
  "re_error",
  "re_format",
  "re_log",
@@ -4468,16 +4580,16 @@
 dependencies = [
  "ahash",
  "anyhow",
  "bytemuck",
  "egui",
  "egui_extras",
  "egui_plot",
- "image 0.24.8",
- "itertools 0.12.0",
+ "image 0.24.9",
+ "itertools 0.12.1",
  "re_data_store",
  "re_entity_db",
  "re_error",
  "re_format",
  "re_log",
  "re_log_types",
  "re_query",
@@ -4495,15 +4607,15 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "77ca1661709691d4f7a493da1a1a8ce802b5c5864beb0bb07c465507c5c732b9"
 dependencies = [
  "ahash",
  "document-features",
  "emath",
  "getrandom",
- "itertools 0.12.0",
+ "itertools 0.12.1",
  "nohash-hasher",
  "parking_lot",
  "re_data_store",
  "re_format",
  "re_int_histogram",
  "re_log",
  "re_log_types",
@@ -4595,18 +4707,18 @@
  "backtrace",
  "bytemuck",
  "clean-path",
  "crossbeam",
  "document-features",
  "fixed",
  "half",
- "itertools 0.12.0",
+ "itertools 0.12.1",
  "natord",
  "nohash-hasher",
- "num-derive 0.4.1",
+ "num-derive",
  "num-traits",
  "re_arrow2",
  "re_format",
  "re_log",
  "re_string_interner",
  "re_tracing",
  "re_tuid",
@@ -4627,15 +4739,15 @@
 version = "0.14.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "473aeac52e20a1fd12d02a1b62c96f5e8a35858de017d2178edb0008db2e9303"
 dependencies = [
  "ahash",
  "backtrace",
  "emath",
- "itertools 0.12.0",
+ "itertools 0.12.1",
  "memory-stats",
  "nohash-hasher",
  "once_cell",
  "parking_lot",
  "re_format",
  "re_log",
  "re_tracing",
@@ -4649,15 +4761,15 @@
 name = "re_query"
 version = "0.14.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6f7bb9f69f80582b90e832742b7a906a6bcb46249975f8c3b5930e017cc15b31"
 dependencies = [
  "backtrace",
  "document-features",
- "itertools 0.12.0",
+ "itertools 0.12.1",
  "re_arrow2",
  "re_data_store",
  "re_format",
  "re_log",
  "re_log_types",
  "re_tracing",
  "re_types_core",
@@ -4670,15 +4782,15 @@
 name = "re_query_cache"
 version = "0.14.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f4ae9b4d0cfac08988a00a8847930c4ddf54b527bba3c80e70dfcf0b0ca5314"
 dependencies = [
  "ahash",
  "indent",
- "itertools 0.12.0",
+ "itertools 0.12.1",
  "parking_lot",
  "paste",
  "re_data_store",
  "re_format",
  "re_log",
  "re_log_types",
  "re_query",
@@ -4692,28 +4804,28 @@
 name = "re_renderer"
 version = "0.14.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "42289ce2cf8bd439096ec2a47c89f12491db6b762dc4d3296be090dcd106296f"
 dependencies = [
  "ahash",
  "anyhow",
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "bytemuck",
  "cfg-if",
  "cfg_aliases 0.2.0",
  "clean-path",
  "crossbeam",
  "document-features",
  "ecolor",
  "enumset",
  "getrandom",
  "glam",
  "gltf",
  "half",
- "itertools 0.12.0",
+ "itertools 0.12.1",
  "macaw",
  "never",
  "notify",
  "ordered-float",
  "parking_lot",
  "pathdiff",
  "profiling",
@@ -4792,15 +4904,15 @@
 name = "re_space_view"
 version = "0.14.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "03085994b975ee3fe13af693dd0b8bd05220cf468af55fa57f7033da25840683"
 dependencies = [
  "ahash",
  "egui",
- "itertools 0.12.0",
+ "itertools 0.12.1",
  "nohash-hasher",
  "re_data_store",
  "re_entity_db",
  "re_log",
  "re_log_types",
  "re_query",
  "re_tracing",
@@ -4855,19 +4967,19 @@
 name = "re_space_view_spatial"
 version = "0.14.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "20478d9c80bd9996eba5e579b856dbf3171188da40118cd3496f17b8ee629644"
 dependencies = [
  "ahash",
  "anyhow",
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "bytemuck",
  "egui",
  "glam",
- "itertools 0.12.0",
+ "itertools 0.12.1",
  "macaw",
  "nohash-hasher",
  "once_cell",
  "parking_lot",
  "rayon",
  "re_data_store",
  "re_data_ui",
@@ -4921,15 +5033,15 @@
 name = "re_space_view_text_document"
 version = "0.14.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ad5920c0549deb79c5a983ef6282802559187bd08d39f1d9889c18942888513"
 dependencies = [
  "egui",
  "egui_commonmark",
- "itertools 0.12.0",
+ "itertools 0.12.1",
  "re_data_store",
  "re_log",
  "re_query",
  "re_renderer",
  "re_space_view",
  "re_tracing",
  "re_types",
@@ -4941,15 +5053,15 @@
 name = "re_space_view_text_log"
 version = "0.14.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e85022ac7be1a816200fbaef53c2248ad5c2be3767ad74fee84b1ab7c09deb11"
 dependencies = [
  "egui",
  "egui_extras",
- "itertools 0.12.0",
+ "itertools 0.12.1",
  "re_data_store",
  "re_data_ui",
  "re_entity_db",
  "re_log",
  "re_log_types",
  "re_query_cache",
  "re_renderer",
@@ -4963,15 +5075,15 @@
 name = "re_space_view_time_series"
 version = "0.14.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06a115e137cbea9ebafd0502681a05ec686a23f1c83b940c2d9eb677a99cc350"
 dependencies = [
  "egui",
  "egui_plot",
- "itertools 0.12.0",
+ "itertools 0.12.1",
  "parking_lot",
  "rayon",
  "re_data_store",
  "re_format",
  "re_log",
  "re_log_types",
  "re_query",
@@ -5001,15 +5113,15 @@
 [[package]]
 name = "re_time_panel"
 version = "0.14.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "84e8cb9e9e6db76edb4ba85c506cd90f59f9a48ac97403c5ffe32b92e4110c99"
 dependencies = [
  "egui",
- "itertools 0.12.0",
+ "itertools 0.12.1",
  "re_data_store",
  "re_data_ui",
  "re_entity_db",
  "re_format",
  "re_log_types",
  "re_tracing",
  "re_ui",
@@ -5020,15 +5132,15 @@
 
 [[package]]
 name = "re_tracing"
 version = "0.14.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf3418cd8e373c23cd0e174b994f662f53f896431550f10c98707e2ffb6057fe"
 dependencies = [
- "puffin 0.19.0",
+ "puffin",
  "puffin_http",
  "re_log",
  "rfd",
 ]
 
 [[package]]
 name = "re_tuid"
@@ -5053,17 +5165,17 @@
  "array-init",
  "bytemuck",
  "document-features",
  "ecolor",
  "egui_plot",
  "glam",
  "half",
- "image 0.24.8",
+ "image 0.24.9",
  "infer",
- "itertools 0.12.0",
+ "itertools 0.12.1",
  "linked-hash-map",
  "mime_guess2",
  "ndarray",
  "once_cell",
  "ply-rs",
  "rayon",
  "re_arrow2",
@@ -5087,25 +5199,25 @@
 dependencies = [
  "anyhow",
  "camino",
  "clang-format",
  "convert_case",
  "flatbuffers",
  "indent",
- "itertools 0.12.0",
+ "itertools 0.12.1",
  "prettyplease",
  "proc-macro2",
  "quote",
  "rayon",
  "re_arrow2",
  "re_build_tools",
  "re_log",
  "re_tracing",
  "rust-format",
- "syn 2.0.48",
+ "syn 2.0.57",
  "tempfile",
  "unindent",
  "xshell",
 ]
 
 [[package]]
 name = "re_types_core"
@@ -5160,16 +5272,16 @@
  "eframe",
  "egui",
  "egui-wgpu",
  "egui_extras",
  "egui_plot",
  "egui_tiles",
  "ehttp",
- "image 0.24.8",
- "itertools 0.12.0",
+ "image 0.24.9",
+ "itertools 0.12.1",
  "once_cell",
  "poll-promise",
  "re_analytics",
  "re_build_info",
  "re_build_tools",
  "re_data_source",
  "re_data_store",
@@ -5225,15 +5337,15 @@
  "bit-vec",
  "bytemuck",
  "egui",
  "egui-wgpu",
  "egui_tiles",
  "glam",
  "half",
- "itertools 0.12.0",
+ "itertools 0.12.1",
  "macaw",
  "ndarray",
  "nohash-hasher",
  "once_cell",
  "parking_lot",
  "re_data_source",
  "re_data_store",
@@ -5260,16 +5372,16 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b2222e1def841fd03fa67d6c6d408ce6812af6fed4f13d61c27a7a392c062c98"
 dependencies = [
  "ahash",
  "egui",
  "egui_tiles",
  "glam",
- "image 0.24.8",
- "itertools 0.12.0",
+ "image 0.24.9",
+ "itertools 0.12.1",
  "nohash-hasher",
  "once_cell",
  "rayon",
  "re_arrow2",
  "re_data_store",
  "re_data_ui",
  "re_entity_db",
@@ -5355,65 +5467,65 @@
  "getrandom",
  "libredox 0.0.1",
  "thiserror",
 ]
 
 [[package]]
 name = "regex"
-version = "1.10.3"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b62dbe01f0b06f9d8dc7d49e05a0785f153b00b2c227856282f671e0318c9b15"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
- "regex-automata 0.4.5",
+ "regex-automata 0.4.6",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6c230d73fb8d8c1b9c0b3135c5142a8acee3a0558fb8db5cf1cb65f8d7862132"
 
 [[package]]
 name = "regex-automata"
-version = "0.4.5"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5bb987efffd3c6d0d8f5f89510bb458559eab11e4f869acb20bf845e016259cd"
+checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "renderdoc-sys"
-version = "1.0.0"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "216080ab382b992234dda86873c18d4c48358f5cfcb70fd693d7f6f2131b628b"
+checksum = "19b30a45b0cd0bcca8037f3d0dc3421eaf95327a17cad11964fb8179b4fc4832"
 
 [[package]]
 name = "rerun"
 version = "0.14.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2a3bdd0368df6721666b743c61c714972a81f7e5f0952994dbdee511eaeb965"
 dependencies = [
  "anyhow",
  "document-features",
  "env_logger",
- "itertools 0.12.0",
+ "itertools 0.12.1",
  "log",
- "puffin 0.19.0",
+ "puffin",
  "rayon",
  "re_analytics",
  "re_build_info",
  "re_build_tools",
  "re_crash_handler",
  "re_entity_db",
  "re_format",
@@ -5461,24 +5573,25 @@
 checksum = "05aaa8004b64fd573fc9d002f4e632d51ad4f026c2b5ba95fcb6c2f32c2c47d8"
 dependencies = [
  "bytemuck",
 ]
 
 [[package]]
 name = "ring"
-version = "0.17.7"
+version = "0.17.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "688c63d65483050968b2a8937f7995f443e27041a0f7700aa59b0822aedebb74"
+checksum = "c17fa4cb658e3583423e915b9f3acc01cceaee1860e33d59ebae66adc3a2dc0d"
 dependencies = [
  "cc",
+ "cfg-if",
  "getrandom",
  "libc",
  "spin",
  "untrusted",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rmp"
 version = "0.8.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f9860a6cc38ed1da53456442089b4dfa35e7cedaa326df63017af88385e6b20"
@@ -5502,48 +5615,26 @@
 [[package]]
 name = "ron"
 version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b91f7eff05f748767f183df4320a63d6936e9c6107d97c9e6bdd9784f4289c94"
 dependencies = [
  "base64 0.21.7",
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "serde",
  "serde_derive",
 ]
 
 [[package]]
 name = "rust-format"
 version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60e7c00b6c3bf5e38a880eec01d7e829d12ca682079f8238a464def3c4b31627"
 
 [[package]]
-name = "rust_hawktracer"
-version = "0.7.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e3480a29b927f66c6e06527be7f49ef4d291a01d694ec1fe85b0de71d6b02ac1"
-dependencies = [
- "rust_hawktracer_normal_macro",
- "rust_hawktracer_proc_macro",
-]
-
-[[package]]
-name = "rust_hawktracer_normal_macro"
-version = "0.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a570059949e1dcdc6f35228fa389f54c2c84dfe0c94c05022baacd56eacd2e9"
-
-[[package]]
-name = "rust_hawktracer_proc_macro"
-version = "0.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb626abdbed5e93f031baae60d72032f56bc964e11ac2ff65f2ba3ed98d6d3e1"
-
-[[package]]
 name = "rustc-demangle"
 version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
 
 [[package]]
 name = "rustc-hash"
@@ -5572,64 +5663,73 @@
  "libc",
  "linux-raw-sys 0.3.8",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.30"
+version = "0.38.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "322394588aaf33c24007e8bb3238ee3e4c5c09c084ab32bc73890b99ff326bca"
+checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys 0.4.13",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.21.10"
+version = "0.22.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9d5a6813c0759e4609cd494e8e725babae6a2ca7b62a5536a13daaec6fcb7ba"
+checksum = "99008d7ad0bbbea527ec27bddbc0e432c5b87d8175178cee68d2eec9c4a1813c"
 dependencies = [
  "log",
  "ring",
+ "rustls-pki-types",
  "rustls-webpki",
- "sct",
+ "subtle",
+ "zeroize",
 ]
 
 [[package]]
+name = "rustls-pki-types"
+version = "1.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ecd36cc4259e3e4514335c4a138c6b43171a8d61d8f5c9348f9fc7529416f247"
+
+[[package]]
 name = "rustls-webpki"
-version = "0.101.7"
+version = "0.102.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b6275d1ee7a1cd780b64aca7726599a1dbc893b1e64144529e55c3c2f745765"
+checksum = "faaa0a62740bedb9b2ef5afa303da42764c012f743917351dc9a237ea1663610"
 dependencies = [
  "ring",
+ "rustls-pki-types",
  "untrusted",
 ]
 
 [[package]]
 name = "rustversion"
 version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7ffc183a10b4478d04cbbbfc96d0873219d962dd5accaff2ffbd4ceb7df837f4"
 
 [[package]]
 name = "ryu"
-version = "1.0.16"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f98d2aa92eebf49b69786be48e4477826b256916e84a57ff2a4f21923b48eb4c"
+checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
 [[package]]
 name = "safetensors"
-version = "0.3.3"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d93279b86b3de76f820a8854dd06cbc33cfa57a417b19c47f6a25280112fb1df"
+checksum = "8d980e6bfb34436fb0a81e42bc41af43f11805bbbca443e7f68e9faaabe669ed"
 dependencies = [
  "serde",
  "serde_json",
 ]
 
 [[package]]
 name = "same-file"
@@ -5649,43 +5749,33 @@
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
-name = "sct"
-version = "0.7.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da046153aa2352493d6cb7da4b6e5c0c057d8a1d0a9aa8560baffdd945acd414"
-dependencies = [
- "ring",
- "untrusted",
-]
-
-[[package]]
 name = "semver"
-version = "1.0.21"
+version = "1.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b97ed7a9823b74f99c7742f5336af7be5ecd3eeafcb1507d1fa93347b1d589b0"
+checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "seq-macro"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a3f0bf26fd526d2a95683cd0f87bf103b8539e2ca1ef48ce002d67aad59aa0b4"
 
 [[package]]
 name = "serde"
-version = "1.0.196"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "870026e60fa08c69f064aa766c10f10b1d62db9ccd4d0abb206472bee0ce3b32"
+checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_bytes"
 version = "0.11.14"
@@ -5693,43 +5783,43 @@
 checksum = "8b8497c313fd43ab992087548117643f6fcd935cbf36f176ffda0aacf9591734"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.196"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "33c85360c95e7d137454dc81d9a4ed2b8efd8fbe19cee57357b32b9771fccb67"
+checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.112"
+version = "1.0.115"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4d1bd37ce2324cf3bf85e5a25f96eb4baf0d5aa6eba43e7ae8958870c4ec48ed"
+checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
 name = "serde_repr"
 version = "0.1.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b2e6b945e9d3df726b65d6ee24060aff8e3533d431f677a9695db04eff9dfdb"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "serde_spanned"
 version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eb3622f419d1296904700073ea6cc23ad690adbd66f13ea683df73298736f0c1"
@@ -5787,17 +5877,17 @@
 name = "simdutf8"
 version = "0.1.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f27f6278552951f1f2b8cf9da965d10969b2efdea95a6ec47987ab46edfe263a"
 
 [[package]]
 name = "similar"
-version = "2.4.0"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32fea41aca09ee824cc9724996433064c89f7777e60762749a4170a14abbfa21"
+checksum = "fa42c91313f1d05da9b26f267f931cf178d4aba455b4c4622dd7355eb80c6640"
 dependencies = [
  "bstr",
  "unicode-segmentation",
 ]
 
 [[package]]
 name = "similar-asserts"
@@ -5841,51 +5931,51 @@
 dependencies = [
  "serde",
  "version_check",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "smithay-client-toolkit"
 version = "0.18.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "922fd3eeab3bd820d76537ce8f582b1cf951eceb5475c28500c7457d9d17f53a"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "calloop",
  "calloop-wayland-source",
  "cursor-icon",
  "libc",
  "log",
- "memmap2 0.9.4",
- "rustix 0.38.30",
+ "memmap2",
+ "rustix 0.38.32",
  "thiserror",
  "wayland-backend",
  "wayland-client",
  "wayland-csd-frame",
  "wayland-cursor",
  "wayland-protocols",
  "wayland-protocols-wlr",
  "wayland-scanner",
  "xkeysym",
 ]
 
 [[package]]
 name = "smithay-clipboard"
-version = "0.7.0"
+version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0bb62b280ce5a5cba847669933a0948d00904cf83845c944eae96a4738cea1a6"
+checksum = "c091e7354ea8059d6ad99eace06dd13ddeedbb0ac72d40a9a6e7ff790525882d"
 dependencies = [
  "libc",
  "smithay-client-toolkit",
  "wayland-backend",
 ]
 
 [[package]]
@@ -5905,20 +5995,20 @@
 dependencies = [
  "libc",
  "winapi",
 ]
 
 [[package]]
 name = "socket2"
-version = "0.5.5"
+version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b5fac59a5cb5dd637972e5fca70daf0523c9067fcdc4842f053dae04a18f8e9"
+checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
 dependencies = [
  "libc",
- "windows-sys 0.48.0",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "spin"
 version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
@@ -5928,15 +6018,15 @@
 
 [[package]]
 name = "spirv"
 version = "0.3.0+sdk-1.3.268.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eda41003dc44290527a59b13432d4a0379379fa074b70174882adfbdfd917844"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "stable_deref_trait"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a8f112729512f8e442d81f95a8a7ddf2b7c6b8a1a6f509a95864142b30cab2d3"
@@ -5944,24 +6034,18 @@
 [[package]]
 name = "static_assertions"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a2eb9349b6444b326872e140eb1cf5e7c522154d69e7a0ffb0fb81c06b37543f"
 
 [[package]]
-name = "str-buf"
-version = "1.0.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e08d8363704e6c71fc928674353e6b7c23dcea9d82d7012c8faf2a3a025f8d0"
-
-[[package]]
 name = "strsim"
-version = "0.10.0"
+version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
+checksum = "5ee073c9e4cd00e28217186dbe12796d692868f432bf2e97ee73bed0c56dfa01"
 
 [[package]]
 name = "strum"
 version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "290d54ea6f91c969195bdbcd7442c8c2a2ba87da8bf60a7ee86a235d4bc1e125"
 dependencies = [
@@ -5970,134 +6054,152 @@
 
 [[package]]
 name = "strum_macros"
 version = "0.25.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23dc1fa9ac9c169a78ba62f0b841814b7abae11bdd047b9c58f893439e309ea0"
 dependencies = [
- "heck",
+ "heck 0.4.1",
  "proc-macro2",
  "quote",
  "rustversion",
- "syn 2.0.48",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "sublime_fuzzy"
 version = "0.7.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fa7986063f7c0ab374407e586d7048a3d5aac94f103f751088bf398e07cd5400"
 
 [[package]]
+name = "subtle"
+version = "2.5.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "81cdd64d312baedb58e21336b31bc043b77e01cc99033ce76ef539f78e965ebc"
+
+[[package]]
 name = "syn"
 version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.48"
+version = "2.0.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f3531638e407dfc0814761abb7c00a5b54992b849452a0646b7f65c9f770f3f"
+checksum = "11a6ae1e52eb25aab8f3fb9fca13be982a373b8f1157ca14b897a825ba4a2d35"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "synstructure"
-version = "0.13.0"
+version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "285ba80e733fac80aa4270fbcdf83772a79b80aa35c97075320abfee4a915b06"
+checksum = "c8af7666ab7b6390ab78131fb5b0fce11d6b7a6951602017c35fa82800708971"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
- "unicode-xid",
+ "syn 2.0.57",
+]
+
+[[package]]
+name = "sysctl"
+version = "0.5.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ec7dddc5f0fee506baf8b9fdb989e242f17e4b11c61dfbb0635b705217199eea"
+dependencies = [
+ "bitflags 2.5.0",
+ "byteorder",
+ "enum-as-inner",
+ "libc",
+ "thiserror",
+ "walkdir",
 ]
 
 [[package]]
 name = "sysinfo"
-version = "0.30.5"
+version = "0.30.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1fb4f3438c8f6389c864e61221cbc97e9bca98b4daf39a5beb7bea660f528bb2"
+checksum = "0c385888ef380a852a16209afc8cfad22795dd8873d69c9a14d2e2088f118d18"
 dependencies = [
  "cfg-if",
  "core-foundation-sys",
  "libc",
  "ntapi",
  "once_cell",
  "windows 0.52.0",
 ]
 
 [[package]]
 name = "system-deps"
-version = "6.2.0"
+version = "6.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2a2d580ff6a20c55dfb86be5f9c238f67835d0e81cbdea8bf5680e0897320331"
+checksum = "a3e535eb8dded36d55ec13eddacd30dec501792ff23a0b1682c38601b8cf2349"
 dependencies = [
  "cfg-expr",
- "heck",
+ "heck 0.5.0",
  "pkg-config",
- "toml 0.8.10",
+ "toml",
  "version-compare",
 ]
 
 [[package]]
 name = "target-lexicon"
 version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "tempfile"
-version = "3.9.0"
+version = "3.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "01ce4141aa927a6d1bd34a041795abd0db1cccba5d5f24b009f694bdf3a1f3fa"
+checksum = "85b77fafb263dd9d05cbeac119526425676db3784113aa9295c88498cbf8bff1"
 dependencies = [
  "cfg-if",
- "fastrand 2.0.1",
- "redox_syscall 0.4.1",
- "rustix 0.38.30",
+ "fastrand 2.0.2",
+ "rustix 0.38.32",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "termcolor"
 version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06794f8f6c5c898b3275aebefa6b8a1cb24cd2c6c79397ab15774837a0bc5755"
 dependencies = [
  "winapi-util",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.56"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d54378c645627613241d077a3a79db965db602882668f9136ac42af9ecb730ad"
+checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.56"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa0faa943b50f3db30a20aa7e265dbc66076993efed8463e8de414e5d06d3471"
+checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "tiff"
 version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ba1310fcea54c6a9a4fd1aad794ecc02c31682f6bfbecdf460bf19533eed1e3e"
@@ -6105,22 +6207,23 @@
  "flate2",
  "jpeg-decoder",
  "weezl",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.31"
+version = "0.3.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f657ba42c3f86e7680e53c8cd3af8abbe56b5491790b46e22e19c0d57463583e"
+checksum = "c8248b6521bb14bc45b4067159b9b6ad792e2d6d754d6c41fb50e29fefe38749"
 dependencies = [
  "deranged",
  "itoa",
  "js-sys",
  "libc",
+ "num-conv",
  "num_threads",
  "powerfmt",
  "serde",
  "time-core",
  "time-macros",
 ]
 
@@ -6128,18 +6231,19 @@
 name = "time-core"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef927ca75afb808a4d64dd374f00a2adf8d0fcff8e7b184af886c3c87ec4a3f3"
 
 [[package]]
 name = "time-macros"
-version = "0.2.16"
+version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26197e33420244aeb70c3e8c78376ca46571bc4e701e4791c2cd9f57dcb3a43f"
+checksum = "7ba3a3ef41e6672a2f0f001392bb5dcd3ff0a9992d618ca761a11c3121547774"
 dependencies = [
+ "num-conv",
  "time-core",
 ]
 
 [[package]]
 name = "tinystl"
 version = "0.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -6171,47 +6275,49 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tobj"
-version = "4.0.1"
+version = "4.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5f7ca3ec0405b0f2f95e0dbcced28882190dc79b0dac63ff82533d256d770223"
+checksum = "c3bd4ba05f29e4c65b6c0c11a58b6465ffa820bac890d76ad407b4e81d8372e8"
 dependencies = [
  "ahash",
 ]
 
 [[package]]
 name = "tokio"
-version = "1.35.1"
+version = "1.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c89b4efa943be685f629b149f53829423f8f5531ea21249408e8e2f8671ec104"
+checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
 dependencies = [
  "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
+ "parking_lot",
  "pin-project-lite",
- "socket2 0.5.5",
+ "signal-hook-registry",
+ "socket2 0.5.6",
  "tokio-macros",
  "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-macros"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "tokio-util"
 version = "0.7.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5419f34732d9eb6ee4c3578b7989078579b7f039cbbb9ca2c4da015749371e15"
@@ -6222,31 +6328,22 @@
  "pin-project-lite",
  "tokio",
  "tracing",
 ]
 
 [[package]]
 name = "toml"
-version = "0.5.11"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f4f7f0dd8d50a853a531c426359045b1998f04219d88799810762cd4ad314234"
-dependencies = [
- "serde",
-]
-
-[[package]]
-name = "toml"
-version = "0.8.10"
+version = "0.8.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a9aad4a3066010876e8dcf5a8a06e70a558751117a145c6ce2b82c2e2054290"
+checksum = "e9dd1545e8208b4a5af1aa9bbd0b4cf7e9ea08fabc5d0a5c67fcaafa17433aa3"
 dependencies = [
  "serde",
  "serde_spanned",
  "toml_datetime",
- "toml_edit 0.22.6",
+ "toml_edit 0.22.9",
 ]
 
 [[package]]
 name = "toml_datetime"
 version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
@@ -6258,22 +6355,33 @@
 name = "toml_edit"
 version = "0.19.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b5bb770da30e5cbfde35a2d7b9b8a2c4b8ef89548a7a6aeab5c9a576e3e7421"
 dependencies = [
  "indexmap",
  "toml_datetime",
- "winnow 0.5.35",
+ "winnow 0.5.40",
 ]
 
 [[package]]
 name = "toml_edit"
-version = "0.22.6"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2c1b5fd4128cc8d3e0cb74d4ed9a9cc7c7284becd4df68f5f940e1ad123606f6"
+checksum = "6a8534fd7f78b5405e860340ad6575217ce99f38d4d5c8f2442cb5ecb50090e1"
+dependencies = [
+ "indexmap",
+ "toml_datetime",
+ "winnow 0.5.40",
+]
+
+[[package]]
+name = "toml_edit"
+version = "0.22.9"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "8e40bb779c5187258fd7aad0eb68cb8706a0a81fa712fbea808ab43c4b8374c4"
 dependencies = [
  "indexmap",
  "serde",
  "serde_spanned",
  "toml_datetime",
  "winnow 0.6.5",
 ]
@@ -6300,15 +6408,15 @@
 name = "tracing-attributes"
 version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
@@ -6326,36 +6434,36 @@
 name = "ttf-parser"
 version = "0.20.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "17f77d76d837a7830fe1d4f12b7b4ba4192c1888001c7164257e4bc6d21d96b4"
 
 [[package]]
 name = "tungstenite"
-version = "0.20.1"
+version = "0.21.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e3dac10fd62eaf6617d3a904ae222845979aec67c615d1c842b4002c7666fb9"
+checksum = "9ef1a641ea34f399a848dea702823bbecfb4c486f911735368f1f137cb8257e1"
 dependencies = [
  "byteorder",
  "bytes",
  "data-encoding",
- "http",
+ "http 1.1.0",
  "httparse",
  "log",
  "rand",
  "sha1",
  "thiserror",
  "url",
  "utf-8",
 ]
 
 [[package]]
 name = "turbojpeg"
-version = "1.0.0"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eb5080f5adaa92c82bf84f825dd092e9692c923ee652f1634835e9a1f372518d"
+checksum = "9af71fa2654444c8dcb711ecbb8f9202778f8421badf71c3d5a118f1570391ed"
 dependencies = [
  "libc",
  "thiserror",
  "turbojpeg-sys",
 ]
 
 [[package]]
@@ -6397,15 +6505,15 @@
 
 [[package]]
 name = "uds_windows"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "89daebc3e6fd160ac4aa9fc8b3bf71e1f74fbf92367ae71fb83a037e8bf164b9"
 dependencies = [
- "memoffset 0.9.0",
+ "memoffset 0.9.1",
  "tempfile",
  "winapi",
 ]
 
 [[package]]
 name = "unicase"
 version = "2.7.0"
@@ -6425,26 +6533,26 @@
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unicode-normalization"
-version = "0.1.22"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
+checksum = "a56d1686db2308d901306f92a263857ef59ea39678a5458e7cb17f01415101f5"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
 name = "unicode-segmentation"
-version = "1.10.1"
+version = "1.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1dd624098567895118886609431a7c3b8f516e41d30e0643f03d94592a147e36"
+checksum = "d4c87d22b6e3f4a18d4d40ef354e97c90fcb14dd91d7dc0aa9d8a1172ebf7202"
 
 [[package]]
 name = "unicode-width"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e51733f11c9c4f72aa0c160008246859e340b00807569a0da0e7a1079b27ba85"
 
@@ -6464,23 +6572,24 @@
 name = "untrusted"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ecb6da28b8a351d773b68d5825ac39017e680750f980f3a1a85cd8dd28a47c1"
 
 [[package]]
 name = "ureq"
-version = "2.9.1"
+version = "2.9.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f8cdd25c339e200129fe4de81451814e5228c9b771d57378817d6117cc2b3f97"
+checksum = "11f214ce18d8b2cbe84ed3aa6486ed3f5b285cf8d8fbdbce9f3f767a724adc35"
 dependencies = [
  "base64 0.21.7",
  "flate2",
  "log",
  "once_cell",
  "rustls",
+ "rustls-pki-types",
  "rustls-webpki",
  "url",
  "webpki-roots",
 ]
 
 [[package]]
 name = "url"
@@ -6510,17 +6619,17 @@
 name = "utf8parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "711b9620af191e0cdc7468a8d14e709c3dcdb115b36f838e601583af800a370a"
 
 [[package]]
 name = "uuid"
-version = "1.7.0"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f00cc9702ca12d3c81455259621e676d0f7251cec66a21e98fe2e9a37db93b2a"
+checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
 dependencies = [
  "getrandom",
  "serde",
  "wasm-bindgen",
 ]
 
 [[package]]
@@ -6532,23 +6641,23 @@
  "aligned-vec",
  "num-traits",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "vec1"
-version = "1.10.1"
+version = "1.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2bda7c41ca331fe9a1c278a9e7ee055f4be7f5eb1c2b72f079b4ff8b5fce9d5c"
+checksum = "ffb60dcfffc189bfd4e2a81333c268619fee9db53da71bce2bcbd8e129c56936"
 
 [[package]]
 name = "version-compare"
-version = "0.1.1"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "579a42fc0b8e0c63b76519a339be31bed574929511fa53c1a3acae26eb258f29"
+checksum = "852e951cb7832cb45cb1169900d19760cfa39b82bc0ea9c0e5a14ae88411c98b"
 
 [[package]]
 name = "version_check"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "49874b5167b65d7193b8aba1567f5c7d93d001cafc34600cee003eda787e483f"
 
@@ -6556,17 +6665,17 @@
 name = "waker-fn"
 version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f3c4517f54858c779bbcbf228f4fca63d121bf85fbecb2dc578cdf4a39395690"
 
 [[package]]
 name = "walkdir"
-version = "2.4.0"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d71d857dc86794ca4c280d616f7da00d2dbfd8cd788846559a6813e6aa4b54ee"
+checksum = "29790946404f91d9c5d06f9874efddea1dc06c5efe94541a7d6863108e3a5e4b"
 dependencies = [
  "same-file",
  "winapi-util",
 ]
 
 [[package]]
 name = "want"
@@ -6581,77 +6690,77 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.90"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1223296a201415c7fad14792dbefaace9bd52b62d33453ade1c5b5f07555406"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.90"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fcdc935b63408d58a32f8cc9738a0bffd8f05cc7c002086c6ef20b7312ad9dcd"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.40"
+version = "0.4.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bde2032aeb86bdfaecc8b261eef3cba735cc426c1f3a3416d1e0791be95fc461"
+checksum = "76bc14366121efc8dbb487ab05bcc9d346b3b5ec0eaa76e46594cabbe51762c0"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.90"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e4c238561b2d428924c49815533a8b9121c664599558a5d9ec51f8a1740a999"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.90"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bae1abb6806dc1ad9e560ed242107c0f6c84335f1749dd4e8ddb012ebd5e25a7"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.90"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4d91413b1c31d7539ba5ef2451af3f0b833a005eb27a631cec32bc0635a8602b"
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
 name = "wasm-streams"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b65dc4c90b63b118468cf747d8bf3566c1913ef60be765b5730ead9e0a3ba129"
 dependencies = [
@@ -6666,86 +6775,86 @@
 name = "wayland-backend"
 version = "0.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d50fa61ce90d76474c87f5fc002828d81b32677340112b4ef08079a9d459a40"
 dependencies = [
  "cc",
  "downcast-rs",
- "rustix 0.38.30",
+ "rustix 0.38.32",
  "scoped-tls",
  "smallvec",
  "wayland-sys",
 ]
 
 [[package]]
 name = "wayland-client"
 version = "0.31.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "82fb96ee935c2cea6668ccb470fb7771f6215d1691746c2d896b447a00ad3f1f"
 dependencies = [
- "bitflags 2.4.2",
- "rustix 0.38.30",
+ "bitflags 2.5.0",
+ "rustix 0.38.32",
  "wayland-backend",
  "wayland-scanner",
 ]
 
 [[package]]
 name = "wayland-csd-frame"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "625c5029dbd43d25e6aa9615e88b829a5cad13b2819c4ae129fdbb7c31ab4c7e"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "cursor-icon",
  "wayland-backend",
 ]
 
 [[package]]
 name = "wayland-cursor"
 version = "0.31.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "71ce5fa868dd13d11a0d04c5e2e65726d0897be8de247c0c5a65886e283231ba"
 dependencies = [
- "rustix 0.38.30",
+ "rustix 0.38.32",
  "wayland-client",
  "xcursor",
 ]
 
 [[package]]
 name = "wayland-protocols"
 version = "0.31.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f81f365b8b4a97f422ac0e8737c438024b5951734506b0e1d775c73030561f4"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "wayland-backend",
  "wayland-client",
  "wayland-scanner",
 ]
 
 [[package]]
 name = "wayland-protocols-plasma"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "23803551115ff9ea9bce586860c5c5a971e360825a0309264102a9495a5ff479"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "wayland-backend",
  "wayland-client",
  "wayland-protocols",
  "wayland-scanner",
 ]
 
 [[package]]
 name = "wayland-protocols-wlr"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ad1f61b76b6c2d8742e10f9ba5c3737f6530b4c243132c2a2ccc8aa96fe25cd6"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "wayland-backend",
  "wayland-client",
  "wayland-protocols",
  "wayland-scanner",
 ]
 
 [[package]]
@@ -6789,46 +6898,49 @@
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "webbrowser"
-version = "0.8.12"
+version = "0.8.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "82b2391658b02c27719fc5a0a73d6e696285138e8b12fba9d4baa70451023c71"
+checksum = "d1b04c569c83a9bb971dd47ec6fd48753315f4bf989b9b04a2e7ca4d7f0dc950"
 dependencies = [
  "core-foundation",
  "home",
  "jni",
  "log",
  "ndk-context",
  "objc",
  "raw-window-handle 0.5.2",
  "url",
  "web-sys",
 ]
 
 [[package]]
 name = "webpki-roots"
-version = "0.25.3"
+version = "0.26.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1778a42e8b3b90bff8d0f5032bf22250792889a5cdc752aa0020c84abe3aaf10"
+checksum = "b3de34ae270483955a94f4b21bdaaeb83d508bb84a01435f393818edb0012009"
+dependencies = [
+ "rustls-pki-types",
+]
 
 [[package]]
 name = "weezl"
 version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53a85b86a771b1c87058196170769dd264f66c0782acf1ae6cc51bfd64b39082"
 
 [[package]]
 name = "wgpu"
-version = "0.19.1"
+version = "0.19.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0bfe9a310dcf2e6b85f00c46059aaeaf4184caa8e29a1ecd4b7a704c3482332d"
+checksum = "a4b1213b52478a7631d6e387543ed8f642bc02c578ef4e3b49aca2a29a7df0cb"
 dependencies = [
  "arrayvec",
  "cfg-if",
  "cfg_aliases 0.1.1",
  "js-sys",
  "log",
  "naga",
@@ -6843,21 +6955,21 @@
  "wgpu-core",
  "wgpu-hal",
  "wgpu-types",
 ]
 
 [[package]]
 name = "wgpu-core"
-version = "0.19.0"
+version = "0.19.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6b15e451d4060ada0d99a64df44e4d590213496da7c4f245572d51071e8e30ed"
+checksum = "f9f6b033c2f00ae0bc8ea872c5989777c60bc241aac4e58b24774faa8b391f78"
 dependencies = [
  "arrayvec",
  "bit-vec",
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "cfg_aliases 0.1.1",
  "codespan-reporting",
  "indexmap",
  "log",
  "naga",
  "once_cell",
  "parking_lot",
@@ -6869,38 +6981,39 @@
  "web-sys",
  "wgpu-hal",
  "wgpu-types",
 ]
 
 [[package]]
 name = "wgpu-hal"
-version = "0.19.1"
+version = "0.19.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e3bb47856236bfafc0bc591a925eb036ac19cd987624a447ff353e7a7e7e6f72"
+checksum = "49f972c280505ab52ffe17e94a7413d9d54b58af0114ab226b9fc4999a47082e"
 dependencies = [
  "android_system_properties",
  "arrayvec",
  "ash",
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "block",
  "cfg_aliases 0.1.1",
  "core-graphics-types",
  "glow",
  "glutin_wgl_sys",
  "gpu-alloc",
  "gpu-allocator",
  "gpu-descriptor",
  "hassle-rs",
  "js-sys",
  "khronos-egl",
  "libc",
- "libloading 0.8.1",
+ "libloading 0.8.3",
  "log",
  "metal",
  "naga",
+ "ndk-sys",
  "objc",
  "once_cell",
  "parking_lot",
  "profiling",
  "raw-window-handle 0.6.0",
  "renderdoc-sys",
  "rustc-hash",
@@ -6910,19 +7023,19 @@
  "web-sys",
  "wgpu-types",
  "winapi",
 ]
 
 [[package]]
 name = "wgpu-types"
-version = "0.19.0"
+version = "0.19.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "895fcbeb772bfb049eb80b2d6e47f6c9af235284e9703c96fc0218a42ffd5af2"
+checksum = "b671ff9fb03f78b46ff176494ee1ebe7d603393f42664be55b64dc8d53969805"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "js-sys",
  "web-sys",
 ]
 
 [[package]]
 name = "widestring"
 version = "1.0.2"
@@ -6951,23 +7064,14 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f29e6f9198ba0d26b4c9f07dbe6f9ed633e1f3d5b8b414090084349e46a52596"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
-name = "winapi-wsapoll"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44c17110f57155602a80dca10be03852116403c9ff3cd25b079d666f2aa3df6e"
-dependencies = [
- "winapi",
-]
-
-[[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
 name = "windows"
@@ -6983,24 +7087,24 @@
 [[package]]
 name = "windows"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e48a53791691ab099e5e2ad123536d0fff50652600abaf43bbf952894110d0be"
 dependencies = [
  "windows-core",
- "windows-targets 0.52.0",
+ "windows-targets 0.52.4",
 ]
 
 [[package]]
 name = "windows-core"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets 0.52.0",
+ "windows-targets 0.52.4",
 ]
 
 [[package]]
 name = "windows-implement"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5e2ee588991b9e7e6c8338edf3333fbe4da35dc72092643958ebb43f0ab2c49c"
@@ -7041,15 +7145,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.0",
+ "windows-targets 0.52.4",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8e5180c00cd44c9b1c88adb3693291f1cd93605ded80c250a75d472756b4d071"
@@ -7076,25 +7180,25 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a18201040b24831fbb9e4eb208f8892e1f50a37feb53cc7ff887feb8f50e7cd"
+checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.0",
- "windows_aarch64_msvc 0.52.0",
- "windows_i686_gnu 0.52.0",
- "windows_i686_msvc 0.52.0",
- "windows_x86_64_gnu 0.52.0",
- "windows_x86_64_gnullvm 0.52.0",
- "windows_x86_64_msvc 0.52.0",
+ "windows_aarch64_gnullvm 0.52.4",
+ "windows_aarch64_msvc 0.52.4",
+ "windows_i686_gnu 0.52.4",
+ "windows_i686_msvc 0.52.4",
+ "windows_x86_64_gnu 0.52.4",
+ "windows_x86_64_gnullvm 0.52.4",
+ "windows_x86_64_msvc 0.52.4",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "597a5118570b68bc08d8d59125332c54f1ba9d9adeedeef5b99b02ba2b0698f8"
@@ -7103,17 +7207,17 @@
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb7764e35d4db8a7921e09562a0304bf2f93e0a51bfccee0bd0bb0b666b015ea"
+checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e08e8864a60f06ef0d0ff4ba04124db8b0fb3be5776a5cd47641e942e58c4d43"
 
@@ -7121,17 +7225,17 @@
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bbaa0368d4f1d2aaefc55b6fcfee13f41544ddf36801e793edbbfd7d7df075ef"
+checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c61d927d8da41da96a81f029489353e68739737d3beca43145c8afec9a31a84f"
 
@@ -7139,17 +7243,17 @@
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a28637cb1fa3560a16915793afb20081aba2c92ee8af57b4d5f28e4b3e7df313"
+checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44d840b6ec649f480a41c8d80f9c65108b92d89345dd94027bfe06ac444d1060"
 
@@ -7157,17 +7261,17 @@
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffe5e8e31046ce6230cc7215707b816e339ff4d4d67c65dffa206fd0f7aa7b9a"
+checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8de912b8b8feb55c064867cf047dda097f92d51efad5b491dfb98f6bbb70cb36"
 
@@ -7175,17 +7279,17 @@
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d6fa32db2bc4a2f5abeacf2b69f7992cd09dca97498da74a151a3132c26befd"
+checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "26d41b46a36d453748aedef1486d5c7a85db22e56aff34643984ea85514e94a3"
 
@@ -7193,17 +7297,17 @@
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1a657e1e9d3f514745a572a6846d3c7aa7dbe1658c056ed9c3344c4109a6949e"
+checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.42.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9aec5da331524158c6d1a4ac0ab1541149c0b9505fde06423b02f5ef0106b9f0"
 
@@ -7211,70 +7315,70 @@
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.0"
+version = "0.52.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dff9641d1cd4be8d1a070daf9e3773c5f67e78b4d9d42263020c057706765c04"
+checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
 
 [[package]]
 name = "winit"
-version = "0.29.10"
+version = "0.29.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c824f11941eeae66ec71111cc2674373c772f482b58939bb4066b642aa2ffcf"
+checksum = "0d59ad965a635657faf09c8f062badd885748428933dad8e8bdd64064d92e5ca"
 dependencies = [
  "ahash",
  "android-activity",
  "atomic-waker",
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "bytemuck",
  "calloop",
  "cfg_aliases 0.1.1",
  "core-foundation",
- "core-graphics 0.23.1",
+ "core-graphics",
  "cursor-icon",
  "icrate",
  "js-sys",
  "libc",
  "log",
- "memmap2 0.9.4",
+ "memmap2",
  "ndk",
  "ndk-sys",
  "objc2 0.4.1",
  "once_cell",
  "orbclient",
  "percent-encoding",
  "raw-window-handle 0.6.0",
  "redox_syscall 0.3.5",
- "rustix 0.38.30",
+ "rustix 0.38.32",
  "smithay-client-toolkit",
  "smol_str",
  "unicode-segmentation",
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "wayland-backend",
  "wayland-client",
  "wayland-protocols",
  "wayland-protocols-plasma",
  "web-sys",
  "web-time",
  "windows-sys 0.48.0",
  "x11-dl",
- "x11rb 0.13.0",
+ "x11rb",
  "xkbcommon-dl",
 ]
 
 [[package]]
 name = "winnow"
-version = "0.5.35"
+version = "0.5.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1931d78a9c73861da0134f453bb1f790ce49b2e30eba8410b4b79bac72b46a2d"
+checksum = "f593a95398737aeed53e489c785df13f3618e41dbcd6718c6addbf1395aa6876"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winnow"
 version = "0.6.5"
@@ -7293,47 +7397,25 @@
  "libc",
  "once_cell",
  "pkg-config",
 ]
 
 [[package]]
 name = "x11rb"
-version = "0.12.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1641b26d4dec61337c35a1b1aaf9e3cba8f46f0b43636c609ab0291a648040a"
-dependencies = [
- "gethostname 0.3.0",
- "nix",
- "winapi",
- "winapi-wsapoll",
- "x11rb-protocol 0.12.0",
-]
-
-[[package]]
-name = "x11rb"
 version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f8f25ead8c7e4cba123243a6367da5d3990e0d3affa708ea19dce96356bd9f1a"
 dependencies = [
  "as-raw-xcb-connection",
- "gethostname 0.4.3",
+ "gethostname",
  "libc",
- "libloading 0.8.1",
+ "libloading 0.8.3",
  "once_cell",
- "rustix 0.38.30",
- "x11rb-protocol 0.13.0",
-]
-
-[[package]]
-name = "x11rb-protocol"
-version = "0.12.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "82d6c3f9a0fb6701fab8f6cea9b0c0bd5d6876f1f89f7fada07e558077c344bc"
-dependencies = [
- "nix",
+ "rustix 0.38.32",
+ "x11rb-protocol",
 ]
 
 [[package]]
 name = "x11rb-protocol"
 version = "0.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e63e71c4b8bd9ffec2c963173a4dc4cbde9ee96961d4fcb4429db9929b606c34"
@@ -7342,29 +7424,29 @@
 name = "xcursor"
 version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6a0ccd7b4a5345edfcd0c3535718a4e9ff7798ffc536bb5b5a0e26ff84732911"
 
 [[package]]
 name = "xdg-home"
-version = "1.0.0"
+version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2769203cd13a0c6015d515be729c526d041e9cf2c0cc478d57faee85f40c6dcd"
+checksum = "21e5a325c3cb8398ad6cf859c1135b25dd29e186679cf2da7581d9679f63b38e"
 dependencies = [
- "nix",
+ "libc",
  "winapi",
 ]
 
 [[package]]
 name = "xkbcommon-dl"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d039de8032a9a8856a6be89cea3e5d12fdd82306ab7c94d74e6deab2460651c5"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "dlib",
  "log",
  "once_cell",
  "xkeysym",
 ]
 
 [[package]]
@@ -7377,26 +7459,26 @@
 name = "xml-rs"
 version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fcb9cbac069e033553e8bb871be2fbdffcab578eb25bd0f7c508cedc6dcd75a"
 
 [[package]]
 name = "xshell"
-version = "0.2.5"
+version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ce2107fe03e558353b4c71ad7626d58ed82efaf56c54134228608893c77023ad"
+checksum = "6db0ab86eae739efd1b054a8d3d16041914030ac4e01cd1dca0cf252fd8b6437"
 dependencies = [
  "xshell-macros",
 ]
 
 [[package]]
 name = "xshell-macros"
-version = "0.2.5"
+version = "0.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7e2c411759b501fb9501aac2b1b2d287a6e93e5bdcf13c25306b23e1b716dd0e"
+checksum = "9d422e8e38ec76e2f06ee439ccc765e9c6a9638b9e7c9f2e8255e4d41e8bd852"
 
 [[package]]
 name = "yoke"
 version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "65e71b2e4f287f467794c671e2b8f8a5f3716b3c829079a1c44740148eff07e4"
 dependencies = [
@@ -7410,23 +7492,23 @@
 name = "yoke-derive"
 version = "0.7.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e6936f0cce458098a201c245a11bef556c6a0181129c7034d10d76d1ec3a2b8"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
  "synstructure",
 ]
 
 [[package]]
 name = "zbus"
-version = "3.14.1"
+version = "3.15.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31de390a2d872e4cd04edd71b425e29853f786dc99317ed72d73d6fcf5ebb948"
+checksum = "675d170b632a6ad49804c8cf2105d7c31eddd3312555cffd4b740e08e97c25e6"
 dependencies = [
  "async-broadcast",
  "async-executor",
  "async-fs 1.6.0",
  "async-io 1.13.0",
  "async-lock 2.8.0",
  "async-process",
@@ -7457,31 +7539,31 @@
  "zbus_macros",
  "zbus_names",
  "zvariant",
 ]
 
 [[package]]
 name = "zbus_macros"
-version = "3.14.1"
+version = "3.15.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "41d1794a946878c0e807f55a397187c11fc7a038ba5d868e7db4f3bd7760bc9d"
+checksum = "7131497b0f887e8061b430c530240063d33bf9455fa34438f388a245da69e0a5"
 dependencies = [
- "proc-macro-crate",
+ "proc-macro-crate 1.3.1",
  "proc-macro2",
  "quote",
  "regex",
  "syn 1.0.109",
  "zvariant_utils",
 ]
 
 [[package]]
 name = "zbus_names"
-version = "2.6.0"
+version = "2.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb80bb776dbda6e23d705cf0123c3b95df99c4ebeaec6c2599d4a5419902b4a9"
+checksum = "437d738d3750bed6ca9b8d423ccc7a8eb284f6b1d6d4e225a0e4e6258d864c8d"
 dependencies = [
  "serde",
  "static_assertions",
  "zvariant",
 ]
 
 [[package]]
@@ -7497,15 +7579,15 @@
 name = "zerocopy-derive"
 version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
 ]
 
 [[package]]
 name = "zerofrom"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "655b0814c5c0b19ade497851070c640773304939a6c0fd5f5fb43da0696d05b7"
@@ -7517,19 +7599,25 @@
 name = "zerofrom-derive"
 version = "0.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e6a647510471d372f2e6c2e6b7219e44d8c574d24fdc11c610a61455782f18c3"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn 2.0.57",
  "synstructure",
 ]
 
 [[package]]
+name = "zeroize"
+version = "1.7.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "525b4ec142c6b68a2d10f01f7bbf6755599ca3f81ea53b8431b7dd348f5fdb2d"
+
+[[package]]
 name = "zip"
 version = "0.6.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "760394e246e4c28189f19d488c058bf16f564016aefac5d32bb1f3b51d5e9261"
 dependencies = [
  "byteorder",
  "crc32fast",
@@ -7558,34 +7646,34 @@
 checksum = "ec866b44a2a1fd6133d363f073ca1b179f438f99e7e5bfb1e33f7181facfe448"
 dependencies = [
  "zune-core",
 ]
 
 [[package]]
 name = "zvariant"
-version = "3.15.0"
+version = "3.15.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44b291bee0d960c53170780af148dca5fa260a63cdd24f1962fa82e03e53338c"
+checksum = "4eef2be88ba09b358d3b58aca6e41cd853631d44787f319a1383ca83424fb2db"
 dependencies = [
  "byteorder",
  "enumflags2",
  "libc",
  "serde",
  "static_assertions",
  "url",
  "zvariant_derive",
 ]
 
 [[package]]
 name = "zvariant_derive"
-version = "3.15.0"
+version = "3.15.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "934d7a7dfc310d6ee06c87ffe88ef4eca7d3e37bb251dece2ef93da8f17d8ecd"
+checksum = "37c24dc0bed72f5f90d1f8bb5b07228cbf63b3c6e9f82d82559d4bae666e7ed9"
 dependencies = [
- "proc-macro-crate",
+ "proc-macro-crate 1.3.1",
  "proc-macro2",
  "quote",
  "syn 1.0.109",
  "zvariant_utils",
 ]
 
 [[package]]
```

### Comparing `kornia_rs-0.1.2/LICENSE` & `kornia_rs-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/Makefile` & `kornia_rs-0.1.3/Makefile`

 * *Files 19% similar despite different names*

```diff
@@ -13,31 +13,31 @@
 .venv:  ## Set up Python virtual environment and install requirements
 	python3 -m venv $(VENV)
 	$(MAKE) requirements
 
 .PHONY: requirements
 requirements: .venv  ## Install/refresh Python project requirements
 	$(VENV_BIN)/python -m pip install --upgrade pip
-	$(VENV_BIN)/python -m pip install -r py-kornia/requirements-dev.txt
+	$(VENV_BIN)/python -m pip install -r kornia-py/requirements-dev.txt
 
 .PHONY: build-python
 build-python: .venv  ## Compile and install Python for development
 	@unset CONDA_PREFIX && source $(VENV_BIN)/activate \
-	&& maturin develop -m py-kornia/Cargo.toml \
+	&& maturin develop -m kornia-py/Cargo.toml \
 
 .PHONY: build-python-release
 build-python-release: .venv  ## Compile and install a faster Python binary with full optimizations
 	@unset CONDA_PREFIX && source $(VENV_BIN)/activate \
-	&& maturin develop -m py-kornia/Cargo.toml --release \
+	&& maturin develop -m kornia-py/Cargo.toml --release \
 
 .PHONY: test-python
 test-python: .venv  ## Run Python tests
 	@unset CONDA_PREFIX && source $(VENV_BIN)/activate \
-	&& maturin develop -m py-kornia/Cargo.toml \
-	&& $(VENV_BIN)/pytest py-kornia/tests
+	&& maturin develop -m kornia-py/Cargo.toml \
+	&& $(VENV_BIN)/pytest kornia-py/tests
 
 .PHONY: clippy
 clippy:  ## Run clippy with all features
 	cargo clippy --workspace --all-targets --all-features --locked -- -D warnings
 
 .PHONY: clippy-default
 clippy-default:  ## Run clippy with default features
@@ -49,13 +49,13 @@
 
 .PHONY: clean
 clean:  ## Clean up caches and build artifacts
 	@rm -rf .venv/
 	@rm -rf target/
 	@rm -f Cargo.lock
 	@cargo clean
-	@$(MAKE) -s -C py-kornia/ $@
+	@$(MAKE) -s -C kornia-py/ $@
 
 .PHONY: help
 help:  ## Display this help screen
 	@echo -e "\033[1mAvailable commands:\033[0m"
 	@grep -E '^[a-z.A-Z_-]+:.*?## .*$$' $(MAKEFILE_LIST) | awk 'BEGIN {FS = ":.*?## "}; {printf "  \033[36m%-22s\033[0m %s\n", $$1, $$2}' | sort
```

### Comparing `kornia_rs-0.1.2/README.md` & `kornia_rs-0.1.3/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -51,31 +51,45 @@
 
 - Read images from AVIF, BMP, DDS, Farbeld, GIF, HDR, ICO, JPEG (libjpeg-turbo), OpenEXR, PNG, PNM, TGA, TIFF, WebP.
 
 ### Image processing
 
 - Convert images to grayscale, resize, crop, rotate, flip, pad, normalize, denormalize, and other image processing operations.
 
+### Video processing
+
+- Capture video frames from a camera.
+
 ## 🛠️ Installation
 
 ### >_ System dependencies
 
-You need to install the following dependencies in your system:
+Dependeing on the features you want to use, you might need to install the following dependencies in your system:
+
+#### turbojpeg
 
 ```bash
 sudo apt-get install nasm
 ```
 
+#### gstreamer
+
+```bash
+sudo apt-get install libgstreamer1.0-dev libgstreamer-plugins-base1.0-dev
+```
+
+** Check the gstreamr installation guide: <https://docs.rs/gstreamer/latest/gstreamer/#installation>
+
 ### 🦀 Rust
 
 Add the following to your `Cargo.toml`:
 
 ```toml
 [dependencies]
-kornia-rs = "0.1.0"
+kornia-rs = { version = "0.1.2", features = ["gstreamer"] }
 ```
 
 Alternatively, you can use the `cargo` command to add the dependency:
 
 ```bash
 cargo add kornia-rs
 ```
@@ -125,14 +139,15 @@
     let _ = rec.log("image", &rerun::Image::try_from(image_viz.data)?);
     let _ = rec.log("gray", &rerun::Image::try_from(gray.data)?);
     let _ = rec.log("gray_resize", &rerun::Image::try_from(gray_resize.data)?);
 
     Ok(())
 }
 ```
+
 ![Screenshot from 2024-03-09 14-31-41](https://github.com/kornia/kornia-rs/assets/5157099/afdc11e6-eb36-4fcc-a6a1-e2240318958d)
 
 ## Python usage
 
 Load an image, that is converted directly to a numpy array to ease the integration with other libraries.
 
 ```python
@@ -240,8 +255,8 @@
 
 ```bash
 make test-python
 ```
 
 ## 💜 Contributing
 
-This is a child project of [Kornia](https://github.com/kornia/kornia). Join the community to get in touch with us, or just sponsor the project: https://opencollective.com/kornia
+This is a child project of [Kornia](https://github.com/kornia/kornia). Join the community to get in touch with us, or just sponsor the project: <https://opencollective.com/kornia>
```

### Comparing `kornia_rs-0.1.2/benches/bench_color.rs` & `kornia_rs-0.1.3/benches/bench_color.rs`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/benches/bench_io.rs` & `kornia_rs-0.1.3/benches/bench_io.rs`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/benches/bench_metrics.rs` & `kornia_rs-0.1.3/benches/bench_metrics.rs`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/benches/bench_resize.rs` & `kornia_rs-0.1.3/benches/bench_resize.rs`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/docker/devel.Dockerfile` & `kornia_rs-0.1.3/docker/devel.Dockerfile`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/docker/release-amd64.Dockerfile` & `kornia_rs-0.1.3/docker/release-amd64.Dockerfile`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/examples/binarize.rs` & `kornia_rs-0.1.3/examples/binarize.rs`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     // convert to grayscale as floating point
     let gray_f32: Image<f32, 1> = kornia_rs::color::gray_from_rgb(&image_f32)?;
 
     // binarize the gray image as floating point
     let gray_bin: Image<f32, 1> = kornia_rs::threshold::threshold_binary(&gray_f32, 0.5, 1.0)?;
 
     // create a Rerun recording stream
-    let rec = rerun::RecordingStreamBuilder::new("Kornia App").connect()?;
+    let rec = rerun::RecordingStreamBuilder::new("Kornia App").spawn()?;
 
-    let _ = rec.log("image", &rerun::Image::try_from(image_f32.data)?);
-    let _ = rec.log("gray", &rerun::Image::try_from(gray_f32.data)?);
-    let _ = rec.log("gray_bin", &rerun::Image::try_from(gray_bin.data)?);
+    rec.log("image", &rerun::Image::try_from(image_f32.data)?)?;
+    rec.log("gray", &rerun::Image::try_from(gray_f32.data)?)?;
+    rec.log("gray_bin", &rerun::Image::try_from(gray_bin.data)?)?;
 
     Ok(())
 }
```

### Comparing `kornia_rs-0.1.2/examples/imgproc.rs` & `kornia_rs-0.1.3/examples/imgproc.rs`

 * *Files 4% similar despite different names*

```diff
@@ -19,16 +19,16 @@
         },
         kornia_rs::resize::InterpolationMode::Bilinear,
     )?;
 
     println!("gray_resize: {:?}", gray_resize.size());
 
     // create a Rerun recording stream
-    let rec = rerun::RecordingStreamBuilder::new("Kornia App").connect()?;
+    let rec = rerun::RecordingStreamBuilder::new("Kornia App").spawn()?;
 
     // log the images
-    let _ = rec.log("image", &rerun::Image::try_from(image_f32.data)?);
-    let _ = rec.log("gray", &rerun::Image::try_from(gray.data)?);
-    let _ = rec.log("gray_resize", &rerun::Image::try_from(gray_resize.data)?);
+    rec.log("image", &rerun::Image::try_from(image_f32.data)?)?;
+    rec.log("gray", &rerun::Image::try_from(gray.data)?)?;
+    rec.log("gray_resize", &rerun::Image::try_from(gray_resize.data)?)?;
 
     Ok(())
 }
```

### Comparing `kornia_rs-0.1.2/examples/metrics.rs` & `kornia_rs-0.1.3/examples/metrics.rs`

 * *Files 11% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     println!("PSNR error: {:?}", psnr);
 
     // or, alternatively, compute the mse using the built-in functions
     let mse_map = image.sub(&image_dirty).powi(2);
     // let mse_ii = mse_map_ii.mean();
 
     // create a Rerun recording stream
-    let rec = rerun::RecordingStreamBuilder::new("Kornia App").connect()?;
+    let rec = rerun::RecordingStreamBuilder::new("Kornia App").spawn()?;
 
     // log the images
-    let _ = rec.log("image", &rerun::Image::try_from(image.data)?);
-    let _ = rec.log("flip", &rerun::Image::try_from(image_dirty.data)?);
-    let _ = rec.log("mse_map", &rerun::Image::try_from(mse_map.data)?);
+    rec.log("image", &rerun::Image::try_from(image.data)?)?;
+    rec.log("flip", &rerun::Image::try_from(image_dirty.data)?)?;
+    rec.log("mse_map", &rerun::Image::try_from(mse_map.data)?)?;
 
     Ok(())
 }
```

### Comparing `kornia_rs-0.1.2/examples/normalize.rs` & `kornia_rs-0.1.3/examples/normalize.rs`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/examples/normalize_ii.rs` & `kornia_rs-0.1.3/examples/normalize_ii.rs`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/src/color.rs` & `kornia_rs-0.1.3/src/color.rs`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/src/distance_transform.rs` & `kornia_rs-0.1.3/src/distance_transform.rs`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/src/flip.rs` & `kornia_rs-0.1.3/src/flip.rs`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/src/image.rs` & `kornia_rs-0.1.3/src/image.rs`

 * *Files 27% similar despite different names*

```diff
@@ -235,14 +235,78 @@
             let xu = U::from(x).expect("Failed to cast image data");
             xu * scale
         });
 
         Ok(Image { data: casted_data })
     }
 
+    /// Get a channel of the image.
+    /// # Arguments
+    ///
+    /// * `channel` - The channel to get.
+    ///
+    /// # Returns
+    ///
+    /// A new image with the given channel.
+    ///
+    /// # Errors
+    ///
+    /// If the channel index is out of bounds, an error is returned.
+    pub fn channel(&self, channel: usize) -> Result<Image<T, 1>>
+    where
+        T: Clone,
+    {
+        if channel >= CHANNELS {
+            return Err(anyhow::anyhow!(
+                "Channel index ({}) out of bounds ({}).",
+                channel,
+                CHANNELS
+            ));
+        }
+
+        let channel_data = self.data.slice(ndarray::s![.., .., channel..channel + 1]);
+
+        Ok(Image {
+            data: channel_data.to_owned(),
+        })
+    }
+
+    /// Split the image into its channels.
+    ///
+    /// # Returns
+    ///
+    /// A vector of images, each containing one channel of the original image.
+    ///
+    /// # Examples
+    ///
+    /// ```
+    /// use kornia_rs::image::{Image, ImageSize};
+    ///
+    /// let image = Image::<f32, 2>::from_size_val(
+    ///   ImageSize {
+    ///    width: 10,
+    ///   height: 20,
+    /// },
+    /// 0.0f32).unwrap();
+    ///
+    /// let channels = image.split_channels().unwrap();
+    /// assert_eq!(channels.len(), 2);
+    /// ```
+    pub fn split_channels(&self) -> Result<Vec<Image<T, 1>>>
+    where
+        T: Clone,
+    {
+        let mut channels = Vec::with_capacity(CHANNELS);
+        for i in 0..CHANNELS {
+            channels.push(self.channel(i)?);
+        }
+
+        Ok(channels)
+    }
+
     // TODO: optimize this
     pub fn mul(&self, scale: T) -> Self
     where
         T: Copy + std::ops::Mul<Output = T>,
     {
         let scaled_data = self.data.map(|&x| x * scale);
         Image { data: scaled_data }
@@ -319,110 +383,222 @@
     }
 
     /// Get the number of channels in the image.
     pub fn num_channels(&self) -> usize {
         CHANNELS
     }
 
-    //pub fn from_file(image_path: &Path) -> Image<u8, 3> {
-    //    match image_path.extension().and_then(|ext| ext.to_str()) {
-    //        Some("jpeg") | Some("jpg") => io::functions::read_image_jpeg(image_path),
-    //        _ => io::functions::read_image_any(image_path),
-    //    }
-    //}
+    /// Get the pixel data of the image as a 4D tensor in NCHW format.
+    ///
+    /// Internally, the image is stored in HWC format, and the function gives
+    /// away ownership of the pixel data.
+    pub fn to_tensor_nchw(self) -> ndarray::Array4<T> {
+        // add batch axis 1xHxWxC
+        let data = self.data.insert_axis(ndarray::Axis(0));
+
+        // permute axes to NHWC -> NCHW
+        data.permuted_axes([0, 3, 1, 2])
+    }
+
+    /// Get the pixel data of the image as a 4D tensor in NHWC format.
+    ///
+    /// Internally, the image is stored in HWC format, and the function gives
+    /// away ownership of the pixel data.
+    pub fn to_tensor_nhwc(self) -> ndarray::Array4<T> {
+        self.data.insert_axis(ndarray::Axis(0))
+    }
+
+    // NOTE: experimental api
+    pub fn set_pixel(&mut self, x: usize, y: usize, ch: usize, val: T) -> Result<()>
+    where
+        T: Copy,
+    {
+        if x >= self.width() || y >= self.height() {
+            return Err(anyhow::anyhow!(
+                "Pixel coordinates ({}, {}) out of bounds ({}, {}).",
+                x,
+                y,
+                self.width(),
+                self.height()
+            ));
+        }
+
+        if ch >= CHANNELS {
+            return Err(anyhow::anyhow!(
+                "Channel index ({}) out of bounds ({}).",
+                ch,
+                CHANNELS
+            ));
+        }
+
+        self.data[[y, x, ch]] = val;
+
+        Ok(())
+    }
+
+    // NOTE: experimental api
+    pub fn get_pixel(&self, x: usize, y: usize, ch: usize) -> Result<T>
+    where
+        T: Copy,
+    {
+        if x >= self.width() || y >= self.height() {
+            return Err(anyhow::anyhow!(
+                "Pixel coordinates ({}, {}) out of bounds ({}, {}).",
+                x,
+                y,
+                self.width(),
+                self.height()
+            ));
+        }
 
-    // TODO: implement from bytes
-    // pub fn from_bytes(bytes: &[u8]) -> Image {
+        if ch >= CHANNELS {
+            return Err(anyhow::anyhow!(
+                "Channel index ({}) out of bounds ({}).",
+                ch,
+                CHANNELS
+            ));
+        }
+
+        Ok(self.data[[y, x, ch]])
+    }
 }
 
 #[cfg(test)]
 mod tests {
-    use crate::image::ImageSize;
+    use crate::image::{Image, ImageSize};
+    use anyhow::Result;
 
     #[test]
     fn image_size() {
-        use crate::image::ImageSize;
         let image_size = ImageSize {
             width: 10,
             height: 20,
         };
         assert_eq!(image_size.width, 10);
         assert_eq!(image_size.height, 20);
     }
 
     #[test]
-    fn image_smoke() {
-        use crate::image::{Image, ImageSize};
+    fn image_smoke() -> Result<()> {
         let image = Image::<u8, 3>::new(
             ImageSize {
                 width: 10,
                 height: 20,
             },
             vec![0u8; 10 * 20 * 3],
-        )
-        .unwrap();
+        )?;
         assert_eq!(image.size().width, 10);
         assert_eq!(image.size().height, 20);
         assert_eq!(image.num_channels(), 3);
+
+        Ok(())
     }
 
     #[test]
-    //fn image_from_file() {
-    //    use crate::image::Image;
-    //    let image_path = std::path::Path::new("tests/data/dog.jpeg");
-    //    let image = Image::<u8, 3>::from_file(image_path);
-    //    assert_eq!(image.size().width, 258);
-    //    assert_eq!(image.size().height, 195);
-    //    assert_eq!(image.num_channels(), 3);
-    //}
-    fn image_from_vec() {
-        use crate::image::Image;
+    fn image_from_vec() -> Result<()> {
         let image: Image<f32, 3> = Image::new(
             ImageSize {
                 height: 3,
                 width: 2,
             },
             vec![0.0; 3 * 2 * 3],
-        )
-        .unwrap();
+        )?;
         assert_eq!(image.size().width, 2);
         assert_eq!(image.size().height, 3);
         assert_eq!(image.num_channels(), 3);
+
+        Ok(())
     }
 
     #[test]
-    fn image_cast() {
-        use crate::image::Image;
+    fn image_cast() -> Result<()> {
         let data = vec![0., 1., 2., 3., 4., 5.];
         let image_f64 = Image::<f64, 3>::new(
             ImageSize {
                 height: 2,
                 width: 1,
             },
             data,
-        )
-        .unwrap();
+        )?;
         assert_eq!(image_f64.data.get((1, 0, 2)).unwrap(), &5.0f64);
 
-        let image_u8 = image_f64.cast::<u8>().unwrap();
+        let image_u8 = image_f64.cast::<u8>()?;
         assert_eq!(image_u8.data.get((1, 0, 2)).unwrap(), &5u8);
 
-        let image_i32: Image<i32, 3> = image_u8.cast().unwrap();
+        let image_i32: Image<i32, 3> = image_u8.cast()?;
         assert_eq!(image_i32.data.get((1, 0, 2)).unwrap(), &5i32);
+
+        Ok(())
     }
 
     #[test]
-    fn image_rgbd() {
-        use crate::image::Image;
+    fn image_rgbd() -> Result<()> {
         let image = Image::<f32, 4>::new(
             ImageSize {
                 height: 2,
                 width: 3,
             },
             vec![0f32; 2 * 3 * 4],
-        )
-        .unwrap();
+        )?;
         assert_eq!(image.size().width, 3);
         assert_eq!(image.size().height, 2);
         assert_eq!(image.num_channels(), 4);
+
+        Ok(())
+    }
+
+    #[test]
+    fn image_channel() -> Result<()> {
+        let image = Image::<f32, 3>::new(
+            ImageSize {
+                height: 2,
+                width: 1,
+            },
+            vec![0., 1., 2., 3., 4., 5.],
+        )?;
+
+        let channel = image.channel(2)?;
+        assert_eq!(channel.data.get((1, 0, 0)).unwrap(), &5.0f32);
+
+        Ok(())
+    }
+
+    #[test]
+    fn image_split_channels() -> Result<()> {
+        let image = Image::<f32, 3>::new(
+            ImageSize {
+                height: 2,
+                width: 1,
+            },
+            vec![0., 1., 2., 3., 4., 5.],
+        )
+        .unwrap();
+        let channels = image.split_channels()?;
+        assert_eq!(channels.len(), 3);
+        assert_eq!(channels[0].data.get((1, 0, 0)).unwrap(), &3.0f32);
+        assert_eq!(channels[1].data.get((1, 0, 0)).unwrap(), &4.0f32);
+        assert_eq!(channels[2].data.get((1, 0, 0)).unwrap(), &5.0f32);
+
+        Ok(())
+    }
+
+    #[test]
+    fn convert_to_tensor() -> Result<()> {
+        let image = Image::<f32, 3>::new(
+            ImageSize {
+                height: 2,
+                width: 1,
+            },
+            vec![0., 1., 2., 3., 4., 5.],
+        )?;
+
+        let tensor_nchw = image.clone().to_tensor_nchw();
+        assert_eq!(tensor_nchw.shape(), &[1, 3, 2, 1]);
+        assert_eq!(tensor_nchw[[0, 2, 1, 0]], 5.0f32);
+
+        let tensor_nhwc = image.to_tensor_nhwc();
+        assert_eq!(tensor_nhwc.shape(), &[1, 2, 1, 3]);
+        assert_eq!(tensor_nhwc[[0, 1, 0, 2]], 5.0f32);
+
+        Ok(())
     }
 }
```

### Comparing `kornia_rs-0.1.2/src/io/functional.rs` & `kornia_rs-0.1.3/src/io/functional.rs`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/src/io/jpeg.rs` & `kornia_rs-0.1.3/src/io/jpeg.rs`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/src/metrics/huber.rs` & `kornia_rs-0.1.3/src/metrics/huber.rs`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/src/metrics/l1.rs` & `kornia_rs-0.1.3/src/metrics/l1.rs`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/src/metrics/mse.rs` & `kornia_rs-0.1.3/src/metrics/mse.rs`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/src/normalize.rs` & `kornia_rs-0.1.3/src/normalize.rs`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/src/resize.rs` & `kornia_rs-0.1.3/src/resize.rs`

 * *Files 10% similar despite different names*

```diff
@@ -35,73 +35,93 @@
     // to create the meshgrid of x and y coordinates of shape (height, width)
     let xx = x.broadcast((ny, nx)).unwrap().to_owned();
     let yy = y.broadcast((nx, ny)).unwrap().t().to_owned();
 
     (xx, yy)
 }
 
+// Send and Sync is required for ndarray::Zip::par_for_each
+pub trait ImageDtype: Copy + Default + Into<f32> + Send + Sync {
+    fn from_f32(x: f32) -> Self;
+}
+
+impl ImageDtype for f32 {
+    fn from_f32(x: f32) -> Self {
+        x
+    }
+}
+
+impl ImageDtype for u8 {
+    fn from_f32(x: f32) -> Self {
+        x.round().clamp(0.0, 255.0) as u8
+    }
+}
+
 /// Kernel for bilinear interpolation
 ///
 /// # Arguments
 ///
 /// * `image` - The input image container.
 /// * `u` - The x coordinate of the pixel to interpolate.
 /// * `v` - The y coordinate of the pixel to interpolate.
 /// * `c` - The channel of the pixel to interpolate.
 ///
 /// # Returns
 ///
 /// The interpolated pixel value.
 // TODO: add support for other data types. Maybe use a trait? or template?
-fn bilinear_interpolation(image: &Array3<f32>, u: f32, v: f32, c: usize) -> f32 {
+fn bilinear_interpolation<T: ImageDtype>(image: &Array3<T>, u: f32, v: f32, c: usize) -> T {
     let (height, width, _) = image.dim();
+
     let iu = u.trunc() as usize;
     let iv = v.trunc() as usize;
 
     let frac_u = u.fract();
     let frac_v = v.fract();
-    let val00 = image[[iv, iu, c]];
-    let val01 = if iu + 1 < width {
-        image[[iv, iu + 1, c]]
+    let val00: f32 = image[[iv, iu, c]].into();
+    let val01: f32 = if iu + 1 < width {
+        image[[iv, iu + 1, c]].into()
     } else {
         val00
     };
-    let val10 = if iv + 1 < height {
-        image[[iv + 1, iu, c]]
+    let val10: f32 = if iv + 1 < height {
+        image[[iv + 1, iu, c]].into()
     } else {
         val00
     };
-    let val11 = if iu + 1 < width && iv + 1 < height {
-        image[[iv + 1, iu + 1, c]]
+    let val11: f32 = if iu + 1 < width && iv + 1 < height {
+        image[[iv + 1, iu + 1, c]].into()
     } else {
         val00
     };
 
     let frac_uu = 1. - frac_u;
     let frac_vv = 1. - frac_v;
 
-    val00 * frac_uu * frac_vv
-        + val01 * frac_u * frac_vv
-        + val10 * frac_uu * frac_v
-        + val11 * frac_u * frac_v
+    T::from_f32(
+        val00 * frac_uu * frac_vv
+            + val01 * frac_u * frac_vv
+            + val10 * frac_uu * frac_v
+            + val11 * frac_u * frac_v,
+    )
 }
 
 /// Kernel for nearest neighbor interpolation
 ///
 /// # Arguments
 ///
 /// * `image` - The input image container.
 /// * `u` - The x coordinate of the pixel to interpolate.
 /// * `v` - The y coordinate of the pixel to interpolate.
 /// * `c` - The channel of the pixel to interpolate.
 ///
 /// # Returns
 ///
 /// The interpolated pixel value.
-fn nearest_neighbor_interpolation(image: &Array3<f32>, u: f32, v: f32, c: usize) -> f32 {
+fn nearest_neighbor_interpolation<T: ImageDtype>(image: &Array3<T>, u: f32, v: f32, c: usize) -> T {
     let (height, width, _) = image.dim();
 
     let iu = u.round() as usize;
     let iv = v.round() as usize;
 
     let iu = iu.clamp(0, width - 1);
     let iv = iv.clamp(0, height - 1);
@@ -112,14 +132,27 @@
 /// Interpolation mode for the resize operation
 #[derive(Debug, Clone, Copy, PartialEq)]
 pub enum InterpolationMode {
     Bilinear,
     Nearest,
 }
 
+pub(crate) fn interpolate_pixel<T: ImageDtype>(
+    image: &Array3<T>,
+    u: f32,
+    v: f32,
+    c: usize,
+    interpolation: InterpolationMode,
+) -> T {
+    match interpolation {
+        InterpolationMode::Bilinear => bilinear_interpolation(image, u, v, c),
+        InterpolationMode::Nearest => nearest_neighbor_interpolation(image, u, v, c),
+    }
+}
+
 /// Resize an image to a new size.
 ///
 /// The function resizes an image to a new size using the specified interpolation mode.
 /// It supports any number of channels and data types.
 ///
 /// # Arguments
 ///
@@ -152,21 +185,21 @@
 ///     kornia_rs::resize::InterpolationMode::Nearest,
 /// )
 /// .unwrap();
 /// assert_eq!(image_resized.num_channels(), 3);
 /// assert_eq!(image_resized.size().width, 2);
 /// assert_eq!(image_resized.size().height, 3);
 /// ```
-pub fn resize_native<const CHANNELS: usize>(
-    image: &Image<f32, CHANNELS>,
+pub fn resize_native<T: ImageDtype, const CHANNELS: usize>(
+    image: &Image<T, CHANNELS>,
     new_size: ImageSize,
     interpolation: InterpolationMode,
-) -> Result<Image<f32, CHANNELS>> {
+) -> Result<Image<T, CHANNELS>> {
     // create the output image
-    let mut output = Image::from_size_val(new_size, 0.0)?;
+    let mut output = Image::from_size_val(new_size, T::default())?;
 
     // create a grid of x and y coordinates for the output image
     // and interpolate the values from the input image.
     let x = ndarray::Array::linspace(0., (image.width() - 1) as f32, new_size.width)
         .insert_axis(ndarray::Axis(0));
     let y = ndarray::Array::linspace(0., (image.height() - 1) as f32, new_size.height)
         .insert_axis(ndarray::Axis(0));
@@ -183,18 +216,16 @@
     ndarray::Zip::from(xy.rows())
         .and(output.data.rows_mut())
         .par_for_each(|uv, mut out| {
             assert_eq!(uv.len(), 2);
             let (u, v) = (uv[0], uv[1]);
 
             // compute the pixel values for each channel
-            let pixels = (0..image.num_channels()).map(|k| match interpolation {
-                InterpolationMode::Bilinear => bilinear_interpolation(&image.data, u, v, k),
-                InterpolationMode::Nearest => nearest_neighbor_interpolation(&image.data, u, v, k),
-            });
+            let pixels = (0..image.num_channels())
+                .map(|k| interpolate_pixel(&image.data, u, v, k, interpolation));
 
             // write the pixel values to the output image
             for (k, pixel) in pixels.enumerate() {
                 out[k] = pixel;
             }
         });
 
@@ -246,27 +277,39 @@
 ///
 /// The function returns an error if the image cannot be resized.
 pub fn resize_fast(
     image: &Image<u8, 3>,
     new_size: ImageSize,
     interpolation: InterpolationMode,
 ) -> Result<Image<u8, 3>> {
-    let src_width = NonZeroU32::new(image.width() as u32).unwrap();
-    let src_height = NonZeroU32::new(image.height() as u32).unwrap();
+    let src_width = NonZeroU32::new(image.width() as u32).ok_or(anyhow::anyhow!(
+        "The width of the input image must be greater than zero."
+    ))?;
+    let src_height = NonZeroU32::new(image.height() as u32).ok_or(anyhow::anyhow!(
+        "The height of the input image must be greater than zero."
+    ))?;
+
+    // get the image data as a contiguous slice
+    let image_data = image.data.as_slice().ok_or(anyhow::anyhow!(
+        "The image data must be contiguous and not empty."
+    ))?;
 
-    // TODO: pass as slice
     let src_image = fr::Image::from_vec_u8(
         src_width,
         src_height,
-        image.data.as_slice().unwrap().to_vec(),
+        image_data.to_vec(),
         fr::PixelType::U8x3,
     )?;
 
-    let dst_width = NonZeroU32::new(new_size.width as u32).unwrap();
-    let dst_height = NonZeroU32::new(new_size.height as u32).unwrap();
+    let dst_width = NonZeroU32::new(new_size.width as u32).ok_or(anyhow::anyhow!(
+        "The width of the output image must be greater than zero."
+    ))?;
+    let dst_height = NonZeroU32::new(new_size.height as u32).ok_or(anyhow::anyhow!(
+        "The height of the output image must be greater than zero."
+    ))?;
 
     let mut dst_image = fr::Image::new(dst_width, dst_height, src_image.pixel_type());
     let mut dst_view = dst_image.view_mut();
 
     let mut resizer = {
         match interpolation {
             InterpolationMode::Bilinear => {
@@ -279,63 +322,63 @@
 
     // TODO: create a new image from the buffer directly from a slice
     Image::new(new_size, dst_image.buffer().to_vec())
 }
 
 #[cfg(test)]
 mod tests {
+    use anyhow::Result;
 
     #[test]
-    fn resize_smoke_ch3() {
+    fn resize_smoke_ch3() -> Result<()> {
         use crate::image::{Image, ImageSize};
         let image = Image::<_, 3>::new(
             ImageSize {
                 width: 4,
                 height: 5,
             },
             vec![0f32; 4 * 5 * 3],
-        )
-        .unwrap();
+        )?;
         let image_resized = super::resize_native(
             &image,
             ImageSize {
                 width: 2,
                 height: 3,
             },
             super::InterpolationMode::Bilinear,
-        )
-        .unwrap();
+        )?;
+
         assert_eq!(image_resized.num_channels(), 3);
         assert_eq!(image_resized.size().width, 2);
         assert_eq!(image_resized.size().height, 3);
+        Ok(())
     }
 
     #[test]
-    fn resize_smoke_ch1() {
+    fn resize_smoke_ch1() -> Result<()> {
         use crate::image::{Image, ImageSize};
         let image = Image::<_, 1>::new(
             ImageSize {
                 width: 4,
                 height: 5,
             },
-            vec![0f32; 4 * 5],
-        )
-        .unwrap();
+            vec![0; 4 * 5],
+        )?;
         let image_resized = super::resize_native(
             &image,
             ImageSize {
                 width: 2,
                 height: 3,
             },
             super::InterpolationMode::Nearest,
-        )
-        .unwrap();
+        )?;
         assert_eq!(image_resized.num_channels(), 1);
         assert_eq!(image_resized.size().width, 2);
         assert_eq!(image_resized.size().height, 3);
+        Ok(())
     }
 
     #[test]
     fn meshgrid() {
         let x = ndarray::Array::linspace(0., 4., 5).insert_axis(ndarray::Axis(0));
         let y = ndarray::Array::linspace(0., 3., 4).insert_axis(ndarray::Axis(0));
         let (xx, yy) = super::meshgrid(&x, &y);
@@ -344,31 +387,30 @@
         assert_eq!(xx[[0, 0]], 0.);
         assert_eq!(xx[[0, 4]], 4.);
         assert_eq!(yy[[0, 0]], 0.);
         assert_eq!(yy[[3, 0]], 3.);
     }
 
     #[test]
-    fn resize_fast() {
+    fn resize_fast() -> Result<()> {
         use crate::image::{Image, ImageSize};
         let image = Image::<_, 3>::new(
             ImageSize {
                 width: 4,
                 height: 5,
             },
             vec![0u8; 4 * 5 * 3],
-        )
-        .unwrap();
+        )?;
         let image_resized = super::resize_fast(
             &image,
             ImageSize {
                 width: 2,
                 height: 3,
             },
             super::InterpolationMode::Nearest,
-        )
-        .unwrap();
+        )?;
         assert_eq!(image_resized.num_channels(), 3);
         assert_eq!(image_resized.size().width, 2);
         assert_eq!(image_resized.size().height, 3);
+        Ok(())
     }
 }
```

### Comparing `kornia_rs-0.1.2/src/tensor.rs` & `kornia_rs-0.1.3/src/tensor.rs`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/src/threshold.rs` & `kornia_rs-0.1.3/src/threshold.rs`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/tests/data/dog.jpeg` & `kornia_rs-0.1.3/tests/data/dog.jpeg`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/tests/data/image.jpeg` & `kornia_rs-0.1.3/tests/data/image.jpeg`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/py-kornia/.gitignore` & `kornia_rs-0.1.3/kornia-py/.gitignore`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/py-kornia/LICENSE` & `kornia_rs-0.1.3/kornia-py/LICENSE`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/py-kornia/README.md` & `kornia_rs-0.1.3/kornia-py/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -51,31 +51,45 @@
 
 - Read images from AVIF, BMP, DDS, Farbeld, GIF, HDR, ICO, JPEG (libjpeg-turbo), OpenEXR, PNG, PNM, TGA, TIFF, WebP.
 
 ### Image processing
 
 - Convert images to grayscale, resize, crop, rotate, flip, pad, normalize, denormalize, and other image processing operations.
 
+### Video processing
+
+- Capture video frames from a camera.
+
 ## 🛠️ Installation
 
 ### >_ System dependencies
 
-You need to install the following dependencies in your system:
+Dependeing on the features you want to use, you might need to install the following dependencies in your system:
+
+#### turbojpeg
 
 ```bash
 sudo apt-get install nasm
 ```
 
+#### gstreamer
+
+```bash
+sudo apt-get install libgstreamer1.0-dev libgstreamer-plugins-base1.0-dev
+```
+
+** Check the gstreamr installation guide: <https://docs.rs/gstreamer/latest/gstreamer/#installation>
+
 ### 🦀 Rust
 
 Add the following to your `Cargo.toml`:
 
 ```toml
 [dependencies]
-kornia-rs = "0.1.0"
+kornia-rs = { version = "0.1.2", features = ["gstreamer"] }
 ```
 
 Alternatively, you can use the `cargo` command to add the dependency:
 
 ```bash
 cargo add kornia-rs
 ```
@@ -125,14 +139,15 @@
     let _ = rec.log("image", &rerun::Image::try_from(image_viz.data)?);
     let _ = rec.log("gray", &rerun::Image::try_from(gray.data)?);
     let _ = rec.log("gray_resize", &rerun::Image::try_from(gray_resize.data)?);
 
     Ok(())
 }
 ```
+
 ![Screenshot from 2024-03-09 14-31-41](https://github.com/kornia/kornia-rs/assets/5157099/afdc11e6-eb36-4fcc-a6a1-e2240318958d)
 
 ## Python usage
 
 Load an image, that is converted directly to a numpy array to ease the integration with other libraries.
 
 ```python
@@ -240,8 +255,8 @@
 
 ```bash
 make test-python
 ```
 
 ## 💜 Contributing
 
-This is a child project of [Kornia](https://github.com/kornia/kornia). Join the community to get in touch with us, or just sponsor the project: https://opencollective.com/kornia
+This is a child project of [Kornia](https://github.com/kornia/kornia). Join the community to get in touch with us, or just sponsor the project: <https://opencollective.com/kornia>
```

### Comparing `kornia_rs-0.1.2/py-kornia/benchmark/bench_io.py` & `kornia_rs-0.1.3/kornia-py/benchmark/bench_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 def read_image_pillow(image_path: str) -> None:
     return np.array(Image.open(image_path))
 
 
 def read_image_kornia(image_path: str) -> None:
     return kornia_rs.read_image_jpeg(image_path)
 
+
 def read_image_tensorflow(image_path: str) -> None:
     return tf.keras.utils.load_img(image_path)
 
 
 tests = [
     {
         "name": "OpenCV",
```

### Comparing `kornia_rs-0.1.2/py-kornia/benchmark/bench_resize.py` & `kornia_rs-0.1.3/kornia-py/benchmark/bench_resize.py`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/py-kornia/src/dlpack.rs` & `kornia_rs-0.1.3/kornia-py/src/dlpack.rs`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/py-kornia/src/image.rs` & `kornia_rs-0.1.3/kornia-py/src/image.rs`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 use pyo3::prelude::*;
 
 // type alias for a 3D numpy array of u8
 pub type PyImage = Py<PyArray3<u8>>;
 
 /// Trait to convert an image to a PyImage (3D numpy array of u8)
 pub trait ToPyImage {
-    fn to_pyimage(&self) -> PyImage;
+    fn to_pyimage(self) -> PyImage;
 }
 
 impl<const CHANNELS: usize> ToPyImage for kornia_rs::image::Image<u8, CHANNELS> {
-    fn to_pyimage(&self) -> PyImage {
+    fn to_pyimage(self) -> PyImage {
         Python::with_gil(|py| self.data.to_pyarray(py).to_owned())
     }
 }
 
 /// Trait to convert a PyImage (3D numpy array of u8) to an image
 pub trait FromPyImage<const CHANNELS: usize> {
     fn from_pyimage(image: PyImage) -> Result<Image<u8, CHANNELS>>;
```

### Comparing `kornia_rs-0.1.2/py-kornia/src/io/functional.rs` & `kornia_rs-0.1.3/kornia-py/src/io/functional.rs`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/py-kornia/src/io/jpeg.rs` & `kornia_rs-0.1.3/kornia-py/src/io/jpeg.rs`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/py-kornia/src/lib.rs` & `kornia_rs-0.1.3/kornia-py/src/lib.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+mod histogram;
 mod image;
 mod io;
 mod resize;
+mod warp;
 
 use crate::image::PyImageSize;
 use crate::io::functional::{read_image_any, read_image_jpeg, write_image_jpeg};
 use crate::io::jpeg::{PyImageDecoder, PyImageEncoder};
 use pyo3::prelude::*;
 
 pub fn get_version() -> String {
@@ -20,12 +22,14 @@
 #[pymodule]
 pub fn kornia_rs(_py: Python, m: &PyModule) -> PyResult<()> {
     m.add("__version__", get_version())?;
     m.add_function(wrap_pyfunction!(read_image_jpeg, m)?)?;
     m.add_function(wrap_pyfunction!(write_image_jpeg, m)?)?;
     m.add_function(wrap_pyfunction!(read_image_any, m)?)?;
     m.add_function(wrap_pyfunction!(resize::resize, m)?)?;
+    m.add_function(wrap_pyfunction!(warp::warp_affine, m)?)?;
+    m.add_function(wrap_pyfunction!(histogram::compute_histogram, m)?)?;
     m.add_class::<PyImageSize>()?;
     m.add_class::<PyImageDecoder>()?;
     m.add_class::<PyImageEncoder>()?;
     Ok(())
 }
```

### Comparing `kornia_rs-0.1.2/py-kornia/src/resize.rs` & `kornia_rs-0.1.3/kornia-py/src/resize.rs`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/py-kornia/tests/test_io.py` & `kornia_rs-0.1.3/kornia-py/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/py-kornia/tests/test_resize.py` & `kornia_rs-0.1.3/kornia-py/tests/test_resize.py`

 * *Files identical despite different names*

### Comparing `kornia_rs-0.1.2/py-kornia/Cargo.lock` & `kornia_rs-0.1.3/kornia-py/Cargo.lock`

 * *Files 14% similar despite different names*

```diff
@@ -12,23 +12,17 @@
 name = "aligned-vec"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4aa90d7ce82d4be67b64039a3d588d38dbcc6736577de4a847025ce5b0c468d1"
 
 [[package]]
 name = "anyhow"
-version = "1.0.80"
+version = "1.0.81"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5ad32ce52e4161730f7098c077cd2ed6229b5804ccf99e5366be1ab72a98b4e1"
-
-[[package]]
-name = "arbitrary"
-version = "0.4.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "db55d72333851e17d572bec876e390cd3b11eb1ef53ae821dd9f3b653d2b4569"
+checksum = "0952808a6c2afd1aa8947271f3a60f1a6763c7b912d210184c5149b5cf147247"
 
 [[package]]
 name = "arbitrary"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7d5a26814d8dcb93b0e5a0ff3c6d80a8843bafb21b39e8e18a6f05471870e110"
 
@@ -36,44 +30,40 @@
 name = "arg_enum_proc_macro"
 version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0ae92a5119aa49cdbcf6b9f893fe4e1d98b04ccbf82ee0584ad948a44a734dea"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn",
 ]
 
 [[package]]
 name = "arrayvec"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
-dependencies = [
- "serde",
-]
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "av1-grain"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6678909d8c5d46a42abcf571271e15fdbc0a225e3646cf23762cd415046c78bf"
 dependencies = [
  "anyhow",
  "arrayvec",
  "log",
  "nom",
  "num-rational",
- "serde",
  "v_frame",
 ]
 
 [[package]]
 name = "avif-serialize"
 version = "0.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -92,74 +82,47 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitstream-io"
-version = "1.10.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e445576659fd04a57b44cbd00aa37aaa815ebefa0aa3cb677a6b5e63d883074f"
-
-[[package]]
-name = "bitstream-io"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "06c9989a51171e2e81038ab168b6ae22886fe9ded214430dbb4f41c28cf176da"
 
 [[package]]
 name = "built"
-version = "0.5.2"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5b9c056b9ed43aee5e064b683aa1ec783e19c6acec7559e3ae931b7490472fbe"
-dependencies = [
- "cargo-lock",
-]
-
-[[package]]
-name = "built"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "38d17f4d6e4dc36d1a02fbedc2753a096848e7c1b0772f7654eab8e2c927dd53"
 
 [[package]]
 name = "bumpalo"
-version = "3.14.0"
+version = "3.15.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f30e7476521f6f8af1a1c4c0b8cc94f0bee37d91763d0ca2665f299b6cd8aec"
+checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
 
 [[package]]
 name = "bytemuck"
-version = "1.14.1"
+version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed2490600f404f2b94c167e31d3ed1d5f3c225a0f3b80230053b3e0b7b962bd9"
+checksum = "5d6d68c57235a3a081186990eca2867354726650f42f7516ca50c28d6281fd15"
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
-name = "cargo-lock"
-version = "8.0.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "031718ddb8f78aa5def78a09e90defe30151d1f6c672f937af4dd916429ed996"
-dependencies = [
- "semver",
- "serde",
- "toml 0.5.11",
- "url",
-]
-
-[[package]]
 name = "cc"
-version = "1.0.83"
+version = "1.0.90"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1174fb0b6ec23863f8b971027804a42614e347eafb0a95bf0b12cdae21fc4d0"
+checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
 dependencies = [
  "jobserver",
  "libc",
 ]
 
 [[package]]
 name = "cfg-expr"
@@ -190,17 +153,17 @@
 name = "color_quant"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3d7b894f5411737b7867f4827955924d7c254fc9f4d91a6aad6b097804b1018b"
 
 [[package]]
 name = "crc32fast"
-version = "1.3.2"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
+checksum = "b3855a8a784b474f333699ef2bbca9db2c4a1f6d9088a90a2d25b1eb53111eaa"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "crossbeam-deque"
 version = "0.8.5"
@@ -230,29 +193,29 @@
 name = "crunchy"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
 
 [[package]]
 name = "either"
-version = "1.9.0"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a26ae43d7bcc3b814de94796a5e736d4029efb0ee900c12e2d54c993ad1a1e07"
+checksum = "11157ac094ffbdde99aa67b23417ebdd801842852b500e395a45a9c0aac03e4a"
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "exr"
-version = "1.6.4"
+version = "1.72.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "279d3efcc55e19917fff7ab3ddd6c14afb6a90881a0078465196fe2f99d08c56"
+checksum = "887d93f60543e9a9362ef8a21beedd0a833c5d9610e18c67abe15a5963dcb1a4"
 dependencies = [
  "bit_field",
  "flume",
  "half",
  "lebe",
  "miniz_oxide",
  "rayon-core",
@@ -288,74 +251,47 @@
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
 name = "flume"
-version = "0.10.14"
+version = "0.11.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1657b4441c3403d9f7b3409e47575237dac27b1b5726df654a6ecbf92f0f7577"
+checksum = "55ac459de2512911e4b674ce33cf20befaba382d05b62b008afc1c8b57cbf181"
 dependencies = [
- "futures-core",
- "futures-sink",
- "nanorand",
- "pin-project",
  "spin",
 ]
 
 [[package]]
-name = "form_urlencoded"
-version = "1.2.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e13624c2627564efccf4934284bdd98cbaa14e79b0b5a141218e507b3a823456"
-dependencies = [
- "percent-encoding",
-]
-
-[[package]]
-name = "futures-core"
-version = "0.3.30"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dfc6580bb841c5a68e9ef15c77ccc837b40a7504914d52e47b8b0e9bbda25a1d"
-
-[[package]]
-name = "futures-sink"
-version = "0.3.30"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
-
-[[package]]
 name = "getrandom"
 version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
 dependencies = [
  "cfg-if",
- "js-sys",
  "libc",
  "wasi",
- "wasm-bindgen",
 ]
 
 [[package]]
 name = "gif"
 version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fb2d69b19215e18bb912fa30f7ce15846e301408695e44e0ef719f1da9e19f2"
 dependencies = [
  "color_quant",
  "weezl",
 ]
 
 [[package]]
 name = "half"
-version = "2.3.1"
+version = "2.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bc52e53916c08643f1b56ec082790d1e86a32e58dc5268f897f313fbae7b4872"
+checksum = "b5eceaaeec696539ddaf7b333340f1af35a5aa87ae3e4f3ead0532f72affab2e"
 dependencies = [
  "cfg-if",
  "crunchy",
 ]
 
 [[package]]
 name = "hashbrown"
@@ -366,22 +302,18 @@
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
-name = "idna"
+name = "heck"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "634d9b1461af396cad843f47fdba5597a4f9e6ddd4bfb6ff5d85028c25cb12f6"
-dependencies = [
- "unicode-bidi",
- "unicode-normalization",
-]
+checksum = "2304e00983f87ffb38b55b444b5e3b60a884b5d30c0fca7d82fe33449bbe55ea"
 
 [[package]]
 name = "image"
 version = "0.25.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a9b4f005360d32e9325029b38ba47ebd7a56f3316df09249368939562d518645"
 dependencies = [
@@ -400,62 +332,53 @@
  "tiff",
  "zune-core",
  "zune-jpeg",
 ]
 
 [[package]]
 name = "image-webp"
-version = "0.1.0"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ba6107a25f04af48ceeb4093eebc9b405ee5a1813a0bab5ecf1805d3eabb3337"
+checksum = "7a84a25dcae3ac487bc24ef280f9e20c79c9b1a3e5e32cbed3041d1c514aa87c"
 dependencies = [
  "byteorder",
  "thiserror",
 ]
 
 [[package]]
 name = "imgref"
 version = "1.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44feda355f4159a7c757171a77de25daf6411e217b4cabd03bd6650690468126"
 
 [[package]]
 name = "indexmap"
-version = "2.2.5"
+version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b0b929d511467233429c45a44ac1dcaa21ba0f5ba11e4879e6ed28ddb4f9df4"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
-version = "2.0.4"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "interpolate_name"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c34819042dc3d3971c46c2190835914dfbe0c3c13f61449b2997f4e9722dfa60"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
-]
-
-[[package]]
-name = "itertools"
-version = "0.10.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
-dependencies = [
- "either",
+ "syn",
 ]
 
 [[package]]
 name = "itertools"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
@@ -475,35 +398,26 @@
 [[package]]
 name = "jpeg-decoder"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f5d4a7da358eff58addd2877a45865158f0d78c911d43a5784ceb7bbf52833b0"
 
 [[package]]
-name = "js-sys"
-version = "0.3.67"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a1d36f1235bc969acba30b7f5990b864423a6068a10f7c90ae8f0112e3a59d1"
-dependencies = [
- "wasm-bindgen",
-]
-
-[[package]]
 name = "kornia-py"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "anyhow",
  "kornia-rs",
  "numpy",
  "pyo3",
 ]
 
 [[package]]
 name = "kornia-rs"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "anyhow",
  "fast_image_resize",
  "image",
  "memmap2",
  "ndarray",
  "num-traits",
@@ -514,35 +428,25 @@
 name = "lebe"
 version = "0.5.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "03087c2bad5e1034e8cace5926dec053fb3790248370865f5117a7d0213354c8"
 
 [[package]]
 name = "libc"
-version = "0.2.152"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "13e3bf6590cbc649f4d1a3eefc9d5d6eb746f5200ffb04e5e142700b8faa56e7"
-
-[[package]]
-name = "libfuzzer-sys"
-version = "0.3.5"
+version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fcf184a4b6b274f82a5df6b357da6055d3e82272327bba281c28bbba6f1664ef"
-dependencies = [
- "arbitrary 0.4.7",
- "cc",
-]
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "libfuzzer-sys"
 version = "0.4.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a96cfd5557eb82f2b83fed4955246c988d331975a002961b07c81584d107e7f7"
 dependencies = [
- "arbitrary 1.3.2",
+ "arbitrary",
  "cc",
  "once_cell",
 ]
 
 [[package]]
 name = "lock_api"
 version = "0.4.11"
@@ -551,17 +455,17 @@
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.20"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "loop9"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0fae87c125b03c1d2c0150c90365d7d6bcc53fb73a9acaef207d2d065860f062"
 dependencies = [
@@ -586,62 +490,53 @@
 dependencies = [
  "cfg-if",
  "rayon",
 ]
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memmap2"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fe751422e4a8caa417e13c3ea66452215d7d63e19e604f4980461212f3ae1322"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
  "simd-adler32",
 ]
 
 [[package]]
-name = "nanorand"
-version = "0.7.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a51313c5820b0b02bd422f4b44776fbf47961755c74ce64afc73bfad10226c3"
-dependencies = [
- "getrandom",
-]
-
-[[package]]
 name = "ndarray"
 version = "0.15.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adb12d4e967ec485a5f71c6311fe28158e9d6f4bc4a447b474184d0f91a8fa32"
 dependencies = [
  "matrixmultiply",
  "num-complex",
@@ -649,17 +544,17 @@
  "num-traits",
  "rawpointer",
  "rayon",
 ]
 
 [[package]]
 name = "new_debug_unreachable"
-version = "1.0.4"
+version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e4a24736216ec316047a1fc4252e27dabb04218aa4a3f37c6e7ddbf1f9782b54"
+checksum = "650eef8c711430f1a879fdd01d4745a7deea475becfb90269c06775983bbf086"
 
 [[package]]
 name = "nom"
 version = "7.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
 dependencies = [
@@ -682,50 +577,38 @@
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-complex"
-version = "0.4.4"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ba157ca0885411de85d6ca030ba7e2a83a28636056c7c699b07c8b6f7383214"
+checksum = "23c6602fda94a57c990fe0df199a035d83576b496aa29f4e634a8ac6004e68a6"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
 name = "num-derive"
-version = "0.3.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "876a53fff98e03a936a674b29568b0e605f06b29372c2489ff4de23f1949743d"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 1.0.109",
-]
-
-[[package]]
-name = "num-derive"
 version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed3955f1a9c7c0c15e092f9c887db08b1fc683305fdf6eb6684f22555355e202"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn",
 ]
 
 [[package]]
 name = "num-integer"
-version = "0.1.45"
+version = "0.1.46"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
+checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
 dependencies = [
- "autocfg",
  "num-traits",
 ]
 
 [[package]]
 name = "num-rational"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -735,17 +618,17 @@
  "num-bigint",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.17"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39e3200413f237f41ab11ad6d161bc7239c84dcb631773ccd7de3dfe4b5c267c"
+checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "numpy"
 version = "0.20.0"
@@ -793,69 +676,49 @@
 [[package]]
 name = "paste"
 version = "1.0.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "de3145af08024dea9fa9914f381a17b8fc6034dfb00f3a84013f7ff43f29ed4c"
 
 [[package]]
-name = "percent-encoding"
-version = "2.3.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
-
-[[package]]
-name = "pin-project"
-version = "1.1.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0302c4a0442c456bd56f841aee5c3bfd17967563f6fadc9ceb9f9c23cf3807e0"
-dependencies = [
- "pin-project-internal",
-]
-
-[[package]]
-name = "pin-project-internal"
-version = "1.1.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "266c042b60c9c76b8d53061e52b2e0d1116abc57cefc8c5cd671619a56ac3690"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn 2.0.48",
-]
-
-[[package]]
 name = "pkg-config"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2900ede94e305130c13ddd391e0ab7cbaeb783945ae07a279c268cb05109c6cb"
+checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
 
 [[package]]
 name = "png"
-version = "0.17.11"
+version = "0.17.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f6c3c3e617595665b8ea2ff95a86066be38fb121ff920a9c0eb282abcd1da5a"
+checksum = "06e4b0d3d1312775e782c86c91a111aa1f910cbb65e1337f9975b5f9a554b5e1"
 dependencies = [
  "bitflags",
  "crc32fast",
  "fdeflate",
  "flate2",
  "miniz_oxide",
 ]
 
 [[package]]
+name = "portable-atomic"
+version = "1.6.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
+
+[[package]]
 name = "ppv-lite86"
 version = "0.2.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b40af805b3121feab8a3c29f04d8ad262fa8e0561883e7653e024ae4479e6de"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.78"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e2422ad645d89c99f8f3e6b88a9fdeca7fabeac836b1002371c4367c8f984aae"
+checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "profiling"
 version = "1.0.15"
@@ -868,76 +731,78 @@
 [[package]]
 name = "profiling-procmacros"
 version = "1.0.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8021cf59c8ec9c432cfc2526ac6b8aa508ecaf29cd415f271b8406c1b851c3fd"
 dependencies = [
  "quote",
- "syn 2.0.48",
+ "syn",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a89dc7a5850d0e983be1ec2a463a171d20990487c3cfcd68b5363f1ee3d6fe0"
+checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07426f0d8fe5a601f26293f300afd1a7b1ed5e78b2a705870c5f30893c5163be"
+checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dbb7dec17e17766b46bca4f1a4215a85006b4c2ecde122076c562dd058da6cf1"
+checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05f738b4e40d50b5711957f142878cfa0f28e054aa0ebdfc3fd137a843f74ed3"
+checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.48",
+ "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.2"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fc910d4851847827daf9d6cdd4a823fbdaab5b8818325c5e97a86da79e8881f"
+checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
- "heck",
+ "heck 0.4.1",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
- "syn 2.0.48",
+ "syn",
 ]
 
 [[package]]
 name = "qoi"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7f6d64c71eb498fe9eae14ce4ec935c555749aef511cca85b5568910d6e48001"
@@ -988,109 +853,73 @@
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
  "getrandom",
 ]
 
 [[package]]
 name = "rav1e"
-version = "0.6.6"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "16c383692a5e7abd9f6d1eddb1a5e0269f859392387883361bb09e5555852ec1"
-dependencies = [
- "arbitrary 0.4.7",
- "arg_enum_proc_macro",
- "arrayvec",
- "av1-grain",
- "bitstream-io 1.10.0",
- "built 0.5.2",
- "cfg-if",
- "interpolate_name",
- "itertools 0.10.5",
- "libc",
- "libfuzzer-sys 0.3.5",
- "log",
- "maybe-rayon",
- "new_debug_unreachable",
- "noop_proc_macro",
- "num-derive 0.3.3",
- "num-traits",
- "once_cell",
- "paste",
- "rand",
- "rand_chacha",
- "rust_hawktracer",
- "rustc_version",
- "simd_helpers",
- "system-deps",
- "thiserror",
- "v_frame",
- "wasm-bindgen",
-]
-
-[[package]]
-name = "rav1e"
 version = "0.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cd87ce80a7665b1cce111f8a16c1f3929f6547ce91ade6addf4ec86a8dda5ce9"
 dependencies = [
- "arbitrary 1.3.2",
+ "arbitrary",
  "arg_enum_proc_macro",
  "arrayvec",
  "av1-grain",
- "bitstream-io 2.2.0",
- "built 0.7.1",
+ "bitstream-io",
+ "built",
  "cfg-if",
  "interpolate_name",
- "itertools 0.12.1",
+ "itertools",
  "libc",
- "libfuzzer-sys 0.4.7",
+ "libfuzzer-sys",
  "log",
  "maybe-rayon",
  "new_debug_unreachable",
  "noop_proc_macro",
- "num-derive 0.4.2",
+ "num-derive",
  "num-traits",
  "once_cell",
  "paste",
  "profiling",
  "rand",
  "rand_chacha",
  "simd_helpers",
  "system-deps",
  "thiserror",
  "v_frame",
+ "wasm-bindgen",
 ]
 
 [[package]]
 name = "ravif"
-version = "0.11.4"
+version = "0.11.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d44feba0b8a381a5efa2c0baf8dace8418904403260233f4a614503b018fc288"
+checksum = "bc13288f5ab39e6d7c9d501759712e6969fcc9734220846fc9ed26cae2cc4234"
 dependencies = [
  "avif-serialize",
  "imgref",
  "loop9",
  "quick-error",
- "rav1e 0.6.6",
- "rav1e 0.7.1",
+ "rav1e",
  "rayon",
  "rgb",
 ]
 
 [[package]]
 name = "rawpointer"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "60a357793950651c4ed0f3f52338f53b2f809f32d83a07f72909fa13e4c6c1e3"
 
 [[package]]
 name = "rayon"
-version = "1.8.1"
+version = "1.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa7237101a77a10773db45d62004a272517633fbcc3df19d96455ede1122e051"
+checksum = "b418a60154510ca1a002a752ca9714984e21e4241e804d32555251faf8b78ffa"
 dependencies = [
  "either",
  "rayon-core",
 ]
 
 [[package]]
 name = "rayon-core"
@@ -1117,66 +946,26 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "05aaa8004b64fd573fc9d002f4e632d51ad4f026c2b5ba95fcb6c2f32c2c47d8"
 dependencies = [
  "bytemuck",
 ]
 
 [[package]]
-name = "rust_hawktracer"
-version = "0.7.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e3480a29b927f66c6e06527be7f49ef4d291a01d694ec1fe85b0de71d6b02ac1"
-dependencies = [
- "rust_hawktracer_normal_macro",
- "rust_hawktracer_proc_macro",
-]
-
-[[package]]
-name = "rust_hawktracer_normal_macro"
-version = "0.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8a570059949e1dcdc6f35228fa389f54c2c84dfe0c94c05022baacd56eacd2e9"
-
-[[package]]
-name = "rust_hawktracer_proc_macro"
-version = "0.4.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cb626abdbed5e93f031baae60d72032f56bc964e11ac2ff65f2ba3ed98d6d3e1"
-
-[[package]]
 name = "rustc-hash"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "08d43f7aa6b08d49f382cde6a7982047c3426db949b1424bc4b7ec9ae12c6ce2"
 
 [[package]]
-name = "rustc_version"
-version = "0.4.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
-dependencies = [
- "semver",
-]
-
-[[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
 
 [[package]]
-name = "semver"
-version = "1.0.22"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
-dependencies = [
- "serde",
-]
-
-[[package]]
 name = "serde"
 version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
 dependencies = [
  "serde_derive",
 ]
@@ -1185,15 +974,15 @@
 name = "serde_derive"
 version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn",
 ]
 
 [[package]]
 name = "serde_spanned"
 version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "eb3622f419d1296904700073ea6cc23ad690adbd66f13ea683df73298736f0c1"
@@ -1214,128 +1003,93 @@
 checksum = "95890f873bec569a0362c235787f3aca6e1e887302ba4840839bcc6459c42da6"
 dependencies = [
  "quote",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "spin"
 version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
 dependencies = [
  "lock_api",
 ]
 
 [[package]]
 name = "syn"
-version = "1.0.109"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
-dependencies = [
- "proc-macro2",
- "quote",
- "unicode-ident",
-]
-
-[[package]]
-name = "syn"
-version = "2.0.48"
+version = "2.0.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f3531638e407dfc0814761abb7c00a5b54992b849452a0646b7f65c9f770f3f"
+checksum = "11a6ae1e52eb25aab8f3fb9fca13be982a373b8f1157ca14b897a825ba4a2d35"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "system-deps"
-version = "6.2.0"
+version = "6.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2a2d580ff6a20c55dfb86be5f9c238f67835d0e81cbdea8bf5680e0897320331"
+checksum = "a3e535eb8dded36d55ec13eddacd30dec501792ff23a0b1682c38601b8cf2349"
 dependencies = [
  "cfg-expr",
- "heck",
+ "heck 0.5.0",
  "pkg-config",
- "toml 0.8.10",
+ "toml",
  "version-compare",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.13"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69758bda2e78f098e4ccb393021a0963bb3442eac05f135c30f61b7370bbafae"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "thiserror"
-version = "1.0.56"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d54378c645627613241d077a3a79db965db602882668f9136ac42af9ecb730ad"
+checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.56"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fa0faa943b50f3db30a20aa7e265dbc66076993efed8463e8de414e5d06d3471"
+checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn",
 ]
 
 [[package]]
 name = "tiff"
 version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ba1310fcea54c6a9a4fd1aad794ecc02c31682f6bfbecdf460bf19533eed1e3e"
 dependencies = [
  "flate2",
  "jpeg-decoder",
  "weezl",
 ]
 
 [[package]]
-name = "tinyvec"
-version = "1.6.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "87cc5ceb3875bb20c2890005a4e226a4651264a5c75edb2421b52861a0a0cb50"
-dependencies = [
- "tinyvec_macros",
-]
-
-[[package]]
-name = "tinyvec_macros"
-version = "0.1.1"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
-
-[[package]]
 name = "toml"
-version = "0.5.11"
+version = "0.8.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f4f7f0dd8d50a853a531c426359045b1998f04219d88799810762cd4ad314234"
-dependencies = [
- "serde",
-]
-
-[[package]]
-name = "toml"
-version = "0.8.10"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9a9aad4a3066010876e8dcf5a8a06e70a558751117a145c6ce2b82c2e2054290"
+checksum = "e9dd1545e8208b4a5af1aa9bbd0b4cf7e9ea08fabc5d0a5c67fcaafa17433aa3"
 dependencies = [
  "serde",
  "serde_spanned",
  "toml_datetime",
  "toml_edit",
 ]
 
@@ -1346,30 +1100,30 @@
 checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
 dependencies = [
  "serde",
 ]
 
 [[package]]
 name = "toml_edit"
-version = "0.22.6"
+version = "0.22.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2c1b5fd4128cc8d3e0cb74d4ed9a9cc7c7284becd4df68f5f940e1ad123606f6"
+checksum = "8e40bb779c5187258fd7aad0eb68cb8706a0a81fa712fbea808ab43c4b8374c4"
 dependencies = [
  "indexmap",
  "serde",
  "serde_spanned",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
 name = "turbojpeg"
-version = "1.0.0"
+version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eb5080f5adaa92c82bf84f825dd092e9692c923ee652f1634835e9a1f372518d"
+checksum = "9af71fa2654444c8dcb711ecbb8f9202778f8421badf71c3d5a118f1570391ed"
 dependencies = [
  "libc",
  "thiserror",
  "turbojpeg-sys",
 ]
 
 [[package]]
@@ -1381,127 +1135,101 @@
  "anyhow",
  "cmake",
  "libc",
  "pkg-config",
 ]
 
 [[package]]
-name = "unicode-bidi"
-version = "0.3.15"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "08f95100a766bf4f8f28f90d77e0a5461bbdb219042e7679bebe79004fed8d75"
-
-[[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
-name = "unicode-normalization"
-version = "0.1.23"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a56d1686db2308d901306f92a263857ef59ea39678a5458e7cb17f01415101f5"
-dependencies = [
- "tinyvec",
-]
-
-[[package]]
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
-name = "url"
-version = "2.5.0"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "31e6302e3bb753d46e83516cae55ae196fc0c309407cf11ab35cc51a4c2a4633"
-dependencies = [
- "form_urlencoded",
- "idna",
- "percent-encoding",
-]
-
-[[package]]
 name = "v_frame"
 version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d6f32aaa24bacd11e488aa9ba66369c7cd514885742c9fe08cfe85884db3e92b"
 dependencies = [
  "aligned-vec",
  "num-traits",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "version-compare"
-version = "0.1.1"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "579a42fc0b8e0c63b76519a339be31bed574929511fa53c1a3acae26eb258f29"
+checksum = "852e951cb7832cb45cb1169900d19760cfa39b82bc0ea9c0e5a14ae88411c98b"
 
 [[package]]
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.90"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1223296a201415c7fad14792dbefaace9bd52b62d33453ade1c5b5f07555406"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.90"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fcdc935b63408d58a32f8cc9738a0bffd8f05cc7c002086c6ef20b7312ad9dcd"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.90"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e4c238561b2d428924c49815533a8b9121c664599558a5d9ec51f8a1740a999"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.90"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bae1abb6806dc1ad9e560ed242107c0f6c84335f1749dd4e8ddb012ebd5e25a7"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.48",
+ "syn",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.90"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4d91413b1c31d7539ba5ef2451af3f0b833a005eb27a631cec32bc0635a8602b"
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
 name = "weezl"
 version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53a85b86a771b1c87058196170769dd264f66c0782acf1ae6cc51bfd64b39082"
```

### Comparing `kornia_rs-0.1.2/pyproject.toml` & `kornia_rs-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -46,8 +46,8 @@
   "numpy==1.23.0",
   "jax[cpu]",
 ]
 
 [tool]
 
 [tool.maturin]
-manifest-path = "py-kornia/Cargo.toml"
+manifest-path = "kornia-py/Cargo.toml"
```

### Comparing `kornia_rs-0.1.2/PKG-INFO` & `kornia_rs-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: kornia_rs
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -86,31 +86,45 @@
 
 - Read images from AVIF, BMP, DDS, Farbeld, GIF, HDR, ICO, JPEG (libjpeg-turbo), OpenEXR, PNG, PNM, TGA, TIFF, WebP.
 
 ### Image processing
 
 - Convert images to grayscale, resize, crop, rotate, flip, pad, normalize, denormalize, and other image processing operations.
 
+### Video processing
+
+- Capture video frames from a camera.
+
 ## 🛠️ Installation
 
 ### >_ System dependencies
 
-You need to install the following dependencies in your system:
+Dependeing on the features you want to use, you might need to install the following dependencies in your system:
+
+#### turbojpeg
 
 ```bash
 sudo apt-get install nasm
 ```
 
+#### gstreamer
+
+```bash
+sudo apt-get install libgstreamer1.0-dev libgstreamer-plugins-base1.0-dev
+```
+
+** Check the gstreamr installation guide: <https://docs.rs/gstreamer/latest/gstreamer/#installation>
+
 ### 🦀 Rust
 
 Add the following to your `Cargo.toml`:
 
 ```toml
 [dependencies]
-kornia-rs = "0.1.0"
+kornia-rs = { version = "0.1.2", features = ["gstreamer"] }
 ```
 
 Alternatively, you can use the `cargo` command to add the dependency:
 
 ```bash
 cargo add kornia-rs
 ```
@@ -160,14 +174,15 @@
     let _ = rec.log("image", &rerun::Image::try_from(image_viz.data)?);
     let _ = rec.log("gray", &rerun::Image::try_from(gray.data)?);
     let _ = rec.log("gray_resize", &rerun::Image::try_from(gray_resize.data)?);
 
     Ok(())
 }
 ```
+
 ![Screenshot from 2024-03-09 14-31-41](https://github.com/kornia/kornia-rs/assets/5157099/afdc11e6-eb36-4fcc-a6a1-e2240318958d)
 
 ## Python usage
 
 Load an image, that is converted directly to a numpy array to ease the integration with other libraries.
 
 ```python
@@ -275,9 +290,9 @@
 
 ```bash
 make test-python
 ```
 
 ## 💜 Contributing
 
-This is a child project of [Kornia](https://github.com/kornia/kornia). Join the community to get in touch with us, or just sponsor the project: https://opencollective.com/kornia
+This is a child project of [Kornia](https://github.com/kornia/kornia). Join the community to get in touch with us, or just sponsor the project: <https://opencollective.com/kornia>
```

