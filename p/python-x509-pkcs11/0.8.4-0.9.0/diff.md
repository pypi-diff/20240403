# Comparing `tmp/python_x509_pkcs11-0.8.4.tar.gz` & `tmp/python_x509_pkcs11-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_x509_pkcs11-0.8.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "python_x509_pkcs11-0.9.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `python_x509_pkcs11-0.8.4.tar` & `python_x509_pkcs11-0.9.0.tar`

### file list

```diff
@@ -1,29 +1,41 @@
--rw-r--r--   0        0        0     1762 2023-12-09 06:17:34.391456 python_x509_pkcs11-0.8.4/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1468 2023-12-09 05:39:09.439547 python_x509_pkcs11-0.8.4/.github/workflows/debian.yaml
--rw-r--r--   0        0        0       79 2023-12-09 05:39:09.439547 python_x509_pkcs11-0.8.4/.gitignore
--rw-r--r--   0        0        0      143 2023-12-09 10:37:11.158044 python_x509_pkcs11-0.8.4/.vscode/settings.json
--rw-r--r--   0        0        0     1045 2023-12-09 05:39:09.439547 python_x509_pkcs11-0.8.4/LICENSE
--rw-r--r--   0        0        0     2287 2023-12-09 06:24:42.064027 python_x509_pkcs11-0.8.4/Makefile
--rw-r--r--   0        0        0     4284 2023-12-09 05:39:09.439547 python_x509_pkcs11-0.8.4/README.md
--rw-r--r--   0        0        0    33290 2023-12-09 05:39:09.439547 python_x509_pkcs11-0.8.4/docs/README.md
--rw-r--r--   0        0        0     1099 2024-01-22 09:50:40.878123 python_x509_pkcs11-0.8.4/pyproject.toml
--rw-r--r--   0        0        0       51 2023-12-09 06:53:03.108646 python_x509_pkcs11-0.8.4/requirements.txt
--rw-r--r--   0        0        0      114 2024-01-22 09:50:49.679034 python_x509_pkcs11-0.8.4/src/python_x509_pkcs11/__init__.py
--rw-r--r--   0        0        0     6657 2023-12-11 02:38:14.730911 python_x509_pkcs11-0.8.4/src/python_x509_pkcs11/ca.py
--rw-r--r--   0        0        0     8143 2023-12-09 05:39:09.440547 python_x509_pkcs11-0.8.4/src/python_x509_pkcs11/crl.py
--rw-r--r--   0        0        0     6437 2023-12-09 05:39:09.440547 python_x509_pkcs11-0.8.4/src/python_x509_pkcs11/crypto.py
--rw-r--r--   0        0        0     8805 2023-12-09 05:39:09.440547 python_x509_pkcs11-0.8.4/src/python_x509_pkcs11/csr.py
--rw-r--r--   0        0        0      802 2023-12-09 05:39:09.440547 python_x509_pkcs11-0.8.4/src/python_x509_pkcs11/error.py
--rw-r--r--   0        0        0     1889 2023-12-09 05:39:09.440547 python_x509_pkcs11-0.8.4/src/python_x509_pkcs11/lib.py
--rw-r--r--   0        0        0    13591 2023-12-09 05:39:09.440547 python_x509_pkcs11-0.8.4/src/python_x509_pkcs11/ocsp.py
--rw-r--r--   0        0        0    35008 2024-01-22 09:49:57.421563 python_x509_pkcs11-0.8.4/src/python_x509_pkcs11/pkcs11_handle.py
--rw-r--r--   0        0        0        0 2023-12-09 05:39:09.440547 python_x509_pkcs11-0.8.4/src/python_x509_pkcs11/py.typed
--rw-r--r--   0        0        0      115 2023-12-09 06:53:07.544619 python_x509_pkcs11-0.8.4/test_requirements.txt
--rw-r--r--   0        0        0       32 2023-12-09 05:39:09.440547 python_x509_pkcs11-0.8.4/tests/__init__.py
--rw-r--r--   0        0        0    14068 2023-12-09 05:39:09.440547 python_x509_pkcs11-0.8.4/tests/test_ca.py
--rw-r--r--   0        0        0     9646 2023-12-09 05:39:09.440547 python_x509_pkcs11-0.8.4/tests/test_crl.py
--rw-r--r--   0        0        0     4049 2023-12-09 05:39:09.440547 python_x509_pkcs11-0.8.4/tests/test_crypto.py
--rw-r--r--   0        0        0    11078 2023-12-09 05:39:09.440547 python_x509_pkcs11-0.8.4/tests/test_csr.py
--rw-r--r--   0        0        0    33921 2023-12-09 05:39:09.440547 python_x509_pkcs11-0.8.4/tests/test_ocsp.py
--rw-r--r--   0        0        0    45740 2023-12-09 05:39:09.441547 python_x509_pkcs11-0.8.4/tests/test_pkcs11_handle.py
--rw-r--r--   0        0        0     4744 1970-01-01 00:00:00.000000 python_x509_pkcs11-0.8.4/PKG-INFO
+-rw-r--r--   0        0        0     1762 2024-02-09 12:34:22.583978 python_x509_pkcs11-0.9.0/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1738 2024-02-21 12:14:46.968922 python_x509_pkcs11-0.9.0/.github/workflows/debian.yaml
+-rw-r--r--   0        0        0      127 2024-04-03 13:36:11.393576 python_x509_pkcs11-0.9.0/.gitignore
+-rw-r--r--   0        0        0      330 2024-03-26 17:55:01.399062 python_x509_pkcs11-0.9.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      177 2024-03-26 17:55:01.399062 python_x509_pkcs11-0.9.0/.vscode/settings.json
+-rw-r--r--   0        0        0      452 2024-02-21 16:45:56.480165 python_x509_pkcs11-0.9.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1045 2024-02-09 12:34:22.583978 python_x509_pkcs11-0.9.0/LICENSE
+-rw-r--r--   0        0        0     2287 2024-02-17 14:00:31.220337 python_x509_pkcs11-0.9.0/Makefile
+-rw-r--r--   0        0        0     4284 2024-02-09 12:34:22.584978 python_x509_pkcs11-0.9.0/README.md
+-rw-r--r--   0        0        0      634 2024-03-26 17:55:01.400062 python_x509_pkcs11-0.9.0/docs/Makefile
+-rw-r--r--   0        0        0    33332 2024-02-12 13:19:33.086363 python_x509_pkcs11-0.9.0/docs/README.md
+-rw-r--r--   0        0        0    39593 2024-04-03 13:35:20.411580 python_x509_pkcs11-0.9.0/docs/api.rst
+-rw-r--r--   0        0        0      997 2024-03-26 17:55:01.403062 python_x509_pkcs11-0.9.0/docs/conf.py
+-rw-r--r--   0        0        0      864 2024-03-26 17:55:01.403062 python_x509_pkcs11-0.9.0/docs/index.rst
+-rw-r--r--   0        0        0     1703 2024-03-26 17:55:01.403062 python_x509_pkcs11-0.9.0/docs/installation.rst
+-rw-r--r--   0        0        0      800 2024-03-26 17:55:01.404062 python_x509_pkcs11-0.9.0/docs/make.bat
+-rw-r--r--   0        0        0        5 2024-03-26 17:55:01.404062 python_x509_pkcs11-0.9.0/docs/requirements.txt
+-rw-r--r--   0        0        0     1263 2024-02-21 16:45:56.481165 python_x509_pkcs11-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       64 2024-02-21 12:14:46.970922 python_x509_pkcs11-0.9.0/requirements.txt
+-rw-r--r--   0        0        0      332 2024-03-26 17:55:01.405062 python_x509_pkcs11-0.9.0/src/python_x509_pkcs11/__init__.py
+-rw-r--r--   0        0        0     9018 2024-03-07 08:46:26.200713 python_x509_pkcs11-0.9.0/src/python_x509_pkcs11/ca.py
+-rw-r--r--   0        0        0    10221 2024-03-07 08:46:26.200713 python_x509_pkcs11-0.9.0/src/python_x509_pkcs11/crl.py
+-rw-r--r--   0        0        0     6446 2024-03-07 08:46:26.201713 python_x509_pkcs11-0.9.0/src/python_x509_pkcs11/crypto.py
+-rw-r--r--   0        0        0    12423 2024-03-07 08:46:26.202713 python_x509_pkcs11-0.9.0/src/python_x509_pkcs11/csr.py
+-rw-r--r--   0        0        0      796 2024-02-14 09:23:27.056104 python_x509_pkcs11-0.9.0/src/python_x509_pkcs11/error.py
+-rw-r--r--   0        0        0     2822 2024-04-03 07:46:59.433140 python_x509_pkcs11-0.9.0/src/python_x509_pkcs11/lib.py
+-rw-r--r--   0        0        0    13833 2024-03-26 17:55:01.406062 python_x509_pkcs11-0.9.0/src/python_x509_pkcs11/ocsp.py
+-rw-r--r--   0        0        0    35107 2024-04-03 13:35:20.414580 python_x509_pkcs11-0.9.0/src/python_x509_pkcs11/pkcs11_handle.py
+-rw-r--r--   0        0        0     7989 2024-04-03 13:35:20.415580 python_x509_pkcs11-0.9.0/src/python_x509_pkcs11/privatekeys.py
+-rw-r--r--   0        0        0        0 2024-02-09 12:34:22.586978 python_x509_pkcs11-0.9.0/src/python_x509_pkcs11/py.typed
+-rw-r--r--   0        0        0      115 2024-02-09 12:34:22.586978 python_x509_pkcs11-0.9.0/test_requirements.txt
+-rw-r--r--   0        0        0       33 2024-02-14 09:23:27.057104 python_x509_pkcs11-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0      833 2024-02-19 13:47:29.331252 python_x509_pkcs11-0.9.0/tests/conftest.py
+-rw-r--r--   0        0        0    14177 2024-02-19 13:47:29.332252 python_x509_pkcs11-0.9.0/tests/test_ca.py
+-rw-r--r--   0        0        0     9734 2024-02-19 13:47:29.332252 python_x509_pkcs11-0.9.0/tests/test_crl.py
+-rw-r--r--   0        0        0     4050 2024-02-14 09:23:27.057104 python_x509_pkcs11-0.9.0/tests/test_crypto.py
+-rw-r--r--   0        0        0    11164 2024-02-19 13:47:29.332252 python_x509_pkcs11-0.9.0/tests/test_csr.py
+-rw-r--r--   0        0        0    34024 2024-02-19 13:47:29.333252 python_x509_pkcs11-0.9.0/tests/test_ocsp.py
+-rw-r--r--   0        0        0    46712 2024-03-26 17:55:01.412062 python_x509_pkcs11-0.9.0/tests/test_pkcs11_handle.py
+-rw-r--r--   0        0        0     7405 2024-04-03 07:44:47.589194 python_x509_pkcs11-0.9.0/tests/test_privatekeys.py
+-rw-r--r--   0        0        0     4808 1970-01-01 00:00:00.000000 python_x509_pkcs11-0.9.0/PKG-INFO
```

### Comparing `python_x509_pkcs11-0.8.4/.devcontainer/devcontainer.json` & `python_x509_pkcs11-0.9.0/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `python_x509_pkcs11-0.8.4/.github/workflows/debian.yaml` & `python_x509_pkcs11-0.9.0/.github/workflows/debian.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 on: [push]
 
 env:
   PKCS11_MODULE: /usr/lib/softhsm/libsofthsm2.so
   PKCS11_TOKEN: my_test_token_1
   PKCS11_PIN: 1234
+  PKCS11_TOKEN_SUPPORT_RECREATE_SESSION: TRUE
 
 jobs:
   test_typecheck_build:
 
     strategy:
       matrix:
         target: ["python:3.9-bookworm", "python:3.10-bookworm","python:3.11-bookworm", "python:3.12-bookworm"]
@@ -33,23 +34,26 @@
           python3 --version
 
 
       - name: Install python dependencies
         run: |
           python3 -m venv .venv && . .venv/bin/activate && \
           python3 -m pip install --upgrade pip && \
-          pip3 install -r requirements.txt -r test_requirements.txt
+          python -m pip install -r requirements.txt -r test_requirements.txt
 
       - name: Setup softhsm2
         run: |
           make new_softhsm
 
+      # https://github.com/pyauth/python-pkcs11/issues/171
+      # . .venv/bin/activate && make test
       - name: Test
         run: |
-          . .venv/bin/activate && make test
+          . .venv/bin/activate && pytest -vv -s --ignore tests/test_privatekeys.py
+          . .venv/bin/activate && pytest -vv -s tests/test_privatekeys.py
 
       - name: Mark github workspace as safe
         run: |
           git config --global --add safe.directory /__w/python_x509_pkcs11/python_x509_pkcs11
 
       - name: Typecheck
         run: |
@@ -57,8 +61,8 @@
           . .venv/bin/activate && make typecheck
 
       - name: Build
         run: |
           . .venv/bin/activate && make build
 
 
-    
+
```

### Comparing `python_x509_pkcs11-0.8.4/LICENSE` & `python_x509_pkcs11-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_x509_pkcs11-0.8.4/Makefile` & `python_x509_pkcs11-0.9.0/Makefile`

 * *Files identical despite different names*

### Comparing `python_x509_pkcs11-0.8.4/README.md` & `python_x509_pkcs11-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `python_x509_pkcs11-0.8.4/docs/README.md` & `python_x509_pkcs11-0.9.0/docs/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -122,16 +122,16 @@
 
 pub = b"0\x82\x01\n\x02\x82\x01\x01\x00\xd9\xb6C,O\xc0\x83\xca\xa5\xcc\xa7<_\xbf$\xdd-YJ0m\xbf\xa8\xf9[\xe7\xcb\x14W6G\n\x13__\xea\xb4Z\xab2\x01\x0f\xa4\xd3\x1c\xbb\xa6\x98\x9d\xcdf\xaa\x07\xcb\xff\xd8\x80\xa9\\\xa1\xf44\x01\xdbY\xa6\xcf\x83\xd2\x83Z\x8a<\xc1\x18\xe5\x8d\xff\xbfzU\x03\x01\x11\xa1\xa1\x98\xcf\xcaVu\xf9\xf3\xa7+ \xe7N9\x07\xfd\xc6\xd0\x7f\xa0\xba&\xef\xb2a\xc6\xa5d\x1c\x93\xe6\xc3\x80\xd1*;\xc8@7\x0fm)\xf93\xe4\x1f\x91\xf4=\xa6\xf8\xed\x9cN\x84\x9b\xf2\xc5\x9f\x9f\x82E\xa5Tm\xb9\xb3:T\xc7_\xb1^[\xf4\x0b\xd8\x0b\xd2\xfb\xe1\x13\x1e,L\xd9\xdc\xed]_#\xca\xa0r\xc2\xc5F \xec\xae\x8d\x08v\x059\x062\xe1\xf7%\x9e\xfd\xfb9\x11(\xa4\x86v\x90\x01\x1c\xbeP\x04\xa3%\x91\x08\xc5\xd5\xc1U\xf6\xd3\x7f\x1f\x9f7`\xce\xc9\xa1\xd9\x8f\\Z\xa8\x1cmz\x19x\xa4'F\xdf\xb2\xb2\x87\xba\xf7\n>]\x9f\xc0K@\xd9\xdb\x02\x03\x01\x00\x01"
 
 priv = b"0\x82\x04\xa4\x02\x01\x00\x02\x82\x01\x01\x00\xd9\xb6C,O\xc0\x83\xca\xa5\xcc\xa7<_\xbf$\xdd-YJ0m\xbf\xa8\xf9[\xe7\xcb\x14W6G\n\x13__\xea\xb4Z\xab2\x01\x0f\xa4\xd3\x1c\xbb\xa6\x98\x9d\xcdf\xaa\x07\xcb\xff\xd8\x80\xa9\\\xa1\xf44\x01\xdbY\xa6\xcf\x83\xd2\x83Z\x8a<\xc1\x18\xe5\x8d\xff\xbfzU\x03\x01\x11\xa1\xa1\x98\xcf\xcaVu\xf9\xf3\xa7+ \xe7N9\x07\xfd\xc6\xd0\x7f\xa0\xba&\xef\xb2a\xc6\xa5d\x1c\x93\xe6\xc3\x80\xd1*;\xc8@7\x0fm)\xf93\xe4\x1f\x91\xf4=\xa6\xf8\xed\x9cN\x84\x9b\xf2\xc5\x9f\x9f\x82E\xa5Tm\xb9\xb3:T\xc7_\xb1^[\xf4\x0b\xd8\x0b\xd2\xfb\xe1\x13\x1e,L\xd9\xdc\xed]_#\xca\xa0r\xc2\xc5F \xec\xae\x8d\x08v\x059\x062\xe1\xf7%\x9e\xfd\xfb9\x11(\xa4\x86v\x90\x01\x1c\xbeP\x04\xa3%\x91\x08\xc5\xd5\xc1U\xf6\xd3\x7f\x1f\x9f7`\xce\xc9\xa1\xd9\x8f\\Z\xa8\x1cmz\x19x\xa4'F\xdf\xb2\xb2\x87\xba\xf7\n>]\x9f\xc0K@\xd9\xdb\x02\x03\x01\x00\x01\x02\x82\x01\x00a5\x1e=\x14\xc6\xf2\x91s\x023\xd1\xa36\xa7q\x12$\x82\x19\xa9\x87 \x1df\xc9\xd2E\x1c\xc3\xa1h\x80I\xdf{\xdeWu\x84\xf80Q\xf9\xe9$h8P\x8d;\xbf\xc3\x87t\x8e\xe8\xb3\xb6&\xa1\xf0\xee\xbbP\x06I5\xa4\xb2\xfd\xa4'\x88Xcv\xc9\xb0g \xba\x1c\xaa\x10\xaf$\x99\xf2\xd04\x11\x0c\x97\xa1\x8c){%\xbf\xc9\xb2\x11\xbaJ\xbb\x93S\x07$\xdd\x1bO\xdd\xea\xb3\xe8\xab\x05\xb9\x83\xc3\xdf\xd85\xcd\x1a%\xd5\xd9\xc4\x933\x83\t\xd3\xea\xcdb\xcb\xec\x9eGqk\x1c\x8c\x06\x8a\\\xae\xbe\xd3+\x0b\xd0R\xbd:\x8a\xf5\xf4\x0f\x0b\xd4\xfa@P=\xe5\xb2\xa1\xb2\x01\x00\x08\xc7\x11?M\x84-\x1e\xbc\xa9\xbf|\x87\x98\xd7\x0e\xf6\xa9\xa6\xcd\x8c8\xa5F8\xacM\x82\xade[\xa9_\xa7Biv\x9c\x06\xa6\x001\xc3I\x1f\xc4\x9by\xd7\xe0\x9e\xb9\n\xbb\x19\\o\xc5i\xd90r\xd4\x1e(\x05\xdd\xedF\xe9\xaa\xbd\x91\xe5\x08\x8f4-\xb6\xd1Q\x02\x81\x81\x00\xf7\x076\xd8i\x87\x12\xf1\xd0$\x07\x1f\xab\xb7^\x0e\xa5\xfb\x83\x98\x00\x0b\\\x1d\xe8s\x15r\x96/\x0e\x0ezB\xc8\xf6\xf3Zmj?\xa0\xc1\x11r\xaf3\x11a\xcd\xa3\xfc\xa0\x03\x04E\x05\x99\x9a\xd9\xff\x8e+\xdcfM\xa8\xe8&\x84\x85\xc5\x11O\x9d4\x1f\xc3\x1f\xef\xed\x13BW\xaa\x93\xc3\x08(v]\xbc\x93V\xb6s\xce\xb1\xa8\xe2\x94\xa5'\xf3\x7f\x90,G[\xfeI\x16\xbe\xb0\xf8J\xca9n\xb5\xfc\x8a\xe2[\xc5\x0c\x95\xd5\x02\x81\x81\x00\xe1\x9ey\xc8\xe2\xd3\x93\xa2nj\xe1.\xaa\xe3\xa7\xf5P\xd1\xd8yM\x01\xdc\x01\x0c\xdbQG\x1b=\xbe\xe4.\x9cM\xc2\xda\xd2\xa4\xb3\x80\xb2\xbd\xbaO\x1bD&]0\x0b\xe6\xf5\x08\xdb*I\xfe+@Aa\x16;\x9a%\x8cof:\x156 \xb0\xe6\xfe\x95\x9bO\x85]\x96\x94S\x05\xc8\x8a\xb6\x92\xb3\x95\xc5\xfbX\xa9S<@\x12\x94K\x8b\xa3\x0f\xebO\xb5\x9f\x0c\x08\xf2\xccS\xfd8\x06\xeb\xaa\x96_\xadm&L~!\x18\xef\x02\x81\x80@.\x04\xa6\xd7K\xfb\xb5\r\xb1\xbe\x94\x10\xe6\x14.\xd4\x1a\xf3\x86\x93D`Kx\xf0%{^\xdf\x9c\xd4P\x19w\xe3\t8\xceB\x93\x83m\x85\xdd\xf8\xfc\xd8\xa0Cp>\x9bH\r\\\xedf\x8a\x1f\xe7P\x85\xbe\xbei\xa0\xdf\xa7\xda8s\t\xdbXi\x89s\x05\xa2-C\x1a\xb2r#\xef\xc0\xf7\xda@\xe2T\x99k\xcf\xcc\xbc\xc5\xb7\x10\x8d\x94B\xa4:\xcd\xf6@Ea\xb1\xe2\x1bRw\x03\xf1E\xfdL>\xbd.\xc0\x94S}\x02\x81\x81\x00\xa2\xce\x13}EH}a\x19\xa2`I\xa7\xa0\xcdc4\xe5\xa7\xfa\xa7\xf9\xee\x82\x87\x7f\x7f\x1f\xfbeK\xe9&E=\xcb\x9c\xd1\xa1m\xb21\xc8\xbc\xb76\xaa\xaf\xb0P\xeaU\xc7}\x93\x80\xe9\x91\xd2-\xf4\xbf\x95&\x7f.\x17/\x8f\xa9\xdc\x02\x8a\x06}9:E\xafUBZU?\xaf\x8d\xad\xa2\xdf+]\xa9V\x9c\xfc\xda\x86@\x89\xe7\x9e\xb7\xed{\xa0F\x8d}nV\xca\xb5l\xe9\xedR\xf9\x1d\xc8\x92\xd3\xf7NJ\xa6=E\xdb\x02\x81\x81\x00\xf5\xa8\xec\x00k\x18\x10KK\xd0D\xa9\xeb\x87==X\xa2\xaa)\xeb\x92\xfa\xf8f\xa6W\xaa\x94\x92\xa1F\t\xc1\x01\xd8%-\x1f\xb71\xefg\x95q\xb3\xa5J[k\xe3\x17\xac\xfd\xbfU\x02\x95\xa4\xf9\xcd\x80!E\x9d\x7f\x9c\xcd\x89uV\x1df\xee\xab\xd3\x1f7$&\x014\xd2\xdd\xc2\xe4?\x1bh*\xb6\x00\x1a\x1fz^\xbc\x97\xde\x9cK\xc8\xf5\xcf0\"\x8c\x8bm\xecUv\xefu\xd9YD\x05\xe8?9J\x8c\x18\x90\x0e\xc4\x88"
 
 
 async def my_func() -> None:
-    await PKCS11Session.import_keypair(pub, priv, "my_rsa_key", "rsa_2048")
-    public_key, identifier = await PKCS11Session.public_key_data(
+    await PKCS11Session().import_keypair(pub, priv, "my_rsa_key", "rsa_2048")
+    public_key, identifier = await PKCS11Session().public_key_data(
         "my_rsa_key",
 	key_type="rsa_2048",
     )
     print(public_key)
     print(identifier)
 
     
@@ -163,15 +163,15 @@
 ### Example usage for create_keypair():
 ```python
 import asyncio
 from python_x509_pkcs11.pkcs11_handle import PKCS11Session
 
 
 async def my_func() -> None:
-    public_key, identifier = await PKCS11Session.create_keypair("my_ed25519_key", key_type="ed25519")
+    public_key, identifier = await PKCS11Session().create_keypair("my_ed25519_key", key_type="ed25519")
     print(public_key)
     print(identifier)
 
 
 asyncio.run(my_func())
 ```
 
@@ -182,16 +182,16 @@
 ### Example usage for key_labels():
 ```python
 import asyncio
 from python_x509_pkcs11.pkcs11_handle import PKCS11Session
 
 
 async def my_func() -> None:
-    public_key, identifier = await PKCS11Session.create_keypair("my_ed25519_key")
-    labels = await PKCS11Session.key_labels()
+    public_key, identifier = await PKCS11Session().create_keypair("my_ed25519_key")
+    labels = await PKCS11Session().key_labels()
     print(labels)
 
 
 asyncio.run(my_func())
 ```
 
 ## sign()
@@ -202,16 +202,16 @@
 ```python
 import asyncio
 from python_x509_pkcs11.pkcs11_handle import PKCS11Session
 
 
 async def my_func() -> None:
     data = b"DATA TO BE SIGNED"
-    public_key, identifier = await PKCS11Session.create_keypair("my_ed25519_key")
-    signature = await PKCS11Session.sign("my_ed25519_key", data)
+    public_key, identifier = await PKCS11Session().create_keypair("my_ed25519_key")
+    signature = await PKCS11Session().sign("my_ed25519_key", data)
     print(signature)
 
 
 asyncio.run(my_func())
 ```
 
 ## verify()
@@ -222,17 +222,17 @@
 ```python
 import asyncio
 from python_x509_pkcs11.pkcs11_handle import PKCS11Session
 
 
 async def my_func() -> None:
     data = b"DATA TO BE SIGNED"
-    public_key, identifier = await PKCS11Session.create_keypair("my_ed25519_key")
-    signature = await PKCS11Session.sign("my_ed25519_key", data)
-    if await PKCS11Session.verify("my_ed25519_key", data, signature):
+    public_key, identifier = await PKCS11Session().create_keypair("my_ed25519_key")
+    signature = await PKCS11Session().sign("my_ed25519_key", data)
+    if await PKCS11Session().verify("my_ed25519_key", data, signature):
         print("OK sig")
     else:
         print("BAD sig")
 
 
 asyncio.run(my_func())
 ```
@@ -244,16 +244,16 @@
 ### Example usage for delete_keypair():
 ```python
 import asyncio
 from python_x509_pkcs11.pkcs11_handle import PKCS11Session
 
 
 async def my_func() -> None:
-    public_key, identifier = await PKCS11Session.create_keypair("my_ed25519_key")
-    await PKCS11Session.delete_keypair("my_ed25519_key")
+    public_key, identifier = await PKCS11Session().create_keypair("my_ed25519_key")
+    await PKCS11Session().delete_keypair("my_ed25519_key")
 
 asyncio.run(my_func())
 ```
 
 ## public_key_data()
 
 The `public_key_data()` function returns the data for the x509 'Public Key Info'
@@ -262,18 +262,18 @@
 ### Example usage for public_key_data():
 ```python
 import asyncio
 from python_x509_pkcs11.pkcs11_handle import PKCS11Session
 
 
 async def my_func() -> None:
-    public_key_created, identifier_created = await PKCS11Session.create_keypair(
+    public_key_created, identifier_created = await PKCS11Session().create_keypair(
         "my_ed25519_key"
     )
-    public_key_loaded, identifier_loaded = await PKCS11Session.public_key_data(
+    public_key_loaded, identifier_loaded = await PKCS11Session().public_key_data(
         "my_ed25519_key"
     )
     print(public_key_created)
     print(public_key_loaded)
     print(identifier_created)
     print(identifier_loaded)
 
@@ -309,15 +309,15 @@
 ZDY1YTdlNTg0ZmJjZWMwMTAyMDAWBgNVHSUBAf8EDDAKBggrBgEFBQcDCDAdBgNV
 HQ4EFgQURbRp9puwNsIbOCEcZWzcz3UkK0UwHwYDVR0jBBgwFoAUhtCxna0AdOe6
 J23GIJ4PENiOV6EwCgYIKoZIzj0EAwIDRwAwRAIgCm8D1+Cfwej2pfrPHNV3myIy
 OsgGSmMGs3uYjac7+j4CIHisanLIGlny5Kgnrmk5yNiN3ZFimdhSd+ovaqjy3O4x
 -----END CERTIFICATE-----"""
 
 async def my_func() -> None:
-    await PKCS11Session.import_certificate(cert_pem, "my_cert")
+    await PKCS11Session().import_certificate(cert_pem, "my_cert")
 
 asyncio.run(my_func())
 ```
 
 ## export_certificate()
 
 The `export_certificate()` function export a certificate from the PKCS11 device with this label.
@@ -346,16 +346,16 @@
 ZDY1YTdlNTg0ZmJjZWMwMTAyMDAWBgNVHSUBAf8EDDAKBggrBgEFBQcDCDAdBgNV
 HQ4EFgQURbRp9puwNsIbOCEcZWzcz3UkK0UwHwYDVR0jBBgwFoAUhtCxna0AdOe6
 J23GIJ4PENiOV6EwCgYIKoZIzj0EAwIDRwAwRAIgCm8D1+Cfwej2pfrPHNV3myIy
 OsgGSmMGs3uYjac7+j4CIHisanLIGlny5Kgnrmk5yNiN3ZFimdhSd+ovaqjy3O4x
 -----END CERTIFICATE-----"""
 
 async def my_func() -> None:
-    await PKCS11Session.import_certificate(cert_pem, "my_cert")
-    cert = await PKCS11Session.export_certificate("my_cert")
+    await PKCS11Session().import_certificate(cert_pem, "my_cert")
+    cert = await PKCS11Session().export_certificate("my_cert")
     print(cert)
 
 asyncio.run(my_func())
 ```
 
 ## delete_certificate()
 
@@ -363,15 +363,15 @@
 
 ### Example usage for delete_certificate():
 ```python
 import asyncio
 from python_x509_pkcs11.pkcs11_handle import PKCS11Session
 
 async def my_func() -> None:
-    await PKCS11Session.delete_certificate(cert_pem)
+    await PKCS11Session().delete_certificate(cert_pem)
 
 asyncio.run(my_func())
 ```
 
 # Sign an CSR
 Our [csr](https://github.com/SUNET/python_x509_pkcs11/blob/main/src/python_x509_pkcs11/csr.py) module currently exposes one function:
 
@@ -442,15 +442,15 @@
         "locality_name": "Stockholm",
         "organization_name": "SUNET",
         "organizational_unit_name": "SUNET Infrastructure",
         "common_name": "ca-test.sunet.se",
         "email_address": "soc@sunet.se",
     }
 
-    public_key, identifier = await PKCS11Session.create_keypair("my_ed25519_key")
+    public_key, identifier = await PKCS11Session().create_keypair("my_ed25519_key")
     cert_pem = await csr.sign_csr("my_ed25519_key", issuer_name, csr_pem)
     print(cert_pem)
 
 
 asyncio.run(my_func())
 ```
 
@@ -581,15 +581,15 @@
         "locality_name": "Stockholm",
         "organization_name": "SUNET",
         "organizational_unit_name": "SUNET Infrastructure",
         "common_name": "ca-test.sunet.se",
         "email_address": "soc@sunet.se",
     }
 
-    public_key, identifier = await PKCS11Session.create_keypair("my_ed25519_key")
+    public_key, identifier = await PKCS11Session().create_keypair("my_ed25519_key")
     crl_pem = await create("my_ed25519_key", name_dict)
     print(crl_pem)
 
 
 asyncio.run(my_func())
 ```
 
@@ -754,15 +754,15 @@
         curr_response["cert_status"] = CertStatus("good")
         curr_response["this_update"] = datetime.datetime.now(datetime.timezone.utc) - datetime.timedelta(minutes=2)
         responses.append(curr_response)
     return responses
 
 
 async def my_func() -> None:
-    await PKCS11Session.create_keypair("my_ed25519_key")
+    await PKCS11Session().create_keypair("my_ed25519_key")
     request_certs_data = [
         (
             b"R\x94\xca?\xac`\xf7i\x819\x14\x94\xa7\x085H\x84\xb4&\xcc",
             b"\xad\xd0\x88DW\x96'\xce\xf4\"\xc6\xc77W\xc9\xefi\xa4[\x8b",
             440320505043419981128735462508870123525487964711,
         )
     ]
```

### Comparing `python_x509_pkcs11-0.8.4/pyproject.toml` & `python_x509_pkcs11-0.9.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,37 @@
-description = "Python async library for signing x509 using keys in an pkcs11 device such as a HSM"
-version = "0.8.4"
-
 [build-system]
-requires = [
-    "flit_core >=2.0",
-]
-
-[tool.flit.metadata]
-module = "python_x509_pkcs11"
+requires = ["flit_core >=3.2,<4"]
+build-backend = "flit_core.buildapi"
 
-
-description-file = "README.md"
+[project]
+name = "python_x509_pkcs11"
+dynamic = ["version", "description"]
 requires-python = ">=3.8"
-
-keywords = "x509,pkcs11,HSM"
-license = "MIT"
-author = "Victor Näslund"
-author-email = "victor@sunet.se"
-home-page = "https://github.com/SUNET/python_x509_pkcs11"
-
-requires = [
+#keywords = x509, pkcs11, HSM
+license = {file = "LICENSE"}
+authors = [
+    { name = "Victor Näslund", email = "victor@sunet.se"},
+    { name = "Magnus Svensson", email ="masv@sunet.se"},
+    { name = "Kushal Das", email = "kushal@sunet.se"}
+]
+readme = "README.md"
+dependencies = [
     "asn1crypto>=1.5.1",
     "python-pkcs11>=0.7.0",
-    "aiohttp"
+    "aiohttp",
+    "cryptography >= 40.0"
 ]
 
+
+[project.urls]
+Source = "https://github.com/SUNET/python_x509_pkcs11"
+
+[tool.flit.sdist]
+include = ["LICENSE", "README.MD"]
+
 [tool.mypy]
 strict = true
 mypy_path = "src"
 packages = "python_x509_pkcs11"
 
 [[tool.mypy.overrides]]
 module = [
```

### Comparing `python_x509_pkcs11-0.8.4/src/python_x509_pkcs11/crypto.py` & `python_x509_pkcs11-0.9.0/src/python_x509_pkcs11/crypto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Our crypto module"""
+
 from typing import Dict, Tuple, Union
 
 from asn1crypto.algos import SignedDigestAlgorithmId
 from asn1crypto.keys import OctetString, PrivateKeyInfo, PublicKeyInfo
 from pkcs11 import Attribute, Key, KeyType, ObjectClass
 from pkcs11.util.ec import encode_named_curve_parameters
 
@@ -178,17 +179,17 @@
 
     asn1 = PrivateKeyInfo.load(der)
     return {
         Attribute.KEY_TYPE: KeyType.EC_EDWARDS,
         Attribute.CLASS: ObjectClass.PRIVATE_KEY,
         Attribute.EC_PARAMS: encode_named_curve_parameters(SignedDigestAlgorithmId(asn1.algorithm).dotted),
         # Only the last 32/57 bytes is the private key values
-        Attribute.VALUE: asn1["private_key"].contents[-32:]
-        if asn1.algorithm == "ed25519"
-        else asn1["private_key"].contents[-57:],
+        Attribute.VALUE: (
+            asn1["private_key"].contents[-32:] if asn1.algorithm == "ed25519" else asn1["private_key"].contents[-57:]
+        ),
     }
 
 
 def encode_eddsa_public_key(key: Key) -> bytes:
     """
     Encode a DER-encoded EdDSA public key as stored by OpenSSL.
     :param PublicKey key: EdDSA public key
```

### Comparing `python_x509_pkcs11-0.8.4/src/python_x509_pkcs11/ocsp.py` & `python_x509_pkcs11-0.9.0/src/python_x509_pkcs11/ocsp.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,16 +4,19 @@
 - request() - Create a OCSP request
 - response() - Create a OCSP response
 - request_nonce() - Quickly extract the nonce or None from a OCSP request
 - certificate_ocsp_data() - Quickly extract the OCSP data from a certificate
 """
 
 import datetime
+import logging
 from typing import Dict, List, Optional, Tuple, Union
 
+logger = logging.getLogger(__name__)
+
 from asn1crypto import pem as asn1_pem
 from asn1crypto.algos import DigestAlgorithm, DigestAlgorithmId
 from asn1crypto.ocsp import (
     BasicOCSPResponse,
     CertId,
     Certificate,
     Certificates,
@@ -32,15 +35,15 @@
     ResponseType,
     Signature,
     TBSRequest,
     TBSRequestExtensions,
 )
 
 from .error import DuplicateExtensionException, OCSPMissingExtensionException
-from .lib import signed_digest_algo
+from .lib import DEFAULT_KEY_TYPE, KEYTYPES, get_keytypes_enum, signed_digest_algo
 from .pkcs11_handle import PKCS11Session
 
 
 def _create_ocsp_request(issuer_name_hash: bytes, issuer_key_hash: bytes, serial_number: int) -> Request:
     cert_id = CertId()
     cert_id["issuer_name_hash"] = issuer_name_hash
     cert_id["issuer_key_hash"] = issuer_key_hash
@@ -65,16 +68,16 @@
     exts = ResponseDataExtensions()
 
     for _, ext in enumerate(extra_extensions):
         if ext["extn_id"].dotted == "1.3.6.1.5.5.7.48.1.2":
             if len(ext["extn_value"].native) < 1 or len(ext["extn_value"].native) > 32:
                 raise ValueError("Nonce length error, https://datatracker.ietf.org/doc/html/rfc8954")
             if len(ext["extn_value"].native) < 16:
-                print("Warning: Ignoring nonce since its smaller than 16 bytes")
-                print("https://datatracker.ietf.org/doc/html/rfc8954")
+                logger.warn("Warning: Ignoring nonce since its smaller than 16 bytes")
+                logger.warn("https://datatracker.ietf.org/doc/html/rfc8954")
                 continue
 
         exts.append(ext)
     response_data["response_extensions"] = exts
 
     return response_data
 
@@ -126,20 +129,18 @@
         exts.append(ext["extn_id"].dotted)
 
     return response_data
 
 
 async def _set_response_signature(
     key_label: str,
-    key_type: Optional[str],
     extra_certs: Optional[List[str]],
     basic_ocsp_response: BasicOCSPResponse,
+    key_type: KEYTYPES = DEFAULT_KEY_TYPE,
 ) -> BasicOCSPResponse:
-    if key_type is None:
-        key_type = "ed25519"
 
     basic_ocsp_response["signature_algorithm"] = signed_digest_algo(key_type)
     basic_ocsp_response["signature"] = await PKCS11Session().sign(
         key_label,
         basic_ocsp_response["tbs_response_data"].dump(),
         key_type=key_type,
     )
@@ -154,21 +155,19 @@
         basic_ocsp_response["certs"] = resp_certs
 
     return basic_ocsp_response
 
 
 async def _set_request_signature(
     key_label: str,
-    key_type: Optional[str],
     signature: Signature,
     data: TBSRequest,
     certs: Optional[List[str]],
+    key_type: KEYTYPES = DEFAULT_KEY_TYPE,
 ) -> Signature:
-    if key_type is None:
-        key_type = "ed25519"
 
     signature["signature_algorithm"] = signed_digest_algo(key_type)
     signature["signature"] = await PKCS11Session().sign(key_label, data.dump(), key_type=key_type)
 
     if certs is not None and certs:
         req_certs = Certificates()
         for cert in certs:
@@ -274,15 +273,15 @@
 
 async def request(  # pylint: disable-msg=too-many-arguments
     request_certs_data: List[Tuple[bytes, bytes, int]],
     key_label: Optional[str] = None,
     requestor_name: Optional[GeneralName] = None,
     certs: Optional[List[str]] = None,
     extra_extensions: Optional[TBSRequestExtensions] = None,
-    key_type: Optional[str] = None,
+    key_type: Union[str, KEYTYPES] = DEFAULT_KEY_TYPE,
 ) -> bytes:
     """Create an OCSP request.
     See https://www.rfc-editor.org/rfc/rfc6960#section-4.1.1
 
     If key_label is not None and requestor_name is not None
     Then sign the request with the key_label key in the PKCS11 device.
 
@@ -295,14 +294,17 @@
     extra_extensions (Optional[asn1crypto.ocsp.TBSRequestExtensions] = None): Extra extensions.
     key_type (Optional[str] = None): Key type to use, ed25519 is default.
 
     Returns:
     bytes
     """
 
+    if isinstance(key_type, str):
+        key_type = get_keytypes_enum(key_type)
+
     # Ensure input data has least one cert data tuple
     if not request_certs_data:
         raise ValueError("request_certs_data must NOT be empty")
 
     reqs = Requests()
     for cert_data in request_certs_data:
         req = _create_ocsp_request(cert_data[0], cert_data[1], cert_data[2])
@@ -322,30 +324,30 @@
     ocsp_request["tbs_request"] = tbs_request
 
     if key_label is not None:
         if requestor_name is None:
             raise ValueError("signing a request requires the requestor_name parameter")
 
         ocsp_request["optional_signature"] = await _set_request_signature(
-            key_label, key_type, Signature(), ocsp_request["tbs_request"], certs
+            key_label, Signature(), ocsp_request["tbs_request"], certs, key_type
         )
 
     ret: bytes = ocsp_request.dump()
     return ret
 
 
 async def response(  # pylint: disable-msg=too-many-arguments
     key_label: str,
     responder_id: Union[Dict[str, str], bytes],
     single_responses: Responses,
     response_status: int,
     extra_extensions: Optional[ResponseDataExtensions] = None,
     produced_at: Optional[datetime.datetime] = None,
     extra_certs: Optional[List[str]] = None,
-    key_type: Optional[str] = None,
+    key_type: Union[str, KEYTYPES] = DEFAULT_KEY_TYPE,
 ) -> bytes:
     """Create an OCSP response with the key_label key in the PKCS11 device.
     See https://www.rfc-editor.org/rfc/rfc6960#section-4.2.1
 
     Parameters:
     key_label (str): Keypair label in the PKCS11 device to sign with.
     responder_id (Dict[str, str]): Dict with the responders x509 Names.
@@ -353,22 +355,25 @@
     response_status (int): Status code for the OCSP response.
     extra_extensions (Optional[asn1crypto.ocsp.ResponseDataExtensions] = None):
     Extra extensions to be written into the response, for example the nonce extension.
     produced_at (Optional[datetime.datetime] = None): What time to write into produced_at.
     It must be in UTC timezone. If None then it will be 2 minutes before UTC now.
     extra_certs (Optional[List[str]] = None): List of PEM encoded certs
     for the client to verify the signature chain.
-    key_type (Optional[str] = None): Key type to use, ed25519 is default.
+    key_type (Union[str, KEYTYPES]): Key type to use, KEYTPES.ED25519 is default.
 
     Returns:
     bytes
     """
 
     ret: bytes
 
+    if isinstance(key_type, str):
+        key_type = get_keytypes_enum(key_type)
+
     # Ensure valid response status
     if response_status not in [0, 1, 2, 3, 5, 6]:  # 4 is not used
         raise ValueError("status code must be one of [0, 1, 2, 3, 5, 6]")
 
     # OCSP response
     ocsp_response = OCSPResponse()
 
@@ -385,15 +390,15 @@
 
     # Set response data
     basic_ocsp_response["tbs_response_data"] = _set_response_data(
         single_responses, responder_id, produced_at, extra_extensions
     )
 
     # Sign the response
-    basic_ocsp_response = await _set_response_signature(key_label, key_type, extra_certs, basic_ocsp_response)
+    basic_ocsp_response = await _set_response_signature(key_label, extra_certs, basic_ocsp_response, key_type)
 
     # Response bytes
     response_bytes = ResponseBytes()
     response_bytes["response_type"] = ResponseType("1.3.6.1.5.5.7.48.1.1")
     response_bytes["response"] = basic_ocsp_response
     ocsp_response["response_bytes"] = response_bytes
```

### Comparing `python_x509_pkcs11-0.8.4/src/python_x509_pkcs11/pkcs11_handle.py` & `python_x509_pkcs11-0.9.0/src/python_x509_pkcs11/pkcs11_handle.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 """Module which handles a PKCS11 session and its exposed methods
 
 # Better to keep a pkcs11 session reference all the time
 # and then when it fails to open a new session for performance
-# See PKCS11Session._healthy_session()
+# See PKCS11Session()._healthy_session()
 
 The classes PKCS11Session and RemotePKCS11 exposes the functions:
 - import_keypair()
 - create_keypair()
 - key_labels()
 - sign()
 - verify()
 - delete_keypair()
 - public_key_data()
 - import_certificate()
 - export_certificate()
 - delete_certificate()
 - get_session()
 """
+
 import base64
+import logging
 import os
 import time
 from asyncio import get_event_loop, sleep
 from concurrent.futures import ThreadPoolExecutor
 from contextlib import asynccontextmanager
 from email import header
 from hashlib import sha256, sha384, sha512
 from socket import timeout
 from threading import Lock, Thread
-from typing import AsyncIterator, Dict, Optional, Tuple, Union
+from typing import Any, AsyncIterator, Dict, Optional, Tuple, Type, Union
+
+logger = logging.getLogger(__name__)
 
 import aiohttp
 from asn1crypto import pem as asn1_pem
 from asn1crypto import x509 as asn1_x509
 from asn1crypto.algos import SignedDigestAlgorithmId
 from asn1crypto.keys import PublicKeyAlgorithm, PublicKeyAlgorithmId, PublicKeyInfo, RSAPublicKey
 from pkcs11 import Attribute, Key, KeyType, Mechanism, ObjectClass, Session, Token, lib
@@ -49,15 +53,15 @@
     convert_asn1_ec_signature,
     convert_rs_ec_signature,
     decode_eddsa_private_key,
     decode_eddsa_public_key,
     encode_eddsa_public_key,
 )
 from .error import PKCS11UnknownErrorException
-from .lib import DEBUG, key_type_values, key_types
+from .lib import DEBUG, DEFAULT_KEY_TYPE, KEY_TYPE_VALUES, KEYTYPES, get_keytypes_enum
 
 TIMEOUT = 10  # Seconds
 pool = ThreadPoolExecutor()
 
 
 @asynccontextmanager
 async def async_lock(lock: Lock) -> AsyncIterator[None]:
@@ -71,284 +75,275 @@
     finally:
         lock.release()
 
 
 class PKCS11Session:
     """Persistent PKCS11 session wrapper."""
 
+    # We want a single instance of this class.
+    # Because pkcs11 allows one connection to the pkcs11 device.
+    _self = None
+
     _session_status: int = 9
     _token: Token
     _lib: lib
 
-    support_recreate_session: Optional[bool] = None
-    base_url: Optional[str]
-    http_data: Optional[Dict[str, str]] = None
-    http_headers: Optional[Dict[str, str]] = None
+    def __new__(cls, *args: Any, **kwargs: Any) -> "PKCS11Session":
+        if cls._self is None:
+            cls._self = super(PKCS11Session, cls).__new__(cls, *args, **kwargs)
+        return cls._self
 
-    lock = Lock()
-    session: Session
-
-    @classmethod
     def __init__(
-        cls,
+        self,
         base_url: Optional[str] = None,
         http_data: Optional[Dict[str, str]] = None,
         http_headers: Optional[Dict[str, str]] = None,
     ) -> None:
-        cls.base_url = base_url
-        cls.http_data = http_data
-        cls.http_headers = http_headers
+        self.lock = Lock()
+
+        self.base_url = base_url
+        self.http_data = http_data
+        self.http_headers = http_headers
+        self.support_recreate_session = False
 
         if "PKCS11_BASE_URL" in os.environ:
-            cls.base_url = os.environ["PKCS11_BASE_URL"]
+            self.base_url = os.environ["PKCS11_BASE_URL"]
             return
 
-        cls.support_recreate_session = False
+        # TODO: Update the recreate session code in a cleaner way.
+
         if "PKCS11_TOKEN_SUPPORT_RECREATE_SESSION" in os.environ:
             if (
                 os.environ["PKCS11_TOKEN_SUPPORT_RECREATE_SESSION"] == "true"
                 or os.environ["PKCS11_TOKEN_SUPPORT_RECREATE_SESSION"] == "TRUE"
             ):
-                cls.support_recreate_session = True
+                self.support_recreate_session = True
 
-        if not cls.support_recreate_session:
-            try:
-                if hasattr(cls, "session"):
-                    return
+        try:
 
-                cls._lib = lib(os.environ["PKCS11_MODULE"])
-                cls._lib.reinitialize()
+            self._lib = lib(os.environ["PKCS11_MODULE"])
+            self._lib.reinitialize()
 
-                # Open the PKCS11 session
-                cls._token = cls._lib.get_token(token_label=os.environ["PKCS11_TOKEN"])
+            # Open the PKCS11 session
+            self._token = self._lib.get_token(token_label=os.environ["PKCS11_TOKEN"])
 
-                # user_pin need to be a string, not bytes
-                cls.session = cls._token.open(rw=True, user_pin=os.environ["PKCS11_PIN"])
-                print("created new pkcs11 session")
+            # user_pin need to be a string, not bytes
+            self.session = self._token.open(rw=True, user_pin=os.environ["PKCS11_PIN"])
+            logger.debug("created new pkcs11 session")
 
-                # Test get a public key from the PKCS11 device
-                _ = cls.session.get_key(
-                    key_type=KeyType.RSA,
-                    object_class=ObjectClass.PUBLIC_KEY,
-                    label="test_pkcs11_device_do_not_use",
+            # Test get a public key from the PKCS11 device
+            _ = self.session.get_key(
+                key_type=KeyType.RSA,
+                object_class=ObjectClass.PUBLIC_KEY,
+                label="test_pkcs11_device_do_not_use",
+            )
+
+        except NoSuchKey:
+            try:
+                _, _ = self.session.generate_keypair(
+                    KeyType.RSA, 512, label="test_pkcs11_device_do_not_use", store=True
                 )
+            except GeneralError:
+                pass
 
-            except NoSuchKey:
-                try:
-                    _, _ = cls.session.generate_keypair(
-                        KeyType.RSA, 512, label="test_pkcs11_device_do_not_use", store=True
-                    )
-                except GeneralError:
-                    pass
+        except GeneralError as exc:
+            logger.error("Failed to open PKCS11 session")
+            logger.error(exc)
 
-            except GeneralError as exc:
-                if DEBUG:
-                    print("Failed to open PKCS11 session")
-                    print(exc)
-
-    @classmethod
-    def _get_pub_key(cls, key_label: str, key_type: str) -> Key:
-        return cls.session.get_key(
-            key_type=key_type_values[key_type],
+    def _get_pub_key(self, key_label: str, key_type: KEYTYPES = DEFAULT_KEY_TYPE) -> Key:
+        return self.session.get_key(
+            key_type=KEY_TYPE_VALUES[key_type],
             object_class=ObjectClass.PUBLIC_KEY,
             label=key_label,
         )
 
-    @classmethod
-    def _public_key_data(cls, key_pub: Key, key_type: str) -> Tuple[str, bytes]:
-        if key_type in ["rsa_2048", "rsa_4096"]:
+    def _public_key_data(self, key_pub: Key, key_type: KEYTYPES) -> Tuple[str, bytes]:
+        if key_type in [KEYTYPES.RSA2048, KEYTYPES.RSA4096]:
             # Create the PublicKeyInfo object
             rsa_pub = RSAPublicKey.load(encode_rsa_public_key(key_pub))
 
             pki = PublicKeyInfo()
             pka = PublicKeyAlgorithm()
             pka["algorithm"] = PublicKeyAlgorithmId("rsa")
             pki["algorithm"] = pka
             pki["public_key"] = rsa_pub
 
-        elif key_type in ["ed25519", "ed448"]:
+        elif key_type in [KEYTYPES.ED25519, KEYTYPES.ED448]:
             pki = PublicKeyInfo.load(encode_eddsa_public_key(key_pub))
 
-        elif key_type in ["secp256r1", "secp384r1", "secp521r1"]:
+        elif key_type in [KEYTYPES.SECP256r1, KEYTYPES.SECP384r1, KEYTYPES.SECP521r1]:
             pki = PublicKeyInfo.load(encode_ec_public_key(key_pub))
-        else:
-            raise ValueError(f"key_type must be in {key_types}")
 
         key_pub_pem: bytes = asn1_pem.armor("PUBLIC KEY", pki.dump())
         return key_pub_pem.decode("utf-8"), pki.sha1
 
-    @classmethod
-    def _open_session(cls, force: Optional[bool] = None, simulate_pkcs11_timeout: Optional[bool] = None) -> None:
+    def _open_session(self, force: Optional[bool] = None, simulate_pkcs11_timeout: Optional[bool] = None) -> None:
         if simulate_pkcs11_timeout:
             time.sleep(TIMEOUT + 1)
 
         if "PKCS11_MODULE" not in os.environ:
-            print("ERROR: PKCS11_MODULE was not an env variable")
+            logger.error("ERROR: PKCS11_MODULE was not an env variable")
         if "PKCS11_TOKEN" not in os.environ:
-            print("ERROR: PKCS11_TOKEN was not an env variable")
+            logger.error("ERROR: PKCS11_TOKEN was not an env variable")
         if "PKCS11_PIN" not in os.environ:
-            print("ERROR: PKCS11_PIN was not an env variable")
+            logger.error("ERROR: PKCS11_PIN was not an env variable")
 
-        cls._session_status = 9
+        self._session_status = 9
         try:
-            # if force or cls.session is None:
-            if force or not hasattr(cls, "session"):
+            # if force or self.session is None:
+            if force or self.session is None:
                 # Reload the PKCS11 lib
-                cls._lib = lib(os.environ["PKCS11_MODULE"])
-                cls._lib.reinitialize()
+                self._lib = lib(os.environ["PKCS11_MODULE"])
+                self._lib.reinitialize()
 
                 # Open the PKCS11 session
-                cls._token = cls._lib.get_token(token_label=os.environ["PKCS11_TOKEN"])
+                self._token = self._lib.get_token(token_label=os.environ["PKCS11_TOKEN"])
                 # user_pin need to be a string, not bytes
-                cls.session = cls._token.open(rw=True, user_pin=os.environ["PKCS11_PIN"])
-                print("created new pkcs11 session")
+                self.session = self._token.open(rw=True, user_pin=os.environ["PKCS11_PIN"])
+                logger.debug("created new pkcs11 session")
 
             # Test get a public key from the PKCS11 device
-            _ = cls.session.get_key(
+            _ = self.session.get_key(
                 key_type=KeyType.RSA,
                 object_class=ObjectClass.PUBLIC_KEY,
                 label="test_pkcs11_device_do_not_use",
             )
-            cls._session_status = 0
+            self._session_status = 0
 
         except NoSuchKey:
             try:
-                _, _ = cls.session.generate_keypair(KeyType.RSA, 512, label="test_pkcs11_device_do_not_use", store=True)
-                cls._session_status = 0
+                _, _ = self.session.generate_keypair(
+                    KeyType.RSA, 512, label="test_pkcs11_device_do_not_use", store=True
+                )
+                self._session_status = 0
             except GeneralError:
                 pass
 
         except GeneralError as exc:
-            if DEBUG:
-                print("Failed to open PKCS11 session")
-                print(exc)
+            logger.error("Failed to open PKCS11 session")
+            logger.error(exc)
 
-    @classmethod
-    async def healthy_session(cls, simulate_pkcs11_timeout: Optional[bool] = None) -> None:
+    async def healthy_session(self, simulate_pkcs11_timeout: Optional[bool] = None) -> None:
         """Run the PKCS11 test command in a thread to easy handle PKCS11 timeouts."""
 
-        if not cls.support_recreate_session:
+        if not self.support_recreate_session:
             return
-
-        thread = Thread(target=cls._open_session, args=([False, simulate_pkcs11_timeout]))
+        thread = Thread(target=self._open_session, args=(False, simulate_pkcs11_timeout))
         thread.start()
         await sleep(0)
         thread.join(timeout=TIMEOUT)
 
-        if thread.is_alive() or cls._session_status != 0:
-            thread2 = Thread(target=cls._open_session, args=([True, simulate_pkcs11_timeout]))
+        if thread.is_alive() or self._session_status != 0:
+            thread2 = Thread(target=self._open_session, args=(True, simulate_pkcs11_timeout))
             thread2.start()
             # yield to other coroutines while we wait for thread2 to join
             await sleep(0)
             thread2.join(timeout=TIMEOUT)
 
-            if thread2.is_alive() or cls._session_status != 0:
+            if thread2.is_alive() or self._session_status != 0:
                 raise PKCS11UnknownErrorException("ERROR: Could not get a healthy PKCS11 connection in time")
 
-    @classmethod
-    async def get_session(cls) -> Session:
+    async def get_session(self) -> Session:
         """Return the PKCS11 session."""
 
-        async with async_lock(cls.lock):
+        async with async_lock(self.lock):
             # Ensure we get a healthy pkcs11 session
-            await cls.healthy_session()
-            return cls.session
+            await self.healthy_session()
+            return self.session
 
-    @classmethod
-    async def import_certificate(cls, cert_pem: str, cert_label: str) -> None:
+    async def import_certificate(self, cert_pem: str, cert_label: str) -> None:
         """Import a certificate into the PKCS11 device with this label.
 
         Parameters:
         cert_pem (str): Certificate in PEM form.
         cert_label (str): Certificate label in the PKCS11 device.
 
         Returns:
         None
         """
 
-        if cls.base_url is not None:
+        if self.base_url is not None:
             http_request_data: Dict[str, str] = {}
 
-            if cls.http_data is not None:
-                http_request_data.update(cls.http_data)
+            if self.http_data is not None:
+                http_request_data.update(self.http_data)
 
             http_request_data["cert_pem"] = cert_pem
             http_request_data["cert_label"] = cert_label
 
-            async with aiohttp.ClientSession(headers=cls.http_headers) as session:
+            async with aiohttp.ClientSession(headers=self.http_headers) as session:
                 async with session.post(
-                    url=f"{cls.base_url}/import_certificate",
+                    url=f"{self.base_url}/import_certificate",
                     json=http_request_data,
-                    headers=cls.http_headers,
+                    headers=self.http_headers,
                     timeout=10,
                 ) as response:
                     response.raise_for_status()
                     # json_body = await response.json()
                     return
 
-        async with async_lock(cls.lock):
+        async with async_lock(self.lock):
             # Ensure we get a healthy pkcs11 session
-            await cls.healthy_session()
+            await self.healthy_session()
 
-            for cert in cls.session.get_objects(
+            for cert in self.session.get_objects(
                 {
                     Attribute.CLASS: ObjectClass.CERTIFICATE,
                     Attribute.LABEL: cert_label,
                 }
             ):
                 raise ValueError("Certificate with that label already exists in the PKCS11 device")
 
             data = cert_pem.encode("utf-8")
             if asn1_pem.detect(data):
                 _, _, data = asn1_pem.unarmor(data)
 
             cert = decode_x509_certificate(data)
             cert[Attribute.TOKEN] = True
             cert[Attribute.LABEL] = cert_label
-            cls.session.create_object(cert)
+            self.session.create_object(cert)
 
-    @classmethod
-    async def export_certificate(cls, cert_label: str) -> str:
+    async def export_certificate(self, cert_label: str) -> str:
         """Export a certificate from the PKCS11 device with this label.
         Returns the PEM encoded cert.
 
         Parameters:
         cert_label (str): Certificate label in the PKCS11 device.
 
         Returns:
         str
         """
 
-        if cls.base_url is not None:
+        if self.base_url is not None:
             http_request_data: Dict[str, str] = {}
 
-            if cls.http_data is not None:
-                http_request_data.update(cls.http_data)
+            if self.http_data is not None:
+                http_request_data.update(self.http_data)
 
             http_request_data["cert_label"] = cert_label
 
-            async with aiohttp.ClientSession(headers=cls.http_headers) as session:
+            async with aiohttp.ClientSession(headers=self.http_headers) as session:
                 async with session.post(
-                    url=f"{cls.base_url}/export_certificate",
+                    url=f"{self.base_url}/export_certificate",
                     json=http_request_data,
-                    headers=cls.http_headers,
+                    headers=self.http_headers,
                     timeout=10,
                 ) as response:
                     response.raise_for_status()
                     json_body = await response.json()
                     ret = json_body["certificate"]  # handle errors
                     if isinstance(ret, str):
                         return ret
                     raise ValueError("Problem with cert")
 
-        async with async_lock(cls.lock):
+        async with async_lock(self.lock):
             # Ensure we get a healthy pkcs11 session
-            await cls.healthy_session()
+            await self.healthy_session()
 
-            for cert in cls.session.get_objects(
+            for cert in self.session.get_objects(
                 {
                     Attribute.CLASS: ObjectClass.CERTIFICATE,
                     Attribute.LABEL: cert_label,
                 }
             ):
                 der_bytes = cert[Attribute.VALUE]
 
@@ -357,601 +352,573 @@
 
                 # Write out a PEM encoded value
                 ret_data: bytes = asn1_pem.armor("CERTIFICATE", cert_asn1.dump())
                 return ret_data.decode("utf-8")
 
             raise ValueError("No such certificate in the PKCS11 device")
 
-    @classmethod
-    async def delete_certificate(cls, cert_label: str) -> None:
+    async def delete_certificate(self, cert_label: str) -> None:
         """Delete a certificate from the PKCS11 device with this label.
 
         Parameters:
         cert_label (str): Certificate label in the PKCS11 device.
         """
 
-        if cls.base_url is not None:
+        if self.base_url is not None:
             http_request_data: Dict[str, str] = {}
 
-            if cls.http_data is not None:
-                http_request_data.update(cls.http_data)
+            if self.http_data is not None:
+                http_request_data.update(self.http_data)
 
             http_request_data["cert_label"] = cert_label
 
-            async with aiohttp.ClientSession(headers=cls.http_headers) as session:
+            async with aiohttp.ClientSession(headers=self.http_headers) as session:
                 async with session.post(
-                    url=f"{cls.base_url}/delete_certificate",
+                    url=f"{self.base_url}/delete_certificate",
                     json=http_request_data,
-                    headers=cls.http_headers,
+                    headers=self.http_headers,
                     timeout=10,
                 ) as response:
                     response.raise_for_status()
                     return
                     # json_body = await response.json()
                     # return json_body["cert_label"] # handle errors
 
-        async with async_lock(cls.lock):
+        async with async_lock(self.lock):
             # Ensure we get a healthy pkcs11 session
-            await cls.healthy_session()
+            await self.healthy_session()
 
-            for cert in cls.session.get_objects(
+            for cert in self.session.get_objects(
                 {
                     Attribute.CLASS: ObjectClass.CERTIFICATE,
                     Attribute.LABEL: cert_label,
                 }
             ):
                 cert.destroy()
 
-    @classmethod
-    async def import_keypair(cls, public_key: bytes, private_key: bytes, key_label: str, key_type: str) -> None:
+    async def import_keypair(
+        self, public_key: bytes, private_key: bytes, key_label: str, key_type: Union[str, KEYTYPES]
+    ) -> None:
         """Import a DER encoded keypair into the PKCS11 device with this label.
         If the label already exists in the PKCS11 device then raise pkcs11.MultipleObjectsReturned.
 
         Generating public_key and private_key can be done with:
         openssl genpkey -algorithm ed25519 -out private.pem
         openssl pkey -in private.pem -outform DER -out private.key
         openssl pkey -in private.pem -pubout -out public.pem
         openssl pkey -in private.pem -pubout -outform DER -out public.key
 
         Parameters:
         public_key (bytes): Public RSA key in DER form.
         private_key (bytes): Private RSA key in DER form.
         key_label (str): Keypair label.
-        key_type (str): Key type.
+        key_type Union[str, KEYTYPES]: Key type in string or enum.
 
         Returns:
         None
         """
 
-        if key_type not in key_types:
-            raise ValueError(f"key_type must be in {key_types}")
+        if isinstance(key_type, str):
+            key_type = get_keytypes_enum(key_type)
 
-        if cls.base_url is not None:
+        if self.base_url is not None:
             http_request_data: Dict[str, str] = {}
 
-            if cls.http_data is not None:
-                http_request_data.update(cls.http_data)
+            if self.http_data is not None:
+                http_request_data.update(self.http_data)
 
             http_request_data["public_key_b64"] = base64.b64encode(public_key).decode("utf-8")
             http_request_data["private_key_b64"] = base64.b64encode(private_key).decode("utf-8")
             http_request_data["key_label"] = key_label
-            http_request_data["key_type"] = key_type
+            http_request_data["key_type"] = key_type.value
 
-            async with aiohttp.ClientSession(headers=cls.http_headers) as session:
+            async with aiohttp.ClientSession(headers=self.http_headers) as session:
                 async with session.post(
-                    url=f"{cls.base_url}/import_keypair", json=http_request_data, headers=cls.http_headers, timeout=10
+                    url=f"{self.base_url}/import_keypair", json=http_request_data, headers=self.http_headers, timeout=10
                 ) as response:
                     response.raise_for_status()
                     return
                     # json_body = await response.json()
 
-        async with async_lock(cls.lock):
+        async with async_lock(self.lock):
             # Ensure we get a healthy pkcs11 session
-            await cls.healthy_session()
+            await self.healthy_session()
 
             try:
-                key_pub = cls._get_pub_key(key_label, key_type)
+                key_pub = self._get_pub_key(key_label, key_type)
                 raise MultipleObjectsReturned
             except NoSuchKey:
                 pass
 
-            if key_type in ["rsa_2048", "rsa_4096"]:
+            if key_type in [KEYTYPES.RSA2048, KEYTYPES.RSA4096]:
                 key_pub = decode_rsa_public_key(public_key)
                 key_priv = decode_rsa_private_key(private_key)
 
-            elif key_type in ["ed25519", "ed448"]:
+            elif key_type in [KEYTYPES.ED25519, KEYTYPES.ED448]:
                 key_pub = decode_eddsa_public_key(public_key)
                 key_priv = decode_eddsa_private_key(private_key)
 
-            elif key_type in ["secp256r1", "secp384r1", "secp521r1"]:
+            elif key_type in [KEYTYPES.SECP256r1, KEYTYPES.SECP384r1, KEYTYPES.SECP521r1]:
                 key_pub = decode_ec_public_key(public_key)
                 key_priv = decode_ec_private_key(private_key)
 
             key_pub[Attribute.TOKEN] = True
             key_pub[Attribute.LABEL] = key_label
             key_priv[Attribute.TOKEN] = True
             key_priv[Attribute.LABEL] = key_label
 
-            cls.session.create_object(key_pub)
-            cls.session.create_object(key_priv)
+            self.session.create_object(key_pub)
+            self.session.create_object(key_priv)
 
-    @classmethod
-    async def create_keypair(cls, key_label: str, key_type: Optional[str] = None) -> Tuple[str, bytes]:
+    async def create_keypair(
+        self, key_label: str, key_type: Union[str, KEYTYPES] = DEFAULT_KEY_TYPE
+    ) -> Tuple[str, bytes]:
         """Create an RSA keypair in the PKCS11 device with this label.
         If the label already exists in the PKCS11 device then raise pkcs11.MultipleObjectsReturned.
         Returns the data for the x509 'Subject Public Key Info'
         and x509 extension 'Subject Key Identifier' valid for this keypair.
 
         ed25519 is default key_type.
 
         Parameters:
         key_label (str): Keypair label.
-        key_type (str = None): Key type.
+        key_type str: Key type, defaults to "ed25519".
 
 
         Returns:
         Tuple[str, bytes]
         """
 
-        if key_type is None:
-            key_type = "ed25519"
-
-        if key_type not in key_types:
-            raise ValueError(f"key_type must be in {key_types}")
+        if isinstance(key_type, str):
+            key_type = get_keytypes_enum(key_type)
 
-        if cls.base_url is not None:
+        if self.base_url is not None:
             http_request_data: Dict[str, str] = {}
 
-            if cls.http_data is not None:
-                http_request_data.update(cls.http_data)
+            if self.http_data is not None:
+                http_request_data.update(self.http_data)
 
             http_request_data["key_label"] = key_label
-            http_request_data["key_type"] = key_type
+            http_request_data["key_type"] = key_type.value
 
-            async with aiohttp.ClientSession(headers=cls.http_headers) as session:
+            async with aiohttp.ClientSession(headers=self.http_headers) as session:
                 async with session.post(
-                    url=f"{cls.base_url}/create_keypair", json=http_request_data, headers=cls.http_headers, timeout=10
+                    url=f"{self.base_url}/create_keypair", json=http_request_data, headers=self.http_headers, timeout=10
                 ) as response:
                     response.raise_for_status()
                     json_body = await response.json()
                     spi = json_body["subjectPublicKeyInfo"]  # handle errors
                     ski = json_body["subjectKeyIdentifier_b64"]
 
                     if isinstance(spi, str) and isinstance(ski, str):  # handle errors
                         return spi, base64.b64decode(ski)
                     raise ValueError("Problem with create keypair")
 
-        async with async_lock(cls.lock):
+        async with async_lock(self.lock):
             # Ensure we get a healthy pkcs11 session
-            await cls.healthy_session()
+            await self.healthy_session()
 
             # Try to get the key, if not exist then create it
             try:
-                key_pub = cls._get_pub_key(key_label, key_type)
+                key_pub = self._get_pub_key(key_label, key_type)
                 raise MultipleObjectsReturned
             except NoSuchKey:
                 # Generate the rsa keypair
-                if key_type in ["rsa_2048", "rsa_4096"]:
-                    key_pub, _ = cls.session.generate_keypair(
-                        KeyType.RSA, int(key_type.split("_")[1]), store=True, label=key_label
+                if key_type in [KEYTYPES.RSA2048, KEYTYPES.RSA4096]:
+                    key_pub, _ = self.session.generate_keypair(
+                        KeyType.RSA, int(key_type.value.split("_")[1]), store=True, label=key_label
                     )
 
-                elif key_type in ["ed25519", "ed448"]:
-                    parameters = cls.session.create_domain_parameters(
+                elif key_type in [KEYTYPES.ED25519, KEYTYPES.ED448]:
+                    parameters = self.session.create_domain_parameters(
                         KeyType.EC_EDWARDS,
                         {
                             Attribute.EC_PARAMS: encode_named_curve_parameters(
-                                SignedDigestAlgorithmId(key_type).dotted
+                                SignedDigestAlgorithmId(key_type.value).dotted
                             ),
                         },
                         local=True,
                     )
                     key_pub, _ = parameters.generate_keypair(
                         mechanism=Mechanism.EC_EDWARDS_KEY_PAIR_GEN, store=True, label=key_label
                     )
 
-                elif key_type in ["secp256r1", "secp384r1", "secp521r1"]:
-                    parameters = cls.session.create_domain_parameters(
+                elif key_type in [KEYTYPES.SECP256r1, KEYTYPES.SECP384r1, KEYTYPES.SECP521r1]:
+                    parameters = self.session.create_domain_parameters(
                         KeyType.EC,
-                        {Attribute.EC_PARAMS: encode_named_curve_parameters(key_type)},
+                        {Attribute.EC_PARAMS: encode_named_curve_parameters(key_type.value)},
                         local=True,
                     )
                     key_pub, _ = parameters.generate_keypair(
                         store=True,
                         label=key_label,
                     )
 
-            return cls._public_key_data(key_pub, key_type)
+            return self._public_key_data(key_pub, key_type)
 
-    @classmethod
-    async def key_labels(cls) -> Dict[str, str]:
+    async def key_labels(self) -> Dict[str, str]:
         """Return a dict of key labels as keys and key type as values in the PKCS11 device.
 
         Returns:
         Dict[str, str]
         """
 
-        if cls.base_url is not None:
-            async with aiohttp.ClientSession(headers=cls.http_headers) as session:
+        if self.base_url is not None:
+            async with aiohttp.ClientSession(headers=self.http_headers) as session:
                 async with session.post(
-                    url=f"{cls.base_url}/key_labels", json=cls.http_data, headers=cls.http_headers, timeout=10
+                    url=f"{self.base_url}/key_labels", json=self.http_data, headers=self.http_headers, timeout=10
                 ) as response:
                     response.raise_for_status()
                     json_body = await response.json()
                     ret = json_body["key_labels"]  # handle errors
 
                     if isinstance(ret, dict):  # handle only [str, str]
                         return ret
                     raise ValueError("Problem with key labels")
 
-        async with async_lock(cls.lock):
+        async with async_lock(self.lock):
             # Ensure we get a healthy pkcs11 session
-            await cls.healthy_session()
+            await self.healthy_session()
 
             key_labels: Dict[str, str] = {}
 
             # For rsa
-            for obj in cls.session.get_objects(
-                {
-                    Attribute.CLASS: ObjectClass.PUBLIC_KEY,
-                    Attribute.KEY_TYPE: key_type_values["rsa_2048"],
-                }
+            for obj in self.session.get_objects(
+                {Attribute.CLASS: ObjectClass.PUBLIC_KEY, Attribute.KEY_TYPE: KEY_TYPE_VALUES[KEYTYPES.RSA2048]}
             ):
                 if obj.key_length == 2048:
                     key_labels[obj.label] = "rsa_2048"
                 elif obj.key_length == 4096:
                     key_labels[obj.label] = "rsa_4096"
                 else:
                     key_labels[obj.label] = "rsa_512"
 
             # For ed25519
-            for obj in cls.session.get_objects(
+            for obj in self.session.get_objects(
                 {
                     Attribute.CLASS: ObjectClass.PUBLIC_KEY,
-                    Attribute.KEY_TYPE: key_type_values["ed25519"],
+                    Attribute.KEY_TYPE: KEY_TYPE_VALUES[KEYTYPES.ED25519],
                     Attribute.EC_PARAMS: encode_named_curve_parameters("1.3.101.112"),
                 }
             ):
                 key_labels[obj.label] = "ed25519"
 
             # For ed448
-            for obj in cls.session.get_objects(
+            for obj in self.session.get_objects(
                 {
                     Attribute.CLASS: ObjectClass.PUBLIC_KEY,
-                    Attribute.KEY_TYPE: key_type_values["ed448"],
+                    Attribute.KEY_TYPE: KEY_TYPE_VALUES[KEYTYPES.ED448],
                     Attribute.EC_PARAMS: encode_named_curve_parameters("1.3.101.113"),
                 }
             ):
                 key_labels[obj.label] = "ed448"
 
             # for secp256r1, secp384r1, secp521r1
-            for curve in ["secp256r1", "secp384r1", "secp521r1"]:
-                for obj in cls.session.get_objects(
+            for curve in [KEYTYPES.SECP256r1, KEYTYPES.SECP384r1, KEYTYPES.SECP521r1]:
+                for obj in self.session.get_objects(
                     {
                         Attribute.CLASS: ObjectClass.PUBLIC_KEY,
-                        Attribute.KEY_TYPE: key_type_values[curve],
-                        Attribute.EC_PARAMS: encode_named_curve_parameters(curve),
+                        Attribute.KEY_TYPE: KEY_TYPE_VALUES[curve],
+                        Attribute.EC_PARAMS: encode_named_curve_parameters(curve.value),
                     }
                 ):
-                    key_labels[obj.label] = curve
+                    key_labels[obj.label] = curve.value
 
             return key_labels
 
-    @classmethod
     async def _sign(  # pylint: disable-msg=too-many-arguments
-        cls,
-        key_label: str,
-        data: bytes,
-        verify_signature: Optional[bool],
-        mechanism: Mechanism,
-        key_type: str,
+        self, key_label: str, data: bytes, verify_signature: Optional[bool], mechanism: Mechanism, key_type: KEYTYPES
     ) -> bytes:
-        async with async_lock(cls.lock):
+
+        async with async_lock(self.lock):
             # Ensure we get a healthy pkcs11 session
-            await cls.healthy_session()
+            await self.healthy_session()
 
             # Get private key to sign the data with
-            key_priv = cls.session.get_key(
-                key_type=key_type_values[key_type],
+            key_priv = self.session.get_key(
+                key_type=KEY_TYPE_VALUES[key_type],
                 object_class=ObjectClass.PRIVATE_KEY,
                 label=key_label,
             )
             if verify_signature:
-                key_pub = cls._get_pub_key(key_label, key_type)
+                key_pub = self._get_pub_key(key_label, key_type)
 
             # Sign the data
             signature = key_priv.sign(data, mechanism=mechanism)
 
             if not isinstance(signature, bytes):
                 raise SignatureInvalid
 
             if verify_signature:
                 if not key_pub.verify(data, signature, mechanism=mechanism):
                     raise SignatureInvalid
 
             return signature
 
-    @classmethod
     async def sign(
-        cls,
+        self,
         key_label: str,
         data: bytes,
         verify_signature: Optional[bool] = None,
-        key_type: Optional[str] = None,
+        key_type: Union[str, KEYTYPES] = DEFAULT_KEY_TYPE,
     ) -> bytes:
         """Sign the data: bytes using the private key
         with the label in the PKCS11 device.
 
         Returns the signed data: bytes for the x509 extension and
         'Authority Key Identifier' valid for this keypair.
 
         Parameters:
         key_label (str): Keypair label.
         data (bytes): Bytes to be signed.
         verify_signature (Union[bool, None] = None):
         If we should verify the signature. PKCS11 operations can be expensive, default None (False)
-        key_type (Union[str, None] = None): Key type.
+        key_type Union[str, KEYTYPES]: Key type, defaults to "ed25519".
 
         Returns:
         bytes
         """
 
-        if key_type is None:
-            key_type = "ed25519"
+        if isinstance(key_type, str):
+            key_type = get_keytypes_enum(key_type)
 
-        if key_type not in key_types:
-            raise ValueError(f"key_type must be in {key_types}")
-
-        if cls.base_url is not None:
+        if self.base_url is not None:
             http_request_data: Dict[str, Union[str, bool]] = {}
 
-            if cls.http_data is not None:
-                http_request_data.update(cls.http_data)
+            if self.http_data is not None:
+                http_request_data.update(self.http_data)
 
             http_request_data["data_b64"] = base64.b64encode(data).decode("utf-8")
             http_request_data["key_label"] = key_label
-            http_request_data["key_type"] = key_type
+            http_request_data["key_type"] = key_type.value
 
             if verify_signature is None or not verify_signature:
                 http_request_data["verify_signature"] = False
             else:
                 http_request_data["verify_signature"] = True
 
-            async with aiohttp.ClientSession(headers=cls.http_headers) as session:
+            async with aiohttp.ClientSession(headers=self.http_headers) as session:
                 async with session.post(
-                    url=f"{cls.base_url}/sign", json=http_request_data, headers=cls.http_headers, timeout=10
+                    url=f"{self.base_url}/sign", json=http_request_data, headers=self.http_headers, timeout=10
                 ) as response:
                     response.raise_for_status()
                     json_body = await response.json()
                     ret = json_body["signature_b64"]  # handle errors
 
                     if isinstance(ret, str):
                         return base64.b64decode(ret)
                     raise ValueError("Problem with signature")
 
-        if key_type in ["ed25519", "ed448"]:
+        if key_type in [KEYTYPES.ED25519, KEYTYPES.ED448]:
             mech = Mechanism.EDDSA
 
-        elif key_type in ["secp256r1", "secp384r1", "secp521r1"]:
+        elif key_type in [KEYTYPES.SECP256r1, KEYTYPES.SECP384r1, KEYTYPES.SECP521r1]:
             mech = Mechanism.ECDSA
 
             # Set hash alg
-            if key_type == "secp256r1":
+            if key_type == KEYTYPES.SECP256r1:
                 hash_obj = sha256()
-            elif key_type == "secp384r1":
+            elif key_type == KEYTYPES.SECP384r1:
                 hash_obj = sha384()
             else:
                 hash_obj = sha512()
 
             hash_obj.update(data)
             data = hash_obj.digest()
 
         else:
-            if key_type == "rsa_2048":
+            if key_type == KEYTYPES.RSA2048:
                 mech = Mechanism.SHA256_RSA_PKCS
             else:
                 mech = Mechanism.SHA512_RSA_PKCS
 
-        signature = await cls._sign(key_label, data, verify_signature, mech, key_type)
+        signature = await self._sign(key_label, data, verify_signature, mech, key_type)
 
         # PKCS11 specific stuff for EC curves, sig is in R&S format, convert it to openssl format
-        if key_type in ["secp256r1", "secp384r1", "secp521r1"]:
-            signature = convert_rs_ec_signature(signature, key_type)
+        if key_type in [KEYTYPES.SECP256r1, KEYTYPES.SECP384r1, KEYTYPES.SECP521r1]:
+            signature = convert_rs_ec_signature(signature, key_type.value)
 
         return signature
 
-    @classmethod
     async def verify(  # pylint: disable-msg=too-many-arguments
-        cls,
-        key_label: str,
-        data: bytes,
-        signature: bytes,
-        key_type: Optional[str] = None,
+        self, key_label: str, data: bytes, signature: bytes, key_type: Union[str, KEYTYPES] = DEFAULT_KEY_TYPE
     ) -> bool:
         """Verify a signature with its data using the private key
         with the label in the PKCS11 device.
 
         Returns True if the signature is valid.
 
         Parameters:
         key_label (str): Keypair label.
         data (bytes): Bytes to be signed.
         signature (bytes): The signature.
-        key_type (Union[str, None] = None): Key type.
+        key_type str: Key type, defaults to "ed25519".
 
         Returns:
         bool
         """
 
-        if key_type is None:
-            key_type = "ed25519"
+        if isinstance(key_type, str):
+            key_type = get_keytypes_enum(key_type)
 
-        if key_type not in key_types:
-            raise ValueError(f"key_type must be in {key_types}")
-
-        if cls.base_url is not None:
+        if self.base_url is not None:
             http_request_data: Dict[str, str] = {}
 
-            if cls.http_data is not None:
-                http_request_data.update(cls.http_data)
+            if self.http_data is not None:
+                http_request_data.update(self.http_data)
 
             http_request_data["data_b64"] = base64.b64encode(data).decode("utf-8")
             http_request_data["signature_b64"] = base64.b64encode(signature).decode("utf-8")
             http_request_data["key_label"] = key_label
-            http_request_data["key_type"] = key_type
+            http_request_data["key_type"] = key_type.value
 
-            async with aiohttp.ClientSession(headers=cls.http_headers) as session:
+            async with aiohttp.ClientSession(headers=self.http_headers) as session:
                 async with session.post(
-                    url=f"{cls.base_url}/verify", json=http_request_data, headers=cls.http_headers, timeout=10
+                    url=f"{self.base_url}/verify", json=http_request_data, headers=self.http_headers, timeout=10
                 ) as response:
                     response.raise_for_status()
                     json_body = await response.json()
                     ret = json_body["verified"]  # handle errors
 
                     if isinstance(ret, bool):
                         return ret
                     raise ValueError("Problem with verify")
 
-        async with async_lock(cls.lock):
+        async with async_lock(self.lock):
             # Ensure we get a healthy pkcs11 session
-            await cls.healthy_session()
+            await self.healthy_session()
 
             # Get public key to sign the data with
-            key_pub = cls._get_pub_key(key_label, key_type)
+            key_pub = self._get_pub_key(key_label, key_type)
 
-            if key_type in ["ed25519", "ed448"]:
+            if key_type in [KEYTYPES.ED25519, KEYTYPES.ED448]:
                 mech = Mechanism.EDDSA
 
-            elif key_type in ["secp256r1", "secp384r1", "secp521r1"]:
+            elif key_type in [KEYTYPES.SECP256r1, KEYTYPES.SECP384r1, KEYTYPES.SECP521r1]:
                 mech = Mechanism.ECDSA
 
                 # Set hash alg
-                if key_type == "secp256r1":
+                if key_type == KEYTYPES.SECP256r1:
                     hash_obj = sha256()
-                elif key_type == "secp384r1":
+                elif key_type == KEYTYPES.SECP384r1:
                     hash_obj = sha384()
                 else:
                     hash_obj = sha512()
 
                 hash_obj.update(data)
                 data = hash_obj.digest()
 
                 try:
-                    signature = convert_asn1_ec_signature(signature, key_type)
+                    signature = convert_asn1_ec_signature(signature, key_type.value)
                 except (IndexError, ValueError):
                     # Signature was not in ASN1 format, signature verification will probably fail.
                     pass
 
             else:  # rsa
-                if key_type == "rsa_2048":
+                if key_type == KEYTYPES.RSA2048:
                     mech = Mechanism.SHA256_RSA_PKCS
                 else:
                     mech = Mechanism.SHA512_RSA_PKCS
 
             if key_pub.verify(data, signature, mechanism=mech):
                 return True
             return False
 
-    @classmethod
-    async def delete_keypair(cls, key_label: str, key_type: Optional[str] = None) -> None:
+    async def delete_keypair(self, key_label: str, key_type: Union[str, KEYTYPES] = DEFAULT_KEY_TYPE) -> None:
         """Delete the keypair from the PKCS11 device.
 
         Parameters:
         key_label (str): Keypair label.
-        key_type (Union[str, None] = None): Key type.
+        key_type (Union[str, KEYTYPES] = None): Key type.
 
         Returns:
         None
         """
 
-        if key_type is None:
-            key_type = "ed25519"
-
-        if key_type not in key_types:
-            raise ValueError(f"key_type must be in {key_types}")
+        if isinstance(key_type, str):
+            key_type = get_keytypes_enum(key_type)
 
-        if cls.base_url is not None:
+        if self.base_url is not None:
             http_request_data: Dict[str, str] = {}
 
-            if cls.http_data is not None:
-                http_request_data.update(cls.http_data)
+            if self.http_data is not None:
+                http_request_data.update(self.http_data)
 
-            http_request_data["key_type"] = key_type
+            http_request_data["key_type"] = key_type.value
             http_request_data["key_label"] = key_label
 
-            async with aiohttp.ClientSession(headers=cls.http_headers) as session:
+            async with aiohttp.ClientSession(headers=self.http_headers) as session:
                 async with session.post(
-                    url=f"{cls.base_url}/delete_keypair", json=http_request_data, headers=cls.http_headers, timeout=10
+                    url=f"{self.base_url}/delete_keypair", json=http_request_data, headers=self.http_headers, timeout=10
                 ) as response:
                     response.raise_for_status()
                     json_body = await response.json()
                     return
                     # ret = json_body["verified"]  # handle errors
 
-        async with async_lock(cls.lock):
+        async with async_lock(self.lock):
             # Ensure we get a healthy pkcs11 session
-            await cls.healthy_session()
+            await self.healthy_session()
 
             try:
-                cls.session.get_key(
-                    key_type=key_type_values[key_type],
+                self.session.get_key(
+                    key_type=KEY_TYPE_VALUES[key_type],
                     object_class=ObjectClass.PUBLIC_KEY,
                     label=key_label,
                 ).destroy()
             finally:
-                cls.session.get_key(
-                    key_type=key_type_values[key_type],
+                self.session.get_key(
+                    key_type=KEY_TYPE_VALUES[key_type],
                     object_class=ObjectClass.PRIVATE_KEY,
                     label=key_label,
                 ).destroy()
 
-    @classmethod
-    async def public_key_data(cls, key_label: str, key_type: Optional[str] = None) -> Tuple[str, bytes]:
+    async def public_key_data(self, key_label: str, key_type: KEYTYPES = DEFAULT_KEY_TYPE) -> Tuple[str, bytes]:
         """Returns the public key in PEM form
         and 'Key Identifier' valid for this keypair.
 
         Parameters:
         key_label (str): Keypair label.
-        key_type (Union[str, None] = None): Key type.
+        key_type (Union[str, KEYTYPES]: Key type, default value is KEYTYPES.ED25519.
 
         Returns:
         Tuple[str, bytes]
         """
 
-        if key_type is None:
-            key_type = "ed25519"
-
-        if key_type not in key_types:
-            raise ValueError(f"key_type must be in {key_types}")
+        if isinstance(key_type, str):
+            key_type = get_keytypes_enum(key_type)
 
-        if cls.base_url is not None:
+        if self.base_url is not None:
             http_request_data: Dict[str, str] = {}
 
-            if cls.http_data is not None:
-                http_request_data.update(cls.http_data)
+            if self.http_data is not None:
+                http_request_data.update(self.http_data)
 
             http_request_data["key_label"] = key_label
-            http_request_data["key_type"] = key_type
+            http_request_data["key_type"] = key_type.value
 
-            async with aiohttp.ClientSession(headers=cls.http_headers) as session:
+            async with aiohttp.ClientSession(headers=self.http_headers) as session:
                 async with session.post(
-                    url=f"{cls.base_url}/public_key_data", json=http_request_data, headers=cls.http_headers, timeout=10
+                    url=f"{self.base_url}/public_key_data",
+                    json=http_request_data,
+                    headers=self.http_headers,
+                    timeout=10,
                 ) as response:
                     response.raise_for_status()
                     json_body = await response.json()
 
                     if json_body["status"] == "error" and json_body["detail"] == "NoSuchKey":
                         raise NoSuchKey()
 
                     spi = json_body["subjectPublicKeyInfo"]  # handle errors
                     ski = json_body["subjectKeyIdentifier_b64"]
 
                     if isinstance(spi, str) and isinstance(ski, str):
                         return spi, base64.b64decode(ski)
                     raise ValueError("Problem with create keypair")
 
-        async with async_lock(cls.lock):
+        async with async_lock(self.lock):
             # Ensure we get a healthy pkcs11 session
-            await cls.healthy_session()
+            await self.healthy_session()
 
-            key_pub = cls._get_pub_key(key_label, key_type)
-            return cls._public_key_data(key_pub, key_type)
+            key_pub = self._get_pub_key(key_label, key_type)
+            return self._public_key_data(key_pub, key_type)
```

### Comparing `python_x509_pkcs11-0.8.4/tests/test_ca.py` & `python_x509_pkcs11-0.9.0/tests/test_ca.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """
 Test to create a new root CA
 """
+
 import asyncio
 import datetime
 import os
 import subprocess
 import unittest
 from typing import Dict
 
 from asn1crypto import csr as asn1_csr
 from asn1crypto import pem as asn1_pem
 from asn1crypto import x509 as asn1_x509
 from asn1crypto.core import GeneralizedTime
 
 from src.python_x509_pkcs11.ca import create
-from src.python_x509_pkcs11.lib import key_types
+from src.python_x509_pkcs11.lib import KEYTYPES
 from src.python_x509_pkcs11.pkcs11_handle import PKCS11Session
 
 # Replace the above with this should you use this code
 # from python_x509_pkcs11.ca import create
 
 name_dict = {
     "country_name": "SE",
@@ -74,16 +75,16 @@
         self.assertTrue(aki == ski)
 
     def test_create_ca(self) -> None:
         """
         Create and self sign a CSR with the key_label in the pkcs11 device.
         """
 
-        for key_type in key_types:
-            new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        for key_type in KEYTYPES:
+            new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
             # Test non default key size
             _, root_cert_pem = asyncio.run(create(new_key_label[:-1], name_dict, key_type=key_type))
             data = root_cert_pem.encode("utf-8")
             if asn1_pem.detect(data):
                 _, _, data = asn1_pem.unarmor(data)
 
             test_cert = asn1_x509.Certificate.load(data)
@@ -119,24 +120,24 @@
             self.assertTrue(isinstance(test_cert, asn1_x509.Certificate))
             self.assertTrue(isinstance(test_cert["tbs_certificate"]["extensions"], asn1_x509.Extensions))
             # CSR exts (key usage and basic constraints
             # + authority and subject key identifier = 4
             self.assertTrue(len(test_cert["tbs_certificate"]["extensions"]) == 4)
 
             # Delete the test keys
-            asyncio.run(PKCS11Session.delete_keypair(new_key_label[:-1], key_type=key_type))
-            asyncio.run(PKCS11Session.delete_keypair(new_key_label[:-2]))
+            asyncio.run(PKCS11Session().delete_keypair(new_key_label[:-1], key_type=key_type))
+            asyncio.run(PKCS11Session().delete_keypair(new_key_label[:-2]))
 
     def test_create_ca_not_before_not_after(self) -> None:
         """
         Create and selfsign a CSR with the key_label in the pkcs11 device
         with non default not_before and not_after.
         """
 
-        new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
 
         # Test not_before parameter
         not_before = datetime.datetime(2022, 1, 1, tzinfo=datetime.timezone.utc)
         _, root_cert_pem = asyncio.run(
             create(
                 new_key_label[:-1],
                 name_dict,
@@ -163,23 +164,23 @@
         if asn1_pem.detect(data):
             _, _, data = asn1_pem.unarmor(data)
         test_c = asn1_x509.Certificate.load(data)
         self.assertTrue(isinstance(test_c, asn1_x509.Certificate))
         self.assertTrue(test_c["tbs_certificate"]["validity"]["not_after"].native == not_after)
 
         # Delete the test keys
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label[:-1]))
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label[:-2]))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label[:-1]))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label[:-2]))
 
     def test_create_ca_with_extensions(self) -> None:
         """
         Create and selfsign a CSR with the key_label in the pkcs11 device.
         """
 
-        new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
         exts = asn1_csr.Extensions()
 
         pkup = asn1_x509.PrivateKeyUsagePeriod()
         pkup["not_before"] = GeneralizedTime(
             datetime.datetime.now(datetime.timezone.utc) - datetime.timedelta(minutes=2)
         )
         pkup["not_after"] = GeneralizedTime(
@@ -216,27 +217,27 @@
 
         cert_exts = test_cert["tbs_certificate"]["extensions"]
         # test pkup ext + CSR exts (key usage and basic constraints
         # + authority and subject key identifier = 5
         self.assertTrue(len(cert_exts) == 5)
 
         # Delete the test key
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label))
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label[:-1]))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label[:-1]))
 
     def test_create_intermediate_ca(self) -> None:
         """
         Create an intermediate CA in the pkcs11 device.
         """
 
-        for key_type in key_types:
-            new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        for key_type in KEYTYPES:
+            new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
             _, root_ca_pem = asyncio.run(create(new_key_label, signer_name_dict, key_type=key_type))
 
-            new_key_label2 = hex(int.from_bytes(os.urandom(20), "big") >> 1)
+            new_key_label2 = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
             _, im_cert_pem = asyncio.run(
                 create(
                     new_key_label2,
                     signed_name_dict,
                     signer_subject_name=signer_name_dict,
                     signer_key_label=new_key_label,
                     key_type=key_type,
@@ -292,25 +293,25 @@
                     ski = extension["extn_value"].native
             for _, extension in enumerate(tbs["extensions"]):
                 if extension["extn_id"].dotted == "2.5.29.35":
                     aki = extension["extn_value"].native["key_identifier"]
             self.assertTrue(ski != aki)
 
             # Delete the test keys
-            asyncio.run(PKCS11Session.delete_keypair(new_key_label, key_type=key_type))
-            asyncio.run(PKCS11Session.delete_keypair(new_key_label2, key_type=key_type))
+            asyncio.run(PKCS11Session().delete_keypair(new_key_label, key_type=key_type))
+            asyncio.run(PKCS11Session().delete_keypair(new_key_label2, key_type=key_type))
 
     def test_create_intermediate_diff_key_type_ca(self) -> None:
         """
         Create an intermediate CA with different key label in the pkcs11 device.
         """
-        new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
         _, root_ca_pem = asyncio.run(create(new_key_label, signer_name_dict, key_type="ed25519"))
 
-        new_key_label2 = hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        new_key_label2 = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
         _, im_cert_pem = asyncio.run(
             create(
                 new_key_label2,
                 signed_name_dict,
                 signer_subject_name=signer_name_dict,
                 signer_key_label=new_key_label,
                 key_type="secp256r1",
@@ -351,9 +352,9 @@
         # Check subject name and issuer name, should not be equal since this is an intermediate CA
         self.assertTrue(
             im_cert_pem_asn1["tbs_certificate"]["subject"].native["common_name"]
             != im_cert_pem_asn1["tbs_certificate"]["issuer"].native["common_name"]
         )
 
         # Delete the test keys
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label, key_type="ed25519"))
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label2, key_type="secp256r1"))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label, key_type="ed25519"))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label2, key_type="secp256r1"))
```

### Comparing `python_x509_pkcs11-0.8.4/tests/test_crl.py` & `python_x509_pkcs11-0.9.0/tests/test_crl.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Test to create and sign a crl
 """
+
 import asyncio
 import datetime
 import os
 import unittest
 
 from asn1crypto import crl as asn1_crl
 from asn1crypto import pem as asn1_pem
@@ -54,16 +55,16 @@
     """
 
     def test_create_new_crl(self) -> None:
         """
         Create and sign a CRL with the key_label in the pkcs11 device.
         """
 
-        new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
-        asyncio.run(PKCS11Session.create_keypair(new_key_label))
+        new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        asyncio.run(PKCS11Session().create_keypair(new_key_label))
 
         crl_pem = asyncio.run(crl.create(new_key_label, subject_name))
 
         data = crl_pem.encode("utf-8")
         if asn1_pem.detect(data):
             _, _, data = asn1_pem.unarmor(data)
         test_crl = asn1_crl.CertificateList.load(data)
@@ -85,24 +86,24 @@
         tbs = test_crl["tbs_cert_list"]
         for _, extension in enumerate(tbs["crl_extensions"]):
             if extension["extn_id"].dotted == "2.5.29.20":
                 self.assertTrue(extension["extn_value"].native == 2)
         self.assertTrue(len(tbs["revoked_certificates"]) == 1)
 
         # Delete the test key
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label))
 
     def test_add_serial_crl(self) -> None:
         """
         Create and sign a CRL with the key_label in the pkcs11 device.
         """
 
         # Revoke first
-        new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
-        asyncio.run(PKCS11Session.create_keypair(new_key_label))
+        new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        asyncio.run(PKCS11Session().create_keypair(new_key_label))
         crl_pem1 = asyncio.run(crl.create(new_key_label, subject_name, serial_number=2342342342343456, reason=3))
         data = crl_pem1.encode("utf-8")
         if asn1_pem.detect(data):
             _, _, data = asn1_pem.unarmor(data)
         test_crl = asn1_crl.CertificateList.load(data)
         self.assertTrue(isinstance(test_crl, asn1_crl.CertificateList))
         self.assertTrue(len(test_crl["tbs_cert_list"]["revoked_certificates"]) == 1)
@@ -138,38 +139,38 @@
         if asn1_pem.detect(data):
             _, _, data = asn1_pem.unarmor(data)
         test_crl = asn1_crl.CertificateList.load(data)
         self.assertTrue(isinstance(test_crl, asn1_crl.CertificateList))
         self.assertTrue(len(test_crl["tbs_cert_list"]["revoked_certificates"]) == 3)
 
         # Delete the test key
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label))
 
     def test_invalid_reason(self) -> None:
         """
         Try to create and sign a CRL with invalid reason
         """
 
         # Revoke first
-        new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
-        asyncio.run(PKCS11Session.create_keypair(new_key_label))
+        new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        asyncio.run(PKCS11Session().create_keypair(new_key_label))
         with self.assertRaises(ValueError):
             asyncio.run(crl.create(new_key_label, subject_name, serial_number=2342342342343456, reason=33))
 
         # Delete the test key
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label))
 
     def test_aki(self) -> None:
         """
         Create and sign a CRL with AKI.
         """
 
-        new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
-        asyncio.run(PKCS11Session.create_keypair(new_key_label))
-        _, identifier = asyncio.run(PKCS11Session.public_key_data(new_key_label))
+        new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        asyncio.run(PKCS11Session().create_keypair(new_key_label))
+        _, identifier = asyncio.run(PKCS11Session().public_key_data(new_key_label))
         crl_pem1 = asyncio.run(crl.create(new_key_label, subject_name))
         data = crl_pem1.encode("utf-8")
         if asn1_pem.detect(data):
             _, _, data = asn1_pem.unarmor(data)
         test_crl = asn1_crl.CertificateList.load(data)
         self.assertTrue(isinstance(test_crl, asn1_crl.CertificateList))
 
@@ -180,26 +181,26 @@
         for _, extension in enumerate(tbs["crl_extensions"]):
             if extension["extn_id"].dotted == "2.5.29.35":
                 self.assertTrue(extension["extn_value"].native["key_identifier"] == identifier)
                 found = True
         self.assertTrue(found)
 
         # Delete the test key
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label))
 
     def test_next_update_this_update(self) -> None:
         """
         Create and sign a CRL with next_update and/or this_update.
         """
 
         # Both
-        new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
         next_update = datetime.datetime(2022, 1, 1, tzinfo=datetime.timezone.utc)
         this_update = datetime.datetime(2022, 1, 3, tzinfo=datetime.timezone.utc)
-        asyncio.run(PKCS11Session.create_keypair(new_key_label))
+        asyncio.run(PKCS11Session().create_keypair(new_key_label))
         crl_pem = asyncio.run(crl.create(new_key_label, subject_name, next_update=next_update, this_update=this_update))
         data = crl_pem.encode("utf-8")
         if asn1_pem.detect(data):
             _, _, data = asn1_pem.unarmor(data)
         test_crl = asn1_crl.CertificateList.load(data)
         tbs = test_crl["tbs_cert_list"]
         self.assertTrue(tbs["next_update"].native == next_update)
@@ -225,8 +226,8 @@
         test_crl = asn1_crl.CertificateList.load(data)
         tbs = test_crl["tbs_cert_list"]
         self.assertTrue(tbs["next_update"].native != next_update)
         self.assertTrue(tbs["this_update"].native == this_update)
         self.assertTrue(tbs["next_update"].native != tbs["this_update"].native)
 
         # Delete the test key
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label))
```

### Comparing `python_x509_pkcs11-0.8.4/tests/test_crypto.py` & `python_x509_pkcs11-0.9.0/tests/test_crypto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Test out crypto module
 """
+
 import unittest
 
 from src.python_x509_pkcs11.crypto import (
     ASN1_INIT,
     ASN1_INTEGER_CODE,
     ASN1_SECP521R1_CODE,
     convert_asn1_ec_signature,
```

### Comparing `python_x509_pkcs11-0.8.4/tests/test_csr.py` & `python_x509_pkcs11-0.9.0/tests/test_csr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Test to sign a csr
 """
+
 import asyncio
 import datetime
 import os
 import unittest
 
 from asn1crypto import csr as asn1_csr
 from asn1crypto import pem as asn1_pem
@@ -76,17 +77,17 @@
 ROBkrutn/L4cP1y2ZTSkcKScezPeMcYhK3A9ktpXxVVSwjFOvCJT1Lz+JN4Vn3kG
 23TCqfTOxgB+ecHKPyKA3112WdXu5B0yRDHrecumxEJDtn3H823xn1WpxzCvqvWX
 IgukK0VlN7pUPKMtAx1Y+sY8z4bwgOmZRQVvYaRbsMJHyjBl/I4XU+W0nOyq6nAW
 eHqaFEFZApnEybHb7JgdpW5TsnvPN1O5YC6bgbRTgLmwGe+pJ5cEtTwrSvWJra8G
 grASjklC2MWbAnXculQuvhPg5F54CK9WldMvd7oYAmbdGIWiffiL
 -----END CERTIFICATE REQUEST-----"""
 
-        new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
 
-        asyncio.run(PKCS11Session.create_keypair(new_key_label))
+        asyncio.run(PKCS11Session().create_keypair(new_key_label))
         cert_pem = asyncio.run(csr.sign_csr(new_key_label, issuer_name, csr_no_exts))
 
         data = cert_pem.encode("utf-8")
         if asn1_pem.detect(data):
             _, _, data = asn1_pem.unarmor(data)
 
         test_cert = asn1_x509.Certificate.load(data)
@@ -113,23 +114,23 @@
         if asn1_pem.detect(data):
             _, _, data = asn1_pem.unarmor(data)
         test_cert = asn1_x509.Certificate.load(data)
         self.assertTrue(isinstance(test_cert, asn1_x509.Certificate))
         self.assertTrue(test_cert["tbs_certificate"]["validity"]["not_after"].native == not_after)
 
         # Delete the test key
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label))
 
     def test_sign_csr_keep_extensions(self) -> None:
         """
         Sign a CSR with the key with the key_label in the pkcs11 device.
         """
 
-        new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
-        asyncio.run(PKCS11Session.create_keypair(new_key_label))
+        new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        asyncio.run(PKCS11Session().create_keypair(new_key_label))
         cert_pem = asyncio.run(csr.sign_csr(new_key_label, issuer_name, CSR_PEM))
 
         data = cert_pem.encode("utf-8")
         if asn1_pem.detect(data):
             _, _, data = asn1_pem.unarmor(data)
 
         test_cert = asn1_x509.Certificate.load(data)
@@ -142,23 +143,23 @@
         # Assert its value is a string
         self.assertTrue(isinstance(exts[0]["extn_value"].native[0], str))
 
         # Assert its correct value
         self.assertTrue(exts[0]["extn_value"].native[0] == "foo.example.org")
 
         # Delete the test key
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label))
 
     def test_sign_csr_no_keep_extensions(self) -> None:
         """
         Sign a CSR with the key with the key_label in the pkcs11 device.
         """
 
-        new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
-        asyncio.run(PKCS11Session.create_keypair(new_key_label))
+        new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        asyncio.run(PKCS11Session().create_keypair(new_key_label))
         cert_pem = asyncio.run(csr.sign_csr(new_key_label, issuer_name, CSR_PEM, keep_csr_extensions=False))
 
         data = cert_pem.encode("utf-8")
         if asn1_pem.detect(data):
             _, _, data = asn1_pem.unarmor(data)
 
         test_cert = asn1_x509.Certificate.load(data)
@@ -176,22 +177,22 @@
 
         # Test authority key identifier
         self.assertTrue(isinstance(exts[1]["extn_value"].native["key_identifier"], bytes))
         self.assertTrue(isinstance(exts[1]["extn_id"].native, str))
         self.assertTrue(exts[1]["extn_id"].native == "authority_key_identifier")
 
         # Delete the test key
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label))
 
     def test_sign_csr_new_extensions(self) -> None:
         """
         Sign a CSR with the key with the key_label in the pkcs11 device.
         """
 
-        new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
         exts = asn1_csr.Extensions()
 
         k_u = asn1_x509.KeyUsage(("100001100",))
         ext1 = asn1_x509.Extension()
         ext1["extn_id"] = asn1_x509.ExtensionId("2.5.29.15")
         ext1["critical"] = True
         ext1["extn_value"] = k_u
@@ -202,15 +203,15 @@
 
         ext2 = asn1_x509.Extension()
         ext2["extn_id"] = asn1_x509.ExtensionId("2.5.29.19")
         ext2["critical"] = True
         ext2["extn_value"] = b_c
         exts.append(ext2)
 
-        asyncio.run(PKCS11Session.create_keypair(new_key_label))
+        asyncio.run(PKCS11Session().create_keypair(new_key_label))
         cert_pem = asyncio.run(
             csr.sign_csr(
                 new_key_label,
                 issuer_name,
                 CSR_PEM,
                 keep_csr_extensions=False,
                 extra_extensions=exts,
@@ -237,39 +238,39 @@
         self.assertTrue(isinstance(exts[1]["extn_id"].native, str))
         self.assertTrue(exts[1]["extn_id"].native == "basic_constraints")
 
         self.assertTrue(isinstance(exts[1]["extn_value"].native["ca"], bool))
         self.assertTrue(exts[1]["extn_value"].native["ca"])
 
         # Delete the test key
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label))
 
     def test_sign_csr_duplicate_extensions(self) -> None:
         """
         Sign a CSR with the key with the key_label in the pkcs11 device.
         """
 
-        new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
         exts = asn1_csr.Extensions()
 
         k_u = asn1_x509.KeyUsage(("100001100",))
         ext1 = asn1_x509.Extension()
         ext1["extn_id"] = asn1_x509.ExtensionId("2.5.29.15")
         ext1["critical"] = True
         ext1["extn_value"] = k_u
         exts.append(ext1)
         exts.append(ext1)
 
-        asyncio.run(PKCS11Session.create_keypair(new_key_label))
+        asyncio.run(PKCS11Session().create_keypair(new_key_label))
         with self.assertRaises(DuplicateExtensionException):
             _ = asyncio.run(
                 csr.sign_csr(
                     new_key_label,
                     issuer_name,
                     CSR_PEM,
                     keep_csr_extensions=False,
                     extra_extensions=exts,
                 )
             )
 
         # Delete the test key
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label))
```

### Comparing `python_x509_pkcs11-0.8.4/tests/test_ocsp.py` & `python_x509_pkcs11-0.9.0/tests/test_ocsp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """
 Test our OCSP
 """
+
 import asyncio
 import datetime
 import os
 import unittest
 from secrets import token_bytes
 from typing import List
 
@@ -207,16 +208,16 @@
         self.assertTrue(test_ocsp["tbs_request"]["request_extensions"][0]["extn_value"].native == nonce_val)
 
     def test_signed_ocsp_request(self) -> None:
         """
         Create a signed_ocsp request.
         """
 
-        new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
-        asyncio.run(PKCS11Session.create_keypair(new_key_label))
+        new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        asyncio.run(PKCS11Session().create_keypair(new_key_label))
         i_name_h, i_key_h, serial, _ = certificate_ocsp_data(TEST_CERT)
         g_n = asn1_x509.GeneralName(name="directory_name", value=(asn1_ocsp.Name().build(requestor_name_dict)))
 
         # Test signed but no requestor name
         with self.assertRaises(ValueError):
             _ = asyncio.run(request([(i_name_h, i_key_h, serial)], key_label=new_key_label))
 
@@ -241,23 +242,23 @@
             )
         )
         test_ocsp = asn1_ocsp.OCSPRequest.load(data)
         self.assertTrue(isinstance(test_ocsp, asn1_ocsp.OCSPRequest))
         self.assertTrue(len(test_ocsp["optional_signature"]["certs"]) == 2)
 
         # Delete the test key
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label))
 
     def test_ocsp_response(self) -> None:
         """
         Create an ocsp response.
         """
 
-        new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
-        asyncio.run(PKCS11Session.create_keypair(new_key_label))
+        new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        asyncio.run(PKCS11Session().create_keypair(new_key_label))
 
         i_name_h, i_key_h, serial, _ = certificate_ocsp_data(TEST_CERT)
         data = asyncio.run(request([(i_name_h, i_key_h, serial)]))
         test_request = asn1_ocsp.OCSPRequest.load(data)
         self.assertTrue(isinstance(test_request, asn1_ocsp.OCSPRequest))
         data = asyncio.run(response(new_key_label, name_dict, _good_response(test_request), 0))
         test_response = asn1_ocsp.OCSPResponse.load(data)
@@ -283,23 +284,23 @@
         data = asyncio.run(response(new_key_label, name_dict, _good_response(test_request), 0, produced_at=produced_at))
         test_response = asn1_ocsp.OCSPResponse.load(data)
         self.assertTrue(
             test_response["response_bytes"]["response"].native["tbs_response_data"]["produced_at"] == produced_at
         )
 
         # Delete the test key
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label))
 
     def test_ocsp_response_cert_status(self) -> None:
         """
         Create an ocsp responses with different cert status
         """
 
-        new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
-        asyncio.run(PKCS11Session.create_keypair(new_key_label))
+        new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        asyncio.run(PKCS11Session().create_keypair(new_key_label))
 
         i_name_h, i_key_h, serial, _ = certificate_ocsp_data(TEST_CERT)
 
         # Revoked
         data = asyncio.run(request([(i_name_h, i_key_h, serial)]))
         test_request = asn1_ocsp.OCSPRequest.load(data)
         self.assertTrue(isinstance(test_request, asn1_ocsp.OCSPRequest))
@@ -344,23 +345,23 @@
         )
         self.assertTrue(
             test_response["response_bytes"]["response"].native["tbs_response_data"]["responses"][2]["cert_status"]
             == "unknown"
         )
 
         # Delete the test key
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label))
 
     def test_ocsp_response_fail(self) -> None:
         """
         Create an unsuccessful ocsp response.
         """
 
-        new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
-        asyncio.run(PKCS11Session.create_keypair(new_key_label))
+        new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        asyncio.run(PKCS11Session().create_keypair(new_key_label))
 
         i_name_h, i_key_h, serial, _ = certificate_ocsp_data(TEST_CERT)
         data = asyncio.run(request([(i_name_h, i_key_h, serial)]))
         test_request = asn1_ocsp.OCSPRequest.load(data)
 
         # Test status codes
         data = asyncio.run(response(new_key_label, name_dict, _good_response(test_request), 1))
@@ -384,23 +385,23 @@
             data = asyncio.run(response(new_key_label, name_dict, _good_response(test_request), 4))
             _ = asn1_ocsp.OCSPResponse.load(data)
         with self.assertRaises(ValueError):
             data = asyncio.run(response(new_key_label, name_dict, _good_response(test_request), 99))
             _ = asn1_ocsp.OCSPResponse.load(data)
 
         # Delete the test key
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label))
 
     def test_ocsp_response_extensions(self) -> None:
         """
         Create an ocsp response with extra extensions.
         """
 
-        new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
-        asyncio.run(PKCS11Session.create_keypair(new_key_label))
+        new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        asyncio.run(PKCS11Session().create_keypair(new_key_label))
 
         i_name_h, i_key_h, serial, _ = certificate_ocsp_data(TEST_CERT)
         data = asyncio.run(request([(i_name_h, i_key_h, serial)]))
         test_request = asn1_ocsp.OCSPRequest.load(data)
 
         # Test too big nonce
         nonce_ext = asn1_ocsp.ResponseDataExtension()
@@ -446,15 +447,15 @@
         )
         self.assertTrue(
             test_response["response_bytes"]["response"].native["tbs_response_data"]["response_extensions"][1]["extn_id"]
             == "extended_revoke"
         )
 
         # Delete the test key
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label))
 
     def test_request_nonce(self) -> None:
         """
         Test request nonce function.
         """
 
         nonce_ext = asn1_ocsp.TBSRequestExtension()
@@ -657,16 +658,16 @@
 C8Nzo/mRk8C0Gcbl4GkDSN/ujrECoapLbxsuKDLhPa6lkmn/N1BWVoohkvwZGcca
 HJfKd3Am/5yYf8w+QQH0LeyZZk9tM+d9XBGrqOFpL0T19zsyKiddbbRXceyftxyc
 5VGw62FbGoNqyVYDR1kX5FSuvOT/29L/5fSLCgn6ow3mH7TX16ZL8vTzDLUqlBtE
 FvdQ0EEx2Pssrry0iD5AieGyK2nKW94UA0gQenvtMS9mxQ==
 -----END CERTIFICATE-----
 """
 
-        new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
-        asyncio.run(PKCS11Session.create_keypair(new_key_label))
+        new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        asyncio.run(PKCS11Session().create_keypair(new_key_label))
 
         i_name_h, i_key_h, serial, _ = certificate_ocsp_data(TEST_CERT)
         data = asyncio.run(request([(i_name_h, i_key_h, serial)]))
         test_request = asn1_ocsp.OCSPRequest.load(data)
         self.assertTrue(isinstance(test_request, asn1_ocsp.OCSPRequest))
         data = asyncio.run(
             response(new_key_label, name_dict, _good_response(test_request), 0, extra_certs=[extra_cert1, extra_cert2])
@@ -693,8 +694,8 @@
             _, _, cert_data = asn1_pem.unarmor(cert_data)
         self.assertTrue(
             test_response["response_bytes"]["response"].native["certs"][1]
             == asn1_ocsp.Certificate.load(cert_data).native
         )
 
         # Delete the test key
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label))
```

### Comparing `python_x509_pkcs11-0.8.4/tests/test_pkcs11_handle.py` & `python_x509_pkcs11-0.9.0/tests/test_pkcs11_handle.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,64 @@
 """
 Test our PKCS11 session handler
 """
+
 import asyncio
 import os
 import unittest
 
 from pkcs11 import Session
 
 # import asn1crypto.x509 as asn1_x509
 from pkcs11.exceptions import MultipleObjectsReturned, NoSuchKey
 
 from src.python_x509_pkcs11.error import PKCS11UnknownErrorException
-from src.python_x509_pkcs11.lib import key_type_values, key_types
+from src.python_x509_pkcs11.lib import KEY_TYPE_VALUES, KEYTYPES
 from src.python_x509_pkcs11.pkcs11_handle import PKCS11Session
 
 # Replace the above with this should you use this code
 # from python_x509_pkcs11.pkcs11_handle import PKCS11Session
 
 
+async def delete_keys():
+    "We delete keys in a loop"
+
+    # No need to delete keys in github actions.
+    session = PKCS11Session()
+    keys = await session.key_labels()
+    for key_label, key_type in keys.items():
+        if key_label == "test_pkcs11_device_do_not_use":
+            continue
+        if key_label.startswith("testpkcs"):
+            await session.delete_keypair(key_label, key_type)
+
+
 class TestPKCS11Handle(unittest.TestCase):
     """
     Test our PKCS11 session handler.
     """
 
+    def tearDown(self):
+        "Cleans up test keys."
+        asyncio.run(delete_keys())
+
     def test_session(self) -> None:
         """Test PKCS11 session"""
 
         with self.assertRaises(PKCS11UnknownErrorException):
-            asyncio.run(PKCS11Session.healthy_session(simulate_pkcs11_timeout=True))
+            asyncio.run(PKCS11Session().healthy_session(simulate_pkcs11_timeout=True))
 
     def test_get_session(self) -> None:
         """Test PKCS11 session"""
 
-        sess = asyncio.run(PKCS11Session.get_session())
+        sess = asyncio.run(PKCS11Session().get_session())
 
         assert isinstance(sess, Session)
         with self.assertRaises(NoSuchKey):
-            sess.get_key(label="test_not_exist", key_type=key_type_values["rsa_2048"])
+            sess.get_key(label="test_not_exist", key_type=KEY_TYPE_VALUES[KEYTYPES.RSA2048])
 
     def test_import_keypair_rsa(self) -> None:
         """Import keypair with key_label in the PKCS11 device.
 
         Generate pub and priv with
         openssl genrsa -out rsaprivkey.pem 2048
         openssl rsa -inform pem -in rsaprivkey.pem -outform der -out PrivateKey.der
@@ -49,42 +67,42 @@
 
         pub = b"0\x82\x01\n\x02\x82\x01\x01\x00\xd9\xb6C,O\xc0\x83\xca\xa5\xcc\xa7<_\xbf$\xdd-YJ0m\xbf\xa8\xf9[\xe7\xcb\x14W6G\n\x13__\xea\xb4Z\xab2\x01\x0f\xa4\xd3\x1c\xbb\xa6\x98\x9d\xcdf\xaa\x07\xcb\xff\xd8\x80\xa9\\\xa1\xf44\x01\xdbY\xa6\xcf\x83\xd2\x83Z\x8a<\xc1\x18\xe5\x8d\xff\xbfzU\x03\x01\x11\xa1\xa1\x98\xcf\xcaVu\xf9\xf3\xa7+ \xe7N9\x07\xfd\xc6\xd0\x7f\xa0\xba&\xef\xb2a\xc6\xa5d\x1c\x93\xe6\xc3\x80\xd1*;\xc8@7\x0fm)\xf93\xe4\x1f\x91\xf4=\xa6\xf8\xed\x9cN\x84\x9b\xf2\xc5\x9f\x9f\x82E\xa5Tm\xb9\xb3:T\xc7_\xb1^[\xf4\x0b\xd8\x0b\xd2\xfb\xe1\x13\x1e,L\xd9\xdc\xed]_#\xca\xa0r\xc2\xc5F \xec\xae\x8d\x08v\x059\x062\xe1\xf7%\x9e\xfd\xfb9\x11(\xa4\x86v\x90\x01\x1c\xbeP\x04\xa3%\x91\x08\xc5\xd5\xc1U\xf6\xd3\x7f\x1f\x9f7`\xce\xc9\xa1\xd9\x8f\\Z\xa8\x1cmz\x19x\xa4'F\xdf\xb2\xb2\x87\xba\xf7\n>]\x9f\xc0K@\xd9\xdb\x02\x03\x01\x00\x01"  # pylint: disable=C0301
         priv = b"0\x82\x04\xa4\x02\x01\x00\x02\x82\x01\x01\x00\xd9\xb6C,O\xc0\x83\xca\xa5\xcc\xa7<_\xbf$\xdd-YJ0m\xbf\xa8\xf9[\xe7\xcb\x14W6G\n\x13__\xea\xb4Z\xab2\x01\x0f\xa4\xd3\x1c\xbb\xa6\x98\x9d\xcdf\xaa\x07\xcb\xff\xd8\x80\xa9\\\xa1\xf44\x01\xdbY\xa6\xcf\x83\xd2\x83Z\x8a<\xc1\x18\xe5\x8d\xff\xbfzU\x03\x01\x11\xa1\xa1\x98\xcf\xcaVu\xf9\xf3\xa7+ \xe7N9\x07\xfd\xc6\xd0\x7f\xa0\xba&\xef\xb2a\xc6\xa5d\x1c\x93\xe6\xc3\x80\xd1*;\xc8@7\x0fm)\xf93\xe4\x1f\x91\xf4=\xa6\xf8\xed\x9cN\x84\x9b\xf2\xc5\x9f\x9f\x82E\xa5Tm\xb9\xb3:T\xc7_\xb1^[\xf4\x0b\xd8\x0b\xd2\xfb\xe1\x13\x1e,L\xd9\xdc\xed]_#\xca\xa0r\xc2\xc5F \xec\xae\x8d\x08v\x059\x062\xe1\xf7%\x9e\xfd\xfb9\x11(\xa4\x86v\x90\x01\x1c\xbeP\x04\xa3%\x91\x08\xc5\xd5\xc1U\xf6\xd3\x7f\x1f\x9f7`\xce\xc9\xa1\xd9\x8f\\Z\xa8\x1cmz\x19x\xa4'F\xdf\xb2\xb2\x87\xba\xf7\n>]\x9f\xc0K@\xd9\xdb\x02\x03\x01\x00\x01\x02\x82\x01\x00a5\x1e=\x14\xc6\xf2\x91s\x023\xd1\xa36\xa7q\x12$\x82\x19\xa9\x87 \x1df\xc9\xd2E\x1c\xc3\xa1h\x80I\xdf{\xdeWu\x84\xf80Q\xf9\xe9$h8P\x8d;\xbf\xc3\x87t\x8e\xe8\xb3\xb6&\xa1\xf0\xee\xbbP\x06I5\xa4\xb2\xfd\xa4'\x88Xcv\xc9\xb0g \xba\x1c\xaa\x10\xaf$\x99\xf2\xd04\x11\x0c\x97\xa1\x8c){%\xbf\xc9\xb2\x11\xbaJ\xbb\x93S\x07$\xdd\x1bO\xdd\xea\xb3\xe8\xab\x05\xb9\x83\xc3\xdf\xd85\xcd\x1a%\xd5\xd9\xc4\x933\x83\t\xd3\xea\xcdb\xcb\xec\x9eGqk\x1c\x8c\x06\x8a\\\xae\xbe\xd3+\x0b\xd0R\xbd:\x8a\xf5\xf4\x0f\x0b\xd4\xfa@P=\xe5\xb2\xa1\xb2\x01\x00\x08\xc7\x11?M\x84-\x1e\xbc\xa9\xbf|\x87\x98\xd7\x0e\xf6\xa9\xa6\xcd\x8c8\xa5F8\xacM\x82\xade[\xa9_\xa7Biv\x9c\x06\xa6\x001\xc3I\x1f\xc4\x9by\xd7\xe0\x9e\xb9\n\xbb\x19\\o\xc5i\xd90r\xd4\x1e(\x05\xdd\xedF\xe9\xaa\xbd\x91\xe5\x08\x8f4-\xb6\xd1Q\x02\x81\x81\x00\xf7\x076\xd8i\x87\x12\xf1\xd0$\x07\x1f\xab\xb7^\x0e\xa5\xfb\x83\x98\x00\x0b\\\x1d\xe8s\x15r\x96/\x0e\x0ezB\xc8\xf6\xf3Zmj?\xa0\xc1\x11r\xaf3\x11a\xcd\xa3\xfc\xa0\x03\x04E\x05\x99\x9a\xd9\xff\x8e+\xdcfM\xa8\xe8&\x84\x85\xc5\x11O\x9d4\x1f\xc3\x1f\xef\xed\x13BW\xaa\x93\xc3\x08(v]\xbc\x93V\xb6s\xce\xb1\xa8\xe2\x94\xa5'\xf3\x7f\x90,G[\xfeI\x16\xbe\xb0\xf8J\xca9n\xb5\xfc\x8a\xe2[\xc5\x0c\x95\xd5\x02\x81\x81\x00\xe1\x9ey\xc8\xe2\xd3\x93\xa2nj\xe1.\xaa\xe3\xa7\xf5P\xd1\xd8yM\x01\xdc\x01\x0c\xdbQG\x1b=\xbe\xe4.\x9cM\xc2\xda\xd2\xa4\xb3\x80\xb2\xbd\xbaO\x1bD&]0\x0b\xe6\xf5\x08\xdb*I\xfe+@Aa\x16;\x9a%\x8cof:\x156 \xb0\xe6\xfe\x95\x9bO\x85]\x96\x94S\x05\xc8\x8a\xb6\x92\xb3\x95\xc5\xfbX\xa9S<@\x12\x94K\x8b\xa3\x0f\xebO\xb5\x9f\x0c\x08\xf2\xccS\xfd8\x06\xeb\xaa\x96_\xadm&L~!\x18\xef\x02\x81\x80@.\x04\xa6\xd7K\xfb\xb5\r\xb1\xbe\x94\x10\xe6\x14.\xd4\x1a\xf3\x86\x93D`Kx\xf0%{^\xdf\x9c\xd4P\x19w\xe3\t8\xceB\x93\x83m\x85\xdd\xf8\xfc\xd8\xa0Cp>\x9bH\r\\\xedf\x8a\x1f\xe7P\x85\xbe\xbei\xa0\xdf\xa7\xda8s\t\xdbXi\x89s\x05\xa2-C\x1a\xb2r#\xef\xc0\xf7\xda@\xe2T\x99k\xcf\xcc\xbc\xc5\xb7\x10\x8d\x94B\xa4:\xcd\xf6@Ea\xb1\xe2\x1bRw\x03\xf1E\xfdL>\xbd.\xc0\x94S}\x02\x81\x81\x00\xa2\xce\x13}EH}a\x19\xa2`I\xa7\xa0\xcdc4\xe5\xa7\xfa\xa7\xf9\xee\x82\x87\x7f\x7f\x1f\xfbeK\xe9&E=\xcb\x9c\xd1\xa1m\xb21\xc8\xbc\xb76\xaa\xaf\xb0P\xeaU\xc7}\x93\x80\xe9\x91\xd2-\xf4\xbf\x95&\x7f.\x17/\x8f\xa9\xdc\x02\x8a\x06}9:E\xafUBZU?\xaf\x8d\xad\xa2\xdf+]\xa9V\x9c\xfc\xda\x86@\x89\xe7\x9e\xb7\xed{\xa0F\x8d}nV\xca\xb5l\xe9\xedR\xf9\x1d\xc8\x92\xd3\xf7NJ\xa6=E\xdb\x02\x81\x81\x00\xf5\xa8\xec\x00k\x18\x10KK\xd0D\xa9\xeb\x87==X\xa2\xaa)\xeb\x92\xfa\xf8f\xa6W\xaa\x94\x92\xa1F\t\xc1\x01\xd8%-\x1f\xb71\xefg\x95q\xb3\xa5J[k\xe3\x17\xac\xfd\xbfU\x02\x95\xa4\xf9\xcd\x80!E\x9d\x7f\x9c\xcd\x89uV\x1df\xee\xab\xd3\x1f7$&\x014\xd2\xdd\xc2\xe4?\x1bh*\xb6\x00\x1a\x1fz^\xbc\x97\xde\x9cK\xc8\xf5\xcf0\"\x8c\x8bm\xecUv\xefu\xd9YD\x05\xe8?9J\x8c\x18\x90\x0e\xc4\x88"  # pylint: disable=C0301
 
         imported_key_label = "imported_keypair_label_RSA"
         signature_val = b"\xd4\x94'N(\x1c\x16\xc11\xf0#\xe0\xb0\x0b\xc4L[D\xed6<-\xb53\xa0\x9fm\xdd\xfd_\xd7\xb5\xbe]KAu\xb5\x99\x11z@-6/-\xc9_\xde\x05\xba\xb6\x81\xad|\x95\xd8*\xc4\xa4<\xcfE\xaaE\x922e\xa1\x81\xa6\xe9\x94:M\x17_\x0ba\xdd\x94|1\x15|;%z\xc2\x9c\xe4b\xf9\x06es@U\xcd\x83x\xb4\x08&\xb7\xc1\xe9\xc8\x04c\x7f\x9b\x0e\xff\xe3\xb68\xbd\xb6\x05\r\xe86\x17L\x1e\xeb\xd7R\xaf\xa2\x7fU\x8e]\x9e\x93\x8f\x17\xed\xa4\x15\xcb\xc5\x84)\xe0\xec\xbe\x90\xba\x1d0jgEY^r\xe8\x18{Q\n\xab\xfe\xf9\xb3#R*8\xc8\x06\xdb\x81\xaf\xd1q\n\xef~S\x9d\xb0\x1f\n\x81@}\xba\xdcL?\xf9\"\xddN|\xb9\x828\x96\x89P\x92&$O\x16P\xbe\xd7\x06\xcc\xd5*P\xcd\x92\x82\xc2\xcf\x94\xf0\x1e\xe3\xc1\xd6\xf9\x1b\xccE!tE\x87\x05o'|\xab\x9b!5ua\xed\xe0\x7f\x15\xc8t;.\xf5"  # pylint: disable=C0301
 
-        asyncio.run(PKCS11Session.import_keypair(pub, priv, imported_key_label, key_type="rsa_2048"))
-        pk_info, identifier = asyncio.run(PKCS11Session.public_key_data(imported_key_label, key_type="rsa_2048"))
+        asyncio.run(PKCS11Session().import_keypair(pub, priv, imported_key_label, key_type="rsa_2048"))
+        pk_info, identifier = asyncio.run(PKCS11Session().public_key_data(imported_key_label, key_type="rsa_2048"))
 
         self.assertTrue(isinstance(identifier, bytes))
         self.assertTrue(identifier == b'\xf0c\xd5\xe2X\xdc\x19@\xa2\xbc#\x13\x0c_\xaae\x16\xde"f')
         self.assertTrue(isinstance(pk_info, str))
 
-        self.assertTrue(imported_key_label in asyncio.run(PKCS11Session.key_labels()))
+        self.assertTrue(imported_key_label in asyncio.run(PKCS11Session().key_labels()))
         with self.assertRaises(MultipleObjectsReturned):
-            asyncio.run(PKCS11Session.import_keypair(pub, priv, imported_key_label, key_type="rsa_2048"))
+            asyncio.run(PKCS11Session().import_keypair(pub, priv, imported_key_label, key_type="rsa_2048"))
 
         data_to_be_signed = b"MY TEST DATA TO BE SIGNED HERE"
-        signature = asyncio.run(PKCS11Session.sign(imported_key_label, data_to_be_signed, key_type="rsa_2048"))
+        signature = asyncio.run(PKCS11Session().sign(imported_key_label, data_to_be_signed, key_type="rsa_2048"))
         self.assertTrue(isinstance(signature, bytes))
         self.assertTrue(signature == signature_val)
         self.assertTrue(
-            asyncio.run(PKCS11Session.verify(imported_key_label, data_to_be_signed, signature, key_type="rsa_2048"))
+            asyncio.run(PKCS11Session().verify(imported_key_label, data_to_be_signed, signature, key_type="rsa_2048"))
         )
         self.assertFalse(
             asyncio.run(
-                PKCS11Session.verify(
+                PKCS11Session().verify(
                     imported_key_label, data_to_be_signed, b"NOT VALID SIGNATURE HERE", key_type="rsa_2048"
                 )
             )
         )
 
         # Delete the test key
-        asyncio.run(PKCS11Session.delete_keypair(imported_key_label, key_type="rsa_2048"))
+        asyncio.run(PKCS11Session().delete_keypair(imported_key_label, key_type="rsa_2048"))
 
     def test_import_keypair_rsa_4096(self) -> None:
         """Import keypair with key_label in the PKCS11 device.
 
         Generate pub and priv with
         openssl genrsa -out rsaprivkey.pem 4096
         openssl rsa -inform pem -in rsaprivkey.pem -outform der -out PrivateKey.der
@@ -93,477 +111,481 @@
 
         pub = b'0\x82\x02\n\x02\x82\x02\x01\x00\xdd\xa8\x14\xa7@h\xb1\xb3\x9e\x82\x87\x0e\xfc\x0c\xb4\xa9\x1f\xe2iO\xc7a\xec,\xb2\x0c\x15N\xe9\xa4nx,c^\xc1\xe2Oe\xfe\x8cG\x1c\xcf#\x195\xd0\xf6\xb3N\xb9\xf7\xe4\xcf\xb0\xfb\xd9<:\xc2\x12\x10\xa1\xd66\xb5\xbd\xedG\x8e(\xb0\x05\xa4.\x12O6\xd0D\xc3\x1a\xed\x00\x86\xe8\x19T\xa6T|\xd8\x8dy&+\xf5\xfb1cq\xac\x92\xed\xed\xe6\xe2\xe9v\xcf\x99\x8a\x9e\xce,"\x8e\xd3\xec\x1e\xa0pl\xe6\xff\x8ai\x9bk\x95\x18\xa6\xcb\x16o\x86\x85T\xe0\x9a)_-#\x87?\x905\xa5\xddw\xb55\xd1\xa1\xd2\x93\xa5\x90\x81\x861\xd3\x82\xd3\x8auy\xc7j\xc2\xed\x92\xdb\x0e>Uam\x13\xde\x03\xfe\xb6\xa0\xfe\xa0\xc8\xb2\x8e\x85\xc2\xc9^w\xe2<$\xe0\xacY\x0b}(H\xb4\xdbj\xe9`\xc4\\\x99\xfesY\xacB;\xae\x82\xfa\xf7\xb2\xef\xea\x9e\xcdS\xe8\x86\xab\x7f\xdb\xc2s\x14!\xf0\xbb\xdd\x03\xe9wa\xe6\xdc/s\xb8\xfb\xef\xefj\xc1SP0c\xa6\xb4R\xca\xa5\x05\x131\xd4\xbfx:\x7f\xc1>\x15\x7f+\xbdlBw\xd9\x80\xc2\x02\xc5I\x8c1\x93w\x8d\x86\x04W~\xa56\xb5oD\x9b\x1f\xc61\xeb\x7f(\xa2\xc0\xd7k\x1d{,\xe4\xac\x81\x10\xbb\ti\x7f\xee\xa4G\xff\xc8\xa3\xfc\xcad41\x82\x1d\x9cb\xa9r\x88\xa1\x92\xdc\x90\xfa\xc4TL\x02v\xc0Ls"\xf4\x08c\x0c|\x8a\xaa\x94\xf6\xae\x8d\xff\x0cE\x94jl\x95\x8b\x10&\x83]\x8f5\xc1\x1e\x8d\x1d*\x19\x06\xff\x1cC\x1ec\xa8\xb4\x05v>\xb9\xb1>\x0b\xd2\xc7q\x99\xc4H\x7f2\xfd\x91\xdc_\x9e\xcd\xdd\x18\x16\xad\xff\xfbY\x13N\xd0L\xb4\x80\x8d\xcc\xb3,p\x84\xd2\x93\xe3\xb0\x1d\xea\xcb\x03\x02o\xc3\x0f\x8b@\xe4NO\x1e;g\xff\x0bm\xe5\xc6\xf86\x9b\xa75\xa9\xb1\x93/Xs\x82\xa8\xd8\xd99B}\x9b\x95\x1e\xba\xb4\xe0\x1fP\x90\xca\xdb\x02\xe2\x14\xca\xf6\x90\x7f\x9a\xd4\xc1\xc2\x84*+\x19\x94\xba%+\x12\xa3\xdf\x97\x02\x03\x01\x00\x01'  # pylint: disable=C0301
         priv = b'0\x82\t)\x02\x01\x00\x02\x82\x02\x01\x00\xdd\xa8\x14\xa7@h\xb1\xb3\x9e\x82\x87\x0e\xfc\x0c\xb4\xa9\x1f\xe2iO\xc7a\xec,\xb2\x0c\x15N\xe9\xa4nx,c^\xc1\xe2Oe\xfe\x8cG\x1c\xcf#\x195\xd0\xf6\xb3N\xb9\xf7\xe4\xcf\xb0\xfb\xd9<:\xc2\x12\x10\xa1\xd66\xb5\xbd\xedG\x8e(\xb0\x05\xa4.\x12O6\xd0D\xc3\x1a\xed\x00\x86\xe8\x19T\xa6T|\xd8\x8dy&+\xf5\xfb1cq\xac\x92\xed\xed\xe6\xe2\xe9v\xcf\x99\x8a\x9e\xce,"\x8e\xd3\xec\x1e\xa0pl\xe6\xff\x8ai\x9bk\x95\x18\xa6\xcb\x16o\x86\x85T\xe0\x9a)_-#\x87?\x905\xa5\xddw\xb55\xd1\xa1\xd2\x93\xa5\x90\x81\x861\xd3\x82\xd3\x8auy\xc7j\xc2\xed\x92\xdb\x0e>Uam\x13\xde\x03\xfe\xb6\xa0\xfe\xa0\xc8\xb2\x8e\x85\xc2\xc9^w\xe2<$\xe0\xacY\x0b}(H\xb4\xdbj\xe9`\xc4\\\x99\xfesY\xacB;\xae\x82\xfa\xf7\xb2\xef\xea\x9e\xcdS\xe8\x86\xab\x7f\xdb\xc2s\x14!\xf0\xbb\xdd\x03\xe9wa\xe6\xdc/s\xb8\xfb\xef\xefj\xc1SP0c\xa6\xb4R\xca\xa5\x05\x131\xd4\xbfx:\x7f\xc1>\x15\x7f+\xbdlBw\xd9\x80\xc2\x02\xc5I\x8c1\x93w\x8d\x86\x04W~\xa56\xb5oD\x9b\x1f\xc61\xeb\x7f(\xa2\xc0\xd7k\x1d{,\xe4\xac\x81\x10\xbb\ti\x7f\xee\xa4G\xff\xc8\xa3\xfc\xcad41\x82\x1d\x9cb\xa9r\x88\xa1\x92\xdc\x90\xfa\xc4TL\x02v\xc0Ls"\xf4\x08c\x0c|\x8a\xaa\x94\xf6\xae\x8d\xff\x0cE\x94jl\x95\x8b\x10&\x83]\x8f5\xc1\x1e\x8d\x1d*\x19\x06\xff\x1cC\x1ec\xa8\xb4\x05v>\xb9\xb1>\x0b\xd2\xc7q\x99\xc4H\x7f2\xfd\x91\xdc_\x9e\xcd\xdd\x18\x16\xad\xff\xfbY\x13N\xd0L\xb4\x80\x8d\xcc\xb3,p\x84\xd2\x93\xe3\xb0\x1d\xea\xcb\x03\x02o\xc3\x0f\x8b@\xe4NO\x1e;g\xff\x0bm\xe5\xc6\xf86\x9b\xa75\xa9\xb1\x93/Xs\x82\xa8\xd8\xd99B}\x9b\x95\x1e\xba\xb4\xe0\x1fP\x90\xca\xdb\x02\xe2\x14\xca\xf6\x90\x7f\x9a\xd4\xc1\xc2\x84*+\x19\x94\xba%+\x12\xa3\xdf\x97\x02\x03\x01\x00\x01\x02\x82\x02\x01\x00\x82\xa01;\xb7\x8b{]\xddF\x13\r\xd3\xa01?\x92\x18\xbd\xf3T\x0e\xf3>\x0b\xd7o\x1fH5\xad\x1c\x89\x1c.\x95\x98\'.vjx\xe6\x13t\x1d\xc1GZ{\xa5#\x97ar\xbc\\OS]UM\x8c\x1b\xb3\xc0\x1e.\xc5\x8c\xeb\xcc2\x9f\xc0w\x9e6\xac\x98\xe4M\x0e\xab)*W\xd1\xc5\xbf\x17\xffS\'\\\x84\x10X0&\x94\xf2B\xbf|\x14=\x82\xf0\x0f"\x9c\xdb\xc2f\xc2?\xc3hD\xb8o\xd8\x91u8\x97{Q*\x7f}=\x9ee\xa4g\xe4_v\xd5\xa3\x18\x01\xe3\xf4*\x93s\xeaA\xaf\xf0L\xbd3\xde\x83@\x88\xfe\xab\xf4\xe5/.7d\xaf\xd5\xc3\xa7\x08\x97\t\x1dE\xc2\xcf]\x96\xdd\xba\x00\xfb\xe3\xb8\xebL\x1b^>\x99\xe2N\x17\xdcm\x91V\x0e{\x93w\xb8\xab\xd0Y\x96\x91\xde\x83\x1a\x07n\x9a\xcf\xf7\xe28\x85\xc9\x8e\xd96\xcc\x88\xb9\xf9K?\xb7M\x8eV\x16+\xf7ka\x11uX~\xd7\xea\x0cA*}\xca@>\xd0\x1bZ\xa6\x19\x83\xb0l\xee\xbf<\xa5\x15\xe3\xfd\xde\xc3\x85N\xf0\xda\xaa\x05.\xd3\x7fg\x85\x95\r\xdai\x00k\x80\x9c\x81\xb2\x0c\xe5\xd8s!@\xe8\xea%d\x87\n\x9eB8\xdd\xe3\xdfh5\xfb$\x14\xa9\xd3\xc5\xbf\xbfx\xfc\xf9\xf2\xfc\xc1\xb9\x1d\x14"\x1e\x98<?\xb7\x90*{X\xa0\xeb\xa9\xa9\x10Y\x19V\xf2\x83:LB\xdd\xae(B\xd2\xb5B\xc8\x8a\x08\xffM\xcc)h\x8fS|\xa5\xa3>&\x14.\x9c\'\xfe\xe0/\xc9\xdb\x9e\xc9\xfc&\xc8\x10>i\xd3ZT\x99n\x02c\x86\xe6:\xb7\x96\xd11\xe7\x00M\x9f\xf1\x83\xe8{\xa6F\x1f \xbas\n\x19pP\xe8\x0b\x02j\xe1z\xe8A\x82u\xc2\xce|d,$\xaf\xf6<7\xd6\x08\x92\xa9\x82\x9c\xb4\x8a\xbeA\xa8\x82\x8d\x83\x1f\x08g\x99\xdc\x7f\xe9\xb5C\xca\xcc\xd7\xb3J\x82\xb9\xfc\xe8\xf2\x1bU\xa0VK\xe1\xbd\x8f\x90\x08\xec\x97\x93\x8d\xbd\x975]8Ax\xde\x80\xd3\xbdr\r\xc639\xd9\x9dTZ\xce!!\x02\x82\x01\x01\x00\xf8btWk~\n\xd9^L\x1b\x16iN\x0b\xb4/\xd6\x9f\xe5\xf3;\xca\xe3\xf46g*ih\xfa\xd9|\x83eR^\x1d\x913\xf9q"\xcf\x84M\x85]\xcapy2|@G3jvp}\x15\xf4\x80\xd0\xbb\xe6\xd75\xb3|\x8d\xbc,\xcc\x83\xf0E\x87\x9c\xab\n\xac\xe1#`\x85-\xaf\x8d/\x08\x9a\xdc\x89\x11\xdbp\x1fcv\xf7\xe0\xc6s\xa2\xdeJM\xd9ku\x93\xa4\xc9\xf0\x9a\x17I\xbd9t\x8f\x1c\xd2\xa9\xefP\x80?\xec\xdd\x97x\x1a\xf4\xd3\t\xac\xd7\xb0\t+\x94\xaf\x90\xdf9N\x0eva!\xd0\x90>\xcf\xfcS\xa9\\\\\xb2a\xaad\xea\x06\xa9\xab\xa50\xfftg-\xcd7\xf8\xae)-\x19\xc9\x8b\xd6\xa8\xe5+W\x8e\xbb\xe6\xe4\xe2%a\x0c\x88\xe9HF\x06\xc2\x7f\xbd\xba\x92\xae\r\xf7"\xa9\xbdK5\xb19\n\x03\xc1p\x05\x04\x87\xf9\xaa\xf3xQ\xd3z\xfb\xab\x8f\xdb\xec\xb30G[B\xf6\x03\xa7\xb4o/\xbb\xf3\xf1Xv&\x90\xab\xdf\x02\x82\x01\x01\x00\xe4s\xd76\rR\xa63\x9cQD\xa7 \x81\xcb\xa3l<B\x95?\x12\n\xc5\xady\x83O5U\x1a\xc0\xd2*\xd4I\x96\xb8\xc3\xfeH1\xecS)j!\xda<\xd3F\xa7Pe[\x1dacL\xf7\xa2\x93\xbf\xc3\xb9\xb4\x1a\x89\x9e\xaf\xf2\xb3\xec\xbe\x11\xe5\x1c$\xb3y\xde\x90t%Q\xb5\x03Ep-\xea\x16f9\xec\x9a\x82\xd1%d\xa3\x0b\xee\xdc\xd8\xd0\xe8\x00\xdb\xed\xa6\xb0\xa8I\x98\xbb\x8d\x1a\xc6\xb7\xb2l\xac\xeb\x83\xab\xac\xa1\xfb\x86\x91\x17\xf6\xb8\x02\xd9v\xacCr\t~\xc6\xfa\xb7\xc8\\F\xc9\x00U\x1cR6\x06\xea\x9b\xa4\xc9/\xd8\rU\x96\xd8Vz\xcel\xcaH2\xb5\x9b\xc0\x89\x0b,\xd9\xc93fh\x92\xa9&\xbal\xf1\x8f\x82\xd5\x9d\x16\xd5\xc4\x9f\xa6\x051\'=\x8c\x1f\xa8\x14?=\x04\xf6\xeb7\x05\xd6\x00/7\x8d\xb97W\xe6\xdf|\x06\x04\x9f\xded\xd2\xa7aN\x1e"\x99a\xb9\x10o\x85\xa9$\xe8\x98\xb1\x9b\x94Y\xf2\xc33\xae\x88\xc3I\x02\x82\x01\x00`@&\xbdI\x96J5\xf9h\x9c\x86\x8e\xc0\x03\xa1\x0bx\xab\xf5\xbb\xcf\xcb\xcb\x91\xf3\x12\xffHa\xb9\xf3U`\xc5~\xa9\xa1\xe3\x86\xb4~\xb6\xf2\x9b^>\xf4\x1db\x80T\xa3\xf9t\x9d\xe3\xff\x89\x8f\xafVT$\x8e\xeb\xe11\x9a \x05\xfc\x89\x8f\xa7\x01\x10\xb0\x80qwm\x8e\xc0\xda\xc2@\xf5\xeaK\xf3\x95\xaf(\x1e\x97^W\x8b\x7f\xaa\x86\x9b\xe0k\x98\xa0J\x92\x9a%\xb1\xd5\x05\xbc\n\xbaC\x84\xe4"\xda\xe2\\p%\xa0\x98R-C\xa1R\x95\x7f\x91\xd8\t\xf6z\xec\xd2\xca\x87N(rXa\x1aV\x81x\x04\xad\x92\x83A\x18<\x06_\xc9\xa0\xf2\x02\x0e\x1a\xe9\xbc\xd5\xc3\xe8#\xa3\x88\x06\xcc\x83\x10\xc9\xbdXp\xab\xfa>\xf4\x10\xb5\xea\xf2\x8awg\xec\xb7\xa2\xc6c\x8f_G7\xa1\x1a\x0f\x85\x0b<]^QP7\xba9T<(Ut\\Q$\xda\xae\x06N\x0f\x19u5\x02FB\xef\x1d"I\xa7%\x16=\x82\x9a#q>\x12\xa4)\x04\xc0\xc3\x19\x02\x82\x01\x00m\xc2V0\xca\xff\xdd\x88H_\'K\xe0\xab[\xaa]\xb3*\x0eH\xaa#p\xcc"\xe8z\xa2\xd6\x0b\xaf~\x8aCJC\xd6\xeb\x9b}\x167C\xd1O\x03\x8a\xb5\xd4\x90J\x8c\xae\xd5\xb2\xec\xfag\x9dF\x88\x14\x076n\x98\x9dl\x17~\xd5\x016d\xa4\x9d\xfb\xe8\x1a\xf2Z\x96\xe2\xe39\xc3\xa3\x95\xfd\tM\xcf\xb9\x9e\xba\xb1\x85H\xa0\xecQ,g\x00\xe8\x85\xbe\xfb\xebW=\xe2\xec\xd1+\xb2\xe4\x9dz\xde\x87\xa6 \xd57#\x0f\x04(\xa8\x07Jk(;P\xef\xfc\xcb\x8aRU\xc9Y\x893\x04sG\xec\x9cY\xc7IUh\x88(}\x0b!\x84\xf0\x9fj\x15@\x9e6%\xaf\xef_0\x86\xe7N\x9a(7\xc0\xc9\x17E\x9b\xac\xcf\xf0\xd3\x11z\x0e*MtU{\xcf\\\xc9L\xa1\xc9\x07\xd9\nu\x07\xb0\x96[\xee:\xde\x05\xd1|\x0e\xf3\xcf\x10\xc6h\xf0\xffA\xcb\xf8\xc6\xd8\xd2@T\xec,\xa3-\xe5\xfe\x9e\xca H|,@\xe2j\xc0\xdf\x162\x91\xd4\xb9\x02\x82\x01\x01\x00\xcdZ\x83\xcf\x9b\x0b\xe17\xd9w\xf0y\xc6\xaa]\xbf\xd7\xc9\tt\x8d\xb5e^\xe4\xda\xad\xa1-\x06\xca\x87\xb9\xe9V\xbe\xcc\xbf"-\xe9\x04\xc8\x97I\xc6\x8c\xf7\'\'\xa8\xb9\xc9V\xb6a\xff$\xb1i\xd8e\x9f@\xba-_NP-F\x1f\x1f\x89h\xa4Q\x1e\xb8*=\x15\xc1\xf4;\xf2\xbbl\x19f\xe0\rLo#\x9ai\xc9\xd8\xfa\x96["\xd9\xa7\x12}\x91\x1a\xb0\xa0<\xa2\xa4\x88.;\xfb\xa7\xab\xc5\x03\x8cI\xaf\n.\xd1\xfayb\x00|`\x04\xf3`\xa1\x9b\xe2\xee\xd7\x8d[a\xdf\x93`\xde\x00\tQ\x94.\x94&s@XqNf\xe5T\xb9\xbc\xc5\xc0Ack!\xca\x90\xe0\xb1o\xcfv\x19\x7f\x8a\x8e\xd7]\x8d\x1a\'\xf6\x11\xc4\x92@\xc8#\xbd\xba\x12\x8bf\x0e\xad\xb3(m\r\xa7U\x90sD\xb0U\xaf\xc5Aw\xb08\xd6\xf8\x9f\xf9\x9c5\x13iQ\xa4<h\xb4\x06\xd8E\xe8\xd1\xd9\xee\x02CX\x8e\xa4\xa3\x97\xd4^\xf4\x89N\x9d}M\xfb\x83'  # pylint: disable=C0301
 
         imported_key_label = "imported_keypair_label_RSA_4096"
         signature_val = b"\xad>\xb6\xf4\x8f\xb1s>\xa8\x99\x10zt\xa2\xf2\xc0&C.\"\x96\x0fOaD\xfa\x10\xe1\xc4qqx\xfd\xc0\x82,\xc1\x0e\xcf\x82\xda\x8d\x9d\xec\xe3\xd6\xe2\xa10;s,\xbb\xa5_\xa4\xb3?\x8bm\x8d!\x85\xacb\xfd\xdc,fkl\r\xb5j\x0e<\xfcI\xea_\x03\x03\x1bi\xa3\x8f\xc2y\xeb^\xe1u\xee\x91dg\xf9y\xd0\xb0\xa4\x00\xba\x0cm\x05\xf9\x19\xec\tq\x8e\xe2]<\x83\xf0\x9f;\xfa\x11}# \xa2\x05\x93\x82\xb9T\xd7\x05n\xa5S\xa7[\xed\xc5\x979\xce\xf8m\xfeA\x8c$09,\xd5\x0f/g\xa1D\x05\xc1`\xd5\x1d\x03#\xd6\x9c\xc9K\xf04\x8fsM\xb6\xd2\x97W\xa9T\x8c\r\xcb\xff[!\xbb\xc2\xfa@\x1a\xbc\xd2r\xbb\x95\x06\x9c\xd7\x88\x9f\x06\t\xb3\xa4\x8f\xed\xa8-\xde\xdd5\xad\xf8F\xbbH\xa6\xdaX\x81\x00\xf7Tge\x04E\xda\xfcN\xf4\xfc\x88X\xebu\x00\x02R\xdePB\x90\xa5\xf2\xb8=vC}(\xee`\xa3:\xe9f3\xf111\xfb\n\x88%A\x87\x9a;\x1e\xfe\x7f5\xeefe=\xbf~\xcf\xbd\x89\xa9\x8d\xd6\x92\x07F\xa0\xc3\xab\x0f\x82\x91\xf8\x1f\xad\xc6)\xd7\xe2r\\\x87\xebS\xaa\xf6\xfb\\\xa76\x16\xb0\xbe\xe5\x1c\x11c\xf7\x03\x83\x0f%\xd1\x17\x8d\x0b9wH\x9d{f\x9f\xc7\xd8\xa8f\xf0\x8d\r;\xdbqZ\xb0p\\G2B8n\x19\x8bOca\xe8S{\xa2s\xc6tcZrl[\xd6\x1c*\x96\xbf\xbd\x87p\xe7\x18K\x1ep\x1aYs\x1e?\xa2\xcd\x8b\xbd\xb2z\xf0d\xb8|I\xb9\x86{\r\xa2A\xe8\x9b[.\x8eu\xa1\xb1\x9f\x00\xe33cF\xc48*\xabHf\x93$o\xa2\x9foVP\xae\xe2[D\xe3A\xb9\xca\xeb\xa9\x13\x00\xce\x03\x81\xe1\xad\xf5\xc0\x8d\x83g1\xfa`'f\xcd\xa1D#\x16\xb4\xf0\x02C?G`{I\x96\xd2_\xdbeYd\xab\xb7\xe9nFx\x07k\xcd\xe9cQ),\x18\xa2\xdb\xac\xd9\xb5?\x85\xac\x11X&l\xb9`\x17"  # pylint: disable=C0301
 
-        asyncio.run(PKCS11Session.import_keypair(pub, priv, imported_key_label, key_type="rsa_4096"))
-        pk_info, identifier = asyncio.run(PKCS11Session.public_key_data(imported_key_label, key_type="rsa_4096"))
+        asyncio.run(PKCS11Session().import_keypair(pub, priv, imported_key_label, key_type="rsa_4096"))
+        pk_info, identifier = asyncio.run(PKCS11Session().public_key_data(imported_key_label, key_type="rsa_4096"))
 
         self.assertTrue(isinstance(identifier, bytes))
         self.assertTrue(identifier == b"\xb9\xdc.\x1a\x15\x8eQ\xd5;\x1d\xab*#\xbcFH\x05\xb4QH")
         self.assertTrue(isinstance(pk_info, str))
 
-        self.assertTrue(imported_key_label in asyncio.run(PKCS11Session.key_labels()))
+        self.assertTrue(imported_key_label in asyncio.run(PKCS11Session().key_labels()))
         with self.assertRaises(MultipleObjectsReturned):
-            asyncio.run(PKCS11Session.import_keypair(pub, priv, imported_key_label, key_type="rsa_4096"))
+            asyncio.run(PKCS11Session().import_keypair(pub, priv, imported_key_label, key_type="rsa_4096"))
 
         data_to_be_signed = b"MY TEST DATA TO BE SIGNED HERE"
-        signature = asyncio.run(PKCS11Session.sign(imported_key_label, data_to_be_signed, key_type="rsa_4096"))
+        signature = asyncio.run(PKCS11Session().sign(imported_key_label, data_to_be_signed, key_type="rsa_4096"))
         self.assertTrue(isinstance(signature, bytes))
         self.assertTrue(signature == signature_val)
         self.assertTrue(
-            asyncio.run(PKCS11Session.verify(imported_key_label, data_to_be_signed, signature, key_type="rsa_4096"))
+            asyncio.run(PKCS11Session().verify(imported_key_label, data_to_be_signed, signature, key_type="rsa_4096"))
         )
         self.assertFalse(
             asyncio.run(
-                PKCS11Session.verify(
+                PKCS11Session().verify(
                     imported_key_label, data_to_be_signed, b"NOT VALID SIGNATURE HERE", key_type="rsa_4096"
                 )
             )
         )
 
         # Delete the test key
-        asyncio.run(PKCS11Session.delete_keypair(imported_key_label, key_type="rsa_4096"))
+        asyncio.run(PKCS11Session().delete_keypair(imported_key_label, key_type="rsa_4096"))
 
     def test_import_keypair_ed25519(self) -> None:
         """Import keypair with key_label in the PKCS11 device.
 
         Generate pub and priv with
         openssl genpkey -algorithm ed25519 -out private.pem
         openssl pkey -in private.pem -outform DER -out private.key
         openssl pkey -in private.pem -pubout -outform DER -out public.key
         """
 
         priv = b"0.\x02\x01\x000\x05\x06\x03+ep\x04\"\x04 ~n\xc3\xf5\x93\xb7\x1dYgO\x88\x90K\x9b\xe1&h\x0f\x0e@\xddh\xcc'\x98\xd2\xe7\xe7\xfb\x03T\xd1"  # pylint: disable=C0301
         pub = b"0*0\x05\x06\x03+ep\x03!\x00\x8b\x07J\x99[\xe4g\x9c\xd9\xfa'\x03\x9a\xb8\x01>&\x10\x1cay~\xadf\x80j\x9eq;\xb3\xf3\x9c"  # pylint: disable=C0301
 
-        for key_type in ["ed25519", None]:
+        for key_type in ["ed25519", KEYTYPES.ED25519]:
             imported_key_label = "imported_keypair_label_ed25519"
-            new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
+            new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
 
-            asyncio.run(PKCS11Session.create_keypair(new_key_label, key_type=key_type))
-            pk_info, identifier = asyncio.run(PKCS11Session.public_key_data(new_key_label, key_type))
+            asyncio.run(PKCS11Session().create_keypair(new_key_label, key_type=key_type))
+            pk_info, identifier = asyncio.run(PKCS11Session().public_key_data(new_key_label, key_type))
 
-            asyncio.run(PKCS11Session.import_keypair(pub, priv, imported_key_label, key_type="ed25519"))
-            pk_info, identifier = asyncio.run(PKCS11Session.public_key_data(imported_key_label, key_type))
+            asyncio.run(PKCS11Session().import_keypair(pub, priv, imported_key_label, key_type="ed25519"))
+            pk_info, identifier = asyncio.run(PKCS11Session().public_key_data(imported_key_label, key_type))
 
             self.assertTrue(isinstance(identifier, bytes))
             self.assertTrue(identifier == b"\xdc\xceO\\\xbe'\x84\xf5\x9b*\x84~;\x1e\xeciJ\xa8\xe3\xd4")
             self.assertTrue(isinstance(pk_info, str))
 
-            self.assertTrue(imported_key_label in asyncio.run(PKCS11Session.key_labels()))
-            self.assertTrue(asyncio.run(PKCS11Session.key_labels())[imported_key_label] == "ed25519")
+            self.assertTrue(imported_key_label in asyncio.run(PKCS11Session().key_labels()))
+            self.assertTrue(asyncio.run(PKCS11Session().key_labels())[imported_key_label] == "ed25519")
             with self.assertRaises(MultipleObjectsReturned):
                 asyncio.run(
-                    PKCS11Session.import_keypair(
+                    PKCS11Session().import_keypair(
                         pub,
                         priv,
                         imported_key_label,
                         key_type="ed25519",
                     )
                 )
 
             data_to_be_signed = b"MY TEST DATA TO BE SIGNED HERE"
             signature = asyncio.run(
-                PKCS11Session.sign(imported_key_label, data_to_be_signed, verify_signature=True, key_type=key_type)
+                PKCS11Session().sign(imported_key_label, data_to_be_signed, verify_signature=True, key_type=key_type)
             )
             self.assertTrue(isinstance(signature, bytes))
             self.assertTrue(
                 signature
                 == b"%\xf4\xadk\x08\xb5\xb4u\xc0Y&\x12\xad\xafn\xed\xd3WJ\x8d(\xb8\xbf\xcb\xc9\x19\xf3\x13\x0e\x9a\x89\xec\x8dk\xd7g;\xb5\xb1\x06;!\x12\xcbW\xcdsT\xce\x87\xe2\xf2\x97\x9eX\xb0i\xccn\xf7\x88\xcd`\r"  # pylint: disable=C0301
             )
             self.assertTrue(
-                asyncio.run(PKCS11Session.verify(imported_key_label, data_to_be_signed, signature, key_type=key_type))
+                asyncio.run(PKCS11Session().verify(imported_key_label, data_to_be_signed, signature, key_type=key_type))
             )
             self.assertFalse(
                 asyncio.run(
-                    PKCS11Session.verify(
+                    PKCS11Session().verify(
                         imported_key_label, data_to_be_signed, b"NOT VALID SIGNATURE HERE", key_type=key_type
                     )
                 )
             )
 
             # Delete the test key
-            asyncio.run(PKCS11Session.delete_keypair(imported_key_label, key_type=key_type))
-            asyncio.run(PKCS11Session.delete_keypair(new_key_label, key_type=key_type))
+            asyncio.run(PKCS11Session().delete_keypair(imported_key_label, key_type=key_type))
+            asyncio.run(PKCS11Session().delete_keypair(new_key_label, key_type=key_type))
 
     def test_import_keypair_ed448(self) -> None:
         """Import keypair with key_label in the PKCS11 device.
 
         Generate pub and priv with
         openssl genpkey -algorithm ed448 -out private.pem
         openssl pkey -in private.pem -outform DER -out private.key
         openssl pkey -in private.pem -pubout -outform DER -out public.key
         """
 
         priv = b"0G\x02\x01\x000\x05\x06\x03+eq\x04;\x049@\x02h\x89\xb4\xfdk\x05\xeblM\xe2\x8fT\x90QH\xacF\x8f\x9c\xd5\xf0b6U\x91Gu\x119Q\xff\x10\xae\x9fG\xe1\x7fiUu\xf3-\xdf\x9di(\xa26.\x93\x0f\xd6{#?"  # pylint: disable=C0301
         pub = b"0C0\x05\x06\x03+eq\x03:\x00N\x9e/u\xd35x]8k\xad\xbf\xf4\x06D\xf83\xcf\xea0\x91WS\xc0o\x17\x9f\xdc\xc7\xd8\xb2\x96\x07a\x14\xea\xf5\xcd\xe2D\xde\x8d\x15\xeb\x9b\xf6\xa7\xbe\r\x81\xa0\xfd\x10\xb2G \x80"  # pylint: disable=C0301
 
-        imported_key_label = "imported_keypair_label_ed448"
-        new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        imported_key_label = "testpkcsimported_keypair_label_ed448"
+        new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
 
-        asyncio.run(PKCS11Session.create_keypair(new_key_label, key_type="ed448"))
-        pk_info, identifier = asyncio.run(PKCS11Session.public_key_data(new_key_label, "ed448"))
+        asyncio.run(PKCS11Session().create_keypair(new_key_label, key_type="ed448"))
+        pk_info, identifier = asyncio.run(PKCS11Session().public_key_data(new_key_label, "ed448"))
 
-        asyncio.run(PKCS11Session.import_keypair(pub, priv, imported_key_label, key_type="ed448"))
-        pk_info, identifier = asyncio.run(PKCS11Session.public_key_data(imported_key_label, key_type="ed448"))
+        asyncio.run(PKCS11Session().import_keypair(pub, priv, imported_key_label, key_type="ed448"))
+        pk_info, identifier = asyncio.run(PKCS11Session().public_key_data(imported_key_label, key_type="ed448"))
         self.assertTrue(isinstance(identifier, bytes))
         self.assertTrue(identifier == b"\xcb\x8d\xa5\x80.\x84\xc87\x18\x99\x1f\x18z^2!\xe6qe=")
         self.assertTrue(isinstance(pk_info, str))
 
-        self.assertTrue(imported_key_label in asyncio.run(PKCS11Session.key_labels()))
-        self.assertTrue(asyncio.run(PKCS11Session.key_labels())[imported_key_label] == "ed448")
+        self.assertTrue(imported_key_label in asyncio.run(PKCS11Session().key_labels()))
+        self.assertTrue(asyncio.run(PKCS11Session().key_labels())[imported_key_label] == "ed448")
         with self.assertRaises(MultipleObjectsReturned):
             asyncio.run(
-                PKCS11Session.import_keypair(
+                PKCS11Session().import_keypair(
                     pub,
                     priv,
                     imported_key_label,
                     "ed448",
                 )
             )
 
         data_to_be_signed = b"MY TEST DATA TO BE SIGNED HERE"
         signature = asyncio.run(
-            PKCS11Session.sign(imported_key_label, data_to_be_signed, verify_signature=True, key_type="ed448")
+            PKCS11Session().sign(imported_key_label, data_to_be_signed, verify_signature=True, key_type="ed448")
         )
         self.assertTrue(isinstance(signature, bytes))
         self.assertTrue(
             signature
             == b'@5\xf1(\x94l\xf6\xec\xd1\x1d\xc43W\xe3\xcb\xaf\x12\xe04\xe6X\xc5<s\xfe\x89\xfa\xb6-\xbe\xaf\x02<\xaa\xd8\xa7\xd8\xea\x01\xcbt\x99\x973sc\x89\xb3\xadG\x0c\xa1\x8e\xc7zY\x80"\xb3\x93\x94\xfaCAwz\x0cs\xf7\xday\x14w\x0f\x94\x05iu\x17J\x8f\x1a\xe2\x8e\xd7\x86ms\t\xc0\x0b\xccq\x10\xd9\xab\xd5\xb6\x98e\xb3\x16#\xef\x93\x1c\xe7\x7f^\r\x9c?\x12\x00'  # pylint: disable=C0301
         )
         self.assertTrue(
-            asyncio.run(PKCS11Session.verify(imported_key_label, data_to_be_signed, signature, key_type="ed448"))
+            asyncio.run(PKCS11Session().verify(imported_key_label, data_to_be_signed, signature, key_type="ed448"))
         )
         self.assertFalse(
             asyncio.run(
-                PKCS11Session.verify(
+                PKCS11Session().verify(
                     imported_key_label, data_to_be_signed, b"NOT VALID SIGNATURE HERE", key_type="ed448"
                 )
             )
         )
 
         # Delete the test key
-        asyncio.run(PKCS11Session.delete_keypair(imported_key_label, key_type="ed448"))
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label, key_type="ed448"))
+        asyncio.run(PKCS11Session().delete_keypair(imported_key_label, key_type="ed448"))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label, key_type="ed448"))
 
     def test_import_keypair_secp256r1(self) -> None:
         """Import keypair with key_label in the PKCS11 device.
 
         openssl ecparam -name secp256r1 -genkey -noout -out private.pem
         openssl ec -in private.pem -outform DER -out private.key
         openssl ec -in private.pem -pubout -out public.pem
         openssl ec -in private.pem -pubout -outform DER -out public.key
 
         """
 
         priv = b"0w\x02\x01\x01\x04 \xc1\x96a \xd3M\xe2\x04\xaaY\xe8{%F\x0eTt?\xa7\x0c\x85\xf3Hh\xbd,&\xe5\x8c\xb5\xa3[\xa0\n\x06\x08*\x86H\xce=\x03\x01\x07\xa1D\x03B\x00\x04\xae-\x90\t\xee-\x8d\xe4\x1b\xcfC\xb4TJ\x89[\x89\x82\x85+9\xb7\x96\xef\x12\xae\xfeG\x1f\xf7aX\x88\xca\xcf\xab9\x0b\xcd>\xb8\xfc\x95g\xa4\xca \r\x9d_\xa2\x1b1*\x17\x11\xc2\x8b\xd0\x98\x94Za\x82"  # pylint: disable=C0301
         pub = b"0Y0\x13\x06\x07*\x86H\xce=\x02\x01\x06\x08*\x86H\xce=\x03\x01\x07\x03B\x00\x04\xae-\x90\t\xee-\x8d\xe4\x1b\xcfC\xb4TJ\x89[\x89\x82\x85+9\xb7\x96\xef\x12\xae\xfeG\x1f\xf7aX\x88\xca\xcf\xab9\x0b\xcd>\xb8\xfc\x95g\xa4\xca \r\x9d_\xa2\x1b1*\x17\x11\xc2\x8b\xd0\x98\x94Za\x82"  # pylint: disable=C0301
 
-        imported_key_label = "imported_keypair_label_secp256r1"
-        new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        imported_key_label = "testpkcsimported_keypair_label_secp256r1"
+        new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
 
-        asyncio.run(PKCS11Session.create_keypair(new_key_label, key_type="secp256r1"))
-        pk_info, identifier = asyncio.run(PKCS11Session.public_key_data(new_key_label, "secp256r1"))
+        asyncio.run(PKCS11Session().create_keypair(new_key_label, key_type="secp256r1"))
+        pk_info, identifier = asyncio.run(PKCS11Session().public_key_data(new_key_label, "secp256r1"))
 
-        asyncio.run(PKCS11Session.import_keypair(pub, priv, imported_key_label, key_type="secp256r1"))
-        pk_info, identifier = asyncio.run(PKCS11Session.public_key_data(imported_key_label, key_type="secp256r1"))
+        asyncio.run(PKCS11Session().import_keypair(pub, priv, imported_key_label, key_type="secp256r1"))
+        pk_info, identifier = asyncio.run(PKCS11Session().public_key_data(imported_key_label, key_type="secp256r1"))
         self.assertTrue(isinstance(identifier, bytes))
         self.assertTrue(identifier == b"E\xb4i\xf6\x9b\xb06\xc2\x1b8!\x1cel\xdc\xcfu$+E")
         self.assertTrue(isinstance(pk_info, str))
 
-        self.assertTrue(imported_key_label in asyncio.run(PKCS11Session.key_labels()))
-        self.assertTrue(asyncio.run(PKCS11Session.key_labels())[imported_key_label] == "secp256r1")
+        self.assertTrue(imported_key_label in asyncio.run(PKCS11Session().key_labels()))
+        self.assertTrue(asyncio.run(PKCS11Session().key_labels())[imported_key_label] == "secp256r1")
         with self.assertRaises(MultipleObjectsReturned):
             asyncio.run(
-                PKCS11Session.import_keypair(
+                PKCS11Session().import_keypair(
                     pub,
                     priv,
                     imported_key_label,
                     "secp256r1",
                 )
             )
 
         data_to_be_signed = b"MY TEST DATA TO BE SIGNED HERE"
         signature = asyncio.run(
-            PKCS11Session.sign(imported_key_label, data_to_be_signed, verify_signature=True, key_type="secp256r1")
+            PKCS11Session().sign(imported_key_label, data_to_be_signed, verify_signature=True, key_type="secp256r1")
         )
         self.assertTrue(isinstance(signature, bytes))
 
         self.assertTrue(
-            asyncio.run(PKCS11Session.verify(imported_key_label, data_to_be_signed, signature, key_type="secp256r1"))
+            asyncio.run(PKCS11Session().verify(imported_key_label, data_to_be_signed, signature, key_type="secp256r1"))
         )
         self.assertFalse(
             asyncio.run(
-                PKCS11Session.verify(
+                PKCS11Session().verify(
                     imported_key_label, data_to_be_signed, b"NOT VALID SIGNATURE HERE", key_type="secp256r1"
                 )
             )
         )
 
         # Delete the test key
-        asyncio.run(PKCS11Session.delete_keypair(imported_key_label, key_type="secp256r1"))
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label, key_type="secp256r1"))
+        asyncio.run(PKCS11Session().delete_keypair(imported_key_label, key_type="secp256r1"))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label, key_type="secp256r1"))
 
     def test_import_keypair_secp384r1(self) -> None:
         """Import keypair with key_label in the PKCS11 device.
 
         openssl ecparam -name secp384r1 -genkey -noout -out private.pem
         openssl ec -in private.pem -outform DER -out private.key
         openssl ec -in private.pem -pubout -out public.pem
         openssl ec -in private.pem -pubout -outform DER -out public.key
 
         """
 
         priv = b'0\x81\xa4\x02\x01\x01\x040:-e\x12#\xab\xcb\xa3v\xfd\xc5\xe2W\x87\x82\x17\x1d\x7f\xbcg\x92\x7f\xc9\xe0G\xdde\x9e0\xf6\x00\x97\xcc\xda\x04\xa0\xda\xf9\x13\x86\x8e7x^\xa8\xbe\xd8\xd7\xa0\x07\x06\x05+\x81\x04\x00"\xa1d\x03b\x00\x04>\x11_\x9f\xb6z\xe6\xdc\xfc\xa7\x1a]\x02\x82\xbe\xdfh\xee\xca\xa6\xd6\xd9\x84\x87[m\x15\x11\xa7\xbea\x94<\x07!\xcb%7\xedFv\xaa\xe0\xf6\x9b\x9c\x00Bo\x1c\xc8\n\x8a\x86\xf6\x82\x15\xf5\x0e\xb98\xdf\x9f+\xb4\xfdG\x17\xc0O$a\xedz-\xc1[\xf1\xa5\xab\t\x1a\xdb>\x9d\xf5^\xb0 ,\xe4A\x9e\xfb\x17e'  # pylint: disable=C0301
         pub = b'0v0\x10\x06\x07*\x86H\xce=\x02\x01\x06\x05+\x81\x04\x00"\x03b\x00\x04>\x11_\x9f\xb6z\xe6\xdc\xfc\xa7\x1a]\x02\x82\xbe\xdfh\xee\xca\xa6\xd6\xd9\x84\x87[m\x15\x11\xa7\xbea\x94<\x07!\xcb%7\xedFv\xaa\xe0\xf6\x9b\x9c\x00Bo\x1c\xc8\n\x8a\x86\xf6\x82\x15\xf5\x0e\xb98\xdf\x9f+\xb4\xfdG\x17\xc0O$a\xedz-\xc1[\xf1\xa5\xab\t\x1a\xdb>\x9d\xf5^\xb0 ,\xe4A\x9e\xfb\x17e'  # pylint: disable=C0301
 
-        imported_key_label = "imported_keypair_label_secp384r1"
-        new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        imported_key_label = "testpkcsimported_keypair_label_secp384r1"
+        new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
 
-        asyncio.run(PKCS11Session.create_keypair(new_key_label, key_type="secp384r1"))
-        pk_info, identifier = asyncio.run(PKCS11Session.public_key_data(new_key_label, "secp384r1"))
+        asyncio.run(PKCS11Session().create_keypair(new_key_label, key_type="secp384r1"))
+        pk_info, identifier = asyncio.run(PKCS11Session().public_key_data(new_key_label, "secp384r1"))
 
-        asyncio.run(PKCS11Session.import_keypair(pub, priv, imported_key_label, key_type="secp384r1"))
-        pk_info, identifier = asyncio.run(PKCS11Session.public_key_data(imported_key_label, key_type="secp384r1"))
+        asyncio.run(PKCS11Session().import_keypair(pub, priv, imported_key_label, key_type="secp384r1"))
+        pk_info, identifier = asyncio.run(PKCS11Session().public_key_data(imported_key_label, key_type="secp384r1"))
         self.assertTrue(isinstance(identifier, bytes))
         self.assertTrue(identifier == b"\xa9\x7f\xe5\x14\xcb\x08\x13\xc6\x18\xf7\xae\t\x8e0\xfc$v\x13\xc8A")
         self.assertTrue(isinstance(pk_info, str))
 
-        self.assertTrue(imported_key_label in asyncio.run(PKCS11Session.key_labels()))
-        self.assertTrue(asyncio.run(PKCS11Session.key_labels())[imported_key_label] == "secp384r1")
+        self.assertTrue(imported_key_label in asyncio.run(PKCS11Session().key_labels()))
+        self.assertTrue(asyncio.run(PKCS11Session().key_labels())[imported_key_label] == "secp384r1")
         with self.assertRaises(MultipleObjectsReturned):
             asyncio.run(
-                PKCS11Session.import_keypair(
+                PKCS11Session().import_keypair(
                     pub,
                     priv,
                     imported_key_label,
                     "secp384r1",
                 )
             )
 
         data_to_be_signed = b"MY TEST DATA TO BE SIGNED HERE"
 
         signature = asyncio.run(
-            PKCS11Session.sign(imported_key_label, data_to_be_signed, verify_signature=True, key_type="secp384r1")
+            PKCS11Session().sign(imported_key_label, data_to_be_signed, verify_signature=True, key_type="secp384r1")
         )
         self.assertTrue(isinstance(signature, bytes))
 
         self.assertTrue(
-            asyncio.run(PKCS11Session.verify(imported_key_label, data_to_be_signed, signature, key_type="secp384r1"))
+            asyncio.run(PKCS11Session().verify(imported_key_label, data_to_be_signed, signature, key_type="secp384r1"))
         )
         self.assertFalse(
             asyncio.run(
-                PKCS11Session.verify(
+                PKCS11Session().verify(
                     imported_key_label, data_to_be_signed, b"NOT VALID SIGNATURE HERE", key_type="secp384r1"
                 )
             )
         )
 
         # Delete the test keys
-        asyncio.run(PKCS11Session.delete_keypair(imported_key_label, key_type="secp384r1"))
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label, key_type="secp384r1"))
+        asyncio.run(PKCS11Session().delete_keypair(imported_key_label, key_type="secp384r1"))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label, key_type="secp384r1"))
 
     def test_import_keypair_secp521r1(self) -> None:
         """Import keypair with key_label in the PKCS11 device.
 
         openssl ecparam -name secp521r1 -genkey -noout -out private.pem
         openssl ec -in private.pem -outform DER -out private.key
         openssl ec -in private.pem -pubout -out public.pem
         openssl ec -in private.pem -pubout -outform DER -out public.key
 
         """
 
         with self.assertRaises(ValueError):
-            asyncio.run(PKCS11Session.import_keypair(b"dummy", b"dummy_data", "dummy", key_type="dummy_key_type"))
+            asyncio.run(PKCS11Session().import_keypair(b"dummy", b"dummy_data", "dummy", key_type="dummy_key_type"))
 
         priv = b'0\x81\xdc\x02\x01\x01\x04B\x00T\xc7"\xc9&\xdb\xe8e\xb8\xf6\xb0\x8c\xd4\xd0\xc0\xbc\xf8\xd8?g\x17Bb:\xeeI\x86\xe6\x86\xb25W\x12\xa9F\x00\xbf\xee\xd7\xb7\xb5}\x9b]\x1a\xce\x97U\x05\x0cX\x19c\x1b\'?i\x94s0,\x175\xfe\x88\xa0\x07\x06\x05+\x81\x04\x00#\xa1\x81\x89\x03\x81\x86\x00\x04\x01\x04\x95"\xe0"\xc6g\xee\xa2:\\\xd9\xa0\x8f\xfa\xad\x07\xeco\t\xa7\x00~3}1\x949\x83\xef\x16-T\x1c\x90\x96) \x8e\x16\xa3\xc1\xd7\xcb\xa0I?\xdf\x07\x8e\xa0\xb8\x82F\xf0\x15\xaf4\x9d\xbb\xd7\xb85\xce\xd4\x01\xc6`\xbd?\xfc]\xa1\x18\x8c\xb9\xb8Z\x10\xb6\x9a&\xa9[\xc9{\xf9\x99\xcc\xe5\xb6\x80!R\xd6(\xa0\x08\xda%\xd45\x0ec[\x87^\xfa\xf7;\x10\t\x95\xbcf\xf1\x97\xd9B7\t\xb6w\x0ce\xec\x81\xe4\xd6~T'  # pylint: disable=C0301
         pub = b'0\x81\x9b0\x10\x06\x07*\x86H\xce=\x02\x01\x06\x05+\x81\x04\x00#\x03\x81\x86\x00\x04\x01\x04\x95"\xe0"\xc6g\xee\xa2:\\\xd9\xa0\x8f\xfa\xad\x07\xeco\t\xa7\x00~3}1\x949\x83\xef\x16-T\x1c\x90\x96) \x8e\x16\xa3\xc1\xd7\xcb\xa0I?\xdf\x07\x8e\xa0\xb8\x82F\xf0\x15\xaf4\x9d\xbb\xd7\xb85\xce\xd4\x01\xc6`\xbd?\xfc]\xa1\x18\x8c\xb9\xb8Z\x10\xb6\x9a&\xa9[\xc9{\xf9\x99\xcc\xe5\xb6\x80!R\xd6(\xa0\x08\xda%\xd45\x0ec[\x87^\xfa\xf7;\x10\t\x95\xbcf\xf1\x97\xd9B7\t\xb6w\x0ce\xec\x81\xe4\xd6~T'  # pylint: disable=C0301
 
-        imported_key_label = "imported_keypair_label_secp521r1"
-        new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        imported_key_label = "testpkcsimported_keypair_label_secp521r1"
+        new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
 
-        asyncio.run(PKCS11Session.create_keypair(new_key_label, key_type="secp521r1"))
-        pk_info, identifier = asyncio.run(PKCS11Session.public_key_data(new_key_label, "secp521r1"))
+        asyncio.run(PKCS11Session().create_keypair(new_key_label, key_type="secp521r1"))
+        pk_info, identifier = asyncio.run(PKCS11Session().public_key_data(new_key_label, "secp521r1"))
 
-        asyncio.run(PKCS11Session.import_keypair(pub, priv, imported_key_label, key_type="secp521r1"))
-        pk_info, identifier = asyncio.run(PKCS11Session.public_key_data(imported_key_label, key_type="secp521r1"))
+        asyncio.run(PKCS11Session().import_keypair(pub, priv, imported_key_label, key_type="secp521r1"))
+        pk_info, identifier = asyncio.run(PKCS11Session().public_key_data(imported_key_label, key_type="secp521r1"))
         self.assertTrue(isinstance(identifier, bytes))
         self.assertTrue(identifier == b"\x02\xf0\xdek\x85\x85\x80\x15\xc3H\xf4\xc5'/\xa4\x1a\x12\x0e\x9a\xd3")
         self.assertTrue(isinstance(pk_info, str))
 
-        self.assertTrue(imported_key_label in asyncio.run(PKCS11Session.key_labels()))
-        self.assertTrue(asyncio.run(PKCS11Session.key_labels())[imported_key_label] == "secp521r1")
+        self.assertTrue(imported_key_label in asyncio.run(PKCS11Session().key_labels()))
+        self.assertTrue(asyncio.run(PKCS11Session().key_labels())[imported_key_label] == "secp521r1")
         with self.assertRaises(MultipleObjectsReturned):
             asyncio.run(
-                PKCS11Session.import_keypair(
+                PKCS11Session().import_keypair(
                     pub,
                     priv,
                     imported_key_label,
                     "secp521r1",
                 )
             )
 
         data_to_be_signed = b"MY TEST DATA TO BE SIGNED HERE"
         signature = asyncio.run(
-            PKCS11Session.sign(imported_key_label, data_to_be_signed, verify_signature=True, key_type="secp521r1")
+            PKCS11Session().sign(imported_key_label, data_to_be_signed, verify_signature=True, key_type="secp521r1")
         )
         self.assertTrue(isinstance(signature, bytes))
 
         self.assertTrue(
-            asyncio.run(PKCS11Session.verify(imported_key_label, data_to_be_signed, signature, key_type="secp521r1"))
+            asyncio.run(PKCS11Session().verify(imported_key_label, data_to_be_signed, signature, key_type="secp521r1"))
         )
         self.assertFalse(
             asyncio.run(
-                PKCS11Session.verify(
+                PKCS11Session().verify(
                     imported_key_label, data_to_be_signed, b"NOT VALID SIGNATURE HERE", key_type="secp521r1"
                 )
             )
         )
 
         # Delete the test key
-        asyncio.run(PKCS11Session.delete_keypair(imported_key_label, key_type="secp521r1"))
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label, key_type="secp521r1"))
+        asyncio.run(PKCS11Session().delete_keypair(imported_key_label, key_type="secp521r1"))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label, key_type="secp521r1"))
 
     def test_create_keypair(self) -> None:
         """Create keypair with key_label in the PKCS11 device."""
 
         with self.assertRaises(ValueError):
-            asyncio.run(PKCS11Session.create_keypair("dummy", key_type="dummy_key_type"))
+            asyncio.run(PKCS11Session().create_keypair("dummy", key_type="dummy_key_type"))
 
-        new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
-        asyncio.run(PKCS11Session.create_keypair(new_key_label, key_type="rsa_2048"))
-        pk_info, identifier = asyncio.run(PKCS11Session.public_key_data(new_key_label, key_type="rsa_2048"))
+        new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        asyncio.run(PKCS11Session().create_keypair(new_key_label, key_type="rsa_2048"))
+        pk_info, identifier = asyncio.run(PKCS11Session().public_key_data(new_key_label, key_type="rsa_2048"))
         self.assertTrue(isinstance(identifier, bytes))
         self.assertTrue(isinstance(pk_info, str))
 
         with self.assertRaises(MultipleObjectsReturned):
-            asyncio.run(PKCS11Session.create_keypair(new_key_label, key_type="rsa_2048"))
-            pk_info, identifier = asyncio.run(PKCS11Session.public_key_data(new_key_label, key_type="rsa_2048"))
+            asyncio.run(PKCS11Session().create_keypair(new_key_label, key_type="rsa_2048"))
+            pk_info, identifier = asyncio.run(PKCS11Session().public_key_data(new_key_label, key_type="rsa_2048"))
 
-        asyncio.run(PKCS11Session.create_keypair(new_key_label[:-1], key_type="rsa_2048"))
-        pk_info2, identifier2 = asyncio.run(PKCS11Session.public_key_data(new_key_label[:-1], key_type="rsa_2048"))
+        asyncio.run(PKCS11Session().create_keypair(new_key_label[:-1], key_type="rsa_2048"))
+        pk_info2, identifier2 = asyncio.run(PKCS11Session().public_key_data(new_key_label[:-1], key_type="rsa_2048"))
         self.assertTrue(isinstance(identifier2, bytes))
         self.assertTrue(isinstance(pk_info2, str))
 
         self.assertTrue(identifier != identifier2)
         self.assertTrue(pk_info != pk_info2)
 
-        asyncio.run(PKCS11Session.create_keypair(new_key_label[:-2], key_type="rsa_4096"))
-        pk_info2, identifier2 = asyncio.run(PKCS11Session.public_key_data(new_key_label[:-2], key_type="rsa_4096"))
+        asyncio.run(PKCS11Session().create_keypair(new_key_label[:-2], key_type="rsa_4096"))
+        pk_info2, identifier2 = asyncio.run(PKCS11Session().public_key_data(new_key_label[:-2], key_type="rsa_4096"))
         self.assertTrue(isinstance(identifier2, bytes))
         self.assertTrue(isinstance(pk_info2, str))
 
         # Test key_labels
-        pk_info3, identifier3 = asyncio.run(PKCS11Session.create_keypair(new_key_label[:-3], key_type="rsa_4096"))
-        key_labels = asyncio.run(PKCS11Session.key_labels())
+        pk_info3, identifier3 = asyncio.run(PKCS11Session().create_keypair(new_key_label[:-3], key_type="rsa_4096"))
+        key_labels = asyncio.run(PKCS11Session().key_labels())
         self.assertTrue(isinstance(key_labels, dict))
         self.assertTrue(len(key_labels) > 0)
         for label in key_labels:
             self.assertTrue(isinstance(label, str))
         self.assertTrue(new_key_label[:-3] in key_labels)
         self.assertFalse("should_not_exists_1232353523" in key_labels)
 
-        pk_info3_1, identifier3_1 = asyncio.run(PKCS11Session.public_key_data(new_key_label[:-3], key_type="rsa_4096"))
+        pk_info3_1, identifier3_1 = asyncio.run(
+            PKCS11Session().public_key_data(new_key_label[:-3], key_type="rsa_4096")
+        )
         self.assertTrue(pk_info3 == pk_info3_1)
         self.assertTrue(identifier3 == identifier3_1)
 
         # Delete the test keys
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label, key_type="rsa_4096"))
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label[:-1], key_type="rsa_4096"))
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label[:-2], key_type="rsa_4096"))
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label[:-3], key_type="rsa_4096"))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label, key_type="rsa_4096"))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label[:-1], key_type="rsa_4096"))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label[:-2], key_type="rsa_4096"))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label[:-3], key_type="rsa_4096"))
 
     def test_delete_keypair(self) -> None:
         """
         Delete keypair with key_label in the PKCS11 device.
         """
 
         with self.assertRaises(ValueError):
-            asyncio.run(PKCS11Session.delete_keypair("dummy", key_type="dummy_key_type"))
+            asyncio.run(PKCS11Session().delete_keypair("dummy", key_type="dummy_key_type"))
 
-        for key_type in key_types:
-            new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        for key_type in KEYTYPES:
+            new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
 
             with self.assertRaises(NoSuchKey):
-                asyncio.run(PKCS11Session.delete_keypair(new_key_label, key_type=key_type))
+                asyncio.run(PKCS11Session().delete_keypair(new_key_label, key_type=key_type))
 
-            asyncio.run(PKCS11Session.create_keypair(new_key_label, key_type=key_type))
-            asyncio.run(PKCS11Session.delete_keypair(new_key_label, key_type=key_type))
+            asyncio.run(PKCS11Session().create_keypair(new_key_label, key_type=key_type))
+            asyncio.run(PKCS11Session().delete_keypair(new_key_label, key_type=key_type))
 
             with self.assertRaises(NoSuchKey):
-                _, _ = asyncio.run(PKCS11Session.public_key_data(new_key_label, key_type=key_type))
+                _, _ = asyncio.run(PKCS11Session().public_key_data(new_key_label, key_type=key_type))
 
     def test_get_public_key_data(self) -> None:
         """
         Get key identifier from public key with key_label in the PKCS11 device.
         """
 
         with self.assertRaises(ValueError):
-            asyncio.run(PKCS11Session.public_key_data("dummy", key_type="dummy_key_type"))
+            asyncio.run(PKCS11Session().public_key_data("dummy", key_type="dummy_key_type"))
 
-        for key_type in key_types:
-            new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
-            asyncio.run(PKCS11Session.create_keypair(new_key_label, key_type=key_type))
-            pk_info, identifier = asyncio.run(PKCS11Session.public_key_data(new_key_label, key_type=key_type))
+        for key_type in KEYTYPES:
+            new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
+            asyncio.run(PKCS11Session().create_keypair(new_key_label, key_type=key_type))
+            pk_info, identifier = asyncio.run(PKCS11Session().public_key_data(new_key_label, key_type=key_type))
             self.assertTrue(isinstance(identifier, bytes))
             self.assertTrue(isinstance(pk_info, str))
 
             with self.assertRaises(NoSuchKey):
-                _, _ = asyncio.run(PKCS11Session.public_key_data(new_key_label[:-2], key_type=key_type))
+                _, _ = asyncio.run(PKCS11Session().public_key_data(new_key_label[:-2], key_type=key_type))
 
             # Delete the test key
-            asyncio.run(PKCS11Session.delete_keypair(new_key_label, key_type=key_type))
+            asyncio.run(PKCS11Session().delete_keypair(new_key_label, key_type=key_type))
 
     def test_sign_and_verify_data_rsa(self) -> None:
         """
         Sign bytes with key_label in the PKCS11 device.
         """
 
         with self.assertRaises(ValueError):
-            asyncio.run(PKCS11Session.sign("dummy", b"dummy_data", key_type="dummy_key_type"))
+            asyncio.run(PKCS11Session().sign("dummy", b"dummy_data", key_type="dummy_key_type"))
 
         with self.assertRaises(ValueError):
-            asyncio.run(PKCS11Session.verify("dummy", b"dummy_data", b"dummy_sig", key_type="dummy_key_type"))
+            asyncio.run(PKCS11Session().verify("dummy", b"dummy_data", b"dummy_sig", key_type="dummy_key_type"))
 
-        new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
-        asyncio.run(PKCS11Session.create_keypair(new_key_label, key_type="rsa_2048"))
+        new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        asyncio.run(PKCS11Session().create_keypair(new_key_label, key_type="rsa_2048"))
         data_to_be_signed = b"MY TEST DATA TO BE SIGNED HERE"
 
-        signature = asyncio.run(PKCS11Session.sign(new_key_label, data_to_be_signed, key_type="rsa_2048"))
+        signature = asyncio.run(PKCS11Session().sign(new_key_label, data_to_be_signed, key_type="rsa_2048"))
         self.assertTrue(isinstance(signature, bytes))
 
-        signature = asyncio.run(PKCS11Session.sign(new_key_label, data_to_be_signed, key_type="rsa_2048"))
+        signature = asyncio.run(PKCS11Session().sign(new_key_label, data_to_be_signed, key_type="rsa_2048"))
         self.assertTrue(isinstance(signature, bytes))
 
         self.assertTrue(
-            asyncio.run(PKCS11Session.verify(new_key_label, data_to_be_signed, signature, key_type="rsa_2048"))
+            asyncio.run(PKCS11Session().verify(new_key_label, data_to_be_signed, signature, key_type="rsa_2048"))
         )
 
         self.assertFalse(
             asyncio.run(
-                PKCS11Session.verify(new_key_label, data_to_be_signed, b"NOT VALID SIGNATURE HERE", key_type="rsa_2048")
+                PKCS11Session().verify(
+                    new_key_label, data_to_be_signed, b"NOT VALID SIGNATURE HERE", key_type="rsa_2048"
+                )
             )
         )
 
         self.assertFalse(
             asyncio.run(
-                PKCS11Session.verify(
+                PKCS11Session().verify(
                     new_key_label,
                     data_to_be_signed,
                     b"NOT VALID SIGNATURE HERE",
                     key_type="rsa_2048",
                 )
             )
         )
 
         # Delete the test key
-        asyncio.run(PKCS11Session.delete_keypair(new_key_label, key_type="rsa_2048"))
+        asyncio.run(PKCS11Session().delete_keypair(new_key_label, key_type="rsa_2048"))
 
     def test_import_export_delete_cert(self) -> None:
         """
         Import, export and delete cert to and from the PKCS11 device.
         """
 
         cert_pem = """-----BEGIN CERTIFICATE-----
@@ -585,20 +607,20 @@
 mV72a3xICxRafOrsOyfYY/3xpdocJynYr5TBvXDWDmGRKz+9vlUUCazHMlLxxK9W
 owuSqWzudPixJNEFnjUXloAafbP1NU+HnVOG2daJqyVpSaiCTyjsK1iJ6hWWMu+g
 Z0C3qdoke9EvHCcwjbvJ8U5Bq5obD8D7nxSKIt/eEjSpqfhdOU3xC98uFxl6709v
 tnmQdMO1DA==
 -----END CERTIFICATE-----
 """
 
-        new_key_label = hex(int.from_bytes(os.urandom(20), "big") >> 1)
-        asyncio.run(PKCS11Session.import_certificate(cert_pem, new_key_label))
+        new_key_label = "testpkcs" + hex(int.from_bytes(os.urandom(20), "big") >> 1)
+        asyncio.run(PKCS11Session().import_certificate(cert_pem, new_key_label))
         with self.assertRaises(ValueError):
-            asyncio.run(PKCS11Session.import_certificate(cert_pem, new_key_label))
+            asyncio.run(PKCS11Session().import_certificate(cert_pem, new_key_label))
 
-        cert = asyncio.run(PKCS11Session.export_certificate(new_key_label))
+        cert = asyncio.run(PKCS11Session().export_certificate(new_key_label))
 
         self.assertTrue(isinstance(cert, str) and len(cert) > 0)
         self.assertTrue(cert_pem == cert)
 
-        asyncio.run(PKCS11Session.delete_certificate(new_key_label))
+        asyncio.run(PKCS11Session().delete_certificate(new_key_label))
         with self.assertRaises(ValueError):
-            asyncio.run(PKCS11Session.export_certificate(new_key_label))
+            asyncio.run(PKCS11Session().export_certificate(new_key_label))
```

### Comparing `python_x509_pkcs11-0.8.4/PKG-INFO` & `python_x509_pkcs11-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: python_x509_pkcs11
-Version: 0.8.4
+Version: 0.9.0
 Summary: Python async library for signing x509 using keys in a pkcs11 device such as an HSM.
-Home-page: https://github.com/SUNET/python_x509_pkcs11
-License: MIT
-Keywords: x509,pkcs11,HSM
-Author: Victor Näslund
-Author-email: victor@sunet.se
+Author-email: Victor Näslund <victor@sunet.se>, Magnus Svensson <masv@sunet.se>, Kushal Das <kushal@sunet.se>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: asn1crypto>=1.5.1
 Requires-Dist: python-pkcs11>=0.7.0
 Requires-Dist: aiohttp
+Requires-Dist: cryptography >= 40.0
+Project-URL: Source, https://github.com/SUNET/python_x509_pkcs11
 
 ![workflow ubuntu](https://github.com/SUNET/python_x509_pkcs11/actions/workflows/ubuntu.yaml/badge.svg)
 ![workflow centos](https://github.com/SUNET/python_x509_pkcs11/actions/workflows/centos.yaml/badge.svg)
 ![workflow debian](https://github.com/SUNET/python_x509_pkcs11/actions/workflows/debian.yaml/badge.svg)
 
 ## python_x509_pkcs11
```

