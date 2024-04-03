# Comparing `tmp/composer-0.21.1.tar.gz` & `tmp/composer-0.21.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composer-0.21.1.tar", last modified: Fri Mar 22 01:14:39 2024, max compression
+gzip compressed data, was "composer-0.21.2.tar", last modified: Wed Apr  3 21:26:04 2024, max compression
```

## Comparing `composer-0.21.1.tar` & `composer-0.21.2.tar`

### file list

```diff
@@ -1,315 +1,315 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.748216 composer-0.21.1/
--rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-03-22 01:14:28.000000 composer-0.21.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-22 01:14:28.000000 composer-0.21.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20625 2024-03-22 01:14:39.748216 composer-0.21.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19811 2024-03-22 01:14:28.000000 composer-0.21.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.696216 composer-0.21.1/composer/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-22 01:14:28.000000 composer-0.21.1/composer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-22 01:14:28.000000 composer-0.21.1/composer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-22 01:14:28.000000 composer-0.21.1/composer/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.696216 composer-0.21.1/composer/algorithms/
--rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.696216 composer-0.21.1/composer/algorithms/alibi/
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/alibi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8550 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/alibi/alibi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.700216 composer-0.21.1/composer/algorithms/alibi/attention_surgery_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/alibi/attention_surgery_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/alibi/attention_surgery_functions/_bert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/alibi/attention_surgery_functions/_gpt2.py
--rw-r--r--   0 runner    (1001) docker     (127)    10389 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/alibi/attention_surgery_functions/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/alibi/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.700216 composer-0.21.1/composer/algorithms/augmix/
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/augmix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11810 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/augmix/augmix.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/augmix/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.700216 composer-0.21.1/composer/algorithms/blurpool/
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/blurpool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/blurpool/blurpool.py
--rw-r--r--   0 runner    (1001) docker     (127)    13165 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/blurpool/blurpool_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/blurpool/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.700216 composer-0.21.1/composer/algorithms/channels_last/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/channels_last/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/channels_last/channels_last.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/channels_last/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.700216 composer-0.21.1/composer/algorithms/colout/
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/colout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/colout/colout.py
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/colout/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.700216 composer-0.21.1/composer/algorithms/cutmix/
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/cutmix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17083 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/cutmix/cutmix.py
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/cutmix/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.704216 composer-0.21.1/composer/algorithms/cutout/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/cutout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/cutout/cutout.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/cutout/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.704216 composer-0.21.1/composer/algorithms/ema/
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/ema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22108 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/ema/ema.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/ema/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.704216 composer-0.21.1/composer/algorithms/factorize/
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/factorize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12068 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/factorize/factorize.py
--rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/factorize/factorize_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    22287 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/factorize/factorize_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/factorize/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.704216 composer-0.21.1/composer/algorithms/gated_linear_units/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/gated_linear_units/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/gated_linear_units/gated_linear_unit_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10631 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/gated_linear_units/gated_linear_units.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/gated_linear_units/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.704216 composer-0.21.1/composer/algorithms/ghost_batchnorm/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/ghost_batchnorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/ghost_batchnorm/ghost_batchnorm.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/ghost_batchnorm/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.704216 composer-0.21.1/composer/algorithms/gradient_clipping/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/gradient_clipping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9799 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/gradient_clipping/gradient_clipping.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/gradient_clipping/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.708216 composer-0.21.1/composer/algorithms/gyro_dropout/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/gyro_dropout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/gyro_dropout/gyro_dropout.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/gyro_dropout/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.708216 composer-0.21.1/composer/algorithms/label_smoothing/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/label_smoothing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/label_smoothing/label_smoothing.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/label_smoothing/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.708216 composer-0.21.1/composer/algorithms/layer_freezing/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/layer_freezing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9080 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/layer_freezing/layer_freezing.py
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/layer_freezing/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.708216 composer-0.21.1/composer/algorithms/low_precision_groupnorm/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/low_precision_groupnorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/low_precision_groupnorm/low_precision_groupnorm.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/low_precision_groupnorm/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.708216 composer-0.21.1/composer/algorithms/low_precision_layernorm/
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/low_precision_layernorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/low_precision_layernorm/low_precision_layernorm.py
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/low_precision_layernorm/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.708216 composer-0.21.1/composer/algorithms/mixup/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/mixup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/mixup/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)     9942 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/mixup/mixup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.708216 composer-0.21.1/composer/algorithms/no_op_model/
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/no_op_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/no_op_model/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/no_op_model/no_op_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.712216 composer-0.21.1/composer/algorithms/progressive_resizing/
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/progressive_resizing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/progressive_resizing/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/progressive_resizing/progressive_resizing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.712216 composer-0.21.1/composer/algorithms/randaugment/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/randaugment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/randaugment/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)     8939 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/randaugment/randaugment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.712216 composer-0.21.1/composer/algorithms/sam/
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/sam/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/sam/sam.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.712216 composer-0.21.1/composer/algorithms/selective_backprop/
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/selective_backprop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/selective_backprop/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)    11777 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/selective_backprop/selective_backprop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.712216 composer-0.21.1/composer/algorithms/seq_length_warmup/
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/seq_length_warmup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/seq_length_warmup/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)    19516 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/seq_length_warmup/seq_length_warmup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.712216 composer-0.21.1/composer/algorithms/squeeze_excite/
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/squeeze_excite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/squeeze_excite/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/squeeze_excite/squeeze_excite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.716216 composer-0.21.1/composer/algorithms/stochastic_depth/
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/stochastic_depth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/stochastic_depth/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/stochastic_depth/stochastic_depth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/stochastic_depth/stochastic_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.716216 composer-0.21.1/composer/algorithms/swa/
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/swa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/swa/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)    13024 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/swa/swa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.716216 composer-0.21.1/composer/algorithms/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/utils/augmentation_common.py
--rw-r--r--   0 runner    (1001) docker     (127)    12119 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/utils/augmentation_primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.716216 composer-0.21.1/composer/algorithms/weight_standardization/
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/weight_standardization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/weight_standardization/metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-03-22 01:14:28.000000 composer-0.21.1/composer/algorithms/weight_standardization/weight_standardization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.720216 composer-0.21.1/composer/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-03-22 01:14:28.000000 composer-0.21.1/composer/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13015 2024-03-22 01:14:28.000000 composer-0.21.1/composer/callbacks/activation_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)    26883 2024-03-22 01:14:28.000000 composer-0.21.1/composer/callbacks/checkpoint_saver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-03-22 01:14:28.000000 composer-0.21.1/composer/callbacks/early_stopper.py
--rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-03-22 01:14:28.000000 composer-0.21.1/composer/callbacks/eval_output_logging_callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-03-22 01:14:28.000000 composer-0.21.1/composer/callbacks/export_for_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-03-22 01:14:28.000000 composer-0.21.1/composer/callbacks/free_outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-03-22 01:14:28.000000 composer-0.21.1/composer/callbacks/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8777 2024-03-22 01:14:28.000000 composer-0.21.1/composer/callbacks/image_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-03-22 01:14:28.000000 composer-0.21.1/composer/callbacks/lr_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     9393 2024-03-22 01:14:28.000000 composer-0.21.1/composer/callbacks/memory_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8826 2024-03-22 01:14:28.000000 composer-0.21.1/composer/callbacks/memory_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)    17348 2024-03-22 01:14:28.000000 composer-0.21.1/composer/callbacks/mlperf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-22 01:14:28.000000 composer-0.21.1/composer/callbacks/nan_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-03-22 01:14:28.000000 composer-0.21.1/composer/callbacks/oom_observer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-03-22 01:14:28.000000 composer-0.21.1/composer/callbacks/optimizer_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8654 2024-03-22 01:14:28.000000 composer-0.21.1/composer/callbacks/runtime_estimator.py
--rw-r--r--   0 runner    (1001) docker     (127)    17116 2024-03-22 01:14:28.000000 composer-0.21.1/composer/callbacks/speed_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-03-22 01:14:28.000000 composer-0.21.1/composer/callbacks/system_metrics_monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-03-22 01:14:28.000000 composer-0.21.1/composer/callbacks/threshold_stopper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.720216 composer-0.21.1/composer/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-03-22 01:14:28.000000 composer-0.21.1/composer/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-22 01:14:28.000000 composer-0.21.1/composer/cli/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    22187 2024-03-22 01:14:28.000000 composer-0.21.1/composer/cli/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.724216 composer-0.21.1/composer/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-03-22 01:14:28.000000 composer-0.21.1/composer/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-03-22 01:14:28.000000 composer-0.21.1/composer/core/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)    17788 2024-03-22 01:14:28.000000 composer-0.21.1/composer/core/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)    15146 2024-03-22 01:14:28.000000 composer-0.21.1/composer/core/data_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)    24106 2024-03-22 01:14:28.000000 composer-0.21.1/composer/core/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-03-22 01:14:28.000000 composer-0.21.1/composer/core/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (127)    11315 2024-03-22 01:14:28.000000 composer-0.21.1/composer/core/event.py
--rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-03-22 01:14:28.000000 composer-0.21.1/composer/core/passes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-03-22 01:14:28.000000 composer-0.21.1/composer/core/precision.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-03-22 01:14:28.000000 composer-0.21.1/composer/core/serializable.py
--rw-r--r--   0 runner    (1001) docker     (127)    83077 2024-03-22 01:14:28.000000 composer-0.21.1/composer/core/state.py
--rw-r--r--   0 runner    (1001) docker     (127)    36521 2024-03-22 01:14:28.000000 composer-0.21.1/composer/core/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-03-22 01:14:28.000000 composer-0.21.1/composer/core/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.724216 composer-0.21.1/composer/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-22 01:14:28.000000 composer-0.21.1/composer/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    83195 2024-03-22 01:14:28.000000 composer-0.21.1/composer/datasets/in_context_learning_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-03-22 01:14:28.000000 composer-0.21.1/composer/datasets/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.724216 composer-0.21.1/composer/devices/
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-03-22 01:14:28.000000 composer-0.21.1/composer/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-03-22 01:14:28.000000 composer-0.21.1/composer/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-22 01:14:28.000000 composer-0.21.1/composer/devices/device_cpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-03-22 01:14:28.000000 composer-0.21.1/composer/devices/device_gpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-03-22 01:14:28.000000 composer-0.21.1/composer/devices/device_hpu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-03-22 01:14:28.000000 composer-0.21.1/composer/devices/device_mps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-03-22 01:14:28.000000 composer-0.21.1/composer/devices/device_neuron.py
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-03-22 01:14:28.000000 composer-0.21.1/composer/devices/device_tpu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.724216 composer-0.21.1/composer/functional/
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-03-22 01:14:28.000000 composer-0.21.1/composer/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.728216 composer-0.21.1/composer/loggers/
--rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-03-22 01:14:28.000000 composer-0.21.1/composer/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10917 2024-03-22 01:14:28.000000 composer-0.21.1/composer/loggers/cometml_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    11062 2024-03-22 01:14:28.000000 composer-0.21.1/composer/loggers/console_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    12032 2024-03-22 01:14:28.000000 composer-0.21.1/composer/loggers/file_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-03-22 01:14:28.000000 composer-0.21.1/composer/loggers/in_memory_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-03-22 01:14:28.000000 composer-0.21.1/composer/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-03-22 01:14:28.000000 composer-0.21.1/composer/loggers/logger_destination.py
--rw-r--r--   0 runner    (1001) docker     (127)    22266 2024-03-22 01:14:28.000000 composer-0.21.1/composer/loggers/mlflow_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    12239 2024-03-22 01:14:28.000000 composer-0.21.1/composer/loggers/mosaicml_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    11579 2024-03-22 01:14:28.000000 composer-0.21.1/composer/loggers/neptune_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    15255 2024-03-22 01:14:28.000000 composer-0.21.1/composer/loggers/progress_bar_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    31771 2024-03-22 01:14:28.000000 composer-0.21.1/composer/loggers/remote_uploader_downloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-03-22 01:14:28.000000 composer-0.21.1/composer/loggers/slack_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-03-22 01:14:28.000000 composer-0.21.1/composer/loggers/tensorboard_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)    17395 2024-03-22 01:14:28.000000 composer-0.21.1/composer/loggers/wandb_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.728216 composer-0.21.1/composer/loss/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-22 01:14:28.000000 composer-0.21.1/composer/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11673 2024-03-22 01:14:28.000000 composer-0.21.1/composer/loss/loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-03-22 01:14:28.000000 composer-0.21.1/composer/loss/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.732216 composer-0.21.1/composer/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-03-22 01:14:28.000000 composer-0.21.1/composer/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16757 2024-03-22 01:14:28.000000 composer-0.21.1/composer/metrics/map.py
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-03-22 01:14:28.000000 composer-0.21.1/composer/metrics/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    38870 2024-03-22 01:14:28.000000 composer-0.21.1/composer/metrics/nlp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.732216 composer-0.21.1/composer/models/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-03-22 01:14:28.000000 composer-0.21.1/composer/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-03-22 01:14:28.000000 composer-0.21.1/composer/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    49317 2024-03-22 01:14:28.000000 composer-0.21.1/composer/models/huggingface.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-03-22 01:14:28.000000 composer-0.21.1/composer/models/initializers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.732216 composer-0.21.1/composer/models/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-22 01:14:28.000000 composer-0.21.1/composer/models/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-03-22 01:14:28.000000 composer-0.21.1/composer/models/tasks/classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.732216 composer-0.21.1/composer/optim/
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-03-22 01:14:28.000000 composer-0.21.1/composer/optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18605 2024-03-22 01:14:28.000000 composer-0.21.1/composer/optim/decoupled_weight_decay.py
--rw-r--r--   0 runner    (1001) docker     (127)    39120 2024-03-22 01:14:28.000000 composer-0.21.1/composer/optim/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.736216 composer-0.21.1/composer/profiler/
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-03-22 01:14:28.000000 composer-0.21.1/composer/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21003 2024-03-22 01:14:28.000000 composer-0.21.1/composer/profiler/json_trace_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-03-22 01:14:28.000000 composer-0.21.1/composer/profiler/json_trace_merger.py
--rw-r--r--   0 runner    (1001) docker     (127)     9088 2024-03-22 01:14:28.000000 composer-0.21.1/composer/profiler/marker.py
--rw-r--r--   0 runner    (1001) docker     (127)    15160 2024-03-22 01:14:28.000000 composer-0.21.1/composer/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-03-22 01:14:28.000000 composer-0.21.1/composer/profiler/profiler_action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-03-22 01:14:28.000000 composer-0.21.1/composer/profiler/profiler_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-03-22 01:14:28.000000 composer-0.21.1/composer/profiler/system_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    18111 2024-03-22 01:14:28.000000 composer-0.21.1/composer/profiler/torch_profiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-03-22 01:14:28.000000 composer-0.21.1/composer/profiler/trace_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-03-22 01:14:28.000000 composer-0.21.1/composer/profiler/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:28.000000 composer-0.21.1/composer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.736216 composer-0.21.1/composer/trainer/
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-22 01:14:28.000000 composer-0.21.1/composer/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-03-22 01:14:28.000000 composer-0.21.1/composer/trainer/_deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-03-22 01:14:28.000000 composer-0.21.1/composer/trainer/_scale_schedule.py
--rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-03-22 01:14:28.000000 composer-0.21.1/composer/trainer/_scaler.py
--rw-r--r--   0 runner    (1001) docker     (127)    38951 2024-03-22 01:14:28.000000 composer-0.21.1/composer/trainer/dist_strategy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-03-22 01:14:28.000000 composer-0.21.1/composer/trainer/meta_safe_apply.py
--rw-r--r--   0 runner    (1001) docker     (127)     4107 2024-03-22 01:14:28.000000 composer-0.21.1/composer/trainer/mosaic_fsdp.py
--rw-r--r--   0 runner    (1001) docker     (127)    51445 2024-03-22 01:14:28.000000 composer-0.21.1/composer/trainer/mosaic_fsdp_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)   181215 2024-03-22 01:14:28.000000 composer-0.21.1/composer/trainer/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.740216 composer-0.21.1/composer/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/auto_log_hparams.py
--rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/batch_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    58011 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    15301 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/collect_env.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/compression.py
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (127)    26200 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/dist.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.740216 composer-0.21.1/composer/utils/eval_client/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/eval_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/eval_client/eval_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/eval_client/lambda_eval_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/eval_client/local_eval_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/eval_client/mosaicml_lambda_eval_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    31422 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/file_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    13356 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/fx_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/import_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    16345 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/iter_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9878 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    18833 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/module_surgery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.744216 composer-0.21.1/composer/utils/object_store/
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/object_store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/object_store/gcs_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     8952 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/object_store/libcloud_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    19428 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/object_store/mlflow_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/object_store/object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/object_store/oci_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     8830 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/object_store/s3_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    12224 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/object_store/sftp_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/object_store/uc_object_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     8442 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/reproducibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/retrying.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/string_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-22 01:14:28.000000 composer-0.21.1/composer/utils/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.696216 composer-0.21.1/composer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20625 2024-03-22 01:14:39.000000 composer-0.21.1/composer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9788 2024-03-22 01:14:39.000000 composer-0.21.1/composer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-22 01:14:39.000000 composer-0.21.1/composer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-22 01:14:39.000000 composer-0.21.1/composer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-03-22 01:14:39.000000 composer-0.21.1/composer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-22 01:14:39.000000 composer-0.21.1/composer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)    36090 2024-03-22 01:14:28.000000 composer-0.21.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 01:14:39.748216 composer-0.21.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8676 2024-03-22 01:14:28.000000 composer-0.21.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 01:14:39.744216 composer-0.21.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-22 01:14:28.000000 composer-0.21.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-03-22 01:14:28.000000 composer-0.21.1/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-03-22 01:14:28.000000 composer-0.21.1/tests/test_docker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-03-22 01:14:28.000000 composer-0.21.1/tests/test_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10059 2024-03-22 01:14:28.000000 composer-0.21.1/tests/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-03-22 01:14:28.000000 composer-0.21.1/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-03-22 01:14:28.000000 composer-0.21.1/tests/test_full_nlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-03-22 01:14:28.000000 composer-0.21.1/tests/test_loss.py
--rw-r--r--   0 runner    (1001) docker     (127)     6928 2024-03-22 01:14:28.000000 composer-0.21.1/tests/test_notebooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-03-22 01:14:28.000000 composer-0.21.1/tests/test_passes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-03-22 01:14:28.000000 composer-0.21.1/tests/test_precision.py
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-03-22 01:14:28.000000 composer-0.21.1/tests/test_simple_nlp.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-22 01:14:28.000000 composer-0.21.1/tests/test_smoketest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-03-22 01:14:28.000000 composer-0.21.1/tests/test_split_batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-03-22 01:14:28.000000 composer-0.21.1/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-03-22 01:14:28.000000 composer-0.21.1/tests/test_time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.023074 composer-0.21.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    10770 2024-04-03 21:25:51.000000 composer-0.21.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-03 21:25:51.000000 composer-0.21.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20625 2024-04-03 21:26:04.023074 composer-0.21.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19811 2024-04-03 21:25:51.000000 composer-0.21.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.979074 composer-0.21.2/composer/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-03 21:25:51.000000 composer-0.21.2/composer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-03 21:25:51.000000 composer-0.21.2/composer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-03 21:25:51.000000 composer-0.21.2/composer/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.983074 composer-0.21.2/composer/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (127)     3947 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.983074 composer-0.21.2/composer/algorithms/alibi/
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/alibi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8550 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/alibi/alibi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.983074 composer-0.21.2/composer/algorithms/alibi/attention_surgery_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/alibi/attention_surgery_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8054 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/alibi/attention_surgery_functions/_bert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/alibi/attention_surgery_functions/_gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10389 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/alibi/attention_surgery_functions/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/alibi/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.983074 composer-0.21.2/composer/algorithms/augmix/
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/augmix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11810 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/augmix/augmix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/augmix/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.983074 composer-0.21.2/composer/algorithms/blurpool/
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/blurpool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7992 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/blurpool/blurpool.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13165 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/blurpool/blurpool_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/blurpool/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.983074 composer-0.21.2/composer/algorithms/channels_last/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/channels_last/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/channels_last/channels_last.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/channels_last/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.983074 composer-0.21.2/composer/algorithms/colout/
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/colout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/colout/colout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/colout/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.987074 composer-0.21.2/composer/algorithms/cutmix/
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/cutmix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17083 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/cutmix/cutmix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/cutmix/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.987074 composer-0.21.2/composer/algorithms/cutout/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/cutout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/cutout/cutout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/cutout/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.987074 composer-0.21.2/composer/algorithms/ema/
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/ema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22108 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/ema/ema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/ema/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.987074 composer-0.21.2/composer/algorithms/factorize/
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/factorize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12068 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/factorize/factorize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15205 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/factorize/factorize_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22287 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/factorize/factorize_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/factorize/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.987074 composer-0.21.2/composer/algorithms/gated_linear_units/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/gated_linear_units/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/gated_linear_units/gated_linear_unit_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10631 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/gated_linear_units/gated_linear_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/gated_linear_units/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.987074 composer-0.21.2/composer/algorithms/ghost_batchnorm/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/ghost_batchnorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8621 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/ghost_batchnorm/ghost_batchnorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/ghost_batchnorm/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.987074 composer-0.21.2/composer/algorithms/gradient_clipping/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/gradient_clipping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9799 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/gradient_clipping/gradient_clipping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/gradient_clipping/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.991074 composer-0.21.2/composer/algorithms/gyro_dropout/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/gyro_dropout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/gyro_dropout/gyro_dropout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/gyro_dropout/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.991074 composer-0.21.2/composer/algorithms/label_smoothing/
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/label_smoothing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/label_smoothing/label_smoothing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/label_smoothing/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.991074 composer-0.21.2/composer/algorithms/layer_freezing/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/layer_freezing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9080 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/layer_freezing/layer_freezing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/layer_freezing/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.991074 composer-0.21.2/composer/algorithms/low_precision_groupnorm/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/low_precision_groupnorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5117 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/low_precision_groupnorm/low_precision_groupnorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/low_precision_groupnorm/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.991074 composer-0.21.2/composer/algorithms/low_precision_layernorm/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/low_precision_layernorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5122 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/low_precision_layernorm/low_precision_layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/low_precision_layernorm/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.991074 composer-0.21.2/composer/algorithms/mixup/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/mixup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/mixup/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9942 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/mixup/mixup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.991074 composer-0.21.2/composer/algorithms/no_op_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/no_op_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/no_op_model/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/no_op_model/no_op_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.991074 composer-0.21.2/composer/algorithms/progressive_resizing/
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/progressive_resizing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/progressive_resizing/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13440 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/progressive_resizing/progressive_resizing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.995074 composer-0.21.2/composer/algorithms/randaugment/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/randaugment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/randaugment/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8939 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/randaugment/randaugment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.995074 composer-0.21.2/composer/algorithms/sam/
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/sam/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6797 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/sam/sam.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.995074 composer-0.21.2/composer/algorithms/selective_backprop/
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/selective_backprop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/selective_backprop/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11777 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/selective_backprop/selective_backprop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.995074 composer-0.21.2/composer/algorithms/seq_length_warmup/
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/seq_length_warmup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/seq_length_warmup/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19516 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/seq_length_warmup/seq_length_warmup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.995074 composer-0.21.2/composer/algorithms/squeeze_excite/
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/squeeze_excite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/squeeze_excite/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/squeeze_excite/squeeze_excite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.995074 composer-0.21.2/composer/algorithms/stochastic_depth/
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/stochastic_depth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/stochastic_depth/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/stochastic_depth/stochastic_depth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/stochastic_depth/stochastic_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.995074 composer-0.21.2/composer/algorithms/swa/
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/swa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/swa/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13024 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/swa/swa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.995074 composer-0.21.2/composer/algorithms/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/utils/augmentation_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12119 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/utils/augmentation_primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.999074 composer-0.21.2/composer/algorithms/weight_standardization/
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/weight_standardization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/weight_standardization/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-03 21:25:51.000000 composer-0.21.2/composer/algorithms/weight_standardization/weight_standardization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.999074 composer-0.21.2/composer/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13015 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/activation_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26883 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/checkpoint_saver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6799 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/early_stopper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5045 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/eval_output_logging_callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/export_for_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/free_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8777 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/image_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/lr_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9393 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/memory_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8826 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/memory_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17348 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/mlperf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/nan_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8544 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/oom_observer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/optimizer_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8654 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/runtime_estimator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17116 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/speed_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3319 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/system_metrics_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5611 2024-04-03 21:25:51.000000 composer-0.21.2/composer/callbacks/threshold_stopper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.999074 composer-0.21.2/composer/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-03 21:25:51.000000 composer-0.21.2/composer/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-03 21:25:51.000000 composer-0.21.2/composer/cli/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    22187 2024-04-03 21:25:51.000000 composer-0.21.2/composer/cli/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.003074 composer-0.21.2/composer/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-03 21:25:51.000000 composer-0.21.2/composer/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5252 2024-04-03 21:25:51.000000 composer-0.21.2/composer/core/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17788 2024-04-03 21:25:51.000000 composer-0.21.2/composer/core/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15334 2024-04-03 21:25:51.000000 composer-0.21.2/composer/core/data_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24244 2024-04-03 21:25:51.000000 composer-0.21.2/composer/core/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-04-03 21:25:51.000000 composer-0.21.2/composer/core/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11315 2024-04-03 21:25:51.000000 composer-0.21.2/composer/core/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2024-04-03 21:25:51.000000 composer-0.21.2/composer/core/passes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-03 21:25:51.000000 composer-0.21.2/composer/core/precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-03 21:25:51.000000 composer-0.21.2/composer/core/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83107 2024-04-03 21:25:51.000000 composer-0.21.2/composer/core/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36521 2024-04-03 21:25:51.000000 composer-0.21.2/composer/core/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-03 21:25:51.000000 composer-0.21.2/composer/core/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.003074 composer-0.21.2/composer/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-03 21:25:51.000000 composer-0.21.2/composer/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83538 2024-04-03 21:25:51.000000 composer-0.21.2/composer/datasets/in_context_learning_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-04-03 21:25:51.000000 composer-0.21.2/composer/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.007074 composer-0.21.2/composer/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-03 21:25:51.000000 composer-0.21.2/composer/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-03 21:25:51.000000 composer-0.21.2/composer/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-03 21:25:51.000000 composer-0.21.2/composer/devices/device_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2252 2024-04-03 21:25:51.000000 composer-0.21.2/composer/devices/device_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-03 21:25:51.000000 composer-0.21.2/composer/devices/device_hpu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-03 21:25:51.000000 composer-0.21.2/composer/devices/device_mps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-03 21:25:51.000000 composer-0.21.2/composer/devices/device_neuron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-03 21:25:51.000000 composer-0.21.2/composer/devices/device_tpu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.007074 composer-0.21.2/composer/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-03 21:25:51.000000 composer-0.21.2/composer/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.007074 composer-0.21.2/composer/loggers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1804 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10917 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/cometml_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11062 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/console_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12032 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/file_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6986 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/in_memory_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/logger_destination.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22266 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/mlflow_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12239 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/mosaicml_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11579 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/neptune_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15255 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/progress_bar_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31771 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/remote_uploader_downloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9216 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/slack_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8541 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/tensorboard_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17395 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loggers/wandb_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.007074 composer-0.21.2/composer/loss/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11673 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loss/loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-03 21:25:51.000000 composer-0.21.2/composer/loss/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.007074 composer-0.21.2/composer/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-04-03 21:25:51.000000 composer-0.21.2/composer/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16757 2024-04-03 21:25:51.000000 composer-0.21.2/composer/metrics/map.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-04-03 21:25:51.000000 composer-0.21.2/composer/metrics/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38870 2024-04-03 21:25:51.000000 composer-0.21.2/composer/metrics/nlp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.011074 composer-0.21.2/composer/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-03 21:25:51.000000 composer-0.21.2/composer/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7301 2024-04-03 21:25:51.000000 composer-0.21.2/composer/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49464 2024-04-03 21:25:51.000000 composer-0.21.2/composer/models/huggingface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-03 21:25:51.000000 composer-0.21.2/composer/models/initializers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.011074 composer-0.21.2/composer/models/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-03 21:25:51.000000 composer-0.21.2/composer/models/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5593 2024-04-03 21:25:51.000000 composer-0.21.2/composer/models/tasks/classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.011074 composer-0.21.2/composer/optim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-03 21:25:51.000000 composer-0.21.2/composer/optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18605 2024-04-03 21:25:51.000000 composer-0.21.2/composer/optim/decoupled_weight_decay.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39120 2024-04-03 21:25:51.000000 composer-0.21.2/composer/optim/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.011074 composer-0.21.2/composer/profiler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-03 21:25:51.000000 composer-0.21.2/composer/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21003 2024-04-03 21:25:51.000000 composer-0.21.2/composer/profiler/json_trace_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6721 2024-04-03 21:25:51.000000 composer-0.21.2/composer/profiler/json_trace_merger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9088 2024-04-03 21:25:51.000000 composer-0.21.2/composer/profiler/marker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15160 2024-04-03 21:25:51.000000 composer-0.21.2/composer/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-03 21:25:51.000000 composer-0.21.2/composer/profiler/profiler_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-03 21:25:51.000000 composer-0.21.2/composer/profiler/profiler_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-04-03 21:25:51.000000 composer-0.21.2/composer/profiler/system_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18111 2024-04-03 21:25:51.000000 composer-0.21.2/composer/profiler/torch_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4046 2024-04-03 21:25:51.000000 composer-0.21.2/composer/profiler/trace_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-03 21:25:51.000000 composer-0.21.2/composer/profiler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 21:25:51.000000 composer-0.21.2/composer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.015074 composer-0.21.2/composer/trainer/
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-03 21:25:51.000000 composer-0.21.2/composer/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7635 2024-04-03 21:25:51.000000 composer-0.21.2/composer/trainer/_deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-03 21:25:51.000000 composer-0.21.2/composer/trainer/_scale_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6496 2024-04-03 21:25:51.000000 composer-0.21.2/composer/trainer/_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38951 2024-04-03 21:25:51.000000 composer-0.21.2/composer/trainer/dist_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4126 2024-04-03 21:25:51.000000 composer-0.21.2/composer/trainer/meta_safe_apply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-04-03 21:25:51.000000 composer-0.21.2/composer/trainer/mosaic_fsdp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51445 2024-04-03 21:25:51.000000 composer-0.21.2/composer/trainer/mosaic_fsdp_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)   182353 2024-04-03 21:25:51.000000 composer-0.21.2/composer/trainer/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.019074 composer-0.21.2/composer/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3995 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4266 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/auto_log_hparams.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/batch_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58034 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15301 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/collect_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4335 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/compression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26544 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/dist.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.019074 composer-0.21.2/composer/utils/eval_client/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/eval_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/eval_client/eval_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/eval_client/lambda_eval_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10985 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/eval_client/local_eval_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3758 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/eval_client/mosaicml_lambda_eval_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31422 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/file_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13356 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/fx_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2379 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/import_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16345 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4178 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/iter_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9878 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18833 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/module_surgery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.019074 composer-0.21.2/composer/utils/object_store/
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/object_store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9627 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/object_store/gcs_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8952 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/object_store/libcloud_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19428 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/object_store/mlflow_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6442 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/object_store/object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9103 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/object_store/oci_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8830 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/object_store/s3_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12224 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/object_store/sftp_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/object_store/uc_object_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8442 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/reproducibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/retrying.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/string_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-03 21:25:51.000000 composer-0.21.2/composer/utils/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:03.983074 composer-0.21.2/composer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20625 2024-04-03 21:26:03.000000 composer-0.21.2/composer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9788 2024-04-03 21:26:03.000000 composer-0.21.2/composer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 21:26:03.000000 composer-0.21.2/composer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-03 21:26:03.000000 composer-0.21.2/composer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2024-04-03 21:26:03.000000 composer-0.21.2/composer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-03 21:26:03.000000 composer-0.21.2/composer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    36090 2024-04-03 21:25:51.000000 composer-0.21.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 21:26:04.023074 composer-0.21.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8752 2024-04-03 21:25:51.000000 composer-0.21.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 21:26:04.023074 composer-0.21.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_docker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10391 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11868 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_full_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7146 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_loss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6928 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_notebooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5855 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_passes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_precision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_simple_nlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_smoketest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_split_batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8757 2024-04-03 21:25:51.000000 composer-0.21.2/tests/test_time.py
```

### Comparing `composer-0.21.1/LICENSE` & `composer-0.21.2/LICENSE`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/PKG-INFO` & `composer-0.21.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composer
-Version: 0.21.1
+Version: 0.21.2
 Summary: Composer is a PyTorch library that enables you to train neural networks faster, at lower cost, and to higher accuracy.
 Home-page: https://github.com/mosaicml/composer
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: composer Version: 0.21.1 Summary: Composer is a
+Metadata-Version: 2.1 Name: composer Version: 0.21.2 Summary: Composer is a
 PyTorch library that enables you to train neural networks faster, at lower
 cost, and to higher accuracy. Home-page: https://github.com/mosaicml/composer
 Author: MosaicML Author-email: team@mosaicml.com Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Python: >=3.9 Description-Content-Type:
 text/markdown Provides-Extra: base Provides-Extra: dev Provides-Extra:
```

### Comparing `composer-0.21.1/README.md` & `composer-0.21.2/README.md`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/__init__.py` & `composer-0.21.2/composer/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/__init__.py` & `composer-0.21.2/composer/algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/alibi/__init__.py` & `composer-0.21.2/composer/algorithms/alibi/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/alibi/alibi.py` & `composer-0.21.2/composer/algorithms/alibi/alibi.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/alibi/attention_surgery_functions/__init__.py` & `composer-0.21.2/composer/algorithms/alibi/attention_surgery_functions/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/alibi/attention_surgery_functions/_bert.py` & `composer-0.21.2/composer/algorithms/alibi/attention_surgery_functions/_bert.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/alibi/attention_surgery_functions/_gpt2.py` & `composer-0.21.2/composer/algorithms/alibi/attention_surgery_functions/_gpt2.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/alibi/attention_surgery_functions/utils.py` & `composer-0.21.2/composer/algorithms/alibi/attention_surgery_functions/utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/augmix/__init__.py` & `composer-0.21.2/composer/algorithms/augmix/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/augmix/augmix.py` & `composer-0.21.2/composer/algorithms/augmix/augmix.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/blurpool/__init__.py` & `composer-0.21.2/composer/algorithms/blurpool/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/blurpool/blurpool.py` & `composer-0.21.2/composer/algorithms/blurpool/blurpool.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/blurpool/blurpool_layers.py` & `composer-0.21.2/composer/algorithms/blurpool/blurpool_layers.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/channels_last/__init__.py` & `composer-0.21.2/composer/algorithms/channels_last/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/channels_last/channels_last.py` & `composer-0.21.2/composer/algorithms/channels_last/channels_last.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/colout/__init__.py` & `composer-0.21.2/composer/algorithms/colout/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/colout/colout.py` & `composer-0.21.2/composer/algorithms/colout/colout.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/cutmix/__init__.py` & `composer-0.21.2/composer/algorithms/cutmix/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/cutmix/cutmix.py` & `composer-0.21.2/composer/algorithms/cutmix/cutmix.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/cutout/cutout.py` & `composer-0.21.2/composer/algorithms/cutout/cutout.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/ema/ema.py` & `composer-0.21.2/composer/algorithms/ema/ema.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/factorize/__init__.py` & `composer-0.21.2/composer/algorithms/factorize/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/factorize/factorize.py` & `composer-0.21.2/composer/algorithms/factorize/factorize.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/factorize/factorize_core.py` & `composer-0.21.2/composer/algorithms/factorize/factorize_core.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/factorize/factorize_modules.py` & `composer-0.21.2/composer/algorithms/factorize/factorize_modules.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/gated_linear_units/__init__.py` & `composer-0.21.2/composer/algorithms/gated_linear_units/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/gated_linear_units/gated_linear_unit_layers.py` & `composer-0.21.2/composer/algorithms/gated_linear_units/gated_linear_unit_layers.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/gated_linear_units/gated_linear_units.py` & `composer-0.21.2/composer/algorithms/gated_linear_units/gated_linear_units.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/ghost_batchnorm/__init__.py` & `composer-0.21.2/composer/algorithms/ghost_batchnorm/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/ghost_batchnorm/ghost_batchnorm.py` & `composer-0.21.2/composer/algorithms/ghost_batchnorm/ghost_batchnorm.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/gradient_clipping/gradient_clipping.py` & `composer-0.21.2/composer/algorithms/gradient_clipping/gradient_clipping.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/gyro_dropout/gyro_dropout.py` & `composer-0.21.2/composer/algorithms/gyro_dropout/gyro_dropout.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/label_smoothing/__init__.py` & `composer-0.21.2/composer/algorithms/label_smoothing/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/label_smoothing/label_smoothing.py` & `composer-0.21.2/composer/algorithms/label_smoothing/label_smoothing.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/label_smoothing/metadata.json` & `composer-0.21.2/composer/algorithms/label_smoothing/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/layer_freezing/layer_freezing.py` & `composer-0.21.2/composer/algorithms/layer_freezing/layer_freezing.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/low_precision_groupnorm/__init__.py` & `composer-0.21.2/composer/algorithms/low_precision_groupnorm/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/low_precision_groupnorm/low_precision_groupnorm.py` & `composer-0.21.2/composer/algorithms/low_precision_groupnorm/low_precision_groupnorm.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/low_precision_layernorm/__init__.py` & `composer-0.21.2/composer/algorithms/low_precision_layernorm/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/low_precision_layernorm/low_precision_layernorm.py` & `composer-0.21.2/composer/algorithms/low_precision_layernorm/low_precision_layernorm.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/mixup/mixup.py` & `composer-0.21.2/composer/algorithms/mixup/mixup.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/no_op_model/__init__.py` & `composer-0.21.2/composer/algorithms/no_op_model/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/no_op_model/no_op_model.py` & `composer-0.21.2/composer/algorithms/no_op_model/no_op_model.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/progressive_resizing/__init__.py` & `composer-0.21.2/composer/algorithms/progressive_resizing/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/progressive_resizing/metadata.json` & `composer-0.21.2/composer/algorithms/progressive_resizing/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/progressive_resizing/progressive_resizing.py` & `composer-0.21.2/composer/algorithms/progressive_resizing/progressive_resizing.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/randaugment/metadata.json` & `composer-0.21.2/composer/algorithms/randaugment/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/randaugment/randaugment.py` & `composer-0.21.2/composer/algorithms/randaugment/randaugment.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/sam/__init__.py` & `composer-0.21.2/composer/algorithms/sam/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/sam/sam.py` & `composer-0.21.2/composer/algorithms/sam/sam.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/selective_backprop/__init__.py` & `composer-0.21.2/composer/algorithms/selective_backprop/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/selective_backprop/selective_backprop.py` & `composer-0.21.2/composer/algorithms/selective_backprop/selective_backprop.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/seq_length_warmup/seq_length_warmup.py` & `composer-0.21.2/composer/algorithms/seq_length_warmup/seq_length_warmup.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/squeeze_excite/__init__.py` & `composer-0.21.2/composer/algorithms/squeeze_excite/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/squeeze_excite/squeeze_excite.py` & `composer-0.21.2/composer/algorithms/squeeze_excite/squeeze_excite.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/stochastic_depth/__init__.py` & `composer-0.21.2/composer/algorithms/stochastic_depth/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/stochastic_depth/metadata.json` & `composer-0.21.2/composer/algorithms/stochastic_depth/metadata.json`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/stochastic_depth/stochastic_depth.py` & `composer-0.21.2/composer/algorithms/stochastic_depth/stochastic_depth.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/stochastic_depth/stochastic_layers.py` & `composer-0.21.2/composer/algorithms/stochastic_depth/stochastic_layers.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/swa/swa.py` & `composer-0.21.2/composer/algorithms/swa/swa.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/utils/augmentation_common.py` & `composer-0.21.2/composer/algorithms/utils/augmentation_common.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/utils/augmentation_primitives.py` & `composer-0.21.2/composer/algorithms/utils/augmentation_primitives.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/warnings.py` & `composer-0.21.2/composer/algorithms/warnings.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/algorithms/weight_standardization/weight_standardization.py` & `composer-0.21.2/composer/algorithms/weight_standardization/weight_standardization.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/callbacks/__init__.py` & `composer-0.21.2/composer/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/callbacks/activation_monitor.py` & `composer-0.21.2/composer/callbacks/activation_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/callbacks/checkpoint_saver.py` & `composer-0.21.2/composer/callbacks/checkpoint_saver.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/callbacks/early_stopper.py` & `composer-0.21.2/composer/callbacks/early_stopper.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/callbacks/eval_output_logging_callback.py` & `composer-0.21.2/composer/callbacks/eval_output_logging_callback.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/callbacks/export_for_inference.py` & `composer-0.21.2/composer/callbacks/export_for_inference.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/callbacks/generate.py` & `composer-0.21.2/composer/callbacks/generate.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/callbacks/image_visualizer.py` & `composer-0.21.2/composer/callbacks/image_visualizer.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/callbacks/lr_monitor.py` & `composer-0.21.2/composer/callbacks/lr_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/callbacks/memory_monitor.py` & `composer-0.21.2/composer/callbacks/memory_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/callbacks/memory_snapshot.py` & `composer-0.21.2/composer/callbacks/memory_snapshot.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/callbacks/mlperf.py` & `composer-0.21.2/composer/callbacks/mlperf.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/callbacks/nan_monitor.py` & `composer-0.21.2/composer/callbacks/nan_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/callbacks/oom_observer.py` & `composer-0.21.2/composer/callbacks/oom_observer.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/callbacks/optimizer_monitor.py` & `composer-0.21.2/composer/callbacks/optimizer_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/callbacks/runtime_estimator.py` & `composer-0.21.2/composer/callbacks/runtime_estimator.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/callbacks/speed_monitor.py` & `composer-0.21.2/composer/callbacks/speed_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/callbacks/system_metrics_monitor.py` & `composer-0.21.2/composer/callbacks/system_metrics_monitor.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/callbacks/threshold_stopper.py` & `composer-0.21.2/composer/callbacks/threshold_stopper.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/cli/launcher.py` & `composer-0.21.2/composer/cli/launcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -363,15 +363,15 @@
                     filename = format.format(
                         rank=global_rank,
                         world_size=world_size,
                         local_rank=local_rank,
                         local_world_size=nproc,
                         node_rank=node_rank,
                     )
-                    return open(filename, 'x+')
+                    return open(filename, 'a+')
 
                 stdout_file = _get_file(stdout_file_format)
                 stderr_file = _get_file(stderr_file_format) if stderr_file_format is not None else None
 
                 process = subprocess.Popen(
                     cmd,
                     stdout=stdout_file,
```

### Comparing `composer-0.21.1/composer/core/__init__.py` & `composer-0.21.2/composer/core/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/core/algorithm.py` & `composer-0.21.2/composer/core/algorithm.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/core/callback.py` & `composer-0.21.2/composer/core/callback.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/core/data_spec.py` & `composer-0.21.2/composer/core/data_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,23 +76,26 @@
         return False
     for item in l:
         if type(item) != first_type:
             return False
     return True
 
 
-def _default_split_batch(batch: Any, microbatch_size: int) -> Sequence:
+def _default_split_batch(batch: Any, microbatch_size: Union[int, float]) -> Sequence:
     """Splits batch into chunks of size `microbatch_size` for gradient accumulation.
 
     Works with tensors, dictionaries of tensors, (x, y) tuples, and lists where ``batch`` is the 2nd dimension.
 
     Args:
         batch (Any): output from the dataloader.
-        microbatch_size (int): Size of microbatches to batch into.
+        microbatch_size (int | float): Size of microbatches to batch into.
     """
+    if isinstance(microbatch_size, float):
+        raise ValueError('_default_split_batch does not support floating point microbatch_size.')
+
     if isinstance(batch, torch.Tensor):  # check for a single stack of tensors
         return _split_tensor(batch, microbatch_size)
     elif isinstance(batch, Mapping):  # check for dictionary (hf style)
         return _split_mapping(batch, microbatch_size)
     elif isinstance(batch, (Tuple, list)) and _check_list_is_primitives(batch):  # check for list of primitives
         return _split_list(batch, microbatch_size)
     elif isinstance(batch, (Tuple, List)):  # check for batch on 2nd dimension
@@ -150,15 +153,15 @@
             :class:`.Timestamp` (training progress tracker).
 
         device_transforms ((Batch) -> Batch, optional): Function called by the :class:`.Trainer` to modify the
             batch once it has been moved onto the device. For example, this function can be used for GPU-based
             normalization. It can modify the batch in-place, and it should return the modified batch. If not specified,
             the batch is not modified.
 
-        split_batch ((Batch, int) -> Sequence[Batch], optional): Function called by the :class:`.Trainer` to
+        split_batch ((Batch, (int | float)) -> Sequence[Batch], optional): Function called by the :class:`.Trainer` to
             split a batch (the first parameter) into microbatches of a given size (the second parameter). If
             the ``dataloader`` yields batches not of type :class:`torch.Tensor`, Mapping, Tuple, or List, then
             this function must be specified.
 
         get_num_samples_in_batch ((Batch) -> Union[int, float], optional): Function that is called by the :class:`.Trainer`
             to get the number of samples in the provided batch.
 
@@ -176,15 +179,15 @@
 
     def __init__(
         self,
         dataloader: Union[Iterable, torch.utils.data.DataLoader],
         num_samples: Optional[int] = None,
         num_tokens: Optional[int] = None,
         device_transforms: Optional[Callable[[Batch], Batch]] = None,
-        split_batch: Optional[Callable[[Batch, int], Sequence[Batch]]] = None,
+        split_batch: Optional[Callable[[Batch, Union[int, float]], Sequence[Batch]]] = None,
         get_num_samples_in_batch: Optional[Callable[[Batch], Union[int, float]]] = None,
         get_num_tokens_in_batch: Optional[Callable[[Batch], int]] = None,
     ) -> None:
         self.dataloader: Union[Iterable, torch.utils.data.DataLoader] = dataloader
         self.num_tokens = num_tokens
         self.device_transforms = self._default_device_transforms if device_transforms is None else device_transforms
         self.split_batch = default_split_batch if split_batch is None else split_batch
```

### Comparing `composer-0.21.1/composer/core/engine.py` & `composer-0.21.2/composer/core/engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,16 +119,19 @@
 # Catch SIGTERM/SIGINT and instead exit via `sys.exit` using same error code, ensuring atexit
 # functions still run. Composer CLI launcher will give a 30 second grace period before sending
 # SIGKILL.
 def sigterm_handler(signal, frame):
     sys.exit(128 + signal)
 
 
-signal.signal(signal.SIGTERM, sigterm_handler)
-signal.signal(signal.SIGINT, sigterm_handler)
+try:
+    signal.signal(signal.SIGTERM, sigterm_handler)
+    signal.signal(signal.SIGINT, sigterm_handler)
+except ValueError:
+    log.warning('Failed to set signal handler. Checkpoints may not be flushed if the process is killed.')
 
 
 def _get_default_passes():
     return [
         passes.sort_selective_backprop_first,
         passes.sort_low_precision_layernorm_last,
         passes.set_filo_order,
```

### Comparing `composer-0.21.1/composer/core/evaluator.py` & `composer-0.21.2/composer/core/evaluator.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/core/event.py` & `composer-0.21.2/composer/core/event.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/core/passes.py` & `composer-0.21.2/composer/core/passes.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/core/precision.py` & `composer-0.21.2/composer/core/precision.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/core/serializable.py` & `composer-0.21.2/composer/core/serializable.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/core/state.py` & `composer-0.21.2/composer/core/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,15 +214,15 @@
 
     Args:
         model (torch.nn.Module): The model, typically as a subclass of :class:`~.ComposerModel`.
         rank_zero_seed (int): The seed used on the rank zero process. It is assumed that each rank's seed is
             ``rank_zero_seed + dist.get_global_rank()``.
         run_name (str): The name for this training run.
         device (Device): The device used by this process. The trainer moves the model and loaded data to this device.
-        device_train_microbatch_size (int, optional): The microbatch size for each device during training.
+        device_train_microbatch_size (int | float, optional): The microbatch size for each device during training.
         auto_microbatching (bool, optional): Whether automatic microbatching is enabled.
         train_dataloader (Iterable, optional): Dataloader used for training
         evaluators (Evaluator | Evaluators, optional): :class:`.Evaluator` used for evaluation.
         dataloader (Iterable, optional): The active DataLoader.
         dataloader_len (int | Time[int], optional): The number of batches per dataloader iteration (e.g. epoch).
             The trainer will yield the first ``dataloader_len`` batches per iteration. If ``-1`` (the default),
             the entire dataloader will be iterated over.
@@ -304,15 +304,15 @@
             ... )
             >>> trainer.fit()
             >>> trainer.state.eval_metrics
             {'eval1': {'MulticlassAccuracy': MulticlassAccuracy()}, 'eval2': {'MulticlassAccuracy': MulticlassAccuracy()}}
         eval_timestamp (Timestamp): The timestamp for the current evaluation dataloader. This timestamp is reset
             before the dataloader is evaluated. The :attr:`~Timestamp.epoch` attribute for this timestamp is always
             ``0``.
-        device_train_microbatch_size (int): The size of each train microbatch per device.
+        device_train_microbatch_size (int | float): The size of each train microbatch per device.
         loss (torch.Tensor | Sequence[torch.Tensor] | Dict[Any, torch.Tensor]): The most recently computed loss.
         model (torch.nn.Module): The training model.
 
             .. note::
 
                 When using DeepSpeed or multi-rank training, the model will be wrapped with
                 :class:`~deepspeed.DeepSpeedEngine` or :class:`~torch.nn.parallel.DistributedDataParallel`,
@@ -377,15 +377,15 @@
         # device
         device: Device,
 
         # stopping conditions
         max_duration: Optional[Union[str, Time[int]]] = None,
 
         # data configurations
-        device_train_microbatch_size: Optional[int] = None,
+        device_train_microbatch_size: Optional[Union[int, float]] = None,
         auto_microbatching: bool = False,
 
         # dataloaders
         train_dataloader: Optional[Iterable] = None,
         evaluators: Optional[Union[Evaluator, Sequence[Evaluator]]] = None,
 
         # these track the current 'active' dataloader
```

### Comparing `composer-0.21.1/composer/core/time.py` & `composer-0.21.2/composer/core/time.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/core/types.py` & `composer-0.21.2/composer/core/types.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/datasets/__init__.py` & `composer-0.21.2/composer/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/datasets/in_context_learning_evaluation.py` & `composer-0.21.2/composer/datasets/in_context_learning_evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -626,25 +626,28 @@
             if 'continuation_indices' in data_pair:
                 batch['continuation_indices'].append(data_pair['continuation_indices'])
 
         batch = convert_tokens_to_tensors(batch, self.tokenize_labels)
         batch['attention_mask'] = ~(batch['input_ids'] == self.pad_tok_id)
         return batch
 
-    def split_batch(self, batch: Any, microbatch_size: int) -> List[Dict[str, Any]]:
+    def split_batch(self, batch: Any, microbatch_size: Union[int, float]) -> List[Dict[str, Any]]:
         """
         Handling for certain specialty columns that must be split into batches in different formats.
 
         Args:
             batch (Dict): Batch of data
-            microbatch_size (int): Size of microbatches
+            microbatch_size (int | float): Size of microbatches
 
         Returns:
             List: List of chunked batches
         """
+        if isinstance(microbatch_size, float):
+            raise ValueError('InContextLearningDataset does not support float microbatch sizes')
+
         # Don't split kwargs that don't change
         # Normally split torch tensors
         # List split lists of strings
         chunked = {}
         for k, v in batch.items():
             if k in self.static_keys:
                 # Defer broadcasting until we know num_chunks
@@ -1024,15 +1027,15 @@
         batch = convert_tokens_to_tensors(batch, self.tokenize_labels)
         batch['attention_mask'] = ~(batch['input_ids'] == self.pad_tok_id)
         return batch
 
     def get_num_samples_in_batch(self, batch) -> int:
         return batch['input_ids'].shape[0] // self.num_choices
 
-    def split_batch(self, batch: Any, microbatch_size: int) -> List[Dict[str, Any]]:
+    def split_batch(self, batch: Any, microbatch_size: Union[int, float]) -> List[Dict[str, Any]]:
         """
         Split batch while ensuring all continuations are in the same microbatch.
 
         In ICL Multiple Choice, we duplicate each data point for each possible continuation.
         When splitting a batch, we have logical example, which refer to one possible question,
         and real example, which refers to one possible continuation. As example count and
         microbatch_size are tracked in logical example, we split logical attributes by
@@ -1040,14 +1043,16 @@
         Args:
             batch (Dict): Batch of data
             microbatch_size (int): Size of microbatches
 
         Returns:
             list: List of chunked batches
         """
+        if isinstance(microbatch_size, float):
+            raise ValueError('InContextLearningMultipleChoiceTaskDataset does not support float microbatch sizes')
         chunked = {}
         for k, v in batch.items():
             if k in self.static_keys:
                 # Defer broadcasting primitives until we know num_chunks
                 pass
             elif type(v) == list:
                 # list of tensors - 'continuation_indices'
```

### Comparing `composer-0.21.1/composer/datasets/utils.py` & `composer-0.21.2/composer/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/devices/__init__.py` & `composer-0.21.2/composer/devices/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/devices/device.py` & `composer-0.21.2/composer/devices/device.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/devices/device_cpu.py` & `composer-0.21.2/composer/devices/device_cpu.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/devices/device_gpu.py` & `composer-0.21.2/composer/devices/device_gpu.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/devices/device_hpu.py` & `composer-0.21.2/composer/devices/device_hpu.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/devices/device_mps.py` & `composer-0.21.2/composer/devices/device_mps.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/devices/device_neuron.py` & `composer-0.21.2/composer/devices/device_neuron.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/devices/device_tpu.py` & `composer-0.21.2/composer/devices/device_tpu.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/functional/__init__.py` & `composer-0.21.2/composer/functional/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/loggers/__init__.py` & `composer-0.21.2/composer/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/loggers/cometml_logger.py` & `composer-0.21.2/composer/loggers/cometml_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/loggers/console_logger.py` & `composer-0.21.2/composer/loggers/console_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/loggers/file_logger.py` & `composer-0.21.2/composer/loggers/file_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/loggers/in_memory_logger.py` & `composer-0.21.2/composer/loggers/in_memory_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/loggers/logger.py` & `composer-0.21.2/composer/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/loggers/logger_destination.py` & `composer-0.21.2/composer/loggers/logger_destination.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/loggers/mlflow_logger.py` & `composer-0.21.2/composer/loggers/mlflow_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/loggers/mosaicml_logger.py` & `composer-0.21.2/composer/loggers/mosaicml_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/loggers/neptune_logger.py` & `composer-0.21.2/composer/loggers/neptune_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/loggers/progress_bar_logger.py` & `composer-0.21.2/composer/loggers/progress_bar_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/loggers/remote_uploader_downloader.py` & `composer-0.21.2/composer/loggers/remote_uploader_downloader.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/loggers/slack_logger.py` & `composer-0.21.2/composer/loggers/slack_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/loggers/tensorboard_logger.py` & `composer-0.21.2/composer/loggers/tensorboard_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/loggers/wandb_logger.py` & `composer-0.21.2/composer/loggers/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/loss/loss.py` & `composer-0.21.2/composer/loss/loss.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/loss/utils.py` & `composer-0.21.2/composer/loss/utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/metrics/__init__.py` & `composer-0.21.2/composer/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/metrics/map.py` & `composer-0.21.2/composer/metrics/map.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/metrics/metrics.py` & `composer-0.21.2/composer/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/metrics/nlp.py` & `composer-0.21.2/composer/metrics/nlp.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/models/__init__.py` & `composer-0.21.2/composer/models/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/models/base.py` & `composer-0.21.2/composer/models/base.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/models/huggingface.py` & `composer-0.21.2/composer/models/huggingface.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 import warnings
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, List, Mapping, Optional, Set, Tuple, Type, Union
 
 import torch
 from torchmetrics import Metric
 
+from composer.devices import DeviceCPU
 from composer.models.base import ComposerModel
 from composer.utils import MissingConditionalImportError, dist, get_file, import_object, is_model_fsdp, safe_torch_load
 from composer.utils.warnings import VersionedDeprecationWarning
 
 try:
     from peft import PeftModel, get_peft_model
     peft_installed = True
@@ -586,14 +587,17 @@
             metrics = self.train_metrics
         else:
             metrics = self.val_metrics
 
         return metrics if metrics else {}
 
     def update_metric(self, batch: Any, outputs: Any, metric: Metric) -> Dict:
+        if metric.device.type == 'cpu':
+            self.labels = DeviceCPU().batch_to_device(self.labels)
+
         if getattr(metric, 'needs_batch', False):
             metric_result = metric.update(batch=batch, outputs=outputs, labels=self.labels)
         else:
             metric_result = metric.update(outputs, self.labels)
         if metric_result is not None:
             # Add the metric name once for each datapoint in the batch
             metric_result['metric_name'] = [metric.__class__.__name__ for _ in range(0, batch['input_ids'].shape[0])]
```

### Comparing `composer-0.21.1/composer/models/initializers.py` & `composer-0.21.2/composer/models/initializers.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/models/tasks/classification.py` & `composer-0.21.2/composer/models/tasks/classification.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/optim/__init__.py` & `composer-0.21.2/composer/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/optim/decoupled_weight_decay.py` & `composer-0.21.2/composer/optim/decoupled_weight_decay.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/optim/scheduler.py` & `composer-0.21.2/composer/optim/scheduler.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/profiler/__init__.py` & `composer-0.21.2/composer/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/profiler/json_trace_handler.py` & `composer-0.21.2/composer/profiler/json_trace_handler.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/profiler/json_trace_merger.py` & `composer-0.21.2/composer/profiler/json_trace_merger.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/profiler/marker.py` & `composer-0.21.2/composer/profiler/marker.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/profiler/profiler.py` & `composer-0.21.2/composer/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/profiler/profiler_action.py` & `composer-0.21.2/composer/profiler/profiler_action.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/profiler/profiler_schedule.py` & `composer-0.21.2/composer/profiler/profiler_schedule.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/profiler/system_profiler.py` & `composer-0.21.2/composer/profiler/system_profiler.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/profiler/torch_profiler.py` & `composer-0.21.2/composer/profiler/torch_profiler.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/profiler/trace_handler.py` & `composer-0.21.2/composer/profiler/trace_handler.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/profiler/utils.py` & `composer-0.21.2/composer/profiler/utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/trainer/_deepspeed.py` & `composer-0.21.2/composer/trainer/_deepspeed.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/trainer/_scale_schedule.py` & `composer-0.21.2/composer/trainer/_scale_schedule.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/trainer/_scaler.py` & `composer-0.21.2/composer/trainer/_scaler.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/trainer/dist_strategy.py` & `composer-0.21.2/composer/trainer/dist_strategy.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/trainer/meta_safe_apply.py` & `composer-0.21.2/composer/trainer/meta_safe_apply.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/trainer/mosaic_fsdp.py` & `composer-0.21.2/composer/trainer/mosaic_fsdp.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,16 +57,16 @@
     elif version.parse(torch.__version__) < version.parse('2.2.1'):
         # Monkey patch for torch < 2.2.1 ie torch == 2.2.0
 
         # Allow 2D HSDP
         from torch.distributed.fsdp import _runtime_utils
         _runtime_utils._validate_and_get_hybrid_shard_state = lambda *args, **kwargs: None
 
-    elif version.parse(torch.__version__) < version.parse('2.2.2'):
-        # Monkey patch for torch < 2.2.2 ie torch == 2.2.1
+    elif version.parse(torch.__version__) < version.parse('2.2.9'):
+        # Monkey patch for torch < 2.3.0 ie torch == 2.2.1/2.2.2 currently
         pass
 
     elif version.parse(torch.__version__) < version.parse('2.3.1'):
         # Monkey patch for torch < 2.3.1 ie torch == 2.3.0
         # Note: this is the same patch as 2.2.0, we are just making a new if branch
         # for clarity and modularity of changes.
```

### Comparing `composer-0.21.1/composer/trainer/mosaic_fsdp_utils.py` & `composer-0.21.2/composer/trainer/mosaic_fsdp_utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/trainer/trainer.py` & `composer-0.21.2/composer/trainer/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -236,15 +236,15 @@
                 raise ValueError(
                     'eval_subset_num_batches must be set when using an infinite sized '
                     'eval_dataloader where length is `None`. Otherwise, evaluation will '
                     'run forever and never terminate.',
                 )
 
 
-def _is_auto_microbatching(device_train_microbatch_size: Optional[Union[int, str]], device: Device):
+def _is_auto_microbatching(device_train_microbatch_size: Optional[Union[int, float, str]], device: Device):
     if device_train_microbatch_size == 'auto':
         warnings.warn((
             "`device_train_microbatch_size='auto'` may potentially fail with unexpected "
             'CUDA errors. Auto microbatching attempts to catch CUDA Out of Memory errors '
             'and adjust the batch size, but it is possible CUDA will be put into an '
             'irrecoverable state due to PyTorch bugs, e.g. integer overflow. In this case, '
             'please manually set device_train_microbatch_size explicitly to an integer '
@@ -256,18 +256,18 @@
             )
         return True
     else:
         return False
 
 
 def _get_initial_device_train_microbatch_size(
-    device_train_microbatch_size: Optional[Union[int, str]],
+    device_train_microbatch_size: Optional[Union[int, float, str]],
     auto_microbatching: bool,
     train_dataloader: Optional[Iterable],
-) -> Optional[int]:
+) -> Optional[Union[int, float]]:
     """Sets initial value of device_train_microbatch_size.
 
     If auto_microbatching, sets initial `device_train_microbatch_size` to per rank batch size. If
     `train_dataloader` is not set yet, returns None and this function will be called again when
     `train_dataloader` is set, such as when `fit()` is called.
     """
     if device_train_microbatch_size is None or auto_microbatching:
@@ -402,18 +402,18 @@
             'Can only use adaptive device_eval_microbatch_size on GPU. Please set device_eval_microbatch_size >= 1.',
         )
     if evaluator.auto_microbatching and hasattr(evaluator.dataloader, 'seq_parallel_world_size'):
         raise ValueError(
             'Auto microbatching on evaluators is not compatible with sequence parallelism. '
             'Please manually set device_eval_microbatch_size or disable sequence parallelism .',
         )
-    if isinstance(evaluator.dataloader.get_num_samples_in_batch, int) and hasattr(
+    if hasattr(
         evaluator.dataloader,
         'seq_parallel_world_size',
-    ) and evaluator.dataloader.get_num_samples_in_batch * evaluator.dataloader.seq_parallel_world_size != 1:  # type: ignore
+    ) and evaluator.dataloader.seq_parallel_world_size > 1 and evaluator.dataloader.batch_size * evaluator.dataloader.seq_parallel_world_size != 1:  # type: ignore
         raise ValueError(
             'Sequence parallelism requires a microbatch size of 1 distributed over the sequence parallel group.',
         )
 
 
 def _distribute_and_get_random_seed(seed: Optional[int], device: Device):
     if seed is None:
@@ -461,14 +461,23 @@
     run_name_list = [generated_run_name]
     # ensure all ranks have the same experiment name
     dist.broadcast_object_list(run_name_list)
     generated_run_name = run_name_list[0]
     return generated_run_name
 
 
+def _get_distributed_sampler(dataloader: DataLoader) -> Optional[DistributedSampler]:
+    """Fetch a distributed sampler from a `dataloader` if it exists."""
+    if isinstance(dataloader.batch_sampler, DistributedSampler):
+        return dataloader.batch_sampler
+    if isinstance(dataloader.sampler, DistributedSampler):
+        return dataloader.sampler
+    return None
+
+
 class Trainer:
     """Train models with Composer algorithms.
 
     The trainer supports models with :class:`~composer.models.base.ComposerModel` instances.
     The :class:`.Trainer` is highly customizable and can support a wide variety of workloads.
     See the :doc:`training guide</trainer/using_the_trainer>` for more information.
 
@@ -900,15 +909,15 @@
 
             The default behavior sets the device to ``'gpu'`` if CUDA is available, and otherwise ``'cpu'``.
         precision (Precision | str, optional): Numerical precision to use for training. One of ``fp32``, ``amp_bf16``
             or ``amp_fp16`` (recommended). (default: ``Precision.FP32`` if training on CPU; ``Precision.AMP_FP16`` if
             training on GPU)
         precision_config (Optional[Dict[str, Any]]): The config for FP8 scaling strategy. See parameters for
             `DelayedScaling <https://docs.nvidia.com/deeplearning/transformer-engine/user-guide/api/common.html?highlight=delayedscaling#transformer_engine.common.recipe.DelayedScaling>`_.
-        device_train_microbatch_size (Union[int, str), optional): The number of samples to process on each device per
+        device_train_microbatch_size (Union[int, float, str), optional): The number of samples to process on each device per
             microbatch during training. Gradients are summed over the microbatches per device. If set to ``auto``,
             dynamically decreases device_train_microbatch_size if microbatch is too large for GPU. (default: ``None``)
 
             .. note:: This is implemented by taking the batch yielded by the ``train_dataloader`` and splitting
                 it into sections of size ``device_train_microbatch_size``. If the batch size of the dataloader
                 is not divisible by ``device_train_microbatch_size``, the last section will be potentially smaller.
         seed (int, optional): The seed used in randomization. If ``None``, then a random seed
@@ -1039,15 +1048,15 @@
         fsdp_config: Optional[Dict[str, Any]] = None,
         fsdp_auto_wrap: bool = True,
 
         # System/Numerics
         device: Optional[Union[str, Device]] = None,
         precision: Optional[Union[str, Precision]] = None,
         precision_config: Optional[Dict[str, Any]] = None,
-        device_train_microbatch_size: Optional[Union[int, str]] = None,
+        device_train_microbatch_size: Optional[Union[int, float, str]] = None,
 
         # Reproducibility
         seed: Optional[int] = None,
         deterministic_mode: bool = False,
 
         # Distributed Training
         dist_timeout: float = 300.0,
@@ -1110,18 +1119,18 @@
             compiled_model.forward = model.dynamo_ctx(compiled_model.forward)
             model = compiled_model
 
         # Microbatching
         auto_microbatching = _is_auto_microbatching(device_train_microbatch_size, device=device)
         if auto_microbatching and train_dataloader is not None and hasattr(train_dataloader, 'seq_parallel_world_size'):
             raise ValueError('`device_train_microbatch_size="auto"` is not compatible with sequence parallelism.')
-        if isinstance(device_train_microbatch_size, int) and train_dataloader is not None and hasattr(
+        if train_dataloader is not None and hasattr(
             train_dataloader,
             'seq_parallel_world_size',
-        ) and device_train_microbatch_size * train_dataloader.seq_parallel_world_size != 1:  # type: ignore
+        ) and train_dataloader.seq_parallel_world_size > 1 and device_train_microbatch_size * train_dataloader.seq_parallel_world_size != 1:  # type: ignore
             raise ValueError(
                 '`Sequence parallelism requires a microbatch size of 1 distributed over the sequence parallel group.',
             )
 
         if auto_microbatching and profiler:
             raise ValueError(
                 "`device_train_microbatch_size='auto'` is not compatible with the profiler. It is "
@@ -1904,15 +1913,15 @@
 
         # Evaluation
         eval_dataloader: Optional[Union[Iterable, DataSpec, Evaluator, Sequence[Evaluator]]] = None,
         eval_subset_num_batches: int = -1,
         eval_interval: Union[int, str, Time, Callable[[State, Event], bool]] = 1,
 
         # Numerics
-        device_train_microbatch_size: Optional[Union[int, str]] = None,
+        device_train_microbatch_size: Optional[Union[int, float, str]] = None,
         precision: Optional[Union[str, Precision]] = None,
     ):
         """Train the model.
 
         The Composer :class:`.Trainer` supports multiple calls to :meth:`.fit`. Any arguments specified during
         the call to :meth:`.fit` will override the values specified when constructing the :class:`.Trainer`.
         All arguments are optional, with the following exceptions:
@@ -2013,15 +2022,15 @@
             optimizers (torch.optim.Optimizer | Sequence[torch.optim.Optimizer], optional): See :class:`.Trainer`.
             schedulers (LRScheduler | ComposerScheduler | Sequence[LRScheduler | ComposerScheduler], optional): See :class:`.Trainer`.
             scale_schedule_ratio (float, optional): See :class:`.Trainer`.
             step_schedulers_every_batch (bool, optional): See :class:`.Trainer`.
             eval_dataloader (Iterable | DataSpec | Evaluator | Sequence[Evaluator], optional): See :class:`.Trainer`.
             eval_subset_num_batches (int, optional): See :class:`.Trainer`.
             eval_interval (int | str | Time | (State, Event) -> bool, optional): See :class:`.Trainer`.
-            device_train_microbatch_size (int | str, optional): See :class:`.Trainer`.
+            device_train_microbatch_size (int | float | str, optional): See :class:`.Trainer`.
             precision (Precision | str, optional): See :class:`.Trainer`.
         """
         # Check Optimizer
         if len(self.state.optimizers) == 0:
             raise ValueError(
                 f'No optimizer was specified when constructing the Trainer. As the '
                 'model had no parameters, SGD was not created by default. This trainer '
@@ -2157,18 +2166,18 @@
                 device=self.state.device,
             )
             if self.state.auto_microbatching and self._train_data_spec is not None and hasattr(
                 self._train_data_spec,
                 'seq_parallel_world_size',
             ):
                 raise ValueError('`device_train_microbatch_size="auto"` is not compatible with sequence parallelism.')
-            if isinstance(device_train_microbatch_size, int) and train_dataloader is not None and hasattr(
+            if train_dataloader is not None and hasattr(
                 train_dataloader,
                 'seq_parallel_world_size',
-            ) and device_train_microbatch_size * train_dataloader.seq_parallel_world_size != 1:  # type: ignore
+            ) and train_dataloader.seq_parallel_world_size > 1 and device_train_microbatch_size * train_dataloader.seq_parallel_world_size != 1:  # type: ignore
                 raise ValueError(
                     '`Sequence parallelism requires a microbatch size of 1 distributed over the sequence parallel group.',
                 )
             if self.state.auto_microbatching and self.state.profiler:
                 raise ValueError(
                     "`device_train_microbatch_size='auto'` is not compatible with the profiler. It is "
                     "recommended to run a mini-run with `device_train_microbatch_size='auto'` to identify "
@@ -2200,20 +2209,29 @@
         """Shutdown the trainer.
 
         .. seealso:: :meth:`.Engine.close` for additional information.
         """
         self.engine.close()
         dist.barrier()
 
-    def _ensure_metrics_device_and_dtype(self, metrics: Dict[str, Metric]):
+    def _ensure_metrics_device_and_dtype(
+        self,
+        metrics: Dict[str, Metric],
+        ensure_cpu: bool = False,
+    ):
         for name, metric in metrics.items():
             # Safety check to ensure the metric and data are on the same device. Normally not
             # needed because the metric is automatically on the same device as the model.
             # See https://torchmetrics.readthedocs.io/en/latest/pages/overview.html for details.
-            metrics[name] = self.state.device.module_to_device(metric)
+
+            # Force all metrics to go on the CPU
+            if ensure_cpu:
+                metrics[name] = DeviceCPU().module_to_device(metric)
+            else:
+                metrics[name] = self.state.device.module_to_device(metric)
             if is_model_deepspeed(self.state.model):
                 # HACK: DeepSpeed somehow manages to convert metric internal states to its own dtype. When
                 # running with FP16, this tends to result in overflows. Let's assume FP32 is good enough.
                 for key in metric._defaults:
                     metric_data = getattr(metric, key)
                     if isinstance(metric_data, torch.Tensor) and metric_data.dtype == torch.float16:
                         metric_data = metric_data.to(torch.float32)  # type: ignore
@@ -2254,32 +2272,34 @@
         """Spin the dataloaders to restore sampler state for current epoch.
 
         Only one batch must be loaded to seed the sampler's generator. since only the first batch is being loaded, the
         dataloader may not be completely iterated through.
         """
         log.debug('Spinning the dataloaders')
 
-        # spin the evaluator dataloaders once to initialize its sampler deterministically
+        # Spin the evaluator dataloaders once to initialize its sampler deterministically
         # so it does not affect any other RNG reads
         eval_state = self.state.dataset_resumption.get('eval', {})
         for evaluator in self.state.evaluators:
             dataloader = evaluator.dataloader.dataloader
-            if isinstance(dataloader, DataLoader) and isinstance(dataloader.sampler, DistributedSampler):
-                dataloader.sampler.set_epoch(0)
+            sampler = _get_distributed_sampler(dataloader) if isinstance(dataloader, DataLoader) else None
+            if isinstance(sampler, DistributedSampler):
+                sampler.set_epoch(0)
             if evaluator.label not in eval_state:
                 for _ in dataloader:
                     break
 
-        # spin the train dataloader's sampler to get to the state of the desired epoch
+        # Spin the train dataloader's sampler to get to the state of the desired epoch
         dataloader = self.state.dataloader
         assert dataloader is not None, 'train dataloader is set on state after FIT_START'
         if 'train' not in self.state.dataset_resumption:
+            sampler = _get_distributed_sampler(dataloader) if isinstance(dataloader, DataLoader) else None
             for epoch in range(int(self.state.timestamp.epoch)):
-                if isinstance(dataloader, DataLoader) and isinstance(dataloader.sampler, DistributedSampler):
-                    dataloader.sampler.set_epoch(epoch)
+                if isinstance(sampler, DistributedSampler):
+                    sampler.set_epoch(epoch)
                 for _ in dataloader:
                     break
 
     def _accumulate_time_across_ranks(
         self,
         num_samples: Union[int, float],
         num_tokens: int,
@@ -2299,15 +2319,15 @@
             )
         else:
             sample_token_tensor = self.state.device.tensor_to_device(
                 torch.tensor([num_samples, num_tokens], dtype=torch.int),
             )
         dist.all_reduce(sample_token_tensor, reduce_operation='SUM')
         if isinstance(num_samples, float):
-            sample_token_tensor_int = sample_token_tensor.to(torch.int)
+            sample_token_tensor_int = sample_token_tensor.round().to(torch.int)
             if torch.any(torch.abs(sample_token_tensor_int - sample_token_tensor) > 1e-4):
                 raise ValueError('The sums of samples and tokens across ranks should each be integers.')
             sample_token_tensor = sample_token_tensor_int
         batch_time_tensor = self.state.device.tensor_to_device(
             torch.tensor([batch_time.total_seconds()], dtype=torch.float32),
         )
         dist.broadcast(batch_time_tensor, src=0)
@@ -2353,16 +2373,17 @@
                 self.engine.run_event(Event.ITERATION_START)
 
             if int(self.state.timestamp.batch_in_epoch) == 0:
                 self.engine.run_event(Event.EPOCH_START)
                 self.logger.log_metrics({'time/epoch': self.state.timestamp.epoch.value})
 
             dataloader = self.state.dataloader
-            if isinstance(dataloader, DataLoader) and isinstance(dataloader.sampler, DistributedSampler):
-                dataloader.sampler.set_epoch(int(self.state.timestamp.epoch))
+            sampler = _get_distributed_sampler(dataloader) if isinstance(dataloader, DataLoader) else None
+            if isinstance(sampler, DistributedSampler):
+                sampler.set_epoch(int(self.state.timestamp.epoch))
 
             for batch_idx, self.state.batch in enumerate(self._iter_dataloader(TrainerMode.TRAIN)):
                 # Spin dataloader forward unless dataloader handles internally with dataset_resumption
                 if self.spin_dataloaders and 'train' not in self.state.dataset_resumption and batch_idx < int(
                     self.state.timestamp.batch_in_epoch,
                 ):
                     # Restore the RNG state immediately before the next batch is yielded from the dataloader
@@ -3198,30 +3219,33 @@
 
         with torch.no_grad(), model_eval_mode(self.state.model):
             self.state.set_dataloader(data_spec.dataloader, evaluator.label, subset_num_batches)
             assert self.state.dataloader is not None, 'dataloader is set'
 
             self.engine.run_event(Event.EVAL_START)
 
-            metrics = self._ensure_metrics_device_and_dtype(metrics)
+            # On MPS device we ensure the eval metrics are computed on CPU to avoid numerical errors
+            metrics = self._ensure_metrics_device_and_dtype(
+                metrics,
+                ensure_cpu=isinstance(self.state.device, DeviceMPS),
+            )
 
             for metric in metrics.values():
                 metric.reset()
 
             dataloader = self.state.dataloader
-            dist_sampler = None
             drop_last = None
             dataset_len = None
             last_batch = False
-            if isinstance(dataloader, DataLoader) and isinstance(dataloader.sampler, DistributedSampler):
+            dist_sampler = _get_distributed_sampler(dataloader) if isinstance(dataloader, DataLoader) else None
+            if isinstance(dist_sampler, DistributedSampler) and isinstance(dataloader, DataLoader):
                 # The distributed sampler uses `set_epoch` to set the random seed
                 # Because evaluation can run on each batch, we use the batch to seed the sampler
                 # so each evaluation will get a proper shuffle.
                 # The epoch provided to `set_epoch` need not be sequential, so this is fine.
-                dist_sampler = dataloader.sampler
                 dist_sampler.set_epoch(int(self.state.timestamp.batch))
                 drop_last = dataloader.drop_last
                 # Only compute the dataset length if drop_last is False, as otherwise we don't need
                 # to remove any duplicate samples.
                 if drop_last == False:
                     try:
                         dataset_len = len(dist_sampler.dataset)  # type: ignore
@@ -3323,20 +3347,22 @@
                                         for v in self.state.outputs:
                                             if isinstance(v, torch.Tensor):
                                                 outputs.append(v.cpu())
                                             else:
                                                 outputs.append(v)
                                     else:
                                         outputs = self.state.outputs.cpu()
+                                    batch = DeviceCPU().batch_to_device(self.state.batch,)
                                 else:
                                     outputs = self.state.outputs
+                                    batch = self.state.batch
 
                                 for metric in metrics.values():
                                     metric_outputs = self._original_model.update_metric(
-                                        self.state.batch,
+                                        batch,
                                         outputs,
                                         metric,
                                     )
                                     self.state.metric_outputs = metric_outputs or {}
 
                     except RuntimeError as e:
                         if evaluator.auto_microbatching and _is_cuda_oom(e):
```

### Comparing `composer-0.21.1/composer/utils/__init__.py` & `composer-0.21.2/composer/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/utils/auto_log_hparams.py` & `composer-0.21.2/composer/utils/auto_log_hparams.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/utils/batch_helpers.py` & `composer-0.21.2/composer/utils/batch_helpers.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/utils/checkpoint.py` & `composer-0.21.2/composer/utils/checkpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     format_name_with_dist_and_time,
     get_file,
     is_tar,
     parse_uri,
 )
 from composer.utils.misc import is_model_deepspeed, partial_format
 from composer.utils.object_store import ObjectStore
+from composer.utils.retrying import retry
 
 if TYPE_CHECKING:
     from composer.core import AlgorithmPass, State
     from composer.loggers import Logger, LoggerDestination
 
 log = logging.getLogger(__name__)
 
@@ -184,14 +185,32 @@
             ValueError if the metadata file is invalid.
         """
         metadata_file_path = self.path / '.metadata'
         _ensure_valid_checkpoint(metadata_file_path)
         return super().read_metadata()
 
 
+@retry(num_attempts=5)
+def download_object_or_file(
+    object_name: str,
+    file_destination: Union[str, Path],
+    object_store: Union[ObjectStore, LoggerDestination],
+):
+    if isinstance(object_store, ObjectStore):
+        object_store.download_object(
+            object_name=object_name,
+            filename=file_destination,
+        )
+    else:
+        object_store.download_file(
+            remote_file_name=object_name,
+            destination=str(file_destination),
+        )
+
+
 # A subclass of FileSystemReaderWithValidation that downloads files from the object store before reading them from the local filesystem.
 class DistCPObjectStoreReader(FileSystemReaderWithValidation):
 
     def __init__(
         self,
         source_path: str,
         destination_path: str,
@@ -204,24 +223,15 @@
         self.device_mesh = device_mesh
 
         # Download metadata file.
         Path(self.destination_path).mkdir(parents=True, exist_ok=True)
         metadata_destination = os.path.join(self.destination_path, '.metadata')
         if dist.get_local_rank() == 0:
             metadata_path = str(Path(source_path) / Path('.metadata'))
-            if isinstance(object_store, ObjectStore):
-                object_store.download_object(
-                    object_name=metadata_path,
-                    filename=metadata_destination,
-                )
-            else:
-                object_store.download_file(
-                    remote_file_name=metadata_path,
-                    destination=metadata_destination,
-                )
+            download_object_or_file(metadata_path, metadata_destination, object_store)
         dist.barrier()
 
         # FileSystemReader takes in a root directory in its constructor, which is the dir where
         # the metadata is expected to be stored. Also, this is parent directory for any shard file relative paths
         # specified in the metadata file.
         super().__init__(destination_path)
 
@@ -240,42 +250,41 @@
         # 2. Download to the destination all files this rank needs if on first replica
         if first_replica:
             log.debug(f'Rank {dist.get_global_rank()} starting to download files.')
 
             # Get the lowest rank in the current node
             local_rank_0 = dist.get_global_rank() - dist.get_local_rank()
 
-            for plan_item in plan.items:
-                relative_file_path = self.storage_data[plan_item.storage_index].relative_path
-                # Check if the file is scheduled to be downloaded by a lower rank on the same node
-                # i.e. if rank 0 and rank 1 on the same node have the same the same required file,
-                # only rank 0 should download it and not rank 1.
-                is_downloaded = any(
-                    relative_file_path in all_file_paths[i] for i in range(local_rank_0, dist.get_global_rank())
-                )
-
-                # Download the shard file to the relative path it's associated to and save that relative path
-                # to the root directory specified to the FileSystem reader constructor.
-                file_destination = str(Path(self.destination_path) / Path(relative_file_path))
-
-                # The file could have already been downloaded as different plan items can point to same file.
-                if not is_downloaded and not os.path.exists(file_destination):
-                    log.debug(f'Downloading {relative_file_path} to {file_destination}.')
-                    object_name = str(Path(self.source_path) / Path(relative_file_path))
-                    if isinstance(self.object_store, ObjectStore):
-                        self.object_store.download_object(
-                            object_name=object_name,
-                            filename=file_destination,
-                        )
-                    else:
-                        self.object_store.download_file(
-                            remote_file_name=object_name,
-                            destination=file_destination,
-                        )
-                    log.debug(f'Finished downloading {relative_file_path} to {file_destination}.')
+            try:
+                for plan_item in plan.items:
+                    relative_file_path = self.storage_data[plan_item.storage_index].relative_path
+                    # Check if the file is scheduled to be downloaded by a lower rank on the same node
+                    # i.e. if rank 0 and rank 1 on the same node have the same the same required file,
+                    # only rank 0 should download it and not rank 1.
+                    is_downloaded = any(
+                        relative_file_path in all_file_paths[i] for i in range(local_rank_0, dist.get_global_rank())
+                    )
+
+                    # Download the shard file to the relative path it's associated to and save that relative path
+                    # to the root directory specified to the FileSystem reader constructor.
+                    file_destination = str(Path(self.destination_path) / Path(relative_file_path))
+
+                    # The file could have already been downloaded as different plan items can point to same file.
+                    if not is_downloaded and not os.path.exists(file_destination):
+                        log.debug(f'Downloading {relative_file_path} to {file_destination}.')
+                        object_name = str(Path(self.source_path) / Path(relative_file_path))
+                        download_object_or_file(object_name, file_destination, self.object_store)
+                        log.debug(f'Finished downloading {relative_file_path} to {file_destination}.')
+            except Exception as e:
+                # PyTorch will capture any exception of this function,
+                # and dist.all_gather_objects(exception) before raising it.
+                # If that all_gather_objects fails, the exception is never visible to user.
+                # We immediately print the exception to avoid that situation.
+                log.error(f'Exception {type(e)} raised during downloading: {str(e)}')
+                raise e
 
         # 3. Wait for all ranks to finish.
         log.debug(f'Rank {dist.get_global_rank()} finished downloading all files.')
         dist.barrier()
         log.debug('Done waiting for all ranks to finish downloading files.')
 
         # 4. Broadcast files to all other replicas if HSDP
@@ -363,24 +372,15 @@
     if object_store is None:
         return not os.path.exists(metadata_path)
     else:
         try:
             _, _, metadata_path = parse_uri(metadata_path)
             with tempfile.TemporaryDirectory() as temp_dir:
                 metadata_destination = os.path.join(str(temp_dir), '.metadata')
-                if isinstance(object_store, ObjectStore):
-                    object_store.download_object(
-                        object_name=metadata_path,
-                        filename=metadata_destination,
-                    )
-                else:
-                    object_store.download_file(
-                        remote_file_name=metadata_path,
-                        destination=metadata_destination,
-                    )
+                download_object_or_file(metadata_path, metadata_destination, object_store)
             return False
         except FileNotFoundError:
             return True
 
 
 def load_checkpoint(
     path: str,
```

### Comparing `composer-0.21.1/composer/utils/collect_env.py` & `composer-0.21.2/composer/utils/collect_env.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/utils/device.py` & `composer-0.21.2/composer/utils/device.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/utils/dist.py` & `composer-0.21.2/composer/utils/dist.py`

 * *Files 1% similar despite different names*

```diff
@@ -575,15 +575,22 @@
         # Fill in the remaining single-rank variables
         os.environ.update(dist_env_var_defaults)
         dist.init_process_group(device_obj.dist_backend, store=dist.HashStore(), world_size=1, rank=0)
     else:
         dist.init_process_group(device_obj.dist_backend, timeout=timeout_timedelta)
 
 
-def get_sampler(dataset: torch.utils.data.Dataset, *, drop_last: bool = False, shuffle: bool = False):
+def get_sampler(
+    dataset: torch.utils.data.Dataset,
+    *,
+    drop_last: bool = False,
+    shuffle: bool = False,
+    num_replicas: Optional[int] = None,
+    rank: Optional[int] = None,
+):
     """Constructs a :class:`~torch.utils.data.distributed.DistributedSampler` for a dataset.
 
     The :class:`~torch.utils.data.distributed.DistributedSampler` assumes that each rank has a complete copy of the
     dataset. It ensures that each rank sees a unique shard for each epoch containing
     ``len(dataset) / get_world_size()`` samples.
 
     .. note::
@@ -591,24 +598,26 @@
         If the ``dataset`` is already sharded by rank, use a :class:`~torch.utils.data.SequentialSampler`
         or :class:`~torch.utils.data.RandomSampler`.
 
     Args:
         dataset (torch.utils.data.Dataset): The dataset.
         drop_last (bool): Whether to trop the last batch.
         shuffle (bool): Whether to shuffle the dataset.
+        num_replicas (int, optional): The number of replicas. If ``None``, defaults to the world size.
+        rank (int, optional): The rank. If ``None``, defaults to the global rank.
 
     Returns:
         torch.utils.data.distributed.DistributedSampler: The sampler.
     """
     return torch.utils.data.DistributedSampler[int](
         dataset,
         drop_last=drop_last,
         shuffle=shuffle,
-        num_replicas=get_world_size(),
-        rank=get_global_rank(),
+        num_replicas=get_world_size() if num_replicas is None else num_replicas,
+        rank=get_global_rank() if rank is None else rank,
     )
 
 
 @contextmanager
 def local_rank_zero_download_and_wait(expected_file_path: str):
     """Context manager to wait for a file to exist on all ranks except local rank zero.
```

### Comparing `composer-0.21.1/composer/utils/eval_client/__init__.py` & `composer-0.21.2/composer/utils/eval_client/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/utils/eval_client/eval_client.py` & `composer-0.21.2/composer/utils/eval_client/eval_client.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/utils/eval_client/lambda_eval_client.py` & `composer-0.21.2/composer/utils/eval_client/lambda_eval_client.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/utils/eval_client/local_eval_client.py` & `composer-0.21.2/composer/utils/eval_client/local_eval_client.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/utils/eval_client/mosaicml_lambda_eval_client.py` & `composer-0.21.2/composer/utils/eval_client/mosaicml_lambda_eval_client.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/utils/file_helpers.py` & `composer-0.21.2/composer/utils/file_helpers.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/utils/fx_utils.py` & `composer-0.21.2/composer/utils/fx_utils.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/utils/import_helpers.py` & `composer-0.21.2/composer/utils/import_helpers.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/utils/inference.py` & `composer-0.21.2/composer/utils/inference.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/utils/iter_helpers.py` & `composer-0.21.2/composer/utils/iter_helpers.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/utils/misc.py` & `composer-0.21.2/composer/utils/misc.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/utils/module_surgery.py` & `composer-0.21.2/composer/utils/module_surgery.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/utils/object_store/__init__.py` & `composer-0.21.2/composer/utils/object_store/__init__.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/utils/object_store/gcs_object_store.py` & `composer-0.21.2/composer/utils/object_store/gcs_object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/utils/object_store/libcloud_object_store.py` & `composer-0.21.2/composer/utils/object_store/libcloud_object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/utils/object_store/mlflow_object_store.py` & `composer-0.21.2/composer/utils/object_store/mlflow_object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/utils/object_store/object_store.py` & `composer-0.21.2/composer/utils/object_store/object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/utils/object_store/oci_object_store.py` & `composer-0.21.2/composer/utils/object_store/oci_object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/utils/object_store/s3_object_store.py` & `composer-0.21.2/composer/utils/object_store/s3_object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/utils/object_store/sftp_object_store.py` & `composer-0.21.2/composer/utils/object_store/sftp_object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/utils/object_store/uc_object_store.py` & `composer-0.21.2/composer/utils/object_store/uc_object_store.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/utils/reproducibility.py` & `composer-0.21.2/composer/utils/reproducibility.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/utils/retrying.py` & `composer-0.21.2/composer/utils/retrying.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,22 +3,25 @@
 
 """Retry helper."""
 
 from __future__ import annotations
 
 import collections.abc
 import functools
+import logging
 import random
 import time
 from typing import Any, Callable, Sequence, Type, TypeVar, Union, cast, overload
 
 TCallable = TypeVar('TCallable', bound=Callable)
 
 __all__ = ['retry']
 
+log = logging.getLogger(__name__)
+
 
 @overload
 def retry(
     exc_class: Union[Type[Exception], Sequence[Type[Exception]]] = ...,
     num_attempts: int = ...,
     initial_backoff: float = ...,
     max_jitter: float = ...,
@@ -82,14 +85,15 @@
         @functools.wraps(func)
         def new_func(*args: Any, **kwargs: Any):
             i = 0
             while True:
                 try:
                     return func(*args, **kwargs)
                 except exc_class as e:
+                    log.debug(f'Attempt {i} failed. Exception type: {type(e)}, message: {str(e)}.')
                     if i + 1 == num_attempts:
                         raise e
                     else:
                         time.sleep(initial_backoff * 2**i + random.random() * max_jitter)
                         i += 1
 
         return cast(TCallable, new_func)
```

### Comparing `composer-0.21.1/composer/utils/string_enum.py` & `composer-0.21.2/composer/utils/string_enum.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer/utils/warnings.py` & `composer-0.21.2/composer/utils/warnings.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer.egg-info/PKG-INFO` & `composer-0.21.2/composer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composer
-Version: 0.21.1
+Version: 0.21.2
 Summary: Composer is a PyTorch library that enables you to train neural networks faster, at lower cost, and to higher accuracy.
 Home-page: https://github.com/mosaicml/composer
 Author: MosaicML
 Author-email: team@mosaicml.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: composer Version: 0.21.1 Summary: Composer is a
+Metadata-Version: 2.1 Name: composer Version: 0.21.2 Summary: Composer is a
 PyTorch library that enables you to train neural networks faster, at lower
 cost, and to higher accuracy. Home-page: https://github.com/mosaicml/composer
 Author: MosaicML Author-email: team@mosaicml.com Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Python: >=3.9 Description-Content-Type:
 text/markdown Provides-Extra: base Provides-Extra: dev Provides-Extra:
```

### Comparing `composer-0.21.1/composer.egg-info/SOURCES.txt` & `composer-0.21.2/composer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/composer.egg-info/requires.txt` & `composer-0.21.2/composer.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,101 +1,102 @@
 pyyaml<7,>=6.0
 tqdm<5,>=4.62.3
-torchmetrics<1.3.2,>=0.10.0
+torchmetrics<1.3.3,>=0.10.0
 torch_optimizer<0.4,>=0.3.0
-torchvision<0.17.2,>=0.13.1
-torch<2.2.2,>=2.0.1
+torchvision<0.17.3,>=0.13.1
+torch<2.2.3,>=2.0.1
 requests<3,>=2.26.0
 numpy<1.27.0,>=1.21.5
 psutil<6,>=5.8.0
 coolname<3,>=1.1.0
 tabulate==0.9.0
 py-cpuinfo<10,>=8.0.0
 packaging<24.1,>=21.3.0
 importlib-metadata<7,>=5.0.0
 mosaicml-cli<0.7,>=0.5.25
 
 [all]
-jupyter==1.0.0
-furo==2022.9.29
-nbsphinx==0.9.1
-google-cloud-storage<3.0,>=2.0.0
-mosaicml-streaming<1.0
+recommonmark==0.7.1
+pillow==9.3.0
 onnx<2,>=1.12.0
-slack_sdk<4,>=3.19.5
-py-cpuinfo<10,>=8.0.0
+sphinxcontrib-devhelp==1.0.0
+ipython==8.11.0
+yamllint==1.35.1
+pynvml<12,>=11.5.0
+onnxruntime<2,>=1.12.1
+ipykernel==6.29.2
+jupyter==1.0.0
+sphinxemoji==0.2.0
+protobuf<5.27
+sphinxcontrib-serializinghtml==1.1.5
+databricks-sdk==0.23.0
 oci<3.0.0,>=2.88.2
-GitPython==3.1.42
+sphinxcontrib.katex==0.9.6
+pytest==7.4.4
+pandoc==2.3
+junitparser==3.1.2
+pypandoc==1.13
+neptune<2.0.0,>=1.6.2
+mlflow<3.0,>=2.11.1
+mosaicml-streaming<1.0
+boto3<2,>=1.21.45
+google-cloud-storage<3.0,>=2.0.0
 fasteners==0.18
+transformers!=4.34.0,<4.40,>=4.11
+apache-libcloud<4,>=3.3.1
 sphinxcontrib-images==0.9.4
-tensorboard<3.0.0,>=2.9.1
-sphinxcontrib-applehelp==1.0.0
-comet_ml<4.0.0,>=3.31.12
-deepspeed==0.8.3
-recommonmark==0.7.1
-pytest==7.4.4
+pydantic<2,>=1.0
+pytest-httpserver<1.1,>=1.0.4
+myst-parser==0.16.1
+nbsphinx==0.9.1
 pre-commit<4,>=3.4.0
-coverage[toml]==7.4.4
-junitparser==3.1.2
-sphinxcontrib-htmlhelp==2.0.0
-databricks-sdk==0.22.0
-traitlets==5.14.1
-pynvml<12,>=11.5.0
 cryptography==41.0.5
-sphinx-argparse==0.4.0
-wandb<0.17,>=0.13.2
-sphinxcontrib-devhelp==1.0.0
-moto[s3]<5,>=4.0.1
-neptune<2.0.0,>=1.6.2
+sentencepiece==0.2.0
+py-cpuinfo<10,>=8.0.0
 sphinx_markdown_tables==0.0.17
-docutils==0.17.1
-pandoc==2.3
-boto3<2,>=1.21.45
-ipykernel==6.29.2
-pandas<3.0,>=2.0.0
-custom_inherit==2.4.1
-sphinx_panels==0.6.0
-mlflow<3.0,>=2.11.1
-sphinxcontrib-serializinghtml==1.1.5
+furo==2022.9.29
+sphinx-copybutton==0.5.2
 mock-ssh-server==0.9.1
-sphinxcontrib-qthelp==1.0.0
-protobuf<3.21
 peft<0.8,>=0.7.0
-yamllint==1.35.1
-ipython==8.11.0
-onnxruntime<2,>=1.12.1
-pytest-httpserver<1.1,>=1.0.4
-transformers!=4.34.0,<4.39,>=4.11
+sphinxcontrib-htmlhelp==2.0.0
+coverage[toml]==7.4.4
+paramiko<3,>=2.11.0
 pytest_codeblocks==0.17.0
 sphinxext.opengraph==0.9.1
-apache-libcloud<4,>=3.3.1
-pypandoc==1.13
-paramiko<3,>=2.11.0
-testbook==0.4.2
-myst-parser==0.16.1
-sphinxemoji==0.2.0
-sphinxcontrib.katex==0.9.6
-sphinx-copybutton==0.5.2
+sphinx_panels==0.6.0
+docutils==0.17.1
+traitlets==5.14.2
+sphinx-argparse==0.4.0
+sphinxcontrib-qthelp==1.0.0
+GitPython==3.1.43
+slack_sdk<4,>=3.19.5
+deepspeed==0.8.3
+pandas<3.0,>=2.0.0
+tensorboard<3.0.0,>=2.9.1
+custom_inherit==2.4.1
+moto[s3]<5,>=4.0.1
+sphinxcontrib-applehelp==1.0.0
+comet_ml<4.0.0,>=3.31.12
 setuptools<=59.5.0
-sentencepiece==0.2.0
-pydantic<2,>=1.0
-datasets<3,>=2.4
+wandb<0.17,>=0.13.2
 pycocotools<3,>=2.0.4
 sphinx==4.4.0
+datasets<3,>=2.4
+testbook==0.4.2
 
 [base]
 
 [coco]
 pycocotools<3,>=2.0.4
 
 [comet_ml]
 comet_ml<4.0.0,>=3.31.12
 
 [databricks]
-databricks-sdk==0.22.0
+databricks-sdk==0.23.0
 
 [deepspeed]
 deepspeed==0.8.3
 pydantic<2,>=1.0
 
 [dev]
 custom_inherit==2.4.1
@@ -124,24 +125,25 @@
 furo==2022.9.29
 sphinx-copybutton==0.5.2
 testbook==0.4.2
 myst-parser==0.16.1
 sphinx_panels==0.6.0
 sphinxcontrib-images==0.9.4
 pytest_codeblocks==0.17.0
-traitlets==5.14.1
+traitlets==5.14.2
 nbsphinx==0.9.1
 pandoc==2.3
 pypandoc==1.13
-GitPython==3.1.42
+GitPython==3.1.43
 moto[s3]<5,>=4.0.1
 mock-ssh-server==0.9.1
 cryptography==41.0.5
 pytest-httpserver<1.1,>=1.0.4
 setuptools<=59.5.0
+pillow==9.3.0
 
 [gcs]
 google-cloud-storage<3.0,>=2.0.0
 
 [libcloud]
 apache-libcloud<4,>=3.3.1
 
@@ -151,15 +153,15 @@
 [mlperf]
 py-cpuinfo<10,>=8.0.0
 
 [neptune]
 neptune<2.0.0,>=1.6.2
 
 [nlp]
-transformers!=4.34.0,<4.39,>=4.11
+transformers!=4.34.0,<4.40,>=4.11
 datasets<3,>=2.4
 
 [oci]
 oci<3.0.0,>=2.88.2
 
 [onnx]
 onnx<2,>=1.12.0
@@ -168,15 +170,15 @@
 [pandas]
 pandas<3.0,>=2.0.0
 
 [peft]
 peft<0.8,>=0.7.0
 
 [sentencepiece]
-protobuf<3.21
+protobuf<5.27
 sentencepiece==0.2.0
 
 [slack]
 slack_sdk<4,>=3.19.5
 
 [streaming]
 mosaicml-streaming<1.0
```

### Comparing `composer-0.21.1/pyproject.toml` & `composer-0.21.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/setup.py` & `composer-0.21.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,18 +74,18 @@
         assert end != -1, 'there should be a balanced number of start and ends'
         long_description = long_description[:start] + \
             long_description[end + len(end_tag):]
 
 install_requires = [
     'pyyaml>=6.0,<7',
     'tqdm>=4.62.3,<5',
-    'torchmetrics>=0.10.0,<1.3.2',
+    'torchmetrics>=0.10.0,<1.3.3',
     'torch_optimizer>=0.3.0,<0.4',
-    'torchvision>=0.13.1,<0.17.2',
-    'torch>=2.0.1,<2.2.2',
+    'torchvision>=0.13.1,<0.17.3',
+    'torch>=2.0.1,<2.2.3',
     'requests>=2.26.0,<3',
     'numpy>=1.21.5,<1.27.0',
     'psutil>=5.8.0,<6',
     'coolname>=1.1.0,<3',
     'tabulate==0.9.0',  # for auto-generating tables
     'py-cpuinfo>=8.0.0,<10',
     'packaging>=21.3.0,<24.1',
@@ -128,24 +128,25 @@
     'furo==2022.9.29',
     'sphinx-copybutton==0.5.2',
     'testbook==0.4.2',
     'myst-parser==0.16.1',
     'sphinx_panels==0.6.0',
     'sphinxcontrib-images==0.9.4',
     'pytest_codeblocks==0.17.0',
-    'traitlets==5.14.1',
+    'traitlets==5.14.2',
     'nbsphinx==0.9.1',
     'pandoc==2.3',
     'pypandoc==1.13',
-    'GitPython==3.1.42',
+    'GitPython==3.1.43',
     'moto[s3]>=4.0.1,<5',
     'mock-ssh-server==0.9.1',
     'cryptography==41.0.5',
     'pytest-httpserver>=1.0.4,<1.1',
     'setuptools<=59.5.0',
+    'pillow==9.3.0',  # Matches the Pillow version listed in the Dockerfile
 ]
 
 extra_deps['system_metrics_monitor'] = {
     'pynvml>=11.5.0,<12',
 }
 
 extra_deps['slack'] = {
@@ -174,24 +175,24 @@
 ]
 
 extra_deps['coco'] = [
     'pycocotools>=2.0.4,<3',
 ]
 
 extra_deps['nlp'] = [
-    'transformers>=4.11,<4.39,!=4.34.0',
+    'transformers>=4.11,!=4.34.0,<4.40',
     'datasets>=2.4,<3',
 ]
 
 extra_deps['peft'] = [
     'peft>=0.7.0,<0.8',
 ]
 
 extra_deps['sentencepiece'] = [
-    'protobuf<3.21',
+    'protobuf<5.27',
     'sentencepiece==0.2.0',
 ]
 
 extra_deps['mlperf'] = [
     # TODO: use pip when available: https://github.com/mlcommons/logging/issues/218
     # "mlperf_logging @ git+https://github.com/mlperf/logging.git",
     'py-cpuinfo>=8.0.0,<10',
@@ -222,15 +223,15 @@
 
 extra_deps['mlflow'] = [
     'mlflow>=2.11.1,<3.0',
 ]
 
 extra_deps['pandas'] = ['pandas>=2.0.0,<3.0']
 
-extra_deps['databricks'] = ['databricks-sdk==0.22.0']
+extra_deps['databricks'] = ['databricks-sdk==0.23.0']
 
 extra_deps['all'] = {dep for deps in extra_deps.values() for dep in deps}
 
 composer_data_files = ['py.typed']
 composer_data_files += package_files('composer', 'yamls', '.yaml')
 composer_data_files += package_files('composer', 'algorithms', '.json')
```

### Comparing `composer-0.21.1/tests/test_cli.py` & `composer-0.21.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/tests/test_device.py` & `composer-0.21.2/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/tests/test_docs.py` & `composer-0.21.2/tests/test_docs.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/tests/test_engine.py` & `composer-0.21.2/tests/test_engine.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # Copyright 2022 MosaicML Composer authors
 # SPDX-License-Identifier: Apache-2.0
 
+import importlib
 import logging
 import os
 import subprocess
 import sys
 import textwrap
+import threading
 from pathlib import Path
 from typing import List
 from unittest.mock import Mock
 
 import pytest
 
 import composer
@@ -319,7 +321,19 @@
         ('composer.core.engine', 10, '[ep=0][ba=0][event=INIT]: Running event'),
         ('composer.core.engine', 10, '[ep=0][ba=0][event=INIT]: Running callback EventCounterCallback'),
         ('composer.core.engine', 10, 'Closing the engine.'),
         ('composer.core.engine', 10, 'Closing callback EventCounterCallback'),
         ('composer.core.engine', 10, 'Post-closing callback EventCounterCallback'),
         ('composer.core.engine', 10, 'Engine closed.'),
     ]
+
+
+def _worker():
+    import composer.core.engine
+    importlib.reload(composer.core.engine)
+
+
+def test_graceful_fallback_when_signal_handler_cannot_be_set():
+    # https://github.com/mosaicml/composer/issues/3151#issue-2205981731
+    t = threading.Thread(target=_worker)
+    t.start()
+    t.join()
```

### Comparing `composer-0.21.1/tests/test_events.py` & `composer-0.21.2/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/tests/test_full_nlp.py` & `composer-0.21.2/tests/test_full_nlp.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/tests/test_loss.py` & `composer-0.21.2/tests/test_loss.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/tests/test_notebooks.py` & `composer-0.21.2/tests/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/tests/test_passes.py` & `composer-0.21.2/tests/test_passes.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/tests/test_precision.py` & `composer-0.21.2/tests/test_precision.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/tests/test_simple_nlp.py` & `composer-0.21.2/tests/test_simple_nlp.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/tests/test_smoketest.py` & `composer-0.21.2/tests/test_smoketest.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/tests/test_split_batch.py` & `composer-0.21.2/tests/test_split_batch.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/tests/test_state.py` & `composer-0.21.2/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `composer-0.21.1/tests/test_time.py` & `composer-0.21.2/tests/test_time.py`

 * *Files identical despite different names*

