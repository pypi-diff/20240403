# Comparing `tmp/dcm_classifier-0.7.0rc1.tar.gz` & `tmp/dcm_classifier-0.7.0rc2.tar.gz`

## Comparing `dcm_classifier-0.7.0rc1.tar` & `dcm_classifier-0.7.0rc2.tar`

### file list

```diff
@@ -1,52 +1,53 @@
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/.git
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/push_pip.sh
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/requirements.txt
--rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/requirements_dev.txt
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/.github/ISSUE_TEMPLATE/chore-template.md
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/.github/ISSUE_TEMPLATE/documentation_improvement.md
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/models/ova_rf_classifier.onnx
--rw-r--r--   0        0        0   197260 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/models/rf_classifier.onnx
--rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/scripts/anonymize_dicom_directory.py
--rw-r--r--   0        0        0     5103 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/scripts/classify_study.py
--rw-r--r--   0        0        0     7627 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/scripts/create_dicom_fields_sheet.py
--rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/scripts/create_training_sheet.py
--rw-r--r--   0        0        0    17402 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/scripts/dcm-classifier-training-tutorial.ipynb
--rw-r--r--   0        0        0    22366 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/scripts/modality_classifier_training.py
--rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/scripts/organize_dicom_to_bids.py
--rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/scripts/orientation_model_training.py
--rwxr-xr-x   0        0        0      796 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/scripts/run_all_dicom_data_sheets.sh
--rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/scripts/running_classifier.ipynb
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/scripts/todo_list
--rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/scripts/training_config.py
--rw-r--r--   0        0        0     7348 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/scripts/utilities.py
--rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/src/dcm_classifier/README.md
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/src/dcm_classifier/__init__.py
--rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/src/dcm_classifier/dicom_config.py
--rw-r--r--   0        0        0    11127 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/src/dcm_classifier/dicom_series.py
--rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/src/dcm_classifier/dicom_validator.py
--rw-r--r--   0        0        0    18769 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/src/dcm_classifier/dicom_volume.py
--rw-r--r--   0        0        0    22684 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/src/dcm_classifier/example_image_processing.py
--rw-r--r--   0        0        0    17904 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/src/dcm_classifier/image_type_inference.py
--rw-r--r--   0        0        0    16845 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/src/dcm_classifier/study_processing.py
--rw-r--r--   0        0        0    32251 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/src/dcm_classifier/utility_functions.py
--rw-r--r--   0        0        0     8871 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/tests/conftest.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/tests/testing_data/.gitignore
--rw-r--r--   0        0        0  2200109 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/tests/testing_data/anonymized_testing_data.tar.gz
--rw-r--r--   0        0        0   190042 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/tests/testing_data/mock_data.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/tests/testing_data/dummy_directory/dir_with_one_file/00.file
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/tests/testing_data/dummy_directory/dir_with_two_files/100.file
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/tests/testing_data/dummy_directory/dir_with_two_files/200.file
--rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/tests/unit_testing/test_dicom_series.py
--rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/tests/unit_testing/test_dicom_validator.py
--rw-r--r--   0        0        0     9894 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/tests/unit_testing/test_dicom_volume.py
--rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/tests/unit_testing/test_study_processing.py
--rw-r--r--   0        0        0    11288 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/tests/unit_testing/test_utility_functions.py
--rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/.gitignore
--rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/LICENSE
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/README.md
--rw-r--r--   0        0        0     1305 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/pyproject.toml
--rw-r--r--   0        0        0     2800 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/push_pip.sh
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/requirements.txt
+-rw-r--r--   0        0        0      387 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/requirements_dev.txt
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/.github/ISSUE_TEMPLATE/chore-template.md
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/.github/ISSUE_TEMPLATE/documentation_improvement.md
+-rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/.github/workflows/push_to_main.yml
+-rw-r--r--   0        0        0   312427 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/models/ova_rf_classifier.onnx
+-rw-r--r--   0        0        0   197260 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/models/rf_classifier.onnx
+-rw-r--r--   0        0        0     2629 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/scripts/anonymize_dicom_directory.py
+-rw-r--r--   0        0        0     5098 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/scripts/classify_study.py
+-rw-r--r--   0        0        0     7627 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/scripts/create_dicom_fields_sheet.py
+-rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/scripts/create_training_sheet.py
+-rw-r--r--   0        0        0    17402 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/scripts/dcm-classifier-training-tutorial.ipynb
+-rw-r--r--   0        0        0    22366 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/scripts/modality_classifier_training.py
+-rw-r--r--   0        0        0     3037 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/scripts/organize_dicom_to_bids.py
+-rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/scripts/orientation_model_training.py
+-rwxr-xr-x   0        0        0      934 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/scripts/run_all_dicom_data_sheets.sh
+-rw-r--r--   0        0        0    11770 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/scripts/running_classifier.ipynb
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/scripts/todo_list
+-rw-r--r--   0        0        0    11826 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/scripts/training_config.py
+-rw-r--r--   0        0        0     7348 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/scripts/utilities.py
+-rw-r--r--   0        0        0      194 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/src/dcm_classifier/README.md
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/src/dcm_classifier/__init__.py
+-rw-r--r--   0        0        0     2990 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/src/dcm_classifier/dicom_config.py
+-rw-r--r--   0        0        0    11127 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/src/dcm_classifier/dicom_series.py
+-rw-r--r--   0        0        0     4663 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/src/dcm_classifier/dicom_validator.py
+-rw-r--r--   0        0        0    18769 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/src/dcm_classifier/dicom_volume.py
+-rw-r--r--   0        0        0    22684 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/src/dcm_classifier/example_image_processing.py
+-rw-r--r--   0        0        0    17904 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/src/dcm_classifier/image_type_inference.py
+-rw-r--r--   0        0        0    16845 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/src/dcm_classifier/study_processing.py
+-rw-r--r--   0        0        0    32251 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/src/dcm_classifier/utility_functions.py
+-rw-r--r--   0        0        0     8871 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/tests/conftest.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/tests/testing_data/.gitignore
+-rw-r--r--   0        0        0  2200109 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/tests/testing_data/anonymized_testing_data.tar.gz
+-rw-r--r--   0        0        0   190042 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/tests/testing_data/mock_data.txt
+-rw-r--r--   0        0        0     1130 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/tests/testing_data/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/tests/testing_data/dummy_directory/dir_with_one_file/00.file
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/tests/testing_data/dummy_directory/dir_with_two_files/100.file
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/tests/testing_data/dummy_directory/dir_with_two_files/200.file
+-rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/tests/unit_testing/test_dicom_series.py
+-rw-r--r--   0        0        0     1912 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/tests/unit_testing/test_dicom_validator.py
+-rw-r--r--   0        0        0     9894 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/tests/unit_testing/test_dicom_volume.py
+-rw-r--r--   0        0        0     4276 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/tests/unit_testing/test_study_processing.py
+-rw-r--r--   0        0        0    11309 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/tests/unit_testing/test_utility_functions.py
+-rw-r--r--   0        0        0     6694 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/.gitignore
+-rw-r--r--   0        0        0    11362 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/LICENSE
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/README.md
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/pyproject.toml
+-rw-r--r--   0        0        0     3148 2020-02-02 00:00:00.000000 dcm_classifier-0.7.0rc2/PKG-INFO
```

### Comparing `dcm_classifier-0.7.0rc1/.pre-commit-config.yaml` & `dcm_classifier-0.7.0rc2/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,17 @@
       - id: check-yaml
       - id: detect-private-key
       - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: name-tests-test
         args: ['--pytest-test-first']
       - id: trailing-whitespace
+      - id: check-added-large-files
+      - id: requirements-txt-fixer
+      - id: check-ast
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
     # Ruff version.
     rev: v0.2.1
 
     hooks:
       # Run the linter.
```

### Comparing `dcm_classifier-0.7.0rc1/.github/PULL_REQUEST_TEMPLATE.md` & `dcm_classifier-0.7.0rc2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Overview
 <!-- _What is the purpose of this pull request?_ -->
 
 # Implementation
-<!-- 
+<!--
 _What items were implemented?_
 _What are their key components and functionality?_
 _What does this add to the overall project?_
 _How do you use this new functionality? (if applicable)_
 -->
 
 # Testing
@@ -17,12 +17,12 @@
 _Where are these documented?_
 -->
 
 # Problems Faced
 <!-- _Did you run into any problems, if so how did you resolve them? -->
 
 # Notes
-<!-- 
+<!--
 _Any screenshots/videos demonstrating the functioning of the changes made in this pull request?_
 _Is there any other important notes related to this pull request?
 
 -->
```

### Comparing `dcm_classifier-0.7.0rc1/.github/ISSUE_TEMPLATE/bug_report.md` & `dcm_classifier-0.7.0rc2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/.github/ISSUE_TEMPLATE/documentation_improvement.md` & `dcm_classifier-0.7.0rc2/.github/ISSUE_TEMPLATE/documentation_improvement.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/.github/ISSUE_TEMPLATE/feature_request.md` & `dcm_classifier-0.7.0rc2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/models/ova_rf_classifier.onnx` & `dcm_classifier-0.7.0rc2/models/ova_rf_classifier.onnx`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/models/rf_classifier.onnx` & `dcm_classifier-0.7.0rc2/models/rf_classifier.onnx`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/scripts/anonymize_dicom_directory.py` & `dcm_classifier-0.7.0rc2/scripts/anonymize_dicom_directory.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/scripts/classify_study.py` & `dcm_classifier-0.7.0rc2/scripts/classify_study.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
             current_dict["Series Modality"] = str(series.get_series_modality())
             current_dict["Acq.Plane"] = str(volume.get_acquisition_plane())
             current_dict["Isotropic"] = str(volume.get_is_isotropic())
             print(volume.get_modality_probabilities().to_string(index=False))
             current_dict["Bvalue"] = str(volume.get_volume_bvalue())
             try:
                 current_dict["SeriesDesc"] = volume.get_volume_series_description()
-            except AttributeError as e:
+            except AttributeError:
                 current_dict["SeriesDesc"] = "None"
             inputs_df: dict[str, Any] = volume.get_volume_dictionary()
             current_dict["ImageType"] = str(inputs_df.get("ImageType", "Unknown"))
             for unwanted in [
                 "FileName",
                 "StudyInstanceUID",
                 "SeriesInstanceUID",
```

### Comparing `dcm_classifier-0.7.0rc1/scripts/create_dicom_fields_sheet.py` & `dcm_classifier-0.7.0rc2/scripts/create_dicom_fields_sheet.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/scripts/create_training_sheet.py` & `dcm_classifier-0.7.0rc2/scripts/create_training_sheet.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/scripts/dcm-classifier-training-tutorial.ipynb` & `dcm_classifier-0.7.0rc2/scripts/dcm-classifier-training-tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/scripts/modality_classifier_training.py` & `dcm_classifier-0.7.0rc2/scripts/modality_classifier_training.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/scripts/organize_dicom_to_bids.py` & `dcm_classifier-0.7.0rc2/scripts/organize_dicom_to_bids.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/scripts/orientation_model_training.py` & `dcm_classifier-0.7.0rc2/scripts/orientation_model_training.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/scripts/running_classifier.ipynb` & `dcm_classifier-0.7.0rc2/scripts/running_classifier.ipynb`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/scripts/todo_list` & `dcm_classifier-0.7.0rc2/scripts/todo_list`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/scripts/training_config.py` & `dcm_classifier-0.7.0rc2/scripts/training_config.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/scripts/utilities.py` & `dcm_classifier-0.7.0rc2/scripts/utilities.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/src/dcm_classifier/dicom_config.py` & `dcm_classifier-0.7.0rc2/src/dcm_classifier/dicom_config.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/src/dcm_classifier/dicom_series.py` & `dcm_classifier-0.7.0rc2/src/dcm_classifier/dicom_series.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/src/dcm_classifier/dicom_validator.py` & `dcm_classifier-0.7.0rc2/src/dcm_classifier/dicom_validator.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/src/dcm_classifier/dicom_volume.py` & `dcm_classifier-0.7.0rc2/src/dcm_classifier/dicom_volume.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/src/dcm_classifier/example_image_processing.py` & `dcm_classifier-0.7.0rc2/src/dcm_classifier/example_image_processing.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/src/dcm_classifier/image_type_inference.py` & `dcm_classifier-0.7.0rc2/src/dcm_classifier/image_type_inference.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/src/dcm_classifier/study_processing.py` & `dcm_classifier-0.7.0rc2/src/dcm_classifier/study_processing.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/src/dcm_classifier/utility_functions.py` & `dcm_classifier-0.7.0rc2/src/dcm_classifier/utility_functions.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/tests/conftest.py` & `dcm_classifier-0.7.0rc2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/tests/testing_data/anonymized_testing_data.tar.gz` & `dcm_classifier-0.7.0rc2/tests/testing_data/anonymized_testing_data.tar.gz`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/tests/testing_data/mock_data.txt` & `dcm_classifier-0.7.0rc2/tests/testing_data/mock_data.txt`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/tests/unit_testing/test_dicom_series.py` & `dcm_classifier-0.7.0rc2/tests/unit_testing/test_dicom_series.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         with pytest.raises(ValueError) as ex:
             series.set_is_isotropic(4)
         assert "ERROR: " in str(ex.value)
 
 
 def test_get_is_isotropic(mock_tracew_series):
     for series in mock_tracew_series:
-        assert series.get_is_isotropic() == False
+        assert series.get_is_isotropic() is False
 
 
 def test_set_invalid_contrast(mock_tracew_series):
     for series in mock_tracew_series:
         with pytest.raises(ValueError) as ex:
             series.set_has_contrast(4)
         assert "ERROR: " in str(ex.value)
```

### Comparing `dcm_classifier-0.7.0rc1/tests/unit_testing/test_dicom_validator.py` & `dcm_classifier-0.7.0rc2/tests/unit_testing/test_dicom_validator.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/tests/unit_testing/test_dicom_volume.py` & `dcm_classifier-0.7.0rc2/tests/unit_testing/test_dicom_volume.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/tests/unit_testing/test_study_processing.py` & `dcm_classifier-0.7.0rc2/tests/unit_testing/test_study_processing.py`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/tests/unit_testing/test_utility_functions.py` & `dcm_classifier-0.7.0rc2/tests/unit_testing/test_utility_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
 import pydicom
 import pytest
 from dcm_classifier.example_image_processing import slugify, rglob_for_singular_result
-from dcm_classifier.image_type_inference import *
+from dcm_classifier.image_type_inference import ImageTypeClassifierBase
 from dcm_classifier.study_processing import ProcessOneDicomStudyToVolumesMappingBase
 from dcm_classifier.utility_functions import (
     vprint,
     get_diffusion_gradient_direction,
     convert_array_to_min_max,
     sanitize_dicom_dataset,
     itk_read_from_dicomfn_list,
@@ -353,8 +353,7 @@
     assert get_coded_dictionary_elements(test_dict) == {}
 
 
 def test_get_EADC_image_type():
     test_dict = {"ImageType": ["ORIGINAL", "PRIMARY", "EADC", "NONE"]}
 
     assert get_coded_dictionary_elements(test_dict)["ImageType_EADC"] == 1
-
```

### Comparing `dcm_classifier-0.7.0rc1/.gitignore` & `dcm_classifier-0.7.0rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/LICENSE` & `dcm_classifier-0.7.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/README.md` & `dcm_classifier-0.7.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `dcm_classifier-0.7.0rc1/pyproject.toml` & `dcm_classifier-0.7.0rc2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,38 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dcm_classifier"
-version = '0.7.0.rc1'
+version = '0.7.0.rc2'
 authors = [
   { name="Michal Brzus", email="michal-brzus@uiowa.edu" },
   { name="Hans Johnson", email="hans-johnson@uiowa.edu" },
 ]
 description = "This is a consolidation of work from NAMIC efforts primarily at the University of Iowa."
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "itk>=5.3.0",
+    "itk-core>=5.3.0",
+    "itk-filtering>=5.3.0",
+    "itk-io>=5.3.0",
+    "itk-numerics>=5.3.0",
+    "onnxruntime>=1.16.2",
+    "pandas>=1.4.0",
+    "pyarrow>=6.0.0",
+    "pydicom>=2.2.0",
+    "python-gdcm>=3.0.10", # NOTE: python-gdcm replaces pylibjpeg for plugin support for pydicom
+    "tabulate>=0.9.0",
+]
 
 [tool.pytest.ini_options]
 minversion = "7.2"
 pythonpath = [
   "src",
   "src/dcm_classifier"
 ]
```

### Comparing `dcm_classifier-0.7.0rc1/PKG-INFO` & `dcm_classifier-0.7.0rc2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,27 @@
 Metadata-Version: 2.3
 Name: dcm_classifier
-Version: 0.7.0rc1
+Version: 0.7.0rc2
 Summary: This is a consolidation of work from NAMIC efforts primarily at the University of Iowa.
 Author-email: Michal Brzus <michal-brzus@uiowa.edu>, Hans Johnson <hans-johnson@uiowa.edu>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.9
+Requires-Python: >=3.10
+Requires-Dist: itk-core>=5.3.0
+Requires-Dist: itk-filtering>=5.3.0
+Requires-Dist: itk-io>=5.3.0
+Requires-Dist: itk-numerics>=5.3.0
+Requires-Dist: itk>=5.3.0
+Requires-Dist: onnxruntime>=1.16.2
+Requires-Dist: pandas>=1.4.0
+Requires-Dist: pyarrow>=6.0.0
+Requires-Dist: pydicom>=2.2.0
+Requires-Dist: python-gdcm>=3.0.10
+Requires-Dist: tabulate>=0.9.0
 Description-Content-Type: text/markdown
 
 # Introduction
 
 In this work, we developed a robust, easily extensible classification framework that extracts key features from well-characterized DICOM header fields for identifying image modality and acquisition plane. Our tool is crucial for eliminating error-prone human interaction and allowing automatization, increasing imaging applications' reliability and efficiency. We used Random Forrest and Decision Tree algorithms to determine the image modality and orientation. We trained on header meta-data of over 49000 scan volumes from multiple studies and achieved over 99% prediction accuracy on image modality and acquisition plane classification.
 
 This project was supported by several funding sources including:
```

