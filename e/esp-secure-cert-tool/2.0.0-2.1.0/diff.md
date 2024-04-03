# Comparing `tmp/esp-secure-cert-tool-2.0.0.tar.gz` & `tmp/esp-secure-cert-tool-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/esp-secure-cert-tool-2.0.0.tar", last modified: Tue Nov 21 05:01:04 2023, max compression
+gzip compressed data, was "dist/esp-secure-cert-tool-2.1.0.tar", last modified: Wed Apr  3 13:05:27 2024, max compression
```

## Comparing `esp-secure-cert-tool-2.0.0.tar` & `esp-secure-cert-tool-2.1.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 05:01:04.000000 esp-secure-cert-tool-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2023-11-21 05:00:54.000000 esp-secure-cert-tool-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2023-11-21 05:00:54.000000 esp-secure-cert-tool-2.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2023-11-21 05:01:04.000000 esp-secure-cert-tool-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4552 2023-11-21 05:00:54.000000 esp-secure-cert-tool-2.0.0/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)    15290 2023-11-21 05:00:54.000000 esp-secure-cert-tool-2.0.0/configure_esp_secure_cert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 05:01:04.000000 esp-secure-cert-tool-2.0.0/esp_secure_cert/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 05:00:54.000000 esp-secure-cert-tool-2.0.0/esp_secure_cert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2023-11-21 05:00:54.000000 esp-secure-cert-tool-2.0.0/esp_secure_cert/configure_ds.py
--rw-r--r--   0 runner    (1001) docker     (127)     7606 2023-11-21 05:00:54.000000 esp-secure-cert-tool-2.0.0/esp_secure_cert/custflash_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     9214 2023-11-21 05:00:54.000000 esp-secure-cert-tool-2.0.0/esp_secure_cert/efuse_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4516 2023-11-21 05:00:54.000000 esp-secure-cert-tool-2.0.0/esp_secure_cert/esp_secure_cert_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     3105 2023-11-21 05:00:54.000000 esp-secure-cert-tool-2.0.0/esp_secure_cert/nvs_format.py
--rw-r--r--   0 runner    (1001) docker     (127)    14908 2023-11-21 05:00:54.000000 esp-secure-cert-tool-2.0.0/esp_secure_cert/tlv_format.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 05:01:04.000000 esp-secure-cert-tool-2.0.0/esp_secure_cert_tool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2023-11-21 05:01:04.000000 esp-secure-cert-tool-2.0.0/esp_secure_cert_tool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      533 2023-11-21 05:01:04.000000 esp-secure-cert-tool-2.0.0/esp_secure_cert_tool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 05:01:04.000000 esp-secure-cert-tool-2.0.0/esp_secure_cert_tool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-11-21 05:01:04.000000 esp-secure-cert-tool-2.0.0/esp_secure_cert_tool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2023-11-21 05:01:04.000000 esp-secure-cert-tool-2.0.0/esp_secure_cert_tool.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2023-11-21 05:00:54.000000 esp-secure-cert-tool-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-21 05:01:04.000000 esp-secure-cert-tool-2.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2023-11-21 05:00:54.000000 esp-secure-cert-tool-2.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:05:27.000000 esp-secure-cert-tool-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-03 13:05:16.000000 esp-secure-cert-tool-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-03 13:05:16.000000 esp-secure-cert-tool-2.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-03 13:05:27.000000 esp-secure-cert-tool-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-04-03 13:05:16.000000 esp-secure-cert-tool-2.1.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15301 2024-04-03 13:05:16.000000 esp-secure-cert-tool-2.1.0/configure_esp_secure_cert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:05:27.000000 esp-secure-cert-tool-2.1.0/esp_secure_cert/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 13:05:16.000000 esp-secure-cert-tool-2.1.0/esp_secure_cert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6830 2024-04-03 13:05:16.000000 esp-secure-cert-tool-2.1.0/esp_secure_cert/configure_ds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7606 2024-04-03 13:05:16.000000 esp-secure-cert-tool-2.1.0/esp_secure_cert/custflash_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9214 2024-04-03 13:05:16.000000 esp-secure-cert-tool-2.1.0/esp_secure_cert/efuse_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-04-03 13:05:16.000000 esp-secure-cert-tool-2.1.0/esp_secure_cert/esp_secure_cert_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2024-04-03 13:05:16.000000 esp-secure-cert-tool-2.1.0/esp_secure_cert/nvs_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14908 2024-04-03 13:05:16.000000 esp-secure-cert-tool-2.1.0/esp_secure_cert/tlv_format.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 13:05:27.000000 esp-secure-cert-tool-2.1.0/esp_secure_cert_tool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-03 13:05:27.000000 esp-secure-cert-tool-2.1.0/esp_secure_cert_tool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-03 13:05:27.000000 esp-secure-cert-tool-2.1.0/esp_secure_cert_tool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 13:05:27.000000 esp-secure-cert-tool-2.1.0/esp_secure_cert_tool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 13:05:27.000000 esp-secure-cert-tool-2.1.0/esp_secure_cert_tool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 13:05:27.000000 esp-secure-cert-tool-2.1.0/esp_secure_cert_tool.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-03 13:05:16.000000 esp-secure-cert-tool-2.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 13:05:27.000000 esp-secure-cert-tool-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-04-03 13:05:16.000000 esp-secure-cert-tool-2.1.0/setup.py
```

### Comparing `esp-secure-cert-tool-2.0.0/LICENSE` & `esp-secure-cert-tool-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `esp-secure-cert-tool-2.0.0/PKG-INFO` & `esp-secure-cert-tool-2.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-secure-cert-tool
-Version: 2.0.0
+Version: 2.1.0
 Summary: A python utility which helps to configure and provisionthe ESP platform with PKI credentials into the esp_secure_cert partition
 Home-page: https://github.com/espressif/esp_secure_cert_mgr/blob/main/tools
 Author: Espressif Systems
 Author-email: 
 License: Apache-2.0
 Project-URL: Documentation, https://github.com/espressif/esp_secure_cert_mgr/blob/main/tools/README.md
 Project-URL: Source, https://github.com/espressif/esp_secure_cert_mgr/blob/main/tools/configure_esp_secure_cert.py
```

### Comparing `esp-secure-cert-tool-2.0.0/README.md` & `esp-secure-cert-tool-2.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -37,19 +37,28 @@
 * When configuring the DS peripheral, by default the configuration script does not enable the read protection for the efuse key block in which the DS key is programmed. This is done for allowing flexibility while using the script for development purpose.
 
 * Please remove the `--configure_ds` argument from these commands if use of the DS peripheral is disabled in the menu config.
 > **WARNING**: This is not recommended for production purpose as the private key shall be stored as plaintext.
 
 ## Generate `esp_secure_cert` partition of type `cust_flash_tlv`:
 
-This command shall generate a binary partition containing the PKI credentials stored in the TLV format.
+This command shall generate a binary partition containing the PKI credentials stored in the TLV format and flash it at the default offset of `0xD000`.
+
 ```
 configure_esp_secure_cert.py -p /* Serial port */ --keep_ds_data_on_host --efuse_key_id 1 --ca-cert cacert.pem --device-cert client.crt --private-key client.key --target_chip /* target chip */ --secure_cert_type cust_flash_tlv --configure_ds
 ```
 
+* When [Flash Encryption](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/security/flash-encryption.html) is enabled for the device, the option ``--skip_flash`` (explained below) can be used to prevent the flashing opereation and only save the `esp_secure_cert.bin` on the host machine. It can then be flashed on the target using below command:
+
+	```esptool.py -p /* Serial Port*/ write_flash 0xD000 esp_secure_cert.bin --encrypt```
+
+	More details regarding [esptool.py](https://docs.espressif.com/projects/esptool/en/latest/esp32/esptool/index.html#esptool-py) utility can be found [here](https://docs.espressif.com/projects/esptool/en/latest/esp32/esptool/index.html).
+
+    Note: This is only applicable for [Development mode](https://docs.espressif.com/projects/esp-idf/en/latest/esp32/security/flash-encryption.html#flash-enc-development-mode) of Flash Encryption.
+
 ## Legacy partition formats:
 
 1. Generate `esp_secure_cert` partition of type `cust_flash`:
 
 ```
 configure_esp_secure_cert.py -p /* Serial port */ --keep_ds_data_on_host --efuse_key_id 1 --ca-cert cacert.pem --device-cert client.crt --private-key client.key --target_chip /* target chip */ --secure_cert_type cust_flash --configure_ds
 ```
```

### Comparing `esp-secure-cert-tool-2.0.0/configure_esp_secure_cert.py` & `esp-secure-cert-tool-2.1.0/configure_esp_secure_cert.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ecdsa_key_file = os.path.join(esp_secure_cert_data_dir, 'ecdsa_key.bin')
 # csv and bin filenames are default filenames
 # for nvs partition files created with this script
 csv_filename = os.path.join(esp_secure_cert_data_dir, 'esp_secure_cert.csv')
 bin_filename = os.path.join(esp_secure_cert_data_dir, 'esp_secure_cert.bin')
 # Targets supported by the script
 supported_targets = {'esp32', 'esp32s2', 'esp32c3', 'esp32s3',
-                     'esp32c6', 'esp32h2'}
+                     'esp32c6', 'esp32h2', 'esp32p4'}
 
 
 # Flash esp_secure_cert partition after its generation
 #
 # @info
 # The partition shall be flashed at the offset provided
 # for the --sec_cert_part_offset option
```

### Comparing `esp-secure-cert-tool-2.0.0/esp_secure_cert/configure_ds.py` & `esp-secure-cert-tool-2.1.0/esp_secure_cert/configure_ds.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,25 @@
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.asymmetric import rsa, ec
 from cryptography.hazmat.primitives.ciphers import Cipher, algorithms, modes
 from cryptography.utils import int_to_bytes
 from esp_secure_cert.esp_secure_cert_helper import load_private_key
 
 supported_targets_rsa_ds = ['esp32s2', 'esp32s3', 'esp32c3',
-                            'esp32c6', 'esp32h2']
+                            'esp32c6', 'esp32h2', 'esp32p4']
 supported_key_size_rsa = {'esp32s2': [1024, 2048, 3072, 4096],
                           'esp32c3': [1024, 2048, 3072],
                           'esp32s3': [1024, 2048, 3072, 4096],
                           'esp32c6': [1024, 2048, 3072],
-                          'esp32h2': [1024, 2048, 3072]}
+                          'esp32h2': [1024, 2048, 3072],
+                          'esp32p4': [1024, 2048, 3072, 4096]}
 
-supported_targets_ecdsa = ['esp32h2']
-supported_key_size_ecdsa = {'esp32h2': [256]}
+supported_targets_ecdsa = ['esp32h2', 'esp32p4']
+supported_key_size_ecdsa = {'esp32h2': [256],
+                            'esp32p4': [256]}
 
 idf_path = os.getenv('IDF_PATH')
 if not idf_path or not os.path.exists(idf_path):
     raise Exception('IDF_PATH not found')
 
 
 def number_as_bytes(number, pad_bits=None):
```

### Comparing `esp-secure-cert-tool-2.0.0/esp_secure_cert/custflash_format.py` & `esp-secure-cert-tool-2.1.0/esp_secure_cert/custflash_format.py`

 * *Files identical despite different names*

### Comparing `esp-secure-cert-tool-2.0.0/esp_secure_cert/efuse_helper.py` & `esp-secure-cert-tool-2.1.0/esp_secure_cert/efuse_helper.py`

 * *Files identical despite different names*

### Comparing `esp-secure-cert-tool-2.0.0/esp_secure_cert/esp_secure_cert_helper.py` & `esp-secure-cert-tool-2.1.0/esp_secure_cert/esp_secure_cert_helper.py`

 * *Files identical despite different names*

### Comparing `esp-secure-cert-tool-2.0.0/esp_secure_cert/nvs_format.py` & `esp-secure-cert-tool-2.1.0/esp_secure_cert/nvs_format.py`

 * *Files identical despite different names*

### Comparing `esp-secure-cert-tool-2.0.0/esp_secure_cert/tlv_format.py` & `esp-secure-cert-tool-2.1.0/esp_secure_cert/tlv_format.py`

 * *Files identical despite different names*

### Comparing `esp-secure-cert-tool-2.0.0/esp_secure_cert_tool.egg-info/PKG-INFO` & `esp-secure-cert-tool-2.1.0/esp_secure_cert_tool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: esp-secure-cert-tool
-Version: 2.0.0
+Version: 2.1.0
 Summary: A python utility which helps to configure and provisionthe ESP platform with PKI credentials into the esp_secure_cert partition
 Home-page: https://github.com/espressif/esp_secure_cert_mgr/blob/main/tools
 Author: Espressif Systems
 Author-email: 
 License: Apache-2.0
 Project-URL: Documentation, https://github.com/espressif/esp_secure_cert_mgr/blob/main/tools/README.md
 Project-URL: Source, https://github.com/espressif/esp_secure_cert_mgr/blob/main/tools/configure_esp_secure_cert.py
```

### Comparing `esp-secure-cert-tool-2.0.0/esp_secure_cert_tool.egg-info/SOURCES.txt` & `esp-secure-cert-tool-2.1.0/esp_secure_cert_tool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `esp-secure-cert-tool-2.0.0/setup.py` & `esp-secure-cert-tool-2.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     print(
         "Package setuptools is missing from your Python installation. "
         "Please see the installation section in the esp-secure-cert-tool "
         "documentation for instructions on how to install it."
     )
     exit(1)
 
-VERSION = "2.0.0"
+VERSION = "2.1.0"
 
 long_description = """
 ====================
 esp-secure-cert-tool
 ====================
 The python utility helps to configure and provision the device with
 PKI credentials to generate the esp_secure_cert partition.
```

