# Comparing `tmp/gdmty-drf-firebase-auth-24.1.1.tar.gz` & `tmp/gdmty-drf-firebase-auth-24.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gdmty-drf-firebase-auth-24.1.1.tar", last modified: Sun Jan 28 01:43:59 2024, max compression
+gzip compressed data, was "gdmty-drf-firebase-auth-24.4.0.tar", last modified: Wed Apr  3 20:07:34 2024, max compression
```

## Comparing `gdmty-drf-firebase-auth-24.1.1.tar` & `gdmty-drf-firebase-auth-24.4.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 niji       (501) staff       (20)        0 2024-01-28 01:43:59.342733 gdmty-drf-firebase-auth-24.1.1/
--rw-r--r--   0 niji       (501) staff       (20)    11351 2024-01-28 00:48:44.000000 gdmty-drf-firebase-auth-24.1.1/LICENSE
--rw-r--r--   0 niji       (501) staff       (20)       48 2024-01-28 00:48:44.000000 gdmty-drf-firebase-auth-24.1.1/MANIFEST.in
--rw-r--r--   0 niji       (501) staff       (20)    19583 2024-01-28 01:43:59.342340 gdmty-drf-firebase-auth-24.1.1/PKG-INFO
--rw-r--r--   0 niji       (501) staff       (20)     5356 2024-01-28 01:02:03.000000 gdmty-drf-firebase-auth-24.1.1/README.md
--rw-r--r--   0 niji       (501) staff       (20)     1629 2024-01-28 01:43:42.000000 gdmty-drf-firebase-auth-24.1.1/pyproject.toml
--rw-r--r--   0 niji       (501) staff       (20)       38 2024-01-28 01:43:59.342794 gdmty-drf-firebase-auth-24.1.1/setup.cfg
-drwxr-xr-x   0 niji       (501) staff       (20)        0 2024-01-28 01:43:59.333533 gdmty-drf-firebase-auth-24.1.1/src/
-drwxr-xr-x   0 niji       (501) staff       (20)        0 2024-01-28 01:43:59.339347 gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth/
--rw-r--r--   0 niji       (501) staff       (20)     1614 2024-01-28 01:43:42.000000 gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth/__init__.py
--rw-r--r--   0 niji       (501) staff       (20)      856 2024-01-28 01:40:35.000000 gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth/admin.py
--rw-r--r--   0 niji       (501) staff       (20)      866 2024-01-28 01:40:35.000000 gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth/apps.py
--rw-r--r--   0 niji       (501) staff       (20)     7977 2024-01-28 01:40:35.000000 gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth/authentication.py
-drwxr-xr-x   0 niji       (501) staff       (20)        0 2024-01-28 01:43:59.341446 gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth/migrations/
--rw-r--r--   0 niji       (501) staff       (20)     1088 2024-01-28 00:48:44.000000 gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth/migrations/0001_initial.py
--rw-r--r--   0 niji       (501) staff       (20)      675 2024-01-28 00:48:44.000000 gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth/migrations/0002_initial.py
--rw-r--r--   0 niji       (501) staff       (20)        0 2024-01-28 00:48:44.000000 gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth/migrations/__init__.py
--rw-r--r--   0 niji       (501) staff       (20)     1709 2024-01-28 01:40:35.000000 gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth/models.py
--rw-r--r--   0 niji       (501) staff       (20)     2612 2024-01-28 01:40:35.000000 gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth/settings.py
--rw-r--r--   0 niji       (501) staff       (20)      725 2024-01-28 01:40:35.000000 gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth/tests.py
--rw-r--r--   0 niji       (501) staff       (20)     2115 2024-01-28 01:40:35.000000 gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth/utils.py
--rw-r--r--   0 niji       (501) staff       (20)      690 2024-01-28 01:40:35.000000 gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth/views.py
-drwxr-xr-x   0 niji       (501) staff       (20)        0 2024-01-28 01:43:59.341637 gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth.egg-info/
--rw-r--r--   0 niji       (501) staff       (20)    19583 2024-01-28 01:43:59.000000 gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth.egg-info/PKG-INFO
--rw-r--r--   0 niji       (501) staff       (20)      807 2024-01-28 01:43:59.000000 gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth.egg-info/SOURCES.txt
--rw-r--r--   0 niji       (501) staff       (20)        1 2024-01-28 01:43:59.000000 gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth.egg-info/dependency_links.txt
--rw-r--r--   0 niji       (501) staff       (20)      130 2024-01-28 01:43:59.000000 gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth.egg-info/requires.txt
--rw-r--r--   0 niji       (501) staff       (20)       24 2024-01-28 01:43:59.000000 gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:34.601416 gdmty-drf-firebase-auth-24.4.0/
+-rw-rw-rw-   0        0        0    11552 2024-04-03 19:57:48.000000 gdmty-drf-firebase-auth-24.4.0/LICENSE
+-rw-rw-rw-   0        0        0       51 2024-04-03 19:57:48.000000 gdmty-drf-firebase-auth-24.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    20264 2024-04-03 20:07:34.600329 gdmty-drf-firebase-auth-24.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5806 2024-04-03 19:57:48.000000 gdmty-drf-firebase-auth-24.4.0/README.md
+-rw-rw-rw-   0        0        0     1680 2024-04-03 20:06:59.000000 gdmty-drf-firebase-auth-24.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-03 20:07:34.601416 gdmty-drf-firebase-auth-24.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:34.579399 gdmty-drf-firebase-auth-24.4.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:34.590730 gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth/
+-rw-rw-rw-   0        0        0     1653 2024-04-03 20:06:59.000000 gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth/__init__.py
+-rw-rw-rw-   0        0        0      877 2024-04-03 19:57:48.000000 gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth/admin.py
+-rw-rw-rw-   0        0        0      888 2024-04-03 19:57:48.000000 gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth/apps.py
+-rw-rw-rw-   0        0        0     8423 2024-04-03 20:04:03.000000 gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth/authentication.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:34.597867 gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth/migrations/
+-rw-rw-rw-   0        0        0     1119 2024-04-03 19:57:48.000000 gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      698 2024-04-03 19:57:48.000000 gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth/migrations/0002_initial.py
+-rw-rw-rw-   0        0        0        0 2024-04-03 19:57:48.000000 gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1759 2024-04-03 19:57:48.000000 gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth/models.py
+-rw-rw-rw-   0        0        0     2494 2024-04-03 19:57:48.000000 gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth/settings.py
+-rw-rw-rw-   0        0        0      743 2024-04-03 19:57:48.000000 gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth/tests.py
+-rw-rw-rw-   0        0        0     2184 2024-04-03 19:57:48.000000 gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth/utils.py
+-rw-rw-rw-   0        0        0      705 2024-04-03 19:57:48.000000 gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth/views.py
+drwxrwxrwx   0        0        0        0 2024-04-03 20:07:34.598884 gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth.egg-info/
+-rw-rw-rw-   0        0        0    20264 2024-04-03 20:07:34.000000 gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      807 2024-04-03 20:07:34.000000 gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-03 20:07:34.000000 gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      130 2024-04-03 20:07:34.000000 gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2024-04-03 20:07:34.000000 gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth.egg-info/top_level.txt
```

### Comparing `gdmty-drf-firebase-auth-24.1.1/LICENSE` & `gdmty-drf-firebase-auth-24.4.0/LICENSE`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright 2023 Gobierno de Monterrey
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright 2023 Gobierno de Monterrey
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `gdmty-drf-firebase-auth-24.1.1/PKG-INFO` & `gdmty-drf-firebase-auth-24.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,346 +1,350 @@
-Metadata-Version: 2.1
-Name: gdmty-drf-firebase-auth
-Version: 24.1.1
-Summary: Custom Django Rest Framework authentication backend than can be used with many firebase projects at same time, and storing as local users.
-Author-email: Gobierno de Monterrey <cesar.benjamin@monterrey.gob.mx>
-License:                                  Apache License
-                                   Version 2.0, January 2004
-                                http://www.apache.org/licenses/
-        
-           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-        
-           1. Definitions.
-        
-              "License" shall mean the terms and conditions for use, reproduction,
-              and distribution as defined by Sections 1 through 9 of this document.
-        
-              "Licensor" shall mean the copyright owner or entity authorized by
-              the copyright owner that is granting the License.
-        
-              "Legal Entity" shall mean the union of the acting entity and all
-              other entities that control, are controlled by, or are under common
-              control with that entity. For the purposes of this definition,
-              "control" means (i) the power, direct or indirect, to cause the
-              direction or management of such entity, whether by contract or
-              otherwise, or (ii) ownership of fifty percent (50%) or more of the
-              outstanding shares, or (iii) beneficial ownership of such entity.
-        
-              "You" (or "Your") shall mean an individual or Legal Entity
-              exercising permissions granted by this License.
-        
-              "Source" form shall mean the preferred form for making modifications,
-              including but not limited to software source code, documentation
-              source, and configuration files.
-        
-              "Object" form shall mean any form resulting from mechanical
-              transformation or translation of a Source form, including but
-              not limited to compiled object code, generated documentation,
-              and conversions to other media types.
-        
-              "Work" shall mean the work of authorship, whether in Source or
-              Object form, made available under the License, as indicated by a
-              copyright notice that is included in or attached to the work
-              (an example is provided in the Appendix below).
-        
-              "Derivative Works" shall mean any work, whether in Source or Object
-              form, that is based on (or derived from) the Work and for which the
-              editorial revisions, annotations, elaborations, or other modifications
-              represent, as a whole, an original work of authorship. For the purposes
-              of this License, Derivative Works shall not include works that remain
-              separable from, or merely link (or bind by name) to the interfaces of,
-              the Work and Derivative Works thereof.
-        
-              "Contribution" shall mean any work of authorship, including
-              the original version of the Work and any modifications or additions
-              to that Work or Derivative Works thereof, that is intentionally
-              submitted to Licensor for inclusion in the Work by the copyright owner
-              or by an individual or Legal Entity authorized to submit on behalf of
-              the copyright owner. For the purposes of this definition, "submitted"
-              means any form of electronic, verbal, or written communication sent
-              to the Licensor or its representatives, including but not limited to
-              communication on electronic mailing lists, source code control systems,
-              and issue tracking systems that are managed by, or on behalf of, the
-              Licensor for the purpose of discussing and improving the Work, but
-              excluding communication that is conspicuously marked or otherwise
-              designated in writing by the copyright owner as "Not a Contribution."
-        
-              "Contributor" shall mean Licensor and any individual or Legal Entity
-              on behalf of whom a Contribution has been received by Licensor and
-              subsequently incorporated within the Work.
-        
-           2. Grant of Copyright License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              copyright license to reproduce, prepare Derivative Works of,
-              publicly display, publicly perform, sublicense, and distribute the
-              Work and such Derivative Works in Source or Object form.
-        
-           3. Grant of Patent License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              (except as stated in this section) patent license to make, have made,
-              use, offer to sell, sell, import, and otherwise transfer the Work,
-              where such license applies only to those patent claims licensable
-              by such Contributor that are necessarily infringed by their
-              Contribution(s) alone or by combination of their Contribution(s)
-              with the Work to which such Contribution(s) was submitted. If You
-              institute patent litigation against any entity (including a
-              cross-claim or counterclaim in a lawsuit) alleging that the Work
-              or a Contribution incorporated within the Work constitutes direct
-              or contributory patent infringement, then any patent licenses
-              granted to You under this License for that Work shall terminate
-              as of the date such litigation is filed.
-        
-           4. Redistribution. You may reproduce and distribute copies of the
-              Work or Derivative Works thereof in any medium, with or without
-              modifications, and in Source or Object form, provided that You
-              meet the following conditions:
-        
-              (a) You must give any other recipients of the Work or
-                  Derivative Works a copy of this License; and
-        
-              (b) You must cause any modified files to carry prominent notices
-                  stating that You changed the files; and
-        
-              (c) You must retain, in the Source form of any Derivative Works
-                  that You distribute, all copyright, patent, trademark, and
-                  attribution notices from the Source form of the Work,
-                  excluding those notices that do not pertain to any part of
-                  the Derivative Works; and
-        
-              (d) If the Work includes a "NOTICE" text file as part of its
-                  distribution, then any Derivative Works that You distribute must
-                  include a readable copy of the attribution notices contained
-                  within such NOTICE file, excluding those notices that do not
-                  pertain to any part of the Derivative Works, in at least one
-                  of the following places: within a NOTICE text file distributed
-                  as part of the Derivative Works; within the Source form or
-                  documentation, if provided along with the Derivative Works; or,
-                  within a display generated by the Derivative Works, if and
-                  wherever such third-party notices normally appear. The contents
-                  of the NOTICE file are for informational purposes only and
-                  do not modify the License. You may add Your own attribution
-                  notices within Derivative Works that You distribute, alongside
-                  or as an addendum to the NOTICE text from the Work, provided
-                  that such additional attribution notices cannot be construed
-                  as modifying the License.
-        
-              You may add Your own copyright statement to Your modifications and
-              may provide additional or different license terms and conditions
-              for use, reproduction, or distribution of Your modifications, or
-              for any such Derivative Works as a whole, provided Your use,
-              reproduction, and distribution of the Work otherwise complies with
-              the conditions stated in this License.
-        
-           5. Submission of Contributions. Unless You explicitly state otherwise,
-              any Contribution intentionally submitted for inclusion in the Work
-              by You to the Licensor shall be under the terms and conditions of
-              this License, without any additional terms or conditions.
-              Notwithstanding the above, nothing herein shall supersede or modify
-              the terms of any separate license agreement you may have executed
-              with Licensor regarding such Contributions.
-        
-           6. Trademarks. This License does not grant permission to use the trade
-              names, trademarks, service marks, or product names of the Licensor,
-              except as required for reasonable and customary use in describing the
-              origin of the Work and reproducing the content of the NOTICE file.
-        
-           7. Disclaimer of Warranty. Unless required by applicable law or
-              agreed to in writing, Licensor provides the Work (and each
-              Contributor provides its Contributions) on an "AS IS" BASIS,
-              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-              implied, including, without limitation, any warranties or conditions
-              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-              PARTICULAR PURPOSE. You are solely responsible for determining the
-              appropriateness of using or redistributing the Work and assume any
-              risks associated with Your exercise of permissions under this License.
-        
-           8. Limitation of Liability. In no event and under no legal theory,
-              whether in tort (including negligence), contract, or otherwise,
-              unless required by applicable law (such as deliberate and grossly
-              negligent acts) or agreed to in writing, shall any Contributor be
-              liable to You for damages, including any direct, indirect, special,
-              incidental, or consequential damages of any character arising as a
-              result of this License or out of the use or inability to use the
-              Work (including but not limited to damages for loss of goodwill,
-              work stoppage, computer failure or malfunction, or any and all
-              other commercial damages or losses), even if such Contributor
-              has been advised of the possibility of such damages.
-        
-           9. Accepting Warranty or Additional Liability. While redistributing
-              the Work or Derivative Works thereof, You may choose to offer,
-              and charge a fee for, acceptance of support, warranty, indemnity,
-              or other liability obligations and/or rights consistent with this
-              License. However, in accepting such obligations, You may act only
-              on Your own behalf and on Your sole responsibility, not on behalf
-              of any other Contributor, and only if You agree to indemnify,
-              defend, and hold each Contributor harmless for any liability
-              incurred by, or claims asserted against, such Contributor by reason
-              of your accepting any such warranty or additional liability.
-        
-           END OF TERMS AND CONDITIONS
-        
-           APPENDIX: How to apply the Apache License to your work.
-        
-              To apply the Apache License to your work, attach the following
-              boilerplate notice, with the fields enclosed by brackets "[]"
-              replaced with your own identifying information. (Don't include
-              the brackets!)  The text should be enclosed in the appropriate
-              comment syntax for the file format. We also recommend that a
-              file or class name and description of purpose be included on the
-              same "printed page" as the copyright notice for easier
-              identification within third-party archives.
-        
-           Copyright 2023 Gobierno de Monterrey
-        
-           Licensed under the Apache License, Version 2.0 (the "License");
-           you may not use this file except in compliance with the License.
-           You may obtain a copy of the License at
-        
-               http://www.apache.org/licenses/LICENSE-2.0
-        
-           Unless required by applicable law or agreed to in writing, software
-           distributed under the License is distributed on an "AS IS" BASIS,
-           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-           See the License for the specific language governing permissions and
-           limitations under the License.
-        
-Project-URL: Homepage, https://github.com/SIGAMty/gdmty-drf-firebase-auth
-Project-URL: Bug Tracker, https://github.com/SIGAMty/gdmty-drf-firebase-auth/issues
-Keywords: django,firebase,jwt,authentication
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.2
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: django<5.0,>=4.2
-Requires-Dist: firebase-admin
-Requires-Dist: djangorestframework
-Requires-Dist: tomli; python_version < "3.11"
-Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
-Requires-Dist: bumpver; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: pip-tools; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-
-# gdmty-drf-firebase-auth
-
-Firebase backend to receive a user idToken and authenticate via Django REST Framework 
-'authentication.BaseAuthentication'. Optionally, a new local user can be created in the process.
-
-## Requirements
-
-* Python 3
-* Django 4
-* Django Rest Framework 3 
-* Firebase Admin SDK
-
-## Installation
-
-```bash
-$ pip install gdmty-drf-firebase-auth
-```
-
-## Configuration
-
-Add the application to your project's `INSTALLED_APPS` in `settings.py`.
-
-```python
-INSTALLED_APPS = [
-    # ...
-    'gdmty_drf_firebase_auth',
-    ...
-]
-```
-
-### General settings
-
-In your project's `settings.py`, add this to the `REST_FRAMEWORK` configuration. Note that if you want to retain access to the browsable API for locally created users, then you will probably want to keep `rest_framework.authentication.SessionAuthentication` too.
-
-```python
-REST_FRAMEWORK = {
-  # ...
-  'DEFAULT_AUTHENTICATION_CLASSES': [
-    # ...
-    'rest_framework.authentication.SessionAuthentication',  # Optional, better to remove for production
-    'rest_framework.authentication.BasicAuthentication',  # Optional, better to remove for production
-    'gdmty_drf_firebase_auth.authentication.FirebaseAuthentication',
-  ]
-}
-```
-
-The `gdmty_drf_firebase_auth` application comes with the following settings as default, which can be overridden in your project's `settings.py` file. For convenience, most of these can be conveniently set form environment variables also. Make sure to nest them within `DEFAULT_FIREBASE_AUTH_CONFIG` as below:
-
-```python
-DEFAULT_FIREBASE_AUTH_CONFIG = {
-    # allow creation of new local user in db
-    'FIREBASE_CREATE_LOCAL_USER': True,
-    # attempt to split firebase user.display_name and set local user, first_name and last_name
-    'FIREBASE_ATTEMPT_CREATE_WITH_DISPLAY_NAME': False,
-    # Authorization header prefix, commonly JWT or Bearer (e.g. Bearer <token>)
-    'FIREBASE_AUTH_HEADER_PREFIX': 'Bearer',
-    # verify that JWT has not been revoked
-    'FIREBASE_CHECK_JWT_REVOKED': True,
-    # require that firebase user.email_verified is True
-    'FIREBASE_AUTH_EMAIL_VERIFICATION': False,
-    # function should accept firebase_admin.auth.UserRecord as argument and return str
-    'FIREBASE_USERNAME_MAPPING_FUNC': map_firebase_uid_to_username
-}
-```
-
-You can get away with leaving all the settings as default
-
-### Firebase per-project settings
-
-It is required to have GCP service accounts, the original project only supports one; the original code has been modified to allow more than one service account, To configure the service accounts, the following configuration must be added in the `settings.py` file of your project, where each element corresponds to a project and in turn, its respective service account.
-
-`BASE_DIR` is the root of your project, where manage.py lives. We assume that you have a folder called `sa` in the root of your project, and that you have placed your service account keyfiles there. You can change this to wherever you like.
-
-```python
-import os
-BASE_DIR = os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
-
-...
-
-FIREBASE_AUTH_SA_KEYFILES = {
-    'project-1': os.path.join(BASE_DIR, 'sa', 'project-1-keyfile.json'),
-    'project-2': os.path.join(BASE_DIR, 'sa', 'project-2-keyfile.json')
-}
-
-FIREBASE_AUTH_PROJECTS = {
-    {'PROJECT_ID': 'project-1', 'SERVICE_ACCOUNT_KEY': FIREBASE_AUTH_SA_KEYFILES['project-1']},
-    {'PROJECT_ID': 'project-2', 'SERVICE_ACCOUNT_KEY': FIREBASE_AUTH_SA_KEYFILES['project-2']},
-}
-```
-
-Now that you have configured the application, run the migrations so that the Firebase data can be stored.
-
-```bash
-(venv) $ ./manage.py migrate gdmty_drf_firebase_auth
-```
-
-All you need to do now is have your client code handle the Firebase popup/redirect authentication flow, retrieve the idToken from the currentUser (Firebase explains this flow well in their docs: `https://firebase.google.com/docs/auth/admin/verify-id-tokens`), and then use the idToken for the user in an `Authorization` header in requests to your API.
-
-```javascript
-Bearer <token>
-```
-
-Now, all is ready!
-
-## Contributing
-
-* Please raise an issue/feature and name your branch 'feature-n' or 'issue-n', where 'n' is the issue number.
-* If you test this code with a Python version not listed above and all is well, please fork and update the README to include the Python version you used :)
-
-## Additional Notes
-
-* This project is a fork of drf-firebase-auth, which seems no longer maintained. The original project only supports one service account, the original code has been modified to allow more than one service account.
-* The initial proposal of this project had the option of use Firebase Auth with email and password, but this option was removed to keep the project clean and simple, and focused on the use of Firebase Auth with idToken for Django REST Framework.
-* If you are looking for a project that supports Firebase Auth with email and password, you can use our side project: `gdmty-django-firebase-auth-email-password` at https://github.com/SIGAMty/gdmty-django-firebase-auth-email-password
-* I almost always setup Django with a custom user class inheriting from AbstractUser, where I switch the USERNAME_FIELD to be 'email'. This backend is set up to assign a username still anyway, but if there are any issues, please raise them and/or make a pull request to help the community!
+Metadata-Version: 2.1
+Name: gdmty-drf-firebase-auth
+Version: 24.4.0
+Summary: Custom Django Rest Framework authentication backend than can be used with many firebase projects at same time, and storing as local users.
+Author-email: Gobierno de Monterrey <cesar.benjamin@monterrey.gob.mx>
+License:                                  Apache License
+                                   Version 2.0, January 2004
+                                http://www.apache.org/licenses/
+        
+           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+        
+           1. Definitions.
+        
+              "License" shall mean the terms and conditions for use, reproduction,
+              and distribution as defined by Sections 1 through 9 of this document.
+        
+              "Licensor" shall mean the copyright owner or entity authorized by
+              the copyright owner that is granting the License.
+        
+              "Legal Entity" shall mean the union of the acting entity and all
+              other entities that control, are controlled by, or are under common
+              control with that entity. For the purposes of this definition,
+              "control" means (i) the power, direct or indirect, to cause the
+              direction or management of such entity, whether by contract or
+              otherwise, or (ii) ownership of fifty percent (50%) or more of the
+              outstanding shares, or (iii) beneficial ownership of such entity.
+        
+              "You" (or "Your") shall mean an individual or Legal Entity
+              exercising permissions granted by this License.
+        
+              "Source" form shall mean the preferred form for making modifications,
+              including but not limited to software source code, documentation
+              source, and configuration files.
+        
+              "Object" form shall mean any form resulting from mechanical
+              transformation or translation of a Source form, including but
+              not limited to compiled object code, generated documentation,
+              and conversions to other media types.
+        
+              "Work" shall mean the work of authorship, whether in Source or
+              Object form, made available under the License, as indicated by a
+              copyright notice that is included in or attached to the work
+              (an example is provided in the Appendix below).
+        
+              "Derivative Works" shall mean any work, whether in Source or Object
+              form, that is based on (or derived from) the Work and for which the
+              editorial revisions, annotations, elaborations, or other modifications
+              represent, as a whole, an original work of authorship. For the purposes
+              of this License, Derivative Works shall not include works that remain
+              separable from, or merely link (or bind by name) to the interfaces of,
+              the Work and Derivative Works thereof.
+        
+              "Contribution" shall mean any work of authorship, including
+              the original version of the Work and any modifications or additions
+              to that Work or Derivative Works thereof, that is intentionally
+              submitted to Licensor for inclusion in the Work by the copyright owner
+              or by an individual or Legal Entity authorized to submit on behalf of
+              the copyright owner. For the purposes of this definition, "submitted"
+              means any form of electronic, verbal, or written communication sent
+              to the Licensor or its representatives, including but not limited to
+              communication on electronic mailing lists, source code control systems,
+              and issue tracking systems that are managed by, or on behalf of, the
+              Licensor for the purpose of discussing and improving the Work, but
+              excluding communication that is conspicuously marked or otherwise
+              designated in writing by the copyright owner as "Not a Contribution."
+        
+              "Contributor" shall mean Licensor and any individual or Legal Entity
+              on behalf of whom a Contribution has been received by Licensor and
+              subsequently incorporated within the Work.
+        
+           2. Grant of Copyright License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              copyright license to reproduce, prepare Derivative Works of,
+              publicly display, publicly perform, sublicense, and distribute the
+              Work and such Derivative Works in Source or Object form.
+        
+           3. Grant of Patent License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              (except as stated in this section) patent license to make, have made,
+              use, offer to sell, sell, import, and otherwise transfer the Work,
+              where such license applies only to those patent claims licensable
+              by such Contributor that are necessarily infringed by their
+              Contribution(s) alone or by combination of their Contribution(s)
+              with the Work to which such Contribution(s) was submitted. If You
+              institute patent litigation against any entity (including a
+              cross-claim or counterclaim in a lawsuit) alleging that the Work
+              or a Contribution incorporated within the Work constitutes direct
+              or contributory patent infringement, then any patent licenses
+              granted to You under this License for that Work shall terminate
+              as of the date such litigation is filed.
+        
+           4. Redistribution. You may reproduce and distribute copies of the
+              Work or Derivative Works thereof in any medium, with or without
+              modifications, and in Source or Object form, provided that You
+              meet the following conditions:
+        
+              (a) You must give any other recipients of the Work or
+                  Derivative Works a copy of this License; and
+        
+              (b) You must cause any modified files to carry prominent notices
+                  stating that You changed the files; and
+        
+              (c) You must retain, in the Source form of any Derivative Works
+                  that You distribute, all copyright, patent, trademark, and
+                  attribution notices from the Source form of the Work,
+                  excluding those notices that do not pertain to any part of
+                  the Derivative Works; and
+        
+              (d) If the Work includes a "NOTICE" text file as part of its
+                  distribution, then any Derivative Works that You distribute must
+                  include a readable copy of the attribution notices contained
+                  within such NOTICE file, excluding those notices that do not
+                  pertain to any part of the Derivative Works, in at least one
+                  of the following places: within a NOTICE text file distributed
+                  as part of the Derivative Works; within the Source form or
+                  documentation, if provided along with the Derivative Works; or,
+                  within a display generated by the Derivative Works, if and
+                  wherever such third-party notices normally appear. The contents
+                  of the NOTICE file are for informational purposes only and
+                  do not modify the License. You may add Your own attribution
+                  notices within Derivative Works that You distribute, alongside
+                  or as an addendum to the NOTICE text from the Work, provided
+                  that such additional attribution notices cannot be construed
+                  as modifying the License.
+        
+              You may add Your own copyright statement to Your modifications and
+              may provide additional or different license terms and conditions
+              for use, reproduction, or distribution of Your modifications, or
+              for any such Derivative Works as a whole, provided Your use,
+              reproduction, and distribution of the Work otherwise complies with
+              the conditions stated in this License.
+        
+           5. Submission of Contributions. Unless You explicitly state otherwise,
+              any Contribution intentionally submitted for inclusion in the Work
+              by You to the Licensor shall be under the terms and conditions of
+              this License, without any additional terms or conditions.
+              Notwithstanding the above, nothing herein shall supersede or modify
+              the terms of any separate license agreement you may have executed
+              with Licensor regarding such Contributions.
+        
+           6. Trademarks. This License does not grant permission to use the trade
+              names, trademarks, service marks, or product names of the Licensor,
+              except as required for reasonable and customary use in describing the
+              origin of the Work and reproducing the content of the NOTICE file.
+        
+           7. Disclaimer of Warranty. Unless required by applicable law or
+              agreed to in writing, Licensor provides the Work (and each
+              Contributor provides its Contributions) on an "AS IS" BASIS,
+              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+              implied, including, without limitation, any warranties or conditions
+              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+              PARTICULAR PURPOSE. You are solely responsible for determining the
+              appropriateness of using or redistributing the Work and assume any
+              risks associated with Your exercise of permissions under this License.
+        
+           8. Limitation of Liability. In no event and under no legal theory,
+              whether in tort (including negligence), contract, or otherwise,
+              unless required by applicable law (such as deliberate and grossly
+              negligent acts) or agreed to in writing, shall any Contributor be
+              liable to You for damages, including any direct, indirect, special,
+              incidental, or consequential damages of any character arising as a
+              result of this License or out of the use or inability to use the
+              Work (including but not limited to damages for loss of goodwill,
+              work stoppage, computer failure or malfunction, or any and all
+              other commercial damages or losses), even if such Contributor
+              has been advised of the possibility of such damages.
+        
+           9. Accepting Warranty or Additional Liability. While redistributing
+              the Work or Derivative Works thereof, You may choose to offer,
+              and charge a fee for, acceptance of support, warranty, indemnity,
+              or other liability obligations and/or rights consistent with this
+              License. However, in accepting such obligations, You may act only
+              on Your own behalf and on Your sole responsibility, not on behalf
+              of any other Contributor, and only if You agree to indemnify,
+              defend, and hold each Contributor harmless for any liability
+              incurred by, or claims asserted against, such Contributor by reason
+              of your accepting any such warranty or additional liability.
+        
+           END OF TERMS AND CONDITIONS
+        
+           APPENDIX: How to apply the Apache License to your work.
+        
+              To apply the Apache License to your work, attach the following
+              boilerplate notice, with the fields enclosed by brackets "[]"
+              replaced with your own identifying information. (Don't include
+              the brackets!)  The text should be enclosed in the appropriate
+              comment syntax for the file format. We also recommend that a
+              file or class name and description of purpose be included on the
+              same "printed page" as the copyright notice for easier
+              identification within third-party archives.
+        
+           Copyright 2023 Gobierno de Monterrey
+        
+           Licensed under the Apache License, Version 2.0 (the "License");
+           you may not use this file except in compliance with the License.
+           You may obtain a copy of the License at
+        
+               http://www.apache.org/licenses/LICENSE-2.0
+        
+           Unless required by applicable law or agreed to in writing, software
+           distributed under the License is distributed on an "AS IS" BASIS,
+           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+           See the License for the specific language governing permissions and
+           limitations under the License.
+        
+Project-URL: Homepage, https://github.com/SIGAMty/gdmty-drf-firebase-auth
+Project-URL: Bug Tracker, https://github.com/SIGAMty/gdmty-drf-firebase-auth/issues
+Keywords: django,firebase,jwt,authentication
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 4.2
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: django<5.0,>=4.2
+Requires-Dist: firebase-admin
+Requires-Dist: djangorestframework
+Requires-Dist: tomli; python_version < "3.11"
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: bumpver; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: pip-tools; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+
+# gdmty-drf-firebase-auth
+
+Firebase backend to receive a user idToken and authenticate via Django REST Framework 
+'authentication.BaseAuthentication'. Optionally, a new local user can be created in the process. 
+This project is basen on the original work of 
+https://github.com/garyburgmann/drf-firebase-auth but with many own contribs to allow 
+get a few features that don't have the original work, but was not able to make a pull reques or 
+contribs because the use cases can be so specific and  will make breaking changes to original code
+
+## Requirements
+
+* Python 3
+* Django 4
+* Django Rest Framework 3 
+* Firebase Admin SDK
+
+## Installation
+
+```bash
+$ pip install gdmty-drf-firebase-auth
+```
+
+## Configuration
+
+Add the application to your project's `INSTALLED_APPS` in `settings.py`.
+
+```python
+INSTALLED_APPS = [
+    # ...
+    'gdmty_drf_firebase_auth',
+    ...
+]
+```
+
+### General settings
+
+In your project's `settings.py`, add this to the `REST_FRAMEWORK` configuration. Note that if you want to retain access to the browsable API for locally created users, then you will probably want to keep `rest_framework.authentication.SessionAuthentication` too.
+
+```python
+REST_FRAMEWORK = {
+  # ...
+  'DEFAULT_AUTHENTICATION_CLASSES': [
+    # ...
+    'rest_framework.authentication.SessionAuthentication',  # Optional, better to remove for production
+    'rest_framework.authentication.BasicAuthentication',  # Optional, better to remove for production
+    'gdmty_drf_firebase_auth.authentication.FirebaseAuthentication',
+  ]
+}
+```
+
+The `gdmty_drf_firebase_auth` application comes with the following settings as default, which can be overridden in your project's `settings.py` file. For convenience, most of these can be conveniently set form environment variables also. Make sure to nest them within `DEFAULT_FIREBASE_AUTH_CONFIG` as below:
+
+```python
+DEFAULT_FIREBASE_AUTH_CONFIG = {
+    # allow creation of new local user in db
+    'FIREBASE_CREATE_LOCAL_USER': True,
+    # attempt to split firebase user.display_name and set local user, first_name and last_name
+    'FIREBASE_ATTEMPT_CREATE_WITH_DISPLAY_NAME': False,
+    # Authorization header prefix, commonly JWT or Bearer (e.g. Bearer <token>)
+    'FIREBASE_AUTH_HEADER_PREFIX': 'Bearer',
+    # verify that JWT has not been revoked
+    'FIREBASE_CHECK_JWT_REVOKED': True,
+    # require that firebase user.email_verified is True
+    'FIREBASE_AUTH_EMAIL_VERIFICATION': False,
+    # function should accept firebase_admin.auth.UserRecord as argument and return str
+    'FIREBASE_USERNAME_MAPPING_FUNC': map_firebase_uid_to_username
+}
+```
+
+You can get away with leaving all the settings as default
+
+### Firebase per-project settings
+
+It is required to have GCP service accounts, the original project only supports one; the original code has been modified to allow more than one service account, To configure the service accounts, the following configuration must be added in the `settings.py` file of your project, where each element corresponds to a project and in turn, its respective service account.
+
+`BASE_DIR` is the root of your project, where manage.py lives. We assume that you have a folder called `sa` in the root of your project, and that you have placed your service account keyfiles there. You can change this to wherever you like.
+
+```python
+import os
+BASE_DIR = os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
+
+...
+
+FIREBASE_AUTH_SA_KEYFILES = {
+    'project-1': os.path.join(BASE_DIR, 'sa', 'project-1-keyfile.json'),
+    'project-2': os.path.join(BASE_DIR, 'sa', 'project-2-keyfile.json')
+}
+
+FIREBASE_AUTH_PROJECTS = [
+    {'PROJECT_ID': 'project-1', 'SERVICE_ACCOUNT_KEY': FIREBASE_AUTH_SA_KEYFILES['project-1']},
+    {'PROJECT_ID': 'project-2', 'SERVICE_ACCOUNT_KEY': FIREBASE_AUTH_SA_KEYFILES['project-2']},
+]
+```
+
+Now that you have configured the application, run the migrations so that the Firebase data can be stored.
+
+```bash
+(venv) $ ./manage.py migrate gdmty_drf_firebase_auth
+```
+
+All you need to do now is have your client code handle the Firebase popup/redirect authentication flow, retrieve the idToken from the currentUser (Firebase explains this flow well in their docs: `https://firebase.google.com/docs/auth/admin/verify-id-tokens`), and then use the idToken for the user in an `Authorization` header in requests to your API.
+
+```javascript
+Bearer <token>
+```
+
+Now, all is ready!
+
+## Contributing
+
+* Please raise an issue/feature and name your branch 'feature-n' or 'issue-n', where 'n' is the issue number.
+* If you test this code with a Python version not listed above and all is well, please fork and update the README to include the Python version you used :)
+
+## Additional Notes
+
+* This project is a fork of drf-firebase-auth, which seems no longer maintained. The original project only supports one service account, the original code has been modified to allow more than one service account.
+* The initial proposal of this project had the option of use Firebase Auth with email and password, but this option was removed to keep the project clean and simple, and focused on the use of Firebase Auth with idToken for Django REST Framework.
+* If you are looking for a project that supports Firebase Auth with email and password, you can use our side project: `gdmty-django-firebase-auth-email-password` at https://github.com/SIGAMty/gdmty-django-firebase-auth-email-password
+* I almost always setup Django with a custom user class inheriting from AbstractUser, where I switch the USERNAME_FIELD to be 'email'. This backend is set up to assign a username still anyway, but if there are any issues, please raise them and/or make a pull request to help the community!
```

### Comparing `gdmty-drf-firebase-auth-24.1.1/README.md` & `gdmty-drf-firebase-auth-24.4.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,115 +1,119 @@
-# gdmty-drf-firebase-auth
-
-Firebase backend to receive a user idToken and authenticate via Django REST Framework 
-'authentication.BaseAuthentication'. Optionally, a new local user can be created in the process.
-
-## Requirements
-
-* Python 3
-* Django 4
-* Django Rest Framework 3 
-* Firebase Admin SDK
-
-## Installation
-
-```bash
-$ pip install gdmty-drf-firebase-auth
-```
-
-## Configuration
-
-Add the application to your project's `INSTALLED_APPS` in `settings.py`.
-
-```python
-INSTALLED_APPS = [
-    # ...
-    'gdmty_drf_firebase_auth',
-    ...
-]
-```
-
-### General settings
-
-In your project's `settings.py`, add this to the `REST_FRAMEWORK` configuration. Note that if you want to retain access to the browsable API for locally created users, then you will probably want to keep `rest_framework.authentication.SessionAuthentication` too.
-
-```python
-REST_FRAMEWORK = {
-  # ...
-  'DEFAULT_AUTHENTICATION_CLASSES': [
-    # ...
-    'rest_framework.authentication.SessionAuthentication',  # Optional, better to remove for production
-    'rest_framework.authentication.BasicAuthentication',  # Optional, better to remove for production
-    'gdmty_drf_firebase_auth.authentication.FirebaseAuthentication',
-  ]
-}
-```
-
-The `gdmty_drf_firebase_auth` application comes with the following settings as default, which can be overridden in your project's `settings.py` file. For convenience, most of these can be conveniently set form environment variables also. Make sure to nest them within `DEFAULT_FIREBASE_AUTH_CONFIG` as below:
-
-```python
-DEFAULT_FIREBASE_AUTH_CONFIG = {
-    # allow creation of new local user in db
-    'FIREBASE_CREATE_LOCAL_USER': True,
-    # attempt to split firebase user.display_name and set local user, first_name and last_name
-    'FIREBASE_ATTEMPT_CREATE_WITH_DISPLAY_NAME': False,
-    # Authorization header prefix, commonly JWT or Bearer (e.g. Bearer <token>)
-    'FIREBASE_AUTH_HEADER_PREFIX': 'Bearer',
-    # verify that JWT has not been revoked
-    'FIREBASE_CHECK_JWT_REVOKED': True,
-    # require that firebase user.email_verified is True
-    'FIREBASE_AUTH_EMAIL_VERIFICATION': False,
-    # function should accept firebase_admin.auth.UserRecord as argument and return str
-    'FIREBASE_USERNAME_MAPPING_FUNC': map_firebase_uid_to_username
-}
-```
-
-You can get away with leaving all the settings as default
-
-### Firebase per-project settings
-
-It is required to have GCP service accounts, the original project only supports one; the original code has been modified to allow more than one service account, To configure the service accounts, the following configuration must be added in the `settings.py` file of your project, where each element corresponds to a project and in turn, its respective service account.
-
-`BASE_DIR` is the root of your project, where manage.py lives. We assume that you have a folder called `sa` in the root of your project, and that you have placed your service account keyfiles there. You can change this to wherever you like.
-
-```python
-import os
-BASE_DIR = os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
-
-...
-
-FIREBASE_AUTH_SA_KEYFILES = {
-    'project-1': os.path.join(BASE_DIR, 'sa', 'project-1-keyfile.json'),
-    'project-2': os.path.join(BASE_DIR, 'sa', 'project-2-keyfile.json')
-}
-
-FIREBASE_AUTH_PROJECTS = {
-    {'PROJECT_ID': 'project-1', 'SERVICE_ACCOUNT_KEY': FIREBASE_AUTH_SA_KEYFILES['project-1']},
-    {'PROJECT_ID': 'project-2', 'SERVICE_ACCOUNT_KEY': FIREBASE_AUTH_SA_KEYFILES['project-2']},
-}
-```
-
-Now that you have configured the application, run the migrations so that the Firebase data can be stored.
-
-```bash
-(venv) $ ./manage.py migrate gdmty_drf_firebase_auth
-```
-
-All you need to do now is have your client code handle the Firebase popup/redirect authentication flow, retrieve the idToken from the currentUser (Firebase explains this flow well in their docs: `https://firebase.google.com/docs/auth/admin/verify-id-tokens`), and then use the idToken for the user in an `Authorization` header in requests to your API.
-
-```javascript
-Bearer <token>
-```
-
-Now, all is ready!
-
-## Contributing
-
-* Please raise an issue/feature and name your branch 'feature-n' or 'issue-n', where 'n' is the issue number.
-* If you test this code with a Python version not listed above and all is well, please fork and update the README to include the Python version you used :)
-
-## Additional Notes
-
-* This project is a fork of drf-firebase-auth, which seems no longer maintained. The original project only supports one service account, the original code has been modified to allow more than one service account.
-* The initial proposal of this project had the option of use Firebase Auth with email and password, but this option was removed to keep the project clean and simple, and focused on the use of Firebase Auth with idToken for Django REST Framework.
-* If you are looking for a project that supports Firebase Auth with email and password, you can use our side project: `gdmty-django-firebase-auth-email-password` at https://github.com/SIGAMty/gdmty-django-firebase-auth-email-password
-* I almost always setup Django with a custom user class inheriting from AbstractUser, where I switch the USERNAME_FIELD to be 'email'. This backend is set up to assign a username still anyway, but if there are any issues, please raise them and/or make a pull request to help the community!
+# gdmty-drf-firebase-auth
+
+Firebase backend to receive a user idToken and authenticate via Django REST Framework 
+'authentication.BaseAuthentication'. Optionally, a new local user can be created in the process. 
+This project is basen on the original work of 
+https://github.com/garyburgmann/drf-firebase-auth but with many own contribs to allow 
+get a few features that don't have the original work, but was not able to make a pull reques or 
+contribs because the use cases can be so specific and  will make breaking changes to original code
+
+## Requirements
+
+* Python 3
+* Django 4
+* Django Rest Framework 3 
+* Firebase Admin SDK
+
+## Installation
+
+```bash
+$ pip install gdmty-drf-firebase-auth
+```
+
+## Configuration
+
+Add the application to your project's `INSTALLED_APPS` in `settings.py`.
+
+```python
+INSTALLED_APPS = [
+    # ...
+    'gdmty_drf_firebase_auth',
+    ...
+]
+```
+
+### General settings
+
+In your project's `settings.py`, add this to the `REST_FRAMEWORK` configuration. Note that if you want to retain access to the browsable API for locally created users, then you will probably want to keep `rest_framework.authentication.SessionAuthentication` too.
+
+```python
+REST_FRAMEWORK = {
+  # ...
+  'DEFAULT_AUTHENTICATION_CLASSES': [
+    # ...
+    'rest_framework.authentication.SessionAuthentication',  # Optional, better to remove for production
+    'rest_framework.authentication.BasicAuthentication',  # Optional, better to remove for production
+    'gdmty_drf_firebase_auth.authentication.FirebaseAuthentication',
+  ]
+}
+```
+
+The `gdmty_drf_firebase_auth` application comes with the following settings as default, which can be overridden in your project's `settings.py` file. For convenience, most of these can be conveniently set form environment variables also. Make sure to nest them within `DEFAULT_FIREBASE_AUTH_CONFIG` as below:
+
+```python
+DEFAULT_FIREBASE_AUTH_CONFIG = {
+    # allow creation of new local user in db
+    'FIREBASE_CREATE_LOCAL_USER': True,
+    # attempt to split firebase user.display_name and set local user, first_name and last_name
+    'FIREBASE_ATTEMPT_CREATE_WITH_DISPLAY_NAME': False,
+    # Authorization header prefix, commonly JWT or Bearer (e.g. Bearer <token>)
+    'FIREBASE_AUTH_HEADER_PREFIX': 'Bearer',
+    # verify that JWT has not been revoked
+    'FIREBASE_CHECK_JWT_REVOKED': True,
+    # require that firebase user.email_verified is True
+    'FIREBASE_AUTH_EMAIL_VERIFICATION': False,
+    # function should accept firebase_admin.auth.UserRecord as argument and return str
+    'FIREBASE_USERNAME_MAPPING_FUNC': map_firebase_uid_to_username
+}
+```
+
+You can get away with leaving all the settings as default
+
+### Firebase per-project settings
+
+It is required to have GCP service accounts, the original project only supports one; the original code has been modified to allow more than one service account, To configure the service accounts, the following configuration must be added in the `settings.py` file of your project, where each element corresponds to a project and in turn, its respective service account.
+
+`BASE_DIR` is the root of your project, where manage.py lives. We assume that you have a folder called `sa` in the root of your project, and that you have placed your service account keyfiles there. You can change this to wherever you like.
+
+```python
+import os
+BASE_DIR = os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
+
+...
+
+FIREBASE_AUTH_SA_KEYFILES = {
+    'project-1': os.path.join(BASE_DIR, 'sa', 'project-1-keyfile.json'),
+    'project-2': os.path.join(BASE_DIR, 'sa', 'project-2-keyfile.json')
+}
+
+FIREBASE_AUTH_PROJECTS = [
+    {'PROJECT_ID': 'project-1', 'SERVICE_ACCOUNT_KEY': FIREBASE_AUTH_SA_KEYFILES['project-1']},
+    {'PROJECT_ID': 'project-2', 'SERVICE_ACCOUNT_KEY': FIREBASE_AUTH_SA_KEYFILES['project-2']},
+]
+```
+
+Now that you have configured the application, run the migrations so that the Firebase data can be stored.
+
+```bash
+(venv) $ ./manage.py migrate gdmty_drf_firebase_auth
+```
+
+All you need to do now is have your client code handle the Firebase popup/redirect authentication flow, retrieve the idToken from the currentUser (Firebase explains this flow well in their docs: `https://firebase.google.com/docs/auth/admin/verify-id-tokens`), and then use the idToken for the user in an `Authorization` header in requests to your API.
+
+```javascript
+Bearer <token>
+```
+
+Now, all is ready!
+
+## Contributing
+
+* Please raise an issue/feature and name your branch 'feature-n' or 'issue-n', where 'n' is the issue number.
+* If you test this code with a Python version not listed above and all is well, please fork and update the README to include the Python version you used :)
+
+## Additional Notes
+
+* This project is a fork of drf-firebase-auth, which seems no longer maintained. The original project only supports one service account, the original code has been modified to allow more than one service account.
+* The initial proposal of this project had the option of use Firebase Auth with email and password, but this option was removed to keep the project clean and simple, and focused on the use of Firebase Auth with idToken for Django REST Framework.
+* If you are looking for a project that supports Firebase Auth with email and password, you can use our side project: `gdmty-django-firebase-auth-email-password` at https://github.com/SIGAMty/gdmty-django-firebase-auth-email-password
+* I almost always setup Django with a custom user class inheriting from AbstractUser, where I switch the USERNAME_FIELD to be 'email'. This backend is set up to assign a username still anyway, but if there are any issues, please raise them and/or make a pull request to help the community!
```

### Comparing `gdmty-drf-firebase-auth-24.1.1/pyproject.toml` & `gdmty-drf-firebase-auth-24.4.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-# pyproject.toml
-
-[build-system]
-requires = ["setuptools>=61.0.0", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "gdmty-drf-firebase-auth"
-version = "24.1.1"
-description = "Custom Django Rest Framework authentication backend than can be used with many firebase projects at same time, and storing as local users."
-readme = "README.md"
-authors = [{ name="Gobierno de Monterrey", email="cesar.benjamin@monterrey.gob.mx" }]
-license = { file = "LICENSE" }
-classifiers = [
-    "License :: OSI Approved :: Apache Software License",
-    "Programming Language :: Python",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.10",
-    "Programming Language :: Python :: 3.11",
-    "Framework :: Django",
-    "Framework :: Django :: 4.2",
-]
-keywords = ["django", "firebase", "jwt", "authentication"]
-dependencies = [
-    "django >= 4.2, < 5.0",
-    "firebase-admin",
-    "djangorestframework",
-    "tomli; python_version < '3.11'",
-]
-requires-python = ">=3.10"
-
-[project.optional-dependencies]
-dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
-
-[project.urls]
-"Homepage" = "https://github.com/SIGAMty/gdmty-drf-firebase-auth"
-"Bug Tracker" = "https://github.com/SIGAMty/gdmty-drf-firebase-auth/issues"
-
-[tool.bumpver]
-current_version = "24.1.1"
-version_pattern = "MAJOR.MINOR.PATCH[-PYTAGNUM]"
-commit_message = "bump version {old_version} -> {new_version}"
-tag_message = "{new_version}"
-tag_scope = "default"
-commit = true
-tag = true
-push = true
-
-[tool.bumpver.file_patterns]
-"pyproject.toml" = ['version = "{version}"']
-"src/gdmty_drf_firebase_auth/__init__.py" = ["{version}"]
+# pyproject.toml
+
+[build-system]
+requires = ["setuptools>=61.0.0", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "gdmty-drf-firebase-auth"
+version = "24.4.0"
+description = "Custom Django Rest Framework authentication backend than can be used with many firebase projects at same time, and storing as local users."
+readme = "README.md"
+authors = [{ name="Gobierno de Monterrey", email="cesar.benjamin@monterrey.gob.mx" }]
+license = { file = "LICENSE" }
+classifiers = [
+    "License :: OSI Approved :: Apache Software License",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Framework :: Django",
+    "Framework :: Django :: 4.2",
+]
+keywords = ["django", "firebase", "jwt", "authentication"]
+dependencies = [
+    "django >= 4.2, < 5.0",
+    "firebase-admin",
+    "djangorestframework",
+    "tomli; python_version < '3.11'",
+]
+requires-python = ">=3.10"
+
+[project.optional-dependencies]
+dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
+
+[project.urls]
+"Homepage" = "https://github.com/SIGAMty/gdmty-drf-firebase-auth"
+"Bug Tracker" = "https://github.com/SIGAMty/gdmty-drf-firebase-auth/issues"
+
+[tool.bumpver]
+current_version = "24.4.0"
+version_pattern = "MAJOR.MINOR.PATCH[-PYTAGNUM]"
+commit_message = "bump version {old_version} -> {new_version}"
+tag_message = "{new_version}"
+tag_scope = "default"
+commit = true
+tag = true
+push = true
+
+[tool.bumpver.file_patterns]
+"pyproject.toml" = ['version = "{version}"']
+"src/gdmty_drf_firebase_auth/__init__.py" = ["{version}"]
```

### Comparing `gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth/__init__.py` & `gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-#!-*- coding: utf-8 -*-
-"""
-Authentication backend for handling firebase user.idToken from incoming
-Authorization header, verifying, and locally authenticating
-
-This package are published as free software under the terms of the Apache License, Version 2.0. Is developed by
-Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
-
-Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', ]
-Email: gobiernodigital@monterrey.gob.mx
-GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
-Package: gdmty_drf_firebase_auth
-PyPi: https://pypi.org/project/gdmty-drf-firebase-auth/
-License: Apache 2.0
-
-This package is a fork of drf-firebase-auth
-with some fixes and improvements.
-This package also adds support for login
-with email and password, and also adds support for
-custom user models. And is fully integrated with gdmty-id.
-
-"""
-
-__title__ = 'gdmty_drf_firebase_auth'
-__version__ = '24.1.1'
-__description__ = (
-    'Custom Django Rest Framework authentication backend for '
-    'parsing Firebase uid tokens and storing as local users.'
-    'This package is a fork of django-firebase-auth '
-    'with some fixes and improvements. '
-    'This package also adds support for login '
-    'with email and password, and also adds support for '
-    'custom user models. And is fully integrated with idmty.'
-)
-__url__ = 'https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth'
-__author__ = 'César Benjamín García Martínez'
-__author_email__ = 'mathereall@gmail.com'
-__license__ = 'Apache 2.0'
-VERSION = __version__
+#!-*- coding: utf-8 -*-
+"""
+Authentication backend for handling firebase user.idToken from incoming
+Authorization header, verifying, and locally authenticating
+
+This package are published as free software under the terms of the Apache License, Version 2.0. Is developed by
+Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
+
+Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', ]
+Email: gobiernodigital@monterrey.gob.mx
+GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
+Package: gdmty_drf_firebase_auth
+PyPi: https://pypi.org/project/gdmty-drf-firebase-auth/
+License: Apache 2.0
+
+This package is a fork of drf-firebase-auth
+with some fixes and improvements.
+This package also adds support for login
+with email and password, and also adds support for
+custom user models. And is fully integrated with gdmty-id.
+
+"""
+
+__title__ = 'gdmty_drf_firebase_auth'
+__version__ = '24.4.0'
+__description__ = (
+    'Custom Django Rest Framework authentication backend for '
+    'parsing Firebase uid tokens and storing as local users.'
+    'This package is a fork of django-firebase-auth '
+    'with some fixes and improvements. '
+    'This package also adds support for login '
+    'with email and password, and also adds support for '
+    'custom user models. And is fully integrated with idmty.'
+)
+__url__ = 'https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth'
+__author__ = 'César Benjamín García Martínez'
+__author_email__ = 'mathereall@gmail.com'
+__license__ = 'Apache 2.0'
+VERSION = __version__
```

### Comparing `gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth/admin.py` & `gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth/admin.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-#!-*- coding: utf-8 -*-
-"""
-Authentication backend for handling firebase user.idToken from incoming
-Authorization header, verifying, and locally authenticating
-
-This package are published as free software under the terms of the Apache License, Version 2.0. Is developed by
-Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
-
-Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', ]
-Email: gobiernodigital@monterrey.gob.mx
-GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
-Package: gdmty_drf_firebase_auth
-PyPi: https://pypi.org/project/gdmty-drf-firebase-auth/
-License: Apache 2.0
-"""
-
-from django.contrib import admin
-from .models import FirebaseUser, FirebaseUserProvider
-
-admin.site.register(FirebaseUser)
-admin.site.register(FirebaseUserProvider)
+#!-*- coding: utf-8 -*-
+"""
+Authentication backend for handling firebase user.idToken from incoming
+Authorization header, verifying, and locally authenticating
+
+This package are published as free software under the terms of the Apache License, Version 2.0. Is developed by
+Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
+
+Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', ]
+Email: gobiernodigital@monterrey.gob.mx
+GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
+Package: gdmty_drf_firebase_auth
+PyPi: https://pypi.org/project/gdmty-drf-firebase-auth/
+License: Apache 2.0
+"""
+
+from django.contrib import admin
+from .models import FirebaseUser, FirebaseUserProvider
+
+admin.site.register(FirebaseUser)
+admin.site.register(FirebaseUserProvider)
```

### Comparing `gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth/authentication.py` & `gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth/authentication.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,184 +1,187 @@
-#!-*- coding: utf-8 -*-
-"""
-Authentication backend for handling firebase user.idToken from incoming
-Authorization header, verifying, and locally authenticating
-
-This package are published as free software under the terms of the Apache License, Version 2.0. Is developed by
-Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
-
-Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', ]
-Email: gobiernodigital@monterrey.gob.mx
-GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
-Package: gdmty_drf_firebase_auth
-PyPi: https://pypi.org/project/gdmty-drf-firebase-auth/
-License: Apache 2.0
-"""
-
-from typing import Tuple, Dict
-import logging
-import firebase_admin
-from firebase_admin import auth as firebase_auth
-from django.utils import timezone
-from django.contrib.auth import get_user_model
-from django.contrib.auth.models import AnonymousUser
-from rest_framework import authentication, exceptions
-from django.conf import settings
-from .settings import api_settings
-from .models import FirebaseUser, FirebaseUserProvider
-from .utils import get_firebase_user_email
-from . import __title__
-
-log = logging.getLogger(__title__)
-User = get_user_model()
-
-firebase_instances = {}
-
-for index, project in enumerate(settings.FIREBASE_AUTH_PROJECTS):
-    if index == 0:
-        default_credentials = firebase_admin.credentials.Certificate(project['SERVICE_ACCOUNT_KEY'])
-        firebase_admin.initialize_app(credential=default_credentials)
-    credentials = firebase_admin.credentials.Certificate(project['SERVICE_ACCOUNT_KEY'])
-    firebase_instances[project['PROJECT_ID']] = firebase_admin.initialize_app(credentials, {'projectId': project['PROJECT_ID']}, name=project['PROJECT_ID'])
-
-
-class FirebaseAuthentication(authentication.TokenAuthentication):
-    """
-    Token based authentication using firebase.
-    """
-    keyword = api_settings.FIREBASE_AUTH_HEADER_PREFIX
-    current_firebase_user_app = None
-
-    def authenticate_credentials(self, token: str) -> Tuple[AnonymousUser, Dict]:
-        try:
-            decoded_token = self._decode_token(token)
-            firebase_user = self._authenticate_token(decoded_token)
-            local_user = self._get_or_create_local_user(firebase_user)
-            self._create_local_firebase_user(local_user, firebase_user)
-            return local_user, decoded_token
-        except Exception as e:
-            raise exceptions.AuthenticationFailed(e)
-
-    def _decode_token(self, token: str) -> Dict:
-        """
-        Attempt to verify JWT from Authorization header with Firebase and return the decoded token
-        """
-        for account in settings.FIREBASE_AUTH_PROJECTS:
-            try:
-                self.current_firebase_user_app = firebase_instances[account['PROJECT_ID']]
-                decoded_token = firebase_auth.verify_id_token(token, app=self.current_firebase_user_app, check_revoked=api_settings.FIREBASE_CHECK_JWT_REVOKED)
-                log.info(f'_decode_token - decoded_token: {decoded_token}')
-                return decoded_token
-            except Exception as e:
-                log.error(f'_decode_token - Exception: {e}')
-                # Continuar con el siguiente intento de verificación
-        raise Exception("Invalida AccessToken")
-
-    def _authenticate_token(self, decoded_token: Dict) -> firebase_auth.UserRecord:
-        """ Returns firebase user if token is authenticated """
-        try:
-            uid = decoded_token.get('uid')
-            log.info(f'_authenticate_token - uid: {uid}')
-            firebase_user = firebase_auth.get_user(uid, app=self.current_firebase_user_app)
-            log.info(f'_authenticate_token - firebase_user: {firebase_user}')
-            if api_settings.FIREBASE_AUTH_EMAIL_VERIFICATION:
-                if not firebase_user.email_verified:
-                    raise Exception('Email address of this user has not been verified.')
-            return firebase_user
-        except Exception as e:
-            log.error(f'_authenticate_token - Exception: {e}')
-            raise Exception(e)
-
-    @staticmethod
-    def _get_or_create_local_user(firebase_user: firebase_auth.UserRecord) -> User:
-        """
-        Attempts to return or create a local User from Firebase user data
-        """
-        email = get_firebase_user_email(firebase_user)
-        log.info(f'_get_or_create_local_user - email: {email}')
-        try:
-            user = User.objects.get(email=email)
-            log.info(
-                f'_get_or_create_local_user - user.is_active: {user.is_active}'
-            )
-            if not user.is_active:
-                raise Exception(
-                    'User account is not currently active.'
-                )
-            user.last_login = timezone.now()
-            user.save()
-        except User.DoesNotExist:
-            log.error(
-                f'_get_or_create_local_user - User.DoesNotExist: {email}'
-            )
-            if not api_settings.FIREBASE_CREATE_LOCAL_USER:
-                raise Exception('User is not registered to the application.')
-            username = \
-                api_settings.FIREBASE_USERNAME_MAPPING_FUNC(firebase_user)
-            log.info(
-                f'_get_or_create_local_user - username: {username}'
-            )
-            try:
-                user = User.objects.create_user(
-                    username=username,
-                    email=email
-                )
-                user.last_login = timezone.now()
-                if (
-                        api_settings.FIREBASE_ATTEMPT_CREATE_WITH_DISPLAY_NAME
-                        and firebase_user.display_name is not None
-                ):
-                    display_name = firebase_user.display_name.split(' ')
-                    if len(display_name) == 2:
-                        user.first_name = display_name[0]
-                        user.last_name = display_name[1]
-                user.save()
-            except Exception as e:
-                raise Exception(e)
-        return user
-
-    @staticmethod
-    def _create_local_firebase_user(user: User, firebase_user: firebase_auth.UserRecord):
-        """ Create a local FireBase model if one does not already exist """
-        # pylint: disable=no-member
-        local_firebase_user = FirebaseUser.objects.filter(
-            user=user
-        ).first()
-
-        if not local_firebase_user:
-            new_firebase_user = FirebaseUser(
-                uid=firebase_user.uid,
-                user=user
-            )
-            new_firebase_user.save()
-            local_firebase_user = new_firebase_user
-
-        if local_firebase_user.uid != firebase_user.uid:
-            local_firebase_user.uid = firebase_user.uid
-            local_firebase_user.save()
-
-        # store FirebaseUserProvider data
-        for provider in firebase_user.provider_data:
-            local_provider = FirebaseUserProvider.objects.filter(
-                provider_id=provider.provider_id,
-                firebase_user=local_firebase_user
-            ).first()
-            if not local_provider:
-                new_local_provider = FirebaseUserProvider.objects.create(
-                    provider_id=provider.provider_id,
-                    uid=provider.uid,
-                    firebase_user=local_firebase_user,
-                )
-                new_local_provider.save()
-
-        # catch locally stored providers no longer associated at Firebase
-        local_providers = FirebaseUserProvider.objects.filter(
-            firebase_user=local_firebase_user
-        )
-        if len(local_providers) != len(firebase_user.provider_data):
-            current_providers = \
-                [x.provider_id for x in firebase_user.provider_data]
-            for provider in local_providers:
-                if provider.provider_id not in current_providers:
-                    FirebaseUserProvider.objects.filter(
-                        id=provider.id
-                    ).delete()
+#!-*- coding: utf-8 -*-
+"""
+Authentication backend for handling firebase user.idToken from incoming
+Authorization header, verifying, and locally authenticating
+
+This package are published as free software under the terms of the Apache License, Version 2.0. Is developed by
+Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
+
+Authors: ['Gary Burgmann', 'César Benjamín García Martínez <mathereall@gmail.com>']
+Email: gobierno.digital@monterrey.gob.mx
+GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
+Package: gdmty_drf_firebase_auth
+PyPi: https://pypi.org/project/gdmty-drf-firebase-auth/
+"""
+
+from typing import Tuple, Dict
+import logging
+import firebase_admin
+from firebase_admin import auth as firebase_auth
+from django.utils import timezone
+from django.contrib.auth import get_user_model
+from django.contrib.auth.models import AnonymousUser
+from rest_framework import authentication, exceptions
+from .settings import api_settings
+from django.conf import settings
+from .models import FirebaseUser, FirebaseUserProvider
+from .utils import get_firebase_user_email
+from . import __title__
+import json
+
+log = logging.getLogger(__title__)
+User = get_user_model()
+
+firebase_instances = {}
+
+for index, project in enumerate(api_settings.FIREBASE_AUTH_PROJECTS):
+    print(index, project)
+    if index == 0:
+        default_credentials = firebase_admin.credentials.Certificate(project['SERVICE_ACCOUNT_KEY'])
+        firebase_admin.initialize_app(credential=default_credentials)
+    credentials = firebase_admin.credentials.Certificate(project['SERVICE_ACCOUNT_KEY'])
+    firebase_instances[project['PROJECT_ID']] = firebase_admin.initialize_app(credentials, {'projectId': project['PROJECT_ID']}, name=project['PROJECT_ID'])
+
+class FirebaseAuthentication(authentication.TokenAuthentication):
+    """
+    Token based authentication using firebase.
+    """
+    keyword = api_settings.FIREBASE_AUTH_HEADER_PREFIX
+    current_firebase_user_app = None
+
+    def authenticate_credentials(self, token: str) -> Tuple[AnonymousUser, Dict]:
+        try:
+            decoded_token = self._decode_token(token)
+            firebase_user = self._authenticate_token(decoded_token)
+            local_user = self._get_or_create_local_user(firebase_user)
+            self._create_local_firebase_user(local_user, firebase_user)
+            return local_user, decoded_token
+        except Exception as e:
+            if settings.DEBUG:
+                raise exceptions.AuthenticationFailed(e)
+
+    def _decode_token(self, token: str) -> Dict:
+        """
+        Attempt to verify JWT from Authorization header with Firebase and return the decoded token
+        """
+        for account in api_settings.FIREBASE_AUTH_PROJECTS:
+            try:
+                self.current_firebase_user_app = firebase_instances[account['PROJECT_ID']]
+                decoded_token = firebase_auth.verify_id_token(token, app=self.current_firebase_user_app, check_revoked=api_settings.FIREBASE_CHECK_JWT_REVOKED)
+                log.info(f'_decode_token - decoded_token: {decoded_token}')
+                return decoded_token
+            except Exception as e:
+                log.error(f'_decode_token - Exception: {e}')
+                # Continuar con el siguiente intento de verificación
+        if settings.DEBUG:
+            log.error(f'Invalid AccessToken')
+            raise Exception("Invalid AccessToken")
+
+    def _authenticate_token(self, decoded_token: Dict) -> firebase_auth.UserRecord:
+        """ Returns firebase user if token is authenticated """
+        try:
+            uid = decoded_token.get('uid')
+            log.info(f'_authenticate_token - uid: {uid}')
+            firebase_user = firebase_auth.get_user(uid, app=self.current_firebase_user_app)
+            log.info(f'_authenticate_token - firebase_user: {firebase_user}')
+            if api_settings.FIREBASE_AUTH_EMAIL_VERIFICATION:
+                if not firebase_user.email_verified:
+                    if settings.DEBUG:
+                        raise Exception('Email address of this user has not been verified.')
+            return firebase_user
+        except Exception as e:
+            log.error(f'_authenticate_token - Exception: {e}')
+            if settings.DEBUG:
+                raise Exception(e)
+
+    @staticmethod
+    def _get_or_create_local_user(firebase_user: firebase_auth.UserRecord) -> User:
+        """
+        Attempts to return or create a local User from Firebase user data
+        """
+        email = get_firebase_user_email(firebase_user)
+        log.info(f'_get_or_create_local_user - email: {email}')
+        try:
+            user = User.objects.get(email=email)
+            log.info(
+                f'_get_or_create_local_user - user.is_active: {user.is_active}'
+            )
+            if not user.is_active:
+                if settings.DEBUG:
+                    raise Exception('User account is not currently active.')
+            user.last_login = timezone.now()
+            user.save()
+        except User.DoesNotExist:
+            log.error(
+                f'_get_or_create_local_user - User.DoesNotExist: {email}'
+            )
+            if not api_settings.FIREBASE_CREATE_LOCAL_USER:
+                if settings.DEBUG:
+                    raise Exception('User is not registered to the application.')
+            username = api_settings.FIREBASE_USERNAME_MAPPING_FUNC(firebase_user)
+            log.info(f'_get_or_create_local_user - username: {username}')
+            try:
+                user = User.objects.create_user(
+                    username=username,
+                    email=email
+                )
+                user.last_login = timezone.now()
+                if (
+                        api_settings.FIREBASE_ATTEMPT_CREATE_WITH_DISPLAY_NAME
+                        and firebase_user.display_name is not None
+                ):
+                    display_name = firebase_user.display_name.split(' ')
+                    if len(display_name) == 2:
+                        user.first_name = display_name[0]
+                        user.last_name = display_name[1]
+                user.save()
+            except Exception as e:
+                if settings.DEBUG:
+                    raise Exception(e)
+        return user
+
+    @staticmethod
+    def _create_local_firebase_user(user: User, firebase_user: firebase_auth.UserRecord):
+        """ Create a local FireBase model if one does not already exist """
+        # pylint: disable=no-member
+        local_firebase_user = FirebaseUser.objects.filter(
+            user=user
+        ).first()
+
+        if not local_firebase_user:
+            new_firebase_user = FirebaseUser(
+                uid=firebase_user.uid,
+                user=user
+            )
+            new_firebase_user.save()
+            local_firebase_user = new_firebase_user
+
+        if local_firebase_user.uid != firebase_user.uid:
+            local_firebase_user.uid = firebase_user.uid
+            local_firebase_user.save()
+
+        # store FirebaseUserProvider data
+        for provider in firebase_user.provider_data:
+            local_provider = FirebaseUserProvider.objects.filter(
+                provider_id=provider.provider_id,
+                firebase_user=local_firebase_user
+            ).first()
+            if not local_provider:
+                new_local_provider = FirebaseUserProvider.objects.create(
+                    provider_id=provider.provider_id,
+                    uid=provider.uid,
+                    firebase_user=local_firebase_user,
+                )
+                new_local_provider.save()
+
+        # catch locally stored providers no longer associated at Firebase
+        local_providers = FirebaseUserProvider.objects.filter(
+            firebase_user=local_firebase_user
+        )
+        if len(local_providers) != len(firebase_user.provider_data):
+            current_providers = \
+                [x.provider_id for x in firebase_user.provider_data]
+            for provider in local_providers:
+                if provider.provider_id not in current_providers:
+                    FirebaseUserProvider.objects.filter(
+                        id=provider.id
+                    ).delete()
```

### Comparing `gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth/migrations/0001_initial.py` & `gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth/migrations/0001_initial.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# Generated by Django 4.2.2 on 2023-08-08 22:27
-
-from django.db import migrations, models
-import django.db.models.deletion
-
-
-class Migration(migrations.Migration):
-
-    initial = True
-
-    dependencies = [
-    ]
-
-    operations = [
-        migrations.CreateModel(
-            name='FirebaseUser',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('uid', models.CharField(max_length=191)),
-            ],
-        ),
-        migrations.CreateModel(
-            name='FirebaseUserProvider',
-            fields=[
-                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
-                ('uid', models.CharField(max_length=191)),
-                ('provider_id', models.CharField(max_length=50)),
-                ('firebase_user', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='provider', related_query_name='provider', to='gdmty_drf_firebase_auth.firebaseuser')),
-            ],
-        ),
-    ]
+# Generated by Django 4.2.2 on 2023-08-08 22:27
+
+from django.db import migrations, models
+import django.db.models.deletion
+
+
+class Migration(migrations.Migration):
+
+    initial = True
+
+    dependencies = [
+    ]
+
+    operations = [
+        migrations.CreateModel(
+            name='FirebaseUser',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('uid', models.CharField(max_length=191)),
+            ],
+        ),
+        migrations.CreateModel(
+            name='FirebaseUserProvider',
+            fields=[
+                ('id', models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID')),
+                ('uid', models.CharField(max_length=191)),
+                ('provider_id', models.CharField(max_length=50)),
+                ('firebase_user', models.ForeignKey(on_delete=django.db.models.deletion.CASCADE, related_name='provider', related_query_name='provider', to='gdmty_drf_firebase_auth.firebaseuser')),
+            ],
+        ),
+    ]
```

### Comparing `gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth/models.py` & `gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth/models.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-#!-*- coding: utf-8 -*-
-
-"""
-Authentication backend for handling firebase user.idToken from incoming
-Authorization header, verifying, and locally authenticating
-
-This package are published as free software under the terms of the Apache License, Version 2.0. Is developed by
-Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
-
-This package is a fork of drf-firebase-auth
-    Models for storing the uid of authenticating firebase users and relating them
-    to the local AUTH_USER_MODEL model.
-    Author: Gary Burgmann
-    Email: garyburgmann@gmail.com
-    Location: Springfield QLD, Australia
-    Last update: 2019-02-10
-
-Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', ]
-Email: gobiernodigital@monterrey.gob.mx
-GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
-Package: gdmty_drf_firebase_auth
-PyPi: https://pypi.org/project/gdmty-drf-firebase-auth/
-License: Apache 2.0
-"""
-
-from django.db import models
-from django.conf import settings
-
-
-class FirebaseUser(models.Model):
-    user = models.OneToOneField(
-        settings.AUTH_USER_MODEL,
-        on_delete=models.CASCADE,
-        null=False,
-        related_name='firebase_user',
-        related_query_name='firebase_user',
-    )
-    uid = models.CharField(max_length=191, null=False,)
-
-
-class FirebaseUserProvider(models.Model):
-    firebase_user = models.ForeignKey(
-        'FirebaseUser',
-        on_delete=models.CASCADE,
-        null=False,
-        related_name='provider',
-        related_query_name='provider',
-    )
-    uid = models.CharField(max_length=191, null=False,)
-    provider_id = models.CharField(max_length=50, null=False,)
+#!-*- coding: utf-8 -*-
+
+"""
+Authentication backend for handling firebase user.idToken from incoming
+Authorization header, verifying, and locally authenticating
+
+This package are published as free software under the terms of the Apache License, Version 2.0. Is developed by
+Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
+
+This package is a fork of drf-firebase-auth
+    Models for storing the uid of authenticating firebase users and relating them
+    to the local AUTH_USER_MODEL model.
+    Author: Gary Burgmann
+    Email: garyburgmann@gmail.com
+    Location: Springfield QLD, Australia
+    Last update: 2019-02-10
+
+Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', ]
+Email: gobiernodigital@monterrey.gob.mx
+GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
+Package: gdmty_drf_firebase_auth
+PyPi: https://pypi.org/project/gdmty-drf-firebase-auth/
+License: Apache 2.0
+"""
+
+from django.db import models
+from django.conf import settings
+
+
+class FirebaseUser(models.Model):
+    user = models.OneToOneField(
+        settings.AUTH_USER_MODEL,
+        on_delete=models.CASCADE,
+        null=False,
+        related_name='firebase_user',
+        related_query_name='firebase_user',
+    )
+    uid = models.CharField(max_length=191, null=False,)
+
+
+class FirebaseUserProvider(models.Model):
+    firebase_user = models.ForeignKey(
+        'FirebaseUser',
+        on_delete=models.CASCADE,
+        null=False,
+        related_name='provider',
+        related_query_name='provider',
+    )
+    uid = models.CharField(max_length=191, null=False,)
+    provider_id = models.CharField(max_length=50, null=False,)
```

### Comparing `gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth/settings.py` & `gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth/settings.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,63 +1,49 @@
-#!-*- coding: utf-8 -*-
-"""
-Authentication backend for handling firebase user.idToken from incoming
-Authorization header, verifying, and locally authenticating
-
-This package are published as free software under the terms of the Apache License, Version 2.0. Is developed by
-Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
-
-Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', ]
-Email: gobiernodigital@monterrey.gob.mx
-GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
-Package: gdmty_drf_firebase_auth
-PyPi: https://pypi.org/project/gdmty-drf-firebase-auth/
-License: Apache 2.0
-"""
-
-
-import os
-import ast
-from django.conf import settings
-from rest_framework.settings import APISettings
-from .utils import map_firebase_uid_to_username
-import logging
-from . import __title__
-
-log = logging.getLogger(__title__)
-
-DEFAULT_FIREBASE_AUTH_CONFIG = {
-    # allow creation of new local user in db
-    'FIREBASE_CREATE_LOCAL_USER': True,
-    # attempt to split firebase user.display_name and set local user, first_name and last_name
-    'FIREBASE_ATTEMPT_CREATE_WITH_DISPLAY_NAME': False,
-    # Authorization header prefix, commonly JWT or Bearer (e.g. Bearer <token>)
-    'FIREBASE_AUTH_HEADER_PREFIX': 'Bearer',
-    # verify that JWT has not been revoked
-    'FIREBASE_CHECK_JWT_REVOKED': True,
-    # require that firebase user.email_verified is True
-    'FIREBASE_AUTH_EMAIL_VERIFICATION': False,
-    # function should accept firebase_admin.auth.UserRecord as argument and return str
-    'FIREBASE_USERNAME_MAPPING_FUNC': map_firebase_uid_to_username
-}
-
-env_config = os.getenv('FIREBASE_AUTH_CONFIG', None)
-
-if env_config:
-    try:
-        config = ast.literal_eval(env_config)
-        if isinstance(dict, config):
-            for key, value in config.items():
-                if key in DEFAULT_FIREBASE_AUTH_CONFIG:
-                    DEFAULT_FIREBASE_AUTH_CONFIG[key] = value
-    except Exception as e:
-        log.info(f'FIREBASE_AUTH_CONFIG - Exception: {e}')
-        log.info("FIREBASE_AUTH_CONFIG no se encontró como variables de entorno, se usará la configuración de "
-                 "settings.py de django si se encuentra, en caso contrario se utilizará la configuración "
-                 "predeterminada.")
-
-USER_FIREBASE_AUTH_CONFIG = getattr(settings, 'FIREBASE_AUTH_CONFIG', None)
-
-# List of settings that may be in string import notation. Used only for compatibility.
-IMPORT_STRINGS = ()
-
-api_settings = APISettings(USER_FIREBASE_AUTH_CONFIG, DEFAULT_FIREBASE_AUTH_CONFIG, IMPORT_STRINGS)
+#!-*- coding: utf-8 -*-
+"""
+Authentication backend for handling firebase user.idToken from incoming
+Authorization header, verifying, and locally authenticating
+
+This package are published as free software under the terms of the Apache License, Version 2.0. Is developed by
+Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
+
+Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', ]
+Email: gobiernodigital@monterrey.gob.mx
+GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
+Package: gdmty_drf_firebase_auth
+PyPi: https://pypi.org/project/gdmty-drf-firebase-auth/
+License: Apache 2.0
+"""
+
+import os
+from django.conf import settings
+from rest_framework.settings import APISettings
+from .utils import map_firebase_uid_to_username
+import logging
+from . import __title__
+import json
+
+log = logging.getLogger(__title__)
+
+FIREBASE_AUTH_CONFIG = getattr(settings, 'FIREBASE_AUTH_CONFIG', None)
+
+DEFAULT_FIREBASE_AUTH_CONFIG = {
+    # allow creation of new local user in db
+    'FIREBASE_CREATE_LOCAL_USER': os.getenv('FIREBASE_CREATE_LOCAL_USER', True),
+    # attempt to split firebase user.display_name and set local user, first_name and last_name
+    'FIREBASE_ATTEMPT_CREATE_WITH_DISPLAY_NAME': os.getenv('FIREBASE_ATTEMPT_CREATE_WITH_DISPLAY_NAME',False),
+    # Authorization header prefix, commonly JWT or Bearer (e.g. Bearer <token>)
+    'FIREBASE_AUTH_HEADER_PREFIX': os.getenv('FIREBASE_AUTH_HEADER_PREFIX', 'Bearer'),
+    # verify that JWT has not been revoked
+    'FIREBASE_CHECK_JWT_REVOKED': os.getenv('FIREBASE_CHECK_JWT_REVOKED', True),
+    # require that firebase user.email_verified is True
+    'FIREBASE_AUTH_EMAIL_VERIFICATION': os.getenv('FIREBASE_AUTH_EMAIL_VERIFICATION', False),
+    # function should accept firebase_admin.auth.UserRecord as argument and return str
+    'FIREBASE_USERNAME_MAPPING_FUNC': map_firebase_uid_to_username,
+    # Project ID and Service Account Keyfile JSON: Loads json from env var or gets object from settings
+    'FIREBASE_AUTH_PROJECTS':  json.loads(os.getenv('FIREBASE_AUTH_PROJECTS')) if json.loads(os.getenv('FIREBASE_AUTH_PROJECTS')) else getattr(settings, 'FIREBASE_AUTH_PROJECTS', None),
+}
+
+# List of settings that may be in string import notation. Used only for compatibility.
+IMPORT_STRINGS = ()
+
+api_settings = APISettings(FIREBASE_AUTH_CONFIG, DEFAULT_FIREBASE_AUTH_CONFIG, IMPORT_STRINGS)
```

### Comparing `gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth/tests.py` & `gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth/views.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-#!-*- coding: utf-8 -*-
-"""
-Authentication backend for handling firebase user.idToken from incoming
-Authorization header, verifying, and locally authenticating
-
-This package are published as free software under the terms of the Apache License, Version 2.0. Is developed by
-Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
-
-Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', ]
-Email: gobiernodigital@monterrey.gob.mx
-GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
-Package: gdmty_drf_firebase_auth
-PyPi: https://pypi.org/project/gdmty-drf-firebase-auth/
-License: Apache 2.0
-"""
-
-from django.test import TestCase
-
+#!-*- coding: utf-8 -*-
+"""
+Authentication backend for handling firebase user.idToken from incoming
+Authorization header, verifying, and locally authenticating
+
+This package are published as free software under the terms of the Apache License, Version 2.0. Is developed by
+Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
+
+Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', ]
+Email: gobiernodigital@monterrey.gob.mx
+GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
+Package: gdmty_drf_firebase_auth
+PyPi: https://pypi.org/project/gdmty-drf-firebase-auth/
+License: Apache 2.0
+"""
```

### Comparing `gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth/utils.py` & `gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth/utils.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-#!-*- coding: utf-8 -*-
-"""
-Authentication backend for handling firebase user.idToken from incoming
-Authorization header, verifying, and locally authenticating
-
-This package are published as free software under the terms of the Apache License, Version 2.0. Is developed by
-Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
-
-Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', ]
-Email: gobiernodigital@monterrey.gob.mx
-GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
-Package: gdmty_drf_firebase_auth
-PyPi: https://pypi.org/project/gdmty-drf-firebase-auth/
-License: Apache 2.0
-"""
-
-import uuid
-from firebase_admin import auth
-
-
-def get_firebase_user_email(firebase_user: auth.UserRecord) -> str:
-    try:
-        return (
-            firebase_user.email
-            if firebase_user.email
-            else firebase_user.provider_data[0].email
-        )
-    except Exception as e:
-        raise Exception(e)
-
-
-def map_firebase_to_username_legacy(firebase_user: auth.UserRecord) -> str:
-    try:
-        username = '_'.join(
-            firebase_user.display_name.split(' ')
-            if firebase_user.display_name
-            else str(uuid.uuid4())
-        )
-        return username if len(username) <= 30 else username[:30]
-    except Exception as e:
-        raise Exception(e)
-
-
-def map_firebase_display_name_to_username(firebase_user: auth.UserRecord) -> str:
-    try:
-        return '_'.join(firebase_user.display_name.split(' '))
-    except Exception as e:
-        raise Exception(e)
-
-
-def map_firebase_uid_to_username(firebase_user: auth.UserRecord) -> str:
-    try:
-        return firebase_user.uid
-    except Exception as e:
-        raise Exception(e)
-
-
-def map_firebase_email_to_username(firebase_user: auth.UserRecord) -> str:
-    try:
-        return get_firebase_user_email(firebase_user)
-    except Exception as e:
-        raise Exception(e)
-
-
-def map_uuid_to_username(_: auth.UserRecord) -> str:
-    try:
-        return str(uuid.uuid4())
-    except Exception as e:
-        raise Exception(e)
+#!-*- coding: utf-8 -*-
+"""
+Authentication backend for handling firebase user.idToken from incoming
+Authorization header, verifying, and locally authenticating
+
+This package are published as free software under the terms of the Apache License, Version 2.0. Is developed by
+Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
+
+Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', ]
+Email: gobiernodigital@monterrey.gob.mx
+GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
+Package: gdmty_drf_firebase_auth
+PyPi: https://pypi.org/project/gdmty-drf-firebase-auth/
+License: Apache 2.0
+"""
+
+import uuid
+from firebase_admin import auth
+
+
+def get_firebase_user_email(firebase_user: auth.UserRecord) -> str:
+    try:
+        return (
+            firebase_user.email
+            if firebase_user.email
+            else firebase_user.provider_data[0].email
+        )
+    except Exception as e:
+        raise Exception(e)
+
+
+def map_firebase_to_username_legacy(firebase_user: auth.UserRecord) -> str:
+    try:
+        username = '_'.join(
+            firebase_user.display_name.split(' ')
+            if firebase_user.display_name
+            else str(uuid.uuid4())
+        )
+        return username if len(username) <= 30 else username[:30]
+    except Exception as e:
+        raise Exception(e)
+
+
+def map_firebase_display_name_to_username(firebase_user: auth.UserRecord) -> str:
+    try:
+        return '_'.join(firebase_user.display_name.split(' '))
+    except Exception as e:
+        raise Exception(e)
+
+
+def map_firebase_uid_to_username(firebase_user: auth.UserRecord) -> str:
+    try:
+        return firebase_user.uid
+    except Exception as e:
+        raise Exception(e)
+
+
+def map_firebase_email_to_username(firebase_user: auth.UserRecord) -> str:
+    try:
+        return get_firebase_user_email(firebase_user)
+    except Exception as e:
+        raise Exception(e)
+
+
+def map_uuid_to_username(_: auth.UserRecord) -> str:
+    try:
+        return str(uuid.uuid4())
+    except Exception as e:
+        raise Exception(e)
```

### Comparing `gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth/views.py` & `gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth/tests.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-#!-*- coding: utf-8 -*-
-"""
-Authentication backend for handling firebase user.idToken from incoming
-Authorization header, verifying, and locally authenticating
-
-This package are published as free software under the terms of the Apache License, Version 2.0. Is developed by
-Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
-
-Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', ]
-Email: gobiernodigital@monterrey.gob.mx
-GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
-Package: gdmty_drf_firebase_auth
-PyPi: https://pypi.org/project/gdmty-drf-firebase-auth/
-License: Apache 2.0
-"""
+#!-*- coding: utf-8 -*-
+"""
+Authentication backend for handling firebase user.idToken from incoming
+Authorization header, verifying, and locally authenticating
+
+This package are published as free software under the terms of the Apache License, Version 2.0. Is developed by
+Dirección de Gobierno Digital of the Secretaría de Innovación y Gobierno Abierto of Municipality of Monterrey.
+
+Authors: ['César Benjamín García Martínez <mathereall@gmail.com>', ]
+Email: gobiernodigital@monterrey.gob.mx
+GitHub: https://github.com/gobiernodigitalmonterrey/gdmty-drf-firebase-auth
+Package: gdmty_drf_firebase_auth
+PyPi: https://pypi.org/project/gdmty-drf-firebase-auth/
+License: Apache 2.0
+"""
+
+from django.test import TestCase
+
```

### Comparing `gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth.egg-info/PKG-INFO` & `gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,346 +1,350 @@
-Metadata-Version: 2.1
-Name: gdmty-drf-firebase-auth
-Version: 24.1.1
-Summary: Custom Django Rest Framework authentication backend than can be used with many firebase projects at same time, and storing as local users.
-Author-email: Gobierno de Monterrey <cesar.benjamin@monterrey.gob.mx>
-License:                                  Apache License
-                                   Version 2.0, January 2004
-                                http://www.apache.org/licenses/
-        
-           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-        
-           1. Definitions.
-        
-              "License" shall mean the terms and conditions for use, reproduction,
-              and distribution as defined by Sections 1 through 9 of this document.
-        
-              "Licensor" shall mean the copyright owner or entity authorized by
-              the copyright owner that is granting the License.
-        
-              "Legal Entity" shall mean the union of the acting entity and all
-              other entities that control, are controlled by, or are under common
-              control with that entity. For the purposes of this definition,
-              "control" means (i) the power, direct or indirect, to cause the
-              direction or management of such entity, whether by contract or
-              otherwise, or (ii) ownership of fifty percent (50%) or more of the
-              outstanding shares, or (iii) beneficial ownership of such entity.
-        
-              "You" (or "Your") shall mean an individual or Legal Entity
-              exercising permissions granted by this License.
-        
-              "Source" form shall mean the preferred form for making modifications,
-              including but not limited to software source code, documentation
-              source, and configuration files.
-        
-              "Object" form shall mean any form resulting from mechanical
-              transformation or translation of a Source form, including but
-              not limited to compiled object code, generated documentation,
-              and conversions to other media types.
-        
-              "Work" shall mean the work of authorship, whether in Source or
-              Object form, made available under the License, as indicated by a
-              copyright notice that is included in or attached to the work
-              (an example is provided in the Appendix below).
-        
-              "Derivative Works" shall mean any work, whether in Source or Object
-              form, that is based on (or derived from) the Work and for which the
-              editorial revisions, annotations, elaborations, or other modifications
-              represent, as a whole, an original work of authorship. For the purposes
-              of this License, Derivative Works shall not include works that remain
-              separable from, or merely link (or bind by name) to the interfaces of,
-              the Work and Derivative Works thereof.
-        
-              "Contribution" shall mean any work of authorship, including
-              the original version of the Work and any modifications or additions
-              to that Work or Derivative Works thereof, that is intentionally
-              submitted to Licensor for inclusion in the Work by the copyright owner
-              or by an individual or Legal Entity authorized to submit on behalf of
-              the copyright owner. For the purposes of this definition, "submitted"
-              means any form of electronic, verbal, or written communication sent
-              to the Licensor or its representatives, including but not limited to
-              communication on electronic mailing lists, source code control systems,
-              and issue tracking systems that are managed by, or on behalf of, the
-              Licensor for the purpose of discussing and improving the Work, but
-              excluding communication that is conspicuously marked or otherwise
-              designated in writing by the copyright owner as "Not a Contribution."
-        
-              "Contributor" shall mean Licensor and any individual or Legal Entity
-              on behalf of whom a Contribution has been received by Licensor and
-              subsequently incorporated within the Work.
-        
-           2. Grant of Copyright License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              copyright license to reproduce, prepare Derivative Works of,
-              publicly display, publicly perform, sublicense, and distribute the
-              Work and such Derivative Works in Source or Object form.
-        
-           3. Grant of Patent License. Subject to the terms and conditions of
-              this License, each Contributor hereby grants to You a perpetual,
-              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-              (except as stated in this section) patent license to make, have made,
-              use, offer to sell, sell, import, and otherwise transfer the Work,
-              where such license applies only to those patent claims licensable
-              by such Contributor that are necessarily infringed by their
-              Contribution(s) alone or by combination of their Contribution(s)
-              with the Work to which such Contribution(s) was submitted. If You
-              institute patent litigation against any entity (including a
-              cross-claim or counterclaim in a lawsuit) alleging that the Work
-              or a Contribution incorporated within the Work constitutes direct
-              or contributory patent infringement, then any patent licenses
-              granted to You under this License for that Work shall terminate
-              as of the date such litigation is filed.
-        
-           4. Redistribution. You may reproduce and distribute copies of the
-              Work or Derivative Works thereof in any medium, with or without
-              modifications, and in Source or Object form, provided that You
-              meet the following conditions:
-        
-              (a) You must give any other recipients of the Work or
-                  Derivative Works a copy of this License; and
-        
-              (b) You must cause any modified files to carry prominent notices
-                  stating that You changed the files; and
-        
-              (c) You must retain, in the Source form of any Derivative Works
-                  that You distribute, all copyright, patent, trademark, and
-                  attribution notices from the Source form of the Work,
-                  excluding those notices that do not pertain to any part of
-                  the Derivative Works; and
-        
-              (d) If the Work includes a "NOTICE" text file as part of its
-                  distribution, then any Derivative Works that You distribute must
-                  include a readable copy of the attribution notices contained
-                  within such NOTICE file, excluding those notices that do not
-                  pertain to any part of the Derivative Works, in at least one
-                  of the following places: within a NOTICE text file distributed
-                  as part of the Derivative Works; within the Source form or
-                  documentation, if provided along with the Derivative Works; or,
-                  within a display generated by the Derivative Works, if and
-                  wherever such third-party notices normally appear. The contents
-                  of the NOTICE file are for informational purposes only and
-                  do not modify the License. You may add Your own attribution
-                  notices within Derivative Works that You distribute, alongside
-                  or as an addendum to the NOTICE text from the Work, provided
-                  that such additional attribution notices cannot be construed
-                  as modifying the License.
-        
-              You may add Your own copyright statement to Your modifications and
-              may provide additional or different license terms and conditions
-              for use, reproduction, or distribution of Your modifications, or
-              for any such Derivative Works as a whole, provided Your use,
-              reproduction, and distribution of the Work otherwise complies with
-              the conditions stated in this License.
-        
-           5. Submission of Contributions. Unless You explicitly state otherwise,
-              any Contribution intentionally submitted for inclusion in the Work
-              by You to the Licensor shall be under the terms and conditions of
-              this License, without any additional terms or conditions.
-              Notwithstanding the above, nothing herein shall supersede or modify
-              the terms of any separate license agreement you may have executed
-              with Licensor regarding such Contributions.
-        
-           6. Trademarks. This License does not grant permission to use the trade
-              names, trademarks, service marks, or product names of the Licensor,
-              except as required for reasonable and customary use in describing the
-              origin of the Work and reproducing the content of the NOTICE file.
-        
-           7. Disclaimer of Warranty. Unless required by applicable law or
-              agreed to in writing, Licensor provides the Work (and each
-              Contributor provides its Contributions) on an "AS IS" BASIS,
-              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-              implied, including, without limitation, any warranties or conditions
-              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-              PARTICULAR PURPOSE. You are solely responsible for determining the
-              appropriateness of using or redistributing the Work and assume any
-              risks associated with Your exercise of permissions under this License.
-        
-           8. Limitation of Liability. In no event and under no legal theory,
-              whether in tort (including negligence), contract, or otherwise,
-              unless required by applicable law (such as deliberate and grossly
-              negligent acts) or agreed to in writing, shall any Contributor be
-              liable to You for damages, including any direct, indirect, special,
-              incidental, or consequential damages of any character arising as a
-              result of this License or out of the use or inability to use the
-              Work (including but not limited to damages for loss of goodwill,
-              work stoppage, computer failure or malfunction, or any and all
-              other commercial damages or losses), even if such Contributor
-              has been advised of the possibility of such damages.
-        
-           9. Accepting Warranty or Additional Liability. While redistributing
-              the Work or Derivative Works thereof, You may choose to offer,
-              and charge a fee for, acceptance of support, warranty, indemnity,
-              or other liability obligations and/or rights consistent with this
-              License. However, in accepting such obligations, You may act only
-              on Your own behalf and on Your sole responsibility, not on behalf
-              of any other Contributor, and only if You agree to indemnify,
-              defend, and hold each Contributor harmless for any liability
-              incurred by, or claims asserted against, such Contributor by reason
-              of your accepting any such warranty or additional liability.
-        
-           END OF TERMS AND CONDITIONS
-        
-           APPENDIX: How to apply the Apache License to your work.
-        
-              To apply the Apache License to your work, attach the following
-              boilerplate notice, with the fields enclosed by brackets "[]"
-              replaced with your own identifying information. (Don't include
-              the brackets!)  The text should be enclosed in the appropriate
-              comment syntax for the file format. We also recommend that a
-              file or class name and description of purpose be included on the
-              same "printed page" as the copyright notice for easier
-              identification within third-party archives.
-        
-           Copyright 2023 Gobierno de Monterrey
-        
-           Licensed under the Apache License, Version 2.0 (the "License");
-           you may not use this file except in compliance with the License.
-           You may obtain a copy of the License at
-        
-               http://www.apache.org/licenses/LICENSE-2.0
-        
-           Unless required by applicable law or agreed to in writing, software
-           distributed under the License is distributed on an "AS IS" BASIS,
-           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-           See the License for the specific language governing permissions and
-           limitations under the License.
-        
-Project-URL: Homepage, https://github.com/SIGAMty/gdmty-drf-firebase-auth
-Project-URL: Bug Tracker, https://github.com/SIGAMty/gdmty-drf-firebase-auth/issues
-Keywords: django,firebase,jwt,authentication
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 4.2
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: django<5.0,>=4.2
-Requires-Dist: firebase-admin
-Requires-Dist: djangorestframework
-Requires-Dist: tomli; python_version < "3.11"
-Provides-Extra: dev
-Requires-Dist: black; extra == "dev"
-Requires-Dist: bumpver; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: pip-tools; extra == "dev"
-Requires-Dist: pytest; extra == "dev"
-
-# gdmty-drf-firebase-auth
-
-Firebase backend to receive a user idToken and authenticate via Django REST Framework 
-'authentication.BaseAuthentication'. Optionally, a new local user can be created in the process.
-
-## Requirements
-
-* Python 3
-* Django 4
-* Django Rest Framework 3 
-* Firebase Admin SDK
-
-## Installation
-
-```bash
-$ pip install gdmty-drf-firebase-auth
-```
-
-## Configuration
-
-Add the application to your project's `INSTALLED_APPS` in `settings.py`.
-
-```python
-INSTALLED_APPS = [
-    # ...
-    'gdmty_drf_firebase_auth',
-    ...
-]
-```
-
-### General settings
-
-In your project's `settings.py`, add this to the `REST_FRAMEWORK` configuration. Note that if you want to retain access to the browsable API for locally created users, then you will probably want to keep `rest_framework.authentication.SessionAuthentication` too.
-
-```python
-REST_FRAMEWORK = {
-  # ...
-  'DEFAULT_AUTHENTICATION_CLASSES': [
-    # ...
-    'rest_framework.authentication.SessionAuthentication',  # Optional, better to remove for production
-    'rest_framework.authentication.BasicAuthentication',  # Optional, better to remove for production
-    'gdmty_drf_firebase_auth.authentication.FirebaseAuthentication',
-  ]
-}
-```
-
-The `gdmty_drf_firebase_auth` application comes with the following settings as default, which can be overridden in your project's `settings.py` file. For convenience, most of these can be conveniently set form environment variables also. Make sure to nest them within `DEFAULT_FIREBASE_AUTH_CONFIG` as below:
-
-```python
-DEFAULT_FIREBASE_AUTH_CONFIG = {
-    # allow creation of new local user in db
-    'FIREBASE_CREATE_LOCAL_USER': True,
-    # attempt to split firebase user.display_name and set local user, first_name and last_name
-    'FIREBASE_ATTEMPT_CREATE_WITH_DISPLAY_NAME': False,
-    # Authorization header prefix, commonly JWT or Bearer (e.g. Bearer <token>)
-    'FIREBASE_AUTH_HEADER_PREFIX': 'Bearer',
-    # verify that JWT has not been revoked
-    'FIREBASE_CHECK_JWT_REVOKED': True,
-    # require that firebase user.email_verified is True
-    'FIREBASE_AUTH_EMAIL_VERIFICATION': False,
-    # function should accept firebase_admin.auth.UserRecord as argument and return str
-    'FIREBASE_USERNAME_MAPPING_FUNC': map_firebase_uid_to_username
-}
-```
-
-You can get away with leaving all the settings as default
-
-### Firebase per-project settings
-
-It is required to have GCP service accounts, the original project only supports one; the original code has been modified to allow more than one service account, To configure the service accounts, the following configuration must be added in the `settings.py` file of your project, where each element corresponds to a project and in turn, its respective service account.
-
-`BASE_DIR` is the root of your project, where manage.py lives. We assume that you have a folder called `sa` in the root of your project, and that you have placed your service account keyfiles there. You can change this to wherever you like.
-
-```python
-import os
-BASE_DIR = os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
-
-...
-
-FIREBASE_AUTH_SA_KEYFILES = {
-    'project-1': os.path.join(BASE_DIR, 'sa', 'project-1-keyfile.json'),
-    'project-2': os.path.join(BASE_DIR, 'sa', 'project-2-keyfile.json')
-}
-
-FIREBASE_AUTH_PROJECTS = {
-    {'PROJECT_ID': 'project-1', 'SERVICE_ACCOUNT_KEY': FIREBASE_AUTH_SA_KEYFILES['project-1']},
-    {'PROJECT_ID': 'project-2', 'SERVICE_ACCOUNT_KEY': FIREBASE_AUTH_SA_KEYFILES['project-2']},
-}
-```
-
-Now that you have configured the application, run the migrations so that the Firebase data can be stored.
-
-```bash
-(venv) $ ./manage.py migrate gdmty_drf_firebase_auth
-```
-
-All you need to do now is have your client code handle the Firebase popup/redirect authentication flow, retrieve the idToken from the currentUser (Firebase explains this flow well in their docs: `https://firebase.google.com/docs/auth/admin/verify-id-tokens`), and then use the idToken for the user in an `Authorization` header in requests to your API.
-
-```javascript
-Bearer <token>
-```
-
-Now, all is ready!
-
-## Contributing
-
-* Please raise an issue/feature and name your branch 'feature-n' or 'issue-n', where 'n' is the issue number.
-* If you test this code with a Python version not listed above and all is well, please fork and update the README to include the Python version you used :)
-
-## Additional Notes
-
-* This project is a fork of drf-firebase-auth, which seems no longer maintained. The original project only supports one service account, the original code has been modified to allow more than one service account.
-* The initial proposal of this project had the option of use Firebase Auth with email and password, but this option was removed to keep the project clean and simple, and focused on the use of Firebase Auth with idToken for Django REST Framework.
-* If you are looking for a project that supports Firebase Auth with email and password, you can use our side project: `gdmty-django-firebase-auth-email-password` at https://github.com/SIGAMty/gdmty-django-firebase-auth-email-password
-* I almost always setup Django with a custom user class inheriting from AbstractUser, where I switch the USERNAME_FIELD to be 'email'. This backend is set up to assign a username still anyway, but if there are any issues, please raise them and/or make a pull request to help the community!
+Metadata-Version: 2.1
+Name: gdmty-drf-firebase-auth
+Version: 24.4.0
+Summary: Custom Django Rest Framework authentication backend than can be used with many firebase projects at same time, and storing as local users.
+Author-email: Gobierno de Monterrey <cesar.benjamin@monterrey.gob.mx>
+License:                                  Apache License
+                                   Version 2.0, January 2004
+                                http://www.apache.org/licenses/
+        
+           TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+        
+           1. Definitions.
+        
+              "License" shall mean the terms and conditions for use, reproduction,
+              and distribution as defined by Sections 1 through 9 of this document.
+        
+              "Licensor" shall mean the copyright owner or entity authorized by
+              the copyright owner that is granting the License.
+        
+              "Legal Entity" shall mean the union of the acting entity and all
+              other entities that control, are controlled by, or are under common
+              control with that entity. For the purposes of this definition,
+              "control" means (i) the power, direct or indirect, to cause the
+              direction or management of such entity, whether by contract or
+              otherwise, or (ii) ownership of fifty percent (50%) or more of the
+              outstanding shares, or (iii) beneficial ownership of such entity.
+        
+              "You" (or "Your") shall mean an individual or Legal Entity
+              exercising permissions granted by this License.
+        
+              "Source" form shall mean the preferred form for making modifications,
+              including but not limited to software source code, documentation
+              source, and configuration files.
+        
+              "Object" form shall mean any form resulting from mechanical
+              transformation or translation of a Source form, including but
+              not limited to compiled object code, generated documentation,
+              and conversions to other media types.
+        
+              "Work" shall mean the work of authorship, whether in Source or
+              Object form, made available under the License, as indicated by a
+              copyright notice that is included in or attached to the work
+              (an example is provided in the Appendix below).
+        
+              "Derivative Works" shall mean any work, whether in Source or Object
+              form, that is based on (or derived from) the Work and for which the
+              editorial revisions, annotations, elaborations, or other modifications
+              represent, as a whole, an original work of authorship. For the purposes
+              of this License, Derivative Works shall not include works that remain
+              separable from, or merely link (or bind by name) to the interfaces of,
+              the Work and Derivative Works thereof.
+        
+              "Contribution" shall mean any work of authorship, including
+              the original version of the Work and any modifications or additions
+              to that Work or Derivative Works thereof, that is intentionally
+              submitted to Licensor for inclusion in the Work by the copyright owner
+              or by an individual or Legal Entity authorized to submit on behalf of
+              the copyright owner. For the purposes of this definition, "submitted"
+              means any form of electronic, verbal, or written communication sent
+              to the Licensor or its representatives, including but not limited to
+              communication on electronic mailing lists, source code control systems,
+              and issue tracking systems that are managed by, or on behalf of, the
+              Licensor for the purpose of discussing and improving the Work, but
+              excluding communication that is conspicuously marked or otherwise
+              designated in writing by the copyright owner as "Not a Contribution."
+        
+              "Contributor" shall mean Licensor and any individual or Legal Entity
+              on behalf of whom a Contribution has been received by Licensor and
+              subsequently incorporated within the Work.
+        
+           2. Grant of Copyright License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              copyright license to reproduce, prepare Derivative Works of,
+              publicly display, publicly perform, sublicense, and distribute the
+              Work and such Derivative Works in Source or Object form.
+        
+           3. Grant of Patent License. Subject to the terms and conditions of
+              this License, each Contributor hereby grants to You a perpetual,
+              worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+              (except as stated in this section) patent license to make, have made,
+              use, offer to sell, sell, import, and otherwise transfer the Work,
+              where such license applies only to those patent claims licensable
+              by such Contributor that are necessarily infringed by their
+              Contribution(s) alone or by combination of their Contribution(s)
+              with the Work to which such Contribution(s) was submitted. If You
+              institute patent litigation against any entity (including a
+              cross-claim or counterclaim in a lawsuit) alleging that the Work
+              or a Contribution incorporated within the Work constitutes direct
+              or contributory patent infringement, then any patent licenses
+              granted to You under this License for that Work shall terminate
+              as of the date such litigation is filed.
+        
+           4. Redistribution. You may reproduce and distribute copies of the
+              Work or Derivative Works thereof in any medium, with or without
+              modifications, and in Source or Object form, provided that You
+              meet the following conditions:
+        
+              (a) You must give any other recipients of the Work or
+                  Derivative Works a copy of this License; and
+        
+              (b) You must cause any modified files to carry prominent notices
+                  stating that You changed the files; and
+        
+              (c) You must retain, in the Source form of any Derivative Works
+                  that You distribute, all copyright, patent, trademark, and
+                  attribution notices from the Source form of the Work,
+                  excluding those notices that do not pertain to any part of
+                  the Derivative Works; and
+        
+              (d) If the Work includes a "NOTICE" text file as part of its
+                  distribution, then any Derivative Works that You distribute must
+                  include a readable copy of the attribution notices contained
+                  within such NOTICE file, excluding those notices that do not
+                  pertain to any part of the Derivative Works, in at least one
+                  of the following places: within a NOTICE text file distributed
+                  as part of the Derivative Works; within the Source form or
+                  documentation, if provided along with the Derivative Works; or,
+                  within a display generated by the Derivative Works, if and
+                  wherever such third-party notices normally appear. The contents
+                  of the NOTICE file are for informational purposes only and
+                  do not modify the License. You may add Your own attribution
+                  notices within Derivative Works that You distribute, alongside
+                  or as an addendum to the NOTICE text from the Work, provided
+                  that such additional attribution notices cannot be construed
+                  as modifying the License.
+        
+              You may add Your own copyright statement to Your modifications and
+              may provide additional or different license terms and conditions
+              for use, reproduction, or distribution of Your modifications, or
+              for any such Derivative Works as a whole, provided Your use,
+              reproduction, and distribution of the Work otherwise complies with
+              the conditions stated in this License.
+        
+           5. Submission of Contributions. Unless You explicitly state otherwise,
+              any Contribution intentionally submitted for inclusion in the Work
+              by You to the Licensor shall be under the terms and conditions of
+              this License, without any additional terms or conditions.
+              Notwithstanding the above, nothing herein shall supersede or modify
+              the terms of any separate license agreement you may have executed
+              with Licensor regarding such Contributions.
+        
+           6. Trademarks. This License does not grant permission to use the trade
+              names, trademarks, service marks, or product names of the Licensor,
+              except as required for reasonable and customary use in describing the
+              origin of the Work and reproducing the content of the NOTICE file.
+        
+           7. Disclaimer of Warranty. Unless required by applicable law or
+              agreed to in writing, Licensor provides the Work (and each
+              Contributor provides its Contributions) on an "AS IS" BASIS,
+              WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+              implied, including, without limitation, any warranties or conditions
+              of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+              PARTICULAR PURPOSE. You are solely responsible for determining the
+              appropriateness of using or redistributing the Work and assume any
+              risks associated with Your exercise of permissions under this License.
+        
+           8. Limitation of Liability. In no event and under no legal theory,
+              whether in tort (including negligence), contract, or otherwise,
+              unless required by applicable law (such as deliberate and grossly
+              negligent acts) or agreed to in writing, shall any Contributor be
+              liable to You for damages, including any direct, indirect, special,
+              incidental, or consequential damages of any character arising as a
+              result of this License or out of the use or inability to use the
+              Work (including but not limited to damages for loss of goodwill,
+              work stoppage, computer failure or malfunction, or any and all
+              other commercial damages or losses), even if such Contributor
+              has been advised of the possibility of such damages.
+        
+           9. Accepting Warranty or Additional Liability. While redistributing
+              the Work or Derivative Works thereof, You may choose to offer,
+              and charge a fee for, acceptance of support, warranty, indemnity,
+              or other liability obligations and/or rights consistent with this
+              License. However, in accepting such obligations, You may act only
+              on Your own behalf and on Your sole responsibility, not on behalf
+              of any other Contributor, and only if You agree to indemnify,
+              defend, and hold each Contributor harmless for any liability
+              incurred by, or claims asserted against, such Contributor by reason
+              of your accepting any such warranty or additional liability.
+        
+           END OF TERMS AND CONDITIONS
+        
+           APPENDIX: How to apply the Apache License to your work.
+        
+              To apply the Apache License to your work, attach the following
+              boilerplate notice, with the fields enclosed by brackets "[]"
+              replaced with your own identifying information. (Don't include
+              the brackets!)  The text should be enclosed in the appropriate
+              comment syntax for the file format. We also recommend that a
+              file or class name and description of purpose be included on the
+              same "printed page" as the copyright notice for easier
+              identification within third-party archives.
+        
+           Copyright 2023 Gobierno de Monterrey
+        
+           Licensed under the Apache License, Version 2.0 (the "License");
+           you may not use this file except in compliance with the License.
+           You may obtain a copy of the License at
+        
+               http://www.apache.org/licenses/LICENSE-2.0
+        
+           Unless required by applicable law or agreed to in writing, software
+           distributed under the License is distributed on an "AS IS" BASIS,
+           WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+           See the License for the specific language governing permissions and
+           limitations under the License.
+        
+Project-URL: Homepage, https://github.com/SIGAMty/gdmty-drf-firebase-auth
+Project-URL: Bug Tracker, https://github.com/SIGAMty/gdmty-drf-firebase-auth/issues
+Keywords: django,firebase,jwt,authentication
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 4.2
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: django<5.0,>=4.2
+Requires-Dist: firebase-admin
+Requires-Dist: djangorestframework
+Requires-Dist: tomli; python_version < "3.11"
+Provides-Extra: dev
+Requires-Dist: black; extra == "dev"
+Requires-Dist: bumpver; extra == "dev"
+Requires-Dist: isort; extra == "dev"
+Requires-Dist: pip-tools; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+
+# gdmty-drf-firebase-auth
+
+Firebase backend to receive a user idToken and authenticate via Django REST Framework 
+'authentication.BaseAuthentication'. Optionally, a new local user can be created in the process. 
+This project is basen on the original work of 
+https://github.com/garyburgmann/drf-firebase-auth but with many own contribs to allow 
+get a few features that don't have the original work, but was not able to make a pull reques or 
+contribs because the use cases can be so specific and  will make breaking changes to original code
+
+## Requirements
+
+* Python 3
+* Django 4
+* Django Rest Framework 3 
+* Firebase Admin SDK
+
+## Installation
+
+```bash
+$ pip install gdmty-drf-firebase-auth
+```
+
+## Configuration
+
+Add the application to your project's `INSTALLED_APPS` in `settings.py`.
+
+```python
+INSTALLED_APPS = [
+    # ...
+    'gdmty_drf_firebase_auth',
+    ...
+]
+```
+
+### General settings
+
+In your project's `settings.py`, add this to the `REST_FRAMEWORK` configuration. Note that if you want to retain access to the browsable API for locally created users, then you will probably want to keep `rest_framework.authentication.SessionAuthentication` too.
+
+```python
+REST_FRAMEWORK = {
+  # ...
+  'DEFAULT_AUTHENTICATION_CLASSES': [
+    # ...
+    'rest_framework.authentication.SessionAuthentication',  # Optional, better to remove for production
+    'rest_framework.authentication.BasicAuthentication',  # Optional, better to remove for production
+    'gdmty_drf_firebase_auth.authentication.FirebaseAuthentication',
+  ]
+}
+```
+
+The `gdmty_drf_firebase_auth` application comes with the following settings as default, which can be overridden in your project's `settings.py` file. For convenience, most of these can be conveniently set form environment variables also. Make sure to nest them within `DEFAULT_FIREBASE_AUTH_CONFIG` as below:
+
+```python
+DEFAULT_FIREBASE_AUTH_CONFIG = {
+    # allow creation of new local user in db
+    'FIREBASE_CREATE_LOCAL_USER': True,
+    # attempt to split firebase user.display_name and set local user, first_name and last_name
+    'FIREBASE_ATTEMPT_CREATE_WITH_DISPLAY_NAME': False,
+    # Authorization header prefix, commonly JWT or Bearer (e.g. Bearer <token>)
+    'FIREBASE_AUTH_HEADER_PREFIX': 'Bearer',
+    # verify that JWT has not been revoked
+    'FIREBASE_CHECK_JWT_REVOKED': True,
+    # require that firebase user.email_verified is True
+    'FIREBASE_AUTH_EMAIL_VERIFICATION': False,
+    # function should accept firebase_admin.auth.UserRecord as argument and return str
+    'FIREBASE_USERNAME_MAPPING_FUNC': map_firebase_uid_to_username
+}
+```
+
+You can get away with leaving all the settings as default
+
+### Firebase per-project settings
+
+It is required to have GCP service accounts, the original project only supports one; the original code has been modified to allow more than one service account, To configure the service accounts, the following configuration must be added in the `settings.py` file of your project, where each element corresponds to a project and in turn, its respective service account.
+
+`BASE_DIR` is the root of your project, where manage.py lives. We assume that you have a folder called `sa` in the root of your project, and that you have placed your service account keyfiles there. You can change this to wherever you like.
+
+```python
+import os
+BASE_DIR = os.path.dirname(os.path.dirname(os.path.dirname(os.path.abspath(__file__))))
+
+...
+
+FIREBASE_AUTH_SA_KEYFILES = {
+    'project-1': os.path.join(BASE_DIR, 'sa', 'project-1-keyfile.json'),
+    'project-2': os.path.join(BASE_DIR, 'sa', 'project-2-keyfile.json')
+}
+
+FIREBASE_AUTH_PROJECTS = [
+    {'PROJECT_ID': 'project-1', 'SERVICE_ACCOUNT_KEY': FIREBASE_AUTH_SA_KEYFILES['project-1']},
+    {'PROJECT_ID': 'project-2', 'SERVICE_ACCOUNT_KEY': FIREBASE_AUTH_SA_KEYFILES['project-2']},
+]
+```
+
+Now that you have configured the application, run the migrations so that the Firebase data can be stored.
+
+```bash
+(venv) $ ./manage.py migrate gdmty_drf_firebase_auth
+```
+
+All you need to do now is have your client code handle the Firebase popup/redirect authentication flow, retrieve the idToken from the currentUser (Firebase explains this flow well in their docs: `https://firebase.google.com/docs/auth/admin/verify-id-tokens`), and then use the idToken for the user in an `Authorization` header in requests to your API.
+
+```javascript
+Bearer <token>
+```
+
+Now, all is ready!
+
+## Contributing
+
+* Please raise an issue/feature and name your branch 'feature-n' or 'issue-n', where 'n' is the issue number.
+* If you test this code with a Python version not listed above and all is well, please fork and update the README to include the Python version you used :)
+
+## Additional Notes
+
+* This project is a fork of drf-firebase-auth, which seems no longer maintained. The original project only supports one service account, the original code has been modified to allow more than one service account.
+* The initial proposal of this project had the option of use Firebase Auth with email and password, but this option was removed to keep the project clean and simple, and focused on the use of Firebase Auth with idToken for Django REST Framework.
+* If you are looking for a project that supports Firebase Auth with email and password, you can use our side project: `gdmty-django-firebase-auth-email-password` at https://github.com/SIGAMty/gdmty-django-firebase-auth-email-password
+* I almost always setup Django with a custom user class inheriting from AbstractUser, where I switch the USERNAME_FIELD to be 'email'. This backend is set up to assign a username still anyway, but if there are any issues, please raise them and/or make a pull request to help the community!
```

### Comparing `gdmty-drf-firebase-auth-24.1.1/src/gdmty_drf_firebase_auth.egg-info/SOURCES.txt` & `gdmty-drf-firebase-auth-24.4.0/src/gdmty_drf_firebase_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

