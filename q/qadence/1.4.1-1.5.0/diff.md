# Comparing `tmp/qadence-1.4.1.tar.gz` & `tmp/qadence-1.5.0.tar.gz`

## Comparing `qadence-1.4.1.tar` & `qadence-1.5.0.tar`

### file list

```diff
@@ -1,152 +1,154 @@
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 qadence-1.4.1/.coveragerc
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 qadence-1.4.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 qadence-1.4.1/MANIFEST.in
--rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 qadence-1.4.1/mkdocs.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 qadence-1.4.1/setup.py
--rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 qadence-1.4.1/.github/dependabot.yml
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 qadence-1.4.1/.github/workflows/build_docs.yml
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 qadence-1.4.1/.github/workflows/dependabot.yml
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 qadence-1.4.1/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 qadence-1.4.1/.github/workflows/test_all.yml
--rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 qadence-1.4.1/.github/workflows/test_examples.yml
--rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 qadence-1.4.1/.github/workflows/test_fast.yml
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/__init__.py
--rw-r--r--   0        0        0    15493 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/backend.py
--rw-r--r--   0        0        0     6892 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/circuit.py
--rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/decompose.py
--rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/divergences.py
--rw-r--r--   0        0        0     9287 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/execution.py
--rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/extensions.py
--rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/finitediff.py
--rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/logger.py
--rw-r--r--   0        0        0    17294 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/overlap.py
--rw-r--r--   0        0        0    12334 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/parameters.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/protocols.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/py.typed
--rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/qubit_support.py
--rw-r--r--   0        0        0    10276 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/register.py
--rw-r--r--   0        0        0    11702 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/serialization.py
--rw-r--r--   0        0        0    14341 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/states.py
--rw-r--r--   0        0        0     9699 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/types.py
--rw-r--r--   0        0        0     8829 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/utils.py
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/analog/__init__.py
--rw-r--r--   0        0        0     6435 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/analog/addressing.py
--rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/analog/constants.py
--rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/analog/device.py
--rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/analog/hamiltonian_terms.py
--rw-r--r--   0        0        0     4223 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/analog/parse_analog.py
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/backends/__init__.py
--rw-r--r--   0        0        0     6831 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/backends/adjoint.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/backends/api.py
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/backends/gpsr.py
--rw-r--r--   0        0        0     5038 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/backends/jax_utils.py
--rw-r--r--   0        0        0     6460 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/backends/utils.py
--rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/backends/braket/__init__.py
--rw-r--r--   0        0        0     8730 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/backends/braket/backend.py
--rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/backends/braket/config.py
--rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/backends/braket/convert_ops.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/backends/horqrux/__init__.py
--rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/backends/horqrux/backend.py
--rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/backends/horqrux/config.py
--rw-r--r--   0        0        0     8564 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/backends/horqrux/convert_ops.py
--rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/backends/pulser/__init__.py
--rw-r--r--   0        0        0    13868 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/backends/pulser/backend.py
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/backends/pulser/channels.py
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/backends/pulser/cloud.py
--rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/backends/pulser/config.py
--rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/backends/pulser/convert_ops.py
--rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/backends/pulser/devices.py
--rw-r--r--   0        0        0    11893 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/backends/pulser/pulses.py
--rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/backends/pulser/waveforms.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/backends/pyqtorch/__init__.py
--rw-r--r--   0        0        0     9584 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/backends/pyqtorch/backend.py
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/backends/pyqtorch/config.py
--rw-r--r--   0        0        0    16928 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/backends/pyqtorch/convert_ops.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/blocks/__init__.py
--rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/blocks/abstract.py
--rw-r--r--   0        0        0    10812 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/blocks/analog.py
--rw-r--r--   0        0        0    17415 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/blocks/block_to_tensor.py
--rw-r--r--   0        0        0     8897 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/blocks/composite.py
--rw-r--r--   0        0        0     6513 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/blocks/embedding.py
--rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/blocks/manipulate.py
--rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/blocks/matrix.py
--rw-r--r--   0        0        0    16631 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/blocks/primitive.py
--rw-r--r--   0        0        0    16358 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/blocks/utils.py
--rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/constructors/__init__.py
--rw-r--r--   0        0        0    12170 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/constructors/ansatze.py
--rw-r--r--   0        0        0    11566 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/constructors/feature_maps.py
--rw-r--r--   0        0        0     8860 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/constructors/hamiltonians.py
--rw-r--r--   0        0        0     7001 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/constructors/iia.py
--rw-r--r--   0        0        0     7688 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/constructors/qft.py
--rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/constructors/rydberg_feature_maps.py
--rw-r--r--   0        0        0     8372 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/constructors/rydberg_hea.py
--rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/constructors/utils.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/constructors/daqc/__init__.py
--rw-r--r--   0        0        0     9922 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/constructors/daqc/daqc.py
--rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/constructors/daqc/gen_parser.py
--rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/constructors/daqc/utils.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/draw/__init__.py
--rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/draw/themes.py
--rw-r--r--   0        0        0    12108 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/draw/utils.py
--rw-r--r--   0        0        0    14997 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/draw/vizbackend.py
--rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/draw/assets/dark/measurement.png
--rw-r--r--   0        0        0     7282 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/draw/assets/dark/measurement.svg
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/draw/assets/light/measurement.png
--rw-r--r--   0        0        0     7282 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/draw/assets/light/measurement.svg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/engines/__init__.py
--rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/engines/differentiable_backend.py
--rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/engines/jax/__init__.py
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/engines/jax/differentiable_backend.py
--rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/engines/jax/differentiable_expectation.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/engines/torch/__init__.py
--rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/engines/torch/differentiable_backend.py
--rw-r--r--   0        0        0    15382 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/engines/torch/differentiable_expectation.py
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/exceptions/__init__.py
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/exceptions/exceptions.py
--rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/measurements/__init__.py
--rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/measurements/protocols.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/measurements/samples.py
--rw-r--r--   0        0        0    12550 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/measurements/shadow.py
--rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/measurements/tomography.py
--rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/measurements/utils.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/mitigations/__init__.py
--rw-r--r--   0        0        0     7768 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/mitigations/analog_zne.py
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/mitigations/protocols.py
--rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/mitigations/readout.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/ml_tools/__init__.py
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/ml_tools/config.py
--rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/ml_tools/data.py
--rw-r--r--   0        0        0    11684 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/ml_tools/models.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/ml_tools/optimize_step.py
--rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/ml_tools/parameters.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/ml_tools/printing.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/ml_tools/saveload.py
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/ml_tools/tensors.py
--rw-r--r--   0        0        0     7289 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/ml_tools/train_grad.py
--rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/ml_tools/train_no_grad.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/ml_tools/utils.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/models/__init__.py
--rw-r--r--   0        0        0    10397 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/models/qnn.py
--rw-r--r--   0        0        0    13859 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/models/quantum_model.py
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/noise/__init__.py
--rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/noise/protocols.py
--rw-r--r--   0        0        0     6736 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/noise/readout.py
--rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/operations/__init__.py
--rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/operations/analog.py
--rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/operations/control_ops.py
--rw-r--r--   0        0        0     7400 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/operations/ham_evo.py
--rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/operations/parametric.py
--rw-r--r--   0        0        0     9011 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/operations/primitive.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/transpile/__init__.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/transpile/apply_fn.py
--rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/transpile/block.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/transpile/circuit.py
--rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/transpile/digitalize.py
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/transpile/flatten.py
--rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/transpile/invert.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 qadence-1.4.1/qadence/transpile/transpile.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qadence-1.4.1/.gitignore
--rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 qadence-1.4.1/LICENSE
--rw-r--r--   0        0        0     6264 2020-02-02 00:00:00.000000 qadence-1.4.1/README.md
--rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 qadence-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     8615 2020-02-02 00:00:00.000000 qadence-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 qadence-1.5.0/.coveragerc
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 qadence-1.5.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 qadence-1.5.0/MANIFEST.in
+-rw-r--r--   0        0        0     4793 2020-02-02 00:00:00.000000 qadence-1.5.0/mkdocs.yml
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 qadence-1.5.0/renovate.json
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 qadence-1.5.0/setup.py
+-rw-r--r--   0        0        0      224 2020-02-02 00:00:00.000000 qadence-1.5.0/.github/dependabot.yml
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 qadence-1.5.0/.github/workflows/build_docs.yml
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 qadence-1.5.0/.github/workflows/dependabot.yml
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 qadence-1.5.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1410 2020-02-02 00:00:00.000000 qadence-1.5.0/.github/workflows/test_all.yml
+-rw-r--r--   0        0        0      676 2020-02-02 00:00:00.000000 qadence-1.5.0/.github/workflows/test_examples.yml
+-rw-r--r--   0        0        0     3063 2020-02-02 00:00:00.000000 qadence-1.5.0/.github/workflows/test_fast.yml
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/__init__.py
+-rw-r--r--   0        0        0    15493 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backend.py
+-rw-r--r--   0        0        0     6892 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/circuit.py
+-rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/decompose.py
+-rw-r--r--   0        0        0     1832 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/divergences.py
+-rw-r--r--   0        0        0     9287 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/execution.py
+-rw-r--r--   0        0        0     4582 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/extensions.py
+-rw-r--r--   0        0        0     1592 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/finitediff.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/libs.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/logger.py
+-rw-r--r--   0        0        0    17294 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/overlap.py
+-rw-r--r--   0        0        0    12334 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/parameters.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/protocols.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/py.typed
+-rw-r--r--   0        0        0     2120 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/qubit_support.py
+-rw-r--r--   0        0        0    10276 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/register.py
+-rw-r--r--   0        0        0    11702 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/serialization.py
+-rw-r--r--   0        0        0    14341 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/states.py
+-rw-r--r--   0        0        0     9699 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/types.py
+-rw-r--r--   0        0        0     8829 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/utils.py
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/analog/__init__.py
+-rw-r--r--   0        0        0     6435 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/analog/addressing.py
+-rw-r--r--   0        0        0     1243 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/analog/constants.py
+-rw-r--r--   0        0        0     2412 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/analog/device.py
+-rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/analog/hamiltonian_terms.py
+-rw-r--r--   0        0        0     4223 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/analog/parse_analog.py
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/__init__.py
+-rw-r--r--   0        0        0     6831 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/adjoint.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/api.py
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/gpsr.py
+-rw-r--r--   0        0        0     5038 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/jax_utils.py
+-rw-r--r--   0        0        0     6490 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/utils.py
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/braket/__init__.py
+-rw-r--r--   0        0        0     8730 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/braket/backend.py
+-rw-r--r--   0        0        0      603 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/braket/config.py
+-rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/braket/convert_ops.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/horqrux/__init__.py
+-rw-r--r--   0        0        0     9330 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/horqrux/backend.py
+-rw-r--r--   0        0        0      901 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/horqrux/config.py
+-rw-r--r--   0        0        0     8564 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/horqrux/convert_ops.py
+-rw-r--r--   0        0        0      116 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/pulser/__init__.py
+-rw-r--r--   0        0        0    13868 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/pulser/backend.py
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/pulser/channels.py
+-rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/pulser/cloud.py
+-rw-r--r--   0        0        0     3122 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/pulser/config.py
+-rw-r--r--   0        0        0     1227 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/pulser/convert_ops.py
+-rw-r--r--   0        0        0     2448 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/pulser/devices.py
+-rw-r--r--   0        0        0    11893 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/pulser/pulses.py
+-rw-r--r--   0        0        0     2227 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/pulser/waveforms.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/pyqtorch/__init__.py
+-rw-r--r--   0        0        0     9763 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/pyqtorch/backend.py
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/pyqtorch/config.py
+-rw-r--r--   0        0        0    17512 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/backends/pyqtorch/convert_ops.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/blocks/__init__.py
+-rw-r--r--   0        0        0    11796 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/blocks/abstract.py
+-rw-r--r--   0        0        0    10812 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/blocks/analog.py
+-rw-r--r--   0        0        0    17415 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/blocks/block_to_tensor.py
+-rw-r--r--   0        0        0     8897 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/blocks/composite.py
+-rw-r--r--   0        0        0     6513 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/blocks/embedding.py
+-rw-r--r--   0        0        0     2387 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/blocks/manipulate.py
+-rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/blocks/matrix.py
+-rw-r--r--   0        0        0    16631 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/blocks/primitive.py
+-rw-r--r--   0        0        0    16358 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/blocks/utils.py
+-rw-r--r--   0        0        0     1152 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/constructors/__init__.py
+-rw-r--r--   0        0        0    12170 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/constructors/ansatze.py
+-rw-r--r--   0        0        0    11566 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/constructors/feature_maps.py
+-rw-r--r--   0        0        0     8860 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/constructors/hamiltonians.py
+-rw-r--r--   0        0        0     7001 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/constructors/iia.py
+-rw-r--r--   0        0        0     7688 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/constructors/qft.py
+-rw-r--r--   0        0        0     4848 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/constructors/rydberg_feature_maps.py
+-rw-r--r--   0        0        0     8372 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/constructors/rydberg_hea.py
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/constructors/utils.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/constructors/daqc/__init__.py
+-rw-r--r--   0        0        0     9922 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/constructors/daqc/daqc.py
+-rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/constructors/daqc/gen_parser.py
+-rw-r--r--   0        0        0     1076 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/constructors/daqc/utils.py
+-rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/draw/__init__.py
+-rw-r--r--   0        0        0     5533 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/draw/themes.py
+-rw-r--r--   0        0        0    12108 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/draw/utils.py
+-rw-r--r--   0        0        0    14997 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/draw/vizbackend.py
+-rw-r--r--   0        0        0      502 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/draw/assets/dark/measurement.png
+-rw-r--r--   0        0        0     7282 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/draw/assets/dark/measurement.svg
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/draw/assets/light/measurement.png
+-rw-r--r--   0        0        0     7282 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/draw/assets/light/measurement.svg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/engines/__init__.py
+-rw-r--r--   0        0        0     5875 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/engines/differentiable_backend.py
+-rw-r--r--   0        0        0      223 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/engines/jax/__init__.py
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/engines/jax/differentiable_backend.py
+-rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/engines/jax/differentiable_expectation.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/engines/torch/__init__.py
+-rw-r--r--   0        0        0     3553 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/engines/torch/differentiable_backend.py
+-rw-r--r--   0        0        0     9161 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/engines/torch/differentiable_expectation.py
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/exceptions/__init__.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/exceptions/exceptions.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/measurements/__init__.py
+-rw-r--r--   0        0        0     1161 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/measurements/protocols.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/measurements/samples.py
+-rw-r--r--   0        0        0    12550 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/measurements/shadow.py
+-rw-r--r--   0        0        0     2665 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/measurements/tomography.py
+-rw-r--r--   0        0        0     6534 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/measurements/utils.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/mitigations/__init__.py
+-rw-r--r--   0        0        0     7768 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/mitigations/analog_zne.py
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/mitigations/protocols.py
+-rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/mitigations/readout.py
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/ml_tools/__init__.py
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/ml_tools/config.py
+-rw-r--r--   0        0        0     4283 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/ml_tools/data.py
+-rw-r--r--   0        0        0    11736 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/ml_tools/models.py
+-rw-r--r--   0        0        0     1800 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/ml_tools/optimize_step.py
+-rw-r--r--   0        0        0     1301 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/ml_tools/parameters.py
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/ml_tools/printing.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/ml_tools/saveload.py
+-rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/ml_tools/tensors.py
+-rw-r--r--   0        0        0     7399 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/ml_tools/train_grad.py
+-rw-r--r--   0        0        0     4714 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/ml_tools/train_no_grad.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/ml_tools/utils.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/models/__init__.py
+-rw-r--r--   0        0        0    10397 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/models/qnn.py
+-rw-r--r--   0        0        0    14107 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/models/quantum_model.py
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/noise/__init__.py
+-rw-r--r--   0        0        0     1653 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/noise/protocols.py
+-rw-r--r--   0        0        0     6736 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/noise/readout.py
+-rw-r--r--   0        0        0     1944 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/operations/__init__.py
+-rw-r--r--   0        0        0     7782 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/operations/analog.py
+-rw-r--r--   0        0        0     9492 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/operations/control_ops.py
+-rw-r--r--   0        0        0     7400 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/operations/ham_evo.py
+-rw-r--r--   0        0        0     4919 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/operations/parametric.py
+-rw-r--r--   0        0        0     9011 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/operations/primitive.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/transpile/__init__.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/transpile/apply_fn.py
+-rw-r--r--   0        0        0    11591 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/transpile/block.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/transpile/circuit.py
+-rw-r--r--   0        0        0     1523 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/transpile/digitalize.py
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/transpile/flatten.py
+-rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/transpile/invert.py
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 qadence-1.5.0/qadence/transpile/transpile.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 qadence-1.5.0/.gitignore
+-rw-r--r--   0        0        0    11358 2020-02-02 00:00:00.000000 qadence-1.5.0/LICENSE
+-rw-r--r--   0        0        0     6536 2020-02-02 00:00:00.000000 qadence-1.5.0/README.md
+-rw-r--r--   0        0        0     5503 2020-02-02 00:00:00.000000 qadence-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     8997 2020-02-02 00:00:00.000000 qadence-1.5.0/PKG-INFO
```

### Comparing `qadence-1.4.1/.pre-commit-config.yaml` & `qadence-1.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/mkdocs.yml` & `qadence-1.5.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/.github/workflows/build_docs.yml` & `qadence-1.5.0/.github/workflows/build_docs.yml`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/.github/workflows/test_all.yml` & `qadence-1.5.0/.github/workflows/test_all.yml`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/.github/workflows/test_examples.yml` & `qadence-1.5.0/.github/workflows/test_examples.yml`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/.github/workflows/test_fast.yml` & `qadence-1.5.0/.github/workflows/test_fast.yml`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/__init__.py` & `qadence-1.5.0/qadence/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from .types import *
 from .utils import *
 
 DEFAULT_FLOAT_DTYPE = torchfloat64
 DEFAULT_COMPLEX_DTYPE = cdouble
 set_default_dtype(DEFAULT_FLOAT_DTYPE)
 
+
 """Fetch the functions defined in the __all__ of each sub-module.
 
 Import to the qadence name space. Make sure each added submodule has the respective definition:
 
     - `__all__ = ["function0", "function1", ...]`
 
 Furthermore, add the submodule to the list below to automatically build
```

### Comparing `qadence-1.4.1/qadence/backend.py` & `qadence-1.5.0/qadence/backend.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/circuit.py` & `qadence-1.5.0/qadence/circuit.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/decompose.py` & `qadence-1.5.0/qadence/decompose.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/divergences.py` & `qadence-1.5.0/qadence/divergences.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/execution.py` & `qadence-1.5.0/qadence/execution.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/extensions.py` & `qadence-1.5.0/qadence/extensions.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/finitediff.py` & `qadence-1.5.0/qadence/finitediff.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/logger.py` & `qadence-1.5.0/qadence/logger.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/overlap.py` & `qadence-1.5.0/qadence/overlap.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/parameters.py` & `qadence-1.5.0/qadence/parameters.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/qubit_support.py` & `qadence-1.5.0/qadence/qubit_support.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/register.py` & `qadence-1.5.0/qadence/register.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/serialization.py` & `qadence-1.5.0/qadence/serialization.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/states.py` & `qadence-1.5.0/qadence/states.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/types.py` & `qadence-1.5.0/qadence/types.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/utils.py` & `qadence-1.5.0/qadence/utils.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/analog/addressing.py` & `qadence-1.5.0/qadence/analog/addressing.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/analog/constants.py` & `qadence-1.5.0/qadence/analog/constants.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/analog/device.py` & `qadence-1.5.0/qadence/analog/device.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/analog/hamiltonian_terms.py` & `qadence-1.5.0/qadence/analog/hamiltonian_terms.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/analog/parse_analog.py` & `qadence-1.5.0/qadence/analog/parse_analog.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/backends/adjoint.py` & `qadence-1.5.0/qadence/backends/adjoint.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/backends/api.py` & `qadence-1.5.0/qadence/backends/api.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/backends/gpsr.py` & `qadence-1.5.0/qadence/backends/gpsr.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/backends/jax_utils.py` & `qadence-1.5.0/qadence/backends/jax_utils.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/backends/utils.py` & `qadence-1.5.0/qadence/backends/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import torch
 from numpy.typing import ArrayLike
 from pyqtorch.apply import apply_operator
 from pyqtorch.parametric import Parametric as PyQParametric
 from torch import (
     Tensor,
     cat,
+    complex64,
     complex128,
     mean,
     no_grad,
     rand,
 )
 
 from qadence.types import ParamDictType
@@ -125,16 +126,16 @@
 
 def is_pyq_shape(state: Tensor, n_qubits: int) -> bool:
     return state.size()[:-1] == [2] * n_qubits  # type: ignore[no-any-return]
 
 
 def validate_state(state: Tensor, n_qubits: int) -> None:
     """Check if a custom initial state conforms to the qadence or the pyqtorch format."""
-    if state.dtype != complex128:
-        raise TypeError(f"Expected type complex128, got {state.dtype}")
+    if state.dtype not in [complex128, complex64]:
+        raise TypeError(f"Expected complex dtype, got {state.dtype}")
     elif len(state.size()) < 2:
         raise ValueError(f"Invalid state shape. Got {state.shape}")
     elif not is_qadence_shape(state, n_qubits) and not is_pyq_shape(state, n_qubits):
         raise ValueError(
             f"Allowed formats for custom initial state are:\
                   (1) Qadence shape: (batch_size, 2**n_qubits)\
                   (2) Pyqtorch shape: (2 * n_qubits + [batch_size])\
```

### Comparing `qadence-1.4.1/qadence/backends/braket/backend.py` & `qadence-1.5.0/qadence/backends/braket/backend.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/backends/braket/config.py` & `qadence-1.5.0/qadence/backends/braket/config.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/backends/braket/convert_ops.py` & `qadence-1.5.0/qadence/backends/braket/convert_ops.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/backends/horqrux/backend.py` & `qadence-1.5.0/qadence/backends/horqrux/backend.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/backends/horqrux/config.py` & `qadence-1.5.0/qadence/backends/horqrux/config.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/backends/horqrux/convert_ops.py` & `qadence-1.5.0/qadence/backends/horqrux/convert_ops.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/backends/pulser/backend.py` & `qadence-1.5.0/qadence/backends/pulser/backend.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/backends/pulser/cloud.py` & `qadence-1.5.0/qadence/backends/pulser/cloud.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/backends/pulser/config.py` & `qadence-1.5.0/qadence/backends/pulser/config.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/backends/pulser/convert_ops.py` & `qadence-1.5.0/qadence/backends/pulser/convert_ops.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/backends/pulser/devices.py` & `qadence-1.5.0/qadence/backends/pulser/devices.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/backends/pulser/pulses.py` & `qadence-1.5.0/qadence/backends/pulser/pulses.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/backends/pulser/waveforms.py` & `qadence-1.5.0/qadence/backends/pulser/waveforms.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/backends/pyqtorch/backend.py` & `qadence-1.5.0/qadence/backends/pyqtorch/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,15 +147,17 @@
         measurement: Measurements | None = None,
         noise: Noise | None = None,
         endianness: Endianness = Endianness.BIG,
     ) -> Tensor:
         if state is None:
             from qadence.states import zero_state
 
-            state = zero_state(circuit.abstract.n_qubits, batch_size=1)
+            state = zero_state(circuit.abstract.n_qubits, batch_size=1).to(
+                dtype=circuit.native.dtype
+            )
         if state.size(0) != 1:
             raise ValueError(
                 "Looping expectation does not make sense with batched initial state. "
                 "Define your initial state with `batch_size=1`"
             )
 
         list_expvals = []
@@ -218,36 +220,37 @@
                             torch.multinomial(input=_probs, num_samples=n_shots, replacement=True)
                         )
                     )
                     if count > 0
                 }
             )
 
-        wf = self.run(circuit=circuit, param_values=param_values, state=state)
-        probs = torch.abs(torch.pow(wf, 2))
-        samples = list(
-            map(
-                lambda _probs: _sample(
-                    _probs=_probs,
-                    n_shots=n_shots,
-                    endianness=endianness,
-                    n_qubits=circuit.abstract.n_qubits,
-                ),
-                probs,
-            )
-        )
-        if noise is not None:
-            samples = apply_noise(noise=noise, samples=samples)
-        if mitigation is not None:
-            logger.warning(
-                "Mitigation protocol is deprecated. Use qadence-protocols instead.",
+        with torch.no_grad():
+            wf = self.run(circuit=circuit, param_values=param_values, state=state)
+            probs = torch.abs(torch.pow(wf, 2))
+            samples = list(
+                map(
+                    lambda _probs: _sample(
+                        _probs=_probs,
+                        n_shots=n_shots,
+                        endianness=endianness,
+                        n_qubits=circuit.abstract.n_qubits,
+                    ),
+                    probs,
+                )
             )
-            assert noise
-            samples = apply_mitigation(noise=noise, mitigation=mitigation, samples=samples)
-        return samples
+            if noise is not None:
+                samples = apply_noise(noise=noise, samples=samples)
+            if mitigation is not None:
+                logger.warning(
+                    "Mitigation protocol is deprecated. Use qadence-protocols instead.",
+                )
+                assert noise
+                samples = apply_mitigation(noise=noise, mitigation=mitigation, samples=samples)
+            return samples
 
     def assign_parameters(self, circuit: ConvertedCircuit, param_values: dict[str, Tensor]) -> Any:
         raise NotImplementedError
 
     @staticmethod
     def _overlap(bras: Tensor, kets: Tensor) -> Tensor:
         from qadence.overlap import overlap_exact
```

### Comparing `qadence-1.4.1/qadence/backends/pyqtorch/config.py` & `qadence-1.5.0/qadence/backends/pyqtorch/config.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/backends/pyqtorch/convert_ops.py` & `qadence-1.5.0/qadence/backends/pyqtorch/convert_ops.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from functools import reduce
 from itertools import chain as flatten
 from math import prod
 from operator import add
-from typing import Sequence, Tuple
+from typing import Any, Sequence, Tuple
 
 import pyqtorch as pyq
 import sympy
 from pyqtorch.apply import apply_operator
 from pyqtorch.matrices import _dagger
 from pyqtorch.utils import is_diag
 from torch import (
@@ -22,14 +22,15 @@
     linalg,
     ones_like,
     permute,
     tensor,
     transpose,
 )
 from torch import device as torch_device
+from torch import dtype as torch_dtype
 from torch.nn import Module
 
 from qadence.backends.utils import (
     finitediff,
     pyqify,
     unpyqify,
 )
@@ -174,25 +175,27 @@
     def __init__(self, block: MatrixBlock, n_qubits: int, config: Configuration = None):
         super().__init__()
         self.n_qubits = n_qubits
         self.qubits = block.qubit_support
         self.register_buffer("mat", block.matrix.unsqueeze(2))
         self.mat: Tensor
         self._device: torch_device = self.mat.device
+        self._dtype: torch_dtype = self.mat.dtype
 
     def forward(self, state: Tensor, _: dict[str, Tensor] = None) -> Tensor:
         return apply_operator(state, self.mat, self.qubits, self.n_qubits)
 
     @property
     def device(self) -> torch_device:
         return self._device
 
-    def to(self, device: torch_device) -> PyQMatrixBlock:
-        self.mat = self.mat.to(device)
-        self._device = device
+    def to(self, *args: Any, **kwargs: Any) -> PyQMatrixBlock:
+        self.mat = self.mat.to(*args, **kwargs)
+        self._device = self.mat.device
+        self._dtype = self.mat.dtype
         return self
 
 
 class PyQComposedBlock(pyq.QuantumCircuit):
     def __init__(
         self,
         ops: list[Module],
@@ -258,28 +261,34 @@
         else:
             self.operation = pyq.QuantumCircuit(
                 n_qubits,
                 convert_block(block, n_qubits, config),
             )
             self._forward = lambda self, state, values: self.operation(state, values)
         self._device = self.operation.device
+        self._dtype = self.operation.dtype
 
     def run(self, state: Tensor, values: dict[str, Tensor]) -> Tensor:
         return self._forward(self, state, values)
 
     def forward(self, state: Tensor, values: dict[str, Tensor]) -> Tensor:
         return pyq.inner_prod(state, self.run(state, values)).real
 
     @property
     def device(self) -> torch_device:
         return self._device
 
-    def to(self, device: torch_device) -> PyQObservable:
-        self.operation = self.operation.to(device)
-        self._device = device
+    @property
+    def dtype(self) -> torch_dtype:
+        return self._dtype
+
+    def to(self, *args: Any, **kwargs: Any) -> PyQObservable:
+        self.operation = self.operation.to(*args, **kwargs)
+        self._device = self.operation.device
+        self._dtype = self.operation.dtype
         return self
 
 
 class PyQHamiltonianEvolution(Module):
     def __init__(
         self,
         qubit_support: Tuple[int, ...],
@@ -334,14 +343,15 @@
 
             self._hamiltonian = _hamiltonian
 
         self._time_evolution = lambda values: values[self.param_names[0]]
         self._device: torch_device = (
             self.hmat.device if hasattr(self, "hmat") else torch_device("cpu")
         )
+        self._dtype: torch_dtype = self.hmat.dtype if hasattr(self, "hmat") else cdouble
 
     def _unitary(self, hamiltonian: Tensor, time_evolution: Tensor) -> Tensor:
         self.batch_size = max(hamiltonian.size()[2], len(time_evolution))
         diag_check = tensor(
             [is_diag(hamiltonian[..., i]) for i in range(hamiltonian.size()[2])], device=self.device
         )
 
@@ -415,18 +425,23 @@
             self.batch_size,
         )
 
     @property
     def device(self) -> torch_device:
         return self._device
 
-    def to(self, device: torch_device) -> PyQHamiltonianEvolution:
+    @property
+    def dtype(self) -> torch_dtype:
+        return self._dtype
+
+    def to(self, *args: Any, **kwargs: Any) -> PyQHamiltonianEvolution:
         if hasattr(self, "hmat"):
-            self.hmat = self.hmat.to(device)
-        self._device = device
+            self.hmat = self.hmat.to(*args, **kwargs)
+            self._device = self.hmat.device
+            self._dtype = self.hmat.dtype
         return self
 
 
 class AddPyQOperation(pyq.QuantumCircuit):
     def __init__(self, n_qubits: int, operations: list[Module]):
         super().__init__(n_qubits=n_qubits, operations=operations)
```

### Comparing `qadence-1.4.1/qadence/blocks/__init__.py` & `qadence-1.5.0/qadence/blocks/__init__.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/blocks/abstract.py` & `qadence-1.5.0/qadence/blocks/abstract.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/blocks/analog.py` & `qadence-1.5.0/qadence/blocks/analog.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/blocks/block_to_tensor.py` & `qadence-1.5.0/qadence/blocks/block_to_tensor.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/blocks/composite.py` & `qadence-1.5.0/qadence/blocks/composite.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/blocks/embedding.py` & `qadence-1.5.0/qadence/blocks/embedding.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/blocks/manipulate.py` & `qadence-1.5.0/qadence/blocks/manipulate.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/blocks/matrix.py` & `qadence-1.5.0/qadence/blocks/matrix.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/blocks/primitive.py` & `qadence-1.5.0/qadence/blocks/primitive.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/blocks/utils.py` & `qadence-1.5.0/qadence/blocks/utils.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/constructors/__init__.py` & `qadence-1.5.0/qadence/constructors/__init__.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/constructors/ansatze.py` & `qadence-1.5.0/qadence/constructors/ansatze.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/constructors/feature_maps.py` & `qadence-1.5.0/qadence/constructors/feature_maps.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/constructors/hamiltonians.py` & `qadence-1.5.0/qadence/constructors/hamiltonians.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/constructors/iia.py` & `qadence-1.5.0/qadence/constructors/iia.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/constructors/qft.py` & `qadence-1.5.0/qadence/constructors/qft.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/constructors/rydberg_feature_maps.py` & `qadence-1.5.0/qadence/constructors/rydberg_feature_maps.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/constructors/rydberg_hea.py` & `qadence-1.5.0/qadence/constructors/rydberg_hea.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/constructors/utils.py` & `qadence-1.5.0/qadence/constructors/utils.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/constructors/daqc/daqc.py` & `qadence-1.5.0/qadence/constructors/daqc/daqc.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/constructors/daqc/gen_parser.py` & `qadence-1.5.0/qadence/constructors/daqc/gen_parser.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/constructors/daqc/utils.py` & `qadence-1.5.0/qadence/constructors/daqc/utils.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/draw/__init__.py` & `qadence-1.5.0/qadence/draw/__init__.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/draw/themes.py` & `qadence-1.5.0/qadence/draw/themes.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/draw/utils.py` & `qadence-1.5.0/qadence/draw/utils.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/draw/vizbackend.py` & `qadence-1.5.0/qadence/draw/vizbackend.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/draw/assets/dark/measurement.svg` & `qadence-1.5.0/qadence/draw/assets/dark/measurement.svg`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/draw/assets/light/measurement.svg` & `qadence-1.5.0/qadence/draw/assets/light/measurement.svg`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/engines/differentiable_backend.py` & `qadence-1.5.0/qadence/engines/differentiable_backend.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/engines/jax/differentiable_backend.py` & `qadence-1.5.0/qadence/engines/jax/differentiable_backend.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/engines/jax/differentiable_expectation.py` & `qadence-1.5.0/qadence/engines/jax/differentiable_expectation.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/engines/torch/differentiable_backend.py` & `qadence-1.5.0/qadence/engines/torch/differentiable_backend.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/engines/torch/differentiable_expectation.py` & `qadence-1.5.0/qadence/models/quantum_model.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,391 +1,364 @@
 from __future__ import annotations
 
+import os
 from collections import Counter, OrderedDict
-from dataclasses import dataclass
-from functools import partial
-from typing import Any, Callable, Sequence
+from dataclasses import asdict
+from pathlib import Path
+from typing import Any, Callable, Optional, Sequence
 
 import torch
-from torch import Tensor
-from torch.autograd import Function
-from torch.nn import Module
-
-from qadence.backend import Backend as QuantumBackend
-from qadence.backend import Converted, ConvertedCircuit, ConvertedObservable
-from qadence.backends.adjoint import AdjointExpectation
-from qadence.backends.utils import infer_batchsize, is_pyq_shape, param_dict, pyqify, validate_state
+from torch import Tensor, nn
+
+from qadence.backend import (
+    Backend,
+    BackendConfiguration,
+    BackendName,
+    ConvertedCircuit,
+    ConvertedObservable,
+)
+from qadence.backends.api import backend_factory, config_factory
 from qadence.blocks.abstract import AbstractBlock
-from qadence.blocks.primitive import PrimitiveBlock
-from qadence.blocks.utils import uuid_to_block, uuid_to_eigen
+from qadence.blocks.utils import chain, unique_parameters
 from qadence.circuit import QuantumCircuit
-from qadence.extensions import get_gpsr_fns
+from qadence.engines.differentiable_backend import DifferentiableBackend
+from qadence.logger import get_logger
 from qadence.measurements import Measurements
 from qadence.mitigations import Mitigations
-from qadence.ml_tools import promote_to_tensor
 from qadence.noise import Noise
+from qadence.parameters import Parameter
 from qadence.types import DiffMode, Endianness
 
+logger = get_logger(__name__)
 
-class PSRExpectation(Function):
-    """Overloads the PyTorch AD system to perform parameter shift rule on quantum circuits."""
 
-    @staticmethod
-    def forward(
-        ctx: Any,
-        expectation_fn: Callable[[dict[str, Tensor]], Tensor],
-        param_psrs: Sequence[Callable],
-        param_keys: Sequence[str],
-        *param_values: Tensor,
-    ) -> Tensor:
-        for param in param_values:
-            param = param.detach()
+class QuantumModel(nn.Module):
+    """The central class of qadence that executes `QuantumCircuit`s and make them differentiable.
 
-        ctx.expectation_fn = expectation_fn
-        ctx.param_psrs = param_psrs
-        ctx.param_keys = param_keys
-        ctx.save_for_backward(*param_values)
-
-        expectation_values = expectation_fn(param_values=param_dict(param_keys, param_values))  # type: ignore[call-arg] # noqa: E501
-        # Stack batches of expectations if so.
-        if isinstance(expectation_values, list):
-            return torch.stack(expectation_values)
-        else:
-            return expectation_values
+    This class should be used as base class for any new quantum model supported in the qadence
+    framework for information on the implementation of custom models see
+    [here](/advanced_tutorials/custom-models.md).
+    """
 
-    @staticmethod
-    def backward(ctx: Any, grad_out: Tensor) -> tuple:
-        params = param_dict(ctx.param_keys, ctx.saved_tensors)
-
-        def expectation_fn(params: dict[str, Tensor]) -> Tensor:
-            return PSRExpectation.apply(
-                ctx.expectation_fn,
-                ctx.param_psrs,
-                params.keys(),
-                *params.values(),
-            )
+    backend: Backend | DifferentiableBackend
+    embedding_fn: Callable
+    _params: nn.ParameterDict
+    _circuit: ConvertedCircuit
+    _observable: list[ConvertedObservable] | None
 
-        def vjp(psr: Callable, name: str) -> Tensor:
-            """
-            !!! warn.
-
-                Sums over gradients corresponding to different observables.
-            """
-            return (grad_out * psr(expectation_fn, params, name)).sum(dim=1)
-
-        grads = [
-            vjp(psr, name) if needs_grad else None
-            for psr, name, needs_grad in zip(
-                ctx.param_psrs, ctx.param_keys, ctx.needs_input_grad[3:]
-            )
-        ]
-        return (None, None, None, *grads)
+    def __init__(
+        self,
+        circuit: QuantumCircuit,
+        observable: list[AbstractBlock] | AbstractBlock | None = None,
+        backend: BackendName | str = BackendName.PYQTORCH,
+        diff_mode: DiffMode = DiffMode.AD,
+        measurement: Measurements | None = None,
+        noise: Noise | None = None,
+        mitigation: Mitigations | None = None,
+        configuration: BackendConfiguration | dict | None = None,
+    ):
+        """Initialize a generic QuantumModel instance.
 
+        Arguments:
+            circuit: The circuit that is executed.
+            observable: Optional observable(s) that are used only in the `expectation` method. You
+                can also provide observables on the fly to the expectation call directly.
+            backend: A backend for circuit execution.
+            diff_mode: A differentiability mode. Parameter shift based modes work on all backends.
+                AD based modes only on PyTorch based backends.
+            measurement: Optional measurement protocol. If None, use
+                exact expectation value with a statevector simulator.
+            configuration: Configuration for the backend.
+            noise: A noise model to use.
 
-@dataclass
-class DifferentiableExpectation:
-    """A handler for differentiating expectation estimation using various engines."""
-
-    backend: QuantumBackend
-    circuit: ConvertedCircuit
-    observable: list[ConvertedObservable] | ConvertedObservable
-    param_values: dict[str, Tensor]
-    state: Tensor | None = None
-    measurement: Measurements | None = None
-    noise: Noise | None = None
-    mitigation: Mitigations | None = None
-    endianness: Endianness = Endianness.BIG
-
-    def ad(self) -> Tensor:
-        self.observable = (
-            self.observable if isinstance(self.observable, list) else [self.observable]
-        )
-        if self.measurement:
-            expectation_fn = self.measurement.get_measurement_fn()
-            expectations = expectation_fn(
-                circuit=self.circuit.original,
-                observables=[obs.original for obs in self.observable],
-                param_values=self.param_values,
-                options=self.measurement.options,
-                state=self.state,
-                backend=self.backend,
-                noise=self.noise,
-                endianness=self.endianness,
-            )
-        else:
-            expectations = self.backend.expectation(
-                circuit=self.circuit,
-                observable=self.observable,
-                param_values=self.param_values,
-                state=self.state,
-                noise=self.noise,
-                mitigation=self.mitigation,
-                endianness=self.endianness,
+        Raises:
+            ValueError: if the `diff_mode` argument is set to None
+        """
+        super().__init__()
+
+        if not isinstance(circuit, QuantumCircuit):
+            TypeError(
+                f"The circuit should be of type '<class QuantumCircuit>'. Got {type(circuit)}."
             )
-        return promote_to_tensor(
-            expectations if isinstance(expectations, Tensor) else torch.tensor(expectations)
-        )
 
-    def adjoint(self) -> Tensor:
-        self.observable = (
-            self.observable if isinstance(self.observable, list) else [self.observable]
+        if diff_mode is None:
+            raise ValueError("`diff_mode` cannot be `None` in a `QuantumModel`.")
+
+        self.backend = backend_factory(
+            backend=backend, diff_mode=diff_mode, configuration=configuration
         )
-        if len(self.observable) > 1:
-            raise NotImplementedError("AdjointExpectation currently only supports one observable.")
 
-        n_qubits = self.circuit.abstract.n_qubits
-        values_batch_size = infer_batchsize(self.param_values)
-        if self.state is None:
-            self.state = self.circuit.native.init_state(batch_size=values_batch_size)
+        if isinstance(observable, list) or observable is None:
+            observable = observable
         else:
-            validate_state(self.state, n_qubits)
-            self.state = (
-                pyqify(self.state, n_qubits)
-                if not is_pyq_shape(self.state, n_qubits)
-                else self.state
-            )
-        batch_size = max(values_batch_size, self.state.size(-1))
-        return (
-            AdjointExpectation.apply(
-                self.circuit.native,
-                self.observable[0].native,  # Currently, adjoint only supports a single observable.
-                self.state,
-                self.param_values.keys(),
-                *self.param_values.values(),
-            )
-            .unsqueeze(1)
-            .reshape(batch_size, 1)
-        )  # we expect (batch_size, n_observables) shape
-
-    def psr(self, psr_fn: Callable, **psr_args: int | float | None) -> Tensor:
-        # wrapper which unpacks the parameters
-        # as pytorch grads can only calculated w.r.t tensors
-        # so we unpack the params, feed in the names separately
-        # as apply doesn't take keyword arguments
-        # We also fold in the observable into the backend which makes
-        # life easier in the custom autodiff.
-        self.observable = (
-            self.observable if isinstance(self.observable, list) else [self.observable]
-        )
+            observable = [observable]
 
-        if self.measurement is not None:
-            expectation_fn = partial(
-                self.measurement.get_measurement_fn(),
-                circuit=self.circuit.original,
-                observables=[obs.original for obs in self.observable],
-                options=self.measurement.options,
-                state=self.state,
-                noise=self.noise,
-                endianness=self.endianness,
-            )
+        def _is_feature_param(p: Parameter) -> bool:
+            return not p.trainable and not p.is_number
+
+        if observable is None:
+            self.inputs = list(filter(_is_feature_param, circuit.unique_parameters))
         else:
-            expectation_fn = partial(
-                self.backend.expectation,
-                circuit=self.circuit,
-                observable=self.observable,
-                state=self.state,
-                noise=self.noise,
-                mitigation=self.mitigation,
-                endianness=self.endianness,
-            )
-        # PSR only applies to parametric circuits.
-        if isinstance(self.observable, ConvertedObservable):
-            self.observable = [self.observable]
-        param_to_psr = self.construct_rules(
-            self.circuit.abstract, [o.abstract for o in self.observable], psr_fn, **psr_args
+            uparams = unique_parameters(chain(circuit.block, *observable))
+            self.inputs = list(filter(_is_feature_param, uparams))
+
+        conv = self.backend.convert(circuit, observable)
+        self.embedding_fn = conv.embedding_fn
+        self._circuit = conv.circuit
+        self._observable = conv.observable
+        self._backend_name = backend
+        self._diff_mode = diff_mode
+        self._measurement = measurement
+        self._noise = noise
+        self._mitigation = mitigation
+        self._params = nn.ParameterDict(
+            {
+                str(key): nn.Parameter(val, requires_grad=val.requires_grad)
+                for key, val in conv.params.items()
+            }
         )
 
-        # Select the subset of all parameters for which PSR apply
-        # which are from the circuit only.
-        self.param_values = {k: self.param_values[k] for k in param_to_psr.keys()}
-
-        return PSRExpectation.apply(expectation_fn, param_to_psr.values(), self.param_values.keys(), *self.param_values.values())  # type: ignore # noqa: E501
-
-    # Make PSR construction a static method to avoid unhashability issues.
-    @staticmethod
-    def construct_rules(
-        circuit: QuantumCircuit,
-        observable: list[AbstractBlock],
-        psr_fn: Callable,
-        **psr_args: int | float | None,
-    ) -> dict[str, Callable]:
-        """Create a mapping between parameters and PSR functions."""
-
-        uuid_to_eigs = uuid_to_eigen(circuit.block)
-        # We currently rely on implicit ordering to match the PSR to the parameter,
-        # because we want to cache PSRs.
-
-        param_to_psr = OrderedDict()
-        for param_id, eigenvalues in uuid_to_eigs.items():
-            if eigenvalues is None:
-                raise ValueError(
-                    f"Eigenvalues are not defined for param_id {param_id}\n"
-                    # f"of type {type(block)}.\n"
-                    "PSR cannot be defined in that case."
-                )
+    @property
+    def vparams(self) -> OrderedDict:
+        return OrderedDict({k: v.data for k, v in self._params.items() if v.requires_grad})
+
+    @property
+    def vals_vparams(self) -> Tensor:
+        """Dictionary with parameters which are actually updated during optimization."""
+        vals = torch.tensor([v for v in self._params.values() if v.requires_grad])
+        vals.requires_grad = False
+        return vals.flatten()
+
+    @property
+    def in_features(self) -> int:
+        """Number of inputs."""
+        return len(self.inputs)
+
+    @property
+    def out_features(self) -> int | None:
+        """Number of outputs."""
+        return 0 if self._observable is None else len(self._observable)
+
+    @property
+    def num_vparams(self) -> int:
+        """The number of variational parameters."""
+        return len(self.vals_vparams)
 
-            param_to_psr[param_id] = psr_fn(eigenvalues, **psr_args)
-        for obs in observable:
-            for param_id, _ in uuid_to_eigen(obs).items():
-                # We need the embedded fixed params of the observable in the param_values dict
-                # to be able to call expectation. Since torch backward requires
-                # a list of param_ids and values of equal length, we need to pass them to PSR too.
-                # Since they are constants their gradients are 0.
-                param_to_psr[param_id] = lambda x: torch.tensor([0.0], requires_grad=False)
-        return param_to_psr
-
-
-class DifferentiableBackend(Module):
-    """A class to abstract the operations done by the autodiff engine.
-
-    Arguments:
-        backend: An instance of the QuantumBackend type perform execution.
-        diff_mode: A differentiable mode supported by the differentiation engine.
-        **psr_args: Arguments that will be passed on to `DifferentiableExpectation`.
-    """
+    def circuit(self, circuit: QuantumCircuit) -> ConvertedCircuit:
+        return self.backend.circuit(circuit)
 
-    def __init__(
-        self,
-        backend: QuantumBackend,
-        diff_mode: DiffMode = DiffMode.AD,
-        **psr_args: int | float | None,
-    ) -> None:
-        super().__init__()
+    def observable(self, observable: AbstractBlock, n_qubits: int) -> Any:
+        return self.backend.observable(observable, n_qubits)
 
-        self.backend = backend
-        self.diff_mode = diff_mode
-        self.psr_args = psr_args
-        # TODO: Add differentiable overlap calculation
-        self._overlap: Callable = None  # type: ignore [assignment]
+    def reset_vparams(self, values: Sequence) -> None:
+        """Reset all the variational parameters with a given list of values."""
+        current_vparams = OrderedDict({k: v for k, v in self._params.items() if v.requires_grad})
+
+        assert (
+            len(values) == self.num_vparams
+        ), "Pass an iterable with the values of all variational parameters"
+        for i, k in enumerate(current_vparams.keys()):
+            current_vparams[k].data = torch.tensor([values[i]])
+
+    def forward(self, *args: Any, **kwargs: Any) -> Tensor:
+        return self.run(*args, **kwargs)
 
     def run(
         self,
-        circuit: ConvertedCircuit,
-        param_values: dict = {},
+        values: dict[str, Tensor] = None,
         state: Tensor | None = None,
         endianness: Endianness = Endianness.BIG,
     ) -> Tensor:
-        """Run on the underlying backend."""
-        return self.backend.run(
-            circuit=circuit, param_values=param_values, state=state, endianness=endianness
+        if values is None:
+            values = {}
+        params = self.embedding_fn(self._params, values)
+        return self.backend.run(self._circuit, params, state=state, endianness=endianness)
+
+    def sample(
+        self,
+        values: dict[str, torch.Tensor] = {},
+        n_shots: int = 1000,
+        state: torch.Tensor | None = None,
+        noise: Noise | None = None,
+        mitigation: Mitigations | None = None,
+        endianness: Endianness = Endianness.BIG,
+    ) -> list[Counter]:
+        params = self.embedding_fn(self._params, values)
+        if noise is None:
+            noise = self._noise
+        else:
+            self._noise = noise
+        if mitigation is None:
+            mitigation = self._mitigation
+        return self.backend.sample(
+            self._circuit,
+            params,
+            n_shots=n_shots,
+            state=state,
+            noise=noise,
+            mitigation=mitigation,
+            endianness=endianness,
         )
 
     def expectation(
         self,
-        circuit: ConvertedCircuit,
-        observable: list[ConvertedObservable] | ConvertedObservable,
-        param_values: dict[str, Tensor] = {},
-        state: Tensor | None = None,
+        values: dict[str, Tensor] = {},
+        observable: list[ConvertedObservable] | ConvertedObservable | None = None,
+        state: Optional[Tensor] = None,
         measurement: Measurements | None = None,
         noise: Noise | None = None,
         mitigation: Mitigations | None = None,
         endianness: Endianness = Endianness.BIG,
     ) -> Tensor:
-        """Compute the expectation value of a given observable.
-
-        Arguments:
-            circuit: A backend native quantum circuit to be executed.
-            observable: A backend native observable to compute the expectation value from.
-            param_values: A dict of values for symbolic substitution.
-            state: An initial state.
-            measurement: A shot-based measurement protocol.
-            endianness: Endianness of the state.
+        """Compute expectation using the given backend.
 
         Returns:
-            A tensor of expectation values.
+            A torch.Tensor of shape n_batches x n_obs
         """
-        observable = observable if isinstance(observable, list) else [observable]
-        differentiable_expectation = DifferentiableExpectation(
-            backend=self.backend,
-            circuit=circuit,
+        if observable is None:
+            if self._observable is None:
+                raise ValueError(
+                    "Provide an AbstractBlock as the observable to compute expectation."
+                    "Either pass a 'native_observable' directly to 'QuantumModel.expectation'"
+                    "or pass a (non-native) '<class AbstractBlock>' to the 'QuantumModel.__init__'."
+                )
+            observable = self._observable
+
+        params = self.embedding_fn(self._params, values)
+        if measurement is None:
+            measurement = self._measurement
+        if noise is None:
+            noise = self._noise
+        else:
+            self._noise = noise
+        if mitigation is None:
+            mitigation = self._mitigation
+        return self.backend.expectation(
+            circuit=self._circuit,
             observable=observable,
-            param_values=param_values,
+            param_values=params,
             state=state,
             measurement=measurement,
             noise=noise,
             mitigation=mitigation,
             endianness=endianness,
         )
 
-        if self.diff_mode == DiffMode.AD:
-            expectation = differentiable_expectation.ad
-        elif self.diff_mode == DiffMode.ADJOINT:
-            expectation = differentiable_expectation.adjoint
-        else:
-            try:
-                fns = get_gpsr_fns()
-                psr_fn = fns[self.diff_mode]
-            except KeyError:
-                raise ValueError(f"{self.diff_mode} differentiation mode is not supported")
-            expectation = partial(differentiable_expectation.psr, psr_fn=psr_fn, **self.psr_args)
-        return expectation()
+    def overlap(self) -> Tensor:
+        raise NotImplementedError("The overlap method is not implemented for this model.")
 
-    def sample(
-        self,
-        circuit: ConvertedCircuit,
-        param_values: dict[str, Tensor],
-        n_shots: int = 1,
-        state: Tensor | None = None,
-        noise: Noise | None = None,
-        mitigation: Mitigations | None = None,
-        endianness: Endianness = Endianness.BIG,
-    ) -> list[Counter]:
-        """Sample bitstring from the registered circuit.
-
-        Arguments:
-            circuit: A backend native quantum circuit to be executed.
-            param_values: The values of the parameters after embedding
-            n_shots: The number of shots. Defaults to 1.
-            state: Initial state.
-            noise: A noise model to use.
-            mitigation: A mitigation protocol to apply to noisy samples.
-            endianness: Endianness of the resulting bitstrings.
-
-        Returns:
-            An iterable with all the sampled bitstrings
-        """
-        with torch.no_grad():
-            return self.backend.sample(
-                circuit=circuit,
-                param_values=param_values,
-                n_shots=n_shots,
-                state=state,
-                noise=noise,
-                mitigation=mitigation,
-                endianness=endianness,
-            )
+    def _to_dict(self, save_params: bool = False) -> dict[str, Any]:
+        d = dict()
+        try:
+            if isinstance(self._observable, list):
+                abs_obs = [obs.abstract._to_dict() for obs in self._observable]
+            else:
+                abs_obs = [dict()]
 
-    def circuit(self, circuit: QuantumCircuit) -> ConvertedCircuit:
-        parametrized_blocks = list(uuid_to_block(circuit.block).values())
-        non_prim_blocks = filter(lambda b: not isinstance(b, PrimitiveBlock), parametrized_blocks)
-        if len(list(non_prim_blocks)) > 0:
-            raise ValueError(
-                "The circuit contains non-primitive blocks that are currently not supported by the "
-                "PSR differentiable mode."
-            )
-        return self.backend.circuit(circuit)
+            d = {
+                "circuit": self._circuit.abstract._to_dict(),
+                "observable": abs_obs,
+                "backend": self._backend_name,
+                "diff_mode": self._diff_mode,
+                "measurement": self._measurement._to_dict()
+                if self._measurement is not None
+                else {},
+                "noise": self._noise._to_dict() if self._noise is not None else {},
+                "backend_configuration": asdict(self.backend.backend.config),  # type: ignore
+            }
+            param_dict_conv = {}
+            if save_params:
+                param_dict_conv = {name: param.data for name, param in self._params.items()}
+            d = {self.__class__.__name__: d, "param_dict": param_dict_conv}
+            logger.debug(f"{self.__class__.__name__} serialized to {d}.")
+        except Exception as e:
+            logger.warning(f"Unable to serialize {self.__class__.__name__} due to {e}.")
+        return d
+
+    @classmethod
+    def _from_dict(cls, d: dict, as_torch: bool = False) -> QuantumModel:
+        from qadence.serialization import deserialize
+
+        qm: QuantumModel
+        try:
+            qm_dict = d[cls.__name__]
+            qm = cls(
+                circuit=QuantumCircuit._from_dict(qm_dict["circuit"]),
+                observable=(
+                    None
+                    if not isinstance(qm_dict["observable"], list)
+                    else [deserialize(q_obs) for q_obs in qm_dict["observable"]]  # type: ignore[misc]
+                ),
+                backend=qm_dict["backend"],
+                diff_mode=qm_dict["diff_mode"],
+                measurement=Measurements._from_dict(qm_dict["measurement"]),
+                noise=Noise._from_dict(qm_dict["noise"]),
+                configuration=config_factory(qm_dict["backend"], qm_dict["backend_configuration"]),
+            )
+
+            if as_torch:
+                conv_pd = torch.nn.ParameterDict()
+                param_dict = d["param_dict"]
+                for n, param in param_dict.items():
+                    conv_pd[n] = torch.nn.Parameter(param)
+                qm._params = conv_pd
+            logger.debug(f"Initialized {cls.__name__} from {d}.")
 
-    def observable(self, observable: AbstractBlock, n_qubits: int) -> ConvertedObservable:
-        if observable is not None and observable.is_parametric:
-            raise ValueError("PSR cannot be applied to a parametric observable.")
-        return self.backend.observable(observable, n_qubits)
+        except Exception as e:
+            logger.warning(f"Unable to deserialize object {d} to {cls.__name__} due to {e}.")
 
-    def convert(
-        self,
-        circuit: QuantumCircuit,
-        observable: list[AbstractBlock] | AbstractBlock | None = None,
-    ) -> Converted:
-        if self.diff_mode != DiffMode.AD and observable is not None:
-            msg = (
-                f"Differentiation mode '{self.diff_mode}' does not support parametric observables."
-            )
-            if isinstance(observable, list):
-                for obs in observable:
-                    if obs.is_parametric:
-                        raise ValueError(msg)
-            else:
-                if observable.is_parametric:
-                    raise ValueError(msg)
-        return self.backend.convert(circuit, observable)
+        return qm
 
-    def assign_parameters(self, circuit: ConvertedCircuit, param_values: dict[str, Tensor]) -> Any:
-        return self.backend.assign_parameters(circuit, param_values)
+    def save(
+        self, folder: str | Path, file_name: str = "quantum_model.pt", save_params: bool = True
+    ) -> None:
+        if not os.path.isdir(folder):
+            raise FileNotFoundError
+        try:
+            torch.save(self._to_dict(save_params), folder / Path(file_name))
+        except Exception as e:
+            print(f"Unable to write QuantumModel to disk due to {e}")
+
+    @classmethod
+    def load(
+        cls, file_path: str | Path, as_torch: bool = False, map_location: str | torch.device = "cpu"
+    ) -> QuantumModel:
+        qm_pt = {}
+        if isinstance(file_path, str):
+            file_path = Path(file_path)
+        if os.path.isdir(file_path):
+            from qadence.ml_tools.saveload import get_latest_checkpoint_name
+
+            file_path = file_path / get_latest_checkpoint_name(file_path, "model")
+
+        try:
+            qm_pt = torch.load(file_path, map_location=map_location)
+        except Exception as e:
+            print(f"Unable to load QuantumModel due to {e}")
+        return cls._from_dict(qm_pt, as_torch)
+
+    def assign_parameters(self, values: dict[str, Tensor]) -> Any:
+        """Return the final, assigned circuit that is used in e.g. `backend.run`."""
+        params = self.embedding_fn(self._params, values)
+        return self.backend.assign_parameters(self._circuit, params)
+
+    def to(self, *args: Any, **kwargs: Any) -> QuantumModel:
+        try:
+            if isinstance(self._circuit.native, torch.nn.Module):
+                # Backends which are not torch-based cannot be moved to 'device'
+                self._circuit.native = self._circuit.native.to(*args, **kwargs)
+                if self._observable is not None:
+                    if isinstance(self._observable, ConvertedObservable):
+                        self._observable.native = self._observable.native.to(*args, **kwargs)
+                    elif isinstance(self._observable, list):
+                        for obs in self._observable:
+                            obs.native = obs.native.to(*args, **kwargs)
+                self._params = self._params.to(
+                    device=self._circuit.native.device,
+                    dtype=torch.float64
+                    if self._circuit.native.dtype == torch.cdouble
+                    else torch.float32,
+                )
+                logger.debug(f"Moved {self} to {args}, {kwargs}.")
+        except Exception as e:
+            logger.warning(f"Unable to move {self} to {args}, {kwargs} due to {e}.")
+        return self
```

### Comparing `qadence-1.4.1/qadence/measurements/protocols.py` & `qadence-1.5.0/qadence/measurements/protocols.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/measurements/samples.py` & `qadence-1.5.0/qadence/measurements/samples.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/measurements/shadow.py` & `qadence-1.5.0/qadence/measurements/shadow.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/measurements/tomography.py` & `qadence-1.5.0/qadence/measurements/tomography.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/measurements/utils.py` & `qadence-1.5.0/qadence/measurements/utils.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/mitigations/analog_zne.py` & `qadence-1.5.0/qadence/mitigations/analog_zne.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/mitigations/protocols.py` & `qadence-1.5.0/qadence/mitigations/protocols.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/mitigations/readout.py` & `qadence-1.5.0/qadence/mitigations/readout.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/ml_tools/__init__.py` & `qadence-1.5.0/qadence/ml_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/ml_tools/config.py` & `qadence-1.5.0/qadence/ml_tools/config.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/ml_tools/data.py` & `qadence-1.5.0/qadence/ml_tools/data.py`

 * *Files 14% similar despite different names*

```diff
@@ -78,42 +78,42 @@
     ```
     """
     ds = InfiniteTensorDataset(*tensors) if infinite else TensorDataset(*tensors)
     return DataLoader(ds, batch_size=batch_size)
 
 
 @singledispatch
-def data_to_device(xs: Any, device: torch_device) -> Any:
+def data_to_device(xs: Any, *args: Any, **kwargs: Any) -> Any:
     """Utility method to move arbitrary data to 'device'."""
-    raise ValueError(f"Cannot move {type(xs)} to a pytorch device.")
+    raise ValueError(f"Unable to move {type(xs)} with input args: {args} and kwargs: {kwargs}.")
 
 
 @data_to_device.register
-def _(xs: None, device: torch_device) -> None:
+def _(xs: None, *args: Any, **kwargs: Any) -> None:
     return xs
 
 
 @data_to_device.register(Tensor)
-def _(xs: Tensor, device: torch_device) -> Tensor:
-    return xs.to(device=device, non_blocking=True)
+def _(xs: Tensor, *args: Any, **kwargs: Any) -> Tensor:
+    return xs.to(*args, **kwargs)
 
 
 @data_to_device.register(list)
-def _(xs: list, device: torch_device) -> list:
-    return [data_to_device(x, device) for x in xs]
+def _(xs: list, *args: Any, **kwargs: Any) -> list:
+    return [data_to_device(x, *args, **kwargs) for x in xs]
 
 
 @data_to_device.register(dict)
-def _(xs: dict, device: torch_device) -> dict:
-    return {key: data_to_device(val, device) for key, val in xs.items()}
+def _(xs: dict, *args: Any, **kwargs: Any) -> dict:
+    return {key: data_to_device(val, *args, **kwargs) for key, val in xs.items()}
 
 
 @data_to_device.register(DataLoader)
-def _(xs: DataLoader, device: torch_device) -> DataLoader:
-    return DataLoader(data_to_device(xs.dataset, device))
+def _(xs: DataLoader, *args: Any, **kwargs: Any) -> DataLoader:
+    return DataLoader(data_to_device(xs.dataset, *args, **kwargs))
 
 
 @data_to_device.register(DictDataLoader)
 def _(xs: DictDataLoader, device: torch_device) -> DictDataLoader:
     return DictDataLoader({key: data_to_device(val, device) for key, val in xs.dataloaders.items()})
```

### Comparing `qadence-1.4.1/qadence/ml_tools/models.py` & `qadence-1.5.0/qadence/ml_tools/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -282,19 +282,19 @@
             out_features=d["out_features"],
             input_scaling=torch.tensor(d["_input_scaling"]),
             output_scaling=torch.tensor(d["_output_scaling"]),
             input_shifting=torch.tensor(d["_input_shifting"]),
             output_shifting=torch.tensor(d["_output_shifting"]),
         )
 
-    def to(self, device: torch.device) -> TransformedModule:
+    def to(self, *args: Any, **kwargs: Any) -> TransformedModule:
         try:
-            self.model = self.model.to(device)
-            self._input_scaling = self._input_scaling.to(device)
-            self._input_shifting = self._input_shifting.to(device)
-            self._output_scaling = self._output_scaling.to(device)
-            self._output_shifting = self._output_shifting.to(device)
+            self.model = self.model.to(*args, **kwargs)
+            self._input_scaling = self._input_scaling.to(*args, **kwargs)
+            self._input_shifting = self._input_shifting.to(*args, **kwargs)
+            self._output_scaling = self._output_scaling.to(*args, **kwargs)
+            self._output_shifting = self._output_shifting.to(*args, **kwargs)
 
-            logger.debug(f"Moved {self} to device {device}.")
+            logger.debug(f"Moved {self} to {args}, {kwargs}.")
         except Exception as e:
-            logger.warning(f"Unable to move {self} to device {device} due to {e}.")
+            logger.warning(f"Unable to move {self} to {args}, {kwargs} due to {e}.")
         return self
```

### Comparing `qadence-1.4.1/qadence/ml_tools/optimize_step.py` & `qadence-1.5.0/qadence/ml_tools/optimize_step.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 def optimize_step(
     model: Module,
     optimizer: Optimizer,
     loss_fn: Callable,
     xs: dict | list | torch.Tensor | None,
     device: torch.device = None,
+    dtype: torch.dtype = None,
 ) -> tuple[torch.Tensor | float, dict | None]:
     """Default Torch optimize step with closure.
 
     This is the default optimization step which should work for most
     of the standard use cases of optimization of Torch models
 
     Args:
@@ -31,15 +32,15 @@
 
     Returns:
         tuple: tuple containing the model, the optimizer, a dictionary with
             the collected metrics and the compute value loss
     """
 
     loss, metrics = None, {}
-    xs_to_device = data_to_device(xs, device)
+    xs_to_device = data_to_device(xs, device=device, dtype=dtype)
 
     def closure() -> Any:
         # NOTE: We need the nonlocal as we can't return a metric dict and
         # because e.g. LBFGS calls this closure multiple times but for some
         # reason the returned loss is always the first one...
         nonlocal metrics, loss
         optimizer.zero_grad()
```

### Comparing `qadence-1.4.1/qadence/ml_tools/parameters.py` & `qadence-1.5.0/qadence/ml_tools/parameters.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/ml_tools/printing.py` & `qadence-1.5.0/qadence/ml_tools/printing.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/ml_tools/saveload.py` & `qadence-1.5.0/qadence/ml_tools/saveload.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/ml_tools/tensors.py` & `qadence-1.5.0/qadence/ml_tools/tensors.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/ml_tools/train_grad.py` & `qadence-1.5.0/qadence/ml_tools/train_grad.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from typing import Callable, Union
 
 from rich.progress import BarColumn, Progress, TaskProgressColumn, TextColumn, TimeRemainingColumn
 from torch import device as torch_device
+from torch import dtype as torch_dtype
 from torch.nn import DataParallel, Module
 from torch.optim import Optimizer
 from torch.utils.data import DataLoader
 from torch.utils.tensorboard import SummaryWriter
 
 from qadence.logger import get_logger
 from qadence.ml_tools.config import TrainConfig
@@ -24,14 +25,15 @@
     dataloader: Union[None, DataLoader, DictDataLoader],
     optimizer: Optimizer,
     config: TrainConfig,
     loss_fn: Callable,
     device: torch_device = None,
     optimize_step: Callable = optimize_step,
     write_tensorboard: Callable = write_tensorboard,
+    dtype: torch_dtype = None,
 ) -> tuple[Module, Optimizer]:
     """Runs the training loop with gradient-based optimizer.
 
     Assumes that `loss_fn` returns a tuple of (loss,
     metrics: dict), where `metrics` is a dict of scalars. Loss and metrics are
     written to tensorboard. Checkpoints are written every
     `config.checkpoint_every` steps (and after the last training step).  If a
@@ -107,17 +109,17 @@
     data = to_dataloader(x, y, batch_size=batch_size, infinite=True)
     train_with_grad(model, data, optimizer, config, loss_fn=loss_fn)
     ```
     """
 
     # Move model to device before optimizer is loaded
     if isinstance(model, DataParallel):
-        model = model.module.to(device)
+        model = model.module.to(device=device, dtype=dtype)
     else:
-        model = model.to(device)
+        model = model.to(device=device, dtype=dtype)
     # load available checkpoint
     init_iter = 0
     if config.folder:
         model, optimizer, init_iter = load_checkpoint(config.folder, model, optimizer)
         logger.debug(f"Loaded model and optimizer from {config.folder}")
     # initialize tensorboard
     writer = SummaryWriter(config.folder, purge_step=init_iter)
```

### Comparing `qadence-1.4.1/qadence/ml_tools/train_no_grad.py` & `qadence-1.5.0/qadence/ml_tools/train_no_grad.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/ml_tools/utils.py` & `qadence-1.5.0/qadence/ml_tools/utils.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/models/qnn.py` & `qadence-1.5.0/qadence/models/qnn.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/noise/protocols.py` & `qadence-1.5.0/qadence/noise/protocols.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/noise/readout.py` & `qadence-1.5.0/qadence/noise/readout.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/operations/__init__.py` & `qadence-1.5.0/qadence/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/operations/analog.py` & `qadence-1.5.0/qadence/operations/analog.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/operations/control_ops.py` & `qadence-1.5.0/qadence/operations/control_ops.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/operations/ham_evo.py` & `qadence-1.5.0/qadence/operations/ham_evo.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/operations/parametric.py` & `qadence-1.5.0/qadence/operations/parametric.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/operations/primitive.py` & `qadence-1.5.0/qadence/operations/primitive.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/transpile/apply_fn.py` & `qadence-1.5.0/qadence/transpile/apply_fn.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/transpile/block.py` & `qadence-1.5.0/qadence/transpile/block.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/transpile/digitalize.py` & `qadence-1.5.0/qadence/transpile/digitalize.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/transpile/flatten.py` & `qadence-1.5.0/qadence/transpile/flatten.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/transpile/invert.py` & `qadence-1.5.0/qadence/transpile/invert.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/qadence/transpile/transpile.py` & `qadence-1.5.0/qadence/transpile/transpile.py`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/.gitignore` & `qadence-1.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/LICENSE` & `qadence-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qadence-1.4.1/README.md` & `qadence-1.5.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -50,14 +50,16 @@
 ```
 
 The default, pre-installed backend for Qadence is [PyQTorch](https://github.com/pasqal-io/pyqtorch), a differentiable state vector simulator for digital-analog simulation based on `PyTorch`. It is possible to install additional, `PyTorch` -based backends and the circuit visualization library using the following extras:
 
 * `pulser`: The [Pulser](https://github.com/pasqal-io/Pulser) backend for composing, simulating and executing pulse sequences for neutral-atom quantum devices.
 * `braket`: The [Braket](https://github.com/amazon-braket/amazon-braket-sdk-python) backend, an open source library that provides a framework for interacting with quantum computing hardware devices through Amazon Braket.
 * `visualization`: A visualization library to display quantum circuit diagrams.
+* `protocols`: A collection of [protocols](https://github.com/pasqal-io/qadence-protocols) for error mitigation in Qadence.
+* `libs`: A collection of [functionalities](https://github.com/pasqal-io/qadence-libs) for graph machine learning problems build on top of Qadence.
 
 Qadence also supports a `JAX` engine which is currently supporting the [Horqrux](https://github.com/pasqal-io/horqrux) backend. `horqrux` is currently only available via the [low-level API](examples/backends/low_level/horqrux_backend.py).
 
 
 To install individual extras, use the following syntax (**IMPORTANT** Make sure to use quotes):
 
 ```bash
```

### Comparing `qadence-1.4.1/pyproject.toml` & `qadence-1.5.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -14,17 +14,17 @@
     { name = "Vincent Elfving", email = "vincent.elfving@pasqal.com" },
     { name = "Dominik Seitz", email = "dominik.seitz@pasqal.com" },
     { name = "Roland Guichard", email = "roland.guichard@pasqal.com" },
     { name = "Joao P. Moutinho", email = "joao.moutinho@pasqal.com"},
     { name = "Vytautas Abramavicius", email = "vytautas.abramavicius@pasqal.com" },
     { name = "Gergana Velikova", email = "gergana.velikova@pasqal.com" },
 ]
-requires-python = ">=3.9,<3.12"
+requires-python = ">=3.9,<3.13"
 license = {text = "Apache 2.0"}
-version = "1.4.1"
+version = "1.5.0"
 classifiers=[
     "License :: OSI Approved :: Apache Software License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
@@ -38,25 +38,25 @@
     "sympytorch>=0.1.2",
     "rich",
     "tensorboard>=2.12.0",
     "deepdiff",
     "jsonschema",
     "nevergrad",
     "scipy",
-    "pyqtorch==1.0.6",
+    "pyqtorch==1.1.0",
     "matplotlib",
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 allow-ambiguous-features = true
 
 [project.optional-dependencies]
 pulser = ["pulser>=v0.15.2", "pasqal-cloud>=0.3.5"]
-braket = ["amazon-braket-sdk"]
+braket = ["amazon-braket-sdk==1.71.0"]
 visualization = [
   "graphviz",
   # FIXME: will be needed once we support latex labels
   # "latex2svg @ git+https://github.com/Moonbase59/latex2svg.git#egg=latex2svg",
   # "scour",
 ]
 horqrux = [
@@ -64,19 +64,21 @@
     "jax",
     "flax",
     "optax",
     "jaxopt",
     "einops",
     "sympy2jax"]
 protocols = ["qadence-protocols"]
+libs = ["qadence-libs"]
 all = [
   "pulser>=0.15.2",
   "amazon-braket-sdk",
   "graphviz",
   "protocols",
+  "libs",
   # FIXME: will be needed once we support latex labels
   # "latex2svg @ git+https://github.com/Moonbase59/latex2svg.git#egg=latex2svg",
   # "scour",
 ]
 
 [tool.hatch.envs.default]
 dependencies = [
```

### Comparing `qadence-1.4.1/PKG-INFO` & `qadence-1.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,50 +1,53 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: qadence
-Version: 1.4.1
+Version: 1.5.0
 Summary: Pasqal interface for circuit-based quantum computing SDKs
 Author-email: Aleksander Wennersteen <aleksander.wennersteen@pasqal.com>, Gert-Jan Both <gert-jan.both@pasqal.com>, Niklas Heim <niklas.heim@pasqal.com>, Mario Dagrada <mario.dagrada@pasqal.com>, Vincent Elfving <vincent.elfving@pasqal.com>, Dominik Seitz <dominik.seitz@pasqal.com>, Roland Guichard <roland.guichard@pasqal.com>, "Joao P. Moutinho" <joao.moutinho@pasqal.com>, Vytautas Abramavicius <vytautas.abramavicius@pasqal.com>, Gergana Velikova <gergana.velikova@pasqal.com>
 License: Apache 2.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: <3.12,>=3.9
+Requires-Python: <3.13,>=3.9
 Requires-Dist: deepdiff
 Requires-Dist: jsonschema
 Requires-Dist: matplotlib
 Requires-Dist: nevergrad
 Requires-Dist: numpy
 Requires-Dist: openfermion
-Requires-Dist: pyqtorch==1.0.6
+Requires-Dist: pyqtorch==1.1.0
 Requires-Dist: rich
 Requires-Dist: scipy
 Requires-Dist: sympytorch>=0.1.2
 Requires-Dist: tensorboard>=2.12.0
 Requires-Dist: torch
 Provides-Extra: all
 Requires-Dist: amazon-braket-sdk; extra == 'all'
 Requires-Dist: graphviz; extra == 'all'
+Requires-Dist: libs; extra == 'all'
 Requires-Dist: protocols; extra == 'all'
 Requires-Dist: pulser>=0.15.2; extra == 'all'
 Provides-Extra: braket
-Requires-Dist: amazon-braket-sdk; extra == 'braket'
+Requires-Dist: amazon-braket-sdk==1.71.0; extra == 'braket'
 Provides-Extra: horqrux
 Requires-Dist: einops; extra == 'horqrux'
 Requires-Dist: flax; extra == 'horqrux'
 Requires-Dist: horqrux==0.6.0; extra == 'horqrux'
 Requires-Dist: jax; extra == 'horqrux'
 Requires-Dist: jaxopt; extra == 'horqrux'
 Requires-Dist: optax; extra == 'horqrux'
 Requires-Dist: sympy2jax; extra == 'horqrux'
+Provides-Extra: libs
+Requires-Dist: qadence-libs; extra == 'libs'
 Provides-Extra: protocols
 Requires-Dist: qadence-protocols; extra == 'protocols'
 Provides-Extra: pulser
 Requires-Dist: pasqal-cloud>=0.3.5; extra == 'pulser'
 Requires-Dist: pulser>=v0.15.2; extra == 'pulser'
 Provides-Extra: visualization
 Requires-Dist: graphviz; extra == 'visualization'
@@ -102,14 +105,16 @@
 ```
 
 The default, pre-installed backend for Qadence is [PyQTorch](https://github.com/pasqal-io/pyqtorch), a differentiable state vector simulator for digital-analog simulation based on `PyTorch`. It is possible to install additional, `PyTorch` -based backends and the circuit visualization library using the following extras:
 
 * `pulser`: The [Pulser](https://github.com/pasqal-io/Pulser) backend for composing, simulating and executing pulse sequences for neutral-atom quantum devices.
 * `braket`: The [Braket](https://github.com/amazon-braket/amazon-braket-sdk-python) backend, an open source library that provides a framework for interacting with quantum computing hardware devices through Amazon Braket.
 * `visualization`: A visualization library to display quantum circuit diagrams.
+* `protocols`: A collection of [protocols](https://github.com/pasqal-io/qadence-protocols) for error mitigation in Qadence.
+* `libs`: A collection of [functionalities](https://github.com/pasqal-io/qadence-libs) for graph machine learning problems build on top of Qadence.
 
 Qadence also supports a `JAX` engine which is currently supporting the [Horqrux](https://github.com/pasqal-io/horqrux) backend. `horqrux` is currently only available via the [low-level API](examples/backends/low_level/horqrux_backend.py).
 
 
 To install individual extras, use the following syntax (**IMPORTANT** Make sure to use quotes):
 
 ```bash
```

