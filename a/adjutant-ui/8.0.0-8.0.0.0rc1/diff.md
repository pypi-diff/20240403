# Comparing `tmp/adjutant-ui-8.0.0.tar.gz` & `tmp/adjutant-ui-8.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adjutant-ui-8.0.0.tar", last modified: Wed Apr  3 11:51:59 2024, max compression
+gzip compressed data, was "adjutant-ui-8.0.0.0rc1.tar", last modified: Fri Mar 15 14:43:41 2024, max compression
```

## Comparing `adjutant-ui-8.0.0.tar` & `adjutant-ui-8.0.0.0rc1.tar`

### file list

```diff
@@ -1,207 +1,207 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.384459 adjutant-ui-8.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      698 2024-04-03 11:51:59.000000 adjutant-ui-8.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2426 2024-04-03 11:51:59.000000 adjutant-ui-8.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1444 2024-04-03 11:51:59.384459 adjutant-ui-8.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.344460 adjutant-ui-8.0.0/adjutant_ui/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.344460 adjutant-ui-8.0.0/adjutant_ui/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24060 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/api/adjutant.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.348460 adjutant-ui-8.0.0/adjutant_ui/content/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.348460 adjutant-ui-8.0.0/adjutant_ui/content/default/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/default/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      798 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/default/panel.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.332460 adjutant-ui-8.0.0/adjutant_ui/content/default/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.348460 adjutant-ui-8.0.0/adjutant_ui/content/default/templates/default/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       28 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/default/templates/default/base.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.348460 adjutant-ui-8.0.0/adjutant_ui/content/email/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/email/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2054 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/email/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      781 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/email/panel.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.332460 adjutant-ui-8.0.0/adjutant_ui/content/email/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.348460 adjutant-ui-8.0.0/adjutant_ui/content/email/templates/email/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/email/templates/email/_change.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/email/templates/email/change.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      772 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/email/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1245 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/email/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.348460 adjutant-ui-8.0.0/adjutant_ui/content/forgot_password/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/forgot_password/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2241 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/forgot_password/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/forgot_password/panel.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.332460 adjutant-ui-8.0.0/adjutant_ui/content/forgot_password/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.348460 adjutant-ui-8.0.0/adjutant_ui/content/forgot_password/templates/auth/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/forgot_password/templates/auth/_login_page.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.352460 adjutant-ui-8.0.0/adjutant_ui/content/forgot_password/templates/forgot_password/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1658 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/forgot_password/templates/forgot_password/_forgot_password_form.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      462 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/forgot_password/templates/forgot_password/_index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/forgot_password/templates/forgot_password/_sent.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/forgot_password/templates/forgot_password/_sent_text.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/forgot_password/templates/forgot_password/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/forgot_password/templates/forgot_password/sent.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      907 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/forgot_password/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      987 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/forgot_password/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.352460 adjutant-ui-8.0.0/adjutant_ui/content/notifications/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/notifications/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/notifications/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3566 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/notifications/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3701 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/notifications/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.332460 adjutant-ui-8.0.0/adjutant_ui/content/notifications/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.356459 adjutant-ui-8.0.0/adjutant_ui/content/notifications/templates/notifications/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/notifications/templates/notifications/detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/notifications/templates/notifications/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/notifications/templates/notifications/table_override.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      844 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/notifications/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2576 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/notifications/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.356459 adjutant-ui-8.0.0/adjutant_ui/content/project_users/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/project_users/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5133 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/project_users/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      815 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/project_users/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5564 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/project_users/tables.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.336460 adjutant-ui-8.0.0/adjutant_ui/content/project_users/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.356459 adjutant-ui-8.0.0/adjutant_ui/content/project_users/templates/project_users/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1009 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/project_users/templates/project_users/_invite.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      572 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/project_users/templates/project_users/_role_help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/project_users/templates/project_users/_update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/project_users/templates/project_users/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/project_users/templates/project_users/invite.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/project_users/templates/project_users/update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      918 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/project_users/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3231 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/project_users/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.360459 adjutant-ui-8.0.0/adjutant_ui/content/quota/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/quota/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2525 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/quota/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      831 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/quota/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6589 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/quota/tables.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.336460 adjutant-ui-8.0.0/adjutant_ui/content/quota/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.360459 adjutant-ui-8.0.0/adjutant_ui/content/quota/templates/quota/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      813 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/quota/templates/quota/_index_help.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2049 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/quota/templates/quota/_update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      596 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/quota/templates/quota/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/quota/templates/quota/region_detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/quota/templates/quota/size_detail.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/quota/templates/quota/update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1064 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/quota/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5985 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/quota/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.364459 adjutant-ui-8.0.0/adjutant_ui/content/signup/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/signup/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2251 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/signup/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      749 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/signup/panel.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.336460 adjutant-ui-8.0.0/adjutant_ui/content/signup/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.364459 adjutant-ui-8.0.0/adjutant_ui/content/signup/templates/auth/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/signup/templates/auth/_login_page.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.364459 adjutant-ui-8.0.0/adjutant_ui/content/signup/templates/signup/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/signup/templates/signup/_index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1500 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/signup/templates/signup/_signup_form.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      430 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/signup/templates/signup/_submitted.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      754 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/signup/templates/signup/_submitted_text.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/signup/templates/signup/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/signup/templates/signup/submitted.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/signup/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1073 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/signup/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.368459 adjutant-ui-8.0.0/adjutant_ui/content/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/tasks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1934 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/tasks/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      786 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/tasks/panel.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7512 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/tasks/tables.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4169 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/tasks/tabs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.336460 adjutant-ui-8.0.0/adjutant_ui/content/tasks/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.368459 adjutant-ui-8.0.0/adjutant_ui/content/tasks/templates/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/tasks/templates/tasks/_task_detail_actions.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/tasks/templates/tasks/_task_detail_notes.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1477 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/tasks/templates/tasks/_task_detail_overview.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/tasks/templates/tasks/_update.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/tasks/templates/tasks/index.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/tasks/templates/tasks/update.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.368459 adjutant-ui-8.0.0/adjutant_ui/content/tasks/templatetags/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/tasks/templatetags/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/tasks/templatetags/task_filters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      932 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/tasks/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3975 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/tasks/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.372459 adjutant-ui-8.0.0/adjutant_ui/content/token/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/token/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2997 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/token/forms.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      789 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/token/panel.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.336460 adjutant-ui-8.0.0/adjutant_ui/content/token/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.372459 adjutant-ui-8.0.0/adjutant_ui/content/token/templates/token/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/token/templates/token/_emailtokenconfirm.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/token/templates/token/_setpassword.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1559 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/token/templates/token/_setpassword_form.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/token/templates/token/_tokenconfirm.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      932 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/token/templates/token/_tokenconfirm_form.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/token/templates/token/emailtokenconfirm.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/token/templates/token/setpassword.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/token/templates/token/tokenconfirm.html
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/token/urls.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5432 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/content/token/views.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.372459 adjutant-ui-8.0.0/adjutant_ui/dashboards/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/dashboards/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      997 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/dashboards/forgot_password_dash.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      913 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/dashboards/management.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      930 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/dashboards/signup_dash.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      921 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/dashboards/token_dash.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.376459 adjutant-ui-8.0.0/adjutant_ui/enabled/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/enabled/_6000_management.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/enabled/_6001_adjutant_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/enabled/_6010_token.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/enabled/_6015_forgot_password.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/enabled/_6020_management_access_control_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/enabled/_6021_management_project_users.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/enabled/_6025_signup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      364 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/enabled/_6070_settings_update_email.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/enabled/_6080_management_quota.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/enabled/_6090_management_task_list.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      455 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/enabled/_6100_management_notification_list.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/enabled/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5234 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/karma.conf.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.336460 adjutant-ui-8.0.0/adjutant_ui/templates/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.376459 adjutant-ui-8.0.0/adjutant_ui/templates/auth/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/templates/auth/_login_page.html
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.380459 adjutant-ui-8.0.0/adjutant_ui/templatetags/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/templatetags/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1422 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/templatetags/relabel_username_field.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.380459 adjutant-ui-8.0.0/adjutant_ui/test/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/test/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.380459 adjutant-ui-8.0.0/adjutant_ui/test/api_tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/test/api_tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/test/api_tests/test_rest_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      760 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/test/helpers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.380459 adjutant-ui-8.0.0/adjutant_ui/test/integration_tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/test/integration_tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1313 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/test/settings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      696 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/test/test_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      629 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/adjutant_ui/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.344460 adjutant-ui-8.0.0/adjutant_ui.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1444 2024-04-03 11:51:59.000000 adjutant-ui-8.0.0/adjutant_ui.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6804 2024-04-03 11:51:59.000000 adjutant-ui-8.0.0/adjutant_ui.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-03 11:51:59.000000 adjutant-ui-8.0.0/adjutant_ui.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-03 11:51:59.000000 adjutant-ui-8.0.0/adjutant_ui.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-04-03 11:51:59.000000 adjutant-ui-8.0.0/adjutant_ui.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       35 2024-04-03 11:51:59.000000 adjutant-ui-8.0.0/adjutant_ui.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2024-04-03 11:51:59.000000 adjutant-ui-8.0.0/adjutant_ui.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/babel-django.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/babel-djangojs.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.380459 adjutant-ui-8.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5569 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/doc/Makefile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.384459 adjutant-ui-8.0.0/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4320 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3291 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/doc/source/configuration.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1426 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/doc/source/installation.rst
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      838 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      793 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/requirements.txt
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    16846 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/run_tests.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      798 2024-04-03 11:51:59.384459 adjutant-ui-8.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2636 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/test-shim.js
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-03 11:51:59.384459 adjutant-ui-8.0.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2402 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/tools/install_venv.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5920 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/tools/install_venv_common.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      506 2024-04-03 11:51:30.000000 adjutant-ui-8.0.0/tools/with_venv.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2815 2024-04-03 11:51:31.000000 adjutant-ui-8.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.106299 adjutant-ui-8.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      328 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      698 2024-03-15 14:43:40.000000 adjutant-ui-8.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2436 2024-03-15 14:43:40.000000 adjutant-ui-8.0.0.0rc1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1449 2024-03-15 14:43:41.106299 adjutant-ui-8.0.0.0rc1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.078295 adjutant-ui-8.0.0.0rc1/adjutant_ui/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.078295 adjutant-ui-8.0.0.0rc1/adjutant_ui/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24060 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/api/adjutant.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.078295 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.078295 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/default/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/default/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      798 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/default/panel.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.070294 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/default/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.078295 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/default/templates/default/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       28 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/default/templates/default/base.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.078295 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/email/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/email/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2054 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/email/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      781 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/email/panel.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.070294 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/email/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.082295 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/email/templates/email/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/email/templates/email/_change.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/email/templates/email/change.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      772 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/email/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1245 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/email/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.082295 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/forgot_password/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/forgot_password/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2241 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/forgot_password/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/forgot_password/panel.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.070294 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/forgot_password/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.082295 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/forgot_password/templates/auth/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/forgot_password/templates/auth/_login_page.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.082295 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/forgot_password/templates/forgot_password/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1658 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/forgot_password/templates/forgot_password/_forgot_password_form.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      462 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/forgot_password/templates/forgot_password/_index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      434 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/forgot_password/templates/forgot_password/_sent.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      751 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/forgot_password/templates/forgot_password/_sent_text.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/forgot_password/templates/forgot_password/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/forgot_password/templates/forgot_password/sent.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      907 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/forgot_password/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      987 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/forgot_password/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.082295 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/notifications/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/notifications/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      811 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/notifications/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3566 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/notifications/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3701 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/notifications/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.070294 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/notifications/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.082295 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/notifications/templates/notifications/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/notifications/templates/notifications/detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      233 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/notifications/templates/notifications/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/notifications/templates/notifications/table_override.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      844 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/notifications/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2576 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/notifications/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.086296 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/project_users/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/project_users/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5133 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/project_users/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      815 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/project_users/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5564 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/project_users/tables.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.070294 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/project_users/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.086296 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/project_users/templates/project_users/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1009 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/project_users/templates/project_users/_invite.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      572 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/project_users/templates/project_users/_role_help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/project_users/templates/project_users/_update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/project_users/templates/project_users/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/project_users/templates/project_users/invite.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/project_users/templates/project_users/update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      918 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/project_users/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3231 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/project_users/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.086296 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/quota/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/quota/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2525 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/quota/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      831 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/quota/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6589 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/quota/tables.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.070294 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/quota/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.090297 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/quota/templates/quota/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      813 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/quota/templates/quota/_index_help.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2049 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/quota/templates/quota/_update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      596 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/quota/templates/quota/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/quota/templates/quota/region_detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/quota/templates/quota/size_detail.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/quota/templates/quota/update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1064 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/quota/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5985 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/quota/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.090297 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/signup/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/signup/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2251 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/signup/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      749 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/signup/panel.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.070294 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/signup/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.090297 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/signup/templates/auth/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/signup/templates/auth/_login_page.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.090297 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/signup/templates/signup/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      444 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/signup/templates/signup/_index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1500 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/signup/templates/signup/_signup_form.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      430 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/signup/templates/signup/_submitted.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      754 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/signup/templates/signup/_submitted_text.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/signup/templates/signup/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/signup/templates/signup/submitted.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      810 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/signup/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1073 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/signup/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.094297 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/tasks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1934 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/tasks/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      786 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/tasks/panel.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7512 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/tasks/tables.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4169 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/tasks/tabs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.070294 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/tasks/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.094297 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/tasks/templates/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/tasks/templates/tasks/_task_detail_actions.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/tasks/templates/tasks/_task_detail_notes.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1477 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/tasks/templates/tasks/_task_detail_overview.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/tasks/templates/tasks/_update.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/tasks/templates/tasks/index.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/tasks/templates/tasks/update.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.094297 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/tasks/templatetags/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/tasks/templatetags/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/tasks/templatetags/task_filters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      932 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/tasks/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3975 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/tasks/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.098298 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/token/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/token/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2997 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/token/forms.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      789 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/token/panel.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.070294 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/token/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.098298 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/token/templates/token/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/token/templates/token/_emailtokenconfirm.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/token/templates/token/_setpassword.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1559 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/token/templates/token/_setpassword_form.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/token/templates/token/_tokenconfirm.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      932 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/token/templates/token/_tokenconfirm_form.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      341 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/token/templates/token/emailtokenconfirm.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      327 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/token/templates/token/setpassword.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/token/templates/token/tokenconfirm.html
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/token/urls.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5432 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/content/token/views.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.098298 adjutant-ui-8.0.0.0rc1/adjutant_ui/dashboards/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/dashboards/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      997 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/dashboards/forgot_password_dash.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      913 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/dashboards/management.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      930 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/dashboards/signup_dash.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      921 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/dashboards/token_dash.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.102299 adjutant-ui-8.0.0.0rc1/adjutant_ui/enabled/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/enabled/_6000_management.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/enabled/_6001_adjutant_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/enabled/_6010_token.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/enabled/_6015_forgot_password.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/enabled/_6020_management_access_control_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      391 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/enabled/_6021_management_project_users.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/enabled/_6025_signup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      364 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/enabled/_6070_settings_update_email.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/enabled/_6080_management_quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      422 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/enabled/_6090_management_task_list.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      455 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/enabled/_6100_management_notification_list.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/enabled/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5234 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/karma.conf.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.074294 adjutant-ui-8.0.0.0rc1/adjutant_ui/templates/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.102299 adjutant-ui-8.0.0.0rc1/adjutant_ui/templates/auth/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/templates/auth/_login_page.html
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.102299 adjutant-ui-8.0.0.0rc1/adjutant_ui/templatetags/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/templatetags/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1422 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/templatetags/relabel_username_field.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.102299 adjutant-ui-8.0.0.0rc1/adjutant_ui/test/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/test/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.102299 adjutant-ui-8.0.0.0rc1/adjutant_ui/test/api_tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/test/api_tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      906 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/test/api_tests/test_rest_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      760 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/test/helpers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.106299 adjutant-ui-8.0.0.0rc1/adjutant_ui/test/integration_tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/test/integration_tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1313 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/test/settings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      696 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/test/test_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      629 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.078295 adjutant-ui-8.0.0.0rc1/adjutant_ui.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1449 2024-03-15 14:43:40.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6804 2024-03-15 14:43:41.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-15 14:43:40.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-15 14:43:40.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-03-15 14:43:40.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       35 2024-03-15 14:43:40.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       12 2024-03-15 14:43:40.000000 adjutant-ui-8.0.0.0rc1/adjutant_ui.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/babel-django.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/babel-djangojs.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.106299 adjutant-ui-8.0.0.0rc1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5569 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/doc/Makefile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.106299 adjutant-ui-8.0.0.0rc1/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4320 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3291 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/doc/source/configuration.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1426 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/doc/source/installation.rst
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      838 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      793 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/requirements.txt
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    16846 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/run_tests.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      798 2024-03-15 14:43:41.106299 adjutant-ui-8.0.0.0rc1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      741 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2636 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/test-shim.js
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-15 14:43:41.106299 adjutant-ui-8.0.0.0rc1/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2402 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/tools/install_venv.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5920 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/tools/install_venv_common.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      506 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/tools/with_venv.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2815 2024-03-15 14:43:16.000000 adjutant-ui-8.0.0.0rc1/tox.ini
```

### Comparing `adjutant-ui-8.0.0/AUTHORS` & `adjutant-ui-8.0.0.0rc1/AUTHORS`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/ChangeLog` & `adjutant-ui-8.0.0.0rc1/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGES
 =======
 
-8.0.0
------
+8.0.0.0rc1
+----------
 
 * Drop lower constraints and remove tests
 
 7.0.0
 -----
 
 * Update zuul settings, drop Python 3.{6,7} support
```

### Comparing `adjutant-ui-8.0.0/LICENSE` & `adjutant-ui-8.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/PKG-INFO` & `adjutant-ui-8.0.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: adjutant-ui
-Version: 8.0.0
+Version: 8.0.0.0rc1
 Summary: Adjutant User Interface
 Home-page: https://github.com/catalyst/adjutant-ui
 Author: Adrian Turjak
 Author-email: adriant@catalyst.net.nz
 License: UNKNOWN
 Description: ===========
         adjutant-ui
```

### Comparing `adjutant-ui-8.0.0/adjutant_ui/api/adjutant.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/api/adjutant.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/default/panel.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/default/panel.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/email/forms.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/email/forms.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/email/panel.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/email/panel.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/email/urls.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/email/urls.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/email/views.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/email/views.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/forgot_password/forms.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/forgot_password/forms.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/forgot_password/panel.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/forgot_password/panel.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/forgot_password/templates/forgot_password/_forgot_password_form.html` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/forgot_password/templates/forgot_password/_forgot_password_form.html`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/forgot_password/templates/forgot_password/_sent_text.html` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/forgot_password/templates/forgot_password/_sent_text.html`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/forgot_password/urls.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/forgot_password/urls.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/forgot_password/views.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/forgot_password/views.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/notifications/panel.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/notifications/panel.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/notifications/tables.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/notifications/tables.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/notifications/tabs.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/notifications/tabs.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/notifications/templates/notifications/detail.html` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/notifications/templates/notifications/detail.html`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/notifications/urls.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/notifications/urls.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/notifications/views.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/notifications/views.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/project_users/forms.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/project_users/forms.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/project_users/panel.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/project_users/panel.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/project_users/tables.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/project_users/tables.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/project_users/templates/project_users/_invite.html` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/project_users/templates/project_users/_invite.html`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/project_users/templates/project_users/_role_help.html` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/project_users/templates/project_users/_role_help.html`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/project_users/templates/project_users/_update.html` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/project_users/templates/project_users/_update.html`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/project_users/urls.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/project_users/urls.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/project_users/views.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/project_users/views.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/quota/forms.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/quota/forms.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/quota/panel.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/quota/panel.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/quota/tables.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/quota/tables.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/quota/templates/quota/_index_help.html` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/quota/templates/quota/_index_help.html`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/quota/templates/quota/_update.html` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/quota/templates/quota/_update.html`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/quota/templates/quota/index.html` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/quota/templates/quota/index.html`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/quota/urls.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/quota/urls.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/quota/views.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/quota/views.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/signup/forms.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/signup/forms.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/signup/panel.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/signup/panel.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/signup/templates/signup/_signup_form.html` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/signup/templates/signup/_signup_form.html`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/signup/templates/signup/_submitted_text.html` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/signup/templates/signup/_submitted_text.html`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/signup/urls.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/signup/urls.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/signup/views.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/signup/views.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/tasks/forms.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/tasks/forms.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/tasks/panel.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/tasks/panel.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/tasks/tables.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/tasks/tables.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/tasks/tabs.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/tasks/tabs.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/tasks/templates/tasks/_task_detail_overview.html` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/tasks/templates/tasks/_task_detail_overview.html`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/tasks/urls.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/tasks/urls.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/tasks/views.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/tasks/views.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/token/forms.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/token/forms.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/token/panel.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/token/panel.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/token/templates/token/_emailtokenconfirm.html` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/token/templates/token/_emailtokenconfirm.html`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/token/templates/token/_setpassword_form.html` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/token/templates/token/_setpassword_form.html`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/token/templates/token/_tokenconfirm_form.html` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/token/templates/token/_tokenconfirm_form.html`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/token/urls.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/token/urls.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/content/token/views.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/content/token/views.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/dashboards/forgot_password_dash.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/dashboards/forgot_password_dash.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/dashboards/management.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/dashboards/management.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/dashboards/signup_dash.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/dashboards/signup_dash.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/dashboards/token_dash.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/dashboards/token_dash.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/karma.conf.js` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/karma.conf.js`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/templatetags/relabel_username_field.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/templatetags/relabel_username_field.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/test/api_tests/test_rest_api.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/test/api_tests/test_rest_api.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/test/helpers.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/test/helpers.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/test/settings.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/test/settings.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/test/test_data.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/test/test_data.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui/version.py` & `adjutant-ui-8.0.0.0rc1/adjutant_ui/version.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/adjutant_ui.egg-info/PKG-INFO` & `adjutant-ui-8.0.0.0rc1/adjutant_ui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: adjutant-ui
-Version: 8.0.0
+Version: 8.0.0.0rc1
 Summary: Adjutant User Interface
 Home-page: https://github.com/catalyst/adjutant-ui
 Author: Adrian Turjak
 Author-email: adriant@catalyst.net.nz
 License: UNKNOWN
 Description: ===========
         adjutant-ui
```

### Comparing `adjutant-ui-8.0.0/adjutant_ui.egg-info/SOURCES.txt` & `adjutant-ui-8.0.0.0rc1/adjutant_ui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/babel-djangojs.cfg` & `adjutant-ui-8.0.0.0rc1/babel-djangojs.cfg`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/doc/Makefile` & `adjutant-ui-8.0.0.0rc1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/doc/source/conf.py` & `adjutant-ui-8.0.0.0rc1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/doc/source/configuration.rst` & `adjutant-ui-8.0.0.0rc1/doc/source/configuration.rst`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/doc/source/installation.rst` & `adjutant-ui-8.0.0.0rc1/doc/source/installation.rst`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/manage.py` & `adjutant-ui-8.0.0.0rc1/manage.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/requirements.txt` & `adjutant-ui-8.0.0.0rc1/requirements.txt`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/run_tests.sh` & `adjutant-ui-8.0.0.0rc1/run_tests.sh`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/setup.cfg` & `adjutant-ui-8.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/setup.py` & `adjutant-ui-8.0.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/test-requirements.txt` & `adjutant-ui-8.0.0.0rc1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/test-shim.js` & `adjutant-ui-8.0.0.0rc1/test-shim.js`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/tools/install_venv.py` & `adjutant-ui-8.0.0.0rc1/tools/install_venv.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/tools/install_venv_common.py` & `adjutant-ui-8.0.0.0rc1/tools/install_venv_common.py`

 * *Files identical despite different names*

### Comparing `adjutant-ui-8.0.0/tox.ini` & `adjutant-ui-8.0.0.0rc1/tox.ini`

 * *Files identical despite different names*

