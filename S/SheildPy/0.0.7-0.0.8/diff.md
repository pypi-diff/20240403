# Comparing `tmp/SheildPy-0.0.7.tar.gz` & `tmp/SheildPy-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SheildPy-0.0.7.tar", last modified: Tue Apr  2 16:48:17 2024, max compression
+gzip compressed data, was "SheildPy-0.0.8.tar", last modified: Wed Apr  3 00:33:44 2024, max compression
```

## Comparing `SheildPy-0.0.7.tar` & `SheildPy-0.0.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:48:17.911400 SheildPy-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-02 16:47:48.000000 SheildPy-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-02 16:48:17.911400 SheildPy-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-02 16:47:48.000000 SheildPy-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-02 16:47:48.000000 SheildPy-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-02 16:48:17.911400 SheildPy-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-02 16:47:48.000000 SheildPy-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:48:17.907400 SheildPy-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:48:17.907400 SheildPy-0.0.7/src/SecuPy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 16:47:48.000000 SheildPy-0.0.7/src/SecuPy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-02 16:47:48.000000 SheildPy-0.0.7/src/SecuPy/access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-02 16:47:48.000000 SheildPy-0.0.7/src/SecuPy/auditing.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-02 16:47:48.000000 SheildPy-0.0.7/src/SecuPy/compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-02 16:47:48.000000 SheildPy-0.0.7/src/SecuPy/data_privacy_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-02 16:47:48.000000 SheildPy-0.0.7/src/SecuPy/documentation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 16:48:17.911400 SheildPy-0.0.7/src/SheildPy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-02 16:48:17.000000 SheildPy-0.0.7/src/SheildPy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-02 16:48:17.000000 SheildPy-0.0.7/src/SheildPy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 16:48:17.000000 SheildPy-0.0.7/src/SheildPy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-02 16:48:17.000000 SheildPy-0.0.7/src/SheildPy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 16:48:17.000000 SheildPy-0.0.7/src/SheildPy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:33:44.039643 SheildPy-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-03 00:33:20.000000 SheildPy-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-04-03 00:33:44.039643 SheildPy-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2024-04-03 00:33:20.000000 SheildPy-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-03 00:33:20.000000 SheildPy-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-03 00:33:44.043643 SheildPy-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-04-03 00:33:20.000000 SheildPy-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:33:44.039643 SheildPy-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:33:44.039643 SheildPy-0.0.8/src/SecuPy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 00:33:20.000000 SheildPy-0.0.8/src/SecuPy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-03 00:33:20.000000 SheildPy-0.0.8/src/SecuPy/access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-03 00:33:20.000000 SheildPy-0.0.8/src/SecuPy/auditing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-03 00:33:20.000000 SheildPy-0.0.8/src/SecuPy/compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-03 00:33:20.000000 SheildPy-0.0.8/src/SecuPy/data_privacy_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-03 00:33:20.000000 SheildPy-0.0.8/src/SecuPy/documentation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:33:44.039643 SheildPy-0.0.8/src/SheildPy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5645 2024-04-03 00:33:44.000000 SheildPy-0.0.8/src/SheildPy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-03 00:33:44.000000 SheildPy-0.0.8/src/SheildPy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 00:33:44.000000 SheildPy-0.0.8/src/SheildPy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-03 00:33:44.000000 SheildPy-0.0.8/src/SheildPy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 00:33:44.000000 SheildPy-0.0.8/src/SheildPy.egg-info/top_level.txt
```

### Comparing `SheildPy-0.0.7/LICENSE` & `SheildPy-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `SheildPy-0.0.7/PKG-INFO` & `SheildPy-0.0.8/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,30 @@
-Metadata-Version: 2.1
-Name: SheildPy
-Version: 0.0.7
-Summary: Protect sensitive data with SheildPy, a Python package offering encryption, anonymization, and compliance tools for data scientists.
-Home-page: https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists
-Author: DeependraVerma
-Author-email: deependra.verma00@gmail.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/issues
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Operating System :: OS Independent
-License-File: LICENSE
-Requires-Dist: pandas
-Requires-Dist: faker
-Requires-Dist: cryptography
-Provides-Extra: testing
-Requires-Dist: pytest>=7.1.3; extra == "testing"
-Requires-Dist: mypy>=0.971; extra == "testing"
-Requires-Dist: flake8>=5.0.4; extra == "testing"
-Requires-Dist: tox>=3.25.1; extra == "testing"
-Requires-Dist: black>=22.8.0; extra == "testing"
-
 # SheildPy: Secure Data Privacy Framework for Python Data Scientists
 
-SheildPy is an all-in-one Python package designed to address data privacy and security concerns for data scientists. Developed by Deependra Verma, SheildPy offers robust encryption, anonymization, and access control tools, ensuring the confidentiality and integrity of sensitive data.
+[![GitHub stars](https://img.shields.io/github/stars/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists.svg)](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/stargazers)
+[![GitHub license](https://img.shields.io/github/license/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists.svg)](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/blob/main/LICENSE)
+
+SheildPy is an all-in-one Python package designed to address data privacy and security concerns for data scientists. Developed by [Deependra Verma](https://www.linkedin.com/in/deependra-verma-data-science/), SheildPy offers robust encryption, anonymization, and access control tools, ensuring the confidentiality and integrity of sensitive data.
+
+## Introduction
 
-## Contact Information
-- **Name:** Deependra Verma
-- **Email:** deependra.verma00@gmail.com
-- **LinkedIn:** [Deependra Verma](https://www.linkedin.com/in/deependra-verma-data-science/)
-- **GitHub Profile:** [DeependraVerma](https://github.com/DeependraVerma)
-- **Portfolio:** [Deependra's Portfolio](https://deependradatascience-productportfolio.netlify.app/)
+SheildPy: Your all-in-one Python package for robust data privacy and security. Encrypt, anonymize, and control access to sensitive data effortlessly.
+
+## Features
+
+### SheildPy provides the following key methods:
+- `encrypt_data(data)`: Encrypts sensitive data to ensure confidentiality.
+- `decrypt_data(encrypted_data)`: Decrypts encrypted data to its original form.
+- `anonymize_data(data, columns_to_anonymize)`: Anonymizes specific columns in a DataFrame.
+- `add_role(role_name, permissions)`: Adds a new role with associated permissions to the access control system.
+- `check_permission(role_name, permission)`: Checks if a role has the specified permission.
 
 ## Installation
 
-You can install SheildPy via pip:
+To install SheildPy, simply run:
 
 ```bash
 pip install SheildPy
 ```
 
 Alternatively, you can clone the GitHub repository:
 
@@ -52,22 +37,32 @@
 ## Dependencies
 
 SheildPy relies on the following dependencies:
 - `pandas>=1.0.0`
 - `faker>=8.0.0`
 - `cryptography>=3.0`
 
-## Methods
+## Usage
+
+
+# Import the package
+from PrivacyPy import DataPrivacyFramework
+
+# Initialize PrivacyPy with encryption key
+encryption_key = "your_encryption_key"
+privacy_framework = DataPrivacyFramework(encryption_key)
+
+# Anonymize sensitive columns (Name, Email)
+anonymized_df = privacy_framework.anonymize_data(data, ['Name', 'Email'])
+
+# Encrypt entire DataFrame
+encrypted_df = privacy_framework.encrypt_data(anonymized_df)
+print("Encrypted DataFrame:")
+print(encrypted_df)
 
-SheildPy provides the following key methods:
-- `encrypt_data(data)`: Encrypts sensitive data to ensure confidentiality.
-- `decrypt_data(encrypted_data)`: Decrypts encrypted data to its original form.
-- `anonymize_data(data, columns_to_anonymize)`: Anonymizes specific columns in a DataFrame.
-- `add_role(role_name, permissions)`: Adds a new role with associated permissions to the access control system.
-- `check_permission(role_name, permission)`: Checks if a role has the specified permission.
 
 ## Users Benefit
 
 SheildPy empowers data scientists with the following benefits:
 - **Data Confidentiality:** Encrypt sensitive data to prevent unauthorized access.
 - **Anonymization:** Anonymize personally identifiable information for privacy protection.
 - **Access Control:** Control data access based on user roles and permissions.
@@ -89,8 +84,16 @@
 2. Clone the forked repository to your local machine.
 3. Create a new branch for your changes.
 4. Make your modifications and improvements.
 5. Test your changes to ensure they work as expected.
 6. Commit your changes and push them to your forked repository.
 7. Submit a pull request to the original repository.
 
-Let's collaborate to make SheildPy the go-to solution for secure data privacy in the Python data science community.
+We welcome contributions from the community! Whether it's fixing bugs, adding new features, or improving documentation, your contributions help make XplainML better for everyone. Check out our [Contributing Guidelines](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/wiki) to get started.
+
+## License
+
+SheildPy is licensed under the [MIT License](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/blob/main/LICENSE). See the [LICENSE](https://github.com/DeependraVerma/SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists/blob/main/LICENSE) file for details.
+
+## About the Author
+
+[Email](mailto:deependra.verma00@gmail.com) | [LinkedIn](https://www.linkedin.com/in/deependra-verma-data-science/) | [GitHub](https://github.com/DeependraVerma) | [Portfolio](https://deependradatascience-productportfolio.netlify.app/)
```

### Comparing `SheildPy-0.0.7/setup.cfg` & `SheildPy-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `SheildPy-0.0.7/setup.py` & `SheildPy-0.0.8/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
         requirements = file_obj.readlines()
         requirements = [req.replace("\n","") for req in requirements]
 
         if HYPEN_E_DOT in requirements:
             requirements.remove(HYPEN_E_DOT)
     return requirements
 
-__version__ = "0.0.7"
+__version__ = "0.0.8"
 REPO_NAME = "SecuPy-Secure-Data-Privacy-Framework-for-Python-Data-Scientists"
 PKG_NAME= "SheildPy"
 AUTHOR_USER_NAME = "DeependraVerma"
 AUTHOR_EMAIL = "deependra.verma00@gmail.com"
 
 setup(
     name=PKG_NAME,
```

### Comparing `SheildPy-0.0.7/src/SecuPy/data_privacy_framework.py` & `SheildPy-0.0.8/src/SecuPy/data_privacy_framework.py`

 * *Files identical despite different names*

