# Comparing `tmp/keystone-25.0.0.tar.gz` & `tmp/keystone-25.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keystone-25.0.0.tar", last modified: Wed Apr  3 11:52:09 2024, max compression
+gzip compressed data, was "keystone-25.0.0.0rc1.tar", last modified: Tue Mar 19 10:21:05 2024, max compression
```

## Comparing `keystone-25.0.0.tar` & `keystone-25.0.0.0rc1.tar`

### file list

```diff
@@ -1,1675 +1,1675 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.781974 keystone-25.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2024-04-03 11:51:37.000000 keystone-25.0.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1443 2024-04-03 11:51:37.000000 keystone-25.0.0/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2024-04-03 11:51:37.000000 keystone-25.0.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7390 2024-04-03 11:51:37.000000 keystone-25.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28905 2024-04-03 11:52:09.000000 keystone-25.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      654 2024-04-03 11:51:37.000000 keystone-25.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   373799 2024-04-03 11:52:08.000000 keystone-25.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1645 2024-04-03 11:51:37.000000 keystone-25.0.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-04-03 11:51:37.000000 keystone-25.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3204 2024-04-03 11:52:09.781974 keystone-25.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1692 2024-04-03 11:51:37.000000 keystone-25.0.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.581973 keystone-25.0.0/api-ref/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.601973 keystone-25.0.0/api-ref/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6364 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.601973 keystone-25.0.0/api-ref/source/v2-ext/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v2-ext/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2884 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v2-ext/ksec2-admin.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1908 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v2-ext/parameters.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.581973 keystone-25.0.0/api-ref/source/v2-ext/samples/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.601973 keystone-25.0.0/api-ref/source/v2-ext/samples/OS-KSEC2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      471 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v2-ext/samples/OS-KSEC2/authenticate-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1079 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v2-ext/samples/OS-KSEC2/authenticate-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v2-ext/samples/OS-KSEC2/credentials-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      409 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v2-ext/samples/OS-KSEC2/credentialswithec2-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v2-ext/samples/OS-KSEC2/ec2Credentials-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v2-ext/samples/OS-KSEC2/ec2Credentials-show-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.605973 keystone-25.0.0/api-ref/source/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13614 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/application-credentials.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29782 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/authenticate-v3.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5565 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/credentials.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14543 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/domains-config-v3.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5875 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/domains.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7650 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/groups.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9664 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15807 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/inherit.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/os-pki.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    60655 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/parameters.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4442 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/policies.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8081 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/project-tags.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8419 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/projects.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5580 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/regions-v3.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26330 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/roles.inc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.585973 keystone-25.0.0/api-ref/source/v3/samples/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.633973 keystone-25.0.0/api-ref/source/v3/samples/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/access-rule-get-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/access-rules-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      488 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/application-credential-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      820 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/application-credential-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      789 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/application-credential-get-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1978 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/application-credential-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/auth-application-credential-id-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/auth-application-credential-name-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1951 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/auth-application-credential-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/auth-password-explicit-unscoped-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/auth-password-explicit-unscoped-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16630 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/auth-password-project-scoped-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/auth-password-system-scoped-request-with-domain.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/auth-password-unscoped-request-with-domain.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/auth-password-unscoped-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/auth-password-unscoped-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/auth-password-user-name-unscoped-response-HTTP.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/auth-token-explicit-unscoped-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/auth-token-scoped-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16627 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/auth-token-scoped-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/auth-token-unscoped-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/auth-token-unscoped-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      705 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/create-role-inferences-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/credential-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/credential-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/credential-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/credential-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/credential-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5789 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/credentials-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/domain-config-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/domain-config-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/domain-config-default-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/domain-config-group-default-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/domain-config-group-option-default-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/domain-config-group-option-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       45 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/domain-config-group-option-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/domain-config-group-option-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/domain-config-group-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/domain-config-group-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/domain-config-group-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/domain-config-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/domain-config-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/domain-config-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/domain-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/domain-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/domain-group-roles-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/domain-group-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/domain-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/domain-specific-role-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/domain-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      294 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/domain-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      549 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/domain-user-roles-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/domains-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/endpoint-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/endpoint-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      427 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/endpoint-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/endpoint-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/endpoint-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12873 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/endpoints-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      719 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/get-available-domain-scopes-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      678 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/get-available-project-scopes-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/get-available-system-scopes-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      705 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/get-role-inferences-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1042 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/get-service-catalog-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/group-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/group-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      573 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/group-roles-domain-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/group-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/group-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/group-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      922 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/group-users-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      802 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/groups-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      443 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/identity-version-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1389 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/identity-versions-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/limit-flat-model-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      461 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/limit-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      589 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/limits-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1095 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/limits-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1221 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/limits-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/limits-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      531 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/limits-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1000 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/list-implied-roles-for-role-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/list-system-roles-for-group-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      463 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/list-system-roles-for-user-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/policies-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/policy-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/policy-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/policy-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/policy-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/policy-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/project-create-domain-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/project-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/project-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/project-enable-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      551 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/project-group-roles-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      736 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/project-show-parents-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/project-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1584 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/project-show-subtree-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/project-tags-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/project-tags-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      524 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/project-tags-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/project-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/project-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/project-user-roles-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3628 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/projects-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/region-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/region-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/region-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/region-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/region-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/regions-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/registered-limit-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      430 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/registered-limits-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      895 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/registered-limits-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1032 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/registered-limits-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/registered-limits-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/registered-limits-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2224 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/role-assignments-effective-list-include-names-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1109 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/role-assignments-effective-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/role-assignments-effective-list-response.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1261 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/role-assignments-list-include-subtree-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1009 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/role-assignments-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/role-assignments-list-response.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/role-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/role-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2316 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/role-inferences-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/role-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/role-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/role-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1792 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/roles-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/service-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/service-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/service-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/service-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/service-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3332 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/services-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/token-validate-request.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/user-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/user-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      894 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/user-groups-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/user-password-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      876 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/user-projects-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      572 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/user-roles-domain-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      352 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/user-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/user-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      438 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/user-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4849 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/admin/users-list-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.585973 keystone-25.0.0/api-ref/source/v3/samples/auth/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.637973 keystone-25.0.0/api-ref/source/v3/samples/auth/requests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/auth/requests/domain-id-password.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/auth/requests/domain-id-token.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/auth/requests/domain-name-password.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/auth/requests/domain-name-token.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/auth/requests/project-id-password.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/auth/requests/project-id-token.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/auth/requests/project-id-totp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/auth/requests/project-name-password.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/auth/requests/project-name-token.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/auth/requests/system-password.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/auth/requests/system-token.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.637973 keystone-25.0.0/api-ref/source/v3/samples/auth/responses/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/auth/responses/auth-receipt-password.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1962 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/auth/responses/domain-scoped-password.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2021 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/auth/responses/domain-scoped-token.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2140 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/auth/responses/project-scoped-password-totp.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2120 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/auth/responses/project-scoped-password.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2179 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/auth/responses/project-scoped-token.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1928 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/auth/responses/system-scoped-password.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1987 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/auth/responses/system-scoped-token.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/samples/auth/responses/unscoped-password.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9456 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/service-catalog.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2169 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/status.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7335 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/system-roles.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12106 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/unified_limits.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8523 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3/users.inc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.605973 keystone-25.0.0/api-ref/source/v3-ext/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9668 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/endpoint-policy.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15901 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/ep-filter.inc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.585973 keystone-25.0.0/api-ref/source/v3-ext/federation/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.605973 keystone-25.0.0/api-ref/source/v3-ext/federation/assertion/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3675 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/assertion/assertion.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      549 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/assertion/parameters.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.605973 keystone-25.0.0/api-ref/source/v3-ext/federation/assertion/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/assertion/samples/ecp-saml-assertion-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5648 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/assertion/samples/ecp-saml-assertion-response.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1249 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/assertion/samples/metadata-response.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/assertion/samples/saml-assertion-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4602 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/assertion/samples/saml-assertion-response.xml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.605973 keystone-25.0.0/api-ref/source/v3-ext/federation/auth/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3975 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/auth/auth.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      979 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/auth/parameters.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.605973 keystone-25.0.0/api-ref/source/v3-ext/federation/auth/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/auth/samples/scoped-token-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2236 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/auth/samples/scoped-token-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/auth/samples/unscoped-token-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.605973 keystone-25.0.0/api-ref/source/v3-ext/federation/identity-provider/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9425 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/identity-provider/idp.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2148 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/identity-provider/parameters.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.609973 keystone-25.0.0/api-ref/source/v3-ext/federation/identity-provider/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/identity-provider/samples/add-protocol-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/identity-provider/samples/add-protocol-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/identity-provider/samples/get-protocol-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      477 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/identity-provider/samples/get-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      535 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/identity-provider/samples/list-protocol-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1154 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/identity-provider/samples/list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/identity-provider/samples/register-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/identity-provider/samples/register-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/identity-provider/samples/update-protocol-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/identity-provider/samples/update-protocol-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/identity-provider/samples/update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      466 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/identity-provider/samples/update-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.609973 keystone-25.0.0/api-ref/source/v3-ext/federation/mapping/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3340 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/mapping/mapping.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/mapping/parameters.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.609973 keystone-25.0.0/api-ref/source/v3-ext/federation/mapping/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      795 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/mapping/samples/create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      928 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/mapping/samples/create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      928 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/mapping/samples/get-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1227 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/mapping/samples/list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/mapping/samples/update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/mapping/samples/update-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.609973 keystone-25.0.0/api-ref/source/v3-ext/federation/projects-domains/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/projects-domains/parameters.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2055 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/projects-domains/projects-domains.inc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.609973 keystone-25.0.0/api-ref/source/v3-ext/federation/projects-domains/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/projects-domains/samples/domain-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      691 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/projects-domains/samples/project-list-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.609973 keystone-25.0.0/api-ref/source/v3-ext/federation/service-provider/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1257 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/service-provider/parameters.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.613973 keystone-25.0.0/api-ref/source/v3-ext/federation/service-provider/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/service-provider/samples/get-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1233 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/service-provider/samples/list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/service-provider/samples/register-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/service-provider/samples/register-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/service-provider/samples/update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/service-provider/samples/update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4217 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation/service-provider/sp.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9975 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/federation.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1031 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13878 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/oauth.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2983 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/oauth2.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15562 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/parameters.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2205 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/revoke.inc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.585973 keystone-25.0.0/api-ref/source/v3-ext/samples/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.613973 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-ENDPOINT-POLICY/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      878 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-ENDPOINT-POLICY/policy-endpoint-associations-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-ENDPOINT-POLICY/policy-show-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.613973 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-EP-FILTER/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-EP-FILTER/create-endpoint-group-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      369 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-EP-FILTER/endpoint-group-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1119 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-EP-FILTER/endpoint-groups-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-EP-FILTER/endpoint-project-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-EP-FILTER/list-associations-by-endpoint-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      814 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-EP-FILTER/list-associations-by-project-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1353 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-EP-FILTER/list-service-endpoints.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-EP-FILTER/update-endpoint-group-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-EP-FILTER/update-endpoint-group-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.613973 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-OAUTH1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-OAUTH1/access-token-create-response.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-OAUTH1/access-token-role-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-OAUTH1/access-token-roles-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      446 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-OAUTH1/access-token-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-OAUTH1/access-tokens-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-OAUTH1/authorize-request-token-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-OAUTH1/authorize-request-token-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-OAUTH1/consumer-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-OAUTH1/consumer-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-OAUTH1/consumer-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-OAUTH1/consumer-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-OAUTH1/consumer-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      549 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-OAUTH1/consumers-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-OAUTH1/request-token-create-response.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.613973 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-OAUTH2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-OAUTH2/token-create-request.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-OAUTH2/token-create-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.613973 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-REVOKE/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-REVOKE/list-revoke-response.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.613973 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-SIMPLE-CERT/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1223 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-SIMPLE-CERT/show-ca-certificate-response.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1187 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-SIMPLE-CERT/show-signing-certificate-response.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.613973 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-TRUST/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1332 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-TRUST/trust-auth-redelegated-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-TRUST/trust-auth-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1249 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-TRUST/trust-auth-trust-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-TRUST/trust-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      828 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-TRUST/trust-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      761 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-TRUST/trust-get-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-TRUST/trust-get-role-delegated-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      722 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-TRUST/trust-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/samples/OS-TRUST/trust-list-roles-delegated-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/simple-cert.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10061 2024-04-03 11:51:37.000000 keystone-25.0.0/api-ref/source/v3-ext/trust.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1099 2024-04-03 11:51:37.000000 keystone-25.0.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.637973 keystone-25.0.0/config-generator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2024-04-03 11:51:37.000000 keystone-25.0.0/config-generator/keystone-policy-generator.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2024-04-03 11:51:37.000000 keystone-25.0.0/config-generator/keystone.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.637973 keystone-25.0.0/devstack/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.585973 keystone-25.0.0/devstack/files/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.637973 keystone-25.0.0/devstack/files/federation/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3794 2024-04-03 11:51:37.000000 keystone-25.0.0/devstack/files/federation/attribute-map.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2024-04-03 11:51:37.000000 keystone-25.0.0/devstack/files/federation/shib_apache_alias.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2024-04-03 11:51:37.000000 keystone-25.0.0/devstack/files/federation/shib_apache_handler.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3769 2024-04-03 11:51:37.000000 keystone-25.0.0/devstack/files/federation/shibboleth2.xml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.637973 keystone-25.0.0/devstack/files/oidc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1601 2024-04-03 11:51:37.000000 keystone-25.0.0/devstack/files/oidc/apache_oidc.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.637973 keystone-25.0.0/devstack/lib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8634 2024-04-03 11:51:37.000000 keystone-25.0.0/devstack/lib/federation.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6524 2024-04-03 11:51:37.000000 keystone-25.0.0/devstack/lib/oidc.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1055 2024-04-03 11:51:37.000000 keystone-25.0.0/devstack/lib/scope.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3686 2024-04-03 11:51:37.000000 keystone-25.0.0/devstack/plugin.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.585973 keystone-25.0.0/devstack/tools/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.637973 keystone-25.0.0/devstack/tools/oidc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/devstack/tools/oidc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1180 2024-04-03 11:51:37.000000 keystone-25.0.0/devstack/tools/oidc/docker-compose.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1893 2024-04-03 11:51:37.000000 keystone-25.0.0/devstack/tools/oidc/setup_keycloak_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.637973 keystone-25.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5753 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/Makefile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.637973 keystone-25.0.0/doc/ext/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/ext/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      541 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.641973 keystone-25.0.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.641973 keystone-25.0.0/doc/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6258 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/_static/horizon-login-idp.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16334 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/_static/horizon-login-sp.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      638 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/_static/support-matrix.css
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.645973 keystone-25.0.0/doc/source/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3722 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/auth-totp.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/authentication-mechanisms.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5936 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/bootstrap.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7832 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/caching-layer.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3349 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/case-insensitive.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13760 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/cli-manage-projects-users-and-roles.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      684 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/configuration.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3177 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/configure-https.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23543 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/configure_tokenless_x509.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4430 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/credential-encryption.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9878 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/domain-specific-config.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      708 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/endpoint-filtering.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      543 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/endpoint-policy.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19951 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/event_notifications.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4176 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/external-authentication.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.649973 keystone-25.0.0/doc/source/admin/federation/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28362 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/federation/configure_federation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/federation/federated_identity.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20607 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/federation/introduction.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31809 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/federation/mapping_combinations.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5126 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/federation/mellon.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8872 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/federation/openidc.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8730 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/federation/shibboleth.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18579 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/fernet-token-faq.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.649973 keystone-25.0.0/doc/source/admin/figures/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    53211 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/figures/keystone-federation.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7680 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/figures/keystone-federation.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/getting-started.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      506 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/health-check-middleware.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14777 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/identity-concepts.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1370 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/identity-sources.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4202 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/identity-support-matrix.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18075 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/integrate-with-ldap.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3890 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/jws-key-rotation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/keystone-features.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1409 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/limit-list-size.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      703 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/logging.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10656 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/manage-services.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      964 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/manage-trusts.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3278 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/multi-factor-authentication.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      939 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/oauth1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5342 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/oauth2-usage-guide.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/operations.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3933 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/performance.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6815 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/resource-options.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7689 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/security-compliance.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21018 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/service-api-protection.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1711 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/token-provider.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4172 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/token-support-matrix.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6378 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/tokens-overview.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/tokens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      881 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/troubleshoot.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21157 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/unified-limits.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11932 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/upgrading.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1497 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/admin/url-safe-naming.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29677 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/api_curl_examples.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.649973 keystone-25.0.0/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1462 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/cli/commands.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      775 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/cli/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4921 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/cli/keystone-manage.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2925 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/cli/keystone-status.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/code_documentation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9276 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.649973 keystone-25.0.0/doc/source/configuration/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      781 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/configuration/config-options.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      590 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/configuration/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/configuration/policy.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.649973 keystone-25.0.0/doc/source/configuration/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/configuration/samples/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/configuration/samples/keystone-conf.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/configuration/samples/logging-conf.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/configuration/samples/policy-yaml.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.653973 keystone-25.0.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8334 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/contributor/api_change_tutorial.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      862 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/contributor/architecture.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3973 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/contributor/auth-plugins.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3660 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/contributor/caching-layer.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2908 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5037 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/contributor/database-migrations.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4188 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/contributor/developing-drivers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4855 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/contributor/doctor-checks.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2099 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/contributor/filtering-responsibilities.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5715 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/contributor/how-can-i-help.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8399 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/contributor/http-api.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1917 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/contributor/id-manage.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1169 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1545 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/contributor/list-truncation.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5583 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/contributor/programming-exercises.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5369 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/contributor/proposing-features.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4645 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/contributor/release-notes.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7517 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/contributor/service-catalog.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29640 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/contributor/services.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7613 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/contributor/set-up-keystone.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14953 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/contributor/testing-keystone.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6049 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/contributor/vision-reflection.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.653973 keystone-25.0.0/doc/source/getting-started/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17078 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/getting-started/architecture.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3588 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/getting-started/community.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/getting-started/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22156 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/getting-started/policy_mapping.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3124 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/indices-tables.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.657973 keystone-25.0.0/doc/source/install/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.657973 keystone-25.0.0/doc/source/install/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2794 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/install/common/get-started-identity.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4948 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/install/common/keystone-users.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3831 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/install/common/openrc.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       45 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/install/get-started-obs.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       45 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/install/get-started-rdo.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       45 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/install/get-started-ubuntu.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1339 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/install/index-obs.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1305 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/install/index-rdo.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1219 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/install/index-ubuntu.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/install/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6903 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/install/keystone-install-obs.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5627 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/install/keystone-install-rdo.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5576 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/install/keystone-install-ubuntu.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/install/keystone-openrc-obs.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/install/keystone-openrc-rdo.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/install/keystone-openrc-ubuntu.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/install/keystone-users-obs.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/install/keystone-users-rdo.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/install/keystone-users-ubuntu.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2817 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/install/keystone-verify-obs.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2817 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/install/keystone-verify-rdo.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2809 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/install/keystone-verify-ubuntu.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.657973 keystone-25.0.0/doc/source/install/shared/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/install/shared/note_configuration_vary_by_distribution.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.657973 keystone-25.0.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16821 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/user/application_credentials.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1065 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3637 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/user/json_home.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3579 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/user/multi-factor-authentication.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3416 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/user/supported_clients.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2647 2024-04-03 11:51:37.000000 keystone-25.0.0/doc/source/user/trusts.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.661973 keystone-25.0.0/etc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2024-04-03 11:51:37.000000 keystone-25.0.0/etc/README.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1929 2024-04-03 11:51:37.000000 keystone-25.0.0/etc/default_catalog.templates
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1046 2024-04-03 11:51:37.000000 keystone-25.0.0/etc/logging.conf.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2024-04-03 11:51:37.000000 keystone-25.0.0/etc/sso_callback_template.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.585973 keystone-25.0.0/examples/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.585973 keystone-25.0.0/examples/pki/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.661973 keystone-25.0.0/examples/pki/certs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1391 2024-04-03 11:51:37.000000 keystone-25.0.0/examples/pki/certs/cacert.pem
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3030 2024-04-03 11:51:37.000000 keystone-25.0.0/examples/pki/certs/middleware.pem
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1326 2024-04-03 11:51:37.000000 keystone-25.0.0/examples/pki/certs/signing_cert.pem
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1326 2024-04-03 11:51:37.000000 keystone-25.0.0/examples/pki/certs/ssl_cert.pem
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.661973 keystone-25.0.0/examples/pki/private/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1704 2024-04-03 11:51:37.000000 keystone-25.0.0/examples/pki/private/cakey.pem
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1704 2024-04-03 11:51:37.000000 keystone-25.0.0/examples/pki/private/signing_key.pem
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1704 2024-04-03 11:51:37.000000 keystone-25.0.0/examples/pki/private/ssl_key.pem
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.661973 keystone-25.0.0/httpd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2024-04-03 11:51:37.000000 keystone-25.0.0/httpd/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      623 2024-04-03 11:51:37.000000 keystone-25.0.0/httpd/keystone-uwsgi-admin.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      623 2024-04-03 11:51:37.000000 keystone-25.0.0/httpd/keystone-uwsgi-public.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2024-04-03 11:51:37.000000 keystone-25.0.0/httpd/uwsgi-keystone.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      991 2024-04-03 11:51:37.000000 keystone-25.0.0/httpd/wsgi-keystone.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.661973 keystone-25.0.0/keystone/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.669973 keystone-25.0.0/keystone/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2416 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.669973 keystone-25.0.0/keystone/api/_shared/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7776 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/_shared/EC2_S3_Resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      417 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/_shared/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10849 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/_shared/authentication.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1789 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/_shared/implied_roles.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3957 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/_shared/json_home_relations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2985 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/_shared/saml.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19701 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9096 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/credentials.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4259 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/discovery.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20181 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/domains.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3557 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/ec2tokens.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5862 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/endpoints.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8791 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5623 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13358 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/os_ep_filter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20143 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/os_federation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19007 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/os_inherit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14927 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/os_oauth1.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16161 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/os_oauth2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2912 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/os_revoke.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2164 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/os_simple_cert.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10810 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21741 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/projects.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3977 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/regions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3699 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/registered_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16163 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/role_assignments.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2482 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/role_inferences.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12263 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/roles.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4397 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/s3tokens.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2977 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7273 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/system.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20650 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/trusts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35853 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/api/users.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.669973 keystone-25.0.0/keystone/application_credential/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      605 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/application_credential/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.669973 keystone-25.0.0/keystone/application_credential/backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/application_credential/backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4607 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/application_credential/backends/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11735 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/application_credential/backends/sql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10648 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/application_credential/core.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2114 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/application_credential/schema.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.669973 keystone-25.0.0/keystone/assignment/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/assignment/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.669973 keystone-25.0.0/keystone/assignment/backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/assignment/backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7489 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/assignment/backends/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17315 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/assignment/backends/sql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    61208 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/assignment/core.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.673973 keystone-25.0.0/keystone/assignment/role_backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/assignment/role_backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4390 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/assignment/role_backends/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      990 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/assignment/role_backends/resource_options.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6568 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/assignment/role_backends/sql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4495 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/assignment/role_backends/sql_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1123 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/assignment/schema.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.673973 keystone-25.0.0/keystone/auth/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/auth/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23262 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/auth/core.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.673973 keystone-25.0.0/keystone/auth/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      619 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/auth/plugins/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1589 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/auth/plugins/application_credential.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3476 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/auth/plugins/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9800 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/auth/plugins/core.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3138 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/auth/plugins/external.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16678 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/auth/plugins/mapped.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2703 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/auth/plugins/oauth1.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1649 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/auth/plugins/password.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5084 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/auth/plugins/token.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4679 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/auth/plugins/totp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5875 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/auth/schema.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.677973 keystone-25.0.0/keystone/catalog/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      630 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/catalog/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.677973 keystone-25.0.0/keystone/catalog/backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/catalog/backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16696 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/catalog/backends/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27762 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/catalog/backends/sql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12360 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/catalog/backends/templated.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13944 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/catalog/core.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2929 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/catalog/schema.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.677973 keystone-25.0.0/keystone/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15015 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/cmd/bootstrap.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    57559 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/cmd/cli.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.677973 keystone-25.0.0/keystone/cmd/doctor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2739 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/cmd/doctor/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2089 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/cmd/doctor/caching.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2911 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/cmd/doctor/credential.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1093 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/cmd/doctor/database.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      934 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/cmd/doctor/debug.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1305 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/cmd/doctor/federation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5586 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/cmd/doctor/ldap.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2407 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/cmd/doctor/security_compliance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1548 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/cmd/doctor/tokens.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1784 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/cmd/doctor/tokens_fernet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6115 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/cmd/idutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1474 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/cmd/manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3905 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/cmd/status.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.681973 keystone-25.0.0/keystone/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1449 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/authorization.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.681973 keystone-25.0.0/keystone/common/cache/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      624 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/cache/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3758 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/cache/_context_cache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6149 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/cache/core.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2917 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4521 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/driver_hints.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11975 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/fernet_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4739 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/json_home.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1651 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/jwt_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7670 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5886 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/password_hashing.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.685973 keystone-25.0.0/keystone/common/policies/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3368 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2120 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/access_rule.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3170 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/access_token.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3510 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/application_credential.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2439 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3870 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3861 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/consumer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3892 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/credential.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4236 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/domain.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7657 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/domain_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3545 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/ec2_credential.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3748 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/endpoint.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9264 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/endpoint_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14576 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/grant.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8665 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4772 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/identity_provider.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6774 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/implied_role.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3097 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/limit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4290 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/mapping.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3867 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10380 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/policy_association.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10726 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/project.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5068 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/project_endpoint.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4224 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/protocol.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3787 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/region.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2570 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/registered_limit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1016 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/revoke_event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6992 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/role.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2934 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/role_assignment.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3730 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4587 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/service_provider.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2982 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/token.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1779 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/token_revocation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6836 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/trust.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5812 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/policies/user.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1753 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/profiler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4553 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/provider_api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.685973 keystone-25.0.0/keystone/common/rbac_enforcer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/rbac_enforcer/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22030 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/rbac_enforcer/enforcer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1254 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/rbac_enforcer/policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6050 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/render_token.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.685973 keystone-25.0.0/keystone/common/resource_options/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      601 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/resource_options/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9368 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/resource_options/core.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.685973 keystone-25.0.0/keystone/common/resource_options/options/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1284 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/resource_options/options/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2898 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/resource_options/options/immutable.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.689973 keystone-25.0.0/keystone/common/sql/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/sql/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2678 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/sql/alembic.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21420 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/sql/core.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.689973 keystone-25.0.0/keystone/common/sql/migrations/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      538 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/sql/migrations/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/sql/migrations/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4647 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/sql/migrations/autogen.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6570 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/sql/migrations/env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9026 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/sql/migrations/manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      976 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/sql/migrations/script.py.mako
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.689973 keystone-25.0.0/keystone/common/sql/migrations/versions/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.589973 keystone-25.0.0/keystone/common/sql/migrations/versions/2024.01/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.689973 keystone-25.0.0/keystone/common/sql/migrations/versions/2024.01/expand/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1100 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/sql/migrations/versions/2024.01/expand/47147121_add_identity_federation_attribute_mapping_schema_version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37329 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/sql/migrations/versions/27e647c0fad4_initial_version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/sql/migrations/versions/CONTRACT_HEAD
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/sql/migrations/versions/EXPAND_HEAD
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.589973 keystone-25.0.0/keystone/common/sql/migrations/versions/bobcat/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.689973 keystone-25.0.0/keystone/common/sql/migrations/versions/bobcat/contract/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1174 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/sql/migrations/versions/bobcat/contract/99de3849d860_fix_incorrect_constraints.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3019 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/sql/migrations/versions/bobcat/contract/c88cdce8f248_remove_duplicate_constraints.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.689973 keystone-25.0.0/keystone/common/sql/migrations/versions/bobcat/expand/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1063 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/sql/migrations/versions/bobcat/expand/11c3b243b4cb_remove_service_provider_relay_state_server_default.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1199 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/sql/migrations/versions/bobcat/expand/b4f8b3f584e0_fix_incorrect_constraints.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.589973 keystone-25.0.0/keystone/common/sql/migrations/versions/yoga/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.689973 keystone-25.0.0/keystone/common/sql/migrations/versions/yoga/contract/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/sql/migrations/versions/yoga/contract/e25ffa003242_initial.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.689973 keystone-25.0.0/keystone/common/sql/migrations/versions/yoga/expand/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/sql/migrations/versions/yoga/expand/29e87d24a316_initial.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10417 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/sql/upgrades.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7913 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/tokenless_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19560 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.689973 keystone-25.0.0/keystone/common/validation/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2344 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/validation/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2085 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/validation/parameter_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3818 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/common/validation/validators.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.693973 keystone-25.0.0/keystone/conf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5589 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1894 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/application_credential.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1375 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/assignment.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4252 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2403 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/catalog.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      925 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2993 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/credential.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5921 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/default.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1632 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/domain_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1588 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/endpoint_filter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1103 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/endpoint_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4727 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/federation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2966 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/fernet_receipts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2918 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/fernet_tokens.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6804 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/identity.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2803 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/identity_mapping.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2352 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/jwt_tokens.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17273 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/ldap.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1856 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/oauth1.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1701 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/oauth2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2797 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1332 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2537 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/receipt.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3788 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1897 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/revoke.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1909 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/role.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5728 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/saml.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5875 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/security_compliance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1237 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/shadow_users.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5191 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/token.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2393 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/tokenless_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/totp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1714 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/trust.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2259 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/unified_limit.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1140 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1789 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/conf/wsgi.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.693973 keystone-25.0.0/keystone/credential/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/credential/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.697973 keystone-25.0.0/keystone/credential/backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/credential/backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3920 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/credential/backends/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4815 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/credential/backends/sql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10050 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/credential/core.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/credential/provider.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.697973 keystone-25.0.0/keystone/credential/providers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/credential/providers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1207 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/credential/providers/core.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.697973 keystone-25.0.0/keystone/credential/providers/fernet/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      610 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/credential/providers/fernet/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4647 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/credential/providers/fernet/core.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1643 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/credential/schema.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.697973 keystone-25.0.0/keystone/endpoint_policy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      598 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/endpoint_policy/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.697973 keystone-25.0.0/keystone/endpoint_policy/backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/endpoint_policy/backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5832 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/endpoint_policy/backends/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6182 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/endpoint_policy/backends/sql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11495 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/endpoint_policy/core.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27422 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/exception.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.697973 keystone-25.0.0/keystone/federation/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/federation/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.697973 keystone-25.0.0/keystone/federation/backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/federation/backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11146 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/federation/backends/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15934 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/federation/backends/sql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/federation/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7336 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/federation/core.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27804 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/federation/idp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4103 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/federation/schema.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37678 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/federation/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      878 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.697973 keystone-25.0.0/keystone/identity/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      679 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/identity/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.701974 keystone-25.0.0/keystone/identity/backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/identity/backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13955 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/identity/backends/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.701974 keystone-25.0.0/keystone/identity/backends/ldap/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      605 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/identity/backends/ldap/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    81249 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/identity/backends/ldap/common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18497 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/identity/backends/ldap/core.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1614 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/identity/backends/ldap/models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5086 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/identity/backends/resource_options.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19701 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/identity/backends/sql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18510 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/identity/backends/sql_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    72588 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/identity/core.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1581 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/identity/generator.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.701974 keystone-25.0.0/keystone/identity/id_generators/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/identity/id_generators/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1246 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/identity/id_generators/sha256.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.701974 keystone-25.0.0/keystone/identity/mapping_backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/identity/mapping_backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3388 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/identity/mapping_backends/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      640 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/identity/mapping_backends/mapping.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4771 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/identity/mapping_backends/sql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3792 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/identity/schema.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.701974 keystone-25.0.0/keystone/identity/shadow_backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/identity/shadow_backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5082 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/identity/shadow_backends/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10969 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/identity/shadow_backends/sql.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.701974 keystone-25.0.0/keystone/limit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      614 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/limit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.701974 keystone-25.0.0/keystone/limit/backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/limit/backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5766 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/limit/backends/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13015 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/limit/backends/sql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5818 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/limit/core.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.701974 keystone-25.0.0/keystone/limit/models/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/limit/models/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1891 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/limit/models/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      948 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/limit/models/flat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7578 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/limit/models/strict_two_level.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3551 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/limit/schema.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.593973 keystone-25.0.0/keystone/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.589973 keystone-25.0.0/keystone/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.701974 keystone-25.0.0/keystone/locale/de/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33367 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/locale/de/LC_MESSAGES/keystone.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.589973 keystone-25.0.0/keystone/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.701974 keystone-25.0.0/keystone/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    60037 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/locale/en_GB/LC_MESSAGES/keystone.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.589973 keystone-25.0.0/keystone/locale/es/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.701974 keystone-25.0.0/keystone/locale/es/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30856 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/locale/es/LC_MESSAGES/keystone.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.589973 keystone-25.0.0/keystone/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.701974 keystone-25.0.0/keystone/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30900 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/locale/fr/LC_MESSAGES/keystone.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.589973 keystone-25.0.0/keystone/locale/it/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.705973 keystone-25.0.0/keystone/locale/it/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30205 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/locale/it/LC_MESSAGES/keystone.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.589973 keystone-25.0.0/keystone/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.705973 keystone-25.0.0/keystone/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    34528 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/locale/ja/LC_MESSAGES/keystone.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.589973 keystone-25.0.0/keystone/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.705973 keystone-25.0.0/keystone/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32127 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/locale/ko_KR/LC_MESSAGES/keystone.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.593973 keystone-25.0.0/keystone/locale/pt_BR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.705973 keystone-25.0.0/keystone/locale/pt_BR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30105 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/locale/pt_BR/LC_MESSAGES/keystone.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.593973 keystone-25.0.0/keystone/locale/ru/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.705973 keystone-25.0.0/keystone/locale/ru/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38111 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/locale/ru/LC_MESSAGES/keystone.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.593973 keystone-25.0.0/keystone/locale/zh_CN/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.705973 keystone-25.0.0/keystone/locale/zh_CN/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28187 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/locale/zh_CN/LC_MESSAGES/keystone.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.593973 keystone-25.0.0/keystone/locale/zh_TW/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.705973 keystone-25.0.0/keystone/locale/zh_TW/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26824 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/locale/zh_TW/LC_MESSAGES/keystone.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.705973 keystone-25.0.0/keystone/models/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/models/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4867 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/models/receipt_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10682 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/models/revoke_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22322 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/models/token_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33038 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/notifications.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.705973 keystone-25.0.0/keystone/oauth1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      629 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/oauth1/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.705973 keystone-25.0.0/keystone/oauth1/backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/oauth1/backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6672 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/oauth1/backends/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10612 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/oauth1/backends/sql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5964 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/oauth1/core.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1357 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/oauth1/schema.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8860 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/oauth1/validator.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.705973 keystone-25.0.0/keystone/oauth2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/oauth2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1016 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/oauth2/handlers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.705973 keystone-25.0.0/keystone/policy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      629 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/policy/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.705973 keystone-25.0.0/keystone/policy/backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/policy/backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2308 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/policy/backends/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1558 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/policy/backends/rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2589 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/policy/backends/sql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2306 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/policy/core.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      970 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/policy/schema.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.705973 keystone-25.0.0/keystone/receipt/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      654 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/receipt/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2511 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/receipt/handlers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6118 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/receipt/provider.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.709973 keystone-25.0.0/keystone/receipt/providers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/receipt/providers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1997 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/receipt/providers/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.709973 keystone-25.0.0/keystone/receipt/providers/fernet/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      676 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/receipt/providers/fernet/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2609 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/receipt/providers/fernet/core.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10163 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/receipt/receipt_formatters.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.709973 keystone-25.0.0/keystone/resource/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      591 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/resource/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.709973 keystone-25.0.0/keystone/resource/backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/resource/backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8923 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/resource/backends/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      999 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/resource/backends/resource_options.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15948 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/resource/backends/sql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5359 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/resource/backends/sql_model.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.709973 keystone-25.0.0/keystone/resource/config_backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/resource/config_backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5312 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/resource/config_backends/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6394 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/resource/config_backends/sql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    71352 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/resource/core.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3286 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/resource/schema.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.709973 keystone-25.0.0/keystone/revoke/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      589 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/revoke/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.709973 keystone-25.0.0/keystone/revoke/backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/revoke/backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2068 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/revoke/backends/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6416 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/revoke/backends/sql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5338 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/revoke/core.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      597 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/revoke/model.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.709973 keystone-25.0.0/keystone/server/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1502 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/server/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2873 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/server/backends.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.709973 keystone-25.0.0/keystone/server/flask/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1670 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/server/flask/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6203 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/server/flask/application.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    44256 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/server/flask/common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6854 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/server/flask/core.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.709973 keystone-25.0.0/keystone/server/flask/request_processing/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/server/flask/request_processing/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3707 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/server/flask/request_processing/json_body.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.713974 keystone-25.0.0/keystone/server/flask/request_processing/middleware/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/server/flask/request_processing/middleware/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19868 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/server/flask/request_processing/middleware/auth_context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1483 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/server/flask/request_processing/middleware/url_normalize.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1092 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/server/flask/request_processing/req_logging.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1255 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/server/wsgi.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.713974 keystone-25.0.0/keystone/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.713974 keystone-25.0.0/keystone/tests/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6580 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/common/auth.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.713974 keystone-25.0.0/keystone/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3305 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/functional/core.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.713974 keystone-25.0.0/keystone/tests/functional/shared/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/functional/shared/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2060 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/functional/shared/test_running.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.713974 keystone-25.0.0/keystone/tests/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12074 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/hacking/checks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.713974 keystone-25.0.0/keystone/tests/protection/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.717974 keystone-25.0.0/keystone/tests/protection/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25271 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_access_rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28216 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_application_credential.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    62806 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_assignment.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7152 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_consumer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    49130 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_credentials.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28838 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_domain_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13992 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_domain_roles.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23074 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_domains.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18727 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_ec2_credential.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27578 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_endpoint_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16059 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_endpoints.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    80900 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_grants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    46719 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14485 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_identity_providers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8453 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_implied_roles.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28602 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17120 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_mappings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14341 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29154 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_policy_association.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19092 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_project_endpoint.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35285 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_project_tags.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35131 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_projects.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17093 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_protocols.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12705 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_regions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15187 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_registered_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13275 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_roles.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15530 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_service_providers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14003 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23758 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_system_assignments.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22583 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_tokens.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38441 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_trusts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37590 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/protection/v3/test_users.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.729974 keystone-25.0.0/keystone/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      660 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.729974 keystone-25.0.0/keystone/tests/unit/application_credential/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/application_credential/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.729974 keystone-25.0.0/keystone/tests/unit/application_credential/backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/application_credential/backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2718 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/application_credential/backends/test_sql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17912 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/application_credential/test_backends.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.729974 keystone-25.0.0/keystone/tests/unit/assignment/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/assignment/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.729974 keystone-25.0.0/keystone/tests/unit/assignment/role_backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/assignment/role_backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5010 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/assignment/role_backends/test_sql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   193143 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/assignment/test_backends.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13008 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/assignment/test_core.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.729974 keystone-25.0.0/keystone/tests/unit/auth/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/auth/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.729974 keystone-25.0.0/keystone/tests/unit/auth/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/auth/plugins/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3991 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/auth/plugins/test_core.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7836 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/auth/plugins/test_mapped.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2735 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/auth/test_controllers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15171 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/auth/test_schema.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.729974 keystone-25.0.0/keystone/tests/unit/backend/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/backend/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5226 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/backend/core_ldap.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1855 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/backend/core_sql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3240 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/base_classes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.733974 keystone-25.0.0/keystone/tests/unit/catalog/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/catalog/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26888 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/catalog/test_backends.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4167 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/catalog/test_core.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.733974 keystone-25.0.0/keystone/tests/unit/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/common/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.733974 keystone-25.0.0/keystone/tests/unit/common/sql/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/common/sql/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10248 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/common/sql/test_upgrades.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7217 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/common/test_cache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11883 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/common/test_database_conflicts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3665 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/common/test_json_home.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    67426 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/common/test_notifications.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3271 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/common/test_provider_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30720 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/common/test_rbac_enforcer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3410 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/common/test_resource_options_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2089 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/common/test_sql_core.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18350 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/common/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.733974 keystone-25.0.0/keystone/tests/unit/config_files/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/config_files/backend_ldap.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1086 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/config_files/backend_ldap_pool.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/config_files/backend_ldap_sql.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/config_files/backend_liveldap.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/config_files/backend_multi_ldap_sql.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      861 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/config_files/backend_pool_liveldap.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/config_files/backend_sql.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/config_files/backend_tls_liveldap.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.733974 keystone-25.0.0/keystone/tests/unit/config_files/domain_configs_default_ldap_one_sql/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/config_files/domain_configs_default_ldap_one_sql/keystone.domain1.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.733974 keystone-25.0.0/keystone/tests/unit/config_files/domain_configs_multi_ldap/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/config_files/domain_configs_multi_ldap/keystone.Default.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/config_files/domain_configs_multi_ldap/keystone.domain1.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      301 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/config_files/domain_configs_multi_ldap/keystone.domain2.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.733974 keystone-25.0.0/keystone/tests/unit/config_files/domain_configs_one_extra_sql/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/config_files/domain_configs_one_extra_sql/keystone.domain2.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.733974 keystone-25.0.0/keystone/tests/unit/config_files/domain_configs_one_sql_one_ldap/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/config_files/domain_configs_one_sql_one_ldap/keystone.Default.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/config_files/domain_configs_one_sql_one_ldap/keystone.domain1.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/config_files/test_auth_plugin.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.733974 keystone-25.0.0/keystone/tests/unit/contrib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/contrib/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.737974 keystone-25.0.0/keystone/tests/unit/contrib/federation/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/contrib/federation/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    45093 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/contrib/federation/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38998 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/core.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.737974 keystone-25.0.0/keystone/tests/unit/credential/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/credential/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4550 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/credential/test_backend_sql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3788 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/credential/test_fernet_provider.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      776 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/default_catalog.templates
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1435 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/default_catalog_multi_region.templates
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5250 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/default_fixtures.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.737974 keystone-25.0.0/keystone/tests/unit/endpoint_policy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/endpoint_policy/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.737974 keystone-25.0.0/keystone/tests/unit/endpoint_policy/backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/endpoint_policy/backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6555 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/endpoint_policy/backends/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1591 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/endpoint_policy/backends/test_sql.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.737974 keystone-25.0.0/keystone/tests/unit/external/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      536 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/external/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/external/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1196 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/external/test_timeutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23656 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/fakeldap.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.737974 keystone-25.0.0/keystone/tests/unit/federation/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/federation/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4976 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/federation/test_core.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11016 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/federation/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1050 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/federation_fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5085 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/filtering.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.737974 keystone-25.0.0/keystone/tests/unit/identity/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/identity/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.737974 keystone-25.0.0/keystone/tests/unit/identity/backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/identity/backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20330 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/identity/backends/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2443 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/identity/backends/test_ldap.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27164 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/identity/backends/test_ldap_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2395 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/identity/backends/test_sql.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.737974 keystone-25.0.0/keystone/tests/unit/identity/shadow_users/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/identity/shadow_users/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8300 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/identity/shadow_users/test_backend.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4770 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/identity/shadow_users/test_core.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    45457 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/identity/test_backend_sql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    62817 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/identity/test_backends.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7749 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/identity/test_core.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/identity_mapping.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.741974 keystone-25.0.0/keystone/tests/unit/ksfixtures/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1153 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/ksfixtures/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2438 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/ksfixtures/auth_plugins.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1383 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/ksfixtures/backendloader.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1601 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/ksfixtures/cache.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4517 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/ksfixtures/database.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10379 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/ksfixtures/hacking.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1906 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/ksfixtures/jws_key_repository.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1369 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/ksfixtures/key_repository.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1445 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/ksfixtures/ldapdb.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4216 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/ksfixtures/logging.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1215 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/ksfixtures/policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      946 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/ksfixtures/temporaryfile.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2682 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/ksfixtures/warnings.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.741974 keystone-25.0.0/keystone/tests/unit/limit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/limit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35260 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/limit/test_backends.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    44167 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/mapping_fixtures.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.741974 keystone-25.0.0/keystone/tests/unit/policy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/policy/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.741974 keystone-25.0.0/keystone/tests/unit/policy/backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/policy/backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2231 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/policy/backends/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1594 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/policy/backends/test_sql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3215 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/policy/test_backends.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.741974 keystone-25.0.0/keystone/tests/unit/receipt/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/receipt/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18247 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/receipt/test_fernet_provider.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2506 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/receipt/test_receipt_serialization.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.741974 keystone-25.0.0/keystone/tests/unit/resource/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/resource/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.741974 keystone-25.0.0/keystone/tests/unit/resource/backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/resource/backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1290 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/resource/backends/test_sql.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.741974 keystone-25.0.0/keystone/tests/unit/resource/config_backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/resource/config_backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2060 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/resource/config_backends/test_sql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    90115 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/resource/test_backends.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30645 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/resource/test_core.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8113 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/rest.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.741974 keystone-25.0.0/keystone/tests/unit/saml2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2422 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/saml2/idp_saml2_metadata.xml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4764 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/saml2/signed_saml2_assertion.xml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.741974 keystone-25.0.0/keystone/tests/unit/server/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/server/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31540 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/server/test_keystone_flask.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6285 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_app_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    62551 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_associate_project_endpoint_extension.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9080 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_auth_plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12134 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_backend_endpoint_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1460 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_backend_endpoint_policy_sql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2192 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_backend_federation_sql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19370 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_backend_id_mapping_sql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   146730 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_backend_ldap.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14617 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_backend_ldap_pool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2406 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_backend_rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    62222 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_backend_sql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14003 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_backend_templated.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    90477 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_cli.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1461 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7750 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_contrib_ec2_core.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10349 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_contrib_s3_core.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1124 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_contrib_simple_cert.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2283 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_driver_hints.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1131 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_entry_points.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11680 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3967 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_hacking_checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      922 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_healthcheck.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8258 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_ldap_livetest.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8382 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_ldap_pool_livetest.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4171 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_ldap_tls_livetest.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    73759 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32608 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_middleware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9887 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3002 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_receipt_provider.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20378 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_revoke.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8022 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_shadow_users.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14110 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_sql_banned_operations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11042 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_sql_upgrade.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2786 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_token_provider.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2584 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_url_middleware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    61596 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_v3.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28745 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_v3_application_credential.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   175651 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_v3_assignment.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   251166 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_v3_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    42581 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_v3_catalog.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    41633 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_v3_credential.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    48095 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_v3_domain_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10099 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_v3_endpoint_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   209947 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_v3_federation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36424 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_v3_filters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    56026 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_v3_identity.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    53357 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_v3_oauth1.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    85876 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_v3_oauth2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8118 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_v3_os_revoke.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2557 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_v3_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    78834 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_v3_resource.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24429 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_v3_trust.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   139339 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_validation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40586 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/test_versions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.741974 keystone-25.0.0/keystone/tests/unit/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3043 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/tests/test_core.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1279 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/tests/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.741974 keystone-25.0.0/keystone/tests/unit/token/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/token/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37069 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/token/test_fernet_provider.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4751 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/token/test_jws_provider.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2991 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/token/test_token_serialization.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.741974 keystone-25.0.0/keystone/tests/unit/trust/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/trust/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23383 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/trust/test_backends.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3903 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/tests/unit/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.741974 keystone-25.0.0/keystone/token/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      630 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/token/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13536 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/token/provider.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.741974 keystone-25.0.0/keystone/token/providers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/token/providers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2941 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/token/providers/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.745974 keystone-25.0.0/keystone/token/providers/fernet/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      605 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/token/providers/fernet/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4091 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/token/providers/fernet/core.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.745974 keystone-25.0.0/keystone/token/providers/jws/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/token/providers/jws/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8217 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/token/providers/jws/core.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    34629 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/token/token_formatters.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.745974 keystone-25.0.0/keystone/trust/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/trust/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.745974 keystone-25.0.0/keystone/trust/backends/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/trust/backends/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3346 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/trust/backends/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9881 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/trust/backends/sql.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8821 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/trust/core.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1907 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/trust/schema.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.661973 keystone-25.0.0/keystone.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3204 2024-04-03 11:52:09.000000 keystone-25.0.0/keystone.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    70129 2024-04-03 11:52:09.000000 keystone-25.0.0/keystone.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-03 11:52:09.000000 keystone-25.0.0/keystone.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3795 2024-04-03 11:52:09.000000 keystone-25.0.0/keystone.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-03 11:52:09.000000 keystone-25.0.0/keystone.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2024-04-03 11:52:09.000000 keystone-25.0.0/keystone.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      989 2024-04-03 11:52:09.000000 keystone-25.0.0/keystone.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2024-04-03 11:52:09.000000 keystone-25.0.0/keystone.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.745974 keystone-25.0.0/keystone_tempest_plugin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2024-04-03 11:51:37.000000 keystone-25.0.0/keystone_tempest_plugin/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.745974 keystone-25.0.0/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2024-04-03 11:51:37.000000 keystone-25.0.0/playbooks/enable-fips.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.745974 keystone-25.0.0/rally-jobs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2024-04-03 11:51:37.000000 keystone-25.0.0/rally-jobs/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2745 2024-04-03 11:51:37.000000 keystone-25.0.0/rally-jobs/keystone.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.597973 keystone-25.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.777974 keystone-25.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/Assignment_V9_driver-c22be069f7baccb0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      642 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/DomainSpecificRoles-fc5dd2ef74a1442c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/Role_V9_driver-971c3aae14d9963d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/V9ResourceDriver-26716f97c0cc1a80.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      776 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/add-bootstrap-cli-192500228cc6e574.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/add-description-to-role-88ab5bb8a96cc002.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/add-expires-at-int-to-trusts-60ae3c5d0c00808a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/add-limit-description-c1f42641d9c6c33d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      503 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/add-unified-limit-apis-c9ebc5116bc2cf93.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/add_bcrypt_sha256_algo-d6b146a59df9373c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/add_password_expires_at_to_user_response-22f14ab629c48bc2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      676 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/admin_token-a5678d712783c145.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      626 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/admin_token-c634ec12fc714255.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bcrypt_truncation_fix-674dc5d7f1e776f2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      657 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bootstrap-update-endpoint-7a63a2329822b6e7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1031 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bp-allow-expired-f5d845b9601bc1ef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1530 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bp-application-credentials-c699f1f17c7d4e2f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bp-basic-default-roles-4ff6502b6ac57d48.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      562 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bp-domain-config-as-stable-716ca5ab33c0cc42.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      301 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bp-domain-config-default-82e42d946ee7cb43.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bp-json-web-tokens-37ce3bcd1356cf1b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bp-manage-migration-c398963a943a89fe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1027 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bp-mfa-auth-receipt-8b459431c1f360ce.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bp-oauth2-client-credentials-ext-c8933f00a7b45be8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      589 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bp-password-expires-validation-4b32fe7032595932.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1179 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bp-pci-dss-notifications-808a205a637bac25.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bp-pci-dss-password-requirements-api-87bc724b2aa554f7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      838 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bp-pci-dss-query-password-expired-users-a7c96a3843bb9abc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3622 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bp-per-user-auth-plugin-reqs-feb95fd907be4b40.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1972 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bp-policy-in-code-722372a27291b9cd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      778 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bp-shadow-mapping-06fc7c71a401d707.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1715 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bp-strict-two-level-model.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bp-support-federated-attr-94084d4073f50280.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      745 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bp-support-oauth2-mtls-8552892a8e0c72d2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1218 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bp-system-scope-7d236ee5992d4e20.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bp-upgrade-checks-0dc692a392a96879.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bp-url-safe-naming-ad90d6a659f5bf3c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1081 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bp-whitelist-extension-for-app-creds-90e5bcd7b2b78b02.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      626 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1017606-98313bb4c1edf250.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1291157-00b5c714a097e84c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1332058-f25e2de40411b711.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1042 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1473292-c21481e6aec29ec2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      559 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1490804-de58a9606edb31eb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1519210-de76097c974f9c93.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      541 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1523369-4d42c841b6e7e54e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1524030-0814724d5c2b7c8d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1524030-ccff6b0ec9d1cbf2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1535878-change-get_project-permission-e460af1256a2c056.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      886 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1542417-d630b7886bb0b369.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1224 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1547684-911aed68a0d3df17.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1347 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1561054-dbe88b552a936a05.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1563101-134df5b99ea48f00.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1571878-1bcaea5337905af0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1582585-a368ac5a252ec84f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1590587-domain-specific-role-assignment-8f120604a6625852.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1594482-52a5dd1d8477b694.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1611102-e1348cbec9b1110a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1613466-credential-update-ec2-type-8fb51ff3ad3a449c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1615014-b30f606a2d202428.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1616424-c46ba773f7ac40ae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1622310-c501cf77437fdfa6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1636950-8fa1a47fce440977.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1638603-354ee4167e6e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1641625-fe463874dc5edb10.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      555 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1641639-b9accc163e61ca15.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      447 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1641645-516709f9da3de26f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1641654-8630ce7bcde43a7e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      661 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1641660-f938267e1ec54071.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1641816-8b39f3f73359c778.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1642212-9964dfd3af0184bd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1642348-83d4c86ad3984d75.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1642457-4533f9810a8cd927.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      968 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1642687-5497fb56fe86806d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      795 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1642687-c7ab1c9be152db20.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1642692-d669c8fcf9e171d9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1645487-ca22c216ec26cc9b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1649138-c53974f6bb0eab14.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      732 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1649446-efff94143823755d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1649616-b835d1dac3401e8c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      696 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1656076-c4422270f73b43b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1659730-17834ba2dde668ae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1042 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1659995-f3e716de743b7291.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1670382-ee851ba4f364d608.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1676497-92271e25f642e2de.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1684994-264fb8f182ced180.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1687593-95e1568291ecd70b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1688137-e4203c9a728690a7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1696574-15a728396350a95a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1700852-de775d0eb2ddfdd1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1701324-739a31f38037f77b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1702211-abb59adda73fd78e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      592 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1703369-9a901d627a1e0316.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      360 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1703666-b8a990f2bf5b62f0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      402 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1704205-bc0570feeb3ec5c4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      983 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1705485-7a1ad17b9cc99b9d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      865 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1718747-50d39fa87bdbb12b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      806 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1724645-a94659dfd0f45b9a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      408 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1727099-1af277b35db34372.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      433 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1727726-0b47608811a2cd16.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      509 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1728907-bab6769ab46bd8aa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      481 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1729933-4a09201e9dface2a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1733754-4d9d3042b8501ec6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1734244-1b4ea83baa72566d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1735250-b60332a7f288cf94.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1736875-c790f568c5f4d671.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1738895-342864cd0285bc42.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1740951-82b7e4bd608742ab.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1744195-a7154ac2e8556efc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1746599-848a1163e52ac0a6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1747694-48c8caa4871300e3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1880 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1748027-decc2e11154b97cf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1748970-eb63ad2030e296f3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1749264-676ca02902bcd169.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1749267-96153d2fa6868f67.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1750415-95ede3a9685b6e0c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2100 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1750660-e2a360ddd6790fc4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2724 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1750669-dfce859550126f03.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1366 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1750673-b53f74944d767ae9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1822 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1750676-cf70c1a27b2c8de3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1843 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1750678-88a38851ca80fc64.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1751045-f950e3fb85e2b573.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1753584-e052bc7805f001b4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1753585-7e11213743754999.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1754048-correct-federated-domain-47cb889d88d7770a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1754677-13ee75ed1b473f26.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1755874-9951f77c6d18431c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1756190-0e5d86d334555931.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1757022-664d0b0db1242bf8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1757151-43eb3baaa175f904.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1759289-466cdf4514de3498.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      575 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1760205-87dedd6d8812db3f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1760521-fec5c88af214401f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1760809-711df870a9d67c0d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1763824-3d2f5169af9d42f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1765193-b40318b9fb5d1c7b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      420 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1773967-b59517a09e0e6141.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1774229-cb968e95c9d81c4d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1183 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1776504-keystone-conversion-to-flask-372a5654a55675c6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1778109-ea15ce6a8207f857.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      995 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1778945-b7f2db3052525ca8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1779889-12eb5edf4cc93a1d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1779903-f2b22cf23a9e01f9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1780159-095ffa0e53be2464.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1780503-70ca1ba3f428dd41.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1782704-0b053eaf5d801dee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      497 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1782922-db822fda486ac773.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1784536-9d1d1e149c605a1d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1785164-2b7ed29266eb4792.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      658 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1787874-13499ec227b8e26c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1317 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1788415-3190279e9c900f76.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1788694-4dc8b3ec47fc6084.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      351 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1789450-9dec1383ffd3de01.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1792026-2de8345a89e2256b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1161 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1794376-53ce14528f00f01d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1794527-866b1caff67977f3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2328 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1794864-3116bf165a146be6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1796887-eaea84e3f9a8ff9f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1801095-6e28d7a86719da74.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1801873-0eb9a5ec3e801190.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      608 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1804292-0107869c7029f79e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1290 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1804446-1a281eadbb044070.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1804462-59ad43f98242dea0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1498 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1804463-74537652166cf656.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      615 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1804482-aa95619320d098fa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1506 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1804483-1d9ccfcb24f25f51.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1665 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1804516-24b0b10ed6fe0589.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      666 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1804517-a351aec088fee066.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1804519-8384a9ead261d4c2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      654 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1804520-d124599967923052.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1555 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1804521-3c0d9f567e8f532f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1651 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1804522-00df902cd2d74ee3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1545 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1804523-d1768909b13b167e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1550 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1805363-0b85d71917ad09d1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1867 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1805366-670867516c6fc4bc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2225 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1805368-ea32c2db2ae57225.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2436 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1805369-ed98d3fcfafb5c43.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1600 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1805371-249c8c9b562ab371.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1234 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1805372-af4ebf4b19500b72.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1547 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1805400-c192be936d277ade.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1463 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1805402-75d0d93f31af620f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1837 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1805403-c003627a64768716.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2066 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1805406-252b45d443af20b3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3643 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1805409-8bc6cc9f1c5bc672.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      605 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1805880-0032024ea6b83563.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      638 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1805880-3fc6b30309a4370f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      604 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1806713-cf5feab23fc78a23.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1194 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1806762-08ff9eecdc03c554.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      639 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1806762-09f414995924db23.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1806762-0b7356ace200a5d3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1806762-2092fee9f6c87dc3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1409 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1806762-c3bfc71cb9bb94f3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      802 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1806762-daed3e27f58f0f6d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      990 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1809116-b65502f3b606b060.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1810393-5a7d379842c51d9b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1811605-9d23080d7e949c25.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1813085-cf24b204e95fd7f5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1814589-f3e7f554bee1c317.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1815771-ae0e4118c552f01e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      617 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1816076-ba39508e6ade529e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1816927-e17f4e596e611380.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1817313-c11481e6eed29ec2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2108 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1818725-96d698e22e648764.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2789 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1818734-d753bfae60ffd030.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      835 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1818736-98ea186a074056f4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      419 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1818845-05f8c3af5ea9abc7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2116 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1818846-d1a8c77d20659ad6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1819036-e2d24655c70d0aad.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      847 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1820333-356dcc8bf9f73fed.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      487 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1823258-9649b56a440b5ae1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      614 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1823258-9f93dbdc0fa8441d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1827431-2f078c13dfc9a02a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1831918-c70cf87ef086d871.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1832265-cb76ccf505c2d9d1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      455 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1833739-f962e8caf3e22068.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1836568-66d853a1f22c5530.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1839133-24570c9fbacb530d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1839577-1226d86ea0744055.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1840291-35af1ac7ba06e166.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1841486-425f367925f5e03f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      438 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1843609-8498b132222596b7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      617 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1844157-7808af9bcea0429d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2153 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1844194-48ae60db49f91bd4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1844207-x27a31f3403xfd7y.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1530 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1844461-08a8bdc5f613b88d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1809 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1844664-905cf6cad2e032a7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1848238-f6533644f7907358.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1054 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1848342-317c9e4afa65a3ff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1272 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1855080-08b28181b7cb2470.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1856881-277103af343187f1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1856904-101af15bb48eb3ca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1856962-2c87d541da61c727.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1858012-584267ada7e33f2c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1872732-7261816d0b170008.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1872733-2377f456a57ad32c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1720 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1872735-0989e51d2248ce1e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1324 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1872737-f8e1ad3b6705b766.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1872753-e2a934eac919ccde.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1083 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1872755-2c81d3267b89f124.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1105 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1873290-ff7f8e4cee15b75a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1878938-70ee2af6fdf66004.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1880252-51036d5353125e15.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1885753-51df25f3ff1d9ae8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1886017-bc2ad648d57101a2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1889936-78d6853b5212b8f1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1896125-b17a4d12730fe493.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      299 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1897280-e7065c4368a325ad.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1901207-13762f85b8a04481.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1901654-69b9f35d11cd0c75.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1926483-a77ab887e0e7f5c9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1929066-6e741c9182620a37.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1941020-cleanup-541a2d372a1cf4cd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      345 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1941020-f694395a9bcea72f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      495 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug-1951632-11272e49e2fa439d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug1828565-0790c4c60ba34100.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug_1526462-df9a3f3974d9040f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2375 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug_1543048_and_1668503-7ead4e15faaab778.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug_1674415-e8a7345aa2b05ab7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug_1688188-256e3572295231a1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      364 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/bug_1698900-f195125bf341d887.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/catalog-caching-12f2532cfb71325a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/catalog_project_id-519f5a70f9f7c4c6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/change_min_pool_retry_max-f5e7c8d315401426.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2745 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/convert-keystone-to-flask-80d980e239b662b0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/deprecate-endpoint-policy-cfg-option-d018acab72a398a0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1008 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/deprecate-json-formatted-policy-file-95f6307f88358f58.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/deprecate-memcache-token-persistence-eac88c80147ea241.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/deprecate-policies-api-b104fbd1d2367b1b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/deprecate-templated-catalog-driver-f811a6040abdc4a8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      575 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/deprecate-v2-apis-894284c17be881d2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1742 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/deprecated-as-of-mitaka-8534e43fa40c1d09.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/deprecated-as-of-newton-be1d8dbcc6bdc68f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/deprecated-as-of-ocata-a5b2f1e3e39f818e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      481 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/deprecated-as-of-pike-506f9aca91674550.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1158 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/deprecated-as-of-queens-8ad7f826e4f08f57.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      572 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/deprecated-as-of-rocky-60b2fa05d07d3a28.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/deprecated-as-of-stein-0166965502cb3be2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/deprecated-as-of-train-de3fe41ff2251385.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/deprecated-socket_timeout-option-d3358b4f2310706c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      515 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/domain-level-limit-support-60e1e330d06227ed.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/dont-enforce-get-s3tokens-ec2tokens-62b90b199e8075d8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      415 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/drop-project-id-fk-b683b414e1585be8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/drop-python-3-6-and-3-7-dc90b86cedced92b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/enable-filter-idp-d0135f4615178cfc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      445 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/enable-inherit-on-default-54ac435230261a6a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/endpoints-from-endpoint_group-project-association-7271fba600322fb6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/eventlet-cleanup-f35fc5f83c16ea1c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1395 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/extensions-to-core-a0d270d216d47276.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/federation-group-ids-mapping-6c56120d65a5cb22.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/filter-mappings-by-entity-77162a146d375385.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/httpd-keystone-d51b7335559b09c8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/identity_driver_new_change_password_method-e8c0e06795bca2d8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      463 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/immutable-resource-options-bug-1807751-acc1e3c689484337.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      408 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/impl-templated-catalog-1d8f6333726b34f8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      641 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/implied-roles-026f401adc0f7fb6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/implied-roles-stable-8b293e187c5620ad.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/insecure_reponse-2a168230709bc8e7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/integrate-osprofiler-ad0e16a542b12899.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      775 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/is-admin-24b34238c83b3a82.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/ldap-conn-pool-enabled-90df94652f1ded53.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/ldap-emulation-91c4d535eb9c3d10.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      567 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/limits-api-refactor-05abf9e6c2e75852.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/list_limit-ldap-support-5d31d51466fc49a6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/list_role_assignment_names-33aedc1e521230b6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      572 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/mapping_populate-521d92445505b8a3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      471 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/max-password-length-truncation-and-warning-bd69090315ec18a7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/migration_squash-f655329ddad7fc2a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/no-default-domain-2161ada44bf7a3f7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/notify-on-user-group-membership-8c0136ee0484e255.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/oauth1-headers-content-type-9a9245d9bbec8f8e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      758 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/oslo.cache-a9ce47bfa8809efa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/password-created_at-nullable-b3c284be50d93ef5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/policy_new_federated_projects_for_user-dcd7bd148efef049.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/pre-cache-tokens-73450934918af26b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      750 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/project-tags-1e72a6779d9d02c5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/projects_as_domains-3ea8a58b4c2965e1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/python3-support-e4189e0a1a6e2e4f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/randomize_urls-c0c19f48b2bfa299.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/remove-db_sync-extension-opt-2ab1f29340281215.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/remove-legacy-migrations-647f60019c8dd9e8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/remove-sqlalchemy-migrate-a4fa47685c7e28c6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/remove-token-auth-middleware-5ea3b3734ce1d9e6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/remove-trust-auth-support-from-v2-de316c9ba46d556d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2467 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/removed-as-of-mitaka-9ff14f87d0b98e7e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1186 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/removed-as-of-newton-721c06b5dcb1b34a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4550 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/removed-as-of-ocata-436bb4b839e74494.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2678 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/removed-as-of-pike-deadbeefdeadbeef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/removed-as-of-queens-94c04e88c08f89aa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1104 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/removed-as-of-rocky-f44c3ba7c3e73d01.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1504 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/removed-as-of-stein-5eb23253b72ab54e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      656 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/removed-as-of-train-92b2942a680eb859.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/removed-as-of-ussuri-d2f6ef8901ef54ed.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/request_context-e143ba9c446a5952.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      640 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/resource-backend-sql-only-03154d8712b36bd0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/resource-driver-33793dd5080ee4d2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      544 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/revert-v2-token-issued-for-non-default-domain-25ea5337f158ef13.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/s3-aws-v4-c6cb75ce8d2289d4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1578 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/scope-and-default-roles-a733c235731bb558.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      662 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/support_encrypted_credentials_at_rest-93dcb67b3508e91a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1230 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/switch-to-alembic-1fa5248f0ce824ae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/tenant_id_to_project_id-42d95d93011785cb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/token-formatter-ec58aba00fa83706.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/token-provider-refactor-a3a64146807daf36.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      521 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/token_expiration_to_match_application_credential-56d058355a9f240d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      474 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/totp-40d93231714c6a20.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      743 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/unified-limit-api-improvment-b34d18769d18a0a7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/use-correct-inspect-8142e317c1e39c2a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/use-pyldap-6e811c28bf350d6d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/use-python-ldap-0318ff7798bdd98d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/v2-dep-d6e7ab2d08119549.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/v3-endpoints-in-v2-list-b0439816938713d6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/v9FederationDriver-cbebcf5f97e1eae2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/notes/x509-auth-df0a229780b8e3ff.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.777974 keystone-25.0.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/source/2023.2.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.777974 keystone-25.0.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.777974 keystone-25.0.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8945 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      862 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/source/liberty.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.597973 keystone-25.0.0/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.597973 keystone-25.0.0/releasenotes/source/locale/en_GB/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.777974 keystone-25.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    94656 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.597973 keystone-25.0.0/releasenotes/source/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.777974 keystone-25.0.0/releasenotes/source/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2728 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.597973 keystone-25.0.0/releasenotes/source/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.777974 keystone-25.0.0/releasenotes/source/locale/ja/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   197755 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.597973 keystone-25.0.0/releasenotes/source/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.777974 keystone-25.0.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5029 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      662 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-04-03 11:51:37.000000 keystone-25.0.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-04-03 11:51:37.000000 keystone-25.0.0/reno.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1415 2024-04-03 11:51:37.000000 keystone-25.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4896 2024-04-03 11:52:09.781974 keystone-25.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-04-03 11:51:37.000000 keystone-25.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2024-04-03 11:51:37.000000 keystone-25.0.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:52:09.781974 keystone-25.0.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2479 2024-04-03 11:51:37.000000 keystone-25.0.0/tools/cover.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      645 2024-04-03 11:51:37.000000 keystone-25.0.0/tools/fast8.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     8816 2024-04-03 11:51:37.000000 keystone-25.0.0/tools/sample_data.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2142 2024-04-03 11:51:37.000000 keystone-25.0.0/tools/test-setup.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5557 2024-04-03 11:51:37.000000 keystone-25.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.320302 keystone-25.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1443 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7390 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28905 2024-03-19 10:21:04.000000 keystone-25.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      654 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   373809 2024-03-19 10:21:03.000000 keystone-25.0.0.0rc1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1645 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3209 2024-03-19 10:21:05.320302 keystone-25.0.0.0rc1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1692 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.032230 keystone-25.0.0.0rc1/api-ref/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.060237 keystone-25.0.0.0rc1/api-ref/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6364 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.060237 keystone-25.0.0.0rc1/api-ref/source/v2-ext/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v2-ext/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2884 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v2-ext/ksec2-admin.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1908 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v2-ext/parameters.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.032230 keystone-25.0.0.0rc1/api-ref/source/v2-ext/samples/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.060237 keystone-25.0.0.0rc1/api-ref/source/v2-ext/samples/OS-KSEC2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      471 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v2-ext/samples/OS-KSEC2/authenticate-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1079 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v2-ext/samples/OS-KSEC2/authenticate-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v2-ext/samples/OS-KSEC2/credentials-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      409 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v2-ext/samples/OS-KSEC2/credentialswithec2-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v2-ext/samples/OS-KSEC2/ec2Credentials-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v2-ext/samples/OS-KSEC2/ec2Credentials-show-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.064238 keystone-25.0.0.0rc1/api-ref/source/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13614 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/application-credentials.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29782 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/authenticate-v3.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5565 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/credentials.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14543 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/domains-config-v3.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5875 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/domains.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7650 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/groups.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9664 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15807 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/inherit.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/os-pki.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    60655 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/parameters.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4442 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/policies.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8081 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/project-tags.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8419 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/projects.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5580 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/regions-v3.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26330 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/roles.inc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.036231 keystone-25.0.0.0rc1/api-ref/source/v3/samples/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.108249 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/access-rule-get-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/access-rules-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      488 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/application-credential-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      820 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/application-credential-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      789 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/application-credential-get-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1978 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/application-credential-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/auth-application-credential-id-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/auth-application-credential-name-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1951 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/auth-application-credential-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      343 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/auth-password-explicit-unscoped-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/auth-password-explicit-unscoped-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16630 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/auth-password-project-scoped-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/auth-password-system-scoped-request-with-domain.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/auth-password-unscoped-request-with-domain.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/auth-password-unscoped-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/auth-password-unscoped-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/auth-password-user-name-unscoped-response-HTTP.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/auth-token-explicit-unscoped-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/auth-token-scoped-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16627 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/auth-token-scoped-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/auth-token-unscoped-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      510 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/auth-token-unscoped-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      705 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/create-role-inferences-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/credential-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/credential-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/credential-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/credential-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/credential-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5789 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/credentials-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/domain-config-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/domain-config-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/domain-config-default-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/domain-config-group-default-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/domain-config-group-option-default-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       36 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/domain-config-group-option-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       45 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/domain-config-group-option-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/domain-config-group-option-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/domain-config-group-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/domain-config-group-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/domain-config-group-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/domain-config-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/domain-config-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/domain-config-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/domain-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/domain-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/domain-group-roles-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/domain-group-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/domain-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/domain-specific-role-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       95 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/domain-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      294 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/domain-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      549 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/domain-user-roles-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/domains-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/endpoint-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      448 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/endpoint-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      427 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/endpoint-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/endpoint-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/endpoint-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12873 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/endpoints-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      719 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/get-available-domain-scopes-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      678 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/get-available-project-scopes-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/get-available-system-scopes-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      705 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/get-role-inferences-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1042 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/get-service-catalog-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/group-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/group-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      573 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/group-roles-domain-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/group-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/group-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/group-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      922 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/group-users-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      802 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/groups-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      443 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/identity-version-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1389 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/identity-versions-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/limit-flat-model-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      461 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/limit-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      589 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/limits-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1095 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/limits-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1221 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/limits-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/limits-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      531 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/limits-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1000 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/list-implied-roles-for-role-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/list-system-roles-for-group-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      463 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/list-system-roles-for-user-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      809 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/policies-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/policy-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/policy-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/policy-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/policy-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/policy-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/project-create-domain-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/project-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/project-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/project-enable-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      551 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/project-group-roles-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      736 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/project-show-parents-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/project-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1584 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/project-show-subtree-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/project-tags-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/project-tags-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      524 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/project-tags-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/project-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/project-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/project-user-roles-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3628 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/projects-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/region-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/region-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/region-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/region-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/region-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/regions-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      412 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/registered-limit-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      430 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/registered-limits-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      895 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/registered-limits-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1032 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/registered-limits-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/registered-limits-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/registered-limits-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2224 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/role-assignments-effective-list-include-names-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1109 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/role-assignments-effective-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/role-assignments-effective-list-response.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1261 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/role-assignments-list-include-subtree-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1009 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/role-assignments-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/role-assignments-list-response.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/role-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/role-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2316 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/role-inferences-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/role-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/role-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/role-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1792 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/roles-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/service-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/service-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/service-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/service-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/service-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3332 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/services-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       54 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/token-validate-request.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/user-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      805 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/user-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      894 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/user-groups-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/user-password-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      876 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/user-projects-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      572 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/user-roles-domain-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      352 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/user-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/user-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      438 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/user-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4849 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/users-list-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.036231 keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.108249 keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/requests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/requests/domain-id-password.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/requests/domain-id-token.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/requests/domain-name-password.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/requests/domain-name-token.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/requests/project-id-password.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/requests/project-id-token.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      428 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/requests/project-id-totp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/requests/project-name-password.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/requests/project-name-token.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/requests/system-password.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/requests/system-token.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.112250 keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/responses/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/responses/auth-receipt-password.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1962 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/responses/domain-scoped-password.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2021 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/responses/domain-scoped-token.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2140 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/responses/project-scoped-password-totp.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2120 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/responses/project-scoped-password.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2179 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/responses/project-scoped-token.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1928 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/responses/system-scoped-password.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1987 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/responses/system-scoped-token.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/responses/unscoped-password.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9456 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/service-catalog.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2169 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/status.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7335 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/system-roles.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12106 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/unified_limits.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8523 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3/users.inc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.064238 keystone-25.0.0.0rc1/api-ref/source/v3-ext/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9668 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/endpoint-policy.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15901 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/ep-filter.inc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.036231 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.068239 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/assertion/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3675 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/assertion/assertion.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      549 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/assertion/parameters.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.068239 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/assertion/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/assertion/samples/ecp-saml-assertion-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5648 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/assertion/samples/ecp-saml-assertion-response.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1249 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/assertion/samples/metadata-response.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/assertion/samples/saml-assertion-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4602 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/assertion/samples/saml-assertion-response.xml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.068239 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/auth/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3975 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/auth/auth.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      979 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/auth/parameters.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.068239 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/auth/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/auth/samples/scoped-token-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2236 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/auth/samples/scoped-token-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/auth/samples/unscoped-token-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.068239 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/identity-provider/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9425 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/identity-provider/idp.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2148 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/identity-provider/parameters.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.072240 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/identity-provider/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/identity-provider/samples/add-protocol-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/identity-provider/samples/add-protocol-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/identity-provider/samples/get-protocol-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      477 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/identity-provider/samples/get-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      535 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/identity-provider/samples/list-protocol-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1154 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/identity-provider/samples/list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/identity-provider/samples/register-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/identity-provider/samples/register-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/identity-provider/samples/update-protocol-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/identity-provider/samples/update-protocol-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/identity-provider/samples/update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      466 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/identity-provider/samples/update-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.072240 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/mapping/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3340 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/mapping/mapping.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/mapping/parameters.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.072240 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/mapping/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      795 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/mapping/samples/create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      928 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/mapping/samples/create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      928 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/mapping/samples/get-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1227 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/mapping/samples/list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/mapping/samples/update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      936 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/mapping/samples/update-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.072240 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/projects-domains/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/projects-domains/parameters.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2055 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/projects-domains/projects-domains.inc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.072240 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/projects-domains/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/projects-domains/samples/domain-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      691 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/projects-domains/samples/project-list-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.072240 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/service-provider/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1257 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/service-provider/parameters.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.076241 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/service-provider/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/service-provider/samples/get-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1233 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/service-provider/samples/list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/service-provider/samples/register-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/service-provider/samples/register-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/service-provider/samples/update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      485 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/service-provider/samples/update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4217 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/service-provider/sp.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9975 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1031 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13878 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/oauth.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2983 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/oauth2.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15562 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/parameters.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2205 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/revoke.inc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.036231 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.076241 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-ENDPOINT-POLICY/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      878 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-ENDPOINT-POLICY/policy-endpoint-associations-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-ENDPOINT-POLICY/policy-show-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.076241 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-EP-FILTER/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-EP-FILTER/create-endpoint-group-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      369 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-EP-FILTER/endpoint-group-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1119 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-EP-FILTER/endpoint-groups-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-EP-FILTER/endpoint-project-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-EP-FILTER/list-associations-by-endpoint-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      814 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-EP-FILTER/list-associations-by-project-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1353 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-EP-FILTER/list-service-endpoints.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-EP-FILTER/update-endpoint-group-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-EP-FILTER/update-endpoint-group-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.080242 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-OAUTH1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-OAUTH1/access-token-create-response.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-OAUTH1/access-token-role-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      634 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-OAUTH1/access-token-roles-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      446 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-OAUTH1/access-token-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      659 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-OAUTH1/access-tokens-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      119 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-OAUTH1/authorize-request-token-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-OAUTH1/authorize-request-token-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-OAUTH1/consumer-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-OAUTH1/consumer-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-OAUTH1/consumer-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       69 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-OAUTH1/consumer-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-OAUTH1/consumer-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      549 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-OAUTH1/consumers-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-OAUTH1/request-token-create-response.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.080242 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-OAUTH2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-OAUTH2/token-create-request.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-OAUTH2/token-create-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.080242 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-REVOKE/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-REVOKE/list-revoke-response.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.080242 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-SIMPLE-CERT/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1223 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-SIMPLE-CERT/show-ca-certificate-response.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1187 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-SIMPLE-CERT/show-signing-certificate-response.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.080242 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-TRUST/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1332 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-TRUST/trust-auth-redelegated-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-TRUST/trust-auth-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1249 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-TRUST/trust-auth-trust-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-TRUST/trust-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      828 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-TRUST/trust-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      761 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-TRUST/trust-get-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-TRUST/trust-get-role-delegated-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      722 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-TRUST/trust-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      397 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-TRUST/trust-list-roles-delegated-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/simple-cert.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10061 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/api-ref/source/v3-ext/trust.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1099 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.112250 keystone-25.0.0.0rc1/config-generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/config-generator/keystone-policy-generator.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      389 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/config-generator/keystone.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.112250 keystone-25.0.0.0rc1/devstack/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.036231 keystone-25.0.0.0rc1/devstack/files/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.112250 keystone-25.0.0.0rc1/devstack/files/federation/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3794 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/devstack/files/federation/attribute-map.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/devstack/files/federation/shib_apache_alias.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/devstack/files/federation/shib_apache_handler.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3769 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/devstack/files/federation/shibboleth2.xml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.112250 keystone-25.0.0.0rc1/devstack/files/oidc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1601 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/devstack/files/oidc/apache_oidc.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.112250 keystone-25.0.0.0rc1/devstack/lib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8634 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/devstack/lib/federation.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6524 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/devstack/lib/oidc.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1055 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/devstack/lib/scope.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3686 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/devstack/plugin.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.036231 keystone-25.0.0.0rc1/devstack/tools/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.112250 keystone-25.0.0.0rc1/devstack/tools/oidc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/devstack/tools/oidc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1180 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/devstack/tools/oidc/docker-compose.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1893 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/devstack/tools/oidc/setup_keycloak_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.112250 keystone-25.0.0.0rc1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5753 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/Makefile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.112250 keystone-25.0.0.0rc1/doc/ext/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/ext/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      541 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.116251 keystone-25.0.0.0rc1/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.116251 keystone-25.0.0.0rc1/doc/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6258 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/_static/horizon-login-idp.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16334 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/_static/horizon-login-sp.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      638 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/_static/support-matrix.css
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.124253 keystone-25.0.0.0rc1/doc/source/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3722 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/auth-totp.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/authentication-mechanisms.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5936 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/bootstrap.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7832 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/caching-layer.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3349 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/case-insensitive.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13760 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/cli-manage-projects-users-and-roles.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      684 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/configuration.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3177 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/configure-https.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23543 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/configure_tokenless_x509.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4430 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/credential-encryption.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9878 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/domain-specific-config.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      708 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/endpoint-filtering.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      543 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/endpoint-policy.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19951 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/event_notifications.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4176 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/external-authentication.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.124253 keystone-25.0.0.0rc1/doc/source/admin/federation/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28362 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/federation/configure_federation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/federation/federated_identity.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20607 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/federation/introduction.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31809 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/federation/mapping_combinations.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5126 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/federation/mellon.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8872 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/federation/openidc.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8730 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/federation/shibboleth.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18579 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/fernet-token-faq.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.124253 keystone-25.0.0.0rc1/doc/source/admin/figures/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    53211 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/figures/keystone-federation.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7680 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/figures/keystone-federation.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/getting-started.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      506 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/health-check-middleware.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14777 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/identity-concepts.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1370 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/identity-sources.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4202 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/identity-support-matrix.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18075 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/integrate-with-ldap.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3890 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/jws-key-rotation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/keystone-features.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1409 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/limit-list-size.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      703 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/logging.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10656 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/manage-services.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      964 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/manage-trusts.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3278 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/multi-factor-authentication.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      939 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/oauth1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5342 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/oauth2-usage-guide.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/operations.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3933 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/performance.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6815 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/resource-options.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7689 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/security-compliance.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21018 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/service-api-protection.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1711 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/token-provider.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4172 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/token-support-matrix.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6378 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/tokens-overview.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/tokens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      881 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/troubleshoot.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21157 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/unified-limits.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11932 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/upgrading.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1497 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/admin/url-safe-naming.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29677 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/api_curl_examples.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.128254 keystone-25.0.0.0rc1/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1462 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/cli/commands.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      775 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4921 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/cli/keystone-manage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2925 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/cli/keystone-status.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/code_documentation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9276 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.128254 keystone-25.0.0.0rc1/doc/source/configuration/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      781 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/configuration/config-options.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      590 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/configuration/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      672 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/configuration/policy.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.128254 keystone-25.0.0.0rc1/doc/source/configuration/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/configuration/samples/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/configuration/samples/keystone-conf.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/configuration/samples/logging-conf.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/configuration/samples/policy-yaml.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.132255 keystone-25.0.0.0rc1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8334 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/contributor/api_change_tutorial.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      862 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/contributor/architecture.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3973 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/contributor/auth-plugins.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3660 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/contributor/caching-layer.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2908 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5037 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/contributor/database-migrations.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4188 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/contributor/developing-drivers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4855 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/contributor/doctor-checks.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2099 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/contributor/filtering-responsibilities.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5715 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/contributor/how-can-i-help.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8399 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/contributor/http-api.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1917 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/contributor/id-manage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1169 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1545 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/contributor/list-truncation.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5583 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/contributor/programming-exercises.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5369 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/contributor/proposing-features.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4645 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/contributor/release-notes.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7517 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/contributor/service-catalog.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29640 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/contributor/services.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7613 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/contributor/set-up-keystone.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14953 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/contributor/testing-keystone.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6049 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/contributor/vision-reflection.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.132255 keystone-25.0.0.0rc1/doc/source/getting-started/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17078 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/getting-started/architecture.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3588 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/getting-started/community.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/getting-started/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22156 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/getting-started/policy_mapping.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3124 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/indices-tables.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.136256 keystone-25.0.0.0rc1/doc/source/install/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.136256 keystone-25.0.0.0rc1/doc/source/install/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2794 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/install/common/get-started-identity.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4948 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/install/common/keystone-users.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3831 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/install/common/openrc.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       45 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/install/get-started-obs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       45 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/install/get-started-rdo.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       45 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/install/get-started-ubuntu.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1339 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/install/index-obs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1305 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/install/index-rdo.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1219 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/install/index-ubuntu.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/install/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6903 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/install/keystone-install-obs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5627 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/install/keystone-install-rdo.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5576 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/install/keystone-install-ubuntu.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/install/keystone-openrc-obs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/install/keystone-openrc-rdo.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       31 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/install/keystone-openrc-ubuntu.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/install/keystone-users-obs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/install/keystone-users-rdo.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/install/keystone-users-ubuntu.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2817 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/install/keystone-verify-obs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2817 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/install/keystone-verify-rdo.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2809 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/install/keystone-verify-ubuntu.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.136256 keystone-25.0.0.0rc1/doc/source/install/shared/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/install/shared/note_configuration_vary_by_distribution.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.136256 keystone-25.0.0.0rc1/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16821 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/user/application_credentials.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1065 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3637 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/user/json_home.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3579 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/user/multi-factor-authentication.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3416 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/user/supported_clients.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2647 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/doc/source/user/trusts.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.136256 keystone-25.0.0.0rc1/etc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/etc/README.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1929 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/etc/default_catalog.templates
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1046 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/etc/logging.conf.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/etc/sso_callback_template.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.040232 keystone-25.0.0.0rc1/examples/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.040232 keystone-25.0.0.0rc1/examples/pki/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.140257 keystone-25.0.0.0rc1/examples/pki/certs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1391 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/examples/pki/certs/cacert.pem
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3030 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/examples/pki/certs/middleware.pem
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1326 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/examples/pki/certs/signing_cert.pem
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1326 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/examples/pki/certs/ssl_cert.pem
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.140257 keystone-25.0.0.0rc1/examples/pki/private/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1704 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/examples/pki/private/cakey.pem
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1704 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/examples/pki/private/signing_key.pem
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1704 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/examples/pki/private/ssl_key.pem
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.140257 keystone-25.0.0.0rc1/httpd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/httpd/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      623 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/httpd/keystone-uwsgi-admin.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      623 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/httpd/keystone-uwsgi-public.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      277 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/httpd/uwsgi-keystone.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      991 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/httpd/wsgi-keystone.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.140257 keystone-25.0.0.0rc1/keystone/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.148259 keystone-25.0.0.0rc1/keystone/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2416 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.148259 keystone-25.0.0.0rc1/keystone/api/_shared/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7776 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/_shared/EC2_S3_Resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      417 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/_shared/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10849 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/_shared/authentication.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1789 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/_shared/implied_roles.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3957 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/_shared/json_home_relations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2985 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/_shared/saml.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19701 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9096 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/credentials.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4259 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/discovery.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20181 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/domains.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3557 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/ec2tokens.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5862 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/endpoints.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8791 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5623 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13358 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/os_ep_filter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20143 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/os_federation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19007 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/os_inherit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14927 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/os_oauth1.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16161 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/os_oauth2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2912 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/os_revoke.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2164 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/os_simple_cert.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10810 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21741 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/projects.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3977 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/regions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3699 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/registered_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16163 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/role_assignments.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2482 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/role_inferences.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12263 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/roles.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4397 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/s3tokens.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2977 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7273 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/system.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20650 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/trusts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35853 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/api/users.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.148259 keystone-25.0.0.0rc1/keystone/application_credential/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      605 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/application_credential/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.152260 keystone-25.0.0.0rc1/keystone/application_credential/backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/application_credential/backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4607 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/application_credential/backends/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11735 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/application_credential/backends/sql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10648 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/application_credential/core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2114 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/application_credential/schema.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.152260 keystone-25.0.0.0rc1/keystone/assignment/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/assignment/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.152260 keystone-25.0.0.0rc1/keystone/assignment/backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/assignment/backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7489 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/assignment/backends/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17315 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/assignment/backends/sql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    61208 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/assignment/core.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.152260 keystone-25.0.0.0rc1/keystone/assignment/role_backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/assignment/role_backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4390 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/assignment/role_backends/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      990 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/assignment/role_backends/resource_options.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6568 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/assignment/role_backends/sql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4495 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/assignment/role_backends/sql_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1123 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/assignment/schema.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.152260 keystone-25.0.0.0rc1/keystone/auth/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/auth/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23262 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/auth/core.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.156261 keystone-25.0.0.0rc1/keystone/auth/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      619 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/auth/plugins/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1589 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/auth/plugins/application_credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3476 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/auth/plugins/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9800 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/auth/plugins/core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3138 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/auth/plugins/external.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16678 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/auth/plugins/mapped.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2703 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/auth/plugins/oauth1.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1649 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/auth/plugins/password.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5084 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/auth/plugins/token.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4679 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/auth/plugins/totp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5875 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/auth/schema.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.156261 keystone-25.0.0.0rc1/keystone/catalog/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      630 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/catalog/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.156261 keystone-25.0.0.0rc1/keystone/catalog/backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/catalog/backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16696 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/catalog/backends/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27762 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/catalog/backends/sql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12360 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/catalog/backends/templated.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13944 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/catalog/core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2929 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/catalog/schema.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.156261 keystone-25.0.0.0rc1/keystone/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15015 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/cmd/bootstrap.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    57559 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/cmd/cli.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.160262 keystone-25.0.0.0rc1/keystone/cmd/doctor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2739 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/cmd/doctor/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2089 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/cmd/doctor/caching.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2911 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/cmd/doctor/credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1093 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/cmd/doctor/database.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      934 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/cmd/doctor/debug.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1305 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/cmd/doctor/federation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5586 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/cmd/doctor/ldap.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2407 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/cmd/doctor/security_compliance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1548 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/cmd/doctor/tokens.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1784 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/cmd/doctor/tokens_fernet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6115 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/cmd/idutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1474 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/cmd/manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3905 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/cmd/status.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.160262 keystone-25.0.0.0rc1/keystone/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1449 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/authorization.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.160262 keystone-25.0.0.0rc1/keystone/common/cache/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      624 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/cache/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3758 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/cache/_context_cache.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6149 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/cache/core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2917 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4521 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/driver_hints.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11975 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/fernet_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4739 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/json_home.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1651 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/jwt_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7670 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5886 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/password_hashing.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.168264 keystone-25.0.0.0rc1/keystone/common/policies/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3368 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2120 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/access_rule.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3170 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/access_token.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3510 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/application_credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2439 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3870 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3861 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/consumer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3892 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4236 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/domain.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7657 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/domain_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3545 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/ec2_credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3748 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/endpoint.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9264 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/endpoint_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14576 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/grant.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8665 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4772 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/identity_provider.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6774 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/implied_role.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3097 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/limit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4290 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/mapping.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3867 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10380 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/policy_association.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10726 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/project.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5068 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/project_endpoint.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4224 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/protocol.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3787 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/region.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2570 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/registered_limit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1016 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/revoke_event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6992 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/role.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2934 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/role_assignment.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3730 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4587 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/service_provider.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2982 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/token.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1779 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/token_revocation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6836 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/trust.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5812 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/policies/user.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1753 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/profiler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4553 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/provider_api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.168264 keystone-25.0.0.0rc1/keystone/common/rbac_enforcer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/rbac_enforcer/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22030 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/rbac_enforcer/enforcer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1254 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/rbac_enforcer/policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6050 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/render_token.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.168264 keystone-25.0.0.0rc1/keystone/common/resource_options/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      601 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/resource_options/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9368 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/resource_options/core.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.168264 keystone-25.0.0.0rc1/keystone/common/resource_options/options/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1284 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/resource_options/options/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2898 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/resource_options/options/immutable.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.168264 keystone-25.0.0.0rc1/keystone/common/sql/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/sql/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2678 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/sql/alembic.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21420 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/sql/core.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.172265 keystone-25.0.0.0rc1/keystone/common/sql/migrations/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      538 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/sql/migrations/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/sql/migrations/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4647 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/sql/migrations/autogen.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6570 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/sql/migrations/env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9026 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/sql/migrations/manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      976 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/sql/migrations/script.py.mako
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.172265 keystone-25.0.0.0rc1/keystone/common/sql/migrations/versions/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.040232 keystone-25.0.0.0rc1/keystone/common/sql/migrations/versions/2024.01/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.172265 keystone-25.0.0.0rc1/keystone/common/sql/migrations/versions/2024.01/expand/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1100 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/sql/migrations/versions/2024.01/expand/47147121_add_identity_federation_attribute_mapping_schema_version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37329 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/sql/migrations/versions/27e647c0fad4_initial_version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/sql/migrations/versions/CONTRACT_HEAD
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/sql/migrations/versions/EXPAND_HEAD
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.040232 keystone-25.0.0.0rc1/keystone/common/sql/migrations/versions/bobcat/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.172265 keystone-25.0.0.0rc1/keystone/common/sql/migrations/versions/bobcat/contract/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1174 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/sql/migrations/versions/bobcat/contract/99de3849d860_fix_incorrect_constraints.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3019 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/sql/migrations/versions/bobcat/contract/c88cdce8f248_remove_duplicate_constraints.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.172265 keystone-25.0.0.0rc1/keystone/common/sql/migrations/versions/bobcat/expand/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1063 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/sql/migrations/versions/bobcat/expand/11c3b243b4cb_remove_service_provider_relay_state_server_default.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1199 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/sql/migrations/versions/bobcat/expand/b4f8b3f584e0_fix_incorrect_constraints.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.044233 keystone-25.0.0.0rc1/keystone/common/sql/migrations/versions/yoga/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.172265 keystone-25.0.0.0rc1/keystone/common/sql/migrations/versions/yoga/contract/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      888 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/sql/migrations/versions/yoga/contract/e25ffa003242_initial.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.172265 keystone-25.0.0.0rc1/keystone/common/sql/migrations/versions/yoga/expand/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/sql/migrations/versions/yoga/expand/29e87d24a316_initial.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10417 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/sql/upgrades.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7913 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/tokenless_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19560 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.172265 keystone-25.0.0.0rc1/keystone/common/validation/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2344 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/validation/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2085 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/validation/parameter_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3818 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/common/validation/validators.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.180267 keystone-25.0.0.0rc1/keystone/conf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5589 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1894 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/application_credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1375 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/assignment.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4252 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2403 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/catalog.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      925 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2993 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5921 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/default.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1632 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/domain_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1588 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/endpoint_filter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1103 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/endpoint_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4727 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/federation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2966 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/fernet_receipts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2918 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/fernet_tokens.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6804 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/identity.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2803 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/identity_mapping.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2352 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/jwt_tokens.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17273 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/ldap.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1856 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/oauth1.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1701 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/oauth2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2797 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1332 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2537 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/receipt.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3788 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1897 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/revoke.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1909 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/role.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5728 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/saml.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5875 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/security_compliance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1237 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/shadow_users.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5191 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/token.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2393 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/tokenless_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/totp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1714 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/trust.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2259 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/unified_limit.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1140 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1789 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/conf/wsgi.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.180267 keystone-25.0.0.0rc1/keystone/credential/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/credential/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.180267 keystone-25.0.0.0rc1/keystone/credential/backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/credential/backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3920 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/credential/backends/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4815 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/credential/backends/sql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10050 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/credential/core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      855 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/credential/provider.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.180267 keystone-25.0.0.0rc1/keystone/credential/providers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/credential/providers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1207 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/credential/providers/core.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.180267 keystone-25.0.0.0rc1/keystone/credential/providers/fernet/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      610 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/credential/providers/fernet/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4647 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/credential/providers/fernet/core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1643 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/credential/schema.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.180267 keystone-25.0.0.0rc1/keystone/endpoint_policy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      598 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/endpoint_policy/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.184268 keystone-25.0.0.0rc1/keystone/endpoint_policy/backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/endpoint_policy/backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5832 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/endpoint_policy/backends/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6182 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/endpoint_policy/backends/sql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11495 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/endpoint_policy/core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27422 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/exception.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.184268 keystone-25.0.0.0rc1/keystone/federation/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      633 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/federation/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.184268 keystone-25.0.0.0rc1/keystone/federation/backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/federation/backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11146 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/federation/backends/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15934 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/federation/backends/sql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/federation/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7336 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/federation/core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27804 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/federation/idp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4103 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/federation/schema.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37678 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/federation/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      878 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.184268 keystone-25.0.0.0rc1/keystone/identity/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      679 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/identity/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.184268 keystone-25.0.0.0rc1/keystone/identity/backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/identity/backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13955 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/identity/backends/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.188269 keystone-25.0.0.0rc1/keystone/identity/backends/ldap/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      605 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/identity/backends/ldap/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    81249 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/identity/backends/ldap/common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18497 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/identity/backends/ldap/core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1614 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/identity/backends/ldap/models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5086 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/identity/backends/resource_options.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19701 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/identity/backends/sql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18510 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/identity/backends/sql_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    72588 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/identity/core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1581 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/identity/generator.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.188269 keystone-25.0.0.0rc1/keystone/identity/id_generators/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/identity/id_generators/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1246 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/identity/id_generators/sha256.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.188269 keystone-25.0.0.0rc1/keystone/identity/mapping_backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/identity/mapping_backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3388 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/identity/mapping_backends/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      640 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/identity/mapping_backends/mapping.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4771 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/identity/mapping_backends/sql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3792 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/identity/schema.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.188269 keystone-25.0.0.0rc1/keystone/identity/shadow_backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/identity/shadow_backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5082 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/identity/shadow_backends/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10969 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/identity/shadow_backends/sql.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.188269 keystone-25.0.0.0rc1/keystone/limit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      614 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/limit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.188269 keystone-25.0.0.0rc1/keystone/limit/backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/limit/backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5766 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/limit/backends/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13015 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/limit/backends/sql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5818 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/limit/core.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.188269 keystone-25.0.0.0rc1/keystone/limit/models/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/limit/models/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1891 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/limit/models/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      948 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/limit/models/flat.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7578 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/limit/models/strict_two_level.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3551 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/limit/schema.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.044233 keystone-25.0.0.0rc1/keystone/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.044233 keystone-25.0.0.0rc1/keystone/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.192270 keystone-25.0.0.0rc1/keystone/locale/de/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33367 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/locale/de/LC_MESSAGES/keystone.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.044233 keystone-25.0.0.0rc1/keystone/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.192270 keystone-25.0.0.0rc1/keystone/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    60037 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/locale/en_GB/LC_MESSAGES/keystone.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.044233 keystone-25.0.0.0rc1/keystone/locale/es/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.192270 keystone-25.0.0.0rc1/keystone/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30856 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/locale/es/LC_MESSAGES/keystone.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.044233 keystone-25.0.0.0rc1/keystone/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.192270 keystone-25.0.0.0rc1/keystone/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30900 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/locale/fr/LC_MESSAGES/keystone.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.044233 keystone-25.0.0.0rc1/keystone/locale/it/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.192270 keystone-25.0.0.0rc1/keystone/locale/it/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30205 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/locale/it/LC_MESSAGES/keystone.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.044233 keystone-25.0.0.0rc1/keystone/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.192270 keystone-25.0.0.0rc1/keystone/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34528 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/locale/ja/LC_MESSAGES/keystone.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.044233 keystone-25.0.0.0rc1/keystone/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.192270 keystone-25.0.0.0rc1/keystone/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32127 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/locale/ko_KR/LC_MESSAGES/keystone.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.044233 keystone-25.0.0.0rc1/keystone/locale/pt_BR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.192270 keystone-25.0.0.0rc1/keystone/locale/pt_BR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30105 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/locale/pt_BR/LC_MESSAGES/keystone.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.044233 keystone-25.0.0.0rc1/keystone/locale/ru/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.192270 keystone-25.0.0.0rc1/keystone/locale/ru/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38111 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/locale/ru/LC_MESSAGES/keystone.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.044233 keystone-25.0.0.0rc1/keystone/locale/zh_CN/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.192270 keystone-25.0.0.0rc1/keystone/locale/zh_CN/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28187 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/locale/zh_CN/LC_MESSAGES/keystone.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.044233 keystone-25.0.0.0rc1/keystone/locale/zh_TW/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.192270 keystone-25.0.0.0rc1/keystone/locale/zh_TW/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26824 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/locale/zh_TW/LC_MESSAGES/keystone.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.192270 keystone-25.0.0.0rc1/keystone/models/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/models/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4867 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/models/receipt_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10682 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/models/revoke_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22322 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/models/token_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33038 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/notifications.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.192270 keystone-25.0.0.0rc1/keystone/oauth1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      629 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/oauth1/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.196271 keystone-25.0.0.0rc1/keystone/oauth1/backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/oauth1/backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6672 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/oauth1/backends/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10612 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/oauth1/backends/sql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5964 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/oauth1/core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1357 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/oauth1/schema.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8860 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/oauth1/validator.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.196271 keystone-25.0.0.0rc1/keystone/oauth2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/oauth2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1016 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/oauth2/handlers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.196271 keystone-25.0.0.0rc1/keystone/policy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      629 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/policy/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.196271 keystone-25.0.0.0rc1/keystone/policy/backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/policy/backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2308 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/policy/backends/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1558 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/policy/backends/rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2589 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/policy/backends/sql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2306 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/policy/core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      970 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/policy/schema.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.196271 keystone-25.0.0.0rc1/keystone/receipt/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      654 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/receipt/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2511 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/receipt/handlers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6118 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/receipt/provider.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.196271 keystone-25.0.0.0rc1/keystone/receipt/providers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/receipt/providers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1997 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/receipt/providers/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.196271 keystone-25.0.0.0rc1/keystone/receipt/providers/fernet/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      676 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/receipt/providers/fernet/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2609 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/receipt/providers/fernet/core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10163 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/receipt/receipt_formatters.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.200272 keystone-25.0.0.0rc1/keystone/resource/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      591 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/resource/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.200272 keystone-25.0.0.0rc1/keystone/resource/backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/resource/backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8923 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/resource/backends/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      999 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/resource/backends/resource_options.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15948 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/resource/backends/sql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5359 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/resource/backends/sql_model.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.200272 keystone-25.0.0.0rc1/keystone/resource/config_backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/resource/config_backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5312 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/resource/config_backends/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6394 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/resource/config_backends/sql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    71352 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/resource/core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3286 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/resource/schema.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.200272 keystone-25.0.0.0rc1/keystone/revoke/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      589 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/revoke/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.200272 keystone-25.0.0.0rc1/keystone/revoke/backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/revoke/backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2068 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/revoke/backends/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6416 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/revoke/backends/sql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5338 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/revoke/core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      597 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/revoke/model.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.200272 keystone-25.0.0.0rc1/keystone/server/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1502 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/server/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2873 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/server/backends.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.204273 keystone-25.0.0.0rc1/keystone/server/flask/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1670 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/server/flask/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6203 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/server/flask/application.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    44256 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/server/flask/common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6854 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/server/flask/core.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.204273 keystone-25.0.0.0rc1/keystone/server/flask/request_processing/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/server/flask/request_processing/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3707 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/server/flask/request_processing/json_body.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.204273 keystone-25.0.0.0rc1/keystone/server/flask/request_processing/middleware/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/server/flask/request_processing/middleware/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19868 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/server/flask/request_processing/middleware/auth_context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1483 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/server/flask/request_processing/middleware/url_normalize.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1092 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/server/flask/request_processing/req_logging.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1255 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/server/wsgi.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.204273 keystone-25.0.0.0rc1/keystone/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.204273 keystone-25.0.0.0rc1/keystone/tests/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6580 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/common/auth.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.204273 keystone-25.0.0.0rc1/keystone/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3305 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/functional/core.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.204273 keystone-25.0.0.0rc1/keystone/tests/functional/shared/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/functional/shared/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2060 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/functional/shared/test_running.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.204273 keystone-25.0.0.0rc1/keystone/tests/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12074 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/hacking/checks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.204273 keystone-25.0.0.0rc1/keystone/tests/protection/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.212275 keystone-25.0.0.0rc1/keystone/tests/protection/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25271 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_access_rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28216 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_application_credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    62806 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_assignment.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7152 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_consumer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    49130 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_credentials.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28838 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_domain_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13992 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_domain_roles.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23074 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_domains.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18727 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_ec2_credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27578 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_endpoint_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16059 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_endpoints.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    80900 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_grants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    46719 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14485 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_identity_providers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8453 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_implied_roles.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28602 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17120 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_mappings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14341 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29154 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_policy_association.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19092 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_project_endpoint.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35285 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_project_tags.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35131 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_projects.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17093 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_protocols.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12705 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_regions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15187 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_registered_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13275 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_roles.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15530 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_service_providers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14003 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23758 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_system_assignments.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22583 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_tokens.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38441 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_trusts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37590 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_users.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.228279 keystone-25.0.0.0rc1/keystone/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      660 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.228279 keystone-25.0.0.0rc1/keystone/tests/unit/application_credential/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/application_credential/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.228279 keystone-25.0.0.0rc1/keystone/tests/unit/application_credential/backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/application_credential/backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2718 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/application_credential/backends/test_sql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17912 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/application_credential/test_backends.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.228279 keystone-25.0.0.0rc1/keystone/tests/unit/assignment/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/assignment/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.228279 keystone-25.0.0.0rc1/keystone/tests/unit/assignment/role_backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/assignment/role_backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5010 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/assignment/role_backends/test_sql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   193143 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/assignment/test_backends.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13008 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/assignment/test_core.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.228279 keystone-25.0.0.0rc1/keystone/tests/unit/auth/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/auth/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.228279 keystone-25.0.0.0rc1/keystone/tests/unit/auth/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/auth/plugins/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3991 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/auth/plugins/test_core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7836 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/auth/plugins/test_mapped.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2735 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/auth/test_controllers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15171 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/auth/test_schema.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.232280 keystone-25.0.0.0rc1/keystone/tests/unit/backend/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/backend/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5226 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/backend/core_ldap.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1855 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/backend/core_sql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3240 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/base_classes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.232280 keystone-25.0.0.0rc1/keystone/tests/unit/catalog/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/catalog/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26888 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/catalog/test_backends.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4167 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/catalog/test_core.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.232280 keystone-25.0.0.0rc1/keystone/tests/unit/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.232280 keystone-25.0.0.0rc1/keystone/tests/unit/common/sql/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/common/sql/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10248 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/common/sql/test_upgrades.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7217 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/common/test_cache.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11883 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/common/test_database_conflicts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3665 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/common/test_json_home.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    67426 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/common/test_notifications.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3271 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/common/test_provider_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30720 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/common/test_rbac_enforcer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3410 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/common/test_resource_options_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2089 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/common/test_sql_core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18350 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/common/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.236281 keystone-25.0.0.0rc1/keystone/tests/unit/config_files/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/config_files/backend_ldap.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1086 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/config_files/backend_ldap_pool.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/config_files/backend_ldap_sql.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/config_files/backend_liveldap.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/config_files/backend_multi_ldap_sql.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      861 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/config_files/backend_pool_liveldap.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/config_files/backend_sql.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/config_files/backend_tls_liveldap.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.236281 keystone-25.0.0.0rc1/keystone/tests/unit/config_files/domain_configs_default_ldap_one_sql/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/config_files/domain_configs_default_ldap_one_sql/keystone.domain1.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.236281 keystone-25.0.0.0rc1/keystone/tests/unit/config_files/domain_configs_multi_ldap/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/config_files/domain_configs_multi_ldap/keystone.Default.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/config_files/domain_configs_multi_ldap/keystone.domain1.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      301 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/config_files/domain_configs_multi_ldap/keystone.domain2.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.236281 keystone-25.0.0.0rc1/keystone/tests/unit/config_files/domain_configs_one_extra_sql/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/config_files/domain_configs_one_extra_sql/keystone.domain2.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.236281 keystone-25.0.0.0rc1/keystone/tests/unit/config_files/domain_configs_one_sql_one_ldap/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/config_files/domain_configs_one_sql_one_ldap/keystone.Default.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/config_files/domain_configs_one_sql_one_ldap/keystone.domain1.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/config_files/test_auth_plugin.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.236281 keystone-25.0.0.0rc1/keystone/tests/unit/contrib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/contrib/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.236281 keystone-25.0.0.0rc1/keystone/tests/unit/contrib/federation/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/contrib/federation/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    45093 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/contrib/federation/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38998 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/core.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.236281 keystone-25.0.0.0rc1/keystone/tests/unit/credential/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/credential/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4550 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/credential/test_backend_sql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3788 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/credential/test_fernet_provider.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      776 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/default_catalog.templates
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1435 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/default_catalog_multi_region.templates
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5250 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/default_fixtures.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.236281 keystone-25.0.0.0rc1/keystone/tests/unit/endpoint_policy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/endpoint_policy/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.236281 keystone-25.0.0.0rc1/keystone/tests/unit/endpoint_policy/backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/endpoint_policy/backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6555 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/endpoint_policy/backends/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1591 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/endpoint_policy/backends/test_sql.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.240282 keystone-25.0.0.0rc1/keystone/tests/unit/external/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      536 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/external/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/external/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1196 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/external/test_timeutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23656 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/fakeldap.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.240282 keystone-25.0.0.0rc1/keystone/tests/unit/federation/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/federation/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4976 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/federation/test_core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11016 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/federation/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1050 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/federation_fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5085 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/filtering.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.240282 keystone-25.0.0.0rc1/keystone/tests/unit/identity/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/identity/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.240282 keystone-25.0.0.0rc1/keystone/tests/unit/identity/backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/identity/backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20330 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/identity/backends/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2443 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/identity/backends/test_ldap.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27164 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/identity/backends/test_ldap_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2395 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/identity/backends/test_sql.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.240282 keystone-25.0.0.0rc1/keystone/tests/unit/identity/shadow_users/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/identity/shadow_users/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8300 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/identity/shadow_users/test_backend.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4770 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/identity/shadow_users/test_core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    45457 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/identity/test_backend_sql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    62817 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/identity/test_backends.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7749 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/identity/test_core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/identity_mapping.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.244283 keystone-25.0.0.0rc1/keystone/tests/unit/ksfixtures/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1153 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/ksfixtures/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2438 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/ksfixtures/auth_plugins.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1383 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/ksfixtures/backendloader.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1601 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/ksfixtures/cache.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4517 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/ksfixtures/database.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10379 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/ksfixtures/hacking.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1906 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/ksfixtures/jws_key_repository.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1369 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/ksfixtures/key_repository.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1445 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/ksfixtures/ldapdb.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4216 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/ksfixtures/logging.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1215 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/ksfixtures/policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      946 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/ksfixtures/temporaryfile.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2682 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/ksfixtures/warnings.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.244283 keystone-25.0.0.0rc1/keystone/tests/unit/limit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/limit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35260 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/limit/test_backends.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    44167 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/mapping_fixtures.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.244283 keystone-25.0.0.0rc1/keystone/tests/unit/policy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/policy/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.244283 keystone-25.0.0.0rc1/keystone/tests/unit/policy/backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/policy/backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2231 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/policy/backends/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1594 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/policy/backends/test_sql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3215 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/policy/test_backends.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.244283 keystone-25.0.0.0rc1/keystone/tests/unit/receipt/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/receipt/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18247 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/receipt/test_fernet_provider.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2506 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/receipt/test_receipt_serialization.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.244283 keystone-25.0.0.0rc1/keystone/tests/unit/resource/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/resource/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.248284 keystone-25.0.0.0rc1/keystone/tests/unit/resource/backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/resource/backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1290 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/resource/backends/test_sql.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.248284 keystone-25.0.0.0rc1/keystone/tests/unit/resource/config_backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/resource/config_backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2060 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/resource/config_backends/test_sql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    90115 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/resource/test_backends.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30645 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/resource/test_core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8113 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/rest.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.248284 keystone-25.0.0.0rc1/keystone/tests/unit/saml2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2422 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/saml2/idp_saml2_metadata.xml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4764 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/saml2/signed_saml2_assertion.xml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.248284 keystone-25.0.0.0rc1/keystone/tests/unit/server/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/server/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31540 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/server/test_keystone_flask.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6285 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_app_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    62551 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_associate_project_endpoint_extension.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9080 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_auth_plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12134 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_backend_endpoint_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1460 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_backend_endpoint_policy_sql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2192 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_backend_federation_sql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19370 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_backend_id_mapping_sql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   146730 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_backend_ldap.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14617 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_backend_ldap_pool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2406 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_backend_rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    62222 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_backend_sql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14003 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_backend_templated.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    90477 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_cli.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1461 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7750 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_contrib_ec2_core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10349 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_contrib_s3_core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1124 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_contrib_simple_cert.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2283 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_driver_hints.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1131 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_entry_points.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11680 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3967 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_hacking_checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      922 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_healthcheck.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8258 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_ldap_livetest.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8382 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_ldap_pool_livetest.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4171 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_ldap_tls_livetest.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    73759 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32608 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_middleware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9887 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3002 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_receipt_provider.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20378 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_revoke.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8022 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_shadow_users.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14110 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_sql_banned_operations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11042 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_sql_upgrade.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2786 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_token_provider.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2584 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_url_middleware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    61596 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_v3.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28745 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_application_credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   175651 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_assignment.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   251166 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    42581 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_catalog.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    41633 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_credential.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    48095 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_domain_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10099 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_endpoint_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   209947 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_federation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36424 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_filters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    56026 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_identity.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    53357 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_oauth1.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    85876 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_oauth2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8118 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_os_revoke.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2557 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    78834 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_resource.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24429 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_trust.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   139339 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_validation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40586 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/test_versions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.248284 keystone-25.0.0.0rc1/keystone/tests/unit/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3043 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/tests/test_core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1279 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/tests/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.248284 keystone-25.0.0.0rc1/keystone/tests/unit/token/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/token/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37069 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/token/test_fernet_provider.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4751 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/token/test_jws_provider.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2991 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/token/test_token_serialization.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.248284 keystone-25.0.0.0rc1/keystone/tests/unit/trust/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/trust/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23383 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/trust/test_backends.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3903 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/tests/unit/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.248284 keystone-25.0.0.0rc1/keystone/token/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      630 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/token/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13536 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/token/provider.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.248284 keystone-25.0.0.0rc1/keystone/token/providers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/token/providers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2941 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/token/providers/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.252285 keystone-25.0.0.0rc1/keystone/token/providers/fernet/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      605 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/token/providers/fernet/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4091 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/token/providers/fernet/core.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.252285 keystone-25.0.0.0rc1/keystone/token/providers/jws/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/token/providers/jws/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8217 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/token/providers/jws/core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34629 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/token/token_formatters.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.252285 keystone-25.0.0.0rc1/keystone/trust/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/trust/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.252285 keystone-25.0.0.0rc1/keystone/trust/backends/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/trust/backends/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3346 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/trust/backends/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9881 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/trust/backends/sql.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8821 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/trust/core.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1907 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/trust/schema.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.144258 keystone-25.0.0.0rc1/keystone.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3209 2024-03-19 10:21:04.000000 keystone-25.0.0.0rc1/keystone.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    70129 2024-03-19 10:21:05.000000 keystone-25.0.0.0rc1/keystone.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-19 10:21:04.000000 keystone-25.0.0.0rc1/keystone.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3795 2024-03-19 10:21:04.000000 keystone-25.0.0.0rc1/keystone.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-19 10:21:04.000000 keystone-25.0.0.0rc1/keystone.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2024-03-19 10:21:04.000000 keystone-25.0.0.0rc1/keystone.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      989 2024-03-19 10:21:04.000000 keystone-25.0.0.0rc1/keystone.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2024-03-19 10:21:04.000000 keystone-25.0.0.0rc1/keystone.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.252285 keystone-25.0.0.0rc1/keystone_tempest_plugin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/keystone_tempest_plugin/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.252285 keystone-25.0.0.0rc1/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/playbooks/enable-fips.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.252285 keystone-25.0.0.0rc1/rally-jobs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/rally-jobs/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2745 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/rally-jobs/keystone.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.052235 keystone-25.0.0.0rc1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.316301 keystone-25.0.0.0rc1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/Assignment_V9_driver-c22be069f7baccb0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      642 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/DomainSpecificRoles-fc5dd2ef74a1442c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/Role_V9_driver-971c3aae14d9963d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/V9ResourceDriver-26716f97c0cc1a80.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      776 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/add-bootstrap-cli-192500228cc6e574.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      195 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/add-description-to-role-88ab5bb8a96cc002.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/add-expires-at-int-to-trusts-60ae3c5d0c00808a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/add-limit-description-c1f42641d9c6c33d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      503 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/add-unified-limit-apis-c9ebc5116bc2cf93.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      219 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/add_bcrypt_sha256_algo-d6b146a59df9373c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/add_password_expires_at_to_user_response-22f14ab629c48bc2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      676 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/admin_token-a5678d712783c145.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      626 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/admin_token-c634ec12fc714255.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      261 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bcrypt_truncation_fix-674dc5d7f1e776f2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      657 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bootstrap-update-endpoint-7a63a2329822b6e7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1031 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bp-allow-expired-f5d845b9601bc1ef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1530 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bp-application-credentials-c699f1f17c7d4e2f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bp-basic-default-roles-4ff6502b6ac57d48.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      562 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bp-domain-config-as-stable-716ca5ab33c0cc42.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      301 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bp-domain-config-default-82e42d946ee7cb43.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bp-json-web-tokens-37ce3bcd1356cf1b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bp-manage-migration-c398963a943a89fe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1027 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bp-mfa-auth-receipt-8b459431c1f360ce.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      498 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bp-oauth2-client-credentials-ext-c8933f00a7b45be8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      589 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bp-password-expires-validation-4b32fe7032595932.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1179 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bp-pci-dss-notifications-808a205a637bac25.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      571 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bp-pci-dss-password-requirements-api-87bc724b2aa554f7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      838 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bp-pci-dss-query-password-expired-users-a7c96a3843bb9abc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3622 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bp-per-user-auth-plugin-reqs-feb95fd907be4b40.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1972 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bp-policy-in-code-722372a27291b9cd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      778 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bp-shadow-mapping-06fc7c71a401d707.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1715 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bp-strict-two-level-model.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bp-support-federated-attr-94084d4073f50280.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      745 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bp-support-oauth2-mtls-8552892a8e0c72d2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1218 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bp-system-scope-7d236ee5992d4e20.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bp-upgrade-checks-0dc692a392a96879.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bp-url-safe-naming-ad90d6a659f5bf3c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1081 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bp-whitelist-extension-for-app-creds-90e5bcd7b2b78b02.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      626 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1017606-98313bb4c1edf250.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1291157-00b5c714a097e84c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1332058-f25e2de40411b711.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1042 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1473292-c21481e6aec29ec2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      559 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1490804-de58a9606edb31eb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      292 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1519210-de76097c974f9c93.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      541 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1523369-4d42c841b6e7e54e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1524030-0814724d5c2b7c8d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      803 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1524030-ccff6b0ec9d1cbf2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1535878-change-get_project-permission-e460af1256a2c056.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      886 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1542417-d630b7886bb0b369.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1224 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1547684-911aed68a0d3df17.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1347 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1561054-dbe88b552a936a05.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1563101-134df5b99ea48f00.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1571878-1bcaea5337905af0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1582585-a368ac5a252ec84f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1590587-domain-specific-role-assignment-8f120604a6625852.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1594482-52a5dd1d8477b694.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1611102-e1348cbec9b1110a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1613466-credential-update-ec2-type-8fb51ff3ad3a449c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1615014-b30f606a2d202428.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1616424-c46ba773f7ac40ae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      702 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1622310-c501cf77437fdfa6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1636950-8fa1a47fce440977.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1638603-354ee4167e6e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      265 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1641625-fe463874dc5edb10.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      555 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1641639-b9accc163e61ca15.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      447 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1641645-516709f9da3de26f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      937 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1641654-8630ce7bcde43a7e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      661 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1641660-f938267e1ec54071.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1641816-8b39f3f73359c778.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1642212-9964dfd3af0184bd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1642348-83d4c86ad3984d75.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1642457-4533f9810a8cd927.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      968 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1642687-5497fb56fe86806d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      795 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1642687-c7ab1c9be152db20.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1642692-d669c8fcf9e171d9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1645487-ca22c216ec26cc9b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1649138-c53974f6bb0eab14.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      732 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1649446-efff94143823755d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1649616-b835d1dac3401e8c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      696 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1656076-c4422270f73b43b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      547 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1659730-17834ba2dde668ae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1042 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1659995-f3e716de743b7291.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      276 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1670382-ee851ba4f364d608.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1676497-92271e25f642e2de.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1684994-264fb8f182ced180.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1687593-95e1568291ecd70b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1688137-e4203c9a728690a7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      332 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1696574-15a728396350a95a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1700852-de775d0eb2ddfdd1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1701324-739a31f38037f77b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1702211-abb59adda73fd78e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      592 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1703369-9a901d627a1e0316.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      360 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1703666-b8a990f2bf5b62f0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      402 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1704205-bc0570feeb3ec5c4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      983 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1705485-7a1ad17b9cc99b9d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      865 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1718747-50d39fa87bdbb12b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      806 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1724645-a94659dfd0f45b9a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      408 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1727099-1af277b35db34372.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      433 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1727726-0b47608811a2cd16.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      509 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1728907-bab6769ab46bd8aa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      481 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1729933-4a09201e9dface2a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1733754-4d9d3042b8501ec6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1734244-1b4ea83baa72566d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1735250-b60332a7f288cf94.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1736875-c790f568c5f4d671.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1738895-342864cd0285bc42.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1740951-82b7e4bd608742ab.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1744195-a7154ac2e8556efc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1746599-848a1163e52ac0a6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1747694-48c8caa4871300e3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1880 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1748027-decc2e11154b97cf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      392 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1748970-eb63ad2030e296f3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1749264-676ca02902bcd169.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1749267-96153d2fa6868f67.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1750415-95ede3a9685b6e0c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2100 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1750660-e2a360ddd6790fc4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2724 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1750669-dfce859550126f03.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1366 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1750673-b53f74944d767ae9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1822 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1750676-cf70c1a27b2c8de3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1843 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1750678-88a38851ca80fc64.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      324 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1751045-f950e3fb85e2b573.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1753584-e052bc7805f001b4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1753585-7e11213743754999.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1754048-correct-federated-domain-47cb889d88d7770a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      371 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1754677-13ee75ed1b473f26.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1755874-9951f77c6d18431c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1756190-0e5d86d334555931.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      386 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1757022-664d0b0db1242bf8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1757151-43eb3baaa175f904.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1759289-466cdf4514de3498.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      575 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1760205-87dedd6d8812db3f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1760521-fec5c88af214401f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1760809-711df870a9d67c0d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1763824-3d2f5169af9d42f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1765193-b40318b9fb5d1c7b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      420 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1773967-b59517a09e0e6141.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1774229-cb968e95c9d81c4d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1183 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1776504-keystone-conversion-to-flask-372a5654a55675c6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1778109-ea15ce6a8207f857.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      995 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1778945-b7f2db3052525ca8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1779889-12eb5edf4cc93a1d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1779903-f2b22cf23a9e01f9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1780159-095ffa0e53be2464.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1780503-70ca1ba3f428dd41.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1782704-0b053eaf5d801dee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      497 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1782922-db822fda486ac773.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1784536-9d1d1e149c605a1d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1785164-2b7ed29266eb4792.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      658 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1787874-13499ec227b8e26c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1317 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1788415-3190279e9c900f76.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1788694-4dc8b3ec47fc6084.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      351 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1789450-9dec1383ffd3de01.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1792026-2de8345a89e2256b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1161 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1794376-53ce14528f00f01d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1794527-866b1caff67977f3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2328 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1794864-3116bf165a146be6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1796887-eaea84e3f9a8ff9f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1801095-6e28d7a86719da74.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1801873-0eb9a5ec3e801190.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      608 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1804292-0107869c7029f79e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1290 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1804446-1a281eadbb044070.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      611 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1804462-59ad43f98242dea0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1498 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1804463-74537652166cf656.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      615 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1804482-aa95619320d098fa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1506 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1804483-1d9ccfcb24f25f51.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1665 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1804516-24b0b10ed6fe0589.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      666 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1804517-a351aec088fee066.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1804519-8384a9ead261d4c2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      654 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1804520-d124599967923052.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1555 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1804521-3c0d9f567e8f532f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1651 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1804522-00df902cd2d74ee3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1545 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1804523-d1768909b13b167e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1550 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1805363-0b85d71917ad09d1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1867 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1805366-670867516c6fc4bc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2225 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1805368-ea32c2db2ae57225.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2436 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1805369-ed98d3fcfafb5c43.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1600 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1805371-249c8c9b562ab371.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1234 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1805372-af4ebf4b19500b72.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1547 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1805400-c192be936d277ade.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1463 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1805402-75d0d93f31af620f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1837 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1805403-c003627a64768716.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2066 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1805406-252b45d443af20b3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3643 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1805409-8bc6cc9f1c5bc672.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      605 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1805880-0032024ea6b83563.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      638 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1805880-3fc6b30309a4370f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      604 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1806713-cf5feab23fc78a23.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1194 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1806762-08ff9eecdc03c554.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      639 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1806762-09f414995924db23.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1806762-0b7356ace200a5d3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1806762-2092fee9f6c87dc3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1409 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1806762-c3bfc71cb9bb94f3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      802 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1806762-daed3e27f58f0f6d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      990 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1809116-b65502f3b606b060.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      224 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1810393-5a7d379842c51d9b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      512 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1811605-9d23080d7e949c25.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1813085-cf24b204e95fd7f5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1814589-f3e7f554bee1c317.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1815771-ae0e4118c552f01e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      617 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1816076-ba39508e6ade529e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      376 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1816927-e17f4e596e611380.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      318 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1817313-c11481e6eed29ec2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2108 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1818725-96d698e22e648764.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2789 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1818734-d753bfae60ffd030.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      835 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1818736-98ea186a074056f4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      419 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1818845-05f8c3af5ea9abc7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2116 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1818846-d1a8c77d20659ad6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1819036-e2d24655c70d0aad.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      847 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1820333-356dcc8bf9f73fed.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      487 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1823258-9649b56a440b5ae1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      614 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1823258-9f93dbdc0fa8441d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      379 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1827431-2f078c13dfc9a02a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1831918-c70cf87ef086d871.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1832265-cb76ccf505c2d9d1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      455 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1833739-f962e8caf3e22068.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1836568-66d853a1f22c5530.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1839133-24570c9fbacb530d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1839577-1226d86ea0744055.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      229 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1840291-35af1ac7ba06e166.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1841486-425f367925f5e03f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      438 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1843609-8498b132222596b7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      617 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1844157-7808af9bcea0429d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2153 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1844194-48ae60db49f91bd4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1844207-x27a31f3403xfd7y.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1530 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1844461-08a8bdc5f613b88d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1809 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1844664-905cf6cad2e032a7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1848238-f6533644f7907358.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1054 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1848342-317c9e4afa65a3ff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1272 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1855080-08b28181b7cb2470.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1856881-277103af343187f1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1856904-101af15bb48eb3ca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1856962-2c87d541da61c727.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      295 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1858012-584267ada7e33f2c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1872732-7261816d0b170008.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1872733-2377f456a57ad32c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1720 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1872735-0989e51d2248ce1e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1324 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1872737-f8e1ad3b6705b766.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1872753-e2a934eac919ccde.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1083 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1872755-2c81d3267b89f124.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1105 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1873290-ff7f8e4cee15b75a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1878938-70ee2af6fdf66004.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1880252-51036d5353125e15.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1885753-51df25f3ff1d9ae8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1886017-bc2ad648d57101a2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1889936-78d6853b5212b8f1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1896125-b17a4d12730fe493.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      299 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1897280-e7065c4368a325ad.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1901207-13762f85b8a04481.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1901654-69b9f35d11cd0c75.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1926483-a77ab887e0e7f5c9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1929066-6e741c9182620a37.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1941020-cleanup-541a2d372a1cf4cd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      345 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1941020-f694395a9bcea72f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      495 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug-1951632-11272e49e2fa439d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug1828565-0790c4c60ba34100.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug_1526462-df9a3f3974d9040f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2375 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug_1543048_and_1668503-7ead4e15faaab778.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug_1674415-e8a7345aa2b05ab7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      279 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug_1688188-256e3572295231a1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      364 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/bug_1698900-f195125bf341d887.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/catalog-caching-12f2532cfb71325a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/catalog_project_id-519f5a70f9f7c4c6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/change_min_pool_retry_max-f5e7c8d315401426.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2745 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/convert-keystone-to-flask-80d980e239b662b0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      291 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/deprecate-endpoint-policy-cfg-option-d018acab72a398a0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1008 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/deprecate-json-formatted-policy-file-95f6307f88358f58.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/deprecate-memcache-token-persistence-eac88c80147ea241.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/deprecate-policies-api-b104fbd1d2367b1b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/deprecate-templated-catalog-driver-f811a6040abdc4a8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      575 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/deprecate-v2-apis-894284c17be881d2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1742 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/deprecated-as-of-mitaka-8534e43fa40c1d09.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      377 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/deprecated-as-of-newton-be1d8dbcc6bdc68f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/deprecated-as-of-ocata-a5b2f1e3e39f818e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      481 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/deprecated-as-of-pike-506f9aca91674550.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1158 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/deprecated-as-of-queens-8ad7f826e4f08f57.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      572 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/deprecated-as-of-rocky-60b2fa05d07d3a28.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/deprecated-as-of-stein-0166965502cb3be2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/deprecated-as-of-train-de3fe41ff2251385.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      628 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/deprecated-socket_timeout-option-d3358b4f2310706c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      515 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/domain-level-limit-support-60e1e330d06227ed.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/dont-enforce-get-s3tokens-ec2tokens-62b90b199e8075d8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      415 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/drop-project-id-fk-b683b414e1585be8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/drop-python-3-6-and-3-7-dc90b86cedced92b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/enable-filter-idp-d0135f4615178cfc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      445 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/enable-inherit-on-default-54ac435230261a6a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/endpoints-from-endpoint_group-project-association-7271fba600322fb6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/eventlet-cleanup-f35fc5f83c16ea1c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1395 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/extensions-to-core-a0d270d216d47276.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      300 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/federation-group-ids-mapping-6c56120d65a5cb22.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/filter-mappings-by-entity-77162a146d375385.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/httpd-keystone-d51b7335559b09c8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/identity_driver_new_change_password_method-e8c0e06795bca2d8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      463 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/immutable-resource-options-bug-1807751-acc1e3c689484337.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      408 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/impl-templated-catalog-1d8f6333726b34f8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      641 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/implied-roles-026f401adc0f7fb6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/implied-roles-stable-8b293e187c5620ad.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/insecure_reponse-2a168230709bc8e7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/integrate-osprofiler-ad0e16a542b12899.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      775 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/is-admin-24b34238c83b3a82.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/ldap-conn-pool-enabled-90df94652f1ded53.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/ldap-emulation-91c4d535eb9c3d10.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      567 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/limits-api-refactor-05abf9e6c2e75852.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/list_limit-ldap-support-5d31d51466fc49a6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/list_role_assignment_names-33aedc1e521230b6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      572 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/mapping_populate-521d92445505b8a3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      471 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/max-password-length-truncation-and-warning-bd69090315ec18a7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/migration_squash-f655329ddad7fc2a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      312 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/no-default-domain-2161ada44bf7a3f7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/notify-on-user-group-membership-8c0136ee0484e255.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/oauth1-headers-content-type-9a9245d9bbec8f8e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      758 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/oslo.cache-a9ce47bfa8809efa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      242 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/password-created_at-nullable-b3c284be50d93ef5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/policy_new_federated_projects_for_user-dcd7bd148efef049.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/pre-cache-tokens-73450934918af26b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      750 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/project-tags-1e72a6779d9d02c5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/projects_as_domains-3ea8a58b4c2965e1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/python3-support-e4189e0a1a6e2e4f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/randomize_urls-c0c19f48b2bfa299.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      200 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/remove-db_sync-extension-opt-2ab1f29340281215.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/remove-legacy-migrations-647f60019c8dd9e8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/remove-sqlalchemy-migrate-a4fa47685c7e28c6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      884 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/remove-token-auth-middleware-5ea3b3734ce1d9e6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/remove-trust-auth-support-from-v2-de316c9ba46d556d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2467 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/removed-as-of-mitaka-9ff14f87d0b98e7e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1186 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/removed-as-of-newton-721c06b5dcb1b34a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4550 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/removed-as-of-ocata-436bb4b839e74494.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2678 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/removed-as-of-pike-deadbeefdeadbeef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      718 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/removed-as-of-queens-94c04e88c08f89aa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1104 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/removed-as-of-rocky-f44c3ba7c3e73d01.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1504 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/removed-as-of-stein-5eb23253b72ab54e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      656 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/removed-as-of-train-92b2942a680eb859.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/removed-as-of-ussuri-d2f6ef8901ef54ed.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/request_context-e143ba9c446a5952.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      640 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/resource-backend-sql-only-03154d8712b36bd0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/resource-driver-33793dd5080ee4d2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      544 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/revert-v2-token-issued-for-non-default-domain-25ea5337f158ef13.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/s3-aws-v4-c6cb75ce8d2289d4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1578 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/scope-and-default-roles-a733c235731bb558.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      662 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/support_encrypted_credentials_at_rest-93dcb67b3508e91a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1230 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/switch-to-alembic-1fa5248f0ce824ae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/tenant_id_to_project_id-42d95d93011785cb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/token-formatter-ec58aba00fa83706.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/token-provider-refactor-a3a64146807daf36.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      521 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/token_expiration_to_match_application_credential-56d058355a9f240d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      474 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/totp-40d93231714c6a20.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      743 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/unified-limit-api-improvment-b34d18769d18a0a7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      326 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/use-correct-inspect-8142e317c1e39c2a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/use-pyldap-6e811c28bf350d6d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/use-python-ldap-0318ff7798bdd98d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/v2-dep-d6e7ab2d08119549.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/v3-endpoints-in-v2-list-b0439816938713d6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/v9FederationDriver-cbebcf5f97e1eae2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/notes/x509-auth-df0a229780b8e3ff.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.320302 keystone-25.0.0.0rc1/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/source/2023.2.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.320302 keystone-25.0.0.0rc1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.320302 keystone-25.0.0.0rc1/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8945 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      862 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/source/liberty.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.056236 keystone-25.0.0.0rc1/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.056236 keystone-25.0.0.0rc1/releasenotes/source/locale/en_GB/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.320302 keystone-25.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    94656 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.056236 keystone-25.0.0.0rc1/releasenotes/source/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.320302 keystone-25.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2728 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.056236 keystone-25.0.0.0rc1/releasenotes/source/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.320302 keystone-25.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   197755 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.056236 keystone-25.0.0.0rc1/releasenotes/source/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.320302 keystone-25.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5029 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      674 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      662 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/reno.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1415 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4896 2024-03-19 10:21:05.324303 keystone-25.0.0.0rc1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-19 10:21:05.320302 keystone-25.0.0.0rc1/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2479 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/tools/cover.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      645 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/tools/fast8.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     8816 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/tools/sample_data.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2142 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/tools/test-setup.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5557 2024-03-19 10:20:35.000000 keystone-25.0.0.0rc1/tox.ini
```

### Comparing `keystone-25.0.0/.mailmap` & `keystone-25.0.0.0rc1/.mailmap`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/.zuul.yaml` & `keystone-25.0.0.0rc1/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/AUTHORS` & `keystone-25.0.0.0rc1/AUTHORS`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/CONTRIBUTING.rst` & `keystone-25.0.0.0rc1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/ChangeLog` & `keystone-25.0.0.0rc1/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGES
 =======
 
-25.0.0
-------
+25.0.0.0rc1
+-----------
 
 * Deprecate templated catalog driver
 * Update regex to detect closed branch
 * Add ability to create users and projects from keystone-manage
 * Remove unused old job templates and experimental jobs
 * api-ref: Fix indentation
 * Drop keystone-dsvm-functional-federation-opensuse15 jobs
```

### Comparing `keystone-25.0.0/HACKING.rst` & `keystone-25.0.0.0rc1/HACKING.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/LICENSE` & `keystone-25.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/PKG-INFO` & `keystone-25.0.0.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keystone
-Version: 25.0.0
+Version: 25.0.0.0rc1
 Summary: OpenStack Identity
 Home-page: https://docs.openstack.org/keystone/latest
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ==================
         OpenStack Keystone
```

### Comparing `keystone-25.0.0/README.rst` & `keystone-25.0.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/conf.py` & `keystone-25.0.0.0rc1/api-ref/source/conf.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v2-ext/ksec2-admin.inc` & `keystone-25.0.0.0rc1/api-ref/source/v2-ext/ksec2-admin.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v2-ext/parameters.yaml` & `keystone-25.0.0.0rc1/api-ref/source/v2-ext/parameters.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v2-ext/samples/OS-KSEC2/authenticate-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v2-ext/samples/OS-KSEC2/authenticate-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/application-credentials.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3/application-credentials.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/authenticate-v3.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3/authenticate-v3.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/credentials.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3/credentials.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/domains-config-v3.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3/domains-config-v3.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/domains.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3/domains.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/groups.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3/groups.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/index.rst` & `keystone-25.0.0.0rc1/api-ref/source/v3/index.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/inherit.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3/inherit.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/parameters.yaml` & `keystone-25.0.0.0rc1/api-ref/source/v3/parameters.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/policies.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3/policies.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/project-tags.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3/project-tags.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/projects.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3/projects.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/regions-v3.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3/regions-v3.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/roles.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3/roles.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/application-credential-create-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/application-credential-create-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/application-credential-get-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/application-credential-get-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/application-credential-list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/application-credential-list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/auth-application-credential-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/auth-application-credential-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/auth-password-explicit-unscoped-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/auth-password-explicit-unscoped-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/auth-password-project-scoped-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/auth-password-project-scoped-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/auth-password-unscoped-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/auth-password-unscoped-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/auth-token-scoped-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/auth-token-scoped-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/create-role-inferences-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/create-role-inferences-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/credential-show-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/credential-show-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/credentials-list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/credentials-list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/domain-group-roles-list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/domain-group-roles-list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/domain-user-roles-list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/domain-user-roles-list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/domains-list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/domains-list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/endpoints-list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/endpoints-list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/get-available-domain-scopes-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/get-available-domain-scopes-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/get-available-project-scopes-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/get-available-project-scopes-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/get-role-inferences-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/get-role-inferences-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/get-service-catalog-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/get-service-catalog-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/group-roles-domain-list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/group-roles-domain-list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/group-users-list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/group-users-list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/groups-list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/groups-list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/identity-versions-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/identity-versions-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/limits-create-request.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/limits-create-request.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/limits-create-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/limits-create-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/limits-list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/limits-list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/limits-update-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/limits-update-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/list-implied-roles-for-role-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/list-implied-roles-for-role-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/policies-list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/policies-list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/project-group-roles-list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/project-group-roles-list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/project-show-parents-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/project-show-parents-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/project-show-subtree-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/project-show-subtree-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/project-tags-update-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/project-tags-update-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/projects-list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/projects-list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/registered-limits-create-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/registered-limits-create-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/registered-limits-list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/registered-limits-list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/role-assignments-effective-list-include-names-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/role-assignments-effective-list-include-names-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/role-assignments-effective-list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/role-assignments-effective-list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/role-assignments-list-include-subtree-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/role-assignments-list-include-subtree-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/role-assignments-list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/role-assignments-list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/role-inferences-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/role-inferences-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/roles-list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/roles-list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/services-list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/services-list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/user-create-request.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/user-create-request.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/user-create-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/user-create-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/user-groups-list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/user-groups-list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/user-projects-list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/user-projects-list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/user-roles-domain-list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/user-roles-domain-list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/admin/users-list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/admin/users-list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/auth/responses/domain-scoped-password.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/responses/domain-scoped-password.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/auth/responses/domain-scoped-token.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/responses/domain-scoped-token.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/auth/responses/project-scoped-password-totp.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/responses/project-scoped-password-totp.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/auth/responses/project-scoped-password.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/responses/project-scoped-password.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/auth/responses/project-scoped-token.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/responses/project-scoped-token.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/auth/responses/system-scoped-password.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/responses/system-scoped-password.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/auth/responses/system-scoped-token.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/responses/system-scoped-token.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/samples/auth/responses/unscoped-password.json` & `keystone-25.0.0.0rc1/api-ref/source/v3/samples/auth/responses/unscoped-password.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/service-catalog.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3/service-catalog.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/status.yaml` & `keystone-25.0.0.0rc1/api-ref/source/v3/status.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/system-roles.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3/system-roles.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/unified_limits.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3/unified_limits.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3/users.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3/users.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/endpoint-policy.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/endpoint-policy.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/ep-filter.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/ep-filter.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/federation/assertion/assertion.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/assertion/assertion.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/federation/assertion/parameters.yaml` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/assertion/parameters.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/federation/assertion/samples/ecp-saml-assertion-response.xml` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/assertion/samples/ecp-saml-assertion-response.xml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/federation/assertion/samples/metadata-response.xml` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/assertion/samples/metadata-response.xml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/federation/assertion/samples/saml-assertion-response.xml` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/assertion/samples/saml-assertion-response.xml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/federation/auth/auth.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/auth/auth.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/federation/auth/parameters.yaml` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/auth/parameters.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/federation/auth/samples/scoped-token-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/auth/samples/scoped-token-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/federation/auth/samples/unscoped-token-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/auth/samples/unscoped-token-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/federation/identity-provider/idp.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/identity-provider/idp.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/federation/identity-provider/parameters.yaml` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/identity-provider/parameters.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/federation/identity-provider/samples/list-protocol-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/identity-provider/samples/list-protocol-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/federation/identity-provider/samples/list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/identity-provider/samples/list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/federation/mapping/mapping.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/mapping/mapping.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/federation/mapping/parameters.yaml` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/mapping/parameters.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/federation/mapping/samples/create-request.json` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/mapping/samples/create-request.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/federation/mapping/samples/create-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/mapping/samples/create-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/federation/mapping/samples/get-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/mapping/samples/get-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/federation/mapping/samples/list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/mapping/samples/list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/federation/mapping/samples/update-request.json` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/mapping/samples/update-request.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/federation/mapping/samples/update-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/mapping/samples/update-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/federation/projects-domains/parameters.yaml` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/projects-domains/parameters.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/federation/projects-domains/projects-domains.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/projects-domains/projects-domains.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/federation/projects-domains/samples/project-list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/projects-domains/samples/project-list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/federation/service-provider/parameters.yaml` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/service-provider/parameters.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/federation/service-provider/samples/list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/service-provider/samples/list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/federation/service-provider/sp.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation/service-provider/sp.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/federation.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/federation.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/index.rst` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/index.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/oauth.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/oauth.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/oauth2.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/oauth2.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/parameters.yaml` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/parameters.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/revoke.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/revoke.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/samples/OS-ENDPOINT-POLICY/policy-endpoint-associations-list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-ENDPOINT-POLICY/policy-endpoint-associations-list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/samples/OS-EP-FILTER/endpoint-groups-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-EP-FILTER/endpoint-groups-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/samples/OS-EP-FILTER/list-associations-by-endpoint-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-EP-FILTER/list-associations-by-endpoint-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/samples/OS-EP-FILTER/list-associations-by-project-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-EP-FILTER/list-associations-by-project-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/samples/OS-EP-FILTER/list-service-endpoints.json` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-EP-FILTER/list-service-endpoints.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/samples/OS-OAUTH1/access-token-roles-list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-OAUTH1/access-token-roles-list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/samples/OS-OAUTH1/access-tokens-list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-OAUTH1/access-tokens-list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/samples/OS-OAUTH1/consumers-list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-OAUTH1/consumers-list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/samples/OS-REVOKE/list-revoke-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-REVOKE/list-revoke-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/samples/OS-SIMPLE-CERT/show-ca-certificate-response.txt` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-SIMPLE-CERT/show-ca-certificate-response.txt`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/samples/OS-SIMPLE-CERT/show-signing-certificate-response.txt` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-SIMPLE-CERT/show-signing-certificate-response.txt`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/samples/OS-TRUST/trust-auth-redelegated-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-TRUST/trust-auth-redelegated-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/samples/OS-TRUST/trust-auth-trust-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-TRUST/trust-auth-trust-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/samples/OS-TRUST/trust-create-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-TRUST/trust-create-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/samples/OS-TRUST/trust-get-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-TRUST/trust-get-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/samples/OS-TRUST/trust-list-response.json` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/samples/OS-TRUST/trust-list-response.json`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/simple-cert.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/simple-cert.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/api-ref/source/v3-ext/trust.inc` & `keystone-25.0.0.0rc1/api-ref/source/v3-ext/trust.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/bindep.txt` & `keystone-25.0.0.0rc1/bindep.txt`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/devstack/files/federation/attribute-map.xml` & `keystone-25.0.0.0rc1/devstack/files/federation/attribute-map.xml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/devstack/files/federation/shib_apache_handler.txt` & `keystone-25.0.0.0rc1/devstack/files/federation/shib_apache_handler.txt`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/devstack/files/federation/shibboleth2.xml` & `keystone-25.0.0.0rc1/devstack/files/federation/shibboleth2.xml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/devstack/files/oidc/apache_oidc.conf` & `keystone-25.0.0.0rc1/devstack/files/oidc/apache_oidc.conf`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/devstack/lib/federation.sh` & `keystone-25.0.0.0rc1/devstack/lib/federation.sh`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/devstack/lib/oidc.sh` & `keystone-25.0.0.0rc1/devstack/lib/oidc.sh`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/devstack/lib/scope.sh` & `keystone-25.0.0.0rc1/devstack/lib/scope.sh`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/devstack/plugin.sh` & `keystone-25.0.0.0rc1/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/devstack/tools/oidc/docker-compose.yaml` & `keystone-25.0.0.0rc1/devstack/tools/oidc/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/devstack/tools/oidc/setup_keycloak_client.py` & `keystone-25.0.0.0rc1/devstack/tools/oidc/setup_keycloak_client.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/Makefile` & `keystone-25.0.0.0rc1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/requirements.txt` & `keystone-25.0.0.0rc1/doc/requirements.txt`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/_static/horizon-login-idp.png` & `keystone-25.0.0.0rc1/doc/source/_static/horizon-login-idp.png`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/_static/horizon-login-sp.png` & `keystone-25.0.0.0rc1/doc/source/_static/horizon-login-sp.png`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/_static/support-matrix.css` & `keystone-25.0.0.0rc1/doc/source/_static/support-matrix.css`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/auth-totp.rst` & `keystone-25.0.0.0rc1/doc/source/admin/auth-totp.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/bootstrap.rst` & `keystone-25.0.0.0rc1/doc/source/admin/bootstrap.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/caching-layer.inc` & `keystone-25.0.0.0rc1/doc/source/admin/caching-layer.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/case-insensitive.rst` & `keystone-25.0.0.0rc1/doc/source/admin/case-insensitive.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/cli-manage-projects-users-and-roles.rst` & `keystone-25.0.0.0rc1/doc/source/admin/cli-manage-projects-users-and-roles.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/configuration.rst` & `keystone-25.0.0.0rc1/doc/source/admin/configuration.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/configure-https.rst` & `keystone-25.0.0.0rc1/doc/source/admin/configure-https.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/configure_tokenless_x509.rst` & `keystone-25.0.0.0rc1/doc/source/admin/configure_tokenless_x509.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/credential-encryption.rst` & `keystone-25.0.0.0rc1/doc/source/admin/credential-encryption.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/domain-specific-config.inc` & `keystone-25.0.0.0rc1/doc/source/admin/domain-specific-config.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/endpoint-filtering.inc` & `keystone-25.0.0.0rc1/doc/source/admin/endpoint-filtering.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/endpoint-policy.inc` & `keystone-25.0.0.0rc1/doc/source/admin/endpoint-policy.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/event_notifications.rst` & `keystone-25.0.0.0rc1/doc/source/admin/event_notifications.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/external-authentication.rst` & `keystone-25.0.0.0rc1/doc/source/admin/external-authentication.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/federation/configure_federation.rst` & `keystone-25.0.0.0rc1/doc/source/admin/federation/configure_federation.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/federation/introduction.rst` & `keystone-25.0.0.0rc1/doc/source/admin/federation/introduction.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/federation/mapping_combinations.rst` & `keystone-25.0.0.0rc1/doc/source/admin/federation/mapping_combinations.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/federation/mellon.inc` & `keystone-25.0.0.0rc1/doc/source/admin/federation/mellon.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/federation/openidc.inc` & `keystone-25.0.0.0rc1/doc/source/admin/federation/openidc.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/federation/shibboleth.inc` & `keystone-25.0.0.0rc1/doc/source/admin/federation/shibboleth.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/fernet-token-faq.rst` & `keystone-25.0.0.0rc1/doc/source/admin/fernet-token-faq.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/figures/keystone-federation.png` & `keystone-25.0.0.0rc1/doc/source/admin/figures/keystone-federation.png`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/figures/keystone-federation.svg` & `keystone-25.0.0.0rc1/doc/source/admin/figures/keystone-federation.svg`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/identity-concepts.rst` & `keystone-25.0.0.0rc1/doc/source/admin/identity-concepts.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/identity-sources.rst` & `keystone-25.0.0.0rc1/doc/source/admin/identity-sources.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/identity-support-matrix.ini` & `keystone-25.0.0.0rc1/doc/source/admin/identity-support-matrix.ini`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/integrate-with-ldap.inc` & `keystone-25.0.0.0rc1/doc/source/admin/integrate-with-ldap.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/jws-key-rotation.rst` & `keystone-25.0.0.0rc1/doc/source/admin/jws-key-rotation.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/limit-list-size.inc` & `keystone-25.0.0.0rc1/doc/source/admin/limit-list-size.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/logging.inc` & `keystone-25.0.0.0rc1/doc/source/admin/logging.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/manage-services.rst` & `keystone-25.0.0.0rc1/doc/source/admin/manage-services.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/manage-trusts.rst` & `keystone-25.0.0.0rc1/doc/source/admin/manage-trusts.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/multi-factor-authentication.rst` & `keystone-25.0.0.0rc1/doc/source/admin/multi-factor-authentication.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/oauth1.rst` & `keystone-25.0.0.0rc1/doc/source/admin/oauth1.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/oauth2-usage-guide.rst` & `keystone-25.0.0.0rc1/doc/source/admin/oauth2-usage-guide.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/performance.inc` & `keystone-25.0.0.0rc1/doc/source/admin/performance.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/resource-options.rst` & `keystone-25.0.0.0rc1/doc/source/admin/resource-options.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/security-compliance.inc` & `keystone-25.0.0.0rc1/doc/source/admin/security-compliance.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/service-api-protection.rst` & `keystone-25.0.0.0rc1/doc/source/admin/service-api-protection.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/token-provider.rst` & `keystone-25.0.0.0rc1/doc/source/admin/token-provider.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/token-support-matrix.ini` & `keystone-25.0.0.0rc1/doc/source/admin/token-support-matrix.ini`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/tokens-overview.rst` & `keystone-25.0.0.0rc1/doc/source/admin/tokens-overview.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/troubleshoot.inc` & `keystone-25.0.0.0rc1/doc/source/admin/troubleshoot.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/unified-limits.rst` & `keystone-25.0.0.0rc1/doc/source/admin/unified-limits.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/upgrading.rst` & `keystone-25.0.0.0rc1/doc/source/admin/upgrading.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/admin/url-safe-naming.inc` & `keystone-25.0.0.0rc1/doc/source/admin/url-safe-naming.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/api_curl_examples.rst` & `keystone-25.0.0.0rc1/doc/source/api_curl_examples.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/cli/commands.rst` & `keystone-25.0.0.0rc1/doc/source/cli/commands.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/cli/index.rst` & `keystone-25.0.0.0rc1/doc/source/cli/index.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/cli/keystone-manage.rst` & `keystone-25.0.0.0rc1/doc/source/cli/keystone-manage.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/cli/keystone-status.rst` & `keystone-25.0.0.0rc1/doc/source/cli/keystone-status.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/conf.py` & `keystone-25.0.0.0rc1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/configuration/config-options.rst` & `keystone-25.0.0.0rc1/doc/source/configuration/config-options.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/configuration/index.rst` & `keystone-25.0.0.0rc1/doc/source/configuration/index.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/configuration/policy.rst` & `keystone-25.0.0.0rc1/doc/source/configuration/policy.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/contributor/api_change_tutorial.rst` & `keystone-25.0.0.0rc1/doc/source/contributor/api_change_tutorial.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/contributor/architecture.rst` & `keystone-25.0.0.0rc1/doc/source/contributor/architecture.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/contributor/auth-plugins.rst` & `keystone-25.0.0.0rc1/doc/source/contributor/auth-plugins.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/contributor/caching-layer.rst` & `keystone-25.0.0.0rc1/doc/source/contributor/caching-layer.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/contributor/contributing.rst` & `keystone-25.0.0.0rc1/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/contributor/database-migrations.rst` & `keystone-25.0.0.0rc1/doc/source/contributor/database-migrations.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/contributor/developing-drivers.rst` & `keystone-25.0.0.0rc1/doc/source/contributor/developing-drivers.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/contributor/doctor-checks.rst` & `keystone-25.0.0.0rc1/doc/source/contributor/doctor-checks.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/contributor/filtering-responsibilities.rst` & `keystone-25.0.0.0rc1/doc/source/contributor/filtering-responsibilities.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/contributor/how-can-i-help.rst` & `keystone-25.0.0.0rc1/doc/source/contributor/how-can-i-help.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/contributor/http-api.rst` & `keystone-25.0.0.0rc1/doc/source/contributor/http-api.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/contributor/id-manage.rst` & `keystone-25.0.0.0rc1/doc/source/contributor/id-manage.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/contributor/index.rst` & `keystone-25.0.0.0rc1/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/contributor/list-truncation.rst` & `keystone-25.0.0.0rc1/doc/source/contributor/list-truncation.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/contributor/programming-exercises.rst` & `keystone-25.0.0.0rc1/doc/source/contributor/programming-exercises.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/contributor/proposing-features.rst` & `keystone-25.0.0.0rc1/doc/source/contributor/proposing-features.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/contributor/release-notes.rst` & `keystone-25.0.0.0rc1/doc/source/contributor/release-notes.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/contributor/service-catalog.rst` & `keystone-25.0.0.0rc1/doc/source/contributor/service-catalog.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/contributor/services.rst` & `keystone-25.0.0.0rc1/doc/source/contributor/services.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/contributor/set-up-keystone.rst` & `keystone-25.0.0.0rc1/doc/source/contributor/set-up-keystone.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/contributor/testing-keystone.rst` & `keystone-25.0.0.0rc1/doc/source/contributor/testing-keystone.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/contributor/vision-reflection.rst` & `keystone-25.0.0.0rc1/doc/source/contributor/vision-reflection.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/getting-started/architecture.rst` & `keystone-25.0.0.0rc1/doc/source/getting-started/architecture.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/getting-started/community.rst` & `keystone-25.0.0.0rc1/doc/source/getting-started/community.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/getting-started/policy_mapping.rst` & `keystone-25.0.0.0rc1/doc/source/getting-started/policy_mapping.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/index.rst` & `keystone-25.0.0.0rc1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/install/common/get-started-identity.inc` & `keystone-25.0.0.0rc1/doc/source/install/common/get-started-identity.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/install/common/keystone-users.inc` & `keystone-25.0.0.0rc1/doc/source/install/common/keystone-users.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/install/common/openrc.inc` & `keystone-25.0.0.0rc1/doc/source/install/common/openrc.inc`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/install/index-obs.rst` & `keystone-25.0.0.0rc1/doc/source/install/index-obs.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/install/index-rdo.rst` & `keystone-25.0.0.0rc1/doc/source/install/index-rdo.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/install/index-ubuntu.rst` & `keystone-25.0.0.0rc1/doc/source/install/index-ubuntu.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/install/index.rst` & `keystone-25.0.0.0rc1/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/install/keystone-install-obs.rst` & `keystone-25.0.0.0rc1/doc/source/install/keystone-install-obs.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/install/keystone-install-rdo.rst` & `keystone-25.0.0.0rc1/doc/source/install/keystone-install-rdo.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/install/keystone-install-ubuntu.rst` & `keystone-25.0.0.0rc1/doc/source/install/keystone-install-ubuntu.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/install/keystone-verify-obs.rst` & `keystone-25.0.0.0rc1/doc/source/install/keystone-verify-obs.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/install/keystone-verify-rdo.rst` & `keystone-25.0.0.0rc1/doc/source/install/keystone-verify-rdo.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/install/keystone-verify-ubuntu.rst` & `keystone-25.0.0.0rc1/doc/source/install/keystone-verify-ubuntu.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/user/application_credentials.rst` & `keystone-25.0.0.0rc1/doc/source/user/application_credentials.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/user/index.rst` & `keystone-25.0.0.0rc1/doc/source/user/index.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/user/json_home.rst` & `keystone-25.0.0.0rc1/doc/source/user/json_home.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/user/multi-factor-authentication.rst` & `keystone-25.0.0.0rc1/doc/source/user/multi-factor-authentication.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/user/supported_clients.rst` & `keystone-25.0.0.0rc1/doc/source/user/supported_clients.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/doc/source/user/trusts.rst` & `keystone-25.0.0.0rc1/doc/source/user/trusts.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/etc/default_catalog.templates` & `keystone-25.0.0.0rc1/etc/default_catalog.templates`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/etc/logging.conf.sample` & `keystone-25.0.0.0rc1/etc/logging.conf.sample`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/etc/sso_callback_template.html` & `keystone-25.0.0.0rc1/etc/sso_callback_template.html`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/examples/pki/certs/cacert.pem` & `keystone-25.0.0.0rc1/examples/pki/certs/cacert.pem`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/examples/pki/certs/middleware.pem` & `keystone-25.0.0.0rc1/examples/pki/certs/middleware.pem`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/examples/pki/certs/signing_cert.pem` & `keystone-25.0.0.0rc1/examples/pki/certs/signing_cert.pem`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/examples/pki/certs/ssl_cert.pem` & `keystone-25.0.0.0rc1/examples/pki/certs/ssl_cert.pem`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/examples/pki/private/cakey.pem` & `keystone-25.0.0.0rc1/examples/pki/private/cakey.pem`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/examples/pki/private/signing_key.pem` & `keystone-25.0.0.0rc1/examples/pki/private/signing_key.pem`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/examples/pki/private/ssl_key.pem` & `keystone-25.0.0.0rc1/examples/pki/private/ssl_key.pem`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/httpd/keystone-uwsgi-admin.ini` & `keystone-25.0.0.0rc1/httpd/keystone-uwsgi-admin.ini`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/httpd/keystone-uwsgi-public.ini` & `keystone-25.0.0.0rc1/httpd/keystone-uwsgi-public.ini`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/httpd/wsgi-keystone.conf` & `keystone-25.0.0.0rc1/httpd/wsgi-keystone.conf`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/__init__.py` & `keystone-25.0.0.0rc1/keystone/api/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/_shared/EC2_S3_Resource.py` & `keystone-25.0.0.0rc1/keystone/api/_shared/EC2_S3_Resource.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/_shared/authentication.py` & `keystone-25.0.0.0rc1/keystone/api/_shared/authentication.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/_shared/implied_roles.py` & `keystone-25.0.0.0rc1/keystone/api/_shared/implied_roles.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/_shared/json_home_relations.py` & `keystone-25.0.0.0rc1/keystone/api/_shared/json_home_relations.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/_shared/saml.py` & `keystone-25.0.0.0rc1/keystone/api/_shared/saml.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/auth.py` & `keystone-25.0.0.0rc1/keystone/api/auth.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/credentials.py` & `keystone-25.0.0.0rc1/keystone/api/credentials.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/discovery.py` & `keystone-25.0.0.0rc1/keystone/api/discovery.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/domains.py` & `keystone-25.0.0.0rc1/keystone/api/domains.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/ec2tokens.py` & `keystone-25.0.0.0rc1/keystone/api/ec2tokens.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/endpoints.py` & `keystone-25.0.0.0rc1/keystone/api/endpoints.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/groups.py` & `keystone-25.0.0.0rc1/keystone/api/groups.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/limits.py` & `keystone-25.0.0.0rc1/keystone/api/limits.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/os_ep_filter.py` & `keystone-25.0.0.0rc1/keystone/api/os_ep_filter.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/os_federation.py` & `keystone-25.0.0.0rc1/keystone/api/os_federation.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/os_inherit.py` & `keystone-25.0.0.0rc1/keystone/api/os_inherit.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/os_oauth1.py` & `keystone-25.0.0.0rc1/keystone/api/os_oauth1.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/os_oauth2.py` & `keystone-25.0.0.0rc1/keystone/api/os_oauth2.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/os_revoke.py` & `keystone-25.0.0.0rc1/keystone/api/os_revoke.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/os_simple_cert.py` & `keystone-25.0.0.0rc1/keystone/api/os_simple_cert.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/policy.py` & `keystone-25.0.0.0rc1/keystone/api/policy.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/projects.py` & `keystone-25.0.0.0rc1/keystone/api/projects.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/regions.py` & `keystone-25.0.0.0rc1/keystone/api/regions.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/registered_limits.py` & `keystone-25.0.0.0rc1/keystone/api/registered_limits.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/role_assignments.py` & `keystone-25.0.0.0rc1/keystone/api/role_assignments.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/role_inferences.py` & `keystone-25.0.0.0rc1/keystone/api/role_inferences.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/roles.py` & `keystone-25.0.0.0rc1/keystone/api/roles.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/s3tokens.py` & `keystone-25.0.0.0rc1/keystone/api/s3tokens.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/services.py` & `keystone-25.0.0.0rc1/keystone/api/services.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/system.py` & `keystone-25.0.0.0rc1/keystone/api/system.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/trusts.py` & `keystone-25.0.0.0rc1/keystone/api/trusts.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/api/users.py` & `keystone-25.0.0.0rc1/keystone/api/users.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/application_credential/__init__.py` & `keystone-25.0.0.0rc1/keystone/application_credential/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/application_credential/backends/base.py` & `keystone-25.0.0.0rc1/keystone/application_credential/backends/base.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/application_credential/backends/sql.py` & `keystone-25.0.0.0rc1/keystone/application_credential/backends/sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/application_credential/core.py` & `keystone-25.0.0.0rc1/keystone/application_credential/core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/application_credential/schema.py` & `keystone-25.0.0.0rc1/keystone/application_credential/schema.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/assignment/__init__.py` & `keystone-25.0.0.0rc1/keystone/assignment/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/assignment/backends/base.py` & `keystone-25.0.0.0rc1/keystone/assignment/backends/base.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/assignment/backends/sql.py` & `keystone-25.0.0.0rc1/keystone/assignment/backends/sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/assignment/core.py` & `keystone-25.0.0.0rc1/keystone/assignment/core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/assignment/role_backends/base.py` & `keystone-25.0.0.0rc1/keystone/assignment/role_backends/base.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/assignment/role_backends/resource_options.py` & `keystone-25.0.0.0rc1/keystone/assignment/role_backends/resource_options.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/assignment/role_backends/sql.py` & `keystone-25.0.0.0rc1/keystone/assignment/role_backends/sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/assignment/role_backends/sql_model.py` & `keystone-25.0.0.0rc1/keystone/assignment/role_backends/sql_model.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/assignment/schema.py` & `keystone-25.0.0.0rc1/keystone/assignment/schema.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/auth/__init__.py` & `keystone-25.0.0.0rc1/keystone/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/auth/core.py` & `keystone-25.0.0.0rc1/keystone/auth/core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/auth/plugins/__init__.py` & `keystone-25.0.0.0rc1/keystone/auth/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/auth/plugins/application_credential.py` & `keystone-25.0.0.0rc1/keystone/auth/plugins/application_credential.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/auth/plugins/base.py` & `keystone-25.0.0.0rc1/keystone/auth/plugins/base.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/auth/plugins/core.py` & `keystone-25.0.0.0rc1/keystone/auth/plugins/core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/auth/plugins/external.py` & `keystone-25.0.0.0rc1/keystone/auth/plugins/external.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/auth/plugins/mapped.py` & `keystone-25.0.0.0rc1/keystone/auth/plugins/mapped.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/auth/plugins/oauth1.py` & `keystone-25.0.0.0rc1/keystone/auth/plugins/oauth1.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/auth/plugins/password.py` & `keystone-25.0.0.0rc1/keystone/auth/plugins/password.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/auth/plugins/token.py` & `keystone-25.0.0.0rc1/keystone/auth/plugins/token.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/auth/plugins/totp.py` & `keystone-25.0.0.0rc1/keystone/auth/plugins/totp.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/auth/schema.py` & `keystone-25.0.0.0rc1/keystone/auth/schema.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/catalog/__init__.py` & `keystone-25.0.0.0rc1/keystone/catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/catalog/backends/base.py` & `keystone-25.0.0.0rc1/keystone/catalog/backends/base.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/catalog/backends/sql.py` & `keystone-25.0.0.0rc1/keystone/catalog/backends/sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/catalog/backends/templated.py` & `keystone-25.0.0.0rc1/keystone/catalog/backends/templated.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/catalog/core.py` & `keystone-25.0.0.0rc1/keystone/catalog/core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/catalog/schema.py` & `keystone-25.0.0.0rc1/keystone/catalog/schema.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/cmd/bootstrap.py` & `keystone-25.0.0.0rc1/keystone/cmd/bootstrap.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/cmd/cli.py` & `keystone-25.0.0.0rc1/keystone/cmd/cli.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/cmd/doctor/__init__.py` & `keystone-25.0.0.0rc1/keystone/cmd/doctor/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/cmd/doctor/caching.py` & `keystone-25.0.0.0rc1/keystone/cmd/doctor/caching.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/cmd/doctor/credential.py` & `keystone-25.0.0.0rc1/keystone/cmd/doctor/credential.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/cmd/doctor/database.py` & `keystone-25.0.0.0rc1/keystone/cmd/doctor/database.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/cmd/doctor/debug.py` & `keystone-25.0.0.0rc1/keystone/cmd/doctor/debug.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/cmd/doctor/federation.py` & `keystone-25.0.0.0rc1/keystone/cmd/doctor/federation.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/cmd/doctor/ldap.py` & `keystone-25.0.0.0rc1/keystone/cmd/doctor/ldap.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/cmd/doctor/security_compliance.py` & `keystone-25.0.0.0rc1/keystone/cmd/doctor/security_compliance.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/cmd/doctor/tokens.py` & `keystone-25.0.0.0rc1/keystone/cmd/doctor/tokens.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/cmd/doctor/tokens_fernet.py` & `keystone-25.0.0.0rc1/keystone/cmd/doctor/tokens_fernet.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/cmd/idutils.py` & `keystone-25.0.0.0rc1/keystone/cmd/idutils.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/cmd/manage.py` & `keystone-25.0.0.0rc1/keystone/cmd/manage.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/cmd/status.py` & `keystone-25.0.0.0rc1/keystone/cmd/status.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/authorization.py` & `keystone-25.0.0.0rc1/keystone/common/authorization.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/cache/__init__.py` & `keystone-25.0.0.0rc1/keystone/common/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/cache/_context_cache.py` & `keystone-25.0.0.0rc1/keystone/common/cache/_context_cache.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/cache/core.py` & `keystone-25.0.0.0rc1/keystone/common/cache/core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/context.py` & `keystone-25.0.0.0rc1/keystone/common/context.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/driver_hints.py` & `keystone-25.0.0.0rc1/keystone/common/driver_hints.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/fernet_utils.py` & `keystone-25.0.0.0rc1/keystone/common/fernet_utils.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/json_home.py` & `keystone-25.0.0.0rc1/keystone/common/json_home.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/jwt_utils.py` & `keystone-25.0.0.0rc1/keystone/common/jwt_utils.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/manager.py` & `keystone-25.0.0.0rc1/keystone/common/manager.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/password_hashing.py` & `keystone-25.0.0.0rc1/keystone/common/password_hashing.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/__init__.py` & `keystone-25.0.0.0rc1/keystone/common/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/access_rule.py` & `keystone-25.0.0.0rc1/keystone/common/policies/access_rule.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/access_token.py` & `keystone-25.0.0.0rc1/keystone/common/policies/access_token.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/application_credential.py` & `keystone-25.0.0.0rc1/keystone/common/policies/application_credential.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/auth.py` & `keystone-25.0.0.0rc1/keystone/common/policies/auth.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/base.py` & `keystone-25.0.0.0rc1/keystone/common/policies/base.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/consumer.py` & `keystone-25.0.0.0rc1/keystone/common/policies/consumer.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/credential.py` & `keystone-25.0.0.0rc1/keystone/common/policies/credential.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/domain.py` & `keystone-25.0.0.0rc1/keystone/common/policies/domain.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/domain_config.py` & `keystone-25.0.0.0rc1/keystone/common/policies/domain_config.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/ec2_credential.py` & `keystone-25.0.0.0rc1/keystone/common/policies/ec2_credential.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/endpoint.py` & `keystone-25.0.0.0rc1/keystone/common/policies/endpoint.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/endpoint_group.py` & `keystone-25.0.0.0rc1/keystone/common/policies/endpoint_group.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/grant.py` & `keystone-25.0.0.0rc1/keystone/common/policies/grant.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/group.py` & `keystone-25.0.0.0rc1/keystone/common/policies/group.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/identity_provider.py` & `keystone-25.0.0.0rc1/keystone/common/policies/identity_provider.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/implied_role.py` & `keystone-25.0.0.0rc1/keystone/common/policies/implied_role.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/limit.py` & `keystone-25.0.0.0rc1/keystone/common/policies/limit.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/mapping.py` & `keystone-25.0.0.0rc1/keystone/common/policies/mapping.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/policy.py` & `keystone-25.0.0.0rc1/keystone/common/policies/policy.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/policy_association.py` & `keystone-25.0.0.0rc1/keystone/common/policies/policy_association.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/project.py` & `keystone-25.0.0.0rc1/keystone/common/policies/project.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/project_endpoint.py` & `keystone-25.0.0.0rc1/keystone/common/policies/project_endpoint.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/protocol.py` & `keystone-25.0.0.0rc1/keystone/common/policies/protocol.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/region.py` & `keystone-25.0.0.0rc1/keystone/common/policies/region.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/registered_limit.py` & `keystone-25.0.0.0rc1/keystone/common/policies/registered_limit.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/revoke_event.py` & `keystone-25.0.0.0rc1/keystone/common/policies/revoke_event.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/role.py` & `keystone-25.0.0.0rc1/keystone/common/policies/role.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/role_assignment.py` & `keystone-25.0.0.0rc1/keystone/common/policies/role_assignment.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/service.py` & `keystone-25.0.0.0rc1/keystone/common/policies/service.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/service_provider.py` & `keystone-25.0.0.0rc1/keystone/common/policies/service_provider.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/token.py` & `keystone-25.0.0.0rc1/keystone/common/policies/token.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/token_revocation.py` & `keystone-25.0.0.0rc1/keystone/common/policies/token_revocation.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/trust.py` & `keystone-25.0.0.0rc1/keystone/common/policies/trust.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/policies/user.py` & `keystone-25.0.0.0rc1/keystone/common/policies/user.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/profiler.py` & `keystone-25.0.0.0rc1/keystone/common/profiler.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/provider_api.py` & `keystone-25.0.0.0rc1/keystone/common/provider_api.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/rbac_enforcer/__init__.py` & `keystone-25.0.0.0rc1/keystone/common/rbac_enforcer/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/rbac_enforcer/enforcer.py` & `keystone-25.0.0.0rc1/keystone/common/rbac_enforcer/enforcer.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/rbac_enforcer/policy.py` & `keystone-25.0.0.0rc1/keystone/common/rbac_enforcer/policy.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/render_token.py` & `keystone-25.0.0.0rc1/keystone/common/render_token.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/resource_options/__init__.py` & `keystone-25.0.0.0rc1/keystone/common/resource_options/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/resource_options/core.py` & `keystone-25.0.0.0rc1/keystone/common/resource_options/core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/resource_options/options/__init__.py` & `keystone-25.0.0.0rc1/keystone/common/resource_options/options/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/resource_options/options/immutable.py` & `keystone-25.0.0.0rc1/keystone/common/resource_options/options/immutable.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/sql/__init__.py` & `keystone-25.0.0.0rc1/keystone/common/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/sql/alembic.ini` & `keystone-25.0.0.0rc1/keystone/common/sql/alembic.ini`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/sql/core.py` & `keystone-25.0.0.0rc1/keystone/common/sql/core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/sql/migrations/README.rst` & `keystone-25.0.0.0rc1/keystone/common/sql/migrations/README.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/sql/migrations/autogen.py` & `keystone-25.0.0.0rc1/keystone/common/sql/migrations/autogen.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/sql/migrations/env.py` & `keystone-25.0.0.0rc1/keystone/common/sql/migrations/env.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/sql/migrations/manage.py` & `keystone-25.0.0.0rc1/keystone/common/sql/migrations/manage.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/sql/migrations/script.py.mako` & `keystone-25.0.0.0rc1/keystone/common/sql/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/sql/migrations/versions/2024.01/expand/47147121_add_identity_federation_attribute_mapping_schema_version.py` & `keystone-25.0.0.0rc1/keystone/common/sql/migrations/versions/2024.01/expand/47147121_add_identity_federation_attribute_mapping_schema_version.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/sql/migrations/versions/27e647c0fad4_initial_version.py` & `keystone-25.0.0.0rc1/keystone/common/sql/migrations/versions/27e647c0fad4_initial_version.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/sql/migrations/versions/bobcat/contract/99de3849d860_fix_incorrect_constraints.py` & `keystone-25.0.0.0rc1/keystone/common/sql/migrations/versions/bobcat/contract/99de3849d860_fix_incorrect_constraints.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/sql/migrations/versions/bobcat/contract/c88cdce8f248_remove_duplicate_constraints.py` & `keystone-25.0.0.0rc1/keystone/common/sql/migrations/versions/bobcat/contract/c88cdce8f248_remove_duplicate_constraints.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/sql/migrations/versions/bobcat/expand/11c3b243b4cb_remove_service_provider_relay_state_server_default.py` & `keystone-25.0.0.0rc1/keystone/common/sql/migrations/versions/bobcat/expand/11c3b243b4cb_remove_service_provider_relay_state_server_default.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/sql/migrations/versions/bobcat/expand/b4f8b3f584e0_fix_incorrect_constraints.py` & `keystone-25.0.0.0rc1/keystone/common/sql/migrations/versions/bobcat/expand/b4f8b3f584e0_fix_incorrect_constraints.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/sql/migrations/versions/yoga/contract/e25ffa003242_initial.py` & `keystone-25.0.0.0rc1/keystone/common/sql/migrations/versions/yoga/contract/e25ffa003242_initial.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/sql/migrations/versions/yoga/expand/29e87d24a316_initial.py` & `keystone-25.0.0.0rc1/keystone/common/sql/migrations/versions/yoga/expand/29e87d24a316_initial.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/sql/upgrades.py` & `keystone-25.0.0.0rc1/keystone/common/sql/upgrades.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/tokenless_auth.py` & `keystone-25.0.0.0rc1/keystone/common/tokenless_auth.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/utils.py` & `keystone-25.0.0.0rc1/keystone/common/utils.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/validation/__init__.py` & `keystone-25.0.0.0rc1/keystone/common/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/validation/parameter_types.py` & `keystone-25.0.0.0rc1/keystone/common/validation/parameter_types.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/common/validation/validators.py` & `keystone-25.0.0.0rc1/keystone/common/validation/validators.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/__init__.py` & `keystone-25.0.0.0rc1/keystone/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/application_credential.py` & `keystone-25.0.0.0rc1/keystone/conf/application_credential.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/assignment.py` & `keystone-25.0.0.0rc1/keystone/conf/assignment.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/auth.py` & `keystone-25.0.0.0rc1/keystone/conf/auth.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/catalog.py` & `keystone-25.0.0.0rc1/keystone/conf/catalog.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/constants.py` & `keystone-25.0.0.0rc1/keystone/conf/constants.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/credential.py` & `keystone-25.0.0.0rc1/keystone/conf/credential.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/default.py` & `keystone-25.0.0.0rc1/keystone/conf/default.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/domain_config.py` & `keystone-25.0.0.0rc1/keystone/conf/domain_config.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/endpoint_filter.py` & `keystone-25.0.0.0rc1/keystone/conf/endpoint_filter.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/endpoint_policy.py` & `keystone-25.0.0.0rc1/keystone/conf/endpoint_policy.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/federation.py` & `keystone-25.0.0.0rc1/keystone/conf/federation.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/fernet_receipts.py` & `keystone-25.0.0.0rc1/keystone/conf/fernet_receipts.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/fernet_tokens.py` & `keystone-25.0.0.0rc1/keystone/conf/fernet_tokens.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/identity.py` & `keystone-25.0.0.0rc1/keystone/conf/identity.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/identity_mapping.py` & `keystone-25.0.0.0rc1/keystone/conf/identity_mapping.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/jwt_tokens.py` & `keystone-25.0.0.0rc1/keystone/conf/jwt_tokens.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/ldap.py` & `keystone-25.0.0.0rc1/keystone/conf/ldap.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/oauth1.py` & `keystone-25.0.0.0rc1/keystone/conf/oauth1.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/oauth2.py` & `keystone-25.0.0.0rc1/keystone/conf/oauth2.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/opts.py` & `keystone-25.0.0.0rc1/keystone/conf/opts.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/policy.py` & `keystone-25.0.0.0rc1/keystone/conf/policy.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/receipt.py` & `keystone-25.0.0.0rc1/keystone/conf/receipt.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/resource.py` & `keystone-25.0.0.0rc1/keystone/conf/resource.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/revoke.py` & `keystone-25.0.0.0rc1/keystone/conf/revoke.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/role.py` & `keystone-25.0.0.0rc1/keystone/conf/role.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/saml.py` & `keystone-25.0.0.0rc1/keystone/conf/saml.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/security_compliance.py` & `keystone-25.0.0.0rc1/keystone/conf/security_compliance.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/shadow_users.py` & `keystone-25.0.0.0rc1/keystone/conf/shadow_users.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/token.py` & `keystone-25.0.0.0rc1/keystone/conf/token.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/tokenless_auth.py` & `keystone-25.0.0.0rc1/keystone/conf/tokenless_auth.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/totp.py` & `keystone-25.0.0.0rc1/keystone/conf/totp.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/trust.py` & `keystone-25.0.0.0rc1/keystone/conf/trust.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/unified_limit.py` & `keystone-25.0.0.0rc1/keystone/conf/unified_limit.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/utils.py` & `keystone-25.0.0.0rc1/keystone/conf/utils.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/conf/wsgi.py` & `keystone-25.0.0.0rc1/keystone/conf/wsgi.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/credential/__init__.py` & `keystone-25.0.0.0rc1/keystone/credential/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/credential/backends/base.py` & `keystone-25.0.0.0rc1/keystone/credential/backends/base.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/credential/backends/sql.py` & `keystone-25.0.0.0rc1/keystone/credential/backends/sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/credential/core.py` & `keystone-25.0.0.0rc1/keystone/credential/core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/credential/provider.py` & `keystone-25.0.0.0rc1/keystone/credential/provider.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/credential/providers/core.py` & `keystone-25.0.0.0rc1/keystone/credential/providers/core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/credential/providers/fernet/__init__.py` & `keystone-25.0.0.0rc1/keystone/credential/providers/fernet/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/credential/providers/fernet/core.py` & `keystone-25.0.0.0rc1/keystone/credential/providers/fernet/core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/credential/schema.py` & `keystone-25.0.0.0rc1/keystone/credential/schema.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/endpoint_policy/__init__.py` & `keystone-25.0.0.0rc1/keystone/endpoint_policy/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/endpoint_policy/backends/base.py` & `keystone-25.0.0.0rc1/keystone/endpoint_policy/backends/base.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/endpoint_policy/backends/sql.py` & `keystone-25.0.0.0rc1/keystone/endpoint_policy/backends/sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/endpoint_policy/core.py` & `keystone-25.0.0.0rc1/keystone/endpoint_policy/core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/exception.py` & `keystone-25.0.0.0rc1/keystone/exception.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/federation/__init__.py` & `keystone-25.0.0.0rc1/keystone/federation/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/federation/backends/base.py` & `keystone-25.0.0.0rc1/keystone/federation/backends/base.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/federation/backends/sql.py` & `keystone-25.0.0.0rc1/keystone/federation/backends/sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/federation/constants.py` & `keystone-25.0.0.0rc1/keystone/federation/constants.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/federation/core.py` & `keystone-25.0.0.0rc1/keystone/federation/core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/federation/idp.py` & `keystone-25.0.0.0rc1/keystone/federation/idp.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/federation/schema.py` & `keystone-25.0.0.0rc1/keystone/federation/schema.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/federation/utils.py` & `keystone-25.0.0.0rc1/keystone/federation/utils.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/i18n.py` & `keystone-25.0.0.0rc1/keystone/i18n.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/identity/__init__.py` & `keystone-25.0.0.0rc1/keystone/identity/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/identity/backends/base.py` & `keystone-25.0.0.0rc1/keystone/identity/backends/base.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/identity/backends/ldap/__init__.py` & `keystone-25.0.0.0rc1/keystone/identity/backends/ldap/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/identity/backends/ldap/common.py` & `keystone-25.0.0.0rc1/keystone/identity/backends/ldap/common.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/identity/backends/ldap/core.py` & `keystone-25.0.0.0rc1/keystone/identity/backends/ldap/core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/identity/backends/ldap/models.py` & `keystone-25.0.0.0rc1/keystone/identity/backends/ldap/models.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/identity/backends/resource_options.py` & `keystone-25.0.0.0rc1/keystone/identity/backends/resource_options.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/identity/backends/sql.py` & `keystone-25.0.0.0rc1/keystone/identity/backends/sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/identity/backends/sql_model.py` & `keystone-25.0.0.0rc1/keystone/identity/backends/sql_model.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/identity/core.py` & `keystone-25.0.0.0rc1/keystone/identity/core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/identity/generator.py` & `keystone-25.0.0.0rc1/keystone/identity/generator.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/identity/id_generators/sha256.py` & `keystone-25.0.0.0rc1/keystone/identity/id_generators/sha256.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/identity/mapping_backends/base.py` & `keystone-25.0.0.0rc1/keystone/identity/mapping_backends/base.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/identity/mapping_backends/mapping.py` & `keystone-25.0.0.0rc1/keystone/identity/mapping_backends/mapping.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/identity/mapping_backends/sql.py` & `keystone-25.0.0.0rc1/keystone/identity/mapping_backends/sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/identity/schema.py` & `keystone-25.0.0.0rc1/keystone/identity/schema.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/identity/shadow_backends/base.py` & `keystone-25.0.0.0rc1/keystone/identity/shadow_backends/base.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/identity/shadow_backends/sql.py` & `keystone-25.0.0.0rc1/keystone/identity/shadow_backends/sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/limit/__init__.py` & `keystone-25.0.0.0rc1/keystone/limit/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/limit/backends/base.py` & `keystone-25.0.0.0rc1/keystone/limit/backends/base.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/limit/backends/sql.py` & `keystone-25.0.0.0rc1/keystone/limit/backends/sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/limit/core.py` & `keystone-25.0.0.0rc1/keystone/limit/core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/limit/models/base.py` & `keystone-25.0.0.0rc1/keystone/limit/models/base.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/limit/models/flat.py` & `keystone-25.0.0.0rc1/keystone/limit/models/flat.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/limit/models/strict_two_level.py` & `keystone-25.0.0.0rc1/keystone/limit/models/strict_two_level.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/limit/schema.py` & `keystone-25.0.0.0rc1/keystone/limit/schema.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/locale/de/LC_MESSAGES/keystone.po` & `keystone-25.0.0.0rc1/keystone/locale/de/LC_MESSAGES/keystone.po`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/locale/en_GB/LC_MESSAGES/keystone.po` & `keystone-25.0.0.0rc1/keystone/locale/en_GB/LC_MESSAGES/keystone.po`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/locale/es/LC_MESSAGES/keystone.po` & `keystone-25.0.0.0rc1/keystone/locale/es/LC_MESSAGES/keystone.po`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/locale/fr/LC_MESSAGES/keystone.po` & `keystone-25.0.0.0rc1/keystone/locale/fr/LC_MESSAGES/keystone.po`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/locale/it/LC_MESSAGES/keystone.po` & `keystone-25.0.0.0rc1/keystone/locale/it/LC_MESSAGES/keystone.po`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/locale/ja/LC_MESSAGES/keystone.po` & `keystone-25.0.0.0rc1/keystone/locale/ja/LC_MESSAGES/keystone.po`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/locale/ko_KR/LC_MESSAGES/keystone.po` & `keystone-25.0.0.0rc1/keystone/locale/ko_KR/LC_MESSAGES/keystone.po`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/locale/pt_BR/LC_MESSAGES/keystone.po` & `keystone-25.0.0.0rc1/keystone/locale/pt_BR/LC_MESSAGES/keystone.po`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/locale/ru/LC_MESSAGES/keystone.po` & `keystone-25.0.0.0rc1/keystone/locale/ru/LC_MESSAGES/keystone.po`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/locale/zh_CN/LC_MESSAGES/keystone.po` & `keystone-25.0.0.0rc1/keystone/locale/zh_CN/LC_MESSAGES/keystone.po`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/locale/zh_TW/LC_MESSAGES/keystone.po` & `keystone-25.0.0.0rc1/keystone/locale/zh_TW/LC_MESSAGES/keystone.po`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/models/receipt_model.py` & `keystone-25.0.0.0rc1/keystone/models/receipt_model.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/models/revoke_model.py` & `keystone-25.0.0.0rc1/keystone/models/revoke_model.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/models/token_model.py` & `keystone-25.0.0.0rc1/keystone/models/token_model.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/notifications.py` & `keystone-25.0.0.0rc1/keystone/notifications.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/oauth1/__init__.py` & `keystone-25.0.0.0rc1/keystone/oauth1/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/oauth1/backends/base.py` & `keystone-25.0.0.0rc1/keystone/oauth1/backends/base.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/oauth1/backends/sql.py` & `keystone-25.0.0.0rc1/keystone/oauth1/backends/sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/oauth1/core.py` & `keystone-25.0.0.0rc1/keystone/oauth1/core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/oauth1/schema.py` & `keystone-25.0.0.0rc1/keystone/oauth1/schema.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/oauth1/validator.py` & `keystone-25.0.0.0rc1/keystone/oauth1/validator.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/oauth2/handlers.py` & `keystone-25.0.0.0rc1/keystone/oauth2/handlers.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/policy/__init__.py` & `keystone-25.0.0.0rc1/keystone/policy/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/policy/backends/base.py` & `keystone-25.0.0.0rc1/keystone/policy/backends/base.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/policy/backends/rules.py` & `keystone-25.0.0.0rc1/keystone/policy/backends/rules.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/policy/backends/sql.py` & `keystone-25.0.0.0rc1/keystone/policy/backends/sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/policy/core.py` & `keystone-25.0.0.0rc1/keystone/policy/core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/policy/schema.py` & `keystone-25.0.0.0rc1/keystone/policy/schema.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/receipt/__init__.py` & `keystone-25.0.0.0rc1/keystone/receipt/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/receipt/handlers.py` & `keystone-25.0.0.0rc1/keystone/receipt/handlers.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/receipt/provider.py` & `keystone-25.0.0.0rc1/keystone/receipt/provider.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/receipt/providers/base.py` & `keystone-25.0.0.0rc1/keystone/receipt/providers/base.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/receipt/providers/fernet/__init__.py` & `keystone-25.0.0.0rc1/keystone/receipt/providers/fernet/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/receipt/providers/fernet/core.py` & `keystone-25.0.0.0rc1/keystone/receipt/providers/fernet/core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/receipt/receipt_formatters.py` & `keystone-25.0.0.0rc1/keystone/receipt/receipt_formatters.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/resource/__init__.py` & `keystone-25.0.0.0rc1/keystone/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/resource/backends/base.py` & `keystone-25.0.0.0rc1/keystone/resource/backends/base.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/resource/backends/resource_options.py` & `keystone-25.0.0.0rc1/keystone/resource/backends/resource_options.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/resource/backends/sql.py` & `keystone-25.0.0.0rc1/keystone/resource/backends/sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/resource/backends/sql_model.py` & `keystone-25.0.0.0rc1/keystone/resource/backends/sql_model.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/resource/config_backends/base.py` & `keystone-25.0.0.0rc1/keystone/resource/config_backends/base.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/resource/config_backends/sql.py` & `keystone-25.0.0.0rc1/keystone/resource/config_backends/sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/resource/core.py` & `keystone-25.0.0.0rc1/keystone/resource/core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/resource/schema.py` & `keystone-25.0.0.0rc1/keystone/resource/schema.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/revoke/__init__.py` & `keystone-25.0.0.0rc1/keystone/revoke/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/revoke/backends/base.py` & `keystone-25.0.0.0rc1/keystone/revoke/backends/base.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/revoke/backends/sql.py` & `keystone-25.0.0.0rc1/keystone/revoke/backends/sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/revoke/core.py` & `keystone-25.0.0.0rc1/keystone/revoke/core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/revoke/model.py` & `keystone-25.0.0.0rc1/keystone/revoke/model.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/server/__init__.py` & `keystone-25.0.0.0rc1/keystone/server/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/server/backends.py` & `keystone-25.0.0.0rc1/keystone/server/backends.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/server/flask/__init__.py` & `keystone-25.0.0.0rc1/keystone/server/flask/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/server/flask/application.py` & `keystone-25.0.0.0rc1/keystone/server/flask/application.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/server/flask/common.py` & `keystone-25.0.0.0rc1/keystone/server/flask/common.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/server/flask/core.py` & `keystone-25.0.0.0rc1/keystone/server/flask/core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/server/flask/request_processing/json_body.py` & `keystone-25.0.0.0rc1/keystone/server/flask/request_processing/json_body.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/server/flask/request_processing/middleware/auth_context.py` & `keystone-25.0.0.0rc1/keystone/server/flask/request_processing/middleware/auth_context.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/server/flask/request_processing/middleware/url_normalize.py` & `keystone-25.0.0.0rc1/keystone/server/flask/request_processing/middleware/url_normalize.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/server/flask/request_processing/req_logging.py` & `keystone-25.0.0.0rc1/keystone/server/flask/request_processing/req_logging.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/server/wsgi.py` & `keystone-25.0.0.0rc1/keystone/server/wsgi.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/common/auth.py` & `keystone-25.0.0.0rc1/keystone/tests/common/auth.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/functional/core.py` & `keystone-25.0.0.0rc1/keystone/tests/functional/core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/functional/shared/test_running.py` & `keystone-25.0.0.0rc1/keystone/tests/functional/shared/test_running.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/hacking/checks.py` & `keystone-25.0.0.0rc1/keystone/tests/hacking/checks.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_access_rules.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_access_rules.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_application_credential.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_application_credential.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_assignment.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_assignment.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_consumer.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_consumer.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_credentials.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_credentials.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_domain_config.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_domain_config.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_domain_roles.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_domain_roles.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_domains.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_domains.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_ec2_credential.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_ec2_credential.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_endpoint_group.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_endpoint_group.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_endpoints.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_grants.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_grants.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_groups.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_groups.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_identity_providers.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_identity_providers.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_implied_roles.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_implied_roles.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_limits.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_limits.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_mappings.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_mappings.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_policy.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_policy.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_policy_association.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_policy_association.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_project_endpoint.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_project_endpoint.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_project_tags.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_project_tags.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_projects.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_projects.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_protocols.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_protocols.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_regions.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_regions.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_registered_limits.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_registered_limits.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_roles.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_roles.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_service_providers.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_service_providers.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_services.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_services.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_system_assignments.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_system_assignments.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_tokens.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_tokens.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_trusts.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_trusts.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/protection/v3/test_users.py` & `keystone-25.0.0.0rc1/keystone/tests/protection/v3/test_users.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/__init__.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/application_credential/backends/test_sql.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/application_credential/backends/test_sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/application_credential/test_backends.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/application_credential/test_backends.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/assignment/role_backends/test_sql.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/assignment/role_backends/test_sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/assignment/test_backends.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/assignment/test_backends.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/assignment/test_core.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/assignment/test_core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/auth/plugins/test_core.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/auth/plugins/test_core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/auth/plugins/test_mapped.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/auth/plugins/test_mapped.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/auth/test_controllers.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/auth/test_controllers.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/auth/test_schema.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/auth/test_schema.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/backend/core_ldap.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/backend/core_ldap.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/backend/core_sql.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/backend/core_sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/base_classes.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/base_classes.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/catalog/test_backends.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/catalog/test_backends.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/catalog/test_core.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/catalog/test_core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/common/sql/test_upgrades.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/common/sql/test_upgrades.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/common/test_cache.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/common/test_cache.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/common/test_database_conflicts.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/common/test_database_conflicts.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/common/test_json_home.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/common/test_json_home.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/common/test_notifications.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/common/test_notifications.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/common/test_provider_api.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/common/test_provider_api.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/common/test_rbac_enforcer.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/common/test_rbac_enforcer.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/common/test_resource_options_common.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/common/test_resource_options_common.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/common/test_sql_core.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/common/test_sql_core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/common/test_utils.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/common/test_utils.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/config_files/backend_ldap_pool.conf` & `keystone-25.0.0.0rc1/keystone/tests/unit/config_files/backend_ldap_pool.conf`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/config_files/backend_pool_liveldap.conf` & `keystone-25.0.0.0rc1/keystone/tests/unit/config_files/backend_pool_liveldap.conf`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/contrib/federation/test_utils.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/contrib/federation/test_utils.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/core.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/credential/test_backend_sql.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/credential/test_backend_sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/credential/test_fernet_provider.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/credential/test_fernet_provider.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/default_catalog.templates` & `keystone-25.0.0.0rc1/keystone/tests/unit/default_catalog.templates`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/default_catalog_multi_region.templates` & `keystone-25.0.0.0rc1/keystone/tests/unit/default_catalog_multi_region.templates`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/default_fixtures.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/default_fixtures.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/endpoint_policy/backends/test_base.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/endpoint_policy/backends/test_base.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/endpoint_policy/backends/test_sql.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/endpoint_policy/backends/test_sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/external/README.rst` & `keystone-25.0.0.0rc1/keystone/tests/unit/external/README.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/external/test_timeutils.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/external/test_timeutils.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/fakeldap.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/fakeldap.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/federation/test_core.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/federation/test_core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/federation/test_utils.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/federation/test_utils.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/federation_fixtures.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/federation_fixtures.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/filtering.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/filtering.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/identity/backends/test_base.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/identity/backends/test_base.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/identity/backends/test_ldap.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/identity/backends/test_ldap.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/identity/backends/test_ldap_common.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/identity/backends/test_ldap_common.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/identity/backends/test_sql.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/identity/backends/test_sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/identity/shadow_users/test_backend.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/identity/shadow_users/test_backend.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/identity/shadow_users/test_core.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/identity/shadow_users/test_core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/identity/test_backend_sql.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/identity/test_backend_sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/identity/test_backends.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/identity/test_backends.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/identity/test_core.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/identity/test_core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/identity_mapping.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/identity_mapping.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/ksfixtures/__init__.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/ksfixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/ksfixtures/auth_plugins.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/ksfixtures/auth_plugins.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/ksfixtures/backendloader.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/ksfixtures/backendloader.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/ksfixtures/cache.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/ksfixtures/cache.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/ksfixtures/database.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/ksfixtures/database.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/ksfixtures/hacking.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/ksfixtures/hacking.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/ksfixtures/jws_key_repository.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/ksfixtures/jws_key_repository.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/ksfixtures/key_repository.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/ksfixtures/key_repository.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/ksfixtures/ldapdb.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/ksfixtures/ldapdb.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/ksfixtures/logging.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/ksfixtures/logging.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/ksfixtures/policy.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/ksfixtures/policy.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/ksfixtures/temporaryfile.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/ksfixtures/temporaryfile.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/ksfixtures/warnings.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/ksfixtures/warnings.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/limit/test_backends.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/limit/test_backends.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/mapping_fixtures.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/mapping_fixtures.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/policy/backends/test_base.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/policy/backends/test_base.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/policy/backends/test_sql.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/policy/backends/test_sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/policy/test_backends.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/policy/test_backends.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/receipt/test_fernet_provider.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/receipt/test_fernet_provider.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/receipt/test_receipt_serialization.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/receipt/test_receipt_serialization.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/resource/backends/test_sql.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/resource/backends/test_sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/resource/config_backends/test_sql.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/resource/config_backends/test_sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/resource/test_backends.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/resource/test_backends.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/resource/test_core.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/resource/test_core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/rest.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/rest.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/saml2/idp_saml2_metadata.xml` & `keystone-25.0.0.0rc1/keystone/tests/unit/saml2/idp_saml2_metadata.xml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/saml2/signed_saml2_assertion.xml` & `keystone-25.0.0.0rc1/keystone/tests/unit/saml2/signed_saml2_assertion.xml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/server/test_keystone_flask.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/server/test_keystone_flask.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_app_config.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_app_config.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_associate_project_endpoint_extension.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_associate_project_endpoint_extension.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_auth_plugin.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_backend_endpoint_policy.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_backend_endpoint_policy.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_backend_endpoint_policy_sql.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_backend_endpoint_policy_sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_backend_federation_sql.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_backend_federation_sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_backend_id_mapping_sql.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_backend_id_mapping_sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_backend_ldap.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_backend_ldap.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_backend_ldap_pool.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_backend_ldap_pool.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_backend_rules.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_backend_rules.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_backend_sql.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_backend_sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_backend_templated.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_backend_templated.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_cli.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_cli.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_config.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_contrib_ec2_core.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_contrib_ec2_core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_contrib_s3_core.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_contrib_s3_core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_contrib_simple_cert.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_contrib_simple_cert.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_driver_hints.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_driver_hints.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_entry_points.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_entry_points.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_exception.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_exception.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_hacking_checks.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_hacking_checks.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_healthcheck.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_healthcheck.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_ldap_livetest.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_ldap_livetest.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_ldap_pool_livetest.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_ldap_pool_livetest.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_ldap_tls_livetest.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_ldap_tls_livetest.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_limits.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_limits.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_middleware.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_middleware.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_policy.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_policy.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_receipt_provider.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_receipt_provider.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_revoke.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_revoke.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_shadow_users.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_shadow_users.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_sql_banned_operations.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_sql_banned_operations.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_sql_upgrade.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_sql_upgrade.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_token_provider.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_token_provider.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_url_middleware.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_url_middleware.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_v3.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_v3.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_v3_application_credential.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_application_credential.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_v3_assignment.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_assignment.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_v3_auth.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_auth.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_v3_catalog.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_catalog.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_v3_credential.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_credential.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_v3_domain_config.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_domain_config.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_v3_endpoint_policy.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_endpoint_policy.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_v3_federation.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_federation.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_v3_filters.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_filters.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_v3_identity.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_identity.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_v3_oauth1.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_oauth1.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_v3_oauth2.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_oauth2.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_v3_os_revoke.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_os_revoke.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_v3_policy.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_policy.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_v3_resource.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_resource.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_v3_trust.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_v3_trust.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_validation.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_validation.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/test_versions.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/test_versions.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/tests/test_core.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/tests/test_utils.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/token/test_fernet_provider.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/token/test_fernet_provider.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/token/test_jws_provider.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/token/test_jws_provider.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/token/test_token_serialization.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/token/test_token_serialization.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/trust/test_backends.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/trust/test_backends.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/tests/unit/utils.py` & `keystone-25.0.0.0rc1/keystone/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/token/__init__.py` & `keystone-25.0.0.0rc1/keystone/token/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/token/provider.py` & `keystone-25.0.0.0rc1/keystone/token/provider.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/token/providers/base.py` & `keystone-25.0.0.0rc1/keystone/token/providers/base.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/token/providers/fernet/__init__.py` & `keystone-25.0.0.0rc1/keystone/token/providers/fernet/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/token/providers/fernet/core.py` & `keystone-25.0.0.0rc1/keystone/token/providers/fernet/core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/token/providers/jws/__init__.py` & `keystone-25.0.0.0rc1/keystone/token/providers/jws/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/token/providers/jws/core.py` & `keystone-25.0.0.0rc1/keystone/token/providers/jws/core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/token/token_formatters.py` & `keystone-25.0.0.0rc1/keystone/token/token_formatters.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/trust/__init__.py` & `keystone-25.0.0.0rc1/keystone/trust/__init__.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/trust/backends/base.py` & `keystone-25.0.0.0rc1/keystone/trust/backends/base.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/trust/backends/sql.py` & `keystone-25.0.0.0rc1/keystone/trust/backends/sql.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/trust/core.py` & `keystone-25.0.0.0rc1/keystone/trust/core.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/trust/schema.py` & `keystone-25.0.0.0rc1/keystone/trust/schema.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone/version.py` & `keystone-25.0.0.0rc1/keystone/version.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone.egg-info/PKG-INFO` & `keystone-25.0.0.0rc1/keystone.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keystone
-Version: 25.0.0
+Version: 25.0.0.0rc1
 Summary: OpenStack Identity
 Home-page: https://docs.openstack.org/keystone/latest
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ==================
         OpenStack Keystone
```

### Comparing `keystone-25.0.0/keystone.egg-info/SOURCES.txt` & `keystone-25.0.0.0rc1/keystone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone.egg-info/entry_points.txt` & `keystone-25.0.0.0rc1/keystone.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/keystone.egg-info/requires.txt` & `keystone-25.0.0.0rc1/keystone.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/rally-jobs/keystone.yaml` & `keystone-25.0.0.0rc1/rally-jobs/keystone.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/Assignment_V9_driver-c22be069f7baccb0.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/Assignment_V9_driver-c22be069f7baccb0.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/DomainSpecificRoles-fc5dd2ef74a1442c.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/DomainSpecificRoles-fc5dd2ef74a1442c.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/add-bootstrap-cli-192500228cc6e574.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/add-bootstrap-cli-192500228cc6e574.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/admin_token-a5678d712783c145.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/admin_token-a5678d712783c145.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/admin_token-c634ec12fc714255.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/admin_token-c634ec12fc714255.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bootstrap-update-endpoint-7a63a2329822b6e7.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bootstrap-update-endpoint-7a63a2329822b6e7.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bp-allow-expired-f5d845b9601bc1ef.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bp-allow-expired-f5d845b9601bc1ef.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bp-application-credentials-c699f1f17c7d4e2f.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bp-application-credentials-c699f1f17c7d4e2f.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bp-basic-default-roles-4ff6502b6ac57d48.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bp-basic-default-roles-4ff6502b6ac57d48.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bp-domain-config-as-stable-716ca5ab33c0cc42.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bp-domain-config-as-stable-716ca5ab33c0cc42.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bp-mfa-auth-receipt-8b459431c1f360ce.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bp-mfa-auth-receipt-8b459431c1f360ce.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bp-password-expires-validation-4b32fe7032595932.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bp-password-expires-validation-4b32fe7032595932.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bp-pci-dss-notifications-808a205a637bac25.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bp-pci-dss-notifications-808a205a637bac25.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bp-pci-dss-password-requirements-api-87bc724b2aa554f7.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bp-pci-dss-password-requirements-api-87bc724b2aa554f7.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bp-pci-dss-query-password-expired-users-a7c96a3843bb9abc.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bp-pci-dss-query-password-expired-users-a7c96a3843bb9abc.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bp-per-user-auth-plugin-reqs-feb95fd907be4b40.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bp-per-user-auth-plugin-reqs-feb95fd907be4b40.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bp-policy-in-code-722372a27291b9cd.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bp-policy-in-code-722372a27291b9cd.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bp-shadow-mapping-06fc7c71a401d707.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bp-shadow-mapping-06fc7c71a401d707.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bp-strict-two-level-model.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bp-strict-two-level-model.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bp-support-oauth2-mtls-8552892a8e0c72d2.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bp-support-oauth2-mtls-8552892a8e0c72d2.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bp-system-scope-7d236ee5992d4e20.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bp-system-scope-7d236ee5992d4e20.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bp-whitelist-extension-for-app-creds-90e5bcd7b2b78b02.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bp-whitelist-extension-for-app-creds-90e5bcd7b2b78b02.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1017606-98313bb4c1edf250.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1017606-98313bb4c1edf250.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1473292-c21481e6aec29ec2.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1473292-c21481e6aec29ec2.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1490804-de58a9606edb31eb.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1490804-de58a9606edb31eb.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1523369-4d42c841b6e7e54e.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1523369-4d42c841b6e7e54e.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1524030-ccff6b0ec9d1cbf2.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1524030-ccff6b0ec9d1cbf2.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1542417-d630b7886bb0b369.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1542417-d630b7886bb0b369.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1547684-911aed68a0d3df17.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1547684-911aed68a0d3df17.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1561054-dbe88b552a936a05.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1561054-dbe88b552a936a05.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1622310-c501cf77437fdfa6.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1622310-c501cf77437fdfa6.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1636950-8fa1a47fce440977.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1636950-8fa1a47fce440977.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1641639-b9accc163e61ca15.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1641639-b9accc163e61ca15.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1641654-8630ce7bcde43a7e.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1641654-8630ce7bcde43a7e.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1641660-f938267e1ec54071.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1641660-f938267e1ec54071.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1642687-5497fb56fe86806d.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1642687-5497fb56fe86806d.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1642687-c7ab1c9be152db20.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1642687-c7ab1c9be152db20.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1649446-efff94143823755d.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1649446-efff94143823755d.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1656076-c4422270f73b43b.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1656076-c4422270f73b43b.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1659730-17834ba2dde668ae.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1659730-17834ba2dde668ae.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1659995-f3e716de743b7291.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1659995-f3e716de743b7291.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1703369-9a901d627a1e0316.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1703369-9a901d627a1e0316.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1705485-7a1ad17b9cc99b9d.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1705485-7a1ad17b9cc99b9d.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1718747-50d39fa87bdbb12b.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1718747-50d39fa87bdbb12b.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1724645-a94659dfd0f45b9a.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1724645-a94659dfd0f45b9a.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1748027-decc2e11154b97cf.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1748027-decc2e11154b97cf.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1750660-e2a360ddd6790fc4.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1750660-e2a360ddd6790fc4.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1750669-dfce859550126f03.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1750669-dfce859550126f03.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1750673-b53f74944d767ae9.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1750673-b53f74944d767ae9.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1750676-cf70c1a27b2c8de3.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1750676-cf70c1a27b2c8de3.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1750678-88a38851ca80fc64.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1750678-88a38851ca80fc64.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1760205-87dedd6d8812db3f.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1760205-87dedd6d8812db3f.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1776504-keystone-conversion-to-flask-372a5654a55675c6.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1776504-keystone-conversion-to-flask-372a5654a55675c6.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1778945-b7f2db3052525ca8.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1778945-b7f2db3052525ca8.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1787874-13499ec227b8e26c.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1787874-13499ec227b8e26c.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1788415-3190279e9c900f76.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1788415-3190279e9c900f76.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1794376-53ce14528f00f01d.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1794376-53ce14528f00f01d.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1794527-866b1caff67977f3.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1794527-866b1caff67977f3.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1794864-3116bf165a146be6.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1794864-3116bf165a146be6.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1804292-0107869c7029f79e.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1804292-0107869c7029f79e.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1804446-1a281eadbb044070.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1804446-1a281eadbb044070.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1804462-59ad43f98242dea0.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1804462-59ad43f98242dea0.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1804463-74537652166cf656.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1804463-74537652166cf656.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1804482-aa95619320d098fa.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1804482-aa95619320d098fa.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1804483-1d9ccfcb24f25f51.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1804483-1d9ccfcb24f25f51.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1804516-24b0b10ed6fe0589.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1804516-24b0b10ed6fe0589.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1804517-a351aec088fee066.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1804517-a351aec088fee066.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1804519-8384a9ead261d4c2.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1804519-8384a9ead261d4c2.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1804520-d124599967923052.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1804520-d124599967923052.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1804521-3c0d9f567e8f532f.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1804521-3c0d9f567e8f532f.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1804522-00df902cd2d74ee3.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1804522-00df902cd2d74ee3.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1804523-d1768909b13b167e.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1804523-d1768909b13b167e.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1805363-0b85d71917ad09d1.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1805363-0b85d71917ad09d1.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1805366-670867516c6fc4bc.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1805366-670867516c6fc4bc.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1805368-ea32c2db2ae57225.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1805368-ea32c2db2ae57225.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1805369-ed98d3fcfafb5c43.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1805369-ed98d3fcfafb5c43.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1805371-249c8c9b562ab371.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1805371-249c8c9b562ab371.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1805372-af4ebf4b19500b72.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1805372-af4ebf4b19500b72.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1805400-c192be936d277ade.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1805400-c192be936d277ade.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1805402-75d0d93f31af620f.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1805402-75d0d93f31af620f.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1805403-c003627a64768716.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1805403-c003627a64768716.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1805406-252b45d443af20b3.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1805406-252b45d443af20b3.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1805409-8bc6cc9f1c5bc672.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1805409-8bc6cc9f1c5bc672.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1805880-0032024ea6b83563.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1805880-0032024ea6b83563.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1805880-3fc6b30309a4370f.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1805880-3fc6b30309a4370f.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1806713-cf5feab23fc78a23.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1806713-cf5feab23fc78a23.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1806762-08ff9eecdc03c554.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1806762-08ff9eecdc03c554.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1806762-09f414995924db23.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1806762-09f414995924db23.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1806762-0b7356ace200a5d3.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1806762-0b7356ace200a5d3.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1806762-2092fee9f6c87dc3.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1806762-2092fee9f6c87dc3.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1806762-c3bfc71cb9bb94f3.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1806762-c3bfc71cb9bb94f3.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1806762-daed3e27f58f0f6d.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1806762-daed3e27f58f0f6d.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1809116-b65502f3b606b060.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1809116-b65502f3b606b060.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1811605-9d23080d7e949c25.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1811605-9d23080d7e949c25.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1816076-ba39508e6ade529e.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1816076-ba39508e6ade529e.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1818725-96d698e22e648764.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1818725-96d698e22e648764.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1818734-d753bfae60ffd030.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1818734-d753bfae60ffd030.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1818736-98ea186a074056f4.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1818736-98ea186a074056f4.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1818846-d1a8c77d20659ad6.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1818846-d1a8c77d20659ad6.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1820333-356dcc8bf9f73fed.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1820333-356dcc8bf9f73fed.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1823258-9f93dbdc0fa8441d.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1823258-9f93dbdc0fa8441d.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1836568-66d853a1f22c5530.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1836568-66d853a1f22c5530.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1844157-7808af9bcea0429d.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1844157-7808af9bcea0429d.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1844194-48ae60db49f91bd4.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1844194-48ae60db49f91bd4.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1844461-08a8bdc5f613b88d.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1844461-08a8bdc5f613b88d.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1844664-905cf6cad2e032a7.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1844664-905cf6cad2e032a7.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1848342-317c9e4afa65a3ff.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1848342-317c9e4afa65a3ff.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1855080-08b28181b7cb2470.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1855080-08b28181b7cb2470.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1872733-2377f456a57ad32c.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1872733-2377f456a57ad32c.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1872735-0989e51d2248ce1e.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1872735-0989e51d2248ce1e.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1872737-f8e1ad3b6705b766.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1872737-f8e1ad3b6705b766.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1872755-2c81d3267b89f124.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1872755-2c81d3267b89f124.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1873290-ff7f8e4cee15b75a.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1873290-ff7f8e4cee15b75a.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1878938-70ee2af6fdf66004.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1878938-70ee2af6fdf66004.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug-1901654-69b9f35d11cd0c75.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug-1901654-69b9f35d11cd0c75.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/bug_1543048_and_1668503-7ead4e15faaab778.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/bug_1543048_and_1668503-7ead4e15faaab778.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/convert-keystone-to-flask-80d980e239b662b0.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/convert-keystone-to-flask-80d980e239b662b0.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/deprecate-json-formatted-policy-file-95f6307f88358f58.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/deprecate-json-formatted-policy-file-95f6307f88358f58.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/deprecate-v2-apis-894284c17be881d2.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/deprecate-v2-apis-894284c17be881d2.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/deprecated-as-of-mitaka-8534e43fa40c1d09.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/deprecated-as-of-mitaka-8534e43fa40c1d09.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/deprecated-as-of-ocata-a5b2f1e3e39f818e.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/deprecated-as-of-ocata-a5b2f1e3e39f818e.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/deprecated-as-of-queens-8ad7f826e4f08f57.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/deprecated-as-of-queens-8ad7f826e4f08f57.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/deprecated-as-of-rocky-60b2fa05d07d3a28.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/deprecated-as-of-rocky-60b2fa05d07d3a28.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/deprecated-socket_timeout-option-d3358b4f2310706c.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/deprecated-socket_timeout-option-d3358b4f2310706c.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/domain-level-limit-support-60e1e330d06227ed.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/domain-level-limit-support-60e1e330d06227ed.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/eventlet-cleanup-f35fc5f83c16ea1c.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/eventlet-cleanup-f35fc5f83c16ea1c.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/extensions-to-core-a0d270d216d47276.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/extensions-to-core-a0d270d216d47276.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/implied-roles-026f401adc0f7fb6.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/implied-roles-026f401adc0f7fb6.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/integrate-osprofiler-ad0e16a542b12899.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/integrate-osprofiler-ad0e16a542b12899.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/is-admin-24b34238c83b3a82.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/is-admin-24b34238c83b3a82.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/limits-api-refactor-05abf9e6c2e75852.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/limits-api-refactor-05abf9e6c2e75852.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/mapping_populate-521d92445505b8a3.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/mapping_populate-521d92445505b8a3.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/oslo.cache-a9ce47bfa8809efa.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/oslo.cache-a9ce47bfa8809efa.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/project-tags-1e72a6779d9d02c5.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/project-tags-1e72a6779d9d02c5.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/remove-token-auth-middleware-5ea3b3734ce1d9e6.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/remove-token-auth-middleware-5ea3b3734ce1d9e6.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/removed-as-of-mitaka-9ff14f87d0b98e7e.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/removed-as-of-mitaka-9ff14f87d0b98e7e.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/removed-as-of-newton-721c06b5dcb1b34a.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/removed-as-of-newton-721c06b5dcb1b34a.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/removed-as-of-ocata-436bb4b839e74494.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/removed-as-of-ocata-436bb4b839e74494.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/removed-as-of-pike-deadbeefdeadbeef.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/removed-as-of-pike-deadbeefdeadbeef.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/removed-as-of-queens-94c04e88c08f89aa.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/removed-as-of-queens-94c04e88c08f89aa.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/removed-as-of-rocky-f44c3ba7c3e73d01.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/removed-as-of-rocky-f44c3ba7c3e73d01.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/removed-as-of-stein-5eb23253b72ab54e.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/removed-as-of-stein-5eb23253b72ab54e.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/removed-as-of-train-92b2942a680eb859.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/removed-as-of-train-92b2942a680eb859.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/resource-backend-sql-only-03154d8712b36bd0.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/resource-backend-sql-only-03154d8712b36bd0.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/revert-v2-token-issued-for-non-default-domain-25ea5337f158ef13.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/revert-v2-token-issued-for-non-default-domain-25ea5337f158ef13.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/scope-and-default-roles-a733c235731bb558.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/scope-and-default-roles-a733c235731bb558.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/support_encrypted_credentials_at_rest-93dcb67b3508e91a.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/support_encrypted_credentials_at_rest-93dcb67b3508e91a.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/switch-to-alembic-1fa5248f0ce824ae.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/switch-to-alembic-1fa5248f0ce824ae.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/token_expiration_to_match_application_credential-56d058355a9f240d.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/token_expiration_to_match_application_credential-56d058355a9f240d.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/notes/unified-limit-api-improvment-b34d18769d18a0a7.yaml` & `keystone-25.0.0.0rc1/releasenotes/notes/unified-limit-api-improvment-b34d18769d18a0a7.yaml`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/source/conf.py` & `keystone-25.0.0.0rc1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/source/index.rst` & `keystone-25.0.0.0rc1/releasenotes/source/index.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po` & `keystone-25.0.0.0rc1/releasenotes/source/locale/en_GB/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po` & `keystone-25.0.0.0rc1/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po` & `keystone-25.0.0.0rc1/releasenotes/source/locale/ja/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po` & `keystone-25.0.0.0rc1/releasenotes/source/locale/ko_KR/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/source/pike.rst` & `keystone-25.0.0.0rc1/releasenotes/source/pike.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/releasenotes/source/unreleased.rst` & `keystone-25.0.0.0rc1/releasenotes/source/unreleased.rst`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/requirements.txt` & `keystone-25.0.0.0rc1/requirements.txt`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/setup.cfg` & `keystone-25.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/setup.py` & `keystone-25.0.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/test-requirements.txt` & `keystone-25.0.0.0rc1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/tools/cover.sh` & `keystone-25.0.0.0rc1/tools/cover.sh`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/tools/fast8.sh` & `keystone-25.0.0.0rc1/tools/fast8.sh`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/tools/sample_data.sh` & `keystone-25.0.0.0rc1/tools/sample_data.sh`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/tools/test-setup.sh` & `keystone-25.0.0.0rc1/tools/test-setup.sh`

 * *Files identical despite different names*

### Comparing `keystone-25.0.0/tox.ini` & `keystone-25.0.0.0rc1/tox.ini`

 * *Files identical despite different names*

