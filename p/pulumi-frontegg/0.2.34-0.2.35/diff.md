# Comparing `tmp/pulumi_frontegg-0.2.34.tar.gz` & `tmp/pulumi_frontegg-0.2.35.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_frontegg-0.2.34.tar", last modified: Tue Feb 27 15:40:22 2024, max compression
+gzip compressed data, was "pulumi_frontegg-0.2.35.tar", last modified: Wed Apr  3 14:20:44 2024, max compression
```

## Comparing `pulumi_frontegg-0.2.34.tar` & `pulumi_frontegg-0.2.35.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 15:40:22.905230 pulumi_frontegg-0.2.34/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-02-27 15:40:22.905230 pulumi_frontegg-0.2.34/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-02-27 15:40:22.000000 pulumi_frontegg-0.2.34/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 15:40:22.905230 pulumi_frontegg-0.2.34/pulumi_frontegg/
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-02-27 15:40:22.000000 pulumi_frontegg-0.2.34/pulumi_frontegg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    72631 2024-02-27 15:40:22.000000 pulumi_frontegg-0.2.34/pulumi_frontegg/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-02-27 15:40:22.000000 pulumi_frontegg-0.2.34/pulumi_frontegg/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-02-27 15:40:22.000000 pulumi_frontegg-0.2.34/pulumi_frontegg/allowed_origin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 15:40:22.905230 pulumi_frontegg-0.2.34/pulumi_frontegg/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-02-27 15:40:22.000000 pulumi_frontegg-0.2.34/pulumi_frontegg/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-02-27 15:40:22.000000 pulumi_frontegg-0.2.34/pulumi_frontegg/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-02-27 15:40:22.000000 pulumi_frontegg-0.2.34/pulumi_frontegg/get_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)    71711 2024-02-27 15:40:22.000000 pulumi_frontegg-0.2.34/pulumi_frontegg/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12391 2024-02-27 15:40:22.000000 pulumi_frontegg-0.2.34/pulumi_frontegg/permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     8849 2024-02-27 15:40:22.000000 pulumi_frontegg-0.2.34/pulumi_frontegg/permission_category.py
--rw-r--r--   0 runner    (1001) docker     (127)    19743 2024-02-27 15:40:22.000000 pulumi_frontegg-0.2.34/pulumi_frontegg/prehook.py
--rw-r--r--   0 runner    (1001) docker     (127)     9754 2024-02-27 15:40:22.000000 pulumi_frontegg-0.2.34/pulumi_frontegg/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-02-27 15:40:22.000000 pulumi_frontegg-0.2.34/pulumi_frontegg/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-27 15:40:22.000000 pulumi_frontegg-0.2.34/pulumi_frontegg/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-02-27 15:40:22.000000 pulumi_frontegg-0.2.34/pulumi_frontegg/redirect_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)    21438 2024-02-27 15:40:22.000000 pulumi_frontegg-0.2.34/pulumi_frontegg/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-02-27 15:40:22.000000 pulumi_frontegg-0.2.34/pulumi_frontegg/tenant.py
--rw-r--r--   0 runner    (1001) docker     (127)    17827 2024-02-27 15:40:22.000000 pulumi_frontegg-0.2.34/pulumi_frontegg/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    17494 2024-02-27 15:40:22.000000 pulumi_frontegg-0.2.34/pulumi_frontegg/webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    93071 2024-02-27 15:40:22.000000 pulumi_frontegg-0.2.34/pulumi_frontegg/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-27 15:40:22.905230 pulumi_frontegg-0.2.34/pulumi_frontegg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-02-27 15:40:22.000000 pulumi_frontegg-0.2.34/pulumi_frontegg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-02-27 15:40:22.000000 pulumi_frontegg-0.2.34/pulumi_frontegg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 15:40:22.000000 pulumi_frontegg-0.2.34/pulumi_frontegg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-27 15:40:22.000000 pulumi_frontegg-0.2.34/pulumi_frontegg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-02-27 15:40:22.000000 pulumi_frontegg-0.2.34/pulumi_frontegg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-02-27 15:40:22.000000 pulumi_frontegg-0.2.34/pulumi_frontegg.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-27 15:40:22.905230 pulumi_frontegg-0.2.34/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-02-27 15:40:22.000000 pulumi_frontegg-0.2.34/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:20:44.945144 pulumi_frontegg-0.2.35/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-03 14:20:44.945144 pulumi_frontegg-0.2.35/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:20:44.945144 pulumi_frontegg-0.2.35/pulumi_frontegg/
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   104037 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9323 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5785 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/allowed_origin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:20:44.945144 pulumi_frontegg-0.2.35/pulumi_frontegg/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4059 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/get_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102460 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12391 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8849 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/permission_category.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19743 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/prehook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9754 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     6474 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/redirect_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21438 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11985 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17827 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17494 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)   126906 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 14:20:44.945144 pulumi_frontegg-0.2.35/pulumi_frontegg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/pulumi_frontegg.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 14:20:44.945144 pulumi_frontegg-0.2.35/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-03 14:20:44.000000 pulumi_frontegg-0.2.35/setup.py
```

### Comparing `pulumi_frontegg-0.2.34/PKG-INFO` & `pulumi_frontegg-0.2.35/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_frontegg
-Version: 0.2.34
+Version: 0.2.35
 Summary: A Pulumi package for creating and managing Frontegg resources.
 Home-page: https://github.com/MaterializeInc/pulumi-frontegg
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-frontegg
 Keywords: pulumi frontegg
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_frontegg-0.2.34/pulumi_frontegg/__init__.py` & `pulumi_frontegg-0.2.35/pulumi_frontegg/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.34/pulumi_frontegg/_inputs.py` & `pulumi_frontegg-0.2.35/pulumi_frontegg/_inputs.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,35 +15,47 @@
     'WorkspaceAdminPortalPaletteErrorArgs',
     'WorkspaceAdminPortalPaletteInfoArgs',
     'WorkspaceAdminPortalPalettePrimaryArgs',
     'WorkspaceAdminPortalPaletteSecondaryArgs',
     'WorkspaceAdminPortalPaletteSuccessArgs',
     'WorkspaceAdminPortalPaletteWarningArgs',
     'WorkspaceAuthPolicyArgs',
+    'WorkspaceBotDetectionEmailArgs',
+    'WorkspaceBruteForceProtectionEmailArgs',
     'WorkspaceBulkTenantsInvitesEmailArgs',
     'WorkspaceCaptchaPolicyArgs',
+    'WorkspaceEmailVerificationEmailArgs',
     'WorkspaceFacebookSocialLoginArgs',
     'WorkspaceGithubSocialLoginArgs',
     'WorkspaceGoogleSocialLoginArgs',
     'WorkspaceHostedLoginArgs',
+    'WorkspaceImpossibleTravelEmailArgs',
     'WorkspaceLockoutPolicyArgs',
     'WorkspaceMagicCodeEmailArgs',
     'WorkspaceMagicLinkEmailArgs',
     'WorkspaceMfaAuthenticationAppArgs',
+    'WorkspaceMfaEnrollEmailArgs',
+    'WorkspaceMfaOtcEmailArgs',
     'WorkspaceMfaPolicyArgs',
+    'WorkspaceMfaRecoveryCodeEmailArgs',
+    'WorkspaceMfaUnenrollEmailArgs',
     'WorkspaceMicrosoftSocialLoginArgs',
     'WorkspaceNewDeviceConnectedEmailArgs',
+    'WorkspaceNewMfaMethodEmailArgs',
     'WorkspaceOidcArgs',
     'WorkspacePasswordPolicyArgs',
     'WorkspacePwnedPasswordEmailArgs',
+    'WorkspaceRemoveMfaMethodEmailArgs',
     'WorkspaceResetPasswordEmailArgs',
     'WorkspaceResetPhoneNumberEmailArgs',
     'WorkspaceSamlArgs',
+    'WorkspaceSmsAuthenticationEnabledEmailArgs',
     'WorkspaceSsoDomainPolicyArgs',
     'WorkspaceSsoMultiTenantPolicyArgs',
+    'WorkspaceSuspiciousIpEmailArgs',
     'WorkspaceUserActivationEmailArgs',
     'WorkspaceUserInvitationEmailArgs',
     'WorkspaceUserUsedInvitationEmailArgs',
 ]
 
 @pulumi.input_type
 class WorkspaceAdminPortalArgs:
@@ -779,14 +791,160 @@
 
     @machine_to_machine_auth_strategy.setter
     def machine_to_machine_auth_strategy(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "machine_to_machine_auth_strategy", value)
 
 
 @pulumi.input_type
+class WorkspaceBotDetectionEmailArgs:
+    def __init__(__self__, *,
+                 from_address: pulumi.Input[str],
+                 from_name: pulumi.Input[str],
+                 html_template: pulumi.Input[str],
+                 subject: pulumi.Input[str],
+                 redirect_url: Optional[pulumi.Input[str]] = None,
+                 success_redirect_url: Optional[pulumi.Input[str]] = None):
+        pulumi.set(__self__, "from_address", from_address)
+        pulumi.set(__self__, "from_name", from_name)
+        pulumi.set(__self__, "html_template", html_template)
+        pulumi.set(__self__, "subject", subject)
+        if redirect_url is not None:
+            pulumi.set(__self__, "redirect_url", redirect_url)
+        if success_redirect_url is not None:
+            pulumi.set(__self__, "success_redirect_url", success_redirect_url)
+
+    @property
+    @pulumi.getter(name="fromAddress")
+    def from_address(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "from_address")
+
+    @from_address.setter
+    def from_address(self, value: pulumi.Input[str]):
+        pulumi.set(self, "from_address", value)
+
+    @property
+    @pulumi.getter(name="fromName")
+    def from_name(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "from_name")
+
+    @from_name.setter
+    def from_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "from_name", value)
+
+    @property
+    @pulumi.getter(name="htmlTemplate")
+    def html_template(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "html_template")
+
+    @html_template.setter
+    def html_template(self, value: pulumi.Input[str]):
+        pulumi.set(self, "html_template", value)
+
+    @property
+    @pulumi.getter
+    def subject(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "subject")
+
+    @subject.setter
+    def subject(self, value: pulumi.Input[str]):
+        pulumi.set(self, "subject", value)
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "redirect_url")
+
+    @redirect_url.setter
+    def redirect_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "redirect_url", value)
+
+    @property
+    @pulumi.getter(name="successRedirectUrl")
+    def success_redirect_url(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "success_redirect_url")
+
+    @success_redirect_url.setter
+    def success_redirect_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "success_redirect_url", value)
+
+
+@pulumi.input_type
+class WorkspaceBruteForceProtectionEmailArgs:
+    def __init__(__self__, *,
+                 from_address: pulumi.Input[str],
+                 from_name: pulumi.Input[str],
+                 html_template: pulumi.Input[str],
+                 subject: pulumi.Input[str],
+                 redirect_url: Optional[pulumi.Input[str]] = None,
+                 success_redirect_url: Optional[pulumi.Input[str]] = None):
+        pulumi.set(__self__, "from_address", from_address)
+        pulumi.set(__self__, "from_name", from_name)
+        pulumi.set(__self__, "html_template", html_template)
+        pulumi.set(__self__, "subject", subject)
+        if redirect_url is not None:
+            pulumi.set(__self__, "redirect_url", redirect_url)
+        if success_redirect_url is not None:
+            pulumi.set(__self__, "success_redirect_url", success_redirect_url)
+
+    @property
+    @pulumi.getter(name="fromAddress")
+    def from_address(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "from_address")
+
+    @from_address.setter
+    def from_address(self, value: pulumi.Input[str]):
+        pulumi.set(self, "from_address", value)
+
+    @property
+    @pulumi.getter(name="fromName")
+    def from_name(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "from_name")
+
+    @from_name.setter
+    def from_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "from_name", value)
+
+    @property
+    @pulumi.getter(name="htmlTemplate")
+    def html_template(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "html_template")
+
+    @html_template.setter
+    def html_template(self, value: pulumi.Input[str]):
+        pulumi.set(self, "html_template", value)
+
+    @property
+    @pulumi.getter
+    def subject(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "subject")
+
+    @subject.setter
+    def subject(self, value: pulumi.Input[str]):
+        pulumi.set(self, "subject", value)
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "redirect_url")
+
+    @redirect_url.setter
+    def redirect_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "redirect_url", value)
+
+    @property
+    @pulumi.getter(name="successRedirectUrl")
+    def success_redirect_url(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "success_redirect_url")
+
+    @success_redirect_url.setter
+    def success_redirect_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "success_redirect_url", value)
+
+
+@pulumi.input_type
 class WorkspaceBulkTenantsInvitesEmailArgs:
     def __init__(__self__, *,
                  from_address: pulumi.Input[str],
                  from_name: pulumi.Input[str],
                  html_template: pulumi.Input[str],
                  subject: pulumi.Input[str],
                  redirect_url: Optional[pulumi.Input[str]] = None,
@@ -902,14 +1060,87 @@
 
     @ignored_emails.setter
     def ignored_emails(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "ignored_emails", value)
 
 
 @pulumi.input_type
+class WorkspaceEmailVerificationEmailArgs:
+    def __init__(__self__, *,
+                 from_address: pulumi.Input[str],
+                 from_name: pulumi.Input[str],
+                 html_template: pulumi.Input[str],
+                 subject: pulumi.Input[str],
+                 redirect_url: Optional[pulumi.Input[str]] = None,
+                 success_redirect_url: Optional[pulumi.Input[str]] = None):
+        pulumi.set(__self__, "from_address", from_address)
+        pulumi.set(__self__, "from_name", from_name)
+        pulumi.set(__self__, "html_template", html_template)
+        pulumi.set(__self__, "subject", subject)
+        if redirect_url is not None:
+            pulumi.set(__self__, "redirect_url", redirect_url)
+        if success_redirect_url is not None:
+            pulumi.set(__self__, "success_redirect_url", success_redirect_url)
+
+    @property
+    @pulumi.getter(name="fromAddress")
+    def from_address(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "from_address")
+
+    @from_address.setter
+    def from_address(self, value: pulumi.Input[str]):
+        pulumi.set(self, "from_address", value)
+
+    @property
+    @pulumi.getter(name="fromName")
+    def from_name(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "from_name")
+
+    @from_name.setter
+    def from_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "from_name", value)
+
+    @property
+    @pulumi.getter(name="htmlTemplate")
+    def html_template(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "html_template")
+
+    @html_template.setter
+    def html_template(self, value: pulumi.Input[str]):
+        pulumi.set(self, "html_template", value)
+
+    @property
+    @pulumi.getter
+    def subject(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "subject")
+
+    @subject.setter
+    def subject(self, value: pulumi.Input[str]):
+        pulumi.set(self, "subject", value)
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "redirect_url")
+
+    @redirect_url.setter
+    def redirect_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "redirect_url", value)
+
+    @property
+    @pulumi.getter(name="successRedirectUrl")
+    def success_redirect_url(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "success_redirect_url")
+
+    @success_redirect_url.setter
+    def success_redirect_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "success_redirect_url", value)
+
+
+@pulumi.input_type
 class WorkspaceFacebookSocialLoginArgs:
     def __init__(__self__, *,
                  redirect_url: pulumi.Input[str],
                  client_id: Optional[pulumi.Input[str]] = None,
                  customised: Optional[pulumi.Input[bool]] = None,
                  secret: Optional[pulumi.Input[str]] = None):
         pulumi.set(__self__, "redirect_url", redirect_url)
@@ -1075,14 +1306,87 @@
 
     @allowed_redirect_urls.setter
     def allowed_redirect_urls(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "allowed_redirect_urls", value)
 
 
 @pulumi.input_type
+class WorkspaceImpossibleTravelEmailArgs:
+    def __init__(__self__, *,
+                 from_address: pulumi.Input[str],
+                 from_name: pulumi.Input[str],
+                 html_template: pulumi.Input[str],
+                 subject: pulumi.Input[str],
+                 redirect_url: Optional[pulumi.Input[str]] = None,
+                 success_redirect_url: Optional[pulumi.Input[str]] = None):
+        pulumi.set(__self__, "from_address", from_address)
+        pulumi.set(__self__, "from_name", from_name)
+        pulumi.set(__self__, "html_template", html_template)
+        pulumi.set(__self__, "subject", subject)
+        if redirect_url is not None:
+            pulumi.set(__self__, "redirect_url", redirect_url)
+        if success_redirect_url is not None:
+            pulumi.set(__self__, "success_redirect_url", success_redirect_url)
+
+    @property
+    @pulumi.getter(name="fromAddress")
+    def from_address(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "from_address")
+
+    @from_address.setter
+    def from_address(self, value: pulumi.Input[str]):
+        pulumi.set(self, "from_address", value)
+
+    @property
+    @pulumi.getter(name="fromName")
+    def from_name(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "from_name")
+
+    @from_name.setter
+    def from_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "from_name", value)
+
+    @property
+    @pulumi.getter(name="htmlTemplate")
+    def html_template(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "html_template")
+
+    @html_template.setter
+    def html_template(self, value: pulumi.Input[str]):
+        pulumi.set(self, "html_template", value)
+
+    @property
+    @pulumi.getter
+    def subject(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "subject")
+
+    @subject.setter
+    def subject(self, value: pulumi.Input[str]):
+        pulumi.set(self, "subject", value)
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "redirect_url")
+
+    @redirect_url.setter
+    def redirect_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "redirect_url", value)
+
+    @property
+    @pulumi.getter(name="successRedirectUrl")
+    def success_redirect_url(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "success_redirect_url")
+
+    @success_redirect_url.setter
+    def success_redirect_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "success_redirect_url", value)
+
+
+@pulumi.input_type
 class WorkspaceLockoutPolicyArgs:
     def __init__(__self__, *,
                  max_attempts: pulumi.Input[int]):
         pulumi.set(__self__, "max_attempts", max_attempts)
 
     @property
     @pulumi.getter(name="maxAttempts")
@@ -1253,14 +1557,160 @@
 
     @service_name.setter
     def service_name(self, value: pulumi.Input[str]):
         pulumi.set(self, "service_name", value)
 
 
 @pulumi.input_type
+class WorkspaceMfaEnrollEmailArgs:
+    def __init__(__self__, *,
+                 from_address: pulumi.Input[str],
+                 from_name: pulumi.Input[str],
+                 html_template: pulumi.Input[str],
+                 subject: pulumi.Input[str],
+                 redirect_url: Optional[pulumi.Input[str]] = None,
+                 success_redirect_url: Optional[pulumi.Input[str]] = None):
+        pulumi.set(__self__, "from_address", from_address)
+        pulumi.set(__self__, "from_name", from_name)
+        pulumi.set(__self__, "html_template", html_template)
+        pulumi.set(__self__, "subject", subject)
+        if redirect_url is not None:
+            pulumi.set(__self__, "redirect_url", redirect_url)
+        if success_redirect_url is not None:
+            pulumi.set(__self__, "success_redirect_url", success_redirect_url)
+
+    @property
+    @pulumi.getter(name="fromAddress")
+    def from_address(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "from_address")
+
+    @from_address.setter
+    def from_address(self, value: pulumi.Input[str]):
+        pulumi.set(self, "from_address", value)
+
+    @property
+    @pulumi.getter(name="fromName")
+    def from_name(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "from_name")
+
+    @from_name.setter
+    def from_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "from_name", value)
+
+    @property
+    @pulumi.getter(name="htmlTemplate")
+    def html_template(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "html_template")
+
+    @html_template.setter
+    def html_template(self, value: pulumi.Input[str]):
+        pulumi.set(self, "html_template", value)
+
+    @property
+    @pulumi.getter
+    def subject(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "subject")
+
+    @subject.setter
+    def subject(self, value: pulumi.Input[str]):
+        pulumi.set(self, "subject", value)
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "redirect_url")
+
+    @redirect_url.setter
+    def redirect_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "redirect_url", value)
+
+    @property
+    @pulumi.getter(name="successRedirectUrl")
+    def success_redirect_url(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "success_redirect_url")
+
+    @success_redirect_url.setter
+    def success_redirect_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "success_redirect_url", value)
+
+
+@pulumi.input_type
+class WorkspaceMfaOtcEmailArgs:
+    def __init__(__self__, *,
+                 from_address: pulumi.Input[str],
+                 from_name: pulumi.Input[str],
+                 html_template: pulumi.Input[str],
+                 subject: pulumi.Input[str],
+                 redirect_url: Optional[pulumi.Input[str]] = None,
+                 success_redirect_url: Optional[pulumi.Input[str]] = None):
+        pulumi.set(__self__, "from_address", from_address)
+        pulumi.set(__self__, "from_name", from_name)
+        pulumi.set(__self__, "html_template", html_template)
+        pulumi.set(__self__, "subject", subject)
+        if redirect_url is not None:
+            pulumi.set(__self__, "redirect_url", redirect_url)
+        if success_redirect_url is not None:
+            pulumi.set(__self__, "success_redirect_url", success_redirect_url)
+
+    @property
+    @pulumi.getter(name="fromAddress")
+    def from_address(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "from_address")
+
+    @from_address.setter
+    def from_address(self, value: pulumi.Input[str]):
+        pulumi.set(self, "from_address", value)
+
+    @property
+    @pulumi.getter(name="fromName")
+    def from_name(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "from_name")
+
+    @from_name.setter
+    def from_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "from_name", value)
+
+    @property
+    @pulumi.getter(name="htmlTemplate")
+    def html_template(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "html_template")
+
+    @html_template.setter
+    def html_template(self, value: pulumi.Input[str]):
+        pulumi.set(self, "html_template", value)
+
+    @property
+    @pulumi.getter
+    def subject(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "subject")
+
+    @subject.setter
+    def subject(self, value: pulumi.Input[str]):
+        pulumi.set(self, "subject", value)
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "redirect_url")
+
+    @redirect_url.setter
+    def redirect_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "redirect_url", value)
+
+    @property
+    @pulumi.getter(name="successRedirectUrl")
+    def success_redirect_url(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "success_redirect_url")
+
+    @success_redirect_url.setter
+    def success_redirect_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "success_redirect_url", value)
+
+
+@pulumi.input_type
 class WorkspaceMfaPolicyArgs:
     def __init__(__self__, *,
                  allow_remember_device: pulumi.Input[bool],
                  device_expiration: pulumi.Input[int],
                  enforce: pulumi.Input[str]):
         pulumi.set(__self__, "allow_remember_device", allow_remember_device)
         pulumi.set(__self__, "device_expiration", device_expiration)
@@ -1291,14 +1741,160 @@
 
     @enforce.setter
     def enforce(self, value: pulumi.Input[str]):
         pulumi.set(self, "enforce", value)
 
 
 @pulumi.input_type
+class WorkspaceMfaRecoveryCodeEmailArgs:
+    def __init__(__self__, *,
+                 from_address: pulumi.Input[str],
+                 from_name: pulumi.Input[str],
+                 html_template: pulumi.Input[str],
+                 subject: pulumi.Input[str],
+                 redirect_url: Optional[pulumi.Input[str]] = None,
+                 success_redirect_url: Optional[pulumi.Input[str]] = None):
+        pulumi.set(__self__, "from_address", from_address)
+        pulumi.set(__self__, "from_name", from_name)
+        pulumi.set(__self__, "html_template", html_template)
+        pulumi.set(__self__, "subject", subject)
+        if redirect_url is not None:
+            pulumi.set(__self__, "redirect_url", redirect_url)
+        if success_redirect_url is not None:
+            pulumi.set(__self__, "success_redirect_url", success_redirect_url)
+
+    @property
+    @pulumi.getter(name="fromAddress")
+    def from_address(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "from_address")
+
+    @from_address.setter
+    def from_address(self, value: pulumi.Input[str]):
+        pulumi.set(self, "from_address", value)
+
+    @property
+    @pulumi.getter(name="fromName")
+    def from_name(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "from_name")
+
+    @from_name.setter
+    def from_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "from_name", value)
+
+    @property
+    @pulumi.getter(name="htmlTemplate")
+    def html_template(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "html_template")
+
+    @html_template.setter
+    def html_template(self, value: pulumi.Input[str]):
+        pulumi.set(self, "html_template", value)
+
+    @property
+    @pulumi.getter
+    def subject(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "subject")
+
+    @subject.setter
+    def subject(self, value: pulumi.Input[str]):
+        pulumi.set(self, "subject", value)
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "redirect_url")
+
+    @redirect_url.setter
+    def redirect_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "redirect_url", value)
+
+    @property
+    @pulumi.getter(name="successRedirectUrl")
+    def success_redirect_url(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "success_redirect_url")
+
+    @success_redirect_url.setter
+    def success_redirect_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "success_redirect_url", value)
+
+
+@pulumi.input_type
+class WorkspaceMfaUnenrollEmailArgs:
+    def __init__(__self__, *,
+                 from_address: pulumi.Input[str],
+                 from_name: pulumi.Input[str],
+                 html_template: pulumi.Input[str],
+                 subject: pulumi.Input[str],
+                 redirect_url: Optional[pulumi.Input[str]] = None,
+                 success_redirect_url: Optional[pulumi.Input[str]] = None):
+        pulumi.set(__self__, "from_address", from_address)
+        pulumi.set(__self__, "from_name", from_name)
+        pulumi.set(__self__, "html_template", html_template)
+        pulumi.set(__self__, "subject", subject)
+        if redirect_url is not None:
+            pulumi.set(__self__, "redirect_url", redirect_url)
+        if success_redirect_url is not None:
+            pulumi.set(__self__, "success_redirect_url", success_redirect_url)
+
+    @property
+    @pulumi.getter(name="fromAddress")
+    def from_address(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "from_address")
+
+    @from_address.setter
+    def from_address(self, value: pulumi.Input[str]):
+        pulumi.set(self, "from_address", value)
+
+    @property
+    @pulumi.getter(name="fromName")
+    def from_name(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "from_name")
+
+    @from_name.setter
+    def from_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "from_name", value)
+
+    @property
+    @pulumi.getter(name="htmlTemplate")
+    def html_template(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "html_template")
+
+    @html_template.setter
+    def html_template(self, value: pulumi.Input[str]):
+        pulumi.set(self, "html_template", value)
+
+    @property
+    @pulumi.getter
+    def subject(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "subject")
+
+    @subject.setter
+    def subject(self, value: pulumi.Input[str]):
+        pulumi.set(self, "subject", value)
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "redirect_url")
+
+    @redirect_url.setter
+    def redirect_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "redirect_url", value)
+
+    @property
+    @pulumi.getter(name="successRedirectUrl")
+    def success_redirect_url(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "success_redirect_url")
+
+    @success_redirect_url.setter
+    def success_redirect_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "success_redirect_url", value)
+
+
+@pulumi.input_type
 class WorkspaceMicrosoftSocialLoginArgs:
     def __init__(__self__, *,
                  redirect_url: pulumi.Input[str],
                  client_id: Optional[pulumi.Input[str]] = None,
                  customised: Optional[pulumi.Input[bool]] = None,
                  secret: Optional[pulumi.Input[str]] = None):
         pulumi.set(__self__, "redirect_url", redirect_url)
@@ -1416,14 +2012,87 @@
 
     @success_redirect_url.setter
     def success_redirect_url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "success_redirect_url", value)
 
 
 @pulumi.input_type
+class WorkspaceNewMfaMethodEmailArgs:
+    def __init__(__self__, *,
+                 from_address: pulumi.Input[str],
+                 from_name: pulumi.Input[str],
+                 html_template: pulumi.Input[str],
+                 subject: pulumi.Input[str],
+                 redirect_url: Optional[pulumi.Input[str]] = None,
+                 success_redirect_url: Optional[pulumi.Input[str]] = None):
+        pulumi.set(__self__, "from_address", from_address)
+        pulumi.set(__self__, "from_name", from_name)
+        pulumi.set(__self__, "html_template", html_template)
+        pulumi.set(__self__, "subject", subject)
+        if redirect_url is not None:
+            pulumi.set(__self__, "redirect_url", redirect_url)
+        if success_redirect_url is not None:
+            pulumi.set(__self__, "success_redirect_url", success_redirect_url)
+
+    @property
+    @pulumi.getter(name="fromAddress")
+    def from_address(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "from_address")
+
+    @from_address.setter
+    def from_address(self, value: pulumi.Input[str]):
+        pulumi.set(self, "from_address", value)
+
+    @property
+    @pulumi.getter(name="fromName")
+    def from_name(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "from_name")
+
+    @from_name.setter
+    def from_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "from_name", value)
+
+    @property
+    @pulumi.getter(name="htmlTemplate")
+    def html_template(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "html_template")
+
+    @html_template.setter
+    def html_template(self, value: pulumi.Input[str]):
+        pulumi.set(self, "html_template", value)
+
+    @property
+    @pulumi.getter
+    def subject(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "subject")
+
+    @subject.setter
+    def subject(self, value: pulumi.Input[str]):
+        pulumi.set(self, "subject", value)
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "redirect_url")
+
+    @redirect_url.setter
+    def redirect_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "redirect_url", value)
+
+    @property
+    @pulumi.getter(name="successRedirectUrl")
+    def success_redirect_url(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "success_redirect_url")
+
+    @success_redirect_url.setter
+    def success_redirect_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "success_redirect_url", value)
+
+
+@pulumi.input_type
 class WorkspaceOidcArgs:
     def __init__(__self__, *,
                  redirect_url: pulumi.Input[str]):
         pulumi.set(__self__, "redirect_url", redirect_url)
 
     @property
     @pulumi.getter(name="redirectUrl")
@@ -1576,14 +2245,87 @@
 
     @success_redirect_url.setter
     def success_redirect_url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "success_redirect_url", value)
 
 
 @pulumi.input_type
+class WorkspaceRemoveMfaMethodEmailArgs:
+    def __init__(__self__, *,
+                 from_address: pulumi.Input[str],
+                 from_name: pulumi.Input[str],
+                 html_template: pulumi.Input[str],
+                 subject: pulumi.Input[str],
+                 redirect_url: Optional[pulumi.Input[str]] = None,
+                 success_redirect_url: Optional[pulumi.Input[str]] = None):
+        pulumi.set(__self__, "from_address", from_address)
+        pulumi.set(__self__, "from_name", from_name)
+        pulumi.set(__self__, "html_template", html_template)
+        pulumi.set(__self__, "subject", subject)
+        if redirect_url is not None:
+            pulumi.set(__self__, "redirect_url", redirect_url)
+        if success_redirect_url is not None:
+            pulumi.set(__self__, "success_redirect_url", success_redirect_url)
+
+    @property
+    @pulumi.getter(name="fromAddress")
+    def from_address(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "from_address")
+
+    @from_address.setter
+    def from_address(self, value: pulumi.Input[str]):
+        pulumi.set(self, "from_address", value)
+
+    @property
+    @pulumi.getter(name="fromName")
+    def from_name(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "from_name")
+
+    @from_name.setter
+    def from_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "from_name", value)
+
+    @property
+    @pulumi.getter(name="htmlTemplate")
+    def html_template(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "html_template")
+
+    @html_template.setter
+    def html_template(self, value: pulumi.Input[str]):
+        pulumi.set(self, "html_template", value)
+
+    @property
+    @pulumi.getter
+    def subject(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "subject")
+
+    @subject.setter
+    def subject(self, value: pulumi.Input[str]):
+        pulumi.set(self, "subject", value)
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "redirect_url")
+
+    @redirect_url.setter
+    def redirect_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "redirect_url", value)
+
+    @property
+    @pulumi.getter(name="successRedirectUrl")
+    def success_redirect_url(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "success_redirect_url")
+
+    @success_redirect_url.setter
+    def success_redirect_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "success_redirect_url", value)
+
+
+@pulumi.input_type
 class WorkspaceResetPasswordEmailArgs:
     def __init__(__self__, *,
                  from_address: pulumi.Input[str],
                  from_name: pulumi.Input[str],
                  html_template: pulumi.Input[str],
                  subject: pulumi.Input[str],
                  redirect_url: Optional[pulumi.Input[str]] = None,
@@ -1761,14 +2503,87 @@
 
     @redirect_url.setter
     def redirect_url(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "redirect_url", value)
 
 
 @pulumi.input_type
+class WorkspaceSmsAuthenticationEnabledEmailArgs:
+    def __init__(__self__, *,
+                 from_address: pulumi.Input[str],
+                 from_name: pulumi.Input[str],
+                 html_template: pulumi.Input[str],
+                 subject: pulumi.Input[str],
+                 redirect_url: Optional[pulumi.Input[str]] = None,
+                 success_redirect_url: Optional[pulumi.Input[str]] = None):
+        pulumi.set(__self__, "from_address", from_address)
+        pulumi.set(__self__, "from_name", from_name)
+        pulumi.set(__self__, "html_template", html_template)
+        pulumi.set(__self__, "subject", subject)
+        if redirect_url is not None:
+            pulumi.set(__self__, "redirect_url", redirect_url)
+        if success_redirect_url is not None:
+            pulumi.set(__self__, "success_redirect_url", success_redirect_url)
+
+    @property
+    @pulumi.getter(name="fromAddress")
+    def from_address(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "from_address")
+
+    @from_address.setter
+    def from_address(self, value: pulumi.Input[str]):
+        pulumi.set(self, "from_address", value)
+
+    @property
+    @pulumi.getter(name="fromName")
+    def from_name(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "from_name")
+
+    @from_name.setter
+    def from_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "from_name", value)
+
+    @property
+    @pulumi.getter(name="htmlTemplate")
+    def html_template(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "html_template")
+
+    @html_template.setter
+    def html_template(self, value: pulumi.Input[str]):
+        pulumi.set(self, "html_template", value)
+
+    @property
+    @pulumi.getter
+    def subject(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "subject")
+
+    @subject.setter
+    def subject(self, value: pulumi.Input[str]):
+        pulumi.set(self, "subject", value)
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "redirect_url")
+
+    @redirect_url.setter
+    def redirect_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "redirect_url", value)
+
+    @property
+    @pulumi.getter(name="successRedirectUrl")
+    def success_redirect_url(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "success_redirect_url")
+
+    @success_redirect_url.setter
+    def success_redirect_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "success_redirect_url", value)
+
+
+@pulumi.input_type
 class WorkspaceSsoDomainPolicyArgs:
     def __init__(__self__, *,
                  allow_verified_users_to_add_domains: Optional[pulumi.Input[bool]] = None,
                  bypass_domain_cross_validation: Optional[pulumi.Input[bool]] = None,
                  skip_domain_verification: Optional[pulumi.Input[bool]] = None):
         if allow_verified_users_to_add_domains is not None:
             pulumi.set(__self__, "allow_verified_users_to_add_domains", allow_verified_users_to_add_domains)
@@ -1831,14 +2646,87 @@
 
     @use_active_tenant.setter
     def use_active_tenant(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "use_active_tenant", value)
 
 
 @pulumi.input_type
+class WorkspaceSuspiciousIpEmailArgs:
+    def __init__(__self__, *,
+                 from_address: pulumi.Input[str],
+                 from_name: pulumi.Input[str],
+                 html_template: pulumi.Input[str],
+                 subject: pulumi.Input[str],
+                 redirect_url: Optional[pulumi.Input[str]] = None,
+                 success_redirect_url: Optional[pulumi.Input[str]] = None):
+        pulumi.set(__self__, "from_address", from_address)
+        pulumi.set(__self__, "from_name", from_name)
+        pulumi.set(__self__, "html_template", html_template)
+        pulumi.set(__self__, "subject", subject)
+        if redirect_url is not None:
+            pulumi.set(__self__, "redirect_url", redirect_url)
+        if success_redirect_url is not None:
+            pulumi.set(__self__, "success_redirect_url", success_redirect_url)
+
+    @property
+    @pulumi.getter(name="fromAddress")
+    def from_address(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "from_address")
+
+    @from_address.setter
+    def from_address(self, value: pulumi.Input[str]):
+        pulumi.set(self, "from_address", value)
+
+    @property
+    @pulumi.getter(name="fromName")
+    def from_name(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "from_name")
+
+    @from_name.setter
+    def from_name(self, value: pulumi.Input[str]):
+        pulumi.set(self, "from_name", value)
+
+    @property
+    @pulumi.getter(name="htmlTemplate")
+    def html_template(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "html_template")
+
+    @html_template.setter
+    def html_template(self, value: pulumi.Input[str]):
+        pulumi.set(self, "html_template", value)
+
+    @property
+    @pulumi.getter
+    def subject(self) -> pulumi.Input[str]:
+        return pulumi.get(self, "subject")
+
+    @subject.setter
+    def subject(self, value: pulumi.Input[str]):
+        pulumi.set(self, "subject", value)
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "redirect_url")
+
+    @redirect_url.setter
+    def redirect_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "redirect_url", value)
+
+    @property
+    @pulumi.getter(name="successRedirectUrl")
+    def success_redirect_url(self) -> Optional[pulumi.Input[str]]:
+        return pulumi.get(self, "success_redirect_url")
+
+    @success_redirect_url.setter
+    def success_redirect_url(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "success_redirect_url", value)
+
+
+@pulumi.input_type
 class WorkspaceUserActivationEmailArgs:
     def __init__(__self__, *,
                  from_address: pulumi.Input[str],
                  from_name: pulumi.Input[str],
                  html_template: pulumi.Input[str],
                  subject: pulumi.Input[str],
                  redirect_url: Optional[pulumi.Input[str]] = None,
```

### Comparing `pulumi_frontegg-0.2.34/pulumi_frontegg/_utilities.py` & `pulumi_frontegg-0.2.35/pulumi_frontegg/_utilities.py`

 * *Files 0% similar despite different names*

```diff
@@ -284,8 +284,8 @@
         await o._future,
         await o._is_known,
         await o._is_secret,
         await o._resources,
     )
 
 def get_plugin_download_url():
-	return "https://github.com/MaterializeInc/pulumi-frontegg/releases/download/v0.2.34/"
+	return "https://github.com/MaterializeInc/pulumi-frontegg/releases/download/v0.2.35/"
```

### Comparing `pulumi_frontegg-0.2.34/pulumi_frontegg/allowed_origin.py` & `pulumi_frontegg-0.2.35/pulumi_frontegg/allowed_origin.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.34/pulumi_frontegg/config/vars.py` & `pulumi_frontegg-0.2.35/pulumi_frontegg/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.34/pulumi_frontegg/get_permission.py` & `pulumi_frontegg-0.2.35/pulumi_frontegg/get_permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.34/pulumi_frontegg/outputs.py` & `pulumi_frontegg-0.2.35/pulumi_frontegg/outputs.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,35 +16,47 @@
     'WorkspaceAdminPortalPaletteError',
     'WorkspaceAdminPortalPaletteInfo',
     'WorkspaceAdminPortalPalettePrimary',
     'WorkspaceAdminPortalPaletteSecondary',
     'WorkspaceAdminPortalPaletteSuccess',
     'WorkspaceAdminPortalPaletteWarning',
     'WorkspaceAuthPolicy',
+    'WorkspaceBotDetectionEmail',
+    'WorkspaceBruteForceProtectionEmail',
     'WorkspaceBulkTenantsInvitesEmail',
     'WorkspaceCaptchaPolicy',
+    'WorkspaceEmailVerificationEmail',
     'WorkspaceFacebookSocialLogin',
     'WorkspaceGithubSocialLogin',
     'WorkspaceGoogleSocialLogin',
     'WorkspaceHostedLogin',
+    'WorkspaceImpossibleTravelEmail',
     'WorkspaceLockoutPolicy',
     'WorkspaceMagicCodeEmail',
     'WorkspaceMagicLinkEmail',
     'WorkspaceMfaAuthenticationApp',
+    'WorkspaceMfaEnrollEmail',
+    'WorkspaceMfaOtcEmail',
     'WorkspaceMfaPolicy',
+    'WorkspaceMfaRecoveryCodeEmail',
+    'WorkspaceMfaUnenrollEmail',
     'WorkspaceMicrosoftSocialLogin',
     'WorkspaceNewDeviceConnectedEmail',
+    'WorkspaceNewMfaMethodEmail',
     'WorkspaceOidc',
     'WorkspacePasswordPolicy',
     'WorkspacePwnedPasswordEmail',
+    'WorkspaceRemoveMfaMethodEmail',
     'WorkspaceResetPasswordEmail',
     'WorkspaceResetPhoneNumberEmail',
     'WorkspaceSaml',
+    'WorkspaceSmsAuthenticationEnabledEmail',
     'WorkspaceSsoDomainPolicy',
     'WorkspaceSsoMultiTenantPolicy',
+    'WorkspaceSuspiciousIpEmail',
     'WorkspaceUserActivationEmail',
     'WorkspaceUserInvitationEmail',
     'WorkspaceUserUsedInvitationEmail',
 ]
 
 @pulumi.output_type
 class WorkspaceAdminPortal(dict):
@@ -718,14 +730,162 @@
     @property
     @pulumi.getter(name="machineToMachineAuthStrategy")
     def machine_to_machine_auth_strategy(self) -> Optional[str]:
         return pulumi.get(self, "machine_to_machine_auth_strategy")
 
 
 @pulumi.output_type
+class WorkspaceBotDetectionEmail(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "fromAddress":
+            suggest = "from_address"
+        elif key == "fromName":
+            suggest = "from_name"
+        elif key == "htmlTemplate":
+            suggest = "html_template"
+        elif key == "redirectUrl":
+            suggest = "redirect_url"
+        elif key == "successRedirectUrl":
+            suggest = "success_redirect_url"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in WorkspaceBotDetectionEmail. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        WorkspaceBotDetectionEmail.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        WorkspaceBotDetectionEmail.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 from_address: str,
+                 from_name: str,
+                 html_template: str,
+                 subject: str,
+                 redirect_url: Optional[str] = None,
+                 success_redirect_url: Optional[str] = None):
+        pulumi.set(__self__, "from_address", from_address)
+        pulumi.set(__self__, "from_name", from_name)
+        pulumi.set(__self__, "html_template", html_template)
+        pulumi.set(__self__, "subject", subject)
+        if redirect_url is not None:
+            pulumi.set(__self__, "redirect_url", redirect_url)
+        if success_redirect_url is not None:
+            pulumi.set(__self__, "success_redirect_url", success_redirect_url)
+
+    @property
+    @pulumi.getter(name="fromAddress")
+    def from_address(self) -> str:
+        return pulumi.get(self, "from_address")
+
+    @property
+    @pulumi.getter(name="fromName")
+    def from_name(self) -> str:
+        return pulumi.get(self, "from_name")
+
+    @property
+    @pulumi.getter(name="htmlTemplate")
+    def html_template(self) -> str:
+        return pulumi.get(self, "html_template")
+
+    @property
+    @pulumi.getter
+    def subject(self) -> str:
+        return pulumi.get(self, "subject")
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> Optional[str]:
+        return pulumi.get(self, "redirect_url")
+
+    @property
+    @pulumi.getter(name="successRedirectUrl")
+    def success_redirect_url(self) -> Optional[str]:
+        return pulumi.get(self, "success_redirect_url")
+
+
+@pulumi.output_type
+class WorkspaceBruteForceProtectionEmail(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "fromAddress":
+            suggest = "from_address"
+        elif key == "fromName":
+            suggest = "from_name"
+        elif key == "htmlTemplate":
+            suggest = "html_template"
+        elif key == "redirectUrl":
+            suggest = "redirect_url"
+        elif key == "successRedirectUrl":
+            suggest = "success_redirect_url"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in WorkspaceBruteForceProtectionEmail. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        WorkspaceBruteForceProtectionEmail.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        WorkspaceBruteForceProtectionEmail.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 from_address: str,
+                 from_name: str,
+                 html_template: str,
+                 subject: str,
+                 redirect_url: Optional[str] = None,
+                 success_redirect_url: Optional[str] = None):
+        pulumi.set(__self__, "from_address", from_address)
+        pulumi.set(__self__, "from_name", from_name)
+        pulumi.set(__self__, "html_template", html_template)
+        pulumi.set(__self__, "subject", subject)
+        if redirect_url is not None:
+            pulumi.set(__self__, "redirect_url", redirect_url)
+        if success_redirect_url is not None:
+            pulumi.set(__self__, "success_redirect_url", success_redirect_url)
+
+    @property
+    @pulumi.getter(name="fromAddress")
+    def from_address(self) -> str:
+        return pulumi.get(self, "from_address")
+
+    @property
+    @pulumi.getter(name="fromName")
+    def from_name(self) -> str:
+        return pulumi.get(self, "from_name")
+
+    @property
+    @pulumi.getter(name="htmlTemplate")
+    def html_template(self) -> str:
+        return pulumi.get(self, "html_template")
+
+    @property
+    @pulumi.getter
+    def subject(self) -> str:
+        return pulumi.get(self, "subject")
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> Optional[str]:
+        return pulumi.get(self, "redirect_url")
+
+    @property
+    @pulumi.getter(name="successRedirectUrl")
+    def success_redirect_url(self) -> Optional[str]:
+        return pulumi.get(self, "success_redirect_url")
+
+
+@pulumi.output_type
 class WorkspaceBulkTenantsInvitesEmail(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "fromAddress":
             suggest = "from_address"
         elif key == "fromName":
@@ -849,14 +1009,88 @@
     @property
     @pulumi.getter(name="ignoredEmails")
     def ignored_emails(self) -> Optional[Sequence[str]]:
         return pulumi.get(self, "ignored_emails")
 
 
 @pulumi.output_type
+class WorkspaceEmailVerificationEmail(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "fromAddress":
+            suggest = "from_address"
+        elif key == "fromName":
+            suggest = "from_name"
+        elif key == "htmlTemplate":
+            suggest = "html_template"
+        elif key == "redirectUrl":
+            suggest = "redirect_url"
+        elif key == "successRedirectUrl":
+            suggest = "success_redirect_url"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in WorkspaceEmailVerificationEmail. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        WorkspaceEmailVerificationEmail.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        WorkspaceEmailVerificationEmail.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 from_address: str,
+                 from_name: str,
+                 html_template: str,
+                 subject: str,
+                 redirect_url: Optional[str] = None,
+                 success_redirect_url: Optional[str] = None):
+        pulumi.set(__self__, "from_address", from_address)
+        pulumi.set(__self__, "from_name", from_name)
+        pulumi.set(__self__, "html_template", html_template)
+        pulumi.set(__self__, "subject", subject)
+        if redirect_url is not None:
+            pulumi.set(__self__, "redirect_url", redirect_url)
+        if success_redirect_url is not None:
+            pulumi.set(__self__, "success_redirect_url", success_redirect_url)
+
+    @property
+    @pulumi.getter(name="fromAddress")
+    def from_address(self) -> str:
+        return pulumi.get(self, "from_address")
+
+    @property
+    @pulumi.getter(name="fromName")
+    def from_name(self) -> str:
+        return pulumi.get(self, "from_name")
+
+    @property
+    @pulumi.getter(name="htmlTemplate")
+    def html_template(self) -> str:
+        return pulumi.get(self, "html_template")
+
+    @property
+    @pulumi.getter
+    def subject(self) -> str:
+        return pulumi.get(self, "subject")
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> Optional[str]:
+        return pulumi.get(self, "redirect_url")
+
+    @property
+    @pulumi.getter(name="successRedirectUrl")
+    def success_redirect_url(self) -> Optional[str]:
+        return pulumi.get(self, "success_redirect_url")
+
+
+@pulumi.output_type
 class WorkspaceFacebookSocialLogin(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "redirectUrl":
             suggest = "redirect_url"
         elif key == "clientId":
@@ -1044,14 +1278,88 @@
     @property
     @pulumi.getter(name="allowedRedirectUrls")
     def allowed_redirect_urls(self) -> Optional[Sequence[str]]:
         return pulumi.get(self, "allowed_redirect_urls")
 
 
 @pulumi.output_type
+class WorkspaceImpossibleTravelEmail(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "fromAddress":
+            suggest = "from_address"
+        elif key == "fromName":
+            suggest = "from_name"
+        elif key == "htmlTemplate":
+            suggest = "html_template"
+        elif key == "redirectUrl":
+            suggest = "redirect_url"
+        elif key == "successRedirectUrl":
+            suggest = "success_redirect_url"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in WorkspaceImpossibleTravelEmail. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        WorkspaceImpossibleTravelEmail.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        WorkspaceImpossibleTravelEmail.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 from_address: str,
+                 from_name: str,
+                 html_template: str,
+                 subject: str,
+                 redirect_url: Optional[str] = None,
+                 success_redirect_url: Optional[str] = None):
+        pulumi.set(__self__, "from_address", from_address)
+        pulumi.set(__self__, "from_name", from_name)
+        pulumi.set(__self__, "html_template", html_template)
+        pulumi.set(__self__, "subject", subject)
+        if redirect_url is not None:
+            pulumi.set(__self__, "redirect_url", redirect_url)
+        if success_redirect_url is not None:
+            pulumi.set(__self__, "success_redirect_url", success_redirect_url)
+
+    @property
+    @pulumi.getter(name="fromAddress")
+    def from_address(self) -> str:
+        return pulumi.get(self, "from_address")
+
+    @property
+    @pulumi.getter(name="fromName")
+    def from_name(self) -> str:
+        return pulumi.get(self, "from_name")
+
+    @property
+    @pulumi.getter(name="htmlTemplate")
+    def html_template(self) -> str:
+        return pulumi.get(self, "html_template")
+
+    @property
+    @pulumi.getter
+    def subject(self) -> str:
+        return pulumi.get(self, "subject")
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> Optional[str]:
+        return pulumi.get(self, "redirect_url")
+
+    @property
+    @pulumi.getter(name="successRedirectUrl")
+    def success_redirect_url(self) -> Optional[str]:
+        return pulumi.get(self, "success_redirect_url")
+
+
+@pulumi.output_type
 class WorkspaceLockoutPolicy(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "maxAttempts":
             suggest = "max_attempts"
 
@@ -1250,14 +1558,162 @@
     @property
     @pulumi.getter(name="serviceName")
     def service_name(self) -> str:
         return pulumi.get(self, "service_name")
 
 
 @pulumi.output_type
+class WorkspaceMfaEnrollEmail(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "fromAddress":
+            suggest = "from_address"
+        elif key == "fromName":
+            suggest = "from_name"
+        elif key == "htmlTemplate":
+            suggest = "html_template"
+        elif key == "redirectUrl":
+            suggest = "redirect_url"
+        elif key == "successRedirectUrl":
+            suggest = "success_redirect_url"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in WorkspaceMfaEnrollEmail. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        WorkspaceMfaEnrollEmail.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        WorkspaceMfaEnrollEmail.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 from_address: str,
+                 from_name: str,
+                 html_template: str,
+                 subject: str,
+                 redirect_url: Optional[str] = None,
+                 success_redirect_url: Optional[str] = None):
+        pulumi.set(__self__, "from_address", from_address)
+        pulumi.set(__self__, "from_name", from_name)
+        pulumi.set(__self__, "html_template", html_template)
+        pulumi.set(__self__, "subject", subject)
+        if redirect_url is not None:
+            pulumi.set(__self__, "redirect_url", redirect_url)
+        if success_redirect_url is not None:
+            pulumi.set(__self__, "success_redirect_url", success_redirect_url)
+
+    @property
+    @pulumi.getter(name="fromAddress")
+    def from_address(self) -> str:
+        return pulumi.get(self, "from_address")
+
+    @property
+    @pulumi.getter(name="fromName")
+    def from_name(self) -> str:
+        return pulumi.get(self, "from_name")
+
+    @property
+    @pulumi.getter(name="htmlTemplate")
+    def html_template(self) -> str:
+        return pulumi.get(self, "html_template")
+
+    @property
+    @pulumi.getter
+    def subject(self) -> str:
+        return pulumi.get(self, "subject")
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> Optional[str]:
+        return pulumi.get(self, "redirect_url")
+
+    @property
+    @pulumi.getter(name="successRedirectUrl")
+    def success_redirect_url(self) -> Optional[str]:
+        return pulumi.get(self, "success_redirect_url")
+
+
+@pulumi.output_type
+class WorkspaceMfaOtcEmail(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "fromAddress":
+            suggest = "from_address"
+        elif key == "fromName":
+            suggest = "from_name"
+        elif key == "htmlTemplate":
+            suggest = "html_template"
+        elif key == "redirectUrl":
+            suggest = "redirect_url"
+        elif key == "successRedirectUrl":
+            suggest = "success_redirect_url"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in WorkspaceMfaOtcEmail. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        WorkspaceMfaOtcEmail.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        WorkspaceMfaOtcEmail.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 from_address: str,
+                 from_name: str,
+                 html_template: str,
+                 subject: str,
+                 redirect_url: Optional[str] = None,
+                 success_redirect_url: Optional[str] = None):
+        pulumi.set(__self__, "from_address", from_address)
+        pulumi.set(__self__, "from_name", from_name)
+        pulumi.set(__self__, "html_template", html_template)
+        pulumi.set(__self__, "subject", subject)
+        if redirect_url is not None:
+            pulumi.set(__self__, "redirect_url", redirect_url)
+        if success_redirect_url is not None:
+            pulumi.set(__self__, "success_redirect_url", success_redirect_url)
+
+    @property
+    @pulumi.getter(name="fromAddress")
+    def from_address(self) -> str:
+        return pulumi.get(self, "from_address")
+
+    @property
+    @pulumi.getter(name="fromName")
+    def from_name(self) -> str:
+        return pulumi.get(self, "from_name")
+
+    @property
+    @pulumi.getter(name="htmlTemplate")
+    def html_template(self) -> str:
+        return pulumi.get(self, "html_template")
+
+    @property
+    @pulumi.getter
+    def subject(self) -> str:
+        return pulumi.get(self, "subject")
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> Optional[str]:
+        return pulumi.get(self, "redirect_url")
+
+    @property
+    @pulumi.getter(name="successRedirectUrl")
+    def success_redirect_url(self) -> Optional[str]:
+        return pulumi.get(self, "success_redirect_url")
+
+
+@pulumi.output_type
 class WorkspaceMfaPolicy(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "allowRememberDevice":
             suggest = "allow_remember_device"
         elif key == "deviceExpiration":
@@ -1295,14 +1751,162 @@
     @property
     @pulumi.getter
     def enforce(self) -> str:
         return pulumi.get(self, "enforce")
 
 
 @pulumi.output_type
+class WorkspaceMfaRecoveryCodeEmail(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "fromAddress":
+            suggest = "from_address"
+        elif key == "fromName":
+            suggest = "from_name"
+        elif key == "htmlTemplate":
+            suggest = "html_template"
+        elif key == "redirectUrl":
+            suggest = "redirect_url"
+        elif key == "successRedirectUrl":
+            suggest = "success_redirect_url"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in WorkspaceMfaRecoveryCodeEmail. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        WorkspaceMfaRecoveryCodeEmail.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        WorkspaceMfaRecoveryCodeEmail.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 from_address: str,
+                 from_name: str,
+                 html_template: str,
+                 subject: str,
+                 redirect_url: Optional[str] = None,
+                 success_redirect_url: Optional[str] = None):
+        pulumi.set(__self__, "from_address", from_address)
+        pulumi.set(__self__, "from_name", from_name)
+        pulumi.set(__self__, "html_template", html_template)
+        pulumi.set(__self__, "subject", subject)
+        if redirect_url is not None:
+            pulumi.set(__self__, "redirect_url", redirect_url)
+        if success_redirect_url is not None:
+            pulumi.set(__self__, "success_redirect_url", success_redirect_url)
+
+    @property
+    @pulumi.getter(name="fromAddress")
+    def from_address(self) -> str:
+        return pulumi.get(self, "from_address")
+
+    @property
+    @pulumi.getter(name="fromName")
+    def from_name(self) -> str:
+        return pulumi.get(self, "from_name")
+
+    @property
+    @pulumi.getter(name="htmlTemplate")
+    def html_template(self) -> str:
+        return pulumi.get(self, "html_template")
+
+    @property
+    @pulumi.getter
+    def subject(self) -> str:
+        return pulumi.get(self, "subject")
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> Optional[str]:
+        return pulumi.get(self, "redirect_url")
+
+    @property
+    @pulumi.getter(name="successRedirectUrl")
+    def success_redirect_url(self) -> Optional[str]:
+        return pulumi.get(self, "success_redirect_url")
+
+
+@pulumi.output_type
+class WorkspaceMfaUnenrollEmail(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "fromAddress":
+            suggest = "from_address"
+        elif key == "fromName":
+            suggest = "from_name"
+        elif key == "htmlTemplate":
+            suggest = "html_template"
+        elif key == "redirectUrl":
+            suggest = "redirect_url"
+        elif key == "successRedirectUrl":
+            suggest = "success_redirect_url"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in WorkspaceMfaUnenrollEmail. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        WorkspaceMfaUnenrollEmail.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        WorkspaceMfaUnenrollEmail.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 from_address: str,
+                 from_name: str,
+                 html_template: str,
+                 subject: str,
+                 redirect_url: Optional[str] = None,
+                 success_redirect_url: Optional[str] = None):
+        pulumi.set(__self__, "from_address", from_address)
+        pulumi.set(__self__, "from_name", from_name)
+        pulumi.set(__self__, "html_template", html_template)
+        pulumi.set(__self__, "subject", subject)
+        if redirect_url is not None:
+            pulumi.set(__self__, "redirect_url", redirect_url)
+        if success_redirect_url is not None:
+            pulumi.set(__self__, "success_redirect_url", success_redirect_url)
+
+    @property
+    @pulumi.getter(name="fromAddress")
+    def from_address(self) -> str:
+        return pulumi.get(self, "from_address")
+
+    @property
+    @pulumi.getter(name="fromName")
+    def from_name(self) -> str:
+        return pulumi.get(self, "from_name")
+
+    @property
+    @pulumi.getter(name="htmlTemplate")
+    def html_template(self) -> str:
+        return pulumi.get(self, "html_template")
+
+    @property
+    @pulumi.getter
+    def subject(self) -> str:
+        return pulumi.get(self, "subject")
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> Optional[str]:
+        return pulumi.get(self, "redirect_url")
+
+    @property
+    @pulumi.getter(name="successRedirectUrl")
+    def success_redirect_url(self) -> Optional[str]:
+        return pulumi.get(self, "success_redirect_url")
+
+
+@pulumi.output_type
 class WorkspaceMicrosoftSocialLogin(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "redirectUrl":
             suggest = "redirect_url"
         elif key == "clientId":
@@ -1424,14 +2028,88 @@
     @property
     @pulumi.getter(name="successRedirectUrl")
     def success_redirect_url(self) -> Optional[str]:
         return pulumi.get(self, "success_redirect_url")
 
 
 @pulumi.output_type
+class WorkspaceNewMfaMethodEmail(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "fromAddress":
+            suggest = "from_address"
+        elif key == "fromName":
+            suggest = "from_name"
+        elif key == "htmlTemplate":
+            suggest = "html_template"
+        elif key == "redirectUrl":
+            suggest = "redirect_url"
+        elif key == "successRedirectUrl":
+            suggest = "success_redirect_url"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in WorkspaceNewMfaMethodEmail. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        WorkspaceNewMfaMethodEmail.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        WorkspaceNewMfaMethodEmail.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 from_address: str,
+                 from_name: str,
+                 html_template: str,
+                 subject: str,
+                 redirect_url: Optional[str] = None,
+                 success_redirect_url: Optional[str] = None):
+        pulumi.set(__self__, "from_address", from_address)
+        pulumi.set(__self__, "from_name", from_name)
+        pulumi.set(__self__, "html_template", html_template)
+        pulumi.set(__self__, "subject", subject)
+        if redirect_url is not None:
+            pulumi.set(__self__, "redirect_url", redirect_url)
+        if success_redirect_url is not None:
+            pulumi.set(__self__, "success_redirect_url", success_redirect_url)
+
+    @property
+    @pulumi.getter(name="fromAddress")
+    def from_address(self) -> str:
+        return pulumi.get(self, "from_address")
+
+    @property
+    @pulumi.getter(name="fromName")
+    def from_name(self) -> str:
+        return pulumi.get(self, "from_name")
+
+    @property
+    @pulumi.getter(name="htmlTemplate")
+    def html_template(self) -> str:
+        return pulumi.get(self, "html_template")
+
+    @property
+    @pulumi.getter
+    def subject(self) -> str:
+        return pulumi.get(self, "subject")
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> Optional[str]:
+        return pulumi.get(self, "redirect_url")
+
+    @property
+    @pulumi.getter(name="successRedirectUrl")
+    def success_redirect_url(self) -> Optional[str]:
+        return pulumi.get(self, "success_redirect_url")
+
+
+@pulumi.output_type
 class WorkspaceOidc(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "redirectUrl":
             suggest = "redirect_url"
 
@@ -1599,14 +2277,88 @@
     @property
     @pulumi.getter(name="successRedirectUrl")
     def success_redirect_url(self) -> Optional[str]:
         return pulumi.get(self, "success_redirect_url")
 
 
 @pulumi.output_type
+class WorkspaceRemoveMfaMethodEmail(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "fromAddress":
+            suggest = "from_address"
+        elif key == "fromName":
+            suggest = "from_name"
+        elif key == "htmlTemplate":
+            suggest = "html_template"
+        elif key == "redirectUrl":
+            suggest = "redirect_url"
+        elif key == "successRedirectUrl":
+            suggest = "success_redirect_url"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in WorkspaceRemoveMfaMethodEmail. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        WorkspaceRemoveMfaMethodEmail.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        WorkspaceRemoveMfaMethodEmail.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 from_address: str,
+                 from_name: str,
+                 html_template: str,
+                 subject: str,
+                 redirect_url: Optional[str] = None,
+                 success_redirect_url: Optional[str] = None):
+        pulumi.set(__self__, "from_address", from_address)
+        pulumi.set(__self__, "from_name", from_name)
+        pulumi.set(__self__, "html_template", html_template)
+        pulumi.set(__self__, "subject", subject)
+        if redirect_url is not None:
+            pulumi.set(__self__, "redirect_url", redirect_url)
+        if success_redirect_url is not None:
+            pulumi.set(__self__, "success_redirect_url", success_redirect_url)
+
+    @property
+    @pulumi.getter(name="fromAddress")
+    def from_address(self) -> str:
+        return pulumi.get(self, "from_address")
+
+    @property
+    @pulumi.getter(name="fromName")
+    def from_name(self) -> str:
+        return pulumi.get(self, "from_name")
+
+    @property
+    @pulumi.getter(name="htmlTemplate")
+    def html_template(self) -> str:
+        return pulumi.get(self, "html_template")
+
+    @property
+    @pulumi.getter
+    def subject(self) -> str:
+        return pulumi.get(self, "subject")
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> Optional[str]:
+        return pulumi.get(self, "redirect_url")
+
+    @property
+    @pulumi.getter(name="successRedirectUrl")
+    def success_redirect_url(self) -> Optional[str]:
+        return pulumi.get(self, "success_redirect_url")
+
+
+@pulumi.output_type
 class WorkspaceResetPasswordEmail(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "fromAddress":
             suggest = "from_address"
         elif key == "fromName":
@@ -1795,14 +2547,88 @@
     @property
     @pulumi.getter(name="redirectUrl")
     def redirect_url(self) -> Optional[str]:
         return pulumi.get(self, "redirect_url")
 
 
 @pulumi.output_type
+class WorkspaceSmsAuthenticationEnabledEmail(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "fromAddress":
+            suggest = "from_address"
+        elif key == "fromName":
+            suggest = "from_name"
+        elif key == "htmlTemplate":
+            suggest = "html_template"
+        elif key == "redirectUrl":
+            suggest = "redirect_url"
+        elif key == "successRedirectUrl":
+            suggest = "success_redirect_url"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in WorkspaceSmsAuthenticationEnabledEmail. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        WorkspaceSmsAuthenticationEnabledEmail.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        WorkspaceSmsAuthenticationEnabledEmail.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 from_address: str,
+                 from_name: str,
+                 html_template: str,
+                 subject: str,
+                 redirect_url: Optional[str] = None,
+                 success_redirect_url: Optional[str] = None):
+        pulumi.set(__self__, "from_address", from_address)
+        pulumi.set(__self__, "from_name", from_name)
+        pulumi.set(__self__, "html_template", html_template)
+        pulumi.set(__self__, "subject", subject)
+        if redirect_url is not None:
+            pulumi.set(__self__, "redirect_url", redirect_url)
+        if success_redirect_url is not None:
+            pulumi.set(__self__, "success_redirect_url", success_redirect_url)
+
+    @property
+    @pulumi.getter(name="fromAddress")
+    def from_address(self) -> str:
+        return pulumi.get(self, "from_address")
+
+    @property
+    @pulumi.getter(name="fromName")
+    def from_name(self) -> str:
+        return pulumi.get(self, "from_name")
+
+    @property
+    @pulumi.getter(name="htmlTemplate")
+    def html_template(self) -> str:
+        return pulumi.get(self, "html_template")
+
+    @property
+    @pulumi.getter
+    def subject(self) -> str:
+        return pulumi.get(self, "subject")
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> Optional[str]:
+        return pulumi.get(self, "redirect_url")
+
+    @property
+    @pulumi.getter(name="successRedirectUrl")
+    def success_redirect_url(self) -> Optional[str]:
+        return pulumi.get(self, "success_redirect_url")
+
+
+@pulumi.output_type
 class WorkspaceSsoDomainPolicy(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "allowVerifiedUsersToAddDomains":
             suggest = "allow_verified_users_to_add_domains"
         elif key == "bypassDomainCrossValidation":
@@ -1885,14 +2711,88 @@
     @property
     @pulumi.getter(name="useActiveTenant")
     def use_active_tenant(self) -> Optional[bool]:
         return pulumi.get(self, "use_active_tenant")
 
 
 @pulumi.output_type
+class WorkspaceSuspiciousIpEmail(dict):
+    @staticmethod
+    def __key_warning(key: str):
+        suggest = None
+        if key == "fromAddress":
+            suggest = "from_address"
+        elif key == "fromName":
+            suggest = "from_name"
+        elif key == "htmlTemplate":
+            suggest = "html_template"
+        elif key == "redirectUrl":
+            suggest = "redirect_url"
+        elif key == "successRedirectUrl":
+            suggest = "success_redirect_url"
+
+        if suggest:
+            pulumi.log.warn(f"Key '{key}' not found in WorkspaceSuspiciousIpEmail. Access the value via the '{suggest}' property getter instead.")
+
+    def __getitem__(self, key: str) -> Any:
+        WorkspaceSuspiciousIpEmail.__key_warning(key)
+        return super().__getitem__(key)
+
+    def get(self, key: str, default = None) -> Any:
+        WorkspaceSuspiciousIpEmail.__key_warning(key)
+        return super().get(key, default)
+
+    def __init__(__self__, *,
+                 from_address: str,
+                 from_name: str,
+                 html_template: str,
+                 subject: str,
+                 redirect_url: Optional[str] = None,
+                 success_redirect_url: Optional[str] = None):
+        pulumi.set(__self__, "from_address", from_address)
+        pulumi.set(__self__, "from_name", from_name)
+        pulumi.set(__self__, "html_template", html_template)
+        pulumi.set(__self__, "subject", subject)
+        if redirect_url is not None:
+            pulumi.set(__self__, "redirect_url", redirect_url)
+        if success_redirect_url is not None:
+            pulumi.set(__self__, "success_redirect_url", success_redirect_url)
+
+    @property
+    @pulumi.getter(name="fromAddress")
+    def from_address(self) -> str:
+        return pulumi.get(self, "from_address")
+
+    @property
+    @pulumi.getter(name="fromName")
+    def from_name(self) -> str:
+        return pulumi.get(self, "from_name")
+
+    @property
+    @pulumi.getter(name="htmlTemplate")
+    def html_template(self) -> str:
+        return pulumi.get(self, "html_template")
+
+    @property
+    @pulumi.getter
+    def subject(self) -> str:
+        return pulumi.get(self, "subject")
+
+    @property
+    @pulumi.getter(name="redirectUrl")
+    def redirect_url(self) -> Optional[str]:
+        return pulumi.get(self, "redirect_url")
+
+    @property
+    @pulumi.getter(name="successRedirectUrl")
+    def success_redirect_url(self) -> Optional[str]:
+        return pulumi.get(self, "success_redirect_url")
+
+
+@pulumi.output_type
 class WorkspaceUserActivationEmail(dict):
     @staticmethod
     def __key_warning(key: str):
         suggest = None
         if key == "fromAddress":
             suggest = "from_address"
         elif key == "fromName":
```

### Comparing `pulumi_frontegg-0.2.34/pulumi_frontegg/permission.py` & `pulumi_frontegg-0.2.35/pulumi_frontegg/permission.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.34/pulumi_frontegg/permission_category.py` & `pulumi_frontegg-0.2.35/pulumi_frontegg/permission_category.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.34/pulumi_frontegg/prehook.py` & `pulumi_frontegg-0.2.35/pulumi_frontegg/prehook.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.34/pulumi_frontegg/provider.py` & `pulumi_frontegg-0.2.35/pulumi_frontegg/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.34/pulumi_frontegg/redirect_uri.py` & `pulumi_frontegg-0.2.35/pulumi_frontegg/redirect_uri.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.34/pulumi_frontegg/role.py` & `pulumi_frontegg-0.2.35/pulumi_frontegg/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.34/pulumi_frontegg/tenant.py` & `pulumi_frontegg-0.2.35/pulumi_frontegg/tenant.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.34/pulumi_frontegg/user.py` & `pulumi_frontegg-0.2.35/pulumi_frontegg/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.34/pulumi_frontegg/webhook.py` & `pulumi_frontegg-0.2.35/pulumi_frontegg/webhook.py`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.34/pulumi_frontegg/workspace.py` & `pulumi_frontegg-0.2.35/pulumi_frontegg/workspace.py`

 * *Files 17% similar despite different names*

```diff
@@ -22,35 +22,47 @@
                  backend_stack: pulumi.Input[str],
                  country: pulumi.Input[str],
                  frontegg_domain: pulumi.Input[str],
                  frontend_stack: pulumi.Input[str],
                  mfa_policy: pulumi.Input['WorkspaceMfaPolicyArgs'],
                  open_saas_installed: pulumi.Input[bool],
                  password_policy: pulumi.Input['WorkspacePasswordPolicyArgs'],
+                 bot_detection_email: Optional[pulumi.Input['WorkspaceBotDetectionEmailArgs']] = None,
+                 brute_force_protection_email: Optional[pulumi.Input['WorkspaceBruteForceProtectionEmailArgs']] = None,
                  bulk_tenants_invites_email: Optional[pulumi.Input['WorkspaceBulkTenantsInvitesEmailArgs']] = None,
                  captcha_policy: Optional[pulumi.Input['WorkspaceCaptchaPolicyArgs']] = None,
                  custom_domain: Optional[pulumi.Input[str]] = None,
+                 email_verification_email: Optional[pulumi.Input['WorkspaceEmailVerificationEmailArgs']] = None,
                  facebook_social_login: Optional[pulumi.Input['WorkspaceFacebookSocialLoginArgs']] = None,
                  github_social_login: Optional[pulumi.Input['WorkspaceGithubSocialLoginArgs']] = None,
                  google_social_login: Optional[pulumi.Input['WorkspaceGoogleSocialLoginArgs']] = None,
                  hosted_login: Optional[pulumi.Input['WorkspaceHostedLoginArgs']] = None,
+                 impossible_travel_email: Optional[pulumi.Input['WorkspaceImpossibleTravelEmailArgs']] = None,
                  lockout_policy: Optional[pulumi.Input['WorkspaceLockoutPolicyArgs']] = None,
                  magic_code_email: Optional[pulumi.Input['WorkspaceMagicCodeEmailArgs']] = None,
                  magic_link_email: Optional[pulumi.Input['WorkspaceMagicLinkEmailArgs']] = None,
                  mfa_authentication_app: Optional[pulumi.Input['WorkspaceMfaAuthenticationAppArgs']] = None,
+                 mfa_enroll_email: Optional[pulumi.Input['WorkspaceMfaEnrollEmailArgs']] = None,
+                 mfa_otc_email: Optional[pulumi.Input['WorkspaceMfaOtcEmailArgs']] = None,
+                 mfa_recovery_code_email: Optional[pulumi.Input['WorkspaceMfaRecoveryCodeEmailArgs']] = None,
+                 mfa_unenroll_email: Optional[pulumi.Input['WorkspaceMfaUnenrollEmailArgs']] = None,
                  microsoft_social_login: Optional[pulumi.Input['WorkspaceMicrosoftSocialLoginArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  new_device_connected_email: Optional[pulumi.Input['WorkspaceNewDeviceConnectedEmailArgs']] = None,
+                 new_mfa_method_email: Optional[pulumi.Input['WorkspaceNewMfaMethodEmailArgs']] = None,
                  oidc: Optional[pulumi.Input['WorkspaceOidcArgs']] = None,
                  pwned_password_email: Optional[pulumi.Input['WorkspacePwnedPasswordEmailArgs']] = None,
+                 remove_mfa_method_email: Optional[pulumi.Input['WorkspaceRemoveMfaMethodEmailArgs']] = None,
                  reset_password_email: Optional[pulumi.Input['WorkspaceResetPasswordEmailArgs']] = None,
                  reset_phone_number_email: Optional[pulumi.Input['WorkspaceResetPhoneNumberEmailArgs']] = None,
                  saml: Optional[pulumi.Input['WorkspaceSamlArgs']] = None,
+                 sms_authentication_enabled_email: Optional[pulumi.Input['WorkspaceSmsAuthenticationEnabledEmailArgs']] = None,
                  sso_domain_policy: Optional[pulumi.Input['WorkspaceSsoDomainPolicyArgs']] = None,
                  sso_multi_tenant_policy: Optional[pulumi.Input['WorkspaceSsoMultiTenantPolicyArgs']] = None,
+                 suspicious_ip_email: Optional[pulumi.Input['WorkspaceSuspiciousIpEmailArgs']] = None,
                  user_activation_email: Optional[pulumi.Input['WorkspaceUserActivationEmailArgs']] = None,
                  user_invitation_email: Optional[pulumi.Input['WorkspaceUserInvitationEmailArgs']] = None,
                  user_used_invitation_email: Optional[pulumi.Input['WorkspaceUserUsedInvitationEmailArgs']] = None):
         """
         The set of arguments for constructing a Workspace resource.
         :param pulumi.Input['WorkspaceAdminPortalArgs'] admin_portal: Configures the admin portal.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_origins: The origins that are allowed to access the workspace. This parameter controls the value of the "Origin" header for API
@@ -60,93 +72,129 @@
         :param pulumi.Input[str] country: The country associated with the workspace.
         :param pulumi.Input[str] frontegg_domain: The domain at which the Frontegg API is served for this workspace. The domain must end with ".frontegg.com" or
                ".us.frontegg.com".
         :param pulumi.Input[str] frontend_stack: The frontend stack of the application associated with the worksapce.
         :param pulumi.Input['WorkspaceMfaPolicyArgs'] mfa_policy: Configures the multi-factor authentication (MFA) policy.
         :param pulumi.Input[bool] open_saas_installed: Whether the application associated with the workspace has OpenSaaS installed.
         :param pulumi.Input['WorkspacePasswordPolicyArgs'] password_policy: Configures the password policy.
+        :param pulumi.Input['WorkspaceBotDetectionEmailArgs'] bot_detection_email: Configures the bot detection email.
+        :param pulumi.Input['WorkspaceBruteForceProtectionEmailArgs'] brute_force_protection_email: Configures the brute force protection email.
         :param pulumi.Input['WorkspaceBulkTenantsInvitesEmailArgs'] bulk_tenants_invites_email: Configures the bulk tenants invite email.
         :param pulumi.Input['WorkspaceCaptchaPolicyArgs'] captcha_policy: Configures the CAPTCHA policy in the signup form.
         :param pulumi.Input[str] custom_domain: A custom domain at which Frontegg services will be reachable. You must configure a CNAME record for this domain that
                points to "ssl.frontegg.com" (or "ssl.<your-region>.frontegg.com") and a TXT record for domain-challenge.<custom_domain>
                that points to your client ID before setting this field.
+        :param pulumi.Input['WorkspaceEmailVerificationEmailArgs'] email_verification_email: Configures the verification email.
         :param pulumi.Input['WorkspaceFacebookSocialLoginArgs'] facebook_social_login: Configures social login with Facebook.
         :param pulumi.Input['WorkspaceGithubSocialLoginArgs'] github_social_login: Configures social login with GitHub.
         :param pulumi.Input['WorkspaceGoogleSocialLoginArgs'] google_social_login: Configures social login with Google.
         :param pulumi.Input['WorkspaceHostedLoginArgs'] hosted_login: Configures Frontegg-hosted OAuth login.
+        :param pulumi.Input['WorkspaceImpossibleTravelEmailArgs'] impossible_travel_email: Configures the impossible travel email.
         :param pulumi.Input['WorkspaceLockoutPolicyArgs'] lockout_policy: Configures the user lockout policy.
         :param pulumi.Input['WorkspaceMagicCodeEmailArgs'] magic_code_email: Configures the one time code email.
         :param pulumi.Input['WorkspaceMagicLinkEmailArgs'] magic_link_email: Configures the magic link email.
         :param pulumi.Input['WorkspaceMfaAuthenticationAppArgs'] mfa_authentication_app: Configures the multi-factor authentication (MFA) via an authentication app.
+        :param pulumi.Input['WorkspaceMfaEnrollEmailArgs'] mfa_enroll_email: Configures the MFA enroll email.
+        :param pulumi.Input['WorkspaceMfaOtcEmailArgs'] mfa_otc_email: Configures the account challenge with code email.
+        :param pulumi.Input['WorkspaceMfaRecoveryCodeEmailArgs'] mfa_recovery_code_email: Configures the MFA recovery code email.
+        :param pulumi.Input['WorkspaceMfaUnenrollEmailArgs'] mfa_unenroll_email: Configures the MFA unenroll email.
         :param pulumi.Input['WorkspaceMicrosoftSocialLoginArgs'] microsoft_social_login: Configures social login with Google.
         :param pulumi.Input[str] name: The name of the workspace.
         :param pulumi.Input['WorkspaceNewDeviceConnectedEmailArgs'] new_device_connected_email: Configures the new device connected email.
+        :param pulumi.Input['WorkspaceNewMfaMethodEmailArgs'] new_mfa_method_email: Configures the new MFA method email.
         :param pulumi.Input['WorkspaceOidcArgs'] oidc: Configures SSO via OIDC.
         :param pulumi.Input['WorkspacePwnedPasswordEmailArgs'] pwned_password_email: Configures the pwned password email.
+        :param pulumi.Input['WorkspaceRemoveMfaMethodEmailArgs'] remove_mfa_method_email: Configures the remove MFA method email.
         :param pulumi.Input['WorkspaceResetPasswordEmailArgs'] reset_password_email: Configures the password reset email.
         :param pulumi.Input['WorkspaceResetPhoneNumberEmailArgs'] reset_phone_number_email: Configures the reset phone number email.
         :param pulumi.Input['WorkspaceSamlArgs'] saml: Configures SSO via SAML.
+        :param pulumi.Input['WorkspaceSmsAuthenticationEnabledEmailArgs'] sms_authentication_enabled_email: Configures the SMS authentication enabled email.
         :param pulumi.Input['WorkspaceSsoDomainPolicyArgs'] sso_domain_policy: Configures how SSO domains are validated.
         :param pulumi.Input['WorkspaceSsoMultiTenantPolicyArgs'] sso_multi_tenant_policy: Configures how multiple tenants can claim the same SSO domain.
+        :param pulumi.Input['WorkspaceSuspiciousIpEmailArgs'] suspicious_ip_email: Configures the suspicious IP email.
         :param pulumi.Input['WorkspaceUserActivationEmailArgs'] user_activation_email: Configures the user activation email.
         :param pulumi.Input['WorkspaceUserInvitationEmailArgs'] user_invitation_email: Configures the user invitation email.
         :param pulumi.Input['WorkspaceUserUsedInvitationEmailArgs'] user_used_invitation_email: Configures the user used invitation email.
         """
         pulumi.set(__self__, "admin_portal", admin_portal)
         pulumi.set(__self__, "allowed_origins", allowed_origins)
         pulumi.set(__self__, "auth_policy", auth_policy)
         pulumi.set(__self__, "backend_stack", backend_stack)
         pulumi.set(__self__, "country", country)
         pulumi.set(__self__, "frontegg_domain", frontegg_domain)
         pulumi.set(__self__, "frontend_stack", frontend_stack)
         pulumi.set(__self__, "mfa_policy", mfa_policy)
         pulumi.set(__self__, "open_saas_installed", open_saas_installed)
         pulumi.set(__self__, "password_policy", password_policy)
+        if bot_detection_email is not None:
+            pulumi.set(__self__, "bot_detection_email", bot_detection_email)
+        if brute_force_protection_email is not None:
+            pulumi.set(__self__, "brute_force_protection_email", brute_force_protection_email)
         if bulk_tenants_invites_email is not None:
             pulumi.set(__self__, "bulk_tenants_invites_email", bulk_tenants_invites_email)
         if captcha_policy is not None:
             pulumi.set(__self__, "captcha_policy", captcha_policy)
         if custom_domain is not None:
             pulumi.set(__self__, "custom_domain", custom_domain)
+        if email_verification_email is not None:
+            pulumi.set(__self__, "email_verification_email", email_verification_email)
         if facebook_social_login is not None:
             pulumi.set(__self__, "facebook_social_login", facebook_social_login)
         if github_social_login is not None:
             pulumi.set(__self__, "github_social_login", github_social_login)
         if google_social_login is not None:
             pulumi.set(__self__, "google_social_login", google_social_login)
         if hosted_login is not None:
             pulumi.set(__self__, "hosted_login", hosted_login)
+        if impossible_travel_email is not None:
+            pulumi.set(__self__, "impossible_travel_email", impossible_travel_email)
         if lockout_policy is not None:
             pulumi.set(__self__, "lockout_policy", lockout_policy)
         if magic_code_email is not None:
             pulumi.set(__self__, "magic_code_email", magic_code_email)
         if magic_link_email is not None:
             pulumi.set(__self__, "magic_link_email", magic_link_email)
         if mfa_authentication_app is not None:
             pulumi.set(__self__, "mfa_authentication_app", mfa_authentication_app)
+        if mfa_enroll_email is not None:
+            pulumi.set(__self__, "mfa_enroll_email", mfa_enroll_email)
+        if mfa_otc_email is not None:
+            pulumi.set(__self__, "mfa_otc_email", mfa_otc_email)
+        if mfa_recovery_code_email is not None:
+            pulumi.set(__self__, "mfa_recovery_code_email", mfa_recovery_code_email)
+        if mfa_unenroll_email is not None:
+            pulumi.set(__self__, "mfa_unenroll_email", mfa_unenroll_email)
         if microsoft_social_login is not None:
             pulumi.set(__self__, "microsoft_social_login", microsoft_social_login)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if new_device_connected_email is not None:
             pulumi.set(__self__, "new_device_connected_email", new_device_connected_email)
+        if new_mfa_method_email is not None:
+            pulumi.set(__self__, "new_mfa_method_email", new_mfa_method_email)
         if oidc is not None:
             pulumi.set(__self__, "oidc", oidc)
         if pwned_password_email is not None:
             pulumi.set(__self__, "pwned_password_email", pwned_password_email)
+        if remove_mfa_method_email is not None:
+            pulumi.set(__self__, "remove_mfa_method_email", remove_mfa_method_email)
         if reset_password_email is not None:
             pulumi.set(__self__, "reset_password_email", reset_password_email)
         if reset_phone_number_email is not None:
             pulumi.set(__self__, "reset_phone_number_email", reset_phone_number_email)
         if saml is not None:
             pulumi.set(__self__, "saml", saml)
+        if sms_authentication_enabled_email is not None:
+            pulumi.set(__self__, "sms_authentication_enabled_email", sms_authentication_enabled_email)
         if sso_domain_policy is not None:
             pulumi.set(__self__, "sso_domain_policy", sso_domain_policy)
         if sso_multi_tenant_policy is not None:
             pulumi.set(__self__, "sso_multi_tenant_policy", sso_multi_tenant_policy)
+        if suspicious_ip_email is not None:
+            pulumi.set(__self__, "suspicious_ip_email", suspicious_ip_email)
         if user_activation_email is not None:
             pulumi.set(__self__, "user_activation_email", user_activation_email)
         if user_invitation_email is not None:
             pulumi.set(__self__, "user_invitation_email", user_invitation_email)
         if user_used_invitation_email is not None:
             pulumi.set(__self__, "user_used_invitation_email", user_used_invitation_email)
 
@@ -269,14 +317,38 @@
         return pulumi.get(self, "password_policy")
 
     @password_policy.setter
     def password_policy(self, value: pulumi.Input['WorkspacePasswordPolicyArgs']):
         pulumi.set(self, "password_policy", value)
 
     @property
+    @pulumi.getter(name="botDetectionEmail")
+    def bot_detection_email(self) -> Optional[pulumi.Input['WorkspaceBotDetectionEmailArgs']]:
+        """
+        Configures the bot detection email.
+        """
+        return pulumi.get(self, "bot_detection_email")
+
+    @bot_detection_email.setter
+    def bot_detection_email(self, value: Optional[pulumi.Input['WorkspaceBotDetectionEmailArgs']]):
+        pulumi.set(self, "bot_detection_email", value)
+
+    @property
+    @pulumi.getter(name="bruteForceProtectionEmail")
+    def brute_force_protection_email(self) -> Optional[pulumi.Input['WorkspaceBruteForceProtectionEmailArgs']]:
+        """
+        Configures the brute force protection email.
+        """
+        return pulumi.get(self, "brute_force_protection_email")
+
+    @brute_force_protection_email.setter
+    def brute_force_protection_email(self, value: Optional[pulumi.Input['WorkspaceBruteForceProtectionEmailArgs']]):
+        pulumi.set(self, "brute_force_protection_email", value)
+
+    @property
     @pulumi.getter(name="bulkTenantsInvitesEmail")
     def bulk_tenants_invites_email(self) -> Optional[pulumi.Input['WorkspaceBulkTenantsInvitesEmailArgs']]:
         """
         Configures the bulk tenants invite email.
         """
         return pulumi.get(self, "bulk_tenants_invites_email")
 
@@ -307,14 +379,26 @@
         return pulumi.get(self, "custom_domain")
 
     @custom_domain.setter
     def custom_domain(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "custom_domain", value)
 
     @property
+    @pulumi.getter(name="emailVerificationEmail")
+    def email_verification_email(self) -> Optional[pulumi.Input['WorkspaceEmailVerificationEmailArgs']]:
+        """
+        Configures the verification email.
+        """
+        return pulumi.get(self, "email_verification_email")
+
+    @email_verification_email.setter
+    def email_verification_email(self, value: Optional[pulumi.Input['WorkspaceEmailVerificationEmailArgs']]):
+        pulumi.set(self, "email_verification_email", value)
+
+    @property
     @pulumi.getter(name="facebookSocialLogin")
     def facebook_social_login(self) -> Optional[pulumi.Input['WorkspaceFacebookSocialLoginArgs']]:
         """
         Configures social login with Facebook.
         """
         return pulumi.get(self, "facebook_social_login")
 
@@ -355,14 +439,26 @@
         return pulumi.get(self, "hosted_login")
 
     @hosted_login.setter
     def hosted_login(self, value: Optional[pulumi.Input['WorkspaceHostedLoginArgs']]):
         pulumi.set(self, "hosted_login", value)
 
     @property
+    @pulumi.getter(name="impossibleTravelEmail")
+    def impossible_travel_email(self) -> Optional[pulumi.Input['WorkspaceImpossibleTravelEmailArgs']]:
+        """
+        Configures the impossible travel email.
+        """
+        return pulumi.get(self, "impossible_travel_email")
+
+    @impossible_travel_email.setter
+    def impossible_travel_email(self, value: Optional[pulumi.Input['WorkspaceImpossibleTravelEmailArgs']]):
+        pulumi.set(self, "impossible_travel_email", value)
+
+    @property
     @pulumi.getter(name="lockoutPolicy")
     def lockout_policy(self) -> Optional[pulumi.Input['WorkspaceLockoutPolicyArgs']]:
         """
         Configures the user lockout policy.
         """
         return pulumi.get(self, "lockout_policy")
 
@@ -403,14 +499,62 @@
         return pulumi.get(self, "mfa_authentication_app")
 
     @mfa_authentication_app.setter
     def mfa_authentication_app(self, value: Optional[pulumi.Input['WorkspaceMfaAuthenticationAppArgs']]):
         pulumi.set(self, "mfa_authentication_app", value)
 
     @property
+    @pulumi.getter(name="mfaEnrollEmail")
+    def mfa_enroll_email(self) -> Optional[pulumi.Input['WorkspaceMfaEnrollEmailArgs']]:
+        """
+        Configures the MFA enroll email.
+        """
+        return pulumi.get(self, "mfa_enroll_email")
+
+    @mfa_enroll_email.setter
+    def mfa_enroll_email(self, value: Optional[pulumi.Input['WorkspaceMfaEnrollEmailArgs']]):
+        pulumi.set(self, "mfa_enroll_email", value)
+
+    @property
+    @pulumi.getter(name="mfaOtcEmail")
+    def mfa_otc_email(self) -> Optional[pulumi.Input['WorkspaceMfaOtcEmailArgs']]:
+        """
+        Configures the account challenge with code email.
+        """
+        return pulumi.get(self, "mfa_otc_email")
+
+    @mfa_otc_email.setter
+    def mfa_otc_email(self, value: Optional[pulumi.Input['WorkspaceMfaOtcEmailArgs']]):
+        pulumi.set(self, "mfa_otc_email", value)
+
+    @property
+    @pulumi.getter(name="mfaRecoveryCodeEmail")
+    def mfa_recovery_code_email(self) -> Optional[pulumi.Input['WorkspaceMfaRecoveryCodeEmailArgs']]:
+        """
+        Configures the MFA recovery code email.
+        """
+        return pulumi.get(self, "mfa_recovery_code_email")
+
+    @mfa_recovery_code_email.setter
+    def mfa_recovery_code_email(self, value: Optional[pulumi.Input['WorkspaceMfaRecoveryCodeEmailArgs']]):
+        pulumi.set(self, "mfa_recovery_code_email", value)
+
+    @property
+    @pulumi.getter(name="mfaUnenrollEmail")
+    def mfa_unenroll_email(self) -> Optional[pulumi.Input['WorkspaceMfaUnenrollEmailArgs']]:
+        """
+        Configures the MFA unenroll email.
+        """
+        return pulumi.get(self, "mfa_unenroll_email")
+
+    @mfa_unenroll_email.setter
+    def mfa_unenroll_email(self, value: Optional[pulumi.Input['WorkspaceMfaUnenrollEmailArgs']]):
+        pulumi.set(self, "mfa_unenroll_email", value)
+
+    @property
     @pulumi.getter(name="microsoftSocialLogin")
     def microsoft_social_login(self) -> Optional[pulumi.Input['WorkspaceMicrosoftSocialLoginArgs']]:
         """
         Configures social login with Google.
         """
         return pulumi.get(self, "microsoft_social_login")
 
@@ -439,14 +583,26 @@
         return pulumi.get(self, "new_device_connected_email")
 
     @new_device_connected_email.setter
     def new_device_connected_email(self, value: Optional[pulumi.Input['WorkspaceNewDeviceConnectedEmailArgs']]):
         pulumi.set(self, "new_device_connected_email", value)
 
     @property
+    @pulumi.getter(name="newMfaMethodEmail")
+    def new_mfa_method_email(self) -> Optional[pulumi.Input['WorkspaceNewMfaMethodEmailArgs']]:
+        """
+        Configures the new MFA method email.
+        """
+        return pulumi.get(self, "new_mfa_method_email")
+
+    @new_mfa_method_email.setter
+    def new_mfa_method_email(self, value: Optional[pulumi.Input['WorkspaceNewMfaMethodEmailArgs']]):
+        pulumi.set(self, "new_mfa_method_email", value)
+
+    @property
     @pulumi.getter
     def oidc(self) -> Optional[pulumi.Input['WorkspaceOidcArgs']]:
         """
         Configures SSO via OIDC.
         """
         return pulumi.get(self, "oidc")
 
@@ -463,14 +619,26 @@
         return pulumi.get(self, "pwned_password_email")
 
     @pwned_password_email.setter
     def pwned_password_email(self, value: Optional[pulumi.Input['WorkspacePwnedPasswordEmailArgs']]):
         pulumi.set(self, "pwned_password_email", value)
 
     @property
+    @pulumi.getter(name="removeMfaMethodEmail")
+    def remove_mfa_method_email(self) -> Optional[pulumi.Input['WorkspaceRemoveMfaMethodEmailArgs']]:
+        """
+        Configures the remove MFA method email.
+        """
+        return pulumi.get(self, "remove_mfa_method_email")
+
+    @remove_mfa_method_email.setter
+    def remove_mfa_method_email(self, value: Optional[pulumi.Input['WorkspaceRemoveMfaMethodEmailArgs']]):
+        pulumi.set(self, "remove_mfa_method_email", value)
+
+    @property
     @pulumi.getter(name="resetPasswordEmail")
     def reset_password_email(self) -> Optional[pulumi.Input['WorkspaceResetPasswordEmailArgs']]:
         """
         Configures the password reset email.
         """
         return pulumi.get(self, "reset_password_email")
 
@@ -499,14 +667,26 @@
         return pulumi.get(self, "saml")
 
     @saml.setter
     def saml(self, value: Optional[pulumi.Input['WorkspaceSamlArgs']]):
         pulumi.set(self, "saml", value)
 
     @property
+    @pulumi.getter(name="smsAuthenticationEnabledEmail")
+    def sms_authentication_enabled_email(self) -> Optional[pulumi.Input['WorkspaceSmsAuthenticationEnabledEmailArgs']]:
+        """
+        Configures the SMS authentication enabled email.
+        """
+        return pulumi.get(self, "sms_authentication_enabled_email")
+
+    @sms_authentication_enabled_email.setter
+    def sms_authentication_enabled_email(self, value: Optional[pulumi.Input['WorkspaceSmsAuthenticationEnabledEmailArgs']]):
+        pulumi.set(self, "sms_authentication_enabled_email", value)
+
+    @property
     @pulumi.getter(name="ssoDomainPolicy")
     def sso_domain_policy(self) -> Optional[pulumi.Input['WorkspaceSsoDomainPolicyArgs']]:
         """
         Configures how SSO domains are validated.
         """
         return pulumi.get(self, "sso_domain_policy")
 
@@ -523,14 +703,26 @@
         return pulumi.get(self, "sso_multi_tenant_policy")
 
     @sso_multi_tenant_policy.setter
     def sso_multi_tenant_policy(self, value: Optional[pulumi.Input['WorkspaceSsoMultiTenantPolicyArgs']]):
         pulumi.set(self, "sso_multi_tenant_policy", value)
 
     @property
+    @pulumi.getter(name="suspiciousIpEmail")
+    def suspicious_ip_email(self) -> Optional[pulumi.Input['WorkspaceSuspiciousIpEmailArgs']]:
+        """
+        Configures the suspicious IP email.
+        """
+        return pulumi.get(self, "suspicious_ip_email")
+
+    @suspicious_ip_email.setter
+    def suspicious_ip_email(self, value: Optional[pulumi.Input['WorkspaceSuspiciousIpEmailArgs']]):
+        pulumi.set(self, "suspicious_ip_email", value)
+
+    @property
     @pulumi.getter(name="userActivationEmail")
     def user_activation_email(self) -> Optional[pulumi.Input['WorkspaceUserActivationEmailArgs']]:
         """
         Configures the user activation email.
         """
         return pulumi.get(self, "user_activation_email")
 
@@ -566,147 +758,195 @@
 @pulumi.input_type
 class _WorkspaceState:
     def __init__(__self__, *,
                  admin_portal: Optional[pulumi.Input['WorkspaceAdminPortalArgs']] = None,
                  allowed_origins: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  auth_policy: Optional[pulumi.Input['WorkspaceAuthPolicyArgs']] = None,
                  backend_stack: Optional[pulumi.Input[str]] = None,
+                 bot_detection_email: Optional[pulumi.Input['WorkspaceBotDetectionEmailArgs']] = None,
+                 brute_force_protection_email: Optional[pulumi.Input['WorkspaceBruteForceProtectionEmailArgs']] = None,
                  bulk_tenants_invites_email: Optional[pulumi.Input['WorkspaceBulkTenantsInvitesEmailArgs']] = None,
                  captcha_policy: Optional[pulumi.Input['WorkspaceCaptchaPolicyArgs']] = None,
                  country: Optional[pulumi.Input[str]] = None,
                  custom_domain: Optional[pulumi.Input[str]] = None,
+                 email_verification_email: Optional[pulumi.Input['WorkspaceEmailVerificationEmailArgs']] = None,
                  facebook_social_login: Optional[pulumi.Input['WorkspaceFacebookSocialLoginArgs']] = None,
                  frontegg_domain: Optional[pulumi.Input[str]] = None,
                  frontend_stack: Optional[pulumi.Input[str]] = None,
                  github_social_login: Optional[pulumi.Input['WorkspaceGithubSocialLoginArgs']] = None,
                  google_social_login: Optional[pulumi.Input['WorkspaceGoogleSocialLoginArgs']] = None,
                  hosted_login: Optional[pulumi.Input['WorkspaceHostedLoginArgs']] = None,
+                 impossible_travel_email: Optional[pulumi.Input['WorkspaceImpossibleTravelEmailArgs']] = None,
                  lockout_policy: Optional[pulumi.Input['WorkspaceLockoutPolicyArgs']] = None,
                  magic_code_email: Optional[pulumi.Input['WorkspaceMagicCodeEmailArgs']] = None,
                  magic_link_email: Optional[pulumi.Input['WorkspaceMagicLinkEmailArgs']] = None,
                  mfa_authentication_app: Optional[pulumi.Input['WorkspaceMfaAuthenticationAppArgs']] = None,
+                 mfa_enroll_email: Optional[pulumi.Input['WorkspaceMfaEnrollEmailArgs']] = None,
+                 mfa_otc_email: Optional[pulumi.Input['WorkspaceMfaOtcEmailArgs']] = None,
                  mfa_policy: Optional[pulumi.Input['WorkspaceMfaPolicyArgs']] = None,
+                 mfa_recovery_code_email: Optional[pulumi.Input['WorkspaceMfaRecoveryCodeEmailArgs']] = None,
+                 mfa_unenroll_email: Optional[pulumi.Input['WorkspaceMfaUnenrollEmailArgs']] = None,
                  microsoft_social_login: Optional[pulumi.Input['WorkspaceMicrosoftSocialLoginArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  new_device_connected_email: Optional[pulumi.Input['WorkspaceNewDeviceConnectedEmailArgs']] = None,
+                 new_mfa_method_email: Optional[pulumi.Input['WorkspaceNewMfaMethodEmailArgs']] = None,
                  oidc: Optional[pulumi.Input['WorkspaceOidcArgs']] = None,
                  open_saas_installed: Optional[pulumi.Input[bool]] = None,
                  password_policy: Optional[pulumi.Input['WorkspacePasswordPolicyArgs']] = None,
                  pwned_password_email: Optional[pulumi.Input['WorkspacePwnedPasswordEmailArgs']] = None,
+                 remove_mfa_method_email: Optional[pulumi.Input['WorkspaceRemoveMfaMethodEmailArgs']] = None,
                  reset_password_email: Optional[pulumi.Input['WorkspaceResetPasswordEmailArgs']] = None,
                  reset_phone_number_email: Optional[pulumi.Input['WorkspaceResetPhoneNumberEmailArgs']] = None,
                  saml: Optional[pulumi.Input['WorkspaceSamlArgs']] = None,
+                 sms_authentication_enabled_email: Optional[pulumi.Input['WorkspaceSmsAuthenticationEnabledEmailArgs']] = None,
                  sso_domain_policy: Optional[pulumi.Input['WorkspaceSsoDomainPolicyArgs']] = None,
                  sso_multi_tenant_policy: Optional[pulumi.Input['WorkspaceSsoMultiTenantPolicyArgs']] = None,
+                 suspicious_ip_email: Optional[pulumi.Input['WorkspaceSuspiciousIpEmailArgs']] = None,
                  user_activation_email: Optional[pulumi.Input['WorkspaceUserActivationEmailArgs']] = None,
                  user_invitation_email: Optional[pulumi.Input['WorkspaceUserInvitationEmailArgs']] = None,
                  user_used_invitation_email: Optional[pulumi.Input['WorkspaceUserUsedInvitationEmailArgs']] = None):
         """
         Input properties used for looking up and filtering Workspace resources.
         :param pulumi.Input['WorkspaceAdminPortalArgs'] admin_portal: Configures the admin portal.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_origins: The origins that are allowed to access the workspace. This parameter controls the value of the "Origin" header for API
                responses.
         :param pulumi.Input['WorkspaceAuthPolicyArgs'] auth_policy: Configures the general authentication policy.
         :param pulumi.Input[str] backend_stack: The backend stack of the application associated with the workspace.
+        :param pulumi.Input['WorkspaceBotDetectionEmailArgs'] bot_detection_email: Configures the bot detection email.
+        :param pulumi.Input['WorkspaceBruteForceProtectionEmailArgs'] brute_force_protection_email: Configures the brute force protection email.
         :param pulumi.Input['WorkspaceBulkTenantsInvitesEmailArgs'] bulk_tenants_invites_email: Configures the bulk tenants invite email.
         :param pulumi.Input['WorkspaceCaptchaPolicyArgs'] captcha_policy: Configures the CAPTCHA policy in the signup form.
         :param pulumi.Input[str] country: The country associated with the workspace.
         :param pulumi.Input[str] custom_domain: A custom domain at which Frontegg services will be reachable. You must configure a CNAME record for this domain that
                points to "ssl.frontegg.com" (or "ssl.<your-region>.frontegg.com") and a TXT record for domain-challenge.<custom_domain>
                that points to your client ID before setting this field.
+        :param pulumi.Input['WorkspaceEmailVerificationEmailArgs'] email_verification_email: Configures the verification email.
         :param pulumi.Input['WorkspaceFacebookSocialLoginArgs'] facebook_social_login: Configures social login with Facebook.
         :param pulumi.Input[str] frontegg_domain: The domain at which the Frontegg API is served for this workspace. The domain must end with ".frontegg.com" or
                ".us.frontegg.com".
         :param pulumi.Input[str] frontend_stack: The frontend stack of the application associated with the worksapce.
         :param pulumi.Input['WorkspaceGithubSocialLoginArgs'] github_social_login: Configures social login with GitHub.
         :param pulumi.Input['WorkspaceGoogleSocialLoginArgs'] google_social_login: Configures social login with Google.
         :param pulumi.Input['WorkspaceHostedLoginArgs'] hosted_login: Configures Frontegg-hosted OAuth login.
+        :param pulumi.Input['WorkspaceImpossibleTravelEmailArgs'] impossible_travel_email: Configures the impossible travel email.
         :param pulumi.Input['WorkspaceLockoutPolicyArgs'] lockout_policy: Configures the user lockout policy.
         :param pulumi.Input['WorkspaceMagicCodeEmailArgs'] magic_code_email: Configures the one time code email.
         :param pulumi.Input['WorkspaceMagicLinkEmailArgs'] magic_link_email: Configures the magic link email.
         :param pulumi.Input['WorkspaceMfaAuthenticationAppArgs'] mfa_authentication_app: Configures the multi-factor authentication (MFA) via an authentication app.
+        :param pulumi.Input['WorkspaceMfaEnrollEmailArgs'] mfa_enroll_email: Configures the MFA enroll email.
+        :param pulumi.Input['WorkspaceMfaOtcEmailArgs'] mfa_otc_email: Configures the account challenge with code email.
         :param pulumi.Input['WorkspaceMfaPolicyArgs'] mfa_policy: Configures the multi-factor authentication (MFA) policy.
+        :param pulumi.Input['WorkspaceMfaRecoveryCodeEmailArgs'] mfa_recovery_code_email: Configures the MFA recovery code email.
+        :param pulumi.Input['WorkspaceMfaUnenrollEmailArgs'] mfa_unenroll_email: Configures the MFA unenroll email.
         :param pulumi.Input['WorkspaceMicrosoftSocialLoginArgs'] microsoft_social_login: Configures social login with Google.
         :param pulumi.Input[str] name: The name of the workspace.
         :param pulumi.Input['WorkspaceNewDeviceConnectedEmailArgs'] new_device_connected_email: Configures the new device connected email.
+        :param pulumi.Input['WorkspaceNewMfaMethodEmailArgs'] new_mfa_method_email: Configures the new MFA method email.
         :param pulumi.Input['WorkspaceOidcArgs'] oidc: Configures SSO via OIDC.
         :param pulumi.Input[bool] open_saas_installed: Whether the application associated with the workspace has OpenSaaS installed.
         :param pulumi.Input['WorkspacePasswordPolicyArgs'] password_policy: Configures the password policy.
         :param pulumi.Input['WorkspacePwnedPasswordEmailArgs'] pwned_password_email: Configures the pwned password email.
+        :param pulumi.Input['WorkspaceRemoveMfaMethodEmailArgs'] remove_mfa_method_email: Configures the remove MFA method email.
         :param pulumi.Input['WorkspaceResetPasswordEmailArgs'] reset_password_email: Configures the password reset email.
         :param pulumi.Input['WorkspaceResetPhoneNumberEmailArgs'] reset_phone_number_email: Configures the reset phone number email.
         :param pulumi.Input['WorkspaceSamlArgs'] saml: Configures SSO via SAML.
+        :param pulumi.Input['WorkspaceSmsAuthenticationEnabledEmailArgs'] sms_authentication_enabled_email: Configures the SMS authentication enabled email.
         :param pulumi.Input['WorkspaceSsoDomainPolicyArgs'] sso_domain_policy: Configures how SSO domains are validated.
         :param pulumi.Input['WorkspaceSsoMultiTenantPolicyArgs'] sso_multi_tenant_policy: Configures how multiple tenants can claim the same SSO domain.
+        :param pulumi.Input['WorkspaceSuspiciousIpEmailArgs'] suspicious_ip_email: Configures the suspicious IP email.
         :param pulumi.Input['WorkspaceUserActivationEmailArgs'] user_activation_email: Configures the user activation email.
         :param pulumi.Input['WorkspaceUserInvitationEmailArgs'] user_invitation_email: Configures the user invitation email.
         :param pulumi.Input['WorkspaceUserUsedInvitationEmailArgs'] user_used_invitation_email: Configures the user used invitation email.
         """
         if admin_portal is not None:
             pulumi.set(__self__, "admin_portal", admin_portal)
         if allowed_origins is not None:
             pulumi.set(__self__, "allowed_origins", allowed_origins)
         if auth_policy is not None:
             pulumi.set(__self__, "auth_policy", auth_policy)
         if backend_stack is not None:
             pulumi.set(__self__, "backend_stack", backend_stack)
+        if bot_detection_email is not None:
+            pulumi.set(__self__, "bot_detection_email", bot_detection_email)
+        if brute_force_protection_email is not None:
+            pulumi.set(__self__, "brute_force_protection_email", brute_force_protection_email)
         if bulk_tenants_invites_email is not None:
             pulumi.set(__self__, "bulk_tenants_invites_email", bulk_tenants_invites_email)
         if captcha_policy is not None:
             pulumi.set(__self__, "captcha_policy", captcha_policy)
         if country is not None:
             pulumi.set(__self__, "country", country)
         if custom_domain is not None:
             pulumi.set(__self__, "custom_domain", custom_domain)
+        if email_verification_email is not None:
+            pulumi.set(__self__, "email_verification_email", email_verification_email)
         if facebook_social_login is not None:
             pulumi.set(__self__, "facebook_social_login", facebook_social_login)
         if frontegg_domain is not None:
             pulumi.set(__self__, "frontegg_domain", frontegg_domain)
         if frontend_stack is not None:
             pulumi.set(__self__, "frontend_stack", frontend_stack)
         if github_social_login is not None:
             pulumi.set(__self__, "github_social_login", github_social_login)
         if google_social_login is not None:
             pulumi.set(__self__, "google_social_login", google_social_login)
         if hosted_login is not None:
             pulumi.set(__self__, "hosted_login", hosted_login)
+        if impossible_travel_email is not None:
+            pulumi.set(__self__, "impossible_travel_email", impossible_travel_email)
         if lockout_policy is not None:
             pulumi.set(__self__, "lockout_policy", lockout_policy)
         if magic_code_email is not None:
             pulumi.set(__self__, "magic_code_email", magic_code_email)
         if magic_link_email is not None:
             pulumi.set(__self__, "magic_link_email", magic_link_email)
         if mfa_authentication_app is not None:
             pulumi.set(__self__, "mfa_authentication_app", mfa_authentication_app)
+        if mfa_enroll_email is not None:
+            pulumi.set(__self__, "mfa_enroll_email", mfa_enroll_email)
+        if mfa_otc_email is not None:
+            pulumi.set(__self__, "mfa_otc_email", mfa_otc_email)
         if mfa_policy is not None:
             pulumi.set(__self__, "mfa_policy", mfa_policy)
+        if mfa_recovery_code_email is not None:
+            pulumi.set(__self__, "mfa_recovery_code_email", mfa_recovery_code_email)
+        if mfa_unenroll_email is not None:
+            pulumi.set(__self__, "mfa_unenroll_email", mfa_unenroll_email)
         if microsoft_social_login is not None:
             pulumi.set(__self__, "microsoft_social_login", microsoft_social_login)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if new_device_connected_email is not None:
             pulumi.set(__self__, "new_device_connected_email", new_device_connected_email)
+        if new_mfa_method_email is not None:
+            pulumi.set(__self__, "new_mfa_method_email", new_mfa_method_email)
         if oidc is not None:
             pulumi.set(__self__, "oidc", oidc)
         if open_saas_installed is not None:
             pulumi.set(__self__, "open_saas_installed", open_saas_installed)
         if password_policy is not None:
             pulumi.set(__self__, "password_policy", password_policy)
         if pwned_password_email is not None:
             pulumi.set(__self__, "pwned_password_email", pwned_password_email)
+        if remove_mfa_method_email is not None:
+            pulumi.set(__self__, "remove_mfa_method_email", remove_mfa_method_email)
         if reset_password_email is not None:
             pulumi.set(__self__, "reset_password_email", reset_password_email)
         if reset_phone_number_email is not None:
             pulumi.set(__self__, "reset_phone_number_email", reset_phone_number_email)
         if saml is not None:
             pulumi.set(__self__, "saml", saml)
+        if sms_authentication_enabled_email is not None:
+            pulumi.set(__self__, "sms_authentication_enabled_email", sms_authentication_enabled_email)
         if sso_domain_policy is not None:
             pulumi.set(__self__, "sso_domain_policy", sso_domain_policy)
         if sso_multi_tenant_policy is not None:
             pulumi.set(__self__, "sso_multi_tenant_policy", sso_multi_tenant_policy)
+        if suspicious_ip_email is not None:
+            pulumi.set(__self__, "suspicious_ip_email", suspicious_ip_email)
         if user_activation_email is not None:
             pulumi.set(__self__, "user_activation_email", user_activation_email)
         if user_invitation_email is not None:
             pulumi.set(__self__, "user_invitation_email", user_invitation_email)
         if user_used_invitation_email is not None:
             pulumi.set(__self__, "user_used_invitation_email", user_used_invitation_email)
 
@@ -756,14 +996,38 @@
         return pulumi.get(self, "backend_stack")
 
     @backend_stack.setter
     def backend_stack(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "backend_stack", value)
 
     @property
+    @pulumi.getter(name="botDetectionEmail")
+    def bot_detection_email(self) -> Optional[pulumi.Input['WorkspaceBotDetectionEmailArgs']]:
+        """
+        Configures the bot detection email.
+        """
+        return pulumi.get(self, "bot_detection_email")
+
+    @bot_detection_email.setter
+    def bot_detection_email(self, value: Optional[pulumi.Input['WorkspaceBotDetectionEmailArgs']]):
+        pulumi.set(self, "bot_detection_email", value)
+
+    @property
+    @pulumi.getter(name="bruteForceProtectionEmail")
+    def brute_force_protection_email(self) -> Optional[pulumi.Input['WorkspaceBruteForceProtectionEmailArgs']]:
+        """
+        Configures the brute force protection email.
+        """
+        return pulumi.get(self, "brute_force_protection_email")
+
+    @brute_force_protection_email.setter
+    def brute_force_protection_email(self, value: Optional[pulumi.Input['WorkspaceBruteForceProtectionEmailArgs']]):
+        pulumi.set(self, "brute_force_protection_email", value)
+
+    @property
     @pulumi.getter(name="bulkTenantsInvitesEmail")
     def bulk_tenants_invites_email(self) -> Optional[pulumi.Input['WorkspaceBulkTenantsInvitesEmailArgs']]:
         """
         Configures the bulk tenants invite email.
         """
         return pulumi.get(self, "bulk_tenants_invites_email")
 
@@ -806,14 +1070,26 @@
         return pulumi.get(self, "custom_domain")
 
     @custom_domain.setter
     def custom_domain(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "custom_domain", value)
 
     @property
+    @pulumi.getter(name="emailVerificationEmail")
+    def email_verification_email(self) -> Optional[pulumi.Input['WorkspaceEmailVerificationEmailArgs']]:
+        """
+        Configures the verification email.
+        """
+        return pulumi.get(self, "email_verification_email")
+
+    @email_verification_email.setter
+    def email_verification_email(self, value: Optional[pulumi.Input['WorkspaceEmailVerificationEmailArgs']]):
+        pulumi.set(self, "email_verification_email", value)
+
+    @property
     @pulumi.getter(name="facebookSocialLogin")
     def facebook_social_login(self) -> Optional[pulumi.Input['WorkspaceFacebookSocialLoginArgs']]:
         """
         Configures social login with Facebook.
         """
         return pulumi.get(self, "facebook_social_login")
 
@@ -879,14 +1155,26 @@
         return pulumi.get(self, "hosted_login")
 
     @hosted_login.setter
     def hosted_login(self, value: Optional[pulumi.Input['WorkspaceHostedLoginArgs']]):
         pulumi.set(self, "hosted_login", value)
 
     @property
+    @pulumi.getter(name="impossibleTravelEmail")
+    def impossible_travel_email(self) -> Optional[pulumi.Input['WorkspaceImpossibleTravelEmailArgs']]:
+        """
+        Configures the impossible travel email.
+        """
+        return pulumi.get(self, "impossible_travel_email")
+
+    @impossible_travel_email.setter
+    def impossible_travel_email(self, value: Optional[pulumi.Input['WorkspaceImpossibleTravelEmailArgs']]):
+        pulumi.set(self, "impossible_travel_email", value)
+
+    @property
     @pulumi.getter(name="lockoutPolicy")
     def lockout_policy(self) -> Optional[pulumi.Input['WorkspaceLockoutPolicyArgs']]:
         """
         Configures the user lockout policy.
         """
         return pulumi.get(self, "lockout_policy")
 
@@ -927,26 +1215,74 @@
         return pulumi.get(self, "mfa_authentication_app")
 
     @mfa_authentication_app.setter
     def mfa_authentication_app(self, value: Optional[pulumi.Input['WorkspaceMfaAuthenticationAppArgs']]):
         pulumi.set(self, "mfa_authentication_app", value)
 
     @property
+    @pulumi.getter(name="mfaEnrollEmail")
+    def mfa_enroll_email(self) -> Optional[pulumi.Input['WorkspaceMfaEnrollEmailArgs']]:
+        """
+        Configures the MFA enroll email.
+        """
+        return pulumi.get(self, "mfa_enroll_email")
+
+    @mfa_enroll_email.setter
+    def mfa_enroll_email(self, value: Optional[pulumi.Input['WorkspaceMfaEnrollEmailArgs']]):
+        pulumi.set(self, "mfa_enroll_email", value)
+
+    @property
+    @pulumi.getter(name="mfaOtcEmail")
+    def mfa_otc_email(self) -> Optional[pulumi.Input['WorkspaceMfaOtcEmailArgs']]:
+        """
+        Configures the account challenge with code email.
+        """
+        return pulumi.get(self, "mfa_otc_email")
+
+    @mfa_otc_email.setter
+    def mfa_otc_email(self, value: Optional[pulumi.Input['WorkspaceMfaOtcEmailArgs']]):
+        pulumi.set(self, "mfa_otc_email", value)
+
+    @property
     @pulumi.getter(name="mfaPolicy")
     def mfa_policy(self) -> Optional[pulumi.Input['WorkspaceMfaPolicyArgs']]:
         """
         Configures the multi-factor authentication (MFA) policy.
         """
         return pulumi.get(self, "mfa_policy")
 
     @mfa_policy.setter
     def mfa_policy(self, value: Optional[pulumi.Input['WorkspaceMfaPolicyArgs']]):
         pulumi.set(self, "mfa_policy", value)
 
     @property
+    @pulumi.getter(name="mfaRecoveryCodeEmail")
+    def mfa_recovery_code_email(self) -> Optional[pulumi.Input['WorkspaceMfaRecoveryCodeEmailArgs']]:
+        """
+        Configures the MFA recovery code email.
+        """
+        return pulumi.get(self, "mfa_recovery_code_email")
+
+    @mfa_recovery_code_email.setter
+    def mfa_recovery_code_email(self, value: Optional[pulumi.Input['WorkspaceMfaRecoveryCodeEmailArgs']]):
+        pulumi.set(self, "mfa_recovery_code_email", value)
+
+    @property
+    @pulumi.getter(name="mfaUnenrollEmail")
+    def mfa_unenroll_email(self) -> Optional[pulumi.Input['WorkspaceMfaUnenrollEmailArgs']]:
+        """
+        Configures the MFA unenroll email.
+        """
+        return pulumi.get(self, "mfa_unenroll_email")
+
+    @mfa_unenroll_email.setter
+    def mfa_unenroll_email(self, value: Optional[pulumi.Input['WorkspaceMfaUnenrollEmailArgs']]):
+        pulumi.set(self, "mfa_unenroll_email", value)
+
+    @property
     @pulumi.getter(name="microsoftSocialLogin")
     def microsoft_social_login(self) -> Optional[pulumi.Input['WorkspaceMicrosoftSocialLoginArgs']]:
         """
         Configures social login with Google.
         """
         return pulumi.get(self, "microsoft_social_login")
 
@@ -975,14 +1311,26 @@
         return pulumi.get(self, "new_device_connected_email")
 
     @new_device_connected_email.setter
     def new_device_connected_email(self, value: Optional[pulumi.Input['WorkspaceNewDeviceConnectedEmailArgs']]):
         pulumi.set(self, "new_device_connected_email", value)
 
     @property
+    @pulumi.getter(name="newMfaMethodEmail")
+    def new_mfa_method_email(self) -> Optional[pulumi.Input['WorkspaceNewMfaMethodEmailArgs']]:
+        """
+        Configures the new MFA method email.
+        """
+        return pulumi.get(self, "new_mfa_method_email")
+
+    @new_mfa_method_email.setter
+    def new_mfa_method_email(self, value: Optional[pulumi.Input['WorkspaceNewMfaMethodEmailArgs']]):
+        pulumi.set(self, "new_mfa_method_email", value)
+
+    @property
     @pulumi.getter
     def oidc(self) -> Optional[pulumi.Input['WorkspaceOidcArgs']]:
         """
         Configures SSO via OIDC.
         """
         return pulumi.get(self, "oidc")
 
@@ -1023,14 +1371,26 @@
         return pulumi.get(self, "pwned_password_email")
 
     @pwned_password_email.setter
     def pwned_password_email(self, value: Optional[pulumi.Input['WorkspacePwnedPasswordEmailArgs']]):
         pulumi.set(self, "pwned_password_email", value)
 
     @property
+    @pulumi.getter(name="removeMfaMethodEmail")
+    def remove_mfa_method_email(self) -> Optional[pulumi.Input['WorkspaceRemoveMfaMethodEmailArgs']]:
+        """
+        Configures the remove MFA method email.
+        """
+        return pulumi.get(self, "remove_mfa_method_email")
+
+    @remove_mfa_method_email.setter
+    def remove_mfa_method_email(self, value: Optional[pulumi.Input['WorkspaceRemoveMfaMethodEmailArgs']]):
+        pulumi.set(self, "remove_mfa_method_email", value)
+
+    @property
     @pulumi.getter(name="resetPasswordEmail")
     def reset_password_email(self) -> Optional[pulumi.Input['WorkspaceResetPasswordEmailArgs']]:
         """
         Configures the password reset email.
         """
         return pulumi.get(self, "reset_password_email")
 
@@ -1059,14 +1419,26 @@
         return pulumi.get(self, "saml")
 
     @saml.setter
     def saml(self, value: Optional[pulumi.Input['WorkspaceSamlArgs']]):
         pulumi.set(self, "saml", value)
 
     @property
+    @pulumi.getter(name="smsAuthenticationEnabledEmail")
+    def sms_authentication_enabled_email(self) -> Optional[pulumi.Input['WorkspaceSmsAuthenticationEnabledEmailArgs']]:
+        """
+        Configures the SMS authentication enabled email.
+        """
+        return pulumi.get(self, "sms_authentication_enabled_email")
+
+    @sms_authentication_enabled_email.setter
+    def sms_authentication_enabled_email(self, value: Optional[pulumi.Input['WorkspaceSmsAuthenticationEnabledEmailArgs']]):
+        pulumi.set(self, "sms_authentication_enabled_email", value)
+
+    @property
     @pulumi.getter(name="ssoDomainPolicy")
     def sso_domain_policy(self) -> Optional[pulumi.Input['WorkspaceSsoDomainPolicyArgs']]:
         """
         Configures how SSO domains are validated.
         """
         return pulumi.get(self, "sso_domain_policy")
 
@@ -1083,14 +1455,26 @@
         return pulumi.get(self, "sso_multi_tenant_policy")
 
     @sso_multi_tenant_policy.setter
     def sso_multi_tenant_policy(self, value: Optional[pulumi.Input['WorkspaceSsoMultiTenantPolicyArgs']]):
         pulumi.set(self, "sso_multi_tenant_policy", value)
 
     @property
+    @pulumi.getter(name="suspiciousIpEmail")
+    def suspicious_ip_email(self) -> Optional[pulumi.Input['WorkspaceSuspiciousIpEmailArgs']]:
+        """
+        Configures the suspicious IP email.
+        """
+        return pulumi.get(self, "suspicious_ip_email")
+
+    @suspicious_ip_email.setter
+    def suspicious_ip_email(self, value: Optional[pulumi.Input['WorkspaceSuspiciousIpEmailArgs']]):
+        pulumi.set(self, "suspicious_ip_email", value)
+
+    @property
     @pulumi.getter(name="userActivationEmail")
     def user_activation_email(self) -> Optional[pulumi.Input['WorkspaceUserActivationEmailArgs']]:
         """
         Configures the user activation email.
         """
         return pulumi.get(self, "user_activation_email")
 
@@ -1128,84 +1512,108 @@
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  admin_portal: Optional[pulumi.Input[pulumi.InputType['WorkspaceAdminPortalArgs']]] = None,
                  allowed_origins: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  auth_policy: Optional[pulumi.Input[pulumi.InputType['WorkspaceAuthPolicyArgs']]] = None,
                  backend_stack: Optional[pulumi.Input[str]] = None,
+                 bot_detection_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceBotDetectionEmailArgs']]] = None,
+                 brute_force_protection_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceBruteForceProtectionEmailArgs']]] = None,
                  bulk_tenants_invites_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceBulkTenantsInvitesEmailArgs']]] = None,
                  captcha_policy: Optional[pulumi.Input[pulumi.InputType['WorkspaceCaptchaPolicyArgs']]] = None,
                  country: Optional[pulumi.Input[str]] = None,
                  custom_domain: Optional[pulumi.Input[str]] = None,
+                 email_verification_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceEmailVerificationEmailArgs']]] = None,
                  facebook_social_login: Optional[pulumi.Input[pulumi.InputType['WorkspaceFacebookSocialLoginArgs']]] = None,
                  frontegg_domain: Optional[pulumi.Input[str]] = None,
                  frontend_stack: Optional[pulumi.Input[str]] = None,
                  github_social_login: Optional[pulumi.Input[pulumi.InputType['WorkspaceGithubSocialLoginArgs']]] = None,
                  google_social_login: Optional[pulumi.Input[pulumi.InputType['WorkspaceGoogleSocialLoginArgs']]] = None,
                  hosted_login: Optional[pulumi.Input[pulumi.InputType['WorkspaceHostedLoginArgs']]] = None,
+                 impossible_travel_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceImpossibleTravelEmailArgs']]] = None,
                  lockout_policy: Optional[pulumi.Input[pulumi.InputType['WorkspaceLockoutPolicyArgs']]] = None,
                  magic_code_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceMagicCodeEmailArgs']]] = None,
                  magic_link_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceMagicLinkEmailArgs']]] = None,
                  mfa_authentication_app: Optional[pulumi.Input[pulumi.InputType['WorkspaceMfaAuthenticationAppArgs']]] = None,
+                 mfa_enroll_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceMfaEnrollEmailArgs']]] = None,
+                 mfa_otc_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceMfaOtcEmailArgs']]] = None,
                  mfa_policy: Optional[pulumi.Input[pulumi.InputType['WorkspaceMfaPolicyArgs']]] = None,
+                 mfa_recovery_code_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceMfaRecoveryCodeEmailArgs']]] = None,
+                 mfa_unenroll_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceMfaUnenrollEmailArgs']]] = None,
                  microsoft_social_login: Optional[pulumi.Input[pulumi.InputType['WorkspaceMicrosoftSocialLoginArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  new_device_connected_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceNewDeviceConnectedEmailArgs']]] = None,
+                 new_mfa_method_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceNewMfaMethodEmailArgs']]] = None,
                  oidc: Optional[pulumi.Input[pulumi.InputType['WorkspaceOidcArgs']]] = None,
                  open_saas_installed: Optional[pulumi.Input[bool]] = None,
                  password_policy: Optional[pulumi.Input[pulumi.InputType['WorkspacePasswordPolicyArgs']]] = None,
                  pwned_password_email: Optional[pulumi.Input[pulumi.InputType['WorkspacePwnedPasswordEmailArgs']]] = None,
+                 remove_mfa_method_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceRemoveMfaMethodEmailArgs']]] = None,
                  reset_password_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceResetPasswordEmailArgs']]] = None,
                  reset_phone_number_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceResetPhoneNumberEmailArgs']]] = None,
                  saml: Optional[pulumi.Input[pulumi.InputType['WorkspaceSamlArgs']]] = None,
+                 sms_authentication_enabled_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceSmsAuthenticationEnabledEmailArgs']]] = None,
                  sso_domain_policy: Optional[pulumi.Input[pulumi.InputType['WorkspaceSsoDomainPolicyArgs']]] = None,
                  sso_multi_tenant_policy: Optional[pulumi.Input[pulumi.InputType['WorkspaceSsoMultiTenantPolicyArgs']]] = None,
+                 suspicious_ip_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceSuspiciousIpEmailArgs']]] = None,
                  user_activation_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceUserActivationEmailArgs']]] = None,
                  user_invitation_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceUserInvitationEmailArgs']]] = None,
                  user_used_invitation_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceUserUsedInvitationEmailArgs']]] = None,
                  __props__=None):
         """
         Create a Workspace resource with the given unique name, props, and options.
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['WorkspaceAdminPortalArgs']] admin_portal: Configures the admin portal.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_origins: The origins that are allowed to access the workspace. This parameter controls the value of the "Origin" header for API
                responses.
         :param pulumi.Input[pulumi.InputType['WorkspaceAuthPolicyArgs']] auth_policy: Configures the general authentication policy.
         :param pulumi.Input[str] backend_stack: The backend stack of the application associated with the workspace.
+        :param pulumi.Input[pulumi.InputType['WorkspaceBotDetectionEmailArgs']] bot_detection_email: Configures the bot detection email.
+        :param pulumi.Input[pulumi.InputType['WorkspaceBruteForceProtectionEmailArgs']] brute_force_protection_email: Configures the brute force protection email.
         :param pulumi.Input[pulumi.InputType['WorkspaceBulkTenantsInvitesEmailArgs']] bulk_tenants_invites_email: Configures the bulk tenants invite email.
         :param pulumi.Input[pulumi.InputType['WorkspaceCaptchaPolicyArgs']] captcha_policy: Configures the CAPTCHA policy in the signup form.
         :param pulumi.Input[str] country: The country associated with the workspace.
         :param pulumi.Input[str] custom_domain: A custom domain at which Frontegg services will be reachable. You must configure a CNAME record for this domain that
                points to "ssl.frontegg.com" (or "ssl.<your-region>.frontegg.com") and a TXT record for domain-challenge.<custom_domain>
                that points to your client ID before setting this field.
+        :param pulumi.Input[pulumi.InputType['WorkspaceEmailVerificationEmailArgs']] email_verification_email: Configures the verification email.
         :param pulumi.Input[pulumi.InputType['WorkspaceFacebookSocialLoginArgs']] facebook_social_login: Configures social login with Facebook.
         :param pulumi.Input[str] frontegg_domain: The domain at which the Frontegg API is served for this workspace. The domain must end with ".frontegg.com" or
                ".us.frontegg.com".
         :param pulumi.Input[str] frontend_stack: The frontend stack of the application associated with the worksapce.
         :param pulumi.Input[pulumi.InputType['WorkspaceGithubSocialLoginArgs']] github_social_login: Configures social login with GitHub.
         :param pulumi.Input[pulumi.InputType['WorkspaceGoogleSocialLoginArgs']] google_social_login: Configures social login with Google.
         :param pulumi.Input[pulumi.InputType['WorkspaceHostedLoginArgs']] hosted_login: Configures Frontegg-hosted OAuth login.
+        :param pulumi.Input[pulumi.InputType['WorkspaceImpossibleTravelEmailArgs']] impossible_travel_email: Configures the impossible travel email.
         :param pulumi.Input[pulumi.InputType['WorkspaceLockoutPolicyArgs']] lockout_policy: Configures the user lockout policy.
         :param pulumi.Input[pulumi.InputType['WorkspaceMagicCodeEmailArgs']] magic_code_email: Configures the one time code email.
         :param pulumi.Input[pulumi.InputType['WorkspaceMagicLinkEmailArgs']] magic_link_email: Configures the magic link email.
         :param pulumi.Input[pulumi.InputType['WorkspaceMfaAuthenticationAppArgs']] mfa_authentication_app: Configures the multi-factor authentication (MFA) via an authentication app.
+        :param pulumi.Input[pulumi.InputType['WorkspaceMfaEnrollEmailArgs']] mfa_enroll_email: Configures the MFA enroll email.
+        :param pulumi.Input[pulumi.InputType['WorkspaceMfaOtcEmailArgs']] mfa_otc_email: Configures the account challenge with code email.
         :param pulumi.Input[pulumi.InputType['WorkspaceMfaPolicyArgs']] mfa_policy: Configures the multi-factor authentication (MFA) policy.
+        :param pulumi.Input[pulumi.InputType['WorkspaceMfaRecoveryCodeEmailArgs']] mfa_recovery_code_email: Configures the MFA recovery code email.
+        :param pulumi.Input[pulumi.InputType['WorkspaceMfaUnenrollEmailArgs']] mfa_unenroll_email: Configures the MFA unenroll email.
         :param pulumi.Input[pulumi.InputType['WorkspaceMicrosoftSocialLoginArgs']] microsoft_social_login: Configures social login with Google.
         :param pulumi.Input[str] name: The name of the workspace.
         :param pulumi.Input[pulumi.InputType['WorkspaceNewDeviceConnectedEmailArgs']] new_device_connected_email: Configures the new device connected email.
+        :param pulumi.Input[pulumi.InputType['WorkspaceNewMfaMethodEmailArgs']] new_mfa_method_email: Configures the new MFA method email.
         :param pulumi.Input[pulumi.InputType['WorkspaceOidcArgs']] oidc: Configures SSO via OIDC.
         :param pulumi.Input[bool] open_saas_installed: Whether the application associated with the workspace has OpenSaaS installed.
         :param pulumi.Input[pulumi.InputType['WorkspacePasswordPolicyArgs']] password_policy: Configures the password policy.
         :param pulumi.Input[pulumi.InputType['WorkspacePwnedPasswordEmailArgs']] pwned_password_email: Configures the pwned password email.
+        :param pulumi.Input[pulumi.InputType['WorkspaceRemoveMfaMethodEmailArgs']] remove_mfa_method_email: Configures the remove MFA method email.
         :param pulumi.Input[pulumi.InputType['WorkspaceResetPasswordEmailArgs']] reset_password_email: Configures the password reset email.
         :param pulumi.Input[pulumi.InputType['WorkspaceResetPhoneNumberEmailArgs']] reset_phone_number_email: Configures the reset phone number email.
         :param pulumi.Input[pulumi.InputType['WorkspaceSamlArgs']] saml: Configures SSO via SAML.
+        :param pulumi.Input[pulumi.InputType['WorkspaceSmsAuthenticationEnabledEmailArgs']] sms_authentication_enabled_email: Configures the SMS authentication enabled email.
         :param pulumi.Input[pulumi.InputType['WorkspaceSsoDomainPolicyArgs']] sso_domain_policy: Configures how SSO domains are validated.
         :param pulumi.Input[pulumi.InputType['WorkspaceSsoMultiTenantPolicyArgs']] sso_multi_tenant_policy: Configures how multiple tenants can claim the same SSO domain.
+        :param pulumi.Input[pulumi.InputType['WorkspaceSuspiciousIpEmailArgs']] suspicious_ip_email: Configures the suspicious IP email.
         :param pulumi.Input[pulumi.InputType['WorkspaceUserActivationEmailArgs']] user_activation_email: Configures the user activation email.
         :param pulumi.Input[pulumi.InputType['WorkspaceUserInvitationEmailArgs']] user_invitation_email: Configures the user invitation email.
         :param pulumi.Input[pulumi.InputType['WorkspaceUserUsedInvitationEmailArgs']] user_used_invitation_email: Configures the user used invitation email.
         """
         ...
     @overload
     def __init__(__self__,
@@ -1229,41 +1637,53 @@
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  admin_portal: Optional[pulumi.Input[pulumi.InputType['WorkspaceAdminPortalArgs']]] = None,
                  allowed_origins: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  auth_policy: Optional[pulumi.Input[pulumi.InputType['WorkspaceAuthPolicyArgs']]] = None,
                  backend_stack: Optional[pulumi.Input[str]] = None,
+                 bot_detection_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceBotDetectionEmailArgs']]] = None,
+                 brute_force_protection_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceBruteForceProtectionEmailArgs']]] = None,
                  bulk_tenants_invites_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceBulkTenantsInvitesEmailArgs']]] = None,
                  captcha_policy: Optional[pulumi.Input[pulumi.InputType['WorkspaceCaptchaPolicyArgs']]] = None,
                  country: Optional[pulumi.Input[str]] = None,
                  custom_domain: Optional[pulumi.Input[str]] = None,
+                 email_verification_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceEmailVerificationEmailArgs']]] = None,
                  facebook_social_login: Optional[pulumi.Input[pulumi.InputType['WorkspaceFacebookSocialLoginArgs']]] = None,
                  frontegg_domain: Optional[pulumi.Input[str]] = None,
                  frontend_stack: Optional[pulumi.Input[str]] = None,
                  github_social_login: Optional[pulumi.Input[pulumi.InputType['WorkspaceGithubSocialLoginArgs']]] = None,
                  google_social_login: Optional[pulumi.Input[pulumi.InputType['WorkspaceGoogleSocialLoginArgs']]] = None,
                  hosted_login: Optional[pulumi.Input[pulumi.InputType['WorkspaceHostedLoginArgs']]] = None,
+                 impossible_travel_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceImpossibleTravelEmailArgs']]] = None,
                  lockout_policy: Optional[pulumi.Input[pulumi.InputType['WorkspaceLockoutPolicyArgs']]] = None,
                  magic_code_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceMagicCodeEmailArgs']]] = None,
                  magic_link_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceMagicLinkEmailArgs']]] = None,
                  mfa_authentication_app: Optional[pulumi.Input[pulumi.InputType['WorkspaceMfaAuthenticationAppArgs']]] = None,
+                 mfa_enroll_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceMfaEnrollEmailArgs']]] = None,
+                 mfa_otc_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceMfaOtcEmailArgs']]] = None,
                  mfa_policy: Optional[pulumi.Input[pulumi.InputType['WorkspaceMfaPolicyArgs']]] = None,
+                 mfa_recovery_code_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceMfaRecoveryCodeEmailArgs']]] = None,
+                 mfa_unenroll_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceMfaUnenrollEmailArgs']]] = None,
                  microsoft_social_login: Optional[pulumi.Input[pulumi.InputType['WorkspaceMicrosoftSocialLoginArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  new_device_connected_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceNewDeviceConnectedEmailArgs']]] = None,
+                 new_mfa_method_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceNewMfaMethodEmailArgs']]] = None,
                  oidc: Optional[pulumi.Input[pulumi.InputType['WorkspaceOidcArgs']]] = None,
                  open_saas_installed: Optional[pulumi.Input[bool]] = None,
                  password_policy: Optional[pulumi.Input[pulumi.InputType['WorkspacePasswordPolicyArgs']]] = None,
                  pwned_password_email: Optional[pulumi.Input[pulumi.InputType['WorkspacePwnedPasswordEmailArgs']]] = None,
+                 remove_mfa_method_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceRemoveMfaMethodEmailArgs']]] = None,
                  reset_password_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceResetPasswordEmailArgs']]] = None,
                  reset_phone_number_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceResetPhoneNumberEmailArgs']]] = None,
                  saml: Optional[pulumi.Input[pulumi.InputType['WorkspaceSamlArgs']]] = None,
+                 sms_authentication_enabled_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceSmsAuthenticationEnabledEmailArgs']]] = None,
                  sso_domain_policy: Optional[pulumi.Input[pulumi.InputType['WorkspaceSsoDomainPolicyArgs']]] = None,
                  sso_multi_tenant_policy: Optional[pulumi.Input[pulumi.InputType['WorkspaceSsoMultiTenantPolicyArgs']]] = None,
+                 suspicious_ip_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceSuspiciousIpEmailArgs']]] = None,
                  user_activation_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceUserActivationEmailArgs']]] = None,
                  user_invitation_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceUserInvitationEmailArgs']]] = None,
                  user_used_invitation_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceUserUsedInvitationEmailArgs']]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
@@ -1280,53 +1700,65 @@
             __props__.__dict__["allowed_origins"] = allowed_origins
             if auth_policy is None and not opts.urn:
                 raise TypeError("Missing required property 'auth_policy'")
             __props__.__dict__["auth_policy"] = auth_policy
             if backend_stack is None and not opts.urn:
                 raise TypeError("Missing required property 'backend_stack'")
             __props__.__dict__["backend_stack"] = backend_stack
+            __props__.__dict__["bot_detection_email"] = bot_detection_email
+            __props__.__dict__["brute_force_protection_email"] = brute_force_protection_email
             __props__.__dict__["bulk_tenants_invites_email"] = bulk_tenants_invites_email
             __props__.__dict__["captcha_policy"] = captcha_policy
             if country is None and not opts.urn:
                 raise TypeError("Missing required property 'country'")
             __props__.__dict__["country"] = country
             __props__.__dict__["custom_domain"] = custom_domain
+            __props__.__dict__["email_verification_email"] = email_verification_email
             __props__.__dict__["facebook_social_login"] = facebook_social_login
             if frontegg_domain is None and not opts.urn:
                 raise TypeError("Missing required property 'frontegg_domain'")
             __props__.__dict__["frontegg_domain"] = frontegg_domain
             if frontend_stack is None and not opts.urn:
                 raise TypeError("Missing required property 'frontend_stack'")
             __props__.__dict__["frontend_stack"] = frontend_stack
             __props__.__dict__["github_social_login"] = github_social_login
             __props__.__dict__["google_social_login"] = google_social_login
             __props__.__dict__["hosted_login"] = hosted_login
+            __props__.__dict__["impossible_travel_email"] = impossible_travel_email
             __props__.__dict__["lockout_policy"] = lockout_policy
             __props__.__dict__["magic_code_email"] = magic_code_email
             __props__.__dict__["magic_link_email"] = magic_link_email
             __props__.__dict__["mfa_authentication_app"] = mfa_authentication_app
+            __props__.__dict__["mfa_enroll_email"] = mfa_enroll_email
+            __props__.__dict__["mfa_otc_email"] = mfa_otc_email
             if mfa_policy is None and not opts.urn:
                 raise TypeError("Missing required property 'mfa_policy'")
             __props__.__dict__["mfa_policy"] = mfa_policy
+            __props__.__dict__["mfa_recovery_code_email"] = mfa_recovery_code_email
+            __props__.__dict__["mfa_unenroll_email"] = mfa_unenroll_email
             __props__.__dict__["microsoft_social_login"] = microsoft_social_login
             __props__.__dict__["name"] = name
             __props__.__dict__["new_device_connected_email"] = new_device_connected_email
+            __props__.__dict__["new_mfa_method_email"] = new_mfa_method_email
             __props__.__dict__["oidc"] = oidc
             if open_saas_installed is None and not opts.urn:
                 raise TypeError("Missing required property 'open_saas_installed'")
             __props__.__dict__["open_saas_installed"] = open_saas_installed
             if password_policy is None and not opts.urn:
                 raise TypeError("Missing required property 'password_policy'")
             __props__.__dict__["password_policy"] = password_policy
             __props__.__dict__["pwned_password_email"] = pwned_password_email
+            __props__.__dict__["remove_mfa_method_email"] = remove_mfa_method_email
             __props__.__dict__["reset_password_email"] = reset_password_email
             __props__.__dict__["reset_phone_number_email"] = reset_phone_number_email
             __props__.__dict__["saml"] = saml
+            __props__.__dict__["sms_authentication_enabled_email"] = sms_authentication_enabled_email
             __props__.__dict__["sso_domain_policy"] = sso_domain_policy
             __props__.__dict__["sso_multi_tenant_policy"] = sso_multi_tenant_policy
+            __props__.__dict__["suspicious_ip_email"] = suspicious_ip_email
             __props__.__dict__["user_activation_email"] = user_activation_email
             __props__.__dict__["user_invitation_email"] = user_invitation_email
             __props__.__dict__["user_used_invitation_email"] = user_used_invitation_email
         super(Workspace, __self__).__init__(
             'frontegg:index/workspace:Workspace',
             resource_name,
             __props__,
@@ -1336,41 +1768,53 @@
     def get(resource_name: str,
             id: pulumi.Input[str],
             opts: Optional[pulumi.ResourceOptions] = None,
             admin_portal: Optional[pulumi.Input[pulumi.InputType['WorkspaceAdminPortalArgs']]] = None,
             allowed_origins: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             auth_policy: Optional[pulumi.Input[pulumi.InputType['WorkspaceAuthPolicyArgs']]] = None,
             backend_stack: Optional[pulumi.Input[str]] = None,
+            bot_detection_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceBotDetectionEmailArgs']]] = None,
+            brute_force_protection_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceBruteForceProtectionEmailArgs']]] = None,
             bulk_tenants_invites_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceBulkTenantsInvitesEmailArgs']]] = None,
             captcha_policy: Optional[pulumi.Input[pulumi.InputType['WorkspaceCaptchaPolicyArgs']]] = None,
             country: Optional[pulumi.Input[str]] = None,
             custom_domain: Optional[pulumi.Input[str]] = None,
+            email_verification_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceEmailVerificationEmailArgs']]] = None,
             facebook_social_login: Optional[pulumi.Input[pulumi.InputType['WorkspaceFacebookSocialLoginArgs']]] = None,
             frontegg_domain: Optional[pulumi.Input[str]] = None,
             frontend_stack: Optional[pulumi.Input[str]] = None,
             github_social_login: Optional[pulumi.Input[pulumi.InputType['WorkspaceGithubSocialLoginArgs']]] = None,
             google_social_login: Optional[pulumi.Input[pulumi.InputType['WorkspaceGoogleSocialLoginArgs']]] = None,
             hosted_login: Optional[pulumi.Input[pulumi.InputType['WorkspaceHostedLoginArgs']]] = None,
+            impossible_travel_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceImpossibleTravelEmailArgs']]] = None,
             lockout_policy: Optional[pulumi.Input[pulumi.InputType['WorkspaceLockoutPolicyArgs']]] = None,
             magic_code_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceMagicCodeEmailArgs']]] = None,
             magic_link_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceMagicLinkEmailArgs']]] = None,
             mfa_authentication_app: Optional[pulumi.Input[pulumi.InputType['WorkspaceMfaAuthenticationAppArgs']]] = None,
+            mfa_enroll_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceMfaEnrollEmailArgs']]] = None,
+            mfa_otc_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceMfaOtcEmailArgs']]] = None,
             mfa_policy: Optional[pulumi.Input[pulumi.InputType['WorkspaceMfaPolicyArgs']]] = None,
+            mfa_recovery_code_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceMfaRecoveryCodeEmailArgs']]] = None,
+            mfa_unenroll_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceMfaUnenrollEmailArgs']]] = None,
             microsoft_social_login: Optional[pulumi.Input[pulumi.InputType['WorkspaceMicrosoftSocialLoginArgs']]] = None,
             name: Optional[pulumi.Input[str]] = None,
             new_device_connected_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceNewDeviceConnectedEmailArgs']]] = None,
+            new_mfa_method_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceNewMfaMethodEmailArgs']]] = None,
             oidc: Optional[pulumi.Input[pulumi.InputType['WorkspaceOidcArgs']]] = None,
             open_saas_installed: Optional[pulumi.Input[bool]] = None,
             password_policy: Optional[pulumi.Input[pulumi.InputType['WorkspacePasswordPolicyArgs']]] = None,
             pwned_password_email: Optional[pulumi.Input[pulumi.InputType['WorkspacePwnedPasswordEmailArgs']]] = None,
+            remove_mfa_method_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceRemoveMfaMethodEmailArgs']]] = None,
             reset_password_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceResetPasswordEmailArgs']]] = None,
             reset_phone_number_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceResetPhoneNumberEmailArgs']]] = None,
             saml: Optional[pulumi.Input[pulumi.InputType['WorkspaceSamlArgs']]] = None,
+            sms_authentication_enabled_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceSmsAuthenticationEnabledEmailArgs']]] = None,
             sso_domain_policy: Optional[pulumi.Input[pulumi.InputType['WorkspaceSsoDomainPolicyArgs']]] = None,
             sso_multi_tenant_policy: Optional[pulumi.Input[pulumi.InputType['WorkspaceSsoMultiTenantPolicyArgs']]] = None,
+            suspicious_ip_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceSuspiciousIpEmailArgs']]] = None,
             user_activation_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceUserActivationEmailArgs']]] = None,
             user_invitation_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceUserInvitationEmailArgs']]] = None,
             user_used_invitation_email: Optional[pulumi.Input[pulumi.InputType['WorkspaceUserUsedInvitationEmailArgs']]] = None) -> 'Workspace':
         """
         Get an existing Workspace resource's state with the given name, id, and optional extra
         properties used to qualify the lookup.
 
@@ -1378,83 +1822,107 @@
         :param pulumi.Input[str] id: The unique provider ID of the resource to lookup.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[pulumi.InputType['WorkspaceAdminPortalArgs']] admin_portal: Configures the admin portal.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] allowed_origins: The origins that are allowed to access the workspace. This parameter controls the value of the "Origin" header for API
                responses.
         :param pulumi.Input[pulumi.InputType['WorkspaceAuthPolicyArgs']] auth_policy: Configures the general authentication policy.
         :param pulumi.Input[str] backend_stack: The backend stack of the application associated with the workspace.
+        :param pulumi.Input[pulumi.InputType['WorkspaceBotDetectionEmailArgs']] bot_detection_email: Configures the bot detection email.
+        :param pulumi.Input[pulumi.InputType['WorkspaceBruteForceProtectionEmailArgs']] brute_force_protection_email: Configures the brute force protection email.
         :param pulumi.Input[pulumi.InputType['WorkspaceBulkTenantsInvitesEmailArgs']] bulk_tenants_invites_email: Configures the bulk tenants invite email.
         :param pulumi.Input[pulumi.InputType['WorkspaceCaptchaPolicyArgs']] captcha_policy: Configures the CAPTCHA policy in the signup form.
         :param pulumi.Input[str] country: The country associated with the workspace.
         :param pulumi.Input[str] custom_domain: A custom domain at which Frontegg services will be reachable. You must configure a CNAME record for this domain that
                points to "ssl.frontegg.com" (or "ssl.<your-region>.frontegg.com") and a TXT record for domain-challenge.<custom_domain>
                that points to your client ID before setting this field.
+        :param pulumi.Input[pulumi.InputType['WorkspaceEmailVerificationEmailArgs']] email_verification_email: Configures the verification email.
         :param pulumi.Input[pulumi.InputType['WorkspaceFacebookSocialLoginArgs']] facebook_social_login: Configures social login with Facebook.
         :param pulumi.Input[str] frontegg_domain: The domain at which the Frontegg API is served for this workspace. The domain must end with ".frontegg.com" or
                ".us.frontegg.com".
         :param pulumi.Input[str] frontend_stack: The frontend stack of the application associated with the worksapce.
         :param pulumi.Input[pulumi.InputType['WorkspaceGithubSocialLoginArgs']] github_social_login: Configures social login with GitHub.
         :param pulumi.Input[pulumi.InputType['WorkspaceGoogleSocialLoginArgs']] google_social_login: Configures social login with Google.
         :param pulumi.Input[pulumi.InputType['WorkspaceHostedLoginArgs']] hosted_login: Configures Frontegg-hosted OAuth login.
+        :param pulumi.Input[pulumi.InputType['WorkspaceImpossibleTravelEmailArgs']] impossible_travel_email: Configures the impossible travel email.
         :param pulumi.Input[pulumi.InputType['WorkspaceLockoutPolicyArgs']] lockout_policy: Configures the user lockout policy.
         :param pulumi.Input[pulumi.InputType['WorkspaceMagicCodeEmailArgs']] magic_code_email: Configures the one time code email.
         :param pulumi.Input[pulumi.InputType['WorkspaceMagicLinkEmailArgs']] magic_link_email: Configures the magic link email.
         :param pulumi.Input[pulumi.InputType['WorkspaceMfaAuthenticationAppArgs']] mfa_authentication_app: Configures the multi-factor authentication (MFA) via an authentication app.
+        :param pulumi.Input[pulumi.InputType['WorkspaceMfaEnrollEmailArgs']] mfa_enroll_email: Configures the MFA enroll email.
+        :param pulumi.Input[pulumi.InputType['WorkspaceMfaOtcEmailArgs']] mfa_otc_email: Configures the account challenge with code email.
         :param pulumi.Input[pulumi.InputType['WorkspaceMfaPolicyArgs']] mfa_policy: Configures the multi-factor authentication (MFA) policy.
+        :param pulumi.Input[pulumi.InputType['WorkspaceMfaRecoveryCodeEmailArgs']] mfa_recovery_code_email: Configures the MFA recovery code email.
+        :param pulumi.Input[pulumi.InputType['WorkspaceMfaUnenrollEmailArgs']] mfa_unenroll_email: Configures the MFA unenroll email.
         :param pulumi.Input[pulumi.InputType['WorkspaceMicrosoftSocialLoginArgs']] microsoft_social_login: Configures social login with Google.
         :param pulumi.Input[str] name: The name of the workspace.
         :param pulumi.Input[pulumi.InputType['WorkspaceNewDeviceConnectedEmailArgs']] new_device_connected_email: Configures the new device connected email.
+        :param pulumi.Input[pulumi.InputType['WorkspaceNewMfaMethodEmailArgs']] new_mfa_method_email: Configures the new MFA method email.
         :param pulumi.Input[pulumi.InputType['WorkspaceOidcArgs']] oidc: Configures SSO via OIDC.
         :param pulumi.Input[bool] open_saas_installed: Whether the application associated with the workspace has OpenSaaS installed.
         :param pulumi.Input[pulumi.InputType['WorkspacePasswordPolicyArgs']] password_policy: Configures the password policy.
         :param pulumi.Input[pulumi.InputType['WorkspacePwnedPasswordEmailArgs']] pwned_password_email: Configures the pwned password email.
+        :param pulumi.Input[pulumi.InputType['WorkspaceRemoveMfaMethodEmailArgs']] remove_mfa_method_email: Configures the remove MFA method email.
         :param pulumi.Input[pulumi.InputType['WorkspaceResetPasswordEmailArgs']] reset_password_email: Configures the password reset email.
         :param pulumi.Input[pulumi.InputType['WorkspaceResetPhoneNumberEmailArgs']] reset_phone_number_email: Configures the reset phone number email.
         :param pulumi.Input[pulumi.InputType['WorkspaceSamlArgs']] saml: Configures SSO via SAML.
+        :param pulumi.Input[pulumi.InputType['WorkspaceSmsAuthenticationEnabledEmailArgs']] sms_authentication_enabled_email: Configures the SMS authentication enabled email.
         :param pulumi.Input[pulumi.InputType['WorkspaceSsoDomainPolicyArgs']] sso_domain_policy: Configures how SSO domains are validated.
         :param pulumi.Input[pulumi.InputType['WorkspaceSsoMultiTenantPolicyArgs']] sso_multi_tenant_policy: Configures how multiple tenants can claim the same SSO domain.
+        :param pulumi.Input[pulumi.InputType['WorkspaceSuspiciousIpEmailArgs']] suspicious_ip_email: Configures the suspicious IP email.
         :param pulumi.Input[pulumi.InputType['WorkspaceUserActivationEmailArgs']] user_activation_email: Configures the user activation email.
         :param pulumi.Input[pulumi.InputType['WorkspaceUserInvitationEmailArgs']] user_invitation_email: Configures the user invitation email.
         :param pulumi.Input[pulumi.InputType['WorkspaceUserUsedInvitationEmailArgs']] user_used_invitation_email: Configures the user used invitation email.
         """
         opts = pulumi.ResourceOptions.merge(opts, pulumi.ResourceOptions(id=id))
 
         __props__ = _WorkspaceState.__new__(_WorkspaceState)
 
         __props__.__dict__["admin_portal"] = admin_portal
         __props__.__dict__["allowed_origins"] = allowed_origins
         __props__.__dict__["auth_policy"] = auth_policy
         __props__.__dict__["backend_stack"] = backend_stack
+        __props__.__dict__["bot_detection_email"] = bot_detection_email
+        __props__.__dict__["brute_force_protection_email"] = brute_force_protection_email
         __props__.__dict__["bulk_tenants_invites_email"] = bulk_tenants_invites_email
         __props__.__dict__["captcha_policy"] = captcha_policy
         __props__.__dict__["country"] = country
         __props__.__dict__["custom_domain"] = custom_domain
+        __props__.__dict__["email_verification_email"] = email_verification_email
         __props__.__dict__["facebook_social_login"] = facebook_social_login
         __props__.__dict__["frontegg_domain"] = frontegg_domain
         __props__.__dict__["frontend_stack"] = frontend_stack
         __props__.__dict__["github_social_login"] = github_social_login
         __props__.__dict__["google_social_login"] = google_social_login
         __props__.__dict__["hosted_login"] = hosted_login
+        __props__.__dict__["impossible_travel_email"] = impossible_travel_email
         __props__.__dict__["lockout_policy"] = lockout_policy
         __props__.__dict__["magic_code_email"] = magic_code_email
         __props__.__dict__["magic_link_email"] = magic_link_email
         __props__.__dict__["mfa_authentication_app"] = mfa_authentication_app
+        __props__.__dict__["mfa_enroll_email"] = mfa_enroll_email
+        __props__.__dict__["mfa_otc_email"] = mfa_otc_email
         __props__.__dict__["mfa_policy"] = mfa_policy
+        __props__.__dict__["mfa_recovery_code_email"] = mfa_recovery_code_email
+        __props__.__dict__["mfa_unenroll_email"] = mfa_unenroll_email
         __props__.__dict__["microsoft_social_login"] = microsoft_social_login
         __props__.__dict__["name"] = name
         __props__.__dict__["new_device_connected_email"] = new_device_connected_email
+        __props__.__dict__["new_mfa_method_email"] = new_mfa_method_email
         __props__.__dict__["oidc"] = oidc
         __props__.__dict__["open_saas_installed"] = open_saas_installed
         __props__.__dict__["password_policy"] = password_policy
         __props__.__dict__["pwned_password_email"] = pwned_password_email
+        __props__.__dict__["remove_mfa_method_email"] = remove_mfa_method_email
         __props__.__dict__["reset_password_email"] = reset_password_email
         __props__.__dict__["reset_phone_number_email"] = reset_phone_number_email
         __props__.__dict__["saml"] = saml
+        __props__.__dict__["sms_authentication_enabled_email"] = sms_authentication_enabled_email
         __props__.__dict__["sso_domain_policy"] = sso_domain_policy
         __props__.__dict__["sso_multi_tenant_policy"] = sso_multi_tenant_policy
+        __props__.__dict__["suspicious_ip_email"] = suspicious_ip_email
         __props__.__dict__["user_activation_email"] = user_activation_email
         __props__.__dict__["user_invitation_email"] = user_invitation_email
         __props__.__dict__["user_used_invitation_email"] = user_used_invitation_email
         return Workspace(resource_name, opts=opts, __props__=__props__)
 
     @property
     @pulumi.getter(name="adminPortal")
@@ -1486,14 +1954,30 @@
     def backend_stack(self) -> pulumi.Output[str]:
         """
         The backend stack of the application associated with the workspace.
         """
         return pulumi.get(self, "backend_stack")
 
     @property
+    @pulumi.getter(name="botDetectionEmail")
+    def bot_detection_email(self) -> pulumi.Output[Optional['outputs.WorkspaceBotDetectionEmail']]:
+        """
+        Configures the bot detection email.
+        """
+        return pulumi.get(self, "bot_detection_email")
+
+    @property
+    @pulumi.getter(name="bruteForceProtectionEmail")
+    def brute_force_protection_email(self) -> pulumi.Output[Optional['outputs.WorkspaceBruteForceProtectionEmail']]:
+        """
+        Configures the brute force protection email.
+        """
+        return pulumi.get(self, "brute_force_protection_email")
+
+    @property
     @pulumi.getter(name="bulkTenantsInvitesEmail")
     def bulk_tenants_invites_email(self) -> pulumi.Output[Optional['outputs.WorkspaceBulkTenantsInvitesEmail']]:
         """
         Configures the bulk tenants invite email.
         """
         return pulumi.get(self, "bulk_tenants_invites_email")
 
@@ -1520,14 +2004,22 @@
         A custom domain at which Frontegg services will be reachable. You must configure a CNAME record for this domain that
         points to "ssl.frontegg.com" (or "ssl.<your-region>.frontegg.com") and a TXT record for domain-challenge.<custom_domain>
         that points to your client ID before setting this field.
         """
         return pulumi.get(self, "custom_domain")
 
     @property
+    @pulumi.getter(name="emailVerificationEmail")
+    def email_verification_email(self) -> pulumi.Output[Optional['outputs.WorkspaceEmailVerificationEmail']]:
+        """
+        Configures the verification email.
+        """
+        return pulumi.get(self, "email_verification_email")
+
+    @property
     @pulumi.getter(name="facebookSocialLogin")
     def facebook_social_login(self) -> pulumi.Output[Optional['outputs.WorkspaceFacebookSocialLogin']]:
         """
         Configures social login with Facebook.
         """
         return pulumi.get(self, "facebook_social_login")
 
@@ -1569,14 +2061,22 @@
     def hosted_login(self) -> pulumi.Output[Optional['outputs.WorkspaceHostedLogin']]:
         """
         Configures Frontegg-hosted OAuth login.
         """
         return pulumi.get(self, "hosted_login")
 
     @property
+    @pulumi.getter(name="impossibleTravelEmail")
+    def impossible_travel_email(self) -> pulumi.Output[Optional['outputs.WorkspaceImpossibleTravelEmail']]:
+        """
+        Configures the impossible travel email.
+        """
+        return pulumi.get(self, "impossible_travel_email")
+
+    @property
     @pulumi.getter(name="lockoutPolicy")
     def lockout_policy(self) -> pulumi.Output[Optional['outputs.WorkspaceLockoutPolicy']]:
         """
         Configures the user lockout policy.
         """
         return pulumi.get(self, "lockout_policy")
 
@@ -1601,22 +2101,54 @@
     def mfa_authentication_app(self) -> pulumi.Output[Optional['outputs.WorkspaceMfaAuthenticationApp']]:
         """
         Configures the multi-factor authentication (MFA) via an authentication app.
         """
         return pulumi.get(self, "mfa_authentication_app")
 
     @property
+    @pulumi.getter(name="mfaEnrollEmail")
+    def mfa_enroll_email(self) -> pulumi.Output[Optional['outputs.WorkspaceMfaEnrollEmail']]:
+        """
+        Configures the MFA enroll email.
+        """
+        return pulumi.get(self, "mfa_enroll_email")
+
+    @property
+    @pulumi.getter(name="mfaOtcEmail")
+    def mfa_otc_email(self) -> pulumi.Output[Optional['outputs.WorkspaceMfaOtcEmail']]:
+        """
+        Configures the account challenge with code email.
+        """
+        return pulumi.get(self, "mfa_otc_email")
+
+    @property
     @pulumi.getter(name="mfaPolicy")
     def mfa_policy(self) -> pulumi.Output['outputs.WorkspaceMfaPolicy']:
         """
         Configures the multi-factor authentication (MFA) policy.
         """
         return pulumi.get(self, "mfa_policy")
 
     @property
+    @pulumi.getter(name="mfaRecoveryCodeEmail")
+    def mfa_recovery_code_email(self) -> pulumi.Output[Optional['outputs.WorkspaceMfaRecoveryCodeEmail']]:
+        """
+        Configures the MFA recovery code email.
+        """
+        return pulumi.get(self, "mfa_recovery_code_email")
+
+    @property
+    @pulumi.getter(name="mfaUnenrollEmail")
+    def mfa_unenroll_email(self) -> pulumi.Output[Optional['outputs.WorkspaceMfaUnenrollEmail']]:
+        """
+        Configures the MFA unenroll email.
+        """
+        return pulumi.get(self, "mfa_unenroll_email")
+
+    @property
     @pulumi.getter(name="microsoftSocialLogin")
     def microsoft_social_login(self) -> pulumi.Output[Optional['outputs.WorkspaceMicrosoftSocialLogin']]:
         """
         Configures social login with Google.
         """
         return pulumi.get(self, "microsoft_social_login")
 
@@ -1633,14 +2165,22 @@
     def new_device_connected_email(self) -> pulumi.Output[Optional['outputs.WorkspaceNewDeviceConnectedEmail']]:
         """
         Configures the new device connected email.
         """
         return pulumi.get(self, "new_device_connected_email")
 
     @property
+    @pulumi.getter(name="newMfaMethodEmail")
+    def new_mfa_method_email(self) -> pulumi.Output[Optional['outputs.WorkspaceNewMfaMethodEmail']]:
+        """
+        Configures the new MFA method email.
+        """
+        return pulumi.get(self, "new_mfa_method_email")
+
+    @property
     @pulumi.getter
     def oidc(self) -> pulumi.Output[Optional['outputs.WorkspaceOidc']]:
         """
         Configures SSO via OIDC.
         """
         return pulumi.get(self, "oidc")
 
@@ -1665,14 +2205,22 @@
     def pwned_password_email(self) -> pulumi.Output[Optional['outputs.WorkspacePwnedPasswordEmail']]:
         """
         Configures the pwned password email.
         """
         return pulumi.get(self, "pwned_password_email")
 
     @property
+    @pulumi.getter(name="removeMfaMethodEmail")
+    def remove_mfa_method_email(self) -> pulumi.Output[Optional['outputs.WorkspaceRemoveMfaMethodEmail']]:
+        """
+        Configures the remove MFA method email.
+        """
+        return pulumi.get(self, "remove_mfa_method_email")
+
+    @property
     @pulumi.getter(name="resetPasswordEmail")
     def reset_password_email(self) -> pulumi.Output[Optional['outputs.WorkspaceResetPasswordEmail']]:
         """
         Configures the password reset email.
         """
         return pulumi.get(self, "reset_password_email")
 
@@ -1689,14 +2237,22 @@
     def saml(self) -> pulumi.Output[Optional['outputs.WorkspaceSaml']]:
         """
         Configures SSO via SAML.
         """
         return pulumi.get(self, "saml")
 
     @property
+    @pulumi.getter(name="smsAuthenticationEnabledEmail")
+    def sms_authentication_enabled_email(self) -> pulumi.Output[Optional['outputs.WorkspaceSmsAuthenticationEnabledEmail']]:
+        """
+        Configures the SMS authentication enabled email.
+        """
+        return pulumi.get(self, "sms_authentication_enabled_email")
+
+    @property
     @pulumi.getter(name="ssoDomainPolicy")
     def sso_domain_policy(self) -> pulumi.Output[Optional['outputs.WorkspaceSsoDomainPolicy']]:
         """
         Configures how SSO domains are validated.
         """
         return pulumi.get(self, "sso_domain_policy")
 
@@ -1705,14 +2261,22 @@
     def sso_multi_tenant_policy(self) -> pulumi.Output[Optional['outputs.WorkspaceSsoMultiTenantPolicy']]:
         """
         Configures how multiple tenants can claim the same SSO domain.
         """
         return pulumi.get(self, "sso_multi_tenant_policy")
 
     @property
+    @pulumi.getter(name="suspiciousIpEmail")
+    def suspicious_ip_email(self) -> pulumi.Output[Optional['outputs.WorkspaceSuspiciousIpEmail']]:
+        """
+        Configures the suspicious IP email.
+        """
+        return pulumi.get(self, "suspicious_ip_email")
+
+    @property
     @pulumi.getter(name="userActivationEmail")
     def user_activation_email(self) -> pulumi.Output[Optional['outputs.WorkspaceUserActivationEmail']]:
         """
         Configures the user activation email.
         """
         return pulumi.get(self, "user_activation_email")
```

### Comparing `pulumi_frontegg-0.2.34/pulumi_frontegg.egg-info/PKG-INFO` & `pulumi_frontegg-0.2.35/pulumi_frontegg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-frontegg
-Version: 0.2.34
+Version: 0.2.35
 Summary: A Pulumi package for creating and managing Frontegg resources.
 Home-page: https://github.com/MaterializeInc/pulumi-frontegg
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-frontegg
 Keywords: pulumi frontegg
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_frontegg-0.2.34/pulumi_frontegg.egg-info/SOURCES.txt` & `pulumi_frontegg-0.2.35/pulumi_frontegg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_frontegg-0.2.34/setup.py` & `pulumi_frontegg-0.2.35/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = '0.2.34'
+VERSION = '0.2.35'
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "frontegg Pulumi Package - Development Version"
```

