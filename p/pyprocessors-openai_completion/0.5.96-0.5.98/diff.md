# Comparing `tmp/pyprocessors_openai_completion-0.5.96.tar.gz` & `tmp/pyprocessors_openai_completion-0.5.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyprocessors_openai_completion-0.5.96.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyprocessors_openai_completion-0.5.98.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyprocessors_openai_completion-0.5.96.tar` & `pyprocessors_openai_completion-0.5.98.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0       97 2023-08-21 14:11:22.567651 pyprocessors_openai_completion-0.5.96/.dockerignore
--rw-r--r--   0        0        0      178 2023-08-21 14:11:22.568651 pyprocessors_openai_completion-0.5.96/.gitignore
--rw-r--r--   0        0        0      448 2023-08-21 14:11:22.569651 pyprocessors_openai_completion-0.5.96/Dockerfile
--rw-r--r--   0        0        0    13510 2023-08-22 07:18:26.113970 pyprocessors_openai_completion-0.5.96/Jenkinsfile
--rw-r--r--   0        0        0      380 2023-08-21 14:11:22.570651 pyprocessors_openai_completion-0.5.96/README.md
--rw-r--r--   0        0        0     1559 2023-08-21 14:11:22.571651 pyprocessors_openai_completion-0.5.96/bumpversion.py
--rw-r--r--   0        0        0       56 2023-08-22 07:27:29.258599 pyprocessors_openai_completion-0.5.96/pyprocessors_openai_completion/__init__.py
--rw-r--r--   0        0        0    17425 2023-08-21 14:11:22.576651 pyprocessors_openai_completion-0.5.96/pyprocessors_openai_completion/openai_completion.py
--rw-r--r--   0        0        0     1923 2023-08-21 14:11:22.577651 pyprocessors_openai_completion-0.5.96/pyprocessors_openai_completion/retry_limit.py
--rw-r--r--   0        0        0     2594 2023-08-21 14:11:22.577651 pyprocessors_openai_completion-0.5.96/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-21 14:11:22.578651 pyprocessors_openai_completion-0.5.96/tests/__init__.py
--rw-r--r--   0        0        0      674 2023-08-21 14:11:22.578651 pyprocessors_openai_completion-0.5.96/tests/data/complexdoc.json
--rw-r--r--   0        0        0     3992 2023-08-21 14:11:22.581651 pyprocessors_openai_completion-0.5.96/tests/data/en_davinci-instruct-beta.json
--rw-r--r--   0        0        0     4868 2023-08-21 14:11:22.582651 pyprocessors_openai_completion-0.5.96/tests/data/en_gpt-3.5-turbo.json
--rw-r--r--   0        0        0     4716 2023-08-21 14:11:22.582651 pyprocessors_openai_completion-0.5.96/tests/data/en_gpt-4.json
--rw-r--r--   0        0        0     4141 2023-08-21 14:11:22.584651 pyprocessors_openai_completion-0.5.96/tests/data/en_text-ada-001.json
--rw-r--r--   0        0        0     3914 2023-08-21 14:11:22.585651 pyprocessors_openai_completion-0.5.96/tests/data/en_text-babbage-001.json
--rw-r--r--   0        0        0     4187 2023-08-21 14:11:22.586651 pyprocessors_openai_completion-0.5.96/tests/data/en_text-curie-001.json
--rw-r--r--   0        0        0     4182 2023-08-21 14:11:22.589651 pyprocessors_openai_completion-0.5.96/tests/data/en_text-davinci-003.json
--rw-r--r--   0        0        0     2202 2023-08-21 14:11:22.592651 pyprocessors_openai_completion-0.5.96/tests/data/fr_davinci-instruct-beta.json
--rw-r--r--   0        0        0     3207 2023-08-21 14:11:22.592651 pyprocessors_openai_completion-0.5.96/tests/data/fr_gpt-3.5-turbo.json
--rw-r--r--   0        0        0     2560 2023-08-21 14:11:22.593651 pyprocessors_openai_completion-0.5.96/tests/data/fr_gpt-4.json
--rw-r--r--   0        0        0     2295 2023-08-21 14:11:22.593651 pyprocessors_openai_completion-0.5.96/tests/data/fr_text-ada-001.json
--rw-r--r--   0        0        0     1699 2023-08-21 14:11:22.594651 pyprocessors_openai_completion-0.5.96/tests/data/fr_text-babbage-001.json
--rw-r--r--   0        0        0     1823 2023-08-21 14:11:22.594651 pyprocessors_openai_completion-0.5.96/tests/data/fr_text-curie-001.json
--rw-r--r--   0        0        0     2366 2023-08-21 14:11:22.594651 pyprocessors_openai_completion-0.5.96/tests/data/fr_text-davinci-003.json
--rw-r--r--   0        0        0     8421 2023-08-21 14:11:22.595651 pyprocessors_openai_completion-0.5.96/tests/data/jinjadocs.json
--rw-r--r--   0        0        0    13529 2023-08-21 14:11:22.595651 pyprocessors_openai_completion-0.5.96/tests/data/jinjadocs_preserve_entities.json
--rw-r--r--   0        0        0    14427 2023-08-21 14:11:22.596651 pyprocessors_openai_completion-0.5.96/tests/data/jinjadocs_substitute_entities.json
--rw-r--r--   0        0        0     5070 2023-08-21 14:11:22.597651 pyprocessors_openai_completion-0.5.96/tests/data/question_segments.json
--rw-r--r--   0        0        0     1219 2023-08-21 14:11:22.598651 pyprocessors_openai_completion-0.5.96/tests/data/question_segments_answer.json
--rw-r--r--   0        0        0    13876 2023-08-21 14:11:22.598651 pyprocessors_openai_completion-0.5.96/tests/test_openai_completion.py
--rw-r--r--   0        0        0      951 2023-08-21 14:11:22.599651 pyprocessors_openai_completion-0.5.96/tox.ini
--rw-r--r--   0        0        0     1340 1970-01-01 00:00:00.000000 pyprocessors_openai_completion-0.5.96/setup.py
--rw-r--r--   0        0        0     2529 1970-01-01 00:00:00.000000 pyprocessors_openai_completion-0.5.96/PKG-INFO
+-rw-r--r--   0        0        0       97 2023-08-21 14:11:22.567651 pyprocessors_openai_completion-0.5.98/.dockerignore
+-rw-r--r--   0        0        0      178 2023-08-21 14:11:22.568651 pyprocessors_openai_completion-0.5.98/.gitignore
+-rw-r--r--   0        0        0      448 2023-08-21 14:11:22.569651 pyprocessors_openai_completion-0.5.98/Dockerfile
+-rw-r--r--   0        0        0    13547 2023-08-25 23:45:42.427552 pyprocessors_openai_completion-0.5.98/Jenkinsfile
+-rw-r--r--   0        0        0      380 2023-08-21 14:11:22.570651 pyprocessors_openai_completion-0.5.98/README.md
+-rw-r--r--   0        0        0     1559 2023-08-21 14:11:22.571651 pyprocessors_openai_completion-0.5.98/bumpversion.py
+-rw-r--r--   0        0        0       56 2023-08-25 23:49:27.452919 pyprocessors_openai_completion-0.5.98/pyprocessors_openai_completion/__init__.py
+-rw-r--r--   0        0        0    17425 2023-08-21 14:11:22.576651 pyprocessors_openai_completion-0.5.98/pyprocessors_openai_completion/openai_completion.py
+-rw-r--r--   0        0        0     1923 2023-08-21 14:11:22.577651 pyprocessors_openai_completion-0.5.98/pyprocessors_openai_completion/retry_limit.py
+-rw-r--r--   0        0        0     2594 2023-08-21 14:11:22.577651 pyprocessors_openai_completion-0.5.98/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-21 14:11:22.578651 pyprocessors_openai_completion-0.5.98/tests/__init__.py
+-rw-r--r--   0        0        0      674 2023-08-21 14:11:22.578651 pyprocessors_openai_completion-0.5.98/tests/data/complexdoc.json
+-rw-r--r--   0        0        0     3992 2023-08-21 14:11:22.581651 pyprocessors_openai_completion-0.5.98/tests/data/en_davinci-instruct-beta.json
+-rw-r--r--   0        0        0     4868 2023-08-21 14:11:22.582651 pyprocessors_openai_completion-0.5.98/tests/data/en_gpt-3.5-turbo.json
+-rw-r--r--   0        0        0     4716 2023-08-21 14:11:22.582651 pyprocessors_openai_completion-0.5.98/tests/data/en_gpt-4.json
+-rw-r--r--   0        0        0     4141 2023-08-21 14:11:22.584651 pyprocessors_openai_completion-0.5.98/tests/data/en_text-ada-001.json
+-rw-r--r--   0        0        0     3914 2023-08-21 14:11:22.585651 pyprocessors_openai_completion-0.5.98/tests/data/en_text-babbage-001.json
+-rw-r--r--   0        0        0     4187 2023-08-21 14:11:22.586651 pyprocessors_openai_completion-0.5.98/tests/data/en_text-curie-001.json
+-rw-r--r--   0        0        0     4182 2023-08-21 14:11:22.589651 pyprocessors_openai_completion-0.5.98/tests/data/en_text-davinci-003.json
+-rw-r--r--   0        0        0     2202 2023-08-21 14:11:22.592651 pyprocessors_openai_completion-0.5.98/tests/data/fr_davinci-instruct-beta.json
+-rw-r--r--   0        0        0     3207 2023-08-21 14:11:22.592651 pyprocessors_openai_completion-0.5.98/tests/data/fr_gpt-3.5-turbo.json
+-rw-r--r--   0        0        0     2560 2023-08-21 14:11:22.593651 pyprocessors_openai_completion-0.5.98/tests/data/fr_gpt-4.json
+-rw-r--r--   0        0        0     2295 2023-08-21 14:11:22.593651 pyprocessors_openai_completion-0.5.98/tests/data/fr_text-ada-001.json
+-rw-r--r--   0        0        0     1699 2023-08-21 14:11:22.594651 pyprocessors_openai_completion-0.5.98/tests/data/fr_text-babbage-001.json
+-rw-r--r--   0        0        0     1823 2023-08-21 14:11:22.594651 pyprocessors_openai_completion-0.5.98/tests/data/fr_text-curie-001.json
+-rw-r--r--   0        0        0     2366 2023-08-21 14:11:22.594651 pyprocessors_openai_completion-0.5.98/tests/data/fr_text-davinci-003.json
+-rw-r--r--   0        0        0     8421 2023-08-21 14:11:22.595651 pyprocessors_openai_completion-0.5.98/tests/data/jinjadocs.json
+-rw-r--r--   0        0        0    13529 2023-08-21 14:11:22.595651 pyprocessors_openai_completion-0.5.98/tests/data/jinjadocs_preserve_entities.json
+-rw-r--r--   0        0        0    14427 2023-08-21 14:11:22.596651 pyprocessors_openai_completion-0.5.98/tests/data/jinjadocs_substitute_entities.json
+-rw-r--r--   0        0        0     5070 2023-08-21 14:11:22.597651 pyprocessors_openai_completion-0.5.98/tests/data/question_segments.json
+-rw-r--r--   0        0        0     1219 2023-08-21 14:11:22.598651 pyprocessors_openai_completion-0.5.98/tests/data/question_segments_answer.json
+-rw-r--r--   0        0        0    13876 2023-08-21 14:11:22.598651 pyprocessors_openai_completion-0.5.98/tests/test_openai_completion.py
+-rw-r--r--   0        0        0      951 2023-08-21 14:11:22.599651 pyprocessors_openai_completion-0.5.98/tox.ini
+-rw-r--r--   0        0        0     1340 1970-01-01 00:00:00.000000 pyprocessors_openai_completion-0.5.98/setup.py
+-rw-r--r--   0        0        0     2529 1970-01-01 00:00:00.000000 pyprocessors_openai_completion-0.5.98/PKG-INFO
```

### Comparing `pyprocessors_openai_completion-0.5.96/Jenkinsfile` & `pyprocessors_openai_completion-0.5.98/Jenkinsfile`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,15 @@
           }
         }
       }
     }
 
     stage('Build, test and publish') {
       when {
+        beforeAgent true
         environment name: 'SKIP_JOB', value: '0'
       }
 
       agent {
         // dockerfile agent
         // Mounted volume for Junit reports
         //   - docker: /root/test-reports
@@ -155,20 +156,20 @@
         // keep using customWorkspace to store Junit report
         ws("/home/jenkins/${JOB_NAME}") {
           script {
             try {
               sh 'rm -f results.xml'
               sh "cp /tmp/_${JOB_NAME}/test-reports/results.xml results.xml"
             } catch (Exception e) {
-              echo 'Exception occurred: ' + e.toString()
+              println 'Exception occurred: ' + e.toString()
             }
             try {
               junit 'results.xml'
             } catch (Exception e) {
-              echo 'Exception occurred: ' + e.toString()
+              println 'Exception occurred: ' + e.toString()
             }
             if (sendEmailNotif("/home/jenkins/${JOB_NAME}", "${BUILD_NUMBER}")) {
               println 'sending Success Build notification'
               CUSTOM_SUBJECT = '[CI - Jenkinzz SUCCESS] ' + CUSTOM_SUBJECT
               emailext(
                   mimeType: 'text/html',
                   subject: CUSTOM_SUBJECT,
@@ -191,20 +192,20 @@
         // keep using customWorkspace to store Junit report
         ws("/home/jenkins/${JOB_NAME}") {
           script {
             try {
               sh 'rm -f results.xml'
               sh "cp /tmp/_${JOB_NAME}/test-reports/results.xml results.xml"
             } catch (Exception e) {
-              echo 'Exception occurred: ' + e.toString()
+              println 'Exception occurred: ' + e.toString()
             }
             try {
               junit 'results.xml'
             } catch (Exception e) {
-              echo 'Exception occurred: ' + e.toString()
+              println 'Exception occurred: ' + e.toString()
             }
             println 'sending Failure Build notification'
             CUSTOM_SUBJECT = '[CI - Jenkinzz FAILURE] ' + CUSTOM_SUBJECT
             emailext(
                 mimeType: 'text/html',
                 subject: CUSTOM_SUBJECT,
                 body: '${DEFAULT_CONTENT}',
```

### Comparing `pyprocessors_openai_completion-0.5.96/bumpversion.py` & `pyprocessors_openai_completion-0.5.98/bumpversion.py`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.96/pyprocessors_openai_completion/openai_completion.py` & `pyprocessors_openai_completion-0.5.98/pyprocessors_openai_completion/openai_completion.py`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.96/pyprocessors_openai_completion/retry_limit.py` & `pyprocessors_openai_completion-0.5.98/pyprocessors_openai_completion/retry_limit.py`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.96/pyproject.toml` & `pyprocessors_openai_completion-0.5.98/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.96/tests/data/complexdoc.json` & `pyprocessors_openai_completion-0.5.98/tests/data/complexdoc.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.96/tests/data/en_davinci-instruct-beta.json` & `pyprocessors_openai_completion-0.5.98/tests/data/en_davinci-instruct-beta.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.96/tests/data/en_gpt-3.5-turbo.json` & `pyprocessors_openai_completion-0.5.98/tests/data/en_gpt-3.5-turbo.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.96/tests/data/en_gpt-4.json` & `pyprocessors_openai_completion-0.5.98/tests/data/en_gpt-4.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.96/tests/data/en_text-ada-001.json` & `pyprocessors_openai_completion-0.5.98/tests/data/en_text-ada-001.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.96/tests/data/en_text-babbage-001.json` & `pyprocessors_openai_completion-0.5.98/tests/data/en_text-babbage-001.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.96/tests/data/en_text-curie-001.json` & `pyprocessors_openai_completion-0.5.98/tests/data/en_text-curie-001.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.96/tests/data/en_text-davinci-003.json` & `pyprocessors_openai_completion-0.5.98/tests/data/en_text-davinci-003.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.96/tests/data/fr_davinci-instruct-beta.json` & `pyprocessors_openai_completion-0.5.98/tests/data/fr_davinci-instruct-beta.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.96/tests/data/fr_gpt-3.5-turbo.json` & `pyprocessors_openai_completion-0.5.98/tests/data/fr_gpt-3.5-turbo.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.96/tests/data/fr_gpt-4.json` & `pyprocessors_openai_completion-0.5.98/tests/data/fr_gpt-4.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.96/tests/data/fr_text-ada-001.json` & `pyprocessors_openai_completion-0.5.98/tests/data/fr_text-ada-001.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.96/tests/data/fr_text-babbage-001.json` & `pyprocessors_openai_completion-0.5.98/tests/data/fr_text-babbage-001.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.96/tests/data/fr_text-curie-001.json` & `pyprocessors_openai_completion-0.5.98/tests/data/fr_text-curie-001.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.96/tests/data/fr_text-davinci-003.json` & `pyprocessors_openai_completion-0.5.98/tests/data/fr_text-davinci-003.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.96/tests/data/jinjadocs.json` & `pyprocessors_openai_completion-0.5.98/tests/data/jinjadocs.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.96/tests/data/jinjadocs_preserve_entities.json` & `pyprocessors_openai_completion-0.5.98/tests/data/jinjadocs_preserve_entities.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.96/tests/data/jinjadocs_substitute_entities.json` & `pyprocessors_openai_completion-0.5.98/tests/data/jinjadocs_substitute_entities.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.96/tests/data/question_segments.json` & `pyprocessors_openai_completion-0.5.98/tests/data/question_segments.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.96/tests/data/question_segments_answer.json` & `pyprocessors_openai_completion-0.5.98/tests/data/question_segments_answer.json`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.96/tests/test_openai_completion.py` & `pyprocessors_openai_completion-0.5.98/tests/test_openai_completion.py`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.96/tox.ini` & `pyprocessors_openai_completion-0.5.98/tox.ini`

 * *Files identical despite different names*

### Comparing `pyprocessors_openai_completion-0.5.96/setup.py` & `pyprocessors_openai_completion-0.5.98/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
           'flask==2.1.3']}
 
 entry_points = \
 {'pyprocessors.plugins': ['openai_completion = '
                           'pyprocessors_openai_completion.openai_completion:OpenAICompletionProcessor']}
 
 setup(name='pyprocessors-openai_completion',
-      version='0.5.96',
+      version='0.5.98',
       description='OpenAICompletion processor',
       author='Olivier Terrier',
       author_email='olivier.terrier@kairntech.com',
       url='https://kairntech.com/',
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `pyprocessors_openai_completion-0.5.96/PKG-INFO` & `pyprocessors_openai_completion-0.5.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyprocessors-openai_completion
-Version: 0.5.96
+Version: 0.5.98
 Summary: OpenAICompletion processor
 Home-page: https://kairntech.com/
 Author: Olivier Terrier
 Author-email: olivier.terrier@kairntech.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
```

