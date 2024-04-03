# Comparing `tmp/caikit-nlp-0.4.7.tar.gz` & `tmp/caikit-nlp-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caikit-nlp-0.4.7.tar", last modified: Tue Apr  2 18:40:10 2024, max compression
+gzip compressed data, was "caikit-nlp-0.4.8.tar", last modified: Wed Apr  3 19:16:29 2024, max compression
```

## Comparing `caikit-nlp-0.4.7.tar` & `caikit-nlp-0.4.8.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.819068 caikit-nlp-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.791068 caikit-nlp-0.4.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.791068 caikit-nlp-0.4.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.github/ISSUE_TEMPLATE/user_story.md
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.795068 caikit-nlp-0.4.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.github/workflows/build-image.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.github/workflows/build-library.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.github/workflows/lint-code.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.github/workflows/publish-library.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (127)    21457 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/.whitesource
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-04-02 18:40:10.819068 caikit-nlp-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.795068 caikit-nlp-0.4.7/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/benchmarks/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.783068 caikit-nlp-0.4.7/benchmarks/logs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.795068 caikit-nlp-0.4.7/benchmarks/logs/llama2-7b/
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/benchmarks/logs/llama2-7b/20230905_183655.output
--rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/benchmarks/logs/llama2-7b/20230905_184809.output
--rw-r--r--   0 runner    (1001) docker     (127)     9795 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/benchmarks/logs/llama2-7b/20230905_191650.output
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/benchmarks/logs/llama2-7b/20230905_194133.output
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/benchmarks/logs/llama2-7b/20230906_135211.output
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.795068 caikit-nlp-0.4.7/caikit_nlp/
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-02 18:40:10.000000 caikit-nlp-0.4.7/caikit_nlp/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.795068 caikit-nlp-0.4.7/caikit_nlp/config/
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/config/config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.795068 caikit-nlp-0.4.7/caikit_nlp/data_model/
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/data_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/data_model/generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.799068 caikit-nlp-0.4.7/caikit_nlp/model_management/
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/model_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/model_management/tgis_auto_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.799068 caikit-nlp-0.4.7/caikit_nlp/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.799068 caikit-nlp-0.4.7/caikit_nlp/modules/text_classification/
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/text_classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/text_classification/sequence_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.799068 caikit-nlp-0.4.7/caikit_nlp/modules/text_embedding/
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/text_embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39423 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/text_embedding/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/text_embedding/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.799068 caikit-nlp-0.4.7/caikit_nlp/modules/text_generation/
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/text_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8496 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/text_generation/peft_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    51230 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/text_generation/peft_prompt_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)    12248 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/text_generation/peft_tgis_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)    26132 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/text_generation/text_generation_local.py
--rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/text_generation/text_generation_tgis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.799068 caikit-nlp-0.4.7/caikit_nlp/modules/token_classification/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/token_classification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16150 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/token_classification/filtered_span_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.799068 caikit-nlp-0.4.7/caikit_nlp/modules/tokenization/
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/tokenization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/modules/tokenization/regex_sentence_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.799068 caikit-nlp-0.4.7/caikit_nlp/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.803068 caikit-nlp-0.4.7/caikit_nlp/resources/pretrained_model/
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/resources/pretrained_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15732 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/resources/pretrained_model/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    21429 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/resources/pretrained_model/hf_auto_causal_lm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/resources/pretrained_model/hf_auto_seq2seq_lm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/resources/pretrained_model/hf_auto_seq_classifier.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.803068 caikit-nlp-0.4.7/caikit_nlp/toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/toolkit/data_stream_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/toolkit/data_type_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/toolkit/task_specific_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.803068 caikit-nlp-0.4.7/caikit_nlp/toolkit/text_generation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/toolkit/text_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/toolkit/text_generation/model_run_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    19662 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/toolkit/text_generation/tgis_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/toolkit/torch_run.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/toolkit/trainer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/toolkit/verbalizer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/caikit_nlp/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.819068 caikit-nlp-0.4.7/caikit_nlp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-04-02 18:40:10.000000 caikit-nlp-0.4.7/caikit_nlp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-02 18:40:10.000000 caikit-nlp-0.4.7/caikit_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:40:10.000000 caikit-nlp-0.4.7/caikit_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-02 18:40:10.000000 caikit-nlp-0.4.7/caikit_nlp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-02 18:40:10.000000 caikit-nlp-0.4.7/caikit_nlp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/code-of-conduct.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.803068 caikit-nlp-0.4.7/examples/
--rw-r--r--   0 runner    (1001) docker     (127)    55479 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/examples/Caikit_Getting_Started.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/examples/compare_local_vs_tgis_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/examples/evaluate_model.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      404 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/examples/kill-text-generation-launcher.sh
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/examples/load_and_run_distributed_peft.py
--rw-r--r--   0 runner    (1001) docker     (127)    13678 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/examples/run_fine_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)    15840 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/examples/run_peft_tuning.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1992 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/examples/text-generation-launcher
--rw-r--r--   0 runner    (1001) docker     (127)    15815 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/examples/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/prompt_tuning_parameter_selection.md
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/runtime_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.803068 caikit-nlp-0.4.7/runtime_template/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1252 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/runtime_template/run_with_gateway.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.807068 caikit-nlp-0.4.7/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      657 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/scripts/dump_apis.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      720 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/scripts/fmt.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      231 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/scripts/run_local.sh
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 18:40:10.819068 caikit-nlp-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/setup_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.807068 caikit-nlp-0.4.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.807068 caikit-nlp-0.4.7/tests/data_model/
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/data_model/test_generation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.807068 caikit-nlp-0.4.7/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)    11719 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.807068 caikit-nlp-0.4.7/tests/fixtures/data_model/
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/data_model/sample_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.807068 caikit-nlp-0.4.7/tests/fixtures/tiny_models/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.807068 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BertForSequenceClassification/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BertForSequenceClassification/config.json
--rw-r--r--   0 runner    (1001) docker     (127)   384767 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BertForSequenceClassification/pytorch_model.bin
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BertForSequenceClassification/special_tokens_map.json
--rw-r--r--   0 runner    (1001) docker     (127)   481096 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BertForSequenceClassification/tf_model.h5
--rw-r--r--   0 runner    (1001) docker     (127)    23061 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BertForSequenceClassification/tokenizer.json
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BertForSequenceClassification/tokenizer_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BertForSequenceClassification/vocab.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.811068 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BloomForCausalLM/
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BloomForCausalLM/config.json
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BloomForCausalLM/generation_config.json
--rw-r--r--   0 runner    (1001) docker     (127)   406260 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BloomForCausalLM/pytorch_model.bin
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BloomForCausalLM/special_tokens_map.json
--rw-r--r--   0 runner    (1001) docker     (127)    33054 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BloomForCausalLM/tokenizer.json
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/BloomForCausalLM/tokenizer_config.json
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.815068 caikit-nlp-0.4.7/tests/fixtures/tiny_models/T5ForConditionalGeneration/
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/T5ForConditionalGeneration/config.json
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/T5ForConditionalGeneration/generation_config.json
--rw-r--r--   0 runner    (1001) docker     (127)   546693 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/T5ForConditionalGeneration/pytorch_model.bin
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/T5ForConditionalGeneration/special_tokens_map.json
--rw-r--r--   0 runner    (1001) docker     (127)   382892 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/T5ForConditionalGeneration/tokenizer.json
--rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/fixtures/tiny_models/T5ForConditionalGeneration/tokenizer_config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.815068 caikit-nlp-0.4.7/tests/model_management/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/model_management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/model_management/test_tgis_auto_finder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.815068 caikit-nlp-0.4.7/tests/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.815068 caikit-nlp-0.4.7/tests/modules/text_classification/
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/modules/text_classification/test_sequence_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.815068 caikit-nlp-0.4.7/tests/modules/text_embedding/
--rw-r--r--   0 runner    (1001) docker     (127)    35704 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/modules/text_embedding/test_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.815068 caikit-nlp-0.4.7/tests/modules/text_generation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/modules/text_generation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/modules/text_generation/test_peft_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    25729 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/modules/text_generation/test_peft_prompt_tuning.py
--rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/modules/text_generation/test_peft_tgis_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     7254 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/modules/text_generation/test_text_generation_local.py
--rw-r--r--   0 runner    (1001) docker     (127)     8300 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/modules/text_generation/test_text_generation_tgis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.815068 caikit-nlp-0.4.7/tests/modules/token_classification/
--rw-r--r--   0 runner    (1001) docker     (127)    18398 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/modules/token_classification/test_filtered_span_classification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.815068 caikit-nlp-0.4.7/tests/modules/tokenization/
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/modules/tokenization/test_regex_sentence_splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.815068 caikit-nlp-0.4.7/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16904 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/resources/test_pretrained_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.815068 caikit-nlp-0.4.7/tests/toolkit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/toolkit/test_data_stream_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/toolkit/test_data_type_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/toolkit/test_task_specific_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/toolkit/test_verbalizers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:40:10.819068 caikit-nlp-0.4.7/tests/toolkit/text_generation/
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tests/toolkit/text_generation/test_model_run_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-02 18:39:58.000000 caikit-nlp-0.4.7/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.669224 caikit-nlp-0.4.8/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.641224 caikit-nlp-0.4.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.641224 caikit-nlp-0.4.8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.github/ISSUE_TEMPLATE/user_story.md
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.645224 caikit-nlp-0.4.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.github/workflows/build-image.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.github/workflows/build-library.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.github/workflows/lint-code.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.github/workflows/publish-library.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (127)    21457 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/.whitesource
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-04-03 19:16:29.669224 caikit-nlp-0.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10588 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.645224 caikit-nlp-0.4.8/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/benchmarks/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.633224 caikit-nlp-0.4.8/benchmarks/logs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.645224 caikit-nlp-0.4.8/benchmarks/logs/llama2-7b/
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/benchmarks/logs/llama2-7b/20230905_183655.output
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/benchmarks/logs/llama2-7b/20230905_184809.output
+-rw-r--r--   0 runner    (1001) docker     (127)     9795 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/benchmarks/logs/llama2-7b/20230905_191650.output
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/benchmarks/logs/llama2-7b/20230905_194133.output
+-rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/benchmarks/logs/llama2-7b/20230906_135211.output
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.645224 caikit-nlp-0.4.8/caikit_nlp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-03 19:16:29.000000 caikit-nlp-0.4.8/caikit_nlp/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.645224 caikit-nlp-0.4.8/caikit_nlp/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/config/config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.645224 caikit-nlp-0.4.8/caikit_nlp/data_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/data_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/data_model/generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.649224 caikit-nlp-0.4.8/caikit_nlp/model_management/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/model_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5168 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/model_management/tgis_auto_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.649224 caikit-nlp-0.4.8/caikit_nlp/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.649224 caikit-nlp-0.4.8/caikit_nlp/modules/text_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/text_classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7859 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/text_classification/sequence_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.649224 caikit-nlp-0.4.8/caikit_nlp/modules/text_embedding/
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/text_embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40080 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/text_embedding/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/text_embedding/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.649224 caikit-nlp-0.4.8/caikit_nlp/modules/text_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/text_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8496 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/text_generation/peft_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51230 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/text_generation/peft_prompt_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12248 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/text_generation/peft_tgis_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26132 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/text_generation/text_generation_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/text_generation/text_generation_tgis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.649224 caikit-nlp-0.4.8/caikit_nlp/modules/token_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/token_classification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16150 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/token_classification/filtered_span_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.649224 caikit-nlp-0.4.8/caikit_nlp/modules/tokenization/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/tokenization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/modules/tokenization/regex_sentence_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.649224 caikit-nlp-0.4.8/caikit_nlp/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.653224 caikit-nlp-0.4.8/caikit_nlp/resources/pretrained_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/resources/pretrained_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15732 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/resources/pretrained_model/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21429 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/resources/pretrained_model/hf_auto_causal_lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/resources/pretrained_model/hf_auto_seq2seq_lm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1903 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/resources/pretrained_model/hf_auto_seq_classifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.653224 caikit-nlp-0.4.8/caikit_nlp/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/toolkit/data_stream_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/toolkit/data_type_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/toolkit/task_specific_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.653224 caikit-nlp-0.4.8/caikit_nlp/toolkit/text_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/toolkit/text_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/toolkit/text_generation/model_run_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19662 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/toolkit/text_generation/tgis_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3335 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/toolkit/torch_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/toolkit/trainer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/toolkit/verbalizer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/caikit_nlp/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.669224 caikit-nlp-0.4.8/caikit_nlp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11424 2024-04-03 19:16:29.000000 caikit-nlp-0.4.8/caikit_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-04-03 19:16:29.000000 caikit-nlp-0.4.8/caikit_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 19:16:29.000000 caikit-nlp-0.4.8/caikit_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-03 19:16:29.000000 caikit-nlp-0.4.8/caikit_nlp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-03 19:16:29.000000 caikit-nlp-0.4.8/caikit_nlp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/code-of-conduct.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.653224 caikit-nlp-0.4.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)    55479 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/examples/Caikit_Getting_Started.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/examples/compare_local_vs_tgis_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7104 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/examples/evaluate_model.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      404 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/examples/kill-text-generation-launcher.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/examples/load_and_run_distributed_peft.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13678 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/examples/run_fine_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15840 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/examples/run_peft_tuning.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1992 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/examples/text-generation-launcher
+-rw-r--r--   0 runner    (1001) docker     (127)    15815 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/examples/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6158 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/prompt_tuning_parameter_selection.md
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/runtime_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.657224 caikit-nlp-0.4.8/runtime_template/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1252 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/runtime_template/run_with_gateway.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.657224 caikit-nlp-0.4.8/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      657 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/scripts/dump_apis.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      720 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/scripts/fmt.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      231 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/scripts/run_local.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 19:16:29.669224 caikit-nlp-0.4.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/setup_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.657224 caikit-nlp-0.4.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.657224 caikit-nlp-0.4.8/tests/data_model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/data_model/test_generation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.657224 caikit-nlp-0.4.8/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)    11719 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.657224 caikit-nlp-0.4.8/tests/fixtures/data_model/
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/data_model/sample_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.657224 caikit-nlp-0.4.8/tests/fixtures/tiny_models/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.661224 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BertForSequenceClassification/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BertForSequenceClassification/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)   384767 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BertForSequenceClassification/pytorch_model.bin
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BertForSequenceClassification/special_tokens_map.json
+-rw-r--r--   0 runner    (1001) docker     (127)   481096 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BertForSequenceClassification/tf_model.h5
+-rw-r--r--   0 runner    (1001) docker     (127)    23061 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BertForSequenceClassification/tokenizer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BertForSequenceClassification/tokenizer_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4679 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BertForSequenceClassification/vocab.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.661224 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BloomForCausalLM/
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BloomForCausalLM/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BloomForCausalLM/generation_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)   406260 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BloomForCausalLM/pytorch_model.bin
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BloomForCausalLM/special_tokens_map.json
+-rw-r--r--   0 runner    (1001) docker     (127)    33054 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BloomForCausalLM/tokenizer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/BloomForCausalLM/tokenizer_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.665224 caikit-nlp-0.4.8/tests/fixtures/tiny_models/T5ForConditionalGeneration/
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/T5ForConditionalGeneration/config.json
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/T5ForConditionalGeneration/generation_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)   546693 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/T5ForConditionalGeneration/pytorch_model.bin
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/T5ForConditionalGeneration/special_tokens_map.json
+-rw-r--r--   0 runner    (1001) docker     (127)   382892 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/T5ForConditionalGeneration/tokenizer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2319 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/fixtures/tiny_models/T5ForConditionalGeneration/tokenizer_config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.665224 caikit-nlp-0.4.8/tests/model_management/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/model_management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9024 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/model_management/test_tgis_auto_finder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.665224 caikit-nlp-0.4.8/tests/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.665224 caikit-nlp-0.4.8/tests/modules/text_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/modules/text_classification/test_sequence_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.665224 caikit-nlp-0.4.8/tests/modules/text_embedding/
+-rw-r--r--   0 runner    (1001) docker     (127)    37559 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/modules/text_embedding/test_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.665224 caikit-nlp-0.4.8/tests/modules/text_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/modules/text_generation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/modules/text_generation/test_peft_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25729 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/modules/text_generation/test_peft_prompt_tuning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6540 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/modules/text_generation/test_peft_tgis_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7254 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/modules/text_generation/test_text_generation_local.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8300 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/modules/text_generation/test_text_generation_tgis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.665224 caikit-nlp-0.4.8/tests/modules/token_classification/
+-rw-r--r--   0 runner    (1001) docker     (127)    18398 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/modules/token_classification/test_filtered_span_classification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.665224 caikit-nlp-0.4.8/tests/modules/tokenization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/modules/tokenization/test_regex_sentence_splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.665224 caikit-nlp-0.4.8/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16904 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/resources/test_pretrained_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.669224 caikit-nlp-0.4.8/tests/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/toolkit/test_data_stream_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/toolkit/test_data_type_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/toolkit/test_task_specific_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/toolkit/test_verbalizers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 19:16:29.669224 caikit-nlp-0.4.8/tests/toolkit/text_generation/
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tests/toolkit/text_generation/test_model_run_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-03 19:16:16.000000 caikit-nlp-0.4.8/tox.ini
```

### Comparing `caikit-nlp-0.4.7/.github/ISSUE_TEMPLATE/bug_report.md` & `caikit-nlp-0.4.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/.github/ISSUE_TEMPLATE/feature_request.md` & `caikit-nlp-0.4.8/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/.github/ISSUE_TEMPLATE/user_story.md` & `caikit-nlp-0.4.8/.github/ISSUE_TEMPLATE/user_story.md`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/.github/workflows/build-image.yml` & `caikit-nlp-0.4.8/.github/workflows/build-image.yml`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/.github/workflows/build-library.yml` & `caikit-nlp-0.4.8/.github/workflows/build-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/.github/workflows/lint-code.yml` & `caikit-nlp-0.4.8/.github/workflows/lint-code.yml`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/.github/workflows/publish-library.yml` & `caikit-nlp-0.4.8/.github/workflows/publish-library.yml`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/.gitignore` & `caikit-nlp-0.4.8/.gitignore`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/.pylintrc` & `caikit-nlp-0.4.8/.pylintrc`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/CONTRIBUTING.md` & `caikit-nlp-0.4.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/Dockerfile` & `caikit-nlp-0.4.8/Dockerfile`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/LICENSE` & `caikit-nlp-0.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/PKG-INFO` & `caikit-nlp-0.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caikit-nlp
-Version: 0.4.7
+Version: 0.4.8
 Summary: Caikit NLP
 License: Apache-2.0
 Project-URL: Source, https://github.com/caikit/caikit-nlp
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `caikit-nlp-0.4.7/README.md` & `caikit-nlp-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/benchmarks/README.md` & `caikit-nlp-0.4.8/benchmarks/README.md`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/benchmarks/logs/llama2-7b/20230905_183655.output` & `caikit-nlp-0.4.8/benchmarks/logs/llama2-7b/20230905_183655.output`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/benchmarks/logs/llama2-7b/20230905_184809.output` & `caikit-nlp-0.4.8/benchmarks/logs/llama2-7b/20230905_184809.output`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/benchmarks/logs/llama2-7b/20230905_191650.output` & `caikit-nlp-0.4.8/benchmarks/logs/llama2-7b/20230905_191650.output`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/benchmarks/logs/llama2-7b/20230905_194133.output` & `caikit-nlp-0.4.8/benchmarks/logs/llama2-7b/20230905_194133.output`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/benchmarks/logs/llama2-7b/20230906_135211.output` & `caikit-nlp-0.4.8/benchmarks/logs/llama2-7b/20230906_135211.output`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/__init__.py` & `caikit-nlp-0.4.8/caikit_nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/config/__init__.py` & `caikit-nlp-0.4.8/caikit_nlp/config/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/config/config.yml` & `caikit-nlp-0.4.8/caikit_nlp/config/config.yml`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/data_model/__init__.py` & `caikit-nlp-0.4.8/caikit_nlp/data_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/data_model/generation.py` & `caikit-nlp-0.4.8/caikit_nlp/data_model/generation.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/model_management/__init__.py` & `caikit-nlp-0.4.8/caikit_nlp/model_management/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/model_management/tgis_auto_finder.py` & `caikit-nlp-0.4.8/caikit_nlp/model_management/tgis_auto_finder.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/modules/__init__.py` & `caikit-nlp-0.4.8/caikit_nlp/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/modules/text_classification/__init__.py` & `caikit-nlp-0.4.8/caikit_nlp/modules/text_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/modules/text_classification/sequence_classification.py` & `caikit-nlp-0.4.8/caikit_nlp/modules/text_classification/sequence_classification.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/modules/text_embedding/__init__.py` & `caikit-nlp-0.4.8/caikit_nlp/modules/text_embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/modules/text_embedding/embedding.py` & `caikit-nlp-0.4.8/caikit_nlp/modules/text_embedding/embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -814,15 +814,17 @@
 
         # Do truncation if given a usable truncation value, else test for need to truncation
         if truncate_input_tokens < 0:
             okay_to_truncate = True
             max_length = max_tokens
         elif 0 < truncate_input_tokens <= max_tokens:
             okay_to_truncate = True
-            max_length = truncate_input_tokens
+            # Add 2 for begin/end tokens, but don't go higher than model's max_tokens
+            max_length = min(truncate_input_tokens + 2, max_tokens)
+
         else:
             okay_to_truncate = not implicit_truncation_errors
             max_length = max_tokens
 
         assert len(texts) > 0, "Cannot truncate nothing"
         assert isinstance(texts[0], str), "Only str can be truncated"
 
@@ -855,25 +857,41 @@
                 return_offsets_mapping=True,
                 return_length=True,
                 return_tensors="pt",
                 truncation=False,
                 padding=True,
             )
 
-            tokens = sum_token_count(tokenized, truncate_only=False)
+            tokens = 0
+            for encoding in tokenized.encodings:
+                tokens = max(sum(encoding.attention_mask), tokens)
             error.log_raise(
                 "<NLP08391926E>",
                 ValueError(
                     f"Token sequence length is longer than the specified "
                     f"maximum sequence length for this model ({tokens} > {max_tokens})."
                 ),
             )
 
         input_token_count = sum_token_count(tokenized, truncate_only=True)
 
+        # Tokenize without overflow for batching and truncation to work together.
+        tokenized = self.tokenizer(
+            *to_tokenize,
+            return_attention_mask=True,
+            return_token_type_ids=False,
+            return_overflowing_tokens=False,
+            return_offsets_mapping=False,
+            return_length=False,
+            return_tensors="pt",
+            truncation=True,
+            padding=True,
+            max_length=max_length,
+        )
+
         return TruncatedTokensTuple(tokenized, input_token_count)
 
     def encode(
         self,
         sentences: Union[str, List[str]],
         batch_size: int = 32,
         show_progress_bar: bool = None,
```

### Comparing `caikit-nlp-0.4.7/caikit_nlp/modules/text_embedding/utils.py` & `caikit-nlp-0.4.8/caikit_nlp/modules/text_embedding/utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/modules/text_generation/__init__.py` & `caikit-nlp-0.4.8/caikit_nlp/modules/text_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/modules/text_generation/peft_config.py` & `caikit-nlp-0.4.8/caikit_nlp/modules/text_generation/peft_config.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/modules/text_generation/peft_prompt_tuning.py` & `caikit-nlp-0.4.8/caikit_nlp/modules/text_generation/peft_prompt_tuning.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/modules/text_generation/peft_tgis_remote.py` & `caikit-nlp-0.4.8/caikit_nlp/modules/text_generation/peft_tgis_remote.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/modules/text_generation/text_generation_local.py` & `caikit-nlp-0.4.8/caikit_nlp/modules/text_generation/text_generation_local.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/modules/text_generation/text_generation_tgis.py` & `caikit-nlp-0.4.8/caikit_nlp/modules/text_generation/text_generation_tgis.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/modules/token_classification/__init__.py` & `caikit-nlp-0.4.8/caikit_nlp/modules/token_classification/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/modules/token_classification/filtered_span_classification.py` & `caikit-nlp-0.4.8/caikit_nlp/modules/token_classification/filtered_span_classification.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/modules/tokenization/__init__.py` & `caikit-nlp-0.4.8/caikit_nlp/modules/tokenization/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/modules/tokenization/regex_sentence_splitter.py` & `caikit-nlp-0.4.8/caikit_nlp/modules/tokenization/regex_sentence_splitter.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/resources/__init__.py` & `caikit-nlp-0.4.8/caikit_nlp/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/resources/pretrained_model/__init__.py` & `caikit-nlp-0.4.8/caikit_nlp/resources/pretrained_model/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/resources/pretrained_model/base.py` & `caikit-nlp-0.4.8/caikit_nlp/resources/pretrained_model/base.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/resources/pretrained_model/hf_auto_causal_lm.py` & `caikit-nlp-0.4.8/caikit_nlp/resources/pretrained_model/hf_auto_causal_lm.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/resources/pretrained_model/hf_auto_seq2seq_lm.py` & `caikit-nlp-0.4.8/caikit_nlp/resources/pretrained_model/hf_auto_seq2seq_lm.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/resources/pretrained_model/hf_auto_seq_classifier.py` & `caikit-nlp-0.4.8/caikit_nlp/resources/pretrained_model/hf_auto_seq_classifier.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/toolkit/data_stream_wrapper.py` & `caikit-nlp-0.4.8/caikit_nlp/toolkit/data_stream_wrapper.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/toolkit/data_type_utils.py` & `caikit-nlp-0.4.8/caikit_nlp/toolkit/data_type_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/toolkit/task_specific_utils.py` & `caikit-nlp-0.4.8/caikit_nlp/toolkit/task_specific_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/toolkit/text_generation/model_run_utils.py` & `caikit-nlp-0.4.8/caikit_nlp/toolkit/text_generation/model_run_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/toolkit/text_generation/tgis_utils.py` & `caikit-nlp-0.4.8/caikit_nlp/toolkit/text_generation/tgis_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/toolkit/torch_run.py` & `caikit-nlp-0.4.8/caikit_nlp/toolkit/torch_run.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/toolkit/trainer_utils.py` & `caikit-nlp-0.4.8/caikit_nlp/toolkit/trainer_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp/toolkit/verbalizer_utils.py` & `caikit-nlp-0.4.8/caikit_nlp/toolkit/verbalizer_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/caikit_nlp.egg-info/PKG-INFO` & `caikit-nlp-0.4.8/caikit_nlp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caikit-nlp
-Version: 0.4.7
+Version: 0.4.8
 Summary: Caikit NLP
 License: Apache-2.0
 Project-URL: Source, https://github.com/caikit/caikit-nlp
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `caikit-nlp-0.4.7/caikit_nlp.egg-info/SOURCES.txt` & `caikit-nlp-0.4.8/caikit_nlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/examples/Caikit_Getting_Started.ipynb` & `caikit-nlp-0.4.8/examples/Caikit_Getting_Started.ipynb`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/examples/compare_local_vs_tgis_models.py` & `caikit-nlp-0.4.8/examples/compare_local_vs_tgis_models.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/examples/evaluate_model.py` & `caikit-nlp-0.4.8/examples/evaluate_model.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/examples/load_and_run_distributed_peft.py` & `caikit-nlp-0.4.8/examples/load_and_run_distributed_peft.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/examples/run_fine_tuning.py` & `caikit-nlp-0.4.8/examples/run_fine_tuning.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/examples/run_peft_tuning.py` & `caikit-nlp-0.4.8/examples/run_peft_tuning.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/examples/text-generation-launcher` & `caikit-nlp-0.4.8/examples/text-generation-launcher`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/examples/utils.py` & `caikit-nlp-0.4.8/examples/utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/prompt_tuning_parameter_selection.md` & `caikit-nlp-0.4.8/prompt_tuning_parameter_selection.md`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/pyproject.toml` & `caikit-nlp-0.4.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/runtime_config.yaml` & `caikit-nlp-0.4.8/runtime_config.yaml`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/runtime_template/run_with_gateway.sh` & `caikit-nlp-0.4.8/runtime_template/run_with_gateway.sh`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/scripts/dump_apis.sh` & `caikit-nlp-0.4.8/scripts/dump_apis.sh`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/scripts/fmt.sh` & `caikit-nlp-0.4.8/scripts/fmt.sh`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/conftest.py` & `caikit-nlp-0.4.8/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/data_model/test_generation.py` & `caikit-nlp-0.4.8/tests/data_model/test_generation.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/fixtures/__init__.py` & `caikit-nlp-0.4.8/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/fixtures/data_model/sample_objects.py` & `caikit-nlp-0.4.8/tests/fixtures/data_model/sample_objects.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/fixtures/tiny_models/BertForSequenceClassification/config.json` & `caikit-nlp-0.4.8/tests/fixtures/tiny_models/BertForSequenceClassification/config.json`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/fixtures/tiny_models/BertForSequenceClassification/pytorch_model.bin` & `caikit-nlp-0.4.8/tests/fixtures/tiny_models/BertForSequenceClassification/pytorch_model.bin`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/fixtures/tiny_models/BertForSequenceClassification/tf_model.h5` & `caikit-nlp-0.4.8/tests/fixtures/tiny_models/BertForSequenceClassification/tf_model.h5`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/fixtures/tiny_models/BertForSequenceClassification/tokenizer.json` & `caikit-nlp-0.4.8/tests/fixtures/tiny_models/BertForSequenceClassification/tokenizer.json`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/fixtures/tiny_models/BertForSequenceClassification/vocab.txt` & `caikit-nlp-0.4.8/tests/fixtures/tiny_models/BertForSequenceClassification/vocab.txt`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/fixtures/tiny_models/BloomForCausalLM/config.json` & `caikit-nlp-0.4.8/tests/fixtures/tiny_models/BloomForCausalLM/config.json`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/fixtures/tiny_models/BloomForCausalLM/pytorch_model.bin` & `caikit-nlp-0.4.8/tests/fixtures/tiny_models/BloomForCausalLM/pytorch_model.bin`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/fixtures/tiny_models/BloomForCausalLM/tokenizer.json` & `caikit-nlp-0.4.8/tests/fixtures/tiny_models/BloomForCausalLM/tokenizer.json`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/fixtures/tiny_models/README.md` & `caikit-nlp-0.4.8/tests/fixtures/tiny_models/README.md`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/fixtures/tiny_models/T5ForConditionalGeneration/config.json` & `caikit-nlp-0.4.8/tests/fixtures/tiny_models/T5ForConditionalGeneration/config.json`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/fixtures/tiny_models/T5ForConditionalGeneration/pytorch_model.bin` & `caikit-nlp-0.4.8/tests/fixtures/tiny_models/T5ForConditionalGeneration/pytorch_model.bin`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/fixtures/tiny_models/T5ForConditionalGeneration/special_tokens_map.json` & `caikit-nlp-0.4.8/tests/fixtures/tiny_models/T5ForConditionalGeneration/special_tokens_map.json`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/fixtures/tiny_models/T5ForConditionalGeneration/tokenizer.json` & `caikit-nlp-0.4.8/tests/fixtures/tiny_models/T5ForConditionalGeneration/tokenizer.json`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/fixtures/tiny_models/T5ForConditionalGeneration/tokenizer_config.json` & `caikit-nlp-0.4.8/tests/fixtures/tiny_models/T5ForConditionalGeneration/tokenizer_config.json`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/model_management/test_tgis_auto_finder.py` & `caikit-nlp-0.4.8/tests/model_management/test_tgis_auto_finder.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/modules/text_classification/test_sequence_classification.py` & `caikit-nlp-0.4.8/tests/modules/text_classification/test_sequence_classification.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/modules/text_embedding/test_embedding.py` & `caikit-nlp-0.4.8/tests/modules/text_embedding/test_embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -677,20 +677,22 @@
         loaded_model.run_rerank_queries(
             queries=[ok],
             documents=[{"text": too_long}],
             truncate_input_tokens=truncate_input_tokens,
         )
 
 
-@pytest.mark.parametrize("truncate_input_tokens", [-1, 99, 512])
+@pytest.mark.parametrize("truncate_input_tokens", [-1, 99, 510, 511, 512])
 def test_too_many_tokens_with_truncation_working(truncate_input_tokens, loaded_model):
     """truncate_input_tokens prevents these endpoints from raising an error when too many tokens.
 
     Test with -1 which lets the model do truncation instead of raising an error.
-    Test with 99 (< 512) which causes our code to do the truncation instead of raising an error.
+    Test with 99 (< 512 -2) which causes our code to do the truncation instead of raising an error.
+    Test with 510 (512 -2) which causes our code to do the truncation instead of raising an error.
+    511 and 512 also behave like 510. The value is allowed, but begin/end tokens will take space.
     """
 
     model_max = loaded_model.model.max_seq_length
 
     ok = "x " * (model_max - 2)  # Subtract 2 for begin/end tokens
     too_long = "x " * (model_max - 1)  # This will go over
 
@@ -745,37 +747,59 @@
     loaded_model.run_rerank_queries(
         queries=[ok],
         documents=[{"text": too_long}],
         truncate_input_tokens=truncate_input_tokens,
     )
 
 
-@pytest.mark.parametrize("truncate_input_tokens", [99, 512, -1])
+@pytest.mark.parametrize(
+    "truncate_input_tokens", [1, 2, 3, 4, 99, 100, 101, 510, 511, 512, -1]
+)
 def test_embeddings_with_truncation(truncate_input_tokens, loaded_model):
     """verify that results are as expected with truncation"""
 
+    max_len = loaded_model.model.max_seq_length - 2
     if truncate_input_tokens is None or truncate_input_tokens < 0:
-        # For -1 we don't truncate, but sentence-transformers will truncate at max_seq_length
-        repeat = loaded_model.model.max_seq_length
+        # For -1 we don't truncate, but sentence-transformers will truncate at max_seq_length - 2
+        repeat = max_len
     else:
-        repeat = truncate_input_tokens
+        repeat = min(
+            truncate_input_tokens, max_len
+        )  # max_len is used when we need -2 for begin/end
 
     # Build a text like "x x x.. x " with room for one more token
     repeat = repeat - 1  # space for the final x or y token to show difference
 
-    base = "x " * repeat  # A bunch of "x" tokens
+    base = ""
+    if repeat > 0:
+        base = "x " * repeat  # A bunch of "x" tokens
     x = base + "x"  # One last "x" that will not get truncated
     y = base + "y"  # A different last character "y" not truncated
     z = y + "z"  # Add token "z" after "y". This should get truncated.
 
     res = loaded_model.run_embeddings(
         texts=[base, x, y, z], truncate_input_tokens=truncate_input_tokens
     )
+    vectors = res.results.vectors  # vectors from batch embeddings
 
-    vectors = res.results.vectors
+    # Compare with results from individual embedding calls in a loop
+    loop_res = []
+    for t in [base, x, y, z]:
+        r = loaded_model.run_embedding(
+            text=t, truncate_input_tokens=truncate_input_tokens
+        )
+        loop_res.append(r)
+    loop_vectors = [
+        r.result for r in loop_res
+    ]  # vectors from loop of single embedding calls
+
+    assert len(vectors) == len(loop_vectors), "expected the same length vectors"
+    # compare the vectors from batch with the single calls
+    for i, e in enumerate(vectors):
+        assert np.allclose(e.data.values, loop_vectors[i].data.values)
 
     # x...xyz is the same as x...xy because that is exactly where truncation worked
     assert len(vectors[2].data.values) == len(vectors[3].data.values)
     assert np.allclose(vectors[2].data.values, vectors[3].data.values)
     for i in range(len(vectors[2].data.values)):
         assert approx(vectors[2].data.values[i]) == approx(vectors[3].data.values[i])
 
@@ -888,17 +912,26 @@
         # [CLS] 5 normal tokens [SEP]
         (["12345"], 5 + 2),
         # [CLS] 5 normal [SEP], [CLS] 4 normal [SEP] [PAD]
         (["12 345", "6 789"], 9 + 4),
     ],
 )
 def test_sum_token_count_no_truncation(texts, expected_count, loaded_model):
-    tokenized, _ = loaded_model.model._truncate_input_tokens(
-        truncate_input_tokens=-1,  # don't truncate. Model's truncation can still apply.
-        texts=texts,
+
+    tokenized = loaded_model.model.tokenizer(
+        texts,
+        return_attention_mask=True,
+        return_token_type_ids=False,
+        return_overflowing_tokens=True,
+        return_offsets_mapping=True,
+        return_length=True,
+        return_tensors="pt",
+        truncation=True,
+        padding=True,
+        max_length=loaded_model.model.max_seq_length,
     )
     token_count = sum_token_count(
         tokenized,
         truncate_only=False,
     )
 
     assert token_count == expected_count
@@ -920,54 +953,73 @@
         #
         # All encodings: [CLS] 123 [SEP] + [CLS] 45 [SEP] [PAD], [CLS] 678 [SEP] + [CLS] 9 [SEP] [PAD] [PAD]
         # Only truncated: [CLS] 123 [SEP] , [CLS] 678 [SEP]
         (["12 345", "6 789"], 5, (3 + 2) + (3 + 2)),
     ],
 )
 def test_sum_token_count_with_truncation(texts, truncate, expected_count, loaded_model):
-    tokenized, _ = loaded_model.model._truncate_input_tokens(
-        truncate_input_tokens=truncate,
-        texts=texts,
+    tokenized = loaded_model.model.tokenizer(
+        texts,
+        return_attention_mask=True,
+        return_token_type_ids=False,
+        return_overflowing_tokens=True,
+        return_offsets_mapping=True,
+        return_length=True,
+        return_tensors="pt",
+        truncation=True,
+        padding=True,
+        max_length=truncate,
     )
     token_count = sum_token_count(
         tokenized,
         truncate_only=True,
     )
 
     assert token_count == expected_count
 
 
-def test_encoding_order(loaded_model: EmbeddingModule):
+@pytest.mark.parametrize(
+    "truncate_input_tokens", [0, 1, 2, 3, 4, 99, 100, 101, 510, 511, 512, 513, -1]
+)
+def test_encoding_order(loaded_model: EmbeddingModule, truncate_input_tokens):
     """Confirm that encoding doesn't modify the original sort order"""
-    separate_embeddings = [loaded_model.run_embedding(text=i) for i in MANY_INPUTS]
-    combined_embeddings = loaded_model.run_embeddings(texts=MANY_INPUTS)
+    separate_embeddings = [
+        loaded_model.run_embedding(text=i, truncate_input_tokens=truncate_input_tokens)
+        for i in MANY_INPUTS
+    ]
+    combined_embeddings = loaded_model.run_embeddings(
+        texts=MANY_INPUTS, truncate_input_tokens=truncate_input_tokens
+    )
 
     separate_vectors = [
         e.to_dict()["result"]["data"]["values"] for e in separate_embeddings
     ]
     combined_vectors = [
         e["data"]["values"] for e in combined_embeddings.to_dict()["results"]["vectors"]
     ]
 
     assert len(separate_vectors) == len(
         combined_vectors
     ), "expected the same number separate and combined embeddings"
 
     # test order by comparing value of individual embeddings in sequence
     for i, e in enumerate(separate_vectors):
-        assert approx(e) == combined_vectors[i]
+        assert np.allclose(e, combined_vectors[i])
 
     # test expected failure case by reordering
     shifted_separate_vectors = separate_vectors[1:] + [separate_vectors[0]]
 
     for i, e in enumerate(shifted_separate_vectors):
         assert e != separate_vectors[i], "expected order to be have been altered"
         assert (
             not approx(e) == combined_vectors[i]
         ), "expected altered order to not match combined vectors"
+        assert not np.allclose(
+            e, combined_vectors[i]
+        ), "expected altered order to not match combined"
 
 
 @pytest.mark.parametrize(
     ("mapping", "expected"),
     [
         ([0, 0, 0, 0, 0], [0]),
         ([0, 1, 2, 3, 4], [0, 1, 2, 3, 4]),
```

### Comparing `caikit-nlp-0.4.7/tests/modules/text_generation/test_peft_config.py` & `caikit-nlp-0.4.8/tests/modules/text_generation/test_peft_config.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/modules/text_generation/test_peft_prompt_tuning.py` & `caikit-nlp-0.4.8/tests/modules/text_generation/test_peft_prompt_tuning.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/modules/text_generation/test_peft_tgis_remote.py` & `caikit-nlp-0.4.8/tests/modules/text_generation/test_peft_tgis_remote.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/modules/text_generation/test_text_generation_local.py` & `caikit-nlp-0.4.8/tests/modules/text_generation/test_text_generation_local.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/modules/text_generation/test_text_generation_tgis.py` & `caikit-nlp-0.4.8/tests/modules/text_generation/test_text_generation_tgis.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/modules/token_classification/test_filtered_span_classification.py` & `caikit-nlp-0.4.8/tests/modules/token_classification/test_filtered_span_classification.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/modules/tokenization/test_regex_sentence_splitter.py` & `caikit-nlp-0.4.8/tests/modules/tokenization/test_regex_sentence_splitter.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/resources/test_pretrained_model.py` & `caikit-nlp-0.4.8/tests/resources/test_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/toolkit/test_data_stream_wrapper.py` & `caikit-nlp-0.4.8/tests/toolkit/test_data_stream_wrapper.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/toolkit/test_data_type_utils.py` & `caikit-nlp-0.4.8/tests/toolkit/test_data_type_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/toolkit/test_task_specific_utils.py` & `caikit-nlp-0.4.8/tests/toolkit/test_task_specific_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/toolkit/test_verbalizers.py` & `caikit-nlp-0.4.8/tests/toolkit/test_verbalizers.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tests/toolkit/text_generation/test_model_run_utils.py` & `caikit-nlp-0.4.8/tests/toolkit/text_generation/test_model_run_utils.py`

 * *Files identical despite different names*

### Comparing `caikit-nlp-0.4.7/tox.ini` & `caikit-nlp-0.4.8/tox.ini`

 * *Files identical despite different names*

