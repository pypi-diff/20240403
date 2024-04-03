# Comparing `tmp/ccs-digitalmarketplace-utils-65.4.0.tar.gz` & `tmp/ccs-digitalmarketplace-utils-66.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ccs-digitalmarketplace-utils-65.4.0.tar", last modified: Wed Apr  3 09:25:46 2024, max compression
+gzip compressed data, was "ccs-digitalmarketplace-utils-66.0.0rc1.tar", last modified: Tue Feb 20 09:56:38 2024, max compression
```

## Comparing `ccs-digitalmarketplace-utils-65.4.0.tar` & `ccs-digitalmarketplace-utils-66.0.0rc1.tar`

### file list

```diff
@@ -1,78 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:25:46.727170 ccs-digitalmarketplace-utils-65.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/LICENCE
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-03 09:25:46.727170 ccs-digitalmarketplace-utils-65.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:25:46.719170 ccs-digitalmarketplace-utils-65.4.0/ccs_digitalmarketplace_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-03 09:25:46.000000 ccs-digitalmarketplace-utils-65.4.0/ccs_digitalmarketplace_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-03 09:25:46.000000 ccs-digitalmarketplace-utils-65.4.0/ccs_digitalmarketplace_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 09:25:46.000000 ccs-digitalmarketplace-utils-65.4.0/ccs_digitalmarketplace_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-03 09:25:46.000000 ccs-digitalmarketplace-utils-65.4.0/ccs_digitalmarketplace_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-03 09:25:46.000000 ccs-digitalmarketplace-utils-65.4.0/ccs_digitalmarketplace_utils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:25:46.723170 ccs-digitalmarketplace-utils-65.4.0/dmutils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/access_control.py
--rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/asset_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/cloudfoundry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/cookie_probe.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/csv_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/dates.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/deprecation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/direct_plus_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/dmp_so_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/documents.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:25:46.723170 ccs-digitalmarketplace-utils-65.4.0/dmutils/email/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10873 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/email/dm_mailchimp.py
--rw-r--r--   0 runner    (1001) docker     (127)     9624 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/email/dm_notify.py
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/email/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/email/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     7911 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/email/tokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/email/user_account_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/env_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:25:46.723170 ccs-digitalmarketplace-utils-65.4.0/dmutils/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/errors/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/errors/frontend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/external.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/feature_flag.py
--rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/flask.py
--rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/flask_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     8900 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/formats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:25:46.727170 ccs-digitalmarketplace-utils-65.4.0/dmutils/forms/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/forms/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     8171 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/forms/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/forms/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/forms/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/forms/mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/forms/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/forms/widgets.py
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/jinja2_environment.py
--rw-r--r--   0 runner    (1001) docker     (127)    11943 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/ods.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:25:46.727170 ccs-digitalmarketplace-utils-65.4.0/dmutils/presenters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/presenters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6516 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/presenters/compliance_communications.py
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/presenters/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/proxy_fix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:25:46.727170 ccs-digitalmarketplace-utils-65.4.0/dmutils/repoutils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/repoutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/request_id.py
--rw-r--r--   0 runner    (1001) docker     (127)    10439 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/s3.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/service_attribute.py
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/session.py
--rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/timing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:25:46.727170 ccs-digitalmarketplace-utils-65.4.0/dmutils/view_helpers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/view_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/view_helpers/compliance_communications.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      384 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/view_helpers/frameworks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/view_helpers/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     9537 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/dmutils/views.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 09:25:46.727170 ccs-digitalmarketplace-utils-65.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-03 09:25:35.000000 ccs-digitalmarketplace-utils-65.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:56:38.729277 ccs-digitalmarketplace-utils-66.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-02-20 09:56:38.729277 ccs-digitalmarketplace-utils-66.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:56:38.721275 ccs-digitalmarketplace-utils-66.0.0rc1/ccs_digitalmarketplace_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-02-20 09:56:38.000000 ccs-digitalmarketplace-utils-66.0.0rc1/ccs_digitalmarketplace_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-02-20 09:56:38.000000 ccs-digitalmarketplace-utils-66.0.0rc1/ccs_digitalmarketplace_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 09:56:38.000000 ccs-digitalmarketplace-utils-66.0.0rc1/ccs_digitalmarketplace_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-02-20 09:56:38.000000 ccs-digitalmarketplace-utils-66.0.0rc1/ccs_digitalmarketplace_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-02-20 09:56:38.000000 ccs-digitalmarketplace-utils-66.0.0rc1/ccs_digitalmarketplace_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:56:38.725276 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/access_control.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1433 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/asset_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/cloudfoundry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2554 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/cookie_probe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/csv_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2772 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/deprecation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5098 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/direct_plus_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/dmp_so_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12807 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/documents.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:56:38.725276 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/email/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10873 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/email/dm_mailchimp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9624 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/email/dm_notify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/email/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/email/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7911 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/email/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/email/user_account_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/env_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:56:38.725276 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/errors/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/errors/frontend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3752 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/feature_flag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5128 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/flask.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/flask_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8900 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/formats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:56:38.729277 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5285 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8065 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4206 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/jinja2_environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11943 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/ods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/proxy_fix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 09:56:38.729277 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/repoutils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/repoutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7760 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/request_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10458 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/service_attribute.py
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5502 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7995 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1391 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2903 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9537 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-20 09:56:38.729277 ccs-digitalmarketplace-utils-66.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-02-20 09:56:27.000000 ccs-digitalmarketplace-utils-66.0.0rc1/setup.py
```

### Comparing `ccs-digitalmarketplace-utils-65.4.0/LICENCE` & `ccs-digitalmarketplace-utils-66.0.0rc1/LICENCE`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/README.md` & `ccs-digitalmarketplace-utils-66.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/ccs_digitalmarketplace_utils.egg-info/SOURCES.txt` & `ccs-digitalmarketplace-utils-66.0.0rc1/ccs_digitalmarketplace_utils.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -53,15 +53,8 @@
 dmutils/forms/errors.py
 dmutils/forms/fields.py
 dmutils/forms/filters.py
 dmutils/forms/helpers.py
 dmutils/forms/mixins.py
 dmutils/forms/validators.py
 dmutils/forms/widgets.py
-dmutils/presenters/__init__.py
-dmutils/presenters/compliance_communications.py
-dmutils/presenters/helpers.py
-dmutils/repoutils/__init__.py
-dmutils/view_helpers/__init__.py
-dmutils/view_helpers/compliance_communications.py
-dmutils/view_helpers/frameworks.py
-dmutils/view_helpers/pagination.py
+dmutils/repoutils/__init__.py
```

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/access_control.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/access_control.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/asset_fingerprint.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/asset_fingerprint.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/authentication.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/authentication.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/cloudfoundry.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/cloudfoundry.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/config.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/config.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,20 +9,17 @@
             elif isinstance(value, int):
                 app.config[key] = _convert_to_int_or_fail(key, os.environ[key])
             else:
                 app.config[key] = os.environ[key]
     app.config['DM_ENVIRONMENT'] = os.environ.get('DM_ENVIRONMENT',
                                                   'development')
 
-    # From Flask 1.0 onwards, ENV is set to either 'production' (default) or 'development'.
-    # If set as 'development' then debug mode will be enabled.
-    # If left as 'production' when running a local development server, it gives an unsettling warning message.
-    # See http://flask.pocoo.org/docs/1.0/config/#environment-and-debug-features
-    if app.config['DM_ENVIRONMENT'] == 'development':
-        app.config['ENV'] = 'development'
+    # From Flask 2.2 onwards, ENV is no longer uses.
+    # To run in debug mode we need to pass the debug flag into the flask command to run the app
+    # See https://flask.palletsprojects.com/en/2.2.x/config/#debug-mode
 
 
 def _convert_to_boolean_or_fail(key, value):
     result = convert_to_boolean(value)
     if not isinstance(result, bool):
         raise ValueError("{} must be boolean".format(key))
     return result
```

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/cookie_probe.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/cookie_probe.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/csv_generator.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/csv_generator.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/dates.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/dates.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/deprecation.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/deprecation.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/direct_plus_client.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/direct_plus_client.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/documents.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/documents.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/email/dm_mailchimp.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/email/dm_mailchimp.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/email/dm_notify.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/email/dm_notify.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/email/helpers.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/email/helpers.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/email/tokens.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/email/tokens.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/email/user_account_email.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/email/user_account_email.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/env_helpers.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/env_helpers.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/errors/api.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/errors/api.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
     try:
         # initially we'll try and assume this is an HTTPException of some sort.  for the most part, the default
         # HTTPExceptions render themselves in the desired way if returned as a response. the only change we want to
         # make is to enclose the error description in json.
         response = e.get_response()
         response.set_data(json.dumps({"error": e.description}))
-        response.mimetype = current_app.config["JSONIFY_MIMETYPE"]
+        response.mimetype = current_app.json.mimetype
 
         return response
     except Exception:
         # either `e` wasn't an HTTPException or something went wrong in trying to jsonify it
         return jsonify(error="Internal error"), 500
```

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/errors/frontend.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/errors/frontend.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/external.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/external.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/feature_flag.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/feature_flag.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/filters.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/filters.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/flask.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/flask.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/flask_init.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/flask_init.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/formats.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/formats.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/forms/errors.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/errors.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/forms/fields.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,26 +34,17 @@
     DMUnitInput,
 )
 
 from .filters import strip_whitespace
 from .validators import EmailValidator
 
 
-__all__ = [
-    'DMBooleanField',
-    'DMDecimalField',
-    'DMHiddenField',
-    'DMIntegerField',
-    'DMRadioField',
-    'DMStringField',
-    'DMEmailField',
-    'DMStripWhitespaceStringField',
-    'DMDateField',
-    'DMFileField',
-]
+__all__ = ['DMBooleanField', 'DMDecimalField', 'DMHiddenField', 'DMIntegerField',
+           'DMRadioField', 'DMStringField', 'DMEmailField', 'DMStripWhitespaceStringField',
+           'DMDateField']
 
 
 class DMBooleanField(DMFieldMixin, wtforms.fields.BooleanField):
     widget = DMCheckboxInput(hide_question=True)
 
     @property
     def href(self):
@@ -254,11 +245,7 @@
         # year}.errors.  In the case where the validator chain hasn't added
         # errors to any of day month or year, we will add the errors to all the
         # fields so that all inputs get highlighted.
         if self.errors and not any((self.year.errors, self.month.errors, self.day.errors)):
             self.year.errors = self.errors
             self.month.errors = self.errors
             self.day.errors = self.errors
-
-
-class DMFileField(DMFieldMixin, wtforms.fields.FileField):
-    pass
```

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/forms/helpers.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/helpers.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/forms/mixins.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/mixins.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/forms/validators.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/validators.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/forms/widgets.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/jinja2_environment.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/jinja2_environment.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/logging.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/logging.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/ods.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/ods.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/proxy_fix.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/proxy_fix.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/request_id.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/request_id.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/s3.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/s3.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 default_region = "eu-west-2"
 
 
 class S3(object):
     def __init__(self, bucket_name, region_name=default_region, **kwargs):
         if flask.current_app:
             app = flask.current_app
-            if app.env == "development" and app.config.get("DM_S3_ENDPOINT_URL"):
+            if app.debug and app.config.get("DM_S3_ENDPOINT_URL"):
                 kwargs.setdefault("endpoint_url", app.config["DM_S3_ENDPOINT_URL"])
         self._resource = boto3.resource("s3", region_name=region_name, **kwargs)
         self._bucket = self._resource.Bucket(bucket_name)
 
     @property
     def bucket_name(self):
         return self._bucket.name
@@ -136,39 +136,38 @@
         """
         path = self._normalize_path(path)
         if self.path_exists(path):
             # Because we are using cloudfront as a load balancer for the assets
             # the URL we generate needs to include the region.
             # However boto3 does not do this so we are having to make use of
             # the AWS CLI to create this URL.
-            result = subprocess.run(
-                [
-                    'aws',
-                    's3',
-                    'presign',
-                    f's3://{self._bucket.name}/{path}',
-                    '--expires-in',
-                    str(expires_in)
-                ],
-                stdout=subprocess.PIPE,
-                check=True,
-            )
-
-            return result.stdout.decode()
-
-            # If we were not using cloudfront as the load balanacer then
-            # the following code would work
-            # return self._resource.meta.client.generate_presigned_url(
-            #     "get_object",
-            #     Params={
-            #         "Bucket": self._bucket.name,
-            #         "Key": path,
-            #     },
-            #     ExpiresIn=expires_in,
-            # )
+            if os.getenv("DM_ENVIRONMENT", None) == "native-aws":
+                result = subprocess.run(
+                    [
+                        'aws',
+                        's3',
+                        'presign',
+                        f's3://{self._bucket.name}/{path}',
+                        '--expires-in',
+                        str(expires_in)
+                    ],
+                    stdout=subprocess.PIPE,
+                    check=True,
+                )
+
+                return result.stdout.decode()
+            else:
+                return self._resource.meta.client.generate_presigned_url(
+                    "get_object",
+                    Params={
+                        "Bucket": self._bucket.name,
+                        "Key": path,
+                    },
+                    ExpiresIn=expires_in,
+                )
 
     def _get_key(self, path):
         path = self._normalize_path(path)
         try:
             obj = self._bucket.Object(path)
             obj.load()
         except S3ResponseError:
```

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/service_attribute.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/service_attribute.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/session.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/session.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/status.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/status.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/timing.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/timing.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/urls.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/urls.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/user.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/user.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/dmutils/views.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/dmutils/views.py`

 * *Files identical despite different names*

### Comparing `ccs-digitalmarketplace-utils-65.4.0/setup.py` & `ccs-digitalmarketplace-utils-66.0.0rc1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,30 +21,30 @@
     description='Common utils for Digital Marketplace apps.',
     long_description=__doc__,
     packages=find_packages(),
     package_data={'dmutils': ['py.typed']},
     include_package_data=True,
     install_requires=[
         'Flask-WTF>=1.2.1',
-        'Flask>=2.0,<2.1',
+        'Flask>=2.3,<3',
         'Flask-gzip>=0.2',
-        'Flask-Login>=0.6.2',
-        'Flask-Session<0.5.0,>=0.4.1',
+        'Flask-Login>=0.6.3',
+        'Flask-Session<0.6.0,>=0.5.0',
         'boto3<2,>=1.7.83',
         'contextlib2>=21.6.0',
         'cryptography>=41.0.4',
         'ccs-digitalmarketplace-apiclient>=25.0.0',
         'govuk-country-register>=0.5.0',
         'mailchimp3==3.0.21',
         'requests>=2.22.0,<3',
         'redis>=5.0.1',
         'fleep<1.1,>=1.0.1',
         'notifications-python-client>=8.1.0,<9.0.0',
         'odfpy>=1.4.1',
         'python-json-logger>=2.0.7,<3.0.0',
         'pytz',
         'unicodecsv>=0.14.1',
-        'werkzeug>=2,<2.1',
+        'werkzeug>=2.3,<3',
         'workdays>=1.4',
     ],
     python_requires=">=3.9,<3.12",
 )
```

